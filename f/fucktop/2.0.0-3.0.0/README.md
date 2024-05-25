# Comparing `tmp/fucktop-2.0.0.tar.gz` & `tmp/fucktop-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\fucktop-2.0.0.tar", last modified: Sat May 25 12:58:38 2024, max compression
+gzip compressed data, was "dist\fucktop-3.0.0.tar", last modified: Sat May 25 13:06:18 2024, max compression
```

## Comparing `fucktop-2.0.0.tar` & `fucktop-3.0.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-25 12:58:38.000000 fucktop-2.0.0/
--rw-rw-rw-   0        0        0      790 2024-05-25 12:58:38.000000 fucktop-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      337 2024-05-25 12:43:30.000000 fucktop-2.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-25 12:58:38.000000 fucktop-2.0.0/fucktop.egg-info/
--rw-rw-rw-   0        0        0      790 2024-05-25 12:58:38.000000 fucktop-2.0.0/fucktop.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      183 2024-05-25 12:58:38.000000 fucktop-2.0.0/fucktop.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-25 12:58:38.000000 fucktop-2.0.0/fucktop.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-05-25 12:58:38.000000 fucktop-2.0.0/fucktop.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-25 12:58:38.000000 fucktop-2.0.0/fucktop.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      979 2024-05-25 12:14:50.000000 fucktop-2.0.0/fucktop.py
--rw-rw-rw-   0        0        0       42 2024-05-25 12:58:38.000000 fucktop-2.0.0/setup.cfg
--rw-rw-rw-   0        0        0      489 2024-05-25 12:58:15.000000 fucktop-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-25 13:06:18.000000 fucktop-3.0.0/
+-rw-rw-rw-   0        0        0      790 2024-05-25 13:06:18.000000 fucktop-3.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0      337 2024-05-25 12:43:30.000000 fucktop-3.0.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-25 13:06:18.000000 fucktop-3.0.0/fucktop.egg-info/
+-rw-rw-rw-   0        0        0      790 2024-05-25 13:06:17.000000 fucktop-3.0.0/fucktop.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      183 2024-05-25 13:06:17.000000 fucktop-3.0.0/fucktop.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 13:06:17.000000 fucktop-3.0.0/fucktop.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-25 13:06:17.000000 fucktop-3.0.0/fucktop.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-25 13:06:17.000000 fucktop-3.0.0/fucktop.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1779 2024-05-25 13:04:39.000000 fucktop-3.0.0/fucktop.py
+-rw-rw-rw-   0        0        0       42 2024-05-25 13:06:18.000000 fucktop-3.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      489 2024-05-25 13:05:57.000000 fucktop-3.0.0/setup.py
```

### Comparing `fucktop-2.0.0/PKG-INFO` & `fucktop-3.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fucktop
-Version: 2.0.0
+Version: 3.0.0
 Summary: 一个免费而热搜工具(喜欢关注:python学霸微信公众号)
 Home-page: UNKNOWN
 Author: Python学霸
 Author-email: python@xueba.com
 License: UNKNOWN
 Description: 
         ### 介绍
```

### Comparing `fucktop-2.0.0/fucktop.egg-info/PKG-INFO` & `fucktop-3.0.0/fucktop.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fucktop
-Version: 2.0.0
+Version: 3.0.0
 Summary: 一个免费而热搜工具(喜欢关注:python学霸微信公众号)
 Home-page: UNKNOWN
 Author: Python学霸
 Author-email: python@xueba.com
 License: UNKNOWN
 Description: 
         ### 介绍
```

