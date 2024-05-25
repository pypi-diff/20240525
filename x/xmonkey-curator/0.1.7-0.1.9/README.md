# Comparing `tmp/xmonkey-curator-0.1.7.tar.gz` & `tmp/xmonkey-curator-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xmonkey-curator-0.1.7.tar", last modified: Thu Apr  4 07:09:24 2024, max compression
+gzip compressed data, was "xmonkey-curator-0.1.9.tar", last modified: Sun Apr  7 22:28:27 2024, max compression
```

## Comparing `xmonkey-curator-0.1.7.tar` & `xmonkey-curator-0.1.9.tar`

### file list

```diff
@@ -1,57 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:09:24.798192 xmonkey-curator-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-04 07:09:21.000000 xmonkey-curator-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-04-04 07:09:24.798192 xmonkey-curator-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-04 07:09:21.000000 xmonkey-curator-0.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 07:09:24.798192 xmonkey-curator-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-04 07:09:21.000000 xmonkey-curator-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:09:24.790192 xmonkey-curator-0.1.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:09:24.790192 xmonkey-curator-0.1.7/src/xmonkey_curator/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 07:09:21.000000 xmonkey-curator-0.1.7/src/xmonkey_curator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-04 07:09:21.000000 xmonkey-curator-0.1.7/src/xmonkey_curator/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-04 07:09:21.000000 xmonkey-curator-0.1.7/src/xmonkey_curator/base_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-04-04 07:09:21.000000 xmonkey-curator-0.1.7/src/xmonkey_curator/file_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-04-04 07:09:21.000000 xmonkey-curator-0.1.7/src/xmonkey_curator/handler_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:09:24.794191 xmonkey-curator-0.1.7/src/xmonkey_curator/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-04 07:09:21.000000 xmonkey-curator-0.1.7/src/xmonkey_curator/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3968 2024-04-04 07:09:21.000000 xmonkey-curator-0.1.7/src/xmonkey_curator/handlers/archive_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-04 07:09:21.000000 xmonkey-curator-0.1.7/src/xmonkey_curator/handlers/archivelib_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-04 07:09:21.000000 xmonkey-curator-0.1.7/src/xmonkey_curator/handlers/cplus_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-04 07:09:21.000000 xmonkey-curator-0.1.7/src/xmonkey_curator/handlers/elf_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-04 07:09:21.000000 xmonkey-curator-0.1.7/src/xmonkey_curator/handlers/java_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-04 07:09:21.000000 xmonkey-curator-0.1.7/src/xmonkey_curator/handlers/jvm_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-04 07:09:21.000000 xmonkey-curator-0.1.7/src/xmonkey_curator/handlers/machos_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-04 07:09:21.000000 xmonkey-curator-0.1.7/src/xmonkey_curator/handlers/objectivec_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-04 07:09:21.000000 xmonkey-curator-0.1.7/src/xmonkey_curator/handlers/octetstream_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-04 07:09:21.000000 xmonkey-curator-0.1.7/src/xmonkey_curator/handlers/perl_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-04 07:09:21.000000 xmonkey-curator-0.1.7/src/xmonkey_curator/handlers/python_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-04 07:09:21.000000 xmonkey-curator-0.1.7/src/xmonkey_curator/handlers/ruby_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-04 07:09:21.000000 xmonkey-curator-0.1.7/src/xmonkey_curator/handlers/rust_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-04-04 07:09:21.000000 xmonkey-curator-0.1.7/src/xmonkey_curator/handlers/sharedlib_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-04 07:09:21.000000 xmonkey-curator-0.1.7/src/xmonkey_curator/handlers/text_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-04-04 07:09:21.000000 xmonkey-curator-0.1.7/src/xmonkey_curator/lexer_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:09:24.798192 xmonkey-curator-0.1.7/src/xmonkey_curator/licenses/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 07:09:21.000000 xmonkey-curator-0.1.7/src/xmonkey_curator/licenses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-04 07:09:21.000000 xmonkey-curator-0.1.7/src/xmonkey_curator/licenses/apache_2_0.json
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-04 07:09:21.000000 xmonkey-curator-0.1.7/src/xmonkey_curator/licenses/gpl_2_0.json
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-04 07:09:21.000000 xmonkey-curator-0.1.7/src/xmonkey_curator/licenses/gpl_3_0.json
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-04 07:09:21.000000 xmonkey-curator-0.1.7/src/xmonkey_curator/licenses/lgpl_2_1.json
--rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-04-04 07:09:21.000000 xmonkey-curator-0.1.7/src/xmonkey_curator/report_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:09:24.798192 xmonkey-curator-0.1.7/src/xmonkey_curator/rules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 07:09:21.000000 xmonkey-curator-0.1.7/src/xmonkey_curator/rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-04 07:09:21.000000 xmonkey-curator-0.1.7/src/xmonkey_curator/rules/license_files.json
--rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-04-04 07:09:21.000000 xmonkey-curator-0.1.7/src/xmonkey_curator/rules_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     8197 2024-04-04 07:09:21.000000 xmonkey-curator-0.1.7/src/xmonkey_curator/scanner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:09:24.798192 xmonkey-curator-0.1.7/src/xmonkey_curator/signatures/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 07:09:21.000000 xmonkey-curator-0.1.7/src/xmonkey_curator/signatures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   214075 2024-04-04 07:09:21.000000 xmonkey-curator-0.1.7/src/xmonkey_curator/signatures/ffmpeg.json
--rw-r--r--   0 runner    (1001) docker     (127)     3517 2024-04-04 07:09:21.000000 xmonkey-curator-0.1.7/src/xmonkey_curator/symbols_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:09:24.798192 xmonkey-curator-0.1.7/src/xmonkey_curator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-04-04 07:09:24.000000 xmonkey-curator-0.1.7/src/xmonkey_curator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-04 07:09:24.000000 xmonkey-curator-0.1.7/src/xmonkey_curator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 07:09:24.000000 xmonkey-curator-0.1.7/src/xmonkey_curator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-04 07:09:24.000000 xmonkey-curator-0.1.7/src/xmonkey_curator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-04 07:09:24.000000 xmonkey-curator-0.1.7/src/xmonkey_curator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-04 07:09:24.000000 xmonkey-curator-0.1.7/src/xmonkey_curator.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:09:24.798192 xmonkey-curator-0.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-04 07:09:21.000000 xmonkey-curator-0.1.7/tests/test_base_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-04 07:09:21.000000 xmonkey-curator-0.1.7/tests/test_text_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:28:27.991522 xmonkey-curator-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-07 22:28:21.000000 xmonkey-curator-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-07 22:28:27.991522 xmonkey-curator-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-07 22:28:21.000000 xmonkey-curator-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 22:28:27.991522 xmonkey-curator-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-04-07 22:28:21.000000 xmonkey-curator-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:28:27.979521 xmonkey-curator-0.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:28:27.983522 xmonkey-curator-0.1.9/src/xmonkey_curator/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 22:28:21.000000 xmonkey-curator-0.1.9/src/xmonkey_curator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-07 22:28:21.000000 xmonkey-curator-0.1.9/src/xmonkey_curator/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-07 22:28:21.000000 xmonkey-curator-0.1.9/src/xmonkey_curator/base_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-04-07 22:28:21.000000 xmonkey-curator-0.1.9/src/xmonkey_curator/file_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-04-07 22:28:21.000000 xmonkey-curator-0.1.9/src/xmonkey_curator/handler_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:28:27.991522 xmonkey-curator-0.1.9/src/xmonkey_curator/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-07 22:28:21.000000 xmonkey-curator-0.1.9/src/xmonkey_curator/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3968 2024-04-07 22:28:21.000000 xmonkey-curator-0.1.9/src/xmonkey_curator/handlers/archive_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-07 22:28:21.000000 xmonkey-curator-0.1.9/src/xmonkey_curator/handlers/archivelib_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-07 22:28:21.000000 xmonkey-curator-0.1.9/src/xmonkey_curator/handlers/cplus_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-07 22:28:21.000000 xmonkey-curator-0.1.9/src/xmonkey_curator/handlers/elf_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-07 22:28:21.000000 xmonkey-curator-0.1.9/src/xmonkey_curator/handlers/java_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-07 22:28:21.000000 xmonkey-curator-0.1.9/src/xmonkey_curator/handlers/jvm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-07 22:28:21.000000 xmonkey-curator-0.1.9/src/xmonkey_curator/handlers/machos_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-07 22:28:21.000000 xmonkey-curator-0.1.9/src/xmonkey_curator/handlers/objectivec_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-07 22:28:21.000000 xmonkey-curator-0.1.9/src/xmonkey_curator/handlers/octetstream_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-07 22:28:21.000000 xmonkey-curator-0.1.9/src/xmonkey_curator/handlers/perl_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-07 22:28:21.000000 xmonkey-curator-0.1.9/src/xmonkey_curator/handlers/python_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-07 22:28:21.000000 xmonkey-curator-0.1.9/src/xmonkey_curator/handlers/ruby_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-07 22:28:21.000000 xmonkey-curator-0.1.9/src/xmonkey_curator/handlers/rust_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-04-07 22:28:21.000000 xmonkey-curator-0.1.9/src/xmonkey_curator/handlers/sharedlib_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-07 22:28:21.000000 xmonkey-curator-0.1.9/src/xmonkey_curator/handlers/text_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-04-07 22:28:21.000000 xmonkey-curator-0.1.9/src/xmonkey_curator/lexer_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:28:27.991522 xmonkey-curator-0.1.9/src/xmonkey_curator/licenses/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 22:28:21.000000 xmonkey-curator-0.1.9/src/xmonkey_curator/licenses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-07 22:28:21.000000 xmonkey-curator-0.1.9/src/xmonkey_curator/licenses/apache_2_0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-07 22:28:21.000000 xmonkey-curator-0.1.9/src/xmonkey_curator/licenses/gpl_2_0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-07 22:28:21.000000 xmonkey-curator-0.1.9/src/xmonkey_curator/licenses/gpl_3_0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-07 22:28:21.000000 xmonkey-curator-0.1.9/src/xmonkey_curator/licenses/lgpl_2_1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-04-07 22:28:21.000000 xmonkey-curator-0.1.9/src/xmonkey_curator/report_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:28:27.991522 xmonkey-curator-0.1.9/src/xmonkey_curator/rules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 22:28:21.000000 xmonkey-curator-0.1.9/src/xmonkey_curator/rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-07 22:28:21.000000 xmonkey-curator-0.1.9/src/xmonkey_curator/rules/license_files.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-04-07 22:28:21.000000 xmonkey-curator-0.1.9/src/xmonkey_curator/rules_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8759 2024-04-07 22:28:21.000000 xmonkey-curator-0.1.9/src/xmonkey_curator/scanner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:28:27.991522 xmonkey-curator-0.1.9/src/xmonkey_curator/signatures/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 22:28:21.000000 xmonkey-curator-0.1.9/src/xmonkey_curator/signatures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   214075 2024-04-07 22:28:21.000000 xmonkey-curator-0.1.9/src/xmonkey_curator/signatures/ffmpeg.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-04-07 22:28:21.000000 xmonkey-curator-0.1.9/src/xmonkey_curator/signatures_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3517 2024-04-07 22:28:21.000000 xmonkey-curator-0.1.9/src/xmonkey_curator/symbols_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:28:27.991522 xmonkey-curator-0.1.9/src/xmonkey_curator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-07 22:28:27.000000 xmonkey-curator-0.1.9/src/xmonkey_curator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-04-07 22:28:27.000000 xmonkey-curator-0.1.9/src/xmonkey_curator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 22:28:27.000000 xmonkey-curator-0.1.9/src/xmonkey_curator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-07 22:28:27.000000 xmonkey-curator-0.1.9/src/xmonkey_curator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-07 22:28:27.000000 xmonkey-curator-0.1.9/src/xmonkey_curator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-07 22:28:27.000000 xmonkey-curator-0.1.9/src/xmonkey_curator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:28:27.991522 xmonkey-curator-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-07 22:28:21.000000 xmonkey-curator-0.1.9/tests/test_base_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-07 22:28:21.000000 xmonkey-curator-0.1.9/tests/test_text_handler.py
```

### Comparing `xmonkey-curator-0.1.7/LICENSE` & `xmonkey-curator-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `xmonkey-curator-0.1.7/PKG-INFO` & `xmonkey-curator-0.1.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xmonkey-curator
-Version: 0.1.7
+Version: 0.1.9
 Summary: Automated OSS curation scanner
 Home-page: https://github.com/Xpertians/xmonkey-curator
 Author: Oscar Valenzuela
 Author-email: oscar.valenzuela.b@gmail.com
 License: Apache 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -17,14 +17,15 @@
 Requires-Dist: python-magic
 Requires-Dist: libmagic
 Requires-Dist: pygments
 Requires-Dist: ssdeep
 Requires-Dist: tqdm
 Requires-Dist: rpmfile
 Requires-Dist: zstandard
+Requires-Dist: requests
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 
 # XMonkey Curator - Automated DESCAM tooling
 
 ## Summary
```

### Comparing `xmonkey-curator-0.1.7/README.md` & `xmonkey-curator-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `xmonkey-curator-0.1.7/setup.py` & `xmonkey-curator-0.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,21 +33,22 @@
         'python-magic',
         'libmagic',
         'pygments',
         'ssdeep',
         'tqdm',
         'rpmfile',
         'zstandard',
+        'requests',
     ],
     extras_require={
         'test': ['pytest'],
     },
     entry_points={
         'console_scripts': [
-            'xmonkey-curator=xmonkey_curator.scanner:scan',
+            'xmonkey-curator=xmonkey_curator.scanner:cli',
         ],
     },
     include_package_data=True,
     package_data={
         'xmonkey_curator': ['signatures/*.json', 'licenses/*.json', 'rules/*.json'],
     },
     test_suite="tests",
```

### Comparing `xmonkey-curator-0.1.7/src/xmonkey_curator/file_utilities.py` & `xmonkey-curator-0.1.9/src/xmonkey_curator/file_utilities.py`

 * *Files identical despite different names*

### Comparing `xmonkey-curator-0.1.7/src/xmonkey_curator/handler_registry.py` & `xmonkey-curator-0.1.9/src/xmonkey_curator/handler_registry.py`

 * *Files identical despite different names*

### Comparing `xmonkey-curator-0.1.7/src/xmonkey_curator/handlers/__init__.py` & `xmonkey-curator-0.1.9/src/xmonkey_curator/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `xmonkey-curator-0.1.7/src/xmonkey_curator/handlers/archive_handler.py` & `xmonkey-curator-0.1.9/src/xmonkey_curator/handlers/archive_handler.py`

 * *Files identical despite different names*

### Comparing `xmonkey-curator-0.1.7/src/xmonkey_curator/handlers/archivelib_handler.py` & `xmonkey-curator-0.1.9/src/xmonkey_curator/handlers/archivelib_handler.py`

 * *Files identical despite different names*

### Comparing `xmonkey-curator-0.1.7/src/xmonkey_curator/handlers/cplus_handler.py` & `xmonkey-curator-0.1.9/src/xmonkey_curator/handlers/cplus_handler.py`

 * *Files identical despite different names*

### Comparing `xmonkey-curator-0.1.7/src/xmonkey_curator/handlers/elf_handler.py` & `xmonkey-curator-0.1.9/src/xmonkey_curator/handlers/elf_handler.py`

 * *Files identical despite different names*

### Comparing `xmonkey-curator-0.1.7/src/xmonkey_curator/handlers/java_handler.py` & `xmonkey-curator-0.1.9/src/xmonkey_curator/handlers/java_handler.py`

 * *Files identical despite different names*

### Comparing `xmonkey-curator-0.1.7/src/xmonkey_curator/handlers/jvm_handler.py` & `xmonkey-curator-0.1.9/src/xmonkey_curator/handlers/jvm_handler.py`

 * *Files identical despite different names*

### Comparing `xmonkey-curator-0.1.7/src/xmonkey_curator/handlers/machos_handler.py` & `xmonkey-curator-0.1.9/src/xmonkey_curator/handlers/machos_handler.py`

 * *Files identical despite different names*

### Comparing `xmonkey-curator-0.1.7/src/xmonkey_curator/handlers/objectivec_handler.py` & `xmonkey-curator-0.1.9/src/xmonkey_curator/handlers/objectivec_handler.py`

 * *Files identical despite different names*

### Comparing `xmonkey-curator-0.1.7/src/xmonkey_curator/handlers/octetstream_handler.py` & `xmonkey-curator-0.1.9/src/xmonkey_curator/handlers/octetstream_handler.py`

 * *Files identical despite different names*

### Comparing `xmonkey-curator-0.1.7/src/xmonkey_curator/handlers/perl_handler.py` & `xmonkey-curator-0.1.9/src/xmonkey_curator/handlers/perl_handler.py`

 * *Files identical despite different names*

### Comparing `xmonkey-curator-0.1.7/src/xmonkey_curator/handlers/python_handler.py` & `xmonkey-curator-0.1.9/src/xmonkey_curator/handlers/python_handler.py`

 * *Files identical despite different names*

### Comparing `xmonkey-curator-0.1.7/src/xmonkey_curator/handlers/ruby_handler.py` & `xmonkey-curator-0.1.9/src/xmonkey_curator/handlers/ruby_handler.py`

 * *Files identical despite different names*

### Comparing `xmonkey-curator-0.1.7/src/xmonkey_curator/handlers/rust_handler.py` & `xmonkey-curator-0.1.9/src/xmonkey_curator/handlers/rust_handler.py`

 * *Files identical despite different names*

### Comparing `xmonkey-curator-0.1.7/src/xmonkey_curator/handlers/sharedlib_handler.py` & `xmonkey-curator-0.1.9/src/xmonkey_curator/handlers/sharedlib_handler.py`

 * *Files identical despite different names*

### Comparing `xmonkey-curator-0.1.7/src/xmonkey_curator/handlers/text_handler.py` & `xmonkey-curator-0.1.9/src/xmonkey_curator/handlers/text_handler.py`

 * *Files identical despite different names*

### Comparing `xmonkey-curator-0.1.7/src/xmonkey_curator/lexer_utilities.py` & `xmonkey-curator-0.1.9/src/xmonkey_curator/lexer_utilities.py`

 * *Files identical despite different names*

### Comparing `xmonkey-curator-0.1.7/src/xmonkey_curator/report_generator.py` & `xmonkey-curator-0.1.9/src/xmonkey_curator/report_generator.py`

 * *Files identical despite different names*

### Comparing `xmonkey-curator-0.1.7/src/xmonkey_curator/rules_handler.py` & `xmonkey-curator-0.1.9/src/xmonkey_curator/rules_handler.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,18 +22,23 @@
     def __init__(self, configuration):
         self.container = []
         self.filepaths = []
         self.configuration = configuration
 
     def classifier(self, results):
         for result in results:
+            entry = {}
             for configStr in self.configuration:
-                if configStr in result['file_path']:
-                    result['FileNameMatch'] = configStr
-            self.container.append(result)
+                configStr = configStr.lower()
+                if configStr in result['file_path'].lower():
+                    entry['file_path'] = result['file_path']
+                    entry['hashes'] = result['hashes']
+                    entry['parent_checksum'] = result['parent_checksum']
+                    entry['FileNameMatch'] = configStr
+                    self.container.append(entry)
         return self.container
 
 
 class RulesHandler:
     def __init__(self):
         self.rules = []
         self.load_rules_from_package()
```

### Comparing `xmonkey-curator-0.1.7/src/xmonkey_curator/scanner.py` & `xmonkey-curator-0.1.9/src/xmonkey_curator/scanner.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from tqdm import tqdm
 from xmonkey_curator.handler_registry import get_handler
 from xmonkey_curator.report_generator import ReportGenerator
 from xmonkey_curator.handlers.archive_handler import ArchiveHandler
 from xmonkey_curator.file_utilities import FileUtilities
 from xmonkey_curator.symbols_handler import SymbolsHandler
 from xmonkey_curator.rules_handler import RulesHandler
+from xmonkey_curator.signatures_handler import SignatureUpdater
 
 
 logging.basicConfig(
     filename='debug.log',
     level=logging.INFO,
     format='%(asctime)s - %(name)s - %(levelname)s - %(message)s'
 )
@@ -41,15 +42,20 @@
     'application/x-rpm',
     'application/x-debian-package',
     'application/java-archive',
     'application/vnd.android.package-archive',
 ]
 
 
-@click.command()
+@click.group()
+def cli():
+    pass
+
+
+@cli.command(help="Scan target files using selected options")
 @click.argument('path', type=click.Path(exists=True))
 @click.option('--force-text', '-t', is_flag=True,
               help="Force using StringExtract for all files.")
 @click.option('--recursive-extraction', '-r', is_flag=True,
               help="Extracting archives files.")
 @click.option('--export-symbols', '-s', is_flag=True,
               help="Include words in the final report.")
@@ -64,14 +70,15 @@
          match_symbols,
          print_report):
     if not recursive_extraction:
         export_symbols = False
     if not export_symbols:
         match_symbols = False
     results = []
+    report = {}
     if os.path.isdir(path):
         logger.info(f"Scanning directory: {path}")
         all_files = [
             os.path.join(root, file)
             for root, _, files in os.walk(path)
             for file in files
         ]
@@ -89,27 +96,38 @@
             '',
             force_text,
             recursive_extraction,
             export_symbols
         )
         if result:
             results.append(result)
+    report['scan_results'] = results
     rules = RulesHandler()
-    results = rules.execute(results)
+    ruleset_results = rules.execute(results)
+    if ruleset_results:
+        report['ruleset_results'] = ruleset_results
     if match_symbols:
         sym_matcher = SymbolsHandler()
         matches = sym_matcher.search(results)
-        results = results + matches
-    report_generator = ReportGenerator(results)
+        report['symbols_matching'] = matches
+    report_generator = ReportGenerator(report)
     if print_report:
         report_generator.print_report()
     else:
         report_generator.save_report('scan_report.json')
 
 
+@cli.command(name='update', help="Update local signature files")
+def update_signatures_command():
+    SignatureUpdater.fetch_and_update_signatures(
+        'Xpertians', 'BSA-Signatures-Experimental', 'signatures'
+    )
+    click.echo("Signatures updated successfully.")
+
+
 def process_file(file_path,
                  results,
                  archive_checksum=None,
                  force_text=False,
                  recursive_extraction=False,
                  export_symbols=False):
     mime_type = FileUtilities.identify_mime_type(file_path)
@@ -241,8 +259,8 @@
                 f"No handler registered for MIME type: {mime_type} "
                 f"for file {file_path}"
             )
             return None
 
 
 if __name__ == '__main__':
-    scan()
+    cli()
```

### Comparing `xmonkey-curator-0.1.7/src/xmonkey_curator/signatures/ffmpeg.json` & `xmonkey-curator-0.1.9/src/xmonkey_curator/signatures/ffmpeg.json`

 * *Files identical despite different names*

### Comparing `xmonkey-curator-0.1.7/src/xmonkey_curator/symbols_handler.py` & `xmonkey-curator-0.1.9/src/xmonkey_curator/symbols_handler.py`

 * *Files identical despite different names*

### Comparing `xmonkey-curator-0.1.7/src/xmonkey_curator.egg-info/PKG-INFO` & `xmonkey-curator-0.1.9/src/xmonkey_curator.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xmonkey-curator
-Version: 0.1.7
+Version: 0.1.9
 Summary: Automated OSS curation scanner
 Home-page: https://github.com/Xpertians/xmonkey-curator
 Author: Oscar Valenzuela
 Author-email: oscar.valenzuela.b@gmail.com
 License: Apache 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -17,14 +17,15 @@
 Requires-Dist: python-magic
 Requires-Dist: libmagic
 Requires-Dist: pygments
 Requires-Dist: ssdeep
 Requires-Dist: tqdm
 Requires-Dist: rpmfile
 Requires-Dist: zstandard
+Requires-Dist: requests
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 
 # XMonkey Curator - Automated DESCAM tooling
 
 ## Summary
```

### Comparing `xmonkey-curator-0.1.7/src/xmonkey_curator.egg-info/SOURCES.txt` & `xmonkey-curator-0.1.9/src/xmonkey_curator.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 src/xmonkey_curator/base_handler.py
 src/xmonkey_curator/file_utilities.py
 src/xmonkey_curator/handler_registry.py
 src/xmonkey_curator/lexer_utilities.py
 src/xmonkey_curator/report_generator.py
 src/xmonkey_curator/rules_handler.py
 src/xmonkey_curator/scanner.py
+src/xmonkey_curator/signatures_handler.py
 src/xmonkey_curator/symbols_handler.py
 src/xmonkey_curator.egg-info/PKG-INFO
 src/xmonkey_curator.egg-info/SOURCES.txt
 src/xmonkey_curator.egg-info/dependency_links.txt
 src/xmonkey_curator.egg-info/entry_points.txt
 src/xmonkey_curator.egg-info/requires.txt
 src/xmonkey_curator.egg-info/top_level.txt
```

### Comparing `xmonkey-curator-0.1.7/tests/test_base_handler.py` & `xmonkey-curator-0.1.9/tests/test_base_handler.py`

 * *Files identical despite different names*

### Comparing `xmonkey-curator-0.1.7/tests/test_text_handler.py` & `xmonkey-curator-0.1.9/tests/test_text_handler.py`

 * *Files identical despite different names*

