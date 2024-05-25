# Comparing `tmp/hermitage-0.1.7.tar.gz` & `tmp/hermitage-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hermitage-0.1.7.tar", max compression
+gzip compressed data, was "hermitage-0.2.0.tar", max compression
```

## Comparing `hermitage-0.1.7.tar` & `hermitage-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,13 @@
--rw-r--r--   0        0        0       46 2024-04-15 11:34:36.787863 hermitage-0.1.7/README.md
--rw-r--r--   0        0        0      257 2024-04-13 13:50:37.630467 hermitage-0.1.7/hermitage/__init__.py
--rw-r--r--   0        0        0       24 2024-04-02 15:23:42.889513 hermitage-0.1.7/hermitage/definition/__init__.py
--rw-r--r--   0        0        0    11820 2024-04-13 13:19:43.140011 hermitage-0.1.7/hermitage/definition/contracts.py
--rw-r--r--   0        0        0       44 2024-04-02 15:23:42.889741 hermitage-0.1.7/hermitage/mappers/__init__.py
--rw-r--r--   0        0        0     1235 2024-04-24 07:28:43.056982 hermitage-0.1.7/hermitage/mappers/invoice.py
--rw-r--r--   0        0        0       31 2024-04-02 15:23:42.889934 hermitage-0.1.7/hermitage/parsers/__init__.py
--rw-r--r--   0        0        0     2866 2024-05-01 16:27:45.315551 hermitage-0.1.7/hermitage/parsers/query.py
--rw-r--r--   0        0        0      361 2024-05-01 16:28:24.399592 hermitage-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      558 1970-01-01 00:00:00.000000 hermitage-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0       46 2024-05-24 13:40:38.562808 hermitage-0.2.0/README.md
+-rw-r--r--   0        0        0      109 2024-05-25 13:54:06.658975 hermitage-0.2.0/hermitage/__init__.py
+-rw-r--r--   0        0        0       86 2024-05-25 13:54:06.659245 hermitage-0.2.0/hermitage/adapters/__init__.py
+-rw-r--r--   0        0        0      194 2024-05-25 13:54:06.659630 hermitage-0.2.0/hermitage/adapters/constraints.py
+-rw-r--r--   0        0        0     4731 2024-05-25 13:54:06.659834 hermitage-0.2.0/hermitage/adapters/cqea.py
+-rw-r--r--   0        0        0     1093 2024-05-25 13:54:06.660002 hermitage-0.2.0/hermitage/adapters/transformers.py
+-rw-r--r--   0        0        0       24 2024-05-25 13:54:06.660098 hermitage-0.2.0/hermitage/definitions/__init__.py
+-rw-r--r--   0        0        0       23 2024-05-25 13:54:06.660260 hermitage-0.2.0/hermitage/definitions/contracts/__init__.py
+-rw-r--r--   0        0        0      485 2024-05-25 13:54:06.660418 hermitage-0.2.0/hermitage/definitions/contracts/adapters.py
+-rw-r--r--   0        0        0      103 2024-05-25 13:54:06.660580 hermitage-0.2.0/hermitage/notation/__init__.py
+-rw-r--r--   0        0        0     4462 2024-05-25 13:54:06.660840 hermitage-0.2.0/hermitage/notation/default.py
+-rw-r--r--   0        0        0      418 2024-05-25 13:54:06.661125 hermitage-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      558 1970-01-01 00:00:00.000000 hermitage-0.2.0/PKG-INFO
```

### Comparing `hermitage-0.1.7/PKG-INFO` & `hermitage-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: hermitage
-Version: 0.1.7
+Version: 0.2.0
 Summary: Universal storage access framework
 Home-page: https://github.com/smairon/hermitage
 Author: Smairon
 Author-email: man@smairon.ru
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: zodchy (>=0.2.3,<0.3.0)
+Requires-Dist: zodchy (>=0.2.4,<0.3.0)
 Project-URL: Repository, https://github.com/smairon/hermitage
 Description-Content-Type: text/markdown
 
 # Hermitage
 Universal storage access framework
```

