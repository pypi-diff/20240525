# Comparing `tmp/liveflask-1.0.9rc5.tar.gz` & `tmp/liveflask-1.0.9rc6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liveflask-1.0.9rc5.tar", last modified: Thu May  9 12:05:02 2024, max compression
+gzip compressed data, was "liveflask-1.0.9rc6.tar", last modified: Thu May  9 17:13:43 2024, max compression
```

## Comparing `liveflask-1.0.9rc5.tar` & `liveflask-1.0.9rc6.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 12:05:02.325068 liveflask-1.0.9rc5/
--rw-rw-rw-   0        0        0     1371 2024-05-09 12:05:02.324069 liveflask-1.0.9rc5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-09 12:05:02.264068 liveflask-1.0.9rc5/liveflask/
--rw-rw-rw-   0        0        0     6326 2024-05-08 12:07:33.000000 liveflask-1.0.9rc5/liveflask/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 12:05:02.275068 liveflask-1.0.9rc5/liveflask/attributes/
--rw-rw-rw-   0        0        0     2023 2024-05-01 21:07:09.000000 liveflask-1.0.9rc5/liveflask/attributes/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 12:05:02.277068 liveflask-1.0.9rc5/liveflask/attributes/__pycache__/
--rw-rw-rw-   0        0        0     3650 2024-05-01 21:07:09.000000 liveflask-1.0.9rc5/liveflask/attributes/__pycache__/__init__.cpython-311.pyc
-drwxrwxrwx   0        0        0        0 2024-05-09 12:05:02.279069 liveflask-1.0.9rc5/liveflask/static/
-drwxrwxrwx   0        0        0        0 2024-05-09 12:05:02.294068 liveflask-1.0.9rc5/liveflask/static/liveflask/
--rw-rw-rw-   0        0        0     4161 2024-05-09 10:51:01.000000 liveflask-1.0.9rc5/liveflask/static/liveflask/action.js
--rw-rw-rw-   0        0        0        0 2024-05-01 21:07:09.000000 liveflask-1.0.9rc5/liveflask/static/liveflask/constants.js
--rw-rw-rw-   0        0        0      245 2024-05-01 21:07:09.000000 liveflask-1.0.9rc5/liveflask/static/liveflask/events.js
--rw-rw-rw-   0        0        0     1328 2024-05-09 00:40:19.000000 liveflask-1.0.9rc5/liveflask/static/liveflask/init.js
--rw-rw-rw-   0        0        0     1649 2024-05-09 12:00:18.000000 liveflask-1.0.9rc5/liveflask/static/liveflask/liveflask.js
--rw-rw-rw-   0        0        0     2191 2024-05-01 21:07:09.000000 liveflask-1.0.9rc5/liveflask/static/liveflask/model.js
--rw-rw-rw-   0        0        0     1660 2024-05-01 21:07:09.000000 liveflask-1.0.9rc5/liveflask/static/liveflask/polling.js
--rw-rw-rw-   0        0        0     9669 2024-05-09 12:00:26.000000 liveflask-1.0.9rc5/liveflask/static/liveflask/utils.js
--rw-rw-rw-   0        0        0    73154 2024-05-01 21:07:09.000000 liveflask-1.0.9rc5/liveflask/static/lodash.min.js
-drwxrwxrwx   0        0        0        0 2024-05-09 12:05:02.299068 liveflask-1.0.9rc5/liveflask/templates/
--rw-rw-rw-   0        0        0        0 2024-05-01 21:07:09.000000 liveflask-1.0.9rc5/liveflask/templates/liveflask-head.html
--rw-rw-rw-   0        0        0      348 2024-05-04 23:19:29.000000 liveflask-1.0.9rc5/liveflask/templates/liveflask-scripts.html
-drwxrwxrwx   0        0        0        0 2024-05-09 12:05:02.311068 liveflask-1.0.9rc5/liveflask/traits/
--rw-rw-rw-   0        0        0      205 2024-05-01 21:07:09.000000 liveflask-1.0.9rc5/liveflask/traits/Bootable.py
--rw-rw-rw-   0        0        0        0 2024-05-01 21:07:09.000000 liveflask-1.0.9rc5/liveflask/traits/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 12:05:02.321068 liveflask-1.0.9rc5/liveflask/traits/__pycache__/
--rw-rw-rw-   0        0        0      867 2024-05-01 21:07:09.000000 liveflask-1.0.9rc5/liveflask/traits/__pycache__/Bootable.cpython-311.pyc
--rw-rw-rw-   0        0        0      198 2024-05-01 21:07:09.000000 liveflask-1.0.9rc5/liveflask/traits/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     3292 2024-05-01 21:07:09.000000 liveflask-1.0.9rc5/liveflask/traits/__pycache__/has_actions.cpython-311.pyc
--rw-rw-rw-   0        0        0     4272 2024-05-01 21:07:09.000000 liveflask-1.0.9rc5/liveflask/traits/__pycache__/has_props.cpython-311.pyc
--rw-rw-rw-   0        0        0     2835 2024-05-01 21:07:09.000000 liveflask-1.0.9rc5/liveflask/traits/__pycache__/has_renders.cpython-311.pyc
--rw-rw-rw-   0        0        0     4776 2024-05-01 21:07:09.000000 liveflask-1.0.9rc5/liveflask/traits/__pycache__/has_snapshots.cpython-311.pyc
--rw-rw-rw-   0        0        0     2042 2024-05-01 21:07:09.000000 liveflask-1.0.9rc5/liveflask/traits/has_actions.py
--rw-rw-rw-   0        0        0     2488 2024-05-01 21:07:09.000000 liveflask-1.0.9rc5/liveflask/traits/has_props.py
--rw-rw-rw-   0        0        0     2486 2024-05-01 21:07:09.000000 liveflask-1.0.9rc5/liveflask/traits/has_renders.py
--rw-rw-rw-   0        0        0     4106 2024-05-01 21:07:09.000000 liveflask-1.0.9rc5/liveflask/traits/has_snapshots.py
--rw-rw-rw-   0        0        0     2032 2024-05-01 21:07:09.000000 liveflask-1.0.9rc5/liveflask/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-09 12:05:02.273068 liveflask-1.0.9rc5/liveflask.egg-info/
--rw-rw-rw-   0        0        0     1371 2024-05-09 12:05:02.000000 liveflask-1.0.9rc5/liveflask.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1239 2024-05-09 12:05:02.000000 liveflask-1.0.9rc5/liveflask.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 12:05:02.000000 liveflask-1.0.9rc5/liveflask.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2024-05-09 12:05:02.000000 liveflask-1.0.9rc5/liveflask.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-09 12:05:02.000000 liveflask-1.0.9rc5/liveflask.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-09 12:05:02.325068 liveflask-1.0.9rc5/setup.cfg
--rw-rw-rw-   0        0        0     1225 2024-05-09 12:04:59.000000 liveflask-1.0.9rc5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 17:13:43.198023 liveflask-1.0.9rc6/
+-rw-rw-rw-   0        0        0     1294 2024-05-09 17:13:43.198023 liveflask-1.0.9rc6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-09 17:13:43.147125 liveflask-1.0.9rc6/liveflask/
+-rw-rw-rw-   0        0        0     6326 2024-05-09 13:02:07.000000 liveflask-1.0.9rc6/liveflask/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 17:13:43.160125 liveflask-1.0.9rc6/liveflask/attributes/
+-rw-rw-rw-   0        0        0     2023 2024-05-09 13:02:07.000000 liveflask-1.0.9rc6/liveflask/attributes/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 17:13:43.161629 liveflask-1.0.9rc6/liveflask/attributes/__pycache__/
+-rw-rw-rw-   0        0        0     3654 2024-05-09 13:02:07.000000 liveflask-1.0.9rc6/liveflask/attributes/__pycache__/__init__.cpython-311.pyc
+drwxrwxrwx   0        0        0        0 2024-05-09 17:13:43.163234 liveflask-1.0.9rc6/liveflask/static/
+drwxrwxrwx   0        0        0        0 2024-05-09 17:13:43.174986 liveflask-1.0.9rc6/liveflask/static/liveflask/
+-rw-rw-rw-   0        0        0     4161 2024-05-09 13:02:07.000000 liveflask-1.0.9rc6/liveflask/static/liveflask/action.js
+-rw-rw-rw-   0        0        0        0 2024-05-09 13:02:07.000000 liveflask-1.0.9rc6/liveflask/static/liveflask/constants.js
+-rw-rw-rw-   0        0        0      245 2024-05-09 13:02:07.000000 liveflask-1.0.9rc6/liveflask/static/liveflask/events.js
+-rw-rw-rw-   0        0        0     1328 2024-05-09 13:02:07.000000 liveflask-1.0.9rc6/liveflask/static/liveflask/init.js
+-rw-rw-rw-   0        0        0     2300 2024-05-09 16:05:04.000000 liveflask-1.0.9rc6/liveflask/static/liveflask/liveflask.js
+-rw-rw-rw-   0        0        0     2191 2024-05-09 13:02:07.000000 liveflask-1.0.9rc6/liveflask/static/liveflask/model.js
+-rw-rw-rw-   0        0        0     1660 2024-05-09 13:02:07.000000 liveflask-1.0.9rc6/liveflask/static/liveflask/polling.js
+-rw-rw-rw-   0        0        0    10413 2024-05-09 13:31:18.000000 liveflask-1.0.9rc6/liveflask/static/liveflask/utils.js
+-rw-rw-rw-   0        0        0    73154 2024-05-09 13:02:07.000000 liveflask-1.0.9rc6/liveflask/static/lodash.min.js
+drwxrwxrwx   0        0        0        0 2024-05-09 17:13:43.177984 liveflask-1.0.9rc6/liveflask/templates/
+-rw-rw-rw-   0        0        0        0 2024-05-09 13:02:07.000000 liveflask-1.0.9rc6/liveflask/templates/liveflask-head.html
+-rw-rw-rw-   0        0        0      348 2024-05-09 13:02:07.000000 liveflask-1.0.9rc6/liveflask/templates/liveflask-scripts.html
+drwxrwxrwx   0        0        0        0 2024-05-09 17:13:43.185023 liveflask-1.0.9rc6/liveflask/traits/
+-rw-rw-rw-   0        0        0      205 2024-05-09 13:02:07.000000 liveflask-1.0.9rc6/liveflask/traits/Bootable.py
+-rw-rw-rw-   0        0        0        0 2024-05-09 13:02:07.000000 liveflask-1.0.9rc6/liveflask/traits/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 17:13:43.196023 liveflask-1.0.9rc6/liveflask/traits/__pycache__/
+-rw-rw-rw-   0        0        0      871 2024-05-09 13:02:07.000000 liveflask-1.0.9rc6/liveflask/traits/__pycache__/Bootable.cpython-311.pyc
+-rw-rw-rw-   0        0        0      202 2024-05-09 13:02:07.000000 liveflask-1.0.9rc6/liveflask/traits/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3296 2024-05-09 13:02:07.000000 liveflask-1.0.9rc6/liveflask/traits/__pycache__/has_actions.cpython-311.pyc
+-rw-rw-rw-   0        0        0     4276 2024-05-09 13:02:07.000000 liveflask-1.0.9rc6/liveflask/traits/__pycache__/has_props.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2839 2024-05-09 13:02:07.000000 liveflask-1.0.9rc6/liveflask/traits/__pycache__/has_renders.cpython-311.pyc
+-rw-rw-rw-   0        0        0     4780 2024-05-09 13:02:07.000000 liveflask-1.0.9rc6/liveflask/traits/__pycache__/has_snapshots.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2042 2024-05-09 13:02:07.000000 liveflask-1.0.9rc6/liveflask/traits/has_actions.py
+-rw-rw-rw-   0        0        0     2488 2024-05-09 13:02:07.000000 liveflask-1.0.9rc6/liveflask/traits/has_props.py
+-rw-rw-rw-   0        0        0     2486 2024-05-09 13:02:07.000000 liveflask-1.0.9rc6/liveflask/traits/has_renders.py
+-rw-rw-rw-   0        0        0     4106 2024-05-09 13:02:07.000000 liveflask-1.0.9rc6/liveflask/traits/has_snapshots.py
+-rw-rw-rw-   0        0        0     2032 2024-05-09 13:02:07.000000 liveflask-1.0.9rc6/liveflask/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-09 17:13:43.158125 liveflask-1.0.9rc6/liveflask.egg-info/
+-rw-rw-rw-   0        0        0     1294 2024-05-09 17:13:43.000000 liveflask-1.0.9rc6/liveflask.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1239 2024-05-09 17:13:43.000000 liveflask-1.0.9rc6/liveflask.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 17:13:43.000000 liveflask-1.0.9rc6/liveflask.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2024-05-09 17:13:43.000000 liveflask-1.0.9rc6/liveflask.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-09 17:13:43.000000 liveflask-1.0.9rc6/liveflask.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-09 17:13:43.198023 liveflask-1.0.9rc6/setup.cfg
+-rw-rw-rw-   0        0        0     1225 2024-05-09 17:11:28.000000 liveflask-1.0.9rc6/setup.py
```

### Comparing `liveflask-1.0.9rc5/PKG-INFO` & `liveflask-1.0.9rc6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 Metadata-Version: 2.1
 Name: liveflask
-Version: 1.0.9rc5
+Version: 1.0.9rc6
 Summary: Seamlessly integrate modern reactive components into Flask templates, eliminating the need for mastering new templating languages or wrestling with complex JavaScript frameworks. With our solution, developers can enhance their Flask applications with dynamic functionality while maintaining a familiar development environment, streamlining the process and ensuring a smoother user experience.
 Home-page: https://github.com/JarriqTheTechie/liveflask
 Author: Jarriq Rolle
 Author-email: jrolle@baysidetechgroup.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: flask
-Requires-Dist: masonite-orm
-Requires-Dist: Flask-WTF
 
 # LiveFlask
 
 LiveFlask is a comprehensive framework for Flask that simplifies the creation of dynamic interfaces, all within the
 familiar environment of Flask.
 
 # Install LiveFlask
```

### Comparing `liveflask-1.0.9rc5/liveflask/__init__.py` & `liveflask-1.0.9rc6/liveflask/__init__.py`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.9rc5/liveflask/attributes/__init__.py` & `liveflask-1.0.9rc6/liveflask/attributes/__init__.py`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.9rc5/liveflask/attributes/__pycache__/__init__.cpython-311.pyc` & `liveflask-1.0.9rc6/liveflask/attributes/__pycache__/__init__.cpython-311.pyc`

 * *Files 12% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xfdae3266 (Wed May  1 21:07:09 2024 UTC)
+moddate:  0x4fc93c66 (Thu May  9 13:02:07 2024 UTC)
 files sz: 2023
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
@@ -19,35 +19,35 @@
    
      4          10 LOAD_CONST               6 ((None,))
                 12 LOAD_CONST               2 ('arg')
                 14 LOAD_NAME                1 (list)
                 16 LOAD_CONST               1 (None)
                 18 BINARY_OP                7 (|)
                 22 BUILD_TUPLE              2
-                24 LOAD_CONST               3 (<code object url, file "C:\Users\jrolle\PycharmProjects\bleh\.venv\Lib\site-packages\liveflask/attributes/__init__.py", line 4>)
+                24 LOAD_CONST               3 (<code object url, file "C:\Users\jrolle\PycharmProjects\ITManager\venv\Lib\site-packages\liveflask/attributes/__init__.py", line 4>)
                 26 MAKE_FUNCTION            5 (defaults, annotations)
                 28 STORE_NAME               2 (url)
    
     24          30 LOAD_CONST               6 ((None,))
                 32 LOAD_CONST               2 ('arg')
                 34 LOAD_NAME                1 (list)
                 36 LOAD_CONST               1 (None)
                 38 BINARY_OP                7 (|)
                 42 BUILD_TUPLE              2
-                44 LOAD_CONST               4 (<code object locked, file "C:\Users\jrolle\PycharmProjects\bleh\.venv\Lib\site-packages\liveflask/attributes/__init__.py", line 24>)
+                44 LOAD_CONST               4 (<code object locked, file "C:\Users\jrolle\PycharmProjects\ITManager\venv\Lib\site-packages\liveflask/attributes/__init__.py", line 24>)
                 46 MAKE_FUNCTION            5 (defaults, annotations)
                 48 STORE_NAME               3 (locked)
    
     44          50 LOAD_CONST               6 ((None,))
                 52 LOAD_CONST               2 ('arg')
                 54 LOAD_NAME                1 (list)
                 56 LOAD_CONST               1 (None)
                 58 BINARY_OP                7 (|)
                 62 BUILD_TUPLE              2
-                64 LOAD_CONST               5 (<code object session, file "C:\Users\jrolle\PycharmProjects\bleh\.venv\Lib\site-packages\liveflask/attributes/__init__.py", line 44>)
+                64 LOAD_CONST               5 (<code object session, file "C:\Users\jrolle\PycharmProjects\ITManager\venv\Lib\site-packages\liveflask/attributes/__init__.py", line 44>)
                 66 MAKE_FUNCTION            5 (defaults, annotations)
                 68 STORE_NAME               4 (session)
                 70 LOAD_CONST               1 (None)
                 72 RETURN_VALUE
    consts
       0
       None
@@ -60,15 +60,15 @@
          code 0x8700970088006601640184087d017c015300
                        0 MAKE_CELL                0 (arg)
          
            4           2 RESUME                   0
          
            5           4 LOAD_CLOSURE             0 (arg)
                        6 BUILD_TUPLE              1
-                       8 LOAD_CONST               1 (<code object decorator, file "C:\Users\jrolle\PycharmProjects\bleh\.venv\Lib\site-packages\liveflask/attributes/__init__.py", line 5>)
+                       8 LOAD_CONST               1 (<code object decorator, file "C:\Users\jrolle\PycharmProjects\ITManager\venv\Lib\site-packages\liveflask/attributes/__init__.py", line 5>)
                       10 MAKE_FUNCTION            8 (closure)
                       12 STORE_FAST               1 (decorator)
          
           21          14 LOAD_FAST                1 (decorator)
                       16 RETURN_VALUE
          consts
             None
@@ -97,15 +97,15 @@
                             34 PRECALL                  2
                             38 CALL                     2
                
                  7          48 PUSH_NULL
                             50 LOAD_BUILD_CLASS
                             52 LOAD_CLOSURE             0 (cls)
                             54 BUILD_TUPLE              1
-                            56 LOAD_CONST               3 (<code object DecoratedClass, file "C:\Users\jrolle\PycharmProjects\bleh\.venv\Lib\site-packages\liveflask/attributes/__init__.py", line 6>)
+                            56 LOAD_CONST               3 (<code object DecoratedClass, file "C:\Users\jrolle\PycharmProjects\ITManager\venv\Lib\site-packages\liveflask/attributes/__init__.py", line 6>)
                             58 MAKE_FUNCTION            8 (closure)
                             60 LOAD_CONST               4 ('DecoratedClass')
                             62 LOAD_DEREF               0 (cls)
                             64 PRECALL                  3
                             68 CALL                     3
                
                  6          78 PRECALL                  0
@@ -156,15 +156,15 @@
                                    8 STORE_NAME               1 (__module__)
                                   10 LOAD_CONST               0 ('url.<locals>.decorator.<locals>.DecoratedClass')
                                   12 STORE_NAME               2 (__qualname__)
                      
                        8          14 LOAD_CLOSURE             0 (__class__)
                                   16 LOAD_CLOSURE             1 (cls)
                                   18 BUILD_TUPLE              2
-                                  20 LOAD_CONST               1 (<code object __init__, file "C:\Users\jrolle\PycharmProjects\bleh\.venv\Lib\site-packages\liveflask/attributes/__init__.py", line 8>)
+                                  20 LOAD_CONST               1 (<code object __init__, file "C:\Users\jrolle\PycharmProjects\ITManager\venv\Lib\site-packages\liveflask/attributes/__init__.py", line 8>)
                                   22 MAKE_FUNCTION            8 (closure)
                                   24 STORE_NAME               3 (__init__)
                                   26 LOAD_CLOSURE             0 (__class__)
                                   28 COPY                     1
                                   30 STORE_NAME               4 (__classcell__)
                                   32 RETURN_VALUE
                      consts
@@ -204,40 +204,40 @@
                                         90 RETURN_VALUE
                            consts
                               None
                            names      ('super', '__init__', '__name__', '__class__')
                            varnames   ('self', 'args', 'kwargs')
                            freevars   ('__class__', 'cls')
                            cellvars   ()
-                           filename   'C:\\Users\\jrolle\\PycharmProjects\\bleh\\.venv\\Lib\\site-packages\\liveflask/attributes/__init__.py'
+                           filename   'C:\\Users\\jrolle\\PycharmProjects\\ITManager\\venv\\Lib\\site-packages\\liveflask/attributes/__init__.py'
                            name       '__init__'
                            firstlineno 8
                            lnotab 0x04013201
                      names      ('__name__', '__module__', '__qualname__', '__init__', '__classcell__')
                      varnames   ()
                      freevars   ('cls',)
                      cellvars   ('__class__',)
-                     filename   'C:\\Users\\jrolle\\PycharmProjects\\bleh\\.venv\\Lib\\site-packages\\liveflask/attributes/__init__.py'
+                     filename   'C:\\Users\\jrolle\\PycharmProjects\\ITManager\\venv\\Lib\\site-packages\\liveflask/attributes/__init__.py'
                      name       'DecoratedClass'
                      firstlineno 6
                      lnotab 0x0e02
                   'DecoratedClass'
                names      ('functools', 'wraps', 'mvlive__url', 'append')
                varnames   ('cls', 'DecoratedClass', 'query_param')
                freevars   ('arg',)
                cellvars   ('cls',)
-               filename   'C:\\Users\\jrolle\\PycharmProjects\\bleh\\.venv\\Lib\\site-packages\\liveflask/attributes/__init__.py'
+               filename   'C:\\Users\\jrolle\\PycharmProjects\\ITManager\\venv\\Lib\\site-packages\\liveflask/attributes/__init__.py'
                name       'decorator'
                firstlineno 5
                lnotab 0x06012a011eff0e0102050e02040108033601
          names      ()
          varnames   ('arg', 'decorator')
          freevars   ()
          cellvars   ('arg',)
-         filename   'C:\\Users\\jrolle\\PycharmProjects\\bleh\\.venv\\Lib\\site-packages\\liveflask/attributes/__init__.py'
+         filename   'C:\\Users\\jrolle\\PycharmProjects\\ITManager\\venv\\Lib\\site-packages\\liveflask/attributes/__init__.py'
          name       'url'
          firstlineno 4
          lnotab 0x04010a10
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 2
@@ -245,15 +245,15 @@
          code 0x8700970088006601640184087d017c015300
                        0 MAKE_CELL                0 (arg)
          
           24           2 RESUME                   0
          
           25           4 LOAD_CLOSURE             0 (arg)
                        6 BUILD_TUPLE              1
-                       8 LOAD_CONST               1 (<code object decorator, file "C:\Users\jrolle\PycharmProjects\bleh\.venv\Lib\site-packages\liveflask/attributes/__init__.py", line 25>)
+                       8 LOAD_CONST               1 (<code object decorator, file "C:\Users\jrolle\PycharmProjects\ITManager\venv\Lib\site-packages\liveflask/attributes/__init__.py", line 25>)
                       10 MAKE_FUNCTION            8 (closure)
                       12 STORE_FAST               1 (decorator)
          
           41          14 LOAD_FAST                1 (decorator)
                       16 RETURN_VALUE
          consts
             None
@@ -282,15 +282,15 @@
                             34 PRECALL                  2
                             38 CALL                     2
                
                 27          48 PUSH_NULL
                             50 LOAD_BUILD_CLASS
                             52 LOAD_CLOSURE             0 (cls)
                             54 BUILD_TUPLE              1
-                            56 LOAD_CONST               3 (<code object DecoratedClass, file "C:\Users\jrolle\PycharmProjects\bleh\.venv\Lib\site-packages\liveflask/attributes/__init__.py", line 26>)
+                            56 LOAD_CONST               3 (<code object DecoratedClass, file "C:\Users\jrolle\PycharmProjects\ITManager\venv\Lib\site-packages\liveflask/attributes/__init__.py", line 26>)
                             58 MAKE_FUNCTION            8 (closure)
                             60 LOAD_CONST               4 ('DecoratedClass')
                             62 LOAD_DEREF               0 (cls)
                             64 PRECALL                  3
                             68 CALL                     3
                
                 26          78 PRECALL                  0
@@ -341,15 +341,15 @@
                                    8 STORE_NAME               1 (__module__)
                                   10 LOAD_CONST               0 ('locked.<locals>.decorator.<locals>.DecoratedClass')
                                   12 STORE_NAME               2 (__qualname__)
                      
                       28          14 LOAD_CLOSURE             0 (__class__)
                                   16 LOAD_CLOSURE             1 (cls)
                                   18 BUILD_TUPLE              2
-                                  20 LOAD_CONST               1 (<code object __init__, file "C:\Users\jrolle\PycharmProjects\bleh\.venv\Lib\site-packages\liveflask/attributes/__init__.py", line 28>)
+                                  20 LOAD_CONST               1 (<code object __init__, file "C:\Users\jrolle\PycharmProjects\ITManager\venv\Lib\site-packages\liveflask/attributes/__init__.py", line 28>)
                                   22 MAKE_FUNCTION            8 (closure)
                                   24 STORE_NAME               3 (__init__)
                                   26 LOAD_CLOSURE             0 (__class__)
                                   28 COPY                     1
                                   30 STORE_NAME               4 (__classcell__)
                                   32 RETURN_VALUE
                      consts
@@ -389,40 +389,40 @@
                                         90 RETURN_VALUE
                            consts
                               None
                            names      ('super', '__init__', '__name__', '__class__')
                            varnames   ('self', 'args', 'kwargs')
                            freevars   ('__class__', 'cls')
                            cellvars   ()
-                           filename   'C:\\Users\\jrolle\\PycharmProjects\\bleh\\.venv\\Lib\\site-packages\\liveflask/attributes/__init__.py'
+                           filename   'C:\\Users\\jrolle\\PycharmProjects\\ITManager\\venv\\Lib\\site-packages\\liveflask/attributes/__init__.py'
                            name       '__init__'
                            firstlineno 28
                            lnotab 0x04013201
                      names      ('__name__', '__module__', '__qualname__', '__init__', '__classcell__')
                      varnames   ()
                      freevars   ('cls',)
                      cellvars   ('__class__',)
-                     filename   'C:\\Users\\jrolle\\PycharmProjects\\bleh\\.venv\\Lib\\site-packages\\liveflask/attributes/__init__.py'
+                     filename   'C:\\Users\\jrolle\\PycharmProjects\\ITManager\\venv\\Lib\\site-packages\\liveflask/attributes/__init__.py'
                      name       'DecoratedClass'
                      firstlineno 26
                      lnotab 0x0e02
                   'DecoratedClass'
                names      ('functools', 'wraps', 'mvlive__locked', 'append')
                varnames   ('cls', 'DecoratedClass', 'locked_prop')
                freevars   ('arg',)
                cellvars   ('cls',)
-               filename   'C:\\Users\\jrolle\\PycharmProjects\\bleh\\.venv\\Lib\\site-packages\\liveflask/attributes/__init__.py'
+               filename   'C:\\Users\\jrolle\\PycharmProjects\\ITManager\\venv\\Lib\\site-packages\\liveflask/attributes/__init__.py'
                name       'decorator'
                firstlineno 25
                lnotab 0x06012a011eff0e0102050e02040108033601
          names      ()
          varnames   ('arg', 'decorator')
          freevars   ()
          cellvars   ('arg',)
-         filename   'C:\\Users\\jrolle\\PycharmProjects\\bleh\\.venv\\Lib\\site-packages\\liveflask/attributes/__init__.py'
+         filename   'C:\\Users\\jrolle\\PycharmProjects\\ITManager\\venv\\Lib\\site-packages\\liveflask/attributes/__init__.py'
          name       'locked'
          firstlineno 24
          lnotab 0x04010a10
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 2
@@ -430,15 +430,15 @@
          code 0x8700970088006601640184087d017c015300
                        0 MAKE_CELL                0 (arg)
          
           44           2 RESUME                   0
          
           45           4 LOAD_CLOSURE             0 (arg)
                        6 BUILD_TUPLE              1
-                       8 LOAD_CONST               1 (<code object decorator, file "C:\Users\jrolle\PycharmProjects\bleh\.venv\Lib\site-packages\liveflask/attributes/__init__.py", line 45>)
+                       8 LOAD_CONST               1 (<code object decorator, file "C:\Users\jrolle\PycharmProjects\ITManager\venv\Lib\site-packages\liveflask/attributes/__init__.py", line 45>)
                       10 MAKE_FUNCTION            8 (closure)
                       12 STORE_FAST               1 (decorator)
          
           61          14 LOAD_FAST                1 (decorator)
                       16 RETURN_VALUE
          consts
             None
@@ -467,15 +467,15 @@
                             34 PRECALL                  2
                             38 CALL                     2
                
                 47          48 PUSH_NULL
                             50 LOAD_BUILD_CLASS
                             52 LOAD_CLOSURE             0 (cls)
                             54 BUILD_TUPLE              1
-                            56 LOAD_CONST               3 (<code object DecoratedClass, file "C:\Users\jrolle\PycharmProjects\bleh\.venv\Lib\site-packages\liveflask/attributes/__init__.py", line 46>)
+                            56 LOAD_CONST               3 (<code object DecoratedClass, file "C:\Users\jrolle\PycharmProjects\ITManager\venv\Lib\site-packages\liveflask/attributes/__init__.py", line 46>)
                             58 MAKE_FUNCTION            8 (closure)
                             60 LOAD_CONST               4 ('DecoratedClass')
                             62 LOAD_DEREF               0 (cls)
                             64 PRECALL                  3
                             68 CALL                     3
                
                 46          78 PRECALL                  0
@@ -526,15 +526,15 @@
                                    8 STORE_NAME               1 (__module__)
                                   10 LOAD_CONST               0 ('session.<locals>.decorator.<locals>.DecoratedClass')
                                   12 STORE_NAME               2 (__qualname__)
                      
                       48          14 LOAD_CLOSURE             0 (__class__)
                                   16 LOAD_CLOSURE             1 (cls)
                                   18 BUILD_TUPLE              2
-                                  20 LOAD_CONST               1 (<code object __init__, file "C:\Users\jrolle\PycharmProjects\bleh\.venv\Lib\site-packages\liveflask/attributes/__init__.py", line 48>)
+                                  20 LOAD_CONST               1 (<code object __init__, file "C:\Users\jrolle\PycharmProjects\ITManager\venv\Lib\site-packages\liveflask/attributes/__init__.py", line 48>)
                                   22 MAKE_FUNCTION            8 (closure)
                                   24 STORE_NAME               3 (__init__)
                                   26 LOAD_CLOSURE             0 (__class__)
                                   28 COPY                     1
                                   30 STORE_NAME               4 (__classcell__)
                                   32 RETURN_VALUE
                      consts
@@ -574,45 +574,45 @@
                                         90 RETURN_VALUE
                            consts
                               None
                            names      ('super', '__init__', '__name__', '__class__')
                            varnames   ('self', 'args', 'kwargs')
                            freevars   ('__class__', 'cls')
                            cellvars   ()
-                           filename   'C:\\Users\\jrolle\\PycharmProjects\\bleh\\.venv\\Lib\\site-packages\\liveflask/attributes/__init__.py'
+                           filename   'C:\\Users\\jrolle\\PycharmProjects\\ITManager\\venv\\Lib\\site-packages\\liveflask/attributes/__init__.py'
                            name       '__init__'
                            firstlineno 48
                            lnotab 0x04013201
                      names      ('__name__', '__module__', '__qualname__', '__init__', '__classcell__')
                      varnames   ()
                      freevars   ('cls',)
                      cellvars   ('__class__',)
-                     filename   'C:\\Users\\jrolle\\PycharmProjects\\bleh\\.venv\\Lib\\site-packages\\liveflask/attributes/__init__.py'
+                     filename   'C:\\Users\\jrolle\\PycharmProjects\\ITManager\\venv\\Lib\\site-packages\\liveflask/attributes/__init__.py'
                      name       'DecoratedClass'
                      firstlineno 46
                      lnotab 0x0e02
                   'DecoratedClass'
                names      ('functools', 'wraps', 'mvlive__session', 'append')
                varnames   ('cls', 'DecoratedClass', 'session_binded_prop')
                freevars   ('arg',)
                cellvars   ('cls',)
-               filename   'C:\\Users\\jrolle\\PycharmProjects\\bleh\\.venv\\Lib\\site-packages\\liveflask/attributes/__init__.py'
+               filename   'C:\\Users\\jrolle\\PycharmProjects\\ITManager\\venv\\Lib\\site-packages\\liveflask/attributes/__init__.py'
                name       'decorator'
                firstlineno 45
                lnotab 0x06012a011eff0e0102050e02040108033601
          names      ()
          varnames   ('arg', 'decorator')
          freevars   ()
          cellvars   ('arg',)
-         filename   'C:\\Users\\jrolle\\PycharmProjects\\bleh\\.venv\\Lib\\site-packages\\liveflask/attributes/__init__.py'
+         filename   'C:\\Users\\jrolle\\PycharmProjects\\ITManager\\venv\\Lib\\site-packages\\liveflask/attributes/__init__.py'
          name       'session'
          firstlineno 44
          lnotab 0x04010a10
       (None,)
    names      ('functools', 'list', 'url', 'locked', 'session')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'C:\\Users\\jrolle\\PycharmProjects\\bleh\\.venv\\Lib\\site-packages\\liveflask/attributes/__init__.py'
+   filename   'C:\\Users\\jrolle\\PycharmProjects\\ITManager\\venv\\Lib\\site-packages\\liveflask/attributes/__init__.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff0201080314141414
```

### Comparing `liveflask-1.0.9rc5/liveflask/static/liveflask/action.js` & `liveflask-1.0.9rc6/liveflask/static/liveflask/action.js`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.9rc5/liveflask/static/liveflask/init.js` & `liveflask-1.0.9rc6/liveflask/static/liveflask/init.js`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.9rc5/liveflask/static/liveflask/model.js` & `liveflask-1.0.9rc6/liveflask/static/liveflask/model.js`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.9rc5/liveflask/static/liveflask/polling.js` & `liveflask-1.0.9rc6/liveflask/static/liveflask/polling.js`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.9rc5/liveflask/static/liveflask/utils.js` & `liveflask-1.0.9rc6/liveflask/static/liveflask/utils.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -127,16 +127,32 @@
 function send_request(el, add_to_payload, target) {
     let updated_element;
     let emits;
     let snapshot = el.__liveflask
     let children = attr_beginswith('data-component', el);
     let elementsWithDataLoading = el.querySelectorAll('[data-loading]');
     elementsWithDataLoading.forEach(element => {
-        console.log("Element with data-loading: ", element);
-        element.style.display = "block";
+        if (element.hasAttribute("data-loading-target")) {
+            let loading_target = element.getAttribute("data-loading-target");
+            if (loading_target && loading_target.includes(',')) {
+                loading_target = loading_target.split(',').map(item => item.trim());
+
+                // Now loading_target is an array containing the split values
+            } else {
+                loading_target = [loading_target];
+            }
+
+            let target_action_or_model = target.getAttribute("data-action") || target.getAttribute("data-model");
+            console.log("Loading Target: ", loading_target)
+            if (loading_target.includes(target_action_or_model)) {
+                element.style.display = "block";
+            }
+        } else {
+            element.style.display = "block";
+        }
     });
 
     fetch("/liveflask/", {
         method: "POST",
         headers: {
             "Content-Type": "application/json",
             "X-CSRF-Token": csrfToken
```

### Comparing `liveflask-1.0.9rc5/liveflask/static/lodash.min.js` & `liveflask-1.0.9rc6/liveflask/static/lodash.min.js`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.9rc5/liveflask/traits/__pycache__/Bootable.cpython-311.pyc` & `liveflask-1.0.9rc6/liveflask/traits/__pycache__/Bootable.cpython-311.pyc`

 * *Files 18% similar despite different names*

#### Python bytecode

```diff
@@ -1,23 +1,23 @@
 magic:    0xa70d0d0a
-moddate:  0xfdae3266 (Wed May  1 21:07:09 2024 UTC)
+moddate:  0x4fc93c66 (Thu May  9 13:02:07 2024 UTC)
 files sz: 205
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
       0x970002004700640084006401a6020000ab0200000000000000005a0064
       025300
      0           0 RESUME                   0
    
      1           2 PUSH_NULL
                  4 LOAD_BUILD_CLASS
-                 6 LOAD_CONST               0 (<code object Bootable, file "C:\Users\jrolle\PycharmProjects\bleh\.venv\Lib\site-packages\liveflask/traits/Bootable.py", line 1>)
+                 6 LOAD_CONST               0 (<code object Bootable, file "C:\Users\jrolle\PycharmProjects\ITManager\venv\Lib\site-packages\liveflask/traits/Bootable.py", line 1>)
                  8 MAKE_FUNCTION            0
                 10 LOAD_CONST               1 ('Bootable')
                 12 PRECALL                  2
                 16 CALL                     2
                 26 STORE_NAME               0 (Bootable)
                 28 LOAD_CONST               2 (None)
                 30 RETURN_VALUE
@@ -34,15 +34,15 @@
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Bootable')
                        8 STORE_NAME               2 (__qualname__)
          
            2          10 LOAD_NAME                3 (staticmethod)
          
-           3          12 LOAD_CONST               1 (<code object init_bootable_hook, file "C:\Users\jrolle\PycharmProjects\bleh\.venv\Lib\site-packages\liveflask/traits/Bootable.py", line 2>)
+           3          12 LOAD_CONST               1 (<code object init_bootable_hook, file "C:\Users\jrolle\PycharmProjects\ITManager\venv\Lib\site-packages\liveflask/traits/Bootable.py", line 2>)
                       14 MAKE_FUNCTION            0
          
            2          16 PRECALL                  0
                       20 CALL                     0
          
            3          30 STORE_NAME               4 (init_bootable_hook)
                       32 LOAD_CONST               2 (None)
@@ -97,30 +97,30 @@
                   None
                   'boot'
                   'booted'
                names      ('hasattr', 'boot', 'booted')
                varnames   ('_class',)
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\jrolle\\PycharmProjects\\bleh\\.venv\\Lib\\site-packages\\liveflask/traits/Bootable.py'
+               filename   'C:\\Users\\jrolle\\PycharmProjects\\ITManager\\venv\\Lib\\site-packages\\liveflask/traits/Bootable.py'
                name       'init_bootable_hook'
                firstlineno 2
                lnotab 0x02022001280220012cff
             None
          names      ('__name__', '__module__', '__qualname__', 'staticmethod', 'init_bootable_hook')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\jrolle\\PycharmProjects\\bleh\\.venv\\Lib\\site-packages\\liveflask/traits/Bootable.py'
+         filename   'C:\\Users\\jrolle\\PycharmProjects\\ITManager\\venv\\Lib\\site-packages\\liveflask/traits/Bootable.py'
          name       'Bootable'
          firstlineno 1
          lnotab 0x0a01020104ff0e01
       'Bootable'
       None
    names      ('Bootable',)
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'C:\\Users\\jrolle\\PycharmProjects\\bleh\\.venv\\Lib\\site-packages\\liveflask/traits/Bootable.py'
+   filename   'C:\\Users\\jrolle\\PycharmProjects\\ITManager\\venv\\Lib\\site-packages\\liveflask/traits/Bootable.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff0201
```

### Comparing `liveflask-1.0.9rc5/liveflask/traits/__pycache__/has_actions.cpython-311.pyc` & `liveflask-1.0.9rc6/liveflask/traits/__pycache__/has_actions.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xfdae3266 (Wed May  1 21:07:09 2024 UTC)
+moddate:  0x4fc93c66 (Thu May  9 13:02:07 2024 UTC)
 files sz: 2042
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
@@ -40,15 +40,15 @@
                 46 IMPORT_NAME              7 (utils)
                 48 IMPORT_FROM              8 (dict_diff_changed_values)
                 50 STORE_NAME               8 (dict_diff_changed_values)
                 52 POP_TOP
    
      8          54 PUSH_NULL
                 56 LOAD_BUILD_CLASS
-                58 LOAD_CONST               6 (<code object HasActions, file "C:\Users\jrolle\PycharmProjects\bleh\.venv\Lib\site-packages\liveflask/traits/has_actions.py", line 8>)
+                58 LOAD_CONST               6 (<code object HasActions, file "C:\Users\jrolle\PycharmProjects\ITManager\venv\Lib\site-packages\liveflask/traits/has_actions.py", line 8>)
                 60 MAKE_FUNCTION            0
                 62 LOAD_CONST               7 ('HasActions')
                 64 PRECALL                  2
                 68 CALL                     2
                 78 STORE_NAME               9 (HasActions)
                 80 LOAD_CONST               8 (None)
                 82 RETURN_VALUE
@@ -76,24 +76,24 @@
            9          10 LOAD_CONST               1 ('component')
                       12 LOAD_NAME                3 (Any)
                       14 LOAD_CONST               2 ('method')
                       16 LOAD_NAME                4 (str)
                       18 LOAD_CONST               3 ('return')
                       20 LOAD_NAME                5 (NoReturn)
                       22 BUILD_TUPLE              6
-                      24 LOAD_CONST               4 (<code object call_method, file "C:\Users\jrolle\PycharmProjects\bleh\.venv\Lib\site-packages\liveflask/traits/has_actions.py", line 9>)
+                      24 LOAD_CONST               4 (<code object call_method, file "C:\Users\jrolle\PycharmProjects\ITManager\venv\Lib\site-packages\liveflask/traits/has_actions.py", line 9>)
                       26 MAKE_FUNCTION            4 (annotations)
                       28 STORE_NAME               6 (call_method)
          
           25          30 LOAD_CONST               1 ('component')
                       32 LOAD_NAME                3 (Any)
                       34 LOAD_CONST               5 ('parsed_method')
                       36 LOAD_NAME                4 (str)
                       38 BUILD_TUPLE              4
-                      40 LOAD_CONST               6 (<code object call_event_handler, file "C:\Users\jrolle\PycharmProjects\bleh\.venv\Lib\site-packages\liveflask/traits/has_actions.py", line 25>)
+                      40 LOAD_CONST               6 (<code object call_event_handler, file "C:\Users\jrolle\PycharmProjects\ITManager\venv\Lib\site-packages\liveflask/traits/has_actions.py", line 25>)
                       42 MAKE_FUNCTION            4 (annotations)
                       44 STORE_NAME               7 (call_event_handler)
                       46 LOAD_CONST               7 (None)
                       48 RETURN_VALUE
          consts
             'HasActions'
             'component'
@@ -199,15 +199,15 @@
                   ('_class',)
                   '__NOVAL__'
                   ()
                names      ('get_props', 'Bootable', 'init_bootable_hook', 'getattr', 'dict_diff_changed_values', 'set_props', 'get', 'session')
                varnames   ('self', 'component', 'method', 'args', 'props', 'new_props', 'item')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\jrolle\\PycharmProjects\\bleh\\.venv\\Lib\\site-packages\\liveflask/traits/has_actions.py'
+               filename   'C:\\Users\\jrolle\\PycharmProjects\\ITManager\\venv\\Lib\\site-packages\\liveflask/traits/has_actions.py'
                name       'call_method'
                firstlineno 9
                lnotab 0x02012a012a020801040326012a01240154013c02
             'parsed_method'
             code
                argcount  : 3
                nlocals   : 7
@@ -285,28 +285,28 @@
                            226 LOAD_FAST                4 (kwargs)
                            228 DICT_MERGE               1
                            230 CALL_FUNCTION_EX         1
                            232 POP_TOP
                
                 48         234 LOAD_CLOSURE             7 (event)
                            236 BUILD_TUPLE              1
-                           238 LOAD_CONST               6 (<code object <listcomp>, file "C:\Users\jrolle\PycharmProjects\bleh\.venv\Lib\site-packages\liveflask/traits/has_actions.py", line 48>)
+                           238 LOAD_CONST               6 (<code object <listcomp>, file "C:\Users\jrolle\PycharmProjects\ITManager\venv\Lib\site-packages\liveflask/traits/has_actions.py", line 48>)
                            240 MAKE_FUNCTION            8 (closure)
                            242 LOAD_FAST                1 (component)
                            244 LOAD_ATTR                5 (emits)
                            254 GET_ITER
                            256 PRECALL                  0
                            260 CALL                     0
                            270 LOAD_FAST                1 (component)
                            272 STORE_ATTR               5 (emits)
                            282 JUMP_FORWARD            24 (to 332)
                
                 50     >>  284 LOAD_CLOSURE             7 (event)
                            286 BUILD_TUPLE              1
-                           288 LOAD_CONST               7 (<code object <listcomp>, file "C:\Users\jrolle\PycharmProjects\bleh\.venv\Lib\site-packages\liveflask/traits/has_actions.py", line 50>)
+                           288 LOAD_CONST               7 (<code object <listcomp>, file "C:\Users\jrolle\PycharmProjects\ITManager\venv\Lib\site-packages\liveflask/traits/has_actions.py", line 50>)
                            290 MAKE_FUNCTION            8 (closure)
                            292 LOAD_FAST                1 (component)
                            294 LOAD_ATTR                5 (emits)
                            304 GET_ITER
                            306 PRECALL                  0
                            310 CALL                     0
                            320 LOAD_FAST                1 (component)
@@ -348,15 +348,15 @@
                              >>   42 RETURN_VALUE
                      consts
                         'event'
                      names      ()
                      varnames   ('.0', 'emit')
                      freevars   ('event',)
                      cellvars   ()
-                     filename   'C:\\Users\\jrolle\\PycharmProjects\\bleh\\.venv\\Lib\\site-packages\\liveflask/traits/has_actions.py'
+                     filename   'C:\\Users\\jrolle\\PycharmProjects\\ITManager\\venv\\Lib\\site-packages\\liveflask/traits/has_actions.py'
                      name       '<listcomp>'
                      firstlineno 48
                      lnotab 0x
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 4
@@ -383,38 +383,38 @@
                              >>   42 RETURN_VALUE
                      consts
                         'event'
                      names      ()
                      varnames   ('.0', 'emit')
                      freevars   ('event',)
                      cellvars   ()
-                     filename   'C:\\Users\\jrolle\\PycharmProjects\\bleh\\.venv\\Lib\\site-packages\\liveflask/traits/has_actions.py'
+                     filename   'C:\\Users\\jrolle\\PycharmProjects\\ITManager\\venv\\Lib\\site-packages\\liveflask/traits/has_actions.py'
                      name       '<listcomp>'
                      firstlineno 50
                      lnotab 0x
                names      ('get_props', 'Bootable', 'init_bootable_hook', 'get', 'getattr', 'emits')
                varnames   ('self', 'component', 'parsed_method', 'args', 'kwargs', 'props', 'listener_method')
                freevars   ()
                cellvars   ('event',)
-               filename   'C:\\Users\\jrolle\\PycharmProjects\\bleh\\.venv\\Lib\\site-packages\\liveflask/traits/has_actions.py'
+               filename   'C:\\Users\\jrolle\\PycharmProjects\\ITManager\\venv\\Lib\\site-packages\\liveflask/traits/has_actions.py'
                name       'call_event_handler'
                firstlineno 25
                lnotab 0x040d2a012a02080110011401360104012c0232023002
             None
          names      ('__name__', '__module__', '__qualname__', 'Any', 'str', 'NoReturn', 'call_method', 'call_event_handler')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\jrolle\\PycharmProjects\\bleh\\.venv\\Lib\\site-packages\\liveflask/traits/has_actions.py'
+         filename   'C:\\Users\\jrolle\\PycharmProjects\\ITManager\\venv\\Lib\\site-packages\\liveflask/traits/has_actions.py'
          name       'HasActions'
          firstlineno 8
          lnotab 0x0a011410
       'HasActions'
       None
    names      ('typing', 'Any', 'NoReturn', 'flask', 'session', 'traits.Bootable', 'Bootable', 'utils', 'dict_diff_changed_values', 'HasActions')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'C:\\Users\\jrolle\\PycharmProjects\\bleh\\.venv\\Lib\\site-packages\\liveflask/traits/has_actions.py'
+   filename   'C:\\Users\\jrolle\\PycharmProjects\\ITManager\\venv\\Lib\\site-packages\\liveflask/traits/has_actions.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff020110020c010c010c03
```

### Comparing `liveflask-1.0.9rc5/liveflask/traits/__pycache__/has_props.cpython-311.pyc` & `liveflask-1.0.9rc6/liveflask/traits/__pycache__/has_props.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xfdae3266 (Wed May  1 21:07:09 2024 UTC)
+moddate:  0x4fc93c66 (Thu May  9 13:02:07 2024 UTC)
 files sz: 2488
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
@@ -26,15 +26,15 @@
                 22 IMPORT_NAME              3 (masoniteorm.collection)
                 24 IMPORT_FROM              4 (Collection)
                 26 STORE_NAME               4 (Collection)
                 28 POP_TOP
    
      5          30 PUSH_NULL
                 32 LOAD_BUILD_CLASS
-                34 LOAD_CONST               3 (<code object HasProps, file "C:\Users\jrolle\PycharmProjects\bleh\.venv\Lib\site-packages\liveflask/traits/has_props.py", line 5>)
+                34 LOAD_CONST               3 (<code object HasProps, file "C:\Users\jrolle\PycharmProjects\ITManager\venv\Lib\site-packages\liveflask/traits/has_props.py", line 5>)
                 36 MAKE_FUNCTION            0
                 38 LOAD_CONST               4 ('HasProps')
                 40 PRECALL                  2
                 44 CALL                     2
                 54 STORE_NAME               5 (HasProps)
                 56 LOAD_CONST               5 (None)
                 58 RETURN_VALUE
@@ -52,37 +52,37 @@
             0484005a066405650764066508640765086606640884045a0964095300
            5           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('HasProps')
                        8 STORE_NAME               2 (__qualname__)
          
-           6          10 LOAD_CONST               1 (<code object get_props, file "C:\Users\jrolle\PycharmProjects\bleh\.venv\Lib\site-packages\liveflask/traits/has_props.py", line 6>)
+           6          10 LOAD_CONST               1 (<code object get_props, file "C:\Users\jrolle\PycharmProjects\ITManager\venv\Lib\site-packages\liveflask/traits/has_props.py", line 6>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (get_props)
          
           28          16 LOAD_CONST               2 ('return')
                       18 LOAD_NAME                4 (NoReturn)
                       20 BUILD_TUPLE              2
-                      22 LOAD_CONST               3 (<code object set_props, file "C:\Users\jrolle\PycharmProjects\bleh\.venv\Lib\site-packages\liveflask/traits/has_props.py", line 28>)
+                      22 LOAD_CONST               3 (<code object set_props, file "C:\Users\jrolle\PycharmProjects\ITManager\venv\Lib\site-packages\liveflask/traits/has_props.py", line 28>)
                       24 MAKE_FUNCTION            4 (annotations)
                       26 STORE_NAME               5 (set_props)
          
-          58          28 LOAD_CONST               4 (<code object dehydrate_props, file "C:\Users\jrolle\PycharmProjects\bleh\.venv\Lib\site-packages\liveflask/traits/has_props.py", line 58>)
+          58          28 LOAD_CONST               4 (<code object dehydrate_props, file "C:\Users\jrolle\PycharmProjects\ITManager\venv\Lib\site-packages\liveflask/traits/has_props.py", line 58>)
                       30 MAKE_FUNCTION            0
                       32 STORE_NAME               6 (dehydrate_props)
          
           71          34 LOAD_CONST               5 ('_class')
                       36 LOAD_NAME                7 (Any)
                       38 LOAD_CONST               6 ('prop')
                       40 LOAD_NAME                8 (str)
                       42 LOAD_CONST               7 ('val')
                       44 LOAD_NAME                8 (str)
                       46 BUILD_TUPLE              6
-                      48 LOAD_CONST               8 (<code object access_nested_dict_in_component, file "C:\Users\jrolle\PycharmProjects\bleh\.venv\Lib\site-packages\liveflask/traits/has_props.py", line 71>)
+                      48 LOAD_CONST               8 (<code object access_nested_dict_in_component, file "C:\Users\jrolle\PycharmProjects\ITManager\venv\Lib\site-packages\liveflask/traits/has_props.py", line 71>)
                       50 MAKE_FUNCTION            4 (annotations)
                       52 STORE_NAME               9 (access_nested_dict_in_component)
                       54 LOAD_CONST               9 (None)
                       56 RETURN_VALUE
          consts
             'HasProps'
             code
@@ -112,15 +112,15 @@
                  7           4 LOAD_GLOBAL              1 (NULL + dict)
                             16 PRECALL                  0
                             20 CALL                     0
                             30 STORE_FAST               2 (props)
                
                  8          32 LOAD_CLOSURE             1 (component)
                             34 BUILD_TUPLE              1
-                            36 LOAD_CONST               1 (<code object <listcomp>, file "C:\Users\jrolle\PycharmProjects\bleh\.venv\Lib\site-packages\liveflask/traits/has_props.py", line 8>)
+                            36 LOAD_CONST               1 (<code object <listcomp>, file "C:\Users\jrolle\PycharmProjects\ITManager\venv\Lib\site-packages\liveflask/traits/has_props.py", line 8>)
                             38 MAKE_FUNCTION            8 (closure)
                             40 LOAD_GLOBAL              3 (NULL + dir)
                             52 LOAD_DEREF               1 (component)
                             54 PRECALL                  1
                             58 CALL                     1
                             68 GET_ITER
                             70 PRECALL                  0
@@ -249,28 +249,28 @@
                      consts
                         '__'
                         False
                      names      ('callable', 'getattr', 'startswith')
                      varnames   ('.0', 'attribute')
                      freevars   ('component',)
                      cellvars   ()
-                     filename   'C:\\Users\\jrolle\\PycharmProjects\\bleh\\.venv\\Lib\\site-packages\\liveflask/traits/has_props.py'
+                     filename   'C:\\Users\\jrolle\\PycharmProjects\\ITManager\\venv\\Lib\\site-packages\\liveflask/traits/has_props.py'
                      name       '<listcomp>'
                      firstlineno 8
                      lnotab 0x0c0138ff02012eff0201
                   0
                   '_'
                   1
                   'updated_'
                   'updating_'
                names      ('dict', 'dir', '__dict__', 'items', 'startswith', 'getattr')
                varnames   ('self', 'component', 'props', 'method_list', 'key', 'method')
                freevars   ()
                cellvars   ('component',)
-               filename   'C:\\Users\\jrolle\\PycharmProjects\\bleh\\.venv\\Lib\\site-packages\\liveflask/traits/has_props.py'
+               filename   'C:\\Users\\jrolle\\PycharmProjects\\ITManager\\venv\\Lib\\site-packages\\liveflask/traits/has_props.py'
                name       'get_props'
                firstlineno 6
                lnotab 0x04011c013603360236010201140102022601080154012a020203
             'return'
             code
                argcount  : 4
                nlocals   : 7
@@ -434,15 +434,15 @@
                   'updating'
                   '.'
                   'updated'
                names      ('mvlive__locked', 'AttributeError', 'hasattr', 'updating', 'getattr', 'access_nested_dict_in_component', 'setattr', 'updated')
                varnames   ('self', '_class', 'prop', 'val', 'updated_hook', 'updating_hook', 'new_val')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\jrolle\\PycharmProjects\\bleh\\.venv\\Lib\\site-packages\\liveflask/traits/has_props.py'
+               filename   'C:\\Users\\jrolle\\PycharmProjects\\ITManager\\venv\\Lib\\site-packages\\liveflask/traits/has_props.py'
                name       'set_props'
                firstlineno 28
                lnotab
                   0x0201120126020a010a0220012c0220013202080130022203200120012c
                   02200136ff
             code
                argcount  : 2
@@ -517,15 +517,15 @@
                   1
                   'collection'
                   0
                names      ('items', 'isinstance', 'Collection', 'to_dict')
                varnames   ('self', 'props', 'data', 'meta', 'key', 'value')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\jrolle\\PycharmProjects\\bleh\\.venv\\Lib\\site-packages\\liveflask/traits/has_props.py'
+               filename   'C:\\Users\\jrolle\\PycharmProjects\\ITManager\\venv\\Lib\\site-packages\\liveflask/traits/has_props.py'
                name       'dehydrate_props'
                firstlineno 58
                lnotab 0x0201040104022c0136013401160118020201
             '_class'
             'prop'
             'val'
             code
@@ -592,30 +592,30 @@
                   '.'
                   0
                   1
                names      ('get_props', 'keys', 'split', '__dict__')
                varnames   ('self', '_class', 'prop', 'val', 'props', 'key')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\jrolle\\PycharmProjects\\bleh\\.venv\\Lib\\site-packages\\liveflask/traits/has_props.py'
+               filename   'C:\\Users\\jrolle\\PycharmProjects\\ITManager\\venv\\Lib\\site-packages\\liveflask/traits/has_props.py'
                name       'access_nested_dict_in_component'
                firstlineno 71
                lnotab 0x02012a012c013e0154fe
             None
          names      ('__name__', '__module__', '__qualname__', 'get_props', 'NoReturn', 'set_props', 'dehydrate_props', 'Any', 'str', 'access_nested_dict_in_component')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\jrolle\\PycharmProjects\\bleh\\.venv\\Lib\\site-packages\\liveflask/traits/has_props.py'
+         filename   'C:\\Users\\jrolle\\PycharmProjects\\ITManager\\venv\\Lib\\site-packages\\liveflask/traits/has_props.py'
          name       'HasProps'
          firstlineno 5
          lnotab 0x0a0106160c1e060d
       'HasProps'
       None
    names      ('typing', 'Any', 'NoReturn', 'masoniteorm.collection', 'Collection', 'HasProps')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'C:\\Users\\jrolle\\PycharmProjects\\bleh\\.venv\\Lib\\site-packages\\liveflask/traits/has_props.py'
+   filename   'C:\\Users\\jrolle\\PycharmProjects\\ITManager\\venv\\Lib\\site-packages\\liveflask/traits/has_props.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff020110010c03
```

### Comparing `liveflask-1.0.9rc5/liveflask/traits/__pycache__/has_renders.cpython-311.pyc` & `liveflask-1.0.9rc6/liveflask/traits/__pycache__/has_renders.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xfdae3266 (Wed May  1 21:07:09 2024 UTC)
+moddate:  0x4fc93c66 (Thu May  9 13:02:07 2024 UTC)
 files sz: 2486
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
@@ -53,15 +53,15 @@
                 66 IMPORT_NAME             10 (utils)
                 68 IMPORT_FROM             11 (to_class)
                 70 STORE_NAME              11 (to_class)
                 72 POP_TOP
    
     11          74 PUSH_NULL
                 76 LOAD_BUILD_CLASS
-                78 LOAD_CONST               8 (<code object HasRenders, file "C:\Users\jrolle\PycharmProjects\bleh\.venv\Lib\site-packages\liveflask/traits/has_renders.py", line 11>)
+                78 LOAD_CONST               8 (<code object HasRenders, file "C:\Users\jrolle\PycharmProjects\ITManager\venv\Lib\site-packages\liveflask/traits/has_renders.py", line 11>)
                 80 MAKE_FUNCTION            0
                 82 LOAD_CONST               9 ('HasRenders')
                 84 PRECALL                  2
                 88 CALL                     2
                 98 STORE_NAME              12 (HasRenders)
                100 LOAD_CONST               1 (None)
                102 RETURN_VALUE
@@ -85,15 +85,15 @@
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('HasRenders')
                        8 STORE_NAME               2 (__qualname__)
          
           12          10 LOAD_CONST               1 ('component_name')
                       12 LOAD_NAME                3 (str)
                       14 BUILD_TUPLE              2
-                      16 LOAD_CONST               2 (<code object inital_render, file "C:\Users\jrolle\PycharmProjects\bleh\.venv\Lib\site-packages\liveflask/traits/has_renders.py", line 12>)
+                      16 LOAD_CONST               2 (<code object inital_render, file "C:\Users\jrolle\PycharmProjects\ITManager\venv\Lib\site-packages\liveflask/traits/has_renders.py", line 12>)
                       18 MAKE_FUNCTION            4 (annotations)
                       20 STORE_NAME               4 (inital_render)
                       22 LOAD_CONST               3 (None)
                       24 RETURN_VALUE
          consts
             'HasRenders'
             'component_name'
@@ -344,32 +344,32 @@
                   'booted'
                   '\n                    <div data-component="{{ component_name }}" id="{{ key }}" data-snapshot="{{ snapshot_attr }}">\n                        {{html|safe}}\n                    </div>\n                '
                   ('snapshot_attr', 'html', 'key', 'component_name')
                names      ('to_class', '__name__', 'get', 'getattr', 'setattr', 'mvlive__session', 'session', 'mvlive__url', 'req', 'args', 'hasattr', 'boot', 'mount', 'booted', 'to_snapshot', 'json', 'dumps', 'Markup', 'render_template_string')
                varnames   ('self', 'component_name', 'args', 'kwargs', '_class', 'component_instance', 'key', 'prop', 'html', 'snapshot', 'snapshot_attr')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\jrolle\\PycharmProjects\\bleh\\.venv\\Lib\\site-packages\\liveflask/traits/has_renders.py'
+               filename   'C:\\Users\\jrolle\\PycharmProjects\\ITManager\\venv\\Lib\\site-packages\\liveflask/traits/has_renders.py'
                name       'inital_render'
                firstlineno 12
                lnotab
                   0x02040a012a0114010e032a01040208022003220312010c010201020116
                   0122ff0efd1208120140010c01020102013efd12062001280220011a0220
                   012803300128040c010c01020408fb10ff
             None
          names      ('__name__', '__module__', '__qualname__', 'str', 'inital_render')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\jrolle\\PycharmProjects\\bleh\\.venv\\Lib\\site-packages\\liveflask/traits/has_renders.py'
+         filename   'C:\\Users\\jrolle\\PycharmProjects\\ITManager\\venv\\Lib\\site-packages\\liveflask/traits/has_renders.py'
          name       'HasRenders'
          firstlineno 11
          lnotab 0x0a01
       'HasRenders'
    names      ('json', 'typing', 'Any', 'flask', 'render_template_string', 'session', 'request', 'req', 'markupsafe', 'Markup', 'utils', 'to_class', 'HasRenders')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'C:\\Users\\jrolle\\PycharmProjects\\bleh\\.venv\\Lib\\site-packages\\liveflask/traits/has_renders.py'
+   filename   'C:\\Users\\jrolle\\PycharmProjects\\ITManager\\venv\\Lib\\site-packages\\liveflask/traits/has_renders.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff020108010c0210010c010c020c03
```

### Comparing `liveflask-1.0.9rc5/liveflask/traits/__pycache__/has_snapshots.cpython-311.pyc` & `liveflask-1.0.9rc6/liveflask/traits/__pycache__/has_snapshots.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xfdae3266 (Wed May  1 21:07:09 2024 UTC)
+moddate:  0x4fc93c66 (Thu May  9 13:02:07 2024 UTC)
 files sz: 4106
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
@@ -59,15 +59,15 @@
                 74 IMPORT_NAME             10 (utils)
                 76 IMPORT_FROM             11 (to_class)
                 78 STORE_NAME              11 (to_class)
                 80 POP_TOP
    
     13          82 PUSH_NULL
                 84 LOAD_BUILD_CLASS
-                86 LOAD_CONST               7 (<code object HasSnapshots, file "C:\Users\jrolle\PycharmProjects\bleh\.venv\Lib\site-packages\liveflask/traits/has_snapshots.py", line 13>)
+                86 LOAD_CONST               7 (<code object HasSnapshots, file "C:\Users\jrolle\PycharmProjects\ITManager\venv\Lib\site-packages\liveflask/traits/has_snapshots.py", line 13>)
                 88 MAKE_FUNCTION            0
                 90 LOAD_CONST               8 ('HasSnapshots')
                 92 PRECALL                  2
                 96 CALL                     2
                106 STORE_NAME              12 (HasSnapshots)
                108 LOAD_CONST               1 (None)
                110 RETURN_VALUE
@@ -96,22 +96,22 @@
           14          10 LOAD_CONST               1 ('req_snapshot')
                       12 LOAD_NAME                3 (dict)
                       14 LOAD_NAME                4 (str)
                       16 LOAD_NAME                5 (Any)
                       18 BUILD_TUPLE              2
                       20 BINARY_SUBSCR
                       30 BUILD_TUPLE              2
-                      32 LOAD_CONST               2 (<code object from_snapshot, file "C:\Users\jrolle\PycharmProjects\bleh\.venv\Lib\site-packages\liveflask/traits/has_snapshots.py", line 14>)
+                      32 LOAD_CONST               2 (<code object from_snapshot, file "C:\Users\jrolle\PycharmProjects\ITManager\venv\Lib\site-packages\liveflask/traits/has_snapshots.py", line 14>)
                       34 MAKE_FUNCTION            4 (annotations)
                       36 STORE_NAME               6 (from_snapshot)
          
           53          38 LOAD_CONST               3 ('_class')
                       40 LOAD_NAME                5 (Any)
                       42 BUILD_TUPLE              2
-                      44 LOAD_CONST               4 (<code object to_snapshot, file "C:\Users\jrolle\PycharmProjects\bleh\.venv\Lib\site-packages\liveflask/traits/has_snapshots.py", line 53>)
+                      44 LOAD_CONST               4 (<code object to_snapshot, file "C:\Users\jrolle\PycharmProjects\ITManager\venv\Lib\site-packages\liveflask/traits/has_snapshots.py", line 53>)
                       46 MAKE_FUNCTION            4 (annotations)
                       48 STORE_NAME               7 (to_snapshot)
                       50 LOAD_CONST               5 (None)
                       52 RETURN_VALUE
          consts
             'HasSnapshots'
             'req_snapshot'
@@ -366,15 +366,15 @@
                   4
                   0
                   1
                names      ('hashlib', 'md5', 'json', 'dumps', 'encode', 'hexdigest', 'to_class', '__name__', '__class__', 'getattr', 'lower', 'secrets', 'token_urlsafe', 'setattr', 'items')
                varnames   ('self', 'req_snapshot', 'req_checksum', 'source_checksum', 'class_name', 'data', '_class', 'key', 'prop')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\jrolle\\PycharmProjects\\bleh\\.venv\\Lib\\site-packages\\liveflask/traits/has_snapshots.py'
+               filename   'C:\\Users\\jrolle\\PycharmProjects\\ITManager\\venv\\Lib\\site-packages\\liveflask/traits/has_snapshots.py'
                name       'from_snapshot'
                firstlineno 14
                lnotab
                   0x02011c0112011401120114011201140112011401120316015eff0e0124
                   ff02081c011c033a01280122022203620122022c013c01
             '_class'
             code
@@ -672,32 +672,32 @@
                   ('sort_keys', 'ensure_ascii')
                   'utf-8'
                   'checksum'
                names      ('get_props', 'hasattr', 'mvlive__url', 'update', 'get', 'key', 'render', '__doc__', 'Markup', 'render_template_string', 'getattr', 'list', 'keys', 'callable', 'isinstance', 'str', 'json', 'loads', 'JSONDecodeError', '__class__', '__name__', 'hashlib', 'md5', 'dumps', 'encode', 'hexdigest')
                varnames   ('self', '_class', 'props', 'key', 'html', 'snapshot')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\jrolle\\PycharmProjects\\bleh\\.venv\\Lib\\site-packages\\liveflask/traits/has_snapshots.py'
+               filename   'C:\\Users\\jrolle\\PycharmProjects\\ITManager\\venv\\Lib\\site-packages\\liveflask/traits/has_snapshots.py'
                name       'to_snapshot'
                firstlineno 53
                lnotab
                   0x02012a0320010a011201480434081801180138ff12040c0116ff040202
                   fe06072202080106020801060546012a0208044601360102013e011c0104
                   ff08fd020a1601020102fd0607160152ff0e0124ff0803
             None
          names      ('__name__', '__module__', '__qualname__', 'dict', 'str', 'Any', 'from_snapshot', 'to_snapshot')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\jrolle\\PycharmProjects\\bleh\\.venv\\Lib\\site-packages\\liveflask/traits/has_snapshots.py'
+         filename   'C:\\Users\\jrolle\\PycharmProjects\\ITManager\\venv\\Lib\\site-packages\\liveflask/traits/has_snapshots.py'
          name       'HasSnapshots'
          firstlineno 13
          lnotab 0x0a011c27
       'HasSnapshots'
    names      ('hashlib', 'json', 'pprint', 'secrets', 'typing', 'Any', 'flask', 'render_template_string', 'markupsafe', 'Markup', 'utils', 'to_class', 'HasSnapshots')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'C:\\Users\\jrolle\\PycharmProjects\\bleh\\.venv\\Lib\\site-packages\\liveflask/traits/has_snapshots.py'
+   filename   'C:\\Users\\jrolle\\PycharmProjects\\ITManager\\venv\\Lib\\site-packages\\liveflask/traits/has_snapshots.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff020108010801080108010c020c010c020c03
```

### Comparing `liveflask-1.0.9rc5/liveflask/traits/has_actions.py` & `liveflask-1.0.9rc6/liveflask/traits/has_actions.py`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.9rc5/liveflask/traits/has_props.py` & `liveflask-1.0.9rc6/liveflask/traits/has_props.py`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.9rc5/liveflask/traits/has_renders.py` & `liveflask-1.0.9rc6/liveflask/traits/has_renders.py`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.9rc5/liveflask/traits/has_snapshots.py` & `liveflask-1.0.9rc6/liveflask/traits/has_snapshots.py`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.9rc5/liveflask/utils.py` & `liveflask-1.0.9rc6/liveflask/utils.py`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.9rc5/liveflask.egg-info/PKG-INFO` & `liveflask-1.0.9rc6/liveflask.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 Metadata-Version: 2.1
 Name: liveflask
-Version: 1.0.9rc5
+Version: 1.0.9rc6
 Summary: Seamlessly integrate modern reactive components into Flask templates, eliminating the need for mastering new templating languages or wrestling with complex JavaScript frameworks. With our solution, developers can enhance their Flask applications with dynamic functionality while maintaining a familiar development environment, streamlining the process and ensuring a smoother user experience.
 Home-page: https://github.com/JarriqTheTechie/liveflask
 Author: Jarriq Rolle
 Author-email: jrolle@baysidetechgroup.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: flask
-Requires-Dist: masonite-orm
-Requires-Dist: Flask-WTF
 
 # LiveFlask
 
 LiveFlask is a comprehensive framework for Flask that simplifies the creation of dynamic interfaces, all within the
 familiar environment of Flask.
 
 # Install LiveFlask
```

### Comparing `liveflask-1.0.9rc5/liveflask.egg-info/SOURCES.txt` & `liveflask-1.0.9rc6/liveflask.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.9rc5/setup.py` & `liveflask-1.0.9rc6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("readme_pypi.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="liveflask",
-    version="1.0.9rc5",
+    version="1.0.9rc6",
     author="Jarriq Rolle",
     author_email="jrolle@baysidetechgroup.com",
     description="Seamlessly integrate modern reactive components into Flask templates, eliminating the need for mastering new templating languages or wrestling with complex JavaScript frameworks. With our solution, developers can enhance their Flask applications with dynamic functionality while maintaining a familiar development environment, streamlining the process and ensuring a smoother user experience.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/JarriqTheTechie/liveflask",
     packages=['liveflask'],
```

