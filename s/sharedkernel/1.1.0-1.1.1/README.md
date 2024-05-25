# Comparing `tmp/sharedkernel-1.1.0.tar.gz` & `tmp/sharedkernel-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sharedkernel-1.1.0.tar", last modified: Sun May 19 06:30:11 2024, max compression
+gzip compressed data, was "sharedkernel-1.1.1.tar", last modified: Sat May 25 13:26:33 2024, max compression
```

## Comparing `sharedkernel-1.1.0.tar` & `sharedkernel-1.1.1.tar`

### file list

```diff
@@ -1,39 +1,38 @@
-drwxrwxrwx   0        0        0        0 2024-05-19 06:30:11.250186 sharedkernel-1.1.0/
--rw-rw-rw-   0        0        0      323 2024-05-19 06:30:11.248185 sharedkernel-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      932 2024-04-22 08:34:48.000000 sharedkernel-1.1.0/README.md
--rw-rw-rw-   0        0        0       42 2024-05-19 06:30:11.251186 sharedkernel-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      609 2024-05-18 08:51:03.000000 sharedkernel-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-19 06:30:10.788519 sharedkernel-1.1.0/sharedkernel/
--rw-rw-rw-   0        0        0      622 2024-04-07 22:32:56.000000 sharedkernel-1.1.0/sharedkernel/common.py
--rw-rw-rw-   0        0        0      326 2024-04-08 09:14:39.000000 sharedkernel-1.1.0/sharedkernel/config.py
-drwxrwxrwx   0        0        0        0 2024-05-19 06:30:10.961319 sharedkernel-1.1.0/sharedkernel/database/
--rw-rw-rw-   0        0        0      114 2024-05-18 09:07:04.000000 sharedkernel-1.1.0/sharedkernel/database/__init__.py
--rw-rw-rw-   0        0        0      190 2024-04-09 05:59:22.000000 sharedkernel-1.1.0/sharedkernel/database/adapter.py
--rw-rw-rw-   0        0        0     2417 2024-05-15 12:13:18.000000 sharedkernel-1.1.0/sharedkernel/database/mongo_repository_base.py
-drwxrwxrwx   0        0        0        0 2024-05-19 06:30:11.012602 sharedkernel-1.1.0/sharedkernel/database/vector_database_repository/
--rw-rw-rw-   0        0        0      146 2024-05-18 09:02:01.000000 sharedkernel-1.1.0/sharedkernel/database/vector_database_repository/__init__.py
--rw-rw-rw-   0        0        0     1279 2024-05-18 10:14:58.000000 sharedkernel-1.1.0/sharedkernel/database/vector_database_repository/chroma_startegy.py
--rw-rw-rw-   0        0        0     1930 2024-05-19 06:26:59.000000 sharedkernel-1.1.0/sharedkernel/database/vector_database_repository/milvus_strategy.py
--rw-rw-rw-   0        0        0     1245 2024-05-18 10:07:13.000000 sharedkernel-1.1.0/sharedkernel/database/vector_database_repository/vector_database_repository.py
--rw-rw-rw-   0        0        0      538 2024-05-18 10:05:23.000000 sharedkernel-1.1.0/sharedkernel/database/vector_database_repository/vector_database_strategy.py
-drwxrwxrwx   0        0        0        0 2024-05-19 06:30:11.085011 sharedkernel-1.1.0/sharedkernel/enum/
--rw-rw-rw-   0        0        0       87 2024-05-18 08:51:03.000000 sharedkernel-1.1.0/sharedkernel/enum/__init__.py
--rw-rw-rw-   0        0        0      387 2024-04-07 22:39:14.000000 sharedkernel-1.1.0/sharedkernel/enum/error_code.py
--rw-rw-rw-   0        0        0      104 2024-05-15 12:22:32.000000 sharedkernel-1.1.0/sharedkernel/enum/vector_database_type.py
-drwxrwxrwx   0        0        0        0 2024-05-19 06:30:11.156108 sharedkernel-1.1.0/sharedkernel/exception/
--rw-rw-rw-   0        0        0      319 2024-04-22 07:11:30.000000 sharedkernel-1.1.0/sharedkernel/exception/__init__.py
--rw-rw-rw-   0        0        0     1016 2024-04-08 09:11:03.000000 sharedkernel-1.1.0/sharedkernel/exception/exception.py
--rw-rw-rw-   0        0        0     3176 2024-04-22 07:11:48.000000 sharedkernel-1.1.0/sharedkernel/exception/exception_handlers.py
--rw-rw-rw-   0        0        0     1178 2024-04-22 06:50:49.000000 sharedkernel-1.1.0/sharedkernel/jwt_service.py
-drwxrwxrwx   0        0        0        0 2024-05-19 06:30:11.238678 sharedkernel-1.1.0/sharedkernel/objects/
--rw-rw-rw-   0        0        0      100 2024-04-22 06:50:23.000000 sharedkernel-1.1.0/sharedkernel/objects/__init__.py
--rw-rw-rw-   0        0        0      186 2024-04-07 22:32:56.000000 sharedkernel-1.1.0/sharedkernel/objects/base_document.py
--rw-rw-rw-   0        0        0      134 2024-04-08 09:19:23.000000 sharedkernel-1.1.0/sharedkernel/objects/jwt_model.py
--rw-rw-rw-   0        0        0      721 2024-04-08 09:11:09.000000 sharedkernel-1.1.0/sharedkernel/objects/result.py
--rw-rw-rw-   0        0        0       98 2024-04-07 22:32:56.000000 sharedkernel-1.1.0/sharedkernel/string_extentions.py
-drwxrwxrwx   0        0        0        0 2024-05-19 06:30:11.246657 sharedkernel-1.1.0/sharedkernel.egg-info/
--rw-rw-rw-   0        0        0      323 2024-05-19 06:30:10.000000 sharedkernel-1.1.0/sharedkernel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1128 2024-05-19 06:30:10.000000 sharedkernel-1.1.0/sharedkernel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-19 06:30:10.000000 sharedkernel-1.1.0/sharedkernel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2024-05-19 06:30:10.000000 sharedkernel-1.1.0/sharedkernel.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-19 06:30:10.000000 sharedkernel-1.1.0/sharedkernel.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-25 13:26:33.256806 sharedkernel-1.1.1/
+-rw-rw-rw-   0        0        0      323 2024-05-25 13:26:33.250797 sharedkernel-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      932 2024-04-22 08:34:48.000000 sharedkernel-1.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-25 13:26:33.257799 sharedkernel-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      609 2024-05-25 12:16:20.000000 sharedkernel-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-25 13:26:33.094800 sharedkernel-1.1.1/sharedkernel/
+-rw-rw-rw-   0        0        0      622 2024-04-07 22:32:56.000000 sharedkernel-1.1.1/sharedkernel/common.py
+-rw-rw-rw-   0        0        0      326 2024-04-08 09:14:39.000000 sharedkernel-1.1.1/sharedkernel/config.py
+drwxrwxrwx   0        0        0        0 2024-05-25 13:26:33.159799 sharedkernel-1.1.1/sharedkernel/database/
+-rw-rw-rw-   0        0        0      114 2024-05-18 09:07:04.000000 sharedkernel-1.1.1/sharedkernel/database/__init__.py
+-rw-rw-rw-   0        0        0     1986 2024-05-25 13:25:52.000000 sharedkernel-1.1.1/sharedkernel/database/mongo_generic_repository.py
+drwxrwxrwx   0        0        0        0 2024-05-25 13:26:33.179798 sharedkernel-1.1.1/sharedkernel/database/vector_database_repository/
+-rw-rw-rw-   0        0        0      146 2024-05-18 09:02:01.000000 sharedkernel-1.1.1/sharedkernel/database/vector_database_repository/__init__.py
+-rw-rw-rw-   0        0        0     1279 2024-05-18 10:14:58.000000 sharedkernel-1.1.1/sharedkernel/database/vector_database_repository/chroma_startegy.py
+-rw-rw-rw-   0        0        0     1930 2024-05-21 13:29:44.000000 sharedkernel-1.1.1/sharedkernel/database/vector_database_repository/milvus_strategy.py
+-rw-rw-rw-   0        0        0     1245 2024-05-18 10:07:13.000000 sharedkernel-1.1.1/sharedkernel/database/vector_database_repository/vector_database_repository.py
+-rw-rw-rw-   0        0        0      538 2024-05-18 10:05:23.000000 sharedkernel-1.1.1/sharedkernel/database/vector_database_repository/vector_database_strategy.py
+drwxrwxrwx   0        0        0        0 2024-05-25 13:26:33.201798 sharedkernel-1.1.1/sharedkernel/enum/
+-rw-rw-rw-   0        0        0       87 2024-05-18 08:51:03.000000 sharedkernel-1.1.1/sharedkernel/enum/__init__.py
+-rw-rw-rw-   0        0        0      387 2024-04-07 22:39:14.000000 sharedkernel-1.1.1/sharedkernel/enum/error_code.py
+-rw-rw-rw-   0        0        0      104 2024-05-15 12:22:32.000000 sharedkernel-1.1.1/sharedkernel/enum/vector_database_type.py
+drwxrwxrwx   0        0        0        0 2024-05-25 13:26:33.218798 sharedkernel-1.1.1/sharedkernel/exception/
+-rw-rw-rw-   0        0        0      319 2024-04-22 07:11:30.000000 sharedkernel-1.1.1/sharedkernel/exception/__init__.py
+-rw-rw-rw-   0        0        0     1016 2024-04-08 09:11:03.000000 sharedkernel-1.1.1/sharedkernel/exception/exception.py
+-rw-rw-rw-   0        0        0     3176 2024-04-22 07:11:48.000000 sharedkernel-1.1.1/sharedkernel/exception/exception_handlers.py
+-rw-rw-rw-   0        0        0     1178 2024-04-22 06:50:49.000000 sharedkernel-1.1.1/sharedkernel/jwt_service.py
+drwxrwxrwx   0        0        0        0 2024-05-25 13:26:33.240802 sharedkernel-1.1.1/sharedkernel/objects/
+-rw-rw-rw-   0        0        0      100 2024-04-22 06:50:23.000000 sharedkernel-1.1.1/sharedkernel/objects/__init__.py
+-rw-rw-rw-   0        0        0      186 2024-04-07 22:32:56.000000 sharedkernel-1.1.1/sharedkernel/objects/base_document.py
+-rw-rw-rw-   0        0        0      134 2024-04-08 09:19:23.000000 sharedkernel-1.1.1/sharedkernel/objects/jwt_model.py
+-rw-rw-rw-   0        0        0      721 2024-04-08 09:11:09.000000 sharedkernel-1.1.1/sharedkernel/objects/result.py
+-rw-rw-rw-   0        0        0       98 2024-04-07 22:32:56.000000 sharedkernel-1.1.1/sharedkernel/string_extentions.py
+drwxrwxrwx   0        0        0        0 2024-05-25 13:26:33.248807 sharedkernel-1.1.1/sharedkernel.egg-info/
+-rw-rw-rw-   0        0        0      323 2024-05-25 13:26:32.000000 sharedkernel-1.1.1/sharedkernel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1098 2024-05-25 13:26:33.000000 sharedkernel-1.1.1/sharedkernel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 13:26:32.000000 sharedkernel-1.1.1/sharedkernel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2024-05-25 13:26:32.000000 sharedkernel-1.1.1/sharedkernel.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-25 13:26:32.000000 sharedkernel-1.1.1/sharedkernel.egg-info/top_level.txt
```

### Comparing `sharedkernel-1.1.0/README.md` & `sharedkernel-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `sharedkernel-1.1.0/setup.py` & `sharedkernel-1.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,10 +4,10 @@
     # Needed to silence warnings (and to be a worthwhile package)
     name='sharedkernel',
     author='Smilinno',
     packages=['sharedkernel','sharedkernel.database','sharedkernel.database.vector_database_repository','sharedkernel.enum','sharedkernel.exception','sharedkernel.objects'],
     # Needed for dependencies
     install_requires=['numpy','requests','pymongo','fastapi==0.89.1','PyJWT','pymilvus','chromadb'],
     # *strongly* suggested for sharing
-    version='1.1.0',
+    version='1.1.1',
     description='sharekernel is an shared package between all python projects',
 )
```

### Comparing `sharedkernel-1.1.0/sharedkernel/common.py` & `sharedkernel-1.1.1/sharedkernel/common.py`

 * *Files identical despite different names*

### Comparing `sharedkernel-1.1.0/sharedkernel/database/vector_database_repository/chroma_startegy.py` & `sharedkernel-1.1.1/sharedkernel/database/vector_database_repository/chroma_startegy.py`

 * *Files identical despite different names*

### Comparing `sharedkernel-1.1.0/sharedkernel/database/vector_database_repository/milvus_strategy.py` & `sharedkernel-1.1.1/sharedkernel/database/vector_database_repository/milvus_strategy.py`

 * *Files identical despite different names*

### Comparing `sharedkernel-1.1.0/sharedkernel/database/vector_database_repository/vector_database_repository.py` & `sharedkernel-1.1.1/sharedkernel/database/vector_database_repository/vector_database_repository.py`

 * *Files identical despite different names*

### Comparing `sharedkernel-1.1.0/sharedkernel/database/vector_database_repository/vector_database_strategy.py` & `sharedkernel-1.1.1/sharedkernel/database/vector_database_repository/vector_database_strategy.py`

 * *Files identical despite different names*

### Comparing `sharedkernel-1.1.0/sharedkernel/exception/exception.py` & `sharedkernel-1.1.1/sharedkernel/exception/exception.py`

 * *Files identical despite different names*

### Comparing `sharedkernel-1.1.0/sharedkernel/exception/exception_handlers.py` & `sharedkernel-1.1.1/sharedkernel/exception/exception_handlers.py`

 * *Files identical despite different names*

### Comparing `sharedkernel-1.1.0/sharedkernel/jwt_service.py` & `sharedkernel-1.1.1/sharedkernel/jwt_service.py`

 * *Files identical despite different names*

### Comparing `sharedkernel-1.1.0/sharedkernel/objects/result.py` & `sharedkernel-1.1.1/sharedkernel/objects/result.py`

 * *Files identical despite different names*

### Comparing `sharedkernel-1.1.0/sharedkernel.egg-info/SOURCES.txt` & `sharedkernel-1.1.1/sharedkernel.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -6,16 +6,15 @@
 sharedkernel/string_extentions.py
 sharedkernel.egg-info/PKG-INFO
 sharedkernel.egg-info/SOURCES.txt
 sharedkernel.egg-info/dependency_links.txt
 sharedkernel.egg-info/requires.txt
 sharedkernel.egg-info/top_level.txt
 sharedkernel/database/__init__.py
-sharedkernel/database/adapter.py
-sharedkernel/database/mongo_repository_base.py
+sharedkernel/database/mongo_generic_repository.py
 sharedkernel/database/vector_database_repository/__init__.py
 sharedkernel/database/vector_database_repository/chroma_startegy.py
 sharedkernel/database/vector_database_repository/milvus_strategy.py
 sharedkernel/database/vector_database_repository/vector_database_repository.py
 sharedkernel/database/vector_database_repository/vector_database_strategy.py
 sharedkernel/enum/__init__.py
 sharedkernel/enum/error_code.py
```

