# Comparing `tmp/dyff_schema-0.8.0.tar.gz` & `tmp/dyff_schema-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dyff_schema-0.8.0.tar", last modified: Thu May 23 22:39:38 2024, max compression
+gzip compressed data, was "dyff_schema-0.9.0.tar", last modified: Fri May 24 22:06:16 2024, max compression
```

## Comparing `dyff_schema-0.8.0.tar` & `dyff_schema-0.9.0.tar`

### file list

```diff
@@ -1,66 +1,67 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 22:39:38.539608 dyff_schema-0.8.0/
--rw-rw-rw-   0 root         (0) root         (0)      434 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1399 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      489 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/.licenserc.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1686 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      108 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/.prettierignore
--rw-rw-rw-   0 root         (0) root         (0)     2192 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/.secrets.baseline
--rw-rw-rw-   0 root         (0) root         (0)     5503 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/CODE_OF_CONDUCT.md
--rw-rw-rw-   0 root         (0) root         (0)    11357 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       43 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/NOTICE
--rw-r--r--   0 root         (0) root         (0)     3458 2024-05-23 22:39:38.539608 dyff_schema-0.8.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2312 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 22:39:38.524608 dyff_schema-0.8.0/dyff/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 22:39:38.531608 dyff_schema-0.8.0/dyff/schema/
--rw-rw-rw-   0 root         (0) root         (0)     1031 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/dyff/schema/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      123 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/dyff/schema/adapters.py
--rw-rw-rw-   0 root         (0) root         (0)      119 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/dyff/schema/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1075 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/dyff/schema/copydoc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 22:39:38.532608 dyff_schema-0.8.0/dyff/schema/dataset/
--rw-rw-rw-   0 root         (0) root         (0)      123 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/dyff/schema/dataset/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      129 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/dyff/schema/dataset/arrow.py
--rw-rw-rw-   0 root         (0) root         (0)      130 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/dyff/schema/dataset/binary.py
--rw-rw-rw-   0 root         (0) root         (0)      138 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/dyff/schema/dataset/classification.py
--rw-rw-rw-   0 root         (0) root         (0)      128 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/dyff/schema/dataset/text.py
--rw-rw-rw-   0 root         (0) root         (0)      130 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/dyff/schema/dataset/vision.py
--rw-rw-rw-   0 root         (0) root         (0)     1422 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/dyff/schema/ids.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 22:39:38.532608 dyff_schema-0.8.0/dyff/schema/io/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/dyff/schema/io/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      123 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/dyff/schema/io/vllm.py
--rw-rw-rw-   0 root         (0) root         (0)      123 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/dyff/schema/platform.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/dyff/schema/py.typed
--rw-rw-rw-   0 root         (0) root         (0)     3788 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/dyff/schema/quantity.py
--rw-rw-rw-   0 root         (0) root         (0)      123 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/dyff/schema/requests.py
--rw-rw-rw-   0 root         (0) root         (0)      119 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/dyff/schema/test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 22:39:38.533608 dyff_schema-0.8.0/dyff/schema/v0/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/dyff/schema/v0/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 22:39:38.534608 dyff_schema-0.8.0/dyff/schema/v0/r1/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/dyff/schema/v0/r1/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    23552 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/dyff/schema/v0/r1/adapters.py
--rw-rw-rw-   0 root         (0) root         (0)    19385 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/dyff/schema/v0/r1/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 22:39:38.536608 dyff_schema-0.8.0/dyff/schema/v0/r1/dataset/
--rw-rw-rw-   0 root         (0) root         (0)     2553 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/dyff/schema/v0/r1/dataset/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12312 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/dyff/schema/v0/r1/dataset/arrow.py
--rw-rw-rw-   0 root         (0) root         (0)      544 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/dyff/schema/v0/r1/dataset/binary.py
--rw-rw-rw-   0 root         (0) root         (0)      311 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/dyff/schema/v0/r1/dataset/classification.py
--rw-rw-rw-   0 root         (0) root         (0)     1008 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/dyff/schema/v0/r1/dataset/text.py
--rw-rw-rw-   0 root         (0) root         (0)      369 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/dyff/schema/v0/r1/dataset/vision.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 22:39:38.536608 dyff_schema-0.8.0/dyff/schema/v0/r1/io/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/dyff/schema/v0/r1/io/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5320 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/dyff/schema/v0/r1/io/vllm.py
--rw-rw-rw-   0 root         (0) root         (0)    61413 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/dyff/schema/v0/r1/platform.py
--rw-rw-rw-   0 root         (0) root         (0)     9728 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/dyff/schema/v0/r1/requests.py
--rw-rw-rw-   0 root         (0) root         (0)    10720 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/dyff/schema/v0/r1/test.py
--rw-rw-rw-   0 root         (0) root         (0)      392 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/dyff/schema/v0/r1/version.py
--rw-rw-rw-   0 root         (0) root         (0)      372 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/dyff/schema/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 22:39:38.538608 dyff_schema-0.8.0/dyff_schema.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3458 2024-05-23 22:39:38.000000 dyff_schema-0.8.0/dyff_schema.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1358 2024-05-23 22:39:38.000000 dyff_schema-0.8.0/dyff_schema.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 22:39:38.000000 dyff_schema-0.8.0/dyff_schema.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       64 2024-05-23 22:39:38.000000 dyff_schema-0.8.0/dyff_schema.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-05-23 22:39:38.000000 dyff_schema-0.8.0/dyff_schema.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      502 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/makefile
--rw-rw-rw-   0 root         (0) root         (0)     1585 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-23 22:39:38.539608 dyff_schema-0.8.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 22:39:38.538608 dyff_schema-0.8.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1449 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/tests/test_import.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 22:06:16.128126 dyff_schema-0.9.0/
+-rw-rw-rw-   0 root         (0) root         (0)      434 2024-05-24 22:06:10.000000 dyff_schema-0.9.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1399 2024-05-24 22:06:10.000000 dyff_schema-0.9.0/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      489 2024-05-24 22:06:10.000000 dyff_schema-0.9.0/.licenserc.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1686 2024-05-24 22:06:10.000000 dyff_schema-0.9.0/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      108 2024-05-24 22:06:10.000000 dyff_schema-0.9.0/.prettierignore
+-rw-rw-rw-   0 root         (0) root         (0)     2192 2024-05-24 22:06:10.000000 dyff_schema-0.9.0/.secrets.baseline
+-rw-rw-rw-   0 root         (0) root         (0)     5503 2024-05-24 22:06:10.000000 dyff_schema-0.9.0/CODE_OF_CONDUCT.md
+-rw-rw-rw-   0 root         (0) root         (0)    11357 2024-05-24 22:06:10.000000 dyff_schema-0.9.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       43 2024-05-24 22:06:10.000000 dyff_schema-0.9.0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     3458 2024-05-24 22:06:16.128126 dyff_schema-0.9.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2312 2024-05-24 22:06:10.000000 dyff_schema-0.9.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 22:06:16.112126 dyff_schema-0.9.0/dyff/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 22:06:16.120126 dyff_schema-0.9.0/dyff/schema/
+-rw-rw-rw-   0 root         (0) root         (0)     1031 2024-05-24 22:06:10.000000 dyff_schema-0.9.0/dyff/schema/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      123 2024-05-24 22:06:10.000000 dyff_schema-0.9.0/dyff/schema/adapters.py
+-rw-rw-rw-   0 root         (0) root         (0)      119 2024-05-24 22:06:10.000000 dyff_schema-0.9.0/dyff/schema/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1075 2024-05-24 22:06:10.000000 dyff_schema-0.9.0/dyff/schema/copydoc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 22:06:16.121126 dyff_schema-0.9.0/dyff/schema/dataset/
+-rw-rw-rw-   0 root         (0) root         (0)      123 2024-05-24 22:06:10.000000 dyff_schema-0.9.0/dyff/schema/dataset/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      129 2024-05-24 22:06:10.000000 dyff_schema-0.9.0/dyff/schema/dataset/arrow.py
+-rw-rw-rw-   0 root         (0) root         (0)      130 2024-05-24 22:06:10.000000 dyff_schema-0.9.0/dyff/schema/dataset/binary.py
+-rw-rw-rw-   0 root         (0) root         (0)      138 2024-05-24 22:06:10.000000 dyff_schema-0.9.0/dyff/schema/dataset/classification.py
+-rw-rw-rw-   0 root         (0) root         (0)      128 2024-05-24 22:06:10.000000 dyff_schema-0.9.0/dyff/schema/dataset/text.py
+-rw-rw-rw-   0 root         (0) root         (0)      130 2024-05-24 22:06:10.000000 dyff_schema-0.9.0/dyff/schema/dataset/vision.py
+-rw-rw-rw-   0 root         (0) root         (0)     1568 2024-05-24 22:06:10.000000 dyff_schema-0.9.0/dyff/schema/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     1422 2024-05-24 22:06:10.000000 dyff_schema-0.9.0/dyff/schema/ids.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 22:06:16.122126 dyff_schema-0.9.0/dyff/schema/io/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-24 22:06:10.000000 dyff_schema-0.9.0/dyff/schema/io/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      123 2024-05-24 22:06:10.000000 dyff_schema-0.9.0/dyff/schema/io/vllm.py
+-rw-rw-rw-   0 root         (0) root         (0)      123 2024-05-24 22:06:10.000000 dyff_schema-0.9.0/dyff/schema/platform.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-24 22:06:10.000000 dyff_schema-0.9.0/dyff/schema/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)     3788 2024-05-24 22:06:10.000000 dyff_schema-0.9.0/dyff/schema/quantity.py
+-rw-rw-rw-   0 root         (0) root         (0)      123 2024-05-24 22:06:10.000000 dyff_schema-0.9.0/dyff/schema/requests.py
+-rw-rw-rw-   0 root         (0) root         (0)      119 2024-05-24 22:06:10.000000 dyff_schema-0.9.0/dyff/schema/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 22:06:16.122126 dyff_schema-0.9.0/dyff/schema/v0/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-24 22:06:10.000000 dyff_schema-0.9.0/dyff/schema/v0/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 22:06:16.124126 dyff_schema-0.9.0/dyff/schema/v0/r1/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-24 22:06:10.000000 dyff_schema-0.9.0/dyff/schema/v0/r1/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    23552 2024-05-24 22:06:10.000000 dyff_schema-0.9.0/dyff/schema/v0/r1/adapters.py
+-rw-rw-rw-   0 root         (0) root         (0)    19385 2024-05-24 22:06:10.000000 dyff_schema-0.9.0/dyff/schema/v0/r1/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 22:06:16.125126 dyff_schema-0.9.0/dyff/schema/v0/r1/dataset/
+-rw-rw-rw-   0 root         (0) root         (0)     2553 2024-05-24 22:06:10.000000 dyff_schema-0.9.0/dyff/schema/v0/r1/dataset/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12312 2024-05-24 22:06:10.000000 dyff_schema-0.9.0/dyff/schema/v0/r1/dataset/arrow.py
+-rw-rw-rw-   0 root         (0) root         (0)      544 2024-05-24 22:06:10.000000 dyff_schema-0.9.0/dyff/schema/v0/r1/dataset/binary.py
+-rw-rw-rw-   0 root         (0) root         (0)      311 2024-05-24 22:06:10.000000 dyff_schema-0.9.0/dyff/schema/v0/r1/dataset/classification.py
+-rw-rw-rw-   0 root         (0) root         (0)     1008 2024-05-24 22:06:10.000000 dyff_schema-0.9.0/dyff/schema/v0/r1/dataset/text.py
+-rw-rw-rw-   0 root         (0) root         (0)      369 2024-05-24 22:06:10.000000 dyff_schema-0.9.0/dyff/schema/v0/r1/dataset/vision.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 22:06:16.126126 dyff_schema-0.9.0/dyff/schema/v0/r1/io/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-24 22:06:10.000000 dyff_schema-0.9.0/dyff/schema/v0/r1/io/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5320 2024-05-24 22:06:10.000000 dyff_schema-0.9.0/dyff/schema/v0/r1/io/vllm.py
+-rw-rw-rw-   0 root         (0) root         (0)    61416 2024-05-24 22:06:10.000000 dyff_schema-0.9.0/dyff/schema/v0/r1/platform.py
+-rw-rw-rw-   0 root         (0) root         (0)     9857 2024-05-24 22:06:10.000000 dyff_schema-0.9.0/dyff/schema/v0/r1/requests.py
+-rw-rw-rw-   0 root         (0) root         (0)    10720 2024-05-24 22:06:10.000000 dyff_schema-0.9.0/dyff/schema/v0/r1/test.py
+-rw-rw-rw-   0 root         (0) root         (0)      392 2024-05-24 22:06:10.000000 dyff_schema-0.9.0/dyff/schema/v0/r1/version.py
+-rw-rw-rw-   0 root         (0) root         (0)      372 2024-05-24 22:06:10.000000 dyff_schema-0.9.0/dyff/schema/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 22:06:16.127126 dyff_schema-0.9.0/dyff_schema.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3458 2024-05-24 22:06:16.000000 dyff_schema-0.9.0/dyff_schema.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1380 2024-05-24 22:06:16.000000 dyff_schema-0.9.0/dyff_schema.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-24 22:06:16.000000 dyff_schema-0.9.0/dyff_schema.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       64 2024-05-24 22:06:16.000000 dyff_schema-0.9.0/dyff_schema.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-05-24 22:06:16.000000 dyff_schema-0.9.0/dyff_schema.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      502 2024-05-24 22:06:10.000000 dyff_schema-0.9.0/makefile
+-rw-rw-rw-   0 root         (0) root         (0)     1585 2024-05-24 22:06:10.000000 dyff_schema-0.9.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-24 22:06:16.128126 dyff_schema-0.9.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 22:06:16.127126 dyff_schema-0.9.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1449 2024-05-24 22:06:10.000000 dyff_schema-0.9.0/tests/test_import.py
```

### Comparing `dyff_schema-0.8.0/.gitlab-ci.yml` & `dyff_schema-0.9.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.8.0/.pre-commit-config.yaml` & `dyff_schema-0.9.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.8.0/.secrets.baseline` & `dyff_schema-0.9.0/.secrets.baseline`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.8.0/CODE_OF_CONDUCT.md` & `dyff_schema-0.9.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.8.0/LICENSE` & `dyff_schema-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.8.0/PKG-INFO` & `dyff_schema-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyff-schema
-Version: 0.8.0
+Version: 0.9.0
 Summary: Data models for the Dyff AI auditing platform.
 Author-email: Digital Safety Research Institute <contact@dsri.org>
 License: Apache-2.0
 Project-URL: Home, https://gitlab.com/dyff/packages/dyff-schema
 Project-URL: Issues, https://gitlab.com/dyff/packages/dyff-schema/-/issues
 Keywords: ai,audit,safety,evaluation
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dyff_schema-0.8.0/README.md` & `dyff_schema-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.8.0/dyff/schema/__init__.py` & `dyff_schema-0.9.0/dyff/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.8.0/dyff/schema/copydoc.py` & `dyff_schema-0.9.0/dyff/schema/copydoc.py`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.8.0/dyff/schema/ids.py` & `dyff_schema-0.9.0/dyff/schema/ids.py`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.8.0/dyff/schema/quantity.py` & `dyff_schema-0.9.0/dyff/schema/quantity.py`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.8.0/dyff/schema/v0/r1/adapters.py` & `dyff_schema-0.9.0/dyff/schema/v0/r1/adapters.py`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.8.0/dyff/schema/v0/r1/base.py` & `dyff_schema-0.9.0/dyff/schema/v0/r1/base.py`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.8.0/dyff/schema/v0/r1/dataset/__init__.py` & `dyff_schema-0.9.0/dyff/schema/v0/r1/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.8.0/dyff/schema/v0/r1/dataset/arrow.py` & `dyff_schema-0.9.0/dyff/schema/v0/r1/dataset/arrow.py`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.8.0/dyff/schema/v0/r1/dataset/binary.py` & `dyff_schema-0.9.0/dyff/schema/v0/r1/dataset/binary.py`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.8.0/dyff/schema/v0/r1/dataset/text.py` & `dyff_schema-0.9.0/dyff/schema/v0/r1/dataset/text.py`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.8.0/dyff/schema/v0/r1/io/vllm.py` & `dyff_schema-0.9.0/dyff/schema/v0/r1/io/vllm.py`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.8.0/dyff/schema/v0/r1/platform.py` & `dyff_schema-0.9.0/dyff/schema/v0/r1/platform.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
 def _dns_domain_regex():
     """One or more DNS labels separated by dots (``.``).
 
     Note that its maximum length is 253 characters, but we can't enforce this in the
     regex.
     """
-    return f"{_dns_label_regex()}(\.{_dns_label_regex()})*"
+    return rf"{_dns_label_regex()}(\.{_dns_label_regex()})*"
 
 
 def _k8s_domain_maxlen():
     """Max length of a k8s domain.
 
     The DNS domain standard specifies 255 characters, but this includes the trailing dot
     and null terminator. We never include a trailing dot in k8s-style domains.
@@ -92,15 +92,15 @@
     DNS subdomain followed by a ``/`` character.
 
     Examples:
 
         * my-multi_segment.key
         * dyff.io/reserved-key
     """
-    return f"^({_dns_domain_regex()}/)?{_dns_label_regex()}$"
+    return rf"^({_dns_domain_regex()}/)?{_dns_label_regex()}$"
 
 
 def _k8s_label_key_maxlen():
     """Max length of a label key.
 
     The prefix segment, if present, has a max length of 253 characters. The
     name segment has a max length of 63 characters.
@@ -122,15 +122,15 @@
 
         * must have 63 characters or fewer (can be empty)
         * unless empty, must begin and end with an alphanumeric character (``[a-z0-9A-Z]``)
         * could contain dashes (``-``), underscores (``_``), dots (``.``), and alphanumerics between
 
     See: https://kubernetes.io/docs/concepts/overview/working-with-objects/labels/
     """
-    return f"^({_k8s_label_regex()})?$"
+    return rf"^({_k8s_label_regex()})?$"
 
 
 def _k8s_label_value_maxlen():
     """Max length of a label value.
 
     Label values must have 63 characters or fewer (can be empty).
```

### Comparing `dyff_schema-0.8.0/dyff/schema/v0/r1/requests.py` & `dyff_schema-0.9.0/dyff/schema/v0/r1/requests.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,17 +8,18 @@
 is created. Similarly, if a resource depends on an instance of another
 resource, the request will refer to the dependency by its ID, while the core
 resource will include the full dependency object as a sub-resource. The
 ``create`` endpoints take a request as input and return a full core resource
 in response.
 """
 
+from __future__ import annotations
 
 from datetime import datetime
-from typing import Any, Optional, Union
+from typing import Optional, Union
 
 import pydantic
 
 from .base import DyffDefaultSerializers
 from .platform import (
     AnalysisBase,
     DatasetBase,
@@ -168,37 +169,39 @@
 
 # Note: Query requests, as they currently exist, don't work with Versioned
 # because fastapi will assign None to every field that the client doesn't
 # specify. I think it's not that important, because all of the query parameters
 # will always be optional. There could be a problem if the semantics of a
 # name change, but let's just not do that!
 class DyffEntityQueryRequest(DyffRequestDefaultValidators):
+    query: Optional[str] = pydantic.Field(
+        default=None,
+        description="A JSON structure describing a query, encoded as a string."
+        " Valid keys are the same as the valid query keys for the corresponding"
+        " endpoint. Values can be scalars or lists. Lists are treated as"
+        " disjunctive queries (i.e., 'value $in list').",
+    )
+
     id: Optional[str] = pydantic.Field(default=None)
     account: Optional[str] = pydantic.Field(default=None)
     status: Optional[str] = pydantic.Field(default=None)
     reason: Optional[str] = pydantic.Field(default=None)
     labels: Optional[str] = pydantic.Field(
         default=None, description="Labels dict represented as a JSON string."
     )
 
-    def dict(self, exclude_unset=True, **kwargs) -> dict[str, Any]:
-        return super().dict(exclude_unset=exclude_unset, **kwargs)
-
-    def json(self, exclude_unset=True, **kwargs) -> Any:
-        return super().json(exclude_unset=exclude_unset, **kwargs)
-
 
 class _AnalysisProductQueryRequest(DyffEntityQueryRequest):
     method: Optional[str] = pydantic.Field(default=None)
     methodName: Optional[str] = pydantic.Field(default=None)
     dataset: Optional[str] = pydantic.Field(default=None)
     evaluation: Optional[str] = pydantic.Field(default=None)
     inferenceService: Optional[str] = pydantic.Field(default=None)
     model: Optional[str] = pydantic.Field(default=None)
-    inputsAnyOf: Optional[str] = pydantic.Field(default=None)
+    inputs: Optional[str] = pydantic.Field(default=None)
 
 
 class AuditQueryRequest(DyffEntityQueryRequest):
     name: Optional[str] = pydantic.Field(default=None)
 
 
 class DatasetQueryRequest(DyffEntityQueryRequest):
```

### Comparing `dyff_schema-0.8.0/dyff/schema/v0/r1/test.py` & `dyff_schema-0.9.0/dyff/schema/v0/r1/test.py`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.8.0/dyff_schema.egg-info/PKG-INFO` & `dyff_schema-0.9.0/dyff_schema.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyff-schema
-Version: 0.8.0
+Version: 0.9.0
 Summary: Data models for the Dyff AI auditing platform.
 Author-email: Digital Safety Research Institute <contact@dsri.org>
 License: Apache-2.0
 Project-URL: Home, https://gitlab.com/dyff/packages/dyff-schema
 Project-URL: Issues, https://gitlab.com/dyff/packages/dyff-schema/-/issues
 Keywords: ai,audit,safety,evaluation
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dyff_schema-0.8.0/dyff_schema.egg-info/SOURCES.txt` & `dyff_schema-0.9.0/dyff_schema.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 README.md
 makefile
 pyproject.toml
 dyff/schema/__init__.py
 dyff/schema/adapters.py
 dyff/schema/base.py
 dyff/schema/copydoc.py
+dyff/schema/errors.py
 dyff/schema/ids.py
 dyff/schema/platform.py
 dyff/schema/py.typed
 dyff/schema/quantity.py
 dyff/schema/requests.py
 dyff/schema/test.py
 dyff/schema/version.py
```

### Comparing `dyff_schema-0.8.0/pyproject.toml` & `dyff_schema-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.8.0/tests/test_import.py` & `dyff_schema-0.9.0/tests/test_import.py`

 * *Files identical despite different names*

