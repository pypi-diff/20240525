# Comparing `tmp/dtogen-0.0.8.tar.gz` & `tmp/dtogen-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dtogen-0.0.8.tar", last modified: Wed May 15 19:38:59 2024, max compression
+gzip compressed data, was "dtogen-0.0.9.tar", last modified: Sat May 25 20:59:31 2024, max compression
```

## Comparing `dtogen-0.0.8.tar` & `dtogen-0.0.9.tar`

### file list

```diff
@@ -1,30 +1,32 @@
-drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2024-05-15 19:38:59.631774 dtogen-0.0.8/
--rw-r--r--   0 mujdecisy   (501) staff       (20)     3151 2024-05-15 19:38:59.631315 dtogen-0.0.8/PKG-INFO
--rw-r--r--   0 mujdecisy   (501) staff       (20)     2777 2023-07-20 21:30:14.000000 dtogen-0.0.8/README.md
-drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2024-05-15 19:38:59.625664 dtogen-0.0.8/dtogen/
--rw-r--r--   0 mujdecisy   (501) staff       (20)     1148 2024-05-15 19:30:55.000000 dtogen-0.0.8/dtogen/__main__.py
--rw-r--r--   0 mujdecisy   (501) staff       (20)     1620 2023-07-22 22:11:21.000000 dtogen-0.0.8/dtogen/dtogenerator.py
-drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2024-05-15 19:38:59.628142 dtogen-0.0.8/dtogen/filewriters/
--rw-r--r--   0 mujdecisy   (501) staff       (20)      183 2023-07-22 22:10:45.000000 dtogen-0.0.8/dtogen/filewriters/__init__.py
--rw-r--r--   0 mujdecisy   (501) staff       (20)     2024 2023-07-22 22:12:24.000000 dtogen-0.0.8/dtogen/filewriters/filewriter.py
--rw-r--r--   0 mujdecisy   (501) staff       (20)      567 2023-07-22 22:11:52.000000 dtogen-0.0.8/dtogen/filewriters/filewriter_java.py
--rw-r--r--   0 mujdecisy   (501) staff       (20)      588 2023-07-22 22:12:03.000000 dtogen-0.0.8/dtogen/filewriters/filewriter_python.py
--rw-r--r--   0 mujdecisy   (501) staff       (20)      558 2023-07-22 22:12:15.000000 dtogen-0.0.8/dtogen/filewriters/filewriter_typescript.py
--rw-r--r--   0 mujdecisy   (501) staff       (20)      567 2023-07-20 21:12:11.000000 dtogen-0.0.8/dtogen/interfaces.py
-drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2024-05-15 19:38:59.629958 dtogen-0.0.8/dtogen/transformers/
--rw-r--r--   0 mujdecisy   (501) staff       (20)      191 2023-07-22 22:10:22.000000 dtogen-0.0.8/dtogen/transformers/__init__.py
--rw-r--r--   0 mujdecisy   (501) staff       (20)     4518 2023-07-22 22:12:57.000000 dtogen-0.0.8/dtogen/transformers/transformer.py
--rw-r--r--   0 mujdecisy   (501) staff       (20)      913 2023-07-22 22:11:38.000000 dtogen-0.0.8/dtogen/transformers/transformer_java.py
--rw-r--r--   0 mujdecisy   (501) staff       (20)      805 2023-07-22 22:12:41.000000 dtogen-0.0.8/dtogen/transformers/transformer_python.py
--rw-r--r--   0 mujdecisy   (501) staff       (20)      836 2023-07-22 22:12:49.000000 dtogen-0.0.8/dtogen/transformers/transformer_typescript.py
-drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2024-05-15 19:38:59.631011 dtogen-0.0.8/dtogen.egg-info/
--rw-r--r--   0 mujdecisy   (501) staff       (20)     3151 2024-05-15 19:38:59.000000 dtogen-0.0.8/dtogen.egg-info/PKG-INFO
--rw-r--r--   0 mujdecisy   (501) staff       (20)      660 2024-05-15 19:38:59.000000 dtogen-0.0.8/dtogen.egg-info/SOURCES.txt
--rw-r--r--   0 mujdecisy   (501) staff       (20)        1 2024-05-15 19:38:59.000000 dtogen-0.0.8/dtogen.egg-info/dependency_links.txt
--rw-r--r--   0 mujdecisy   (501) staff       (20)       22 2024-05-15 19:38:59.000000 dtogen-0.0.8/dtogen.egg-info/requires.txt
--rw-r--r--   0 mujdecisy   (501) staff       (20)        7 2024-05-15 19:38:59.000000 dtogen-0.0.8/dtogen.egg-info/top_level.txt
--rw-r--r--   0 mujdecisy   (501) staff       (20)       38 2024-05-15 19:38:59.631922 dtogen-0.0.8/setup.cfg
--rw-r--r--   0 mujdecisy   (501) staff       (20)      741 2024-05-15 19:31:25.000000 dtogen-0.0.8/setup.py
-drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2024-05-15 19:38:59.630601 dtogen-0.0.8/test/
--rw-r--r--   0 mujdecisy   (501) staff       (20)     1195 2023-07-22 06:17:14.000000 dtogen-0.0.8/test/test_dtogenerator.py
--rw-r--r--   0 mujdecisy   (501) staff       (20)     1285 2023-07-22 06:17:14.000000 dtogen-0.0.8/test/test_transform.py
+drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2024-05-25 20:59:31.196550 dtogen-0.0.9/
+-rw-r--r--   0 mujdecisy   (501) staff       (20)     3151 2024-05-25 20:59:31.196245 dtogen-0.0.9/PKG-INFO
+-rw-r--r--   0 mujdecisy   (501) staff       (20)     2777 2023-07-20 21:30:14.000000 dtogen-0.0.9/README.md
+drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2024-05-25 20:59:31.192158 dtogen-0.0.9/dtogen/
+-rw-r--r--   0 mujdecisy   (501) staff       (20)       28 2024-05-25 20:49:40.000000 dtogen-0.0.9/dtogen/__init__.py
+-rw-r--r--   0 mujdecisy   (501) staff       (20)       67 2024-05-25 20:49:17.000000 dtogen-0.0.9/dtogen/__main__.py
+-rw-r--r--   0 mujdecisy   (501) staff       (20)     1620 2024-05-25 20:55:59.000000 dtogen-0.0.9/dtogen/dtogenerator.py
+drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2024-05-25 20:59:31.194073 dtogen-0.0.9/dtogen/filewriters/
+-rw-r--r--   0 mujdecisy   (501) staff       (20)      183 2023-07-22 22:10:45.000000 dtogen-0.0.9/dtogen/filewriters/__init__.py
+-rw-r--r--   0 mujdecisy   (501) staff       (20)     2024 2023-07-22 22:12:24.000000 dtogen-0.0.9/dtogen/filewriters/filewriter.py
+-rw-r--r--   0 mujdecisy   (501) staff       (20)      567 2023-07-22 22:11:52.000000 dtogen-0.0.9/dtogen/filewriters/filewriter_java.py
+-rw-r--r--   0 mujdecisy   (501) staff       (20)      588 2023-07-22 22:12:03.000000 dtogen-0.0.9/dtogen/filewriters/filewriter_python.py
+-rw-r--r--   0 mujdecisy   (501) staff       (20)      558 2023-07-22 22:12:15.000000 dtogen-0.0.9/dtogen/filewriters/filewriter_typescript.py
+-rw-r--r--   0 mujdecisy   (501) staff       (20)      567 2023-07-20 21:12:11.000000 dtogen-0.0.9/dtogen/interfaces.py
+-rw-r--r--   0 mujdecisy   (501) staff       (20)     1207 2024-05-25 20:48:51.000000 dtogen-0.0.9/dtogen/run.py
+drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2024-05-25 20:59:31.195356 dtogen-0.0.9/dtogen/transformers/
+-rw-r--r--   0 mujdecisy   (501) staff       (20)      191 2023-07-22 22:10:22.000000 dtogen-0.0.9/dtogen/transformers/__init__.py
+-rw-r--r--   0 mujdecisy   (501) staff       (20)     4518 2023-07-22 22:12:57.000000 dtogen-0.0.9/dtogen/transformers/transformer.py
+-rw-r--r--   0 mujdecisy   (501) staff       (20)      913 2023-07-22 22:11:38.000000 dtogen-0.0.9/dtogen/transformers/transformer_java.py
+-rw-r--r--   0 mujdecisy   (501) staff       (20)      805 2023-07-22 22:12:41.000000 dtogen-0.0.9/dtogen/transformers/transformer_python.py
+-rw-r--r--   0 mujdecisy   (501) staff       (20)      836 2023-07-22 22:12:49.000000 dtogen-0.0.9/dtogen/transformers/transformer_typescript.py
+drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2024-05-25 20:59:31.195944 dtogen-0.0.9/dtogen.egg-info/
+-rw-r--r--   0 mujdecisy   (501) staff       (20)     3151 2024-05-25 20:59:31.000000 dtogen-0.0.9/dtogen.egg-info/PKG-INFO
+-rw-r--r--   0 mujdecisy   (501) staff       (20)      693 2024-05-25 20:59:31.000000 dtogen-0.0.9/dtogen.egg-info/SOURCES.txt
+-rw-r--r--   0 mujdecisy   (501) staff       (20)        1 2024-05-25 20:59:31.000000 dtogen-0.0.9/dtogen.egg-info/dependency_links.txt
+-rw-r--r--   0 mujdecisy   (501) staff       (20)       22 2024-05-25 20:59:31.000000 dtogen-0.0.9/dtogen.egg-info/requires.txt
+-rw-r--r--   0 mujdecisy   (501) staff       (20)        7 2024-05-25 20:59:31.000000 dtogen-0.0.9/dtogen.egg-info/top_level.txt
+-rw-r--r--   0 mujdecisy   (501) staff       (20)       38 2024-05-25 20:59:31.196605 dtogen-0.0.9/setup.cfg
+-rw-r--r--   0 mujdecisy   (501) staff       (20)      741 2024-05-25 20:59:31.000000 dtogen-0.0.9/setup.py
+drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2024-05-25 20:59:31.195710 dtogen-0.0.9/test/
+-rw-r--r--   0 mujdecisy   (501) staff       (20)     1195 2023-07-22 06:17:14.000000 dtogen-0.0.9/test/test_dtogenerator.py
+-rw-r--r--   0 mujdecisy   (501) staff       (20)     1285 2023-07-22 06:17:14.000000 dtogen-0.0.9/test/test_transform.py
```

### Comparing `dtogen-0.0.8/PKG-INFO` & `dtogen-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtogen
-Version: 0.0.8
+Version: 0.0.9
 Summary: DTO generator for Java, TypeScript, Python
 Home-page: https://github.com/mujdecisy/dtogen
 Author: mujdecisy
 Author-email: mujdecisy@gmail.com
 Keywords: python,DTO,generator
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `dtogen-0.0.8/README.md` & `dtogen-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `dtogen-0.0.8/dtogen/__main__.py` & `dtogen-0.0.9/dtogen/run.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 import argparse
-
 from dtogen.interfaces import DtoGenArgs
 from .dtogenerator import DtoGenerator
 
+def main():
+    arg_parser = argparse.ArgumentParser(description="Generate DTOs from a YAML file")
+    arg_parser.add_argument(
+        "-i", "--input", metavar="INPUT", type=str, required=True, help="input YAML file"
+    )
+    arg_parser.add_argument(
+        "-o", "--output", metavar="OUTPUT", type=str, required=True, help="output directory"
+    )
+    arg_parser.add_argument(
+        "-l",
+        "--lang",
+        metavar="LANG",
+        type=str,
+        required=True,
+        help="output language",
+        choices=["python", "java", "typescript"],
+    )
+    arg_parser.add_argument(
+        "--java-package", metavar="PACKAGE", type=str, help="Java package"
+    )
 
-arg_parser = argparse.ArgumentParser(description="Generate DTOs from a YAML file")
-arg_parser.add_argument(
-    "-i", "--input", metavar="INPUT", type=str, required=True, help="input YAML file"
-)
-arg_parser.add_argument(
-    "-o", "--output", metavar="OUTPUT", type=str, required=True, help="output directory"
-)
-arg_parser.add_argument(
-    "-l",
-    "--lang",
-    metavar="LANG",
-    type=str,
-    required=True,
-    help="output language",
-    choices=["python", "java", "typescript"],
-)
-arg_parser.add_argument(
-    "--java-package", metavar="PACKAGE", type=str, help="Java package"
-)
-
-if __name__ == "__main__":
     args = arg_parser.parse_args()
 
     if args.lang == "java" and not args.java_package:
         arg_parser.error("--java-package is required for java output")
 
     dtogen_args = DtoGenArgs()
     dtogen_args.input_file = args.input
```

### Comparing `dtogen-0.0.8/dtogen/dtogenerator.py` & `dtogen-0.0.9/dtogen/dtogenerator.py`

 * *Files identical despite different names*

### Comparing `dtogen-0.0.8/dtogen/filewriters/filewriter.py` & `dtogen-0.0.9/dtogen/filewriters/filewriter.py`

 * *Files identical despite different names*

### Comparing `dtogen-0.0.8/dtogen/filewriters/filewriter_java.py` & `dtogen-0.0.9/dtogen/filewriters/filewriter_java.py`

 * *Files identical despite different names*

### Comparing `dtogen-0.0.8/dtogen/filewriters/filewriter_python.py` & `dtogen-0.0.9/dtogen/filewriters/filewriter_python.py`

 * *Files identical despite different names*

### Comparing `dtogen-0.0.8/dtogen/filewriters/filewriter_typescript.py` & `dtogen-0.0.9/dtogen/filewriters/filewriter_typescript.py`

 * *Files identical despite different names*

### Comparing `dtogen-0.0.8/dtogen/interfaces.py` & `dtogen-0.0.9/dtogen/interfaces.py`

 * *Files identical despite different names*

### Comparing `dtogen-0.0.8/dtogen/transformers/transformer.py` & `dtogen-0.0.9/dtogen/transformers/transformer.py`

 * *Files identical despite different names*

### Comparing `dtogen-0.0.8/dtogen/transformers/transformer_java.py` & `dtogen-0.0.9/dtogen/transformers/transformer_java.py`

 * *Files identical despite different names*

### Comparing `dtogen-0.0.8/dtogen/transformers/transformer_python.py` & `dtogen-0.0.9/dtogen/transformers/transformer_python.py`

 * *Files identical despite different names*

### Comparing `dtogen-0.0.8/dtogen/transformers/transformer_typescript.py` & `dtogen-0.0.9/dtogen/transformers/transformer_typescript.py`

 * *Files identical despite different names*

### Comparing `dtogen-0.0.8/dtogen.egg-info/PKG-INFO` & `dtogen-0.0.9/dtogen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtogen
-Version: 0.0.8
+Version: 0.0.9
 Summary: DTO generator for Java, TypeScript, Python
 Home-page: https://github.com/mujdecisy/dtogen
 Author: mujdecisy
 Author-email: mujdecisy@gmail.com
 Keywords: python,DTO,generator
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `dtogen-0.0.8/dtogen.egg-info/SOURCES.txt` & `dtogen-0.0.9/dtogen.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 README.md
 setup.py
+dtogen/__init__.py
 dtogen/__main__.py
 dtogen/dtogenerator.py
 dtogen/interfaces.py
+dtogen/run.py
 dtogen.egg-info/PKG-INFO
 dtogen.egg-info/SOURCES.txt
 dtogen.egg-info/dependency_links.txt
 dtogen.egg-info/requires.txt
 dtogen.egg-info/top_level.txt
 dtogen/filewriters/__init__.py
 dtogen/filewriters/filewriter.py
```

### Comparing `dtogen-0.0.8/setup.py` & `dtogen-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 HERE = os.path.abspath(os.path.dirname(__file__))
 
 with open(os.path.join(HERE, "README.md")) as fid:
     README = fid.read()
 
 setup(
     name="dtogen",
-    version="0.0.8",
+    version="0.0.9",
     description="DTO generator for Java, TypeScript, Python",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/mujdecisy/dtogen",
     keywords=["python", "DTO", "generator"],
     author="mujdecisy",
     author_email="mujdecisy@gmail.com",
```

### Comparing `dtogen-0.0.8/test/test_dtogenerator.py` & `dtogen-0.0.9/test/test_dtogenerator.py`

 * *Files identical despite different names*

### Comparing `dtogen-0.0.8/test/test_transform.py` & `dtogen-0.0.9/test/test_transform.py`

 * *Files identical despite different names*

