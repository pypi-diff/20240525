# Comparing `tmp/zodchy_notations-0.1.2.tar.gz` & `tmp/zodchy_notations-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zodchy_notations-0.1.2.tar", max compression
+gzip compressed data, was "zodchy_notations-0.1.3.tar", max compression
```

## Comparing `zodchy_notations-0.1.2.tar` & `zodchy_notations-0.1.3.tar`

### file list

```diff
@@ -1,10 +1,6 @@
--rw-r--r--   0        0        0        7 2023-08-10 15:42:17.045483 zodchy_notations-0.1.2/README.md
--rw-r--r--   0        0        0      425 2024-04-29 10:49:14.831691 zodchy_notations-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       20 2024-04-27 06:57:44.545249 zodchy_notations-0.1.2/zodchy_notations/__init__.py
--rw-r--r--   0        0        0       19 2024-04-27 06:57:44.549266 zodchy_notations-0.1.2/zodchy_notations/query/__init__.py
--rw-r--r--   0        0        0      199 2024-04-29 10:38:01.392581 zodchy_notations-0.1.2/zodchy_notations/query/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      206 2024-04-29 10:40:10.912374 zodchy_notations-0.1.2/zodchy_notations/query/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     6787 2024-04-29 10:38:01.393653 zodchy_notations-0.1.2/zodchy_notations/query/__pycache__/math.cpython-310.pyc
--rw-r--r--   0        0        0    13538 2024-04-29 10:48:00.491625 zodchy_notations-0.1.2/zodchy_notations/query/__pycache__/math.cpython-312.pyc
--rw-r--r--   0        0        0     8571 2024-04-29 10:48:00.285679 zodchy_notations-0.1.2/zodchy_notations/query/math.py
--rw-r--r--   0        0        0      503 1970-01-01 00:00:00.000000 zodchy_notations-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        7 2023-08-10 15:42:17.045483 zodchy_notations-0.1.3/README.md
+-rw-r--r--   0        0        0      425 2024-05-25 17:34:33.528636 zodchy_notations-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       20 2024-04-27 06:57:44.545249 zodchy_notations-0.1.3/zodchy_notations/__init__.py
+-rw-r--r--   0        0        0       19 2024-04-27 06:57:44.549266 zodchy_notations-0.1.3/zodchy_notations/query/__init__.py
+-rw-r--r--   0        0        0     8571 2024-04-29 10:48:00.285679 zodchy_notations-0.1.3/zodchy_notations/query/math.py
+-rw-r--r--   0        0        0      554 1970-01-01 00:00:00.000000 zodchy_notations-0.1.3/PKG-INFO
```

### Comparing `zodchy_notations-0.1.2/zodchy_notations/query/math.py` & `zodchy_notations-0.1.3/zodchy_notations/query/math.py`

 * *Files identical despite different names*

