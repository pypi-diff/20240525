# Comparing `tmp/import_expression-1.1.4.tar.gz` & `tmp/import_expression-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/import_expression-1.1.4.tar", last modified: Tue Jun  9 21:07:59 2020, max compression
+gzip compressed data, was "import_expression-1.1.5.tar", last modified: Sat May 25 01:19:31 2024, max compression
```

## Comparing `import_expression-1.1.4.tar` & `import_expression-1.1.5.tar`

### file list

```diff
@@ -1,25 +1,28 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2020-06-09 21:07:59.648264 import_expression-1.1.4/
--rw-r--r--   0 user      (1000) user      (1000)       30 2020-04-04 00:41:26.000000 import_expression-1.1.4/MANIFEST.in
--rw-r--r--   0 user      (1000) user      (1000)     4049 2020-06-09 21:07:59.648264 import_expression-1.1.4/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)     2946 2020-05-07 18:42:02.000000 import_expression-1.1.4/README.md
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2020-06-09 21:07:59.644930 import_expression-1.1.4/import_expression/
--rwxr-xr-x   0 user      (1000) user      (1000)     5513 2020-04-04 00:48:46.000000 import_expression-1.1.4/import_expression/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)     9128 2020-05-01 00:02:30.000000 import_expression-1.1.4/import_expression/__main__.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2020-06-09 21:07:59.644930 import_expression-1.1.4/import_expression/_codec/
--rw-r--r--   0 user      (1000) user      (1000)     1663 2020-04-04 03:39:44.000000 import_expression-1.1.4/import_expression/_codec/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)      836 2020-04-04 00:41:26.000000 import_expression-1.1.4/import_expression/_codec/compat.py
--rw-r--r--   0 user      (1000) user      (1000)      965 2020-04-04 03:24:11.000000 import_expression-1.1.4/import_expression/_main2.py
--rw-r--r--   0 user      (1000) user      (1000)     7436 2020-06-09 01:58:36.000000 import_expression-1.1.4/import_expression/_parser.py
--rw-r--r--   0 user      (1000) user      (1000)     4341 2020-04-04 00:41:26.000000 import_expression-1.1.4/import_expression/_syntax.py
--rw-r--r--   0 user      (1000) user      (1000)     1243 2019-10-23 22:20:10.000000 import_expression-1.1.4/import_expression/constants.py
--rw-r--r--   0 user      (1000) user      (1000)       22 2020-06-09 21:07:11.000000 import_expression-1.1.4/import_expression/version.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2020-06-09 21:07:59.644930 import_expression-1.1.4/import_expression.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     4049 2020-06-09 21:07:59.000000 import_expression-1.1.4/import_expression.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      578 2020-06-09 21:07:59.000000 import_expression-1.1.4/import_expression.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2020-06-09 21:07:59.000000 import_expression-1.1.4/import_expression.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)      181 2020-06-09 21:07:59.000000 import_expression-1.1.4/import_expression.egg-info/entry_points.txt
--rw-r--r--   0 user      (1000) user      (1000)       51 2020-06-09 21:07:59.000000 import_expression-1.1.4/import_expression.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)       18 2020-06-09 21:07:59.000000 import_expression-1.1.4/import_expression.egg-info/top_level.txt
--rw-r--r--   0 user      (1000) user      (1000)      130 2020-05-28 04:06:01.000000 import_expression-1.1.4/import_expression.pth
--rw-r--r--   0 user      (1000) user      (1000)       38 2020-06-09 21:07:59.648264 import_expression-1.1.4/setup.cfg
--rwxr-xr-x   0 user      (1000) user      (1000)     5035 2020-05-28 04:06:01.000000 import_expression-1.1.4/setup.py
+drwxr-x---   0 user      (1000) user      (1000)        0 2024-05-25 01:19:31.776662 import_expression-1.1.5/
+-rw-r-----   0 user      (1000) user      (1000)     4280 2024-05-25 01:05:33.000000 import_expression-1.1.5/LICENSE
+-rw-r-----   0 user      (1000) user      (1000)     1112 2024-05-25 01:05:33.000000 import_expression-1.1.5/LICENSE-header
+-rw-r-----   0 user      (1000) user      (1000)       47 2024-05-25 01:05:33.000000 import_expression-1.1.5/MANIFEST.in
+-rw-r--r--   0 user      (1000) user      (1000)     3495 2024-05-25 01:19:31.773328 import_expression-1.1.5/PKG-INFO
+-rw-r-----   0 user      (1000) user      (1000)     2946 2024-05-25 01:05:33.000000 import_expression-1.1.5/README.md
+drwxr-x---   0 user      (1000) user      (1000)        0 2024-05-25 01:19:31.773328 import_expression-1.1.5/import_expression/
+-rwxr-x---   0 user      (1000) user      (1000)     5513 2024-05-25 01:05:33.000000 import_expression-1.1.5/import_expression/__init__.py
+-rw-r-----   0 user      (1000) user      (1000)     9330 2024-05-25 01:05:33.000000 import_expression-1.1.5/import_expression/__main__.py
+drwxr-x---   0 user      (1000) user      (1000)        0 2024-05-25 01:19:31.773328 import_expression-1.1.5/import_expression/_codec/
+-rw-r-----   0 user      (1000) user      (1000)     1663 2024-05-25 01:05:33.000000 import_expression-1.1.5/import_expression/_codec/__init__.py
+-rw-r-----   0 user      (1000) user      (1000)      836 2024-05-25 01:05:33.000000 import_expression-1.1.5/import_expression/_codec/compat.py
+-rw-r-----   0 user      (1000) user      (1000)      965 2024-05-25 01:05:33.000000 import_expression-1.1.5/import_expression/_main2.py
+-rw-r-----   0 user      (1000) user      (1000)     7436 2024-05-25 01:05:33.000000 import_expression-1.1.5/import_expression/_parser.py
+-rw-r-----   0 user      (1000) user      (1000)     4341 2024-05-25 01:05:33.000000 import_expression-1.1.5/import_expression/_syntax.py
+-rw-r-----   0 user      (1000) user      (1000)     1243 2024-05-25 01:05:33.000000 import_expression-1.1.5/import_expression/constants.py
+-rw-r-----   0 user      (1000) user      (1000)       22 2024-05-25 01:19:05.000000 import_expression-1.1.5/import_expression/version.py
+drwxr-x---   0 user      (1000) user      (1000)        0 2024-05-25 01:19:31.773328 import_expression-1.1.5/import_expression.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)     3495 2024-05-25 01:19:31.000000 import_expression-1.1.5/import_expression.egg-info/PKG-INFO
+-rw-r-----   0 user      (1000) user      (1000)      610 2024-05-25 01:19:31.000000 import_expression-1.1.5/import_expression.egg-info/SOURCES.txt
+-rw-r-----   0 user      (1000) user      (1000)        1 2024-05-25 01:19:31.000000 import_expression-1.1.5/import_expression.egg-info/dependency_links.txt
+-rw-r-----   0 user      (1000) user      (1000)      180 2024-05-25 01:19:31.000000 import_expression-1.1.5/import_expression.egg-info/entry_points.txt
+-rw-r-----   0 user      (1000) user      (1000)       51 2024-05-25 01:19:31.000000 import_expression-1.1.5/import_expression.egg-info/requires.txt
+-rw-r-----   0 user      (1000) user      (1000)       18 2024-05-25 01:19:31.000000 import_expression-1.1.5/import_expression.egg-info/top_level.txt
+-rw-r-----   0 user      (1000) user      (1000)      130 2024-05-25 01:05:33.000000 import_expression-1.1.5/import_expression.pth
+-rw-r-----   0 user      (1000) user      (1000)       38 2024-05-25 01:19:31.776662 import_expression-1.1.5/setup.cfg
+-rwxr-x---   0 user      (1000) user      (1000)     5035 2024-05-25 01:05:33.000000 import_expression-1.1.5/setup.py
+-rw-r-----   0 user      (1000) user      (1000)     8747 2024-05-25 01:05:33.000000 import_expression-1.1.5/tests.py
```

### Comparing `import_expression-1.1.4/PKG-INFO` & `import_expression-1.1.5/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,100 +1,104 @@
 Metadata-Version: 2.1
 Name: import_expression
-Version: 1.1.4
+Version: 1.1.5
 Summary: Parses a superset of Python allowing for inline module import expressions
 Home-page: https://github.com/iomintz/import-expression-parser
 Author: io mintz
 Author-email: io@mintz.cc
 License: MIT
-Description: # Import Expression Parser (for lack of a better name)
-        
-        [![Build Status](https://img.shields.io/travis/iomintz/import-expression-parser/main.svg?label=tests)](https://travis-ci.org/iomintz/import-expression-parser)
-        [![Coverage Status](https://coveralls.io/repos/github/iomintz/import-expression-parser/badge.svg?branch=main)](https://coveralls.io/github/iomintz/import-expression-parser?branch=main)
-        
-        Import Expression Parser converts code like this:
-        
-        ```py
-        urllib.parse!.quote('hello there')
-        ```
-        
-        Into this equivalent code:
-        ```py
-        importlib.import_module('urllib.parse').quote('hello there')
-        ```
-        
-        ## Usage
-        
-        ```py
-        >>> import import_expression
-        >>> import_expression.eval('collections!.Counter("bccdddeeee")')
-        Counter({'e': 4, 'd': 3, 'c': 2, 'b': 1})
-        ```
-        
-        The other public functions are `exec`, `compile`, `parse`, `find_imports`, and `update_globals`.
-        See their docstrings for details.
-        
-        By default, the filename for `SyntaxError`s is `<string>`.
-        To change this, pass in a filename via the `filename` kwarg.
-        
-        ### Reusing compiled code objects
-        
-        import_expression.eval/exec/compile should not be passed strings in a tight loop. \
-        Doing so will recompile the string every time. Instead, you should pre-compile the string to a code object
-        and pass that to import_expression.eval / import_expression.exec.
-        For example, instead of this:
-        
-        ```py
-        for line in sys.stdin:
-        	print(import_expression.eval('foo!.bar(l)', dict(l=line))
-        ```
-        
-        Prefer this:
-        
-        ```py
-        code = import_expression.compile('foo!.bar(l)', mode='eval')
-        for line in sys.stdin:
-        	print(import_expression.eval(code, dict(l=line)))
-        ```
-        
-        ### Custom encoding
-        
-        ```py
-        # encoding: import_expression
-        print(typing!.TYPE_CHECKING)
-        ```
-        
-        This file, when run, will print True/False. For maximum laziness you can also do `#coding:ie`.
-        
-        ### REPL usage
-        
-        Run `import-expression` for an import expression enabled REPL. \
-        Run `import-expression -a` for a REPL that supports both import expressions and top level `await` (3.8+).
-        
-        See `import-expression --help` for more details.
-        
-        ### Running a file
-        
-        Run `import-expression <filename.py>`.
-        
-        ### File rewriter
-        
-        Run `import-expression-rewrite <file.py>` to rewrite a file containing import expressions to standard Python. \
-        Add the `-i` flag to rewrite in-place.
-        
-        ## Limitations / Known Issues
-        
-        * Due to the hell that is f-string parsing, and because `!` is already an operator inside f-strings,
-          import expressions inside f-strings will likely never be supported.
-        * Due to python limitations, results of `import_expression.exec` will have no effect on the caller's globals or locals
-          without an explicit `globals` argument.
-        * Unlike real operators, spaces before and after the import expression operator (such as `x ! .y`) are not supported.
-        
-        ## [License](https://github.com/iomintz/import-expression-parser/blob/main/LICENSE)
-        
-        Copyright © 2018–2019 Io Mintz <<io@mintz.cc>>. All Rights Reserved. \
-        Licensed under the MIT License. See the LICENSE file for details.
-        
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: LICENSE-header
+Requires-Dist: astunparse<2.0.0,>=1.6.3
 Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-cov; extra == "test"
+
+# Import Expression Parser (for lack of a better name)
+
+[![Build Status](https://img.shields.io/travis/iomintz/import-expression-parser/main.svg?label=tests)](https://travis-ci.org/iomintz/import-expression-parser)
+[![Coverage Status](https://coveralls.io/repos/github/iomintz/import-expression-parser/badge.svg?branch=main)](https://coveralls.io/github/iomintz/import-expression-parser?branch=main)
+
+Import Expression Parser converts code like this:
+
+```py
+urllib.parse!.quote('hello there')
+```
+
+Into this equivalent code:
+```py
+importlib.import_module('urllib.parse').quote('hello there')
+```
+
+## Usage
+
+```py
+>>> import import_expression
+>>> import_expression.eval('collections!.Counter("bccdddeeee")')
+Counter({'e': 4, 'd': 3, 'c': 2, 'b': 1})
+```
+
+The other public functions are `exec`, `compile`, `parse`, `find_imports`, and `update_globals`.
+See their docstrings for details.
+
+By default, the filename for `SyntaxError`s is `<string>`.
+To change this, pass in a filename via the `filename` kwarg.
+
+### Reusing compiled code objects
+
+import_expression.eval/exec/compile should not be passed strings in a tight loop. \
+Doing so will recompile the string every time. Instead, you should pre-compile the string to a code object
+and pass that to import_expression.eval / import_expression.exec.
+For example, instead of this:
+
+```py
+for line in sys.stdin:
+	print(import_expression.eval('foo!.bar(l)', dict(l=line))
+```
+
+Prefer this:
+
+```py
+code = import_expression.compile('foo!.bar(l)', mode='eval')
+for line in sys.stdin:
+	print(import_expression.eval(code, dict(l=line)))
+```
+
+### Custom encoding
+
+```py
+# encoding: import_expression
+print(typing!.TYPE_CHECKING)
+```
+
+This file, when run, will print True/False. For maximum laziness you can also do `#coding:ie`.
+
+### REPL usage
+
+Run `import-expression` for an import expression enabled REPL. \
+Run `import-expression -a` for a REPL that supports both import expressions and top level `await` (3.8+).
+
+See `import-expression --help` for more details.
+
+### Running a file
+
+Run `import-expression <filename.py>`.
+
+### File rewriter
+
+Run `import-expression-rewrite <file.py>` to rewrite a file containing import expressions to standard Python. \
+Add the `-i` flag to rewrite in-place.
+
+## Limitations / Known Issues
+
+* Due to the hell that is f-string parsing, and because `!` is already an operator inside f-strings,
+  import expressions inside f-strings will likely never be supported.
+* Due to python limitations, results of `import_expression.exec` will have no effect on the caller's globals or locals
+  without an explicit `globals` argument.
+* Unlike real operators, spaces before and after the import expression operator (such as `x ! .y`) are not supported.
+
+## [License](https://github.com/iomintz/import-expression-parser/blob/main/LICENSE)
+
+Copyright © 2018–2019 Io Mintz <<io@mintz.cc>>. All Rights Reserved. \
+Licensed under the MIT License. See the LICENSE file for details.
```

### Comparing `import_expression-1.1.4/README.md` & `import_expression-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `import_expression-1.1.4/import_expression/__init__.py` & `import_expression-1.1.5/import_expression/__init__.py`

 * *Files identical despite different names*

### Comparing `import_expression-1.1.4/import_expression/__main__.py` & `import_expression-1.1.5/import_expression/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 import rlcompleter
 import sys
 import traceback
 import threading
 import types
 import warnings
 from asyncio import futures
-from codeop import PyCF_DONT_IMPLY_DEDENT
+from codeop import PyCF_DONT_IMPLY_DEDENT, PyCF_ALLOW_INCOMPLETE_INPUT
 
 import import_expression
 from import_expression import constants
 
 if os.path.basename(sys.argv[0]) == 'import_expression':
 	import warnings
 	warnings.warn(UserWarning(
@@ -69,23 +69,28 @@
 # this must be vendored as codeop.Compile is hardcoded to use builtins.compile
 class ImportExpressionCompile:
 	"""Instances of this class behave much like the built-in compile
 	function, but if one is used to compile text containing a future
 	statement, it "remembers" and compiles all subsequent program texts
 	with the statement in force."""
 	def __init__(self):
-		self.flags = PyCF_DONT_IMPLY_DEDENT
+		self.flags = PyCF_DONT_IMPLY_DEDENT | PyCF_ALLOW_INCOMPLETE_INPUT
 
-	def __call__(self, source, filename, symbol):
-		codeob = import_expression.compile(source, filename, symbol, self.flags, dont_inherit=True)
+	def __call__(self, source, filename, symbol, **kwargs):
+		flags = self.flags
+		if kwargs.get('incomplete_input', True) is False:
+			flags &= ~PyCF_DONT_IMPLY_DEDENT
+			flags &= ~PyCF_ALLOW_INCOMPLETE_INPUT
+		codeob = import_expression.compile(source, filename, symbol, flags, True)
 		for feature in features:
 			if codeob.co_flags & feature.compiler_flag:
 				self.flags |= feature.compiler_flag
 		return codeob
 
+
 class ImportExpressionInteractiveConsole(code.InteractiveConsole):
 	def __init__(self, locals=None, filename='<console>'):
 		super().__init__(locals, filename)
 		self.locals.update({constants.IMPORTER: importlib.import_module})
 		self.compile = ImportExpressionCommandCompiler()
 
 # we must vendor this class because it creates global variables that the main code depends on
```

### Comparing `import_expression-1.1.4/import_expression/_codec/__init__.py` & `import_expression-1.1.5/import_expression/_codec/__init__.py`

 * *Files identical despite different names*

### Comparing `import_expression-1.1.4/import_expression/_codec/compat.py` & `import_expression-1.1.5/import_expression/_codec/compat.py`

 * *Files identical despite different names*

### Comparing `import_expression-1.1.4/import_expression/_main2.py` & `import_expression-1.1.5/import_expression/_main2.py`

 * *Files identical despite different names*

### Comparing `import_expression-1.1.4/import_expression/_parser.py` & `import_expression-1.1.5/import_expression/_parser.py`

 * *Files identical despite different names*

### Comparing `import_expression-1.1.4/import_expression/_syntax.py` & `import_expression-1.1.5/import_expression/_syntax.py`

 * *Files identical despite different names*

### Comparing `import_expression-1.1.4/import_expression/constants.py` & `import_expression-1.1.5/import_expression/constants.py`

 * *Files identical despite different names*

### Comparing `import_expression-1.1.4/import_expression.egg-info/PKG-INFO` & `import_expression-1.1.5/import_expression.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,100 +1,104 @@
 Metadata-Version: 2.1
-Name: import-expression
-Version: 1.1.4
+Name: import_expression
+Version: 1.1.5
 Summary: Parses a superset of Python allowing for inline module import expressions
 Home-page: https://github.com/iomintz/import-expression-parser
 Author: io mintz
 Author-email: io@mintz.cc
 License: MIT
-Description: # Import Expression Parser (for lack of a better name)
-        
-        [![Build Status](https://img.shields.io/travis/iomintz/import-expression-parser/main.svg?label=tests)](https://travis-ci.org/iomintz/import-expression-parser)
-        [![Coverage Status](https://coveralls.io/repos/github/iomintz/import-expression-parser/badge.svg?branch=main)](https://coveralls.io/github/iomintz/import-expression-parser?branch=main)
-        
-        Import Expression Parser converts code like this:
-        
-        ```py
-        urllib.parse!.quote('hello there')
-        ```
-        
-        Into this equivalent code:
-        ```py
-        importlib.import_module('urllib.parse').quote('hello there')
-        ```
-        
-        ## Usage
-        
-        ```py
-        >>> import import_expression
-        >>> import_expression.eval('collections!.Counter("bccdddeeee")')
-        Counter({'e': 4, 'd': 3, 'c': 2, 'b': 1})
-        ```
-        
-        The other public functions are `exec`, `compile`, `parse`, `find_imports`, and `update_globals`.
-        See their docstrings for details.
-        
-        By default, the filename for `SyntaxError`s is `<string>`.
-        To change this, pass in a filename via the `filename` kwarg.
-        
-        ### Reusing compiled code objects
-        
-        import_expression.eval/exec/compile should not be passed strings in a tight loop. \
-        Doing so will recompile the string every time. Instead, you should pre-compile the string to a code object
-        and pass that to import_expression.eval / import_expression.exec.
-        For example, instead of this:
-        
-        ```py
-        for line in sys.stdin:
-        	print(import_expression.eval('foo!.bar(l)', dict(l=line))
-        ```
-        
-        Prefer this:
-        
-        ```py
-        code = import_expression.compile('foo!.bar(l)', mode='eval')
-        for line in sys.stdin:
-        	print(import_expression.eval(code, dict(l=line)))
-        ```
-        
-        ### Custom encoding
-        
-        ```py
-        # encoding: import_expression
-        print(typing!.TYPE_CHECKING)
-        ```
-        
-        This file, when run, will print True/False. For maximum laziness you can also do `#coding:ie`.
-        
-        ### REPL usage
-        
-        Run `import-expression` for an import expression enabled REPL. \
-        Run `import-expression -a` for a REPL that supports both import expressions and top level `await` (3.8+).
-        
-        See `import-expression --help` for more details.
-        
-        ### Running a file
-        
-        Run `import-expression <filename.py>`.
-        
-        ### File rewriter
-        
-        Run `import-expression-rewrite <file.py>` to rewrite a file containing import expressions to standard Python. \
-        Add the `-i` flag to rewrite in-place.
-        
-        ## Limitations / Known Issues
-        
-        * Due to the hell that is f-string parsing, and because `!` is already an operator inside f-strings,
-          import expressions inside f-strings will likely never be supported.
-        * Due to python limitations, results of `import_expression.exec` will have no effect on the caller's globals or locals
-          without an explicit `globals` argument.
-        * Unlike real operators, spaces before and after the import expression operator (such as `x ! .y`) are not supported.
-        
-        ## [License](https://github.com/iomintz/import-expression-parser/blob/main/LICENSE)
-        
-        Copyright © 2018–2019 Io Mintz <<io@mintz.cc>>. All Rights Reserved. \
-        Licensed under the MIT License. See the LICENSE file for details.
-        
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: LICENSE-header
+Requires-Dist: astunparse<2.0.0,>=1.6.3
 Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-cov; extra == "test"
+
+# Import Expression Parser (for lack of a better name)
+
+[![Build Status](https://img.shields.io/travis/iomintz/import-expression-parser/main.svg?label=tests)](https://travis-ci.org/iomintz/import-expression-parser)
+[![Coverage Status](https://coveralls.io/repos/github/iomintz/import-expression-parser/badge.svg?branch=main)](https://coveralls.io/github/iomintz/import-expression-parser?branch=main)
+
+Import Expression Parser converts code like this:
+
+```py
+urllib.parse!.quote('hello there')
+```
+
+Into this equivalent code:
+```py
+importlib.import_module('urllib.parse').quote('hello there')
+```
+
+## Usage
+
+```py
+>>> import import_expression
+>>> import_expression.eval('collections!.Counter("bccdddeeee")')
+Counter({'e': 4, 'd': 3, 'c': 2, 'b': 1})
+```
+
+The other public functions are `exec`, `compile`, `parse`, `find_imports`, and `update_globals`.
+See their docstrings for details.
+
+By default, the filename for `SyntaxError`s is `<string>`.
+To change this, pass in a filename via the `filename` kwarg.
+
+### Reusing compiled code objects
+
+import_expression.eval/exec/compile should not be passed strings in a tight loop. \
+Doing so will recompile the string every time. Instead, you should pre-compile the string to a code object
+and pass that to import_expression.eval / import_expression.exec.
+For example, instead of this:
+
+```py
+for line in sys.stdin:
+	print(import_expression.eval('foo!.bar(l)', dict(l=line))
+```
+
+Prefer this:
+
+```py
+code = import_expression.compile('foo!.bar(l)', mode='eval')
+for line in sys.stdin:
+	print(import_expression.eval(code, dict(l=line)))
+```
+
+### Custom encoding
+
+```py
+# encoding: import_expression
+print(typing!.TYPE_CHECKING)
+```
+
+This file, when run, will print True/False. For maximum laziness you can also do `#coding:ie`.
+
+### REPL usage
+
+Run `import-expression` for an import expression enabled REPL. \
+Run `import-expression -a` for a REPL that supports both import expressions and top level `await` (3.8+).
+
+See `import-expression --help` for more details.
+
+### Running a file
+
+Run `import-expression <filename.py>`.
+
+### File rewriter
+
+Run `import-expression-rewrite <file.py>` to rewrite a file containing import expressions to standard Python. \
+Add the `-i` flag to rewrite in-place.
+
+## Limitations / Known Issues
+
+* Due to the hell that is f-string parsing, and because `!` is already an operator inside f-strings,
+  import expressions inside f-strings will likely never be supported.
+* Due to python limitations, results of `import_expression.exec` will have no effect on the caller's globals or locals
+  without an explicit `globals` argument.
+* Unlike real operators, spaces before and after the import expression operator (such as `x ! .y`) are not supported.
+
+## [License](https://github.com/iomintz/import-expression-parser/blob/main/LICENSE)
+
+Copyright © 2018–2019 Io Mintz <<io@mintz.cc>>. All Rights Reserved. \
+Licensed under the MIT License. See the LICENSE file for details.
```

### Comparing `import_expression-1.1.4/import_expression.egg-info/SOURCES.txt` & `import_expression-1.1.5/import_expression.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,14 @@
+LICENSE
+LICENSE-header
 MANIFEST.in
 README.md
 import_expression.pth
 setup.py
+tests.py
 import_expression/__init__.py
 import_expression/__main__.py
 import_expression/_main2.py
 import_expression/_parser.py
 import_expression/_syntax.py
 import_expression/constants.py
 import_expression/version.py
```

### Comparing `import_expression-1.1.4/setup.py` & `import_expression-1.1.5/setup.py`

 * *Files identical despite different names*

