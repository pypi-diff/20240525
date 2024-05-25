# Comparing `tmp/comment_scanner-0.2.tar.gz` & `tmp/comment_scanner-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "comment_scanner-0.2.tar", last modified: Sat May 25 12:14:39 2024, max compression
+gzip compressed data, was "comment_scanner-0.3.tar", last modified: Sat May 25 13:20:55 2024, max compression
```

## Comparing `comment_scanner-0.2.tar` & `comment_scanner-0.3.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-25 12:14:39.092556 comment_scanner-0.2/
--rw-rw-rw-   0        0        0     3729 2024-05-25 12:14:39.092556 comment_scanner-0.2/PKG-INFO
--rw-rw-rw-   0        0        0     3473 2024-05-25 12:12:46.000000 comment_scanner-0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-25 12:14:38.954103 comment_scanner-0.2/comment_scanner/
--rw-rw-rw-   0        0        0       89 2024-05-25 09:29:08.000000 comment_scanner-0.2/comment_scanner/__init__.py
--rw-rw-rw-   0        0        0     3447 2024-05-25 10:45:57.000000 comment_scanner-0.2/comment_scanner/comment_scanner.py
-drwxrwxrwx   0        0        0        0 2024-05-25 12:14:39.084623 comment_scanner-0.2/comment_scanner/parsers/
--rw-rw-rw-   0        0        0        0 2024-02-29 17:55:20.000000 comment_scanner-0.2/comment_scanner/parsers/__init__.py
--rw-rw-rw-   0        0        0     2528 2024-05-25 09:18:31.000000 comment_scanner-0.2/comment_scanner/parsers/c_parser.py
--rw-rw-rw-   0        0        0     1543 2024-05-25 12:13:22.000000 comment_scanner-0.2/comment_scanner/parsers/common.py
--rw-rw-rw-   0        0        0     3643 2024-05-25 09:18:32.000000 comment_scanner-0.2/comment_scanner/parsers/js_parser.py
--rw-rw-rw-   0        0        0     2709 2024-05-25 09:18:33.000000 comment_scanner-0.2/comment_scanner/parsers/python_parser.py
-drwxrwxrwx   0        0        0        0 2024-05-25 12:14:39.035040 comment_scanner-0.2/comment_scanner.egg-info/
--rw-rw-rw-   0        0        0     3729 2024-05-25 12:14:38.000000 comment_scanner-0.2/comment_scanner.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      539 2024-05-25 12:14:38.000000 comment_scanner-0.2/comment_scanner.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-25 12:14:38.000000 comment_scanner-0.2/comment_scanner.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2024-05-25 12:14:38.000000 comment_scanner-0.2/comment_scanner.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-05-25 09:20:36.000000 comment_scanner-0.2/comment_scanner.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       25 2024-05-25 12:14:38.000000 comment_scanner-0.2/comment_scanner.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-25 12:14:38.000000 comment_scanner-0.2/comment_scanner.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-25 12:14:39.092556 comment_scanner-0.2/setup.cfg
--rw-rw-rw-   0        0        0      758 2024-05-25 12:13:59.000000 comment_scanner-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-25 13:20:55.652671 comment_scanner-0.3/
+-rw-rw-rw-   0        0        0     1088 2024-05-25 12:30:33.000000 comment_scanner-0.3/LICENSE
+-rw-rw-rw-   0        0        0       34 2024-05-25 12:29:34.000000 comment_scanner-0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     4526 2024-05-25 13:20:55.652671 comment_scanner-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3952 2024-05-25 13:14:21.000000 comment_scanner-0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-25 13:20:55.598278 comment_scanner-0.3/comment_scanner/
+-rw-rw-rw-   0        0        0       89 2024-05-25 09:29:08.000000 comment_scanner-0.3/comment_scanner/__init__.py
+-rw-rw-rw-   0        0        0     3671 2024-05-25 13:01:16.000000 comment_scanner-0.3/comment_scanner/comment_scanner.py
+drwxrwxrwx   0        0        0        0 2024-05-25 13:20:55.652671 comment_scanner-0.3/comment_scanner/parsers/
+-rw-rw-rw-   0        0        0        0 2024-02-29 17:55:20.000000 comment_scanner-0.3/comment_scanner/parsers/__init__.py
+-rw-rw-rw-   0        0        0     2528 2024-05-25 09:18:31.000000 comment_scanner-0.3/comment_scanner/parsers/c_parser.py
+-rw-rw-rw-   0        0        0     1543 2024-05-25 12:13:22.000000 comment_scanner-0.3/comment_scanner/parsers/common.py
+-rw-rw-rw-   0        0        0     3643 2024-05-25 09:18:32.000000 comment_scanner-0.3/comment_scanner/parsers/js_parser.py
+-rw-rw-rw-   0        0        0     2709 2024-05-25 09:18:33.000000 comment_scanner-0.3/comment_scanner/parsers/python_parser.py
+drwxrwxrwx   0        0        0        0 2024-05-25 13:20:55.636689 comment_scanner-0.3/comment_scanner.egg-info/
+-rw-rw-rw-   0        0        0     4526 2024-05-25 13:20:55.000000 comment_scanner-0.3/comment_scanner.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      559 2024-05-25 13:20:55.000000 comment_scanner-0.3/comment_scanner.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 13:20:55.000000 comment_scanner-0.3/comment_scanner.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2024-05-25 13:20:55.000000 comment_scanner-0.3/comment_scanner.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-25 09:20:36.000000 comment_scanner-0.3/comment_scanner.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       25 2024-05-25 13:20:55.000000 comment_scanner-0.3/comment_scanner.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-25 13:20:55.000000 comment_scanner-0.3/comment_scanner.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-25 13:20:55.652671 comment_scanner-0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1068 2024-05-25 13:20:53.000000 comment_scanner-0.3/setup.py
```

### Comparing `comment_scanner-0.2/PKG-INFO` & `comment_scanner-0.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,64 +1,70 @@
-Metadata-Version: 2.1
-Name: comment_scanner
-Version: 0.2
-Summary: Parse comments from various source code files
-Author: Faiz Alam
-Author-email: mohdfaizalam53@gmail.com
-License: MIT
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-
 
 # Comment Scanner
 
 Comment Scanner is a Python module designed to extract comments from source code files of various types.
+
+## Features
+- **Multi-language Support**: Works with any programming language.
+- **Comment Types**: Supports single-line, in-line and multi-line comments.
+- **Line Numbers**: Provides the line number for each comment found.
+- **CLI Tool**: Fetch comments from a file via the command line.
+
+
 ## Installation
 
 Install comment scanner using pip/pip3.
 
 ```bash
   pip3 install comment_scanner
 ```
-    
-    
-## Usage
-Comment can be fetched from a source code file or from string text. 
+
+
+## API Usage
+Comment can be fetched from a source code file or from string text.
 
 ```python
 import comment_scanner
 
 # to fetch comments from source file
 comment_scanner.fetch_from_file('/path/of/file')
 
 # to fetch comments from string text
 comment_scanner.fetch_from_str('...')
 
 ```
 
 Both the method returns a list of Comment object of the following structure
 ```
-Comment(comment text, line_no, is_multiline) 
+Comment(comment text, line_no, is_multiline)
 ```
 In case of multi-line comment line_no is of List type containing all the line from the start of the comment till the end comment line.
 
-### Mime Type
-Comment scanner uses python-magic module under the hood to find the mime type of a file and it works for most cases. 
+## CLI Usage
+```bash
+comment_scanner <file_path> [-m or --mime <mime_type>]
+```
+- <file_path>: The path to the code file.
+- -m or --mime <mime_type>: (Optional) The MIME type of the file.
+
+
+## Mime Type
+Comment scanner uses python-magic module under the hood to find the mime type of a file and it works for most cases.
 
 But the user can describe the mime type of the string or file by using `mime` parameter. For supported mime-types, refer to the supported programming laguage section.
 
 
 ```python
 import comment_scanner
 
 comment_scanner.fetch_from_file('/path/of/main.py', mime='text/x-python')
 comment_scanner.fetch_from_str('....', mime='text/x-javascript')
 ```
 
-## Example 
+## Example
 Consider `main.py` contains the following code:
 ```python
 import requests
 
 # The API endpoint
 url = "https://jsonplaceholder.typicode.com/posts/1"
 
@@ -67,32 +73,32 @@
 
 # Print the response
 response_json = response.json()
 print(response_json)
 
 """
 {
-    'userId': 1, 
-    'id': 1, 
-    'title': 'sunt aut facere repellat provident occaecati excepturi optio reprehenderit', 
+    'userId': 1,
+    'id': 1,
+    'title': 'sunt aut facere repellat provident occaecati excepturi optio reprehenderit',
     'body': 'quia et suscipit\nsuscipit recusandae consequuntur expedita et cum\nreprehenderit molestiae ut ut quas totam\nnostrum rerum est autem sunt rem eveniet architecto'
 }
 """
 ```
 If we want to parse all the comments present in this file, we can use comment_scanner like this
 
 ```python
 import comment_scanner
 comments = comment_scanner.fetch_from_file('main.py')
 ```
 This returns the following output:
 ```
-[Comment(The API endpoint, 3, False), 
-Comment(A GET request to the API, 6, False), 
-Comment(Print the response, 9, False), 
+[Comment(The API endpoint, 3, False),
+Comment(A GET request to the API, 6, False),
+Comment(Print the response, 9, False),
 Comment({
     'userId': 1,
     'id': 1,
     'title': 'sunt aut facere repellat provident occaecati excepturi optio reprehenderit',
     'body': 'quia et suscipit\nsuscipit recusandae consequuntur expedita et cum\nreprehenderit molestiae ut ut quas totam\nnostrum rerum est autem sunt rem eveniet architecto'
 }, [13, 14, 15, 16, 17, 18, 19, 20], True)]
 ```
@@ -103,28 +109,27 @@
 for comment in comments:
     comment_text.append(comment.text())
 
 print(comment_text)
 ```
 
 ## Supported Programming Language
-Comment scanner currently supports the following source languages. 
+Comment scanner currently supports the following source languages.
 
 | Language |  mime type |
 |-----|--------|
 | c   | text/x-c |
 | c++   | text/x-c++  |
-| C#   | text/x-c# | 
+| C#   | text/x-c# |
 | java   | text/x-java |
 | javascript   | text/x-javascript  |
 | python   | text/x-python |
 | go   | text/x-go |
 
 And more on the way!
 ## Contributing
 
 Contributions are welcome! Please [fork](https://github.com/FaizAlam/comment-scanner/fork) the repository and submit a pull request.
 ## License
 
 License
 This project is licensed under the [MIT](https://choosealicense.com/licenses/mit/) License.
-
```

### Comparing `comment_scanner-0.2/README.md` & `comment_scanner-0.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,54 +1,86 @@
+Metadata-Version: 2.1
+Name: comment_scanner
+Version: 0.3
+Summary: Parse comments from various source code files
+Home-page: https://github.com/FaizAlam/comment-scanner
+Author: Faiz Alam
+Author-email: mohdfaizalam53@gmail.com
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Software Development :: Documentation
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 
 # Comment Scanner
 
 Comment Scanner is a Python module designed to extract comments from source code files of various types.
+
+## Features
+- **Multi-language Support**: Works with any programming language.
+- **Comment Types**: Supports single-line, in-line and multi-line comments.
+- **Line Numbers**: Provides the line number for each comment found.
+- **CLI Tool**: Fetch comments from a file via the command line.
+
+
 ## Installation
 
 Install comment scanner using pip/pip3.
 
 ```bash
   pip3 install comment_scanner
 ```
-    
-    
-## Usage
-Comment can be fetched from a source code file or from string text. 
+
+
+## API Usage
+Comment can be fetched from a source code file or from string text.
 
 ```python
 import comment_scanner
 
 # to fetch comments from source file
 comment_scanner.fetch_from_file('/path/of/file')
 
 # to fetch comments from string text
 comment_scanner.fetch_from_str('...')
 
 ```
 
 Both the method returns a list of Comment object of the following structure
 ```
-Comment(comment text, line_no, is_multiline) 
+Comment(comment text, line_no, is_multiline)
 ```
 In case of multi-line comment line_no is of List type containing all the line from the start of the comment till the end comment line.
 
-### Mime Type
-Comment scanner uses python-magic module under the hood to find the mime type of a file and it works for most cases. 
+## CLI Usage
+```bash
+comment_scanner <file_path> [-m or --mime <mime_type>]
+```
+- <file_path>: The path to the code file.
+- -m or --mime <mime_type>: (Optional) The MIME type of the file.
+
+
+## Mime Type
+Comment scanner uses python-magic module under the hood to find the mime type of a file and it works for most cases.
 
 But the user can describe the mime type of the string or file by using `mime` parameter. For supported mime-types, refer to the supported programming laguage section.
 
 
 ```python
 import comment_scanner
 
 comment_scanner.fetch_from_file('/path/of/main.py', mime='text/x-python')
 comment_scanner.fetch_from_str('....', mime='text/x-javascript')
 ```
 
-## Example 
+## Example
 Consider `main.py` contains the following code:
 ```python
 import requests
 
 # The API endpoint
 url = "https://jsonplaceholder.typicode.com/posts/1"
 
@@ -57,32 +89,32 @@
 
 # Print the response
 response_json = response.json()
 print(response_json)
 
 """
 {
-    'userId': 1, 
-    'id': 1, 
-    'title': 'sunt aut facere repellat provident occaecati excepturi optio reprehenderit', 
+    'userId': 1,
+    'id': 1,
+    'title': 'sunt aut facere repellat provident occaecati excepturi optio reprehenderit',
     'body': 'quia et suscipit\nsuscipit recusandae consequuntur expedita et cum\nreprehenderit molestiae ut ut quas totam\nnostrum rerum est autem sunt rem eveniet architecto'
 }
 """
 ```
 If we want to parse all the comments present in this file, we can use comment_scanner like this
 
 ```python
 import comment_scanner
 comments = comment_scanner.fetch_from_file('main.py')
 ```
 This returns the following output:
 ```
-[Comment(The API endpoint, 3, False), 
-Comment(A GET request to the API, 6, False), 
-Comment(Print the response, 9, False), 
+[Comment(The API endpoint, 3, False),
+Comment(A GET request to the API, 6, False),
+Comment(Print the response, 9, False),
 Comment({
     'userId': 1,
     'id': 1,
     'title': 'sunt aut facere repellat provident occaecati excepturi optio reprehenderit',
     'body': 'quia et suscipit\nsuscipit recusandae consequuntur expedita et cum\nreprehenderit molestiae ut ut quas totam\nnostrum rerum est autem sunt rem eveniet architecto'
 }, [13, 14, 15, 16, 17, 18, 19, 20], True)]
 ```
@@ -93,28 +125,27 @@
 for comment in comments:
     comment_text.append(comment.text())
 
 print(comment_text)
 ```
 
 ## Supported Programming Language
-Comment scanner currently supports the following source languages. 
+Comment scanner currently supports the following source languages.
 
 | Language |  mime type |
 |-----|--------|
 | c   | text/x-c |
 | c++   | text/x-c++  |
-| C#   | text/x-c# | 
+| C#   | text/x-c# |
 | java   | text/x-java |
 | javascript   | text/x-javascript  |
 | python   | text/x-python |
 | go   | text/x-go |
 
 And more on the way!
 ## Contributing
 
 Contributions are welcome! Please [fork](https://github.com/FaizAlam/comment-scanner/fork) the repository and submit a pull request.
 ## License
 
 License
 This project is licensed under the [MIT](https://choosealicense.com/licenses/mit/) License.
-
```

### Comparing `comment_scanner-0.2/comment_scanner/comment_scanner.py` & `comment_scanner-0.3/comment_scanner/comment_scanner.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     """
     if not mime:
         if not has_magic:
             raise ImportError('python-magic was not imported')
         mime = magic.from_file(filename, mime=True)
         if isinstance(mime, bytes):
             mime = mime.decode('utf-8')
-
+    
     if mime not in MIME_MAP:
         raise UnsupportedError(f"Unsupported MIME type {mime}")
 
     with open(filename, 'r', encoding='utf-8') as code:
         try:
             parser = MIME_MAP[mime]
             return parser.extract_comments(code.read())
@@ -97,20 +97,25 @@
 
 
 def main():
     """Extracts comments from files and prints them to stdout"""
     parser = argparse.ArgumentParser(
         description="Extracts comments from files and prints them to stdout"
     )
-    parser.add_argument('filename', nargs='+', help='File to extract comments from')
+    parser.add_argument('filename', nargs='+', help='File to extract comments from', type=str)
+    parser.add_argument('-m','--mime', help='MIME type of file(s) to extract comments from')
+    
     args = parser.parse_args()
 
     for filename in args.filename:
         try:
-            comments = fetch_from_file(filename)
+            if args.mime:
+                comments = fetch_from_file(filename, args.mime)
+            else:
+                comments = fetch_from_file(filename)
             return comments
         except Error as exc:
             sys.stderr.write(str(exc))
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `comment_scanner-0.2/comment_scanner/parsers/c_parser.py` & `comment_scanner-0.3/comment_scanner/parsers/c_parser.py`

 * *Files identical despite different names*

### Comparing `comment_scanner-0.2/comment_scanner/parsers/common.py` & `comment_scanner-0.3/comment_scanner/parsers/common.py`

 * *Files identical despite different names*

### Comparing `comment_scanner-0.2/comment_scanner/parsers/js_parser.py` & `comment_scanner-0.3/comment_scanner/parsers/js_parser.py`

 * *Files identical despite different names*

### Comparing `comment_scanner-0.2/comment_scanner/parsers/python_parser.py` & `comment_scanner-0.3/comment_scanner/parsers/python_parser.py`

 * *Files identical despite different names*

### Comparing `comment_scanner-0.2/comment_scanner.egg-info/PKG-INFO` & `comment_scanner-0.3/comment_scanner.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,64 +1,86 @@
 Metadata-Version: 2.1
 Name: comment-scanner
-Version: 0.2
+Version: 0.3
 Summary: Parse comments from various source code files
+Home-page: https://github.com/FaizAlam/comment-scanner
 Author: Faiz Alam
 Author-email: mohdfaizalam53@gmail.com
-License: MIT
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Software Development :: Documentation
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 
 # Comment Scanner
 
 Comment Scanner is a Python module designed to extract comments from source code files of various types.
+
+## Features
+- **Multi-language Support**: Works with any programming language.
+- **Comment Types**: Supports single-line, in-line and multi-line comments.
+- **Line Numbers**: Provides the line number for each comment found.
+- **CLI Tool**: Fetch comments from a file via the command line.
+
+
 ## Installation
 
 Install comment scanner using pip/pip3.
 
 ```bash
   pip3 install comment_scanner
 ```
-    
-    
-## Usage
-Comment can be fetched from a source code file or from string text. 
+
+
+## API Usage
+Comment can be fetched from a source code file or from string text.
 
 ```python
 import comment_scanner
 
 # to fetch comments from source file
 comment_scanner.fetch_from_file('/path/of/file')
 
 # to fetch comments from string text
 comment_scanner.fetch_from_str('...')
 
 ```
 
 Both the method returns a list of Comment object of the following structure
 ```
-Comment(comment text, line_no, is_multiline) 
+Comment(comment text, line_no, is_multiline)
 ```
 In case of multi-line comment line_no is of List type containing all the line from the start of the comment till the end comment line.
 
-### Mime Type
-Comment scanner uses python-magic module under the hood to find the mime type of a file and it works for most cases. 
+## CLI Usage
+```bash
+comment_scanner <file_path> [-m or --mime <mime_type>]
+```
+- <file_path>: The path to the code file.
+- -m or --mime <mime_type>: (Optional) The MIME type of the file.
+
+
+## Mime Type
+Comment scanner uses python-magic module under the hood to find the mime type of a file and it works for most cases.
 
 But the user can describe the mime type of the string or file by using `mime` parameter. For supported mime-types, refer to the supported programming laguage section.
 
 
 ```python
 import comment_scanner
 
 comment_scanner.fetch_from_file('/path/of/main.py', mime='text/x-python')
 comment_scanner.fetch_from_str('....', mime='text/x-javascript')
 ```
 
-## Example 
+## Example
 Consider `main.py` contains the following code:
 ```python
 import requests
 
 # The API endpoint
 url = "https://jsonplaceholder.typicode.com/posts/1"
 
@@ -67,32 +89,32 @@
 
 # Print the response
 response_json = response.json()
 print(response_json)
 
 """
 {
-    'userId': 1, 
-    'id': 1, 
-    'title': 'sunt aut facere repellat provident occaecati excepturi optio reprehenderit', 
+    'userId': 1,
+    'id': 1,
+    'title': 'sunt aut facere repellat provident occaecati excepturi optio reprehenderit',
     'body': 'quia et suscipit\nsuscipit recusandae consequuntur expedita et cum\nreprehenderit molestiae ut ut quas totam\nnostrum rerum est autem sunt rem eveniet architecto'
 }
 """
 ```
 If we want to parse all the comments present in this file, we can use comment_scanner like this
 
 ```python
 import comment_scanner
 comments = comment_scanner.fetch_from_file('main.py')
 ```
 This returns the following output:
 ```
-[Comment(The API endpoint, 3, False), 
-Comment(A GET request to the API, 6, False), 
-Comment(Print the response, 9, False), 
+[Comment(The API endpoint, 3, False),
+Comment(A GET request to the API, 6, False),
+Comment(Print the response, 9, False),
 Comment({
     'userId': 1,
     'id': 1,
     'title': 'sunt aut facere repellat provident occaecati excepturi optio reprehenderit',
     'body': 'quia et suscipit\nsuscipit recusandae consequuntur expedita et cum\nreprehenderit molestiae ut ut quas totam\nnostrum rerum est autem sunt rem eveniet architecto'
 }, [13, 14, 15, 16, 17, 18, 19, 20], True)]
 ```
@@ -103,28 +125,27 @@
 for comment in comments:
     comment_text.append(comment.text())
 
 print(comment_text)
 ```
 
 ## Supported Programming Language
-Comment scanner currently supports the following source languages. 
+Comment scanner currently supports the following source languages.
 
 | Language |  mime type |
 |-----|--------|
 | c   | text/x-c |
 | c++   | text/x-c++  |
-| C#   | text/x-c# | 
+| C#   | text/x-c# |
 | java   | text/x-java |
 | javascript   | text/x-javascript  |
 | python   | text/x-python |
 | go   | text/x-go |
 
 And more on the way!
 ## Contributing
 
 Contributions are welcome! Please [fork](https://github.com/FaizAlam/comment-scanner/fork) the repository and submit a pull request.
 ## License
 
 License
 This project is licensed under the [MIT](https://choosealicense.com/licenses/mit/) License.
-
```

### Comparing `comment_scanner-0.2/comment_scanner.egg-info/SOURCES.txt` & `comment_scanner-0.3/comment_scanner.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+LICENSE
+MANIFEST.in
 README.md
 setup.py
 comment_scanner/__init__.py
 comment_scanner/comment_scanner.py
 comment_scanner.egg-info/PKG-INFO
 comment_scanner.egg-info/SOURCES.txt
 comment_scanner.egg-info/dependency_links.txt
```

