# Comparing `tmp/dyff_schema-0.7.2.tar.gz` & `tmp/dyff_schema-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dyff_schema-0.7.2.tar", last modified: Wed May 22 02:11:56 2024, max compression
+gzip compressed data, was "dyff_schema-0.8.0.tar", last modified: Thu May 23 22:39:38 2024, max compression
```

## Comparing `dyff_schema-0.7.2.tar` & `dyff_schema-0.8.0.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:11:56.765609 dyff_schema-0.7.2/
--rw-rw-rw-   0 root         (0) root         (0)      434 2024-05-22 02:11:50.000000 dyff_schema-0.7.2/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1399 2024-05-22 02:11:50.000000 dyff_schema-0.7.2/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      489 2024-05-22 02:11:50.000000 dyff_schema-0.7.2/.licenserc.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1686 2024-05-22 02:11:50.000000 dyff_schema-0.7.2/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      108 2024-05-22 02:11:50.000000 dyff_schema-0.7.2/.prettierignore
--rw-rw-rw-   0 root         (0) root         (0)     2192 2024-05-22 02:11:50.000000 dyff_schema-0.7.2/.secrets.baseline
--rw-rw-rw-   0 root         (0) root         (0)     5503 2024-05-22 02:11:50.000000 dyff_schema-0.7.2/CODE_OF_CONDUCT.md
--rw-rw-rw-   0 root         (0) root         (0)    11357 2024-05-22 02:11:50.000000 dyff_schema-0.7.2/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       43 2024-05-22 02:11:50.000000 dyff_schema-0.7.2/NOTICE
--rw-r--r--   0 root         (0) root         (0)     3458 2024-05-22 02:11:56.764609 dyff_schema-0.7.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2312 2024-05-22 02:11:50.000000 dyff_schema-0.7.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:11:56.749609 dyff_schema-0.7.2/dyff/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:11:56.756609 dyff_schema-0.7.2/dyff/schema/
--rw-rw-rw-   0 root         (0) root         (0)     1031 2024-05-22 02:11:50.000000 dyff_schema-0.7.2/dyff/schema/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      123 2024-05-22 02:11:50.000000 dyff_schema-0.7.2/dyff/schema/adapters.py
--rw-rw-rw-   0 root         (0) root         (0)      119 2024-05-22 02:11:50.000000 dyff_schema-0.7.2/dyff/schema/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1075 2024-05-22 02:11:50.000000 dyff_schema-0.7.2/dyff/schema/copydoc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:11:56.757609 dyff_schema-0.7.2/dyff/schema/dataset/
--rw-rw-rw-   0 root         (0) root         (0)      123 2024-05-22 02:11:50.000000 dyff_schema-0.7.2/dyff/schema/dataset/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      129 2024-05-22 02:11:50.000000 dyff_schema-0.7.2/dyff/schema/dataset/arrow.py
--rw-rw-rw-   0 root         (0) root         (0)      130 2024-05-22 02:11:50.000000 dyff_schema-0.7.2/dyff/schema/dataset/binary.py
--rw-rw-rw-   0 root         (0) root         (0)      138 2024-05-22 02:11:50.000000 dyff_schema-0.7.2/dyff/schema/dataset/classification.py
--rw-rw-rw-   0 root         (0) root         (0)      128 2024-05-22 02:11:50.000000 dyff_schema-0.7.2/dyff/schema/dataset/text.py
--rw-rw-rw-   0 root         (0) root         (0)      130 2024-05-22 02:11:50.000000 dyff_schema-0.7.2/dyff/schema/dataset/vision.py
--rw-rw-rw-   0 root         (0) root         (0)     1422 2024-05-22 02:11:50.000000 dyff_schema-0.7.2/dyff/schema/ids.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:11:56.758609 dyff_schema-0.7.2/dyff/schema/io/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-22 02:11:50.000000 dyff_schema-0.7.2/dyff/schema/io/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      123 2024-05-22 02:11:50.000000 dyff_schema-0.7.2/dyff/schema/io/vllm.py
--rw-rw-rw-   0 root         (0) root         (0)      123 2024-05-22 02:11:50.000000 dyff_schema-0.7.2/dyff/schema/platform.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 02:11:50.000000 dyff_schema-0.7.2/dyff/schema/py.typed
--rw-rw-rw-   0 root         (0) root         (0)     3788 2024-05-22 02:11:50.000000 dyff_schema-0.7.2/dyff/schema/quantity.py
--rw-rw-rw-   0 root         (0) root         (0)      123 2024-05-22 02:11:50.000000 dyff_schema-0.7.2/dyff/schema/requests.py
--rw-rw-rw-   0 root         (0) root         (0)      119 2024-05-22 02:11:50.000000 dyff_schema-0.7.2/dyff/schema/test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:11:56.758609 dyff_schema-0.7.2/dyff/schema/v0/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-22 02:11:50.000000 dyff_schema-0.7.2/dyff/schema/v0/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:11:56.760609 dyff_schema-0.7.2/dyff/schema/v0/r1/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-22 02:11:50.000000 dyff_schema-0.7.2/dyff/schema/v0/r1/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    23552 2024-05-22 02:11:50.000000 dyff_schema-0.7.2/dyff/schema/v0/r1/adapters.py
--rw-rw-rw-   0 root         (0) root         (0)    17471 2024-05-22 02:11:50.000000 dyff_schema-0.7.2/dyff/schema/v0/r1/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:11:56.762609 dyff_schema-0.7.2/dyff/schema/v0/r1/dataset/
--rw-rw-rw-   0 root         (0) root         (0)     2553 2024-05-22 02:11:50.000000 dyff_schema-0.7.2/dyff/schema/v0/r1/dataset/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12312 2024-05-22 02:11:50.000000 dyff_schema-0.7.2/dyff/schema/v0/r1/dataset/arrow.py
--rw-rw-rw-   0 root         (0) root         (0)      544 2024-05-22 02:11:50.000000 dyff_schema-0.7.2/dyff/schema/v0/r1/dataset/binary.py
--rw-rw-rw-   0 root         (0) root         (0)      311 2024-05-22 02:11:50.000000 dyff_schema-0.7.2/dyff/schema/v0/r1/dataset/classification.py
--rw-rw-rw-   0 root         (0) root         (0)     1008 2024-05-22 02:11:50.000000 dyff_schema-0.7.2/dyff/schema/v0/r1/dataset/text.py
--rw-rw-rw-   0 root         (0) root         (0)      369 2024-05-22 02:11:50.000000 dyff_schema-0.7.2/dyff/schema/v0/r1/dataset/vision.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:11:56.762609 dyff_schema-0.7.2/dyff/schema/v0/r1/io/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-22 02:11:50.000000 dyff_schema-0.7.2/dyff/schema/v0/r1/io/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5320 2024-05-22 02:11:50.000000 dyff_schema-0.7.2/dyff/schema/v0/r1/io/vllm.py
--rw-rw-rw-   0 root         (0) root         (0)    61574 2024-05-22 02:11:50.000000 dyff_schema-0.7.2/dyff/schema/v0/r1/platform.py
--rw-rw-rw-   0 root         (0) root         (0)     8913 2024-05-22 02:11:50.000000 dyff_schema-0.7.2/dyff/schema/v0/r1/requests.py
--rw-rw-rw-   0 root         (0) root         (0)    10720 2024-05-22 02:11:50.000000 dyff_schema-0.7.2/dyff/schema/v0/r1/test.py
--rw-rw-rw-   0 root         (0) root         (0)      392 2024-05-22 02:11:50.000000 dyff_schema-0.7.2/dyff/schema/v0/r1/version.py
--rw-rw-rw-   0 root         (0) root         (0)      372 2024-05-22 02:11:50.000000 dyff_schema-0.7.2/dyff/schema/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:11:56.764609 dyff_schema-0.7.2/dyff_schema.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3458 2024-05-22 02:11:56.000000 dyff_schema-0.7.2/dyff_schema.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1358 2024-05-22 02:11:56.000000 dyff_schema-0.7.2/dyff_schema.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-22 02:11:56.000000 dyff_schema-0.7.2/dyff_schema.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       64 2024-05-22 02:11:56.000000 dyff_schema-0.7.2/dyff_schema.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-05-22 02:11:56.000000 dyff_schema-0.7.2/dyff_schema.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      502 2024-05-22 02:11:50.000000 dyff_schema-0.7.2/makefile
--rw-rw-rw-   0 root         (0) root         (0)     1585 2024-05-22 02:11:50.000000 dyff_schema-0.7.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-22 02:11:56.765609 dyff_schema-0.7.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:11:56.763609 dyff_schema-0.7.2/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1449 2024-05-22 02:11:50.000000 dyff_schema-0.7.2/tests/test_import.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 22:39:38.539608 dyff_schema-0.8.0/
+-rw-rw-rw-   0 root         (0) root         (0)      434 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1399 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      489 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/.licenserc.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1686 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      108 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/.prettierignore
+-rw-rw-rw-   0 root         (0) root         (0)     2192 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/.secrets.baseline
+-rw-rw-rw-   0 root         (0) root         (0)     5503 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/CODE_OF_CONDUCT.md
+-rw-rw-rw-   0 root         (0) root         (0)    11357 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       43 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     3458 2024-05-23 22:39:38.539608 dyff_schema-0.8.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2312 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 22:39:38.524608 dyff_schema-0.8.0/dyff/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 22:39:38.531608 dyff_schema-0.8.0/dyff/schema/
+-rw-rw-rw-   0 root         (0) root         (0)     1031 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/dyff/schema/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      123 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/dyff/schema/adapters.py
+-rw-rw-rw-   0 root         (0) root         (0)      119 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/dyff/schema/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1075 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/dyff/schema/copydoc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 22:39:38.532608 dyff_schema-0.8.0/dyff/schema/dataset/
+-rw-rw-rw-   0 root         (0) root         (0)      123 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/dyff/schema/dataset/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      129 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/dyff/schema/dataset/arrow.py
+-rw-rw-rw-   0 root         (0) root         (0)      130 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/dyff/schema/dataset/binary.py
+-rw-rw-rw-   0 root         (0) root         (0)      138 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/dyff/schema/dataset/classification.py
+-rw-rw-rw-   0 root         (0) root         (0)      128 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/dyff/schema/dataset/text.py
+-rw-rw-rw-   0 root         (0) root         (0)      130 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/dyff/schema/dataset/vision.py
+-rw-rw-rw-   0 root         (0) root         (0)     1422 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/dyff/schema/ids.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 22:39:38.532608 dyff_schema-0.8.0/dyff/schema/io/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/dyff/schema/io/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      123 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/dyff/schema/io/vllm.py
+-rw-rw-rw-   0 root         (0) root         (0)      123 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/dyff/schema/platform.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/dyff/schema/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)     3788 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/dyff/schema/quantity.py
+-rw-rw-rw-   0 root         (0) root         (0)      123 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/dyff/schema/requests.py
+-rw-rw-rw-   0 root         (0) root         (0)      119 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/dyff/schema/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 22:39:38.533608 dyff_schema-0.8.0/dyff/schema/v0/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/dyff/schema/v0/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 22:39:38.534608 dyff_schema-0.8.0/dyff/schema/v0/r1/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/dyff/schema/v0/r1/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    23552 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/dyff/schema/v0/r1/adapters.py
+-rw-rw-rw-   0 root         (0) root         (0)    19385 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/dyff/schema/v0/r1/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 22:39:38.536608 dyff_schema-0.8.0/dyff/schema/v0/r1/dataset/
+-rw-rw-rw-   0 root         (0) root         (0)     2553 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/dyff/schema/v0/r1/dataset/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12312 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/dyff/schema/v0/r1/dataset/arrow.py
+-rw-rw-rw-   0 root         (0) root         (0)      544 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/dyff/schema/v0/r1/dataset/binary.py
+-rw-rw-rw-   0 root         (0) root         (0)      311 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/dyff/schema/v0/r1/dataset/classification.py
+-rw-rw-rw-   0 root         (0) root         (0)     1008 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/dyff/schema/v0/r1/dataset/text.py
+-rw-rw-rw-   0 root         (0) root         (0)      369 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/dyff/schema/v0/r1/dataset/vision.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 22:39:38.536608 dyff_schema-0.8.0/dyff/schema/v0/r1/io/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/dyff/schema/v0/r1/io/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5320 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/dyff/schema/v0/r1/io/vllm.py
+-rw-rw-rw-   0 root         (0) root         (0)    61413 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/dyff/schema/v0/r1/platform.py
+-rw-rw-rw-   0 root         (0) root         (0)     9728 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/dyff/schema/v0/r1/requests.py
+-rw-rw-rw-   0 root         (0) root         (0)    10720 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/dyff/schema/v0/r1/test.py
+-rw-rw-rw-   0 root         (0) root         (0)      392 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/dyff/schema/v0/r1/version.py
+-rw-rw-rw-   0 root         (0) root         (0)      372 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/dyff/schema/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 22:39:38.538608 dyff_schema-0.8.0/dyff_schema.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3458 2024-05-23 22:39:38.000000 dyff_schema-0.8.0/dyff_schema.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1358 2024-05-23 22:39:38.000000 dyff_schema-0.8.0/dyff_schema.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 22:39:38.000000 dyff_schema-0.8.0/dyff_schema.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       64 2024-05-23 22:39:38.000000 dyff_schema-0.8.0/dyff_schema.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-05-23 22:39:38.000000 dyff_schema-0.8.0/dyff_schema.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      502 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/makefile
+-rw-rw-rw-   0 root         (0) root         (0)     1585 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-23 22:39:38.539608 dyff_schema-0.8.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 22:39:38.538608 dyff_schema-0.8.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1449 2024-05-23 22:39:32.000000 dyff_schema-0.8.0/tests/test_import.py
```

### Comparing `dyff_schema-0.7.2/.gitlab-ci.yml` & `dyff_schema-0.8.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.7.2/.pre-commit-config.yaml` & `dyff_schema-0.8.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.7.2/.secrets.baseline` & `dyff_schema-0.8.0/.secrets.baseline`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.7.2/CODE_OF_CONDUCT.md` & `dyff_schema-0.8.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.7.2/LICENSE` & `dyff_schema-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.7.2/PKG-INFO` & `dyff_schema-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyff-schema
-Version: 0.7.2
+Version: 0.8.0
 Summary: Data models for the Dyff AI auditing platform.
 Author-email: Digital Safety Research Institute <contact@dsri.org>
 License: Apache-2.0
 Project-URL: Home, https://gitlab.com/dyff/packages/dyff-schema
 Project-URL: Issues, https://gitlab.com/dyff/packages/dyff-schema/-/issues
 Keywords: ai,audit,safety,evaluation
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dyff_schema-0.7.2/README.md` & `dyff_schema-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.7.2/dyff/schema/__init__.py` & `dyff_schema-0.8.0/dyff/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.7.2/dyff/schema/copydoc.py` & `dyff_schema-0.8.0/dyff/schema/copydoc.py`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.7.2/dyff/schema/ids.py` & `dyff_schema-0.8.0/dyff/schema/ids.py`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.7.2/dyff/schema/quantity.py` & `dyff_schema-0.8.0/dyff/schema/quantity.py`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.7.2/dyff/schema/v0/r1/adapters.py` & `dyff_schema-0.8.0/dyff/schema/v0/r1/adapters.py`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.7.2/dyff/schema/v0/r1/base.py` & `dyff_schema-0.8.0/dyff/schema/v0/r1/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # SPDX-FileCopyrightText: 2024 UL Research Institutes
 # SPDX-License-Identifier: Apache-2.0
 
-from datetime import datetime
-from typing import Any, Generic, NamedTuple, Optional, Type, TypeVar
+from __future__ import annotations
+
+import json
+from datetime import datetime, timezone
+from typing import Any, Generic, Literal, NamedTuple, Optional, Type, TypeVar
 
 import pydantic
 
 # ----------------------------------------------------------------------------
 # Fixed-width numeric type value bounds
 
 
@@ -551,41 +554,87 @@
         return pydantic.conlist(item_type)
     else:
         if list_size <= 0:
             raise ValueError(f"list_size {list_size} must be > 0")
         return pydantic.conlist(item_type, min_items=list_size, max_items=list_size)
 
 
-class DyffSchemaBaseModel(pydantic.BaseModel):
-    """Base class for pydantic models that used for defining data schemas.
+# mypy gets confused because 'dict' is the name of a method in DyffDefaultSerializers
+_ModelAsDict = dict[str, Any]
+
+
+class DyffDefaultSerializers(pydantic.BaseModel):
+    """This must be the base class for *all pydantic models* in the Dyff schema.
 
     Overrides serialization functions to serialize by alias, so that "round-trip"
     serialization is the default for fields with aliases. We prefer aliases because we
     can 1) use _underscore_names_ as reserved names in our data schema, and 2) allow
     Python reserved words like 'bytes' as field names.
     """
 
+    def dict(self, *, by_alias: bool = True, **kwargs) -> _ModelAsDict:
+        return super().dict(by_alias=by_alias, **kwargs)
+
+    def json(self, *, by_alias: bool = True, **kwargs) -> str:
+        return super().json(by_alias=by_alias, **kwargs)
+
+    def model_dump(
+        self,
+        *,
+        mode: Literal["python", "json"] = "python",
+        by_alias: bool = True,
+        **kwargs,
+    ) -> _ModelAsDict:
+        """Encode the object as a dict containing only JSON datatypes.
+
+        .. deprecated::
+
+            FIXME: This emulates a Pydantic 2 feature, but the mode="json"
+            option can only be implemented in an inefficient way. Remove when
+            we convert to Pydantic 2. See: DYFF-223
+        """
+        if mode == "python":
+            return self.dict(by_alias=by_alias, **kwargs)
+        else:
+            return json.loads(self.json(by_alias=by_alias, **kwargs))
+
+
+# Note: I *really* wanted to require datetimes to have timezones, like in
+# DyffRequestDefaultValidators, but some existing objects in the Auth database
+# don't have timezones set currently for historical reasons. It's actually
+# better if all datetimes in the system are UTC, so that their JSON
+# representations (i.e., isoformat strings) are well-ordered.
+class DyffSchemaBaseModel(DyffDefaultSerializers):
+    """This should be the base class for *almost all* non-request models in the Dyff
+    schema. Models that do not inherit from this class *must* still inherit from
+    DyffDefaultSerializers.
+
+    Adds a root validator to ensure that all datetime fields are represented in the UTC
+    timezone. This is necessary to avoid errors when comparing "naive" and "aware"
+    datetimes. Using the UTC timezone everywhere ensures that JSON representations of
+    datetimes are well-ordered.
+    """
+
     @pydantic.root_validator
-    def _require_datetime_timezone_aware(cls, values):
+    def _ensure_datetime_timezone_utc(cls, values):
+        update = {}
         for k, v in values.items():
             if isinstance(v, datetime):
                 if v.tzinfo is None:
-                    raise ValueError(f"{cls.__qualname__}.{k}: timezone not set")
+                    update[k] = v.replace(tzinfo=timezone.utc)
+                elif v.tzinfo != timezone.utc:
+                    update[k] = v.astimezone(timezone.utc)
+        values.update(update)
         return values
 
-    def dict(self, *, by_alias: bool = True, **kwargs) -> dict[str, Any]:
-        return super().dict(by_alias=by_alias, **kwargs)
-
-    def json(self, *, by_alias: bool = True, **kwargs) -> str:
-        return super().json(by_alias=by_alias, **kwargs)
-
 
 __all__ = [
     "DTYPE",
     "DType",
+    "DyffDefaultSerializers",
     "DyffSchemaBaseModel",
     "FixedWidthFloat",
     "FixedWidthInt",
     "Float32",
     "Float64",
     "Int8",
     "Int16",
```

### Comparing `dyff_schema-0.7.2/dyff/schema/v0/r1/dataset/__init__.py` & `dyff_schema-0.8.0/dyff/schema/v0/r1/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.7.2/dyff/schema/v0/r1/dataset/arrow.py` & `dyff_schema-0.8.0/dyff/schema/v0/r1/dataset/arrow.py`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.7.2/dyff/schema/v0/r1/dataset/binary.py` & `dyff_schema-0.8.0/dyff/schema/v0/r1/dataset/binary.py`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.7.2/dyff/schema/v0/r1/dataset/text.py` & `dyff_schema-0.8.0/dyff/schema/v0/r1/dataset/text.py`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.7.2/dyff/schema/v0/r1/io/vllm.py` & `dyff_schema-0.8.0/dyff/schema/v0/r1/io/vllm.py`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.7.2/dyff/schema/v0/r1/platform.py` & `dyff_schema-0.8.0/dyff/schema/v0/r1/platform.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
       description of a resource inside of an outer resource that depends on it.
       We include the full dependency data structure so that downstream
       components don't need to be able to look it up by ID.
 """
 # mypy: disable-error-code="import-untyped"
 import abc
 import enum
-from datetime import datetime, timezone
+from datetime import datetime
 from enum import Enum
 from typing import Any, Literal, NamedTuple, Optional, Type, Union
 
 import pyarrow
 import pydantic
 from typing_extensions import TypeAlias
 
@@ -528,18 +528,15 @@
     )
     entities: list[str] = pydantic.Field(
         default_factory=list,
         description="The access grant applies to all resources with IDs listed in 'entities'",
     )
 
 
-# FIXME: We can't derive from DyffSchemaBaseModel right now because existing
-# APIKeys don't have a timezone set for their datetime members.
-# See: DYFF-406
-class APIKey(pydantic.BaseModel):
+class APIKey(DyffSchemaBaseModel):
     """A description of a set of permissions granted to a single subject (either an
     account or a workload).
 
     Dyff API clients authenticate with a *token* that contains a cryptographically
     signed APIKey.
     """
 
@@ -560,29 +557,34 @@
         default=None,
         description="For account keys: a secret value to check when verifying the APIKey",
     )
     grants: list[AccessGrant] = pydantic.Field(
         default_factory=list, description="AccessGrants associated with the APIKey"
     )
 
-    @pydantic.root_validator
-    def _ensure_datetime_timezone_aware(cls, values):
-        update = {}
-        for k, v in values.items():
-            if isinstance(v, datetime):
-                if v.tzinfo is None:
-                    update[k] = v.replace(tzinfo=timezone.utc)
-        values.update(update)
-        return values
 
-    def dict(self, *, by_alias: bool = True, **kwargs) -> dict[str, Any]:
-        return super().dict(by_alias=by_alias, **kwargs)
+class Identity(DyffSchemaBaseModel):
+    """The identity of an Account according to one or more external identity
+    providers."""
 
-    def json(self, *, by_alias: bool = True, **kwargs) -> str:
-        return super().json(by_alias=by_alias, **kwargs)
+    google: Optional[str] = pydantic.Field(default=None)
+
+
+class Account(DyffSchemaBaseModel):
+    """An Account in the system.
+
+    All entities are owned by an Account.
+    """
+
+    name: str
+    identity: Identity = pydantic.Field(default_factory=Identity)
+    apiKeys: list[APIKey] = pydantic.Field(default_factory=list)
+    # --- Added by system
+    id: Optional[str] = None
+    creationTime: Optional[datetime] = None
 
 
 # ----------------------------------------------------------------------------
 
 
 class Digest(DyffSchemaBaseModel):
     md5: Optional[str] = pydantic.Field(
@@ -1856,14 +1858,15 @@
 ]
 
 
 __all__ = [
     "Accelerator",
     "AcceleratorGPU",
     "AccessGrant",
+    "Account",
     "Analysis",
     "AnalysisArgument",
     "AnalysisBase",
     "AnalysisInput",
     "AnalysisOutputQueryFields",
     "AnalysisScope",
     "Annotation",
@@ -1896,14 +1899,15 @@
     "Family",
     "FamilyMember",
     "FamilyMemberKind",
     "ForeignInferenceService",
     "ForeignMethod",
     "ForeignModel",
     "Frameworks",
+    "Identity",
     "InferenceInterface",
     "InferenceService",
     "InferenceServiceBase",
     "InferenceServiceBuilder",
     "InferenceServiceRunner",
     "InferenceServiceRunnerKind",
     "InferenceServiceSources",
```

### Comparing `dyff_schema-0.7.2/dyff/schema/v0/r1/requests.py` & `dyff_schema-0.8.0/dyff/schema/v0/r1/requests.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 
 from datetime import datetime
 from typing import Any, Optional, Union
 
 import pydantic
 
-from .base import DyffSchemaBaseModel
+from .base import DyffDefaultSerializers
 from .platform import (
     AnalysisBase,
     DatasetBase,
     DataView,
     DocumentationBase,
     EvaluationBase,
     InferenceServiceBase,
@@ -33,44 +33,65 @@
     ModuleBase,
     ReportBase,
     TagBase,
 )
 from .version import SchemaVersion
 
 
-class DyffEntityCreateRequest(SchemaVersion, DyffSchemaBaseModel):
+class DyffRequestDefaultValidators(DyffDefaultSerializers):
+    """This must be the base class for *all* request models in the Dyff schema.
+
+    Adds a root validator to ensure that all user-provided datetime fields have a
+    timezone set. Timezones will be converted to UTC once the data enters the platform,
+    but we allow requests to have non-UTC timezones for user convenience.
+    """
+
+    @pydantic.root_validator
+    def _require_datetime_timezone_aware(cls, values):
+        for k, v in values.items():
+            if isinstance(v, datetime):
+                if v.tzinfo is None:
+                    raise ValueError(f"{cls.__qualname__}.{k}: timezone not set")
+        return values
+
+
+class DyffRequestBase(SchemaVersion, DyffRequestDefaultValidators):
+    pass
+
+
+class DyffEntityCreateRequest(DyffRequestBase):
     account: str = pydantic.Field(description="Account that owns the entity")
 
 
 class AnalysisCreateRequest(DyffEntityCreateRequest, AnalysisBase):
     """An Analysis transforms Datasets, Evaluations, and Measurements into new
     Measurements or SafetyCases."""
 
     method: str = pydantic.Field(description="Method ID")
 
 
 class DatasetCreateRequest(DyffEntityCreateRequest, DatasetBase):
     pass
 
 
-class DocumentationEditRequest(SchemaVersion, DocumentationBase):
+class DocumentationEditRequest(DyffRequestBase, DocumentationBase):
     pass
 
 
 class InferenceServiceCreateRequest(DyffEntityCreateRequest, InferenceServiceBase):
     model: Optional[str] = pydantic.Field(
         default=None, description="ID of Model backing the service, if applicable"
     )
 
 
 class InferenceSessionCreateRequest(DyffEntityCreateRequest, InferenceSessionBase):
     inferenceService: str = pydantic.Field(description="InferenceService ID")
 
 
-class InferenceSessionTokenCreateRequest(SchemaVersion, DyffSchemaBaseModel):
+class InferenceSessionTokenCreateRequest(DyffRequestBase):
     expires: Optional[datetime] = pydantic.Field(
         default=None,
         description="Expiration time of the token. Must be <= expiration time"
         " of session. Default: expiration time of session.",
     )
 
 
@@ -133,28 +154,28 @@
 
     evaluationView: Optional[Union[str, DataView]] = pydantic.Field(
         default=None,
         description="View of the evaluation output data required by the report.",
     )
 
 
-class TagCreateRequest(SchemaVersion, TagBase):
+class TagCreateRequest(DyffRequestBase, TagBase):
     pass
 
 
-class LabelUpdateRequest(SchemaVersion, Labeled):
+class LabelUpdateRequest(DyffRequestBase, Labeled):
     pass
 
 
 # Note: Query requests, as they currently exist, don't work with Versioned
 # because fastapi will assign None to every field that the client doesn't
 # specify. I think it's not that important, because all of the query parameters
 # will always be optional. There could be a problem if the semantics of a
 # name change, but let's just not do that!
-class DyffEntityQueryRequest(DyffSchemaBaseModel):
+class DyffEntityQueryRequest(DyffRequestDefaultValidators):
     id: Optional[str] = pydantic.Field(default=None)
     account: Optional[str] = pydantic.Field(default=None)
     status: Optional[str] = pydantic.Field(default=None)
     reason: Optional[str] = pydantic.Field(default=None)
     labels: Optional[str] = pydantic.Field(
         default=None, description="Labels dict represented as a JSON string."
     )
@@ -236,14 +257,16 @@
 
 
 __all__ = [
     "AnalysisCreateRequest",
     "AuditQueryRequest",
     "DyffEntityCreateRequest",
     "DyffEntityQueryRequest",
+    "DyffRequestBase",
+    "DyffRequestDefaultValidators",
     "DatasetCreateRequest",
     "DatasetQueryRequest",
     "DocumentationEditRequest",
     "EvaluationCreateRequest",
     "EvaluationQueryRequest",
     "EvaluationInferenceSessionRequest",
     "InferenceServiceCreateRequest",
```

### Comparing `dyff_schema-0.7.2/dyff/schema/v0/r1/test.py` & `dyff_schema-0.8.0/dyff/schema/v0/r1/test.py`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.7.2/dyff_schema.egg-info/PKG-INFO` & `dyff_schema-0.8.0/dyff_schema.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyff-schema
-Version: 0.7.2
+Version: 0.8.0
 Summary: Data models for the Dyff AI auditing platform.
 Author-email: Digital Safety Research Institute <contact@dsri.org>
 License: Apache-2.0
 Project-URL: Home, https://gitlab.com/dyff/packages/dyff-schema
 Project-URL: Issues, https://gitlab.com/dyff/packages/dyff-schema/-/issues
 Keywords: ai,audit,safety,evaluation
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dyff_schema-0.7.2/dyff_schema.egg-info/SOURCES.txt` & `dyff_schema-0.8.0/dyff_schema.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.7.2/pyproject.toml` & `dyff_schema-0.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.7.2/tests/test_import.py` & `dyff_schema-0.8.0/tests/test_import.py`

 * *Files identical despite different names*

