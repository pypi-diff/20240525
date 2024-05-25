# Comparing `tmp/lexbuilder-1.1.0.tar.gz` & `tmp/LexBuilder-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lexbuilder-1.1.0.tar", last modified: Mon May  6 17:43:03 2024, max compression
+gzip compressed data, was "LexBuilder-1.2.0.tar", last modified: Sat May 25 20:23:14 2024, max compression
```

## Comparing `lexbuilder-1.1.0.tar` & `LexBuilder-1.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 alexander554  (1000) alexander554  (1000)        0 2024-05-06 17:43:03.582765 lexbuilder-1.1.0/
--rw-rw-r--   0 alexander554  (1000) alexander554  (1000)     1096 2024-01-08 18:53:21.000000 lexbuilder-1.1.0/LICENSE
-drwxrwxr-x   0 alexander554  (1000) alexander554  (1000)        0 2024-05-06 17:43:03.579765 lexbuilder-1.1.0/LexBuilder/
--rw-rw-r--   0 alexander554  (1000) alexander554  (1000)     3503 2024-05-06 17:23:53.000000 lexbuilder-1.1.0/LexBuilder/BaseCppLexer.py
--rw-rw-r--   0 alexander554  (1000) alexander554  (1000)     3284 2024-05-06 17:23:53.000000 lexbuilder-1.1.0/LexBuilder/BasePyLexer.py
--rw-rw-r--   0 alexander554  (1000) alexander554  (1000)     3537 2024-05-06 17:39:59.000000 lexbuilder-1.1.0/LexBuilder/Builder.py
--rw-rw-r--   0 alexander554  (1000) alexander554  (1000)      117 2024-05-06 17:21:27.000000 lexbuilder-1.1.0/LexBuilder/__init__.py
-drwxrwxr-x   0 alexander554  (1000) alexander554  (1000)        0 2024-05-06 17:43:03.581765 lexbuilder-1.1.0/LexBuilder.egg-info/
--rw-r--r--   0 alexander554  (1000) alexander554  (1000)     2766 2024-05-06 17:43:03.000000 lexbuilder-1.1.0/LexBuilder.egg-info/PKG-INFO
--rw-rw-r--   0 alexander554  (1000) alexander554  (1000)      270 2024-05-06 17:43:03.000000 lexbuilder-1.1.0/LexBuilder.egg-info/SOURCES.txt
--rw-rw-r--   0 alexander554  (1000) alexander554  (1000)        1 2024-05-06 17:43:03.000000 lexbuilder-1.1.0/LexBuilder.egg-info/dependency_links.txt
--rw-rw-r--   0 alexander554  (1000) alexander554  (1000)       11 2024-05-06 17:43:03.000000 lexbuilder-1.1.0/LexBuilder.egg-info/top_level.txt
--rw-r--r--   0 alexander554  (1000) alexander554  (1000)     2766 2024-05-06 17:43:03.582765 lexbuilder-1.1.0/PKG-INFO
--rw-rw-r--   0 alexander554  (1000) alexander554  (1000)     2337 2024-05-06 17:39:59.000000 lexbuilder-1.1.0/README.md
--rw-rw-r--   0 alexander554  (1000) alexander554  (1000)       38 2024-05-06 17:43:03.582765 lexbuilder-1.1.0/setup.cfg
--rw-rw-r--   0 alexander554  (1000) alexander554  (1000)      634 2024-05-06 17:40:34.000000 lexbuilder-1.1.0/setup.py
+drwxrwxr-x   0 alexander554  (1000) alexander554  (1000)        0 2024-05-25 20:23:14.035749 LexBuilder-1.2.0/
+-rw-rw-r--   0 alexander554  (1000) alexander554  (1000)     1096 2024-01-08 18:53:21.000000 LexBuilder-1.2.0/LICENSE
+drwxrwxr-x   0 alexander554  (1000) alexander554  (1000)        0 2024-05-25 20:23:14.034749 LexBuilder-1.2.0/LexBuilder/
+-rw-rw-r--   0 alexander554  (1000) alexander554  (1000)     3503 2024-05-06 17:23:53.000000 LexBuilder-1.2.0/LexBuilder/BaseCppLexer.py
+-rw-rw-r--   0 alexander554  (1000) alexander554  (1000)     3284 2024-05-06 17:23:53.000000 LexBuilder-1.2.0/LexBuilder/BasePyLexer.py
+-rw-rw-r--   0 alexander554  (1000) alexander554  (1000)     3717 2024-05-25 20:04:45.000000 LexBuilder-1.2.0/LexBuilder/Builder.py
+-rw-rw-r--   0 alexander554  (1000) alexander554  (1000)      117 2024-05-06 17:21:27.000000 LexBuilder-1.2.0/LexBuilder/__init__.py
+drwxrwxr-x   0 alexander554  (1000) alexander554  (1000)        0 2024-05-25 20:23:14.035749 LexBuilder-1.2.0/LexBuilder.egg-info/
+-rw-rw-r--   0 alexander554  (1000) alexander554  (1000)     3092 2024-05-25 20:23:13.000000 LexBuilder-1.2.0/LexBuilder.egg-info/PKG-INFO
+-rw-rw-r--   0 alexander554  (1000) alexander554  (1000)      270 2024-05-25 20:23:14.000000 LexBuilder-1.2.0/LexBuilder.egg-info/SOURCES.txt
+-rw-rw-r--   0 alexander554  (1000) alexander554  (1000)        1 2024-05-25 20:23:13.000000 LexBuilder-1.2.0/LexBuilder.egg-info/dependency_links.txt
+-rw-rw-r--   0 alexander554  (1000) alexander554  (1000)       11 2024-05-25 20:23:13.000000 LexBuilder-1.2.0/LexBuilder.egg-info/top_level.txt
+-rw-rw-r--   0 alexander554  (1000) alexander554  (1000)     3092 2024-05-25 20:23:14.035749 LexBuilder-1.2.0/PKG-INFO
+-rw-rw-r--   0 alexander554  (1000) alexander554  (1000)     2652 2024-05-25 20:16:23.000000 LexBuilder-1.2.0/README.md
+-rw-rw-r--   0 alexander554  (1000) alexander554  (1000)       38 2024-05-25 20:23:14.036749 LexBuilder-1.2.0/setup.cfg
+-rw-rw-r--   0 alexander554  (1000) alexander554  (1000)      645 2024-05-25 20:22:17.000000 LexBuilder-1.2.0/setup.py
```

### Comparing `lexbuilder-1.1.0/LICENSE` & `LexBuilder-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lexbuilder-1.1.0/LexBuilder/BaseCppLexer.py` & `LexBuilder-1.2.0/LexBuilder/BaseCppLexer.py`

 * *Files identical despite different names*

### Comparing `lexbuilder-1.1.0/LexBuilder/BasePyLexer.py` & `LexBuilder-1.2.0/LexBuilder/BasePyLexer.py`

 * *Files identical despite different names*

### Comparing `lexbuilder-1.1.0/LexBuilder/Builder.py` & `LexBuilder-1.2.0/LexBuilder/Builder.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,16 +5,19 @@
 class Token:
     def __init__(self, name, value):
         self.name = name
         self.value = value
 
 
 class PyBuilder:
-    def __init__(self, tokens):
-        self.tokens = tokens
+    def __init__(self, tokens=None):
+        self.tokens = tokens if tokens else []
+
+    def add_token(self, token):
+        self.tokens.append(token)
 
     def generate_code_for_tokens(self):
         result1 = ""
         result2 = ""
         result3 = ""
 
         for token in self.tokens:
@@ -42,16 +45,19 @@
         with open("Lexer.py", "w", encoding="utf-8") as file:
             file.write("import sys\n\n\n")
             file.write(pytypes.format(code1) + "\n")
             file.write(pylexer.substitute(first=code2, second=code3) + "\n\n")
 
 
 class CppBuilder:
-    def __init__(self, tokens):
-        self.tokens = tokens
+    def __init__(self, tokens=None):
+        self.tokens = tokens if tokens else []
+
+    def add_token(self, token):
+        self.tokens.append(token)
 
     def generate_code_for_tokens(self):
         result1 = "\n"
         result2 = ""
         result3 = ""
 
         for token in self.tokens:
```

### Comparing `lexbuilder-1.1.0/LexBuilder.egg-info/PKG-INFO` & `LexBuilder-1.2.0/LexBuilder.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 Metadata-Version: 2.1
 Name: LexBuilder
-Version: 1.1.0
+Version: 1.2.0
 Summary: Library for automatic construction of lexers
 Author: Alexander554
 Author-email: gaa.28112008@gmail.com
-Keywords: python c++ lexer
+Keywords: lexbuilder python c++ lexer
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # About LexBuilder:
 LexBuilder is a library for automatically building a lexer in Python and C++. In the future, the library will be able to build lexers in major programming languages such as Golang, Java/Kotlin, etc.
 
 ## About Syntax:
-In order for the library to generate the Lexer.py or Lexer.h file, you need to pass a list of tokens to the Builder class.
-To declare a token, you need to import the Token() class from the Builder() class. You need to pass the token name and its value to the Token() class. Afterwards, add all the tokens we created to a list and pass it as an argument to the PyBuilder() or CppBuilder class. By default, the lexer contains the tokens:
-
+In order for the library to generate a Lexer.py or Lexer.h file, you need to pass a list of tokens to the Builder class or use its .add_token() method. To declare a token, you need to import the Token() class from the Builder() class. You need to pass the token name and its value to the Token() class. After that, add all the tokens we created to a list and pass it as an argument to the PyBuilder() or CppBuilder class. By default, the lexer contains the tokens:
 ```python
 INT_NUMBER = "INT_NUMBER"
 FLOAT_NUMBER = "FLOAT_NUMBER"
 STRING = "STRING"
 PLUS = "PLUS"
 MINUS = "MINUS"
 VAR = "VAR"
@@ -41,59 +39,71 @@
 #
 ## Python Example:
 ### Generate Lexer:
 ```python
 from LexBuilder.Builder import PyBuilder, Token
 
 
+MULTIPLY = Token("MULTIPLY", "*")
 DIVIDE = Token("DIVIDE", "/")
 PRINT = Token("PRINT", "print")
-INPUT = Token("INPUT", "input")
 
-tokens = [DIVIDE, PRINT, INPUT]
+tokens = [MULTIPLY, DIVIDE, PRINT]
 
 lexer = PyBuilder(tokens)
+
+lexer.add_token(Token("INPUT", "input"))
+lexer.add_token(Token("LPAREN", "("))
+lexer.add_token(Token("RPAREN", ")"))
+
 lexer.build()
 ```
 
 ### Use Lexer:
 ```python
 from Lexer import *
 
 
-code = 'print "Hello, world!"'
+code = 'print("Hello, world!")'
 lexer = Lexer(code)
 
 token = lexer.get_next_token()
 print(token)
 
 while token.type != EOF:
     token = lexer.get_next_token()
     print(token)
 ```
 
 ```python
 Token(PRINT, "print")
+Token(LPAREN, "(")
 Token(STRING, "Hello, world!")
+Token(RPAREN, ")")
 Token(EOF, None)
 ```
 #
 ## C++ Example:
 ### Generate Lexer:
 ```python
 from LexBuilder.Builder import CppBuilder, Token
 
 
+MULTIPLY = Token("MULTIPLY", "*")
 DIVIDE = Token("DIVIDE", "/")
 PRINT = Token("PRINT", "print")
-INPUT = Token("INPUT", "input")
 
-tokens = [DIVIDE, PRINT, INPUT]
+tokens = [MULTIPLY, DIVIDE, PRINT]
 
 lexer = CppBuilder(tokens)
+
+lexer.add_token(Token("INPUT", "input"))
+lexer.add_token(Token("LPAREN", "("))
+lexer.add_token(Token("RPAREN", ")"))
+
 lexer.build()
 ```
 
 ### Use Lexer:
 ```cpp
 #include "Lexer.h"
```

### Comparing `lexbuilder-1.1.0/PKG-INFO` & `LexBuilder-1.2.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 Metadata-Version: 2.1
 Name: LexBuilder
-Version: 1.1.0
+Version: 1.2.0
 Summary: Library for automatic construction of lexers
 Author: Alexander554
 Author-email: gaa.28112008@gmail.com
-Keywords: python c++ lexer
+Keywords: lexbuilder python c++ lexer
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # About LexBuilder:
 LexBuilder is a library for automatically building a lexer in Python and C++. In the future, the library will be able to build lexers in major programming languages such as Golang, Java/Kotlin, etc.
 
 ## About Syntax:
-In order for the library to generate the Lexer.py or Lexer.h file, you need to pass a list of tokens to the Builder class.
-To declare a token, you need to import the Token() class from the Builder() class. You need to pass the token name and its value to the Token() class. Afterwards, add all the tokens we created to a list and pass it as an argument to the PyBuilder() or CppBuilder class. By default, the lexer contains the tokens:
-
+In order for the library to generate a Lexer.py or Lexer.h file, you need to pass a list of tokens to the Builder class or use its .add_token() method. To declare a token, you need to import the Token() class from the Builder() class. You need to pass the token name and its value to the Token() class. After that, add all the tokens we created to a list and pass it as an argument to the PyBuilder() or CppBuilder class. By default, the lexer contains the tokens:
 ```python
 INT_NUMBER = "INT_NUMBER"
 FLOAT_NUMBER = "FLOAT_NUMBER"
 STRING = "STRING"
 PLUS = "PLUS"
 MINUS = "MINUS"
 VAR = "VAR"
@@ -41,59 +39,71 @@
 #
 ## Python Example:
 ### Generate Lexer:
 ```python
 from LexBuilder.Builder import PyBuilder, Token
 
 
+MULTIPLY = Token("MULTIPLY", "*")
 DIVIDE = Token("DIVIDE", "/")
 PRINT = Token("PRINT", "print")
-INPUT = Token("INPUT", "input")
 
-tokens = [DIVIDE, PRINT, INPUT]
+tokens = [MULTIPLY, DIVIDE, PRINT]
 
 lexer = PyBuilder(tokens)
+
+lexer.add_token(Token("INPUT", "input"))
+lexer.add_token(Token("LPAREN", "("))
+lexer.add_token(Token("RPAREN", ")"))
+
 lexer.build()
 ```
 
 ### Use Lexer:
 ```python
 from Lexer import *
 
 
-code = 'print "Hello, world!"'
+code = 'print("Hello, world!")'
 lexer = Lexer(code)
 
 token = lexer.get_next_token()
 print(token)
 
 while token.type != EOF:
     token = lexer.get_next_token()
     print(token)
 ```
 
 ```python
 Token(PRINT, "print")
+Token(LPAREN, "(")
 Token(STRING, "Hello, world!")
+Token(RPAREN, ")")
 Token(EOF, None)
 ```
 #
 ## C++ Example:
 ### Generate Lexer:
 ```python
 from LexBuilder.Builder import CppBuilder, Token
 
 
+MULTIPLY = Token("MULTIPLY", "*")
 DIVIDE = Token("DIVIDE", "/")
 PRINT = Token("PRINT", "print")
-INPUT = Token("INPUT", "input")
 
-tokens = [DIVIDE, PRINT, INPUT]
+tokens = [MULTIPLY, DIVIDE, PRINT]
 
 lexer = CppBuilder(tokens)
+
+lexer.add_token(Token("INPUT", "input"))
+lexer.add_token(Token("LPAREN", "("))
+lexer.add_token(Token("RPAREN", ")"))
+
 lexer.build()
 ```
 
 ### Use Lexer:
 ```cpp
 #include "Lexer.h"
```

### Comparing `lexbuilder-1.1.0/README.md` & `LexBuilder-1.2.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 # About LexBuilder:
 LexBuilder is a library for automatically building a lexer in Python and C++. In the future, the library will be able to build lexers in major programming languages such as Golang, Java/Kotlin, etc.
 
 ## About Syntax:
-In order for the library to generate the Lexer.py or Lexer.h file, you need to pass a list of tokens to the Builder class.
-To declare a token, you need to import the Token() class from the Builder() class. You need to pass the token name and its value to the Token() class. Afterwards, add all the tokens we created to a list and pass it as an argument to the PyBuilder() or CppBuilder class. By default, the lexer contains the tokens:
-
+In order for the library to generate a Lexer.py or Lexer.h file, you need to pass a list of tokens to the Builder class or use its .add_token() method. To declare a token, you need to import the Token() class from the Builder() class. You need to pass the token name and its value to the Token() class. After that, add all the tokens we created to a list and pass it as an argument to the PyBuilder() or CppBuilder class. By default, the lexer contains the tokens:
 ```python
 INT_NUMBER = "INT_NUMBER"
 FLOAT_NUMBER = "FLOAT_NUMBER"
 STRING = "STRING"
 PLUS = "PLUS"
 MINUS = "MINUS"
 VAR = "VAR"
@@ -27,59 +25,71 @@
 #
 ## Python Example:
 ### Generate Lexer:
 ```python
 from LexBuilder.Builder import PyBuilder, Token
 
 
+MULTIPLY = Token("MULTIPLY", "*")
 DIVIDE = Token("DIVIDE", "/")
 PRINT = Token("PRINT", "print")
-INPUT = Token("INPUT", "input")
 
-tokens = [DIVIDE, PRINT, INPUT]
+tokens = [MULTIPLY, DIVIDE, PRINT]
 
 lexer = PyBuilder(tokens)
+
+lexer.add_token(Token("INPUT", "input"))
+lexer.add_token(Token("LPAREN", "("))
+lexer.add_token(Token("RPAREN", ")"))
+
 lexer.build()
 ```
 
 ### Use Lexer:
 ```python
 from Lexer import *
 
 
-code = 'print "Hello, world!"'
+code = 'print("Hello, world!")'
 lexer = Lexer(code)
 
 token = lexer.get_next_token()
 print(token)
 
 while token.type != EOF:
     token = lexer.get_next_token()
     print(token)
 ```
 
 ```python
 Token(PRINT, "print")
+Token(LPAREN, "(")
 Token(STRING, "Hello, world!")
+Token(RPAREN, ")")
 Token(EOF, None)
 ```
 #
 ## C++ Example:
 ### Generate Lexer:
 ```python
 from LexBuilder.Builder import CppBuilder, Token
 
 
+MULTIPLY = Token("MULTIPLY", "*")
 DIVIDE = Token("DIVIDE", "/")
 PRINT = Token("PRINT", "print")
-INPUT = Token("INPUT", "input")
 
-tokens = [DIVIDE, PRINT, INPUT]
+tokens = [MULTIPLY, DIVIDE, PRINT]
 
 lexer = CppBuilder(tokens)
+
+lexer.add_token(Token("INPUT", "input"))
+lexer.add_token(Token("LPAREN", "("))
+lexer.add_token(Token("RPAREN", ")"))
+
 lexer.build()
 ```
 
 ### Use Lexer:
 ```cpp
 #include "Lexer.h"
```

### Comparing `lexbuilder-1.1.0/setup.py` & `LexBuilder-1.2.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 
 def readme():
   with open('README.md', 'r') as f:
     return f.read()
 
 setup(
   name='LexBuilder',
-  version='1.1.0',
+  version='1.2.0',
   author='Alexander554',
   author_email='gaa.28112008@gmail.com',
   description='Library for automatic construction of lexers',
   long_description=readme(),
   long_description_content_type='text/markdown',
   packages=find_packages(),
   install_requires=[''],
   classifiers=[
     'Programming Language :: Python :: 3.11',
     'License :: OSI Approved :: MIT License',
     'Operating System :: OS Independent'
   ],
-  keywords='python c++ lexer',
+  keywords='lexbuilder python c++ lexer',
   python_requires='>=3.7'
 )
```

