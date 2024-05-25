# Comparing `tmp/better_web3-4.0.0b3.tar.gz` & `tmp/better_web3-4.0.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "better_web3-4.0.0b3.tar", max compression
+gzip compressed data, was "better_web3-4.0.0b4.tar", max compression
```

## Comparing `better_web3-4.0.0b3.tar` & `better_web3-4.0.0b4.tar`

### file list

```diff
@@ -1,20 +1,17 @@
--rw-r--r--   0        0        0      224 2024-05-25 04:36:12.322385 better_web3-4.0.0b3/better_web3/__init__.py
--rw-r--r--   0        0        0     1752 2024-05-25 04:36:12.324383 better_web3-4.0.0b3/better_web3/caip_2.py
--rw-r--r--   0        0        0    11052 2024-05-25 05:59:38.348397 better_web3-4.0.0b3/better_web3/chain.py
--rw-r--r--   0        0        0      497 2024-05-25 05:44:27.207734 better_web3-4.0.0b3/better_web3/contract.py
--rw-r--r--   0        0        0      933 2024-05-24 15:45:44.526320 better_web3-4.0.0b3/better_web3/models.py
--rw-r--r--   0        0        0      504 2024-05-25 05:40:55.256224 better_web3-4.0.0b3/better_web3/utils/__init__.py
--rw-r--r--   0        0        0      917 2023-12-16 17:27:32.282000 better_web3-4.0.0b3/better_web3/utils/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      698 2024-01-10 21:46:32.920666 better_web3-4.0.0b3/better_web3/utils/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     4358 2023-12-16 17:27:34.414000 better_web3-4.0.0b3/better_web3/utils/__pycache__/eth.cpython-311.pyc
--rw-r--r--   0        0        0     3533 2024-01-10 21:46:32.922666 better_web3-4.0.0b3/better_web3/utils/__pycache__/eth.cpython-312.pyc
--rw-r--r--   0        0        0     3719 2023-12-16 17:27:36.000000 better_web3-4.0.0b3/better_web3/utils/__pycache__/file.cpython-311.pyc
--rw-r--r--   0        0        0     2780 2024-01-10 21:46:32.923666 better_web3-4.0.0b3/better_web3/utils/__pycache__/file.cpython-312.pyc
--rw-r--r--   0        0        0      837 2023-12-16 17:27:37.593000 better_web3-4.0.0b3/better_web3/utils/__pycache__/other.cpython-311.pyc
--rw-r--r--   0        0        0      707 2024-01-10 21:46:32.927171 better_web3-4.0.0b3/better_web3/utils/__pycache__/other.cpython-312.pyc
--rw-r--r--   0        0        0      470 2024-05-25 05:40:55.251225 better_web3-4.0.0b3/better_web3/utils/eth.py
--rw-r--r--   0        0        0      331 2024-05-25 05:40:55.259224 better_web3-4.0.0b3/better_web3/utils/file.py
--rw-r--r--   0        0        0      406 2024-04-02 04:04:59.695626 better_web3-4.0.0b3/better_web3/utils/other.py
--rw-r--r--   0        0        0      521 2024-05-25 05:40:55.254223 better_web3-4.0.0b3/pyproject.toml
--rw-r--r--   0        0        0      760 2024-04-02 09:22:28.119803 better_web3-4.0.0b3/README.md
--rw-r--r--   0        0        0     1441 1970-01-01 00:00:00.000000 better_web3-4.0.0b3/PKG-INFO
+-rw-r--r--   0        0        0      224 2024-05-25 04:36:12.322385 better_web3-4.0.0b4/better_web3/__init__.py
+-rw-r--r--   0        0        0     1752 2024-05-25 04:36:12.324383 better_web3-4.0.0b4/better_web3/caip_2.py
+-rw-r--r--   0        0        0    11052 2024-05-25 05:59:38.348397 better_web3-4.0.0b4/better_web3/chain.py
+-rw-r--r--   0        0        0      497 2024-05-25 05:44:27.207734 better_web3-4.0.0b4/better_web3/contract.py
+-rw-r--r--   0        0        0      933 2024-05-24 15:45:44.526320 better_web3-4.0.0b4/better_web3/models.py
+-rw-r--r--   0        0        0      137 2024-05-25 06:19:06.436481 better_web3-4.0.0b4/better_web3/utils/__init__.py
+-rw-r--r--   0        0        0      917 2023-12-16 17:27:32.282000 better_web3-4.0.0b4/better_web3/utils/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      698 2024-01-10 21:46:32.920666 better_web3-4.0.0b4/better_web3/utils/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     4358 2023-12-16 17:27:34.414000 better_web3-4.0.0b4/better_web3/utils/__pycache__/eth.cpython-311.pyc
+-rw-r--r--   0        0        0     3533 2024-01-10 21:46:32.922666 better_web3-4.0.0b4/better_web3/utils/__pycache__/eth.cpython-312.pyc
+-rw-r--r--   0        0        0      837 2023-12-16 17:27:37.593000 better_web3-4.0.0b4/better_web3/utils/__pycache__/other.cpython-311.pyc
+-rw-r--r--   0        0        0      707 2024-01-10 21:46:32.927171 better_web3-4.0.0b4/better_web3/utils/__pycache__/other.cpython-312.pyc
+-rw-r--r--   0        0        0      434 2024-05-25 06:19:06.433481 better_web3-4.0.0b4/better_web3/utils/eth.py
+-rw-r--r--   0        0        0      406 2024-04-02 04:04:59.695626 better_web3-4.0.0b4/better_web3/utils/other.py
+-rw-r--r--   0        0        0      521 2024-05-25 06:19:17.607211 better_web3-4.0.0b4/pyproject.toml
+-rw-r--r--   0        0        0      760 2024-04-02 09:22:28.119803 better_web3-4.0.0b4/README.md
+-rw-r--r--   0        0        0     1441 1970-01-01 00:00:00.000000 better_web3-4.0.0b4/PKG-INFO
```

### Comparing `better_web3-4.0.0b3/better_web3/caip_2.py` & `better_web3-4.0.0b4/better_web3/caip_2.py`

 * *Files identical despite different names*

### Comparing `better_web3-4.0.0b3/better_web3/chain.py` & `better_web3-4.0.0b4/better_web3/chain.py`

 * *Files identical despite different names*

### Comparing `better_web3-4.0.0b3/better_web3/models.py` & `better_web3-4.0.0b4/better_web3/models.py`

 * *Files identical despite different names*

### Comparing `better_web3-4.0.0b3/better_web3/utils/__pycache__/__init__.cpython-311.pyc` & `better_web3-4.0.0b4/better_web3/utils/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-4.0.0b3/better_web3/utils/__pycache__/__init__.cpython-312.pyc` & `better_web3-4.0.0b4/better_web3/utils/__pycache__/__init__.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-4.0.0b3/better_web3/utils/__pycache__/eth.cpython-311.pyc` & `better_web3-4.0.0b4/better_web3/utils/__pycache__/eth.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-4.0.0b3/better_web3/utils/__pycache__/eth.cpython-312.pyc` & `better_web3-4.0.0b4/better_web3/utils/__pycache__/eth.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-4.0.0b3/better_web3/utils/__pycache__/other.cpython-311.pyc` & `better_web3-4.0.0b4/better_web3/utils/__pycache__/other.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-4.0.0b3/better_web3/utils/__pycache__/other.cpython-312.pyc` & `better_web3-4.0.0b4/better_web3/utils/__pycache__/other.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-4.0.0b3/pyproject.toml` & `better_web3-4.0.0b4/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "better-web3"
-version = "4.0.0.b3"
+version = "4.0.0.b4"
 description = "Web3 stuff"
 authors = ["Alen <alen.kimov@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/alenkimov/better_web3"
 packages = [{include = "better_web3"}]
 
 [tool.poetry.dependencies]
```

### Comparing `better_web3-4.0.0b3/README.md` & `better_web3-4.0.0b4/README.md`

 * *Files identical despite different names*

### Comparing `better_web3-4.0.0b3/PKG-INFO` & `better_web3-4.0.0b4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: better-web3
-Version: 4.0.0b3
+Version: 4.0.0b4
 Summary: Web3 stuff
 Home-page: https://github.com/alenkimov/better_web3
 Author: Alen
 Author-email: alen.kimov@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

