# Comparing `tmp/promptgen-0.0.1.tar.gz` & `tmp/promptgen-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptgen-0.0.1.tar", last modified: Thu May 23 06:16:15 2024, max compression
+gzip compressed data, was "promptgen-0.0.2.tar", last modified: Fri May 24 23:33:01 2024, max compression
```

## Comparing `promptgen-0.0.1.tar` & `promptgen-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 06:16:15.460519 promptgen-0.0.1/
--rw-rw-rw-   0        0        0    35823 2024-05-23 05:19:57.000000 promptgen-0.0.1/LICENSE
--rw-rw-rw-   0        0        0    43467 2024-05-23 06:16:15.459519 promptgen-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1696 2024-05-23 06:05:01.000000 promptgen-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 06:16:15.440519 promptgen-0.0.1/promptgen/
--rw-rw-rw-   0        0        0      189 2024-05-23 05:19:57.000000 promptgen-0.0.1/promptgen/__init__.py
--rw-rw-rw-   0        0        0    25090 2024-05-23 05:19:57.000000 promptgen-0.0.1/promptgen/promptgen.py
-drwxrwxrwx   0        0        0        0 2024-05-23 06:16:15.458520 promptgen-0.0.1/promptgen.egg-info/
--rw-rw-rw-   0        0        0    43467 2024-05-23 06:16:15.000000 promptgen-0.0.1/promptgen.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      241 2024-05-23 06:16:15.000000 promptgen-0.0.1/promptgen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 06:16:15.000000 promptgen-0.0.1/promptgen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-05-23 06:16:15.000000 promptgen-0.0.1/promptgen.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-23 06:16:15.000000 promptgen-0.0.1/promptgen.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      775 2024-05-23 06:12:33.000000 promptgen-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-23 06:16:15.460519 promptgen-0.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-24 23:33:01.165634 promptgen-0.0.2/
+-rw-rw-rw-   0        0        0    35823 2024-05-21 23:17:03.000000 promptgen-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0    43632 2024-05-24 23:33:01.162627 promptgen-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1861 2024-05-24 23:18:35.000000 promptgen-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-24 23:33:01.115998 promptgen-0.0.2/promptgen/
+-rw-rw-rw-   0        0        0      205 2024-05-24 20:28:09.000000 promptgen-0.0.2/promptgen/__init__.py
+-rw-rw-rw-   0        0        0     5824 2024-05-24 21:08:09.000000 promptgen-0.0.2/promptgen/parsetab.py
+-rw-rw-rw-   0        0        0    25717 2024-05-24 21:14:31.000000 promptgen-0.0.2/promptgen/promptgen.py
+drwxrwxrwx   0        0        0        0 2024-05-24 23:33:01.157750 promptgen-0.0.2/promptgen.egg-info/
+-rw-rw-rw-   0        0        0    43632 2024-05-24 23:33:00.000000 promptgen-0.0.2/promptgen.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      263 2024-05-24 23:33:00.000000 promptgen-0.0.2/promptgen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 23:33:00.000000 promptgen-0.0.2/promptgen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-24 23:33:00.000000 promptgen-0.0.2/promptgen.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-24 23:33:00.000000 promptgen-0.0.2/promptgen.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      775 2024-05-24 23:32:37.000000 promptgen-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-24 23:33:01.166909 promptgen-0.0.2/setup.cfg
```

### Comparing `promptgen-0.0.1/LICENSE` & `promptgen-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `promptgen-0.0.1/PKG-INFO` & `promptgen-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptgen
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python Parser to generate lists of prompts from a line of script(s)
 Author-email: Tony Beeman <beeman@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -717,11 +717,18 @@
 # ForEach Command
 foreach( array_cmd, [repeat = 1], [index = 0])
 Creates new prompts, which means batch_count will be ignored.
 The parser will walk through the current list of prompts, and repeat each item once (or more times if repeat > 1).
 expands will be processed in the order of the indexes, then in order they appear in the list.
 
 # Basic Math
-{{2 + 3}} will generate 5, etc. Correct operator precedence in NYI
-
-
+{{2 + 3}} will generate 5, etc.
 
+# Tests:
+To run tests:
+python .\test.py
+
+To change tests, update test.json, then run:
+python .\test.py --save_tests
+Finally, copy test_output.json to test.json and run
+python .\test.py
+To verify
```

### Comparing `promptgen-0.0.1/README.md` & `promptgen-0.0.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -27,11 +27,18 @@
 # ForEach Command
 foreach( array_cmd, [repeat = 1], [index = 0])
 Creates new prompts, which means batch_count will be ignored.
 The parser will walk through the current list of prompts, and repeat each item once (or more times if repeat > 1).
 expands will be processed in the order of the indexes, then in order they appear in the list.
 
 # Basic Math
-{{2 + 3}} will generate 5, etc. Correct operator precedence in NYI
-
+{{2 + 3}} will generate 5, etc.
 
+# Tests:
+To run tests:
+python .\test.py
 
+To change tests, update test.json, then run:
+python .\test.py --save_tests
+Finally, copy test_output.json to test.json and run
+python .\test.py
+To verify
```

### Comparing `promptgen-0.0.1/promptgen/promptgen.py` & `promptgen-0.0.2/promptgen/promptgen.py`

 * *Files 5% similar despite different names*

```diff
@@ -295,62 +295,65 @@
         except TypeError as te:
             print(f"self.m_children is not iterable in {self.m_type}")
         return processed_children
 
 
     def process_this(self, processed_children, state: GlobalState, global_iteration, stack_depth):
         res = None
-        match self.m_type:
-            case "func":
-                res = self.run_func(self.m_leaf, processed_children[0], global_iteration, state)
-            case "arglist":
-                res = processed_children
-            case "array":
-                res = processed_children[0]
-            case "binop":
-                try:
-                    print(f"{type(processed_children[0])} {self.m_leaf} {type(processed_children[1])}")
+        try:
+            match self.m_type:
+                case "func":
+                    res = self.run_func(self.m_leaf, processed_children[0], global_iteration, state)
+                case "arglist":
+                    res = processed_children
+                case "array":
+                    res = processed_children[0]
+                case "binop":                    
                     match self.m_leaf:
                         case "+":
                             res = processed_children[0] + processed_children[1]
                         case "-":
                             res = processed_children[0] - processed_children[1]
                         case "*":
                             res = processed_children[0] * processed_children[1]
                         case "/":
                             res = processed_children[0] / processed_children[1]
                         case "%":
                             res = processed_children[0] % processed_children[1]
-                except Exception as ex:
-                    res = f"FAILED{self.m_leaf}"
-                    print(f"Failed Binary Operation: {self.m_leaf}, Exception: {str(ex)}")
-            case "id":
-                match self.m_leaf:
-                    case "batch_size":
-                        res = state.batch_size
-                    case "batch_count":
-                        res = state.batch_count
-                    case "iteration":
-                        res = global_iteration
-                    case "prompt_count":
-                        res = state.prompt_count
-                    case _:
-                        res = self.m_leaf
-            case "constant":
-                res = self.m_leaf    
-            case "list":
-                res = state.get_list(processed_children[0].lower())
-            case "foreachargs":
-                res = processed_children[0]
-            case "passthru":
-                res = processed_children[0]
-            case _:
-                print(f"Unknown Type {self.m_type}")
-                res = processed_children[0]
-
+                case "unop":
+                    match self.m_leaf:
+                        case "-":
+                            res = -1 * processed_children[0]
+                case "id":
+                    match self.m_leaf:
+                        case "batch_size":
+                            res = state.batch_size
+                        case "batch_count":
+                            res = state.batch_count
+                        case "iteration":
+                            res = global_iteration
+                        case "prompt_count":
+                            res = state.prompt_count
+                        case _:
+                            res = self.m_leaf
+                case "constant":
+                    res = self.m_leaf    
+                case "list":
+                    res = state.get_list(processed_children[0].lower())
+                case "foreachargs":
+                    res = processed_children[0]
+                case "passthru":
+                    res = processed_children[0]
+                case _:
+                    print(f"Unknown Type {self.m_type}")
+                    res = ""
+        except Exception as ex:
+            res = f"FAILED{self.m_leaf}"
+            print(f"Failed Binary Operation: {self.m_leaf}, Exception: {str(ex)}")
+ 
         return res
 
 
     def process(self, state: GlobalState, global_iteration, stack_depth=0):
         tab = ' ' * stack_depth
         leafstring = ('(' + str(self.m_leaf) + ')') if self.m_leaf is not None else ''
         nodestring = f"{self.m_type + leafstring} node"
@@ -490,14 +493,15 @@
         return 0xFF * self.index + self.original_index
 
 def p_statement_expr(p):
     'statement : expression'
     p[0] = ParseNodeRoot("passthru", [ p[1] ] )
 
 # foreach( array_cmd, [repeat = 1], [index = 0] )
+
 def p_statement_foreach(p):
     'statement : FOREACH LPAREN foreachargs RPAREN'
     p[0] = ParseNodeRoot("foreach", [ p[3] ] )
 
 def p_foreachargs_onearg(p):
     'foreachargs : expression'
     p[0] = ParseNode('foreachargs', [ p[1] ])
@@ -506,51 +510,51 @@
     'foreachargs : expression COMMA NUMBER'
     p[0] = ParseNode('foreachargs', [ p[1], ParseNode("constant", [], p[3] ) ])
 
 def p_foreachargs_threearg(p):
     'foreachargs : expression COMMA NUMBER COMMA NUMBER'
     p[0] = ParseNode('foreachargs', [ p[1], ParseNode("constant", [], p[3]), ParseNode("constant", [], p[5] ) ] )
 
+# expressions
+
 def p_expression_id(p):
     'expression : ID'
     p[0] = ParseNode("id", [], p[1])
 
+def p_expression_parenthesis(p):
+    'expression : LPAREN expression RPAREN'
+    p[0] = ParseNode("passthru", [ p[2] ])
+
+# function calls
+
 def p_expression_func(p):
     'expression : ID LPAREN arglist RPAREN'
     p[0] = ParseNode("func", [ p[3] ], p[1] )
 
 def p_arglist_args(p):
     'arglist : expression COMMA arglist'
     p[3].insert_child(0, p[1])
     p[0] = p[3]
 
 def p_arglist_expr(p):
     'arglist : expression'
     p[0] = ParseNode("arglist", [ p[1] ])
 
 # Math
-def p_expression_add(p):
-    'expression : expression PLUS expression'
-    p[0] = ParseNode("binop", [ p[1], p[3] ], "+")
-
-def p_expression_sub(p):
-    'expression : expression MINUS expression'
-    p[0] = ParseNode("binop", [ p[1], p[3] ], "-")
-
-def p_expression_mult(p):
-    'expression : expression MULT expression'
-    p[0] = ParseNode("binop", [ p[1], p[3] ], "*")
-
-def p_expression_div(p):
-    'expression : expression DIV expression'
-    p[0] = ParseNode("binop", [ p[1], p[3] ], "/")
-
-def p_expression_mod(p):
-    'expression : expression MOD expression'
-    p[0] = ParseNode("binop", [ p[1], p[3] ], "%")
+def p_expression_binop(p):
+    '''expression : expression PLUS expression
+                 | expression MINUS expression
+                 | expression MULT expression
+                 | expression DIV expression
+                 | expression MOD expression'''
+    p[0] = ParseNode("binop", [ p[1], p[3] ], p[2])
+
+def p_expression_unop(p):
+    'expression : MINUS expression'
+    p[0] = ParseNode("unop", [ p[2] ], p[1])
 
 # Arrays
 
 def p_expression_array(p):
     'expression : array'
     p[0] = p[1]
 
@@ -569,76 +573,77 @@
     'expression : constant'
     p[0] = p[1]
 
 def p_constant_string(p):
     'constant : STRING'
     p[0] = ParseNode("constant", [], p[1].strip('"') )
 
-def p_constant_neg_number(p):
-    'constant : MINUS NUMBER'
-    p[0] = ParseNode("constant", [], -1 * p[1])
-
 def p_constant_number(p):
     'constant : NUMBER'
     p[0] = ParseNode("constant", [], p[1] )
 
-
 def p_error(p):
     print(f"Syntax error in input: {p}")
 
-# Build the parser
-g_parser = yacc.yacc()
 
+#precedence
+
+precedence = (
+    ('left', 'PLUS', 'MINUS'),
+    ('left', 'MULT', 'DIV'),
+)
 
+# Build the parser
+g_parser = yacc.yacc()
 
 class CodeSpan:
-    m_raw = ""
+    m_raw_span = ""
     m_tokens = None
     m_tree:ParseNodeRoot = None
     m_db = None
     m_orig_index = 0
 
     def __init__(self, raw_code, orig_index):
         global g_lexer
         global g_debug_lexer
 
-        self.m_raw = raw_code
+        self.m_raw_span = raw_code
         self.m_tokens = []
         self.m_tree = None
         self.m_orig_index = orig_index
 
     def get_tokens(self):        
         if (len(self.m_tokens) == 0):
-            g_lexer.input(self.m_raw)
+            g_lexer.input(self.m_raw_span)
             while True:
                 tok = g_lexer.token()
                 if not tok:
                     break
                 self.m_tokens.append(tok)
 
         return self.m_tokens
     
     def get_raw_code(self):
-        return self.m_raw
+        return self.m_raw_span
     
     def describe_self(self):
-        s = f"Raw Code: {self.m_raw}\n" 
+        s = f"Raw Code: {self.m_raw_span}\n" 
         for t in self.m_tokens:
             s += f"{str(t)};"
         s += "\n"
         return s        
     
     def get_parse_root(self) -> ParseNodeRoot:
         global g_parser
         if (self.m_tree is None):
             #try:
-                self.m_tree = g_parser.parse(self.m_raw)
+                self.m_tree = g_parser.parse(self.m_raw_span)
                 self.m_tree.original_index = self.m_orig_index
             #except Exception as ex:
-            #    print(f"Parse Exception parsing {self.m_raw}")
+            #    print(f"Parse Exception parsing {self.m_raw_span}")
             #    print(type(ex))
             #    print(ex.args)
             #    print(ex)
         return self.m_tree
 
 
 class Prompt:
@@ -664,36 +669,36 @@
     @seed.setter
     def seed(self, value: int):
         self.m_seed = value
 
 
 class TemplateParser:
     m_codes: list[CodeSpan]
-    m_raw: str
+    m_raw_template: str
     m_state: GlobalState = None
 
     def __init__(self):
         self.m_codes = []
         self.m_state = GlobalState()
         self.m_state.batch_count = 2
         self.m_state.batch_size = 4
         return
     
     @property
     def raw_prompt(self):
-        return self.m_raw
+        return self.m_raw_template
     
     @raw_prompt.setter
     def raw_prompt(self, value):
-        self.m_raw = value
+        self.m_raw_template = value
         self.m_codes = []
         # Add strings between {{ and }} to codes
         rx = r'{{(?P<code>([^}]|}[^}])*)}}'
         i = 0
-        for m in re.finditer(rx, self.m_raw):
+        for m in re.finditer(rx, self.m_raw_template):
             c = m.group('code')
             if (c is not None):
                 self.m_codes.append(CodeSpan(c, i))
                 i += 1
 
     @property
     def batch_size(self):
@@ -734,43 +739,54 @@
 
         prompts = []
         self.m_state.prompt_count = count
         for i in range(0, count):
             prompts.append(self.produce_prompt(i))
         return prompts
 
+    def debug_template(self):
+        output = f"------\nDEBUGGING {self.m_raw_template}\n------\n"
+        output += self.get_token_prompt()
+        output += "------"
+        return output
+    
     def get_token_prompt(self):
-        output = self.m_raw
+        output = self.m_raw_template
         for c in self.m_codes:
             res = " ".join(str(x) for x in c.get_tokens())
             raw = "{{" + c.get_raw_code() + "}}"
             output = output.replace(raw, str(res))
         return output
     
     def add_callback_handler(self, callback_handler: CallbackHandler):
         self.m_state.add_callback_handler(callback_handler)
 
     def produce_prompt(self, iteration):
-        output = self.m_raw
+        output = self.m_raw_template
         for c in self.m_codes:
             res = c.get_parse_root().process(self.m_state, iteration)
             raw = "{{" + c.get_raw_code() + "}}"
             output = output.replace(raw, str(res))
         return output
 
     def describe_self(self):
         s = "PARSER:\n"
-        s += f"Raw Prompt: {self.m_raw}\n"
+        s += f"Raw Prompt: {self.m_raw_template}\n"
         s += f"CODES\n----\n"
         for c in self.m_codes:
             s += c.describe_self()
         return s
 
 
 def generate_prompts(template: str, batch_count = 1, batch_size = 1, callback_handler: CallbackHandler = None):
     parser = TemplateParser()
     parser.batch_size = batch_size
     parser.batch_count = batch_count
     parser.raw_prompt = template
     parser.add_callback_handler(callback_handler)
     return parser.get_all_prompts()
 
+def debug_template(template: str, callback_handler: CallbackHandler = None):
+    parser = TemplateParser()
+    parser.raw_prompt = template
+    parser.add_callback_handler(callback_handler)
+    return parser.debug_template()
```

### Comparing `promptgen-0.0.1/promptgen.egg-info/PKG-INFO` & `promptgen-0.0.2/promptgen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptgen
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python Parser to generate lists of prompts from a line of script(s)
 Author-email: Tony Beeman <beeman@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -717,11 +717,18 @@
 # ForEach Command
 foreach( array_cmd, [repeat = 1], [index = 0])
 Creates new prompts, which means batch_count will be ignored.
 The parser will walk through the current list of prompts, and repeat each item once (or more times if repeat > 1).
 expands will be processed in the order of the indexes, then in order they appear in the list.
 
 # Basic Math
-{{2 + 3}} will generate 5, etc. Correct operator precedence in NYI
-
-
+{{2 + 3}} will generate 5, etc.
 
+# Tests:
+To run tests:
+python .\test.py
+
+To change tests, update test.json, then run:
+python .\test.py --save_tests
+Finally, copy test_output.json to test.json and run
+python .\test.py
+To verify
```

### Comparing `promptgen-0.0.1/pyproject.toml` & `promptgen-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "promptgen"
-version = "0.0.1"
+version = "0.0.2"
 description = "Python Parser to generate lists of prompts from a line of script(s)"
 readme = "README.md"
 authors = [{ name = "Tony Beeman", email = "beeman@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License (GPL)",
     "Programming Language :: Python",
```

