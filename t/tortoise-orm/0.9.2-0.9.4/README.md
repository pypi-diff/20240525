# Comparing `tmp/tortoise-orm-0.9.2.tar.gz` & `tmp/tortoise-orm-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tortoise-orm-0.9.2.tar", last modified: Fri Jul  6 14:03:29 2018, max compression
+gzip compressed data, was "dist/tortoise-orm-0.9.4.tar", last modified: Tue Jul 17 08:16:22 2018, max compression
```

## Comparing `tortoise-orm-0.9.2.tar` & `tortoise-orm-0.9.4.tar`

### file list

```diff
@@ -1,112 +1,186 @@
-drwxr-xr-x   0 andreybondar   (501) staff       (20)        0 2018-07-06 14:03:29.000000 tortoise-orm-0.9.2/
--rw-r--r--   0 andreybondar   (501) staff       (20)     6002 2018-07-06 14:03:29.000000 tortoise-orm-0.9.2/PKG-INFO
-drwxr-xr-x   0 andreybondar   (501) staff       (20)        0 2018-07-06 14:03:29.000000 tortoise-orm-0.9.2/tortoise_orm.egg-info/
--rw-r--r--   0 andreybondar   (501) staff       (20)     6002 2018-07-06 14:03:29.000000 tortoise-orm-0.9.2/tortoise_orm.egg-info/PKG-INFO
--rw-r--r--   0 andreybondar   (501) staff       (20)     3630 2018-07-06 14:03:29.000000 tortoise-orm-0.9.2/tortoise_orm.egg-info/SOURCES.txt
--rw-r--r--   0 andreybondar   (501) staff       (20)       34 2018-07-06 14:03:29.000000 tortoise-orm-0.9.2/tortoise_orm.egg-info/requires.txt
--rw-r--r--   0 andreybondar   (501) staff       (20)        9 2018-07-06 14:03:29.000000 tortoise-orm-0.9.2/tortoise_orm.egg-info/top_level.txt
--rw-r--r--   0 andreybondar   (501) staff       (20)        1 2018-07-06 14:03:29.000000 tortoise-orm-0.9.2/tortoise_orm.egg-info/dependency_links.txt
--rw-r--r--   0 andreybondar   (501) staff       (20)       34 2018-07-04 08:12:39.000000 tortoise-orm-0.9.2/requirements.txt
--rw-r--r--   0 andreybondar   (501) staff       (20)       58 2018-03-29 18:11:07.000000 tortoise-orm-0.9.2/MANIFEST.in
--rw-r--r--   0 andreybondar   (501) staff       (20)     1717 2018-06-29 08:38:53.000000 tortoise-orm-0.9.2/setup.py
--rw-r--r--   0 andreybondar   (501) staff       (20)       38 2018-07-06 14:03:29.000000 tortoise-orm-0.9.2/setup.cfg
--rw-r--r--   0 andreybondar   (501) staff       (20)     4079 2018-07-06 14:01:57.000000 tortoise-orm-0.9.2/README.rst
-drwxr-xr-x   0 andreybondar   (501) staff       (20)        0 2018-07-06 14:03:29.000000 tortoise-orm-0.9.2/tortoise/
-drwxr-xr-x   0 andreybondar   (501) staff       (20)        0 2018-07-06 14:03:29.000000 tortoise-orm-0.9.2/tortoise/pylint/
-drwxr-xr-x   0 andreybondar   (501) staff       (20)        0 2018-07-06 14:03:29.000000 tortoise-orm-0.9.2/tortoise/pylint/__pycache__/
--rw-r--r--   0 andreybondar   (501) staff       (20)     2984 2018-06-29 12:51:31.000000 tortoise-orm-0.9.2/tortoise/pylint/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0 andreybondar   (501) staff       (20)     2172 2018-06-29 10:17:59.000000 tortoise-orm-0.9.2/tortoise/aggregation.py
--rw-r--r--   0 andreybondar   (501) staff       (20)     6148 2018-05-14 13:42:14.000000 tortoise-orm-0.9.2/tortoise/.DS_Store
--rw-r--r--   0 andreybondar   (501) staff       (20)    14339 2018-07-06 14:01:57.000000 tortoise-orm-0.9.2/tortoise/models.py
--rw-r--r--   0 andreybondar   (501) staff       (20)    10872 2018-07-06 14:01:57.000000 tortoise-orm-0.9.2/tortoise/fields.py
-drwxr-xr-x   0 andreybondar   (501) staff       (20)        0 2018-07-06 14:03:29.000000 tortoise-orm-0.9.2/tortoise/backends/
-drwxr-xr-x   0 andreybondar   (501) staff       (20)        0 2018-07-06 14:03:29.000000 tortoise-orm-0.9.2/tortoise/backends/dummy/
--rw-r--r--   0 andreybondar   (501) staff       (20)        0 2018-03-24 19:47:14.000000 tortoise-orm-0.9.2/tortoise/backends/dummy/__init__.py
--rw-r--r--   0 andreybondar   (501) staff       (20)     6148 2018-05-14 13:42:14.000000 tortoise-orm-0.9.2/tortoise/backends/.DS_Store
-drwxr-xr-x   0 andreybondar   (501) staff       (20)        0 2018-07-06 14:03:29.000000 tortoise-orm-0.9.2/tortoise/backends/asyncpg/
--rw-r--r--   0 andreybondar   (501) staff       (20)     6148 2018-05-14 13:41:13.000000 tortoise-orm-0.9.2/tortoise/backends/asyncpg/.DS_Store
--rw-r--r--   0 andreybondar   (501) staff       (20)     6567 2018-07-06 14:01:57.000000 tortoise-orm-0.9.2/tortoise/backends/asyncpg/client.py
--rw-r--r--   0 andreybondar   (501) staff       (20)        0 2018-03-24 06:07:06.000000 tortoise-orm-0.9.2/tortoise/backends/asyncpg/__init__.py
-drwxr-xr-x   0 andreybondar   (501) staff       (20)        0 2018-07-06 14:03:29.000000 tortoise-orm-0.9.2/tortoise/backends/asyncpg/__pycache__/
--rw-r--r--   0 andreybondar   (501) staff       (20)     6301 2018-07-06 14:03:06.000000 tortoise-orm-0.9.2/tortoise/backends/asyncpg/__pycache__/client.cpython-36.pyc
--rw-r--r--   0 andreybondar   (501) staff       (20)      960 2018-07-06 14:03:06.000000 tortoise-orm-0.9.2/tortoise/backends/asyncpg/__pycache__/schema_generator.cpython-36.pyc
--rw-r--r--   0 andreybondar   (501) staff       (20)     1059 2018-07-02 07:36:02.000000 tortoise-orm-0.9.2/tortoise/backends/asyncpg/__pycache__/executor.cpython-36.pyc
--rw-r--r--   0 andreybondar   (501) staff       (20)     1032 2018-07-04 08:13:04.000000 tortoise-orm-0.9.2/tortoise/backends/asyncpg/__pycache__/fields.cpython-36.pyc
--rw-r--r--   0 andreybondar   (501) staff       (20)      169 2018-04-03 13:43:43.000000 tortoise-orm-0.9.2/tortoise/backends/asyncpg/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0 andreybondar   (501) staff       (20)      428 2018-07-06 14:01:57.000000 tortoise-orm-0.9.2/tortoise/backends/asyncpg/schema_generator.py
--rw-r--r--   0 andreybondar   (501) staff       (20)      901 2018-07-02 07:35:18.000000 tortoise-orm-0.9.2/tortoise/backends/asyncpg/executor.py
--rw-r--r--   0 andreybondar   (501) staff       (20)        0 2018-03-24 06:00:52.000000 tortoise-orm-0.9.2/tortoise/backends/__init__.py
-drwxr-xr-x   0 andreybondar   (501) staff       (20)        0 2018-07-06 14:03:29.000000 tortoise-orm-0.9.2/tortoise/backends/sqlite/
--rw-r--r--   0 andreybondar   (501) staff       (20)     6148 2018-05-14 13:41:12.000000 tortoise-orm-0.9.2/tortoise/backends/sqlite/.DS_Store
--rw-r--r--   0 andreybondar   (501) staff       (20)     4390 2018-07-06 14:01:57.000000 tortoise-orm-0.9.2/tortoise/backends/sqlite/client.py
--rw-r--r--   0 andreybondar   (501) staff       (20)        0 2018-03-28 17:36:51.000000 tortoise-orm-0.9.2/tortoise/backends/sqlite/__init__.py
-drwxr-xr-x   0 andreybondar   (501) staff       (20)        0 2018-07-06 14:03:29.000000 tortoise-orm-0.9.2/tortoise/backends/sqlite/__pycache__/
--rw-r--r--   0 andreybondar   (501) staff       (20)     5632 2018-07-06 14:03:06.000000 tortoise-orm-0.9.2/tortoise/backends/sqlite/__pycache__/client.cpython-36.pyc
--rw-r--r--   0 andreybondar   (501) staff       (20)     1039 2018-07-06 14:03:07.000000 tortoise-orm-0.9.2/tortoise/backends/sqlite/__pycache__/schema_generator.cpython-36.pyc
--rw-r--r--   0 andreybondar   (501) staff       (20)     1803 2018-07-06 14:03:07.000000 tortoise-orm-0.9.2/tortoise/backends/sqlite/__pycache__/executor.cpython-36.pyc
--rw-r--r--   0 andreybondar   (501) staff       (20)      168 2018-03-29 10:06:00.000000 tortoise-orm-0.9.2/tortoise/backends/sqlite/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0 andreybondar   (501) staff       (20)      557 2018-07-06 14:01:57.000000 tortoise-orm-0.9.2/tortoise/backends/sqlite/schema_generator.py
--rw-r--r--   0 andreybondar   (501) staff       (20)     1646 2018-07-06 14:01:57.000000 tortoise-orm-0.9.2/tortoise/backends/sqlite/executor.py
-drwxr-xr-x   0 andreybondar   (501) staff       (20)        0 2018-07-06 14:03:29.000000 tortoise-orm-0.9.2/tortoise/backends/__pycache__/
--rw-r--r--   0 andreybondar   (501) staff       (20)      161 2018-03-29 10:05:34.000000 tortoise-orm-0.9.2/tortoise/backends/__pycache__/__init__.cpython-36.pyc
-drwxr-xr-x   0 andreybondar   (501) staff       (20)        0 2018-07-06 14:03:29.000000 tortoise-orm-0.9.2/tortoise/backends/base/
--rw-r--r--   0 andreybondar   (501) staff       (20)     6148 2018-05-14 13:41:14.000000 tortoise-orm-0.9.2/tortoise/backends/base/.DS_Store
--rw-r--r--   0 andreybondar   (501) staff       (20)     1997 2018-07-04 08:12:39.000000 tortoise-orm-0.9.2/tortoise/backends/base/db_url.py
--rw-r--r--   0 andreybondar   (501) staff       (20)     2596 2018-07-06 14:01:57.000000 tortoise-orm-0.9.2/tortoise/backends/base/client.py
--rw-r--r--   0 andreybondar   (501) staff       (20)        0 2018-03-24 06:07:06.000000 tortoise-orm-0.9.2/tortoise/backends/base/__init__.py
-drwxr-xr-x   0 andreybondar   (501) staff       (20)        0 2018-07-06 14:03:29.000000 tortoise-orm-0.9.2/tortoise/backends/base/__pycache__/
--rw-r--r--   0 andreybondar   (501) staff       (20)     4014 2018-07-06 14:03:06.000000 tortoise-orm-0.9.2/tortoise/backends/base/__pycache__/client.cpython-36.pyc
--rw-r--r--   0 andreybondar   (501) staff       (20)     4174 2018-07-06 14:03:06.000000 tortoise-orm-0.9.2/tortoise/backends/base/__pycache__/schema_generator.cpython-36.pyc
--rw-r--r--   0 andreybondar   (501) staff       (20)     8212 2018-07-06 14:03:06.000000 tortoise-orm-0.9.2/tortoise/backends/base/__pycache__/executor.cpython-36.pyc
--rw-r--r--   0 andreybondar   (501) staff       (20)     1591 2018-07-04 08:13:04.000000 tortoise-orm-0.9.2/tortoise/backends/base/__pycache__/db_url.cpython-36.pyc
--rw-r--r--   0 andreybondar   (501) staff       (20)      166 2018-03-29 10:05:34.000000 tortoise-orm-0.9.2/tortoise/backends/base/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0 andreybondar   (501) staff       (20)     5356 2018-07-06 14:01:57.000000 tortoise-orm-0.9.2/tortoise/backends/base/schema_generator.py
--rw-r--r--   0 andreybondar   (501) staff       (20)    10361 2018-07-06 14:01:57.000000 tortoise-orm-0.9.2/tortoise/backends/base/executor.py
-drwxr-xr-x   0 andreybondar   (501) staff       (20)        0 2018-07-06 14:03:29.000000 tortoise-orm-0.9.2/tortoise/tests/
--rw-r--r--   0 andreybondar   (501) staff       (20)      742 2018-07-04 08:12:39.000000 tortoise-orm-0.9.2/tortoise/tests/test_basic.py
--rw-r--r--   0 andreybondar   (501) staff       (20)      817 2018-07-06 14:01:57.000000 tortoise-orm-0.9.2/tortoise/tests/test_schema_create.py
--rw-r--r--   0 andreybondar   (501) staff       (20)     1895 2018-07-04 08:12:39.000000 tortoise-orm-0.9.2/tortoise/tests/test_aggregation.py
--rw-r--r--   0 andreybondar   (501) staff       (20)        0 2018-07-04 08:12:39.000000 tortoise-orm-0.9.2/tortoise/tests/__init__.py
-drwxr-xr-x   0 andreybondar   (501) staff       (20)        0 2018-07-06 14:03:29.000000 tortoise-orm-0.9.2/tortoise/tests/__pycache__/
--rw-r--r--   0 andreybondar   (501) staff       (20)    16857 2018-07-06 14:03:07.000000 tortoise-orm-0.9.2/tortoise/tests/__pycache__/test_fields.cpython-36.pyc
--rw-r--r--   0 andreybondar   (501) staff       (20)     2111 2018-07-04 08:13:04.000000 tortoise-orm-0.9.2/tortoise/tests/__pycache__/test_relations.cpython-36.pyc
--rw-r--r--   0 andreybondar   (501) staff       (20)     1110 2018-07-04 08:13:04.000000 tortoise-orm-0.9.2/tortoise/tests/__pycache__/test_transactions.cpython-36.pyc
--rw-r--r--   0 andreybondar   (501) staff       (20)     1739 2018-07-04 08:13:03.000000 tortoise-orm-0.9.2/tortoise/tests/__pycache__/test_aggregation.cpython-36.pyc
--rw-r--r--   0 andreybondar   (501) staff       (20)     1084 2018-07-06 14:03:07.000000 tortoise-orm-0.9.2/tortoise/tests/__pycache__/test_schema_create.cpython-36.pyc
--rw-r--r--   0 andreybondar   (501) staff       (20)     1003 2018-07-04 08:13:04.000000 tortoise-orm-0.9.2/tortoise/tests/__pycache__/test_prefetching.cpython-36.pyc
--rw-r--r--   0 andreybondar   (501) staff       (20)     2484 2018-07-06 14:03:07.000000 tortoise-orm-0.9.2/tortoise/tests/__pycache__/test_two_databases.cpython-36.pyc
--rw-r--r--   0 andreybondar   (501) staff       (20)      939 2018-07-04 08:13:04.000000 tortoise-orm-0.9.2/tortoise/tests/__pycache__/test_basic.cpython-36.pyc
--rw-r--r--   0 andreybondar   (501) staff       (20)     1729 2018-07-04 08:13:04.000000 tortoise-orm-0.9.2/tortoise/tests/__pycache__/test_filtering.cpython-36.pyc
--rw-r--r--   0 andreybondar   (501) staff       (20)     5257 2018-07-06 14:03:07.000000 tortoise-orm-0.9.2/tortoise/tests/__pycache__/testmodels.cpython-36.pyc
--rw-r--r--   0 andreybondar   (501) staff       (20)      158 2018-07-04 08:13:03.000000 tortoise-orm-0.9.2/tortoise/tests/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0 andreybondar   (501) staff       (20)      937 2018-07-04 08:12:39.000000 tortoise-orm-0.9.2/tortoise/tests/test_transactions.py
--rw-r--r--   0 andreybondar   (501) staff       (20)    14187 2018-07-06 14:01:57.000000 tortoise-orm-0.9.2/tortoise/tests/test_fields.py
--rw-r--r--   0 andreybondar   (501) staff       (20)     3269 2018-07-06 14:01:57.000000 tortoise-orm-0.9.2/tortoise/tests/testmodels.py
--rw-r--r--   0 andreybondar   (501) staff       (20)     2418 2018-07-06 14:01:57.000000 tortoise-orm-0.9.2/tortoise/tests/test_two_databases.py
--rw-r--r--   0 andreybondar   (501) staff       (20)      760 2018-07-04 08:12:39.000000 tortoise-orm-0.9.2/tortoise/tests/test_prefetching.py
--rw-r--r--   0 andreybondar   (501) staff       (20)     2125 2018-07-04 08:12:39.000000 tortoise-orm-0.9.2/tortoise/tests/test_relations.py
--rw-r--r--   0 andreybondar   (501) staff       (20)     1955 2018-07-04 08:12:39.000000 tortoise-orm-0.9.2/tortoise/tests/test_filtering.py
--rw-r--r--   0 andreybondar   (501) staff       (20)     6758 2018-07-06 14:02:50.000000 tortoise-orm-0.9.2/tortoise/__init__.py
-drwxr-xr-x   0 andreybondar   (501) staff       (20)        0 2018-07-06 14:03:29.000000 tortoise-orm-0.9.2/tortoise/__pycache__/
--rw-r--r--   0 andreybondar   (501) staff       (20)     4178 2018-06-29 12:51:31.000000 tortoise-orm-0.9.2/tortoise/__pycache__/query_utils.cpython-36.pyc
--rw-r--r--   0 andreybondar   (501) staff       (20)     1463 2018-07-06 14:03:06.000000 tortoise-orm-0.9.2/tortoise/__pycache__/exceptions.cpython-36.pyc
--rw-r--r--   0 andreybondar   (501) staff       (20)     2254 2018-06-29 12:51:31.000000 tortoise-orm-0.9.2/tortoise/__pycache__/aggregation.cpython-36.pyc
--rw-r--r--   0 andreybondar   (501) staff       (20)    19258 2018-07-06 14:03:06.000000 tortoise-orm-0.9.2/tortoise/__pycache__/queryset.cpython-36.pyc
--rw-r--r--   0 andreybondar   (501) staff       (20)    10589 2018-07-06 14:03:06.000000 tortoise-orm-0.9.2/tortoise/__pycache__/models.cpython-36.pyc
--rw-r--r--   0 andreybondar   (501) staff       (20)     1205 2018-04-12 13:02:01.000000 tortoise-orm-0.9.2/tortoise/__pycache__/utils.cpython-36.pyc
--rw-r--r--   0 andreybondar   (501) staff       (20)    12718 2018-07-06 14:03:06.000000 tortoise-orm-0.9.2/tortoise/__pycache__/fields.cpython-36.pyc
--rw-r--r--   0 andreybondar   (501) staff       (20)     3968 2018-07-06 14:03:06.000000 tortoise-orm-0.9.2/tortoise/__pycache__/__init__.cpython-36.pyc
-drwxr-xr-x   0 andreybondar   (501) staff       (20)        0 2018-07-06 14:03:29.000000 tortoise-orm-0.9.2/tortoise/contrib/
-drwxr-xr-x   0 andreybondar   (501) staff       (20)        0 2018-07-06 14:03:29.000000 tortoise-orm-0.9.2/tortoise/contrib/pylint/
--rw-r--r--   0 andreybondar   (501) staff       (20)     4829 2018-07-04 08:12:39.000000 tortoise-orm-0.9.2/tortoise/contrib/pylint/__init__.py
-drwxr-xr-x   0 andreybondar   (501) staff       (20)        0 2018-07-06 14:03:29.000000 tortoise-orm-0.9.2/tortoise/contrib/test/
--rw-r--r--   0 andreybondar   (501) staff       (20)     2076 2018-07-04 08:12:39.000000 tortoise-orm-0.9.2/tortoise/contrib/test/__init__.py
-drwxr-xr-x   0 andreybondar   (501) staff       (20)        0 2018-07-06 14:03:29.000000 tortoise-orm-0.9.2/tortoise/contrib/test/__pycache__/
--rw-r--r--   0 andreybondar   (501) staff       (20)     2229 2018-07-04 08:13:03.000000 tortoise-orm-0.9.2/tortoise/contrib/test/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0 andreybondar   (501) staff       (20)        0 2018-07-04 08:12:39.000000 tortoise-orm-0.9.2/tortoise/contrib/__init__.py
-drwxr-xr-x   0 andreybondar   (501) staff       (20)        0 2018-07-06 14:03:29.000000 tortoise-orm-0.9.2/tortoise/contrib/__pycache__/
--rw-r--r--   0 andreybondar   (501) staff       (20)      160 2018-07-04 08:13:03.000000 tortoise-orm-0.9.2/tortoise/contrib/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0 andreybondar   (501) staff       (20)      693 2018-04-12 13:01:54.000000 tortoise-orm-0.9.2/tortoise/utils.py
--rw-r--r--   0 andreybondar   (501) staff       (20)    25549 2018-07-06 14:01:57.000000 tortoise-orm-0.9.2/tortoise/queryset.py
--rw-r--r--   0 andreybondar   (501) staff       (20)      570 2018-07-06 14:01:57.000000 tortoise-orm-0.9.2/tortoise/exceptions.py
--rw-r--r--   0 andreybondar   (501) staff       (20)     5568 2018-06-29 10:17:59.000000 tortoise-orm-0.9.2/tortoise/query_utils.py
+drwxr-xr-x   0 andreybondar   (501) staff       (20)        0 2018-07-17 08:16:22.000000 tortoise-orm-0.9.4/
+-rw-r--r--   0 andreybondar   (501) staff       (20)     6345 2018-07-17 08:16:22.000000 tortoise-orm-0.9.4/PKG-INFO
+drwxr-xr-x   0 andreybondar   (501) staff       (20)        0 2018-07-17 08:16:22.000000 tortoise-orm-0.9.4/tortoise_orm.egg-info/
+-rw-r--r--   0 andreybondar   (501) staff       (20)     6345 2018-07-17 08:16:21.000000 tortoise-orm-0.9.4/tortoise_orm.egg-info/PKG-INFO
+-rw-r--r--   0 andreybondar   (501) staff       (20)     7722 2018-07-17 08:16:22.000000 tortoise-orm-0.9.4/tortoise_orm.egg-info/SOURCES.txt
+-rw-r--r--   0 andreybondar   (501) staff       (20)       34 2018-07-17 08:16:21.000000 tortoise-orm-0.9.4/tortoise_orm.egg-info/requires.txt
+-rw-r--r--   0 andreybondar   (501) staff       (20)        9 2018-07-17 08:16:21.000000 tortoise-orm-0.9.4/tortoise_orm.egg-info/top_level.txt
+-rw-r--r--   0 andreybondar   (501) staff       (20)        1 2018-07-17 08:16:21.000000 tortoise-orm-0.9.4/tortoise_orm.egg-info/dependency_links.txt
+-rw-r--r--   0 andreybondar   (501) staff       (20)       34 2018-07-17 08:14:22.000000 tortoise-orm-0.9.4/requirements.txt
+-rw-r--r--   0 andreybondar   (501) staff       (20)       64 2018-07-17 08:16:01.000000 tortoise-orm-0.9.4/MANIFEST.in
+-rw-r--r--   0 andreybondar   (501) staff       (20)     1806 2018-07-17 08:16:01.000000 tortoise-orm-0.9.4/setup.py
+-rw-r--r--   0 andreybondar   (501) staff       (20)       38 2018-07-17 08:16:22.000000 tortoise-orm-0.9.4/setup.cfg
+-rw-r--r--   0 andreybondar   (501) staff       (20)     4382 2018-07-10 09:39:40.000000 tortoise-orm-0.9.4/README.rst
+-rw-r--r--   0 andreybondar   (501) staff       (20)    11342 2018-03-29 09:50:16.000000 tortoise-orm-0.9.4/LICENSE.txt
+drwxr-xr-x   0 andreybondar   (501) staff       (20)        0 2018-07-17 08:16:22.000000 tortoise-orm-0.9.4/tortoise/
+drwxr-xr-x   0 andreybondar   (501) staff       (20)        0 2018-07-17 08:16:22.000000 tortoise-orm-0.9.4/tortoise/pylint/
+drwxr-xr-x   0 andreybondar   (501) staff       (20)        0 2018-07-17 08:16:22.000000 tortoise-orm-0.9.4/tortoise/pylint/__pycache__/
+-rw-r--r--   0 andreybondar   (501) staff       (20)     2984 2018-06-29 12:51:31.000000 tortoise-orm-0.9.4/tortoise/pylint/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)     2301 2018-07-10 09:39:40.000000 tortoise-orm-0.9.4/tortoise/aggregation.py
+-rw-r--r--   0 andreybondar   (501) staff       (20)     6148 2018-05-14 13:42:14.000000 tortoise-orm-0.9.4/tortoise/.DS_Store
+-rw-r--r--   0 andreybondar   (501) staff       (20)    15097 2018-07-17 08:16:01.000000 tortoise-orm-0.9.4/tortoise/models.py
+-rw-r--r--   0 andreybondar   (501) staff       (20)    14862 2018-07-17 08:16:01.000000 tortoise-orm-0.9.4/tortoise/fields.py
+drwxr-xr-x   0 andreybondar   (501) staff       (20)        0 2018-07-17 08:16:22.000000 tortoise-orm-0.9.4/tortoise/backends/
+-rw-r--r--   0 andreybondar   (501) staff       (20)     6148 2018-05-14 13:42:14.000000 tortoise-orm-0.9.4/tortoise/backends/.DS_Store
+drwxr-xr-x   0 andreybondar   (501) staff       (20)        0 2018-07-17 08:16:22.000000 tortoise-orm-0.9.4/tortoise/backends/asyncpg/
+-rw-r--r--   0 andreybondar   (501) staff       (20)     6148 2018-05-14 13:41:13.000000 tortoise-orm-0.9.4/tortoise/backends/asyncpg/.DS_Store
+-rw-r--r--   0 andreybondar   (501) staff       (20)     6610 2018-07-17 08:14:22.000000 tortoise-orm-0.9.4/tortoise/backends/asyncpg/client.py
+-rw-r--r--   0 andreybondar   (501) staff       (20)        0 2018-07-17 08:14:22.000000 tortoise-orm-0.9.4/tortoise/backends/asyncpg/__init__.py
+drwxr-xr-x   0 andreybondar   (501) staff       (20)        0 2018-07-17 08:16:22.000000 tortoise-orm-0.9.4/tortoise/backends/asyncpg/__pycache__/
+-rw-r--r--   0 andreybondar   (501) staff       (20)     6465 2018-07-16 12:09:54.000000 tortoise-orm-0.9.4/tortoise/backends/asyncpg/__pycache__/client.cpython-36.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)     6305 2018-07-06 15:59:59.000000 tortoise-orm-0.9.4/tortoise/backends/asyncpg/__pycache__/client.cpython-37.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)     6826 2018-07-06 16:30:05.000000 tortoise-orm-0.9.4/tortoise/backends/asyncpg/__pycache__/client.cpython-35.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)      960 2018-07-06 14:03:06.000000 tortoise-orm-0.9.4/tortoise/backends/asyncpg/__pycache__/schema_generator.cpython-36.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)      964 2018-07-06 15:59:59.000000 tortoise-orm-0.9.4/tortoise/backends/asyncpg/__pycache__/schema_generator.cpython-37.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)      984 2018-07-06 16:30:05.000000 tortoise-orm-0.9.4/tortoise/backends/asyncpg/__pycache__/schema_generator.cpython-35.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)     1063 2018-07-06 15:59:59.000000 tortoise-orm-0.9.4/tortoise/backends/asyncpg/__pycache__/executor.cpython-37.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)     1059 2018-07-02 07:36:02.000000 tortoise-orm-0.9.4/tortoise/backends/asyncpg/__pycache__/executor.cpython-36.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)     1144 2018-07-06 16:30:05.000000 tortoise-orm-0.9.4/tortoise/backends/asyncpg/__pycache__/executor.cpython-35.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)     1032 2018-07-04 08:13:04.000000 tortoise-orm-0.9.4/tortoise/backends/asyncpg/__pycache__/fields.cpython-36.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)      235 2018-07-15 16:51:38.000000 tortoise-orm-0.9.4/tortoise/backends/asyncpg/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)      173 2018-07-06 15:59:59.000000 tortoise-orm-0.9.4/tortoise/backends/asyncpg/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)      169 2018-07-06 16:30:05.000000 tortoise-orm-0.9.4/tortoise/backends/asyncpg/__pycache__/__init__.cpython-35.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)      428 2018-07-06 14:01:57.000000 tortoise-orm-0.9.4/tortoise/backends/asyncpg/schema_generator.py
+-rw-r--r--   0 andreybondar   (501) staff       (20)      901 2018-07-02 07:35:18.000000 tortoise-orm-0.9.4/tortoise/backends/asyncpg/executor.py
+-rw-r--r--   0 andreybondar   (501) staff       (20)        0 2018-03-24 06:00:52.000000 tortoise-orm-0.9.4/tortoise/backends/__init__.py
+drwxr-xr-x   0 andreybondar   (501) staff       (20)        0 2018-07-17 08:16:22.000000 tortoise-orm-0.9.4/tortoise/backends/sqlite/
+-rw-r--r--   0 andreybondar   (501) staff       (20)     6148 2018-05-14 13:41:12.000000 tortoise-orm-0.9.4/tortoise/backends/sqlite/.DS_Store
+-rw-r--r--   0 andreybondar   (501) staff       (20)     4390 2018-07-17 08:14:22.000000 tortoise-orm-0.9.4/tortoise/backends/sqlite/client.py
+-rw-r--r--   0 andreybondar   (501) staff       (20)        0 2018-07-17 08:14:22.000000 tortoise-orm-0.9.4/tortoise/backends/sqlite/__init__.py
+drwxr-xr-x   0 andreybondar   (501) staff       (20)        0 2018-07-17 08:16:22.000000 tortoise-orm-0.9.4/tortoise/backends/sqlite/__pycache__/
+-rw-r--r--   0 andreybondar   (501) staff       (20)     5796 2018-07-16 12:09:54.000000 tortoise-orm-0.9.4/tortoise/backends/sqlite/__pycache__/client.cpython-36.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)     6189 2018-07-15 19:35:33.000000 tortoise-orm-0.9.4/tortoise/backends/sqlite/__pycache__/client.cpython-37.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)     5959 2018-07-06 16:30:05.000000 tortoise-orm-0.9.4/tortoise/backends/sqlite/__pycache__/client.cpython-35.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)     1039 2018-07-06 14:03:07.000000 tortoise-orm-0.9.4/tortoise/backends/sqlite/__pycache__/schema_generator.cpython-36.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)     1043 2018-07-06 15:59:59.000000 tortoise-orm-0.9.4/tortoise/backends/sqlite/__pycache__/schema_generator.cpython-37.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)     1069 2018-07-06 16:30:05.000000 tortoise-orm-0.9.4/tortoise/backends/sqlite/__pycache__/schema_generator.cpython-35.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)     1807 2018-07-06 15:59:59.000000 tortoise-orm-0.9.4/tortoise/backends/sqlite/__pycache__/executor.cpython-37.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)     1803 2018-07-06 14:03:07.000000 tortoise-orm-0.9.4/tortoise/backends/sqlite/__pycache__/executor.cpython-36.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)     1960 2018-07-06 16:30:05.000000 tortoise-orm-0.9.4/tortoise/backends/sqlite/__pycache__/executor.cpython-35.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)      231 2018-07-11 16:19:37.000000 tortoise-orm-0.9.4/tortoise/backends/sqlite/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)      235 2018-07-15 19:35:33.000000 tortoise-orm-0.9.4/tortoise/backends/sqlite/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)      168 2018-07-06 16:30:05.000000 tortoise-orm-0.9.4/tortoise/backends/sqlite/__pycache__/__init__.cpython-35.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)      557 2018-07-06 14:01:57.000000 tortoise-orm-0.9.4/tortoise/backends/sqlite/schema_generator.py
+-rw-r--r--   0 andreybondar   (501) staff       (20)     1646 2018-07-06 14:01:57.000000 tortoise-orm-0.9.4/tortoise/backends/sqlite/executor.py
+drwxr-xr-x   0 andreybondar   (501) staff       (20)        0 2018-07-17 08:16:22.000000 tortoise-orm-0.9.4/tortoise/backends/__pycache__/
+-rw-r--r--   0 andreybondar   (501) staff       (20)      161 2018-03-29 10:05:34.000000 tortoise-orm-0.9.4/tortoise/backends/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)      118 2018-07-06 15:46:58.000000 tortoise-orm-0.9.4/tortoise/backends/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)      161 2018-07-06 16:30:05.000000 tortoise-orm-0.9.4/tortoise/backends/__pycache__/__init__.cpython-35.pyc
+drwxr-xr-x   0 andreybondar   (501) staff       (20)        0 2018-07-17 08:16:22.000000 tortoise-orm-0.9.4/tortoise/backends/base/
+-rw-r--r--   0 andreybondar   (501) staff       (20)     6148 2018-05-14 13:41:14.000000 tortoise-orm-0.9.4/tortoise/backends/base/.DS_Store
+-rw-r--r--   0 andreybondar   (501) staff       (20)     2045 2018-07-17 08:16:01.000000 tortoise-orm-0.9.4/tortoise/backends/base/db_url.py
+-rw-r--r--   0 andreybondar   (501) staff       (20)     2596 2018-07-17 08:14:22.000000 tortoise-orm-0.9.4/tortoise/backends/base/client.py
+-rw-r--r--   0 andreybondar   (501) staff       (20)        0 2018-03-24 06:07:06.000000 tortoise-orm-0.9.4/tortoise/backends/base/__init__.py
+drwxr-xr-x   0 andreybondar   (501) staff       (20)        0 2018-07-17 08:16:22.000000 tortoise-orm-0.9.4/tortoise/backends/base/__pycache__/
+-rw-r--r--   0 andreybondar   (501) staff       (20)     4055 2018-07-16 12:09:54.000000 tortoise-orm-0.9.4/tortoise/backends/base/__pycache__/client.cpython-36.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)     4201 2018-07-15 19:35:33.000000 tortoise-orm-0.9.4/tortoise/backends/base/__pycache__/client.cpython-37.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)     4218 2018-07-06 16:30:05.000000 tortoise-orm-0.9.4/tortoise/backends/base/__pycache__/client.cpython-35.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)     4174 2018-07-06 14:03:06.000000 tortoise-orm-0.9.4/tortoise/backends/base/__pycache__/schema_generator.cpython-36.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)     4133 2018-07-06 15:46:58.000000 tortoise-orm-0.9.4/tortoise/backends/base/__pycache__/schema_generator.cpython-37.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)     4543 2018-07-06 16:30:05.000000 tortoise-orm-0.9.4/tortoise/backends/base/__pycache__/schema_generator.cpython-35.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)     8267 2018-07-15 19:35:33.000000 tortoise-orm-0.9.4/tortoise/backends/base/__pycache__/executor.cpython-37.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)     8263 2018-07-11 15:01:48.000000 tortoise-orm-0.9.4/tortoise/backends/base/__pycache__/executor.cpython-36.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)     9083 2018-07-06 16:30:05.000000 tortoise-orm-0.9.4/tortoise/backends/base/__pycache__/executor.cpython-35.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)     1817 2018-07-15 17:34:22.000000 tortoise-orm-0.9.4/tortoise/backends/base/__pycache__/db_url.cpython-36.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)     1593 2018-07-06 15:59:59.000000 tortoise-orm-0.9.4/tortoise/backends/base/__pycache__/db_url.cpython-37.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)     1770 2018-07-06 16:30:05.000000 tortoise-orm-0.9.4/tortoise/backends/base/__pycache__/db_url.cpython-35.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)      166 2018-03-29 10:05:34.000000 tortoise-orm-0.9.4/tortoise/backends/base/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)      123 2018-07-06 15:46:58.000000 tortoise-orm-0.9.4/tortoise/backends/base/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)      166 2018-07-06 16:30:05.000000 tortoise-orm-0.9.4/tortoise/backends/base/__pycache__/__init__.cpython-35.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)     5499 2018-07-17 08:16:01.000000 tortoise-orm-0.9.4/tortoise/backends/base/schema_generator.py
+-rw-r--r--   0 andreybondar   (501) staff       (20)    10521 2018-07-17 08:16:01.000000 tortoise-orm-0.9.4/tortoise/backends/base/executor.py
+drwxr-xr-x   0 andreybondar   (501) staff       (20)        0 2018-07-17 08:16:22.000000 tortoise-orm-0.9.4/tortoise/tests/
+-rw-r--r--   0 andreybondar   (501) staff       (20)      738 2018-07-17 08:16:01.000000 tortoise-orm-0.9.4/tortoise/tests/test_basic.py
+-rw-r--r--   0 andreybondar   (501) staff       (20)      813 2018-07-17 08:16:01.000000 tortoise-orm-0.9.4/tortoise/tests/test_schema_create.py
+-rw-r--r--   0 andreybondar   (501) staff       (20)     1891 2018-07-17 08:16:01.000000 tortoise-orm-0.9.4/tortoise/tests/test_aggregation.py
+-rw-r--r--   0 andreybondar   (501) staff       (20)        0 2018-07-04 08:12:39.000000 tortoise-orm-0.9.4/tortoise/tests/__init__.py
+drwxr-xr-x   0 andreybondar   (501) staff       (20)        0 2018-07-17 08:16:22.000000 tortoise-orm-0.9.4/tortoise/tests/__pycache__/
+-rw-r--r--   0 andreybondar   (501) staff       (20)    16857 2018-07-06 14:03:07.000000 tortoise-orm-0.9.4/tortoise/tests/__pycache__/test_fields.cpython-36.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)    16856 2018-07-06 15:59:59.000000 tortoise-orm-0.9.4/tortoise/tests/__pycache__/test_fields.cpython-37.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)    18088 2018-07-06 16:30:05.000000 tortoise-orm-0.9.4/tortoise/tests/__pycache__/test_fields.cpython-35.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)     2111 2018-07-04 08:13:04.000000 tortoise-orm-0.9.4/tortoise/tests/__pycache__/test_relations.cpython-36.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)     1178 2018-07-06 16:30:05.000000 tortoise-orm-0.9.4/tortoise/tests/__pycache__/test_transactions.cpython-35.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)     2103 2018-07-06 15:59:59.000000 tortoise-orm-0.9.4/tortoise/tests/__pycache__/test_relations.cpython-37.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)     2284 2018-07-06 16:30:05.000000 tortoise-orm-0.9.4/tortoise/tests/__pycache__/test_relations.cpython-35.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)     1114 2018-07-06 15:59:59.000000 tortoise-orm-0.9.4/tortoise/tests/__pycache__/test_transactions.cpython-37.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)     2493 2018-07-16 12:21:08.000000 tortoise-orm-0.9.4/tortoise/tests/__pycache__/test_transactions.cpython-36.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)     1743 2018-07-06 15:59:59.000000 tortoise-orm-0.9.4/tortoise/tests/__pycache__/test_aggregation.cpython-37.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)     1739 2018-07-04 08:13:03.000000 tortoise-orm-0.9.4/tortoise/tests/__pycache__/test_aggregation.cpython-36.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)     1890 2018-07-06 16:30:05.000000 tortoise-orm-0.9.4/tortoise/tests/__pycache__/test_aggregation.cpython-35.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)     1007 2018-07-06 15:59:59.000000 tortoise-orm-0.9.4/tortoise/tests/__pycache__/test_prefetching.cpython-37.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)     1084 2018-07-06 14:03:07.000000 tortoise-orm-0.9.4/tortoise/tests/__pycache__/test_schema_create.cpython-36.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)     1088 2018-07-06 15:59:59.000000 tortoise-orm-0.9.4/tortoise/tests/__pycache__/test_schema_create.cpython-37.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)     1003 2018-07-04 08:13:04.000000 tortoise-orm-0.9.4/tortoise/tests/__pycache__/test_prefetching.cpython-36.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)     1165 2018-07-06 16:30:05.000000 tortoise-orm-0.9.4/tortoise/tests/__pycache__/test_schema_create.cpython-35.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)     1070 2018-07-06 16:30:05.000000 tortoise-orm-0.9.4/tortoise/tests/__pycache__/test_prefetching.cpython-35.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)     2488 2018-07-06 15:59:59.000000 tortoise-orm-0.9.4/tortoise/tests/__pycache__/test_two_databases.cpython-37.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)     3296 2018-07-16 12:21:54.000000 tortoise-orm-0.9.4/tortoise/tests/__pycache__/test_two_databases.cpython-36.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)     2668 2018-07-06 16:30:05.000000 tortoise-orm-0.9.4/tortoise/tests/__pycache__/test_two_databases.cpython-35.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)      998 2018-07-06 16:30:05.000000 tortoise-orm-0.9.4/tortoise/tests/__pycache__/test_basic.cpython-35.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)      943 2018-07-06 15:59:59.000000 tortoise-orm-0.9.4/tortoise/tests/__pycache__/test_basic.cpython-37.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)      939 2018-07-04 08:13:04.000000 tortoise-orm-0.9.4/tortoise/tests/__pycache__/test_basic.cpython-36.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)     1729 2018-07-04 08:13:04.000000 tortoise-orm-0.9.4/tortoise/tests/__pycache__/test_filtering.cpython-36.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)     5257 2018-07-06 14:03:07.000000 tortoise-orm-0.9.4/tortoise/tests/__pycache__/testmodels.cpython-36.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)     5261 2018-07-06 15:59:59.000000 tortoise-orm-0.9.4/tortoise/tests/__pycache__/testmodels.cpython-37.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)     1733 2018-07-06 15:59:59.000000 tortoise-orm-0.9.4/tortoise/tests/__pycache__/test_filtering.cpython-37.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)     1891 2018-07-06 16:30:05.000000 tortoise-orm-0.9.4/tortoise/tests/__pycache__/test_filtering.cpython-35.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)     5698 2018-07-06 16:30:05.000000 tortoise-orm-0.9.4/tortoise/tests/__pycache__/testmodels.cpython-35.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)      158 2018-07-04 08:13:03.000000 tortoise-orm-0.9.4/tortoise/tests/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)      162 2018-07-06 15:59:59.000000 tortoise-orm-0.9.4/tortoise/tests/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)      158 2018-07-06 16:30:05.000000 tortoise-orm-0.9.4/tortoise/tests/__pycache__/__init__.cpython-35.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)      944 2018-07-17 08:16:01.000000 tortoise-orm-0.9.4/tortoise/tests/test_transactions.py
+-rw-r--r--   0 andreybondar   (501) staff       (20)    14324 2018-07-17 08:16:01.000000 tortoise-orm-0.9.4/tortoise/tests/test_fields.py
+-rw-r--r--   0 andreybondar   (501) staff       (20)     3651 2018-07-17 08:16:01.000000 tortoise-orm-0.9.4/tortoise/tests/testmodels.py
+-rw-r--r--   0 andreybondar   (501) staff       (20)     2525 2018-07-17 08:16:01.000000 tortoise-orm-0.9.4/tortoise/tests/test_two_databases.py
+-rw-r--r--   0 andreybondar   (501) staff       (20)      756 2018-07-17 08:16:01.000000 tortoise-orm-0.9.4/tortoise/tests/test_prefetching.py
+-rw-r--r--   0 andreybondar   (501) staff       (20)     2121 2018-07-17 08:16:01.000000 tortoise-orm-0.9.4/tortoise/tests/test_relations.py
+-rw-r--r--   0 andreybondar   (501) staff       (20)     1951 2018-07-17 08:16:01.000000 tortoise-orm-0.9.4/tortoise/tests/test_filtering.py
+-rw-r--r--   0 andreybondar   (501) staff       (20)     6999 2018-07-17 08:16:11.000000 tortoise-orm-0.9.4/tortoise/__init__.py
+drwxr-xr-x   0 andreybondar   (501) staff       (20)        0 2018-07-17 08:16:22.000000 tortoise-orm-0.9.4/tortoise/__pycache__/
+-rw-r--r--   0 andreybondar   (501) staff       (20)     4725 2018-07-06 16:30:05.000000 tortoise-orm-0.9.4/tortoise/__pycache__/query_utils.cpython-35.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)     4417 2018-07-11 15:01:48.000000 tortoise-orm-0.9.4/tortoise/__pycache__/query_utils.cpython-36.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)     4421 2018-07-15 19:35:33.000000 tortoise-orm-0.9.4/tortoise/__pycache__/query_utils.cpython-37.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)     1598 2018-07-15 18:01:23.000000 tortoise-orm-0.9.4/tortoise/__pycache__/exceptions.cpython-36.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)     2513 2018-07-06 16:30:05.000000 tortoise-orm-0.9.4/tortoise/__pycache__/aggregation.cpython-35.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)     1602 2018-07-15 19:35:33.000000 tortoise-orm-0.9.4/tortoise/__pycache__/exceptions.cpython-37.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)     1526 2018-07-06 16:30:05.000000 tortoise-orm-0.9.4/tortoise/__pycache__/exceptions.cpython-35.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)     2395 2018-07-15 19:35:33.000000 tortoise-orm-0.9.4/tortoise/__pycache__/aggregation.cpython-37.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)     2391 2018-07-11 15:01:48.000000 tortoise-orm-0.9.4/tortoise/__pycache__/aggregation.cpython-36.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)    19255 2018-07-15 19:35:33.000000 tortoise-orm-0.9.4/tortoise/__pycache__/queryset.cpython-37.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)    19255 2018-07-11 15:01:48.000000 tortoise-orm-0.9.4/tortoise/__pycache__/queryset.cpython-36.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)    21654 2018-07-06 16:30:05.000000 tortoise-orm-0.9.4/tortoise/__pycache__/queryset.cpython-35.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)    10788 2018-07-15 19:07:00.000000 tortoise-orm-0.9.4/tortoise/__pycache__/models.cpython-36.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)    10784 2018-07-15 19:35:33.000000 tortoise-orm-0.9.4/tortoise/__pycache__/models.cpython-37.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)    11875 2018-07-06 16:30:05.000000 tortoise-orm-0.9.4/tortoise/__pycache__/models.cpython-35.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)     1593 2018-07-06 16:30:05.000000 tortoise-orm-0.9.4/tortoise/__pycache__/utils.cpython-35.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)     1513 2018-07-15 17:34:22.000000 tortoise-orm-0.9.4/tortoise/__pycache__/utils.cpython-36.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)     1517 2018-07-15 19:35:33.000000 tortoise-orm-0.9.4/tortoise/__pycache__/utils.cpython-37.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)    13891 2018-07-06 16:30:05.000000 tortoise-orm-0.9.4/tortoise/__pycache__/fields.cpython-35.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)    13112 2018-07-15 19:12:51.000000 tortoise-orm-0.9.4/tortoise/__pycache__/fields.cpython-37.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)     1531 2018-07-16 12:09:54.000000 tortoise-orm-0.9.4/tortoise/__pycache__/context.cpython-36.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)     1230 2018-07-15 19:35:33.000000 tortoise-orm-0.9.4/tortoise/__pycache__/context.cpython-37.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)    13125 2018-07-11 15:01:48.000000 tortoise-orm-0.9.4/tortoise/__pycache__/fields.cpython-36.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)     7621 2018-07-16 16:10:34.000000 tortoise-orm-0.9.4/tortoise/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)     5786 2018-07-15 19:12:51.000000 tortoise-orm-0.9.4/tortoise/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)     4451 2018-07-06 16:30:05.000000 tortoise-orm-0.9.4/tortoise/__pycache__/__init__.cpython-35.pyc
+drwxr-xr-x   0 andreybondar   (501) staff       (20)        0 2018-07-17 08:16:22.000000 tortoise-orm-0.9.4/tortoise/contrib/
+drwxr-xr-x   0 andreybondar   (501) staff       (20)        0 2018-07-17 08:16:22.000000 tortoise-orm-0.9.4/tortoise/contrib/pylint/
+-rw-r--r--   0 andreybondar   (501) staff       (20)     4883 2018-07-17 08:16:01.000000 tortoise-orm-0.9.4/tortoise/contrib/pylint/__init__.py
+drwxr-xr-x   0 andreybondar   (501) staff       (20)        0 2018-07-17 08:16:22.000000 tortoise-orm-0.9.4/tortoise/contrib/pylint/__pycache__/
+-rw-r--r--   0 andreybondar   (501) staff       (20)     3182 2018-07-06 15:51:24.000000 tortoise-orm-0.9.4/tortoise/contrib/pylint/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)     3161 2018-07-06 15:46:58.000000 tortoise-orm-0.9.4/tortoise/contrib/pylint/__pycache__/__init__.cpython-37.pyc
+drwxr-xr-x   0 andreybondar   (501) staff       (20)        0 2018-07-17 08:16:22.000000 tortoise-orm-0.9.4/tortoise/contrib/test/
+-rw-r--r--   0 andreybondar   (501) staff       (20)     3921 2018-07-17 08:16:01.000000 tortoise-orm-0.9.4/tortoise/contrib/test/__init__.py
+drwxr-xr-x   0 andreybondar   (501) staff       (20)        0 2018-07-17 08:16:22.000000 tortoise-orm-0.9.4/tortoise/contrib/test/__pycache__/
+-rw-r--r--   0 andreybondar   (501) staff       (20)     1969 2018-07-15 17:52:19.000000 tortoise-orm-0.9.4/tortoise/contrib/test/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)     2233 2018-07-06 15:59:59.000000 tortoise-orm-0.9.4/tortoise/contrib/test/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)     2417 2018-07-06 16:30:05.000000 tortoise-orm-0.9.4/tortoise/contrib/test/__pycache__/__init__.cpython-35.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)        0 2018-07-04 08:12:39.000000 tortoise-orm-0.9.4/tortoise/contrib/__init__.py
+drwxr-xr-x   0 andreybondar   (501) staff       (20)        0 2018-07-17 08:16:22.000000 tortoise-orm-0.9.4/tortoise/contrib/__pycache__/
+-rw-r--r--   0 andreybondar   (501) staff       (20)      160 2018-07-04 08:13:03.000000 tortoise-orm-0.9.4/tortoise/contrib/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)      117 2018-07-06 15:46:58.000000 tortoise-orm-0.9.4/tortoise/contrib/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)      160 2018-07-06 16:30:05.000000 tortoise-orm-0.9.4/tortoise/contrib/__pycache__/__init__.cpython-35.pyc
+-rw-r--r--   0 andreybondar   (501) staff       (20)     1019 2018-07-17 08:16:01.000000 tortoise-orm-0.9.4/tortoise/utils.py
+-rw-r--r--   0 andreybondar   (501) staff       (20)    28563 2018-07-17 08:16:01.000000 tortoise-orm-0.9.4/tortoise/queryset.py
+-rw-r--r--   0 andreybondar   (501) staff       (20)     1384 2018-07-17 08:16:01.000000 tortoise-orm-0.9.4/tortoise/exceptions.py
+-rw-r--r--   0 andreybondar   (501) staff       (20)     5925 2018-07-10 09:39:40.000000 tortoise-orm-0.9.4/tortoise/query_utils.py
```

### Comparing `tortoise-orm-0.9.2/PKG-INFO` & `tortoise-orm-0.9.4/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 Metadata-Version: 1.1
 Name: tortoise-orm
-Version: 0.9.2
+Version: 0.9.4
 Summary: Easy async ORM for python, built with relations in mind
 Home-page: https://github.com/Zeliboba5/tortoise-orm
 Author: Andrey Bondar
 Author-email: andrey@bondar.ru
 License: Apache License Version 2.0
 Description: ========
         Tortoise
         ========
         
+        .. image:: https://travis-ci.com/Zeliboba5/tortoise-orm.svg?branch=master
+            :target: https://travis-ci.com/Zeliboba5/tortoise-orm
+        .. image:: https://coveralls.io/repos/github/Zeliboba5/tortoise-orm/badge.svg?branch=master
+            :target: https://coveralls.io/github/Zeliboba5/tortoise-orm?branch=master
+        
         Introduction
         ============
         Tortoise is easy-to-use asyncio ORM inspired by Django.
         
         It is built with relations between models in mind and provides simple api for it, that gives you potential for building web services with easy abstractions.
         
         You can find docs at `readthedocs <http://tortoise-orm.readthedocs.io/en/latest/>`_
```

### Comparing `tortoise-orm-0.9.2/tortoise_orm.egg-info/PKG-INFO` & `tortoise-orm-0.9.4/tortoise_orm.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 Metadata-Version: 1.1
 Name: tortoise-orm
-Version: 0.9.2
+Version: 0.9.4
 Summary: Easy async ORM for python, built with relations in mind
 Home-page: https://github.com/Zeliboba5/tortoise-orm
 Author: Andrey Bondar
 Author-email: andrey@bondar.ru
 License: Apache License Version 2.0
 Description: ========
         Tortoise
         ========
         
+        .. image:: https://travis-ci.com/Zeliboba5/tortoise-orm.svg?branch=master
+            :target: https://travis-ci.com/Zeliboba5/tortoise-orm
+        .. image:: https://coveralls.io/repos/github/Zeliboba5/tortoise-orm/badge.svg?branch=master
+            :target: https://coveralls.io/github/Zeliboba5/tortoise-orm?branch=master
+        
         Introduction
         ============
         Tortoise is easy-to-use asyncio ORM inspired by Django.
         
         It is built with relations between models in mind and provides simple api for it, that gives you potential for building web services with easy abstractions.
         
         You can find docs at `readthedocs <http://tortoise-orm.readthedocs.io/en/latest/>`_
```

### Comparing `tortoise-orm-0.9.2/setup.py` & `tortoise-orm-0.9.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf8
 import re
 import sys
 
-from setuptools import setup
+from setuptools import find_packages, setup
 
 if sys.version_info < (3, 5, 3):
     raise RuntimeError("tortoise requires Python 3.5.3+")
 
 
 def version():
     verstrline = open('tortoise/__init__.py', "rt").read()
@@ -32,15 +32,18 @@
     author="Andrey Bondar",
     author_email="andrey@bondar.ru",
 
     # License
     license='Apache License Version 2.0',
 
     # Packages
-    packages=["tortoise"],
+    packages=find_packages(
+        include=['tortoise*'],
+        exclude=['tortoise.tests']
+    ),
 
     # Include additional files into the package
     include_package_data=True,
 
     # Details
     url="https://github.com/Zeliboba5/tortoise-orm",
     description="Easy async ORM for python, built with relations in mind",
```

### Comparing `tortoise-orm-0.9.2/README.rst` & `tortoise-orm-0.9.4/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 ========
 Tortoise
 ========
 
+.. image:: https://travis-ci.com/Zeliboba5/tortoise-orm.svg?branch=master
+    :target: https://travis-ci.com/Zeliboba5/tortoise-orm
+.. image:: https://coveralls.io/repos/github/Zeliboba5/tortoise-orm/badge.svg?branch=master
+    :target: https://coveralls.io/github/Zeliboba5/tortoise-orm?branch=master
+
 Introduction
 ============
 Tortoise is easy-to-use asyncio ORM inspired by Django.
 
 It is built with relations between models in mind and provides simple api for it, that gives you potential for building web services with easy abstractions.
 
 You can find docs at `readthedocs <http://tortoise-orm.readthedocs.io/en/latest/>`_
```

### Comparing `tortoise-orm-0.9.2/tortoise/pylint/__pycache__/__init__.cpython-36.pyc` & `tortoise-orm-0.9.4/tortoise/pylint/__pycache__/__init__.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `tortoise-orm-0.9.2/tortoise/aggregation.py` & `tortoise-orm-0.9.4/tortoise/aggregation.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 from pypika.functions import Avg as PypikaAvg
 from pypika.functions import Count as PypikaCount
 from pypika.functions import Max as PypikaMax
 from pypika.functions import Min as PypikaMin
 from pypika.functions import Sum as PypikaSum
 from pypika.terms import AggregateFunction
 
+from tortoise.exceptions import ConfigurationError
+
 
 class Aggregate:
     aggregation_func = AggregateFunction
 
     def __init__(self, field):
         self.field = field
 
@@ -29,15 +31,16 @@
                 )
             else:
                 aggregation['field'] = self.aggregation_func(
                     getattr(Table(model._meta.table), field_split[0])
                 )
             return aggregation
         else:
-            assert field_split[0] in model._meta.fetch_fields
+            if field_split[0] not in model._meta.fetch_fields:
+                raise ConfigurationError('{} not resolvable'.format(field))
             related_field = model._meta.fields_map[field_split[0]]
             join = (Table(model._meta.table), field_split[0], related_field)
             aggregation = self._resolve_field_for_model(
                 '__'.join(field_split[1:]), related_field.type
             )
             aggregation['joins'].append(join)
             return aggregation
```

### Comparing `tortoise-orm-0.9.2/tortoise/.DS_Store` & `tortoise-orm-0.9.4/tortoise/.DS_Store`

 * *Files identical despite different names*

### Comparing `tortoise-orm-0.9.2/tortoise/models.py` & `tortoise-orm-0.9.4/tortoise/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import operator
+from typing import Dict, Optional, Set  # noqa
 
 from pypika import Table, functions
 from pypika.enums import SqlTypes
 
 from tortoise import fields
+from tortoise.backends.base.client import BaseDBAsyncClient  # noqa
+from tortoise.exceptions import ConfigurationError, OperationalError
 from tortoise.fields import ManyToManyRelationManager, RelationQueryContainer
 from tortoise.queryset import QuerySet
 
 
 def is_in(field, value):
     return field.isin(value)
 
@@ -124,15 +127,15 @@
             'table': Table(field.type._meta.table),
             'value_encoder': list,
         },
     }
     return filters
 
 
-def get_filters_for_field(field_name: str, field: fields.Field, source_field: str):
+def get_filters_for_field(field_name: str, field: Optional[fields.Field], source_field: str):
     if isinstance(field, fields.ManyToManyField):
         return get_m2m_filters(field_name, field)
     filters = {
         field_name: {
             'field': source_field,
             'operator': operator.eq,
         },
@@ -199,39 +202,42 @@
             'operator': insensitive_ends_with,
         },
     }
     return filters
 
 
 class MetaInfo:
+    __slots__ = ('abstract', 'table', 'app', 'fields', 'db_fields', 'm2m_fields', 'fk_fields',
+                 'backward_fk_fields', 'fetch_fields', 'fields_db_projection',
+                 'fields_db_projection_reverse', 'filters', 'fields_map', 'db')
+
     def __init__(self, meta):
-        self.abstract = getattr(meta, 'abstract', False)
-        self.table = getattr(meta, 'table', None)
-        self.app = getattr(meta, 'app', 'models')
-        self.fields = set()
-        self.db_fields = set()
-        self.m2m_fields = set()
-        self.fk_fields = set()
-        self.backward_fk_fields = set()
-        self.fetch_fields = set()
-        self.fields_db_projection = {}
-        self.fields_db_projection_reverse = {}
-        self.filters = {}
-        self.fields_map = {}
-        self.db = None
+        self.abstract = getattr(meta, 'abstract', False)  # type: bool
+        self.table = getattr(meta, 'table', None)  # type: Optional[Table]
+        self.app = getattr(meta, 'app', 'models')  # type: str
+        self.fields = set()  # type: Set[str]
+        self.db_fields = set()  # type: Set[str]
+        self.m2m_fields = set()  # type: Set[str]
+        self.fk_fields = set()  # type: Set[str]
+        self.backward_fk_fields = set()  # type: Set[str]
+        self.fetch_fields = set()  # type: Set[str]
+        self.fields_db_projection = {}  # type: Dict[str,str]
+        self.fields_db_projection_reverse = {}  # type: Dict[str,str]
+        self.filters = {}  # type: Dict[str, Dict[str, dict]]
+        self.fields_map = {}  # type: Dict[str, fields.Field]
+        self.db = None  # type: Optional[BaseDBAsyncClient]
 
 
 class ModelMeta(type):
     def __new__(mcs, name, bases, attrs, *args, **kwargs):
-        fields_db_projection = {}
-        fields_map = {}
-        filters = {}
-        fk_fields = set()
-        m2m_fields = set()
-        meta = MetaInfo(attrs.get('Meta'))
+        fields_db_projection = {}  # type: Dict[str,str]
+        fields_map = {}  # type: Dict[str, fields.Field]
+        filters = {}  # type: Dict[str, Dict[str, dict]]
+        fk_fields = set()  # type: Set[str]
+        m2m_fields = set()  # type: Set[str]
 
         for key, value in attrs.items():
             if isinstance(value, fields.Field):
                 fields_map[key] = value
                 if isinstance(value, fields.ForeignKeyField):
                     key_field = '{}_id'.format(key)
                     value.source_field = key_field
@@ -256,36 +262,42 @@
                     filters.update(
                         get_filters_for_field(
                             field_name=key,
                             field=fields_map[key],
                             source_field=fields_db_projection[key]
                         )
                     )
-        new_class = super().__new__(mcs, name, bases, attrs)
 
-        new_class._meta = meta
-        new_class._meta.fields_map = fields_map
-        new_class._meta.fields_db_projection = fields_db_projection
-        new_class._meta.fields_db_projection_reverse = {
+        attrs['_meta'] = meta = MetaInfo(attrs.get('Meta'))
+
+        if 'id' not in attrs:
+            attrs['id'] = None
+
+        meta = meta
+        meta.fields_map = fields_map
+        meta.fields_db_projection = fields_db_projection
+        meta.fields_db_projection_reverse = {
             value: key
             for key, value in fields_db_projection.items()
         }
-        new_class._meta.fields = set(fields_map.keys())
-        new_class._meta.db_fields = set(fields_db_projection.values())
-        new_class._meta.filters = filters
-        new_class._meta.fk_fields = fk_fields
-        new_class._meta.backward_fk_fields = set()
-        new_class._meta.m2m_fields = m2m_fields
-        new_class._meta.fetch_fields = fk_fields | m2m_fields
-        new_class._meta.db = None
+        meta.fields = set(fields_map.keys())
+        meta.db_fields = set(fields_db_projection.values())
+        meta.filters = filters
+        meta.fk_fields = fk_fields
+        meta.backward_fk_fields = set()
+        meta.m2m_fields = m2m_fields
+        meta.fetch_fields = fk_fields | m2m_fields
+        meta.db = None
         if not fields_map:
-            new_class._meta.abstract = True
-        if not new_class._meta.abstract:
+            meta.abstract = True
+
+        new_class = super().__new__(mcs, name, bases, attrs)
+        if not meta.abstract:
             from tortoise import Tortoise
-            Tortoise.register_model(new_class._meta.app, new_class.__name__, new_class)
+            Tortoise.register_model(meta.app, new_class.__name__, new_class)
         return new_class
 
 
 class Model(metaclass=ModelMeta):
     def __init__(self, *args, **kwargs):
         is_new = not bool(kwargs.get('id'))
 
@@ -301,26 +313,26 @@
                 setattr(self, key, field.default)
             else:
                 setattr(self, key, None)
 
         passed_fields = set(kwargs.keys())
         for key, value in kwargs.items():
             if key in self._meta.fk_fields:
-                assert hasattr(value, 'id') and value.id, (
-                    'You should first call .save() on {} before referring to it'.format(value)
-                )
+                if hasattr(value, 'id') and not value.id:
+                    raise OperationalError(
+                        'You should first call .save() on {} before referring to it'.format(value))
                 relation_field = '{}_id'.format(key)
                 setattr(self, relation_field, value.id)
                 passed_fields.add(relation_field)
             elif key in self._meta.backward_fk_fields:
-                raise AssertionError(
+                raise ConfigurationError(
                     'You can\'t set backward relations through init, change related model instead'
                 )
             elif key in self._meta.m2m_fields:
-                raise AssertionError(
+                raise ConfigurationError(
                     'You can\'t set m2m relations through init, use m2m_manager instead'
                 )
             elif key in self._meta.fields:
                 field_object = self._meta.fields_map[key]
                 if value is None and not field_object.null:
                     raise ValueError('{} is non nullable field, but null was passed'.format(key))
                 setattr(self, key, field_object.to_python_value(value))
@@ -375,15 +387,15 @@
     def __str__(self):
         return self.__class__.__name__
 
     def __repr__(self):
         return '<{}: {}>'.format(self.__class__.__name__, self.__str__())
 
     def __hash__(self):
-        if not hasattr(self.id) or not self.id:
+        if self.id:
             raise TypeError('Model instances without id are unhashable')
         return hash(self.id)
 
     def __eq__(self, other):
         # pylint: disable=C0123
         if type(self) == type(other) and self.id == other.id:
             return True
@@ -414,16 +426,15 @@
 
     @classmethod
     def all(cls):
         return QuerySet(cls)
 
     @classmethod
     def get(cls, *args, **kwargs):
-        # TODO: Raise exception if no result
-        return QuerySet(cls).filter(*args, **kwargs).first()
+        return QuerySet(cls).get(*args, **kwargs)
 
     @classmethod
     async def fetch_for_list(cls, instance_list, *args, using_db=None):
         db = using_db if using_db else cls._meta.db
         await db.executor_class(
             model=cls,
             db=db,
```

### Comparing `tortoise-orm-0.9.2/tortoise/fields.py` & `tortoise-orm-0.9.4/tortoise/backends/base/executor.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,326 +1,221 @@
 import datetime
-import functools
-import json
-from decimal import Decimal
+from typing import Dict  # noqa
 
 from pypika import Table
 
-import ciso8601
-from tortoise.exceptions import ConfigurationError, NoValuesFetched
-from tortoise.utils import AsyncIteratorWrapper
-
-CASCADE = 'CASCADE'
-RESTRICT = 'RESTRICT'
-SET_NULL = 'SET NULL'
-SET_DEFAULT = 'SET DEFAULT'
-
-# Doing this we can replace json dumps/loads with different implementations
-JSON_DUMPS = functools.partial(
-    json.dumps,
-    separators=(',', ':')
-)
-JSON_LOADS = json.loads
-
-
-class Field:
-    def __init__(
-        self,
-        type=None,
-        source_field=None,
-        generated=False,
-        pk=False,
-        null=False,
-        default=None,
-        unique=False,
-        **kwargs
-    ):
-        self.type = type
-        self.source_field = source_field
-        self.generated = generated
-        self.pk = pk
-        self.default = default
-        self.null = null
-        self.unique = unique
-
-    def to_db_value(self, value):
-        return value
-
-    def to_python_value(self, value):
-        if value is None or isinstance(value, self.type):
-            return value
-        return self.type(value)
-
-
-class IntField(Field):
-    def __init__(self, source_field=None, pk=False, **kwargs):
-        kwargs['generated'] = bool(kwargs.get('generated')) | pk
-        super().__init__(int, source_field, **kwargs)
-        self.reference = kwargs.get('reference')
-        self.pk = pk
-
-
-class SmallIntField(Field):
-    def __init__(self, **kwargs):
-        super().__init__(int, **kwargs)
-
-
-class CharField(Field):
-    def __init__(self, max_length=0, **kwargs):
-        if int(max_length) < 1:
-            raise ConfigurationError('max_digits must be >= 1')
-        self.max_length = int(max_length)
-        super().__init__(str, **kwargs)
-
-
-class TextField(Field):
-    def __init__(self, **kwargs):
-        super().__init__(str, **kwargs)
-
-
-class BooleanField(Field):
-    def __init__(self, **kwargs):
-        super().__init__(bool, **kwargs)
-
-
-class DecimalField(Field):
-    def __init__(self, max_digits=0, decimal_places=-1, **kwargs):
-        if int(max_digits) < 1:
-            raise ConfigurationError('max_digits must be >= 1')
-        if int(decimal_places) < 0:
-            raise ConfigurationError('decimal_places must be >= 0')
-        super().__init__(Decimal, **kwargs)
-        self.max_digits = max_digits
-        self.decimal_places = decimal_places
-
-
-class DatetimeField(Field):
-    def __init__(self, auto_now=False, auto_now_add=False, **kwargs):
-        if auto_now_add and auto_now:
-            raise ConfigurationError('You can choose only auto_now or auto_now_add')
-        auto_now_add = auto_now_add | auto_now
-        kwargs['generated'] = bool(kwargs.get('generated')) | auto_now_add
-        super().__init__(datetime.datetime, **kwargs)
-        self.auto_now = auto_now
-        self.auto_now_add = auto_now_add
-
-    def to_python_value(self, value):
-        if value is None or isinstance(value, self.type):
-            return value
-        return ciso8601.parse_datetime(value)
-
-
-class DateField(Field):
-    def __init__(self, **kwargs):
-        super().__init__(datetime.date, **kwargs)
-
-    def to_python_value(self, value):
-        if value is None or isinstance(value, self.type):
-            return value
-        return ciso8601.parse_datetime(value).date()
-
-
-class FloatField(Field):
-    def __init__(self, **kwargs):
-        super().__init__(float, **kwargs)
-
-
-class JSONField(Field):
-    def __init__(self, encoder=JSON_DUMPS, decoder=JSON_LOADS, **kwargs):
-        super().__init__((dict, list), **kwargs)
-        self.encoder = encoder
-        self.decoder = decoder
-
-    def to_db_value(self, value):
-        if value is None:
-            return value
-        return self.encoder(value)
-
-    def to_python_value(self, value):
-        if value is None or isinstance(value, self.type):
-            return value
-        return self.decoder(value)
-
-
-class ForeignKeyField(Field):
-    def __init__(self, model_name, related_name=None, on_delete=CASCADE, **kwargs):
-        super().__init__(**kwargs)
-        assert isinstance(model_name, str) and len(model_name.split(".")) == 2, \
-            'Foreign key accepts model name in format "app.Model"'
-        self.model_name = model_name
-        self.related_name = related_name
-        assert on_delete in {CASCADE, RESTRICT, SET_NULL}
-        assert ((on_delete == SET_NULL) == bool(kwargs.get('null'))) or on_delete != SET_NULL
-        self.on_delete = on_delete
-
-
-class ManyToManyField(Field):
-    def __init__(
-        self,
-        model_name,
-        through=None,
-        forward_key=None,
-        backward_key=None,
-        related_name=None,
-        **kwargs
-    ):
-        super().__init__(**kwargs)
-        assert len(model_name.split(".")
-                   ) == 2, 'Foreign key accepts model name in format "app.Model"'
-        self.model_name = model_name
-        self.related_name = related_name
-        self.forward_key = forward_key if forward_key else '{}_id'.format(
-            model_name.split(".")[1].lower()
-        )
-        self.backward_key = backward_key
-        self.through = through
-        self._generated = False
-
+from tortoise import fields
+from tortoise.exceptions import OperationalError
 
-class BackwardFKRelation:
-    def __init__(self, type, relation_field, **kwargs):
-        self.type = type
-        self.relation_field = relation_field
 
-
-class RelationQueryContainer:
-    def __init__(self, model, relation_field, instance, is_new):
+class BaseExecutor:
+    def __init__(self, model, db=None, prefetch_map=None, prefetch_queries=None):
         self.model = model
-        self.relation_field = relation_field
-        self.instance = instance
-        self._fetched = is_new
-        self._custom_query = False
-        self.related_objects = []
-
-    @property
-    def _query(self):
-        assert self.instance.id, (
-            "This objects hasn't been instanced, call .save() before calling related queries"
-        )
-        return self.model.filter(**{self.relation_field: self.instance.id})
+        self.db = db
+        self.connection = None
+        self.prefetch_map = prefetch_map if prefetch_map else {}
+        self._prefetch_queries = prefetch_queries if prefetch_queries else {}
+
+    async def execute_select(self, query, custom_fields=None):
+        self.connection = await self.db.get_single_connection()
+        raw_results = await self.connection.execute_query(str(query))
+        instance_list = []
+        for row in raw_results:
+            instance = self.model(**row)
+            if custom_fields:
+                for field in custom_fields:
+                    setattr(instance, field, row[field])
+            instance_list.append(instance)
+        await self._execute_prefetch_queries(instance_list)
+        await self.db.release_single_connection(self.connection)
+        self.connection = None
+        return instance_list
+
+    def _prepare_insert_columns(self):
+        regular_columns = []
+        python_generated_column_pairs = []
+        now = datetime.datetime.utcnow()
+        for column in self.model._meta.fields_db_projection.keys():
+            field_object = self.model._meta.fields_map[column]
+            if isinstance(field_object, fields.DatetimeField) and field_object.auto_now_add:
+                python_generated_column_pairs.append((column, now))
+            elif field_object.generated:
+                continue
+            else:
+                regular_columns.append(column)
+        return regular_columns, python_generated_column_pairs
+
+    def _field_to_db(self, field_object, attr):
+        return field_object.to_db_value(attr)
+
+    def _get_prepared_value(self, instance, column):
+        return self._field_to_db(self.model._meta.fields_map[column], getattr(instance, column))
+
+    def _prepare_insert_values(self, instance, regular_columns, generated_column_pairs):
+        values = [self._get_prepared_value(instance, column) for column in regular_columns]
+        result_columns = [self.model._meta.fields_db_projection[c] for c in regular_columns]
+        for column, value in generated_column_pairs:
+            result_columns.append(self.model._meta.fields_db_projection[column])
+            values.append(value)
+            setattr(instance, column, value)
+        return result_columns, values
+
+    async def execute_insert(self, instance):
+        # Insert should implement returning new id to saved object
+        # Each db has it's own methods for it, so each implementation should
+        # go to descendant executors
+        raise NotImplementedError()  # pragma: nocoverage
+
+    async def execute_update(self, instance):
+        self.connection = await self.db.get_single_connection()
+        table = Table(self.model._meta.table)
+        query = self.connection.query_class.update(table)
+        for field, db_field in self.model._meta.fields_db_projection.items():
+            field_object = self.model._meta.fields_map[field]
+            if isinstance(field_object, fields.DatetimeField) and field_object.auto_now:
+                now = datetime.datetime.utcnow()
+                query = query.set(db_field, now)
+                setattr(instance, field, now)
+            elif field_object.generated:
+                continue
+            else:
+                query = query.set(
+                    db_field,
+                    self._field_to_db(field_object, getattr(instance, field))
+                )
+        query = query.where(table.id == instance.id)
+        await self.connection.execute_query(str(query))
+        await self.db.release_single_connection(self.connection)
+        self.connection = None
+        return instance
+
+    async def execute_delete(self, instance):
+        table = Table(self.model._meta.table)
+        query = self.db.query_class.from_(table).where(table.id == instance.id).delete()
+        await self.db.execute_query(str(query))
+        return instance
+
+    async def _prefetch_reverse_relation(self, instance_list, field, related_query):
+        instance_id_set = set()
+        for instance in instance_list:
+            instance_id_set.add(instance.id)
+        backward_relation_manager = getattr(self.model, field)
+        relation_field = backward_relation_manager.relation_field
 
-    def __contains__(self, item):
-        if not self._fetched:
-            raise NoValuesFetched(
-                'No values were fetched for this relation, first use .fetch_related()'
-            )
-        return item in self.related_objects
-
-    def __iter__(self):
-        if not self._fetched:
-            raise NoValuesFetched(
-                'No values were fetched for this relation, first use .fetch_related()'
-            )
-        return self.related_objects.__iter__()
-
-    def __len__(self):
-        if not self._fetched:
-            raise NoValuesFetched(
-                'No values were fetched for this relation, first use .fetch_related()'
-            )
-        return len(self.related_objects)
-
-    def __bool__(self):
-        if not self._fetched:
-            raise NoValuesFetched(
-                'No values were fetched for this relation, first use .fetch_related()'
-            )
-        return bool(self.related_objects)
-
-    def __getitem__(self, item):
-        if not self._fetched:
-            raise NoValuesFetched(
-                'No values were fetched for this relation, first use .fetch_related()'
-            )
-        return self.related_objects[item]
-
-    async def __aiter__(self):
-        self.related_objects = await self._query
-        self._fetched = True
-        return AsyncIteratorWrapper(self.related_objects)
-
-    def filter(self, *args, **kwargs):
-        return self._query.filter(*args, **kwargs)
-
-    def all(self):
-        return self
-
-    def order_by(self, *args, **kwargs):
-        return self._query.order_by(*args, **kwargs)
-
-    def limit(self, *args, **kwargs):
-        return self._query.limit(*args, **kwargs)
-
-    def offset(self, *args, **kwargs):
-        return self._query.offset(*args, **kwargs)
-
-    def distinct(self, *args, **kwargs):
-        return self._query.distinct(*args, **kwargs)
-
-    def _set_result_for_query(self, sequence):
-        for item in sequence:
-            assert isinstance(item, self.model)
-        self._fetched = True
-        self.related_objects = sequence
-
-
-class ManyToManyRelationManager(RelationQueryContainer):
-    def __init__(self, model, instance, m2m_field, is_new):
-        super().__init__(model, m2m_field.related_name, instance, is_new)
-        self.field = m2m_field
-        self.model = m2m_field.type
-        self.instance = instance
-        self._db = self.model._meta.db
-
-    async def add(self, *instances, using_db=None):
-        if not instances:
-            return
-        db = using_db if using_db else self._db
-        through_table = Table(self.field.through)
-        select_query = db.query_class.from_(through_table).where(
-            getattr(through_table, self.field.backward_key) == self.instance.id
-        ).select(self.field.backward_key, self.field.forward_key)
-        query = db.query_class.into(through_table).columns(
-            getattr(through_table, self.field.forward_key),
-            getattr(through_table, self.field.backward_key),
+        related_object_list = await related_query.filter(
+            **{'{}__in'.format(relation_field): list(instance_id_set)}
         )
-        criterion = getattr(through_table, self.field.forward_key) == instances[0].id
-        for instance_to_add in instances[1:]:
-            criterion |= getattr(through_table, self.field.forward_key) == instance_to_add.id
-        select_query = select_query.where(criterion)
-
-        already_existing_relations_raw = await db.execute_query(str(select_query))
-        already_existing_relations = set((r[self.field.backward_key], r[self.field.forward_key])
-                                         for r in already_existing_relations_raw)
-
-        insert_is_required = False
-        for instance_to_add in instances:
-            if (self.instance.id, instance_to_add.id) in already_existing_relations:
-                continue
-            query = query.insert(instance_to_add.id, self.instance.id)
-            insert_is_required = True
-        if insert_is_required:
-            await db.execute_query(str(query))
-
-    async def clear(self, using_db=None):
-        db = using_db if using_db else self._db
-        through_table = Table(self.field.through)
-        query = db.query_class.from_(through_table).where(
-            getattr(through_table, self.field.backward_key) == self.instance.id
-        ).delete()
-        await db.execute_query(str(query))
-
-    async def remove(self, *instances, using_db=None):
-        db = using_db if using_db else self._db
-        assert instances
-        through_table = Table(self.field.through)
-        condition = (
-            getattr(through_table, self.field.forward_key) == instances[0].id
-            & getattr(through_table, self.field.backward_key) == self.instance.id
+
+        related_object_map = {}  # type: Dict[str, list]
+        for entry in related_object_list:
+            object_id = getattr(entry, relation_field)
+            if object_id in related_object_map.keys():
+                related_object_map[object_id].append(entry)
+            else:
+                related_object_map[object_id] = [entry]
+        for instance in instance_list:
+            relation_container = getattr(instance, field)
+            relation_container._set_result_for_query(related_object_map.get(instance.id, []))
+        return instance_list
+
+    async def _prefetch_m2m_relation(self, instance_list, field, related_query):
+        instance_id_set = set()
+        for instance in instance_list:
+            instance_id_set.add(instance.id)
+
+        field_object = self.model._meta.fields_map[field]
+
+        through_table = Table(field_object.through)
+
+        subquery = self.connection.query_class.from_(through_table).select(
+            getattr(through_table, field_object.backward_key).as_('_backward_relation_key'),
+            getattr(through_table, field_object.forward_key).as_('_forward_relation_key')
+        ).where(getattr(through_table, field_object.backward_key).isin(instance_id_set))
+
+        related_query_table = Table(related_query.model._meta.table)
+        query = related_query.query.join(subquery).on(
+            subquery._forward_relation_key == related_query_table.id
+        ).select(
+            subquery._backward_relation_key.as_('_backward_relation_key'),
+            *[getattr(related_query_table, field).as_(field) for field in related_query.fields]
         )
-        for instance_to_remove in instances[1:]:
-            condition |= (
-                getattr(through_table, self.field.forward_key) == instance_to_remove.id
-                & getattr(through_table, self.field.backward_key) == self.instance.id
-            )
-        query = db.query_class.from_(through_table).where(condition).delete()
-        await db.execute_query(str(query))
+        raw_results = await self.connection.execute_query(str(query))
+        relations = {(e['_backward_relation_key'], e['id']) for e in raw_results}
+        related_object_list = [related_query.model(**e) for e in raw_results]
+        await self.__class__(
+            model=related_query.model,
+            db=self.connection,
+            prefetch_map=related_query._prefetch_map,
+        ).fetch_for_list(related_object_list)
+        related_object_map = {e.id: e for e in related_object_list}
+        relation_map = {}  # type: Dict[str, list]
+
+        for object_id, related_object_id in relations:
+            if object_id not in relation_map:
+                relation_map[object_id] = []
+            relation_map[object_id].append(related_object_map[related_object_id])
+
+        for instance in instance_list:
+            relation_container = getattr(instance, field)
+            relation_container._set_result_for_query(relation_map.get(instance.id, []))
+        return instance_list
+
+    async def _prefetch_direct_relation(self, instance_list, field, related_query):
+        related_objects_for_fetch = set()
+        relation_key_field = '{}_id'.format(field)
+        for instance in instance_list:
+            if getattr(instance, relation_key_field):
+                related_objects_for_fetch.add(getattr(instance, relation_key_field))
+        if related_objects_for_fetch:
+            related_object_list = await related_query.filter(id__in=list(related_objects_for_fetch))
+            related_object_map = {obj.id: obj for obj in related_object_list}
+            for instance in instance_list:
+                setattr(
+                    instance, field, related_object_map.get(getattr(instance, relation_key_field))
+                )
+        return instance_list
+
+    def _make_prefetch_queries(self):
+        for field, forwarded_prefetches in self.prefetch_map.items():
+            if field in self._prefetch_queries:
+                related_query = self._prefetch_queries.get(field)
+            else:
+                related_model_field = self.model._meta.fields_map.get(field)
+                related_model = related_model_field.type
+                related_query = related_model.all().using_db(self.connection)
+            if forwarded_prefetches:
+                related_query = related_query.prefetch_related(*forwarded_prefetches)
+            self._prefetch_queries[field] = related_query
+
+    async def _do_prefetch(self, instance_id_list, field, related_query):
+        if isinstance(getattr(self.model, field), fields.BackwardFKRelation):
+            return await self._prefetch_reverse_relation(instance_id_list, field, related_query)
+        elif isinstance(getattr(self.model, field), fields.ManyToManyField):
+            return await self._prefetch_m2m_relation(instance_id_list, field, related_query)
+        else:
+            return await self._prefetch_direct_relation(instance_id_list, field, related_query)
+
+    async def _execute_prefetch_queries(self, instance_list):
+        if instance_list and (self.prefetch_map or self._prefetch_queries):
+            self._make_prefetch_queries()
+            for field, related_query in self._prefetch_queries.items():
+                await self._do_prefetch(instance_list, field, related_query)
+        return instance_list
+
+    async def fetch_for_list(self, instance_list, *args):
+        self.connection = await self.db.get_single_connection()
+        self.prefetch_map = {}
+        for relation in args:
+            relation_split = relation.split('__')
+            first_level_field = relation_split[0]
+            if first_level_field not in self.model._meta.fetch_fields:
+                raise OperationalError('relation {} for {} not found'.format(
+                    first_level_field, self.model._meta.table))
+            if first_level_field not in self.prefetch_map.keys():
+                self.prefetch_map[first_level_field] = set()
+            forwarded_prefetch = '__'.join(relation_split[1:])
+            if forwarded_prefetch:
+                self.prefetch_map[first_level_field].add(forwarded_prefetch)
+        await self._execute_prefetch_queries(instance_list)
+        await self.db.release_single_connection(self.connection)
+        self.connection = None
+        return instance_list
```

### Comparing `tortoise-orm-0.9.2/tortoise/backends/.DS_Store` & `tortoise-orm-0.9.4/tortoise/backends/.DS_Store`

 * *Files identical despite different names*

### Comparing `tortoise-orm-0.9.2/tortoise/backends/asyncpg/.DS_Store` & `tortoise-orm-0.9.4/tortoise/backends/asyncpg/.DS_Store`

 * *Files identical despite different names*

### Comparing `tortoise-orm-0.9.2/tortoise/backends/asyncpg/client.py` & `tortoise-orm-0.9.4/tortoise/backends/asyncpg/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import asyncpg
 from pypika import PostgreSQLQuery
 
 from tortoise.backends.asyncpg.executor import AsyncpgExecutor
 from tortoise.backends.asyncpg.schema_generator import AsyncpgSchemaGenerator
 from tortoise.backends.base.client import (BaseDBAsyncClient, ConnectionWrapper,
                                            SingleConnectionWrapper)
-from tortoise.exceptions import IntegrityError, OperationalError
+from tortoise.exceptions import ConfigurationError, IntegrityError, OperationalError
 
 
 class AsyncpgDBClient(BaseDBAsyncClient):
     DSN_TEMPLATE = 'postgres://{user}:{password}@{host}:{port}/{database}'
     query_class = PostgreSQLQuery
     executor_class = AsyncpgExecutor
     schema_generator = AsyncpgSchemaGenerator
@@ -127,15 +127,16 @@
         async with self.acquire_connection() as connection:
             self.log.debug(script)
             await connection.execute(script)
 
 
 class TransactionWrapper(AsyncpgDBClient):
     def __init__(self, pool=None, connection=None):
-        assert bool(pool) != bool(connection), 'You must pass either connection or pool'
+        if pool and connection:
+            raise ConfigurationError('You must pass either connection or pool')
         self._connection = connection
         self.log = logging.getLogger('db_client')
         self._pool = pool
         self.single_connection = True
         self._single_connection_class = type(
             'SingleConnectionWrapper', (SingleConnectionWrapper, self.__class__), {}
         )
```

### Comparing `tortoise-orm-0.9.2/tortoise/backends/asyncpg/__pycache__/client.cpython-36.pyc` & `tortoise-orm-0.9.4/tortoise/backends/asyncpg/__pycache__/client.cpython-37.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.6 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 10% similar despite different names*

```diff
@@ -1,394 +1,395 @@
-00000000: 330d 0d0a 5576 3f5b a719 0000 e300 0000  3...Uv?[........
-00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 7c00 0000 6400 6401 6c00 5a00 6400  .s|...d.d.l.Z.d.
-00000030: 6401 6c01 5a01 6400 6402 6c02 6d03 5a03  d.l.Z.d.d.l.m.Z.
-00000040: 0100 6400 6403 6c04 6d05 5a05 0100 6400  ..d.d.l.m.Z...d.
-00000050: 6404 6c06 6d07 5a07 0100 6400 6405 6c08  d.l.m.Z...d.d.l.
-00000060: 6d09 5a09 6d0a 5a0a 6d0b 5a0b 0100 6400  m.Z.m.Z.m.Z...d.
-00000070: 6406 6c0c 6d0d 5a0d 6d0e 5a0e 0100 4700  d.l.m.Z.m.Z...G.
-00000080: 6407 6408 8400 6408 6509 8303 5a0f 4700  d.d...d.e...Z.G.
-00000090: 6409 640a 8400 640a 650f 8303 5a10 6401  d.d...d.e...Z.d.
-000000a0: 5300 290b e900 0000 004e 2901 da0f 506f  S.)......N)...Po
-000000b0: 7374 6772 6553 514c 5175 6572 7929 01da  stgreSQLQuery)..
-000000c0: 0f41 7379 6e63 7067 4578 6563 7574 6f72  .AsyncpgExecutor
-000000d0: 2901 da16 4173 796e 6370 6753 6368 656d  )...AsyncpgSchem
-000000e0: 6147 656e 6572 6174 6f72 2903 da11 4261  aGenerator)...Ba
-000000f0: 7365 4442 4173 796e 6343 6c69 656e 74da  seDBAsyncClient.
-00000100: 1143 6f6e 6e65 6374 696f 6e57 7261 7070  .ConnectionWrapp
-00000110: 6572 da17 5369 6e67 6c65 436f 6e6e 6563  er..SingleConnec
-00000120: 7469 6f6e 5772 6170 7065 7229 02da 0e49  tionWrapper)...I
-00000130: 6e74 6567 7269 7479 4572 726f 72da 104f  ntegrityError..O
-00000140: 7065 7261 7469 6f6e 616c 4572 726f 7263  perationalErrorc
-00000150: 0000 0000 0000 0000 0000 0000 0300 0000  ................
-00000160: 0000 0000 737c 0000 0065 005a 0164 005a  ....s|...e.Z.d.Z
-00000170: 0264 015a 0365 045a 0565 065a 0765 085a  .d.Z.e.Z.e.Z.e.Z
-00000180: 0987 0066 0164 0264 0384 085a 0a64 0464  ...f.d.d...Z.d.d
-00000190: 0584 005a 0b64 0664 0784 005a 0c64 0864  ...Z.d.d...Z.d.d
-000001a0: 0984 005a 0d64 0a64 0b84 005a 0e64 0c64  ...Z.d.d...Z.d.d
-000001b0: 0d84 005a 0f64 0e64 0f84 005a 1064 1064  ...Z.d.d...Z.d.d
-000001c0: 1184 005a 1164 1264 1384 005a 1264 1464  ...Z.d.d...Z.d.d
-000001d0: 1584 005a 1364 1664 1784 005a 1487 0004  ...Z.d.d...Z....
-000001e0: 005a 1553 0029 18da 0f41 7379 6e63 7067  .Z.S.)...Asyncpg
-000001f0: 4442 436c 6965 6e74 7a35 706f 7374 6772  DBClientz5postgr
-00000200: 6573 3a2f 2f7b 7573 6572 7d3a 7b70 6173  es://{user}:{pas
-00000210: 7377 6f72 647d 407b 686f 7374 7d3a 7b70  sword}@{host}:{p
-00000220: 6f72 747d 2f7b 6461 7461 6261 7365 7d63  ort}/{database}c
-00000230: 0600 0000 0000 0000 0800 0000 0700 0000  ................
-00000240: 0f00 0000 7372 0000 0074 0083 006a 017c  ....sr...t...j.|
-00000250: 067c 078e 0101 007c 017c 005f 027c 027c  .|.....|.|._.|.|
-00000260: 005f 037c 037c 005f 047c 047c 005f 057c  ._.|.|._.|.|._.|
-00000270: 057c 005f 067c 006a 076a 087c 006a 027c  .|._.|.j.j.|.j.|
-00000280: 006a 037c 006a 057c 006a 067c 006a 0464  .j.|.j.|.j.|.j.d
-00000290: 018d 057c 005f 0964 007c 005f 0a64 007c  ...|._.d.|._.d.|
-000002a0: 005f 0b74 0c64 0274 0d7c 006a 0e66 0269  ._.t.d.t.|.j.f.i
-000002b0: 0083 037c 005f 0f64 0053 0029 034e 2905  ...|._.d.S.).N).
-000002c0: da04 7573 6572 da08 7061 7373 776f 7264  ..user..password
-000002d0: da04 686f 7374 da04 706f 7274 da08 6461  ..host..port..da
-000002e0: 7461 6261 7365 da12 5472 616e 7361 6374  tabase..Transact
-000002f0: 696f 6e57 7261 7070 6572 2910 da05 7375  ionWrapper)...su
-00000300: 7065 72da 085f 5f69 6e69 745f 5f72 0b00  per..__init__r..
-00000310: 0000 720c 0000 0072 0f00 0000 720d 0000  ..r....r....r...
-00000320: 0072 0e00 0000 da0c 4453 4e5f 5445 4d50  .r......DSN_TEMP
-00000330: 4c41 5445 da06 666f 726d 6174 da03 6473  LATE..format..ds
-00000340: 6eda 085f 6462 5f70 6f6f 6cda 0b5f 636f  n.._db_pool.._co
-00000350: 6e6e 6563 7469 6f6e da04 7479 7065 7210  nnection..typer.
-00000360: 0000 00da 095f 5f63 6c61 7373 5f5f da12  .....__class__..
-00000370: 5f74 7261 6e73 6163 7469 6f6e 5f63 6c61  _transaction_cla
-00000380: 7373 2908 da04 7365 6c66 720b 0000 0072  ss)...selfr....r
-00000390: 0c00 0000 720f 0000 0072 0d00 0000 720e  ....r....r....r.
-000003a0: 0000 00da 0461 7267 73da 066b 7761 7267  .....args..kwarg
-000003b0: 7329 0172 1900 0000 a900 fa54 2f55 7365  s).r.......T/Use
-000003c0: 7273 2f61 6e64 7265 7962 6f6e 6461 722f  rs/andreybondar/
-000003d0: 5079 4368 6172 6d50 726f 6a65 6374 732f  PyCharmProjects/
-000003e0: 746f 7274 6f69 7365 2d6f 726d 2f74 6f72  tortoise-orm/tor
-000003f0: 746f 6973 652f 6261 636b 656e 6473 2f61  toise/backends/a
-00000400: 7379 6e63 7067 2f63 6c69 656e 742e 7079  syncpg/client.py
-00000410: 7212 0000 0013 0000 0073 2000 0000 0001  r........s .....
-00000420: 0e02 0601 0601 0601 0601 0602 0601 0401  ................
-00000430: 0401 0401 0401 0c02 0601 0602 0201 7a18  ..............z.
-00000440: 4173 796e 6370 6744 4243 6c69 656e 742e  AsyncpgDBClient.
-00000450: 5f5f 696e 6974 5f5f 6301 0000 0000 0000  __init__c.......
-00000460: 0001 0000 0007 0000 00c3 0000 0073 5600  .............sV.
-00000470: 0000 7c00 6a00 731c 7401 6a02 7c00 6a03  ..|.j.s.t.j.|.j.
-00000480: 8301 4900 6400 4800 7c00 5f04 6e14 7401  ..I.d.H.|._.n.t.
-00000490: 6a05 7c00 6a03 8301 4900 6400 4800 7c00  j.|.j...I.d.H.|.
-000004a0: 5f06 7c00 6a07 6a08 6401 6a09 7c00 6a0a  _.|.j.j.d.j.|.j.
-000004b0: 7c00 6a0b 7c00 6a0c 7c00 6a0d 6402 8d04  |.j.|.j.|.j.d...
-000004c0: 8301 0100 6400 5300 2903 4e7a 5743 7265  ....d.S.).NzWCre
-000004d0: 6174 6564 2063 6f6e 6e65 6374 696f 6e20  ated connection 
-000004e0: 7769 7468 2070 6172 616d 733a 2075 7365  with params: use
-000004f0: 723d 7b75 7365 727d 2064 6174 6162 6173  r={user} databas
-00000500: 653d 7b64 6174 6162 6173 657d 2068 6f73  e={database} hos
-00000510: 743d 7b68 6f73 747d 2070 6f72 743d 7b70  t={host} port={p
-00000520: 6f72 747d 2904 720b 0000 0072 0f00 0000  ort}).r....r....
-00000530: 720d 0000 0072 0e00 0000 290e da11 7369  r....r....)...si
-00000540: 6e67 6c65 5f63 6f6e 6e65 6374 696f 6eda  ngle_connection.
-00000550: 0761 7379 6e63 7067 5a0b 6372 6561 7465  .asyncpgZ.create
-00000560: 5f70 6f6f 6c72 1500 0000 7216 0000 00da  _poolr....r.....
-00000570: 0763 6f6e 6e65 6374 7217 0000 00da 036c  .connectr......l
-00000580: 6f67 da05 6465 6275 6772 1400 0000 720b  og..debugr....r.
-00000590: 0000 0072 0f00 0000 720d 0000 0072 0e00  ...r....r....r..
-000005a0: 0000 2901 721b 0000 0072 1e00 0000 721e  ..).r....r....r.
-000005b0: 0000 0072 1f00 0000 da11 6372 6561 7465  ...r......create
-000005c0: 5f63 6f6e 6e65 6374 696f 6e2a 0000 0073  _connection*...s
-000005d0: 0c00 0000 0001 0601 1602 1401 0601 0402  ................
-000005e0: 7a21 4173 796e 6370 6744 4243 6c69 656e  z!AsyncpgDBClien
-000005f0: 742e 6372 6561 7465 5f63 6f6e 6e65 6374  t.create_connect
-00000600: 696f 6e63 0100 0000 0000 0000 0100 0000  ionc............
-00000610: 0200 0000 c300 0000 732c 0000 007c 006a  ........s,...|.j
-00000620: 0073 187c 006a 016a 0283 0049 0064 0048  .s.|.j.j...I.d.H
-00000630: 0001 006e 107c 006a 036a 0283 0049 0064  ...n.|.j.j...I.d
-00000640: 0048 0001 0064 0053 0029 014e 2904 7220  .H...d.S.).N).r 
-00000650: 0000 0072 1600 0000 da05 636c 6f73 6572  ...r......closer
-00000660: 1700 0000 2901 721b 0000 0072 1e00 0000  ....).r....r....
-00000670: 721e 0000 0072 1f00 0000 7226 0000 0036  r....r....r&...6
-00000680: 0000 0073 0600 0000 0001 0601 1202 7a15  ...s..........z.
-00000690: 4173 796e 6370 6744 4243 6c69 656e 742e  AsyncpgDBClient.
-000006a0: 636c 6f73 6563 0100 0000 0000 0000 0200  closec..........
-000006b0: 0000 0800 0000 c300 0000 736e 0000 007c  ..........sn...|
-000006c0: 006a 007d 0164 017c 005f 0074 016a 027c  .j.}.d.|._.t.j.|
-000006d0: 006a 036a 047c 006a 057c 006a 067c 006a  .j.j.|.j.|.j.|.j
-000006e0: 077c 006a 0864 0264 038d 0583 0149 0064  .|.j.d.d.....I.d
-000006f0: 0048 007c 005f 097c 006a 0a64 046a 047c  .H.|._.|.j.d.j.|
-00000700: 006a 0b7c 006a 0583 0283 0149 0064 0048  .j.|.j.....I.d.H
-00000710: 0001 007c 006a 096a 0c83 0049 0064 0048  ...|.j.j...I.d.H
-00000720: 0001 007c 017c 005f 0064 0053 0029 054e  ...|.|._.d.S.).N
-00000730: 54da 0029 0572 0b00 0000 720c 0000 0072  T..).r....r....r
-00000740: 0d00 0000 720e 0000 0072 0f00 0000 7a1b  ....r....r....z.
-00000750: 4352 4541 5445 2044 4154 4142 4153 4520  CREATE DATABASE 
-00000760: 7b7d 204f 574e 4552 207b 7d29 0d72 2000  {} OWNER {}).r .
-00000770: 0000 7221 0000 0072 2200 0000 7213 0000  ..r!...r"...r...
-00000780: 0072 1400 0000 720b 0000 0072 0c00 0000  .r....r....r....
-00000790: 720d 0000 0072 0e00 0000 7217 0000 00da  r....r....r.....
-000007a0: 0e65 7865 6375 7465 5f73 6372 6970 7472  .execute_scriptr
-000007b0: 0f00 0000 7226 0000 0029 0272 1b00 0000  ....r&...).r....
-000007c0: 7220 0000 0072 1e00 0000 721e 0000 0072  r ...r....r....r
-000007d0: 1f00 0000 da09 6462 5f63 7265 6174 653c  ......db_create<
-000007e0: 0000 0073 1800 0000 0001 0601 0601 0a01  ...s............
-000007f0: 0401 0401 0401 0401 1202 0401 1802 1001  ................
-00000800: 7a19 4173 796e 6370 6744 4243 6c69 656e  z.AsyncpgDBClien
-00000810: 742e 6462 5f63 7265 6174 6563 0100 0000  t.db_createc....
-00000820: 0000 0000 0200 0000 0b00 0000 c300 0000  ................
-00000830: 7386 0000 007c 006a 007d 0164 017c 005f  s....|.j.}.d.|._
-00000840: 0074 016a 027c 006a 036a 047c 006a 057c  .t.j.|.j.j.|.j.|
-00000850: 006a 067c 006a 077c 006a 0864 0264 038d  .j.|.j.|.j.d.d..
-00000860: 0583 0149 0064 0048 007c 005f 0979 1c7c  ...I.d.H.|._.y.|
-00000870: 006a 0a64 046a 047c 006a 0b83 0183 0149  .j.d.j.|.j.....I
-00000880: 0064 0048 0001 0057 006e 1604 0074 016a  .d.H...W.n...t.j
-00000890: 0c6b 0a72 6a01 0001 0001 0059 006e 0258  .k.rj......Y.n.X
-000008a0: 007c 006a 096a 0d83 0049 0064 0048 0001  .|.j.j...I.d.H..
-000008b0: 007c 017c 005f 0064 0053 0029 054e 5472  .|.|._.d.S.).NTr
-000008c0: 2700 0000 2905 720b 0000 0072 0c00 0000  '...).r....r....
-000008d0: 720d 0000 0072 0e00 0000 720f 0000 007a  r....r....r....z
-000008e0: 1044 524f 5020 4441 5441 4241 5345 207b  .DROP DATABASE {
-000008f0: 7d29 0e72 2000 0000 7221 0000 0072 2200  }).r ...r!...r".
-00000900: 0000 7213 0000 0072 1400 0000 720b 0000  ..r....r....r...
-00000910: 0072 0c00 0000 720d 0000 0072 0e00 0000  .r....r....r....
-00000920: 7217 0000 0072 2800 0000 720f 0000 005a  r....r(...r....Z
-00000930: 1749 6e76 616c 6964 4361 7461 6c6f 674e  .InvalidCatalogN
-00000940: 616d 6545 7272 6f72 7226 0000 0029 0272  ameErrorr&...).r
-00000950: 1b00 0000 7220 0000 0072 1e00 0000 721e  ....r ...r....r.
-00000960: 0000 0072 1f00 0000 da09 6462 5f64 656c  ...r......db_del
-00000970: 6574 654c 0000 0073 1c00 0000 0001 0601  eteL...s........
-00000980: 0601 0a01 0401 0401 0401 0401 1202 0201  ................
-00000990: 1c01 1001 0601 1001 7a19 4173 796e 6370  ........z.Asyncp
-000009a0: 6744 4243 6c69 656e 742e 6462 5f64 656c  gDBClient.db_del
-000009b0: 6574 6563 0100 0000 0000 0000 0100 0000  etec............
-000009c0: 0200 0000 4300 0000 731e 0000 007c 006a  ....C...s....|.j
-000009d0: 0073 107c 006a 016a 0283 0053 0074 037c  .s.|.j.j...S.t.|
-000009e0: 006a 0483 0153 0064 0053 0029 014e 2905  .j...S.d.S.).N).
-000009f0: 7220 0000 0072 1600 0000 da07 6163 7175  r ...r......acqu
-00000a00: 6972 6572 0600 0000 7217 0000 0029 0172  irer....r....).r
-00000a10: 1b00 0000 721e 0000 0072 1e00 0000 721f  ....r....r....r.
-00000a20: 0000 00da 1261 6371 7569 7265 5f63 6f6e  .....acquire_con
-00000a30: 6e65 6374 696f 6e5d 0000 0073 0600 0000  nection]...s....
-00000a40: 0001 0601 0a02 7a22 4173 796e 6370 6744  ......z"AsyncpgD
-00000a50: 4243 6c69 656e 742e 6163 7175 6972 655f  BClient.acquire_
-00000a60: 636f 6e6e 6563 7469 6f6e 6301 0000 0000  connectionc.....
-00000a70: 0000 0001 0000 0003 0000 0043 0000 0073  ...........C...s
-00000a80: 2600 0000 7c00 6a00 7214 7c00 6a01 7c00  &...|.j.r.|.j.|.
-00000a90: 6a02 6401 8d01 5300 7c00 6a01 7c00 6a03  j.d...S.|.j.|.j.
-00000aa0: 6402 8d01 5300 6400 5300 2903 4e29 01da  d...S.d.S.).N)..
-00000ab0: 0a63 6f6e 6e65 6374 696f 6e29 01da 0470  .connection)...p
-00000ac0: 6f6f 6c29 0472 2000 0000 721a 0000 0072  ool).r ...r....r
-00000ad0: 1700 0000 7216 0000 0029 0172 1b00 0000  ....r....).r....
-00000ae0: 721e 0000 0072 1e00 0000 721f 0000 00da  r....r....r.....
-00000af0: 0e69 6e5f 7472 616e 7361 6374 696f 6e63  .in_transactionc
-00000b00: 0000 0073 0600 0000 0001 0601 0e02 7a1e  ...s..........z.
-00000b10: 4173 796e 6370 6744 4243 6c69 656e 742e  AsyncpgDBClient.
-00000b20: 696e 5f74 7261 6e73 6163 7469 6f6e 6302  in_transactionc.
-00000b30: 0000 0000 0000 0004 0000 0010 0000 00c3  ................
-00000b40: 0000 0073 9e00 0000 793e 7c00 6a00 8300  ...s....y>|.j...
-00000b50: 3400 4900 6400 4800 9a1e 7d02 7c00 6a01  4.I.d.H...}.|.j.
-00000b60: 6a02 7c01 8301 0100 7c02 6a03 7c01 8301  j.|.....|.j.|...
-00000b70: 4900 6400 4800 5300 5100 4900 6400 4800  I.d.H.S.Q.I.d.H.
-00000b80: 5200 5800 5700 6e5a 0400 7404 6a05 6a06  R.X.W.nZ..t.j.j.
-00000b90: 6b0a 726c 0100 7d03 0100 7a0e 7407 7c03  k.rl..}...z.t.|.
-00000ba0: 8301 8201 5700 5900 6400 6400 7d03 7e03  ....W.Y.d.d.}.~.
-00000bb0: 5800 6e2e 0400 7404 6a05 6a08 6b0a 7298  X.n...t.j.j.k.r.
-00000bc0: 0100 7d03 0100 7a0e 7409 7c03 8301 8201  ..}...z.t.|.....
-00000bd0: 5700 5900 6400 6400 7d03 7e03 5800 6e02  W.Y.d.d.}.~.X.n.
-00000be0: 5800 6400 5300 2901 4e29 0a72 2c00 0000  X.d.S.).N).r,...
-00000bf0: 7223 0000 0072 2400 0000 5a05 6665 7463  r#...r$...Z.fetc
-00000c00: 6872 2100 0000 da0a 6578 6365 7074 696f  hr!.....exceptio
-00000c10: 6e73 5a13 5379 6e74 6178 4f72 4163 6365  nsZ.SyntaxOrAcce
-00000c20: 7373 4572 726f 7272 0900 0000 5a21 496e  ssErrorr....Z!In
-00000c30: 7465 6772 6974 7943 6f6e 7374 7261 696e  tegrityConstrain
-00000c40: 7456 696f 6c61 7469 6f6e 4572 726f 7272  tViolationErrorr
-00000c50: 0800 0000 2904 721b 0000 00da 0571 7565  ....).r......que
-00000c60: 7279 722d 0000 00da 0365 7863 721e 0000  ryr-.....excr...
-00000c70: 0072 1e00 0000 721f 0000 00da 0d65 7865  .r....r......exe
-00000c80: 6375 7465 5f71 7565 7279 6900 0000 7310  cute_queryi...s.
-00000c90: 0000 0000 0102 0112 010c 0120 0114 0118  ........... ....
-00000ca0: 0114 017a 1d41 7379 6e63 7067 4442 436c  ...z.AsyncpgDBCl
-00000cb0: 6965 6e74 2e65 7865 6375 7465 5f71 7565  ient.execute_que
-00000cc0: 7279 6301 0000 0000 0000 0002 0000 0003  ryc.............
-00000cd0: 0000 00c3 0000 0073 3600 0000 7c00 6a00  .......s6...|.j.
-00000ce0: 7214 7c00 6a01 7c00 6a02 7c00 8302 5300  r.|.j.|.j.|...S.
-00000cf0: 7c00 6a03 6a04 6400 8301 4900 6400 4800  |.j.j.d...I.d.H.
-00000d00: 7d01 7c00 6a01 7c01 7c00 8302 5300 6400  }.|.j.|.|...S.d.
-00000d10: 5300 2901 4e29 0572 2000 0000 da18 5f73  S.).N).r ....._s
-00000d20: 696e 676c 655f 636f 6e6e 6563 7469 6f6e  ingle_connection
-00000d30: 5f63 6c61 7373 7217 0000 0072 1600 0000  _classr....r....
-00000d40: da08 5f61 6371 7569 7265 2902 721b 0000  .._acquire).r...
-00000d50: 0072 2d00 0000 721e 0000 0072 1e00 0000  .r-...r....r....
-00000d60: 721f 0000 00da 1567 6574 5f73 696e 676c  r......get_singl
-00000d70: 655f 636f 6e6e 6563 7469 6f6e 7300 0000  e_connections...
-00000d80: 7308 0000 0000 0106 010e 0212 017a 2541  s............z%A
-00000d90: 7379 6e63 7067 4442 436c 6965 6e74 2e67  syncpgDBClient.g
-00000da0: 6574 5f73 696e 676c 655f 636f 6e6e 6563  et_single_connec
-00000db0: 7469 6f6e 6302 0000 0000 0000 0002 0000  tionc...........
-00000dc0: 0002 0000 00c3 0000 0073 1e00 0000 7c00  .........s....|.
-00000dd0: 6a00 731a 7c00 6a01 6a02 7c01 6a03 8301  j.s.|.j.j.|.j...
-00000de0: 4900 6400 4800 0100 6400 5300 2901 4e29  I.d.H...d.S.).N)
-00000df0: 0472 2000 0000 7216 0000 00da 0772 656c  .r ...r......rel
-00000e00: 6561 7365 722d 0000 0029 0272 1b00 0000  easer-...).r....
-00000e10: 7220 0000 0072 1e00 0000 721e 0000 0072  r ...r....r....r
-00000e20: 1f00 0000 da19 7265 6c65 6173 655f 7369  ......release_si
-00000e30: 6e67 6c65 5f63 6f6e 6e65 6374 696f 6e7a  ngle_connectionz
-00000e40: 0000 0073 0400 0000 0001 0601 7a29 4173  ...s........z)As
-00000e50: 796e 6370 6744 4243 6c69 656e 742e 7265  yncpgDBClient.re
-00000e60: 6c65 6173 655f 7369 6e67 6c65 5f63 6f6e  lease_single_con
-00000e70: 6e65 6374 696f 6e63 0200 0000 0000 0000  nectionc........
-00000e80: 0300 0000 0a00 0000 c300 0000 7342 0000  ............sB..
-00000e90: 007c 006a 0083 0034 0049 0064 0048 009a  .|.j...4.I.d.H..
-00000ea0: 227d 027c 006a 016a 027c 0183 0101 007c  "}.|.j.j.|.....|
-00000eb0: 026a 037c 0183 0149 0064 0048 0001 0057  .j.|...I.d.H...W
-00000ec0: 0064 0051 0049 0064 0048 0052 0058 0064  .d.Q.I.d.H.R.X.d
-00000ed0: 0053 0029 014e 2904 722c 0000 0072 2300  .S.).N).r,...r#.
-00000ee0: 0000 7224 0000 00da 0765 7865 6375 7465  ..r$.....execute
-00000ef0: 2903 721b 0000 00da 0673 6372 6970 7472  ).r......scriptr
-00000f00: 2d00 0000 721e 0000 0072 1e00 0000 721f  -...r....r....r.
-00000f10: 0000 0072 2800 0000 7e00 0000 7306 0000  ...r(...~...s...
-00000f20: 0000 0112 010c 017a 1e41 7379 6e63 7067  .......z.Asyncpg
-00000f30: 4442 436c 6965 6e74 2e65 7865 6375 7465  DBClient.execute
-00000f40: 5f73 6372 6970 7429 16da 085f 5f6e 616d  _script)...__nam
-00000f50: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
-00000f60: 0c5f 5f71 7561 6c6e 616d 655f 5f72 1300  .__qualname__r..
-00000f70: 0000 7202 0000 00da 0b71 7565 7279 5f63  ..r......query_c
-00000f80: 6c61 7373 7203 0000 00da 0e65 7865 6375  lassr......execu
-00000f90: 746f 725f 636c 6173 7372 0400 0000 da10  tor_classr......
-00000fa0: 7363 6865 6d61 5f67 656e 6572 6174 6f72  schema_generator
-00000fb0: 7212 0000 0072 2500 0000 7226 0000 0072  r....r%...r&...r
-00000fc0: 2900 0000 722a 0000 0072 2c00 0000 722f  )...r*...r,...r/
-00000fd0: 0000 0072 3300 0000 7236 0000 0072 3800  ...r3...r6...r8.
-00000fe0: 0000 7228 0000 00da 0d5f 5f63 6c61 7373  ..r(.....__class
-00000ff0: 6365 6c6c 5f5f 721e 0000 0072 1e00 0000  cell__r....r....
-00001000: 2901 7219 0000 0072 1f00 0000 720a 0000  ).r....r....r...
-00001010: 000d 0000 0073 1e00 0000 0801 0401 0401  .....s..........
-00001020: 0401 0402 0c17 080c 0806 0810 0811 0806  ................
-00001030: 0806 080a 0807 0804 720a 0000 0063 0000  ........r....c..
-00001040: 0000 0000 0000 0000 0000 0300 0000 4000  ..............@.
-00001050: 0000 734e 0000 0065 005a 0164 005a 0264  ..sN...e.Z.d.Z.d
-00001060: 1264 0264 0384 015a 0364 0464 0584 005a  .d.d...Z.d.d...Z
-00001070: 0464 0664 0784 005a 0564 0864 0984 005a  .d.d...Z.d.d...Z
-00001080: 0664 0a64 0b84 005a 0764 0c64 0d84 005a  .d.d...Z.d.d...Z
-00001090: 0864 0e64 0f84 005a 0964 1064 1184 005a  .d.d...Z.d.d...Z
-000010a0: 0a64 0153 0029 1372 1000 0000 4e63 0300  .d.S.).r....Nc..
-000010b0: 0000 0000 0000 0300 0000 0400 0000 4300  ..............C.
-000010c0: 0000 7356 0000 0074 007c 0183 0174 007c  ..sV...t.|...t.|
-000010d0: 0283 016b 0373 1874 0164 0183 0182 017c  ...k.s.t.d.....|
-000010e0: 027c 005f 0274 036a 0464 0283 017c 005f  .|._.t.j.d...|._
-000010f0: 057c 017c 005f 0664 037c 005f 0774 0864  .|.|._.d.|._.t.d
-00001100: 0474 097c 006a 0a66 0269 0083 037c 005f  .t.|.j.f.i...|._
-00001110: 0b7c 006a 0a7c 005f 0c64 0053 0029 054e  .|.j.|._.d.S.).N
-00001120: 7a27 596f 7520 6d75 7374 2070 6173 7320  z'You must pass 
-00001130: 6569 7468 6572 2063 6f6e 6e65 6374 696f  either connectio
-00001140: 6e20 6f72 2070 6f6f 6cda 0964 625f 636c  n or pool..db_cl
-00001150: 6965 6e74 5472 0700 0000 290d da04 626f  ientTr....)...bo
-00001160: 6f6c da0e 4173 7365 7274 696f 6e45 7272  ol..AssertionErr
-00001170: 6f72 7217 0000 00da 076c 6f67 6769 6e67  orr......logging
-00001180: da09 6765 744c 6f67 6765 7272 2300 0000  ..getLoggerr#...
-00001190: da05 5f70 6f6f 6c72 2000 0000 7218 0000  .._poolr ...r...
-000011a0: 0072 0700 0000 7219 0000 0072 3400 0000  .r....r....r4...
-000011b0: 721a 0000 0029 0372 1b00 0000 722e 0000  r....).r....r...
-000011c0: 0072 2d00 0000 721e 0000 0072 1e00 0000  .r-...r....r....
-000011d0: 721f 0000 0072 1200 0000 8500 0000 7310  r....r........s.
-000011e0: 0000 0000 0118 0106 010c 0106 0106 0102  ................
-000011f0: 0112 027a 1b54 7261 6e73 6163 7469 6f6e  ...z.Transaction
-00001200: 5772 6170 7065 722e 5f5f 696e 6974 5f5f  Wrapper.__init__
-00001210: 6301 0000 0000 0000 0001 0000 0002 0000  c...............
-00001220: 0043 0000 0073 0a00 0000 7400 7c00 6a01  .C...s....t.|.j.
-00001230: 8301 5300 2901 4e29 0272 0600 0000 7217  ..S.).N).r....r.
-00001240: 0000 0029 0172 1b00 0000 721e 0000 0072  ...).r....r....r
-00001250: 1e00 0000 721f 0000 0072 2c00 0000 9000  ....r....r,.....
-00001260: 0000 7302 0000 0000 017a 2554 7261 6e73  ..s......z%Trans
-00001270: 6163 7469 6f6e 5772 6170 7065 722e 6163  actionWrapper.ac
-00001280: 7175 6972 655f 636f 6e6e 6563 7469 6f6e  quire_connection
-00001290: 6301 0000 0000 0000 0001 0000 0002 0000  c...............
-000012a0: 00c3 0000 0073 1200 0000 7c00 6a00 6a01  .....s....|.j.j.
-000012b0: 6400 8301 4900 6400 4800 5300 2901 4e29  d...I.d.H.S.).N)
-000012c0: 0272 4700 0000 7235 0000 0029 0172 1b00  .rG...r5...).r..
-000012d0: 0000 721e 0000 0072 1e00 0000 721f 0000  ..r....r....r...
-000012e0: 00da 0f5f 6765 745f 636f 6e6e 6563 7469  ..._get_connecti
-000012f0: 6f6e 9300 0000 7302 0000 0000 017a 2254  on....s......z"T
-00001300: 7261 6e73 6163 7469 6f6e 5772 6170 7065  ransactionWrappe
-00001310: 722e 5f67 6574 5f63 6f6e 6e65 6374 696f  r._get_connectio
-00001320: 6e63 0100 0000 0000 0000 0100 0000 0200  nc..............
-00001330: 0000 c300 0000 7336 0000 007c 006a 0073  ......s6...|.j.s
-00001340: 167c 006a 0183 0049 0064 0048 007c 005f  .|.j...I.d.H.|._
-00001350: 007c 006a 006a 0283 007c 005f 027c 006a  .|.j.j...|._.|.j
-00001360: 026a 0383 0049 0064 0048 0001 0064 0053  .j...I.d.H...d.S
-00001370: 0029 014e 2904 7217 0000 0072 4800 0000  .).N).r....rH...
-00001380: da0b 7472 616e 7361 6374 696f 6eda 0573  ..transaction..s
-00001390: 7461 7274 2901 721b 0000 0072 1e00 0000  tart).r....r....
-000013a0: 721e 0000 0072 1f00 0000 724a 0000 0096  r....r....rJ....
-000013b0: 0000 0073 0800 0000 0001 0601 1001 0c01  ...s............
-000013c0: 7a18 5472 616e 7361 6374 696f 6e57 7261  z.TransactionWra
-000013d0: 7070 6572 2e73 7461 7274 6301 0000 0000  pper.startc.....
-000013e0: 0000 0001 0000 0002 0000 00c3 0000 0073  ...............s
-000013f0: 3400 0000 7c00 6a00 6a01 8300 4900 6400  4...|.j.j...I.d.
-00001400: 4800 0100 7c00 6a02 7230 7c00 6a02 6a03  H...|.j.r0|.j.j.
-00001410: 7c00 6a04 8301 4900 6400 4800 0100 6400  |.j...I.d.H...d.
-00001420: 7c00 5f04 6400 5300 2901 4e29 0572 4900  |._.d.S.).N).rI.
-00001430: 0000 da06 636f 6d6d 6974 7247 0000 0072  ....commitrG...r
-00001440: 3700 0000 7217 0000 0029 0172 1b00 0000  7...r....).r....
-00001450: 721e 0000 0072 1e00 0000 721f 0000 0072  r....r....r....r
-00001460: 4b00 0000 9c00 0000 7308 0000 0000 0110  K.......s.......
-00001470: 0106 0114 017a 1954 7261 6e73 6163 7469  .....z.Transacti
-00001480: 6f6e 5772 6170 7065 722e 636f 6d6d 6974  onWrapper.commit
-00001490: 6301 0000 0000 0000 0001 0000 0002 0000  c...............
-000014a0: 00c3 0000 0073 3400 0000 7c00 6a00 6a01  .....s4...|.j.j.
-000014b0: 8300 4900 6400 4800 0100 7c00 6a02 7230  ..I.d.H...|.j.r0
-000014c0: 7c00 6a02 6a03 7c00 6a04 8301 4900 6400  |.j.j.|.j...I.d.
-000014d0: 4800 0100 6400 7c00 5f04 6400 5300 2901  H...d.|._.d.S.).
-000014e0: 4e29 0572 4900 0000 da08 726f 6c6c 6261  N).rI.....rollba
-000014f0: 636b 7247 0000 0072 3700 0000 7217 0000  ckrG...r7...r...
-00001500: 0029 0172 1b00 0000 721e 0000 0072 1e00  .).r....r....r..
-00001510: 0000 721f 0000 0072 4c00 0000 a200 0000  ..r....rL.......
-00001520: 7308 0000 0000 0110 0106 0114 017a 1b54  s............z.T
-00001530: 7261 6e73 6163 7469 6f6e 5772 6170 7065  ransactionWrappe
-00001540: 722e 726f 6c6c 6261 636b 6301 0000 0000  r.rollbackc.....
-00001550: 0000 0001 0000 0002 0000 00c3 0000 0073  ...............s
-00001560: 3600 0000 7c00 6a00 7316 7c00 6a01 8300  6...|.j.s.|.j...
-00001570: 4900 6400 4800 7c00 5f00 7c00 6a00 6a02  I.d.H.|._.|.j.j.
-00001580: 8300 7c00 5f02 7c00 6a02 6a03 8300 4900  ..|._.|.j.j...I.
-00001590: 6400 4800 0100 7c00 5300 2901 4e29 0472  d.H...|.S.).N).r
-000015a0: 1700 0000 7248 0000 0072 4900 0000 724a  ....rH...rI...rJ
-000015b0: 0000 0029 0172 1b00 0000 721e 0000 0072  ...).r....r....r
-000015c0: 1e00 0000 721f 0000 00da 0a5f 5f61 656e  ....r......__aen
-000015d0: 7465 725f 5fa8 0000 0073 0a00 0000 0001  ter__....s......
-000015e0: 0601 1001 0c01 1001 7a1d 5472 616e 7361  ........z.Transa
-000015f0: 6374 696f 6e57 7261 7070 6572 2e5f 5f61  ctionWrapper.__a
-00001600: 656e 7465 725f 5f63 0400 0000 0000 0000  enter__c........
-00001610: 0400 0000 0200 0000 c300 0000 736c 0000  ............sl..
-00001620: 007c 0172 387c 006a 006a 0183 0049 0064  .|.r8|.j.j...I.d
-00001630: 0048 0001 007c 006a 0272 347c 006a 026a  .H...|.j.r4|.j.j
-00001640: 037c 006a 0483 0149 0064 0048 0001 0064  .|.j...I.d.H...d
-00001650: 007c 005f 0464 0153 007c 006a 006a 0583  .|._.d.S.|.j.j..
-00001660: 0049 0064 0048 0001 007c 006a 0272 687c  .I.d.H...|.j.rh|
-00001670: 006a 026a 037c 006a 0483 0149 0064 0048  .j.j.|.j...I.d.H
-00001680: 0001 0064 007c 005f 0464 0053 0029 024e  ...d.|._.d.S.).N
-00001690: 4629 0672 4900 0000 724c 0000 0072 4700  F).rI...rL...rG.
-000016a0: 0000 7237 0000 0072 1700 0000 724b 0000  ..r7...r....rK..
-000016b0: 0029 0472 1b00 0000 da08 6578 635f 7479  .).r......exc_ty
-000016c0: 7065 da07 6578 635f 7661 6cda 0665 7863  pe..exc_val..exc
-000016d0: 5f74 6272 1e00 0000 721e 0000 0072 1f00  _tbr....r....r..
-000016e0: 0000 da09 5f5f 6165 7869 745f 5faf 0000  ....__aexit__...
-000016f0: 0073 1400 0000 0001 0401 1001 0601 1401  .s..............
-00001700: 0601 0401 1001 0601 1401 7a1c 5472 616e  ..........z.Tran
-00001710: 7361 6374 696f 6e57 7261 7070 6572 2e5f  sactionWrapper._
-00001720: 5f61 6578 6974 5f5f 2902 4e4e 290b 723b  _aexit__).NN).r;
-00001730: 0000 0072 3c00 0000 723d 0000 0072 1200  ...r<...r=...r..
-00001740: 0000 722c 0000 0072 4800 0000 724a 0000  ..r,...rH...rJ..
-00001750: 0072 4b00 0000 724c 0000 0072 4d00 0000  .rK...rL...rM...
-00001760: 7251 0000 0072 1e00 0000 721e 0000 0072  rQ...r....r....r
-00001770: 1e00 0000 721f 0000 0072 1000 0000 8400  ....r....r......
-00001780: 0000 7310 0000 0008 010a 0b08 0308 0308  ..s.............
-00001790: 0608 0608 0608 0772 1000 0000 2911 7245  .......r....).rE
-000017a0: 0000 0072 2100 0000 da06 7079 7069 6b61  ...r!.....pypika
-000017b0: 7202 0000 005a 2274 6f72 746f 6973 652e  r....Z"tortoise.
-000017c0: 6261 636b 656e 6473 2e61 7379 6e63 7067  backends.asyncpg
-000017d0: 2e65 7865 6375 746f 7272 0300 0000 5a2a  .executorr....Z*
-000017e0: 746f 7274 6f69 7365 2e62 6163 6b65 6e64  tortoise.backend
-000017f0: 732e 6173 796e 6370 672e 7363 6865 6d61  s.asyncpg.schema
-00001800: 5f67 656e 6572 6174 6f72 7204 0000 00da  _generatorr.....
-00001810: 1d74 6f72 746f 6973 652e 6261 636b 656e  .tortoise.backen
-00001820: 6473 2e62 6173 652e 636c 6965 6e74 7205  ds.base.clientr.
-00001830: 0000 0072 0600 0000 7207 0000 00da 1374  ...r....r......t
-00001840: 6f72 746f 6973 652e 6578 6365 7074 696f  ortoise.exceptio
-00001850: 6e73 7208 0000 0072 0900 0000 720a 0000  nsr....r....r...
-00001860: 0072 1000 0000 721e 0000 0072 1e00 0000  .r....r....r....
-00001870: 721e 0000 0072 1f00 0000 da08 3c6d 6f64  r....r......<mod
-00001880: 756c 653e 0100 0000 7310 0000 0008 0208  ule>....s.......
-00001890: 010c 020c 010c 0114 0210 0310 77         ............w
+00000000: 420d 0d0a 0000 0000 5576 3f5b a719 0000  B.......Uv?[....
+00000010: e300 0000 0000 0000 0000 0000 0004 0000  ................
+00000020: 0040 0000 0073 7c00 0000 6400 6401 6c00  .@...s|...d.d.l.
+00000030: 5a00 6400 6401 6c01 5a01 6400 6402 6c02  Z.d.d.l.Z.d.d.l.
+00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
+00000050: 0100 6400 6404 6c06 6d07 5a07 0100 6400  ..d.d.l.m.Z...d.
+00000060: 6405 6c08 6d09 5a09 6d0a 5a0a 6d0b 5a0b  d.l.m.Z.m.Z.m.Z.
+00000070: 0100 6400 6406 6c0c 6d0d 5a0d 6d0e 5a0e  ..d.d.l.m.Z.m.Z.
+00000080: 0100 4700 6407 6408 8400 6408 6509 8303  ..G.d.d...d.e...
+00000090: 5a0f 4700 6409 640a 8400 640a 650f 8303  Z.G.d.d...d.e...
+000000a0: 5a10 6401 5300 290b e900 0000 004e 2901  Z.d.S.)......N).
+000000b0: da0f 506f 7374 6772 6553 514c 5175 6572  ..PostgreSQLQuer
+000000c0: 7929 01da 0f41 7379 6e63 7067 4578 6563  y)...AsyncpgExec
+000000d0: 7574 6f72 2901 da16 4173 796e 6370 6753  utor)...AsyncpgS
+000000e0: 6368 656d 6147 656e 6572 6174 6f72 2903  chemaGenerator).
+000000f0: da11 4261 7365 4442 4173 796e 6343 6c69  ..BaseDBAsyncCli
+00000100: 656e 74da 1143 6f6e 6e65 6374 696f 6e57  ent..ConnectionW
+00000110: 7261 7070 6572 da17 5369 6e67 6c65 436f  rapper..SingleCo
+00000120: 6e6e 6563 7469 6f6e 5772 6170 7065 7229  nnectionWrapper)
+00000130: 02da 0e49 6e74 6567 7269 7479 4572 726f  ...IntegrityErro
+00000140: 72da 104f 7065 7261 7469 6f6e 616c 4572  r..OperationalEr
+00000150: 726f 7263 0000 0000 0000 0000 0000 0000  rorc............
+00000160: 0300 0000 0000 0000 737c 0000 0065 005a  ........s|...e.Z
+00000170: 0164 005a 0264 015a 0365 045a 0565 065a  .d.Z.d.Z.e.Z.e.Z
+00000180: 0765 085a 0987 0066 0164 0264 0384 085a  .e.Z...f.d.d...Z
+00000190: 0a64 0464 0584 005a 0b64 0664 0784 005a  .d.d...Z.d.d...Z
+000001a0: 0c64 0864 0984 005a 0d64 0a64 0b84 005a  .d.d...Z.d.d...Z
+000001b0: 0e64 0c64 0d84 005a 0f64 0e64 0f84 005a  .d.d...Z.d.d...Z
+000001c0: 1064 1064 1184 005a 1164 1264 1384 005a  .d.d...Z.d.d...Z
+000001d0: 1264 1464 1584 005a 1364 1664 1784 005a  .d.d...Z.d.d...Z
+000001e0: 1487 0004 005a 1553 0029 18da 0f41 7379  .....Z.S.)...Asy
+000001f0: 6e63 7067 4442 436c 6965 6e74 7a35 706f  ncpgDBClientz5po
+00000200: 7374 6772 6573 3a2f 2f7b 7573 6572 7d3a  stgres://{user}:
+00000210: 7b70 6173 7377 6f72 647d 407b 686f 7374  {password}@{host
+00000220: 7d3a 7b70 6f72 747d 2f7b 6461 7461 6261  }:{port}/{databa
+00000230: 7365 7d63 0600 0000 0000 0000 0800 0000  se}c............
+00000240: 0700 0000 0f00 0000 7372 0000 0074 0083  ........sr...t..
+00000250: 006a 017c 067c 078e 0101 007c 017c 005f  .j.|.|.....|.|._
+00000260: 027c 027c 005f 037c 037c 005f 047c 047c  .|.|._.|.|._.|.|
+00000270: 005f 057c 057c 005f 067c 006a 076a 087c  ._.|.|._.|.j.j.|
+00000280: 006a 027c 006a 037c 006a 057c 006a 067c  .j.|.j.|.j.|.j.|
+00000290: 006a 0464 018d 057c 005f 0964 007c 005f  .j.d...|._.d.|._
+000002a0: 0a64 007c 005f 0b74 0c64 0274 0d7c 006a  .d.|._.t.d.t.|.j
+000002b0: 0e66 0269 0083 037c 005f 0f64 0053 0029  .f.i...|._.d.S.)
+000002c0: 034e 2905 da04 7573 6572 da08 7061 7373  .N)...user..pass
+000002d0: 776f 7264 da04 686f 7374 da04 706f 7274  word..host..port
+000002e0: da08 6461 7461 6261 7365 da12 5472 616e  ..database..Tran
+000002f0: 7361 6374 696f 6e57 7261 7070 6572 2910  sactionWrapper).
+00000300: da05 7375 7065 72da 085f 5f69 6e69 745f  ..super..__init_
+00000310: 5f72 0b00 0000 720c 0000 0072 0f00 0000  _r....r....r....
+00000320: 720d 0000 0072 0e00 0000 da0c 4453 4e5f  r....r......DSN_
+00000330: 5445 4d50 4c41 5445 da06 666f 726d 6174  TEMPLATE..format
+00000340: da03 6473 6eda 085f 6462 5f70 6f6f 6cda  ..dsn.._db_pool.
+00000350: 0b5f 636f 6e6e 6563 7469 6f6e da04 7479  ._connection..ty
+00000360: 7065 7210 0000 00da 095f 5f63 6c61 7373  per......__class
+00000370: 5f5f da12 5f74 7261 6e73 6163 7469 6f6e  __.._transaction
+00000380: 5f63 6c61 7373 2908 da04 7365 6c66 720b  _class)...selfr.
+00000390: 0000 0072 0c00 0000 720f 0000 0072 0d00  ...r....r....r..
+000003a0: 0000 720e 0000 00da 0461 7267 73da 066b  ..r......args..k
+000003b0: 7761 7267 7329 0172 1900 0000 a900 fa54  wargs).r.......T
+000003c0: 2f55 7365 7273 2f61 6e64 7265 7962 6f6e  /Users/andreybon
+000003d0: 6461 722f 5079 4368 6172 6d50 726f 6a65  dar/PyCharmProje
+000003e0: 6374 732f 746f 7274 6f69 7365 2d6f 726d  cts/tortoise-orm
+000003f0: 2f74 6f72 746f 6973 652f 6261 636b 656e  /tortoise/backen
+00000400: 6473 2f61 7379 6e63 7067 2f63 6c69 656e  ds/asyncpg/clien
+00000410: 742e 7079 7212 0000 0013 0000 0073 2000  t.pyr........s .
+00000420: 0000 0001 0e02 0601 0601 0601 0601 0602  ................
+00000430: 0601 0401 0401 0401 0401 0c02 0601 0602  ................
+00000440: 0201 7a18 4173 796e 6370 6744 4243 6c69  ..z.AsyncpgDBCli
+00000450: 656e 742e 5f5f 696e 6974 5f5f 6301 0000  ent.__init__c...
+00000460: 0000 0000 0001 0000 0008 0000 00c3 0000  ................
+00000470: 0073 5600 0000 7c00 6a00 731c 7401 a002  .sV...|.j.s.t...
+00000480: 7c00 6a03 a101 4900 6400 4800 7c00 5f04  |.j...I.d.H.|._.
+00000490: 6e14 7401 a005 7c00 6a03 a101 4900 6400  n.t...|.j...I.d.
+000004a0: 4800 7c00 5f06 7c00 6a07 a008 6401 6a09  H.|._.|.j...d.j.
+000004b0: 7c00 6a0a 7c00 6a0b 7c00 6a0c 7c00 6a0d  |.j.|.j.|.j.|.j.
+000004c0: 6402 8d04 a101 0100 6400 5300 2903 4e7a  d.......d.S.).Nz
+000004d0: 5743 7265 6174 6564 2063 6f6e 6e65 6374  WCreated connect
+000004e0: 696f 6e20 7769 7468 2070 6172 616d 733a  ion with params:
+000004f0: 2075 7365 723d 7b75 7365 727d 2064 6174   user={user} dat
+00000500: 6162 6173 653d 7b64 6174 6162 6173 657d  abase={database}
+00000510: 2068 6f73 743d 7b68 6f73 747d 2070 6f72   host={host} por
+00000520: 743d 7b70 6f72 747d 2904 720b 0000 0072  t={port}).r....r
+00000530: 0f00 0000 720d 0000 0072 0e00 0000 290e  ....r....r....).
+00000540: da11 7369 6e67 6c65 5f63 6f6e 6e65 6374  ..single_connect
+00000550: 696f 6eda 0761 7379 6e63 7067 5a0b 6372  ion..asyncpgZ.cr
+00000560: 6561 7465 5f70 6f6f 6c72 1500 0000 7216  eate_poolr....r.
+00000570: 0000 00da 0763 6f6e 6e65 6374 7217 0000  .....connectr...
+00000580: 00da 036c 6f67 da05 6465 6275 6772 1400  ...log..debugr..
+00000590: 0000 720b 0000 0072 0f00 0000 720d 0000  ..r....r....r...
+000005a0: 0072 0e00 0000 2901 721b 0000 0072 1e00  .r....).r....r..
+000005b0: 0000 721e 0000 0072 1f00 0000 da11 6372  ..r....r......cr
+000005c0: 6561 7465 5f63 6f6e 6e65 6374 696f 6e2a  eate_connection*
+000005d0: 0000 0073 0c00 0000 0001 0601 1602 1401  ...s............
+000005e0: 0601 0402 7a21 4173 796e 6370 6744 4243  ....z!AsyncpgDBC
+000005f0: 6c69 656e 742e 6372 6561 7465 5f63 6f6e  lient.create_con
+00000600: 6e65 6374 696f 6e63 0100 0000 0000 0000  nectionc........
+00000610: 0100 0000 0200 0000 c300 0000 732c 0000  ............s,..
+00000620: 007c 006a 0073 187c 006a 01a0 02a1 0049  .|.j.s.|.j.....I
+00000630: 0064 0048 0001 006e 107c 006a 03a0 02a1  .d.H...n.|.j....
+00000640: 0049 0064 0048 0001 0064 0053 0029 014e  .I.d.H...d.S.).N
+00000650: 2904 7220 0000 0072 1600 0000 da05 636c  ).r ...r......cl
+00000660: 6f73 6572 1700 0000 2901 721b 0000 0072  oser....).r....r
+00000670: 1e00 0000 721e 0000 0072 1f00 0000 7226  ....r....r....r&
+00000680: 0000 0036 0000 0073 0600 0000 0001 0601  ...6...s........
+00000690: 1202 7a15 4173 796e 6370 6744 4243 6c69  ..z.AsyncpgDBCli
+000006a0: 656e 742e 636c 6f73 6563 0100 0000 0000  ent.closec......
+000006b0: 0000 0200 0000 0900 0000 c300 0000 736e  ..............sn
+000006c0: 0000 007c 006a 007d 0164 017c 005f 0074  ...|.j.}.d.|._.t
+000006d0: 01a0 027c 006a 036a 047c 006a 057c 006a  ...|.j.j.|.j.|.j
+000006e0: 067c 006a 077c 006a 0864 0264 038d 05a1  .|.j.|.j.d.d....
+000006f0: 0149 0064 0048 007c 005f 097c 00a0 0a64  .I.d.H.|._.|...d
+00000700: 04a0 047c 006a 0b7c 006a 05a1 02a1 0149  ...|.j.|.j.....I
+00000710: 0064 0048 0001 007c 006a 09a0 0ca1 0049  .d.H...|.j.....I
+00000720: 0064 0048 0001 007c 017c 005f 0064 0053  .d.H...|.|._.d.S
+00000730: 0029 054e 54da 0029 0572 0b00 0000 720c  .).NT..).r....r.
+00000740: 0000 0072 0d00 0000 720e 0000 0072 0f00  ...r....r....r..
+00000750: 0000 7a1b 4352 4541 5445 2044 4154 4142  ..z.CREATE DATAB
+00000760: 4153 4520 7b7d 204f 574e 4552 207b 7d29  ASE {} OWNER {})
+00000770: 0d72 2000 0000 7221 0000 0072 2200 0000  .r ...r!...r"...
+00000780: 7213 0000 0072 1400 0000 720b 0000 0072  r....r....r....r
+00000790: 0c00 0000 720d 0000 0072 0e00 0000 7217  ....r....r....r.
+000007a0: 0000 00da 0e65 7865 6375 7465 5f73 6372  .....execute_scr
+000007b0: 6970 7472 0f00 0000 7226 0000 0029 0272  iptr....r&...).r
+000007c0: 1b00 0000 7220 0000 0072 1e00 0000 721e  ....r ...r....r.
+000007d0: 0000 0072 1f00 0000 da09 6462 5f63 7265  ...r......db_cre
+000007e0: 6174 653c 0000 0073 1800 0000 0001 0601  ate<...s........
+000007f0: 0601 0a01 0401 0401 0401 0401 1202 0401  ................
+00000800: 1802 1001 7a19 4173 796e 6370 6744 4243  ....z.AsyncpgDBC
+00000810: 6c69 656e 742e 6462 5f63 7265 6174 6563  lient.db_createc
+00000820: 0100 0000 0000 0000 0200 0000 0900 0000  ................
+00000830: c300 0000 7386 0000 007c 006a 007d 0164  ....s....|.j.}.d
+00000840: 017c 005f 0074 01a0 027c 006a 036a 047c  .|._.t...|.j.j.|
+00000850: 006a 057c 006a 067c 006a 077c 006a 0864  .j.|.j.|.j.|.j.d
+00000860: 0264 038d 05a1 0149 0064 0048 007c 005f  .d.....I.d.H.|._
+00000870: 0979 1c7c 00a0 0a64 04a0 047c 006a 0ba1  .y.|...d...|.j..
+00000880: 01a1 0149 0064 0048 0001 0057 006e 1604  ...I.d.H...W.n..
+00000890: 0074 016a 0c6b 0a72 6a01 0001 0001 0059  .t.j.k.rj......Y
+000008a0: 006e 0258 007c 006a 09a0 0da1 0049 0064  .n.X.|.j.....I.d
+000008b0: 0048 0001 007c 017c 005f 0064 0053 0029  .H...|.|._.d.S.)
+000008c0: 054e 5472 2700 0000 2905 720b 0000 0072  .NTr'...).r....r
+000008d0: 0c00 0000 720d 0000 0072 0e00 0000 720f  ....r....r....r.
+000008e0: 0000 007a 1044 524f 5020 4441 5441 4241  ...z.DROP DATABA
+000008f0: 5345 207b 7d29 0e72 2000 0000 7221 0000  SE {}).r ...r!..
+00000900: 0072 2200 0000 7213 0000 0072 1400 0000  .r"...r....r....
+00000910: 720b 0000 0072 0c00 0000 720d 0000 0072  r....r....r....r
+00000920: 0e00 0000 7217 0000 0072 2800 0000 720f  ....r....r(...r.
+00000930: 0000 005a 1749 6e76 616c 6964 4361 7461  ...Z.InvalidCata
+00000940: 6c6f 674e 616d 6545 7272 6f72 7226 0000  logNameErrorr&..
+00000950: 0029 0272 1b00 0000 7220 0000 0072 1e00  .).r....r ...r..
+00000960: 0000 721e 0000 0072 1f00 0000 da09 6462  ..r....r......db
+00000970: 5f64 656c 6574 654c 0000 0073 1c00 0000  _deleteL...s....
+00000980: 0001 0601 0601 0a01 0401 0401 0401 0401  ................
+00000990: 1202 0201 1c01 1001 0601 1001 7a19 4173  ............z.As
+000009a0: 796e 6370 6744 4243 6c69 656e 742e 6462  yncpgDBClient.db
+000009b0: 5f64 656c 6574 6563 0100 0000 0000 0000  _deletec........
+000009c0: 0100 0000 0200 0000 4300 0000 731e 0000  ........C...s...
+000009d0: 007c 006a 0073 107c 006a 01a0 02a1 0053  .|.j.s.|.j.....S
+000009e0: 0074 037c 006a 0483 0153 0064 0053 0029  .t.|.j...S.d.S.)
+000009f0: 014e 2905 7220 0000 0072 1600 0000 da07  .N).r ...r......
+00000a00: 6163 7175 6972 6572 0600 0000 7217 0000  acquirer....r...
+00000a10: 0029 0172 1b00 0000 721e 0000 0072 1e00  .).r....r....r..
+00000a20: 0000 721f 0000 00da 1261 6371 7569 7265  ..r......acquire
+00000a30: 5f63 6f6e 6e65 6374 696f 6e5d 0000 0073  _connection]...s
+00000a40: 0600 0000 0001 0601 0a02 7a22 4173 796e  ..........z"Asyn
+00000a50: 6370 6744 4243 6c69 656e 742e 6163 7175  cpgDBClient.acqu
+00000a60: 6972 655f 636f 6e6e 6563 7469 6f6e 6301  ire_connectionc.
+00000a70: 0000 0000 0000 0001 0000 0003 0000 0043  ...............C
+00000a80: 0000 0073 2600 0000 7c00 6a00 7214 7c00  ...s&...|.j.r.|.
+00000a90: 6a01 7c00 6a02 6401 8d01 5300 7c00 6a01  j.|.j.d...S.|.j.
+00000aa0: 7c00 6a03 6402 8d01 5300 6400 5300 2903  |.j.d...S.d.S.).
+00000ab0: 4e29 01da 0a63 6f6e 6e65 6374 696f 6e29  N)...connection)
+00000ac0: 01da 0470 6f6f 6c29 0472 2000 0000 721a  ...pool).r ...r.
+00000ad0: 0000 0072 1700 0000 7216 0000 0029 0172  ...r....r....).r
+00000ae0: 1b00 0000 721e 0000 0072 1e00 0000 721f  ....r....r....r.
+00000af0: 0000 00da 0e69 6e5f 7472 616e 7361 6374  .....in_transact
+00000b00: 696f 6e63 0000 0073 0600 0000 0001 0601  ionc...s........
+00000b10: 0e02 7a1e 4173 796e 6370 6744 4243 6c69  ..z.AsyncpgDBCli
+00000b20: 656e 742e 696e 5f74 7261 6e73 6163 7469  ent.in_transacti
+00000b30: 6f6e 6302 0000 0000 0000 0004 0000 000a  onc.............
+00000b40: 0000 00c3 0000 0073 9e00 0000 793e 7c00  .......s....y>|.
+00000b50: a000 a100 3400 4900 6400 4800 9a1e 7d02  ....4.I.d.H...}.
+00000b60: 7c00 6a01 a002 7c01 a101 0100 7c02 a003  |.j...|.....|...
+00000b70: 7c01 a101 4900 6400 4800 5300 5100 4900  |...I.d.H.S.Q.I.
+00000b80: 6400 4800 5200 5800 5700 6e5a 0400 7404  d.H.R.X.W.nZ..t.
+00000b90: 6a05 6a06 6b0a 726c 0100 7d03 0100 7a0c  j.j.k.rl..}...z.
+00000ba0: 7407 7c03 8301 8201 5700 6400 6400 7d03  t.|.....W.d.d.}.
+00000bb0: 7e03 5800 5900 6e2e 0400 7404 6a05 6a08  ~.X.Y.n...t.j.j.
+00000bc0: 6b0a 7298 0100 7d03 0100 7a0c 7409 7c03  k.r...}...z.t.|.
+00000bd0: 8301 8201 5700 6400 6400 7d03 7e03 5800  ....W.d.d.}.~.X.
+00000be0: 5900 6e02 5800 6400 5300 2901 4e29 0a72  Y.n.X.d.S.).N).r
+00000bf0: 2c00 0000 7223 0000 0072 2400 0000 5a05  ,...r#...r$...Z.
+00000c00: 6665 7463 6872 2100 0000 da0a 6578 6365  fetchr!.....exce
+00000c10: 7074 696f 6e73 5a13 5379 6e74 6178 4f72  ptionsZ.SyntaxOr
+00000c20: 4163 6365 7373 4572 726f 7272 0900 0000  AccessErrorr....
+00000c30: 5a21 496e 7465 6772 6974 7943 6f6e 7374  Z!IntegrityConst
+00000c40: 7261 696e 7456 696f 6c61 7469 6f6e 4572  raintViolationEr
+00000c50: 726f 7272 0800 0000 2904 721b 0000 00da  rorr....).r.....
+00000c60: 0571 7565 7279 722d 0000 00da 0365 7863  .queryr-.....exc
+00000c70: 721e 0000 0072 1e00 0000 721f 0000 00da  r....r....r.....
+00000c80: 0d65 7865 6375 7465 5f71 7565 7279 6900  .execute_queryi.
+00000c90: 0000 7310 0000 0000 0102 0112 010c 0120  ..s............ 
+00000ca0: 0114 0118 0114 017a 1d41 7379 6e63 7067  .......z.Asyncpg
+00000cb0: 4442 436c 6965 6e74 2e65 7865 6375 7465  DBClient.execute
+00000cc0: 5f71 7565 7279 6301 0000 0000 0000 0002  _queryc.........
+00000cd0: 0000 0004 0000 00c3 0000 0073 3600 0000  ...........s6...
+00000ce0: 7c00 6a00 7214 7c00 a001 7c00 6a02 7c00  |.j.r.|...|.j.|.
+00000cf0: a102 5300 7c00 6a03 a004 6400 a101 4900  ..S.|.j...d...I.
+00000d00: 6400 4800 7d01 7c00 a001 7c01 7c00 a102  d.H.}.|...|.|...
+00000d10: 5300 6400 5300 2901 4e29 0572 2000 0000  S.d.S.).N).r ...
+00000d20: da18 5f73 696e 676c 655f 636f 6e6e 6563  .._single_connec
+00000d30: 7469 6f6e 5f63 6c61 7373 7217 0000 0072  tion_classr....r
+00000d40: 1600 0000 da08 5f61 6371 7569 7265 2902  ......_acquire).
+00000d50: 721b 0000 0072 2d00 0000 721e 0000 0072  r....r-...r....r
+00000d60: 1e00 0000 721f 0000 00da 1567 6574 5f73  ....r......get_s
+00000d70: 696e 676c 655f 636f 6e6e 6563 7469 6f6e  ingle_connection
+00000d80: 7300 0000 7308 0000 0000 0106 010e 0212  s...s...........
+00000d90: 017a 2541 7379 6e63 7067 4442 436c 6965  .z%AsyncpgDBClie
+00000da0: 6e74 2e67 6574 5f73 696e 676c 655f 636f  nt.get_single_co
+00000db0: 6e6e 6563 7469 6f6e 6302 0000 0000 0000  nnectionc.......
+00000dc0: 0002 0000 0003 0000 00c3 0000 0073 1e00  .............s..
+00000dd0: 0000 7c00 6a00 731a 7c00 6a01 a002 7c01  ..|.j.s.|.j...|.
+00000de0: 6a03 a101 4900 6400 4800 0100 6400 5300  j...I.d.H...d.S.
+00000df0: 2901 4e29 0472 2000 0000 7216 0000 00da  ).N).r ...r.....
+00000e00: 0772 656c 6561 7365 722d 0000 0029 0272  .releaser-...).r
+00000e10: 1b00 0000 7220 0000 0072 1e00 0000 721e  ....r ...r....r.
+00000e20: 0000 0072 1f00 0000 da19 7265 6c65 6173  ...r......releas
+00000e30: 655f 7369 6e67 6c65 5f63 6f6e 6e65 6374  e_single_connect
+00000e40: 696f 6e7a 0000 0073 0400 0000 0001 0601  ionz...s........
+00000e50: 7a29 4173 796e 6370 6744 4243 6c69 656e  z)AsyncpgDBClien
+00000e60: 742e 7265 6c65 6173 655f 7369 6e67 6c65  t.release_single
+00000e70: 5f63 6f6e 6e65 6374 696f 6e63 0200 0000  _connectionc....
+00000e80: 0000 0000 0300 0000 0a00 0000 c300 0000  ................
+00000e90: 7342 0000 007c 00a0 00a1 0034 0049 0064  sB...|.....4.I.d
+00000ea0: 0048 009a 227d 027c 006a 01a0 027c 01a1  .H.."}.|.j...|..
+00000eb0: 0101 007c 02a0 037c 01a1 0149 0064 0048  ...|...|...I.d.H
+00000ec0: 0001 0057 0064 0051 0049 0064 0048 0052  ...W.d.Q.I.d.H.R
+00000ed0: 0058 0064 0053 0029 014e 2904 722c 0000  .X.d.S.).N).r,..
+00000ee0: 0072 2300 0000 7224 0000 00da 0765 7865  .r#...r$.....exe
+00000ef0: 6375 7465 2903 721b 0000 00da 0673 6372  cute).r......scr
+00000f00: 6970 7472 2d00 0000 721e 0000 0072 1e00  iptr-...r....r..
+00000f10: 0000 721f 0000 0072 2800 0000 7e00 0000  ..r....r(...~...
+00000f20: 7306 0000 0000 0112 010c 017a 1e41 7379  s..........z.Asy
+00000f30: 6e63 7067 4442 436c 6965 6e74 2e65 7865  ncpgDBClient.exe
+00000f40: 6375 7465 5f73 6372 6970 7429 16da 085f  cute_script)..._
+00000f50: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
+00000f60: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
+00000f70: 5f72 1300 0000 7202 0000 00da 0b71 7565  _r....r......que
+00000f80: 7279 5f63 6c61 7373 7203 0000 00da 0e65  ry_classr......e
+00000f90: 7865 6375 746f 725f 636c 6173 7372 0400  xecutor_classr..
+00000fa0: 0000 da10 7363 6865 6d61 5f67 656e 6572  ....schema_gener
+00000fb0: 6174 6f72 7212 0000 0072 2500 0000 7226  atorr....r%...r&
+00000fc0: 0000 0072 2900 0000 722a 0000 0072 2c00  ...r)...r*...r,.
+00000fd0: 0000 722f 0000 0072 3300 0000 7236 0000  ..r/...r3...r6..
+00000fe0: 0072 3800 0000 7228 0000 00da 0d5f 5f63  .r8...r(.....__c
+00000ff0: 6c61 7373 6365 6c6c 5f5f 721e 0000 0072  lasscell__r....r
+00001000: 1e00 0000 2901 7219 0000 0072 1f00 0000  ....).r....r....
+00001010: 720a 0000 000d 0000 0073 1e00 0000 0801  r........s......
+00001020: 0401 0401 0401 0402 0c17 080c 0806 0810  ................
+00001030: 0811 0806 0806 080a 0807 0804 720a 0000  ............r...
+00001040: 0063 0000 0000 0000 0000 0000 0000 0300  .c..............
+00001050: 0000 4000 0000 734e 0000 0065 005a 0164  ..@...sN...e.Z.d
+00001060: 005a 0264 1264 0264 0384 015a 0364 0464  .Z.d.d.d...Z.d.d
+00001070: 0584 005a 0464 0664 0784 005a 0564 0864  ...Z.d.d...Z.d.d
+00001080: 0984 005a 0664 0a64 0b84 005a 0764 0c64  ...Z.d.d...Z.d.d
+00001090: 0d84 005a 0864 0e64 0f84 005a 0964 1064  ...Z.d.d...Z.d.d
+000010a0: 1184 005a 0a64 0153 0029 1372 1000 0000  ...Z.d.S.).r....
+000010b0: 4e63 0300 0000 0000 0000 0300 0000 0400  Nc..............
+000010c0: 0000 4300 0000 7356 0000 0074 007c 0183  ..C...sV...t.|..
+000010d0: 0174 007c 0283 016b 0373 1874 0164 0183  .t.|...k.s.t.d..
+000010e0: 0182 017c 027c 005f 0274 03a0 0464 02a1  ...|.|._.t...d..
+000010f0: 017c 005f 057c 017c 005f 0664 037c 005f  .|._.|.|._.d.|._
+00001100: 0774 0864 0474 097c 006a 0a66 0269 0083  .t.d.t.|.j.f.i..
+00001110: 037c 005f 0b7c 006a 0a7c 005f 0c64 0053  .|._.|.j.|._.d.S
+00001120: 0029 054e 7a27 596f 7520 6d75 7374 2070  .).Nz'You must p
+00001130: 6173 7320 6569 7468 6572 2063 6f6e 6e65  ass either conne
+00001140: 6374 696f 6e20 6f72 2070 6f6f 6cda 0964  ction or pool..d
+00001150: 625f 636c 6965 6e74 5472 0700 0000 290d  b_clientTr....).
+00001160: da04 626f 6f6c da0e 4173 7365 7274 696f  ..bool..Assertio
+00001170: 6e45 7272 6f72 7217 0000 00da 076c 6f67  nErrorr......log
+00001180: 6769 6e67 da09 6765 744c 6f67 6765 7272  ging..getLoggerr
+00001190: 2300 0000 da05 5f70 6f6f 6c72 2000 0000  #....._poolr ...
+000011a0: 7218 0000 0072 0700 0000 7219 0000 0072  r....r....r....r
+000011b0: 3400 0000 721a 0000 0029 0372 1b00 0000  4...r....).r....
+000011c0: 722e 0000 0072 2d00 0000 721e 0000 0072  r....r-...r....r
+000011d0: 1e00 0000 721f 0000 0072 1200 0000 8500  ....r....r......
+000011e0: 0000 7310 0000 0000 0118 0106 010c 0106  ..s.............
+000011f0: 0106 0102 0112 027a 1b54 7261 6e73 6163  .......z.Transac
+00001200: 7469 6f6e 5772 6170 7065 722e 5f5f 696e  tionWrapper.__in
+00001210: 6974 5f5f 6301 0000 0000 0000 0001 0000  it__c...........
+00001220: 0002 0000 0043 0000 0073 0a00 0000 7400  .....C...s....t.
+00001230: 7c00 6a01 8301 5300 2901 4e29 0272 0600  |.j...S.).N).r..
+00001240: 0000 7217 0000 0029 0172 1b00 0000 721e  ..r....).r....r.
+00001250: 0000 0072 1e00 0000 721f 0000 0072 2c00  ...r....r....r,.
+00001260: 0000 9000 0000 7302 0000 0000 017a 2554  ......s......z%T
+00001270: 7261 6e73 6163 7469 6f6e 5772 6170 7065  ransactionWrappe
+00001280: 722e 6163 7175 6972 655f 636f 6e6e 6563  r.acquire_connec
+00001290: 7469 6f6e 6301 0000 0000 0000 0001 0000  tionc...........
+000012a0: 0003 0000 00c3 0000 0073 1200 0000 7c00  .........s....|.
+000012b0: 6a00 a001 6400 a101 4900 6400 4800 5300  j...d...I.d.H.S.
+000012c0: 2901 4e29 0272 4700 0000 7235 0000 0029  ).N).rG...r5...)
+000012d0: 0172 1b00 0000 721e 0000 0072 1e00 0000  .r....r....r....
+000012e0: 721f 0000 00da 0f5f 6765 745f 636f 6e6e  r......_get_conn
+000012f0: 6563 7469 6f6e 9300 0000 7302 0000 0000  ection....s.....
+00001300: 017a 2254 7261 6e73 6163 7469 6f6e 5772  .z"TransactionWr
+00001310: 6170 7065 722e 5f67 6574 5f63 6f6e 6e65  apper._get_conne
+00001320: 6374 696f 6e63 0100 0000 0000 0000 0100  ctionc..........
+00001330: 0000 0200 0000 c300 0000 7336 0000 007c  ..........s6...|
+00001340: 006a 0073 167c 00a0 01a1 0049 0064 0048  .j.s.|.....I.d.H
+00001350: 007c 005f 007c 006a 00a0 02a1 007c 005f  .|._.|.j.....|._
+00001360: 027c 006a 02a0 03a1 0049 0064 0048 0001  .|.j.....I.d.H..
+00001370: 0064 0053 0029 014e 2904 7217 0000 0072  .d.S.).N).r....r
+00001380: 4800 0000 da0b 7472 616e 7361 6374 696f  H.....transactio
+00001390: 6eda 0573 7461 7274 2901 721b 0000 0072  n..start).r....r
+000013a0: 1e00 0000 721e 0000 0072 1f00 0000 724a  ....r....r....rJ
+000013b0: 0000 0096 0000 0073 0800 0000 0001 0601  .......s........
+000013c0: 1001 0c01 7a18 5472 616e 7361 6374 696f  ....z.Transactio
+000013d0: 6e57 7261 7070 6572 2e73 7461 7274 6301  nWrapper.startc.
+000013e0: 0000 0000 0000 0001 0000 0003 0000 00c3  ................
+000013f0: 0000 0073 3400 0000 7c00 6a00 a001 a100  ...s4...|.j.....
+00001400: 4900 6400 4800 0100 7c00 6a02 7230 7c00  I.d.H...|.j.r0|.
+00001410: 6a02 a003 7c00 6a04 a101 4900 6400 4800  j...|.j...I.d.H.
+00001420: 0100 6400 7c00 5f04 6400 5300 2901 4e29  ..d.|._.d.S.).N)
+00001430: 0572 4900 0000 da06 636f 6d6d 6974 7247  .rI.....commitrG
+00001440: 0000 0072 3700 0000 7217 0000 0029 0172  ...r7...r....).r
+00001450: 1b00 0000 721e 0000 0072 1e00 0000 721f  ....r....r....r.
+00001460: 0000 0072 4b00 0000 9c00 0000 7308 0000  ...rK.......s...
+00001470: 0000 0110 0106 0114 017a 1954 7261 6e73  .........z.Trans
+00001480: 6163 7469 6f6e 5772 6170 7065 722e 636f  actionWrapper.co
+00001490: 6d6d 6974 6301 0000 0000 0000 0001 0000  mmitc...........
+000014a0: 0003 0000 00c3 0000 0073 3400 0000 7c00  .........s4...|.
+000014b0: 6a00 a001 a100 4900 6400 4800 0100 7c00  j.....I.d.H...|.
+000014c0: 6a02 7230 7c00 6a02 a003 7c00 6a04 a101  j.r0|.j...|.j...
+000014d0: 4900 6400 4800 0100 6400 7c00 5f04 6400  I.d.H...d.|._.d.
+000014e0: 5300 2901 4e29 0572 4900 0000 da08 726f  S.).N).rI.....ro
+000014f0: 6c6c 6261 636b 7247 0000 0072 3700 0000  llbackrG...r7...
+00001500: 7217 0000 0029 0172 1b00 0000 721e 0000  r....).r....r...
+00001510: 0072 1e00 0000 721f 0000 0072 4c00 0000  .r....r....rL...
+00001520: a200 0000 7308 0000 0000 0110 0106 0114  ....s...........
+00001530: 017a 1b54 7261 6e73 6163 7469 6f6e 5772  .z.TransactionWr
+00001540: 6170 7065 722e 726f 6c6c 6261 636b 6301  apper.rollbackc.
+00001550: 0000 0000 0000 0001 0000 0002 0000 00c3  ................
+00001560: 0000 0073 3600 0000 7c00 6a00 7316 7c00  ...s6...|.j.s.|.
+00001570: a001 a100 4900 6400 4800 7c00 5f00 7c00  ....I.d.H.|._.|.
+00001580: 6a00 a002 a100 7c00 5f02 7c00 6a02 a003  j.....|._.|.j...
+00001590: a100 4900 6400 4800 0100 7c00 5300 2901  ..I.d.H...|.S.).
+000015a0: 4e29 0472 1700 0000 7248 0000 0072 4900  N).r....rH...rI.
+000015b0: 0000 724a 0000 0029 0172 1b00 0000 721e  ..rJ...).r....r.
+000015c0: 0000 0072 1e00 0000 721f 0000 00da 0a5f  ...r....r......_
+000015d0: 5f61 656e 7465 725f 5fa8 0000 0073 0a00  _aenter__....s..
+000015e0: 0000 0001 0601 1001 0c01 1001 7a1d 5472  ............z.Tr
+000015f0: 616e 7361 6374 696f 6e57 7261 7070 6572  ansactionWrapper
+00001600: 2e5f 5f61 656e 7465 725f 5f63 0400 0000  .__aenter__c....
+00001610: 0000 0000 0400 0000 0300 0000 c300 0000  ................
+00001620: 736c 0000 007c 0172 387c 006a 00a0 01a1  sl...|.r8|.j....
+00001630: 0049 0064 0048 0001 007c 006a 0272 347c  .I.d.H...|.j.r4|
+00001640: 006a 02a0 037c 006a 04a1 0149 0064 0048  .j...|.j...I.d.H
+00001650: 0001 0064 007c 005f 0464 0153 007c 006a  ...d.|._.d.S.|.j
+00001660: 00a0 05a1 0049 0064 0048 0001 007c 006a  .....I.d.H...|.j
+00001670: 0272 687c 006a 02a0 037c 006a 04a1 0149  .rh|.j...|.j...I
+00001680: 0064 0048 0001 0064 007c 005f 0464 0053  .d.H...d.|._.d.S
+00001690: 0029 024e 4629 0672 4900 0000 724c 0000  .).NF).rI...rL..
+000016a0: 0072 4700 0000 7237 0000 0072 1700 0000  .rG...r7...r....
+000016b0: 724b 0000 0029 0472 1b00 0000 da08 6578  rK...).r......ex
+000016c0: 635f 7479 7065 da07 6578 635f 7661 6cda  c_type..exc_val.
+000016d0: 0665 7863 5f74 6272 1e00 0000 721e 0000  .exc_tbr....r...
+000016e0: 0072 1f00 0000 da09 5f5f 6165 7869 745f  .r......__aexit_
+000016f0: 5faf 0000 0073 1400 0000 0001 0401 1001  _....s..........
+00001700: 0601 1401 0601 0401 1001 0601 1401 7a1c  ..............z.
+00001710: 5472 616e 7361 6374 696f 6e57 7261 7070  TransactionWrapp
+00001720: 6572 2e5f 5f61 6578 6974 5f5f 2902 4e4e  er.__aexit__).NN
+00001730: 290b 723b 0000 0072 3c00 0000 723d 0000  ).r;...r<...r=..
+00001740: 0072 1200 0000 722c 0000 0072 4800 0000  .r....r,...rH...
+00001750: 724a 0000 0072 4b00 0000 724c 0000 0072  rJ...rK...rL...r
+00001760: 4d00 0000 7251 0000 0072 1e00 0000 721e  M...rQ...r....r.
+00001770: 0000 0072 1e00 0000 721f 0000 0072 1000  ...r....r....r..
+00001780: 0000 8400 0000 7310 0000 0008 010a 0b08  ......s.........
+00001790: 0308 0308 0608 0608 0608 0772 1000 0000  ...........r....
+000017a0: 2911 7245 0000 0072 2100 0000 da06 7079  ).rE...r!.....py
+000017b0: 7069 6b61 7202 0000 005a 2274 6f72 746f  pikar....Z"torto
+000017c0: 6973 652e 6261 636b 656e 6473 2e61 7379  ise.backends.asy
+000017d0: 6e63 7067 2e65 7865 6375 746f 7272 0300  ncpg.executorr..
+000017e0: 0000 5a2a 746f 7274 6f69 7365 2e62 6163  ..Z*tortoise.bac
+000017f0: 6b65 6e64 732e 6173 796e 6370 672e 7363  kends.asyncpg.sc
+00001800: 6865 6d61 5f67 656e 6572 6174 6f72 7204  hema_generatorr.
+00001810: 0000 00da 1d74 6f72 746f 6973 652e 6261  .....tortoise.ba
+00001820: 636b 656e 6473 2e62 6173 652e 636c 6965  ckends.base.clie
+00001830: 6e74 7205 0000 0072 0600 0000 7207 0000  ntr....r....r...
+00001840: 00da 1374 6f72 746f 6973 652e 6578 6365  ...tortoise.exce
+00001850: 7074 696f 6e73 7208 0000 0072 0900 0000  ptionsr....r....
+00001860: 720a 0000 0072 1000 0000 721e 0000 0072  r....r....r....r
+00001870: 1e00 0000 721e 0000 0072 1f00 0000 da08  ....r....r......
+00001880: 3c6d 6f64 756c 653e 0100 0000 7310 0000  <module>....s...
+00001890: 0008 0208 010c 020c 010c 0114 0210 0310  ................
+000018a0: 77                                       w
```

### Comparing `tortoise-orm-0.9.2/tortoise/backends/asyncpg/__pycache__/schema_generator.cpython-36.pyc` & `tortoise-orm-0.9.4/tortoise/backends/asyncpg/__pycache__/schema_generator.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `tortoise-orm-0.9.2/tortoise/backends/asyncpg/__pycache__/executor.cpython-36.pyc` & `tortoise-orm-0.9.4/tortoise/backends/asyncpg/__pycache__/executor.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `tortoise-orm-0.9.2/tortoise/backends/asyncpg/__pycache__/fields.cpython-36.pyc` & `tortoise-orm-0.9.4/tortoise/backends/asyncpg/__pycache__/fields.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `tortoise-orm-0.9.2/tortoise/backends/asyncpg/executor.py` & `tortoise-orm-0.9.4/tortoise/backends/asyncpg/executor.py`

 * *Files identical despite different names*

### Comparing `tortoise-orm-0.9.2/tortoise/backends/sqlite/.DS_Store` & `tortoise-orm-0.9.4/tortoise/backends/sqlite/.DS_Store`

 * *Files identical despite different names*

### Comparing `tortoise-orm-0.9.2/tortoise/backends/sqlite/client.py` & `tortoise-orm-0.9.4/tortoise/backends/sqlite/client.py`

 * *Files identical despite different names*

### Comparing `tortoise-orm-0.9.2/tortoise/backends/sqlite/__pycache__/client.cpython-36.pyc` & `tortoise-orm-0.9.4/tortoise/backends/sqlite/__pycache__/client.cpython-35.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.6 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 22% similar despite different names*

```diff
@@ -1,352 +1,373 @@
-00000000: 330d 0d0a 5576 3f5b 2611 0000 e300 0000  3...Uv?[&.......
+00000000: 170d 0d0a 5576 3f5b 2611 0000 e300 0000  ....Uv?[&.......
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 8800 0000 6400 6401 6c00 5a00 6400  .s....d.d.l.Z.d.
-00000030: 6401 6c01 5a01 6400 6401 6c02 5a02 6400  d.l.Z.d.d.l.Z.d.
-00000040: 6401 6c03 5a03 6400 6402 6c04 6d05 5a05  d.l.Z.d.d.l.m.Z.
-00000050: 0100 6400 6403 6c06 6d07 5a07 6d08 5a08  ..d.d.l.m.Z.m.Z.
-00000060: 0100 6400 6404 6c09 6d0a 5a0a 0100 6400  ..d.d.l.m.Z...d.
-00000070: 6405 6c0b 6d0c 5a0c 0100 6400 6406 6c0d  d.l.m.Z...d.d.l.
-00000080: 6d0e 5a0e 6d0f 5a0f 0100 4700 6407 6408  m.Z.m.Z...G.d.d.
-00000090: 8400 6408 6505 8303 5a10 4700 6409 640a  ..d.e...Z.G.d.d.
-000000a0: 8400 640a 6510 8303 5a11 6401 5300 290b  ..d.e...Z.d.S.).
-000000b0: e900 0000 004e 2901 da11 4261 7365 4442  .....N)...BaseDB
-000000c0: 4173 796e 6343 6c69 656e 7429 02da 1143  AsyncClient)...C
-000000d0: 6f6e 6e65 6374 696f 6e57 7261 7070 6572  onnectionWrapper
-000000e0: da17 5369 6e67 6c65 436f 6e6e 6563 7469  ..SingleConnecti
-000000f0: 6f6e 5772 6170 7065 7229 01da 0e53 716c  onWrapper)...Sql
-00000100: 6974 6545 7865 6375 746f 7229 01da 1553  iteExecutor)...S
-00000110: 716c 6974 6553 6368 656d 6147 656e 6572  qliteSchemaGener
-00000120: 6174 6f72 2902 da0e 496e 7465 6772 6974  ator)...Integrit
-00000130: 7945 7272 6f72 da10 4f70 6572 6174 696f  yError..Operatio
-00000140: 6e61 6c45 7272 6f72 6300 0000 0000 0000  nalErrorc.......
-00000150: 0000 0000 0003 0000 0000 0000 0073 7e00  .............s~.
-00000160: 0000 6500 5a01 6400 5a02 6503 5a04 6505  ..e.Z.d.Z.e.Z.e.
-00000170: 5a06 8700 6601 6401 6402 8408 5a07 6403  Z...f.d.d...Z.d.
-00000180: 6404 8400 5a08 6405 6406 8400 5a09 6407  d...Z.d.d...Z.d.
-00000190: 6408 8400 5a0a 6409 640a 8400 5a0b 640b  d...Z.d.d...Z.d.
-000001a0: 640c 8400 5a0c 640d 640e 8400 5a0d 641a  d...Z.d.d...Z.d.
-000001b0: 6410 6411 8401 5a0e 6412 6413 8400 5a0f  d.d...Z.d.d...Z.
-000001c0: 6414 6415 8400 5a10 6416 6417 8400 5a11  d.d...Z.d.d...Z.
-000001d0: 6418 6419 8400 5a12 8700 0400 5a13 5300  d.d...Z.....Z.S.
-000001e0: 291b da0c 5371 6c69 7465 436c 6965 6e74  )...SqliteClient
-000001f0: 6302 0000 0000 0000 0004 0000 0004 0000  c...............
-00000200: 000f 0000 0073 4000 0000 7400 8300 6a01  .....s@...t...j.
-00000210: 7c02 7c03 8e01 0100 7c01 7c00 5f02 7403  |.|.....|.|._.t.
-00000220: 6401 7404 7c00 6a05 6602 6900 8303 7c00  d.t.|.j.f.i...|.
-00000230: 5f06 7403 6402 7407 7c00 6a05 6602 6900  _.t.d.t.|.j.f.i.
-00000240: 8303 7c00 5f08 6400 5300 2903 4eda 1254  ..|._.d.S.).N..T
-00000250: 7261 6e73 6163 7469 6f6e 5772 6170 7065  ransactionWrappe
-00000260: 7272 0400 0000 2909 da05 7375 7065 72da  rr....)...super.
-00000270: 085f 5f69 6e69 745f 5fda 0866 696c 656e  .__init__..filen
-00000280: 616d 65da 0474 7970 6572 0a00 0000 da09  ame..typer......
-00000290: 5f5f 636c 6173 735f 5fda 125f 7472 616e  __class__.._tran
-000002a0: 7361 6374 696f 6e5f 636c 6173 7372 0400  saction_classr..
-000002b0: 0000 da18 5f73 696e 676c 655f 636f 6e6e  ...._single_conn
-000002c0: 6563 7469 6f6e 5f63 6c61 7373 2904 da04  ection_class)...
-000002d0: 7365 6c66 720d 0000 00da 0461 7267 73da  selfr......args.
-000002e0: 066b 7761 7267 7329 0172 0f00 0000 a900  .kwargs).r......
-000002f0: fa53 2f55 7365 7273 2f61 6e64 7265 7962  .S/Users/andreyb
-00000300: 6f6e 6461 722f 5079 4368 6172 6d50 726f  ondar/PyCharmPro
-00000310: 6a65 6374 732f 746f 7274 6f69 7365 2d6f  jects/tortoise-o
-00000320: 726d 2f74 6f72 746f 6973 652f 6261 636b  rm/tortoise/back
-00000330: 656e 6473 2f73 716c 6974 652f 636c 6965  ends/sqlite/clie
-00000340: 6e74 2e70 7972 0c00 0000 1200 0000 730c  nt.pyr........s.
-00000350: 0000 0000 010e 0106 0102 0112 0202 017a  ...............z
-00000360: 1553 716c 6974 6543 6c69 656e 742e 5f5f  .SqliteClient.__
-00000370: 696e 6974 5f5f 6301 0000 0000 0000 0001  init__c.........
-00000380: 0000 0001 0000 00c3 0000 0073 0400 0000  ...........s....
-00000390: 6400 5300 2901 4e72 1500 0000 2901 7212  d.S.).Nr....).r.
-000003a0: 0000 0072 1500 0000 7215 0000 0072 1600  ...r....r....r..
-000003b0: 0000 da11 6372 6561 7465 5f63 6f6e 6e65  ....create_conne
-000003c0: 6374 696f 6e1c 0000 0073 0200 0000 0001  ction....s......
-000003d0: 7a1e 5371 6c69 7465 436c 6965 6e74 2e63  z.SqliteClient.c
-000003e0: 7265 6174 655f 636f 6e6e 6563 7469 6f6e  reate_connection
-000003f0: 6301 0000 0000 0000 0001 0000 0001 0000  c...............
-00000400: 00c3 0000 0073 0400 0000 6400 5300 2901  .....s....d.S.).
-00000410: 4e72 1500 0000 2901 7212 0000 0072 1500  Nr....).r....r..
-00000420: 0000 7215 0000 0072 1600 0000 da05 636c  ..r....r......cl
-00000430: 6f73 651f 0000 0073 0200 0000 0001 7a12  ose....s......z.
-00000440: 5371 6c69 7465 436c 6965 6e74 2e63 6c6f  SqliteClient.clo
-00000450: 7365 6301 0000 0000 0000 0001 0000 0002  sec.............
-00000460: 0000 00c3 0000 0073 1a00 0000 7400 6a01  .......s....t.j.
-00000470: 6a02 7c00 6a03 8301 7216 7404 6401 8301  j.|.j...r.t.d...
-00000480: 8201 6400 5300 2902 4e7a 2b44 4220 6361  ..d.S.).Nz+DB ca
-00000490: 6e6e 6f74 2062 6520 6372 6561 7465 642c  nnot be created,
-000004a0: 2061 7320 6974 2061 6c72 6561 6479 2065   as it already e
-000004b0: 7869 7374 732e 2905 da02 6f73 da04 7061  xists.)...os..pa
-000004c0: 7468 da06 6973 6669 6c65 720d 0000 0072  th..isfiler....r
-000004d0: 0800 0000 2901 7212 0000 0072 1500 0000  ....).r....r....
-000004e0: 7215 0000 0072 1600 0000 da09 6462 5f63  r....r......db_c
-000004f0: 7265 6174 6522 0000 0073 0400 0000 0001  reate"...s......
-00000500: 0e01 7a16 5371 6c69 7465 436c 6965 6e74  ..z.SqliteClient
-00000510: 2e64 625f 6372 6561 7465 6301 0000 0000  .db_createc.....
-00000520: 0000 0001 0000 000b 0000 00c3 0000 0073  ...............s
-00000530: 2a00 0000 7910 7400 6a01 7c00 6a02 8301  *...y.t.j.|.j...
-00000540: 0100 5700 6e14 0400 7403 6b0a 7224 0100  ..W.n...t.k.r$..
-00000550: 0100 0100 5900 6e02 5800 6400 5300 2901  ....Y.n.X.d.S.).
-00000560: 4e29 0472 1900 0000 da06 7265 6d6f 7665  N).r......remove
-00000570: 720d 0000 00da 1146 696c 654e 6f74 466f  r......FileNotFo
-00000580: 756e 6445 7272 6f72 2901 7212 0000 0072  undError).r....r
-00000590: 1500 0000 7215 0000 0072 1600 0000 da09  ....r....r......
-000005a0: 6462 5f64 656c 6574 6526 0000 0073 0800  db_delete&...s..
-000005b0: 0000 0001 0201 1001 0e01 7a16 5371 6c69  ..........z.Sqli
-000005c0: 7465 436c 6965 6e74 2e64 625f 6465 6c65  teClient.db_dele
-000005d0: 7465 6301 0000 0000 0000 0002 0000 0002  tec.............
-000005e0: 0000 0043 0000 0073 1000 0000 7400 6a01  ...C...s....t.j.
-000005f0: 7c00 6a02 8301 7d01 7c01 5300 2901 4e29  |.j...}.|.S.).N)
-00000600: 03da 0961 696f 7371 6c69 7465 da07 636f  ...aiosqlite..co
-00000610: 6e6e 6563 7472 0d00 0000 2902 7212 0000  nnectr....).r...
-00000620: 00da 0a63 6f6e 6e65 6374 696f 6e72 1500  ...connectionr..
-00000630: 0000 7215 0000 0072 1600 0000 da12 6163  ..r....r......ac
-00000640: 7175 6972 655f 636f 6e6e 6563 7469 6f6e  quire_connection
-00000650: 2c00 0000 7304 0000 0000 010c 017a 1f53  ,...s........z.S
-00000660: 716c 6974 6543 6c69 656e 742e 6163 7175  qliteClient.acqu
-00000670: 6972 655f 636f 6e6e 6563 7469 6f6e 6301  ire_connectionc.
-00000680: 0000 0000 0000 0001 0000 0003 0000 0043  ...............C
-00000690: 0000 0073 1400 0000 7c00 6a00 7401 6a02  ...s....|.j.t.j.
-000006a0: 7c00 6a03 8301 6401 8d01 5300 2902 4e29  |.j...d...S.).N)
-000006b0: 0172 2200 0000 2904 7210 0000 0072 2000  .r"...).r....r .
-000006c0: 0000 7221 0000 0072 0d00 0000 2901 7212  ..r!...r....).r.
-000006d0: 0000 0072 1500 0000 7215 0000 0072 1600  ...r....r....r..
-000006e0: 0000 da0e 696e 5f74 7261 6e73 6163 7469  ....in_transacti
-000006f0: 6f6e 3000 0000 7302 0000 0000 017a 1b53  on0...s......z.S
-00000700: 716c 6974 6543 6c69 656e 742e 696e 5f74  qliteClient.in_t
-00000710: 7261 6e73 6163 7469 6f6e 4663 0300 0000  ransactionFc....
-00000720: 0000 0000 0800 0000 1000 0000 c300 0000  ................
-00000730: 73f6 0000 007c 006a 006a 017c 0183 0101  s....|.j.j.|....
-00000740: 0079 8e7c 006a 0283 0034 0049 0064 0048  .y.|.j...4.I.d.H
-00000750: 009a 6e7d 0374 036a 047c 036a 055f 067c  ..n}.t.j.|.j._.|
-00000760: 036a 077c 0183 0149 0064 0048 007d 047c  .j.|...I.d.H.}.|
-00000770: 006a 087c 0383 0149 0064 0048 0001 007c  .j.|...I.d.H...|
-00000780: 046a 0983 0049 0064 0048 007d 057c 0272  .j...I.d.H.}.|.r
-00000790: 7e7c 046a 0764 0183 0149 0064 0048 0001  ~|.j.d...I.d.H..
-000007a0: 007c 046a 0a83 0049 0064 0048 007d 067c  .|.j...I.d.H.}.|
-000007b0: 0653 0064 0264 0384 007c 0544 0083 0153  .S.d.d...|.D...S
-000007c0: 0051 0049 0064 0048 0052 0058 0057 006e  .Q.I.d.H.R.X.W.n
-000007d0: 5604 0074 036a 0b6b 0a72 c601 007d 0701  V..t.j.k.r...}..
-000007e0: 007a 0e74 0b7c 0783 0182 0157 0059 0064  .z.t.|.....W.Y.d
-000007f0: 0064 007d 077e 0758 006e 2c04 0074 036a  .d.}.~.X.n,..t.j
-00000800: 0c6b 0a72 f001 007d 0701 007a 0e74 0c7c  .k.r...}...z.t.|
-00000810: 0783 0182 0157 0059 0064 0064 007d 077e  .....W.Y.d.d.}.~
-00000820: 0758 006e 0258 0064 0053 0029 044e 7a1a  .X.n.X.d.S.).Nz.
-00000830: 5345 4c45 4354 206c 6173 745f 696e 7365  SELECT last_inse
-00000840: 7274 5f72 6f77 6964 2829 6301 0000 0000  rt_rowid()c.....
-00000850: 0000 0002 0000 0004 0000 0053 0000 0073  ...........S...s
-00000860: 1400 0000 6700 7c00 5d0c 7d01 7400 7c01  ....g.|.].}.t.|.
-00000870: 8301 9102 7104 5300 7215 0000 0029 01da  ....q.S.r....)..
-00000880: 0464 6963 7429 02da 022e 30da 0372 6f77  .dict)....0..row
-00000890: 7215 0000 0072 1500 0000 7216 0000 00fa  r....r....r.....
-000008a0: 0a3c 6c69 7374 636f 6d70 3e3f 0000 0073  .<listcomp>?...s
-000008b0: 0200 0000 0600 7a2e 5371 6c69 7465 436c  ......z.SqliteCl
-000008c0: 6965 6e74 2e65 7865 6375 7465 5f71 7565  ient.execute_que
-000008d0: 7279 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973  ry.<locals>.<lis
-000008e0: 7463 6f6d 703e 290d da03 6c6f 67da 0564  tcomp>)...log..d
-000008f0: 6562 7567 7223 0000 00da 0773 716c 6974  ebugr#.....sqlit
-00000900: 6533 da03 526f 77da 055f 636f 6e6e da0b  e3..Row.._conn..
-00000910: 726f 775f 6661 6374 6f72 79da 0765 7865  row_factory..exe
-00000920: 6375 7465 da07 5f63 6f6d 6d69 74da 0866  cute.._commit..f
-00000930: 6574 6368 616c 6cda 0866 6574 6368 6f6e  etchall..fetchon
-00000940: 6572 0800 0000 7207 0000 0029 0872 1200  er....r....).r..
-00000950: 0000 da05 7175 6572 795a 0f67 6574 5f69  ....queryZ.get_i
-00000960: 6e73 6572 7465 645f 6964 7222 0000 00da  nserted_idr"....
-00000970: 0663 7572 736f 72da 0772 6573 756c 7473  .cursor..results
-00000980: 5a0b 696e 7365 7274 6564 5f69 64da 0365  Z.inserted_id..e
-00000990: 7863 7215 0000 0072 1500 0000 7216 0000  xcr....r....r...
-000009a0: 00da 0d65 7865 6375 7465 5f71 7565 7279  ...execute_query
-000009b0: 3300 0000 7320 0000 0000 010c 0102 0112  3...s ..........
-000009c0: 010a 0110 0110 010e 0104 0110 010e 0104  ................
-000009d0: 011e 0112 0118 0112 017a 1a53 716c 6974  .........z.Sqlit
-000009e0: 6543 6c69 656e 742e 6578 6563 7574 655f  eClient.execute_
-000009f0: 7175 6572 7963 0200 0000 0000 0000 0300  queryc..........
-00000a00: 0000 0a00 0000 c300 0000 7342 0000 007c  ..........sB...|
-00000a10: 006a 0083 0034 0049 0064 0048 009a 227d  .j...4.I.d.H.."}
-00000a20: 027c 006a 016a 027c 0183 0101 007c 026a  .|.j.j.|.....|.j
-00000a30: 037c 0183 0149 0064 0048 0001 0057 0064  .|...I.d.H...W.d
-00000a40: 0051 0049 0064 0048 0052 0058 0064 0053  .Q.I.d.H.R.X.d.S
-00000a50: 0029 014e 2904 7223 0000 0072 2900 0000  .).N).r#...r)...
-00000a60: 722a 0000 00da 0d65 7865 6375 7465 7363  r*.....executesc
-00000a70: 7269 7074 2903 7212 0000 00da 0673 6372  ript).r......scr
-00000a80: 6970 7472 2200 0000 7215 0000 0072 1500  iptr"...r....r..
-00000a90: 0000 7216 0000 00da 0e65 7865 6375 7465  ..r......execute
-00000aa0: 5f73 6372 6970 7445 0000 0073 0600 0000  _scriptE...s....
-00000ab0: 0001 1201 0c01 7a1b 5371 6c69 7465 436c  ......z.SqliteCl
-00000ac0: 6965 6e74 2e65 7865 6375 7465 5f73 6372  ient.execute_scr
-00000ad0: 6970 7463 0100 0000 0000 0000 0200 0000  iptc............
-00000ae0: 0300 0000 c300 0000 732e 0000 0074 006a  ........s....t.j
-00000af0: 017c 006a 0283 017d 017c 016a 0383 0001  .|.j...}.|.j....
-00000b00: 007c 016a 0483 0049 0064 0048 0001 007c  .|.j...I.d.H...|
-00000b10: 006a 057c 017c 0083 0253 0029 014e 2906  .j.|.|...S.).N).
-00000b20: 7220 0000 0072 2100 0000 720d 0000 00da  r ...r!...r.....
-00000b30: 0573 7461 7274 da08 5f63 6f6e 6e65 6374  .start.._connect
-00000b40: 7211 0000 0029 0272 1200 0000 7222 0000  r....).r....r"..
-00000b50: 0072 1500 0000 7215 0000 0072 1600 0000  .r....r....r....
-00000b60: da15 6765 745f 7369 6e67 6c65 5f63 6f6e  ..get_single_con
-00000b70: 6e65 6374 696f 6e4a 0000 0073 0800 0000  nectionJ...s....
-00000b80: 0001 0c01 0801 0e01 7a22 5371 6c69 7465  ........z"Sqlite
-00000b90: 436c 6965 6e74 2e67 6574 5f73 696e 676c  Client.get_singl
-00000ba0: 655f 636f 6e6e 6563 7469 6f6e 6302 0000  e_connectionc...
-00000bb0: 0000 0000 0002 0000 0002 0000 00c3 0000  ................
-00000bc0: 0073 1400 0000 7c01 6a00 6a01 8300 4900  .s....|.j.j...I.
-00000bd0: 6400 4800 0100 6400 5300 2901 4e29 0272  d.H...d.S.).N).r
-00000be0: 2200 0000 7218 0000 0029 0272 1200 0000  "...r....).r....
-00000bf0: da11 7369 6e67 6c65 5f63 6f6e 6e65 6374  ..single_connect
-00000c00: 696f 6e72 1500 0000 7215 0000 0072 1600  ionr....r....r..
-00000c10: 0000 da19 7265 6c65 6173 655f 7369 6e67  ....release_sing
-00000c20: 6c65 5f63 6f6e 6e65 6374 696f 6e50 0000  le_connectionP..
-00000c30: 0073 0200 0000 0001 7a26 5371 6c69 7465  .s......z&Sqlite
-00000c40: 436c 6965 6e74 2e72 656c 6561 7365 5f73  Client.release_s
-00000c50: 696e 676c 655f 636f 6e6e 6563 7469 6f6e  ingle_connection
-00000c60: 6302 0000 0000 0000 0002 0000 0002 0000  c...............
-00000c70: 00c3 0000 0073 1200 0000 7c01 6a00 8300  .....s....|.j...
-00000c80: 4900 6400 4800 0100 6400 5300 2901 4e29  I.d.H...d.S.).N)
-00000c90: 01da 0663 6f6d 6d69 7429 0272 1200 0000  ...commit).r....
-00000ca0: 7222 0000 0072 1500 0000 7215 0000 0072  r"...r....r....r
-00000cb0: 1600 0000 7230 0000 0053 0000 0073 0200  ....r0...S...s..
-00000cc0: 0000 0001 7a14 5371 6c69 7465 436c 6965  ....z.SqliteClie
-00000cd0: 6e74 2e5f 636f 6d6d 6974 2901 4629 14da  nt._commit).F)..
-00000ce0: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
-00000cf0: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
-00000d00: 655f 5f72 0500 0000 da0e 6578 6563 7574  e__r......execut
-00000d10: 6f72 5f63 6c61 7373 7206 0000 00da 1073  or_classr......s
-00000d20: 6368 656d 615f 6765 6e65 7261 746f 7272  chema_generatorr
-00000d30: 0c00 0000 7217 0000 0072 1800 0000 721c  ....r....r....r.
-00000d40: 0000 0072 1f00 0000 7223 0000 0072 2400  ...r....r#...r$.
-00000d50: 0000 7237 0000 0072 3a00 0000 723d 0000  ..r7...r:...r=..
-00000d60: 0072 3f00 0000 7230 0000 00da 0d5f 5f63  .r?...r0.....__c
-00000d70: 6c61 7373 6365 6c6c 5f5f 7215 0000 0072  lasscell__r....r
-00000d80: 1500 0000 2901 720f 0000 0072 1600 0000  ....).r....r....
-00000d90: 7209 0000 000e 0000 0073 1c00 0000 0801  r........s......
-00000da0: 0401 0402 0c0a 0803 0803 0804 0806 0804  ................
-00000db0: 0803 0a12 0805 0806 0803 7209 0000 0063  ..........r....c
-00000dc0: 0000 0000 0000 0000 0000 0000 0200 0000  ................
-00000dd0: 4000 0000 735c 0000 0065 005a 0164 005a  @...s\...e.Z.d.Z
-00000de0: 0264 0164 0284 005a 0364 0364 0484 005a  .d.d...Z.d.d...Z
-00000df0: 0464 0564 0684 005a 0564 0764 0884 005a  .d.d...Z.d.d...Z
-00000e00: 0664 0964 0a84 005a 0764 0b64 0c84 005a  .d.d...Z.d.d...Z
-00000e10: 0864 0d64 0e84 005a 0964 0f64 1084 005a  .d.d...Z.d.d...Z
-00000e20: 0a64 1164 1284 005a 0b64 1364 1484 005a  .d.d...Z.d.d...Z
-00000e30: 0c64 1553 0029 1672 0a00 0000 6302 0000  .d.S.).r....c...
-00000e40: 0000 0000 0002 0000 0004 0000 0043 0000  .............C..
-00000e50: 0073 3800 0000 7c01 7c00 5f00 7401 6a02  .s8...|.|._.t.j.
-00000e60: 6401 8301 7c00 5f03 6402 7c00 5f04 7405  d...|._.d.|._.t.
-00000e70: 6403 7406 7c00 6a07 6602 6900 8303 7c00  d.t.|.j.f.i...|.
-00000e80: 5f08 7c00 6a07 7c00 5f09 6400 5300 2904  _.|.j.|._.d.S.).
-00000e90: 4eda 0964 625f 636c 6965 6e74 5472 0400  N..db_clientTr..
-00000ea0: 0000 290a da0b 5f63 6f6e 6e65 6374 696f  ..)..._connectio
-00000eb0: 6eda 076c 6f67 6769 6e67 da09 6765 744c  n..logging..getL
-00000ec0: 6f67 6765 7272 2900 0000 723e 0000 0072  oggerr)...r>...r
-00000ed0: 0e00 0000 7204 0000 0072 0f00 0000 7211  ....r....r....r.
-00000ee0: 0000 0072 1000 0000 2902 7212 0000 0072  ...r....).r....r
-00000ef0: 2200 0000 7215 0000 0072 1500 0000 7216  "...r....r....r.
-00000f00: 0000 0072 0c00 0000 5800 0000 730c 0000  ...r....X...s...
-00000f10: 0000 0106 010c 0106 0102 0112 027a 1b54  .............z.T
-00000f20: 7261 6e73 6163 7469 6f6e 5772 6170 7065  ransactionWrappe
-00000f30: 722e 5f5f 696e 6974 5f5f 6301 0000 0000  r.__init__c.....
-00000f40: 0000 0001 0000 0002 0000 0043 0000 0073  ...........C...s
-00000f50: 0a00 0000 7400 7c00 6a01 8301 5300 2901  ....t.|.j...S.).
-00000f60: 4e29 0272 0300 0000 7248 0000 0029 0172  N).r....rH...).r
-00000f70: 1200 0000 7215 0000 0072 1500 0000 7216  ....r....r....r.
-00000f80: 0000 0072 2300 0000 6100 0000 7302 0000  ...r#...a...s...
-00000f90: 0000 017a 2554 7261 6e73 6163 7469 6f6e  ...z%Transaction
-00000fa0: 5772 6170 7065 722e 6163 7175 6972 655f  Wrapper.acquire_
-00000fb0: 636f 6e6e 6563 7469 6f6e 6301 0000 0000  connectionc.....
-00000fc0: 0000 0001 0000 0003 0000 00c3 0000 0073  ...............s
-00000fd0: 0e00 0000 7c00 6a00 7c00 6a01 7c00 8302  ....|.j.|.j.|...
-00000fe0: 5300 2901 4e29 0272 1100 0000 7248 0000  S.).N).r....rH..
-00000ff0: 0029 0172 1200 0000 7215 0000 0072 1500  .).r....r....r..
-00001000: 0000 7216 0000 0072 3d00 0000 6400 0000  ..r....r=...d...
-00001010: 7302 0000 0000 017a 2854 7261 6e73 6163  s......z(Transac
-00001020: 7469 6f6e 5772 6170 7065 722e 6765 745f  tionWrapper.get_
-00001030: 7369 6e67 6c65 5f63 6f6e 6e65 6374 696f  single_connectio
-00001040: 6e63 0200 0000 0000 0000 0200 0000 0100  nc..............
-00001050: 0000 c300 0000 7304 0000 0064 0053 0029  ......s....d.S.)
-00001060: 014e 7215 0000 0029 0272 1200 0000 723e  .Nr....).r....r>
-00001070: 0000 0072 1500 0000 7215 0000 0072 1600  ...r....r....r..
-00001080: 0000 723f 0000 0067 0000 0073 0200 0000  ..r?...g...s....
-00001090: 0001 7a2c 5472 616e 7361 6374 696f 6e57  ..z,TransactionW
-000010a0: 7261 7070 6572 2e72 656c 6561 7365 5f73  rapper.release_s
-000010b0: 696e 676c 655f 636f 6e6e 6563 7469 6f6e  ingle_connection
-000010c0: 6301 0000 0000 0000 0001 0000 0002 0000  c...............
-000010d0: 00c3 0000 0073 1e00 0000 7c00 6a00 6a01  .....s....|.j.j.
-000010e0: 8300 0100 7c00 6a00 6a02 8300 4900 6400  ....|.j.j...I.d.
-000010f0: 4800 0100 6400 5300 2901 4e29 0372 4800  H...d.S.).N).rH.
-00001100: 0000 723b 0000 0072 3c00 0000 2901 7212  ..r;...r<...).r.
-00001110: 0000 0072 1500 0000 7215 0000 0072 1600  ...r....r....r..
-00001120: 0000 723b 0000 006a 0000 0073 0400 0000  ..r;...j...s....
-00001130: 0001 0a01 7a18 5472 616e 7361 6374 696f  ....z.Transactio
-00001140: 6e57 7261 7070 6572 2e73 7461 7274 6301  nWrapper.startc.
-00001150: 0000 0000 0000 0001 0000 0002 0000 00c3  ................
-00001160: 0000 0073 2400 0000 7c00 6a00 6a01 8300  ...s$...|.j.j...
-00001170: 4900 6400 4800 0100 7c00 6a00 6a02 8300  I.d.H...|.j.j...
-00001180: 4900 6400 4800 0100 6400 5300 2901 4e29  I.d.H...d.S.).N)
-00001190: 0372 4800 0000 da08 726f 6c6c 6261 636b  .rH.....rollback
-000011a0: 7218 0000 0029 0172 1200 0000 7215 0000  r....).r....r...
-000011b0: 0072 1500 0000 7216 0000 0072 4b00 0000  .r....r....rK...
-000011c0: 6e00 0000 7304 0000 0000 0110 017a 1b54  n...s........z.T
-000011d0: 7261 6e73 6163 7469 6f6e 5772 6170 7065  ransactionWrappe
-000011e0: 722e 726f 6c6c 6261 636b 6301 0000 0000  r.rollbackc.....
-000011f0: 0000 0001 0000 0002 0000 00c3 0000 0073  ...............s
-00001200: 2400 0000 7c00 6a00 6a01 8300 4900 6400  $...|.j.j...I.d.
-00001210: 4800 0100 7c00 6a00 6a02 8300 4900 6400  H...|.j.j...I.d.
-00001220: 4800 0100 6400 5300 2901 4e29 0372 4800  H...d.S.).N).rH.
-00001230: 0000 7240 0000 0072 1800 0000 2901 7212  ..r@...r....).r.
+00000020: 0073 bc00 0000 6400 0064 0100 6c00 005a  .s....d..d..l..Z
+00000030: 0000 6400 0064 0100 6c01 005a 0100 6400  ..d..d..l..Z..d.
+00000040: 0064 0100 6c02 005a 0200 6400 0064 0100  .d..l..Z..d..d..
+00000050: 6c03 005a 0300 6400 0064 0200 6c04 006d  l..Z..d..d..l..m
+00000060: 0500 5a05 0001 6400 0064 0300 6c06 006d  ..Z...d..d..l..m
+00000070: 0700 5a07 006d 0800 5a08 0001 6400 0064  ..Z..m..Z...d..d
+00000080: 0400 6c09 006d 0a00 5a0a 0001 6400 0064  ..l..m..Z...d..d
+00000090: 0500 6c0b 006d 0c00 5a0c 0001 6400 0064  ..l..m..Z...d..d
+000000a0: 0600 6c0d 006d 0e00 5a0e 006d 0f00 5a0f  ..l..m..Z..m..Z.
+000000b0: 0001 4764 0700 6408 0084 0000 6408 0065  ..Gd..d.....d..e
+000000c0: 0500 8303 005a 1000 4764 0900 640a 0084  .....Z..Gd..d...
+000000d0: 0000 640a 0065 1000 8303 005a 1100 6401  ..d..e.....Z..d.
+000000e0: 0053 290b e900 0000 004e 2901 da11 4261  .S)......N)...Ba
+000000f0: 7365 4442 4173 796e 6343 6c69 656e 7429  seDBAsyncClient)
+00000100: 02da 1143 6f6e 6e65 6374 696f 6e57 7261  ...ConnectionWra
+00000110: 7070 6572 da17 5369 6e67 6c65 436f 6e6e  pper..SingleConn
+00000120: 6563 7469 6f6e 5772 6170 7065 7229 01da  ectionWrapper)..
+00000130: 0e53 716c 6974 6545 7865 6375 746f 7229  .SqliteExecutor)
+00000140: 01da 1553 716c 6974 6553 6368 656d 6147  ...SqliteSchemaG
+00000150: 656e 6572 6174 6f72 2902 da0e 496e 7465  enerator)...Inte
+00000160: 6772 6974 7945 7272 6f72 da10 4f70 6572  grityError..Oper
+00000170: 6174 696f 6e61 6c45 7272 6f72 6300 0000  ationalErrorc...
+00000180: 0000 0000 0000 0000 0003 0000 0000 0000  ................
+00000190: 0073 b500 0000 6500 005a 0100 6400 005a  .s....e..Z..d..Z
+000001a0: 0200 6503 005a 0400 6505 005a 0600 8700  ..e..Z..e..Z....
+000001b0: 0066 0100 6401 0064 0200 8600 005a 0700  .f..d..d.....Z..
+000001c0: 6403 0064 0400 8400 005a 0800 6405 0064  d..d.....Z..d..d
+000001d0: 0600 8400 005a 0900 6407 0064 0800 8400  .....Z..d..d....
+000001e0: 005a 0a00 6409 0064 0a00 8400 005a 0b00  .Z..d..d.....Z..
+000001f0: 640b 0064 0c00 8400 005a 0c00 640d 0064  d..d.....Z..d..d
+00000200: 0e00 8400 005a 0d00 640f 0064 1000 6411  .....Z..d..d..d.
+00000210: 0084 0100 5a0e 0064 1200 6413 0084 0000  ....Z..d..d.....
+00000220: 5a0f 0064 1400 6415 0084 0000 5a10 0064  Z..d..d.....Z..d
+00000230: 1600 6417 0084 0000 5a11 0064 1800 6419  ..d.....Z..d..d.
+00000240: 0084 0000 5a12 0087 0000 5329 1ada 0c53  ....Z.....S)...S
+00000250: 716c 6974 6543 6c69 656e 7463 0200 0000  qliteClientc....
+00000260: 0000 0000 0400 0000 0400 0000 0f00 0000  ................
+00000270: 735c 0000 0074 0000 8300 006a 0100 7c02  s\...t.....j..|.
+00000280: 007c 0300 8e00 0001 7c01 007c 0000 5f02  .|......|..|.._.
+00000290: 0074 0300 6401 0074 0400 7c00 006a 0500  .t..d..t..|..j..
+000002a0: 6602 0069 0000 8303 007c 0000 5f06 0074  f..i.....|.._..t
+000002b0: 0300 6402 0074 0700 7c00 006a 0500 6602  ..d..t..|..j..f.
+000002c0: 0069 0000 8303 007c 0000 5f08 0064 0000  .i.....|.._..d..
+000002d0: 5329 034e da12 5472 616e 7361 6374 696f  S).N..Transactio
+000002e0: 6e57 7261 7070 6572 7204 0000 0029 09da  nWrapperr....)..
+000002f0: 0573 7570 6572 da08 5f5f 696e 6974 5f5f  .super..__init__
+00000300: da08 6669 6c65 6e61 6d65 da04 7479 7065  ..filename..type
+00000310: 720a 0000 00da 095f 5f63 6c61 7373 5f5f  r......__class__
+00000320: da12 5f74 7261 6e73 6163 7469 6f6e 5f63  .._transaction_c
+00000330: 6c61 7373 7204 0000 00da 185f 7369 6e67  lassr......_sing
+00000340: 6c65 5f63 6f6e 6e65 6374 696f 6e5f 636c  le_connection_cl
+00000350: 6173 7329 04da 0473 656c 6672 0d00 0000  ass)...selfr....
+00000360: da04 6172 6773 da06 6b77 6172 6773 2901  ..args..kwargs).
+00000370: 720f 0000 00a9 00fa 532f 5573 6572 732f  r.......S/Users/
+00000380: 616e 6472 6579 626f 6e64 6172 2f50 7943  andreybondar/PyC
+00000390: 6861 726d 5072 6f6a 6563 7473 2f74 6f72  harmProjects/tor
+000003a0: 746f 6973 652d 6f72 6d2f 746f 7274 6f69  toise-orm/tortoi
+000003b0: 7365 2f62 6163 6b65 6e64 732f 7371 6c69  se/backends/sqli
+000003c0: 7465 2f63 6c69 656e 742e 7079 720c 0000  te/client.pyr...
+000003d0: 0012 0000 0073 0c00 0000 0001 1301 0901  .....s..........
+000003e0: 0301 1b02 0301 7a15 5371 6c69 7465 436c  ......z.SqliteCl
+000003f0: 6965 6e74 2e5f 5f69 6e69 745f 5f63 0100  ient.__init__c..
+00000400: 0000 0000 0000 0100 0000 0100 0000 c300  ................
+00000410: 0000 7304 0000 0064 0000 5329 014e 7215  ..s....d..S).Nr.
+00000420: 0000 0029 0172 1200 0000 7215 0000 0072  ...).r....r....r
+00000430: 1500 0000 7216 0000 00da 1163 7265 6174  ....r......creat
+00000440: 655f 636f 6e6e 6563 7469 6f6e 1c00 0000  e_connection....
+00000450: 7302 0000 0000 017a 1e53 716c 6974 6543  s......z.SqliteC
+00000460: 6c69 656e 742e 6372 6561 7465 5f63 6f6e  lient.create_con
+00000470: 6e65 6374 696f 6e63 0100 0000 0000 0000  nectionc........
+00000480: 0100 0000 0100 0000 c300 0000 7304 0000  ............s...
+00000490: 0064 0000 5329 014e 7215 0000 0029 0172  .d..S).Nr....).r
+000004a0: 1200 0000 7215 0000 0072 1500 0000 7216  ....r....r....r.
+000004b0: 0000 00da 0563 6c6f 7365 1f00 0000 7302  .....close....s.
+000004c0: 0000 0000 017a 1253 716c 6974 6543 6c69  .....z.SqliteCli
+000004d0: 656e 742e 636c 6f73 6563 0100 0000 0000  ent.closec......
+000004e0: 0000 0100 0000 0200 0000 c300 0000 7325  ..............s%
+000004f0: 0000 0074 0000 6a01 006a 0200 7c00 006a  ...t..j..j..|..j
+00000500: 0300 8301 0072 2100 7404 0064 0100 8301  .....r!.t..d....
+00000510: 0082 0100 6400 0053 2902 4e7a 2b44 4220  ....d..S).Nz+DB 
+00000520: 6361 6e6e 6f74 2062 6520 6372 6561 7465  cannot be create
+00000530: 642c 2061 7320 6974 2061 6c72 6561 6479  d, as it already
+00000540: 2065 7869 7374 732e 2905 da02 6f73 da04   exists.)...os..
+00000550: 7061 7468 da06 6973 6669 6c65 720d 0000  path..isfiler...
+00000560: 0072 0800 0000 2901 7212 0000 0072 1500  .r....).r....r..
+00000570: 0000 7215 0000 0072 1600 0000 da09 6462  ..r....r......db
+00000580: 5f63 7265 6174 6522 0000 0073 0400 0000  _create"...s....
+00000590: 0001 1501 7a16 5371 6c69 7465 436c 6965  ....z.SqliteClie
+000005a0: 6e74 2e64 625f 6372 6561 7465 6301 0000  nt.db_createc...
+000005b0: 0000 0000 0001 0000 000b 0000 00c3 0000  ................
+000005c0: 0073 2d00 0000 7914 0074 0000 6a01 007c  .s-...y..t..j..|
+000005d0: 0000 6a02 0083 0100 0157 6e12 0004 7403  ..j......Wn...t.
+000005e0: 006b 0a00 7228 0001 0101 596e 0100 5864  .k..r(....Yn..Xd
+000005f0: 0000 5329 014e 2904 7219 0000 00da 0672  ..S).N).r......r
+00000600: 656d 6f76 6572 0d00 0000 da11 4669 6c65  emover......File
+00000610: 4e6f 7446 6f75 6e64 4572 726f 7229 0172  NotFoundError).r
+00000620: 1200 0000 7215 0000 0072 1500 0000 7216  ....r....r....r.
+00000630: 0000 00da 0964 625f 6465 6c65 7465 2600  .....db_delete&.
+00000640: 0000 7308 0000 0000 0103 0114 010d 017a  ..s............z
+00000650: 1653 716c 6974 6543 6c69 656e 742e 6462  .SqliteClient.db
+00000660: 5f64 656c 6574 6563 0100 0000 0000 0000  _deletec........
+00000670: 0200 0000 0200 0000 4300 0000 7316 0000  ........C...s...
+00000680: 0074 0000 6a01 007c 0000 6a02 0083 0100  .t..j..|..j.....
+00000690: 7d01 007c 0100 5329 014e 2903 da09 6169  }..|..S).N)...ai
+000006a0: 6f73 716c 6974 65da 0763 6f6e 6e65 6374  osqlite..connect
+000006b0: 720d 0000 0029 0272 1200 0000 da0a 636f  r....).r......co
+000006c0: 6e6e 6563 7469 6f6e 7215 0000 0072 1500  nnectionr....r..
+000006d0: 0000 7216 0000 00da 1261 6371 7569 7265  ..r......acquire
+000006e0: 5f63 6f6e 6e65 6374 696f 6e2c 0000 0073  _connection,...s
+000006f0: 0400 0000 0001 1201 7a1f 5371 6c69 7465  ........z.Sqlite
+00000700: 436c 6965 6e74 2e61 6371 7569 7265 5f63  Client.acquire_c
+00000710: 6f6e 6e65 6374 696f 6e63 0100 0000 0000  onnectionc......
+00000720: 0000 0100 0000 0400 0000 4300 0000 731c  ..........C...s.
+00000730: 0000 007c 0000 6a00 0064 0100 7401 006a  ...|..j..d..t..j
+00000740: 0200 7c00 006a 0300 8301 0083 0001 5329  ..|..j........S)
+00000750: 024e 7222 0000 0029 0472 1000 0000 7220  .Nr"...).r....r 
+00000760: 0000 0072 2100 0000 720d 0000 0029 0172  ...r!...r....).r
+00000770: 1200 0000 7215 0000 0072 1500 0000 7216  ....r....r....r.
+00000780: 0000 00da 0e69 6e5f 7472 616e 7361 6374  .....in_transact
+00000790: 696f 6e30 0000 0073 0200 0000 0001 7a1b  ion0...s......z.
+000007a0: 5371 6c69 7465 436c 6965 6e74 2e69 6e5f  SqliteClient.in_
+000007b0: 7472 616e 7361 6374 696f 6e46 6303 0000  transactionFc...
+000007c0: 0000 0000 0008 0000 0010 0000 00e3 0000  ................
+000007d0: 0073 2701 0000 7c00 006a 0000 6a01 007c  .s'...|..j..j..|
+000007e0: 0100 8301 0001 79a9 007c 0000 6a02 0083  ......y..|..j...
+000007f0: 0000 3449 6400 0048 9a8b 007d 0300 7403  ..4Id..H...}..t.
+00000800: 006a 0400 7c03 006a 0500 5f06 007c 0300  .j..|..j.._..|..
+00000810: 6a07 007c 0100 8301 0049 6400 0048 7d04  j..|.....Id..H}.
+00000820: 007c 0000 6a08 007c 0300 8301 0049 6400  .|..j..|.....Id.
+00000830: 0048 017c 0400 6a09 0083 0000 4964 0000  .H.|..j.....Id..
+00000840: 487d 0500 7c02 0072 9b00 7c04 006a 0700  H}..|..r..|..j..
+00000850: 6401 0083 0100 4964 0000 4801 7c04 006a  d.....Id..H.|..j
+00000860: 0a00 8300 0049 6400 0048 7d06 007c 0600  .....Id..H}..|..
+00000870: 5364 0200 6403 0084 0000 7c05 0044 8301  Sd..d.....|..D..
+00000880: 0053 5764 0000 5149 6400 0048 5258 576e  .SWd..QId..HRXWn
+00000890: 6700 0474 0300 6a0b 006b 0a00 72ef 0001  g..t..j..k..r...
+000008a0: 7d07 0001 7a11 0074 0b00 7c07 0083 0100  }...z..t..|.....
+000008b0: 8201 0057 5964 0000 6400 007d 0700 7e07  ...WYd..d..}..~.
+000008c0: 0058 6e34 0004 7403 006a 0c00 6b0a 0072  .Xn4..t..j..k..r
+000008d0: 2201 017d 0700 017a 1100 740c 007c 0700  "..}...z..t..|..
+000008e0: 8301 0082 0100 5759 6400 0064 0000 7d07  ......WYd..d..}.
+000008f0: 007e 0700 586e 0100 5864 0000 5329 044e  .~..Xn..Xd..S).N
+00000900: 7a1a 5345 4c45 4354 206c 6173 745f 696e  z.SELECT last_in
+00000910: 7365 7274 5f72 6f77 6964 2829 6301 0000  sert_rowid()c...
+00000920: 0000 0000 0002 0000 0004 0000 0053 0000  .............S..
+00000930: 0073 1c00 0000 6700 007c 0000 5d12 007d  .s....g..|..]..}
+00000940: 0100 7400 007c 0100 8301 0091 0200 7106  ..t..|........q.
+00000950: 0053 7215 0000 0029 01da 0464 6963 7429  .Sr....)...dict)
+00000960: 02da 022e 30da 0372 6f77 7215 0000 0072  ....0..rowr....r
+00000970: 1500 0000 7216 0000 00fa 0a3c 6c69 7374  ....r......<list
+00000980: 636f 6d70 3e3f 0000 0073 0200 0000 0900  comp>?...s......
+00000990: 7a2e 5371 6c69 7465 436c 6965 6e74 2e65  z.SqliteClient.e
+000009a0: 7865 6375 7465 5f71 7565 7279 2e3c 6c6f  xecute_query.<lo
+000009b0: 6361 6c73 3e2e 3c6c 6973 7463 6f6d 703e  cals>.<listcomp>
+000009c0: 290d da03 6c6f 67da 0564 6562 7567 7223  )...log..debugr#
+000009d0: 0000 00da 0773 716c 6974 6533 da03 526f  .....sqlite3..Ro
+000009e0: 77da 055f 636f 6e6e da0b 726f 775f 6661  w.._conn..row_fa
+000009f0: 6374 6f72 79da 0765 7865 6375 7465 da07  ctory..execute..
+00000a00: 5f63 6f6d 6d69 74da 0866 6574 6368 616c  _commit..fetchal
+00000a10: 6cda 0866 6574 6368 6f6e 6572 0800 0000  l..fetchoner....
+00000a20: 7207 0000 0029 0872 1200 0000 da05 7175  r....).r......qu
+00000a30: 6572 795a 0f67 6574 5f69 6e73 6572 7465  eryZ.get_inserte
+00000a40: 645f 6964 7222 0000 00da 0663 7572 736f  d_idr".....curso
+00000a50: 72da 0772 6573 756c 7473 5a0b 696e 7365  r..resultsZ.inse
+00000a60: 7274 6564 5f69 64da 0365 7863 7215 0000  rted_id..excr...
+00000a70: 0072 1500 0000 7216 0000 00da 0d65 7865  .r....r......exe
+00000a80: 6375 7465 5f71 7565 7279 3300 0000 7320  cute_query3...s 
+00000a90: 0000 0000 0110 0103 0115 010f 0114 0112  ................
+00000aa0: 0111 0106 0112 0111 0104 0121 0115 011e  ...........!....
+00000ab0: 0115 017a 1a53 716c 6974 6543 6c69 656e  ...z.SqliteClien
+00000ac0: 742e 6578 6563 7574 655f 7175 6572 7963  t.execute_queryc
+00000ad0: 0200 0000 0000 0000 0300 0000 0a00 0000  ................
+00000ae0: e300 0000 7347 0000 007c 0000 6a00 0083  ....sG...|..j...
+00000af0: 0000 3449 6400 0048 9a29 007d 0200 7c00  ..4Id..H.).}..|.
+00000b00: 006a 0100 6a02 007c 0100 8301 0001 7c02  .j..j..|......|.
+00000b10: 006a 0300 7c01 0083 0100 4964 0000 4801  .j..|.....Id..H.
+00000b20: 5764 0000 5149 6400 0048 5258 6400 0053  Wd..QId..HRXd..S
+00000b30: 2901 4e29 0472 2300 0000 7229 0000 0072  ).N).r#...r)...r
+00000b40: 2a00 0000 da0d 6578 6563 7574 6573 6372  *.....executescr
+00000b50: 6970 7429 0372 1200 0000 da06 7363 7269  ipt).r......scri
+00000b60: 7074 7222 0000 0072 1500 0000 7215 0000  ptr"...r....r...
+00000b70: 0072 1600 0000 da0e 6578 6563 7574 655f  .r......execute_
+00000b80: 7363 7269 7074 4500 0000 7306 0000 0000  scriptE...s.....
+00000b90: 0115 0110 017a 1b53 716c 6974 6543 6c69  .....z.SqliteCli
+00000ba0: 656e 742e 6578 6563 7574 655f 7363 7269  ent.execute_scri
+00000bb0: 7074 6301 0000 0000 0000 0002 0000 0003  ptc.............
+00000bc0: 0000 00e3 0000 0073 3b00 0000 7400 006a  .......s;...t..j
+00000bd0: 0100 7c00 006a 0200 8301 007d 0100 7c01  ..|..j.....}..|.
+00000be0: 006a 0300 8300 0001 7c01 006a 0400 8300  .j......|..j....
+00000bf0: 0049 6400 0048 017c 0000 6a05 007c 0100  .Id..H.|..j..|..
+00000c00: 7c00 0083 0200 5329 014e 2906 7220 0000  |.....S).N).r ..
+00000c10: 0072 2100 0000 720d 0000 00da 0573 7461  .r!...r......sta
+00000c20: 7274 da08 5f63 6f6e 6e65 6374 7211 0000  rt.._connectr...
+00000c30: 0029 0272 1200 0000 7222 0000 0072 1500  .).r....r"...r..
+00000c40: 0000 7215 0000 0072 1600 0000 da15 6765  ..r....r......ge
+00000c50: 745f 7369 6e67 6c65 5f63 6f6e 6e65 6374  t_single_connect
+00000c60: 696f 6e4a 0000 0073 0800 0000 0001 1201  ionJ...s........
+00000c70: 0a01 0f01 7a22 5371 6c69 7465 436c 6965  ....z"SqliteClie
+00000c80: 6e74 2e67 6574 5f73 696e 676c 655f 636f  nt.get_single_co
+00000c90: 6e6e 6563 7469 6f6e 6302 0000 0000 0000  nnectionc.......
+00000ca0: 0002 0000 0002 0000 00e3 0000 0073 1600  .............s..
+00000cb0: 0000 7c01 006a 0000 6a01 0083 0000 4964  ..|..j..j.....Id
+00000cc0: 0000 4801 6400 0053 2901 4e29 0272 2200  ..H.d..S).N).r".
+00000cd0: 0000 7218 0000 0029 0272 1200 0000 da11  ..r....).r......
+00000ce0: 7369 6e67 6c65 5f63 6f6e 6e65 6374 696f  single_connectio
+00000cf0: 6e72 1500 0000 7215 0000 0072 1600 0000  nr....r....r....
+00000d00: da19 7265 6c65 6173 655f 7369 6e67 6c65  ..release_single
+00000d10: 5f63 6f6e 6e65 6374 696f 6e50 0000 0073  _connectionP...s
+00000d20: 0200 0000 0001 7a26 5371 6c69 7465 436c  ......z&SqliteCl
+00000d30: 6965 6e74 2e72 656c 6561 7365 5f73 696e  ient.release_sin
+00000d40: 676c 655f 636f 6e6e 6563 7469 6f6e 6302  gle_connectionc.
+00000d50: 0000 0000 0000 0002 0000 0002 0000 00e3  ................
+00000d60: 0000 0073 1300 0000 7c01 006a 0000 8300  ...s....|..j....
+00000d70: 0049 6400 0048 0164 0000 5329 014e 2901  .Id..H.d..S).N).
+00000d80: da06 636f 6d6d 6974 2902 7212 0000 0072  ..commit).r....r
+00000d90: 2200 0000 7215 0000 0072 1500 0000 7216  "...r....r....r.
+00000da0: 0000 0072 3000 0000 5300 0000 7302 0000  ...r0...S...s...
+00000db0: 0000 017a 1453 716c 6974 6543 6c69 656e  ...z.SqliteClien
+00000dc0: 742e 5f63 6f6d 6d69 7429 13da 085f 5f6e  t._commit)...__n
+00000dd0: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
+00000de0: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5f72  _..__qualname__r
+00000df0: 0500 0000 da0e 6578 6563 7574 6f72 5f63  ......executor_c
+00000e00: 6c61 7373 7206 0000 00da 1073 6368 656d  lassr......schem
+00000e10: 615f 6765 6e65 7261 746f 7272 0c00 0000  a_generatorr....
+00000e20: 7217 0000 0072 1800 0000 721c 0000 0072  r....r....r....r
+00000e30: 1f00 0000 7223 0000 0072 2400 0000 7237  ....r#...r$...r7
+00000e40: 0000 0072 3a00 0000 723d 0000 0072 3f00  ...r:...r=...r?.
+00000e50: 0000 7230 0000 0072 1500 0000 7215 0000  ..r0...r....r...
+00000e60: 0029 0172 0f00 0000 7216 0000 0072 0900  .).r....r....r..
+00000e70: 0000 0e00 0000 731c 0000 000c 0106 0106  ......s.........
+00000e80: 0212 0a0c 030c 030c 040c 060c 040c 030f  ................
+00000e90: 120c 050c 060c 0372 0900 0000 6300 0000  .......r....c...
+00000ea0: 0000 0000 0000 0000 0002 0000 0040 0000  .............@..
+00000eb0: 0073 8800 0000 6500 005a 0100 6400 005a  .s....e..Z..d..Z
+00000ec0: 0200 6401 0064 0200 8400 005a 0300 6403  ..d..d.....Z..d.
+00000ed0: 0064 0400 8400 005a 0400 6405 0064 0600  .d.....Z..d..d..
+00000ee0: 8400 005a 0500 6407 0064 0800 8400 005a  ...Z..d..d.....Z
+00000ef0: 0600 6409 0064 0a00 8400 005a 0700 640b  ..d..d.....Z..d.
+00000f00: 0064 0c00 8400 005a 0800 640d 0064 0e00  .d.....Z..d..d..
+00000f10: 8400 005a 0900 640f 0064 1000 8400 005a  ...Z..d..d.....Z
+00000f20: 0a00 6411 0064 1200 8400 005a 0b00 6413  ..d..d.....Z..d.
+00000f30: 0064 1400 8400 005a 0c00 6415 0053 2916  .d.....Z..d..S).
+00000f40: 720a 0000 0063 0200 0000 0000 0000 0200  r....c..........
+00000f50: 0000 0400 0000 4300 0000 7352 0000 007c  ......C...sR...|
+00000f60: 0100 7c00 005f 0000 7401 006a 0200 6401  ..|.._..t..j..d.
+00000f70: 0083 0100 7c00 005f 0300 6402 007c 0000  ....|.._..d..|..
+00000f80: 5f04 0074 0500 6403 0074 0600 7c00 006a  _..t..d..t..|..j
+00000f90: 0700 6602 0069 0000 8303 007c 0000 5f08  ..f..i.....|.._.
+00000fa0: 007c 0000 6a07 007c 0000 5f09 0064 0000  .|..j..|.._..d..
+00000fb0: 5329 044e da09 6462 5f63 6c69 656e 7454  S).N..db_clientT
+00000fc0: 7204 0000 0029 0ada 0b5f 636f 6e6e 6563  r....)..._connec
+00000fd0: 7469 6f6e da07 6c6f 6767 696e 67da 0967  tion..logging..g
+00000fe0: 6574 4c6f 6767 6572 7229 0000 0072 3e00  etLoggerr)...r>.
+00000ff0: 0000 720e 0000 0072 0400 0000 720f 0000  ..r....r....r...
+00001000: 0072 1100 0000 7210 0000 0029 0272 1200  .r....r....).r..
+00001010: 0000 7222 0000 0072 1500 0000 7215 0000  ..r"...r....r...
+00001020: 0072 1600 0000 720c 0000 0058 0000 0073  .r....r....X...s
+00001030: 0c00 0000 0001 0901 1201 0901 0301 1b02  ................
+00001040: 7a1b 5472 616e 7361 6374 696f 6e57 7261  z.TransactionWra
+00001050: 7070 6572 2e5f 5f69 6e69 745f 5f63 0100  pper.__init__c..
+00001060: 0000 0000 0000 0100 0000 0200 0000 4300  ..............C.
+00001070: 0000 730d 0000 0074 0000 7c00 006a 0100  ..s....t..|..j..
+00001080: 8301 0053 2901 4e29 0272 0300 0000 7247  ...S).N).r....rG
+00001090: 0000 0029 0172 1200 0000 7215 0000 0072  ...).r....r....r
+000010a0: 1500 0000 7216 0000 0072 2300 0000 6100  ....r....r#...a.
+000010b0: 0000 7302 0000 0000 017a 2554 7261 6e73  ..s......z%Trans
+000010c0: 6163 7469 6f6e 5772 6170 7065 722e 6163  actionWrapper.ac
+000010d0: 7175 6972 655f 636f 6e6e 6563 7469 6f6e  quire_connection
+000010e0: 6301 0000 0000 0000 0001 0000 0003 0000  c...............
+000010f0: 00c3 0000 0073 1300 0000 7c00 006a 0000  .....s....|..j..
+00001100: 7c00 006a 0100 7c00 0083 0200 5329 014e  |..j..|.....S).N
+00001110: 2902 7211 0000 0072 4700 0000 2901 7212  ).r....rG...).r.
+00001120: 0000 0072 1500 0000 7215 0000 0072 1600  ...r....r....r..
+00001130: 0000 723d 0000 0064 0000 0073 0200 0000  ..r=...d...s....
+00001140: 0001 7a28 5472 616e 7361 6374 696f 6e57  ..z(TransactionW
+00001150: 7261 7070 6572 2e67 6574 5f73 696e 676c  rapper.get_singl
+00001160: 655f 636f 6e6e 6563 7469 6f6e 6302 0000  e_connectionc...
+00001170: 0000 0000 0002 0000 0001 0000 00c3 0000  ................
+00001180: 0073 0400 0000 6400 0053 2901 4e72 1500  .s....d..S).Nr..
+00001190: 0000 2902 7212 0000 0072 3e00 0000 7215  ..).r....r>...r.
+000011a0: 0000 0072 1500 0000 7216 0000 0072 3f00  ...r....r....r?.
+000011b0: 0000 6700 0000 7302 0000 0000 017a 2c54  ..g...s......z,T
+000011c0: 7261 6e73 6163 7469 6f6e 5772 6170 7065  ransactionWrappe
+000011d0: 722e 7265 6c65 6173 655f 7369 6e67 6c65  r.release_single
+000011e0: 5f63 6f6e 6e65 6374 696f 6e63 0100 0000  _connectionc....
+000011f0: 0000 0000 0100 0000 0200 0000 e300 0000  ................
+00001200: 7323 0000 007c 0000 6a00 006a 0100 8300  s#...|..j..j....
+00001210: 0001 7c00 006a 0000 6a02 0083 0000 4964  ..|..j..j.....Id
+00001220: 0000 4801 6400 0053 2901 4e29 0372 4700  ..H.d..S).N).rG.
+00001230: 0000 723b 0000 0072 3c00 0000 2901 7212  ..r;...r<...).r.
 00001240: 0000 0072 1500 0000 7215 0000 0072 1600  ...r....r....r..
-00001250: 0000 7240 0000 0072 0000 0073 0400 0000  ..r@...r...s....
-00001260: 0001 1001 7a19 5472 616e 7361 6374 696f  ....z.Transactio
-00001270: 6e57 7261 7070 6572 2e63 6f6d 6d69 7463  nWrapper.commitc
-00001280: 0100 0000 0000 0000 0100 0000 0200 0000  ................
-00001290: c300 0000 731e 0000 007c 006a 006a 0183  ....s....|.j.j..
-000012a0: 0001 007c 006a 006a 0283 0049 0064 0048  ...|.j.j...I.d.H
-000012b0: 0001 007c 0053 0029 014e 2903 7248 0000  ...|.S.).N).rH..
-000012c0: 0072 3b00 0000 723c 0000 0029 0172 1200  .r;...r<...).r..
-000012d0: 0000 7215 0000 0072 1500 0000 7216 0000  ..r....r....r...
-000012e0: 00da 0a5f 5f61 656e 7465 725f 5f76 0000  ...__aenter__v..
-000012f0: 0073 0600 0000 0001 0a01 1001 7a1d 5472  .s..........z.Tr
-00001300: 616e 7361 6374 696f 6e57 7261 7070 6572  ansactionWrapper
-00001310: 2e5f 5f61 656e 7465 725f 5f63 0400 0000  .__aenter__c....
-00001320: 0000 0000 0400 0000 0200 0000 c300 0000  ................
-00001330: 734c 0000 007c 0172 287c 006a 006a 0183  sL...|.r(|.j.j..
-00001340: 0049 0064 0048 0001 007c 006a 006a 0283  .I.d.H...|.j.j..
-00001350: 0049 0064 0048 0001 0064 0153 007c 006a  .I.d.H...d.S.|.j
-00001360: 006a 0383 0049 0064 0048 0001 007c 006a  .j...I.d.H...|.j
-00001370: 006a 0283 0049 0064 0048 0001 0064 0053  .j...I.d.H...d.S
-00001380: 0029 024e 4629 0472 4800 0000 724b 0000  .).NF).rH...rK..
-00001390: 0072 1800 0000 7240 0000 0029 0472 1200  .r....r@...).r..
-000013a0: 0000 da08 6578 635f 7479 7065 da07 6578  ....exc_type..ex
-000013b0: 635f 7661 6cda 0665 7863 5f74 6272 1500  c_val..exc_tbr..
-000013c0: 0000 7215 0000 0072 1600 0000 da09 5f5f  ..r....r......__
-000013d0: 6165 7869 745f 5f7b 0000 0073 0c00 0000  aexit__{...s....
-000013e0: 0001 0401 1001 1001 0401 1001 7a1c 5472  ............z.Tr
-000013f0: 616e 7361 6374 696f 6e57 7261 7070 6572  ansactionWrapper
-00001400: 2e5f 5f61 6578 6974 5f5f 6302 0000 0000  .__aexit__c.....
-00001410: 0000 0002 0000 0001 0000 00c3 0000 0073  ...............s
-00001420: 0400 0000 6400 5300 2901 4e72 1500 0000  ....d.S.).Nr....
-00001430: 2902 7212 0000 0072 2200 0000 7215 0000  ).r....r"...r...
-00001440: 0072 1500 0000 7216 0000 0072 3000 0000  .r....r....r0...
-00001450: 8300 0000 7302 0000 0000 017a 1a54 7261  ....s......z.Tra
-00001460: 6e73 6163 7469 6f6e 5772 6170 7065 722e  nsactionWrapper.
-00001470: 5f63 6f6d 6d69 744e 290d 7241 0000 0072  _commitN).rA...r
-00001480: 4200 0000 7243 0000 0072 0c00 0000 7223  B...rC...r....r#
-00001490: 0000 0072 3d00 0000 723f 0000 0072 3b00  ...r=...r?...r;.
-000014a0: 0000 724b 0000 0072 4000 0000 724c 0000  ..rK...r@...rL..
-000014b0: 0072 5000 0000 7230 0000 0072 1500 0000  .rP...r0...r....
-000014c0: 7215 0000 0072 1500 0000 7216 0000 0072  r....r....r....r
-000014d0: 0a00 0000 5700 0000 7314 0000 0008 0108  ....W...s.......
-000014e0: 0908 0308 0308 0308 0408 0408 0408 0508  ................
-000014f0: 0872 0a00 0000 2912 7249 0000 0072 1900  .r....).rI...r..
-00001500: 0000 722b 0000 0072 2000 0000 da08 746f  ..r+...r .....to
-00001510: 7274 6f69 7365 7202 0000 00da 1d74 6f72  rtoiser......tor
-00001520: 746f 6973 652e 6261 636b 656e 6473 2e62  toise.backends.b
-00001530: 6173 652e 636c 6965 6e74 7203 0000 0072  ase.clientr....r
-00001540: 0400 0000 5a21 746f 7274 6f69 7365 2e62  ....Z!tortoise.b
-00001550: 6163 6b65 6e64 732e 7371 6c69 7465 2e65  ackends.sqlite.e
-00001560: 7865 6375 746f 7272 0500 0000 5a29 746f  xecutorr....Z)to
-00001570: 7274 6f69 7365 2e62 6163 6b65 6e64 732e  rtoise.backends.
-00001580: 7371 6c69 7465 2e73 6368 656d 615f 6765  sqlite.schema_ge
-00001590: 6e65 7261 746f 7272 0600 0000 da13 746f  neratorr......to
-000015a0: 7274 6f69 7365 2e65 7863 6570 7469 6f6e  rtoise.exception
-000015b0: 7372 0700 0000 7208 0000 0072 0900 0000  sr....r....r....
-000015c0: 720a 0000 0072 1500 0000 7215 0000 0072  r....r....r....r
-000015d0: 1500 0000 7216 0000 00da 083c 6d6f 6475  ....r......<modu
-000015e0: 6c65 3e01 0000 0073 1400 0000 0801 0801  le>....s........
-000015f0: 0802 0802 0c01 1001 0c01 0c01 1003 1049  ...............I
+00001250: 0000 723b 0000 006a 0000 0073 0400 0000  ..r;...j...s....
+00001260: 0001 0d01 7a18 5472 616e 7361 6374 696f  ....z.Transactio
+00001270: 6e57 7261 7070 6572 2e73 7461 7274 6301  nWrapper.startc.
+00001280: 0000 0000 0000 0001 0000 0002 0000 00e3  ................
+00001290: 0000 0073 2800 0000 7c00 006a 0000 6a01  ...s(...|..j..j.
+000012a0: 0083 0000 4964 0000 4801 7c00 006a 0000  ....Id..H.|..j..
+000012b0: 6a02 0083 0000 4964 0000 4801 6400 0053  j.....Id..H.d..S
+000012c0: 2901 4e29 0372 4700 0000 da08 726f 6c6c  ).N).rG.....roll
+000012d0: 6261 636b 7218 0000 0029 0172 1200 0000  backr....).r....
+000012e0: 7215 0000 0072 1500 0000 7216 0000 0072  r....r....r....r
+000012f0: 4a00 0000 6e00 0000 7304 0000 0000 0112  J...n...s.......
+00001300: 017a 1b54 7261 6e73 6163 7469 6f6e 5772  .z.TransactionWr
+00001310: 6170 7065 722e 726f 6c6c 6261 636b 6301  apper.rollbackc.
+00001320: 0000 0000 0000 0001 0000 0002 0000 00e3  ................
+00001330: 0000 0073 2800 0000 7c00 006a 0000 6a01  ...s(...|..j..j.
+00001340: 0083 0000 4964 0000 4801 7c00 006a 0000  ....Id..H.|..j..
+00001350: 6a02 0083 0000 4964 0000 4801 6400 0053  j.....Id..H.d..S
+00001360: 2901 4e29 0372 4700 0000 7240 0000 0072  ).N).rG...r@...r
+00001370: 1800 0000 2901 7212 0000 0072 1500 0000  ....).r....r....
+00001380: 7215 0000 0072 1600 0000 7240 0000 0072  r....r....r@...r
+00001390: 0000 0073 0400 0000 0001 1201 7a19 5472  ...s........z.Tr
+000013a0: 616e 7361 6374 696f 6e57 7261 7070 6572  ansactionWrapper
+000013b0: 2e63 6f6d 6d69 7463 0100 0000 0000 0000  .commitc........
+000013c0: 0100 0000 0200 0000 e300 0000 7323 0000  ............s#..
+000013d0: 007c 0000 6a00 006a 0100 8300 0001 7c00  .|..j..j......|.
+000013e0: 006a 0000 6a02 0083 0000 4964 0000 4801  .j..j.....Id..H.
+000013f0: 7c00 0053 2901 4e29 0372 4700 0000 723b  |..S).N).rG...r;
+00001400: 0000 0072 3c00 0000 2901 7212 0000 0072  ...r<...).r....r
+00001410: 1500 0000 7215 0000 0072 1600 0000 da0a  ....r....r......
+00001420: 5f5f 6165 6e74 6572 5f5f 7600 0000 7306  __aenter__v...s.
+00001430: 0000 0000 010d 0112 017a 1d54 7261 6e73  .........z.Trans
+00001440: 6163 7469 6f6e 5772 6170 7065 722e 5f5f  actionWrapper.__
+00001450: 6165 6e74 6572 5f5f 6304 0000 0000 0000  aenter__c.......
+00001460: 0004 0000 0002 0000 00e3 0000 0073 5600  .............sV.
+00001470: 0000 7c01 0072 2e00 7c00 006a 0000 6a01  ..|..r..|..j..j.
+00001480: 0083 0000 4964 0000 4801 7c00 006a 0000  ....Id..H.|..j..
+00001490: 6a02 0083 0000 4964 0000 4801 6401 0053  j.....Id..H.d..S
+000014a0: 7c00 006a 0000 6a03 0083 0000 4964 0000  |..j..j.....Id..
+000014b0: 4801 7c00 006a 0000 6a02 0083 0000 4964  H.|..j..j.....Id
+000014c0: 0000 4801 6400 0053 2902 4e46 2904 7247  ..H.d..S).NF).rG
+000014d0: 0000 0072 4a00 0000 7218 0000 0072 4000  ...rJ...r....r@.
+000014e0: 0000 2904 7212 0000 00da 0865 7863 5f74  ..).r......exc_t
+000014f0: 7970 65da 0765 7863 5f76 616c da06 6578  ype..exc_val..ex
+00001500: 635f 7462 7215 0000 0072 1500 0000 7216  c_tbr....r....r.
+00001510: 0000 00da 095f 5f61 6578 6974 5f5f 7b00  .....__aexit__{.
+00001520: 0000 730c 0000 0000 0106 0112 0112 0104  ..s.............
+00001530: 0112 017a 1c54 7261 6e73 6163 7469 6f6e  ...z.Transaction
+00001540: 5772 6170 7065 722e 5f5f 6165 7869 745f  Wrapper.__aexit_
+00001550: 5f63 0200 0000 0000 0000 0200 0000 0100  _c..............
+00001560: 0000 c300 0000 7304 0000 0064 0000 5329  ......s....d..S)
+00001570: 014e 7215 0000 0029 0272 1200 0000 7222  .Nr....).r....r"
+00001580: 0000 0072 1500 0000 7215 0000 0072 1600  ...r....r....r..
+00001590: 0000 7230 0000 0083 0000 0073 0200 0000  ..r0.......s....
+000015a0: 0001 7a1a 5472 616e 7361 6374 696f 6e57  ..z.TransactionW
+000015b0: 7261 7070 6572 2e5f 636f 6d6d 6974 4e29  rapper._commitN)
+000015c0: 0d72 4100 0000 7242 0000 0072 4300 0000  .rA...rB...rC...
+000015d0: 720c 0000 0072 2300 0000 723d 0000 0072  r....r#...r=...r
+000015e0: 3f00 0000 723b 0000 0072 4a00 0000 7240  ?...r;...rJ...r@
+000015f0: 0000 0072 4b00 0000 724f 0000 0072 3000  ...rK...rO...r0.
+00001600: 0000 7215 0000 0072 1500 0000 7215 0000  ..r....r....r...
+00001610: 0072 1600 0000 720a 0000 0057 0000 0073  .r....r....W...s
+00001620: 1400 0000 0c01 0c09 0c03 0c03 0c03 0c04  ................
+00001630: 0c04 0c04 0c05 0c08 720a 0000 0029 1272  ........r....).r
+00001640: 4800 0000 7219 0000 0072 2b00 0000 7220  H...r....r+...r 
+00001650: 0000 00da 0874 6f72 746f 6973 6572 0200  .....tortoiser..
+00001660: 0000 da1d 746f 7274 6f69 7365 2e62 6163  ....tortoise.bac
+00001670: 6b65 6e64 732e 6261 7365 2e63 6c69 656e  kends.base.clien
+00001680: 7472 0300 0000 7204 0000 005a 2174 6f72  tr....r....Z!tor
+00001690: 746f 6973 652e 6261 636b 656e 6473 2e73  toise.backends.s
+000016a0: 716c 6974 652e 6578 6563 7574 6f72 7205  qlite.executorr.
+000016b0: 0000 005a 2974 6f72 746f 6973 652e 6261  ...Z)tortoise.ba
+000016c0: 636b 656e 6473 2e73 716c 6974 652e 7363  ckends.sqlite.sc
+000016d0: 6865 6d61 5f67 656e 6572 6174 6f72 7206  hema_generatorr.
+000016e0: 0000 00da 1374 6f72 746f 6973 652e 6578  .....tortoise.ex
+000016f0: 6365 7074 696f 6e73 7207 0000 0072 0800  ceptionsr....r..
+00001700: 0000 7209 0000 0072 0a00 0000 7215 0000  ..r....r....r...
+00001710: 0072 1500 0000 7215 0000 0072 1600 0000  .r....r....r....
+00001720: da08 3c6d 6f64 756c 653e 0100 0000 7314  ..<module>....s.
+00001730: 0000 000c 010c 010c 020c 0210 0116 0110  ................
+00001740: 0110 0116 0316 49                        ......I
```

### Comparing `tortoise-orm-0.9.2/tortoise/backends/sqlite/__pycache__/schema_generator.cpython-36.pyc` & `tortoise-orm-0.9.4/tortoise/backends/sqlite/__pycache__/schema_generator.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `tortoise-orm-0.9.2/tortoise/backends/sqlite/__pycache__/executor.cpython-36.pyc` & `tortoise-orm-0.9.4/tortoise/backends/sqlite/__pycache__/executor.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `tortoise-orm-0.9.2/tortoise/backends/sqlite/schema_generator.py` & `tortoise-orm-0.9.4/tortoise/backends/sqlite/schema_generator.py`

 * *Files identical despite different names*

### Comparing `tortoise-orm-0.9.2/tortoise/backends/sqlite/executor.py` & `tortoise-orm-0.9.4/tortoise/backends/sqlite/executor.py`

 * *Files identical despite different names*

### Comparing `tortoise-orm-0.9.2/tortoise/backends/base/.DS_Store` & `tortoise-orm-0.9.4/tortoise/backends/base/.DS_Store`

 * *Files identical despite different names*

### Comparing `tortoise-orm-0.9.2/tortoise/backends/base/db_url.py` & `tortoise-orm-0.9.4/tortoise/backends/base/db_url.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,69 +1,70 @@
 import urllib.parse as urlparse
 import uuid
 
 from tortoise.backends.asyncpg.client import AsyncpgDBClient
 from tortoise.backends.sqlite.client import SqliteClient
+from tortoise.exceptions import ConfigurationError
 
 urlparse.uses_netloc.append('postgres')
 urlparse.uses_netloc.append('sqlite')
 DB_LOOKUP = {
     'postgres': {
         'client': AsyncpgDBClient,
         'vars': {
             'path': 'database',
             'hostname': 'host',
             'port': 'port',
             'username': 'user',
             'password': 'password',
         },
-        'test_defaults': {
-            'single_connection': True
-        },
     },
     'sqlite': {
         'client': SqliteClient,
         'skip_first_char': False,
         'vars': {
             'path': 'filename',
         },
     },
 }
 
 
 def expand_db_url(db_url: str, testing: bool = False) -> dict:
     url = urlparse.urlparse(db_url)
+    if url.scheme not in DB_LOOKUP:
+        raise ConfigurationError('Unknown DB scheme: {}'.format(url.scheme))
+
     db = DB_LOOKUP[url.scheme]
     if db.get('skip_first_char', True):
         path = url.path[1:]
     else:
         path = url.path
-    if '?' in path and not url.query:
-        path, query = path.split('?', 2)
-    else:
-        path, query = path, url.query
+
+    if not path:
+        raise ConfigurationError('No path specified for DB_URL')
 
     params = {}  # type: dict
-    params.update(db.get('test_defaults', {}))  # type: ignore
-    for key, val in urlparse.parse_qs(query).items():
+    for key, val in urlparse.parse_qs(url.query).items():
         params[key] = val[-1]
 
     if testing:
         params['single_connection'] = True
         path = path.replace('\\{', '{').replace('\\}', '}')
         path = path.format(uuid.uuid4().hex)
 
     vars = {}  # type: dict
-    vars.update(db.get('vars', {}))  # type: ignore
-    if vars.get('path'):
-        params[vars['path']] = path
+    vars.update(db['vars'])  # type: ignore
+    params[vars['path']] = path
     if vars.get('hostname'):
         params[vars['hostname']] = str(url.hostname or '')
-    if vars.get('port'):
-        params[vars['port']] = str(url.port or '')
+    try:
+        if vars.get('port'):
+            params[vars['port']] = str(url.port or '')
+    except ValueError:
+        raise ConfigurationError('Port is not an integer')
     if vars.get('username'):
         params[vars['username']] = str(url.username or '')
     if vars.get('password'):
         params[vars['password']] = str(url.password or '')
 
     return {
         'params': params,
```

### Comparing `tortoise-orm-0.9.2/tortoise/backends/base/client.py` & `tortoise-orm-0.9.4/tortoise/backends/base/client.py`

 * *Files identical despite different names*

### Comparing `tortoise-orm-0.9.2/tortoise/backends/base/__pycache__/client.cpython-36.pyc` & `tortoise-orm-0.9.4/tortoise/backends/base/__pycache__/client.cpython-37.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.6 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,251 +1,263 @@
-00000000: 330d 0d0a 5576 3f5b 240a 0000 e300 0000  3...Uv?[$.......
-00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 5c00 0000 6400 6401 6c00 5a00 6400  .s\...d.d.l.Z.d.
-00000030: 6402 6c01 6d02 5a02 0100 6400 6403 6c03  d.l.m.Z...d.d.l.
-00000040: 6d04 5a04 0100 6400 6404 6c05 6d06 5a06  m.Z...d.d.l.m.Z.
-00000050: 0100 4700 6405 6406 8400 6406 8302 5a07  ..G.d.d...d...Z.
-00000060: 4700 6407 6408 8400 6408 8302 5a08 4700  G.d.d...d...Z.G.
-00000070: 6409 640a 8400 640a 6507 8303 5a09 6401  d.d...d.e...Z.d.
-00000080: 5300 290b e900 0000 004e 2901 da05 5175  S.)......N)...Qu
-00000090: 6572 7929 01da 0c42 6173 6545 7865 6375  ery)...BaseExecu
-000000a0: 746f 7229 01da 1342 6173 6553 6368 656d  tor)...BaseSchem
-000000b0: 6147 656e 6572 6174 6f72 6300 0000 0000  aGeneratorc.....
-000000c0: 0000 0000 0000 0003 0000 0040 0000 0073  ...........@...s
-000000d0: 7200 0000 6500 5a01 6400 5a02 6503 5a04  r...e.Z.d.Z.e.Z.
-000000e0: 6505 5a06 6507 5a08 6419 6402 6403 8401  e.Z.e.Z.d.d.d...
-000000f0: 5a09 6404 6405 8400 5a0a 6406 6407 8400  Z.d.d...Z.d.d...
-00000100: 5a0b 6408 6409 8400 5a0c 640a 640b 8400  Z.d.d...Z.d.d...
-00000110: 5a0d 640c 640d 8400 5a0e 640e 640f 8400  Z.d.d...Z.d.d...
-00000120: 5a0f 6410 6411 8400 5a10 6412 6413 8400  Z.d.d...Z.d.d...
-00000130: 5a11 6414 6415 8400 5a12 6416 6417 8400  Z.d.d...Z.d.d...
-00000140: 5a13 6418 5300 291a da11 4261 7365 4442  Z.d.S.)...BaseDB
-00000150: 4173 796e 6343 6c69 656e 7446 6302 0000  AsyncClientFc...
-00000160: 0000 0000 0003 0000 0004 0000 004b 0000  .............K..
-00000170: 0073 2a00 0000 7400 6a01 6401 8301 7c00  .s*...t.j.d...|.
-00000180: 5f02 7c01 7c00 5f03 7404 6402 7405 7c00  _.|.|._.t.d.t.|.
-00000190: 6a06 6602 6900 8303 7c00 5f07 6400 5300  j.f.i...|._.d.S.
-000001a0: 2903 4eda 0964 625f 636c 6965 6e74 da17  ).N..db_client..
-000001b0: 5369 6e67 6c65 436f 6e6e 6563 7469 6f6e  SingleConnection
-000001c0: 5772 6170 7065 7229 08da 076c 6f67 6769  Wrapper)...loggi
-000001d0: 6e67 da09 6765 744c 6f67 6765 72da 036c  ng..getLogger..l
-000001e0: 6f67 da11 7369 6e67 6c65 5f63 6f6e 6e65  og..single_conne
-000001f0: 6374 696f 6eda 0474 7970 6572 0700 0000  ction..typer....
-00000200: da09 5f5f 636c 6173 735f 5f5a 185f 7369  ..__class__Z._si
-00000210: 6e67 6c65 5f63 6f6e 6e65 6374 696f 6e5f  ngle_connection_
-00000220: 636c 6173 7329 03da 0473 656c 6672 0b00  class)...selfr..
-00000230: 0000 da06 6b77 6172 6773 a900 7210 0000  ....kwargs..r...
-00000240: 00fa 512f 5573 6572 732f 616e 6472 6579  ..Q/Users/andrey
-00000250: 626f 6e64 6172 2f50 7943 6861 726d 5072  bondar/PyCharmPr
-00000260: 6f6a 6563 7473 2f74 6f72 746f 6973 652d  ojects/tortoise-
-00000270: 6f72 6d2f 746f 7274 6f69 7365 2f62 6163  orm/tortoise/bac
-00000280: 6b65 6e64 732f 6261 7365 2f63 6c69 656e  kends/base/clien
-00000290: 742e 7079 da08 5f5f 696e 6974 5f5f 0e00  t.py..__init__..
-000002a0: 0000 7308 0000 0000 010c 0106 0102 017a  ..s............z
-000002b0: 1a42 6173 6544 4241 7379 6e63 436c 6965  .BaseDBAsyncClie
-000002c0: 6e74 2e5f 5f69 6e69 745f 5f63 0100 0000  nt.__init__c....
-000002d0: 0000 0000 0100 0000 0100 0000 c300 0000  ................
-000002e0: 730a 0000 0074 0083 0082 0164 0053 0029  s....t.....d.S.)
-000002f0: 014e 2901 da13 4e6f 7449 6d70 6c65 6d65  .N)...NotImpleme
-00000300: 6e74 6564 4572 726f 7229 0172 0e00 0000  ntedError).r....
-00000310: 7210 0000 0072 1000 0000 7211 0000 00da  r....r....r.....
-00000320: 1163 7265 6174 655f 636f 6e6e 6563 7469  .create_connecti
-00000330: 6f6e 1500 0000 7302 0000 0000 017a 2342  on....s......z#B
-00000340: 6173 6544 4241 7379 6e63 436c 6965 6e74  aseDBAsyncClient
-00000350: 2e63 7265 6174 655f 636f 6e6e 6563 7469  .create_connecti
-00000360: 6f6e 6301 0000 0000 0000 0001 0000 0001  onc.............
-00000370: 0000 00c3 0000 0073 0a00 0000 7400 8300  .......s....t...
-00000380: 8201 6400 5300 2901 4e29 0172 1300 0000  ..d.S.).N).r....
-00000390: 2901 720e 0000 0072 1000 0000 7210 0000  ).r....r....r...
-000003a0: 0072 1100 0000 da05 636c 6f73 6518 0000  .r......close...
-000003b0: 0073 0200 0000 0001 7a17 4261 7365 4442  .s......z.BaseDB
-000003c0: 4173 796e 6343 6c69 656e 742e 636c 6f73  AsyncClient.clos
-000003d0: 6563 0100 0000 0000 0000 0100 0000 0100  ec..............
-000003e0: 0000 c300 0000 730a 0000 0074 0083 0082  ......s....t....
-000003f0: 0164 0053 0029 014e 2901 7213 0000 0029  .d.S.).N).r....)
-00000400: 0172 0e00 0000 7210 0000 0072 1000 0000  .r....r....r....
-00000410: 7211 0000 00da 0964 625f 6372 6561 7465  r......db_create
-00000420: 1b00 0000 7302 0000 0000 017a 1b42 6173  ....s......z.Bas
-00000430: 6544 4241 7379 6e63 436c 6965 6e74 2e64  eDBAsyncClient.d
-00000440: 625f 6372 6561 7465 6301 0000 0000 0000  b_createc.......
-00000450: 0001 0000 0001 0000 00c3 0000 0073 0a00  .............s..
-00000460: 0000 7400 8300 8201 6400 5300 2901 4e29  ..t.....d.S.).N)
-00000470: 0172 1300 0000 2901 720e 0000 0072 1000  .r....).r....r..
-00000480: 0000 7210 0000 0072 1100 0000 da09 6462  ..r....r......db
-00000490: 5f64 656c 6574 651e 0000 0073 0200 0000  _delete....s....
-000004a0: 0001 7a1b 4261 7365 4442 4173 796e 6343  ..z.BaseDBAsyncC
-000004b0: 6c69 656e 742e 6462 5f64 656c 6574 6563  lient.db_deletec
-000004c0: 0100 0000 0000 0000 0100 0000 0100 0000  ................
-000004d0: 4300 0000 730a 0000 0074 0083 0082 0164  C...s....t.....d
-000004e0: 0053 0029 014e 2901 7213 0000 0029 0172  .S.).N).r....).r
-000004f0: 0e00 0000 7210 0000 0072 1000 0000 7211  ....r....r....r.
-00000500: 0000 00da 1261 6371 7569 7265 5f63 6f6e  .....acquire_con
-00000510: 6e65 6374 696f 6e21 0000 0073 0200 0000  nection!...s....
-00000520: 0001 7a24 4261 7365 4442 4173 796e 6343  ..z$BaseDBAsyncC
-00000530: 6c69 656e 742e 6163 7175 6972 655f 636f  lient.acquire_co
-00000540: 6e6e 6563 7469 6f6e 6301 0000 0000 0000  nnectionc.......
-00000550: 0001 0000 0001 0000 0043 0000 0073 0a00  .........C...s..
-00000560: 0000 7400 8300 8201 6400 5300 2901 4e29  ..t.....d.S.).N)
-00000570: 0172 1300 0000 2901 720e 0000 0072 1000  .r....).r....r..
-00000580: 0000 7210 0000 0072 1100 0000 da0e 696e  ..r....r......in
-00000590: 5f74 7261 6e73 6163 7469 6f6e 2400 0000  _transaction$...
-000005a0: 7302 0000 0000 017a 2042 6173 6544 4241  s......z BaseDBA
-000005b0: 7379 6e63 436c 6965 6e74 2e69 6e5f 7472  syncClient.in_tr
-000005c0: 616e 7361 6374 696f 6e63 0200 0000 0000  ansactionc......
-000005d0: 0000 0200 0000 0100 0000 c300 0000 730a  ..............s.
-000005e0: 0000 0074 0083 0082 0164 0053 0029 014e  ...t.....d.S.).N
-000005f0: 2901 7213 0000 0029 0272 0e00 0000 da05  ).r....).r......
-00000600: 7175 6572 7972 1000 0000 7210 0000 0072  queryr....r....r
-00000610: 1100 0000 da0d 6578 6563 7574 655f 7175  ......execute_qu
-00000620: 6572 7927 0000 0073 0200 0000 0001 7a1f  ery'...s......z.
-00000630: 4261 7365 4442 4173 796e 6343 6c69 656e  BaseDBAsyncClien
-00000640: 742e 6578 6563 7574 655f 7175 6572 7963  t.execute_queryc
-00000650: 0200 0000 0000 0000 0200 0000 0100 0000  ................
-00000660: c300 0000 730a 0000 0074 0083 0082 0164  ....s....t.....d
-00000670: 0053 0029 014e 2901 7213 0000 0029 0272  .S.).N).r....).r
-00000680: 0e00 0000 da06 7363 7269 7074 7210 0000  ......scriptr...
-00000690: 0072 1000 0000 7211 0000 00da 0e65 7865  .r....r......exe
-000006a0: 6375 7465 5f73 6372 6970 742a 0000 0073  cute_script*...s
-000006b0: 0200 0000 0001 7a20 4261 7365 4442 4173  ......z BaseDBAs
-000006c0: 796e 6343 6c69 656e 742e 6578 6563 7574  yncClient.execut
-000006d0: 655f 7363 7269 7074 6301 0000 0000 0000  e_scriptc.......
-000006e0: 0001 0000 0001 0000 00c3 0000 0073 0a00  .............s..
-000006f0: 0000 7400 8300 8201 6400 5300 2901 4e29  ..t.....d.S.).N)
-00000700: 0172 1300 0000 2901 720e 0000 0072 1000  .r....).r....r..
-00000710: 0000 7210 0000 0072 1100 0000 da15 6765  ..r....r......ge
-00000720: 745f 7369 6e67 6c65 5f63 6f6e 6e65 6374  t_single_connect
-00000730: 696f 6e2d 0000 0073 0200 0000 0001 7a27  ion-...s......z'
-00000740: 4261 7365 4442 4173 796e 6343 6c69 656e  BaseDBAsyncClien
-00000750: 742e 6765 745f 7369 6e67 6c65 5f63 6f6e  t.get_single_con
-00000760: 6e65 6374 696f 6e63 0200 0000 0000 0000  nectionc........
-00000770: 0200 0000 0100 0000 c300 0000 730a 0000  ............s...
-00000780: 0074 0083 0082 0164 0053 0029 014e 2901  .t.....d.S.).N).
-00000790: 7213 0000 0029 0272 0e00 0000 720b 0000  r....).r....r...
-000007a0: 0072 1000 0000 7210 0000 0072 1100 0000  .r....r....r....
-000007b0: da19 7265 6c65 6173 655f 7369 6e67 6c65  ..release_single
-000007c0: 5f63 6f6e 6e65 6374 696f 6e30 0000 0073  _connection0...s
-000007d0: 0200 0000 0001 7a2b 4261 7365 4442 4173  ......z+BaseDBAs
-000007e0: 796e 6343 6c69 656e 742e 7265 6c65 6173  yncClient.releas
-000007f0: 655f 7369 6e67 6c65 5f63 6f6e 6e65 6374  e_single_connect
-00000800: 696f 6e4e 2901 4629 14da 085f 5f6e 616d  ionN).F)...__nam
-00000810: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
-00000820: 0c5f 5f71 7561 6c6e 616d 655f 5f72 0200  .__qualname__r..
-00000830: 0000 da0b 7175 6572 795f 636c 6173 7372  ....query_classr
-00000840: 0300 0000 5a0e 6578 6563 7574 6f72 5f63  ....Z.executor_c
-00000850: 6c61 7373 7204 0000 00da 1073 6368 656d  lassr......schem
-00000860: 615f 6765 6e65 7261 746f 7272 1200 0000  a_generatorr....
-00000870: 7214 0000 0072 1500 0000 7216 0000 0072  r....r....r....r
-00000880: 1700 0000 7218 0000 0072 1900 0000 721b  ....r....r....r.
-00000890: 0000 0072 1d00 0000 721e 0000 0072 1f00  ...r....r....r..
-000008a0: 0000 7210 0000 0072 1000 0000 7210 0000  ..r....r....r...
-000008b0: 0072 1100 0000 7205 0000 0009 0000 0073  .r....r........s
-000008c0: 1c00 0000 0801 0401 0401 0402 0a07 0803  ................
-000008d0: 0803 0803 0803 0803 0803 0803 0803 0803  ................
-000008e0: 7205 0000 0063 0000 0000 0000 0000 0000  r....c..........
-000008f0: 0000 0200 0000 4000 0000 7324 0000 0065  ......@...s$...e
-00000900: 005a 0164 005a 0264 0164 0284 005a 0364  .Z.d.Z.d.d...Z.d
-00000910: 0364 0484 005a 0464 0564 0684 005a 0564  .d...Z.d.d...Z.d
-00000920: 0753 0029 08da 1143 6f6e 6e65 6374 696f  .S.)...Connectio
-00000930: 6e57 7261 7070 6572 6302 0000 0000 0000  nWrapperc.......
-00000940: 0002 0000 0002 0000 0043 0000 0073 0a00  .........C...s..
-00000950: 0000 7c01 7c00 5f00 6400 5300 2901 4e29  ..|.|._.d.S.).N)
-00000960: 01da 0a63 6f6e 6e65 6374 696f 6e29 0272  ...connection).r
-00000970: 0e00 0000 7226 0000 0072 1000 0000 7210  ....r&...r....r.
-00000980: 0000 0072 1100 0000 7212 0000 0035 0000  ...r....r....5..
-00000990: 0073 0200 0000 0001 7a1a 436f 6e6e 6563  .s......z.Connec
-000009a0: 7469 6f6e 5772 6170 7065 722e 5f5f 696e  tionWrapper.__in
-000009b0: 6974 5f5f 6301 0000 0000 0000 0001 0000  it__c...........
-000009c0: 0001 0000 00c3 0000 0073 0600 0000 7c00  .........s....|.
-000009d0: 6a00 5300 2901 4e29 0172 2600 0000 2901  j.S.).N).r&...).
-000009e0: 720e 0000 0072 1000 0000 7210 0000 0072  r....r....r....r
-000009f0: 1100 0000 da0a 5f5f 6165 6e74 6572 5f5f  ......__aenter__
-00000a00: 3800 0000 7302 0000 0000 017a 1c43 6f6e  8...s......z.Con
-00000a10: 6e65 6374 696f 6e57 7261 7070 6572 2e5f  nectionWrapper._
-00000a20: 5f61 656e 7465 725f 5f63 0400 0000 0000  _aenter__c......
-00000a30: 0000 0400 0000 0100 0000 c300 0000 7304  ..............s.
-00000a40: 0000 0064 0053 0029 014e 7210 0000 0029  ...d.S.).Nr....)
-00000a50: 0472 0e00 0000 da08 6578 635f 7479 7065  .r......exc_type
-00000a60: da07 6578 635f 7661 6cda 0665 7863 5f74  ..exc_val..exc_t
-00000a70: 6272 1000 0000 7210 0000 0072 1100 0000  br....r....r....
-00000a80: da09 5f5f 6165 7869 745f 5f3b 0000 0073  ..__aexit__;...s
-00000a90: 0200 0000 0001 7a1b 436f 6e6e 6563 7469  ......z.Connecti
-00000aa0: 6f6e 5772 6170 7065 722e 5f5f 6165 7869  onWrapper.__aexi
-00000ab0: 745f 5f4e 2906 7220 0000 0072 2100 0000  t__N).r ...r!...
-00000ac0: 7222 0000 0072 1200 0000 7227 0000 0072  r"...r....r'...r
-00000ad0: 2b00 0000 7210 0000 0072 1000 0000 7210  +...r....r....r.
-00000ae0: 0000 0072 1100 0000 7225 0000 0034 0000  ...r....r%...4..
-00000af0: 0073 0600 0000 0801 0803 0803 7225 0000  .s..........r%..
-00000b00: 0063 0000 0000 0000 0000 0000 0000 0200  .c..............
-00000b10: 0000 4000 0000 733c 0000 0065 005a 0164  ..@...s<...e.Z.d
-00000b20: 005a 0264 0164 0284 005a 0364 0364 0484  .Z.d.d...Z.d.d..
-00000b30: 005a 0464 0564 0684 005a 0564 0764 0884  .Z.d.d...Z.d.d..
-00000b40: 005a 0664 0964 0a84 005a 0764 0b64 0c84  .Z.d.d...Z.d.d..
-00000b50: 005a 0864 0d53 0029 0e72 0700 0000 6303  .Z.d.S.).r....c.
-00000b60: 0000 0000 0000 0003 0000 0002 0000 0043  ...............C
-00000b70: 0000 0073 2200 0000 7c01 7c00 5f00 7c02  ...s"...|.|._.|.
-00000b80: 7c00 5f01 7402 6a03 6401 8301 7c00 5f04  |._.t.j.d...|._.
-00000b90: 6402 7c00 5f05 6400 5300 2903 4e72 0600  d.|._.d.S.).Nr..
-00000ba0: 0000 5429 0672 2600 0000 da06 7061 7265  ..T).r&.....pare
-00000bb0: 6e74 7208 0000 0072 0900 0000 720a 0000  ntr....r....r...
-00000bc0: 0072 0b00 0000 2903 720e 0000 0072 2600  .r....).r....r&.
-00000bd0: 0000 722c 0000 0072 1000 0000 7210 0000  ..r,...r....r...
-00000be0: 0072 1100 0000 7212 0000 0040 0000 0073  .r....r....@...s
-00000bf0: 0800 0000 0001 0601 0601 0c01 7a20 5369  ............z Si
-00000c00: 6e67 6c65 436f 6e6e 6563 7469 6f6e 5772  ngleConnectionWr
-00000c10: 6170 7065 722e 5f5f 696e 6974 5f5f 6301  apper.__init__c.
-00000c20: 0000 0000 0000 0001 0000 0002 0000 0043  ...............C
-00000c30: 0000 0073 0a00 0000 7400 7c00 6a01 8301  ...s....t.|.j...
-00000c40: 5300 2901 4e29 0272 2500 0000 7226 0000  S.).N).r%...r&..
-00000c50: 0029 0172 0e00 0000 7210 0000 0072 1000  .).r....r....r..
-00000c60: 0000 7211 0000 0072 1800 0000 4600 0000  ..r....r....F...
-00000c70: 7302 0000 0000 017a 2a53 696e 676c 6543  s......z*SingleC
-00000c80: 6f6e 6e65 6374 696f 6e57 7261 7070 6572  onnectionWrapper
-00000c90: 2e61 6371 7569 7265 5f63 6f6e 6e65 6374  .acquire_connect
-00000ca0: 696f 6e63 0100 0000 0000 0000 0100 0000  ionc............
-00000cb0: 0300 0000 c300 0000 730e 0000 007c 006a  ........s....|.j
-00000cc0: 007c 006a 017c 0083 0253 0029 014e 2902  .|.j.|...S.).N).
-00000cd0: 720d 0000 0072 2600 0000 2901 720e 0000  r....r&...).r...
-00000ce0: 0072 1000 0000 7210 0000 0072 1100 0000  .r....r....r....
-00000cf0: 721e 0000 0049 0000 0073 0200 0000 0003  r....I...s......
-00000d00: 7a2d 5369 6e67 6c65 436f 6e6e 6563 7469  z-SingleConnecti
-00000d10: 6f6e 5772 6170 7065 722e 6765 745f 7369  onWrapper.get_si
-00000d20: 6e67 6c65 5f63 6f6e 6e65 6374 696f 6e63  ngle_connectionc
-00000d30: 0200 0000 0000 0000 0200 0000 0100 0000  ................
-00000d40: c300 0000 7304 0000 0064 0053 0029 014e  ....s....d.S.).N
-00000d50: 7210 0000 0029 0272 0e00 0000 720b 0000  r....).r....r...
-00000d60: 0072 1000 0000 7210 0000 0072 1100 0000  .r....r....r....
-00000d70: 721f 0000 004e 0000 0073 0200 0000 0001  r....N...s......
-00000d80: 7a31 5369 6e67 6c65 436f 6e6e 6563 7469  z1SingleConnecti
-00000d90: 6f6e 5772 6170 7065 722e 7265 6c65 6173  onWrapper.releas
-00000da0: 655f 7369 6e67 6c65 5f63 6f6e 6e65 6374  e_single_connect
-00000db0: 696f 6e63 0100 0000 0000 0000 0100 0000  ionc............
-00000dc0: 0100 0000 c300 0000 7304 0000 007c 0053  ........s....|.S
-00000dd0: 0029 014e 7210 0000 0029 0172 0e00 0000  .).Nr....).r....
-00000de0: 7210 0000 0072 1000 0000 7211 0000 0072  r....r....r....r
-00000df0: 2700 0000 5100 0000 7302 0000 0000 017a  '...Q...s......z
-00000e00: 2253 696e 676c 6543 6f6e 6e65 6374 696f  "SingleConnectio
-00000e10: 6e57 7261 7070 6572 2e5f 5f61 656e 7465  nWrapper.__aente
-00000e20: 725f 5f63 0400 0000 0000 0000 0400 0000  r__c............
-00000e30: 0100 0000 c300 0000 7304 0000 0064 0053  ........s....d.S
-00000e40: 0029 014e 7210 0000 0029 0472 0e00 0000  .).Nr....).r....
-00000e50: 7228 0000 0072 2900 0000 722a 0000 0072  r(...r)...r*...r
-00000e60: 1000 0000 7210 0000 0072 1100 0000 722b  ....r....r....r+
-00000e70: 0000 0054 0000 0073 0200 0000 0001 7a21  ...T...s......z!
-00000e80: 5369 6e67 6c65 436f 6e6e 6563 7469 6f6e  SingleConnection
-00000e90: 5772 6170 7065 722e 5f5f 6165 7869 745f  Wrapper.__aexit_
-00000ea0: 5f4e 2909 7220 0000 0072 2100 0000 7222  _N).r ...r!...r"
-00000eb0: 0000 0072 1200 0000 7218 0000 0072 1e00  ...r....r....r..
-00000ec0: 0000 721f 0000 0072 2700 0000 722b 0000  ..r....r'...r+..
-00000ed0: 0072 1000 0000 7210 0000 0072 1000 0000  .r....r....r....
-00000ee0: 7211 0000 0072 0700 0000 3f00 0000 730c  r....r....?...s.
-00000ef0: 0000 0008 0108 0608 0308 0508 0308 0372  ...............r
-00000f00: 0700 0000 290a 7208 0000 00da 0670 7970  ....).r......pyp
-00000f10: 696b 6172 0200 0000 5a1f 746f 7274 6f69  ikar....Z.tortoi
-00000f20: 7365 2e62 6163 6b65 6e64 732e 6261 7365  se.backends.base
-00000f30: 2e65 7865 6375 746f 7272 0300 0000 5a27  .executorr....Z'
-00000f40: 746f 7274 6f69 7365 2e62 6163 6b65 6e64  tortoise.backend
-00000f50: 732e 6261 7365 2e73 6368 656d 615f 6765  s.base.schema_ge
-00000f60: 6e65 7261 746f 7272 0400 0000 7205 0000  neratorr....r...
-00000f70: 0072 2500 0000 7207 0000 0072 1000 0000  .r%...r....r....
-00000f80: 7210 0000 0072 1000 0000 7211 0000 00da  r....r....r.....
-00000f90: 083c 6d6f 6475 6c65 3e01 0000 0073 0c00  .<module>....s..
-00000fa0: 0000 0802 0c02 0c01 0c03 0e2b 0e0b       ...........+..
+00000000: 420d 0d0a 0000 0000 0c79 4b5b e20a 0000  B........yK[....
+00000010: e300 0000 0000 0000 0000 0000 0004 0000  ................
+00000020: 0040 0000 0073 5c00 0000 6400 6401 6c00  .@...s\...d.d.l.
+00000030: 5a00 6400 6402 6c01 6d02 5a02 0100 6400  Z.d.d.l.m.Z...d.
+00000040: 6403 6c03 6d04 5a04 0100 6400 6404 6c05  d.l.m.Z...d.d.l.
+00000050: 6d06 5a06 0100 4700 6405 6406 8400 6406  m.Z...G.d.d...d.
+00000060: 8302 5a07 4700 6407 6408 8400 6408 8302  ..Z.G.d.d...d...
+00000070: 5a08 4700 6409 640a 8400 640a 6507 8303  Z.G.d.d...d.e...
+00000080: 5a09 6401 5300 290b e900 0000 004e 2901  Z.d.S.)......N).
+00000090: da05 5175 6572 7929 01da 0c42 6173 6545  ..Query)...BaseE
+000000a0: 7865 6375 746f 7229 01da 1342 6173 6553  xecutor)...BaseS
+000000b0: 6368 656d 6147 656e 6572 6174 6f72 6300  chemaGeneratorc.
+000000c0: 0000 0000 0000 0000 0000 0003 0000 0040  ...............@
+000000d0: 0000 0073 7a00 0000 6500 5a01 6400 5a02  ...sz...e.Z.d.Z.
+000000e0: 6503 5a04 6505 5a06 6507 5a08 641b 6402  e.Z.e.Z.e.Z.d.d.
+000000f0: 6403 8401 5a09 6404 6405 8400 5a0a 6406  d...Z.d.d...Z.d.
+00000100: 6407 8400 5a0b 6408 6409 8400 5a0c 640a  d...Z.d.d...Z.d.
+00000110: 640b 8400 5a0d 640c 640d 8400 5a0e 640e  d...Z.d.d...Z.d.
+00000120: 640f 8400 5a0f 6410 6411 8400 5a10 6412  d...Z.d.d...Z.d.
+00000130: 6413 8400 5a11 6414 6415 8400 5a12 6416  d...Z.d.d...Z.d.
+00000140: 6417 8400 5a13 6418 6419 8400 5a14 641a  d...Z.d.d...Z.d.
+00000150: 5300 291c da11 4261 7365 4442 4173 796e  S.)...BaseDBAsyn
+00000160: 6343 6c69 656e 7446 6302 0000 0000 0000  cClientFc.......
+00000170: 0003 0000 0004 0000 004b 0000 0073 2a00  .........K...s*.
+00000180: 0000 7400 a001 6401 a101 7c00 5f02 7c01  ..t...d...|._.|.
+00000190: 7c00 5f03 7404 6402 7405 7c00 6a06 6602  |._.t.d.t.|.j.f.
+000001a0: 6900 8303 7c00 5f07 6400 5300 2903 4eda  i...|._.d.S.).N.
+000001b0: 0964 625f 636c 6965 6e74 da17 5369 6e67  .db_client..Sing
+000001c0: 6c65 436f 6e6e 6563 7469 6f6e 5772 6170  leConnectionWrap
+000001d0: 7065 7229 08da 076c 6f67 6769 6e67 da09  per)...logging..
+000001e0: 6765 744c 6f67 6765 72da 036c 6f67 da11  getLogger..log..
+000001f0: 7369 6e67 6c65 5f63 6f6e 6e65 6374 696f  single_connectio
+00000200: 6eda 0474 7970 6572 0700 0000 da09 5f5f  n..typer......__
+00000210: 636c 6173 735f 5f5a 185f 7369 6e67 6c65  class__Z._single
+00000220: 5f63 6f6e 6e65 6374 696f 6e5f 636c 6173  _connection_clas
+00000230: 7329 03da 0473 656c 6672 0b00 0000 da06  s)...selfr......
+00000240: 6b77 6172 6773 a900 7210 0000 00fa 512f  kwargs..r.....Q/
+00000250: 5573 6572 732f 616e 6472 6579 626f 6e64  Users/andreybond
+00000260: 6172 2f50 7943 6861 726d 5072 6f6a 6563  ar/PyCharmProjec
+00000270: 7473 2f74 6f72 746f 6973 652d 6f72 6d2f  ts/tortoise-orm/
+00000280: 746f 7274 6f69 7365 2f62 6163 6b65 6e64  tortoise/backend
+00000290: 732f 6261 7365 2f63 6c69 656e 742e 7079  s/base/client.py
+000002a0: da08 5f5f 696e 6974 5f5f 0e00 0000 7308  ..__init__....s.
+000002b0: 0000 0000 010c 0106 0102 017a 1a42 6173  ...........z.Bas
+000002c0: 6544 4241 7379 6e63 436c 6965 6e74 2e5f  eDBAsyncClient._
+000002d0: 5f69 6e69 745f 5f63 0100 0000 0000 0000  _init__c........
+000002e0: 0100 0000 0100 0000 c300 0000 730a 0000  ............s...
+000002f0: 0074 0083 0082 0164 0053 0029 014e 2901  .t.....d.S.).N).
+00000300: da13 4e6f 7449 6d70 6c65 6d65 6e74 6564  ..NotImplemented
+00000310: 4572 726f 7229 0172 0e00 0000 7210 0000  Error).r....r...
+00000320: 0072 1000 0000 7211 0000 00da 1163 7265  .r....r......cre
+00000330: 6174 655f 636f 6e6e 6563 7469 6f6e 1500  ate_connection..
+00000340: 0000 7302 0000 0000 017a 2342 6173 6544  ..s......z#BaseD
+00000350: 4241 7379 6e63 436c 6965 6e74 2e63 7265  BAsyncClient.cre
+00000360: 6174 655f 636f 6e6e 6563 7469 6f6e 6301  ate_connectionc.
+00000370: 0000 0000 0000 0001 0000 0001 0000 00c3  ................
+00000380: 0000 0073 0a00 0000 7400 8300 8201 6400  ...s....t.....d.
+00000390: 5300 2901 4e29 0172 1300 0000 2901 720e  S.).N).r....).r.
+000003a0: 0000 0072 1000 0000 7210 0000 0072 1100  ...r....r....r..
+000003b0: 0000 da05 636c 6f73 6518 0000 0073 0200  ....close....s..
+000003c0: 0000 0001 7a17 4261 7365 4442 4173 796e  ....z.BaseDBAsyn
+000003d0: 6343 6c69 656e 742e 636c 6f73 6563 0100  cClient.closec..
+000003e0: 0000 0000 0000 0100 0000 0100 0000 c300  ................
+000003f0: 0000 730a 0000 0074 0083 0082 0164 0053  ..s....t.....d.S
+00000400: 0029 014e 2901 7213 0000 0029 0172 0e00  .).N).r....).r..
+00000410: 0000 7210 0000 0072 1000 0000 7211 0000  ..r....r....r...
+00000420: 00da 0964 625f 6372 6561 7465 1b00 0000  ...db_create....
+00000430: 7302 0000 0000 017a 1b42 6173 6544 4241  s......z.BaseDBA
+00000440: 7379 6e63 436c 6965 6e74 2e64 625f 6372  syncClient.db_cr
+00000450: 6561 7465 6301 0000 0000 0000 0001 0000  eatec...........
+00000460: 0001 0000 00c3 0000 0073 0a00 0000 7400  .........s....t.
+00000470: 8300 8201 6400 5300 2901 4e29 0172 1300  ....d.S.).N).r..
+00000480: 0000 2901 720e 0000 0072 1000 0000 7210  ..).r....r....r.
+00000490: 0000 0072 1100 0000 da09 6462 5f64 656c  ...r......db_del
+000004a0: 6574 651e 0000 0073 0200 0000 0001 7a1b  ete....s......z.
+000004b0: 4261 7365 4442 4173 796e 6343 6c69 656e  BaseDBAsyncClien
+000004c0: 742e 6462 5f64 656c 6574 6563 0100 0000  t.db_deletec....
+000004d0: 0000 0000 0100 0000 0100 0000 4300 0000  ............C...
+000004e0: 730a 0000 0074 0083 0082 0164 0053 0029  s....t.....d.S.)
+000004f0: 014e 2901 7213 0000 0029 0172 0e00 0000  .N).r....).r....
+00000500: 7210 0000 0072 1000 0000 7211 0000 00da  r....r....r.....
+00000510: 1261 6371 7569 7265 5f63 6f6e 6e65 6374  .acquire_connect
+00000520: 696f 6e21 0000 0073 0200 0000 0001 7a24  ion!...s......z$
+00000530: 4261 7365 4442 4173 796e 6343 6c69 656e  BaseDBAsyncClien
+00000540: 742e 6163 7175 6972 655f 636f 6e6e 6563  t.acquire_connec
+00000550: 7469 6f6e 6301 0000 0000 0000 0001 0000  tionc...........
+00000560: 0001 0000 0043 0000 0073 0a00 0000 7400  .....C...s....t.
+00000570: 8300 8201 6400 5300 2901 4e29 0172 1300  ....d.S.).N).r..
+00000580: 0000 2901 720e 0000 0072 1000 0000 7210  ..).r....r....r.
+00000590: 0000 0072 1100 0000 da0e 696e 5f74 7261  ...r......in_tra
+000005a0: 6e73 6163 7469 6f6e 2400 0000 7302 0000  nsaction$...s...
+000005b0: 0000 017a 2042 6173 6544 4241 7379 6e63  ...z BaseDBAsync
+000005c0: 436c 6965 6e74 2e69 6e5f 7472 616e 7361  Client.in_transa
+000005d0: 6374 696f 6e63 0100 0000 0000 0000 0100  ctionc..........
+000005e0: 0000 0100 0000 4300 0000 730a 0000 0074  ......C...s....t
+000005f0: 0083 0082 0164 0053 0029 014e 2901 7213  .....d.S.).N).r.
+00000600: 0000 0029 0172 0e00 0000 7210 0000 0072  ...).r....r....r
+00000610: 1000 0000 7211 0000 00da 0d69 6e5f 636f  ....r......in_co
+00000620: 6e6e 6563 7469 6f6e 2700 0000 7302 0000  nnection'...s...
+00000630: 0000 017a 1f42 6173 6544 4241 7379 6e63  ...z.BaseDBAsync
+00000640: 436c 6965 6e74 2e69 6e5f 636f 6e6e 6563  Client.in_connec
+00000650: 7469 6f6e 6302 0000 0000 0000 0002 0000  tionc...........
+00000660: 0001 0000 00c3 0000 0073 0a00 0000 7400  .........s....t.
+00000670: 8300 8201 6400 5300 2901 4e29 0172 1300  ....d.S.).N).r..
+00000680: 0000 2902 720e 0000 00da 0571 7565 7279  ..).r......query
+00000690: 7210 0000 0072 1000 0000 7211 0000 00da  r....r....r.....
+000006a0: 0d65 7865 6375 7465 5f71 7565 7279 2a00  .execute_query*.
+000006b0: 0000 7302 0000 0000 017a 1f42 6173 6544  ..s......z.BaseD
+000006c0: 4241 7379 6e63 436c 6965 6e74 2e65 7865  BAsyncClient.exe
+000006d0: 6375 7465 5f71 7565 7279 6302 0000 0000  cute_queryc.....
+000006e0: 0000 0002 0000 0001 0000 00c3 0000 0073  ...............s
+000006f0: 0a00 0000 7400 8300 8201 6400 5300 2901  ....t.....d.S.).
+00000700: 4e29 0172 1300 0000 2902 720e 0000 005a  N).r....).r....Z
+00000710: 0673 6372 6970 7472 1000 0000 7210 0000  .scriptr....r...
+00000720: 0072 1100 0000 da0e 6578 6563 7574 655f  .r......execute_
+00000730: 7363 7269 7074 2d00 0000 7302 0000 0000  script-...s.....
+00000740: 017a 2042 6173 6544 4241 7379 6e63 436c  .z BaseDBAsyncCl
+00000750: 6965 6e74 2e65 7865 6375 7465 5f73 6372  ient.execute_scr
+00000760: 6970 7463 0100 0000 0000 0000 0100 0000  iptc............
+00000770: 0100 0000 c300 0000 730a 0000 0074 0083  ........s....t..
+00000780: 0082 0164 0053 0029 014e 2901 7213 0000  ...d.S.).N).r...
+00000790: 0029 0172 0e00 0000 7210 0000 0072 1000  .).r....r....r..
+000007a0: 0000 7211 0000 00da 1567 6574 5f73 696e  ..r......get_sin
+000007b0: 676c 655f 636f 6e6e 6563 7469 6f6e 3000  gle_connection0.
+000007c0: 0000 7302 0000 0000 017a 2742 6173 6544  ..s......z'BaseD
+000007d0: 4241 7379 6e63 436c 6965 6e74 2e67 6574  BAsyncClient.get
+000007e0: 5f73 696e 676c 655f 636f 6e6e 6563 7469  _single_connecti
+000007f0: 6f6e 6302 0000 0000 0000 0002 0000 0001  onc.............
+00000800: 0000 00c3 0000 0073 0a00 0000 7400 8300  .......s....t...
+00000810: 8201 6400 5300 2901 4e29 0172 1300 0000  ..d.S.).N).r....
+00000820: 2902 720e 0000 0072 0b00 0000 7210 0000  ).r....r....r...
+00000830: 0072 1000 0000 7211 0000 00da 1972 656c  .r....r......rel
+00000840: 6561 7365 5f73 696e 676c 655f 636f 6e6e  ease_single_conn
+00000850: 6563 7469 6f6e 3300 0000 7302 0000 0000  ection3...s.....
+00000860: 017a 2b42 6173 6544 4241 7379 6e63 436c  .z+BaseDBAsyncCl
+00000870: 6965 6e74 2e72 656c 6561 7365 5f73 696e  ient.release_sin
+00000880: 676c 655f 636f 6e6e 6563 7469 6f6e 4e29  gle_connectionN)
+00000890: 0146 2915 da08 5f5f 6e61 6d65 5f5f da0a  .F)...__name__..
+000008a0: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
+000008b0: 616c 6e61 6d65 5f5f 7202 0000 00da 0b71  alname__r......q
+000008c0: 7565 7279 5f63 6c61 7373 7203 0000 005a  uery_classr....Z
+000008d0: 0e65 7865 6375 746f 725f 636c 6173 7372  .executor_classr
+000008e0: 0400 0000 da10 7363 6865 6d61 5f67 656e  ......schema_gen
+000008f0: 6572 6174 6f72 7212 0000 0072 1400 0000  eratorr....r....
+00000900: 7215 0000 0072 1600 0000 7217 0000 0072  r....r....r....r
+00000910: 1800 0000 7219 0000 0072 1a00 0000 721c  ....r....r....r.
+00000920: 0000 0072 1d00 0000 721e 0000 0072 1f00  ...r....r....r..
+00000930: 0000 7210 0000 0072 1000 0000 7210 0000  ..r....r....r...
+00000940: 0072 1100 0000 7205 0000 0009 0000 0073  .r....r........s
+00000950: 1e00 0000 0801 0401 0401 0402 0a07 0803  ................
+00000960: 0803 0803 0803 0803 0803 0803 0803 0803  ................
+00000970: 0803 7205 0000 0063 0000 0000 0000 0000  ..r....c........
+00000980: 0000 0000 0200 0000 4000 0000 7324 0000  ........@...s$..
+00000990: 0065 005a 0164 005a 0264 0164 0284 005a  .e.Z.d.Z.d.d...Z
+000009a0: 0364 0364 0484 005a 0464 0564 0684 005a  .d.d...Z.d.d...Z
+000009b0: 0564 0753 0029 08da 1143 6f6e 6e65 6374  .d.S.)...Connect
+000009c0: 696f 6e57 7261 7070 6572 6302 0000 0000  ionWrapperc.....
+000009d0: 0000 0002 0000 0002 0000 0043 0000 0073  ...........C...s
+000009e0: 0a00 0000 7c01 7c00 5f00 6400 5300 2901  ....|.|._.d.S.).
+000009f0: 4e29 01da 0a63 6f6e 6e65 6374 696f 6e29  N)...connection)
+00000a00: 0272 0e00 0000 7226 0000 0072 1000 0000  .r....r&...r....
+00000a10: 7210 0000 0072 1100 0000 7212 0000 0038  r....r....r....8
+00000a20: 0000 0073 0200 0000 0001 7a1a 436f 6e6e  ...s......z.Conn
+00000a30: 6563 7469 6f6e 5772 6170 7065 722e 5f5f  ectionWrapper.__
+00000a40: 696e 6974 5f5f 6301 0000 0000 0000 0001  init__c.........
+00000a50: 0000 0001 0000 00c3 0000 0073 0600 0000  ...........s....
+00000a60: 7c00 6a00 5300 2901 4e29 0172 2600 0000  |.j.S.).N).r&...
+00000a70: 2901 720e 0000 0072 1000 0000 7210 0000  ).r....r....r...
+00000a80: 0072 1100 0000 da0a 5f5f 6165 6e74 6572  .r......__aenter
+00000a90: 5f5f 3b00 0000 7302 0000 0000 017a 1c43  __;...s......z.C
+00000aa0: 6f6e 6e65 6374 696f 6e57 7261 7070 6572  onnectionWrapper
+00000ab0: 2e5f 5f61 656e 7465 725f 5f63 0400 0000  .__aenter__c....
+00000ac0: 0000 0000 0400 0000 0100 0000 c300 0000  ................
+00000ad0: 7304 0000 0064 0053 0029 014e 7210 0000  s....d.S.).Nr...
+00000ae0: 0029 0472 0e00 0000 da08 6578 635f 7479  .).r......exc_ty
+00000af0: 7065 da07 6578 635f 7661 6cda 0665 7863  pe..exc_val..exc
+00000b00: 5f74 6272 1000 0000 7210 0000 0072 1100  _tbr....r....r..
+00000b10: 0000 da09 5f5f 6165 7869 745f 5f3e 0000  ....__aexit__>..
+00000b20: 0073 0200 0000 0001 7a1b 436f 6e6e 6563  .s......z.Connec
+00000b30: 7469 6f6e 5772 6170 7065 722e 5f5f 6165  tionWrapper.__ae
+00000b40: 7869 745f 5f4e 2906 7220 0000 0072 2100  xit__N).r ...r!.
+00000b50: 0000 7222 0000 0072 1200 0000 7227 0000  ..r"...r....r'..
+00000b60: 0072 2b00 0000 7210 0000 0072 1000 0000  .r+...r....r....
+00000b70: 7210 0000 0072 1100 0000 7225 0000 0037  r....r....r%...7
+00000b80: 0000 0073 0600 0000 0801 0803 0803 7225  ...s..........r%
+00000b90: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+00000ba0: 0300 0000 4000 0000 733e 0000 0065 005a  ....@...s>...e.Z
+00000bb0: 0164 005a 0264 0e64 0264 0384 015a 0364  .d.Z.d.d.d...Z.d
+00000bc0: 0464 0584 005a 0464 0664 0784 005a 0564  .d...Z.d.d...Z.d
+00000bd0: 0864 0984 005a 0664 0a64 0b84 005a 0764  .d...Z.d.d...Z.d
+00000be0: 0c64 0d84 005a 0864 0153 0029 0f72 0700  .d...Z.d.S.).r..
+00000bf0: 0000 4e63 0300 0000 0000 0000 0300 0000  ..Nc............
+00000c00: 0300 0000 4300 0000 7322 0000 007c 017c  ....C...s"...|.|
+00000c10: 005f 0074 01a0 0264 01a1 017c 005f 0364  ._.t...d...|._.d
+00000c20: 027c 005f 047c 027c 005f 0564 0053 0029  .|._.|.|._.d.S.)
+00000c30: 034e 7206 0000 0054 2906 7226 0000 0072  .Nr....T).r&...r
+00000c40: 0800 0000 7209 0000 0072 0a00 0000 720b  ....r....r....r.
+00000c50: 0000 00da 1063 6c6f 7369 6e67 5f63 616c  .....closing_cal
+00000c60: 6c62 6163 6b29 0372 0e00 0000 7226 0000  lback).r....r&..
+00000c70: 0072 2c00 0000 7210 0000 0072 1000 0000  .r,...r....r....
+00000c80: 7211 0000 0072 1200 0000 4300 0000 7308  r....r....C...s.
+00000c90: 0000 0000 0106 010c 0106 017a 2053 696e  ...........z Sin
+00000ca0: 676c 6543 6f6e 6e65 6374 696f 6e57 7261  gleConnectionWra
+00000cb0: 7070 6572 2e5f 5f69 6e69 745f 5f63 0100  pper.__init__c..
+00000cc0: 0000 0000 0000 0100 0000 0200 0000 4300  ..............C.
+00000cd0: 0000 730a 0000 0074 007c 006a 0183 0153  ..s....t.|.j...S
+00000ce0: 0029 014e 2902 7225 0000 0072 2600 0000  .).N).r%...r&...
+00000cf0: 2901 720e 0000 0072 1000 0000 7210 0000  ).r....r....r...
+00000d00: 0072 1100 0000 7218 0000 0049 0000 0073  .r....r....I...s
+00000d10: 0200 0000 0001 7a2a 5369 6e67 6c65 436f  ......z*SingleCo
+00000d20: 6e6e 6563 7469 6f6e 5772 6170 7065 722e  nnectionWrapper.
+00000d30: 6163 7175 6972 655f 636f 6e6e 6563 7469  acquire_connecti
+00000d40: 6f6e 6301 0000 0000 0000 0001 0000 0004  onc.............
+00000d50: 0000 00c3 0000 0073 0e00 0000 7c00 a000  .......s....|...
+00000d60: 7c00 6a01 7c00 a102 5300 2901 4e29 0272  |.j.|...S.).N).r
+00000d70: 0d00 0000 7226 0000 0029 0172 0e00 0000  ....r&...).r....
+00000d80: 7210 0000 0072 1000 0000 7211 0000 0072  r....r....r....r
+00000d90: 1e00 0000 4c00 0000 7302 0000 0000 037a  ....L...s......z
+00000da0: 2d53 696e 676c 6543 6f6e 6e65 6374 696f  -SingleConnectio
+00000db0: 6e57 7261 7070 6572 2e67 6574 5f73 696e  nWrapper.get_sin
+00000dc0: 676c 655f 636f 6e6e 6563 7469 6f6e 6302  gle_connectionc.
+00000dd0: 0000 0000 0000 0002 0000 0001 0000 00c3  ................
+00000de0: 0000 0073 0400 0000 6400 5300 2901 4e72  ...s....d.S.).Nr
+00000df0: 1000 0000 2902 720e 0000 0072 0b00 0000  ....).r....r....
+00000e00: 7210 0000 0072 1000 0000 7211 0000 0072  r....r....r....r
+00000e10: 1f00 0000 5100 0000 7302 0000 0000 017a  ....Q...s......z
+00000e20: 3153 696e 676c 6543 6f6e 6e65 6374 696f  1SingleConnectio
+00000e30: 6e57 7261 7070 6572 2e72 656c 6561 7365  nWrapper.release
+00000e40: 5f73 696e 676c 655f 636f 6e6e 6563 7469  _single_connecti
+00000e50: 6f6e 6301 0000 0000 0000 0001 0000 0001  onc.............
+00000e60: 0000 00c3 0000 0073 0400 0000 7c00 5300  .......s....|.S.
+00000e70: 2901 4e72 1000 0000 2901 720e 0000 0072  ).Nr....).r....r
+00000e80: 1000 0000 7210 0000 0072 1100 0000 7227  ....r....r....r'
+00000e90: 0000 0054 0000 0073 0200 0000 0001 7a22  ...T...s......z"
+00000ea0: 5369 6e67 6c65 436f 6e6e 6563 7469 6f6e  SingleConnection
+00000eb0: 5772 6170 7065 722e 5f5f 6165 6e74 6572  Wrapper.__aenter
+00000ec0: 5f5f 6304 0000 0000 0000 0004 0000 0003  __c.............
+00000ed0: 0000 00c3 0000 0073 1a00 0000 7c00 6a00  .......s....|.j.
+00000ee0: 7216 7c00 a000 7c00 a101 4900 6400 4800  r.|...|...I.d.H.
+00000ef0: 0100 6400 5300 2901 4e29 0172 2c00 0000  ..d.S.).N).r,...
+00000f00: 2904 720e 0000 0072 2800 0000 7229 0000  ).r....r(...r)..
+00000f10: 0072 2a00 0000 7210 0000 0072 1000 0000  .r*...r....r....
+00000f20: 7211 0000 0072 2b00 0000 5700 0000 7304  r....r+...W...s.
+00000f30: 0000 0000 0106 017a 2153 696e 676c 6543  .......z!SingleC
+00000f40: 6f6e 6e65 6374 696f 6e57 7261 7070 6572  onnectionWrapper
+00000f50: 2e5f 5f61 6578 6974 5f5f 2901 4e29 0972  .__aexit__).N).r
+00000f60: 2000 0000 7221 0000 0072 2200 0000 7212   ...r!...r"...r.
+00000f70: 0000 0072 1800 0000 721e 0000 0072 1f00  ...r....r....r..
+00000f80: 0000 7227 0000 0072 2b00 0000 7210 0000  ..r'...r+...r...
+00000f90: 0072 1000 0000 7210 0000 0072 1100 0000  .r....r....r....
+00000fa0: 7207 0000 0042 0000 0073 0c00 0000 0801  r....B...s......
+00000fb0: 0a06 0803 0805 0803 0803 7207 0000 0029  ..........r....)
+00000fc0: 0a72 0800 0000 da06 7079 7069 6b61 7202  .r......pypikar.
+00000fd0: 0000 005a 1f74 6f72 746f 6973 652e 6261  ...Z.tortoise.ba
+00000fe0: 636b 656e 6473 2e62 6173 652e 6578 6563  ckends.base.exec
+00000ff0: 7574 6f72 7203 0000 005a 2774 6f72 746f  utorr....Z'torto
+00001000: 6973 652e 6261 636b 656e 6473 2e62 6173  ise.backends.bas
+00001010: 652e 7363 6865 6d61 5f67 656e 6572 6174  e.schema_generat
+00001020: 6f72 7204 0000 0072 0500 0000 7225 0000  orr....r....r%..
+00001030: 0072 0700 0000 7210 0000 0072 1000 0000  .r....r....r....
+00001040: 7210 0000 0072 1100 0000 da08 3c6d 6f64  r....r......<mod
+00001050: 756c 653e 0100 0000 730c 0000 0008 020c  ule>....s.......
+00001060: 020c 010c 030e 2e0e 0b                   .........
```

### Comparing `tortoise-orm-0.9.2/tortoise/backends/base/__pycache__/schema_generator.cpython-36.pyc` & `tortoise-orm-0.9.4/tortoise/backends/base/__pycache__/schema_generator.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `tortoise-orm-0.9.2/tortoise/backends/base/__pycache__/executor.cpython-36.pyc` & `tortoise-orm-0.9.4/tortoise/backends/base/__pycache__/executor.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.6 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 10% similar despite different names*

```diff
@@ -1,514 +1,517 @@
-00000000: 330d 0d0a 5576 3f5b 7928 0000 e300 0000  3...Uv?[y(......
+00000000: 330d 0d0a dc7e 445b c728 0000 e300 0000  3....~D[.(......
 00000010: 0000 0000 0000 0000 0003 0000 0040 0000  .............@..
-00000020: 0073 3200 0000 6400 6401 6c00 5a00 6400  .s2...d.d.l.Z.d.
+00000020: 0073 3e00 0000 6400 6401 6c00 5a00 6400  .s>...d.d.l.Z.d.
 00000030: 6402 6c01 6d02 5a02 0100 6400 6403 6c03  d.l.m.Z...d.d.l.
-00000040: 6d04 5a04 0100 4700 6404 6405 8400 6405  m.Z...G.d.d...d.
-00000050: 8302 5a05 6401 5300 2906 e900 0000 004e  ..Z.d.S.)......N
-00000060: 2901 da05 5461 626c 6529 01da 0666 6965  )...Table)...fie
-00000070: 6c64 7363 0000 0000 0000 0000 0000 0000  ldsc............
-00000080: 0300 0000 4000 0000 7390 0000 0065 005a  ....@...s....e.Z
-00000090: 0164 005a 0264 2264 0264 0384 015a 0364  .d.Z.d"d.d...Z.d
-000000a0: 2364 0464 0584 015a 0464 0664 0784 005a  #d.d...Z.d.d...Z
-000000b0: 0564 0864 0984 005a 0664 0a64 0b84 005a  .d.d...Z.d.d...Z
-000000c0: 0764 0c64 0d84 005a 0864 0e64 0f84 005a  .d.d...Z.d.d...Z
-000000d0: 0964 1064 1184 005a 0a64 1264 1384 005a  .d.d...Z.d.d...Z
-000000e0: 0b64 1464 1584 005a 0c64 1664 1784 005a  .d.d...Z.d.d...Z
-000000f0: 0d64 1864 1984 005a 0e64 1a64 1b84 005a  .d.d...Z.d.d...Z
-00000100: 0f64 1c64 1d84 005a 1064 1e64 1f84 005a  .d.d...Z.d.d...Z
-00000110: 1164 2064 2184 005a 1264 0153 0029 24da  .d d!..Z.d.S.)$.
-00000120: 0c42 6173 6545 7865 6375 746f 724e 6305  .BaseExecutorNc.
-00000130: 0000 0000 0000 0005 0000 0002 0000 0043  ...............C
-00000140: 0000 0073 3200 0000 7c01 7c00 5f00 7c02  ...s2...|.|._.|.
-00000150: 7c00 5f01 6400 7c00 5f02 7c03 721a 7c03  |._.d.|._.|.r.|.
-00000160: 6e02 6900 7c00 5f03 7c04 7228 7c04 6e02  n.i.|._.|.r(|.n.
-00000170: 6900 7c00 5f04 6400 5300 2901 4e29 05da  i.|._.d.S.).N)..
-00000180: 056d 6f64 656c da02 6462 da0a 636f 6e6e  .model..db..conn
-00000190: 6563 7469 6f6e da0c 7072 6566 6574 6368  ection..prefetch
-000001a0: 5f6d 6170 da11 5f70 7265 6665 7463 685f  _map.._prefetch_
-000001b0: 7175 6572 6965 7329 05da 0473 656c 6672  queries)...selfr
-000001c0: 0500 0000 7206 0000 0072 0800 0000 5a10  ....r....r....Z.
-000001d0: 7072 6566 6574 6368 5f71 7565 7269 6573  prefetch_queries
-000001e0: a900 720b 0000 00fa 532f 5573 6572 732f  ..r.....S/Users/
-000001f0: 616e 6472 6579 626f 6e64 6172 2f50 7943  andreybondar/PyC
-00000200: 6861 726d 5072 6f6a 6563 7473 2f74 6f72  harmProjects/tor
-00000210: 746f 6973 652d 6f72 6d2f 746f 7274 6f69  toise-orm/tortoi
-00000220: 7365 2f62 6163 6b65 6e64 732f 6261 7365  se/backends/base
-00000230: 2f65 7865 6375 746f 722e 7079 da08 5f5f  /executor.py..__
-00000240: 696e 6974 5f5f 0900 0000 730a 0000 0000  init__....s.....
-00000250: 0106 0106 0106 010e 017a 1542 6173 6545  .........z.BaseE
-00000260: 7865 6375 746f 722e 5f5f 696e 6974 5f5f  xecutor.__init__
-00000270: 6303 0000 0000 0000 0008 0000 0007 0000  c...............
-00000280: 00c3 0000 0073 a000 0000 7c00 6a00 6a01  .....s....|.j.j.
-00000290: 8300 4900 6400 4800 7c00 5f02 7c00 6a02  ..I.d.H.|._.|.j.
-000002a0: 6a03 7404 7c01 8301 8301 4900 6400 4800  j.t.|.....I.d.H.
-000002b0: 7d03 6700 7d04 7844 7c03 4400 5d3c 7d05  }.g.}.xD|.D.]<}.
-000002c0: 7c00 6a05 6600 7c05 8e01 7d06 7c02 7264  |.j.f.|...}.|.rd
-000002d0: 781c 7c02 4400 5d14 7d07 7406 7c06 7c07  x.|.D.].}.t.|.|.
-000002e0: 7c05 7c07 1900 8303 0100 714c 5700 7c04  |.|.......qLW.|.
-000002f0: 6a07 7c06 8301 0100 7132 5700 7c00 6a08  j.|.....q2W.|.j.
-00000300: 7c04 8301 4900 6400 4800 0100 7c00 6a00  |...I.d.H...|.j.
-00000310: 6a09 7c00 6a02 8301 4900 6400 4800 0100  j.|.j...I.d.H...
-00000320: 6400 7c00 5f02 7c04 5300 2901 4e29 0a72  d.|._.|.S.).N).r
-00000330: 0600 0000 da15 6765 745f 7369 6e67 6c65  ......get_single
-00000340: 5f63 6f6e 6e65 6374 696f 6e72 0700 0000  _connectionr....
-00000350: da0d 6578 6563 7574 655f 7175 6572 79da  ..execute_query.
-00000360: 0373 7472 7205 0000 00da 0773 6574 6174  .strr......setat
-00000370: 7472 da06 6170 7065 6e64 da19 5f65 7865  tr..append.._exe
-00000380: 6375 7465 5f70 7265 6665 7463 685f 7175  cute_prefetch_qu
-00000390: 6572 6965 73da 1972 656c 6561 7365 5f73  eries..release_s
-000003a0: 696e 676c 655f 636f 6e6e 6563 7469 6f6e  ingle_connection
-000003b0: 2908 720a 0000 00da 0571 7565 7279 5a0d  ).r......queryZ.
-000003c0: 6375 7374 6f6d 5f66 6965 6c64 73da 0b72  custom_fields..r
-000003d0: 6177 5f72 6573 756c 7473 da0d 696e 7374  aw_results..inst
-000003e0: 616e 6365 5f6c 6973 74da 0372 6f77 da08  ance_list..row..
-000003f0: 696e 7374 616e 6365 da05 6669 656c 6472  instance..fieldr
-00000400: 0b00 0000 720b 0000 0072 0c00 0000 da0e  ....r....r......
-00000410: 6578 6563 7574 655f 7365 6c65 6374 1000  execute_select..
-00000420: 0000 731a 0000 0000 0112 0116 0104 010a  ..s.............
-00000430: 010c 0104 010a 0114 010e 0110 0114 0106  ................
-00000440: 017a 1b42 6173 6545 7865 6375 746f 722e  .z.BaseExecutor.
-00000450: 6578 6563 7574 655f 7365 6c65 6374 6301  execute_selectc.
-00000460: 0000 0000 0000 0006 0000 0004 0000 0043  ...............C
-00000470: 0000 0073 7600 0000 6700 7d01 6700 7d02  ...sv...g.}.g.}.
-00000480: 7400 6a00 6a01 8300 7d03 785a 7c00 6a02  t.j.j...}.xZ|.j.
-00000490: 6a03 6a04 6a05 8300 4400 5d48 7d04 7c00  j.j.j...D.]H}.|.
-000004a0: 6a02 6a03 6a06 7c04 1900 7d05 7407 7c05  j.j.j.|...}.t.|.
-000004b0: 7408 6a09 8302 7256 7c05 6a0a 7256 7c02  t.j...rV|.j.rV|.
-000004c0: 6a0b 7c04 7c03 6602 8301 0100 7122 7c05  j.|.|.f.....q"|.
-000004d0: 6a0c 7260 7122 7122 7c01 6a0b 7c04 8301  j.r`q"q"|.j.|...
-000004e0: 0100 7122 5700 7c01 7c02 6602 5300 2901  ..q"W.|.|.f.S.).
-000004f0: 4e29 0dda 0864 6174 6574 696d 65da 0675  N)...datetime..u
-00000500: 7463 6e6f 7772 0500 0000 da05 5f6d 6574  tcnowr......_met
-00000510: 61da 1466 6965 6c64 735f 6462 5f70 726f  a..fields_db_pro
-00000520: 6a65 6374 696f 6eda 046b 6579 73da 0a66  jection..keys..f
-00000530: 6965 6c64 735f 6d61 70da 0a69 7369 6e73  ields_map..isins
-00000540: 7461 6e63 6572 0300 0000 da0d 4461 7465  tancer......Date
-00000550: 7469 6d65 4669 656c 64da 0c61 7574 6f5f  timeField..auto_
-00000560: 6e6f 775f 6164 6472 1200 0000 da09 6765  now_addr......ge
-00000570: 6e65 7261 7465 6429 0672 0a00 0000 da0f  nerated).r......
-00000580: 7265 6775 6c61 725f 636f 6c75 6d6e 735a  regular_columnsZ
-00000590: 1d70 7974 686f 6e5f 6765 6e65 7261 7465  .python_generate
-000005a0: 645f 636f 6c75 6d6e 5f70 6169 7273 da03  d_column_pairs..
-000005b0: 6e6f 77da 0663 6f6c 756d 6eda 0c66 6965  now..column..fie
-000005c0: 6c64 5f6f 626a 6563 7472 0b00 0000 720b  ld_objectr....r.
-000005d0: 0000 0072 0c00 0000 da17 5f70 7265 7061  ...r......_prepa
-000005e0: 7265 5f69 6e73 6572 745f 636f 6c75 6d6e  re_insert_column
-000005f0: 731f 0000 0073 1600 0000 0001 0401 0401  s....s..........
-00000600: 0a01 1401 0e01 1201 1001 0601 0402 0e01  ................
-00000610: 7a24 4261 7365 4578 6563 7574 6f72 2e5f  z$BaseExecutor._
-00000620: 7072 6570 6172 655f 696e 7365 7274 5f63  prepare_insert_c
-00000630: 6f6c 756d 6e73 6303 0000 0000 0000 0003  olumnsc.........
-00000640: 0000 0002 0000 0043 0000 0073 0a00 0000  .......C...s....
-00000650: 7c01 6a00 7c02 8301 5300 2901 4e29 01da  |.j.|...S.).N)..
-00000660: 0b74 6f5f 6462 5f76 616c 7565 2903 720a  .to_db_value).r.
-00000670: 0000 0072 2900 0000 da04 6174 7472 720b  ...r).....attrr.
-00000680: 0000 0072 0b00 0000 720c 0000 00da 0c5f  ...r....r......_
-00000690: 6669 656c 645f 746f 5f64 622d 0000 0073  field_to_db-...s
-000006a0: 0200 0000 0001 7a19 4261 7365 4578 6563  ......z.BaseExec
-000006b0: 7574 6f72 2e5f 6669 656c 645f 746f 5f64  utor._field_to_d
-000006c0: 6263 0300 0000 0000 0000 0300 0000 0500  bc..............
-000006d0: 0000 4300 0000 731c 0000 007c 006a 007c  ..C...s....|.j.|
-000006e0: 006a 016a 026a 037c 0219 0074 047c 017c  .j.j.j.|...t.|.|
-000006f0: 0283 0283 0253 0029 014e 2905 722d 0000  .....S.).N).r-..
-00000700: 0072 0500 0000 721e 0000 0072 2100 0000  .r....r....r!...
-00000710: da07 6765 7461 7474 7229 0372 0a00 0000  ..getattr).r....
-00000720: 7219 0000 0072 2800 0000 720b 0000 0072  r....r(...r....r
-00000730: 0b00 0000 720c 0000 00da 135f 6765 745f  ....r......_get_
-00000740: 7072 6570 6172 6564 5f76 616c 7565 3000  prepared_value0.
-00000750: 0000 7302 0000 0000 017a 2042 6173 6545  ..s......z BaseE
-00000760: 7865 6375 746f 722e 5f67 6574 5f70 7265  xecutor._get_pre
-00000770: 7061 7265 645f 7661 6c75 6563 0400 0000  pared_valuec....
-00000780: 0000 0000 0800 0000 0500 0000 0300 0000  ................
-00000790: 736a 0000 0087 0087 0166 0264 0164 0284  sj.......f.d.d..
-000007a0: 087c 0244 0083 017d 0487 0166 0164 0364  .|.D...}...f.d.d
-000007b0: 0284 087c 0244 0083 017d 0578 3a7c 0344  ...|.D...}.x:|.D
-000007c0: 005d 325c 027d 067d 077c 056a 0088 016a  .]2\.}.}.|.j...j
-000007d0: 016a 026a 037c 0619 0083 0101 007c 046a  .j.j.|.......|.j
-000007e0: 007c 0783 0101 0074 0488 007c 067c 0783  .|.....t...|.|..
-000007f0: 0301 0071 2c57 007c 057c 0466 0253 0029  ...q,W.|.|.f.S.)
-00000800: 044e 6301 0000 0000 0000 0002 0000 0005  .Nc.............
-00000810: 0000 0013 0000 0073 1800 0000 6700 7c00  .......s....g.|.
-00000820: 5d10 7d01 8801 6a00 8800 7c01 8302 9102  ].}...j...|.....
-00000830: 7104 5300 720b 0000 0029 0172 2f00 0000  q.S.r....).r/...
-00000840: 2902 da02 2e30 7228 0000 0029 0272 1900  )....0r(...).r..
-00000850: 0000 720a 0000 0072 0b00 0000 720c 0000  ..r....r....r...
-00000860: 00fa 0a3c 6c69 7374 636f 6d70 3e34 0000  ...<listcomp>4..
-00000870: 0073 0200 0000 0600 7a37 4261 7365 4578  .s......z7BaseEx
-00000880: 6563 7574 6f72 2e5f 7072 6570 6172 655f  ecutor._prepare_
-00000890: 696e 7365 7274 5f76 616c 7565 732e 3c6c  insert_values.<l
-000008a0: 6f63 616c 733e 2e3c 6c69 7374 636f 6d70  ocals>.<listcomp
-000008b0: 3e63 0100 0000 0000 0000 0200 0000 0400  >c..............
-000008c0: 0000 1300 0000 731a 0000 0067 007c 005d  ......s....g.|.]
-000008d0: 127d 0188 006a 006a 016a 027c 0119 0091  .}...j.j.j.|....
-000008e0: 0271 0453 0072 0b00 0000 2903 7205 0000  .q.S.r....).r...
-000008f0: 0072 1e00 0000 721f 0000 0029 0272 3000  .r....r....).r0.
-00000900: 0000 da01 6329 0172 0a00 0000 720b 0000  ....c).r....r...
-00000910: 0072 0c00 0000 7231 0000 0035 0000 0073  .r....r1...5...s
-00000920: 0200 0000 0600 2905 7212 0000 0072 0500  ......).r....r..
-00000930: 0000 721e 0000 0072 1f00 0000 7211 0000  ..r....r....r...
-00000940: 0029 0872 0a00 0000 7219 0000 0072 2600  .).r....r....r&.
-00000950: 0000 5a16 6765 6e65 7261 7465 645f 636f  ..Z.generated_co
-00000960: 6c75 6d6e 5f70 6169 7273 da06 7661 6c75  lumn_pairs..valu
-00000970: 6573 5a0e 7265 7375 6c74 5f63 6f6c 756d  esZ.result_colum
-00000980: 6e73 7228 0000 00da 0576 616c 7565 720b  nsr(.....valuer.
-00000990: 0000 0029 0272 1900 0000 720a 0000 0072  ...).r....r....r
-000009a0: 0c00 0000 da16 5f70 7265 7061 7265 5f69  ......_prepare_i
-000009b0: 6e73 6572 745f 7661 6c75 6573 3300 0000  nsert_values3...
-000009c0: 730e 0000 0000 0114 0112 010e 0114 010a  s...............
-000009d0: 0110 017a 2342 6173 6545 7865 6375 746f  ...z#BaseExecuto
-000009e0: 722e 5f70 7265 7061 7265 5f69 6e73 6572  r._prepare_inser
-000009f0: 745f 7661 6c75 6573 6302 0000 0000 0000  t_valuesc.......
-00000a00: 0002 0000 0001 0000 00c3 0000 0073 0a00  .............s..
-00000a10: 0000 7400 8300 8201 6400 5300 2901 4e29  ..t.....d.S.).N)
-00000a20: 01da 134e 6f74 496d 706c 656d 656e 7465  ...NotImplemente
-00000a30: 6445 7272 6f72 2902 720a 0000 0072 1900  dError).r....r..
-00000a40: 0000 720b 0000 0072 0b00 0000 720c 0000  ..r....r....r...
-00000a50: 00da 0e65 7865 6375 7465 5f69 6e73 6572  ...execute_inser
-00000a60: 743c 0000 0073 0200 0000 0004 7a1b 4261  t<...s......z.Ba
-00000a70: 7365 4578 6563 7574 6f72 2e65 7865 6375  seExecutor.execu
-00000a80: 7465 5f69 6e73 6572 7463 0200 0000 0000  te_insertc......
-00000a90: 0000 0800 0000 0800 0000 c300 0000 73f8  ..............s.
-00000aa0: 0000 007c 006a 006a 0183 0049 0064 0048  ...|.j.j...I.d.H
-00000ab0: 007c 005f 0274 037c 006a 046a 056a 0683  .|._.t.|.j.j.j..
-00000ac0: 017d 027c 006a 026a 076a 087c 0283 017d  .}.|.j.j.j.|...}
-00000ad0: 0378 827c 006a 046a 056a 096a 0a83 0044  .x.|.j.j.j.j...D
-00000ae0: 005d 705c 027d 047d 057c 006a 046a 056a  .]p\.}.}.|.j.j.j
-00000af0: 0b7c 0419 007d 0674 0c7c 0674 0d6a 0e83  .|...}.t.|.t.j..
-00000b00: 0272 8a7c 066a 0f72 8a74 106a 106a 1183  .r.|.j.r.t.j.j..
-00000b10: 007d 077c 036a 127c 057c 0783 027d 0374  .}.|.j.|.|...}.t
-00000b20: 137c 017c 047c 0783 0301 0071 3e7c 066a  .|.|.|.....q>|.j
-00000b30: 1472 9471 3e71 3e7c 036a 127c 057c 006a  .r.q>q>|.j.|.|.j
-00000b40: 157c 0674 167c 017c 0483 0283 0283 027d  .|.t.|.|.......}
-00000b50: 0371 3e57 007c 036a 177c 026a 187c 016a  .q>W.|.j.|.j.|.j
-00000b60: 186b 0283 017d 037c 006a 026a 1974 1a7c  .k...}.|.j.j.t.|
-00000b70: 0383 0183 0149 0064 0048 0001 007c 006a  .....I.d.H...|.j
-00000b80: 006a 1b7c 006a 0283 0149 0064 0048 0001  .j.|.j...I.d.H..
-00000b90: 0064 007c 005f 027c 0153 0029 014e 291c  .d.|._.|.S.).N).
-00000ba0: 7206 0000 0072 0e00 0000 7207 0000 0072  r....r....r....r
-00000bb0: 0200 0000 7205 0000 0072 1e00 0000 da05  ....r....r......
-00000bc0: 7461 626c 65da 0b71 7565 7279 5f63 6c61  table..query_cla
-00000bd0: 7373 da06 7570 6461 7465 721f 0000 00da  ss..updater.....
-00000be0: 0569 7465 6d73 7221 0000 0072 2200 0000  .itemsr!...r"...
-00000bf0: 7203 0000 0072 2300 0000 da08 6175 746f  r....r#.....auto
-00000c00: 5f6e 6f77 721c 0000 0072 1d00 0000 da03  _nowr....r......
-00000c10: 7365 7472 1100 0000 7225 0000 0072 2d00  setr....r%...r-.
-00000c20: 0000 722e 0000 00da 0577 6865 7265 da02  ..r......where..
-00000c30: 6964 720f 0000 0072 1000 0000 7214 0000  idr....r....r...
-00000c40: 0029 0872 0a00 0000 7219 0000 0072 3800  .).r....r....r8.
-00000c50: 0000 7215 0000 0072 1a00 0000 5a08 6462  ..r....r....Z.db
-00000c60: 5f66 6965 6c64 7229 0000 0072 2700 0000  _fieldr)...r'...
-00000c70: 720b 0000 0072 0b00 0000 720c 0000 00da  r....r....r.....
-00000c80: 0e65 7865 6375 7465 5f75 7064 6174 6542  .execute_updateB
-00000c90: 0000 0073 2600 0000 0001 1201 0e01 0e01  ...s&...........
-00000ca0: 1801 0e01 1201 0a01 0c01 0e01 0601 0402  ................
-00000cb0: 0401 0201 1802 1201 1601 1401 0601 7a1b  ..............z.
-00000cc0: 4261 7365 4578 6563 7574 6f72 2e65 7865  BaseExecutor.exe
-00000cd0: 6375 7465 5f75 7064 6174 6563 0200 0000  cute_updatec....
-00000ce0: 0000 0000 0400 0000 0300 0000 c300 0000  ................
-00000cf0: 7348 0000 0074 007c 006a 016a 026a 0383  sH...t.|.j.j.j..
-00000d00: 017d 027c 006a 046a 056a 067c 0283 016a  .}.|.j.j.j.|...j
-00000d10: 077c 026a 087c 016a 086b 0283 016a 0983  .|.j.|.j.k...j..
-00000d20: 007d 037c 006a 046a 0a74 0b7c 0383 0183  .}.|.j.j.t.|....
-00000d30: 0149 0064 0048 0001 007c 0153 0029 014e  .I.d.H...|.S.).N
-00000d40: 290c 7202 0000 0072 0500 0000 721e 0000  ).r....r....r...
-00000d50: 0072 3800 0000 7206 0000 0072 3900 0000  .r8...r....r9...
-00000d60: da05 6672 6f6d 5f72 3e00 0000 723f 0000  ..from_r>...r?..
-00000d70: 00da 0664 656c 6574 6572 0f00 0000 7210  ...deleter....r.
-00000d80: 0000 0029 0472 0a00 0000 7219 0000 0072  ...).r....r....r
-00000d90: 3800 0000 7215 0000 0072 0b00 0000 720b  8...r....r....r.
-00000da0: 0000 0072 0c00 0000 da0e 6578 6563 7574  ...r......execut
-00000db0: 655f 6465 6c65 7465 5900 0000 7308 0000  e_deleteY...s...
-00000dc0: 0000 010e 0120 0116 017a 1b42 6173 6545  ..... ...z.BaseE
-00000dd0: 7865 6375 746f 722e 6578 6563 7574 655f  xecutor.execute_
-00000de0: 6465 6c65 7465 6304 0000 0000 0000 000d  deletec.........
-00000df0: 0000 0005 0000 00c3 0000 0073 c400 0000  ...........s....
-00000e00: 7400 8300 7d04 7818 7c01 4400 5d10 7d05  t...}.x.|.D.].}.
-00000e10: 7c04 6a01 7c05 6a02 8301 0100 710c 5700  |.j.|.j.....q.W.
-00000e20: 7403 7c00 6a04 7c02 8302 7d06 7c06 6a05  t.|.j.|...}.|.j.
-00000e30: 7d07 7c03 6a06 6600 6401 6a07 7c07 8301  }.|.j.f.d.j.|...
-00000e40: 7408 7c04 8301 6901 8e01 4900 6400 4800  t.|...i...I.d.H.
-00000e50: 7d08 6900 7d09 783c 7c08 4400 5d34 7d0a  }.i.}.x<|.D.]4}.
-00000e60: 7403 7c0a 7c07 8302 7d0b 7c0b 7c09 6a09  t.|.|...}.|.|.j.
-00000e70: 8300 6b06 7286 7c09 7c0b 1900 6a0a 7c0a  ..k.r.|.|...j.|.
-00000e80: 8301 0100 715c 7c0a 6701 7c09 7c0b 3c00  ....q\|.g.|.|.<.
-00000e90: 715c 5700 782a 7c01 4400 5d22 7d05 7403  q\W.x*|.D.]"}.t.
-00000ea0: 7c05 7c02 8302 7d0c 7c0c 6a0b 7c09 6a0c  |.|...}.|.j.|.j.
-00000eb0: 7c05 6a02 6700 8302 8301 0100 719a 5700  |.j.g.......q.W.
-00000ec0: 7c01 5300 2902 4e7a 067b 7d5f 5f69 6e29  |.S.).Nz.{}__in)
-00000ed0: 0d72 3d00 0000 da03 6164 6472 3f00 0000  .r=.....addr?...
-00000ee0: 722e 0000 0072 0500 0000 da0e 7265 6c61  r....r......rela
-00000ef0: 7469 6f6e 5f66 6965 6c64 da06 6669 6c74  tion_field..filt
-00000f00: 6572 da06 666f 726d 6174 da04 6c69 7374  er..format..list
-00000f10: 7220 0000 0072 1200 0000 da15 5f73 6574  r ...r......_set
-00000f20: 5f72 6573 756c 745f 666f 725f 7175 6572  _result_for_quer
-00000f30: 79da 0367 6574 290d 720a 0000 0072 1700  y..get).r....r..
-00000f40: 0000 721a 0000 00da 0d72 656c 6174 6564  ..r......related
-00000f50: 5f71 7565 7279 da0f 696e 7374 616e 6365  _query..instance
-00000f60: 5f69 645f 7365 7472 1900 0000 5a19 6261  _id_setr....Z.ba
-00000f70: 636b 7761 7264 5f72 656c 6174 696f 6e5f  ckward_relation_
-00000f80: 6d61 6e61 6765 7272 4500 0000 da13 7265  managerrE.....re
-00000f90: 6c61 7465 645f 6f62 6a65 6374 5f6c 6973  lated_object_lis
-00000fa0: 74da 1272 656c 6174 6564 5f6f 626a 6563  t..related_objec
-00000fb0: 745f 6d61 70da 0565 6e74 7279 da09 6f62  t_map..entry..ob
-00000fc0: 6a65 6374 5f69 64da 1272 656c 6174 696f  ject_id..relatio
-00000fd0: 6e5f 636f 6e74 6169 6e65 7272 0b00 0000  n_containerr....
-00000fe0: 720b 0000 0072 0c00 0000 da1a 5f70 7265  r....r......_pre
-00000ff0: 6665 7463 685f 7265 7665 7273 655f 7265  fetch_reverse_re
-00001000: 6c61 7469 6f6e 5f00 0000 7322 0000 0000  lation_...s"....
-00001010: 0106 010a 0110 010c 0106 0206 011a 0304  ................
-00001020: 010a 010a 010c 0110 020e 010a 010a 0118  ................
-00001030: 017a 2742 6173 6545 7865 6375 746f 722e  .z'BaseExecutor.
-00001040: 5f70 7265 6665 7463 685f 7265 7665 7273  _prefetch_revers
-00001050: 655f 7265 6c61 7469 6f6e 6304 0000 0000  e_relationc.....
-00001060: 0000 0012 0000 0005 0000 0083 0000 0073  ...............s
-00001070: 9e01 0000 7400 8300 7d04 7818 7c01 4400  ....t...}.x.|.D.
-00001080: 5d10 7d05 7c04 6a01 7c05 6a02 8301 0100  ].}.|.j.|.j.....
-00001090: 710c 5700 7c00 6a03 6a04 6a05 7c02 1900  q.W.|.j.j.j.|...
-000010a0: 7d06 7406 7c06 6a07 8301 7d07 7c00 6a08  }.t.|.j...}.|.j.
-000010b0: 6a09 6a0a 7c07 8301 6a0b 740c 7c07 7c06  j.j.|...j.t.|.|.
-000010c0: 6a0d 8302 6a0e 6401 8301 740c 7c07 7c06  j...j.d...t.|.|.
-000010d0: 6a0f 8302 6a0e 6402 8301 8302 6a10 740c  j...j.d.....j.t.
-000010e0: 7c07 7c06 6a0d 8302 6a11 7c04 8301 8301  |.|.j...j.|.....
-000010f0: 7d08 7406 8800 6a03 6a04 6a12 8301 8901  }.t...j.j.j.....
-00001100: 8800 6a13 6a14 7c08 8301 6a15 7c08 6a16  ..j.j.|...j.|.j.
-00001110: 8801 6a02 6b02 8301 6a0b 7c08 6a17 6a0e  ..j.k...j.|.j.j.
-00001120: 6401 8301 6601 8701 6601 6403 6404 8408  d...f...f.d.d...
-00001130: 8800 6a18 4400 8301 9e02 8e00 7d09 7c00  ..j.D.......}.|.
-00001140: 6a08 6a19 741a 7c09 8301 8301 4900 6400  j.j.t.|.....I.d.
-00001150: 4800 7d0a 6405 6406 8400 7c0a 4400 8301  H.}.d.d...|.D...
-00001160: 7d0b 8700 6601 6407 6404 8408 7c0a 4400  }...f.d.d...|.D.
-00001170: 8301 7d0c 7c00 6a1b 8800 6a03 7c00 6a08  ..}.|.j...j.|.j.
-00001180: 8800 6a1c 6408 8d03 6a1d 7c0c 8301 4900  ..j.d...j.|...I.
-00001190: 6400 4800 0100 6409 640a 8400 7c0c 4400  d.H...d.d...|.D.
-000011a0: 8301 7d0d 6900 7d0e 7836 7c0b 4400 5d2e  ..}.i.}.x6|.D.].
-000011b0: 5c02 7d0f 7d10 7c0f 7c0e 6b07 9001 7254  \.}.}.|.|.k...rT
-000011c0: 6700 7c0e 7c0f 3c00 7c0e 7c0f 1900 6a1e  g.|.|.<.|.|...j.
-000011d0: 7c0d 7c10 1900 8301 0100 9001 713a 5700  |.|.........q:W.
-000011e0: 782c 7c01 4400 5d24 7d05 740c 7c05 7c02  x,|.D.]$}.t.|.|.
-000011f0: 8302 7d11 7c11 6a1f 7c0e 6a20 7c05 6a02  ..}.|.j.|.j |.j.
-00001200: 6700 8302 8301 0100 9001 7172 5700 7c01  g.........qrW.|.
-00001210: 5300 290b 4eda 165f 6261 636b 7761 7264  S.).N.._backward
-00001220: 5f72 656c 6174 696f 6e5f 6b65 79da 155f  _relation_key.._
-00001230: 666f 7277 6172 645f 7265 6c61 7469 6f6e  forward_relation
-00001240: 5f6b 6579 6301 0000 0000 0000 0002 0000  _keyc...........
-00001250: 0005 0000 0013 0000 0073 1c00 0000 6700  .........s....g.
-00001260: 7c00 5d14 7d01 7400 8800 7c01 8302 6a01  |.].}.t...|...j.
-00001270: 7c01 8301 9102 7104 5300 720b 0000 0029  |.....q.S.r....)
-00001280: 0272 2e00 0000 da03 6173 5f29 0272 3000  .r......as_).r0.
-00001290: 0000 721a 0000 0029 01da 1372 656c 6174  ..r....)...relat
-000012a0: 6564 5f71 7565 7279 5f74 6162 6c65 720b  ed_query_tabler.
-000012b0: 0000 0072 0c00 0000 7231 0000 0089 0000  ...r....r1......
-000012c0: 0073 0200 0000 0600 7a37 4261 7365 4578  .s......z7BaseEx
-000012d0: 6563 7574 6f72 2e5f 7072 6566 6574 6368  ecutor._prefetch
-000012e0: 5f6d 326d 5f72 656c 6174 696f 6e2e 3c6c  _m2m_relation.<l
-000012f0: 6f63 616c 733e 2e3c 6c69 7374 636f 6d70  ocals>.<listcomp
-00001300: 3e63 0100 0000 0000 0000 0200 0000 0500  >c..............
-00001310: 0000 5300 0000 731c 0000 0068 007c 005d  ..S...s....h.|.]
-00001320: 147d 017c 0164 0019 007c 0164 0119 0066  .}.|.d...|.d...f
-00001330: 0292 0271 0453 0029 0272 5300 0000 723f  ...q.S.).rS...r?
-00001340: 0000 0072 0b00 0000 2902 7230 0000 00da  ...r....).r0....
-00001350: 0165 720b 0000 0072 0b00 0000 720c 0000  .er....r....r...
-00001360: 00fa 093c 7365 7463 6f6d 703e 8c00 0000  ...<setcomp>....
-00001370: 7302 0000 0006 007a 3642 6173 6545 7865  s......z6BaseExe
-00001380: 6375 746f 722e 5f70 7265 6665 7463 685f  cutor._prefetch_
-00001390: 6d32 6d5f 7265 6c61 7469 6f6e 2e3c 6c6f  m2m_relation.<lo
-000013a0: 6361 6c73 3e2e 3c73 6574 636f 6d70 3e63  cals>.<setcomp>c
-000013b0: 0100 0000 0000 0000 0200 0000 0500 0000  ................
-000013c0: 1300 0000 7318 0000 0067 007c 005d 107d  ....s....g.|.].}
-000013d0: 0188 006a 0066 007c 018e 0191 0271 0453  ...j.f.|.....q.S
-000013e0: 0072 0b00 0000 2901 7205 0000 0029 0272  .r....).r....).r
-000013f0: 3000 0000 7257 0000 0029 0172 4b00 0000  0...rW...).rK...
-00001400: 720b 0000 0072 0c00 0000 7231 0000 008d  r....r....r1....
-00001410: 0000 0073 0200 0000 0600 2903 7205 0000  ...s......).r...
-00001420: 0072 0600 0000 7208 0000 0063 0100 0000  .r....r....c....
-00001430: 0000 0000 0200 0000 0400 0000 5300 0000  ............S...
-00001440: 7314 0000 0069 007c 005d 0c7d 017c 017c  s....i.|.].}.|.|
-00001450: 016a 0093 0271 0453 0072 0b00 0000 2901  .j...q.S.r....).
-00001460: 723f 0000 0029 0272 3000 0000 7257 0000  r?...).r0...rW..
-00001470: 0072 0b00 0000 720b 0000 0072 0c00 0000  .r....r....r....
-00001480: fa0a 3c64 6963 7463 6f6d 703e 9300 0000  ..<dictcomp>....
-00001490: 7302 0000 0006 007a 3742 6173 6545 7865  s......z7BaseExe
-000014a0: 6375 746f 722e 5f70 7265 6665 7463 685f  cutor._prefetch_
-000014b0: 6d32 6d5f 7265 6c61 7469 6f6e 2e3c 6c6f  m2m_relation.<lo
-000014c0: 6361 6c73 3e2e 3c64 6963 7463 6f6d 703e  cals>.<dictcomp>
-000014d0: 2921 723d 0000 0072 4400 0000 723f 0000  )!r=...rD...r?..
-000014e0: 0072 0500 0000 721e 0000 0072 2100 0000  .r....r....r!...
-000014f0: 7202 0000 00da 0774 6872 6f75 6768 7207  r......throughr.
-00001500: 0000 0072 3900 0000 7241 0000 00da 0673  ...r9...rA.....s
-00001510: 656c 6563 7472 2e00 0000 da0c 6261 636b  electr......back
-00001520: 7761 7264 5f6b 6579 7255 0000 00da 0b66  ward_keyrU.....f
-00001530: 6f72 7761 7264 5f6b 6579 723e 0000 00da  orward_keyr>....
-00001540: 0469 7369 6e72 3800 0000 7215 0000 00da  .isinr8...r.....
-00001550: 046a 6f69 6eda 026f 6e72 5400 0000 7253  .join..onrT...rS
-00001560: 0000 0072 0300 0000 720f 0000 0072 1000  ...r....r....r..
-00001570: 0000 da09 5f5f 636c 6173 735f 5f5a 0d5f  ....__class__Z._
-00001580: 7072 6566 6574 6368 5f6d 6170 da0e 6665  prefetch_map..fe
-00001590: 7463 685f 666f 725f 6c69 7374 7212 0000  tch_for_listr...
-000015a0: 0072 4900 0000 724a 0000 0029 1272 0a00  .rI...rJ...).r..
-000015b0: 0000 7217 0000 0072 1a00 0000 724b 0000  ..r....r....rK..
-000015c0: 0072 4c00 0000 7219 0000 0072 2900 0000  .rL...r....r)...
-000015d0: da0d 7468 726f 7567 685f 7461 626c 65da  ..through_table.
-000015e0: 0873 7562 7175 6572 7972 1500 0000 7216  .subqueryr....r.
-000015f0: 0000 005a 0972 656c 6174 696f 6e73 724d  ...Z.relationsrM
-00001600: 0000 0072 4e00 0000 5a0c 7265 6c61 7469  ...rN...Z.relati
-00001610: 6f6e 5f6d 6170 7250 0000 005a 1172 656c  on_maprP...Z.rel
-00001620: 6174 6564 5f6f 626a 6563 745f 6964 7251  ated_object_idrQ
-00001630: 0000 0072 0b00 0000 2902 724b 0000 0072  ...r....).rK...r
-00001640: 5600 0000 720c 0000 00da 165f 7072 6566  V...r......_pref
-00001650: 6574 6368 5f6d 326d 5f72 656c 6174 696f  etch_m2m_relatio
-00001660: 6e76 0000 0073 4000 0000 0001 0601 0a01  nv...s@.........
-00001670: 1002 0e02 0a02 0e01 1001 1401 1402 0e01  ................
-00001680: 0c01 0e02 0c01 1802 1601 0e01 1201 0401  ................
-00001690: 0401 0401 0a01 0c01 0e01 0402 0e01 0a01  ................
-000016a0: 0801 1802 0a01 0a01 1a01 7a23 4261 7365  ..........z#Base
-000016b0: 4578 6563 7574 6f72 2e5f 7072 6566 6574  Executor._prefet
-000016c0: 6368 5f6d 326d 5f72 656c 6174 696f 6e63  ch_m2m_relationc
-000016d0: 0400 0000 0000 0000 0900 0000 0800 0000  ................
-000016e0: c300 0000 738a 0000 0074 0083 007d 0464  ....s....t...}.d
-000016f0: 016a 017c 0283 017d 0578 267c 0144 005d  .j.|...}.x&|.D.]
-00001700: 1e7d 0674 027c 067c 0583 0272 167c 046a  .}.t.|.|...r.|.j
-00001710: 0374 027c 067c 0583 0283 0101 0071 1657  .t.|.|.......q.W
-00001720: 007c 0472 867c 036a 0474 057c 0483 0164  .|.r.|.j.t.|...d
-00001730: 028d 0149 0064 0048 007d 0764 0364 0484  ...I.d.H.}.d.d..
-00001740: 007c 0744 0083 017d 0878 247c 0144 005d  .|.D...}.x$|.D.]
-00001750: 1c7d 0674 067c 067c 027c 086a 0774 027c  .}.t.|.|.|.j.t.|
-00001760: 067c 0583 0283 0183 0301 0071 6657 007c  .|.........qfW.|
-00001770: 0153 0029 054e 7a05 7b7d 5f69 6429 015a  .S.).Nz.{}_id).Z
-00001780: 0669 645f 5f69 6e63 0100 0000 0000 0000  .id__inc........
-00001790: 0200 0000 0400 0000 5300 0000 7314 0000  ........S...s...
-000017a0: 0069 007c 005d 0c7d 017c 017c 016a 0093  .i.|.].}.|.|.j..
-000017b0: 0271 0453 0072 0b00 0000 2901 723f 0000  .q.S.r....).r?..
-000017c0: 0029 0272 3000 0000 da03 6f62 6a72 0b00  .).r0.....objr..
-000017d0: 0000 720b 0000 0072 0c00 0000 7259 0000  ..r....r....rY..
-000017e0: 00a8 0000 0073 0200 0000 0600 7a3a 4261  .....s......z:Ba
-000017f0: 7365 4578 6563 7574 6f72 2e5f 7072 6566  seExecutor._pref
-00001800: 6574 6368 5f64 6972 6563 745f 7265 6c61  etch_direct_rela
-00001810: 7469 6f6e 2e3c 6c6f 6361 6c73 3e2e 3c64  tion.<locals>.<d
-00001820: 6963 7463 6f6d 703e 2908 723d 0000 0072  ictcomp>).r=...r
-00001830: 4700 0000 722e 0000 0072 4400 0000 7246  G...r....rD...rF
-00001840: 0000 0072 4800 0000 7211 0000 0072 4a00  ...rH...r....rJ.
-00001850: 0000 2909 720a 0000 0072 1700 0000 721a  ..).r....r....r.
-00001860: 0000 0072 4b00 0000 5a19 7265 6c61 7465  ...rK...Z.relate
-00001870: 645f 6f62 6a65 6374 735f 666f 725f 6665  d_objects_for_fe
-00001880: 7463 685a 1272 656c 6174 696f 6e5f 6b65  tchZ.relation_ke
-00001890: 795f 6669 656c 6472 1900 0000 724d 0000  y_fieldr....rM..
-000018a0: 0072 4e00 0000 720b 0000 0072 0b00 0000  .rN...r....r....
-000018b0: 720c 0000 00da 195f 7072 6566 6574 6368  r......_prefetch
-000018c0: 5f64 6972 6563 745f 7265 6c61 7469 6f6e  _direct_relation
-000018d0: a000 0000 7318 0000 0000 0106 010a 010a  ....s...........
-000018e0: 010a 0114 0104 0116 010e 010a 0102 011a  ................
-000018f0: 027a 2642 6173 6545 7865 6375 746f 722e  .z&BaseExecutor.
-00001900: 5f70 7265 6665 7463 685f 6469 7265 6374  _prefetch_direct
-00001910: 5f72 656c 6174 696f 6e63 0100 0000 0000  _relationc......
-00001920: 0000 0600 0000 0400 0000 4300 0000 7372  ..........C...sr
-00001930: 0000 0078 6c7c 006a 006a 0183 0044 005d  ...xl|.j.j...D.]
-00001940: 5e5c 027d 017d 027c 017c 006a 026b 0672  ^\.}.}.|.|.j.k.r
-00001950: 2c7c 006a 026a 037c 0183 017d 036e 267c  ,|.j.j.|...}.n&|
-00001960: 006a 046a 056a 066a 037c 0183 017d 047c  .j.j.j.j.|...}.|
-00001970: 046a 077d 057c 056a 0883 006a 097c 006a  .j.}.|.j...j.|.j
-00001980: 0a83 017d 037c 0272 607c 036a 0b7c 028e  ...}.|.r`|.j.|..
-00001990: 007d 037c 037c 006a 027c 013c 0071 0c57  .}.|.|.j.|.<.q.W
-000019a0: 0064 0053 0029 014e 290c 7208 0000 0072  .d.S.).N).r....r
-000019b0: 3b00 0000 7209 0000 0072 4a00 0000 7205  ;...r....rJ...r.
-000019c0: 0000 0072 1e00 0000 7221 0000 00da 0474  ...r....r!.....t
-000019d0: 7970 65da 0361 6c6c da08 7573 696e 675f  ype..all..using_
-000019e0: 6462 7207 0000 005a 1070 7265 6665 7463  dbr....Z.prefetc
-000019f0: 685f 7265 6c61 7465 6429 0672 0a00 0000  h_related).r....
-00001a00: 721a 0000 005a 1466 6f72 7761 7264 6564  r....Z.forwarded
-00001a10: 5f70 7265 6665 7463 6865 7372 4b00 0000  _prefetchesrK...
-00001a20: 5a13 7265 6c61 7465 645f 6d6f 6465 6c5f  Z.related_model_
-00001a30: 6669 656c 64da 0d72 656c 6174 6564 5f6d  field..related_m
-00001a40: 6f64 656c 720b 0000 0072 0b00 0000 720c  odelr....r....r.
-00001a50: 0000 00da 165f 6d61 6b65 5f70 7265 6665  ....._make_prefe
-00001a60: 7463 685f 7175 6572 6965 73af 0000 0073  tch_queries....s
-00001a70: 1200 0000 0001 1401 0a01 0e02 1001 0601  ................
-00001a80: 1001 0401 0a01 7a23 4261 7365 4578 6563  ......z#BaseExec
-00001a90: 7574 6f72 2e5f 6d61 6b65 5f70 7265 6665  utor._make_prefe
-00001aa0: 7463 685f 7175 6572 6965 7363 0400 0000  tch_queriesc....
-00001ab0: 0000 0000 0400 0000 0400 0000 c300 0000  ................
-00001ac0: 7368 0000 0074 0074 017c 006a 027c 0283  sh...t.t.|.j.|..
-00001ad0: 0274 036a 0483 0272 287c 006a 057c 017c  .t.j...r(|.j.|.|
-00001ae0: 027c 0383 0349 0064 0048 0053 0074 0074  .|...I.d.H.S.t.t
-00001af0: 017c 006a 027c 0283 0274 036a 0683 0272  .|.j.|...t.j...r
-00001b00: 507c 006a 077c 017c 027c 0383 0349 0064  P|.j.|.|.|...I.d
-00001b10: 0048 0053 007c 006a 087c 017c 027c 0383  .H.S.|.j.|.|.|..
-00001b20: 0349 0064 0048 0053 0064 0053 0029 014e  .I.d.H.S.d.S.).N
-00001b30: 2909 7222 0000 0072 2e00 0000 7205 0000  ).r"...r....r...
-00001b40: 0072 0300 0000 da12 4261 636b 7761 7264  .r......Backward
-00001b50: 464b 5265 6c61 7469 6f6e 7252 0000 00da  FKRelationrR....
-00001b60: 0f4d 616e 7954 6f4d 616e 7946 6965 6c64  .ManyToManyField
-00001b70: 7265 0000 0072 6700 0000 2904 720a 0000  re...rg...).r...
-00001b80: 005a 1069 6e73 7461 6e63 655f 6964 5f6c  .Z.instance_id_l
-00001b90: 6973 7472 1a00 0000 724b 0000 0072 0b00  istr....rK...r..
-00001ba0: 0000 720b 0000 0072 0c00 0000 da0c 5f64  ..r....r......_d
-00001bb0: 6f5f 7072 6566 6574 6368 bb00 0000 730a  o_prefetch....s.
-00001bc0: 0000 0000 0114 0114 0114 0114 027a 1942  .............z.B
-00001bd0: 6173 6545 7865 6375 746f 722e 5f64 6f5f  aseExecutor._do_
-00001be0: 7072 6566 6574 6368 6302 0000 0000 0000  prefetchc.......
-00001bf0: 0004 0000 0005 0000 00c3 0000 0073 4800  .............sH.
-00001c00: 0000 7c01 7244 7c00 6a00 7310 7c00 6a01  ..|.rD|.j.s.|.j.
-00001c10: 7244 7c00 6a02 8300 0100 782a 7c00 6a01  rD|.j.....x*|.j.
-00001c20: 6a03 8300 4400 5d1c 5c02 7d02 7d03 7c00  j...D.].\.}.}.|.
-00001c30: 6a04 7c01 7c02 7c03 8303 4900 6400 4800  j.|.|.|...I.d.H.
-00001c40: 0100 7124 5700 7c01 5300 2901 4e29 0572  ..q$W.|.S.).N).r
-00001c50: 0800 0000 7209 0000 0072 6c00 0000 723b  ....r....rl...r;
-00001c60: 0000 0072 6f00 0000 2904 720a 0000 0072  ...ro...).r....r
-00001c70: 1700 0000 721a 0000 0072 4b00 0000 720b  ....r....rK...r.
-00001c80: 0000 0072 0b00 0000 720c 0000 0072 1300  ...r....r....r..
-00001c90: 0000 c300 0000 730a 0000 0000 0110 0108  ......s.........
-00001ca0: 0114 0118 017a 2642 6173 6545 7865 6375  .....z&BaseExecu
-00001cb0: 746f 722e 5f65 7865 6375 7465 5f70 7265  tor._execute_pre
-00001cc0: 6665 7463 685f 7175 6572 6965 7363 0200  fetch_queriesc..
-00001cd0: 0000 0000 0000 0700 0000 0500 0000 c700  ................
-00001ce0: 0000 73ca 0000 007c 006a 006a 0183 0049  ..s....|.j.j...I
-00001cf0: 0064 0048 007c 005f 0269 007c 005f 0378  .d.H.|._.i.|._.x
-00001d00: 827c 0244 005d 7a7d 037c 036a 0464 0183  .|.D.]z}.|.j.d..
-00001d10: 017d 047c 0464 0219 007d 057c 057c 006a  .}.|.d...}.|.|.j
-00001d20: 056a 066a 076b 0673 5874 0864 036a 097c  .j.j.k.sXt.d.j.|
-00001d30: 057c 006a 056a 066a 0a83 0283 0182 017c  .|.j.j.j.......|
-00001d40: 057c 006a 036a 0b83 006b 0772 7274 0c83  .|.j.j...k.rrt..
-00001d50: 007c 006a 037c 053c 0064 016a 0d7c 0464  .|.j.|.<.d.j.|.d
-00001d60: 0464 0085 0219 0083 017d 067c 0672 1e7c  .d.......}.|.r.|
-00001d70: 006a 037c 0519 006a 0e7c 0683 0101 0071  .j.|...j.|.....q
-00001d80: 1e57 007c 006a 0f7c 0183 0149 0064 0048  .W.|.j.|...I.d.H
-00001d90: 0001 007c 006a 006a 107c 006a 0283 0149  ...|.j.j.|.j...I
-00001da0: 0064 0048 0001 0064 007c 005f 027c 0153  .d.H...d.|._.|.S
-00001db0: 0029 054e da02 5f5f 7201 0000 007a 1c72  .).N..__r....z.r
-00001dc0: 656c 6174 696f 6e20 7b7d 2066 6f72 207b  elation {} for {
-00001dd0: 7d20 6e6f 7420 666f 756e 64e9 0100 0000  } not found.....
-00001de0: 2911 7206 0000 0072 0e00 0000 7207 0000  ).r....r....r...
-00001df0: 0072 0800 0000 da05 7370 6c69 7472 0500  .r......splitr..
-00001e00: 0000 721e 0000 00da 0c66 6574 6368 5f66  ..r......fetch_f
-00001e10: 6965 6c64 73da 0e41 7373 6572 7469 6f6e  ields..Assertion
-00001e20: 4572 726f 7272 4700 0000 7238 0000 0072  ErrorrG...r8...r
-00001e30: 2000 0000 723d 0000 0072 5f00 0000 7244   ...r=...r_...rD
-00001e40: 0000 0072 1300 0000 7214 0000 0029 0772  ...r....r....).r
-00001e50: 0a00 0000 7217 0000 00da 0461 7267 73da  ....r......args.
-00001e60: 0872 656c 6174 696f 6e5a 0e72 656c 6174  .relationZ.relat
-00001e70: 696f 6e5f 7370 6c69 745a 1166 6972 7374  ion_splitZ.first
-00001e80: 5f6c 6576 656c 5f66 6965 6c64 5a12 666f  _level_fieldZ.fo
-00001e90: 7277 6172 6465 645f 7072 6566 6574 6368  rwarded_prefetch
-00001ea0: 720b 0000 0072 0b00 0000 720c 0000 0072  r....r....r....r
-00001eb0: 6200 0000 ca00 0000 7320 0000 0000 0112  b.......s ......
-00001ec0: 0106 010a 010a 0108 0210 0114 010e 010c  ................
-00001ed0: 0112 0104 0114 0110 0114 0106 017a 1b42  .............z.B
-00001ee0: 6173 6545 7865 6375 746f 722e 6665 7463  aseExecutor.fetc
-00001ef0: 685f 666f 725f 6c69 7374 2903 4e4e 4e29  h_for_list).NNN)
-00001f00: 014e 2913 da08 5f5f 6e61 6d65 5f5f da0a  .N)...__name__..
-00001f10: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
-00001f20: 616c 6e61 6d65 5f5f 720d 0000 0072 1b00  alname__r....r..
-00001f30: 0000 722a 0000 0072 2d00 0000 722f 0000  ..r*...r-...r/..
-00001f40: 0072 3500 0000 7237 0000 0072 4000 0000  .r5...r7...r@...
-00001f50: 7243 0000 0072 5200 0000 7265 0000 0072  rC...rR...re...r
-00001f60: 6700 0000 726c 0000 0072 6f00 0000 7213  g...rl...ro...r.
-00001f70: 0000 0072 6200 0000 720b 0000 0072 0b00  ...rb...r....r..
-00001f80: 0000 720b 0000 0072 0c00 0000 7204 0000  ..r....r....r...
-00001f90: 0008 0000 0073 2000 0000 0801 0a07 0a0f  .....s .........
-00001fa0: 080e 0803 0803 0809 0806 0817 0806 0817  ................
-00001fb0: 082a 080f 080c 0808 0807 7204 0000 0029  .*........r....)
-00001fc0: 0672 1c00 0000 da06 7079 7069 6b61 7202  .r......pypikar.
-00001fd0: 0000 00da 0874 6f72 746f 6973 6572 0300  .....tortoiser..
-00001fe0: 0000 7204 0000 0072 0b00 0000 720b 0000  ..r....r....r...
-00001ff0: 0072 0b00 0000 720c 0000 00da 083c 6d6f  .r....r......<mo
-00002000: 6475 6c65 3e01 0000 0073 0600 0000 0802  dule>....s......
-00002010: 0c02 0c03                                ....
+00000040: 6d04 5a04 0100 6400 6404 6c05 6d06 5a06  m.Z...d.d.l.m.Z.
+00000050: 0100 4700 6405 6406 8400 6406 8302 5a07  ..G.d.d...d...Z.
+00000060: 6401 5300 2907 e900 0000 004e 2901 da05  d.S.)......N)...
+00000070: 5461 626c 6529 01da 0666 6965 6c64 7329  Table)...fields)
+00000080: 01da 104f 7065 7261 7469 6f6e 616c 4572  ...OperationalEr
+00000090: 726f 7263 0000 0000 0000 0000 0000 0000  rorc............
+000000a0: 0300 0000 4000 0000 7390 0000 0065 005a  ....@...s....e.Z
+000000b0: 0164 005a 0264 2264 0264 0384 015a 0364  .d.Z.d"d.d...Z.d
+000000c0: 2364 0464 0584 015a 0464 0664 0784 005a  #d.d...Z.d.d...Z
+000000d0: 0564 0864 0984 005a 0664 0a64 0b84 005a  .d.d...Z.d.d...Z
+000000e0: 0764 0c64 0d84 005a 0864 0e64 0f84 005a  .d.d...Z.d.d...Z
+000000f0: 0964 1064 1184 005a 0a64 1264 1384 005a  .d.d...Z.d.d...Z
+00000100: 0b64 1464 1584 005a 0c64 1664 1784 005a  .d.d...Z.d.d...Z
+00000110: 0d64 1864 1984 005a 0e64 1a64 1b84 005a  .d.d...Z.d.d...Z
+00000120: 0f64 1c64 1d84 005a 1064 1e64 1f84 005a  .d.d...Z.d.d...Z
+00000130: 1164 2064 2184 005a 1264 0153 0029 24da  .d d!..Z.d.S.)$.
+00000140: 0c42 6173 6545 7865 6375 746f 724e 6305  .BaseExecutorNc.
+00000150: 0000 0000 0000 0005 0000 0002 0000 0043  ...............C
+00000160: 0000 0073 3200 0000 7c01 7c00 5f00 7c02  ...s2...|.|._.|.
+00000170: 7c00 5f01 6400 7c00 5f02 7c03 721a 7c03  |._.d.|._.|.r.|.
+00000180: 6e02 6900 7c00 5f03 7c04 7228 7c04 6e02  n.i.|._.|.r(|.n.
+00000190: 6900 7c00 5f04 6400 5300 2901 4e29 05da  i.|._.d.S.).N)..
+000001a0: 056d 6f64 656c da02 6462 da0a 636f 6e6e  .model..db..conn
+000001b0: 6563 7469 6f6e da0c 7072 6566 6574 6368  ection..prefetch
+000001c0: 5f6d 6170 da11 5f70 7265 6665 7463 685f  _map.._prefetch_
+000001d0: 7175 6572 6965 7329 05da 0473 656c 6672  queries)...selfr
+000001e0: 0600 0000 7207 0000 0072 0900 0000 5a10  ....r....r....Z.
+000001f0: 7072 6566 6574 6368 5f71 7565 7269 6573  prefetch_queries
+00000200: a900 720c 0000 00fa 532f 5573 6572 732f  ..r.....S/Users/
+00000210: 616e 6472 6579 626f 6e64 6172 2f50 7943  andreybondar/PyC
+00000220: 6861 726d 5072 6f6a 6563 7473 2f74 6f72  harmProjects/tor
+00000230: 746f 6973 652d 6f72 6d2f 746f 7274 6f69  toise-orm/tortoi
+00000240: 7365 2f62 6163 6b65 6e64 732f 6261 7365  se/backends/base
+00000250: 2f65 7865 6375 746f 722e 7079 da08 5f5f  /executor.py..__
+00000260: 696e 6974 5f5f 0a00 0000 730a 0000 0000  init__....s.....
+00000270: 0106 0106 0106 010e 017a 1542 6173 6545  .........z.BaseE
+00000280: 7865 6375 746f 722e 5f5f 696e 6974 5f5f  xecutor.__init__
+00000290: 6303 0000 0000 0000 0008 0000 0007 0000  c...............
+000002a0: 00c3 0000 0073 a000 0000 7c00 6a00 6a01  .....s....|.j.j.
+000002b0: 8300 4900 6400 4800 7c00 5f02 7c00 6a02  ..I.d.H.|._.|.j.
+000002c0: 6a03 7404 7c01 8301 8301 4900 6400 4800  j.t.|.....I.d.H.
+000002d0: 7d03 6700 7d04 7844 7c03 4400 5d3c 7d05  }.g.}.xD|.D.]<}.
+000002e0: 7c00 6a05 6600 7c05 8e01 7d06 7c02 7264  |.j.f.|...}.|.rd
+000002f0: 781c 7c02 4400 5d14 7d07 7406 7c06 7c07  x.|.D.].}.t.|.|.
+00000300: 7c05 7c07 1900 8303 0100 714c 5700 7c04  |.|.......qLW.|.
+00000310: 6a07 7c06 8301 0100 7132 5700 7c00 6a08  j.|.....q2W.|.j.
+00000320: 7c04 8301 4900 6400 4800 0100 7c00 6a00  |...I.d.H...|.j.
+00000330: 6a09 7c00 6a02 8301 4900 6400 4800 0100  j.|.j...I.d.H...
+00000340: 6400 7c00 5f02 7c04 5300 2901 4e29 0a72  d.|._.|.S.).N).r
+00000350: 0700 0000 da15 6765 745f 7369 6e67 6c65  ......get_single
+00000360: 5f63 6f6e 6e65 6374 696f 6e72 0800 0000  _connectionr....
+00000370: da0d 6578 6563 7574 655f 7175 6572 79da  ..execute_query.
+00000380: 0373 7472 7206 0000 00da 0773 6574 6174  .strr......setat
+00000390: 7472 da06 6170 7065 6e64 da19 5f65 7865  tr..append.._exe
+000003a0: 6375 7465 5f70 7265 6665 7463 685f 7175  cute_prefetch_qu
+000003b0: 6572 6965 73da 1972 656c 6561 7365 5f73  eries..release_s
+000003c0: 696e 676c 655f 636f 6e6e 6563 7469 6f6e  ingle_connection
+000003d0: 2908 720b 0000 00da 0571 7565 7279 5a0d  ).r......queryZ.
+000003e0: 6375 7374 6f6d 5f66 6965 6c64 73da 0b72  custom_fields..r
+000003f0: 6177 5f72 6573 756c 7473 da0d 696e 7374  aw_results..inst
+00000400: 616e 6365 5f6c 6973 74da 0372 6f77 da08  ance_list..row..
+00000410: 696e 7374 616e 6365 da05 6669 656c 6472  instance..fieldr
+00000420: 0c00 0000 720c 0000 0072 0d00 0000 da0e  ....r....r......
+00000430: 6578 6563 7574 655f 7365 6c65 6374 1100  execute_select..
+00000440: 0000 731a 0000 0000 0112 0116 0104 010a  ..s.............
+00000450: 010c 0104 010a 0114 010e 0110 0114 0106  ................
+00000460: 017a 1b42 6173 6545 7865 6375 746f 722e  .z.BaseExecutor.
+00000470: 6578 6563 7574 655f 7365 6c65 6374 6301  execute_selectc.
+00000480: 0000 0000 0000 0006 0000 0004 0000 0043  ...............C
+00000490: 0000 0073 7600 0000 6700 7d01 6700 7d02  ...sv...g.}.g.}.
+000004a0: 7400 6a00 6a01 8300 7d03 785a 7c00 6a02  t.j.j...}.xZ|.j.
+000004b0: 6a03 6a04 6a05 8300 4400 5d48 7d04 7c00  j.j.j...D.]H}.|.
+000004c0: 6a02 6a03 6a06 7c04 1900 7d05 7407 7c05  j.j.j.|...}.t.|.
+000004d0: 7408 6a09 8302 7256 7c05 6a0a 7256 7c02  t.j...rV|.j.rV|.
+000004e0: 6a0b 7c04 7c03 6602 8301 0100 7122 7c05  j.|.|.f.....q"|.
+000004f0: 6a0c 7260 7122 7122 7c01 6a0b 7c04 8301  j.r`q"q"|.j.|...
+00000500: 0100 7122 5700 7c01 7c02 6602 5300 2901  ..q"W.|.|.f.S.).
+00000510: 4e29 0dda 0864 6174 6574 696d 65da 0675  N)...datetime..u
+00000520: 7463 6e6f 7772 0600 0000 da05 5f6d 6574  tcnowr......_met
+00000530: 61da 1466 6965 6c64 735f 6462 5f70 726f  a..fields_db_pro
+00000540: 6a65 6374 696f 6eda 046b 6579 73da 0a66  jection..keys..f
+00000550: 6965 6c64 735f 6d61 70da 0a69 7369 6e73  ields_map..isins
+00000560: 7461 6e63 6572 0300 0000 da0d 4461 7465  tancer......Date
+00000570: 7469 6d65 4669 656c 64da 0c61 7574 6f5f  timeField..auto_
+00000580: 6e6f 775f 6164 6472 1300 0000 da09 6765  now_addr......ge
+00000590: 6e65 7261 7465 6429 0672 0b00 0000 da0f  nerated).r......
+000005a0: 7265 6775 6c61 725f 636f 6c75 6d6e 735a  regular_columnsZ
+000005b0: 1d70 7974 686f 6e5f 6765 6e65 7261 7465  .python_generate
+000005c0: 645f 636f 6c75 6d6e 5f70 6169 7273 da03  d_column_pairs..
+000005d0: 6e6f 77da 0663 6f6c 756d 6eda 0c66 6965  now..column..fie
+000005e0: 6c64 5f6f 626a 6563 7472 0c00 0000 720c  ld_objectr....r.
+000005f0: 0000 0072 0d00 0000 da17 5f70 7265 7061  ...r......_prepa
+00000600: 7265 5f69 6e73 6572 745f 636f 6c75 6d6e  re_insert_column
+00000610: 7320 0000 0073 1600 0000 0001 0401 0401  s ...s..........
+00000620: 0a01 1401 0e01 1201 1001 0601 0402 0e01  ................
+00000630: 7a24 4261 7365 4578 6563 7574 6f72 2e5f  z$BaseExecutor._
+00000640: 7072 6570 6172 655f 696e 7365 7274 5f63  prepare_insert_c
+00000650: 6f6c 756d 6e73 6303 0000 0000 0000 0003  olumnsc.........
+00000660: 0000 0002 0000 0043 0000 0073 0a00 0000  .......C...s....
+00000670: 7c01 6a00 7c02 8301 5300 2901 4e29 01da  |.j.|...S.).N)..
+00000680: 0b74 6f5f 6462 5f76 616c 7565 2903 720b  .to_db_value).r.
+00000690: 0000 0072 2a00 0000 da04 6174 7472 720c  ...r*.....attrr.
+000006a0: 0000 0072 0c00 0000 720d 0000 00da 0c5f  ...r....r......_
+000006b0: 6669 656c 645f 746f 5f64 622e 0000 0073  field_to_db....s
+000006c0: 0200 0000 0001 7a19 4261 7365 4578 6563  ......z.BaseExec
+000006d0: 7574 6f72 2e5f 6669 656c 645f 746f 5f64  utor._field_to_d
+000006e0: 6263 0300 0000 0000 0000 0300 0000 0500  bc..............
+000006f0: 0000 4300 0000 731c 0000 007c 006a 007c  ..C...s....|.j.|
+00000700: 006a 016a 026a 037c 0219 0074 047c 017c  .j.j.j.|...t.|.|
+00000710: 0283 0283 0253 0029 014e 2905 722e 0000  .....S.).N).r...
+00000720: 0072 0600 0000 721f 0000 0072 2200 0000  .r....r....r"...
+00000730: da07 6765 7461 7474 7229 0372 0b00 0000  ..getattr).r....
+00000740: 721a 0000 0072 2900 0000 720c 0000 0072  r....r)...r....r
+00000750: 0c00 0000 720d 0000 00da 135f 6765 745f  ....r......_get_
+00000760: 7072 6570 6172 6564 5f76 616c 7565 3100  prepared_value1.
+00000770: 0000 7302 0000 0000 017a 2042 6173 6545  ..s......z BaseE
+00000780: 7865 6375 746f 722e 5f67 6574 5f70 7265  xecutor._get_pre
+00000790: 7061 7265 645f 7661 6c75 6563 0400 0000  pared_valuec....
+000007a0: 0000 0000 0800 0000 0500 0000 0300 0000  ................
+000007b0: 736a 0000 0087 0087 0166 0264 0164 0284  sj.......f.d.d..
+000007c0: 087c 0244 0083 017d 0487 0166 0164 0364  .|.D...}...f.d.d
+000007d0: 0284 087c 0244 0083 017d 0578 3a7c 0344  ...|.D...}.x:|.D
+000007e0: 005d 325c 027d 067d 077c 056a 0088 016a  .]2\.}.}.|.j...j
+000007f0: 016a 026a 037c 0619 0083 0101 007c 046a  .j.j.|.......|.j
+00000800: 007c 0783 0101 0074 0488 007c 067c 0783  .|.....t...|.|..
+00000810: 0301 0071 2c57 007c 057c 0466 0253 0029  ...q,W.|.|.f.S.)
+00000820: 044e 6301 0000 0000 0000 0002 0000 0005  .Nc.............
+00000830: 0000 0013 0000 0073 1800 0000 6700 7c00  .......s....g.|.
+00000840: 5d10 7d01 8801 6a00 8800 7c01 8302 9102  ].}...j...|.....
+00000850: 7104 5300 720c 0000 0029 0172 3000 0000  q.S.r....).r0...
+00000860: 2902 da02 2e30 7229 0000 0029 0272 1a00  )....0r)...).r..
+00000870: 0000 720b 0000 0072 0c00 0000 720d 0000  ..r....r....r...
+00000880: 00fa 0a3c 6c69 7374 636f 6d70 3e35 0000  ...<listcomp>5..
+00000890: 0073 0200 0000 0600 7a37 4261 7365 4578  .s......z7BaseEx
+000008a0: 6563 7574 6f72 2e5f 7072 6570 6172 655f  ecutor._prepare_
+000008b0: 696e 7365 7274 5f76 616c 7565 732e 3c6c  insert_values.<l
+000008c0: 6f63 616c 733e 2e3c 6c69 7374 636f 6d70  ocals>.<listcomp
+000008d0: 3e63 0100 0000 0000 0000 0200 0000 0400  >c..............
+000008e0: 0000 1300 0000 731a 0000 0067 007c 005d  ......s....g.|.]
+000008f0: 127d 0188 006a 006a 016a 027c 0119 0091  .}...j.j.j.|....
+00000900: 0271 0453 0072 0c00 0000 2903 7206 0000  .q.S.r....).r...
+00000910: 0072 1f00 0000 7220 0000 0029 0272 3100  .r....r ...).r1.
+00000920: 0000 da01 6329 0172 0b00 0000 720c 0000  ....c).r....r...
+00000930: 0072 0d00 0000 7232 0000 0036 0000 0073  .r....r2...6...s
+00000940: 0200 0000 0600 2905 7213 0000 0072 0600  ......).r....r..
+00000950: 0000 721f 0000 0072 2000 0000 7212 0000  ..r....r ...r...
+00000960: 0029 0872 0b00 0000 721a 0000 0072 2700  .).r....r....r'.
+00000970: 0000 5a16 6765 6e65 7261 7465 645f 636f  ..Z.generated_co
+00000980: 6c75 6d6e 5f70 6169 7273 da06 7661 6c75  lumn_pairs..valu
+00000990: 6573 5a0e 7265 7375 6c74 5f63 6f6c 756d  esZ.result_colum
+000009a0: 6e73 7229 0000 00da 0576 616c 7565 720c  nsr).....valuer.
+000009b0: 0000 0029 0272 1a00 0000 720b 0000 0072  ...).r....r....r
+000009c0: 0d00 0000 da16 5f70 7265 7061 7265 5f69  ......_prepare_i
+000009d0: 6e73 6572 745f 7661 6c75 6573 3400 0000  nsert_values4...
+000009e0: 730e 0000 0000 0114 0112 010e 0114 010a  s...............
+000009f0: 0110 017a 2342 6173 6545 7865 6375 746f  ...z#BaseExecuto
+00000a00: 722e 5f70 7265 7061 7265 5f69 6e73 6572  r._prepare_inser
+00000a10: 745f 7661 6c75 6573 6302 0000 0000 0000  t_valuesc.......
+00000a20: 0002 0000 0001 0000 00c3 0000 0073 0a00  .............s..
+00000a30: 0000 7400 8300 8201 6400 5300 2901 4e29  ..t.....d.S.).N)
+00000a40: 01da 134e 6f74 496d 706c 656d 656e 7465  ...NotImplemente
+00000a50: 6445 7272 6f72 2902 720b 0000 0072 1a00  dError).r....r..
+00000a60: 0000 720c 0000 0072 0c00 0000 720d 0000  ..r....r....r...
+00000a70: 00da 0e65 7865 6375 7465 5f69 6e73 6572  ...execute_inser
+00000a80: 743d 0000 0073 0200 0000 0004 7a1b 4261  t=...s......z.Ba
+00000a90: 7365 4578 6563 7574 6f72 2e65 7865 6375  seExecutor.execu
+00000aa0: 7465 5f69 6e73 6572 7463 0200 0000 0000  te_insertc......
+00000ab0: 0000 0800 0000 0800 0000 c300 0000 73f8  ..............s.
+00000ac0: 0000 007c 006a 006a 0183 0049 0064 0048  ...|.j.j...I.d.H
+00000ad0: 007c 005f 0274 037c 006a 046a 056a 0683  .|._.t.|.j.j.j..
+00000ae0: 017d 027c 006a 026a 076a 087c 0283 017d  .}.|.j.j.j.|...}
+00000af0: 0378 827c 006a 046a 056a 096a 0a83 0044  .x.|.j.j.j.j...D
+00000b00: 005d 705c 027d 047d 057c 006a 046a 056a  .]p\.}.}.|.j.j.j
+00000b10: 0b7c 0419 007d 0674 0c7c 0674 0d6a 0e83  .|...}.t.|.t.j..
+00000b20: 0272 8a7c 066a 0f72 8a74 106a 106a 1183  .r.|.j.r.t.j.j..
+00000b30: 007d 077c 036a 127c 057c 0783 027d 0374  .}.|.j.|.|...}.t
+00000b40: 137c 017c 047c 0783 0301 0071 3e7c 066a  .|.|.|.....q>|.j
+00000b50: 1472 9471 3e71 3e7c 036a 127c 057c 006a  .r.q>q>|.j.|.|.j
+00000b60: 157c 0674 167c 017c 0483 0283 0283 027d  .|.t.|.|.......}
+00000b70: 0371 3e57 007c 036a 177c 026a 187c 016a  .q>W.|.j.|.j.|.j
+00000b80: 186b 0283 017d 037c 006a 026a 1974 1a7c  .k...}.|.j.j.t.|
+00000b90: 0383 0183 0149 0064 0048 0001 007c 006a  .....I.d.H...|.j
+00000ba0: 006a 1b7c 006a 0283 0149 0064 0048 0001  .j.|.j...I.d.H..
+00000bb0: 0064 007c 005f 027c 0153 0029 014e 291c  .d.|._.|.S.).N).
+00000bc0: 7207 0000 0072 0f00 0000 7208 0000 0072  r....r....r....r
+00000bd0: 0200 0000 7206 0000 0072 1f00 0000 da05  ....r....r......
+00000be0: 7461 626c 65da 0b71 7565 7279 5f63 6c61  table..query_cla
+00000bf0: 7373 da06 7570 6461 7465 7220 0000 00da  ss..updater ....
+00000c00: 0569 7465 6d73 7222 0000 0072 2300 0000  .itemsr"...r#...
+00000c10: 7203 0000 0072 2400 0000 da08 6175 746f  r....r$.....auto
+00000c20: 5f6e 6f77 721d 0000 0072 1e00 0000 da03  _nowr....r......
+00000c30: 7365 7472 1200 0000 7226 0000 0072 2e00  setr....r&...r..
+00000c40: 0000 722f 0000 00da 0577 6865 7265 da02  ..r/.....where..
+00000c50: 6964 7210 0000 0072 1100 0000 7215 0000  idr....r....r...
+00000c60: 0029 0872 0b00 0000 721a 0000 0072 3900  .).r....r....r9.
+00000c70: 0000 7216 0000 0072 1b00 0000 5a08 6462  ..r....r....Z.db
+00000c80: 5f66 6965 6c64 722a 0000 0072 2800 0000  _fieldr*...r(...
+00000c90: 720c 0000 0072 0c00 0000 720d 0000 00da  r....r....r.....
+00000ca0: 0e65 7865 6375 7465 5f75 7064 6174 6543  .execute_updateC
+00000cb0: 0000 0073 2600 0000 0001 1201 0e01 0e01  ...s&...........
+00000cc0: 1801 0e01 1201 0a01 0c01 0e01 0601 0402  ................
+00000cd0: 0401 0201 1802 1201 1601 1401 0601 7a1b  ..............z.
+00000ce0: 4261 7365 4578 6563 7574 6f72 2e65 7865  BaseExecutor.exe
+00000cf0: 6375 7465 5f75 7064 6174 6563 0200 0000  cute_updatec....
+00000d00: 0000 0000 0400 0000 0300 0000 c300 0000  ................
+00000d10: 7348 0000 0074 007c 006a 016a 026a 0383  sH...t.|.j.j.j..
+00000d20: 017d 027c 006a 046a 056a 067c 0283 016a  .}.|.j.j.j.|...j
+00000d30: 077c 026a 087c 016a 086b 0283 016a 0983  .|.j.|.j.k...j..
+00000d40: 007d 037c 006a 046a 0a74 0b7c 0383 0183  .}.|.j.j.t.|....
+00000d50: 0149 0064 0048 0001 007c 0153 0029 014e  .I.d.H...|.S.).N
+00000d60: 290c 7202 0000 0072 0600 0000 721f 0000  ).r....r....r...
+00000d70: 0072 3900 0000 7207 0000 0072 3a00 0000  .r9...r....r:...
+00000d80: da05 6672 6f6d 5f72 3f00 0000 7240 0000  ..from_r?...r@..
+00000d90: 00da 0664 656c 6574 6572 1000 0000 7211  ...deleter....r.
+00000da0: 0000 0029 0472 0b00 0000 721a 0000 0072  ...).r....r....r
+00000db0: 3900 0000 7216 0000 0072 0c00 0000 720c  9...r....r....r.
+00000dc0: 0000 0072 0d00 0000 da0e 6578 6563 7574  ...r......execut
+00000dd0: 655f 6465 6c65 7465 5a00 0000 7308 0000  e_deleteZ...s...
+00000de0: 0000 010e 0120 0116 017a 1b42 6173 6545  ..... ...z.BaseE
+00000df0: 7865 6375 746f 722e 6578 6563 7574 655f  xecutor.execute_
+00000e00: 6465 6c65 7465 6304 0000 0000 0000 000d  deletec.........
+00000e10: 0000 0005 0000 00c3 0000 0073 c400 0000  ...........s....
+00000e20: 7400 8300 7d04 7818 7c01 4400 5d10 7d05  t...}.x.|.D.].}.
+00000e30: 7c04 6a01 7c05 6a02 8301 0100 710c 5700  |.j.|.j.....q.W.
+00000e40: 7403 7c00 6a04 7c02 8302 7d06 7c06 6a05  t.|.j.|...}.|.j.
+00000e50: 7d07 7c03 6a06 6600 6401 6a07 7c07 8301  }.|.j.f.d.j.|...
+00000e60: 7408 7c04 8301 6901 8e01 4900 6400 4800  t.|...i...I.d.H.
+00000e70: 7d08 6900 7d09 783c 7c08 4400 5d34 7d0a  }.i.}.x<|.D.]4}.
+00000e80: 7403 7c0a 7c07 8302 7d0b 7c0b 7c09 6a09  t.|.|...}.|.|.j.
+00000e90: 8300 6b06 7286 7c09 7c0b 1900 6a0a 7c0a  ..k.r.|.|...j.|.
+00000ea0: 8301 0100 715c 7c0a 6701 7c09 7c0b 3c00  ....q\|.g.|.|.<.
+00000eb0: 715c 5700 782a 7c01 4400 5d22 7d05 7403  q\W.x*|.D.]"}.t.
+00000ec0: 7c05 7c02 8302 7d0c 7c0c 6a0b 7c09 6a0c  |.|...}.|.j.|.j.
+00000ed0: 7c05 6a02 6700 8302 8301 0100 719a 5700  |.j.g.......q.W.
+00000ee0: 7c01 5300 2902 4e7a 067b 7d5f 5f69 6e29  |.S.).Nz.{}__in)
+00000ef0: 0d72 3e00 0000 da03 6164 6472 4000 0000  .r>.....addr@...
+00000f00: 722f 0000 0072 0600 0000 da0e 7265 6c61  r/...r......rela
+00000f10: 7469 6f6e 5f66 6965 6c64 da06 6669 6c74  tion_field..filt
+00000f20: 6572 da06 666f 726d 6174 da04 6c69 7374  er..format..list
+00000f30: 7221 0000 0072 1300 0000 da15 5f73 6574  r!...r......_set
+00000f40: 5f72 6573 756c 745f 666f 725f 7175 6572  _result_for_quer
+00000f50: 79da 0367 6574 290d 720b 0000 0072 1800  y..get).r....r..
+00000f60: 0000 721b 0000 00da 0d72 656c 6174 6564  ..r......related
+00000f70: 5f71 7565 7279 da0f 696e 7374 616e 6365  _query..instance
+00000f80: 5f69 645f 7365 7472 1a00 0000 5a19 6261  _id_setr....Z.ba
+00000f90: 636b 7761 7264 5f72 656c 6174 696f 6e5f  ckward_relation_
+00000fa0: 6d61 6e61 6765 7272 4600 0000 da13 7265  managerrF.....re
+00000fb0: 6c61 7465 645f 6f62 6a65 6374 5f6c 6973  lated_object_lis
+00000fc0: 74da 1272 656c 6174 6564 5f6f 626a 6563  t..related_objec
+00000fd0: 745f 6d61 70da 0565 6e74 7279 da09 6f62  t_map..entry..ob
+00000fe0: 6a65 6374 5f69 64da 1272 656c 6174 696f  ject_id..relatio
+00000ff0: 6e5f 636f 6e74 6169 6e65 7272 0c00 0000  n_containerr....
+00001000: 720c 0000 0072 0d00 0000 da1a 5f70 7265  r....r......_pre
+00001010: 6665 7463 685f 7265 7665 7273 655f 7265  fetch_reverse_re
+00001020: 6c61 7469 6f6e 6000 0000 7322 0000 0000  lation`...s"....
+00001030: 0106 010a 0110 010c 0106 0206 011a 0304  ................
+00001040: 010a 010a 010c 0110 020e 010a 010a 0118  ................
+00001050: 017a 2742 6173 6545 7865 6375 746f 722e  .z'BaseExecutor.
+00001060: 5f70 7265 6665 7463 685f 7265 7665 7273  _prefetch_revers
+00001070: 655f 7265 6c61 7469 6f6e 6304 0000 0000  e_relationc.....
+00001080: 0000 0012 0000 0005 0000 0083 0000 0073  ...............s
+00001090: 9e01 0000 7400 8300 7d04 7818 7c01 4400  ....t...}.x.|.D.
+000010a0: 5d10 7d05 7c04 6a01 7c05 6a02 8301 0100  ].}.|.j.|.j.....
+000010b0: 710c 5700 7c00 6a03 6a04 6a05 7c02 1900  q.W.|.j.j.j.|...
+000010c0: 7d06 7406 7c06 6a07 8301 7d07 7c00 6a08  }.t.|.j...}.|.j.
+000010d0: 6a09 6a0a 7c07 8301 6a0b 740c 7c07 7c06  j.j.|...j.t.|.|.
+000010e0: 6a0d 8302 6a0e 6401 8301 740c 7c07 7c06  j...j.d...t.|.|.
+000010f0: 6a0f 8302 6a0e 6402 8301 8302 6a10 740c  j...j.d.....j.t.
+00001100: 7c07 7c06 6a0d 8302 6a11 7c04 8301 8301  |.|.j...j.|.....
+00001110: 7d08 7406 8800 6a03 6a04 6a12 8301 8901  }.t...j.j.j.....
+00001120: 8800 6a13 6a14 7c08 8301 6a15 7c08 6a16  ..j.j.|...j.|.j.
+00001130: 8801 6a02 6b02 8301 6a0b 7c08 6a17 6a0e  ..j.k...j.|.j.j.
+00001140: 6401 8301 6601 8701 6601 6403 6404 8408  d...f...f.d.d...
+00001150: 8800 6a18 4400 8301 9e02 8e00 7d09 7c00  ..j.D.......}.|.
+00001160: 6a08 6a19 741a 7c09 8301 8301 4900 6400  j.j.t.|.....I.d.
+00001170: 4800 7d0a 6405 6406 8400 7c0a 4400 8301  H.}.d.d...|.D...
+00001180: 7d0b 8700 6601 6407 6404 8408 7c0a 4400  }...f.d.d...|.D.
+00001190: 8301 7d0c 7c00 6a1b 8800 6a03 7c00 6a08  ..}.|.j...j.|.j.
+000011a0: 8800 6a1c 6408 8d03 6a1d 7c0c 8301 4900  ..j.d...j.|...I.
+000011b0: 6400 4800 0100 6409 640a 8400 7c0c 4400  d.H...d.d...|.D.
+000011c0: 8301 7d0d 6900 7d0e 7836 7c0b 4400 5d2e  ..}.i.}.x6|.D.].
+000011d0: 5c02 7d0f 7d10 7c0f 7c0e 6b07 9001 7254  \.}.}.|.|.k...rT
+000011e0: 6700 7c0e 7c0f 3c00 7c0e 7c0f 1900 6a1e  g.|.|.<.|.|...j.
+000011f0: 7c0d 7c10 1900 8301 0100 9001 713a 5700  |.|.........q:W.
+00001200: 782c 7c01 4400 5d24 7d05 740c 7c05 7c02  x,|.D.]$}.t.|.|.
+00001210: 8302 7d11 7c11 6a1f 7c0e 6a20 7c05 6a02  ..}.|.j.|.j |.j.
+00001220: 6700 8302 8301 0100 9001 7172 5700 7c01  g.........qrW.|.
+00001230: 5300 290b 4eda 165f 6261 636b 7761 7264  S.).N.._backward
+00001240: 5f72 656c 6174 696f 6e5f 6b65 79da 155f  _relation_key.._
+00001250: 666f 7277 6172 645f 7265 6c61 7469 6f6e  forward_relation
+00001260: 5f6b 6579 6301 0000 0000 0000 0002 0000  _keyc...........
+00001270: 0005 0000 0013 0000 0073 1c00 0000 6700  .........s....g.
+00001280: 7c00 5d14 7d01 7400 8800 7c01 8302 6a01  |.].}.t...|...j.
+00001290: 7c01 8301 9102 7104 5300 720c 0000 0029  |.....q.S.r....)
+000012a0: 0272 2f00 0000 da03 6173 5f29 0272 3100  .r/.....as_).r1.
+000012b0: 0000 721b 0000 0029 01da 1372 656c 6174  ..r....)...relat
+000012c0: 6564 5f71 7565 7279 5f74 6162 6c65 720c  ed_query_tabler.
+000012d0: 0000 0072 0d00 0000 7232 0000 008a 0000  ...r....r2......
+000012e0: 0073 0200 0000 0600 7a37 4261 7365 4578  .s......z7BaseEx
+000012f0: 6563 7574 6f72 2e5f 7072 6566 6574 6368  ecutor._prefetch
+00001300: 5f6d 326d 5f72 656c 6174 696f 6e2e 3c6c  _m2m_relation.<l
+00001310: 6f63 616c 733e 2e3c 6c69 7374 636f 6d70  ocals>.<listcomp
+00001320: 3e63 0100 0000 0000 0000 0200 0000 0500  >c..............
+00001330: 0000 5300 0000 731c 0000 0068 007c 005d  ..S...s....h.|.]
+00001340: 147d 017c 0164 0019 007c 0164 0119 0066  .}.|.d...|.d...f
+00001350: 0292 0271 0453 0029 0272 5400 0000 7240  ...q.S.).rT...r@
+00001360: 0000 0072 0c00 0000 2902 7231 0000 00da  ...r....).r1....
+00001370: 0165 720c 0000 0072 0c00 0000 720d 0000  .er....r....r...
+00001380: 00fa 093c 7365 7463 6f6d 703e 8d00 0000  ...<setcomp>....
+00001390: 7302 0000 0006 007a 3642 6173 6545 7865  s......z6BaseExe
+000013a0: 6375 746f 722e 5f70 7265 6665 7463 685f  cutor._prefetch_
+000013b0: 6d32 6d5f 7265 6c61 7469 6f6e 2e3c 6c6f  m2m_relation.<lo
+000013c0: 6361 6c73 3e2e 3c73 6574 636f 6d70 3e63  cals>.<setcomp>c
+000013d0: 0100 0000 0000 0000 0200 0000 0500 0000  ................
+000013e0: 1300 0000 7318 0000 0067 007c 005d 107d  ....s....g.|.].}
+000013f0: 0188 006a 0066 007c 018e 0191 0271 0453  ...j.f.|.....q.S
+00001400: 0072 0c00 0000 2901 7206 0000 0029 0272  .r....).r....).r
+00001410: 3100 0000 7258 0000 0029 0172 4c00 0000  1...rX...).rL...
+00001420: 720c 0000 0072 0d00 0000 7232 0000 008e  r....r....r2....
+00001430: 0000 0073 0200 0000 0600 2903 7206 0000  ...s......).r...
+00001440: 0072 0700 0000 7209 0000 0063 0100 0000  .r....r....c....
+00001450: 0000 0000 0200 0000 0400 0000 5300 0000  ............S...
+00001460: 7314 0000 0069 007c 005d 0c7d 017c 017c  s....i.|.].}.|.|
+00001470: 016a 0093 0271 0453 0072 0c00 0000 2901  .j...q.S.r....).
+00001480: 7240 0000 0029 0272 3100 0000 7258 0000  r@...).r1...rX..
+00001490: 0072 0c00 0000 720c 0000 0072 0d00 0000  .r....r....r....
+000014a0: fa0a 3c64 6963 7463 6f6d 703e 9400 0000  ..<dictcomp>....
+000014b0: 7302 0000 0006 007a 3742 6173 6545 7865  s......z7BaseExe
+000014c0: 6375 746f 722e 5f70 7265 6665 7463 685f  cutor._prefetch_
+000014d0: 6d32 6d5f 7265 6c61 7469 6f6e 2e3c 6c6f  m2m_relation.<lo
+000014e0: 6361 6c73 3e2e 3c64 6963 7463 6f6d 703e  cals>.<dictcomp>
+000014f0: 2921 723e 0000 0072 4500 0000 7240 0000  )!r>...rE...r@..
+00001500: 0072 0600 0000 721f 0000 0072 2200 0000  .r....r....r"...
+00001510: 7202 0000 00da 0774 6872 6f75 6768 7208  r......throughr.
+00001520: 0000 0072 3a00 0000 7242 0000 00da 0673  ...r:...rB.....s
+00001530: 656c 6563 7472 2f00 0000 da0c 6261 636b  electr/.....back
+00001540: 7761 7264 5f6b 6579 7256 0000 00da 0b66  ward_keyrV.....f
+00001550: 6f72 7761 7264 5f6b 6579 723f 0000 00da  orward_keyr?....
+00001560: 0469 7369 6e72 3900 0000 7216 0000 00da  .isinr9...r.....
+00001570: 046a 6f69 6eda 026f 6e72 5500 0000 7254  .join..onrU...rT
+00001580: 0000 0072 0300 0000 7210 0000 0072 1100  ...r....r....r..
+00001590: 0000 da09 5f5f 636c 6173 735f 5f5a 0d5f  ....__class__Z._
+000015a0: 7072 6566 6574 6368 5f6d 6170 da0e 6665  prefetch_map..fe
+000015b0: 7463 685f 666f 725f 6c69 7374 7213 0000  tch_for_listr...
+000015c0: 0072 4a00 0000 724b 0000 0029 1272 0b00  .rJ...rK...).r..
+000015d0: 0000 7218 0000 0072 1b00 0000 724c 0000  ..r....r....rL..
+000015e0: 0072 4d00 0000 721a 0000 0072 2a00 0000  .rM...r....r*...
+000015f0: da0d 7468 726f 7567 685f 7461 626c 65da  ..through_table.
+00001600: 0873 7562 7175 6572 7972 1600 0000 7217  .subqueryr....r.
+00001610: 0000 005a 0972 656c 6174 696f 6e73 724e  ...Z.relationsrN
+00001620: 0000 0072 4f00 0000 5a0c 7265 6c61 7469  ...rO...Z.relati
+00001630: 6f6e 5f6d 6170 7251 0000 005a 1172 656c  on_maprQ...Z.rel
+00001640: 6174 6564 5f6f 626a 6563 745f 6964 7252  ated_object_idrR
+00001650: 0000 0072 0c00 0000 2902 724c 0000 0072  ...r....).rL...r
+00001660: 5700 0000 720d 0000 00da 165f 7072 6566  W...r......_pref
+00001670: 6574 6368 5f6d 326d 5f72 656c 6174 696f  etch_m2m_relatio
+00001680: 6e77 0000 0073 4000 0000 0001 0601 0a01  nw...s@.........
+00001690: 1002 0e02 0a02 0e01 1001 1401 1402 0e01  ................
+000016a0: 0c01 0e02 0c01 1802 1601 0e01 1201 0401  ................
+000016b0: 0401 0401 0a01 0c01 0e01 0402 0e01 0a01  ................
+000016c0: 0801 1802 0a01 0a01 1a01 7a23 4261 7365  ..........z#Base
+000016d0: 4578 6563 7574 6f72 2e5f 7072 6566 6574  Executor._prefet
+000016e0: 6368 5f6d 326d 5f72 656c 6174 696f 6e63  ch_m2m_relationc
+000016f0: 0400 0000 0000 0000 0900 0000 0800 0000  ................
+00001700: c300 0000 738a 0000 0074 0083 007d 0464  ....s....t...}.d
+00001710: 016a 017c 0283 017d 0578 267c 0144 005d  .j.|...}.x&|.D.]
+00001720: 1e7d 0674 027c 067c 0583 0272 167c 046a  .}.t.|.|...r.|.j
+00001730: 0374 027c 067c 0583 0283 0101 0071 1657  .t.|.|.......q.W
+00001740: 007c 0472 867c 036a 0474 057c 0483 0164  .|.r.|.j.t.|...d
+00001750: 028d 0149 0064 0048 007d 0764 0364 0484  ...I.d.H.}.d.d..
+00001760: 007c 0744 0083 017d 0878 247c 0144 005d  .|.D...}.x$|.D.]
+00001770: 1c7d 0674 067c 067c 027c 086a 0774 027c  .}.t.|.|.|.j.t.|
+00001780: 067c 0583 0283 0183 0301 0071 6657 007c  .|.........qfW.|
+00001790: 0153 0029 054e 7a05 7b7d 5f69 6429 015a  .S.).Nz.{}_id).Z
+000017a0: 0669 645f 5f69 6e63 0100 0000 0000 0000  .id__inc........
+000017b0: 0200 0000 0400 0000 5300 0000 7314 0000  ........S...s...
+000017c0: 0069 007c 005d 0c7d 017c 017c 016a 0093  .i.|.].}.|.|.j..
+000017d0: 0271 0453 0072 0c00 0000 2901 7240 0000  .q.S.r....).r@..
+000017e0: 0029 0272 3100 0000 da03 6f62 6a72 0c00  .).r1.....objr..
+000017f0: 0000 720c 0000 0072 0d00 0000 725a 0000  ..r....r....rZ..
+00001800: 00a9 0000 0073 0200 0000 0600 7a3a 4261  .....s......z:Ba
+00001810: 7365 4578 6563 7574 6f72 2e5f 7072 6566  seExecutor._pref
+00001820: 6574 6368 5f64 6972 6563 745f 7265 6c61  etch_direct_rela
+00001830: 7469 6f6e 2e3c 6c6f 6361 6c73 3e2e 3c64  tion.<locals>.<d
+00001840: 6963 7463 6f6d 703e 2908 723e 0000 0072  ictcomp>).r>...r
+00001850: 4800 0000 722f 0000 0072 4500 0000 7247  H...r/...rE...rG
+00001860: 0000 0072 4900 0000 7212 0000 0072 4b00  ...rI...r....rK.
+00001870: 0000 2909 720b 0000 0072 1800 0000 721b  ..).r....r....r.
+00001880: 0000 0072 4c00 0000 5a19 7265 6c61 7465  ...rL...Z.relate
+00001890: 645f 6f62 6a65 6374 735f 666f 725f 6665  d_objects_for_fe
+000018a0: 7463 685a 1272 656c 6174 696f 6e5f 6b65  tchZ.relation_ke
+000018b0: 795f 6669 656c 6472 1a00 0000 724e 0000  y_fieldr....rN..
+000018c0: 0072 4f00 0000 720c 0000 0072 0c00 0000  .rO...r....r....
+000018d0: 720d 0000 00da 195f 7072 6566 6574 6368  r......_prefetch
+000018e0: 5f64 6972 6563 745f 7265 6c61 7469 6f6e  _direct_relation
+000018f0: a100 0000 7318 0000 0000 0106 010a 010a  ....s...........
+00001900: 010a 0114 0104 0116 010e 010a 0102 011a  ................
+00001910: 027a 2642 6173 6545 7865 6375 746f 722e  .z&BaseExecutor.
+00001920: 5f70 7265 6665 7463 685f 6469 7265 6374  _prefetch_direct
+00001930: 5f72 656c 6174 696f 6e63 0100 0000 0000  _relationc......
+00001940: 0000 0600 0000 0400 0000 4300 0000 7372  ..........C...sr
+00001950: 0000 0078 6c7c 006a 006a 0183 0044 005d  ...xl|.j.j...D.]
+00001960: 5e5c 027d 017d 027c 017c 006a 026b 0672  ^\.}.}.|.|.j.k.r
+00001970: 2c7c 006a 026a 037c 0183 017d 036e 267c  ,|.j.j.|...}.n&|
+00001980: 006a 046a 056a 066a 037c 0183 017d 047c  .j.j.j.j.|...}.|
+00001990: 046a 077d 057c 056a 0883 006a 097c 006a  .j.}.|.j...j.|.j
+000019a0: 0a83 017d 037c 0272 607c 036a 0b7c 028e  ...}.|.r`|.j.|..
+000019b0: 007d 037c 037c 006a 027c 013c 0071 0c57  .}.|.|.j.|.<.q.W
+000019c0: 0064 0053 0029 014e 290c 7209 0000 0072  .d.S.).N).r....r
+000019d0: 3c00 0000 720a 0000 0072 4b00 0000 7206  <...r....rK...r.
+000019e0: 0000 0072 1f00 0000 7222 0000 00da 0474  ...r....r".....t
+000019f0: 7970 65da 0361 6c6c da08 7573 696e 675f  ype..all..using_
+00001a00: 6462 7208 0000 005a 1070 7265 6665 7463  dbr....Z.prefetc
+00001a10: 685f 7265 6c61 7465 6429 0672 0b00 0000  h_related).r....
+00001a20: 721b 0000 005a 1466 6f72 7761 7264 6564  r....Z.forwarded
+00001a30: 5f70 7265 6665 7463 6865 7372 4c00 0000  _prefetchesrL...
+00001a40: 5a13 7265 6c61 7465 645f 6d6f 6465 6c5f  Z.related_model_
+00001a50: 6669 656c 64da 0d72 656c 6174 6564 5f6d  field..related_m
+00001a60: 6f64 656c 720c 0000 0072 0c00 0000 720d  odelr....r....r.
+00001a70: 0000 00da 165f 6d61 6b65 5f70 7265 6665  ....._make_prefe
+00001a80: 7463 685f 7175 6572 6965 73b0 0000 0073  tch_queries....s
+00001a90: 1200 0000 0001 1401 0a01 0e02 1001 0601  ................
+00001aa0: 1001 0401 0a01 7a23 4261 7365 4578 6563  ......z#BaseExec
+00001ab0: 7574 6f72 2e5f 6d61 6b65 5f70 7265 6665  utor._make_prefe
+00001ac0: 7463 685f 7175 6572 6965 7363 0400 0000  tch_queriesc....
+00001ad0: 0000 0000 0400 0000 0400 0000 c300 0000  ................
+00001ae0: 7368 0000 0074 0074 017c 006a 027c 0283  sh...t.t.|.j.|..
+00001af0: 0274 036a 0483 0272 287c 006a 057c 017c  .t.j...r(|.j.|.|
+00001b00: 027c 0383 0349 0064 0048 0053 0074 0074  .|...I.d.H.S.t.t
+00001b10: 017c 006a 027c 0283 0274 036a 0683 0272  .|.j.|...t.j...r
+00001b20: 507c 006a 077c 017c 027c 0383 0349 0064  P|.j.|.|.|...I.d
+00001b30: 0048 0053 007c 006a 087c 017c 027c 0383  .H.S.|.j.|.|.|..
+00001b40: 0349 0064 0048 0053 0064 0053 0029 014e  .I.d.H.S.d.S.).N
+00001b50: 2909 7223 0000 0072 2f00 0000 7206 0000  ).r#...r/...r...
+00001b60: 0072 0300 0000 da12 4261 636b 7761 7264  .r......Backward
+00001b70: 464b 5265 6c61 7469 6f6e 7253 0000 00da  FKRelationrS....
+00001b80: 0f4d 616e 7954 6f4d 616e 7946 6965 6c64  .ManyToManyField
+00001b90: 7266 0000 0072 6800 0000 2904 720b 0000  rf...rh...).r...
+00001ba0: 005a 1069 6e73 7461 6e63 655f 6964 5f6c  .Z.instance_id_l
+00001bb0: 6973 7472 1b00 0000 724c 0000 0072 0c00  istr....rL...r..
+00001bc0: 0000 720c 0000 0072 0d00 0000 da0c 5f64  ..r....r......_d
+00001bd0: 6f5f 7072 6566 6574 6368 bc00 0000 730a  o_prefetch....s.
+00001be0: 0000 0000 0114 0114 0114 0114 027a 1942  .............z.B
+00001bf0: 6173 6545 7865 6375 746f 722e 5f64 6f5f  aseExecutor._do_
+00001c00: 7072 6566 6574 6368 6302 0000 0000 0000  prefetchc.......
+00001c10: 0004 0000 0005 0000 00c3 0000 0073 4800  .............sH.
+00001c20: 0000 7c01 7244 7c00 6a00 7310 7c00 6a01  ..|.rD|.j.s.|.j.
+00001c30: 7244 7c00 6a02 8300 0100 782a 7c00 6a01  rD|.j.....x*|.j.
+00001c40: 6a03 8300 4400 5d1c 5c02 7d02 7d03 7c00  j...D.].\.}.}.|.
+00001c50: 6a04 7c01 7c02 7c03 8303 4900 6400 4800  j.|.|.|...I.d.H.
+00001c60: 0100 7124 5700 7c01 5300 2901 4e29 0572  ..q$W.|.S.).N).r
+00001c70: 0900 0000 720a 0000 0072 6d00 0000 723c  ....r....rm...r<
+00001c80: 0000 0072 7000 0000 2904 720b 0000 0072  ...rp...).r....r
+00001c90: 1800 0000 721b 0000 0072 4c00 0000 720c  ....r....rL...r.
+00001ca0: 0000 0072 0c00 0000 720d 0000 0072 1400  ...r....r....r..
+00001cb0: 0000 c400 0000 730a 0000 0000 0110 0108  ......s.........
+00001cc0: 0114 0118 017a 2642 6173 6545 7865 6375  .....z&BaseExecu
+00001cd0: 746f 722e 5f65 7865 6375 7465 5f70 7265  tor._execute_pre
+00001ce0: 6665 7463 685f 7175 6572 6965 7363 0200  fetch_queriesc..
+00001cf0: 0000 0000 0000 0700 0000 0500 0000 c700  ................
+00001d00: 0000 73ca 0000 007c 006a 006a 0183 0049  ..s....|.j.j...I
+00001d10: 0064 0048 007c 005f 0269 007c 005f 0378  .d.H.|._.i.|._.x
+00001d20: 827c 0244 005d 7a7d 037c 036a 0464 0183  .|.D.]z}.|.j.d..
+00001d30: 017d 047c 0464 0219 007d 057c 057c 006a  .}.|.d...}.|.|.j
+00001d40: 056a 066a 076b 0772 5874 0864 036a 097c  .j.j.k.rXt.d.j.|
+00001d50: 057c 006a 056a 066a 0a83 0283 0182 017c  .|.j.j.j.......|
+00001d60: 057c 006a 036a 0b83 006b 0772 7274 0c83  .|.j.j...k.rrt..
+00001d70: 007c 006a 037c 053c 0064 016a 0d7c 0464  .|.j.|.<.d.j.|.d
+00001d80: 0464 0085 0219 0083 017d 067c 0672 1e7c  .d.......}.|.r.|
+00001d90: 006a 037c 0519 006a 0e7c 0683 0101 0071  .j.|...j.|.....q
+00001da0: 1e57 007c 006a 0f7c 0183 0149 0064 0048  .W.|.j.|...I.d.H
+00001db0: 0001 007c 006a 006a 107c 006a 0283 0149  ...|.j.j.|.j...I
+00001dc0: 0064 0048 0001 0064 007c 005f 027c 0153  .d.H...d.|._.|.S
+00001dd0: 0029 054e da02 5f5f 7201 0000 007a 1c72  .).N..__r....z.r
+00001de0: 656c 6174 696f 6e20 7b7d 2066 6f72 207b  elation {} for {
+00001df0: 7d20 6e6f 7420 666f 756e 64e9 0100 0000  } not found.....
+00001e00: 2911 7207 0000 0072 0f00 0000 7208 0000  ).r....r....r...
+00001e10: 0072 0900 0000 da05 7370 6c69 7472 0600  .r......splitr..
+00001e20: 0000 721f 0000 00da 0c66 6574 6368 5f66  ..r......fetch_f
+00001e30: 6965 6c64 7372 0400 0000 7248 0000 0072  ieldsr....rH...r
+00001e40: 3900 0000 7221 0000 0072 3e00 0000 7260  9...r!...r>...r`
+00001e50: 0000 0072 4500 0000 7214 0000 0072 1500  ...rE...r....r..
+00001e60: 0000 2907 720b 0000 0072 1800 0000 da04  ..).r....r......
+00001e70: 6172 6773 da08 7265 6c61 7469 6f6e 5a0e  args..relationZ.
+00001e80: 7265 6c61 7469 6f6e 5f73 706c 6974 5a11  relation_splitZ.
+00001e90: 6669 7273 745f 6c65 7665 6c5f 6669 656c  first_level_fiel
+00001ea0: 645a 1266 6f72 7761 7264 6564 5f70 7265  dZ.forwarded_pre
+00001eb0: 6665 7463 6872 0c00 0000 720c 0000 0072  fetchr....r....r
+00001ec0: 0d00 0000 7263 0000 00cb 0000 0073 2200  ....rc.......s".
+00001ed0: 0000 0001 1201 0601 0a01 0a01 0801 0e01  ................
+00001ee0: 0601 1001 0e01 0c01 1201 0401 1401 1001  ................
+00001ef0: 1401 0601 7a1b 4261 7365 4578 6563 7574  ....z.BaseExecut
+00001f00: 6f72 2e66 6574 6368 5f66 6f72 5f6c 6973  or.fetch_for_lis
+00001f10: 7429 034e 4e4e 2901 4e29 13da 085f 5f6e  t).NNN).N)...__n
+00001f20: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
+00001f30: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5f72  _..__qualname__r
+00001f40: 0e00 0000 721c 0000 0072 2b00 0000 722e  ....r....r+...r.
+00001f50: 0000 0072 3000 0000 7236 0000 0072 3800  ...r0...r6...r8.
+00001f60: 0000 7241 0000 0072 4400 0000 7253 0000  ..rA...rD...rS..
+00001f70: 0072 6600 0000 7268 0000 0072 6d00 0000  .rf...rh...rm...
+00001f80: 7270 0000 0072 1400 0000 7263 0000 0072  rp...r....rc...r
+00001f90: 0c00 0000 720c 0000 0072 0c00 0000 720d  ....r....r....r.
+00001fa0: 0000 0072 0500 0000 0900 0000 7320 0000  ...r........s ..
+00001fb0: 0008 010a 070a 0f08 0e08 0308 0308 0908  ................
+00001fc0: 0608 1708 0608 1708 2a08 0f08 0c08 0808  ........*.......
+00001fd0: 0772 0500 0000 2908 721d 0000 00da 0670  .r....).r......p
+00001fe0: 7970 696b 6172 0200 0000 da08 746f 7274  ypikar......tort
+00001ff0: 6f69 7365 7203 0000 00da 1374 6f72 746f  oiser......torto
+00002000: 6973 652e 6578 6365 7074 696f 6e73 7204  ise.exceptionsr.
+00002010: 0000 0072 0500 0000 720c 0000 0072 0c00  ...r....r....r..
+00002020: 0000 720c 0000 0072 0d00 0000 da08 3c6d  ..r....r......<m
+00002030: 6f64 756c 653e 0100 0000 7308 0000 0008  odule>....s.....
+00002040: 020c 020c 010c 03                        .......
```

### Comparing `tortoise-orm-0.9.2/tortoise/backends/base/schema_generator.py` & `tortoise-orm-0.9.4/tortoise/backends/base/schema_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,11 @@
+from typing import List, Set  # noqa
+
 from tortoise import fields
+from tortoise.exceptions import ConfigurationError
 
 TABLE_CREATE_TEMPLATE = 'CREATE TABLE "{}" ({});'
 FIELD_TEMPLATE = '"{name}" {type} {nullable} {unique}'
 FK_TEMPLATE = ' REFERENCES "{table}" (id) ON DELETE {on_delete}'
 M2M_TABLE_TEMPLATE = (
     'CREATE TABLE "{table_name}" '
     '("{backward_key}" INT NOT NULL REFERENCES "{backward_table}" (id) ON DELETE CASCADE, '
@@ -31,15 +34,15 @@
         # All databases have their unique way for autoincrement,
         # has to implement in children
         raise NotImplementedError()  # pragma: nocoverage
 
     def _get_auto_now_add_default(self):
         raise NotImplementedError()  # pragma: nocoverage
 
-    def _get_table_sql(self, model):
+    def _get_table_sql(self, model) -> dict:
         fields_to_create = []
         m2m_tables_for_create = []
         references = set()
         for field_name, db_field in model._meta.fields_db_projection.items():
             field_object = model._meta.fields_map[field_name]
             if isinstance(field_object, fields.IntField) and field_object.pk:
                 fields_to_create.append(self._get_primary_key_create_string(field_name))
@@ -103,26 +106,26 @@
 
         tables_to_create = []
         for model in models_to_create:
             tables_to_create.append(self._get_table_sql(model))
 
         tables_to_create_count = len(tables_to_create)
 
-        created_tables = set()
+        created_tables = set()  # type: Set[dict]
         ordered_tables_for_create = []
-        m2m_tables_to_create = []
+        m2m_tables_to_create = []  # type: List[str]
         while True:
             if len(created_tables) == tables_to_create_count:
                 break
             try:
                 next_table_for_create = next(
                     t for t in tables_to_create if t['references'].issubset(created_tables)
                 )
             except StopIteration:
-                raise ValueError("Can't create schema due to cyclic fk references")
+                raise ConfigurationError("Can't create schema due to cyclic fk references")
             tables_to_create.remove(next_table_for_create)
             created_tables.add(next_table_for_create['table'])
             ordered_tables_for_create.append(next_table_for_create['table_creation_string'])
             m2m_tables_to_create += next_table_for_create['m2m_tables']
 
         schema_creation_string = ' '.join(ordered_tables_for_create + m2m_tables_to_create)
         return schema_creation_string
```

### Comparing `tortoise-orm-0.9.2/tortoise/tests/test_basic.py` & `tortoise-orm-0.9.4/tortoise/tests/test_basic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from tortoise.contrib.test import TestCase
+from tortoise.contrib import test
 from tortoise.tests.testmodels import Tournament
 
 
-class TestBasic(TestCase):
+class TestBasic(test.TestCase):
     async def test_basic(self):
         event = await Tournament.create(name='Test')
         await Tournament.filter(id=event.id).update(name='Updated name')
         saved_event = await Tournament.filter(name='Updated name').first()
         self.assertEqual(saved_event.id, event.id)
         await Tournament(name='Test 2').save()
         self.assertEqual(
```

### Comparing `tortoise-orm-0.9.2/tortoise/tests/test_schema_create.py` & `tortoise-orm-0.9.4/tortoise/tests/test_schema_create.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import datetime
 
-from tortoise.contrib.test import TestCase
+from tortoise.contrib import test
 from tortoise.tests.testmodels import Event, Team, Tournament
 
 
-class TestSchemaCreate(TestCase):
+class TestSchemaCreate(test.TestCase):
 
     async def test_schema_create(self):
         tournament = await Tournament.create(name='Test')
         self.assertEqual(
             tournament.created and tournament.created.date(),
             datetime.datetime.utcnow().date()
         )
```

### Comparing `tortoise-orm-0.9.2/tortoise/tests/test_aggregation.py` & `tortoise-orm-0.9.4/tortoise/tests/test_aggregation.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from tortoise.aggregation import Count, Min, Sum
-from tortoise.contrib.test import TestCase
+from tortoise.contrib import test
 from tortoise.tests.testmodels import Event, Team, Tournament
 
 
-class TestAggregation(TestCase):
+class TestAggregation(test.TestCase):
     async def test_aggregation(self):
         tournament = Tournament(name='New Tournament')
         await tournament.save()
         await Tournament.create(name='Second tournament')
         await Event(name='Without participants', tournament_id=tournament.id).save()
         event = Event(name='Test', tournament_id=tournament.id)
         await event.save()
```

### Comparing `tortoise-orm-0.9.2/tortoise/tests/__pycache__/test_fields.cpython-36.pyc` & `tortoise-orm-0.9.4/tortoise/tests/__pycache__/test_fields.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `tortoise-orm-0.9.2/tortoise/tests/__pycache__/test_relations.cpython-36.pyc` & `tortoise-orm-0.9.4/tortoise/tests/__pycache__/test_relations.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `tortoise-orm-0.9.2/tortoise/tests/__pycache__/test_transactions.cpython-36.pyc` & `tortoise-orm-0.9.4/tortoise/tests/__pycache__/test_transactions.cpython-37.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.6 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 14% similar despite different names*

```diff
@@ -1,70 +1,70 @@
-00000000: 330d 0d0a 7781 3c5b a903 0000 e300 0000  3...w.<[........
-00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 3800 0000 6400 6401 6c00 6d01 5a01  .s8...d.d.l.m.Z.
-00000030: 0100 6400 6402 6c02 6d03 5a03 0100 6400  ..d.d.l.m.Z...d.
-00000040: 6403 6c04 6d05 5a05 0100 4700 6404 6405  d.l.m.Z...G.d.d.
-00000050: 8400 6405 6501 8303 5a06 6406 5300 2907  ..d.e...Z.d.S.).
-00000060: e900 0000 0029 01da 0854 6573 7443 6173  .....)...TestCas
-00000070: 6529 01da 104f 7065 7261 7469 6f6e 616c  e)...Operational
-00000080: 4572 726f 7229 01da 0a54 6f75 726e 616d  Error)...Tournam
-00000090: 656e 7463 0000 0000 0000 0000 0000 0000  entc............
-000000a0: 0200 0000 4000 0000 7314 0000 0065 005a  ....@...s....e.Z
-000000b0: 0164 005a 0264 0164 0284 005a 0364 0353  .d.Z.d.d...Z.d.S
-000000c0: 0029 04da 1054 6573 7454 7261 6e73 6163  .)...TestTransac
-000000d0: 7469 6f6e 7363 0100 0000 0000 0000 0400  tionsc..........
-000000e0: 0000 1100 0000 c300 0000 73d8 0000 007c  ..........s....|
-000000f0: 006a 0074 0183 018f a401 007c 006a 026a  .j.t.......|.j.j
-00000100: 0383 0034 0049 0064 0048 009a 807d 0174  ...4.I.d.H...}.t
-00000110: 0464 0164 028d 017d 027c 026a 057c 0164  .d.d...}.|.j.|.d
-00000120: 038d 0149 0064 0048 0001 0074 046a 067c  ...I.d.H...t.j.|
-00000130: 026a 0764 048d 016a 087c 0183 016a 0964  .j.d...j.|...j.d
-00000140: 0564 028d 0149 0064 0048 0001 0074 046a  .d...I.d.H...t.j
-00000150: 0664 0564 028d 016a 087c 0183 016a 0a83  .d.d...j.|...j..
-00000160: 0049 0064 0048 007d 037c 006a 0b7c 036a  .I.d.H.}.|.j.|.j
-00000170: 077c 026a 0783 0201 007c 016a 0c64 0683  .|.j.....|.j.d..
-00000180: 0149 0064 0048 0001 0057 0064 0051 0049  .I.d.H...W.d.Q.I
-00000190: 0064 0048 0052 0058 0057 0064 0051 0052  .d.H.R.X.W.d.Q.R
-000001a0: 0058 0074 046a 0664 0564 028d 016a 0a83  .X.t.j.d.d...j..
-000001b0: 0049 0064 0048 007d 037c 006a 0d7c 0383  .I.d.H.}.|.j.|..
-000001c0: 0101 0064 0053 0029 074e da04 5465 7374  ...d.S.).N..Test
-000001d0: 2901 da04 6e61 6d65 2901 da08 7573 696e  )...name)...usin
-000001e0: 675f 6462 2901 da02 6964 7a0c 5570 6461  g_db)...idz.Upda
-000001f0: 7465 6420 6e61 6d65 7a20 5345 4c45 4354  ted namez SELECT
-00000200: 202a 2046 524f 4d20 6e6f 6e5f 6578 6973   * FROM non_exis
-00000210: 7465 6e74 5f74 6162 6c65 290e da0c 6173  tent_table)...as
-00000220: 7365 7274 5261 6973 6573 7203 0000 00da  sertRaisesr.....
-00000230: 0264 62da 0e69 6e5f 7472 616e 7361 6374  .db..in_transact
-00000240: 696f 6e72 0400 0000 da04 7361 7665 da06  ionr......save..
-00000250: 6669 6c74 6572 7209 0000 0072 0800 0000  filterr....r....
-00000260: da06 7570 6461 7465 da05 6669 7273 74da  ..update..first.
-00000270: 0b61 7373 6572 7445 7175 616c da0d 6578  .assertEqual..ex
-00000280: 6563 7574 655f 7175 6572 79da 0c61 7373  ecute_query..ass
-00000290: 6572 7449 734e 6f6e 6529 04da 0473 656c  ertIsNone)...sel
-000002a0: 66da 0a63 6f6e 6e65 6374 696f 6eda 0565  f..connection..e
-000002b0: 7665 6e74 da0b 7361 7665 645f 6576 656e  vent..saved_even
-000002c0: 74a9 0072 1800 0000 fa54 2f55 7365 7273  t..r.....T/Users
-000002d0: 2f61 6e64 7265 7962 6f6e 6461 722f 5079  /andreybondar/Py
-000002e0: 4368 6172 6d50 726f 6a65 6374 732f 746f  CharmProjects/to
-000002f0: 7274 6f69 7365 2d6f 726d 2f74 6f72 746f  rtoise-orm/torto
-00000300: 6973 652f 7465 7374 732f 7465 7374 5f74  ise/tests/test_t
-00000310: 7261 6e73 6163 7469 6f6e 732e 7079 da11  ransactions.py..
-00000320: 7465 7374 5f74 7261 6e73 6163 7469 6f6e  test_transaction
-00000330: 7308 0000 0073 1800 0000 0001 0c01 1401  s....s..........
-00000340: 0a01 1201 0e01 1401 0401 1801 1001 2a02  ..............*.
-00000350: 1601 7a22 5465 7374 5472 616e 7361 6374  ..z"TestTransact
-00000360: 696f 6e73 2e74 6573 745f 7472 616e 7361  ions.test_transa
-00000370: 6374 696f 6e73 4e29 04da 085f 5f6e 616d  ctionsN)...__nam
-00000380: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
-00000390: 0c5f 5f71 7561 6c6e 616d 655f 5f72 1a00  .__qualname__r..
-000003a0: 0000 7218 0000 0072 1800 0000 7218 0000  ..r....r....r...
-000003b0: 0072 1900 0000 7205 0000 0006 0000 0073  .r....r........s
-000003c0: 0200 0000 0802 7205 0000 004e 2907 da15  ......r....N)...
-000003d0: 746f 7274 6f69 7365 2e63 6f6e 7472 6962  tortoise.contrib
-000003e0: 2e74 6573 7472 0200 0000 da13 746f 7274  .testr......tort
-000003f0: 6f69 7365 2e65 7863 6570 7469 6f6e 7372  oise.exceptionsr
-00000400: 0300 0000 da19 746f 7274 6f69 7365 2e74  ......tortoise.t
-00000410: 6573 7473 2e74 6573 746d 6f64 656c 7372  ests.testmodelsr
-00000420: 0400 0000 7205 0000 0072 1800 0000 7218  ....r....r....r.
-00000430: 0000 0072 1800 0000 7219 0000 00da 083c  ...r....r......<
-00000440: 6d6f 6475 6c65 3e01 0000 0073 0600 0000  module>....s....
-00000450: 0c01 0c01 0c03                           ......
+00000000: 420d 0d0a 0000 0000 7781 3c5b a903 0000  B.......w.<[....
+00000010: e300 0000 0000 0000 0000 0000 0004 0000  ................
+00000020: 0040 0000 0073 3800 0000 6400 6401 6c00  .@...s8...d.d.l.
+00000030: 6d01 5a01 0100 6400 6402 6c02 6d03 5a03  m.Z...d.d.l.m.Z.
+00000040: 0100 6400 6403 6c04 6d05 5a05 0100 4700  ..d.d.l.m.Z...G.
+00000050: 6404 6405 8400 6405 6501 8303 5a06 6406  d.d...d.e...Z.d.
+00000060: 5300 2907 e900 0000 0029 01da 0854 6573  S.)......)...Tes
+00000070: 7443 6173 6529 01da 104f 7065 7261 7469  tCase)...Operati
+00000080: 6f6e 616c 4572 726f 7229 01da 0a54 6f75  onalError)...Tou
+00000090: 726e 616d 656e 7463 0000 0000 0000 0000  rnamentc........
+000000a0: 0000 0000 0200 0000 4000 0000 7314 0000  ........@...s...
+000000b0: 0065 005a 0164 005a 0264 0164 0284 005a  .e.Z.d.Z.d.d...Z
+000000c0: 0364 0353 0029 04da 1054 6573 7454 7261  .d.S.)...TestTra
+000000d0: 6e73 6163 7469 6f6e 7363 0100 0000 0000  nsactionsc......
+000000e0: 0000 0400 0000 0b00 0000 c300 0000 73d8  ..............s.
+000000f0: 0000 007c 00a0 0074 01a1 018f a401 007c  ...|...t.......|
+00000100: 006a 02a0 03a1 0034 0049 0064 0048 009a  .j.....4.I.d.H..
+00000110: 807d 0174 0464 0164 028d 017d 027c 026a  .}.t.d.d...}.|.j
+00000120: 057c 0164 038d 0149 0064 0048 0001 0074  .|.d...I.d.H...t
+00000130: 046a 067c 026a 0764 048d 01a0 087c 01a1  .j.|.j.d.....|..
+00000140: 016a 0964 0564 028d 0149 0064 0048 0001  .j.d.d...I.d.H..
+00000150: 0074 046a 0664 0564 028d 01a0 087c 01a1  .t.j.d.d.....|..
+00000160: 01a0 0aa1 0049 0064 0048 007d 037c 00a0  .....I.d.H.}.|..
+00000170: 0b7c 036a 077c 026a 07a1 0201 007c 01a0  .|.j.|.j.....|..
+00000180: 0c64 06a1 0149 0064 0048 0001 0057 0064  .d...I.d.H...W.d
+00000190: 0051 0049 0064 0048 0052 0058 0057 0064  .Q.I.d.H.R.X.W.d
+000001a0: 0051 0052 0058 0074 046a 0664 0564 028d  .Q.R.X.t.j.d.d..
+000001b0: 01a0 0aa1 0049 0064 0048 007d 037c 00a0  .....I.d.H.}.|..
+000001c0: 0d7c 03a1 0101 0064 0053 0029 074e da04  .|.....d.S.).N..
+000001d0: 5465 7374 2901 da04 6e61 6d65 2901 da08  Test)...name)...
+000001e0: 7573 696e 675f 6462 2901 da02 6964 7a0c  using_db)...idz.
+000001f0: 5570 6461 7465 6420 6e61 6d65 7a20 5345  Updated namez SE
+00000200: 4c45 4354 202a 2046 524f 4d20 6e6f 6e5f  LECT * FROM non_
+00000210: 6578 6973 7465 6e74 5f74 6162 6c65 290e  existent_table).
+00000220: da0c 6173 7365 7274 5261 6973 6573 7203  ..assertRaisesr.
+00000230: 0000 00da 0264 62da 0e69 6e5f 7472 616e  .....db..in_tran
+00000240: 7361 6374 696f 6e72 0400 0000 da04 7361  sactionr......sa
+00000250: 7665 da06 6669 6c74 6572 7209 0000 0072  ve..filterr....r
+00000260: 0800 0000 da06 7570 6461 7465 da05 6669  ......update..fi
+00000270: 7273 74da 0b61 7373 6572 7445 7175 616c  rst..assertEqual
+00000280: da0d 6578 6563 7574 655f 7175 6572 79da  ..execute_query.
+00000290: 0c61 7373 6572 7449 734e 6f6e 6529 04da  .assertIsNone)..
+000002a0: 0473 656c 66da 0a63 6f6e 6e65 6374 696f  .self..connectio
+000002b0: 6eda 0565 7665 6e74 da0b 7361 7665 645f  n..event..saved_
+000002c0: 6576 656e 74a9 0072 1800 0000 fa54 2f55  event..r.....T/U
+000002d0: 7365 7273 2f61 6e64 7265 7962 6f6e 6461  sers/andreybonda
+000002e0: 722f 5079 4368 6172 6d50 726f 6a65 6374  r/PyCharmProject
+000002f0: 732f 746f 7274 6f69 7365 2d6f 726d 2f74  s/tortoise-orm/t
+00000300: 6f72 746f 6973 652f 7465 7374 732f 7465  ortoise/tests/te
+00000310: 7374 5f74 7261 6e73 6163 7469 6f6e 732e  st_transactions.
+00000320: 7079 da11 7465 7374 5f74 7261 6e73 6163  py..test_transac
+00000330: 7469 6f6e 7308 0000 0073 1800 0000 0001  tions....s......
+00000340: 0c01 1401 0a01 1201 0e01 1401 0401 1801  ................
+00000350: 1001 2a02 1601 7a22 5465 7374 5472 616e  ..*...z"TestTran
+00000360: 7361 6374 696f 6e73 2e74 6573 745f 7472  sactions.test_tr
+00000370: 616e 7361 6374 696f 6e73 4e29 04da 085f  ansactionsN)..._
+00000380: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
+00000390: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
+000003a0: 5f72 1a00 0000 7218 0000 0072 1800 0000  _r....r....r....
+000003b0: 7218 0000 0072 1900 0000 7205 0000 0006  r....r....r.....
+000003c0: 0000 0073 0200 0000 0802 7205 0000 004e  ...s......r....N
+000003d0: 2907 da15 746f 7274 6f69 7365 2e63 6f6e  )...tortoise.con
+000003e0: 7472 6962 2e74 6573 7472 0200 0000 da13  trib.testr......
+000003f0: 746f 7274 6f69 7365 2e65 7863 6570 7469  tortoise.excepti
+00000400: 6f6e 7372 0300 0000 da19 746f 7274 6f69  onsr......tortoi
+00000410: 7365 2e74 6573 7473 2e74 6573 746d 6f64  se.tests.testmod
+00000420: 656c 7372 0400 0000 7205 0000 0072 1800  elsr....r....r..
+00000430: 0000 7218 0000 0072 1800 0000 7219 0000  ..r....r....r...
+00000440: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
+00000450: 0600 0000 0c01 0c01 0c03                 ..........
```

### Comparing `tortoise-orm-0.9.2/tortoise/tests/__pycache__/test_aggregation.cpython-36.pyc` & `tortoise-orm-0.9.4/tortoise/tests/__pycache__/test_aggregation.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `tortoise-orm-0.9.2/tortoise/tests/__pycache__/test_schema_create.cpython-36.pyc` & `tortoise-orm-0.9.4/tortoise/tests/__pycache__/test_schema_create.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `tortoise-orm-0.9.2/tortoise/tests/__pycache__/test_prefetching.cpython-36.pyc` & `tortoise-orm-0.9.4/tortoise/tests/__pycache__/test_prefetching.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `tortoise-orm-0.9.2/tortoise/tests/__pycache__/test_two_databases.cpython-36.pyc` & `tortoise-orm-0.9.4/tortoise/tests/__pycache__/test_two_databases.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.6 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 19% similar despite different names*

```diff
@@ -1,156 +1,206 @@
-00000000: 330d 0d0a 5576 3f5b 7209 0000 e300 0000  3...Uv?[r.......
+00000000: 330d 0d0a d98d 4c5b 520e 0000 e300 0000  3.....L[R.......
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 5800 0000 6400 6401 6c00 6d01 5a01  .sX...d.d.l.m.Z.
+00000020: 0073 7800 0000 6400 6401 6c00 6d01 5a01  .sx...d.d.l.m.Z.
 00000030: 0100 6400 6402 6c02 6d03 5a03 0100 6400  ..d.d.l.m.Z...d.
 00000040: 6403 6c04 6d05 5a05 0100 6400 6404 6c06  d.l.m.Z...d.d.l.
-00000050: 6d07 5a07 6d08 5a08 6d09 5a09 0100 6400  m.Z.m.Z.m.Z...d.
-00000060: 6405 6c0a 6d0b 5a0b 0100 4700 6406 6407  d.l.m.Z...G.d.d.
-00000070: 8400 6407 6503 8303 5a0c 6408 5300 2909  ..d.e...Z.d.S.).
-00000080: e900 0000 0029 01da 0854 6f72 746f 6973  .....)...Tortois
-00000090: 6529 01da 0854 6573 7443 6173 6529 01da  e)...TestCase)..
-000000a0: 104f 7065 7261 7469 6f6e 616c 4572 726f  .OperationalErro
-000000b0: 7229 03da 0845 7665 6e74 5477 6fda 0754  r)...EventTwo..T
-000000c0: 6561 6d54 776f da0a 546f 7572 6e61 6d65  eamTwo..Tourname
-000000d0: 6e74 2901 da0f 6765 6e65 7261 7465 5f73  nt)...generate_s
-000000e0: 6368 656d 6163 0000 0000 0000 0000 0000  chemac..........
-000000f0: 0000 0200 0000 4000 0000 732c 0000 0065  ......@...s,...e
-00000100: 005a 0164 005a 0264 0164 0284 005a 0364  .Z.d.Z.d.d...Z.d
-00000110: 0364 0484 005a 0464 0564 0684 005a 0564  .d...Z.d.d...Z.d
-00000120: 0764 0884 005a 0664 0953 0029 0ada 1054  .d...Z.d.S.)...T
-00000130: 6573 7454 776f 4461 7461 6261 7365 7363  estTwoDatabasesc
-00000140: 0100 0000 0000 0000 0100 0000 0400 0000  ................
-00000150: c300 0000 7368 0000 007c 006a 0083 0049  ....sh...|.j...I
-00000160: 0064 0048 0001 007c 006a 0183 0049 0064  .d.H...|.j...I.d
-00000170: 0048 007c 005f 027c 006a 0183 0049 0064  .H.|._.|.j...I.d
-00000180: 0048 007c 005f 0374 046a 057c 006a 027c  .H.|._.t.j.|.j.|
-00000190: 006a 0364 019c 0264 028d 0101 0074 067c  .j.d...d.....t.|
-000001a0: 006a 0283 0149 0064 0048 0001 0074 067c  .j...I.d.H...t.|
-000001b0: 006a 0383 0149 0064 0048 0001 0064 0053  .j...I.d.H...d.S
-000001c0: 0029 034e 2902 da06 6d6f 6465 6c73 da06  .).N)...models..
-000001d0: 6576 656e 7473 2901 da0a 6462 5f72 6f75  events)...db_rou
-000001e0: 7469 6e67 2907 da0b 5f74 6561 7244 6f77  ting)..._tearDow
-000001f0: 6e44 42da 0567 6574 4442 da02 6462 da09  nDB..getDB..db..
-00000200: 7365 636f 6e64 5f64 6272 0200 0000 da0f  second_dbr......
-00000210: 5f63 6c69 656e 745f 726f 7574 696e 6772  _client_routingr
-00000220: 0800 0000 2901 da04 7365 6c66 a900 7213  ....)...self..r.
-00000230: 0000 00fa 552f 5573 6572 732f 616e 6472  ....U/Users/andr
-00000240: 6579 626f 6e64 6172 2f50 7943 6861 726d  eybondar/PyCharm
-00000250: 5072 6f6a 6563 7473 2f74 6f72 746f 6973  Projects/tortois
-00000260: 652d 6f72 6d2f 746f 7274 6f69 7365 2f74  e-orm/tortoise/t
-00000270: 6573 7473 2f74 6573 745f 7477 6f5f 6461  ests/test_two_da
-00000280: 7461 6261 7365 732e 7079 da05 7365 7455  tabases.py..setU
-00000290: 7009 0000 0073 1000 0000 0001 0e01 1001  p....s..........
-000002a0: 1001 0401 0401 0e02 1001 7a16 5465 7374  ..........z.Test
-000002b0: 5477 6f44 6174 6162 6173 6573 2e73 6574  TwoDatabases.set
-000002c0: 5570 6301 0000 0000 0000 0001 0000 0002  Upc.............
-000002d0: 0000 00c3 0000 0073 2400 0000 7c00 6a00  .......s$...|.j.
-000002e0: 6a01 8300 4900 6400 4800 0100 7c00 6a00  j...I.d.H...|.j.
-000002f0: 6a02 8300 4900 6400 4800 0100 6400 5300  j...I.d.H...d.S.
-00000300: 2901 4e29 0372 1000 0000 da05 636c 6f73  ).N).r......clos
-00000310: 65da 0964 625f 6465 6c65 7465 2901 7212  e..db_delete).r.
-00000320: 0000 0072 1300 0000 7213 0000 0072 1400  ...r....r....r..
-00000330: 0000 da08 7465 6172 446f 776e 1400 0000  ....tearDown....
-00000340: 7304 0000 0000 0110 017a 1954 6573 7454  s........z.TestT
-00000350: 776f 4461 7461 6261 7365 732e 7465 6172  woDatabases.tear
-00000360: 446f 776e 6301 0000 0000 0000 0003 0000  Downc...........
-00000370: 000d 0000 00c3 0000 0073 8600 0000 7400  .........s....t.
-00000380: 6a01 6401 6402 8d01 4900 6400 4800 7d01  j.d.d...I.d.H.}.
-00000390: 7402 6a01 6403 7c01 6a03 6404 8d02 4900  t.j.d.|.j.d...I.
-000003a0: 6400 4800 0100 7c00 6a04 7405 8301 8f18  d.H...|.j.t.....
-000003b0: 0100 7c00 6a06 6a07 6405 8301 4900 6400  ..|.j.j.d...I.d.
-000003c0: 4800 0100 5700 6400 5100 5200 5800 7c00  H...W.d.Q.R.X.|.
-000003d0: 6a08 6a07 6405 8301 4900 6400 4800 7d02  j.j.d...I.d.H.}.
-000003e0: 7c00 6a09 740a 7c02 6406 1900 6a0b 8300  |.j.t.|.d...j...
-000003f0: 8301 6407 6403 6407 6408 9c03 8302 0100  ..d.d.d.d.......
-00000400: 6400 5300 2909 4e72 0700 0000 2901 da04  d.S.).Nr....)...
-00000410: 6e61 6d65 da05 4576 656e 7429 0272 1900  name..Event).r..
-00000420: 0000 da0d 746f 7572 6e61 6d65 6e74 5f69  ....tournament_i
-00000430: 647a 1853 454c 4543 5420 2a20 4652 4f4d  dz.SELECT * FROM
-00000440: 2022 6576 656e 7474 776f 2272 0100 0000   "eventtwo"r....
-00000450: e901 0000 0029 03da 0269 6472 1900 0000  .....)...idr....
-00000460: 721b 0000 0029 0c72 0700 0000 da06 6372  r....).r......cr
-00000470: 6561 7465 7205 0000 0072 1d00 0000 da0c  eater....r......
-00000480: 6173 7365 7274 5261 6973 6573 7204 0000  assertRaisesr...
-00000490: 0072 0f00 0000 da0d 6578 6563 7574 655f  .r......execute_
-000004a0: 7175 6572 7972 1000 0000 da0b 6173 7365  queryr......asse
-000004b0: 7274 4571 7561 6cda 0464 6963 74da 0569  rtEqual..dict..i
-000004c0: 7465 6d73 2903 7212 0000 00da 0a74 6f75  tems).r......tou
-000004d0: 726e 616d 656e 74da 0772 6573 756c 7473  rnament..results
-000004e0: 7213 0000 0072 1300 0000 7214 0000 00da  r....r....r.....
-000004f0: 1274 6573 745f 7477 6f5f 6461 7461 6261  .test_two_databa
-00000500: 7365 7318 0000 0073 0c00 0000 0001 1201  ses....s........
-00000510: 1602 0c01 1c02 1201 7a23 5465 7374 5477  ........z#TestTw
-00000520: 6f44 6174 6162 6173 6573 2e74 6573 745f  oDatabases.test_
-00000530: 7477 6f5f 6461 7461 6261 7365 7363 0100  two_databasesc..
-00000540: 0000 0000 0000 0700 0000 0d00 0000 c300  ................
-00000550: 0000 7378 0100 0074 006a 0164 0164 028d  ..sx...t.j.d.d..
-00000560: 0149 0064 0048 007d 0174 026a 0164 037c  .I.d.H.}.t.j.d.|
-00000570: 016a 0364 048d 0249 0064 0048 007d 027c  .j.d...I.d.H.}.|
-00000580: 006a 0474 0583 018f 1801 007c 006a 066a  .j.t.......|.j.j
-00000590: 0764 0583 0149 0064 0048 0001 0057 0064  .d...I.d.H...W.d
-000005a0: 0051 0052 0058 007c 006a 086a 0764 0583  .Q.R.X.|.j.j.d..
-000005b0: 0149 0064 0048 007d 037c 006a 0974 0a7c  .I.d.H.}.|.j.t.|
-000005c0: 0364 0619 006a 0b83 0083 0164 0764 0364  .d...j.....d.d.d
-000005d0: 0764 089c 0383 0201 0067 007d 0478 4874  .d.......g.}.xHt
-000005e0: 0c64 0983 0144 005d 3c7d 0574 0d6a 0164  .d...D.]<}.t.j.d
-000005f0: 0a6a 0e7c 0564 0717 0083 0164 028d 0149  .j.|.d.....d...I
-00000600: 0064 0048 007d 067c 046a 0f7c 0683 0101  .d.H.}.|.j.|....
-00000610: 007c 026a 106a 117c 0683 0149 0064 0048  .|.j.j.|...I.d.H
-00000620: 0001 0071 9057 007c 006a 0974 0d6a 1283  ...q.W.|.j.t.j..
-00000630: 006a 1364 0b83 0149 0064 0048 007c 0483  .j.d...I.d.H.|..
-00000640: 0201 007c 006a 097c 026a 106a 1283 006a  ...|.j.|.j.j...j
-00000650: 1364 0b83 0149 0064 0048 007c 0483 0201  .d...I.d.H.|....
-00000660: 007c 006a 0974 0d6a 1283 006a 1364 0b83  .|.j.t.j...j.d..
-00000670: 016a 1464 0c64 0b83 0249 0064 0048 0064  .j.d.d...I.d.H.d
-00000680: 0764 0d64 0e9c 0264 0964 0f64 0e9c 0267  .d.d...d.d.d...g
-00000690: 0283 0201 007c 006a 097c 026a 106a 1283  .....|.j.|.j.j..
-000006a0: 006a 1364 0b83 016a 1464 0c64 0b83 0249  .j.d...j.d.d...I
-000006b0: 0064 0048 0064 0764 0d64 0e9c 0264 0964  .d.H.d.d.d...d.d
-000006c0: 0f64 0e9c 0267 0283 0201 0064 0053 0029  .d...g.....d.S.)
-000006d0: 104e 7207 0000 0029 0172 1900 0000 721a  .Nr....).r....r.
-000006e0: 0000 0029 0272 1900 0000 721b 0000 007a  ...).r....r....z
-000006f0: 1853 454c 4543 5420 2a20 4652 4f4d 2022  .SELECT * FROM "
-00000700: 6576 656e 7474 776f 2272 0100 0000 721c  eventtwo"r....r.
-00000710: 0000 0029 0372 1d00 0000 7219 0000 0072  ...).r....r....r
-00000720: 1b00 0000 e902 0000 007a 0754 6561 6d20  .........z.Team 
-00000730: 7b7d 7219 0000 0072 1d00 0000 7a06 5465  {}r....r....z.Te
-00000740: 616d 2031 2902 721d 0000 0072 1900 0000  am 1).r....r....
-00000750: 7a06 5465 616d 2032 2915 7207 0000 0072  z.Team 2).r....r
-00000760: 1e00 0000 7205 0000 0072 1d00 0000 721f  ....r....r....r.
-00000770: 0000 0072 0400 0000 720f 0000 0072 2000  ...r....r....r .
-00000780: 0000 7210 0000 0072 2100 0000 7222 0000  ..r....r!...r"..
-00000790: 0072 2300 0000 da05 7261 6e67 6572 0600  .r#.....ranger..
-000007a0: 0000 da06 666f 726d 6174 da06 6170 7065  ....format..appe
-000007b0: 6e64 da0c 7061 7274 6963 6970 616e 7473  nd..participants
-000007c0: da03 6164 64da 0361 6c6c da08 6f72 6465  ..add..all..orde
-000007d0: 725f 6279 da06 7661 6c75 6573 2907 7212  r_by..values).r.
-000007e0: 0000 0072 2400 0000 da05 6576 656e 7472  ...r$.....eventr
-000007f0: 2500 0000 da05 7465 616d 73da 0169 da04  %.....teams..i..
-00000800: 7465 616d 7213 0000 0072 1300 0000 7214  teamr....r....r.
-00000810: 0000 00da 1b74 6573 745f 7477 6f5f 6461  .....test_two_da
-00000820: 7461 6261 7365 735f 7265 6c61 7469 6f6e  tabases_relation
-00000830: 2200 0000 7326 0000 0000 0112 0116 020c  "...s&..........
-00000840: 011c 0212 0120 0204 010e 011c 010a 0116  ..... ..........
-00000850: 021c 011e 0204 011a 0116 0204 011c 017a  ...............z
-00000860: 2c54 6573 7454 776f 4461 7461 6261 7365  ,TestTwoDatabase
-00000870: 732e 7465 7374 5f74 776f 5f64 6174 6162  s.test_two_datab
-00000880: 6173 6573 5f72 656c 6174 696f 6e4e 2907  ases_relationN).
-00000890: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
-000008a0: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
-000008b0: 6d65 5f5f 7215 0000 0072 1800 0000 7226  me__r....r....r&
-000008c0: 0000 0072 3400 0000 7213 0000 0072 1300  ...r4...r....r..
-000008d0: 0000 7213 0000 0072 1400 0000 7209 0000  ..r....r....r...
-000008e0: 0008 0000 0073 0800 0000 0801 080b 0804  .....s..........
-000008f0: 080a 7209 0000 004e 290d da08 746f 7274  ..r....N)...tort
-00000900: 6f69 7365 7202 0000 00da 1574 6f72 746f  oiser......torto
-00000910: 6973 652e 636f 6e74 7269 622e 7465 7374  ise.contrib.test
-00000920: 7203 0000 00da 1374 6f72 746f 6973 652e  r......tortoise.
-00000930: 6578 6365 7074 696f 6e73 7204 0000 00da  exceptionsr.....
-00000940: 1974 6f72 746f 6973 652e 7465 7374 732e  .tortoise.tests.
-00000950: 7465 7374 6d6f 6465 6c73 7205 0000 0072  testmodelsr....r
-00000960: 0600 0000 7207 0000 00da 0e74 6f72 746f  ....r......torto
-00000970: 6973 652e 7574 696c 7372 0800 0000 7209  ise.utilsr....r.
-00000980: 0000 0072 1300 0000 7213 0000 0072 1300  ...r....r....r..
-00000990: 0000 7214 0000 00da 083c 6d6f 6475 6c65  ..r......<module
-000009a0: 3e01 0000 0073 0a00 0000 0c01 0c01 0c01  >....s..........
-000009b0: 1401 0c03                                ....
+00000050: 6d07 5a07 6d08 5a08 0100 6400 6405 6c09  m.Z.m.Z...d.d.l.
+00000060: 6d0a 5a0a 0100 6400 6406 6c0b 6d0c 5a0c  m.Z...d.d.l.m.Z.
+00000070: 6d0d 5a0d 6d0e 5a0e 6d0f 5a0f 0100 6400  m.Z.m.Z.m.Z...d.
+00000080: 6407 6c10 6d11 5a11 0100 4700 6408 6409  d.l.m.Z...G.d.d.
+00000090: 8400 6409 6507 8303 5a12 640a 5300 290b  ..d.e...Z.d.S.).
+000000a0: e900 0000 0029 01da 0854 6f72 746f 6973  .....)...Tortois
+000000b0: 6529 01da 1667 6574 5f63 6f6e 6669 675f  e)...get_config_
+000000c0: 6672 6f6d 5f64 625f 7572 6c29 01da 0e69  from_db_url)...i
+000000d0: 6e5f 7472 616e 7361 6374 696f 6e29 02da  n_transaction)..
+000000e0: 0854 6573 7443 6173 65da 1054 4f52 544f  .TestCase..TORTO
+000000f0: 4953 455f 5445 5354 5f44 4229 01da 104f  ISE_TEST_DB)...O
+00000100: 7065 7261 7469 6f6e 616c 4572 726f 7229  perationalError)
+00000110: 04da 0845 7665 6e74 5477 6fda 0754 6561  ...EventTwo..Tea
+00000120: 6d54 776f da0a 546f 7572 6e61 6d65 6e74  mTwo..Tournament
+00000130: da05 4576 656e 7429 01da 1a67 656e 6572  ..Event)...gener
+00000140: 6174 655f 7363 6865 6d61 5f66 6f72 5f63  ate_schema_for_c
+00000150: 6c69 656e 7463 0000 0000 0000 0000 0000  lientc..........
+00000160: 0000 0200 0000 4000 0000 732c 0000 0065  ......@...s,...e
+00000170: 005a 0164 005a 0264 0164 0284 005a 0364  .Z.d.Z.d.d...Z.d
+00000180: 0364 0484 005a 0464 0564 0684 005a 0564  .d...Z.d.d...Z.d
+00000190: 0764 0884 005a 0664 0953 0029 0ada 1054  .d...Z.d.S.)...T
+000001a0: 6573 7454 776f 4461 7461 6261 7365 7363  estTwoDatabasesc
+000001b0: 0100 0000 0000 0000 0400 0000 0500 0000  ................
+000001c0: c300 0000 738c 0000 0074 006a 0172 147c  ....s....t.j.r.|
+000001d0: 006a 0283 0049 0064 0048 0001 0074 0374  .j...I.d.H...t.t
+000001e0: 0464 0164 0264 038d 037d 0174 0374 0464  .d.d.d...}.t.t.d
+000001f0: 0164 0464 038d 037d 027c 0164 0519 007c  .d.d...}.|.d...|
+00000200: 0264 0519 0096 027c 0164 0619 007c 0264  .d.....|.d...|.d
+00000210: 0619 0096 0264 079c 027d 0374 006a 057c  .....d...}.t.j.|
+00000220: 0383 0149 0064 0048 0001 0074 006a 0683  ...I.d.H...t.j..
+00000230: 0049 0064 0048 0001 0074 006a 0764 0283  .I.d.H...t.j.d..
+00000240: 017c 005f 0874 006a 0764 0483 017c 005f  .|._.t.j.d...|._
+00000250: 0964 0053 0029 084e 54da 066d 6f64 656c  .d.S.).NT..model
+00000260: 7329 02da 0774 6573 7469 6e67 da09 6170  s)...testing..ap
+00000270: 705f 6c61 6265 6cda 0665 7665 6e74 73da  p_label..events.
+00000280: 0b63 6f6e 6e65 6374 696f 6e73 da04 6170  .connections..ap
+00000290: 7073 2902 7212 0000 0072 1300 0000 290a  ps).r....r....).
+000002a0: 7202 0000 00da 075f 696e 6974 6564 da0b  r......_inited..
+000002b0: 5f74 6561 7244 6f77 6e44 4272 0300 0000  _tearDownDBr....
+000002c0: 7206 0000 00da 0469 6e69 74da 1067 656e  r......init..gen
+000002d0: 6572 6174 655f 7363 6865 6d61 73da 0e67  erate_schemas..g
+000002e0: 6574 5f63 6f6e 6e65 6374 696f 6eda 0264  et_connection..d
+000002f0: 62da 0973 6563 6f6e 645f 6462 2904 da04  b..second_db)...
+00000300: 7365 6c66 5a0f 6669 7273 745f 6462 5f63  selfZ.first_db_c
+00000310: 6f6e 6669 675a 1073 6563 6f6e 645f 6462  onfigZ.second_db
+00000320: 5f63 6f6e 6669 675a 0d6d 6572 6765 645f  _configZ.merged_
+00000330: 636f 6e66 6967 a900 721c 0000 00fa 552f  config..r.....U/
+00000340: 5573 6572 732f 616e 6472 6579 626f 6e64  Users/andreybond
+00000350: 6172 2f50 7943 6861 726d 5072 6f6a 6563  ar/PyCharmProjec
+00000360: 7473 2f74 6f72 746f 6973 652d 6f72 6d2f  ts/tortoise-orm/
+00000370: 746f 7274 6f69 7365 2f74 6573 7473 2f74  tortoise/tests/t
+00000380: 6573 745f 7477 6f5f 6461 7461 6261 7365  est_two_database
+00000390: 732e 7079 da05 7365 7455 700b 0000 0073  s.py..setUp....s
+000003a0: 2000 0000 0001 0601 0e01 0201 0201 0201   ...............
+000003b0: 0802 0201 0201 0201 0803 0e01 1402 1001  ................
+000003c0: 0e01 0c01 7a16 5465 7374 5477 6f44 6174  ....z.TestTwoDat
+000003d0: 6162 6173 6573 2e73 6574 5570 6301 0000  abases.setUpc...
+000003e0: 0000 0000 0003 0000 000d 0000 00c3 0000  ................
+000003f0: 0073 8600 0000 7400 6a01 6401 6402 8d01  .s....t.j.d.d...
+00000400: 4900 6400 4800 7d01 7402 6a01 6403 7c01  I.d.H.}.t.j.d.|.
+00000410: 6a03 6404 8d02 4900 6400 4800 0100 7c00  j.d...I.d.H...|.
+00000420: 6a04 7405 8301 8f18 0100 7c00 6a06 6a07  j.t.......|.j.j.
+00000430: 6405 8301 4900 6400 4800 0100 5700 6400  d...I.d.H...W.d.
+00000440: 5100 5200 5800 7c00 6a08 6a07 6405 8301  Q.R.X.|.j.j.d...
+00000450: 4900 6400 4800 7d02 7c00 6a09 740a 7c02  I.d.H.}.|.j.t.|.
+00000460: 6406 1900 6a0b 8300 8301 6407 6403 6407  d...j.....d.d.d.
+00000470: 6408 9c03 8302 0100 6400 5300 2909 4e72  d.......d.S.).Nr
+00000480: 0a00 0000 2901 da04 6e61 6d65 720b 0000  ....)...namer...
+00000490: 0029 0272 1f00 0000 da0d 746f 7572 6e61  .).r......tourna
+000004a0: 6d65 6e74 5f69 647a 1853 454c 4543 5420  ment_idz.SELECT 
+000004b0: 2a20 4652 4f4d 2022 6576 656e 7474 776f  * FROM "eventtwo
+000004c0: 2272 0100 0000 e901 0000 0029 03da 0269  "r.........)...i
+000004d0: 6472 1f00 0000 7220 0000 0029 0c72 0a00  dr....r ...).r..
+000004e0: 0000 da06 6372 6561 7465 7208 0000 0072  ....creater....r
+000004f0: 2200 0000 da0c 6173 7365 7274 5261 6973  ".....assertRais
+00000500: 6573 7207 0000 0072 1900 0000 da0d 6578  esr....r......ex
+00000510: 6563 7574 655f 7175 6572 7972 1a00 0000  ecute_queryr....
+00000520: da0b 6173 7365 7274 4571 7561 6cda 0464  ..assertEqual..d
+00000530: 6963 74da 0569 7465 6d73 2903 721b 0000  ict..items).r...
+00000540: 00da 0a74 6f75 726e 616d 656e 74da 0772  ...tournament..r
+00000550: 6573 756c 7473 721c 0000 0072 1c00 0000  esultsr....r....
+00000560: 721d 0000 00da 1274 6573 745f 7477 6f5f  r......test_two_
+00000570: 6461 7461 6261 7365 7321 0000 0073 0c00  databases!...s..
+00000580: 0000 0001 1201 1602 0c01 1c02 1201 7a23  ..............z#
+00000590: 5465 7374 5477 6f44 6174 6162 6173 6573  TestTwoDatabases
+000005a0: 2e74 6573 745f 7477 6f5f 6461 7461 6261  .test_two_databa
+000005b0: 7365 7363 0100 0000 0000 0000 0700 0000  sesc............
+000005c0: 0d00 0000 c300 0000 7378 0100 0074 006a  ........sx...t.j
+000005d0: 0164 0164 028d 0149 0064 0048 007d 0174  .d.d...I.d.H.}.t
+000005e0: 026a 0164 037c 016a 0364 048d 0249 0064  .j.d.|.j.d...I.d
+000005f0: 0048 007d 027c 006a 0474 0583 018f 1801  .H.}.|.j.t......
+00000600: 007c 006a 066a 0764 0583 0149 0064 0048  .|.j.j.d...I.d.H
+00000610: 0001 0057 0064 0051 0052 0058 007c 006a  ...W.d.Q.R.X.|.j
+00000620: 086a 0764 0583 0149 0064 0048 007d 037c  .j.d...I.d.H.}.|
+00000630: 006a 0974 0a7c 0364 0619 006a 0b83 0083  .j.t.|.d...j....
+00000640: 0164 0764 0364 0764 089c 0383 0201 0067  .d.d.d.d.......g
+00000650: 007d 0478 4874 0c64 0983 0144 005d 3c7d  .}.xHt.d...D.]<}
+00000660: 0574 0d6a 0164 0a6a 0e7c 0564 0717 0083  .t.j.d.j.|.d....
+00000670: 0164 028d 0149 0064 0048 007d 067c 046a  .d...I.d.H.}.|.j
+00000680: 0f7c 0683 0101 007c 026a 106a 117c 0683  .|.....|.j.j.|..
+00000690: 0149 0064 0048 0001 0071 9057 007c 006a  .I.d.H...q.W.|.j
+000006a0: 0974 0d6a 1283 006a 1364 0b83 0149 0064  .t.j...j.d...I.d
+000006b0: 0048 007c 0483 0201 007c 006a 097c 026a  .H.|.....|.j.|.j
+000006c0: 106a 1283 006a 1364 0b83 0149 0064 0048  .j...j.d...I.d.H
+000006d0: 007c 0483 0201 007c 006a 0974 0d6a 1283  .|.....|.j.t.j..
+000006e0: 006a 1364 0b83 016a 1464 0c64 0b83 0249  .j.d...j.d.d...I
+000006f0: 0064 0048 0064 0764 0d64 0e9c 0264 0964  .d.H.d.d.d...d.d
+00000700: 0f64 0e9c 0267 0283 0201 007c 006a 097c  .d...g.....|.j.|
+00000710: 026a 106a 1283 006a 1364 0b83 016a 1464  .j.j...j.d...j.d
+00000720: 0c64 0b83 0249 0064 0048 0064 0764 0d64  .d...I.d.H.d.d.d
+00000730: 0e9c 0264 0964 0f64 0e9c 0267 0283 0201  ...d.d.d...g....
+00000740: 0064 0053 0029 104e 720a 0000 0029 0172  .d.S.).Nr....).r
+00000750: 1f00 0000 720b 0000 0029 0272 1f00 0000  ....r....).r....
+00000760: 7220 0000 007a 1853 454c 4543 5420 2a20  r ...z.SELECT * 
+00000770: 4652 4f4d 2022 6576 656e 7474 776f 2272  FROM "eventtwo"r
+00000780: 0100 0000 7221 0000 0029 0372 2200 0000  ....r!...).r"...
+00000790: 721f 0000 0072 2000 0000 e902 0000 007a  r....r ........z
+000007a0: 0754 6561 6d20 7b7d 721f 0000 0072 2200  .Team {}r....r".
+000007b0: 0000 7a06 5465 616d 2031 2902 7222 0000  ..z.Team 1).r"..
+000007c0: 0072 1f00 0000 7a06 5465 616d 2032 2915  .r....z.Team 2).
+000007d0: 720a 0000 0072 2300 0000 7208 0000 0072  r....r#...r....r
+000007e0: 2200 0000 7224 0000 0072 0700 0000 7219  "...r$...r....r.
+000007f0: 0000 0072 2500 0000 721a 0000 0072 2600  ...r%...r....r&.
+00000800: 0000 7227 0000 0072 2800 0000 da05 7261  ..r'...r(.....ra
+00000810: 6e67 6572 0900 0000 da06 666f 726d 6174  nger......format
+00000820: da06 6170 7065 6e64 da0c 7061 7274 6963  ..append..partic
+00000830: 6970 616e 7473 da03 6164 64da 0361 6c6c  ipants..add..all
+00000840: da08 6f72 6465 725f 6279 da06 7661 6c75  ..order_by..valu
+00000850: 6573 2907 721b 0000 0072 2900 0000 da05  es).r....r).....
+00000860: 6576 656e 7472 2a00 0000 da05 7465 616d  eventr*.....team
+00000870: 73da 0169 da04 7465 616d 721c 0000 0072  s..i..teamr....r
+00000880: 1c00 0000 721d 0000 00da 1b74 6573 745f  ....r......test_
+00000890: 7477 6f5f 6461 7461 6261 7365 735f 7265  two_databases_re
+000008a0: 6c61 7469 6f6e 2b00 0000 7326 0000 0000  lation+...s&....
+000008b0: 0112 0116 020c 011c 0212 0120 0204 010e  ........... ....
+000008c0: 011c 010a 0116 021c 011e 0204 011a 0116  ................
+000008d0: 0204 011c 017a 2c54 6573 7454 776f 4461  .....z,TestTwoDa
+000008e0: 7461 6261 7365 732e 7465 7374 5f74 776f  tabases.test_two
+000008f0: 5f64 6174 6162 6173 6573 5f72 656c 6174  _databases_relat
+00000900: 696f 6e63 0100 0000 0000 0000 0600 0000  ionc............
+00000910: 1200 0000 c300 0000 73f6 0000 0074 0064  ........s....t.d
+00000920: 0183 0134 0049 0064 0048 009a 8801 0074  ...4.I.d.H.....t
+00000930: 016a 0264 0264 038d 0149 0064 0048 007d  .j.d.d...I.d.H.}
+00000940: 0174 036a 0264 047c 0164 058d 0249 0064  .t.j.d.|.d...I.d
+00000950: 0048 0001 0074 0064 0683 0134 0049 0064  .H...t.d...4.I.d
+00000960: 0048 009a 4001 0074 046a 0264 077c 016a  .H..@..t.j.d.|.j
+00000970: 0564 088d 0249 0064 0048 007d 0274 066a  .d...I.d.H.}.t.j
+00000980: 0264 0964 038d 0149 0064 0048 007d 037c  .d.d...I.d.H.}.|
+00000990: 026a 076a 087c 0383 0149 0064 0048 0001  .j.j.|...I.d.H..
+000009a0: 0057 0064 0051 0049 0064 0048 0052 0058  .W.d.Q.I.d.H.R.X
+000009b0: 0057 0064 0051 0049 0064 0048 0052 0058  .W.d.Q.I.d.H.R.X
+000009c0: 0074 016a 0964 0264 038d 016a 0a83 0049  .t.j.d.d...j...I
+000009d0: 0064 0048 007d 047c 006a 0b7c 016a 057c  .d.H.}.|.j.|.j.|
+000009e0: 046a 0583 0201 0074 046a 097c 016a 0564  .j.....t.j.|.j.d
+000009f0: 0a8d 016a 0a83 0049 0064 0048 007d 057c  ...j...I.d.H.}.|
+00000a00: 006a 0b7c 026a 057c 056a 0583 0201 0064  .j.|.j.|.j.....d
+00000a10: 0053 0029 0b4e 720e 0000 0072 0a00 0000  .S.).Nr....r....
+00000a20: 2901 721f 0000 005a 0645 7665 6e74 3129  ).r....Z.Event1)
+00000a30: 0272 1f00 0000 7229 0000 0072 1100 0000  .r....r)...r....
+00000a40: 5a06 4576 656e 7432 2902 721f 0000 0072  Z.Event2).r....r
+00000a50: 2000 0000 7a06 5465 616d 2031 2901 7220   ...z.Team 1).r 
+00000a60: 0000 0029 0c72 0400 0000 720a 0000 0072  ...).r....r....r
+00000a70: 2300 0000 720b 0000 0072 0800 0000 7222  #...r....r....r"
+00000a80: 0000 0072 0900 0000 7230 0000 0072 3100  ...r....r0...r1.
+00000a90: 0000 da06 6669 6c74 6572 da05 6669 7273  ....filter..firs
+00000aa0: 7472 2600 0000 2906 721b 0000 0072 2900  tr&...).r....r).
+00000ab0: 0000 7235 0000 0072 3800 0000 da10 7361  ..r5...r8.....sa
+00000ac0: 7665 645f 746f 7572 6e61 6d65 6e74 da0b  ved_tournament..
+00000ad0: 7361 7665 645f 6576 656e 7472 1c00 0000  saved_eventr....
+00000ae0: 721c 0000 0072 1d00 0000 da29 7465 7374  r....r.....)test
+00000af0: 5f74 776f 5f64 6174 6162 6173 6573 5f74  _two_databases_t
+00000b00: 7261 6e73 6163 7469 6f6e 735f 7377 6974  ransactions_swit
+00000b10: 6368 5f64 6247 0000 0073 1600 0000 0001  ch_dbG...s......
+00000b20: 1201 1201 1401 1201 1601 1201 3202 1601  ............2...
+00000b30: 1001 1801 7a3a 5465 7374 5477 6f44 6174  ....z:TestTwoDat
+00000b40: 6162 6173 6573 2e74 6573 745f 7477 6f5f  abases.test_two_
+00000b50: 6461 7461 6261 7365 735f 7472 616e 7361  databases_transa
+00000b60: 6374 696f 6e73 5f73 7769 7463 685f 6462  ctions_switch_db
+00000b70: 4e29 07da 085f 5f6e 616d 655f 5fda 0a5f  N)...__name__.._
+00000b80: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
+00000b90: 6c6e 616d 655f 5f72 1e00 0000 722b 0000  lname__r....r+..
+00000ba0: 0072 3900 0000 723e 0000 0072 1c00 0000  .r9...r>...r....
+00000bb0: 721c 0000 0072 1c00 0000 721d 0000 0072  r....r....r....r
+00000bc0: 0d00 0000 0a00 0000 7308 0000 0008 0108  ........s.......
+00000bd0: 1608 0a08 1c72 0d00 0000 4e29 13da 0874  .....r....N)...t
+00000be0: 6f72 746f 6973 6572 0200 0000 da1d 746f  ortoiser......to
+00000bf0: 7274 6f69 7365 2e62 6163 6b65 6e64 732e  rtoise.backends.
+00000c00: 6261 7365 2e64 625f 7572 6c72 0300 0000  base.db_urlr....
+00000c10: da10 746f 7274 6f69 7365 2e63 6f6e 7465  ..tortoise.conte
+00000c20: 7874 7204 0000 00da 1574 6f72 746f 6973  xtr......tortois
+00000c30: 652e 636f 6e74 7269 622e 7465 7374 7205  e.contrib.testr.
+00000c40: 0000 0072 0600 0000 da13 746f 7274 6f69  ...r......tortoi
+00000c50: 7365 2e65 7863 6570 7469 6f6e 7372 0700  se.exceptionsr..
+00000c60: 0000 da19 746f 7274 6f69 7365 2e74 6573  ....tortoise.tes
+00000c70: 7473 2e74 6573 746d 6f64 656c 7372 0800  ts.testmodelsr..
+00000c80: 0000 7209 0000 0072 0a00 0000 720b 0000  ..r....r....r...
+00000c90: 00da 0e74 6f72 746f 6973 652e 7574 696c  ...tortoise.util
+00000ca0: 7372 0c00 0000 720d 0000 0072 1c00 0000  sr....r....r....
+00000cb0: 721c 0000 0072 1c00 0000 721d 0000 00da  r....r....r.....
+00000cc0: 083c 6d6f 6475 6c65 3e01 0000 0073 0e00  .<module>....s..
+00000cd0: 0000 0c01 0c01 0c01 1001 0c01 1801 0c03  ................
```

### Comparing `tortoise-orm-0.9.2/tortoise/tests/__pycache__/test_basic.cpython-36.pyc` & `tortoise-orm-0.9.4/tortoise/tests/__pycache__/test_basic.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `tortoise-orm-0.9.2/tortoise/tests/__pycache__/test_filtering.cpython-36.pyc` & `tortoise-orm-0.9.4/tortoise/tests/__pycache__/test_filtering.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `tortoise-orm-0.9.2/tortoise/tests/__pycache__/testmodels.cpython-36.pyc` & `tortoise-orm-0.9.4/tortoise/tests/__pycache__/testmodels.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `tortoise-orm-0.9.2/tortoise/tests/test_transactions.py` & `tortoise-orm-0.9.4/tortoise/tests/test_transactions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from tortoise.contrib.test import TestCase
+from tortoise.contrib import test
 from tortoise.exceptions import OperationalError
 from tortoise.tests.testmodels import Tournament
 
 
-class TestTransactions(TestCase):
+class TestTransactions(test.TransactionTestCase):
 
     async def test_transactions(self):
         with self.assertRaises(OperationalError):
             async with self.db.in_transaction() as connection:
                 event = Tournament(name='Test')
                 await event.save(using_db=connection)
                 await Tournament.filter(id=event.id).using_db(
```

### Comparing `tortoise-orm-0.9.2/tortoise/tests/test_fields.py` & `tortoise-orm-0.9.4/tortoise/tests/test_fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-import unittest
 from datetime import date, datetime, timedelta
 from decimal import Decimal
 from time import sleep
 
 from tortoise import fields
-from tortoise.contrib.test import TestCase
+from tortoise.contrib import test
 from tortoise.exceptions import ConfigurationError, IntegrityError
 from tortoise.tests import testmodels
 
 
-class TestFieldErrors(unittest.TestCase):
+class TestFieldErrors(test.SimpleTestCase):
 
     def test_char_field_empty(self):
         with self.assertRaises(ConfigurationError):
             fields.CharField()
 
     def test_char_field_zero(self):
         with self.assertRaises(ConfigurationError):
@@ -32,15 +31,15 @@
             fields.DecimalField(max_digits=2, decimal_places=-1)
 
     def test_datetime_field_auto_bad(self):
         with self.assertRaises(ConfigurationError):
             fields.DatetimeField(auto_now=True, auto_now_add=True)
 
 
-class TestIntFields(TestCase):
+class TestIntFields(test.TransactionTestCase):
     async def test_empty(self):
         with self.assertRaises(IntegrityError):
             await testmodels.IntFields.create()
 
     async def test_create(self):
         obj0 = await testmodels.IntFields.create(intnum=1)
         obj = await testmodels.IntFields.get(id=obj0.id)
@@ -62,15 +61,15 @@
 
     async def test_values_list(self):
         obj0 = await testmodels.IntFields.create(intnum=1)
         values = await testmodels.IntFields.get(id=obj0.id).values_list('intnum', flat=True)
         self.assertEqual(values[0], 1)
 
 
-class TestSmallIntFields(TestCase):
+class TestSmallIntFields(test.TransactionTestCase):
     async def test_empty(self):
         with self.assertRaises(IntegrityError):
             await testmodels.SmallIntFields.create()
 
     async def test_create(self):
         obj0 = await testmodels.SmallIntFields.create(smallintnum=2)
         obj = await testmodels.SmallIntFields.get(id=obj0.id)
@@ -88,15 +87,15 @@
     async def test_values_list(self):
         obj0 = await testmodels.SmallIntFields.create(smallintnum=2)
         values = await testmodels.SmallIntFields.get(
             id=obj0.id).values_list('smallintnum', flat=True)
         self.assertEqual(values[0], 2)
 
 
-class TestCharFields(TestCase):
+class TestCharFields(test.TransactionTestCase):
     async def test_empty(self):
         with self.assertRaises(IntegrityError):
             await testmodels.CharFields.create()
 
     async def test_create(self):
         obj0 = await testmodels.CharFields.create(char='moo')
         obj = await testmodels.CharFields.get(id=obj0.id)
@@ -118,15 +117,15 @@
 
     async def test_values_list(self):
         obj0 = await testmodels.CharFields.create(char='moo')
         values = await testmodels.CharFields.get(id=obj0.id).values_list('char', flat=True)
         self.assertEqual(values[0], 'moo')
 
 
-class TestTextFields(TestCase):
+class TestTextFields(test.TransactionTestCase):
     async def test_empty(self):
         with self.assertRaises(IntegrityError):
             await testmodels.TextFields.create()
 
     async def test_create(self):
         obj0 = await testmodels.TextFields.create(text='baa')
         obj = await testmodels.TextFields.get(id=obj0.id)
@@ -143,15 +142,15 @@
 
     async def test_values_list(self):
         obj0 = await testmodels.TextFields.create(text='baa')
         values = await testmodels.TextFields.get(id=obj0.id).values_list('text', flat=True)
         self.assertEqual(values[0], 'baa')
 
 
-class TestBooleanFields(TestCase):
+class TestBooleanFields(test.TransactionTestCase):
     async def test_empty(self):
         with self.assertRaises(IntegrityError):
             await testmodels.BooleanFields.create()
 
     async def test_create(self):
         obj0 = await testmodels.BooleanFields.create(boolean=True)
         obj = await testmodels.BooleanFields.get(id=obj0.id)
@@ -168,15 +167,15 @@
 
     async def test_values_list(self):
         obj0 = await testmodels.BooleanFields.create(boolean=True)
         values = await testmodels.BooleanFields.get(id=obj0.id).values_list('boolean', flat=True)
         self.assertEqual(values[0], True)
 
 
-class TestDecimalFields(TestCase):
+class TestDecimalFields(test.TransactionTestCase):
     async def test_empty(self):
         with self.assertRaises(IntegrityError):
             await testmodels.DecimalFields.create()
 
     async def test_create(self):
         obj0 = await testmodels.DecimalFields.create(decimal=Decimal('1.23456'), decimal_nodec=18.7)
         obj = await testmodels.DecimalFields.get(id=obj0.id)
@@ -196,15 +195,15 @@
     async def test_values_list(self):
         obj0 = await testmodels.DecimalFields.create(decimal=Decimal('1.23456'), decimal_nodec=18.7)
         values = await testmodels.DecimalFields.get(
             id=obj0.id).values_list('decimal', 'decimal_nodec')
         self.assertEqual(list(values[0]), [Decimal('1.2346'), 19])
 
 
-class TestDatetimeFields(TestCase):
+class TestDatetimeFields(test.TransactionTestCase):
     async def test_empty(self):
         with self.assertRaises(IntegrityError):
             await testmodels.DatetimeFields.create()
 
     async def test_create(self):
         now = datetime.utcnow()
         obj0 = await testmodels.DatetimeFields.create(datetime=now)
@@ -240,15 +239,15 @@
     async def test_values_list(self):
         now = datetime.utcnow()
         obj0 = await testmodels.DatetimeFields.create(datetime=now)
         values = await testmodels.DatetimeFields.get(id=obj0.id).values_list('datetime', flat=True)
         self.assertEqual(values[0], now)
 
 
-class TestDateFields(TestCase):
+class TestDateFields(test.TransactionTestCase):
     async def test_empty(self):
         with self.assertRaises(IntegrityError):
             await testmodels.DateFields.create()
 
     async def test_create(self):
         today = date.today()
         obj0 = await testmodels.DateFields.create(date=today)
@@ -274,15 +273,15 @@
     async def test_values_list(self):
         today = date.today()
         obj0 = await testmodels.DateFields.create(date=today)
         values = await testmodels.DateFields.get(id=obj0.id).values_list('date', flat=True)
         self.assertEqual(values[0], today)
 
 
-class TestFloatFields(TestCase):
+class TestFloatFields(test.TransactionTestCase):
     async def test_empty(self):
         with self.assertRaises(IntegrityError):
             await testmodels.FloatFields.create()
 
     async def test_create(self):
         obj0 = await testmodels.FloatFields.create(floatnum=1.23)
         obj = await testmodels.FloatFields.get(id=obj0.id)
@@ -310,15 +309,15 @@
 
     async def test_values_list(self):
         obj0 = await testmodels.FloatFields.create(floatnum=1.23)
         values = await testmodels.FloatFields.filter(id=obj0.id).values_list('floatnum')
         self.assertEqual(list(values[0]), [1.23])
 
 
-class TestJSONFields(TestCase):
+class TestJSONFields(test.TransactionTestCase):
     async def test_empty(self):
         with self.assertRaises(IntegrityError):
             await testmodels.JSONFields.create()
 
     async def test_create(self):
         obj0 = await testmodels.JSONFields.create(data={'some': ['text', 3]})
         obj = await testmodels.JSONFields.get(id=obj0.id)
```

### Comparing `tortoise-orm-0.9.2/tortoise/tests/testmodels.py` & `tortoise-orm-0.9.4/tortoise/tests/testmodels.py`

 * *Files 9% similar despite different names*

```diff
@@ -127,7 +127,21 @@
     floatnum_null = fields.FloatField(null=True)
 
 
 class JSONFields(Model):
     id = fields.IntField(pk=True)
     data = fields.JSONField()
     data_null = fields.JSONField(null=True)
+
+
+# TODO: Test that minimaly specified relations work as expected
+class MinRelation(Model):
+    id = fields.IntField(pk=True)
+    tournament = fields.ForeignKeyField('models.Tournament')
+    participants = fields.ManyToManyField(
+        'models.Team'
+    )
+
+
+# TODO: Test that no id models work as expected
+class NoID(Model):
+    char = fields.CharField(max_length=255, null=True)
```

### Comparing `tortoise-orm-0.9.2/tortoise/tests/test_two_databases.py` & `tortoise-orm-0.9.4/tortoise/tests/test_two_databases.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 from tortoise import Tortoise
-from tortoise.contrib.test import TestCase
+from tortoise.contrib import test
 from tortoise.exceptions import OperationalError
 from tortoise.tests.testmodels import EventTwo, TeamTwo, Tournament
 from tortoise.utils import generate_schema
 
 
-class TestTwoDatabases(TestCase):
+class TestTwoDatabases(test.SimpleTestCase):
     async def setUp(self):
-        await self._tearDownDB()
         self.db = await self.getDB()
         self.second_db = await self.getDB()
         Tortoise._client_routing(db_routing={
             'models': self.db,
             'events': self.second_db,
         })
+
+        if not Tortoise._inited:
+            Tortoise._init_relations()
+
         await generate_schema(self.db)
         await generate_schema(self.second_db)
 
     async def tearDown(self):
+        await self.db.close()
+        await self.db.db_delete()
         await self.second_db.close()
         await self.second_db.db_delete()
 
     async def test_two_databases(self):
         tournament = await Tournament.create(name='Tournament')
         await EventTwo.create(name='Event', tournament_id=tournament.id)
```

### Comparing `tortoise-orm-0.9.2/tortoise/tests/test_prefetching.py` & `tortoise-orm-0.9.4/tortoise/tests/test_prefetching.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from tortoise.contrib.test import TestCase
+from tortoise.contrib import test
 from tortoise.query_utils import Prefetch
 from tortoise.tests.testmodels import Event, Tournament
 
 
-class TestPrefetching(TestCase):
+class TestPrefetching(test.TestCase):
     async def test_prefetching(self):
         tournament = await Tournament.create(name='tournament')
         await Event.create(name='First', tournament=tournament)
         await Event.create(name='Second', tournament=tournament)
         tournament_with_filtered = await Tournament.all().prefetch_related(
             Prefetch('events', queryset=Event.filter(name='First'))
         ).first()
```

### Comparing `tortoise-orm-0.9.2/tortoise/tests/test_relations.py` & `tortoise-orm-0.9.4/tortoise/tests/test_relations.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from tortoise.contrib.test import TestCase
+from tortoise.contrib import test
 from tortoise.tests.testmodels import Event, Team, Tournament
 
 
-class TestRelations(TestCase):
+class TestRelations(test.TestCase):
     async def test_relations(self):
         tournament = Tournament(name='New Tournament')
         await tournament.save()
         await Event(name='Without participants', tournament_id=tournament.id).save()
         event = Event(name='Test', tournament_id=tournament.id)
         await event.save()
         participants = []
```

### Comparing `tortoise-orm-0.9.2/tortoise/tests/test_filtering.py` & `tortoise-orm-0.9.4/tortoise/tests/test_filtering.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from tortoise.contrib.test import TestCase
+from tortoise.contrib import test
 from tortoise.query_utils import Q
 from tortoise.tests.testmodels import Event, Team, Tournament
 
 
-class TestFiltering(TestCase):
+class TestFiltering(test.TestCase):
     async def test_filtering(self):
         tournament = Tournament(name='Tournament')
         await tournament.save()
 
         second_tournament = Tournament(name='Tournament 2')
         await second_tournament.save()
```

### Comparing `tortoise-orm-0.9.2/tortoise/__init__.py` & `tortoise-orm-0.9.4/tortoise/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,86 +1,87 @@
 from tortoise import fields
 from tortoise.backends.base.client import BaseDBAsyncClient
-from tortoise.exceptions import ConfigurationError, MultiplyObjectsReturned  # noqa
-from tortoise.fields import ManyToManyRelationManager  # noqa
+from tortoise.exceptions import ConfigurationError
 from tortoise.models import get_backward_fk_filters, get_m2m_filters
-from tortoise.queryset import QuerySet  # noqa
 
 
 class Tortoise:
     apps = {}  # type: dict
     _inited = False
     _db_routing = None
     _global_connection = None
 
     @classmethod
     def register_model(cls, app, name, model):
         if app not in cls.apps:
             cls.apps[app] = {}
-        assert name not in cls.apps[app], '{} duplicates in {}'.format(name, app)
+        if name in cls.apps[app]:
+            raise ConfigurationError('{} duplicates in {}'.format(name, app))
         cls.apps[app][name] = model
 
     @classmethod
     def _set_connection_routing(cls, db_routing):
-        assert set(db_routing.keys()) == set(cls.apps.keys()), (
-            'No db instanced for apps: {}'
-            .format(", ".join(set(db_routing.keys()) ^ set(cls.apps.keys())))
-        )
+        if set(db_routing.keys()) != set(cls.apps.keys()):
+            raise ConfigurationError('No db instanced for apps: {}'.format(
+                ", ".join(set(db_routing.keys()) ^ set(cls.apps.keys()))))
         for app, client in db_routing.items():
             for model in cls.apps[app].values():
                 model._meta.db = client
 
     @classmethod
     def _set_global_connection(cls, db_client):
         for app in cls.apps.values():
             for model in app.values():
                 model._meta.db = db_client
 
     @classmethod
     def _client_routing(cls, global_client=None, db_routing=None):
-        assert bool(global_client) != bool(db_routing), (
-            'You must pass either global connection or routing'
-        )
+        if global_client and db_routing:
+            raise ConfigurationError('You must pass either global_client or db_routing')
         if global_client:
-            assert isinstance(global_client, BaseDBAsyncClient)
+            if not isinstance(global_client, BaseDBAsyncClient):
+                raise ConfigurationError('global_client must inherit from BaseDBAsyncClient')
             cls._set_global_connection(global_client)
-        else:
-            assert all(isinstance(c, BaseDBAsyncClient) for c in db_routing.values())
+        elif db_routing:
+            if not all(isinstance(c, BaseDBAsyncClient) for c in db_routing.values()):
+                raise ConfigurationError('All app values must inherit from BaseDBAsyncClient')
             cls._set_connection_routing(db_routing)
+        else:
+            raise ConfigurationError('You must pass either global_client or db_routing')
 
     @classmethod
     def _init_relations(cls):
+        cls._inited = True
         for app_name, app in cls.apps.items():
             for model_name, model in app.items():
                 if not model._meta.table:
                     model._meta.table = model.__name__.lower()
 
                 for field in model._meta.fk_fields:
                     field_object = model._meta.fields_map[field]
                     reference = field_object.model_name
                     related_app_name, related_model_name = reference.split('.')
                     related_model = cls.apps[related_app_name][related_model_name]
                     field_object.type = related_model
                     backward_relation_name = field_object.related_name
                     if not backward_relation_name:
                         backward_relation_name = '{}s'.format(model._meta.table)
-                    assert backward_relation_name not in related_model._meta.fields, (
-                        'backward relation "{}" duplicates in model {}'.format(
-                            backward_relation_name, related_model_name
-                        )
-                    )
-                    relation = fields.BackwardFKRelation(model, '{}_id'.format(field))
-                    setattr(related_model, backward_relation_name, relation)
+                    if backward_relation_name in related_model._meta.fields:
+                        raise ConfigurationError(
+                            'backward relation "{}" duplicates in model {}'.format(
+                                backward_relation_name, related_model_name))
+                    fk_relation = fields.BackwardFKRelation(model, '{}_id'.format(field))
+                    setattr(related_model, backward_relation_name, fk_relation)
                     related_model._meta.filters.update(
-                        get_backward_fk_filters(backward_relation_name, relation)
+                        get_backward_fk_filters(backward_relation_name, fk_relation)
                     )
 
                     related_model._meta.backward_fk_fields.add(backward_relation_name)
                     related_model._meta.fetch_fields.add(backward_relation_name)
-                    related_model._meta.fields_map[backward_relation_name] = relation
+                    related_model._meta.fields_map[backward_relation_name] = fk_relation
                     related_model._meta.fields.add(backward_relation_name)
 
                 for field in model._meta.m2m_fields:
                     field_object = model._meta.fields_map[field]
                     if field_object._generated:
                         continue
 
@@ -94,57 +95,55 @@
                     related_model = cls.apps[related_app_name][related_model_name]
 
                     field_object.type = related_model
 
                     backward_relation_name = field_object.related_name
                     if not backward_relation_name:
                         backward_relation_name = '{}s'.format(model._meta.table)
-                    assert backward_relation_name not in related_model._meta.fields, (
-                        'backward relation "{}" duplicates in model {}'.format(
-                            backward_relation_name, related_model_name
-                        )
-                    )
+                    if backward_relation_name in related_model._meta.fields:
+                        raise ConfigurationError(
+                            'backward relation "{}" duplicates in model {}'.format(
+                                backward_relation_name, related_model_name))
 
                     if not field_object.through:
                         related_model_table_name = (
                             related_model._meta.table
                             if related_model._meta.table else related_model.__name__.lower()
                         )
 
                         field_object.through = '{}_{}'.format(
                             model._meta.table,
                             related_model_table_name,
                         )
 
-                    relation = fields.ManyToManyField(
+                    m2m_relation = fields.ManyToManyField(
                         '{}.{}'.format(app_name, model_name),
                         field_object.through,
                         forward_key=field_object.backward_key,
                         backward_key=field_object.forward_key,
                         related_name=field,
                         type=model
                     )
-                    relation._generated = True
+                    m2m_relation._generated = True
                     setattr(
                         related_model,
                         backward_relation_name,
-                        relation,
+                        m2m_relation,
                     )
                     model._meta.filters.update(get_m2m_filters(field, field_object))
                     related_model._meta.filters.update(
-                        get_m2m_filters(backward_relation_name, relation)
+                        get_m2m_filters(backward_relation_name, m2m_relation)
                     )
                     related_model._meta.m2m_fields.add(backward_relation_name)
                     related_model._meta.fetch_fields.add(backward_relation_name)
-                    related_model._meta.fields_map[backward_relation_name] = relation
+                    related_model._meta.fields_map[backward_relation_name] = m2m_relation
                     related_model._meta.fields.add(backward_relation_name)
 
     @classmethod
     def init(cls, global_client=None, db_routing=None):
         if cls._inited:
             raise ConfigurationError('Already initialised')
         cls._client_routing(global_client=global_client, db_routing=db_routing)
         cls._init_relations()
-        cls._inited = True
 
 
-__version__ = "0.9.2"
+__version__ = "0.9.4"
```

### Comparing `tortoise-orm-0.9.2/tortoise/__pycache__/query_utils.cpython-36.pyc` & `tortoise-orm-0.9.4/tortoise/__pycache__/query_utils.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.6 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 16% similar despite different names*

```diff
@@ -1,262 +1,277 @@
-00000000: 330d 0d0a 5707 365b c015 0000 e300 0000  3...W.6[........
+00000000: 330d 0d0a dc7e 445b 2517 0000 e300 0000  3....~D[%.......
 00000010: 0000 0000 0000 0000 0003 0000 0040 0000  .............@..
-00000020: 0073 3800 0000 6400 6401 6c00 6d01 5a01  .s8...d.d.l.m.Z.
-00000030: 0100 6400 6402 6c02 6d03 5a03 0100 4700  ..d.d.l.m.Z...G.
-00000040: 6403 6404 8400 6404 8302 5a04 4700 6405  d.d...d...Z.G.d.
-00000050: 6406 8400 6406 8302 5a05 6407 5300 2908  d...d...Z.d.S.).
-00000060: e900 0000 0029 01da 0554 6162 6c65 2901  .....)...Table).
-00000070: da06 6669 656c 6473 6300 0000 0000 0000  ..fieldsc.......
-00000080: 0000 0000 0003 0000 0040 0000 0073 5a00  .........@...sZ.
-00000090: 0000 6500 5a01 6400 5a02 6401 5a03 6402  ..e.Z.d.Z.d.Z.d.
-000000a0: 5a04 6503 6403 9c01 6404 6405 8402 5a05  Z.e.d...d.d...Z.
-000000b0: 6406 6407 8400 5a06 6408 6409 8400 5a07  d.d...Z.d.d...Z.
-000000c0: 640a 640b 8400 5a08 640c 640d 8400 5a09  d.d...Z.d.d...Z.
-000000d0: 640e 640f 8400 5a0a 6410 6411 8400 5a0b  d.d...Z.d.d...Z.
-000000e0: 6412 6413 8400 5a0c 6414 5300 2915 da01  d.d...Z.d.S.)...
-000000f0: 51da 0341 4e44 da02 4f52 2901 da09 6a6f  Q..AND..OR)...jo
-00000100: 696e 5f74 7970 6563 0100 0000 0100 0000  in_typec........
-00000110: 0400 0000 0300 0000 4f00 0000 735a 0000  ........O...sZ..
-00000120: 0074 007c 0283 016f 0e74 007c 0383 010c  .t.|...o.t.|....
-00000130: 0073 1a74 0164 0183 0182 0174 0264 0264  .s.t.d.....t.d.d
-00000140: 0384 007c 0244 0083 0183 0173 3074 0182  ...|.D.....s0t..
-00000150: 017c 027c 005f 037c 037c 005f 047c 017c  .|.|._.|.|._.|.|
-00000160: 006a 057c 006a 0668 026b 0673 5074 0182  .j.|.j.h.k.sPt..
-00000170: 017c 017c 005f 0764 0053 0029 044e 7a38  .|.|._.d.S.).Nz8
-00000180: 796f 7520 6361 6e20 7061 7373 206f 6e6c  you can pass onl
-00000190: 7920 5120 6e6f 6465 7320 6f72 2066 696c  y Q nodes or fil
-000001a0: 7465 7220 6b77 6172 6773 2069 6e20 6f6e  ter kwargs in on
-000001b0: 6520 5120 6e6f 6465 6301 0000 0000 0000  e Q nodec.......
-000001c0: 0002 0000 0004 0000 0073 0000 0073 1800  .........s...s..
-000001d0: 0000 7c00 5d10 7d01 7400 7c01 7401 8302  ..|.].}.t.|.t...
-000001e0: 5600 0100 7102 6400 5300 2901 4e29 02da  V...q.d.S.).N)..
-000001f0: 0a69 7369 6e73 7461 6e63 6572 0400 0000  .isinstancer....
-00000200: 2902 da02 2e30 da04 6e6f 6465 a900 720b  )....0..node..r.
-00000210: 0000 00fa 192e 2f74 6f72 746f 6973 652f  ....../tortoise/
-00000220: 7175 6572 795f 7574 696c 732e 7079 fa09  query_utils.py..
-00000230: 3c67 656e 6578 7072 3e0d 0000 0073 0200  <genexpr>....s..
-00000240: 0000 0400 7a1d 512e 5f5f 696e 6974 5f5f  ....z.Q.__init__
-00000250: 2e3c 6c6f 6361 6c73 3e2e 3c67 656e 6578  .<locals>.<genex
-00000260: 7072 3e29 08da 0462 6f6f 6cda 0e41 7373  pr>)...bool..Ass
-00000270: 6572 7469 6f6e 4572 726f 72da 0361 6c6c  ertionError..all
-00000280: da08 6368 696c 6472 656e da07 6669 6c74  ..children..filt
-00000290: 6572 7372 0500 0000 7206 0000 0072 0700  ersr....r....r..
-000002a0: 0000 2904 da04 7365 6c66 7207 0000 00da  ..)...selfr.....
-000002b0: 0461 7267 73da 066b 7761 7267 7372 0b00  .args..kwargsr..
-000002c0: 0000 720b 0000 0072 0c00 0000 da08 5f5f  ..r....r......__
-000002d0: 696e 6974 5f5f 0a00 0000 730e 0000 0000  init__....s.....
-000002e0: 0108 0112 0116 0106 0106 0114 017a 0a51  .............z.Q
-000002f0: 2e5f 5f69 6e69 745f 5f63 0200 0000 0000  .__init__c......
-00000300: 0000 0200 0000 0500 0000 4300 0000 731e  ..........C...s.
-00000310: 0000 0074 007c 0174 0183 0273 0e74 0282  ...t.|.t...s.t..
-00000320: 0174 017c 007c 017c 006a 0364 018d 0353  .t.|.|.|.j.d...S
-00000330: 0029 024e 2901 7207 0000 0029 0472 0800  .).N).r....).r..
-00000340: 0000 7204 0000 0072 0f00 0000 7205 0000  ..r....r....r...
-00000350: 0029 0272 1300 0000 da05 6f74 6865 7272  .).r......otherr
-00000360: 0b00 0000 720b 0000 0072 0c00 0000 da07  ....r....r......
-00000370: 5f5f 616e 645f 5f13 0000 0073 0400 0000  __and__....s....
-00000380: 0001 0e01 7a09 512e 5f5f 616e 645f 5f63  ....z.Q.__and__c
-00000390: 0200 0000 0000 0000 0200 0000 0500 0000  ................
-000003a0: 4300 0000 731e 0000 0074 007c 0174 0183  C...s....t.|.t..
-000003b0: 0273 0e74 0282 0174 017c 007c 017c 006a  .s.t...t.|.|.|.j
-000003c0: 0364 018d 0353 0029 024e 2901 7207 0000  .d...S.).N).r...
-000003d0: 0029 0472 0800 0000 7204 0000 0072 0f00  .).r....r....r..
-000003e0: 0000 7206 0000 0029 0272 1300 0000 7217  ..r....).r....r.
-000003f0: 0000 0072 0b00 0000 720b 0000 0072 0c00  ...r....r....r..
-00000400: 0000 da06 5f5f 6f72 5f5f 1700 0000 7304  ....__or__....s.
-00000410: 0000 0000 010e 017a 0851 2e5f 5f6f 725f  .......z.Q.__or_
-00000420: 5f63 0400 0000 0000 0000 0600 0000 0600  _c..............
-00000430: 0000 4300 0000 7344 0000 007c 0264 0119  ..C...sD...|.d..
-00000440: 007c 016a 0074 017c 0264 0119 007c 0264  .|.j.t.|.d...|.d
-00000450: 0219 0083 026b 0266 027d 047c 0264 0319  .....k.f.}.|.d..
-00000460: 0074 017c 0264 0119 007c 0264 0419 0083  .t.|.d...|.d....
-00000470: 027c 0383 027d 057c 057c 0466 0253 0029  .|...}.|.|.f.S.)
-00000480: 054e da05 7461 626c 65da 0c62 6163 6b77  .N..table..backw
-00000490: 6172 645f 6b65 79da 086f 7065 7261 746f  ard_key..operato
-000004a0: 72da 0566 6965 6c64 2902 da02 6964 da07  r..field)...id..
-000004b0: 6765 7461 7474 7229 0672 1300 0000 721a  getattr).r....r.
-000004c0: 0000 00da 0570 6172 616d da05 7661 6c75  .....param..valu
-000004d0: 65da 046a 6f69 6eda 0963 7269 7465 7269  e..join..criteri
-000004e0: 6f6e 720b 0000 0072 0b00 0000 720c 0000  onr....r....r...
-000004f0: 00da 175f 6765 745f 6672 6f6d 5f72 656c  ..._get_from_rel
-00000500: 6174 6564 5f74 6162 6c65 1b00 0000 7306  ated_table....s.
-00000510: 0000 0000 0120 011c 017a 1951 2e5f 6765  ..... ...z.Q._ge
-00000520: 745f 6672 6f6d 5f72 656c 6174 6564 5f74  t_from_related_t
-00000530: 6162 6c65 6304 0000 0000 0000 000c 0000  ablec...........
-00000540: 0007 0000 0043 0000 0073 2c01 0000 7400  .....C...s,...t.
-00000550: 7c01 6a01 6a02 8301 7d04 6700 7d05 7c02  |.j.j...}.g.}.|.
-00000560: 6a03 6401 8301 6402 1900 7d06 7c01 6a01  j.d...d...}.|.j.
-00000570: 6a04 7c06 1900 7d07 7405 7c07 7406 6a07  j.|...}.t.|.t.j.
-00000580: 8302 7288 7400 7c07 6a08 6a01 6a02 8301  ..r.t.|.j.j.j...
-00000590: 7d08 7400 7c07 6a09 8301 7d09 7c05 6a0a  }.t.|.j...}.|.j.
-000005a0: 7c09 7c04 6a0b 740c 7c09 7c07 6a0d 8302  |.|.j.t.|.|.j...
-000005b0: 6b02 6602 8301 0100 7c05 6a0a 7c08 740c  k.f.....|.j.|.t.
-000005c0: 7c09 7c07 6a0e 8302 7c08 6a0b 6b02 6602  |.|.j...|.j.k.f.
-000005d0: 8301 0100 6e66 7405 7c07 7406 6a0f 8302  ....nft.|.t.j...
-000005e0: 72c0 7400 7c07 6a08 6a01 6a02 8301 7d08  r.t.|.j.j.j...}.
-000005f0: 7c05 6a0a 7c08 7c04 6a0b 740c 7c08 7c07  |.j.|.|.j.t.|.|.
-00000600: 6a10 8302 6b02 6602 8301 0100 6e2e 7400  j...k.f.....n.t.
-00000610: 7c07 6a08 6a01 6a02 8301 7d08 7c05 6a0a  |.j.j.j...}.|.j.
-00000620: 7c08 7c08 6a0b 740c 7c04 6403 6a11 7c06  |.|.j.t.|.d.j.|.
-00000630: 8301 8302 6b02 6602 8301 0100 7412 6600  ....k.f.....t.f.
-00000640: 6401 6a13 7c02 6a03 6401 8301 6404 6400  d.j.|.j.d...d.d.
-00000650: 8502 1900 8301 7c03 6901 8e01 6a14 7c07  ......|.i...j.|.
-00000660: 6a08 8301 5c02 7d0a 7d0b 7c05 7c0b 3700  j...\.}.}.|.|.7.
-00000670: 7d05 7c0a 7c05 6602 5300 2905 4eda 025f  }.|.|.f.S.).N.._
-00000680: 5f72 0100 0000 7a05 7b7d 5f69 64e9 0100  _r....z.{}_id...
-00000690: 0000 2915 7202 0000 00da 055f 6d65 7461  ..).r......_meta
-000006a0: 721a 0000 00da 0573 706c 6974 da0a 6669  r......split..fi
-000006b0: 656c 6473 5f6d 6170 7208 0000 0072 0300  elds_mapr....r..
-000006c0: 0000 da0f 4d61 6e79 546f 4d61 6e79 4669  ....ManyToManyFi
-000006d0: 656c 64da 0474 7970 65da 0774 6872 6f75  eld..type..throu
-000006e0: 6768 da06 6170 7065 6e64 721e 0000 0072  gh..appendr....r
-000006f0: 1f00 0000 721b 0000 00da 0b66 6f72 7761  ....r......forwa
-00000700: 7264 5f6b 6579 da12 4261 636b 7761 7264  rd_key..Backward
-00000710: 464b 5265 6c61 7469 6f6e da0e 7265 6c61  FKRelation..rela
-00000720: 7469 6f6e 5f66 6965 6c64 da06 666f 726d  tion_field..form
-00000730: 6174 7204 0000 0072 2200 0000 da11 7265  atr....r".....re
-00000740: 736f 6c76 655f 666f 725f 6d6f 6465 6c29  solve_for_model)
-00000750: 0c72 1300 0000 da05 6d6f 6465 6cda 036b  .r......model..k
-00000760: 6579 7221 0000 0072 1a00 0000 da0e 7265  eyr!...r......re
-00000770: 7175 6972 6564 5f6a 6f69 6e73 da12 7265  quired_joins..re
-00000780: 6c61 7465 645f 6669 656c 645f 6e61 6d65  lated_field_name
-00000790: da0d 7265 6c61 7465 645f 6669 656c 64da  ..related_field.
-000007a0: 0d72 656c 6174 6564 5f74 6162 6c65 da0d  .related_table..
-000007b0: 7468 726f 7567 685f 7461 626c 65da 0d6e  through_table..n
-000007c0: 6577 5f63 7269 7465 7269 6f6e da09 6e65  ew_criterion..ne
-000007d0: 775f 6a6f 696e 7372 0b00 0000 720b 0000  w_joinsr....r...
-000007e0: 0072 0c00 0000 da16 5f72 6573 6f6c 7665  .r......_resolve
-000007f0: 5f6e 6573 7465 645f 6669 6c74 6572 2000  _nested_filter .
-00000800: 0000 732e 0000 0000 010c 0104 010e 010c  ..s.............
-00000810: 010c 010e 010a 0104 0118 0204 011a 020c  ................
-00000820: 010e 0104 011a 030e 0104 0102 011a 0322  ..............."
-00000830: 010c 0308 017a 1851 2e5f 7265 736f 6c76  .....z.Q._resolv
-00000840: 655f 6e65 7374 6564 5f66 696c 7465 7263  e_nested_filterc
-00000850: 0200 0000 0000 0000 0d00 0000 0600 0000  ................
-00000860: 4300 0000 7318 0100 0064 007d 0274 007c  C...s....d.}.t.|
-00000870: 016a 016a 0283 017d 0367 007d 0478 fa7c  .j.j...}.g.}.x.|
-00000880: 006a 036a 0483 0044 005d ec5c 027d 057d  .j.j...D.].\.}.}
-00000890: 067c 057c 016a 016a 036b 0772 667c 056a  .|.|.j.j.k.rf|.j
-000008a0: 0564 0183 0164 0219 007c 016a 016a 066b  .d...d...|.j.j.k
-000008b0: 0672 667c 006a 077c 017c 057c 0683 035c  .rf|.j.|.|.|...\
-000008c0: 027d 077d 087c 047c 0837 007d 046e 7c7c  .}.}.|.|.7.}.n||
-000008d0: 016a 016a 037c 0519 007d 097c 096a 0864  .j.j.|...}.|.j.d
-000008e0: 0383 0172 9e7c 006a 097c 0964 0319 007c  ...r.|.j.|.d...|
-000008f0: 097c 0683 035c 027d 077d 0a7c 046a 0a7c  .|...\.}.}.|.j.|
-00000900: 0a83 0101 006e 447c 016a 016a 0b7c 0964  .....nD|.j.j.|.d
-00000910: 0419 0019 007d 0b7c 096a 0864 0583 0172  .....}.|.j.d...r
-00000920: c07c 0964 0519 006e 047c 0b6a 0c7d 0c7c  .|.d...n.|.j.}.|
-00000930: 0964 0619 0074 0d7c 037c 0964 0419 0083  .d...t.|.|.d....
-00000940: 027c 0c7c 0683 0183 027d 077c 0273 ec7c  .|.|.....}.|.s.|
-00000950: 077d 0271 207c 006a 0e7c 006a 0f6b 0290  .}.q |.j.|.j.k..
-00000960: 0172 047c 027c 074d 007d 0271 207c 027c  .r.|.|.M.}.q |.|
-00000970: 074f 007d 0271 2057 007c 027c 0466 0253  .O.}.q W.|.|.f.S
-00000980: 0029 074e 7225 0000 0072 0100 0000 721a  .).Nr%...r....r.
-00000990: 0000 0072 1d00 0000 da0d 7661 6c75 655f  ...r......value_
-000009a0: 656e 636f 6465 7272 1c00 0000 2910 7202  encoderr....).r.
-000009b0: 0000 0072 2700 0000 721a 0000 0072 1200  ...r'...r....r..
-000009c0: 0000 da05 6974 656d 7372 2800 0000 da0c  ....itemsr(.....
-000009d0: 6665 7463 685f 6669 656c 6473 723c 0000  fetch_fieldsr<..
-000009e0: 00da 0367 6574 7224 0000 0072 2d00 0000  ...getr$...r-...
-000009f0: 7229 0000 00da 0b74 6f5f 6462 5f76 616c  r).....to_db_val
-00000a00: 7565 721f 0000 0072 0700 0000 7205 0000  uer....r....r...
-00000a10: 0029 0d72 1300 0000 7233 0000 0072 2300  .).r....r3...r#.
-00000a20: 0000 721a 0000 0072 3500 0000 7234 0000  ..r....r5...r4..
-00000a30: 0072 2100 0000 723a 0000 0072 3b00 0000  .r!...r:...r;...
-00000a40: 7220 0000 0072 2200 0000 da0c 6669 656c  r ...r".....fiel
-00000a50: 645f 6f62 6a65 6374 723d 0000 0072 0b00  d_objectr=...r..
-00000a60: 0000 720b 0000 0072 0c00 0000 da0f 5f72  ..r....r......_r
-00000a70: 6573 6f6c 7665 5f6b 7761 7267 7341 0000  esolve_kwargsA..
-00000a80: 0073 2a00 0000 0001 0401 0c01 0401 1401  .s*.............
-00000a90: 2201 1201 0a02 0c01 0a01 1601 0c02 1003  "...............
-00000aa0: 1802 0601 1602 0401 0602 0e01 0a02 0c01  ................
-00000ab0: 7a11 512e 5f72 6573 6f6c 7665 5f6b 7761  z.Q._resolve_kwa
-00000ac0: 7267 7363 0200 0000 0000 0000 0700 0000  rgsc............
-00000ad0: 0300 0000 4300 0000 735e 0000 0064 007d  ....C...s^...d.}
-00000ae0: 0267 007d 0378 4c7c 006a 0044 005d 427d  .g.}.xL|.j.D.]B}
-00000af0: 047c 046a 017c 0183 015c 027d 057d 067c  .|.j.|...\.}.}.|
-00000b00: 037c 0637 007d 037c 0273 347c 057d 0271  .|.7.}.|.s4|.}.q
-00000b10: 107c 006a 027c 006a 036b 0272 4a7c 027c  .|.j.|.j.k.rJ|.|
-00000b20: 054d 007d 0271 107c 027c 054f 007d 0271  .M.}.q.|.|.O.}.q
-00000b30: 1057 007c 027c 0366 0253 0029 014e 2904  .W.|.|.f.S.).N).
-00000b40: 7211 0000 0072 3200 0000 7207 0000 0072  r....r2...r....r
-00000b50: 0500 0000 2907 7213 0000 0072 3300 0000  ....).r....r3...
-00000b60: 7223 0000 0072 3500 0000 720a 0000 0072  r#...r5...r....r
-00000b70: 3a00 0000 5a0e 6368 696c 6472 656e 5f6a  :...Z.children_j
-00000b80: 6f69 6e73 720b 0000 0072 0b00 0000 720c  oinsr....r....r.
-00000b90: 0000 00da 115f 7265 736f 6c76 655f 6368  ....._resolve_ch
-00000ba0: 696c 6472 656e 6000 0000 7316 0000 0000  ildren`...s.....
-00000bb0: 0104 0104 010c 010e 0108 0104 0106 020c  ................
-00000bc0: 010a 020c 017a 1351 2e5f 7265 736f 6c76  .....z.Q._resolv
-00000bd0: 655f 6368 696c 6472 656e 6302 0000 0000  e_childrenc.....
-00000be0: 0000 0002 0000 0002 0000 0043 0000 0073  ...........C...s
-00000bf0: 1e00 0000 7c00 6a00 7210 7c00 6a01 7c01  ....|.j.r.|.j.|.
-00000c00: 8301 5300 7c00 6a02 7c01 8301 5300 6400  ..S.|.j.|...S.d.
-00000c10: 5300 2901 4e29 0372 1200 0000 7243 0000  S.).N).r....rC..
-00000c20: 0072 4400 0000 2902 7213 0000 0072 3300  .rD...).r....r3.
-00000c30: 0000 720b 0000 0072 0b00 0000 720c 0000  ..r....r....r...
-00000c40: 0072 3200 0000 6f00 0000 7306 0000 0000  .r2...o...s.....
-00000c50: 0106 010a 027a 1351 2e72 6573 6f6c 7665  .....z.Q.resolve
-00000c60: 5f66 6f72 5f6d 6f64 656c 4e29 0dda 085f  _for_modelN)..._
-00000c70: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
-00000c80: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
-00000c90: 5f72 0500 0000 7206 0000 0072 1600 0000  _r....r....r....
-00000ca0: 7218 0000 0072 1900 0000 7224 0000 0072  r....r....r$...r
-00000cb0: 3c00 0000 7243 0000 0072 4400 0000 7232  <...rC...rD...r2
-00000cc0: 0000 0072 0b00 0000 720b 0000 0072 0b00  ...r....r....r..
-00000cd0: 0000 720c 0000 0072 0400 0000 0600 0000  ..r....r........
-00000ce0: 7314 0000 0008 0104 0104 020e 0908 0408  s...............
-00000cf0: 0408 0508 2108 1f08 0f72 0400 0000 6300  ....!....r....c.
-00000d00: 0000 0000 0000 0000 0000 0002 0000 0040  ...............@
-00000d10: 0000 0073 1c00 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
-00000d20: 6401 6402 8400 5a03 6403 6404 8400 5a04  d.d...Z.d.d...Z.
-00000d30: 6405 5300 2906 da08 5072 6566 6574 6368  d.S.)...Prefetch
-00000d40: 6303 0000 0000 0000 0003 0000 0002 0000  c...............
-00000d50: 0043 0000 0073 1000 0000 7c01 7c00 5f00  .C...s....|.|._.
-00000d60: 7c02 7c00 5f01 6400 5300 2901 4e29 02da  |.|._.d.S.).N)..
-00000d70: 0872 656c 6174 696f 6eda 0871 7565 7279  .relation..query
-00000d80: 7365 7429 0372 1300 0000 7249 0000 0072  set).r....rI...r
-00000d90: 4a00 0000 720b 0000 0072 0b00 0000 720c  J...r....r....r.
-00000da0: 0000 0072 1600 0000 7700 0000 7304 0000  ...r....w...s...
-00000db0: 0000 0106 017a 1150 7265 6665 7463 682e  .....z.Prefetch.
-00000dc0: 5f5f 696e 6974 5f5f 6302 0000 0000 0000  __init__c.......
-00000dd0: 0005 0000 0004 0000 0043 0000 0073 9200  .........C...s..
-00000de0: 0000 7c00 6a00 6a01 6401 8301 7d02 7c02  ..|.j.j.d...}.|.
-00000df0: 6402 1900 7d03 7c03 7c01 6a02 6a03 6a04  d...}.|.|.j.j.j.
-00000e00: 6b06 7338 7405 6403 6a06 7c03 7c01 6a02  k.s8t.d.j.|.|.j.
-00000e10: 6a03 6a07 8302 8301 8201 6401 6a08 7c02  j.j.......d.j.|.
-00000e20: 6404 6400 8502 1900 8301 7d04 7c04 7282  d.d.......}.|.r.
-00000e30: 7c03 7c01 6a09 6a0a 8300 6b07 7268 740b  |.|.j.j...k.rht.
-00000e40: 8300 7c01 6a09 7c03 3c00 7c01 6a09 7c03  ..|.j.|.<.|.j.|.
-00000e50: 1900 6a0c 740d 7c04 7c00 6a0e 8302 8301  ..j.t.|.|.j.....
-00000e60: 0100 6e0c 7c00 6a0e 7c01 6a0f 7c03 3c00  ..n.|.j.|.j.|.<.
-00000e70: 6400 5300 2905 4e72 2500 0000 7201 0000  d.S.).Nr%...r...
-00000e80: 007a 1c72 656c 6174 696f 6e20 7b7d 2066  .z.relation {} f
-00000e90: 6f72 207b 7d20 6e6f 7420 666f 756e 6472  or {} not foundr
-00000ea0: 2600 0000 2910 7249 0000 0072 2800 0000  &...).rI...r(...
-00000eb0: 7233 0000 0072 2700 0000 723f 0000 0072  r3...r'...r?...r
-00000ec0: 0f00 0000 7231 0000 0072 1a00 0000 7222  ....r1...r....r"
-00000ed0: 0000 00da 0d5f 7072 6566 6574 6368 5f6d  ....._prefetch_m
-00000ee0: 6170 da04 6b65 7973 da03 7365 74da 0361  ap..keys..set..a
-00000ef0: 6464 7248 0000 0072 4a00 0000 da11 5f70  ddrH...rJ....._p
-00000f00: 7265 6665 7463 685f 7175 6572 6965 7329  refetch_queries)
-00000f10: 0572 1300 0000 724a 0000 00da 0e72 656c  .r....rJ.....rel
-00000f20: 6174 696f 6e5f 7370 6c69 74da 1166 6972  ation_split..fir
-00000f30: 7374 5f6c 6576 656c 5f66 6965 6c64 da12  st_level_field..
-00000f40: 666f 7277 6172 6465 645f 7072 6566 6574  forwarded_prefet
-00000f50: 6368 720b 0000 0072 0b00 0000 720c 0000  chr....r....r...
-00000f60: 00da 1472 6573 6f6c 7665 5f66 6f72 5f71  ...resolve_for_q
-00000f70: 7565 7279 7365 747b 0000 0073 1600 0000  ueryset{...s....
-00000f80: 0001 0c01 0802 1001 1401 1201 0401 0e01  ................
-00000f90: 0c01 0a01 1003 7a1d 5072 6566 6574 6368  ......z.Prefetch
-00000fa0: 2e72 6573 6f6c 7665 5f66 6f72 5f71 7565  .resolve_for_que
-00000fb0: 7279 7365 744e 2905 7245 0000 0072 4600  rysetN).rE...rF.
-00000fc0: 0000 7247 0000 0072 1600 0000 7253 0000  ..rG...r....rS..
-00000fd0: 0072 0b00 0000 720b 0000 0072 0b00 0000  .r....r....r....
-00000fe0: 720c 0000 0072 4800 0000 7600 0000 7304  r....rH...v...s.
-00000ff0: 0000 0008 0108 0472 4800 0000 4e29 06da  .......rH...N)..
-00001000: 0670 7970 696b 6172 0200 0000 da08 746f  .pypikar......to
-00001010: 7274 6f69 7365 7203 0000 0072 0400 0000  rtoiser....r....
-00001020: 7248 0000 0072 0b00 0000 720b 0000 0072  rH...r....r....r
-00001030: 0b00 0000 720c 0000 00da 083c 6d6f 6475  ....r......<modu
-00001040: 6c65 3e01 0000 0073 0600 0000 0c02 0c03  le>....s........
-00001050: 0e70                                     .p
+00000020: 0073 4400 0000 6400 6401 6c00 6d01 5a01  .sD...d.d.l.m.Z.
+00000030: 0100 6400 6402 6c02 6d03 5a03 0100 6400  ..d.d.l.m.Z...d.
+00000040: 6403 6c04 6d05 5a05 0100 4700 6404 6405  d.l.m.Z...G.d.d.
+00000050: 8400 6405 8302 5a06 4700 6406 6407 8400  ..d...Z.G.d.d...
+00000060: 6407 8302 5a07 6408 5300 2909 e900 0000  d...Z.d.S.).....
+00000070: 0029 01da 0554 6162 6c65 2901 da06 6669  .)...Table)...fi
+00000080: 656c 6473 2901 da10 4f70 6572 6174 696f  elds)...Operatio
+00000090: 6e61 6c45 7272 6f72 6300 0000 0000 0000  nalErrorc.......
+000000a0: 0000 0000 0003 0000 0040 0000 0073 5a00  .........@...sZ.
+000000b0: 0000 6500 5a01 6400 5a02 6401 5a03 6402  ..e.Z.d.Z.d.Z.d.
+000000c0: 5a04 6503 6403 9c01 6404 6405 8402 5a05  Z.e.d...d.d...Z.
+000000d0: 6406 6407 8400 5a06 6408 6409 8400 5a07  d.d...Z.d.d...Z.
+000000e0: 640a 640b 8400 5a08 640c 640d 8400 5a09  d.d...Z.d.d...Z.
+000000f0: 640e 640f 8400 5a0a 6410 6411 8400 5a0b  d.d...Z.d.d...Z.
+00000100: 6412 6413 8400 5a0c 6414 5300 2915 da01  d.d...Z.d.S.)...
+00000110: 51da 0341 4e44 da02 4f52 2901 da09 6a6f  Q..AND..OR)...jo
+00000120: 696e 5f74 7970 6563 0100 0000 0100 0000  in_typec........
+00000130: 0400 0000 0300 0000 4f00 0000 7358 0000  ........O...sX..
+00000140: 007c 0272 107c 0372 1074 0064 0183 0182  .|.r.|.r.t.d....
+00000150: 0174 0164 0264 0384 007c 0244 0083 0183  .t.d.d...|.D....
+00000160: 0173 2a74 0064 0483 0182 017c 027c 005f  .s*t.d.....|.|._
+00000170: 027c 037c 005f 037c 017c 006a 047c 006a  .|.|._.|.|.j.|.j
+00000180: 0568 026b 0772 4e74 0064 0583 0182 017c  .h.k.rNt.d.....|
+00000190: 017c 005f 0664 0053 0029 064e 7a38 596f  .|._.d.S.).Nz8Yo
+000001a0: 7520 6361 6e20 7061 7373 206f 6e6c 7920  u can pass only 
+000001b0: 5120 6e6f 6465 7320 6f72 2066 696c 7465  Q nodes or filte
+000001c0: 7220 6b77 6172 6773 2069 6e20 6f6e 6520  r kwargs in one 
+000001d0: 5120 6e6f 6465 6301 0000 0000 0000 0002  Q nodec.........
+000001e0: 0000 0004 0000 0073 0000 0073 1800 0000  .......s...s....
+000001f0: 7c00 5d10 7d01 7400 7c01 7401 8302 5600  |.].}.t.|.t...V.
+00000200: 0100 7102 6400 5300 2901 4e29 02da 0a69  ..q.d.S.).N)...i
+00000210: 7369 6e73 7461 6e63 6572 0500 0000 2902  sinstancer....).
+00000220: da02 2e30 da04 6e6f 6465 a900 720c 0000  ...0..node..r...
+00000230: 00fa 482f 5573 6572 732f 616e 6472 6579  ..H/Users/andrey
+00000240: 626f 6e64 6172 2f50 7943 6861 726d 5072  bondar/PyCharmPr
+00000250: 6f6a 6563 7473 2f74 6f72 746f 6973 652d  ojects/tortoise-
+00000260: 6f72 6d2f 746f 7274 6f69 7365 2f71 7565  orm/tortoise/que
+00000270: 7279 5f75 7469 6c73 2e70 79fa 093c 6765  ry_utils.py..<ge
+00000280: 6e65 7870 723e 0e00 0000 7302 0000 0004  nexpr>....s.....
+00000290: 007a 1d51 2e5f 5f69 6e69 745f 5f2e 3c6c  .z.Q.__init__.<l
+000002a0: 6f63 616c 733e 2e3c 6765 6e65 7870 723e  ocals>.<genexpr>
+000002b0: 7a25 416c 6c20 6f72 6465 7265 6420 6172  z%All ordered ar
+000002c0: 6775 6d65 6e74 7320 6d75 7374 2062 6520  guments must be 
+000002d0: 5120 6e6f 6465 737a 1b6a 6f69 6e5f 7479  Q nodesz.join_ty
+000002e0: 7065 206d 7573 7420 6265 2041 4e44 206f  pe must be AND o
+000002f0: 7220 4f52 2907 7204 0000 00da 0361 6c6c  r OR).r......all
+00000300: da08 6368 696c 6472 656e da07 6669 6c74  ..children..filt
+00000310: 6572 7372 0600 0000 7207 0000 0072 0800  ersr....r....r..
+00000320: 0000 2904 da04 7365 6c66 7208 0000 00da  ..)...selfr.....
+00000330: 0461 7267 73da 066b 7761 7267 7372 0c00  .args..kwargsr..
+00000340: 0000 720c 0000 0072 0d00 0000 da08 5f5f  ..r....r......__
+00000350: 696e 6974 5f5f 0b00 0000 7312 0000 0000  init__....s.....
+00000360: 0108 0108 0112 0108 0106 0106 0110 0108  ................
+00000370: 017a 0a51 2e5f 5f69 6e69 745f 5f63 0200  .z.Q.__init__c..
+00000380: 0000 0000 0000 0200 0000 0500 0000 4300  ..............C.
+00000390: 0000 7322 0000 0074 007c 0174 0183 0273  ..s"...t.|.t...s
+000003a0: 1274 0264 0183 0182 0174 017c 007c 017c  .t.d.....t.|.|.|
+000003b0: 006a 0364 028d 0353 0029 034e 7a1f 414e  .j.d...S.).Nz.AN
+000003c0: 4420 6f70 6572 6174 696f 6e20 7265 7175  D operation requ
+000003d0: 6972 6573 2061 2051 206e 6f64 6529 0172  ires a Q node).r
+000003e0: 0800 0000 2904 7209 0000 0072 0500 0000  ....).r....r....
+000003f0: 7204 0000 0072 0600 0000 2902 7212 0000  r....r....).r...
+00000400: 00da 056f 7468 6572 720c 0000 0072 0c00  ...otherr....r..
+00000410: 0000 720d 0000 00da 075f 5f61 6e64 5f5f  ..r......__and__
+00000420: 1600 0000 7306 0000 0000 010a 0108 017a  ....s..........z
+00000430: 0951 2e5f 5f61 6e64 5f5f 6302 0000 0000  .Q.__and__c.....
+00000440: 0000 0002 0000 0005 0000 0043 0000 0073  ...........C...s
+00000450: 2200 0000 7400 7c01 7401 8302 7312 7402  "...t.|.t...s.t.
+00000460: 6401 8301 8201 7401 7c00 7c01 7c00 6a03  d.....t.|.|.|.j.
+00000470: 6402 8d03 5300 2903 4e7a 1e4f 5220 6f70  d...S.).Nz.OR op
+00000480: 6572 6174 696f 6e20 7265 7175 6972 6573  eration requires
+00000490: 2061 2051 206e 6f64 6529 0172 0800 0000   a Q node).r....
+000004a0: 2904 7209 0000 0072 0500 0000 7204 0000  ).r....r....r...
+000004b0: 0072 0700 0000 2902 7212 0000 0072 1600  .r....).r....r..
+000004c0: 0000 720c 0000 0072 0c00 0000 720d 0000  ..r....r....r...
+000004d0: 00da 065f 5f6f 725f 5f1b 0000 0073 0600  ...__or__....s..
+000004e0: 0000 0001 0a01 0801 7a08 512e 5f5f 6f72  ........z.Q.__or
+000004f0: 5f5f 6304 0000 0000 0000 0006 0000 0006  __c.............
+00000500: 0000 0043 0000 0073 4400 0000 7c02 6401  ...C...sD...|.d.
+00000510: 1900 7c01 6a00 7401 7c02 6401 1900 7c02  ..|.j.t.|.d...|.
+00000520: 6402 1900 8302 6b02 6602 7d04 7c02 6403  d.....k.f.}.|.d.
+00000530: 1900 7401 7c02 6401 1900 7c02 6404 1900  ..t.|.d...|.d...
+00000540: 8302 7c03 8302 7d05 7c05 7c04 6602 5300  ..|...}.|.|.f.S.
+00000550: 2905 4eda 0574 6162 6c65 da0c 6261 636b  ).N..table..back
+00000560: 7761 7264 5f6b 6579 da08 6f70 6572 6174  ward_key..operat
+00000570: 6f72 da05 6669 656c 6429 02da 0269 64da  or..field)...id.
+00000580: 0767 6574 6174 7472 2906 7212 0000 0072  .getattr).r....r
+00000590: 1900 0000 da05 7061 7261 6dda 0576 616c  ......param..val
+000005a0: 7565 da04 6a6f 696e da09 6372 6974 6572  ue..join..criter
+000005b0: 696f 6e72 0c00 0000 720c 0000 0072 0d00  ionr....r....r..
+000005c0: 0000 da17 5f67 6574 5f66 726f 6d5f 7265  ...._get_from_re
+000005d0: 6c61 7465 645f 7461 626c 6520 0000 0073  lated_table ...s
+000005e0: 0600 0000 0001 2001 1c01 7a19 512e 5f67  ...... ...z.Q._g
+000005f0: 6574 5f66 726f 6d5f 7265 6c61 7465 645f  et_from_related_
+00000600: 7461 626c 6563 0400 0000 0000 0000 0c00  tablec..........
+00000610: 0000 0700 0000 4300 0000 732c 0100 0074  ......C...s,...t
+00000620: 007c 016a 016a 0283 017d 0467 007d 057c  .|.j.j...}.g.}.|
+00000630: 026a 0364 0183 0164 0219 007d 067c 016a  .j.d...d...}.|.j
+00000640: 016a 047c 0619 007d 0774 057c 0774 066a  .j.|...}.t.|.t.j
+00000650: 0783 0272 8874 007c 076a 086a 016a 0283  ...r.t.|.j.j.j..
+00000660: 017d 0874 007c 076a 0983 017d 097c 056a  .}.t.|.j...}.|.j
+00000670: 0a7c 097c 046a 0b74 0c7c 097c 076a 0d83  .|.|.j.t.|.|.j..
+00000680: 026b 0266 0283 0101 007c 056a 0a7c 0874  .k.f.....|.j.|.t
+00000690: 0c7c 097c 076a 0e83 027c 086a 0b6b 0266  .|.|.j...|.j.k.f
+000006a0: 0283 0101 006e 6674 057c 0774 066a 0f83  .....nft.|.t.j..
+000006b0: 0272 c074 007c 076a 086a 016a 0283 017d  .r.t.|.j.j.j...}
+000006c0: 087c 056a 0a7c 087c 046a 0b74 0c7c 087c  .|.j.|.|.j.t.|.|
+000006d0: 076a 1083 026b 0266 0283 0101 006e 2e74  .j...k.f.....n.t
+000006e0: 007c 076a 086a 016a 0283 017d 087c 056a  .|.j.j.j...}.|.j
+000006f0: 0a7c 087c 086a 0b74 0c7c 0464 036a 117c  .|.|.j.t.|.d.j.|
+00000700: 0683 0183 026b 0266 0283 0101 0074 1266  .....k.f.....t.f
+00000710: 0064 016a 137c 026a 0364 0183 0164 0464  .d.j.|.j.d...d.d
+00000720: 0085 0219 0083 017c 0369 018e 016a 147c  .......|.i...j.|
+00000730: 076a 0883 015c 027d 0a7d 0b7c 057c 0b37  .j...\.}.}.|.|.7
+00000740: 007d 057c 0a7c 0566 0253 0029 054e da02  .}.|.|.f.S.).N..
+00000750: 5f5f 7201 0000 007a 057b 7d5f 6964 e901  __r....z.{}_id..
+00000760: 0000 0029 1572 0200 0000 da05 5f6d 6574  ...).r......_met
+00000770: 6172 1900 0000 da05 7370 6c69 74da 0a66  ar......split..f
+00000780: 6965 6c64 735f 6d61 7072 0900 0000 7203  ields_mapr....r.
+00000790: 0000 00da 0f4d 616e 7954 6f4d 616e 7946  .....ManyToManyF
+000007a0: 6965 6c64 da04 7479 7065 da07 7468 726f  ield..type..thro
+000007b0: 7567 68da 0661 7070 656e 6472 1d00 0000  ugh..appendr....
+000007c0: 721e 0000 0072 1a00 0000 da0b 666f 7277  r....r......forw
+000007d0: 6172 645f 6b65 79da 1242 6163 6b77 6172  ard_key..Backwar
+000007e0: 6446 4b52 656c 6174 696f 6eda 0e72 656c  dFKRelation..rel
+000007f0: 6174 696f 6e5f 6669 656c 64da 0666 6f72  ation_field..for
+00000800: 6d61 7472 0500 0000 7221 0000 00da 1172  matr....r!.....r
+00000810: 6573 6f6c 7665 5f66 6f72 5f6d 6f64 656c  esolve_for_model
+00000820: 290c 7212 0000 00da 056d 6f64 656c da03  ).r......model..
+00000830: 6b65 7972 2000 0000 7219 0000 00da 0e72  keyr ...r......r
+00000840: 6571 7569 7265 645f 6a6f 696e 73da 1272  equired_joins..r
+00000850: 656c 6174 6564 5f66 6965 6c64 5f6e 616d  elated_field_nam
+00000860: 65da 0d72 656c 6174 6564 5f66 6965 6c64  e..related_field
+00000870: da0d 7265 6c61 7465 645f 7461 626c 65da  ..related_table.
+00000880: 0d74 6872 6f75 6768 5f74 6162 6c65 da0d  .through_table..
+00000890: 6e65 775f 6372 6974 6572 696f 6eda 096e  new_criterion..n
+000008a0: 6577 5f6a 6f69 6e73 720c 0000 0072 0c00  ew_joinsr....r..
+000008b0: 0000 720d 0000 00da 165f 7265 736f 6c76  ..r......_resolv
+000008c0: 655f 6e65 7374 6564 5f66 696c 7465 7225  e_nested_filter%
+000008d0: 0000 0073 2e00 0000 0001 0c01 0401 0e01  ...s............
+000008e0: 0c01 0c01 0e01 0a01 0401 1802 0401 1a02  ................
+000008f0: 0c01 0e01 0401 1a03 0e01 0401 0201 1a03  ................
+00000900: 2201 0c03 0801 7a18 512e 5f72 6573 6f6c  ".....z.Q._resol
+00000910: 7665 5f6e 6573 7465 645f 6669 6c74 6572  ve_nested_filter
+00000920: 6302 0000 0000 0000 000d 0000 0006 0000  c...............
+00000930: 0043 0000 0073 1801 0000 6400 7d02 7400  .C...s....d.}.t.
+00000940: 7c01 6a01 6a02 8301 7d03 6700 7d04 78fa  |.j.j...}.g.}.x.
+00000950: 7c00 6a03 6a04 8300 4400 5dec 5c02 7d05  |.j.j...D.].\.}.
+00000960: 7d06 7c05 7c01 6a01 6a03 6b07 7266 7c05  }.|.|.j.j.k.rf|.
+00000970: 6a05 6401 8301 6402 1900 7c01 6a01 6a06  j.d...d...|.j.j.
+00000980: 6b06 7266 7c00 6a07 7c01 7c05 7c06 8303  k.rf|.j.|.|.|...
+00000990: 5c02 7d07 7d08 7c04 7c08 3700 7d04 6e7c  \.}.}.|.|.7.}.n|
+000009a0: 7c01 6a01 6a03 7c05 1900 7d09 7c09 6a08  |.j.j.|...}.|.j.
+000009b0: 6403 8301 729e 7c00 6a09 7c09 6403 1900  d...r.|.j.|.d...
+000009c0: 7c09 7c06 8303 5c02 7d07 7d0a 7c04 6a0a  |.|...\.}.}.|.j.
+000009d0: 7c0a 8301 0100 6e44 7c01 6a01 6a0b 7c09  |.....nD|.j.j.|.
+000009e0: 6404 1900 1900 7d0b 7c09 6a08 6405 8301  d.....}.|.j.d...
+000009f0: 72c0 7c09 6405 1900 6e04 7c0b 6a0c 7d0c  r.|.d...n.|.j.}.
+00000a00: 7c09 6406 1900 740d 7c03 7c09 6404 1900  |.d...t.|.|.d...
+00000a10: 8302 7c0c 7c06 8301 8302 7d07 7c02 73ec  ..|.|.....}.|.s.
+00000a20: 7c07 7d02 7120 7c00 6a0e 7c00 6a0f 6b02  |.}.q |.j.|.j.k.
+00000a30: 9001 7204 7c02 7c07 4d00 7d02 7120 7c02  ..r.|.|.M.}.q |.
+00000a40: 7c07 4f00 7d02 7120 5700 7c02 7c04 6602  |.O.}.q W.|.|.f.
+00000a50: 5300 2907 4e72 2400 0000 7201 0000 0072  S.).Nr$...r....r
+00000a60: 1900 0000 721c 0000 00da 0d76 616c 7565  ....r......value
+00000a70: 5f65 6e63 6f64 6572 721b 0000 0029 1072  _encoderr....).r
+00000a80: 0200 0000 7226 0000 0072 1900 0000 7211  ....r&...r....r.
+00000a90: 0000 00da 0569 7465 6d73 7227 0000 00da  .....itemsr'....
+00000aa0: 0c66 6574 6368 5f66 6965 6c64 7372 3b00  .fetch_fieldsr;.
+00000ab0: 0000 da03 6765 7472 2300 0000 722c 0000  ....getr#...r,..
+00000ac0: 0072 2800 0000 da0b 746f 5f64 625f 7661  .r(.....to_db_va
+00000ad0: 6c75 6572 1e00 0000 7208 0000 0072 0600  luer....r....r..
+00000ae0: 0000 290d 7212 0000 0072 3200 0000 7222  ..).r....r2...r"
+00000af0: 0000 0072 1900 0000 7234 0000 0072 3300  ...r....r4...r3.
+00000b00: 0000 7220 0000 0072 3900 0000 723a 0000  ..r ...r9...r:..
+00000b10: 0072 1f00 0000 7221 0000 00da 0c66 6965  .r....r!.....fie
+00000b20: 6c64 5f6f 626a 6563 7472 3c00 0000 720c  ld_objectr<...r.
+00000b30: 0000 0072 0c00 0000 720d 0000 00da 0f5f  ...r....r......_
+00000b40: 7265 736f 6c76 655f 6b77 6172 6773 4600  resolve_kwargsF.
+00000b50: 0000 732a 0000 0000 0104 010c 0104 0114  ..s*............
+00000b60: 0122 0112 010a 020c 010a 0116 010c 0210  ."..............
+00000b70: 0318 0206 0116 0204 0106 020e 010a 020c  ................
+00000b80: 017a 1151 2e5f 7265 736f 6c76 655f 6b77  .z.Q._resolve_kw
+00000b90: 6172 6773 6302 0000 0000 0000 0007 0000  argsc...........
+00000ba0: 0003 0000 0043 0000 0073 5e00 0000 6400  .....C...s^...d.
+00000bb0: 7d02 6700 7d03 784c 7c00 6a00 4400 5d42  }.g.}.xL|.j.D.]B
+00000bc0: 7d04 7c04 6a01 7c01 8301 5c02 7d05 7d06  }.|.j.|...\.}.}.
+00000bd0: 7c03 7c06 3700 7d03 7c02 7334 7c05 7d02  |.|.7.}.|.s4|.}.
+00000be0: 7110 7c00 6a02 7c00 6a03 6b02 724a 7c02  q.|.j.|.j.k.rJ|.
+00000bf0: 7c05 4d00 7d02 7110 7c02 7c05 4f00 7d02  |.M.}.q.|.|.O.}.
+00000c00: 7110 5700 7c02 7c03 6602 5300 2901 4e29  q.W.|.|.f.S.).N)
+00000c10: 0472 1000 0000 7231 0000 0072 0800 0000  .r....r1...r....
+00000c20: 7206 0000 0029 0772 1200 0000 7232 0000  r....).r....r2..
+00000c30: 0072 2200 0000 7234 0000 0072 0b00 0000  .r"...r4...r....
+00000c40: 7239 0000 005a 0e63 6869 6c64 7265 6e5f  r9...Z.children_
+00000c50: 6a6f 696e 7372 0c00 0000 720c 0000 0072  joinsr....r....r
+00000c60: 0d00 0000 da11 5f72 6573 6f6c 7665 5f63  ......_resolve_c
+00000c70: 6869 6c64 7265 6e65 0000 0073 1600 0000  hildrene...s....
+00000c80: 0001 0401 0401 0c01 0e01 0801 0401 0602  ................
+00000c90: 0c01 0a02 0c01 7a13 512e 5f72 6573 6f6c  ......z.Q._resol
+00000ca0: 7665 5f63 6869 6c64 7265 6e63 0200 0000  ve_childrenc....
+00000cb0: 0000 0000 0200 0000 0200 0000 4300 0000  ............C...
+00000cc0: 731e 0000 007c 006a 0072 107c 006a 017c  s....|.j.r.|.j.|
+00000cd0: 0183 0153 007c 006a 027c 0183 0153 0064  ...S.|.j.|...S.d
+00000ce0: 0053 0029 014e 2903 7211 0000 0072 4200  .S.).N).r....rB.
+00000cf0: 0000 7243 0000 0029 0272 1200 0000 7232  ..rC...).r....r2
+00000d00: 0000 0072 0c00 0000 720c 0000 0072 0d00  ...r....r....r..
+00000d10: 0000 7231 0000 0074 0000 0073 0600 0000  ..r1...t...s....
+00000d20: 0001 0601 0a02 7a13 512e 7265 736f 6c76  ......z.Q.resolv
+00000d30: 655f 666f 725f 6d6f 6465 6c4e 290d da08  e_for_modelN)...
+00000d40: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
+00000d50: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
+00000d60: 5f5f 7206 0000 0072 0700 0000 7215 0000  __r....r....r...
+00000d70: 0072 1700 0000 7218 0000 0072 2300 0000  .r....r....r#...
+00000d80: 723b 0000 0072 4200 0000 7243 0000 0072  r;...rB...rC...r
+00000d90: 3100 0000 720c 0000 0072 0c00 0000 720c  1...r....r....r.
+00000da0: 0000 0072 0d00 0000 7205 0000 0007 0000  ...r....r.......
+00000db0: 0073 1400 0000 0801 0401 0402 0e0b 0805  .s..............
+00000dc0: 0805 0805 0821 081f 080f 7205 0000 0063  .....!....r....c
+00000dd0: 0000 0000 0000 0000 0000 0000 0200 0000  ................
+00000de0: 4000 0000 731c 0000 0065 005a 0164 005a  @...s....e.Z.d.Z
+00000df0: 0264 0164 0284 005a 0364 0364 0484 005a  .d.d...Z.d.d...Z
+00000e00: 0464 0553 0029 06da 0850 7265 6665 7463  .d.S.)...Prefetc
+00000e10: 6863 0300 0000 0000 0000 0300 0000 0200  hc..............
+00000e20: 0000 4300 0000 7310 0000 007c 017c 005f  ..C...s....|.|._
+00000e30: 007c 027c 005f 0164 0053 0029 014e 2902  .|.|._.d.S.).N).
+00000e40: da08 7265 6c61 7469 6f6e da08 7175 6572  ..relation..quer
+00000e50: 7973 6574 2903 7212 0000 0072 4800 0000  yset).r....rH...
+00000e60: 7249 0000 0072 0c00 0000 720c 0000 0072  rI...r....r....r
+00000e70: 0d00 0000 7215 0000 007c 0000 0073 0400  ....r....|...s..
+00000e80: 0000 0001 0601 7a11 5072 6566 6574 6368  ......z.Prefetch
+00000e90: 2e5f 5f69 6e69 745f 5f63 0200 0000 0000  .__init__c......
+00000ea0: 0000 0500 0000 0400 0000 4300 0000 7392  ..........C...s.
+00000eb0: 0000 007c 006a 006a 0164 0183 017d 027c  ...|.j.j.d...}.|
+00000ec0: 0264 0219 007d 037c 037c 016a 026a 036a  .d...}.|.|.j.j.j
+00000ed0: 046b 0772 3874 0564 036a 067c 037c 016a  .k.r8t.d.j.|.|.j
+00000ee0: 026a 036a 0783 0283 0182 0164 016a 087c  .j.j.......d.j.|
+00000ef0: 0264 0464 0085 0219 0083 017d 047c 0472  .d.d.......}.|.r
+00000f00: 827c 037c 016a 096a 0a83 006b 0772 6874  .|.|.j.j...k.rht
+00000f10: 0b83 007c 016a 097c 033c 007c 016a 097c  ...|.j.|.<.|.j.|
+00000f20: 0319 006a 0c74 0d7c 047c 006a 0e83 0283  ...j.t.|.|.j....
+00000f30: 0101 006e 0c7c 006a 0e7c 016a 0f7c 033c  ...n.|.j.|.j.|.<
+00000f40: 0064 0053 0029 054e 7224 0000 0072 0100  .d.S.).Nr$...r..
+00000f50: 0000 7a1c 7265 6c61 7469 6f6e 207b 7d20  ..z.relation {} 
+00000f60: 666f 7220 7b7d 206e 6f74 2066 6f75 6e64  for {} not found
+00000f70: 7225 0000 0029 1072 4800 0000 7227 0000  r%...).rH...r'..
+00000f80: 0072 3200 0000 7226 0000 0072 3e00 0000  .r2...r&...r>...
+00000f90: 7204 0000 0072 3000 0000 7219 0000 0072  r....r0...r....r
+00000fa0: 2100 0000 da0d 5f70 7265 6665 7463 685f  !....._prefetch_
+00000fb0: 6d61 70da 046b 6579 73da 0373 6574 da03  map..keys..set..
+00000fc0: 6164 6472 4700 0000 7249 0000 00da 115f  addrG...rI....._
+00000fd0: 7072 6566 6574 6368 5f71 7565 7269 6573  prefetch_queries
+00000fe0: 2905 7212 0000 0072 4900 0000 da0e 7265  ).r....rI.....re
+00000ff0: 6c61 7469 6f6e 5f73 706c 6974 da11 6669  lation_split..fi
+00001000: 7273 745f 6c65 7665 6c5f 6669 656c 64da  rst_level_field.
+00001010: 1266 6f72 7761 7264 6564 5f70 7265 6665  .forwarded_prefe
+00001020: 7463 6872 0c00 0000 720c 0000 0072 0d00  tchr....r....r..
+00001030: 0000 da14 7265 736f 6c76 655f 666f 725f  ....resolve_for_
+00001040: 7175 6572 7973 6574 8000 0000 7318 0000  queryset....s...
+00001050: 0000 010c 0108 010e 0106 0110 0112 0104  ................
+00001060: 010e 010c 010a 0110 037a 1d50 7265 6665  .........z.Prefe
+00001070: 7463 682e 7265 736f 6c76 655f 666f 725f  tch.resolve_for_
+00001080: 7175 6572 7973 6574 4e29 0572 4400 0000  querysetN).rD...
+00001090: 7245 0000 0072 4600 0000 7215 0000 0072  rE...rF...r....r
+000010a0: 5200 0000 720c 0000 0072 0c00 0000 720c  R...r....r....r.
+000010b0: 0000 0072 0d00 0000 7247 0000 007b 0000  ...r....rG...{..
+000010c0: 0073 0400 0000 0801 0804 7247 0000 004e  .s........rG...N
+000010d0: 2908 da06 7079 7069 6b61 7202 0000 00da  )...pypikar.....
+000010e0: 0874 6f72 746f 6973 6572 0300 0000 da13  .tortoiser......
+000010f0: 746f 7274 6f69 7365 2e65 7863 6570 7469  tortoise.excepti
+00001100: 6f6e 7372 0400 0000 7205 0000 0072 4700  onsr....r....rG.
+00001110: 0000 720c 0000 0072 0c00 0000 720c 0000  ..r....r....r...
+00001120: 0072 0d00 0000 da08 3c6d 6f64 756c 653e  .r......<module>
+00001130: 0100 0000 7308 0000 000c 020c 010c 030e  ....s...........
+00001140: 74                                       t
```

### Comparing `tortoise-orm-0.9.2/tortoise/__pycache__/exceptions.cpython-36.pyc` & `tortoise-orm-0.9.4/tortoise/__pycache__/exceptions.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.6 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,92 +1,100 @@
-00000000: 330d 0d0a 5576 3f5b 3a02 0000 e300 0000  3...Uv?[:.......
+00000000: 330d 0d0a ed8b 4b5b 7802 0000 e300 0000  3.....K[x.......
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 7400 0000 4700 6400 6401 8400 6401  .st...G.d.d...d.
+00000020: 0073 8400 0000 4700 6400 6401 8400 6401  .s....G.d.d...d.
 00000030: 6500 8303 5a01 4700 6402 6403 8400 6403  e...Z.G.d.d...d.
 00000040: 6501 8303 5a02 4700 6404 6405 8400 6405  e...Z.G.d.d...d.
 00000050: 6501 8303 5a03 4700 6406 6407 8400 6407  e...Z.G.d.d...d.
 00000060: 6501 8303 5a04 4700 6408 6409 8400 6409  e...Z.G.d.d...d.
 00000070: 6501 8303 5a05 4700 640a 640b 8400 640b  e...Z.G.d.d...d.
-00000080: 6500 8303 5a06 4700 640c 640d 8400 640d  e...Z.G.d.d...d.
-00000090: 6500 8303 5a07 640e 5300 290f 6300 0000  e...Z.d.S.).c...
-000000a0: 0000 0000 0000 0000 0001 0000 0040 0000  .............@..
-000000b0: 0073 0c00 0000 6500 5a01 6400 5a02 6401  .s....e.Z.d.Z.d.
-000000c0: 5300 2902 da10 4261 7365 4f52 4d45 7863  S.)...BaseORMExc
-000000d0: 6570 7469 6f6e 4e29 03da 085f 5f6e 616d  eptionN)...__nam
-000000e0: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
-000000f0: 0c5f 5f71 7561 6c6e 616d 655f 5fa9 0072  .__qualname__..r
-00000100: 0500 0000 7205 0000 00fa 472f 5573 6572  ....r.....G/User
-00000110: 732f 616e 6472 6579 626f 6e64 6172 2f50  s/andreybondar/P
-00000120: 7943 6861 726d 5072 6f6a 6563 7473 2f74  yCharmProjects/t
-00000130: 6f72 746f 6973 652d 6f72 6d2f 746f 7274  ortoise-orm/tort
-00000140: 6f69 7365 2f65 7863 6570 7469 6f6e 732e  oise/exceptions.
-00000150: 7079 7201 0000 0001 0000 0073 0200 0000  pyr........s....
-00000160: 0801 7201 0000 0063 0000 0000 0000 0000  ..r....c........
-00000170: 0000 0000 0400 0000 0000 0000 7322 0000  ............s"..
-00000180: 0065 005a 0164 005a 0264 015a 0364 0587  .e.Z.d.Z.d.Z.d..
-00000190: 0066 0164 0364 0484 095a 0487 0004 005a  .f.d.d...Z.....Z
-000001a0: 0553 0029 06da 174d 756c 7469 706c 794f  .S.)...MultiplyO
-000001b0: 626a 6563 7473 5265 7475 726e 6564 7a2f  bjectsReturnedz/
-000001c0: 4d75 6c74 6970 6c79 206f 626a 6563 7473  Multiply objects
-000001d0: 2072 6574 7572 6e65 642c 2065 7870 6563   returned, expec
-000001e0: 7465 6420 6578 6163 746c 7920 6f6e 654e  ted exactly oneN
-000001f0: 6302 0000 0000 0000 0003 0000 0003 0000  c...............
-00000200: 000b 0000 0073 2000 0000 7c01 730a 7c00  .....s ...|.s.|.
-00000210: 6a00 7d01 7401 8300 6a02 7c01 6601 7c02  j.}.t...j.|.f.|.
-00000220: 9e02 8e00 0100 6400 5300 2901 4e29 03da  ......d.S.).N)..
-00000230: 0f64 6566 6175 6c74 5f6d 6573 7361 6765  .default_message
-00000240: da05 7375 7065 72da 085f 5f69 6e69 745f  ..super..__init_
-00000250: 5f29 03da 0473 656c 66da 076d 6573 7361  _)...self..messa
-00000260: 6765 da06 6b77 6172 6773 2901 da09 5f5f  ge..kwargs)...__
-00000270: 636c 6173 735f 5f72 0500 0000 7206 0000  class__r....r...
-00000280: 0072 0a00 0000 0800 0000 7306 0000 0000  .r........s.....
-00000290: 0104 0106 017a 204d 756c 7469 706c 794f  .....z MultiplyO
-000002a0: 626a 6563 7473 5265 7475 726e 6564 2e5f  bjectsReturned._
-000002b0: 5f69 6e69 745f 5f29 014e 2906 7202 0000  _init__).N).r...
-000002c0: 0072 0300 0000 7204 0000 0072 0800 0000  .r....r....r....
-000002d0: 720a 0000 00da 0d5f 5f63 6c61 7373 6365  r......__classce
-000002e0: 6c6c 5f5f 7205 0000 0072 0500 0000 2901  ll__r....r....).
-000002f0: 720e 0000 0072 0600 0000 7207 0000 0005  r....r....r.....
-00000300: 0000 0073 0400 0000 0801 0402 7207 0000  ...s........r...
-00000310: 0063 0000 0000 0000 0000 0000 0000 0100  .c..............
-00000320: 0000 4000 0000 730c 0000 0065 005a 0164  ..@...s....e.Z.d
-00000330: 005a 0264 0153 0029 02da 0a46 6965 6c64  .Z.d.S.)...Field
-00000340: 4572 726f 724e 2903 7202 0000 0072 0300  ErrorN).r....r..
-00000350: 0000 7204 0000 0072 0500 0000 7205 0000  ..r....r....r...
-00000360: 0072 0500 0000 7206 0000 0072 1000 0000  .r....r....r....
-00000370: 0e00 0000 7302 0000 0008 0172 1000 0000  ....s......r....
-00000380: 6300 0000 0000 0000 0000 0000 0001 0000  c...............
-00000390: 0040 0000 0073 0c00 0000 6500 5a01 6400  .@...s....e.Z.d.
-000003a0: 5a02 6401 5300 2902 da0f 4e6f 5661 6c75  Z.d.S.)...NoValu
-000003b0: 6573 4665 7463 6865 644e 2903 7202 0000  esFetchedN).r...
-000003c0: 0072 0300 0000 7204 0000 0072 0500 0000  .r....r....r....
-000003d0: 7205 0000 0072 0500 0000 7206 0000 0072  r....r....r....r
-000003e0: 1100 0000 1200 0000 7302 0000 0008 0172  ........s......r
-000003f0: 1100 0000 6300 0000 0000 0000 0000 0000  ....c...........
-00000400: 0001 0000 0040 0000 0073 0c00 0000 6500  .....@...s....e.
-00000410: 5a01 6400 5a02 6401 5300 2902 da10 4f70  Z.d.Z.d.S.)...Op
-00000420: 6572 6174 696f 6e61 6c45 7272 6f72 4e29  erationalErrorN)
-00000430: 0372 0200 0000 7203 0000 0072 0400 0000  .r....r....r....
-00000440: 7205 0000 0072 0500 0000 7205 0000 0072  r....r....r....r
-00000450: 0600 0000 7212 0000 0016 0000 0073 0200  ....r........s..
-00000460: 0000 0801 7212 0000 0063 0000 0000 0000  ....r....c......
-00000470: 0000 0000 0000 0100 0000 4000 0000 730c  ..........@...s.
-00000480: 0000 0065 005a 0164 005a 0264 0153 0029  ...e.Z.d.Z.d.S.)
-00000490: 02da 1243 6f6e 6669 6775 7261 7469 6f6e  ...Configuration
-000004a0: 4572 726f 724e 2903 7202 0000 0072 0300  ErrorN).r....r..
-000004b0: 0000 7204 0000 0072 0500 0000 7205 0000  ..r....r....r...
-000004c0: 0072 0500 0000 7206 0000 0072 1300 0000  .r....r....r....
-000004d0: 1a00 0000 7302 0000 0008 0172 1300 0000  ....s......r....
-000004e0: 6300 0000 0000 0000 0000 0000 0001 0000  c...............
-000004f0: 0040 0000 0073 0c00 0000 6500 5a01 6400  .@...s....e.Z.d.
-00000500: 5a02 6401 5300 2902 da0e 496e 7465 6772  Z.d.S.)...Integr
-00000510: 6974 7945 7272 6f72 4e29 0372 0200 0000  ityErrorN).r....
-00000520: 7203 0000 0072 0400 0000 7205 0000 0072  r....r....r....r
-00000530: 0500 0000 7205 0000 0072 0600 0000 7214  ....r....r....r.
-00000540: 0000 001e 0000 0073 0200 0000 0801 7214  .......s......r.
-00000550: 0000 004e 2908 da09 4578 6365 7074 696f  ...N)...Exceptio
-00000560: 6e72 0100 0000 7207 0000 0072 1000 0000  nr....r....r....
-00000570: 7211 0000 0072 1200 0000 7213 0000 0072  r....r....r....r
-00000580: 1400 0000 7205 0000 0072 0500 0000 7205  ....r....r....r.
-00000590: 0000 0072 0600 0000 da08 3c6d 6f64 756c  ...r......<modul
-000005a0: 653e 0100 0000 730c 0000 0010 0410 0910  e>....s.........
-000005b0: 0410 0410 0410 04                        .......
+00000080: 6501 8303 5a06 4700 640c 640d 8400 640d  e...Z.G.d.d...d.
+00000090: 6501 8303 5a07 4700 640e 640f 8400 640f  e...Z.G.d.d...d.
+000000a0: 6501 8303 5a08 6410 5300 2911 6300 0000  e...Z.d.S.).c...
+000000b0: 0000 0000 0000 0000 0001 0000 0040 0000  .............@..
+000000c0: 0073 0c00 0000 6500 5a01 6400 5a02 6401  .s....e.Z.d.Z.d.
+000000d0: 5300 2902 da10 4261 7365 4f52 4d45 7863  S.)...BaseORMExc
+000000e0: 6570 7469 6f6e 4e29 03da 085f 5f6e 616d  eptionN)...__nam
+000000f0: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
+00000100: 0c5f 5f71 7561 6c6e 616d 655f 5fa9 0072  .__qualname__..r
+00000110: 0500 0000 7205 0000 00fa 472f 5573 6572  ....r.....G/User
+00000120: 732f 616e 6472 6579 626f 6e64 6172 2f50  s/andreybondar/P
+00000130: 7943 6861 726d 5072 6f6a 6563 7473 2f74  yCharmProjects/t
+00000140: 6f72 746f 6973 652d 6f72 6d2f 746f 7274  ortoise-orm/tort
+00000150: 6f69 7365 2f65 7863 6570 7469 6f6e 732e  oise/exceptions.
+00000160: 7079 7201 0000 0001 0000 0073 0200 0000  pyr........s....
+00000170: 0801 7201 0000 0063 0000 0000 0000 0000  ..r....c........
+00000180: 0000 0000 0400 0000 0000 0000 7322 0000  ............s"..
+00000190: 0065 005a 0164 005a 0264 015a 0364 0587  .e.Z.d.Z.d.Z.d..
+000001a0: 0066 0164 0364 0484 095a 0487 0004 005a  .f.d.d...Z.....Z
+000001b0: 0553 0029 06da 174d 756c 7469 706c 794f  .S.)...MultiplyO
+000001c0: 626a 6563 7473 5265 7475 726e 6564 7a2f  bjectsReturnedz/
+000001d0: 4d75 6c74 6970 6c79 206f 626a 6563 7473  Multiply objects
+000001e0: 2072 6574 7572 6e65 642c 2065 7870 6563   returned, expec
+000001f0: 7465 6420 6578 6163 746c 7920 6f6e 654e  ted exactly oneN
+00000200: 6302 0000 0000 0000 0003 0000 0003 0000  c...............
+00000210: 000b 0000 0073 2000 0000 7c01 730a 7c00  .....s ...|.s.|.
+00000220: 6a00 7d01 7401 8300 6a02 7c01 6601 7c02  j.}.t...j.|.f.|.
+00000230: 9e02 8e00 0100 6400 5300 2901 4e29 03da  ......d.S.).N)..
+00000240: 0f64 6566 6175 6c74 5f6d 6573 7361 6765  .default_message
+00000250: da05 7375 7065 72da 085f 5f69 6e69 745f  ..super..__init_
+00000260: 5f29 03da 0473 656c 66da 076d 6573 7361  _)...self..messa
+00000270: 6765 da06 6b77 6172 6773 2901 da09 5f5f  ge..kwargs)...__
+00000280: 636c 6173 735f 5f72 0500 0000 7206 0000  class__r....r...
+00000290: 0072 0a00 0000 0800 0000 7306 0000 0000  .r........s.....
+000002a0: 0104 0106 017a 204d 756c 7469 706c 794f  .....z MultiplyO
+000002b0: 626a 6563 7473 5265 7475 726e 6564 2e5f  bjectsReturned._
+000002c0: 5f69 6e69 745f 5f29 014e 2906 7202 0000  _init__).N).r...
+000002d0: 0072 0300 0000 7204 0000 0072 0800 0000  .r....r....r....
+000002e0: 720a 0000 00da 0d5f 5f63 6c61 7373 6365  r......__classce
+000002f0: 6c6c 5f5f 7205 0000 0072 0500 0000 2901  ll__r....r....).
+00000300: 720e 0000 0072 0600 0000 7207 0000 0005  r....r....r.....
+00000310: 0000 0073 0400 0000 0801 0402 7207 0000  ...s........r...
+00000320: 0063 0000 0000 0000 0000 0000 0000 0100  .c..............
+00000330: 0000 4000 0000 730c 0000 0065 005a 0164  ..@...s....e.Z.d
+00000340: 005a 0264 0153 0029 02da 0a46 6965 6c64  .Z.d.S.)...Field
+00000350: 4572 726f 724e 2903 7202 0000 0072 0300  ErrorN).r....r..
+00000360: 0000 7204 0000 0072 0500 0000 7205 0000  ..r....r....r...
+00000370: 0072 0500 0000 7206 0000 0072 1000 0000  .r....r....r....
+00000380: 0e00 0000 7302 0000 0008 0172 1000 0000  ....s......r....
+00000390: 6300 0000 0000 0000 0000 0000 0001 0000  c...............
+000003a0: 0040 0000 0073 0c00 0000 6500 5a01 6400  .@...s....e.Z.d.
+000003b0: 5a02 6401 5300 2902 da0b 5061 7261 6d73  Z.d.S.)...Params
+000003c0: 4572 726f 724e 2903 7202 0000 0072 0300  ErrorN).r....r..
+000003d0: 0000 7204 0000 0072 0500 0000 7205 0000  ..r....r....r...
+000003e0: 0072 0500 0000 7206 0000 0072 1100 0000  .r....r....r....
+000003f0: 1200 0000 7302 0000 0008 0172 1100 0000  ....s......r....
+00000400: 6300 0000 0000 0000 0000 0000 0001 0000  c...............
+00000410: 0040 0000 0073 0c00 0000 6500 5a01 6400  .@...s....e.Z.d.
+00000420: 5a02 6401 5300 2902 da0f 4e6f 5661 6c75  Z.d.S.)...NoValu
+00000430: 6573 4665 7463 6865 644e 2903 7202 0000  esFetchedN).r...
+00000440: 0072 0300 0000 7204 0000 0072 0500 0000  .r....r....r....
+00000450: 7205 0000 0072 0500 0000 7206 0000 0072  r....r....r....r
+00000460: 1200 0000 1600 0000 7302 0000 0008 0172  ........s......r
+00000470: 1200 0000 6300 0000 0000 0000 0000 0000  ....c...........
+00000480: 0001 0000 0040 0000 0073 0c00 0000 6500  .....@...s....e.
+00000490: 5a01 6400 5a02 6401 5300 2902 da10 4f70  Z.d.Z.d.S.)...Op
+000004a0: 6572 6174 696f 6e61 6c45 7272 6f72 4e29  erationalErrorN)
+000004b0: 0372 0200 0000 7203 0000 0072 0400 0000  .r....r....r....
+000004c0: 7205 0000 0072 0500 0000 7205 0000 0072  r....r....r....r
+000004d0: 0600 0000 7213 0000 001a 0000 0073 0200  ....r........s..
+000004e0: 0000 0801 7213 0000 0063 0000 0000 0000  ....r....c......
+000004f0: 0000 0000 0000 0100 0000 4000 0000 730c  ..........@...s.
+00000500: 0000 0065 005a 0164 005a 0264 0153 0029  ...e.Z.d.Z.d.S.)
+00000510: 02da 1243 6f6e 6669 6775 7261 7469 6f6e  ...Configuration
+00000520: 4572 726f 724e 2903 7202 0000 0072 0300  ErrorN).r....r..
+00000530: 0000 7204 0000 0072 0500 0000 7205 0000  ..r....r....r...
+00000540: 0072 0500 0000 7206 0000 0072 1400 0000  .r....r....r....
+00000550: 1e00 0000 7302 0000 0008 0172 1400 0000  ....s......r....
+00000560: 6300 0000 0000 0000 0000 0000 0001 0000  c...............
+00000570: 0040 0000 0073 0c00 0000 6500 5a01 6400  .@...s....e.Z.d.
+00000580: 5a02 6401 5300 2902 da0e 496e 7465 6772  Z.d.S.)...Integr
+00000590: 6974 7945 7272 6f72 4e29 0372 0200 0000  ityErrorN).r....
+000005a0: 7203 0000 0072 0400 0000 7205 0000 0072  r....r....r....r
+000005b0: 0500 0000 7205 0000 0072 0600 0000 7215  ....r....r....r.
+000005c0: 0000 0022 0000 0073 0200 0000 0801 7215  ..."...s......r.
+000005d0: 0000 004e 2909 da09 4578 6365 7074 696f  ...N)...Exceptio
+000005e0: 6e72 0100 0000 7207 0000 0072 1000 0000  nr....r....r....
+000005f0: 7211 0000 0072 1200 0000 7213 0000 0072  r....r....r....r
+00000600: 1400 0000 7215 0000 0072 0500 0000 7205  ....r....r....r.
+00000610: 0000 0072 0500 0000 7206 0000 00da 083c  ...r....r......<
+00000620: 6d6f 6475 6c65 3e01 0000 0073 0e00 0000  module>....s....
+00000630: 1004 1009 1004 1004 1004 1004 1004       ..............
```

### Comparing `tortoise-orm-0.9.2/tortoise/__pycache__/aggregation.cpython-36.pyc` & `tortoise-orm-0.9.4/tortoise/__pycache__/aggregation.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.6 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 18% similar despite different names*

```diff
@@ -1,141 +1,150 @@
-00000000: 330d 0d0a 5707 365b 7c08 0000 e300 0000  3...W.6[|.......
+00000000: 330d 0d0a dc7e 445b fd08 0000 e300 0000  3....~D[........
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 b600 0000 6400 6401 6c00 6d01 5a01  .s....d.d.l.m.Z.
+00000020: 0073 c200 0000 6400 6401 6c00 6d01 5a01  .s....d.d.l.m.Z.
 00000030: 0100 6400 6402 6c02 6d03 5a04 0100 6400  ..d.d.l.m.Z...d.
 00000040: 6403 6c02 6d05 5a06 0100 6400 6404 6c02  d.l.m.Z...d.d.l.
 00000050: 6d07 5a08 0100 6400 6405 6c02 6d09 5a0a  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6406 6c02 6d0b 5a0c 0100 6400  ..d.d.l.m.Z...d.
-00000070: 6407 6c0d 6d0e 5a0e 0100 4700 6408 6409  d.l.m.Z...G.d.d.
-00000080: 8400 6409 8302 5a0f 4700 640a 640b 8400  ..d...Z.G.d.d...
-00000090: 640b 650f 8303 5a05 4700 640c 640d 8400  d.e...Z.G.d.d...
-000000a0: 640d 650f 8303 5a0b 4700 640e 640f 8400  d.e...Z.G.d.d...
-000000b0: 640f 650f 8303 5a07 4700 6410 6411 8400  d.e...Z.G.d.d...
-000000c0: 6411 650f 8303 5a09 4700 6412 6413 8400  d.e...Z.G.d.d...
-000000d0: 6413 650f 8303 5a03 6414 5300 2915 e900  d.e...Z.d.S.)...
-000000e0: 0000 0029 01da 0554 6162 6c65 2901 da03  ...)...Table)...
-000000f0: 4176 6729 01da 0543 6f75 6e74 2901 da03  Avg)...Count)...
-00000100: 4d61 7829 01da 034d 696e 2901 da03 5375  Max)...Min)...Su
-00000110: 6d29 01da 1141 6767 7265 6761 7465 4675  m)...AggregateFu
-00000120: 6e63 7469 6f6e 6300 0000 0000 0000 0000  nctionc.........
-00000130: 0000 0002 0000 0040 0000 0073 2800 0000  .......@...s(...
-00000140: 6500 5a01 6400 5a02 6503 5a04 6401 6402  e.Z.d.Z.e.Z.d.d.
-00000150: 8400 5a05 6403 6404 8400 5a06 6405 6406  ..Z.d.d...Z.d.d.
-00000160: 8400 5a07 6407 5300 2908 da09 4167 6772  ..Z.d.S.)...Aggr
-00000170: 6567 6174 6563 0200 0000 0000 0000 0200  egatec..........
-00000180: 0000 0200 0000 4300 0000 730a 0000 007c  ......C...s....|
-00000190: 017c 005f 0064 0053 0029 014e 2901 da05  .|._.d.S.).N)...
-000001a0: 6669 656c 6429 02da 0473 656c 6672 0a00  field)...selfr..
-000001b0: 0000 a900 720c 0000 00fa 192e 2f74 6f72  ....r......./tor
-000001c0: 746f 6973 652f 6167 6772 6567 6174 696f  toise/aggregatio
-000001d0: 6e2e 7079 da08 5f5f 696e 6974 5f5f 0d00  n.py..__init__..
-000001e0: 0000 7302 0000 0000 017a 1241 6767 7265  ..s......z.Aggre
-000001f0: 6761 7465 2e5f 5f69 6e69 745f 5f63 0300  gate.__init__c..
-00000200: 0000 0000 0000 0700 0000 0500 0000 4300  ..............C.
-00000210: 0000 7310 0100 007c 016a 0064 0183 017d  ..s....|.j.d...}
-00000220: 037c 0364 0264 0085 0219 0073 a467 0064  .|.d.d.....s.g.d
-00000230: 0064 039c 027d 047c 0364 0419 007c 026a  .d...}.|.d...|.j
-00000240: 016a 026b 0672 807c 026a 016a 037c 0364  .j.k.r.|.j.j.|.d
-00000250: 0419 0019 007d 0574 047c 026a 016a 0583  .....}.t.|.j.j..
-00000260: 017c 0364 0419 007c 0566 037d 067c 0464  .|.d...|.f.}.|.d
-00000270: 0519 006a 067c 0683 0101 007c 006a 0774  ...j.|.....|.j.t
-00000280: 047c 056a 086a 016a 0583 016a 0983 017c  .|.j.j.j...j...|
-00000290: 0464 063c 006e 207c 006a 0774 0a74 047c  .d.<.n |.j.t.t.|
-000002a0: 026a 016a 0583 017c 0364 0419 0083 0283  .j.j...|.d......
-000002b0: 017c 0464 063c 007c 0453 007c 0364 0419  .|.d.<.|.S.|.d..
-000002c0: 007c 026a 016a 026b 0673 b874 0b82 017c  .|.j.j.k.s.t...|
-000002d0: 026a 016a 037c 0364 0419 0019 007d 0574  .j.j.|.d.....}.t
-000002e0: 047c 026a 016a 0583 017c 0364 0419 007c  .|.j.j...|.d...|
-000002f0: 0566 037d 067c 006a 0c64 016a 0d7c 0364  .f.}.|.j.d.j.|.d
-00000300: 0264 0085 0219 0083 017c 056a 0883 027d  .d.......|.j...}
-00000310: 047c 0464 0519 006a 067c 0683 0101 007c  .|.d...j.|.....|
-00000320: 0453 0064 0053 0029 074e da02 5f5f e901  .S.d.S.).N..__..
-00000330: 0000 0029 02da 056a 6f69 6e73 720a 0000  ...)...joinsr...
-00000340: 0072 0100 0000 7211 0000 0072 0a00 0000  .r....r....r....
-00000350: 290e da05 7370 6c69 74da 055f 6d65 7461  )...split.._meta
-00000360: da0c 6665 7463 685f 6669 656c 6473 da0a  ..fetch_fields..
-00000370: 6669 656c 6473 5f6d 6170 7202 0000 00da  fields_mapr.....
-00000380: 0574 6162 6c65 da06 6170 7065 6e64 da10  .table..append..
-00000390: 6167 6772 6567 6174 696f 6e5f 6675 6e63  aggregation_func
-000003a0: da04 7479 7065 da02 6964 da07 6765 7461  ..type..id..geta
-000003b0: 7474 72da 0e41 7373 6572 7469 6f6e 4572  ttr..AssertionEr
-000003c0: 726f 72da 185f 7265 736f 6c76 655f 6669  ror.._resolve_fi
-000003d0: 656c 645f 666f 725f 6d6f 6465 6cda 046a  eld_for_model..j
-000003e0: 6f69 6e29 0772 0b00 0000 720a 0000 00da  oin).r....r.....
-000003f0: 056d 6f64 656c 5a0b 6669 656c 645f 7370  .modelZ.field_sp
-00000400: 6c69 74da 0b61 6767 7265 6761 7469 6f6e  lit..aggregation
-00000410: da0d 7265 6c61 7465 645f 6669 656c 6472  ..related_fieldr
-00000420: 1e00 0000 720c 0000 0072 0c00 0000 720d  ....r....r....r.
-00000430: 0000 0072 1d00 0000 1000 0000 7328 0000  ...r........s(..
-00000440: 0000 010a 010c 0202 0108 0210 0110 0116  ................
-00000450: 010e 0104 0118 0304 011c 0204 0214 0110  ................
-00000460: 0116 0104 0118 020e 017a 2241 6767 7265  .........z"Aggre
-00000470: 6761 7465 2e5f 7265 736f 6c76 655f 6669  gate._resolve_fi
-00000480: 656c 645f 666f 725f 6d6f 6465 6c63 0200  eld_for_modelc..
-00000490: 0000 0000 0000 0300 0000 0300 0000 4300  ..............C.
-000004a0: 0000 7322 0000 007c 006a 007c 006a 017c  ..s"...|.j.|.j.|
-000004b0: 0183 027d 0274 027c 0264 0119 0083 017c  ...}.t.|.d.....|
-000004c0: 0264 013c 007c 0253 0029 024e 7211 0000  .d.<.|.S.).Nr...
-000004d0: 0029 0372 1d00 0000 720a 0000 00da 0872  .).r....r......r
-000004e0: 6576 6572 7365 6429 0372 0b00 0000 721f  eversed).r....r.
-000004f0: 0000 0072 2000 0000 720c 0000 0072 0c00  ...r ...r....r..
-00000500: 0000 720d 0000 00da 1172 6573 6f6c 7665  ..r......resolve
-00000510: 5f66 6f72 5f6d 6f64 656c 2d00 0000 7306  _for_model-...s.
-00000520: 0000 0000 010e 0110 017a 1b41 6767 7265  .........z.Aggre
-00000530: 6761 7465 2e72 6573 6f6c 7665 5f66 6f72  gate.resolve_for
-00000540: 5f6d 6f64 656c 4e29 08da 085f 5f6e 616d  _modelN)...__nam
-00000550: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
-00000560: 0c5f 5f71 7561 6c6e 616d 655f 5f72 0800  .__qualname__r..
-00000570: 0000 7218 0000 0072 0e00 0000 721d 0000  ..r....r....r...
-00000580: 0072 2300 0000 720c 0000 0072 0c00 0000  .r#...r....r....
-00000590: 720c 0000 0072 0d00 0000 7209 0000 000a  r....r....r.....
-000005a0: 0000 0073 0800 0000 0801 0402 0803 081d  ...s............
-000005b0: 7209 0000 0063 0000 0000 0000 0000 0000  r....c..........
-000005c0: 0000 0100 0000 4000 0000 7310 0000 0065  ......@...s....e
-000005d0: 005a 0164 005a 0265 035a 0464 0153 0029  .Z.d.Z.e.Z.d.S.)
-000005e0: 0272 0400 0000 4e29 0572 2400 0000 7225  .r....N).r$...r%
-000005f0: 0000 0072 2600 0000 da0b 5079 7069 6b61  ...r&.....Pypika
-00000600: 436f 756e 7472 1800 0000 720c 0000 0072  Countr....r....r
-00000610: 0c00 0000 720c 0000 0072 0d00 0000 7204  ....r....r....r.
-00000620: 0000 0033 0000 0073 0200 0000 0801 7204  ...3...s......r.
-00000630: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-00000640: 0100 0000 4000 0000 7310 0000 0065 005a  ....@...s....e.Z
-00000650: 0164 005a 0265 035a 0464 0153 0029 0272  .d.Z.e.Z.d.S.).r
-00000660: 0700 0000 4e29 0572 2400 0000 7225 0000  ....N).r$...r%..
-00000670: 0072 2600 0000 da09 5079 7069 6b61 5375  .r&.....PypikaSu
-00000680: 6d72 1800 0000 720c 0000 0072 0c00 0000  mr....r....r....
-00000690: 720c 0000 0072 0d00 0000 7207 0000 0037  r....r....r....7
-000006a0: 0000 0073 0200 0000 0801 7207 0000 0063  ...s......r....c
-000006b0: 0000 0000 0000 0000 0000 0000 0100 0000  ................
-000006c0: 4000 0000 7310 0000 0065 005a 0164 005a  @...s....e.Z.d.Z
-000006d0: 0265 035a 0464 0153 0029 0272 0500 0000  .e.Z.d.S.).r....
-000006e0: 4e29 0572 2400 0000 7225 0000 0072 2600  N).r$...r%...r&.
-000006f0: 0000 da09 5079 7069 6b61 4d61 7872 1800  ....PypikaMaxr..
-00000700: 0000 720c 0000 0072 0c00 0000 720c 0000  ..r....r....r...
-00000710: 0072 0d00 0000 7205 0000 003b 0000 0073  .r....r....;...s
-00000720: 0200 0000 0801 7205 0000 0063 0000 0000  ......r....c....
-00000730: 0000 0000 0000 0000 0100 0000 4000 0000  ............@...
-00000740: 7310 0000 0065 005a 0164 005a 0265 035a  s....e.Z.d.Z.e.Z
-00000750: 0464 0153 0029 0272 0600 0000 4e29 0572  .d.S.).r....N).r
-00000760: 2400 0000 7225 0000 0072 2600 0000 da09  $...r%...r&.....
-00000770: 5079 7069 6b61 4d69 6e72 1800 0000 720c  PypikaMinr....r.
-00000780: 0000 0072 0c00 0000 720c 0000 0072 0d00  ...r....r....r..
-00000790: 0000 7206 0000 003f 0000 0073 0200 0000  ..r....?...s....
-000007a0: 0801 7206 0000 0063 0000 0000 0000 0000  ..r....c........
-000007b0: 0000 0000 0100 0000 4000 0000 7310 0000  ........@...s...
-000007c0: 0065 005a 0164 005a 0265 035a 0464 0153  .e.Z.d.Z.e.Z.d.S
-000007d0: 0029 0272 0300 0000 4e29 0572 2400 0000  .).r....N).r$...
-000007e0: 7225 0000 0072 2600 0000 da09 5079 7069  r%...r&.....Pypi
-000007f0: 6b61 4176 6772 1800 0000 720c 0000 0072  kaAvgr....r....r
-00000800: 0c00 0000 720c 0000 0072 0d00 0000 7203  ....r....r....r.
-00000810: 0000 0043 0000 0073 0200 0000 0801 7203  ...C...s......r.
-00000820: 0000 004e 2910 da06 7079 7069 6b61 7202  ...N)...pypikar.
-00000830: 0000 00da 1070 7970 696b 612e 6675 6e63  .....pypika.func
-00000840: 7469 6f6e 7372 0300 0000 722b 0000 0072  tionsr....r+...r
-00000850: 0400 0000 7227 0000 0072 0500 0000 7229  ....r'...r....r)
-00000860: 0000 0072 0600 0000 722a 0000 0072 0700  ...r....r*...r..
-00000870: 0000 7228 0000 00da 0c70 7970 696b 612e  ..r(.....pypika.
-00000880: 7465 726d 7372 0800 0000 7209 0000 0072  termsr....r....r
-00000890: 0c00 0000 720c 0000 0072 0c00 0000 720d  ....r....r....r.
-000008a0: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
-000008b0: 0073 1800 0000 0c01 0c01 0c01 0c01 0c01  .s..............
-000008c0: 0c01 0c03 0e29 1004 1004 1004 1004       .....)........
+00000070: 6407 6c0d 6d0e 5a0e 0100 6400 6408 6c0f  d.l.m.Z...d.d.l.
+00000080: 6d10 5a10 0100 4700 6409 640a 8400 640a  m.Z...G.d.d...d.
+00000090: 8302 5a11 4700 640b 640c 8400 640c 6511  ..Z.G.d.d...d.e.
+000000a0: 8303 5a05 4700 640d 640e 8400 640e 6511  ..Z.G.d.d...d.e.
+000000b0: 8303 5a0b 4700 640f 6410 8400 6410 6511  ..Z.G.d.d...d.e.
+000000c0: 8303 5a07 4700 6411 6412 8400 6412 6511  ..Z.G.d.d...d.e.
+000000d0: 8303 5a09 4700 6413 6414 8400 6414 6511  ..Z.G.d.d...d.e.
+000000e0: 8303 5a03 6415 5300 2916 e900 0000 0029  ..Z.d.S.)......)
+000000f0: 01da 0554 6162 6c65 2901 da03 4176 6729  ...Table)...Avg)
+00000100: 01da 0543 6f75 6e74 2901 da03 4d61 7829  ...Count)...Max)
+00000110: 01da 034d 696e 2901 da03 5375 6d29 01da  ...Min)...Sum)..
+00000120: 1141 6767 7265 6761 7465 4675 6e63 7469  .AggregateFuncti
+00000130: 6f6e 2901 da12 436f 6e66 6967 7572 6174  on)...Configurat
+00000140: 696f 6e45 7272 6f72 6300 0000 0000 0000  ionErrorc.......
+00000150: 0000 0000 0002 0000 0040 0000 0073 2800  .........@...s(.
+00000160: 0000 6500 5a01 6400 5a02 6503 5a04 6401  ..e.Z.d.Z.e.Z.d.
+00000170: 6402 8400 5a05 6403 6404 8400 5a06 6405  d...Z.d.d...Z.d.
+00000180: 6406 8400 5a07 6407 5300 2908 da09 4167  d...Z.d.S.)...Ag
+00000190: 6772 6567 6174 6563 0200 0000 0000 0000  gregatec........
+000001a0: 0200 0000 0200 0000 4300 0000 730a 0000  ........C...s...
+000001b0: 007c 017c 005f 0064 0053 0029 014e 2901  .|.|._.d.S.).N).
+000001c0: da05 6669 656c 6429 02da 0473 656c 6672  ..field)...selfr
+000001d0: 0b00 0000 a900 720d 0000 00fa 482f 5573  ......r.....H/Us
+000001e0: 6572 732f 616e 6472 6579 626f 6e64 6172  ers/andreybondar
+000001f0: 2f50 7943 6861 726d 5072 6f6a 6563 7473  /PyCharmProjects
+00000200: 2f74 6f72 746f 6973 652d 6f72 6d2f 746f  /tortoise-orm/to
+00000210: 7274 6f69 7365 2f61 6767 7265 6761 7469  rtoise/aggregati
+00000220: 6f6e 2e70 79da 085f 5f69 6e69 745f 5f0f  on.py..__init__.
+00000230: 0000 0073 0200 0000 0001 7a12 4167 6772  ...s......z.Aggr
+00000240: 6567 6174 652e 5f5f 696e 6974 5f5f 6303  egate.__init__c.
+00000250: 0000 0000 0000 0007 0000 0005 0000 0043  ...............C
+00000260: 0000 0073 1a01 0000 7c01 6a00 6401 8301  ...s....|.j.d...
+00000270: 7d03 7c03 6402 6400 8502 1900 73a4 6700  }.|.d.d.....s.g.
+00000280: 6400 6403 9c02 7d04 7c03 6404 1900 7c02  d.d...}.|.d...|.
+00000290: 6a01 6a02 6b06 7280 7c02 6a01 6a03 7c03  j.j.k.r.|.j.j.|.
+000002a0: 6404 1900 1900 7d05 7404 7c02 6a01 6a05  d.....}.t.|.j.j.
+000002b0: 8301 7c03 6404 1900 7c05 6603 7d06 7c04  ..|.d...|.f.}.|.
+000002c0: 6405 1900 6a06 7c06 8301 0100 7c00 6a07  d...j.|.....|.j.
+000002d0: 7404 7c05 6a08 6a01 6a05 8301 6a09 8301  t.|.j.j.j...j...
+000002e0: 7c04 6406 3c00 6e20 7c00 6a07 740a 7404  |.d.<.n |.j.t.t.
+000002f0: 7c02 6a01 6a05 8301 7c03 6404 1900 8302  |.j.j...|.d.....
+00000300: 8301 7c04 6406 3c00 7c04 5300 7c03 6404  ..|.d.<.|.S.|.d.
+00000310: 1900 7c02 6a01 6a02 6b07 72c2 740b 6407  ..|.j.j.k.r.t.d.
+00000320: 6a0c 7c01 8301 8301 8201 7c02 6a01 6a03  j.|.......|.j.j.
+00000330: 7c03 6404 1900 1900 7d05 7404 7c02 6a01  |.d.....}.t.|.j.
+00000340: 6a05 8301 7c03 6404 1900 7c05 6603 7d06  j...|.d...|.f.}.
+00000350: 7c00 6a0d 6401 6a0e 7c03 6402 6400 8502  |.j.d.j.|.d.d...
+00000360: 1900 8301 7c05 6a08 8302 7d04 7c04 6405  ....|.j...}.|.d.
+00000370: 1900 6a06 7c06 8301 0100 7c04 5300 6400  ..j.|.....|.S.d.
+00000380: 5300 2908 4eda 025f 5fe9 0100 0000 2902  S.).N..__.....).
+00000390: da05 6a6f 696e 7372 0b00 0000 7201 0000  ..joinsr....r...
+000003a0: 0072 1200 0000 720b 0000 007a 117b 7d20  .r....r....z.{} 
+000003b0: 6e6f 7420 7265 736f 6c76 6162 6c65 290f  not resolvable).
+000003c0: da05 7370 6c69 74da 055f 6d65 7461 da0c  ..split.._meta..
+000003d0: 6665 7463 685f 6669 656c 6473 da0a 6669  fetch_fields..fi
+000003e0: 656c 6473 5f6d 6170 7202 0000 00da 0574  elds_mapr......t
+000003f0: 6162 6c65 da06 6170 7065 6e64 da10 6167  able..append..ag
+00000400: 6772 6567 6174 696f 6e5f 6675 6e63 da04  gregation_func..
+00000410: 7479 7065 da02 6964 da07 6765 7461 7474  type..id..getatt
+00000420: 7272 0900 0000 da06 666f 726d 6174 da18  rr......format..
+00000430: 5f72 6573 6f6c 7665 5f66 6965 6c64 5f66  _resolve_field_f
+00000440: 6f72 5f6d 6f64 656c da04 6a6f 696e 2907  or_model..join).
+00000450: 720c 0000 0072 0b00 0000 da05 6d6f 6465  r....r......mode
+00000460: 6cda 0b66 6965 6c64 5f73 706c 6974 da0b  l..field_split..
+00000470: 6167 6772 6567 6174 696f 6eda 0d72 656c  aggregation..rel
+00000480: 6174 6564 5f66 6965 6c64 721f 0000 0072  ated_fieldr....r
+00000490: 0d00 0000 720d 0000 0072 0e00 0000 721e  ....r....r....r.
+000004a0: 0000 0012 0000 0073 2a00 0000 0001 0a01  .......s*.......
+000004b0: 0c02 0201 0802 1001 1001 1601 0e01 0401  ................
+000004c0: 1803 0401 1c02 0402 1001 0e01 1001 1601  ................
+000004d0: 0401 1802 0e01 7a22 4167 6772 6567 6174  ......z"Aggregat
+000004e0: 652e 5f72 6573 6f6c 7665 5f66 6965 6c64  e._resolve_field
+000004f0: 5f66 6f72 5f6d 6f64 656c 6302 0000 0000  _for_modelc.....
+00000500: 0000 0003 0000 0003 0000 0043 0000 0073  ...........C...s
+00000510: 2200 0000 7c00 6a00 7c00 6a01 7c01 8302  "...|.j.|.j.|...
+00000520: 7d02 7402 7c02 6401 1900 8301 7c02 6401  }.t.|.d.....|.d.
+00000530: 3c00 7c02 5300 2902 4e72 1200 0000 2903  <.|.S.).Nr....).
+00000540: 721e 0000 0072 0b00 0000 da08 7265 7665  r....r......reve
+00000550: 7273 6564 2903 720c 0000 0072 2000 0000  rsed).r....r ...
+00000560: 7222 0000 0072 0d00 0000 720d 0000 0072  r"...r....r....r
+00000570: 0e00 0000 da11 7265 736f 6c76 655f 666f  ......resolve_fo
+00000580: 725f 6d6f 6465 6c30 0000 0073 0600 0000  r_model0...s....
+00000590: 0001 0e01 1001 7a1b 4167 6772 6567 6174  ......z.Aggregat
+000005a0: 652e 7265 736f 6c76 655f 666f 725f 6d6f  e.resolve_for_mo
+000005b0: 6465 6c4e 2908 da08 5f5f 6e61 6d65 5f5f  delN)...__name__
+000005c0: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
+000005d0: 7175 616c 6e61 6d65 5f5f 7208 0000 0072  qualname__r....r
+000005e0: 1900 0000 720f 0000 0072 1e00 0000 7225  ....r....r....r%
+000005f0: 0000 0072 0d00 0000 720d 0000 0072 0d00  ...r....r....r..
+00000600: 0000 720e 0000 0072 0a00 0000 0c00 0000  ..r....r........
+00000610: 7308 0000 0008 0104 0208 0308 1e72 0a00  s............r..
+00000620: 0000 6300 0000 0000 0000 0000 0000 0001  ..c.............
+00000630: 0000 0040 0000 0073 1000 0000 6500 5a01  ...@...s....e.Z.
+00000640: 6400 5a02 6503 5a04 6401 5300 2902 7204  d.Z.e.Z.d.S.).r.
+00000650: 0000 004e 2905 7226 0000 0072 2700 0000  ...N).r&...r'...
+00000660: 7228 0000 00da 0b50 7970 696b 6143 6f75  r(.....PypikaCou
+00000670: 6e74 7219 0000 0072 0d00 0000 720d 0000  ntr....r....r...
+00000680: 0072 0d00 0000 720e 0000 0072 0400 0000  .r....r....r....
+00000690: 3600 0000 7302 0000 0008 0172 0400 0000  6...s......r....
+000006a0: 6300 0000 0000 0000 0000 0000 0001 0000  c...............
+000006b0: 0040 0000 0073 1000 0000 6500 5a01 6400  .@...s....e.Z.d.
+000006c0: 5a02 6503 5a04 6401 5300 2902 7207 0000  Z.e.Z.d.S.).r...
+000006d0: 004e 2905 7226 0000 0072 2700 0000 7228  .N).r&...r'...r(
+000006e0: 0000 00da 0950 7970 696b 6153 756d 7219  .....PypikaSumr.
+000006f0: 0000 0072 0d00 0000 720d 0000 0072 0d00  ...r....r....r..
+00000700: 0000 720e 0000 0072 0700 0000 3a00 0000  ..r....r....:...
+00000710: 7302 0000 0008 0172 0700 0000 6300 0000  s......r....c...
+00000720: 0000 0000 0000 0000 0001 0000 0040 0000  .............@..
+00000730: 0073 1000 0000 6500 5a01 6400 5a02 6503  .s....e.Z.d.Z.e.
+00000740: 5a04 6401 5300 2902 7205 0000 004e 2905  Z.d.S.).r....N).
+00000750: 7226 0000 0072 2700 0000 7228 0000 00da  r&...r'...r(....
+00000760: 0950 7970 696b 614d 6178 7219 0000 0072  .PypikaMaxr....r
+00000770: 0d00 0000 720d 0000 0072 0d00 0000 720e  ....r....r....r.
+00000780: 0000 0072 0500 0000 3e00 0000 7302 0000  ...r....>...s...
+00000790: 0008 0172 0500 0000 6300 0000 0000 0000  ...r....c.......
+000007a0: 0000 0000 0001 0000 0040 0000 0073 1000  .........@...s..
+000007b0: 0000 6500 5a01 6400 5a02 6503 5a04 6401  ..e.Z.d.Z.e.Z.d.
+000007c0: 5300 2902 7206 0000 004e 2905 7226 0000  S.).r....N).r&..
+000007d0: 0072 2700 0000 7228 0000 00da 0950 7970  .r'...r(.....Pyp
+000007e0: 696b 614d 696e 7219 0000 0072 0d00 0000  ikaMinr....r....
+000007f0: 720d 0000 0072 0d00 0000 720e 0000 0072  r....r....r....r
+00000800: 0600 0000 4200 0000 7302 0000 0008 0172  ....B...s......r
+00000810: 0600 0000 6300 0000 0000 0000 0000 0000  ....c...........
+00000820: 0001 0000 0040 0000 0073 1000 0000 6500  .....@...s....e.
+00000830: 5a01 6400 5a02 6503 5a04 6401 5300 2902  Z.d.Z.e.Z.d.S.).
+00000840: 7203 0000 004e 2905 7226 0000 0072 2700  r....N).r&...r'.
+00000850: 0000 7228 0000 00da 0950 7970 696b 6141  ..r(.....PypikaA
+00000860: 7667 7219 0000 0072 0d00 0000 720d 0000  vgr....r....r...
+00000870: 0072 0d00 0000 720e 0000 0072 0300 0000  .r....r....r....
+00000880: 4600 0000 7302 0000 0008 0172 0300 0000  F...s......r....
+00000890: 4e29 12da 0670 7970 696b 6172 0200 0000  N)...pypikar....
+000008a0: da10 7079 7069 6b61 2e66 756e 6374 696f  ..pypika.functio
+000008b0: 6e73 7203 0000 0072 2d00 0000 7204 0000  nsr....r-...r...
+000008c0: 0072 2900 0000 7205 0000 0072 2b00 0000  .r)...r....r+...
+000008d0: 7206 0000 0072 2c00 0000 7207 0000 0072  r....r,...r....r
+000008e0: 2a00 0000 da0c 7079 7069 6b61 2e74 6572  *.....pypika.ter
+000008f0: 6d73 7208 0000 00da 1374 6f72 746f 6973  msr......tortois
+00000900: 652e 6578 6365 7074 696f 6e73 7209 0000  e.exceptionsr...
+00000910: 0072 0a00 0000 720d 0000 0072 0d00 0000  .r....r....r....
+00000920: 720d 0000 0072 0e00 0000 da08 3c6d 6f64  r....r......<mod
+00000930: 756c 653e 0100 0000 731a 0000 000c 010c  ule>....s.......
+00000940: 010c 010c 010c 010c 010c 020c 030e 2a10  ..............*.
+00000950: 0410 0410 0410 04                        .......
```

### Comparing `tortoise-orm-0.9.2/tortoise/__pycache__/queryset.cpython-36.pyc` & `tortoise-orm-0.9.4/tortoise/__pycache__/queryset.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.6 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 13% similar despite different names*

```diff
@@ -1,1204 +1,1204 @@
-00000000: 330d 0d0a 5576 3f5b cd63 0000 e300 0000  3...Uv?[.c......
+00000000: 330d 0d0a dc7e 445b d763 0000 e300 0000  3....~D[.c......
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 0201 0000 6400 6401 6c00 6d01 5a01  .s....d.d.l.m.Z.
+00000020: 0073 0601 0000 6400 6401 6c00 6d01 5a01  .s....d.d.l.m.Z.
 00000030: 6d02 5a02 0100 6400 6402 6c00 6d03 5a04  m.Z...d.d.l.m.Z.
 00000040: 0100 6400 6403 6c00 6d05 5a05 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6404 6c06 6d07 5a07 0100 6400 6405 6c08  d.l.m.Z...d.d.l.
 00000060: 6d09 5a09 0100 6400 6406 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 0100 6400 6407 6c0c 6d0d 5a0d 0100 6400  ..d.d.l.m.Z...d.
-00000080: 6408 6c0e 6d0f 5a0f 0100 6400 6409 6c10  d.l.m.Z...d.d.l.
-00000090: 6d11 5a11 6d12 5a12 0100 6400 640a 6c13  m.Z.m.Z...d.d.l.
-000000a0: 6d14 5a14 0100 4700 640b 640c 8400 640c  m.Z...G.d.d...d.
-000000b0: 8302 5a15 4700 640d 640e 8400 640e 6515  ..Z.G.d.d...d.e.
-000000c0: 8303 5a16 4700 640f 6410 8400 6410 6515  ..Z.G.d.d...d.e.
-000000d0: 8303 5a17 4700 6411 6412 8400 6412 6515  ..Z.G.d.d...d.e.
-000000e0: 8303 5a18 4700 6413 6414 8400 6414 6515  ..Z.G.d.d...d.e.
-000000f0: 8303 5a19 4700 6415 6416 8400 6416 6515  ..Z.G.d.d...d.e.
-00000100: 8303 5a1a 4700 6417 6418 8400 6418 651a  ..Z.G.d.d...d.e.
-00000110: 8303 5a1b 4700 6419 641a 8400 641a 651a  ..Z.G.d.d...d.e.
-00000120: 8303 5a1c 641b 5300 291c e900 0000 0029  ..Z.d.S.)......)
-00000130: 02da 084a 6f69 6e54 7970 65da 054f 7264  ...JoinType..Ord
-00000140: 6572 2901 da0f 506f 7374 6772 6553 514c  er)...PostgreSQL
-00000150: 5175 6572 7929 01da 0554 6162 6c65 2901  Query)...Table).
-00000160: da05 436f 756e 7429 01da 0666 6965 6c64  ..Count)...field
-00000170: 7329 01da 0941 6767 7265 6761 7465 2901  s)...Aggregate).
-00000180: da11 4261 7365 4442 4173 796e 6343 6c69  ..BaseDBAsyncCli
-00000190: 656e 7429 01da 0a46 6965 6c64 4572 726f  ent)...FieldErro
-000001a0: 7229 02da 0850 7265 6665 7463 68da 0151  r)...Prefetch..Q
-000001b0: 2901 da14 4173 796e 6349 7465 7261 746f  )...AsyncIterato
-000001c0: 7257 7261 7070 6572 6300 0000 0000 0000  rWrapperc.......
-000001d0: 0000 0000 0002 0000 0040 0000 0073 4400  .........@...sD.
-000001e0: 0000 6500 5a01 6400 5a02 6401 6402 8400  ..e.Z.d.Z.d.d...
-000001f0: 5a03 6403 6404 8400 5a04 6405 6406 8400  Z.d.d...Z.d.d...
-00000200: 5a05 6407 6408 8400 5a06 6409 640a 8400  Z.d.d...Z.d.d...
-00000210: 5a07 640b 640c 8400 5a08 640d 640e 8400  Z.d.d...Z.d.d...
-00000220: 5a09 640f 5300 2910 da0e 4177 6169 7461  Z.d.S.)...Awaita
-00000230: 626c 6551 7565 7279 6301 0000 0000 0000  bleQueryc.......
-00000240: 0001 0000 0002 0000 0043 0000 0073 1600  .........C...s..
-00000250: 0000 6700 7c00 5f00 6400 7c00 5f01 6400  ..g.|._.d.|._.d.
-00000260: 7c00 5f02 6400 5300 2901 4e29 03da 0e5f  |._.d.S.).N)..._
-00000270: 6a6f 696e 6564 5f74 6162 6c65 73da 0571  joined_tables..q
-00000280: 7565 7279 da05 6d6f 6465 6c29 01da 0473  uery..model)...s
-00000290: 656c 66a9 0072 1300 0000 fa45 2f55 7365  elf..r.....E/Use
-000002a0: 7273 2f61 6e64 7265 7962 6f6e 6461 722f  rs/andreybondar/
-000002b0: 5079 4368 6172 6d50 726f 6a65 6374 732f  PyCharmProjects/
-000002c0: 746f 7274 6f69 7365 2d6f 726d 2f74 6f72  tortoise-orm/tor
-000002d0: 746f 6973 652f 7175 6572 7973 6574 2e70  toise/queryset.p
-000002e0: 79da 085f 5f69 6e69 745f 5f0f 0000 0073  y..__init__....s
-000002f0: 0600 0000 0001 0601 0601 7a17 4177 6169  ..........z.Awai
-00000300: 7461 626c 6551 7565 7279 2e5f 5f69 6e69  tableQuery.__ini
-00000310: 745f 5f63 0400 0000 0000 0000 0400 0000  t__c............
-00000320: 0600 0000 4300 0000 736a 0000 007c 0264  ....C...sj...|.d
-00000330: 0119 007c 006a 006b 0772 407c 006a 016a  ...|.j.k.r@|.j.j
-00000340: 027c 0264 0119 0074 036a 0464 028d 026a  .|.d...t.j.d...j
-00000350: 057c 016a 0674 077c 0264 0119 007c 0264  .|.j.t.|.d...|.d
-00000360: 0319 0083 026b 0283 017c 005f 017c 006a  .....k...|._.|.j
-00000370: 016a 087c 0264 0419 0074 077c 0264 0119  .j.|.d...t.|.d..
-00000380: 007c 0264 0519 0083 027c 0383 0283 017c  .|.d.....|.....|
-00000390: 005f 0164 0053 0029 064e da05 7461 626c  ._.d.S.).N..tabl
-000003a0: 6529 01da 0368 6f77 da0c 6261 636b 7761  e)...how..backwa
-000003b0: 7264 5f6b 6579 da08 6f70 6572 6174 6f72  rd_key..operator
-000003c0: da05 6669 656c 6429 0972 0f00 0000 7210  ..field).r....r.
-000003d0: 0000 00da 046a 6f69 6e72 0200 0000 da0a  .....joinr......
-000003e0: 6c65 6674 5f6f 7574 6572 da02 6f6e da02  left_outer..on..
-000003f0: 6964 da07 6765 7461 7474 72da 0577 6865  id..getattr..whe
-00000400: 7265 2904 7212 0000 0072 1600 0000 da05  re).r....r......
-00000410: 7061 7261 6dda 0576 616c 7565 7213 0000  param..valuer...
-00000420: 0072 1300 0000 7214 0000 00da 1a5f 6669  .r....r......_fi
-00000430: 6c74 6572 5f66 726f 6d5f 7265 6c61 7465  lter_from_relate
-00000440: 645f 7461 626c 6514 0000 0073 0c00 0000  d_table....s....
-00000450: 0001 0e01 0601 1001 1c01 0601 7a29 4177  ............z)Aw
-00000460: 6169 7461 626c 6551 7565 7279 2e5f 6669  aitableQuery._fi
-00000470: 6c74 6572 5f66 726f 6d5f 7265 6c61 7465  lter_from_relate
-00000480: 645f 7461 626c 6563 0700 0000 0000 0000  d_tablec........
-00000490: 1400 0000 0700 0000 4300 0000 7366 0100  ........C...sf..
-000004a0: 0074 007c 016a 016a 0283 017d 0778 767c  .t.|.j.j...}.xv|
-000004b0: 0344 005d 6e7d 087c 086a 037c 0183 015c  .D.]n}.|.j.|...\
-000004c0: 027d 097d 0a78 4c7c 0a44 005d 447d 0b7c  .}.}.xL|.D.]D}.|
-000004d0: 0b64 0119 007c 006a 046b 0772 2a7c 006a  .d...|.j.k.r*|.j
-000004e0: 056a 067c 0b64 0119 0074 076a 0864 028d  .j.|.d...t.j.d..
-000004f0: 026a 097c 0b64 0319 0083 017c 005f 057c  .j.|.d.....|._.|
-00000500: 006a 046a 0a7c 0b64 0119 0083 0101 0071  .j.j.|.d.......q
-00000510: 2a57 007c 006a 056a 0b7c 0983 017c 005f  *W.|.j.j.|...|._
-00000520: 0571 1257 0078 887c 026a 0c83 0044 005d  .q.W.x.|.j...D.]
-00000530: 7c5c 027d 0c7d 0d7c 016a 016a 0d7c 0c19  |\.}.}.|.j.j.|..
-00000540: 007d 0e7c 0e6a 0e64 0483 0172 bc7c 006a  .}.|.j.d...r.|.j
-00000550: 0f7c 077c 0e7c 0d83 0301 0071 8e7c 016a  .|.|.|.....q.|.j
-00000560: 016a 107c 0e64 0519 0019 007d 0f7c 0e6a  .j.|.d.....}.|.j
-00000570: 0e64 0683 0172 de7c 0e64 0619 006e 047c  .d...r.|.d...n.|
-00000580: 0f6a 117d 107c 006a 056a 0b7c 0e64 0719  .j.}.|.j.j.|.d..
-00000590: 0074 127c 077c 0e64 0519 0083 027c 107c  .t.|.|.d.....|.|
-000005a0: 0d83 0183 0283 017c 005f 0571 8e57 0078  .......|._.q.W.x
-000005b0: 527c 046a 0c83 0044 005d 465c 027d 0c7d  R|.j...D.]F\.}.}
-000005c0: 0d7c 067c 0c19 007d 117c 057c 1164 0519  .|.|...}.|.|.d..
-000005d0: 0019 007d 127c 126a 037c 006a 1383 017d  ...}.|.j.|.j...}
-000005e0: 137c 006a 056a 147c 1164 0719 007c 1364  .|.j.j.|.d...|.d
-000005f0: 0519 007c 0d83 0283 017c 005f 0590 0171  ...|.....|._...q
-00000600: 1857 0064 0053 0029 084e 7201 0000 0029  .W.d.S.).Nr....)
-00000610: 0172 1700 0000 e901 0000 0072 1600 0000  .r.........r....
-00000620: 721a 0000 00da 0d76 616c 7565 5f65 6e63  r......value_enc
-00000630: 6f64 6572 7219 0000 0029 1572 0500 0000  oderr....).r....
-00000640: da05 5f6d 6574 6172 1600 0000 da11 7265  .._metar......re
-00000650: 736f 6c76 655f 666f 725f 6d6f 6465 6c72  solve_for_modelr
-00000660: 0f00 0000 7210 0000 0072 1b00 0000 7202  ....r....r....r.
-00000670: 0000 0072 1c00 0000 721d 0000 00da 0661  ...r....r......a
-00000680: 7070 656e 6472 2000 0000 da05 6974 656d  ppendr .....item
-00000690: 73da 0766 696c 7465 7273 da03 6765 7472  s..filters..getr
-000006a0: 2300 0000 da0a 6669 656c 6473 5f6d 6170  #.....fields_map
-000006b0: da0b 746f 5f64 625f 7661 6c75 6572 1f00  ..to_db_valuer..
-000006c0: 0000 7211 0000 00da 0668 6176 696e 6729  ..r......having)
-000006d0: 1472 1200 0000 7211 0000 00da 0d66 696c  .r....r......fil
-000006e0: 7465 725f 6b77 6172 6773 da09 715f 6f62  ter_kwargs..q_ob
-000006f0: 6a65 6374 7372 2e00 0000 da0b 616e 6e6f  jectsr......anno
-00000700: 7461 7469 6f6e 73da 0e63 7573 746f 6d5f  tations..custom_
-00000710: 6669 6c74 6572 7372 1600 0000 da04 6e6f  filtersr......no
-00000720: 6465 da09 6372 6974 6572 696f 6e5a 0e72  de..criterionZ.r
-00000730: 6571 7569 7265 645f 6a6f 696e 7372 1b00  equired_joinsr..
-00000740: 0000 da03 6b65 7972 2200 0000 7221 0000  ....keyr"...r!..
-00000750: 00da 0c66 6965 6c64 5f6f 626a 6563 7472  ...field_objectr
-00000760: 2500 0000 5a0b 6861 7669 6e67 5f69 6e66  %...Z.having_inf
-00000770: 6fda 0b61 6767 7265 6761 7469 6f6e da10  o..aggregation..
-00000780: 6167 6772 6567 6174 696f 6e5f 696e 666f  aggregation_info
-00000790: 7213 0000 0072 1300 0000 7214 0000 00da  r....r....r.....
-000007a0: 0f72 6573 6f6c 7665 5f66 696c 7465 7273  .resolve_filters
-000007b0: 1d00 0000 732c 0000 0000 010c 010a 010e  ....s,..........
-000007c0: 010a 010e 0122 0114 0112 0112 010c 010a  ....."..........
-000007d0: 0110 0210 0318 0206 0124 0212 0108 010c  .........$......
-000007e0: 010c 0106 017a 1e41 7761 6974 6162 6c65  .....z.Awaitable
-000007f0: 5175 6572 792e 7265 736f 6c76 655f 6669  Query.resolve_fi
-00000800: 6c74 6572 7363 0400 0000 0000 0000 0700  ltersc..........
-00000810: 0000 0500 0000 4300 0000 7356 0100 0074  ......C...sV...t
-00000820: 007c 0374 016a 0283 0272 a274 037c 036a  .|.t.j...r.t.|.j
-00000830: 046a 056a 0683 017d 0474 037c 036a 0783  .j.j...}.t.|.j..
-00000840: 017d 057c 057c 006a 086b 0772 627c 006a  .}.|.|.j.k.rb|.j
-00000850: 096a 0a7c 0574 0b6a 0c64 018d 026a 0d7c  .j.|.t.j.d...j.|
-00000860: 016a 0e74 0f7c 057c 036a 1083 026b 0283  .j.t.|.|.j...k..
-00000870: 017c 005f 097c 006a 086a 117c 0583 0101  .|._.|.j.j.|....
-00000880: 007c 047c 006a 086b 0772 a07c 006a 096a  .|.|.j.k.r.|.j.j
-00000890: 0a7c 0474 0b6a 0c64 018d 026a 0d74 0f7c  .|.t.j.d...j.t.|
-000008a0: 057c 036a 1283 027c 046a 0e6b 0283 017c  .|.j...|.j.k...|
-000008b0: 005f 097c 006a 086a 117c 0483 0101 006e  ._.|.j.j.|.....n
-000008c0: b074 007c 0374 016a 1383 0272 fc74 037c  .t.|.t.j...r.t.|
-000008d0: 036a 046a 056a 0683 017d 047c 047c 006a  .j.j.j...}.|.|.j
-000008e0: 086b 0772 fa7c 006a 096a 0a7c 0474 0b6a  .k.r.|.j.j.|.t.j
-000008f0: 0c64 018d 026a 0d7c 016a 0e74 0f7c 047c  .d...j.|.j.t.|.|
-00000900: 036a 1483 026b 0283 017c 005f 097c 006a  .j...k...|._.|.j
-00000910: 086a 117c 0483 0101 006e 5674 037c 036a  .j.|.....nVt.|.j
-00000920: 046a 056a 0683 017d 047c 047c 006a 086b  .j.j...}.|.|.j.k
-00000930: 0790 0172 5264 026a 157c 0283 017d 067c  ...rRd.j.|...}.|
-00000940: 006a 096a 0a7c 0474 0b6a 0c64 018d 026a  .j.j.|.t.j.d...j
-00000950: 0d7c 046a 0e74 0f7c 017c 0683 026b 0283  .|.j.t.|.|...k..
-00000960: 017c 005f 097c 006a 086a 117c 0483 0101  .|._.|.j.j.|....
-00000970: 0064 0053 0029 034e 2901 7217 0000 007a  .d.S.).N).r....z
-00000980: 057b 7d5f 6964 2916 da0a 6973 696e 7374  .{}_id)...isinst
-00000990: 616e 6365 7207 0000 00da 0f4d 616e 7954  ancer......ManyT
-000009a0: 6f4d 616e 7946 6965 6c64 7205 0000 00da  oManyFieldr.....
-000009b0: 0474 7970 6572 2600 0000 7216 0000 00da  .typer&...r.....
-000009c0: 0774 6872 6f75 6768 720f 0000 0072 1000  .throughr....r..
-000009d0: 0000 721b 0000 0072 0200 0000 721c 0000  ..r....r....r...
-000009e0: 0072 1d00 0000 721e 0000 0072 1f00 0000  .r....r....r....
-000009f0: 7218 0000 0072 2800 0000 da0b 666f 7277  r....r(.....forw
-00000a00: 6172 645f 6b65 79da 1242 6163 6b77 6172  ard_key..Backwar
-00000a10: 6446 4b52 656c 6174 696f 6eda 0e72 656c  dFKRelation..rel
-00000a20: 6174 696f 6e5f 6669 656c 64da 0666 6f72  ation_field..for
-00000a30: 6d61 7429 0772 1200 0000 7216 0000 00da  mat).r....r.....
-00000a40: 1272 656c 6174 6564 5f66 6965 6c64 5f6e  .related_field_n
-00000a50: 616d 65da 0d72 656c 6174 6564 5f66 6965  ame..related_fie
-00000a60: 6c64 da0d 7265 6c61 7465 645f 7461 626c  ld..related_tabl
-00000a70: 65da 0d74 6872 6f75 6768 5f74 6162 6c65  e..through_table
-00000a80: 5a15 7265 6c61 7465 645f 6964 5f66 6965  Z.related_id_fie
-00000a90: 6c64 5f6e 616d 6572 1300 0000 7213 0000  ld_namer....r...
-00000aa0: 0072 1400 0000 da14 5f6a 6f69 6e5f 7461  .r......_join_ta
-00000ab0: 626c 655f 6279 5f66 6965 6c64 3b00 0000  ble_by_field;...
-00000ac0: 7336 0000 0000 010c 010e 010a 010a 0106  s6..............
-00000ad0: 010c 0116 010c 010a 0106 010c 0116 010e  ................
-00000ae0: 010c 010e 010a 0106 010c 0116 010e 020e  ................
-00000af0: 010c 010a 0106 010c 0114 017a 2341 7761  ...........z#Awa
-00000b00: 6974 6162 6c65 5175 6572 792e 5f6a 6f69  itableQuery._joi
-00000b10: 6e5f 7461 626c 655f 6279 5f66 6965 6c64  n_table_by_field
-00000b20: 6304 0000 0000 0000 000b 0000 0007 0000  c...............
-00000b30: 0043 0000 0073 2601 0000 7400 7c01 6a01  .C...s&...t.|.j.
-00000b40: 6a02 8301 7d04 9001 7812 7c02 4400 9001  j...}...x.|.D...
-00000b50: 5d08 7d05 7c05 6401 1900 7d06 7c06 7c01  ].}.|.d...}.|.|.
-00000b60: 6a01 6a03 6b06 7238 7404 6402 8301 8201  j.j.k.r8t.d.....
-00000b70: 7114 7c06 6a05 6403 8301 6401 1900 7c01  q.|.j.d...d...|.
-00000b80: 6a01 6a03 6b06 72a6 7c06 6a05 6403 8301  j.j.k.r.|.j.d...
-00000b90: 6401 1900 7d07 7c01 6a01 6a06 7c07 1900  d...}.|.j.j.|...
-00000ba0: 7d08 7c00 6a07 7c04 7c07 7c08 8303 0100  }.|.j.|.|.|.....
-00000bb0: 7c00 6a08 7c08 6a09 6403 6a0a 7c06 6a05  |.j.|.j.d.j.|.j.
-00000bc0: 6403 8301 6404 6400 8502 1900 8301 7c05  d...d.d.......|.
-00000bd0: 6404 1900 6602 6701 6900 8303 0100 7114  d...f.g.i.....q.
-00000be0: 7c06 7c03 6b06 72de 7c03 7c06 1900 7d09  |.|.k.r.|.|...}.
-00000bf0: 7c09 6a0b 7c00 6a0c 8301 7d0a 7c00 6a0d  |.j.|.j...}.|.j.
-00000c00: 6a0e 7c0a 6405 1900 7c05 6404 1900 6406  j.|.d...|.d...d.
-00000c10: 8d02 7c00 5f0d 7114 7c06 7c01 6a01 6a0f  ..|._.q.|.|.j.j.
-00000c20: 6b07 72fe 7410 6407 6a11 7c06 7c00 6a0c  k.r.t.d.j.|.|.j.
-00000c30: 6a12 8302 8301 8201 7c00 6a0d 6a0e 7413  j.......|.j.j.t.
-00000c40: 7c04 7c05 6401 1900 8302 7c05 6404 1900  |.|.d.....|.d...
-00000c50: 6406 8d02 7c00 5f0d 7114 5700 6400 5300  d...|._.q.W.d.S.
-00000c60: 2908 4e72 0100 0000 7a4d 4669 6c74 6572  ).Nr....zMFilter
-00000c70: 696e 6720 6279 2072 656c 6174 696f 6e20  ing by relation 
-00000c80: 6973 206e 6f74 2070 6f73 7369 626c 6520  is not possible 
-00000c90: 6669 6c74 6572 2062 7920 6e65 7374 6564  filter by nested
-00000ca0: 2066 6965 6c64 206f 6620 7265 6c61 7465   field of relate
-00000cb0: 6420 6d6f 6465 6cda 025f 5f72 2400 0000  d model..__r$...
-00000cc0: 721a 0000 0029 01da 056f 7264 6572 7a1d  r....)...orderz.
-00000cd0: 556e 6b6e 6f77 6e20 6669 656c 6420 7b7d  Unknown field {}
-00000ce0: 2066 6f72 206d 6f64 656c 207b 7d29 1472   for model {}).r
-00000cf0: 0500 0000 7226 0000 0072 1600 0000 da0c  ....r&...r......
-00000d00: 6665 7463 685f 6669 656c 6473 da0a 5661  fetch_fields..Va
-00000d10: 6c75 6545 7272 6f72 da05 7370 6c69 7472  lueError..splitr
-00000d20: 2c00 0000 7246 0000 00da 1072 6573 6f6c  ,...rF.....resol
-00000d30: 7665 5f6f 7264 6572 696e 6772 3c00 0000  ve_orderingr<...
-00000d40: 721b 0000 0072 2700 0000 7211 0000 0072  r....r'...r....r
-00000d50: 1000 0000 da07 6f72 6465 7262 7972 0700  ......orderbyr..
-00000d60: 0000 720a 0000 0072 4100 0000 da08 5f5f  ..r....rA.....__
-00000d70: 6e61 6d65 5f5f 721f 0000 0029 0b72 1200  name__r....).r..
-00000d80: 0000 7211 0000 00da 096f 7264 6572 696e  ..r......orderin
-00000d90: 6773 7231 0000 0072 1600 0000 da08 6f72  gsr1...r......or
-00000da0: 6465 7269 6e67 da0a 6669 656c 645f 6e61  dering..field_na
-00000db0: 6d65 7242 0000 0072 4300 0000 7237 0000  merB...rC...r7..
-00000dc0: 0072 3800 0000 7213 0000 0072 1300 0000  .r8...r....r....
-00000dd0: 7214 0000 0072 4c00 0000 5900 0000 732c  r....rL...Y...s,
-00000de0: 0000 0000 010c 010e 0108 010c 0102 0108  ................
-00000df0: 0216 010e 010c 010e 0104 012c 0208 0108  ...........,....
-00000e00: 010c 011c 020c 0102 0104 0102 010c 037a  ...............z
-00000e10: 1f41 7761 6974 6162 6c65 5175 6572 792e  .AwaitableQuery.
-00000e20: 7265 736f 6c76 655f 6f72 6465 7269 6e67  resolve_ordering
-00000e30: 6301 0000 0000 0000 0001 0000 0001 0000  c...............
-00000e40: 0043 0000 0073 0c00 0000 7c00 6a00 8300  .C...s....|.j...
-00000e50: 6a01 8300 5300 2901 4e29 02da 085f 6578  j...S.).N)..._ex
-00000e60: 6563 7574 65da 095f 5f61 7761 6974 5f5f  ecute..__await__
-00000e70: 2901 7212 0000 0072 1300 0000 7213 0000  ).r....r....r...
-00000e80: 0072 1400 0000 7253 0000 0076 0000 0073  .r....rS...v...s
-00000e90: 0200 0000 0001 7a18 4177 6169 7461 626c  ......z.Awaitabl
-00000ea0: 6551 7565 7279 2e5f 5f61 7761 6974 5f5f  eQuery.__await__
-00000eb0: 6301 0000 0000 0000 0001 0000 0001 0000  c...............
-00000ec0: 00c3 0000 0073 0a00 0000 7400 8300 8201  .....s....t.....
-00000ed0: 6400 5300 2901 4e29 01da 134e 6f74 496d  d.S.).N)...NotIm
-00000ee0: 706c 656d 656e 7465 6445 7272 6f72 2901  plementedError).
-00000ef0: 7212 0000 0072 1300 0000 7213 0000 0072  r....r....r....r
-00000f00: 1400 0000 7252 0000 0079 0000 0073 0200  ....rR...y...s..
-00000f10: 0000 0001 7a17 4177 6169 7461 626c 6551  ....z.AwaitableQ
-00000f20: 7565 7279 2e5f 6578 6563 7574 654e 290a  uery._executeN).
-00000f30: 724e 0000 00da 0a5f 5f6d 6f64 756c 655f  rN.....__module_
-00000f40: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5f72  _..__qualname__r
-00000f50: 1500 0000 7223 0000 0072 3900 0000 7246  ....r#...r9...rF
-00000f60: 0000 0072 4c00 0000 7253 0000 0072 5200  ...rL...rS...rR.
-00000f70: 0000 7213 0000 0072 1300 0000 7213 0000  ..r....r....r...
-00000f80: 0072 1400 0000 720e 0000 000e 0000 0073  .r....r........s
-00000f90: 0e00 0000 0801 0805 0809 081e 081e 081d  ................
-00000fa0: 0803 720e 0000 0063 0000 0000 0000 0000  ..r....c........
-00000fb0: 0000 0000 0300 0000 0000 0000 73d0 0000  ............s...
-00000fc0: 0065 005a 0164 005a 0287 0066 0164 0164  .e.Z.d.Z...f.d.d
-00000fd0: 0284 085a 0364 0364 0484 005a 0464 0564  ...Z.d.d...Z.d.d
-00000fe0: 0684 005a 0564 0764 0884 005a 0664 0964  ...Z.d.d...Z.d.d
-00000ff0: 0a84 005a 0764 0b64 0c84 005a 0864 0d64  ...Z.d.d...Z.d.d
-00001000: 0e84 005a 0964 0f64 1084 005a 0a64 1164  ...Z.d.d...Z.d.d
-00001010: 129c 0164 1364 1484 025a 0b64 1564 1684  ...d.d...Z.d.d..
-00001020: 005a 0c64 1764 1884 005a 0d64 1964 1a84  .Z.d.d...Z.d.d..
-00001030: 005a 0e64 1b64 1c84 005a 0f64 1d64 1e84  .Z.d.d...Z.d.d..
-00001040: 005a 1064 1f64 2084 005a 1164 2164 2284  .Z.d.d ..Z.d!d".
-00001050: 005a 1264 2364 2484 005a 1365 1464 259c  .Z.d#d$..Z.e.d%.
-00001060: 0164 2664 2784 045a 1564 2864 2984 005a  .d&d'..Z.d(d)..Z
-00001070: 1664 2a64 2b84 005a 1764 2c64 2d84 005a  .d*d+..Z.d,d-..Z
-00001080: 1864 2e64 2f84 005a 1987 0004 005a 1a53  .d.d/..Z.....Z.S
-00001090: 0029 30da 0851 7565 7279 5365 7463 0200  .)0..QuerySetc..
-000010a0: 0000 0000 0000 0200 0000 0200 0000 0300  ................
-000010b0: 0000 7388 0000 0074 0083 006a 0183 0001  ..s....t...j....
-000010c0: 007c 016a 026a 037c 005f 047c 017c 005f  .|.j.j.|._.|.|._
-000010d0: 0574 066a 077c 016a 026a 0883 017c 005f  .t.j.|.j.j...|._
-000010e0: 0969 007c 005f 0a69 007c 005f 0b64 017c  .i.|._.i.|._.d.|
-000010f0: 005f 0c64 017c 005f 0d64 007c 005f 0e64  ._.d.|._.d.|._.d
-00001100: 007c 005f 0f64 007c 005f 1069 007c 005f  .|._.d.|._.i.|._
-00001110: 1167 007c 005f 1267 007c 005f 1367 007c  .g.|._.g.|._.g.|
-00001120: 005f 1464 017c 005f 1569 007c 005f 1669  ._.d.|._.i.|._.i
-00001130: 007c 005f 1769 007c 005f 1864 0053 0029  .|._.i.|._.d.S.)
-00001140: 024e 4629 19da 0573 7570 6572 7215 0000  .NF)...superr...
-00001150: 0072 2600 0000 da09 6462 5f66 6965 6c64  .r&.....db_field
-00001160: 7372 0700 0000 7211 0000 00da 0551 7565  sr....r......Que
-00001170: 7279 da05 6672 6f6d 5f72 1600 0000 7210  ry..from_r....r.
-00001180: 0000 00da 0d5f 7072 6566 6574 6368 5f6d  ....._prefetch_m
-00001190: 6170 da11 5f70 7265 6665 7463 685f 7175  ap.._prefetch_qu
-000011a0: 6572 6965 73da 075f 7369 6e67 6c65 da06  eries.._single..
-000011b0: 5f63 6f75 6e74 da03 5f64 62da 065f 6c69  _count.._db.._li
-000011c0: 6d69 74da 075f 6f66 6673 6574 da0e 5f66  mit.._offset.._f
-000011d0: 696c 7465 725f 6b77 6172 6773 da0a 5f6f  ilter_kwargs.._o
-000011e0: 7264 6572 696e 6773 720f 0000 00da 165f  rderingsr......_
-000011f0: 715f 6f62 6a65 6374 735f 666f 725f 7265  q_objects_for_re
-00001200: 736f 6c76 65da 095f 6469 7374 696e 6374  solve.._distinct
-00001210: da0c 5f61 6e6e 6f74 6174 696f 6e73 da07  .._annotations..
-00001220: 5f68 6176 696e 67da 195f 6176 6169 6c61  _having.._availa
-00001230: 626c 655f 6375 7374 6f6d 5f66 696c 7465  ble_custom_filte
-00001240: 7273 2902 7212 0000 0072 1100 0000 2901  rs).r....r....).
-00001250: da09 5f5f 636c 6173 735f 5f72 1300 0000  ..__class__r....
-00001260: 7214 0000 0072 1500 0000 7e00 0000 7326  r....r....~...s&
-00001270: 0000 0000 010a 010a 0106 0110 0106 0106  ................
-00001280: 0106 0106 0106 0106 0106 0106 0106 0106  ................
-00001290: 0106 0106 0106 0106 017a 1151 7565 7279  .........z.Query
-000012a0: 5365 742e 5f5f 696e 6974 5f5f 6301 0000  Set.__init__c...
-000012b0: 0000 0000 0002 0000 0002 0000 0043 0000  .............C..
-000012c0: 0073 9800 0000 7c00 6a00 7c00 6a01 8301  .s....|.j.|.j...
-000012d0: 7d01 7c00 6a02 7c01 5f02 7c00 6a03 7c01  }.|.j.|._.|.j.|.
-000012e0: 5f03 7c00 6a04 7c01 5f04 7c00 6a05 7c01  _.|.j.|._.|.j.|.
-000012f0: 5f05 7c00 6a06 7c01 5f06 7c00 6a07 7c01  _.|.j.|._.|.j.|.
-00001300: 5f07 7c00 6a08 7c01 5f08 7409 7c00 6a0a  _.|.j.|._.t.|.j.
-00001310: 8301 7c01 5f0a 740b 7c00 6a0c 8301 7c01  ..|._.t.|.j...|.
-00001320: 5f0c 740b 7c00 6a0d 8301 7c01 5f0d 740b  _.t.|.j...|._.t.
-00001330: 7c00 6a0e 8301 7c01 5f0e 7c00 6a0f 7c01  |.j...|._.|.j.|.
-00001340: 5f0f 7c00 6a10 7c01 5f10 7c00 6a11 7c01  _.|.j.|._.|.j.|.
-00001350: 5f11 7c00 6a12 7c01 5f12 7c01 5300 2901  _.|.j.|._.|.S.).
-00001360: 4e29 1372 6a00 0000 7211 0000 0072 5c00  N).rj...r....r\.
-00001370: 0000 725d 0000 0072 5e00 0000 725f 0000  ..r]...r^...r_..
-00001380: 0072 6000 0000 7261 0000 0072 6200 0000  .r`...ra...rb...
-00001390: da04 6469 6374 7263 0000 00da 046c 6973  ..dictrc.....lis
-000013a0: 7472 6400 0000 720f 0000 0072 6500 0000  trd...r....re...
-000013b0: 7266 0000 0072 6700 0000 7268 0000 0072  rf...rg...rh...r
-000013c0: 6900 0000 2902 7212 0000 00da 0871 7565  i...).r......que
-000013d0: 7279 7365 7472 1300 0000 7213 0000 0072  rysetr....r....r
-000013e0: 1400 0000 da06 5f63 6c6f 6e65 9300 0000  ......_clone....
-000013f0: 7322 0000 0000 010c 0108 0108 0108 0108  s"..............
-00001400: 0108 0108 0108 010c 010c 010c 010c 0108  ................
-00001410: 0108 0108 0108 017a 0f51 7565 7279 5365  .......z.QuerySe
-00001420: 742e 5f63 6c6f 6e65 6301 0000 0000 0000  t._clonec.......
-00001430: 0008 0000 0006 0000 004f 0000 0073 e800  .........O...s..
-00001440: 0000 7c00 6a00 8300 7d03 782a 7c01 4400  ..|.j...}.x*|.D.
-00001450: 5d22 7d04 7401 7c04 7402 8302 7324 7403  ]"}.t.|.t...s$t.
-00001460: 6401 8301 8201 7c03 6a04 6a05 7c04 8301  d.....|.j.j.|...
-00001470: 0100 710e 5700 78ae 7c02 6a06 8300 4400  ..q.W.x.|.j...D.
-00001480: 5da2 5c02 7d05 7d06 7c05 7c03 6a07 6a08  ].\.}.}.|.|.j.j.
-00001490: 6a09 6b06 7260 7c06 7c03 6a0a 7c05 3c00  j.k.r`|.|.j.|.<.
-000014a0: 713e 7c05 7c00 6a07 6a08 6a0b 6b06 728c  q>|.|.j.j.j.k.r.
-000014b0: 7c00 6a07 6a08 6a0c 7c05 1900 7d07 7c06  |.j.j.j.|...}.|.
-000014c0: 6a0d 7c03 6a0a 7c07 6a0e 3c00 713e 7c05  j.|.j.|.j.<.q>|.
-000014d0: 6a0f 6402 8301 6403 1900 7c00 6a07 6a08  j.d...d...|.j.j.
-000014e0: 6a10 6b06 72bc 7c03 6a04 6a05 7402 6600  j.k.r.|.j.j.t.f.
-000014f0: 7c05 7c06 6901 8e01 8301 0100 713e 7c05  |.|.i.......q>|.
-00001500: 7c00 6a11 6b06 72d2 7c06 7c03 6a12 7c05  |.j.k.r.|.|.j.|.
-00001510: 3c00 713e 7413 6404 6a14 7c05 8301 8301  <.q>t.d.j.|.....
-00001520: 8201 713e 5700 7c03 5300 2905 4e7a 1a65  ..q>W.|.S.).Nz.e
-00001530: 7870 6563 7465 6420 5120 6f62 6a65 6374  xpected Q object
-00001540: 7320 6173 2061 7267 7372 4700 0000 7201  s as argsrG...r.
-00001550: 0000 007a 1775 6e6b 6e6f 776e 2066 696c  ...z.unknown fil
-00001560: 7465 7220 7061 7261 6d20 7b7d 2915 726e  ter param {}).rn
-00001570: 0000 0072 3a00 0000 720c 0000 00da 0954  ...r:...r......T
-00001580: 7970 6545 7272 6f72 7265 0000 0072 2800  ypeErrorre...r(.
-00001590: 0000 7229 0000 0072 1100 0000 7226 0000  ..r)...r....r&..
-000015a0: 0072 2a00 0000 7263 0000 00da 0966 6b5f  .r*...rc.....fk_
-000015b0: 6669 656c 6473 722c 0000 0072 1e00 0000  fieldsr,...r....
-000015c0: da0c 736f 7572 6365 5f66 6965 6c64 724b  ..source_fieldrK
-000015d0: 0000 0072 4900 0000 7269 0000 0072 6800  ...rI...ri...rh.
-000015e0: 0000 720a 0000 0072 4100 0000 2908 7212  ..r....rA...).r.
-000015f0: 0000 00da 0461 7267 73da 066b 7761 7267  .....args..kwarg
-00001600: 7372 6d00 0000 da03 6172 6772 3500 0000  srm.....argr5...
-00001610: 7222 0000 0072 3600 0000 7213 0000 0072  r"...r6...r....r
-00001620: 1300 0000 7214 0000 00da 0666 696c 7465  ....r......filte
-00001630: 72a6 0000 0073 2200 0000 0001 0801 0a01  r....s".........
-00001640: 0a01 0801 1001 1201 0e01 0c01 0e01 0e01  ................
-00001650: 1001 1801 1801 0a01 0c02 1201 7a0f 5175  ............z.Qu
-00001660: 6572 7953 6574 2e66 696c 7465 7263 0100  erySet.filterc..
-00001670: 0000 0000 0000 0700 0000 0500 0000 4700  ..............G.
-00001680: 0000 7392 0000 007c 006a 0083 007d 0267  ..s....|.j...}.g
-00001690: 007d 0378 7a7c 0144 005d 727d 0474 016a  .}.xz|.D.]r}.t.j
-000016a0: 027d 057c 0464 0119 0064 026b 0272 3c7c  .}.|.d...d.k.r<|
-000016b0: 0464 0364 0085 0219 007d 0674 016a 037d  .d.d.....}.t.j.}
-000016c0: 056e 047c 047d 067c 066a 0464 0483 0164  .n.|.}.|.j.d...d
-000016d0: 0119 007c 006a 056a 066a 076b 0670 607c  ...|.j.j.j.k.p`|
-000016e0: 067c 006a 086b 0673 7674 0964 056a 0a7c  .|.j.k.svt.d.j.|
-000016f0: 067c 006a 056a 0b83 0283 0182 017c 036a  .|.j.j.......|.j
-00001700: 0c7c 067c 0566 0283 0101 0071 1257 007c  .|.|.f.....q.W.|
-00001710: 037c 025f 0d7c 0253 0029 064e 7201 0000  .|._.|.S.).Nr...
-00001720: 00fa 012d 7224 0000 0072 4700 0000 7a1d  ...-r$...rG...z.
-00001730: 556e 6b6e 6f77 6e20 6669 656c 6420 7b7d  Unknown field {}
-00001740: 2066 6f72 206d 6f64 656c 207b 7d29 0e72   for model {}).r
-00001750: 6e00 0000 7203 0000 00da 0361 7363 da04  n...r......asc..
-00001760: 6465 7363 724b 0000 0072 1100 0000 7226  descrK...r....r&
-00001770: 0000 0072 0700 0000 7267 0000 0072 0a00  ...r....rg...r..
-00001780: 0000 7241 0000 0072 4e00 0000 7228 0000  ..rA...rN...r(..
-00001790: 0072 6400 0000 2907 7212 0000 0072 4f00  .rd...).r....rO.
-000017a0: 0000 726d 0000 005a 0c6e 6577 5f6f 7264  ..rm...Z.new_ord
-000017b0: 6572 696e 6772 5000 0000 5a0a 6f72 6465  eringrP...Z.orde
-000017c0: 725f 7479 7065 7251 0000 0072 1300 0000  r_typerQ...r....
-000017d0: 7213 0000 0072 1400 0000 da08 6f72 6465  r....r......orde
-000017e0: 725f 6279 ba00 0000 7322 0000 0000 0108  r_by....s"......
-000017f0: 0104 010a 0106 010c 010c 0108 0204 0318  ................
-00001800: 010a 0202 0104 0102 010c 0312 0106 017a  ...............z
-00001810: 1151 7565 7279 5365 742e 6f72 6465 725f  .QuerySet.order_
-00001820: 6279 6302 0000 0000 0000 0003 0000 0002  byc.............
-00001830: 0000 0043 0000 0073 1200 0000 7c00 6a00  ...C...s....|.j.
-00001840: 8300 7d02 7c01 7c02 5f01 7c02 5300 2901  ..}.|.|._.|.S.).
-00001850: 4e29 0272 6e00 0000 7261 0000 0029 0372  N).rn...ra...).r
-00001860: 1200 0000 da05 6c69 6d69 7472 6d00 0000  ......limitrm...
-00001870: 7213 0000 0072 1300 0000 7214 0000 0072  r....r....r....r
-00001880: 7a00 0000 d300 0000 7306 0000 0000 0108  z.......s.......
-00001890: 0106 017a 0e51 7565 7279 5365 742e 6c69  ...z.QuerySet.li
-000018a0: 6d69 7463 0200 0000 0000 0000 0300 0000  mitc............
-000018b0: 0200 0000 4300 0000 7312 0000 007c 006a  ....C...s....|.j
-000018c0: 0083 007d 027c 017c 025f 017c 0253 0029  ...}.|.|._.|.S.)
-000018d0: 014e 2902 726e 0000 0072 6200 0000 2903  .N).rn...rb...).
-000018e0: 7212 0000 00da 066f 6666 7365 7472 6d00  r......offsetrm.
-000018f0: 0000 7213 0000 0072 1300 0000 7214 0000  ..r....r....r...
-00001900: 0072 7b00 0000 d800 0000 7306 0000 0000  .r{.......s.....
-00001910: 0108 0106 017a 0f51 7565 7279 5365 742e  .....z.QuerySet.
-00001920: 6f66 6673 6574 6301 0000 0000 0000 0002  offsetc.........
-00001930: 0000 0002 0000 0043 0000 0073 1200 0000  .......C...s....
-00001940: 7c00 6a00 8300 7d01 6401 7c01 5f01 7c01  |.j...}.d.|._.|.
-00001950: 5300 2902 4e54 2902 726e 0000 0072 6600  S.).NT).rn...rf.
-00001960: 0000 2902 7212 0000 0072 6d00 0000 7213  ..).r....rm...r.
-00001970: 0000 0072 1300 0000 7214 0000 00da 0864  ...r....r......d
-00001980: 6973 7469 6e63 74dd 0000 0073 0600 0000  istinct....s....
-00001990: 0001 0801 0601 7a11 5175 6572 7953 6574  ......z.QuerySet
-000019a0: 2e64 6973 7469 6e63 7463 0100 0000 0000  .distinctc......
-000019b0: 0000 0600 0000 0600 0000 4b00 0000 735e  ..........K...s^
-000019c0: 0000 007c 006a 0083 007d 0278 507c 016a  ...|.j...}.xP|.j
-000019d0: 0183 0044 005d 445c 027d 037d 0474 027c  ...D.]D\.}.}.t.|
-000019e0: 0474 0383 0273 2c74 0464 0183 0182 017c  .t...s,t.d.....|
-000019f0: 047c 026a 057c 033c 0064 0264 036c 066d  .|.j.|.<.d.d.l.m
-00001a00: 077d 0501 007c 026a 086a 097c 057c 0364  .}...|.j.j.|.|.d
-00001a10: 007c 0383 0383 0101 0071 1257 007c 0253  .|.......q.W.|.S
-00001a20: 0029 044e 7a2a 7661 6c75 6520 6973 2065  .).Nz*value is e
-00001a30: 7870 6563 7465 6420 746f 2062 6520 4167  xpected to be Ag
-00001a40: 6772 6567 6174 6520 696e 7374 616e 6365  gregate instance
-00001a50: 7201 0000 0029 01da 1567 6574 5f66 696c  r....)...get_fil
-00001a60: 7465 7273 5f66 6f72 5f66 6965 6c64 290a  ters_for_field).
-00001a70: 726e 0000 0072 2900 0000 723a 0000 0072  rn...r)...r:...r
-00001a80: 0800 0000 726f 0000 0072 6700 0000 da0f  ....ro...rg.....
-00001a90: 746f 7274 6f69 7365 2e6d 6f64 656c 7372  tortoise.modelsr
-00001aa0: 7d00 0000 7269 0000 00da 0675 7064 6174  }...ri.....updat
-00001ab0: 6529 0672 1200 0000 7273 0000 0072 6d00  e).r....rs...rm.
-00001ac0: 0000 7235 0000 0072 3700 0000 727d 0000  ..r5...r7...r}..
-00001ad0: 0072 1300 0000 7213 0000 0072 1400 0000  .r....r....r....
-00001ae0: da08 616e 6e6f 7461 7465 e200 0000 7310  ..annotate....s.
-00001af0: 0000 0000 0108 0112 010a 0108 010a 010c  ................
-00001b00: 0118 017a 1151 7565 7279 5365 742e 616e  ...z.QuerySet.an
-00001b10: 6e6f 7461 7465 4629 01da 0466 6c61 7463  notateF)...flatc
-00001b20: 0100 0000 0100 0000 0300 0000 0f00 0000  ................
-00001b30: 4700 0000 7338 0000 0074 007c 006a 017c  G...s8...t.|.j.|
-00001b40: 006a 027c 006a 037c 006a 047c 017c 027c  .j.|.j.|.j.|.|.|
-00001b50: 006a 057c 006a 067c 006a 077c 006a 087c  .j.|.j.|.j.|.j.|
-00001b60: 006a 097c 006a 0a7c 006a 0b64 018d 0d53  .j.|.j.|.j.d...S
-00001b70: 0029 024e 290d da02 6462 7211 0000 0072  .).N)...dbr....r
-00001b80: 2f00 0000 7230 0000 0072 8100 0000 da16  /...r0...r......
-00001b90: 6669 656c 6473 5f66 6f72 5f73 656c 6563  fields_for_selec
-00001ba0: 745f 6c69 7374 727c 0000 0072 7a00 0000  t_listr|...rz...
-00001bb0: 727b 0000 0072 4f00 0000 7231 0000 0072  r{...rO...r1...r
-00001bc0: 2e00 0000 7232 0000 0029 0cda 0f56 616c  ....r2...)...Val
-00001bd0: 7565 734c 6973 7451 7565 7279 7260 0000  uesListQueryr`..
-00001be0: 0072 1100 0000 7263 0000 0072 6500 0000  .r....rc...re...
-00001bf0: 7266 0000 0072 6100 0000 7262 0000 0072  rf...ra...rb...r
-00001c00: 6400 0000 7267 0000 0072 6800 0000 7269  d...rg...rh...ri
-00001c10: 0000 0029 0372 1200 0000 7281 0000 0072  ...).r....r....r
-00001c20: 0700 0000 7213 0000 0072 1300 0000 7214  ....r....r....r.
-00001c30: 0000 00da 0b76 616c 7565 735f 6c69 7374  .....values_list
-00001c40: ec00 0000 731c 0000 0000 0102 0104 0104  ....s...........
-00001c50: 0104 0104 0102 0102 0104 0104 0104 0104  ................
-00001c60: 0104 0104 017a 1451 7565 7279 5365 742e  .....z.QuerySet.
-00001c70: 7661 6c75 6573 5f6c 6973 7463 0100 0000  values_listc....
-00001c80: 0000 0000 0600 0000 0e00 0000 4f00 0000  ............O...
-00001c90: 739a 0000 0069 007d 0378 2a7c 0144 005d  s....i.}.x*|.D.]
-00001ca0: 227d 047c 047c 036b 0672 2474 0064 016a  "}.|.|.k.r$t.d.j
-00001cb0: 017c 0483 0183 0182 017c 047c 037c 043c  .|.......|.|.|.<
-00001cc0: 0071 0a57 0078 327c 026a 0283 0044 005d  .q.W.x2|.j...D.]
-00001cd0: 265c 027d 057d 047c 057c 036b 0672 5874  &\.}.}.|.|.k.rXt
-00001ce0: 0064 016a 017c 0583 0183 0182 017c 047c  .d.j.|.......|.|
-00001cf0: 037c 053c 0071 3a57 0074 037c 006a 047c  .|.<.q:W.t.|.j.|
-00001d00: 006a 057c 006a 067c 006a 077c 037c 006a  .j.|.j.|.j.|.|.j
-00001d10: 087c 006a 097c 006a 0a7c 006a 0b7c 006a  .|.j.|.j.|.j.|.j
-00001d20: 0c7c 006a 0d7c 006a 0e64 028d 0c53 0029  .|.j.|.j.d...S.)
-00001d30: 034e 7a10 4475 706c 6963 6174 6520 6b65  .Nz.Duplicate ke
-00001d40: 7920 7b7d 290c 7282 0000 0072 1100 0000  y {}).r....r....
-00001d50: 722f 0000 0072 3000 0000 da11 6669 656c  r/...r0.....fiel
-00001d60: 6473 5f66 6f72 5f73 656c 6563 7472 7c00  ds_for_selectr|.
-00001d70: 0000 727a 0000 0072 7b00 0000 724f 0000  ..rz...r{...rO..
-00001d80: 0072 3100 0000 722e 0000 0072 3200 0000  .r1...r....r2...
-00001d90: 290f 720a 0000 0072 4100 0000 7229 0000  ).r....rA...r)..
-00001da0: 00da 0b56 616c 7565 7351 7565 7279 7260  ...ValuesQueryr`
-00001db0: 0000 0072 1100 0000 7263 0000 0072 6500  ...r....rc...re.
-00001dc0: 0000 7266 0000 0072 6100 0000 7262 0000  ..rf...ra...rb..
-00001dd0: 0072 6400 0000 7267 0000 0072 6800 0000  .rd...rg...rh...
-00001de0: 7269 0000 0029 0672 1200 0000 7272 0000  ri...).r....rr..
-00001df0: 0072 7300 0000 7286 0000 0072 1a00 0000  .rs...r....r....
-00001e00: da09 7265 7475 726e 5f61 7372 1300 0000  ..return_asr....
-00001e10: 7213 0000 0072 1400 0000 da06 7661 6c75  r....r......valu
-00001e20: 6573 fd00 0000 732c 0000 0000 0104 010a  es....s,........
-00001e30: 0108 010e 010c 0212 0108 010e 010c 0202  ................
-00001e40: 0104 0104 0104 0104 0102 0104 0104 0104  ................
-00001e50: 0104 0104 0104 017a 0f51 7565 7279 5365  .......z.QuerySe
-00001e60: 742e 7661 6c75 6573 6301 0000 0000 0000  t.valuesc.......
-00001e70: 0001 0000 0009 0000 0043 0000 0073 2400  .........C...s$.
-00001e80: 0000 7400 7c00 6a01 7c00 6a02 7c00 6a03  ..t.|.j.|.j.|.j.
-00001e90: 7c00 6a04 7c00 6a05 7c00 6a06 7c00 6a07  |.j.|.j.|.j.|.j.
-00001ea0: 6401 8d07 5300 2902 4e29 0772 8200 0000  d...S.).N).r....
-00001eb0: 7211 0000 0072 2f00 0000 7230 0000 0072  r....r/...r0...r
-00001ec0: 3100 0000 722e 0000 0072 3200 0000 2908  1...r....r2...).
-00001ed0: da0b 4465 6c65 7465 5175 6572 7972 6000  ..DeleteQueryr`.
-00001ee0: 0000 7211 0000 0072 6300 0000 7265 0000  ..r....rc...re..
-00001ef0: 0072 6700 0000 7268 0000 0072 6900 0000  .rg...rh...ri...
-00001f00: 2901 7212 0000 0072 1300 0000 7213 0000  ).r....r....r...
-00001f10: 0072 1400 0000 da06 6465 6c65 7465 1801  .r......delete..
-00001f20: 0000 7310 0000 0000 0102 0104 0104 0104  ..s.............
-00001f30: 0104 0104 0104 017a 0f51 7565 7279 5365  .......z.QuerySe
-00001f40: 742e 6465 6c65 7465 6301 0000 0000 0000  t.deletec.......
-00001f50: 0002 0000 000a 0000 004b 0000 0073 2600  .........K...s&.
-00001f60: 0000 7400 7c00 6a01 7c00 6a02 7c00 6a03  ..t.|.j.|.j.|.j.
-00001f70: 7c01 7c00 6a04 7c00 6a05 7c00 6a06 7c00  |.|.j.|.j.|.j.|.
-00001f80: 6a07 6401 8d08 5300 2902 4e29 0872 8200  j.d...S.).N).r..
-00001f90: 0000 7211 0000 0072 2f00 0000 da0d 7570  ..r....r/.....up
-00001fa0: 6461 7465 5f6b 7761 7267 7372 3000 0000  date_kwargsr0...
-00001fb0: 7231 0000 0072 2e00 0000 7232 0000 0029  r1...r....r2...)
-00001fc0: 08da 0b55 7064 6174 6551 7565 7279 7260  ...UpdateQueryr`
-00001fd0: 0000 0072 1100 0000 7263 0000 0072 6500  ...r....rc...re.
-00001fe0: 0000 7267 0000 0072 6800 0000 7269 0000  ..rg...rh...ri..
-00001ff0: 0029 0272 1200 0000 7273 0000 0072 1300  .).r....rs...r..
-00002000: 0000 7213 0000 0072 1400 0000 727f 0000  ..r....r....r...
-00002010: 0023 0100 0073 1200 0000 0001 0201 0401  .#...s..........
-00002020: 0401 0401 0201 0401 0401 0401 7a0f 5175  ............z.Qu
-00002030: 6572 7953 6574 2e75 7064 6174 6563 0100  erySet.updatec..
-00002040: 0000 0000 0000 0100 0000 0900 0000 4300  ..............C.
-00002050: 0000 7324 0000 0074 007c 006a 017c 006a  ..s$...t.|.j.|.j
-00002060: 027c 006a 037c 006a 047c 006a 057c 006a  .|.j.|.j.|.j.|.j
-00002070: 067c 006a 0764 018d 0753 0029 024e 2907  .|.j.d...S.).N).
-00002080: 7282 0000 0072 1100 0000 722f 0000 0072  r....r....r/...r
-00002090: 3000 0000 7231 0000 0072 2e00 0000 7232  0...r1...r....r2
-000020a0: 0000 0029 08da 0a43 6f75 6e74 5175 6572  ...)...CountQuer
-000020b0: 7972 6000 0000 7211 0000 0072 6300 0000  yr`...r....rc...
-000020c0: 7265 0000 0072 6700 0000 7268 0000 0072  re...rg...rh...r
-000020d0: 6900 0000 2901 7212 0000 0072 1300 0000  i...).r....r....
-000020e0: 7213 0000 0072 1400 0000 da05 636f 756e  r....r......coun
-000020f0: 742f 0100 0073 1000 0000 0001 0201 0401  t/...s..........
-00002100: 0401 0401 0401 0401 0401 7a0e 5175 6572  ..........z.Quer
-00002110: 7953 6574 2e63 6f75 6e74 6301 0000 0000  ySet.countc.....
-00002120: 0000 0001 0000 0001 0000 0043 0000 0073  ...........C...s
-00002130: 0800 0000 7c00 6a00 8300 5300 2901 4e29  ....|.j...S.).N)
-00002140: 0172 6e00 0000 2901 7212 0000 0072 1300  .rn...).r....r..
-00002150: 0000 7213 0000 0072 1400 0000 da03 616c  ..r....r......al
-00002160: 6c3a 0100 0073 0200 0000 0001 7a0c 5175  l:...s......z.Qu
-00002170: 6572 7953 6574 2e61 6c6c 6301 0000 0000  erySet.allc.....
-00002180: 0000 0002 0000 0002 0000 0043 0000 0073  ...........C...s
-00002190: 1800 0000 7c00 6a00 8300 7d01 6401 7c01  ....|.j...}.d.|.
-000021a0: 5f01 6402 7c01 5f02 7c01 5300 2903 4e72  _.d.|._.|.S.).Nr
-000021b0: 2400 0000 5429 0372 6e00 0000 7261 0000  $...T).rn...ra..
-000021c0: 0072 5e00 0000 2902 7212 0000 0072 6d00  .r^...).r....rm.
-000021d0: 0000 7213 0000 0072 1300 0000 7214 0000  ..r....r....r...
-000021e0: 00da 0566 6972 7374 3d01 0000 7308 0000  ...first=...s...
-000021f0: 0000 0108 0106 0106 017a 0e51 7565 7279  .........z.Query
-00002200: 5365 742e 6669 7273 7463 0300 0000 0000  Set.firstc......
-00002210: 0000 0300 0000 0100 0000 4300 0000 7304  ..........C...s.
-00002220: 0000 0064 0053 0029 014e 7213 0000 0029  ...d.S.).Nr....)
-00002230: 0372 1200 0000 726d 0000 005a 0870 7265  .r....rm...Z.pre
-00002240: 6665 7463 6872 1300 0000 7213 0000 0072  fetchr....r....r
-00002250: 1400 0000 da18 5f72 6573 6f6c 7665 5f70  ......_resolve_p
-00002260: 7265 6665 7463 685f 6f62 6a65 6374 4301  refetch_objectC.
-00002270: 0000 7302 0000 0000 017a 2151 7565 7279  ..s......z!Query
-00002280: 5365 742e 5f72 6573 6f6c 7665 5f70 7265  Set._resolve_pre
-00002290: 6665 7463 685f 6f62 6a65 6374 6301 0000  fetch_objectc...
-000022a0: 0000 0000 0007 0000 0005 0000 0047 0000  .............G..
-000022b0: 0073 ac00 0000 7c00 6a00 8300 7d02 6900  .s....|.j...}.i.
-000022c0: 7c02 5f01 7898 7c01 4400 5d90 7d03 7402  |._.x.|.D.].}.t.
-000022d0: 7c03 7403 8302 722e 7c03 6a04 7c02 8301  |.t...r.|.j.|...
-000022e0: 0100 7114 7c03 6a05 6401 8301 7d04 7c04  ..q.|.j.d...}.|.
-000022f0: 6402 1900 7d05 7c05 7c00 6a06 6a07 6a08  d...}.|.|.j.j.j.
-00002300: 6b07 7264 7409 6403 6a0a 7c05 7c00 6a06  k.rdt.d.j.|.|.j.
-00002310: 6a07 6a0b 8302 8301 8201 7c05 7c02 6a01  j.j.......|.|.j.
-00002320: 6a0c 8300 6b07 727e 740d 8300 7c02 6a01  j...k.r~t...|.j.
-00002330: 7c05 3c00 6401 6a0e 7c04 6404 6400 8502  |.<.d.j.|.d.d...
-00002340: 1900 8301 7d06 7c06 7214 7c02 6a01 7c05  ....}.|.r.|.j.|.
-00002350: 1900 6a0f 7c06 8301 0100 7114 5700 7c02  ..j.|.....q.W.|.
-00002360: 5300 2905 4e72 4700 0000 7201 0000 007a  S.).NrG...r....z
-00002370: 1c72 656c 6174 696f 6e20 7b7d 2066 6f72  .relation {} for
-00002380: 207b 7d20 6e6f 7420 666f 756e 6472 2400   {} not foundr$.
-00002390: 0000 2910 726e 0000 0072 5c00 0000 723a  ..).rn...r\...r:
-000023a0: 0000 0072 0b00 0000 5a14 7265 736f 6c76  ...r....Z.resolv
-000023b0: 655f 666f 725f 7175 6572 7973 6574 724b  e_for_querysetrK
-000023c0: 0000 0072 1100 0000 7226 0000 0072 4900  ...r....r&...rI.
-000023d0: 0000 720a 0000 0072 4100 0000 7216 0000  ..r....rA...r...
-000023e0: 00da 046b 6579 73da 0373 6574 721b 0000  ...keys..setr...
-000023f0: 00da 0361 6464 2907 7212 0000 0072 7200  ...add).r....rr.
-00002400: 0000 726d 0000 00da 0872 656c 6174 696f  ..rm.....relatio
-00002410: 6eda 0e72 656c 6174 696f 6e5f 7370 6c69  n..relation_spli
-00002420: 74da 1166 6972 7374 5f6c 6576 656c 5f66  t..first_level_f
-00002430: 6965 6c64 da12 666f 7277 6172 6465 645f  ield..forwarded_
-00002440: 7072 6566 6574 6368 7213 0000 0072 1300  prefetchr....r..
-00002450: 0000 7214 0000 00da 1070 7265 6665 7463  ..r......prefetc
-00002460: 685f 7265 6c61 7465 6446 0100 0073 2400  h_relatedF...s$.
-00002470: 0000 0001 0801 0602 0a01 0a01 0a01 0201  ................
-00002480: 0a01 0801 0e01 0201 0401 1003 0e01 0c01  ................
-00002490: 1201 0401 1401 7a19 5175 6572 7953 6574  ......z.QuerySet
-000024a0: 2e70 7265 6665 7463 685f 7265 6c61 7465  .prefetch_relate
-000024b0: 6429 0172 6000 0000 6302 0000 0000 0000  d).r`...c.......
-000024c0: 0003 0000 0002 0000 0043 0000 0073 1200  .........C...s..
-000024d0: 0000 7c00 6a00 8300 7d02 7c01 7c02 5f01  ..|.j...}.|.|._.
-000024e0: 7c02 5300 2901 4e29 0272 6e00 0000 7260  |.S.).N).rn...r`
-000024f0: 0000 0029 0372 1200 0000 7260 0000 0072  ...).r....r`...r
-00002500: 6d00 0000 7213 0000 0072 1300 0000 7214  m...r....r....r.
-00002510: 0000 00da 0875 7369 6e67 5f64 625d 0100  .....using_db]..
-00002520: 0073 0600 0000 0001 0801 0601 7a11 5175  .s..........z.Qu
-00002530: 6572 7953 6574 2e75 7369 6e67 5f64 6263  erySet.using_dbc
-00002540: 0100 0000 0000 0000 0600 0000 0400 0000  ................
-00002550: 4300 0000 7384 0000 007c 006a 0073 0a64  C...s....|.j.s.d
-00002560: 0053 0074 017c 006a 026a 036a 0483 017d  .S.t.|.j.j.j...}
-00002570: 017c 006a 056a 067c 016a 0783 017c 005f  .|.j.j.|.j...|._
-00002580: 0578 567c 006a 006a 0883 0044 005d 485c  .xV|.j.j...D.]H\
-00002590: 027d 027d 037c 036a 097c 006a 0283 017d  .}.}.|.j.|.j...}
-000025a0: 0478 1a7c 0464 0119 0044 005d 0e7d 057c  .x.|.d...D.].}.|
-000025b0: 006a 0a7c 058e 0001 0071 5257 007c 006a  .j.|.....qRW.|.j
-000025c0: 056a 0b7c 0464 0219 006a 0c7c 0283 0183  .j.|.d...j.|....
-000025d0: 017c 005f 0571 3457 0064 0053 0029 034e  .|._.q4W.d.S.).N
-000025e0: 5a05 6a6f 696e 7372 1a00 0000 290d 7267  Z.joinsr....).rg
-000025f0: 0000 0072 0500 0000 7211 0000 0072 2600  ...r....r....r&.
-00002600: 0000 7216 0000 0072 1000 0000 da07 6772  ..r....r......gr
-00002610: 6f75 7062 7972 1e00 0000 7229 0000 0072  oupbyr....r)...r
-00002620: 2700 0000 7246 0000 00da 0673 656c 6563  '...rF.....selec
-00002630: 74da 0361 735f 2906 7212 0000 0072 1600  t..as_).r....r..
-00002640: 0000 7235 0000 005a 0961 6767 7265 6761  ..r5...Z.aggrega
-00002650: 7465 7238 0000 0072 1b00 0000 7213 0000  ter8...r....r...
-00002660: 0072 1300 0000 7214 0000 00da 115f 7265  .r....r......_re
-00002670: 736f 6c76 655f 616e 6e6f 7461 7465 6201  solve_annotateb.
-00002680: 0000 7312 0000 0000 0106 0104 010e 0110  ..s.............
-00002690: 0114 010c 010e 010e 017a 1a51 7565 7279  .........z.Query
-000026a0: 5365 742e 5f72 6573 6f6c 7665 5f61 6e6e  Set._resolve_ann
-000026b0: 6f74 6174 6563 0100 0000 0000 0000 0300  otatec..........
-000026c0: 0000 0800 0000 4300 0000 73bc 0000 007c  ......C...s....|
-000026d0: 006a 0072 0c7c 006a 006e 087c 006a 016a  .j.r.|.j.n.|.j.j
-000026e0: 026a 037d 0174 047c 006a 016a 026a 0583  .j.}.t.|.j.j.j..
-000026f0: 017d 027c 016a 066a 077c 0283 016a 087c  .}.|.j.j.|...j.|
-00002700: 006a 098e 007c 005f 0a7c 006a 0b83 0001  .j...|._.|.j....
-00002710: 007c 006a 0c7c 006a 017c 006a 0d7c 006a  .|.j.|.j.|.j.|.j
-00002720: 0e7c 006a 0f7c 006a 107c 006a 1164 018d  .|.j.|.j.|.j.d..
-00002730: 0601 007c 006a 1272 7a7c 006a 0a6a 137c  ...|.j.rz|.j.j.|
-00002740: 006a 1283 017c 005f 0a7c 006a 1472 907c  .j...|._.|.j.r.|
-00002750: 006a 0a6a 157c 006a 1483 017c 005f 0a7c  .j.j.|.j...|._.|
-00002760: 006a 1672 a27c 006a 0a6a 1783 007c 005f  .j.r.|.j.j...|._
-00002770: 0a7c 006a 187c 006a 017c 006a 197c 006a  .|.j.|.j.|.j.|.j
-00002780: 0f83 0301 007c 006a 0a53 0029 024e 2906  .....|.j.S.).N).
-00002790: 7211 0000 0072 2f00 0000 7230 0000 0072  r....r/...r0...r
-000027a0: 3100 0000 722e 0000 0072 3200 0000 291a  1...r....r2...).
-000027b0: 7260 0000 0072 1100 0000 7226 0000 0072  r`...r....r&...r
-000027c0: 8200 0000 7205 0000 0072 1600 0000 da0b  ....r....r......
-000027d0: 7175 6572 795f 636c 6173 7372 5b00 0000  query_classr[...
-000027e0: 729d 0000 0072 0700 0000 7210 0000 0072  r....r....r....r
-000027f0: 9f00 0000 7239 0000 0072 6300 0000 7265  ....r9...rc...re
-00002800: 0000 0072 6700 0000 7268 0000 0072 6900  ...rg...rh...ri.
-00002810: 0000 7261 0000 0072 7a00 0000 7262 0000  ..ra...rz...rb..
-00002820: 0072 7b00 0000 7266 0000 0072 7c00 0000  .r{...rf...r|...
-00002830: 724c 0000 0072 6400 0000 2903 7212 0000  rL...rd...).r...
-00002840: 0072 8200 0000 7216 0000 0072 1300 0000  .r....r....r....
-00002850: 7213 0000 0072 1400 0000 da0b 5f6d 616b  r....r......_mak
-00002860: 655f 7175 6572 796d 0100 0073 2600 0000  e_querym...s&...
-00002870: 0001 1601 0e01 1601 0801 0401 0401 0401  ................
-00002880: 0401 0401 0401 0a02 0601 1001 0601 1001  ................
-00002890: 0601 0c01 1401 7a14 5175 6572 7953 6574  ......z.QuerySet
-000028a0: 2e5f 6d61 6b65 5f71 7565 7279 6301 0000  ._make_queryc...
-000028b0: 0000 0000 0003 0000 0006 0000 00c3 0000  ................
-000028c0: 0073 7800 0000 7c00 6a00 8300 7c00 5f01  .sx...|.j...|._.
-000028d0: 7c00 6a02 7216 7c00 6a02 6e08 7c00 6a03  |.j.r.|.j.n.|.j.
-000028e0: 6a04 6a05 7d01 7c01 6a06 7c00 6a03 7c01  j.j.}.|.j.|.j.|.
-000028f0: 7c00 6a07 7c00 6a08 6401 8d04 6a09 7c00  |.j.|.j.d...j.|.
-00002900: 6a01 740a 7c00 6a0b 6a0c 8300 8301 6402  j.t.|.j.j.....d.
-00002910: 8d02 4900 6400 4800 7d02 7c02 7366 7c00  ..I.d.H.}.|.sf|.
-00002920: 6a0d 7262 6400 5300 6700 5300 7c00 6a0d  j.rbd.S.g.S.|.j.
-00002930: 7274 7c02 6403 1900 5300 7c02 5300 2904  rt|.d...S.|.S.).
-00002940: 4e29 0472 1100 0000 7282 0000 00da 0c70  N).r....r......p
-00002950: 7265 6665 7463 685f 6d61 70da 1070 7265  refetch_map..pre
-00002960: 6665 7463 685f 7175 6572 6965 7329 01da  fetch_queries)..
-00002970: 0d63 7573 746f 6d5f 6669 656c 6473 7201  .custom_fieldsr.
-00002980: 0000 0029 0e72 a100 0000 7210 0000 0072  ...).r....r....r
-00002990: 6000 0000 7211 0000 0072 2600 0000 7282  `...r....r&...r.
-000029a0: 0000 00da 0e65 7865 6375 746f 725f 636c  .....executor_cl
-000029b0: 6173 7372 5c00 0000 725d 0000 00da 0e65  assr\...r].....e
-000029c0: 7865 6375 7465 5f73 656c 6563 7472 6c00  xecute_selectrl.
-000029d0: 0000 7267 0000 0072 9300 0000 725e 0000  ..rg...r....r^..
-000029e0: 0029 0372 1200 0000 7282 0000 00da 0d69  .).r....r......i
-000029f0: 6e73 7461 6e63 655f 6c69 7374 7213 0000  nstance_listr...
-00002a00: 0072 1300 0000 7214 0000 0072 5200 0000  .r....r....rR...
-00002a10: 8301 0000 731e 0000 0000 010a 0116 0104  ....s...........
-00002a20: 0104 0102 0104 010a 021c 0204 0106 0104  ................
-00002a30: 0104 0106 0108 017a 1151 7565 7279 5365  .......z.QuerySe
-00002a40: 742e 5f65 7865 6375 7465 6301 0000 0000  t._executec.....
-00002a50: 0000 0002 0000 0002 0000 00c3 0000 0073  ...............s
-00002a60: 1200 0000 7c00 4900 6400 4800 7d01 7400  ....|.I.d.H.}.t.
-00002a70: 7c01 8301 5300 2901 4e29 0172 0d00 0000  |...S.).N).r....
-00002a80: 2902 7212 0000 00da 0672 6573 756c 7472  ).r......resultr
-00002a90: 1300 0000 7213 0000 0072 1400 0000 da09  ....r....r......
-00002aa0: 5f5f 6169 7465 725f 5f96 0100 0073 0400  __aiter__....s..
-00002ab0: 0000 0001 0a01 7a12 5175 6572 7953 6574  ......z.QuerySet
-00002ac0: 2e5f 5f61 6974 6572 5f5f 291b 724e 0000  .__aiter__).rN..
-00002ad0: 0072 5500 0000 7256 0000 0072 1500 0000  .rU...rV...r....
-00002ae0: 726e 0000 0072 7500 0000 7279 0000 0072  rn...ru...ry...r
-00002af0: 7a00 0000 727b 0000 0072 7c00 0000 7280  z...r{...r|...r.
-00002b00: 0000 0072 8500 0000 7289 0000 0072 8b00  ...r....r....r..
-00002b10: 0000 727f 0000 0072 8f00 0000 7290 0000  ..r....r....r...
-00002b20: 0072 9100 0000 7292 0000 0072 9a00 0000  .r....r....r....
-00002b30: 7209 0000 0072 9b00 0000 729f 0000 0072  r....r....r....r
-00002b40: a100 0000 7252 0000 0072 a900 0000 da0d  ....rR...r......
-00002b50: 5f5f 636c 6173 7363 656c 6c5f 5f72 1300  __classcell__r..
-00002b60: 0000 7213 0000 0029 0172 6a00 0000 7214  ..r....).rj...r.
-00002b70: 0000 0072 5700 0000 7d00 0000 732c 0000  ...rW...}...s,..
+00000080: 6408 6c0e 6d0f 5a0f 6d10 5a10 0100 6400  d.l.m.Z.m.Z...d.
+00000090: 6409 6c11 6d12 5a12 6d13 5a13 0100 6400  d.l.m.Z.m.Z...d.
+000000a0: 640a 6c14 6d15 5a15 0100 4700 640b 640c  d.l.m.Z...G.d.d.
+000000b0: 8400 640c 8302 5a16 4700 640d 640e 8400  ..d...Z.G.d.d...
+000000c0: 640e 6516 8303 5a17 4700 640f 6410 8400  d.e...Z.G.d.d...
+000000d0: 6410 6516 8303 5a18 4700 6411 6412 8400  d.e...Z.G.d.d...
+000000e0: 6412 6516 8303 5a19 4700 6413 6414 8400  d.e...Z.G.d.d...
+000000f0: 6414 6516 8303 5a1a 4700 6415 6416 8400  d.e...Z.G.d.d...
+00000100: 6416 6516 8303 5a1b 4700 6417 6418 8400  d.e...Z.G.d.d...
+00000110: 6418 651b 8303 5a1c 4700 6419 641a 8400  d.e...Z.G.d.d...
+00000120: 641a 651b 8303 5a1d 641b 5300 291c e900  d.e...Z.d.S.)...
+00000130: 0000 0029 02da 084a 6f69 6e54 7970 65da  ...)...JoinType.
+00000140: 054f 7264 6572 2901 da0f 506f 7374 6772  .Order)...Postgr
+00000150: 6553 514c 5175 6572 7929 01da 0554 6162  eSQLQuery)...Tab
+00000160: 6c65 2901 da05 436f 756e 7429 01da 0666  le)...Count)...f
+00000170: 6965 6c64 7329 01da 0941 6767 7265 6761  ields)...Aggrega
+00000180: 7465 2901 da11 4261 7365 4442 4173 796e  te)...BaseDBAsyn
+00000190: 6343 6c69 656e 7429 02da 0a46 6965 6c64  cClient)...Field
+000001a0: 4572 726f 72da 104f 7065 7261 7469 6f6e  Error..Operation
+000001b0: 616c 4572 726f 7229 02da 0850 7265 6665  alError)...Prefe
+000001c0: 7463 68da 0151 2901 da12 5175 6572 7941  tch..Q)...QueryA
+000001d0: 7379 6e63 4974 6572 6174 6f72 6300 0000  syncIteratorc...
+000001e0: 0000 0000 0000 0000 0002 0000 0040 0000  .............@..
+000001f0: 0073 4400 0000 6500 5a01 6400 5a02 6401  .sD...e.Z.d.Z.d.
+00000200: 6402 8400 5a03 6403 6404 8400 5a04 6405  d...Z.d.d...Z.d.
+00000210: 6406 8400 5a05 6407 6408 8400 5a06 6409  d...Z.d.d...Z.d.
+00000220: 640a 8400 5a07 640b 640c 8400 5a08 640d  d...Z.d.d...Z.d.
+00000230: 640e 8400 5a09 640f 5300 2910 da0e 4177  d...Z.d.S.)...Aw
+00000240: 6169 7461 626c 6551 7565 7279 6301 0000  aitableQueryc...
+00000250: 0000 0000 0001 0000 0002 0000 0043 0000  .............C..
+00000260: 0073 1600 0000 6700 7c00 5f00 6400 7c00  .s....g.|._.d.|.
+00000270: 5f01 6400 7c00 5f02 6400 5300 2901 4e29  _.d.|._.d.S.).N)
+00000280: 03da 0e5f 6a6f 696e 6564 5f74 6162 6c65  ..._joined_table
+00000290: 73da 0571 7565 7279 da05 6d6f 6465 6c29  s..query..model)
+000002a0: 01da 0473 656c 66a9 0072 1400 0000 fa45  ...self..r.....E
+000002b0: 2f55 7365 7273 2f61 6e64 7265 7962 6f6e  /Users/andreybon
+000002c0: 6461 722f 5079 4368 6172 6d50 726f 6a65  dar/PyCharmProje
+000002d0: 6374 732f 746f 7274 6f69 7365 2d6f 726d  cts/tortoise-orm
+000002e0: 2f74 6f72 746f 6973 652f 7175 6572 7973  /tortoise/querys
+000002f0: 6574 2e70 79da 085f 5f69 6e69 745f 5f0f  et.py..__init__.
+00000300: 0000 0073 0600 0000 0001 0601 0601 7a17  ...s..........z.
+00000310: 4177 6169 7461 626c 6551 7565 7279 2e5f  AwaitableQuery._
+00000320: 5f69 6e69 745f 5f63 0400 0000 0000 0000  _init__c........
+00000330: 0400 0000 0600 0000 4300 0000 736a 0000  ........C...sj..
+00000340: 007c 0264 0119 007c 006a 006b 0772 407c  .|.d...|.j.k.r@|
+00000350: 006a 016a 027c 0264 0119 0074 036a 0464  .j.j.|.d...t.j.d
+00000360: 028d 026a 057c 016a 0674 077c 0264 0119  ...j.|.j.t.|.d..
+00000370: 007c 0264 0319 0083 026b 0283 017c 005f  .|.d.....k...|._
+00000380: 017c 006a 016a 087c 0264 0419 0074 077c  .|.j.j.|.d...t.|
+00000390: 0264 0119 007c 0264 0519 0083 027c 0383  .d...|.d.....|..
+000003a0: 0283 017c 005f 0164 0053 0029 064e da05  ...|._.d.S.).N..
+000003b0: 7461 626c 6529 01da 0368 6f77 da0c 6261  table)...how..ba
+000003c0: 636b 7761 7264 5f6b 6579 da08 6f70 6572  ckward_key..oper
+000003d0: 6174 6f72 da05 6669 656c 6429 0972 1000  ator..field).r..
+000003e0: 0000 7211 0000 00da 046a 6f69 6e72 0200  ..r......joinr..
+000003f0: 0000 da0a 6c65 6674 5f6f 7574 6572 da02  ....left_outer..
+00000400: 6f6e da02 6964 da07 6765 7461 7474 72da  on..id..getattr.
+00000410: 0577 6865 7265 2904 7213 0000 0072 1700  .where).r....r..
+00000420: 0000 da05 7061 7261 6dda 0576 616c 7565  ....param..value
+00000430: 7214 0000 0072 1400 0000 7215 0000 00da  r....r....r.....
+00000440: 1a5f 6669 6c74 6572 5f66 726f 6d5f 7265  ._filter_from_re
+00000450: 6c61 7465 645f 7461 626c 6514 0000 0073  lated_table....s
+00000460: 0c00 0000 0001 0e01 0601 1001 1c01 0601  ................
+00000470: 7a29 4177 6169 7461 626c 6551 7565 7279  z)AwaitableQuery
+00000480: 2e5f 6669 6c74 6572 5f66 726f 6d5f 7265  ._filter_from_re
+00000490: 6c61 7465 645f 7461 626c 6563 0700 0000  lated_tablec....
+000004a0: 0000 0000 1400 0000 0700 0000 4300 0000  ............C...
+000004b0: 7366 0100 0074 007c 016a 016a 0283 017d  sf...t.|.j.j...}
+000004c0: 0778 767c 0344 005d 6e7d 087c 086a 037c  .xv|.D.]n}.|.j.|
+000004d0: 0183 015c 027d 097d 0a78 4c7c 0a44 005d  ...\.}.}.xL|.D.]
+000004e0: 447d 0b7c 0b64 0119 007c 006a 046b 0772  D}.|.d...|.j.k.r
+000004f0: 2a7c 006a 056a 067c 0b64 0119 0074 076a  *|.j.j.|.d...t.j
+00000500: 0864 028d 026a 097c 0b64 0319 0083 017c  .d...j.|.d.....|
+00000510: 005f 057c 006a 046a 0a7c 0b64 0119 0083  ._.|.j.j.|.d....
+00000520: 0101 0071 2a57 007c 006a 056a 0b7c 0983  ...q*W.|.j.j.|..
+00000530: 017c 005f 0571 1257 0078 887c 026a 0c83  .|._.q.W.x.|.j..
+00000540: 0044 005d 7c5c 027d 0c7d 0d7c 016a 016a  .D.]|\.}.}.|.j.j
+00000550: 0d7c 0c19 007d 0e7c 0e6a 0e64 0483 0172  .|...}.|.j.d...r
+00000560: bc7c 006a 0f7c 077c 0e7c 0d83 0301 0071  .|.j.|.|.|.....q
+00000570: 8e7c 016a 016a 107c 0e64 0519 0019 007d  .|.j.j.|.d.....}
+00000580: 0f7c 0e6a 0e64 0683 0172 de7c 0e64 0619  .|.j.d...r.|.d..
+00000590: 006e 047c 0f6a 117d 107c 006a 056a 0b7c  .n.|.j.}.|.j.j.|
+000005a0: 0e64 0719 0074 127c 077c 0e64 0519 0083  .d...t.|.|.d....
+000005b0: 027c 107c 0d83 0183 0283 017c 005f 0571  .|.|.......|._.q
+000005c0: 8e57 0078 527c 046a 0c83 0044 005d 465c  .W.xR|.j...D.]F\
+000005d0: 027d 0c7d 0d7c 067c 0c19 007d 117c 057c  .}.}.|.|...}.|.|
+000005e0: 1164 0519 0019 007d 127c 126a 037c 006a  .d.....}.|.j.|.j
+000005f0: 1383 017d 137c 006a 056a 147c 1164 0719  ...}.|.j.j.|.d..
+00000600: 007c 1364 0519 007c 0d83 0283 017c 005f  .|.d...|.....|._
+00000610: 0590 0171 1857 0064 0053 0029 084e 7201  ...q.W.d.S.).Nr.
+00000620: 0000 0029 0172 1800 0000 e901 0000 0072  ...).r.........r
+00000630: 1700 0000 721b 0000 00da 0d76 616c 7565  ....r......value
+00000640: 5f65 6e63 6f64 6572 721a 0000 0029 1572  _encoderr....).r
+00000650: 0500 0000 da05 5f6d 6574 6172 1700 0000  ......_metar....
+00000660: da11 7265 736f 6c76 655f 666f 725f 6d6f  ..resolve_for_mo
+00000670: 6465 6c72 1000 0000 7211 0000 0072 1c00  delr....r....r..
+00000680: 0000 7202 0000 0072 1d00 0000 721e 0000  ..r....r....r...
+00000690: 00da 0661 7070 656e 6472 2100 0000 da05  ...appendr!.....
+000006a0: 6974 656d 73da 0766 696c 7465 7273 da03  items..filters..
+000006b0: 6765 7472 2400 0000 da0a 6669 656c 6473  getr$.....fields
+000006c0: 5f6d 6170 da0b 746f 5f64 625f 7661 6c75  _map..to_db_valu
+000006d0: 6572 2000 0000 7212 0000 00da 0668 6176  er ...r......hav
+000006e0: 696e 6729 1472 1300 0000 7212 0000 00da  ing).r....r.....
+000006f0: 0d66 696c 7465 725f 6b77 6172 6773 da09  .filter_kwargs..
+00000700: 715f 6f62 6a65 6374 7372 2f00 0000 da0b  q_objectsr/.....
+00000710: 616e 6e6f 7461 7469 6f6e 73da 0e63 7573  annotations..cus
+00000720: 746f 6d5f 6669 6c74 6572 7372 1700 0000  tom_filtersr....
+00000730: da04 6e6f 6465 da09 6372 6974 6572 696f  ..node..criterio
+00000740: 6e5a 0e72 6571 7569 7265 645f 6a6f 696e  nZ.required_join
+00000750: 7372 1c00 0000 da03 6b65 7972 2300 0000  sr......keyr#...
+00000760: 7222 0000 00da 0c66 6965 6c64 5f6f 626a  r".....field_obj
+00000770: 6563 7472 2600 0000 5a0b 6861 7669 6e67  ectr&...Z.having
+00000780: 5f69 6e66 6fda 0b61 6767 7265 6761 7469  _info..aggregati
+00000790: 6f6e da10 6167 6772 6567 6174 696f 6e5f  on..aggregation_
+000007a0: 696e 666f 7214 0000 0072 1400 0000 7215  infor....r....r.
+000007b0: 0000 00da 0f72 6573 6f6c 7665 5f66 696c  .....resolve_fil
+000007c0: 7465 7273 1d00 0000 732c 0000 0000 010c  ters....s,......
+000007d0: 010a 010e 010a 010e 0122 0114 0112 0112  ........."......
+000007e0: 010c 010a 0110 0210 0318 0206 0124 0212  .............$..
+000007f0: 0108 010c 010c 0106 017a 1e41 7761 6974  .........z.Await
+00000800: 6162 6c65 5175 6572 792e 7265 736f 6c76  ableQuery.resolv
+00000810: 655f 6669 6c74 6572 7363 0400 0000 0000  e_filtersc......
+00000820: 0000 0700 0000 0500 0000 4300 0000 7356  ..........C...sV
+00000830: 0100 0074 007c 0374 016a 0283 0272 a274  ...t.|.t.j...r.t
+00000840: 037c 036a 046a 056a 0683 017d 0474 037c  .|.j.j.j...}.t.|
+00000850: 036a 0783 017d 057c 057c 006a 086b 0772  .j...}.|.|.j.k.r
+00000860: 627c 006a 096a 0a7c 0574 0b6a 0c64 018d  b|.j.j.|.t.j.d..
+00000870: 026a 0d7c 016a 0e74 0f7c 057c 036a 1083  .j.|.j.t.|.|.j..
+00000880: 026b 0283 017c 005f 097c 006a 086a 117c  .k...|._.|.j.j.|
+00000890: 0583 0101 007c 047c 006a 086b 0772 a07c  .....|.|.j.k.r.|
+000008a0: 006a 096a 0a7c 0474 0b6a 0c64 018d 026a  .j.j.|.t.j.d...j
+000008b0: 0d74 0f7c 057c 036a 1283 027c 046a 0e6b  .t.|.|.j...|.j.k
+000008c0: 0283 017c 005f 097c 006a 086a 117c 0483  ...|._.|.j.j.|..
+000008d0: 0101 006e b074 007c 0374 016a 1383 0272  ...n.t.|.t.j...r
+000008e0: fc74 037c 036a 046a 056a 0683 017d 047c  .t.|.j.j.j...}.|
+000008f0: 047c 006a 086b 0772 fa7c 006a 096a 0a7c  .|.j.k.r.|.j.j.|
+00000900: 0474 0b6a 0c64 018d 026a 0d7c 016a 0e74  .t.j.d...j.|.j.t
+00000910: 0f7c 047c 036a 1483 026b 0283 017c 005f  .|.|.j...k...|._
+00000920: 097c 006a 086a 117c 0483 0101 006e 5674  .|.j.j.|.....nVt
+00000930: 037c 036a 046a 056a 0683 017d 047c 047c  .|.j.j.j...}.|.|
+00000940: 006a 086b 0790 0172 5264 026a 157c 0283  .j.k...rRd.j.|..
+00000950: 017d 067c 006a 096a 0a7c 0474 0b6a 0c64  .}.|.j.j.|.t.j.d
+00000960: 018d 026a 0d7c 046a 0e74 0f7c 017c 0683  ...j.|.j.t.|.|..
+00000970: 026b 0283 017c 005f 097c 006a 086a 117c  .k...|._.|.j.j.|
+00000980: 0483 0101 0064 0053 0029 034e 2901 7218  .....d.S.).N).r.
+00000990: 0000 007a 057b 7d5f 6964 2916 da0a 6973  ...z.{}_id)...is
+000009a0: 696e 7374 616e 6365 7207 0000 00da 0f4d  instancer......M
+000009b0: 616e 7954 6f4d 616e 7946 6965 6c64 7205  anyToManyFieldr.
+000009c0: 0000 00da 0474 7970 6572 2700 0000 7217  .....typer'...r.
+000009d0: 0000 00da 0774 6872 6f75 6768 7210 0000  .....throughr...
+000009e0: 0072 1100 0000 721c 0000 0072 0200 0000  .r....r....r....
+000009f0: 721d 0000 0072 1e00 0000 721f 0000 0072  r....r....r....r
+00000a00: 2000 0000 7219 0000 0072 2900 0000 da0b   ...r....r).....
+00000a10: 666f 7277 6172 645f 6b65 79da 1242 6163  forward_key..Bac
+00000a20: 6b77 6172 6446 4b52 656c 6174 696f 6eda  kwardFKRelation.
+00000a30: 0e72 656c 6174 696f 6e5f 6669 656c 64da  .relation_field.
+00000a40: 0666 6f72 6d61 7429 0772 1300 0000 7217  .format).r....r.
+00000a50: 0000 00da 1272 656c 6174 6564 5f66 6965  .....related_fie
+00000a60: 6c64 5f6e 616d 65da 0d72 656c 6174 6564  ld_name..related
+00000a70: 5f66 6965 6c64 da0d 7265 6c61 7465 645f  _field..related_
+00000a80: 7461 626c 65da 0d74 6872 6f75 6768 5f74  table..through_t
+00000a90: 6162 6c65 5a15 7265 6c61 7465 645f 6964  ableZ.related_id
+00000aa0: 5f66 6965 6c64 5f6e 616d 6572 1400 0000  _field_namer....
+00000ab0: 7214 0000 0072 1500 0000 da14 5f6a 6f69  r....r......_joi
+00000ac0: 6e5f 7461 626c 655f 6279 5f66 6965 6c64  n_table_by_field
+00000ad0: 3b00 0000 7336 0000 0000 010c 010e 010a  ;...s6..........
+00000ae0: 010a 0106 010c 0116 010c 010a 0106 010c  ................
+00000af0: 0116 010e 010c 010e 010a 0106 010c 0116  ................
+00000b00: 010e 020e 010c 010a 0106 010c 0114 017a  ...............z
+00000b10: 2341 7761 6974 6162 6c65 5175 6572 792e  #AwaitableQuery.
+00000b20: 5f6a 6f69 6e5f 7461 626c 655f 6279 5f66  _join_table_by_f
+00000b30: 6965 6c64 6304 0000 0000 0000 000b 0000  ieldc...........
+00000b40: 0007 0000 0043 0000 0073 2601 0000 7400  .....C...s&...t.
+00000b50: 7c01 6a01 6a02 8301 7d04 9001 7812 7c02  |.j.j...}...x.|.
+00000b60: 4400 9001 5d08 7d05 7c05 6401 1900 7d06  D...].}.|.d...}.
+00000b70: 7c06 7c01 6a01 6a03 6b06 7238 7404 6402  |.|.j.j.k.r8t.d.
+00000b80: 8301 8201 7114 7c06 6a05 6403 8301 6401  ....q.|.j.d...d.
+00000b90: 1900 7c01 6a01 6a03 6b06 72a6 7c06 6a05  ..|.j.j.k.r.|.j.
+00000ba0: 6403 8301 6401 1900 7d07 7c01 6a01 6a06  d...d...}.|.j.j.
+00000bb0: 7c07 1900 7d08 7c00 6a07 7c04 7c07 7c08  |...}.|.j.|.|.|.
+00000bc0: 8303 0100 7c00 6a08 7c08 6a09 6403 6a0a  ....|.j.|.j.d.j.
+00000bd0: 7c06 6a05 6403 8301 6404 6400 8502 1900  |.j.d...d.d.....
+00000be0: 8301 7c05 6404 1900 6602 6701 6900 8303  ..|.d...f.g.i...
+00000bf0: 0100 7114 7c06 7c03 6b06 72de 7c03 7c06  ..q.|.|.k.r.|.|.
+00000c00: 1900 7d09 7c09 6a0b 7c00 6a0c 8301 7d0a  ..}.|.j.|.j...}.
+00000c10: 7c00 6a0d 6a0e 7c0a 6405 1900 7c05 6404  |.j.j.|.d...|.d.
+00000c20: 1900 6406 8d02 7c00 5f0d 7114 7c06 7c01  ..d...|._.q.|.|.
+00000c30: 6a01 6a0f 6b07 72fe 7410 6407 6a11 7c06  j.j.k.r.t.d.j.|.
+00000c40: 7c00 6a0c 6a12 8302 8301 8201 7c00 6a0d  |.j.j.......|.j.
+00000c50: 6a0e 7413 7c04 7c05 6401 1900 8302 7c05  j.t.|.|.d.....|.
+00000c60: 6404 1900 6406 8d02 7c00 5f0d 7114 5700  d...d...|._.q.W.
+00000c70: 6400 5300 2908 4e72 0100 0000 7a4d 4669  d.S.).Nr....zMFi
+00000c80: 6c74 6572 696e 6720 6279 2072 656c 6174  ltering by relat
+00000c90: 696f 6e20 6973 206e 6f74 2070 6f73 7369  ion is not possi
+00000ca0: 626c 6520 6669 6c74 6572 2062 7920 6e65  ble filter by ne
+00000cb0: 7374 6564 2066 6965 6c64 206f 6620 7265  sted field of re
+00000cc0: 6c61 7465 6420 6d6f 6465 6cda 025f 5f72  lated model..__r
+00000cd0: 2500 0000 721b 0000 0029 01da 056f 7264  %...r....)...ord
+00000ce0: 6572 7a1d 556e 6b6e 6f77 6e20 6669 656c  erz.Unknown fiel
+00000cf0: 6420 7b7d 2066 6f72 206d 6f64 656c 207b  d {} for model {
+00000d00: 7d29 1472 0500 0000 7227 0000 0072 1700  }).r....r'...r..
+00000d10: 0000 da0c 6665 7463 685f 6669 656c 6473  ....fetch_fields
+00000d20: da0a 5661 6c75 6545 7272 6f72 da05 7370  ..ValueError..sp
+00000d30: 6c69 7472 2d00 0000 7247 0000 00da 1072  litr-...rG.....r
+00000d40: 6573 6f6c 7665 5f6f 7264 6572 696e 6772  esolve_orderingr
+00000d50: 3d00 0000 721c 0000 0072 2800 0000 7212  =...r....r(...r.
+00000d60: 0000 0072 1100 0000 da07 6f72 6465 7262  ...r......orderb
+00000d70: 7972 0700 0000 720a 0000 0072 4200 0000  yr....r....rB...
+00000d80: da08 5f5f 6e61 6d65 5f5f 7220 0000 0029  ..__name__r ...)
+00000d90: 0b72 1300 0000 7212 0000 00da 096f 7264  .r....r......ord
+00000da0: 6572 696e 6773 7232 0000 0072 1700 0000  eringsr2...r....
+00000db0: da08 6f72 6465 7269 6e67 da0a 6669 656c  ..ordering..fiel
+00000dc0: 645f 6e61 6d65 7243 0000 0072 4400 0000  d_namerC...rD...
+00000dd0: 7238 0000 0072 3900 0000 7214 0000 0072  r8...r9...r....r
+00000de0: 1400 0000 7215 0000 0072 4d00 0000 5900  ....r....rM...Y.
+00000df0: 0000 732c 0000 0000 010c 010e 0108 010c  ..s,............
+00000e00: 0102 0108 0216 010e 010c 010e 0104 012c  ...............,
+00000e10: 0208 0108 010c 011c 020c 0102 0104 0102  ................
+00000e20: 010c 037a 1f41 7761 6974 6162 6c65 5175  ...z.AwaitableQu
+00000e30: 6572 792e 7265 736f 6c76 655f 6f72 6465  ery.resolve_orde
+00000e40: 7269 6e67 6301 0000 0000 0000 0001 0000  ringc...........
+00000e50: 0001 0000 0043 0000 0073 0c00 0000 7c00  .....C...s....|.
+00000e60: 6a00 8300 6a01 8300 5300 2901 4e29 02da  j...j...S.).N)..
+00000e70: 085f 6578 6563 7574 65da 095f 5f61 7761  ._execute..__awa
+00000e80: 6974 5f5f 2901 7213 0000 0072 1400 0000  it__).r....r....
+00000e90: 7214 0000 0072 1500 0000 7254 0000 0076  r....r....rT...v
+00000ea0: 0000 0073 0200 0000 0001 7a18 4177 6169  ...s......z.Awai
+00000eb0: 7461 626c 6551 7565 7279 2e5f 5f61 7761  tableQuery.__awa
+00000ec0: 6974 5f5f 6301 0000 0000 0000 0001 0000  it__c...........
+00000ed0: 0001 0000 00c3 0000 0073 0a00 0000 7400  .........s....t.
+00000ee0: 8300 8201 6400 5300 2901 4e29 01da 134e  ....d.S.).N)...N
+00000ef0: 6f74 496d 706c 656d 656e 7465 6445 7272  otImplementedErr
+00000f00: 6f72 2901 7213 0000 0072 1400 0000 7214  or).r....r....r.
+00000f10: 0000 0072 1500 0000 7253 0000 0079 0000  ...r....rS...y..
+00000f20: 0073 0200 0000 0001 7a17 4177 6169 7461  .s......z.Awaita
+00000f30: 626c 6551 7565 7279 2e5f 6578 6563 7574  bleQuery._execut
+00000f40: 654e 290a 724f 0000 00da 0a5f 5f6d 6f64  eN).rO.....__mod
+00000f50: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
+00000f60: 655f 5f72 1600 0000 7224 0000 0072 3a00  e__r....r$...r:.
+00000f70: 0000 7247 0000 0072 4d00 0000 7254 0000  ..rG...rM...rT..
+00000f80: 0072 5300 0000 7214 0000 0072 1400 0000  .rS...r....r....
+00000f90: 7214 0000 0072 1500 0000 720f 0000 000e  r....r....r.....
+00000fa0: 0000 0073 0e00 0000 0801 0805 0809 081e  ...s............
+00000fb0: 081e 081d 0803 720f 0000 0063 0000 0000  ......r....c....
+00000fc0: 0000 0000 0000 0000 0300 0000 0000 0000  ................
+00000fd0: 73d0 0000 0065 005a 0164 005a 0287 0066  s....e.Z.d.Z...f
+00000fe0: 0164 0164 0284 085a 0364 0364 0484 005a  .d.d...Z.d.d...Z
+00000ff0: 0464 0564 0684 005a 0564 0764 0884 005a  .d.d...Z.d.d...Z
+00001000: 0664 0964 0a84 005a 0764 0b64 0c84 005a  .d.d...Z.d.d...Z
+00001010: 0864 0d64 0e84 005a 0964 0f64 1084 005a  .d.d...Z.d.d...Z
+00001020: 0a64 1164 129c 0164 1364 1484 025a 0b64  .d.d...d.d...Z.d
+00001030: 1564 1684 005a 0c64 1764 1884 005a 0d64  .d...Z.d.d...Z.d
+00001040: 1964 1a84 005a 0e64 1b64 1c84 005a 0f64  .d...Z.d.d...Z.d
+00001050: 1d64 1e84 005a 1064 1f64 2084 005a 1164  .d...Z.d.d ..Z.d
+00001060: 2164 2284 005a 1264 2364 2484 005a 1365  !d"..Z.d#d$..Z.e
+00001070: 1464 259c 0164 2664 2784 045a 1564 2864  .d%..d&d'..Z.d(d
+00001080: 2984 005a 1664 2a64 2b84 005a 1764 2c64  )..Z.d*d+..Z.d,d
+00001090: 2d84 005a 1864 2e64 2f84 005a 1987 0004  -..Z.d.d/..Z....
+000010a0: 005a 1a53 0029 30da 0851 7565 7279 5365  .Z.S.)0..QuerySe
+000010b0: 7463 0200 0000 0000 0000 0200 0000 0200  tc..............
+000010c0: 0000 0300 0000 7388 0000 0074 0083 006a  ......s....t...j
+000010d0: 0183 0001 007c 016a 026a 037c 005f 047c  .....|.j.j.|._.|
+000010e0: 017c 005f 0574 066a 077c 016a 026a 0883  .|._.t.j.|.j.j..
+000010f0: 017c 005f 0969 007c 005f 0a69 007c 005f  .|._.i.|._.i.|._
+00001100: 0b64 017c 005f 0c64 017c 005f 0d64 007c  .d.|._.d.|._.d.|
+00001110: 005f 0e64 007c 005f 0f64 007c 005f 1069  ._.d.|._.d.|._.i
+00001120: 007c 005f 1167 007c 005f 1267 007c 005f  .|._.g.|._.g.|._
+00001130: 1367 007c 005f 1464 017c 005f 1569 007c  .g.|._.d.|._.i.|
+00001140: 005f 1669 007c 005f 1769 007c 005f 1864  ._.i.|._.i.|._.d
+00001150: 0053 0029 024e 4629 19da 0573 7570 6572  .S.).NF)...super
+00001160: 7216 0000 0072 2700 0000 da09 6462 5f66  r....r'.....db_f
+00001170: 6965 6c64 7372 0700 0000 7212 0000 00da  ieldsr....r.....
+00001180: 0551 7565 7279 da05 6672 6f6d 5f72 1700  .Query..from_r..
+00001190: 0000 7211 0000 00da 0d5f 7072 6566 6574  ..r......_prefet
+000011a0: 6368 5f6d 6170 da11 5f70 7265 6665 7463  ch_map.._prefetc
+000011b0: 685f 7175 6572 6965 73da 075f 7369 6e67  h_queries.._sing
+000011c0: 6c65 da06 5f63 6f75 6e74 da03 5f64 62da  le.._count.._db.
+000011d0: 065f 6c69 6d69 74da 075f 6f66 6673 6574  ._limit.._offset
+000011e0: da0e 5f66 696c 7465 725f 6b77 6172 6773  .._filter_kwargs
+000011f0: da0a 5f6f 7264 6572 696e 6773 7210 0000  .._orderingsr...
+00001200: 00da 165f 715f 6f62 6a65 6374 735f 666f  ..._q_objects_fo
+00001210: 725f 7265 736f 6c76 65da 095f 6469 7374  r_resolve.._dist
+00001220: 696e 6374 da0c 5f61 6e6e 6f74 6174 696f  inct.._annotatio
+00001230: 6e73 da07 5f68 6176 696e 67da 195f 6176  ns.._having.._av
+00001240: 6169 6c61 626c 655f 6375 7374 6f6d 5f66  ailable_custom_f
+00001250: 696c 7465 7273 2902 7213 0000 0072 1200  ilters).r....r..
+00001260: 0000 2901 da09 5f5f 636c 6173 735f 5f72  ..)...__class__r
+00001270: 1400 0000 7215 0000 0072 1600 0000 7e00  ....r....r....~.
+00001280: 0000 7326 0000 0000 010a 010a 0106 0110  ..s&............
+00001290: 0106 0106 0106 0106 0106 0106 0106 0106  ................
+000012a0: 0106 0106 0106 0106 0106 0106 017a 1151  .............z.Q
+000012b0: 7565 7279 5365 742e 5f5f 696e 6974 5f5f  uerySet.__init__
+000012c0: 6301 0000 0000 0000 0002 0000 0002 0000  c...............
+000012d0: 0043 0000 0073 9800 0000 7c00 6a00 7c00  .C...s....|.j.|.
+000012e0: 6a01 8301 7d01 7c00 6a02 7c01 5f02 7c00  j...}.|.j.|._.|.
+000012f0: 6a03 7c01 5f03 7c00 6a04 7c01 5f04 7c00  j.|._.|.j.|._.|.
+00001300: 6a05 7c01 5f05 7c00 6a06 7c01 5f06 7c00  j.|._.|.j.|._.|.
+00001310: 6a07 7c01 5f07 7c00 6a08 7c01 5f08 7409  j.|._.|.j.|._.t.
+00001320: 7c00 6a0a 8301 7c01 5f0a 740b 7c00 6a0c  |.j...|._.t.|.j.
+00001330: 8301 7c01 5f0c 740b 7c00 6a0d 8301 7c01  ..|._.t.|.j...|.
+00001340: 5f0d 740b 7c00 6a0e 8301 7c01 5f0e 7c00  _.t.|.j...|._.|.
+00001350: 6a0f 7c01 5f0f 7c00 6a10 7c01 5f10 7c00  j.|._.|.j.|._.|.
+00001360: 6a11 7c01 5f11 7c00 6a12 7c01 5f12 7c01  j.|._.|.j.|._.|.
+00001370: 5300 2901 4e29 1372 6b00 0000 7212 0000  S.).N).rk...r...
+00001380: 0072 5d00 0000 725e 0000 0072 5f00 0000  .r]...r^...r_...
+00001390: 7260 0000 0072 6100 0000 7262 0000 0072  r`...ra...rb...r
+000013a0: 6300 0000 da04 6469 6374 7264 0000 00da  c.....dictrd....
+000013b0: 046c 6973 7472 6500 0000 7210 0000 0072  .listre...r....r
+000013c0: 6600 0000 7267 0000 0072 6800 0000 7269  f...rg...rh...ri
+000013d0: 0000 0072 6a00 0000 2902 7213 0000 00da  ...rj...).r.....
+000013e0: 0871 7565 7279 7365 7472 1400 0000 7214  .querysetr....r.
+000013f0: 0000 0072 1500 0000 da06 5f63 6c6f 6e65  ...r......_clone
+00001400: 9300 0000 7322 0000 0000 010c 0108 0108  ....s"..........
+00001410: 0108 0108 0108 0108 0108 010c 010c 010c  ................
+00001420: 010c 0108 0108 0108 0108 017a 0f51 7565  ...........z.Que
+00001430: 7279 5365 742e 5f63 6c6f 6e65 6301 0000  rySet._clonec...
+00001440: 0000 0000 0008 0000 0006 0000 004f 0000  .............O..
+00001450: 0073 e800 0000 7c00 6a00 8300 7d03 782a  .s....|.j...}.x*
+00001460: 7c01 4400 5d22 7d04 7401 7c04 7402 8302  |.D.]"}.t.|.t...
+00001470: 7324 7403 6401 8301 8201 7c03 6a04 6a05  s$t.d.....|.j.j.
+00001480: 7c04 8301 0100 710e 5700 78ae 7c02 6a06  |.....q.W.x.|.j.
+00001490: 8300 4400 5da2 5c02 7d05 7d06 7c05 7c03  ..D.].\.}.}.|.|.
+000014a0: 6a07 6a08 6a09 6b06 7260 7c06 7c03 6a0a  j.j.j.k.r`|.|.j.
+000014b0: 7c05 3c00 713e 7c05 7c00 6a07 6a08 6a0b  |.<.q>|.|.j.j.j.
+000014c0: 6b06 728c 7c00 6a07 6a08 6a0c 7c05 1900  k.r.|.j.j.j.|...
+000014d0: 7d07 7c06 6a0d 7c03 6a0a 7c07 6a0e 3c00  }.|.j.|.j.|.j.<.
+000014e0: 713e 7c05 6a0f 6402 8301 6403 1900 7c00  q>|.j.d...d...|.
+000014f0: 6a07 6a08 6a10 6b06 72bc 7c03 6a04 6a05  j.j.j.k.r.|.j.j.
+00001500: 7402 6600 7c05 7c06 6901 8e01 8301 0100  t.f.|.|.i.......
+00001510: 713e 7c05 7c00 6a11 6b06 72d2 7c06 7c03  q>|.|.j.k.r.|.|.
+00001520: 6a12 7c05 3c00 713e 7413 6404 6a14 7c05  j.|.<.q>t.d.j.|.
+00001530: 8301 8301 8201 713e 5700 7c03 5300 2905  ......q>W.|.S.).
+00001540: 4e7a 1a65 7870 6563 7465 6420 5120 6f62  Nz.expected Q ob
+00001550: 6a65 6374 7320 6173 2061 7267 7372 4800  jects as argsrH.
+00001560: 0000 7201 0000 007a 1775 6e6b 6e6f 776e  ..r....z.unknown
+00001570: 2066 696c 7465 7220 7061 7261 6d20 7b7d   filter param {}
+00001580: 2915 726f 0000 0072 3b00 0000 720d 0000  ).ro...r;...r...
+00001590: 00da 0954 7970 6545 7272 6f72 7266 0000  ...TypeErrorrf..
+000015a0: 0072 2900 0000 722a 0000 0072 1200 0000  .r)...r*...r....
+000015b0: 7227 0000 0072 2b00 0000 7264 0000 00da  r'...r+...rd....
+000015c0: 0966 6b5f 6669 656c 6473 722d 0000 0072  .fk_fieldsr-...r
+000015d0: 1f00 0000 da0c 736f 7572 6365 5f66 6965  ......source_fie
+000015e0: 6c64 724c 0000 0072 4a00 0000 726a 0000  ldrL...rJ...rj..
+000015f0: 0072 6900 0000 720a 0000 0072 4200 0000  .ri...r....rB...
+00001600: 2908 7213 0000 00da 0461 7267 73da 066b  ).r......args..k
+00001610: 7761 7267 7372 6e00 0000 da03 6172 6772  wargsrn.....argr
+00001620: 3600 0000 7223 0000 0072 3700 0000 7214  6...r#...r7...r.
+00001630: 0000 0072 1400 0000 7215 0000 00da 0666  ...r....r......f
+00001640: 696c 7465 72a6 0000 0073 2200 0000 0001  ilter....s".....
+00001650: 0801 0a01 0a01 0801 1001 1201 0e01 0c01  ................
+00001660: 0e01 0e01 1001 1801 1801 0a01 0c02 1201  ................
+00001670: 7a0f 5175 6572 7953 6574 2e66 696c 7465  z.QuerySet.filte
+00001680: 7263 0100 0000 0000 0000 0700 0000 0500  rc..............
+00001690: 0000 4700 0000 7392 0000 007c 006a 0083  ..G...s....|.j..
+000016a0: 007d 0267 007d 0378 7a7c 0144 005d 727d  .}.g.}.xz|.D.]r}
+000016b0: 0474 016a 027d 057c 0464 0119 0064 026b  .t.j.}.|.d...d.k
+000016c0: 0272 3c7c 0464 0364 0085 0219 007d 0674  .r<|.d.d.....}.t
+000016d0: 016a 037d 056e 047c 047d 067c 066a 0464  .j.}.n.|.}.|.j.d
+000016e0: 0483 0164 0119 007c 006a 056a 066a 076b  ...d...|.j.j.j.k
+000016f0: 0670 607c 067c 006a 086b 0673 7674 0964  .p`|.|.j.k.svt.d
+00001700: 056a 0a7c 067c 006a 056a 0b83 0283 0182  .j.|.|.j.j......
+00001710: 017c 036a 0c7c 067c 0566 0283 0101 0071  .|.j.|.|.f.....q
+00001720: 1257 007c 037c 025f 0d7c 0253 0029 064e  .W.|.|._.|.S.).N
+00001730: 7201 0000 00fa 012d 7225 0000 0072 4800  r......-r%...rH.
+00001740: 0000 7a1d 556e 6b6e 6f77 6e20 6669 656c  ..z.Unknown fiel
+00001750: 6420 7b7d 2066 6f72 206d 6f64 656c 207b  d {} for model {
+00001760: 7d29 0e72 6f00 0000 7203 0000 00da 0361  }).ro...r......a
+00001770: 7363 da04 6465 7363 724c 0000 0072 1200  sc..descrL...r..
+00001780: 0000 7227 0000 0072 0700 0000 7268 0000  ..r'...r....rh..
+00001790: 0072 0a00 0000 7242 0000 0072 4f00 0000  .r....rB...rO...
+000017a0: 7229 0000 0072 6500 0000 2907 7213 0000  r)...re...).r...
+000017b0: 0072 5000 0000 726e 0000 005a 0c6e 6577  .rP...rn...Z.new
+000017c0: 5f6f 7264 6572 696e 6772 5100 0000 5a0a  _orderingrQ...Z.
+000017d0: 6f72 6465 725f 7479 7065 7252 0000 0072  order_typerR...r
+000017e0: 1400 0000 7214 0000 0072 1500 0000 da08  ....r....r......
+000017f0: 6f72 6465 725f 6279 ba00 0000 7322 0000  order_by....s"..
+00001800: 0000 0108 0104 010a 0106 010c 010c 0108  ................
+00001810: 0204 0318 010a 0202 0104 0102 010c 0312  ................
+00001820: 0106 017a 1151 7565 7279 5365 742e 6f72  ...z.QuerySet.or
+00001830: 6465 725f 6279 6302 0000 0000 0000 0003  der_byc.........
+00001840: 0000 0002 0000 0043 0000 0073 1200 0000  .......C...s....
+00001850: 7c00 6a00 8300 7d02 7c01 7c02 5f01 7c02  |.j...}.|.|._.|.
+00001860: 5300 2901 4e29 0272 6f00 0000 7262 0000  S.).N).ro...rb..
+00001870: 0029 0372 1300 0000 da05 6c69 6d69 7472  .).r......limitr
+00001880: 6e00 0000 7214 0000 0072 1400 0000 7215  n...r....r....r.
+00001890: 0000 0072 7b00 0000 d300 0000 7306 0000  ...r{.......s...
+000018a0: 0000 0108 0106 017a 0e51 7565 7279 5365  .......z.QuerySe
+000018b0: 742e 6c69 6d69 7463 0200 0000 0000 0000  t.limitc........
+000018c0: 0300 0000 0200 0000 4300 0000 7312 0000  ........C...s...
+000018d0: 007c 006a 0083 007d 027c 017c 025f 017c  .|.j...}.|.|._.|
+000018e0: 0253 0029 014e 2902 726f 0000 0072 6300  .S.).N).ro...rc.
+000018f0: 0000 2903 7213 0000 00da 066f 6666 7365  ..).r......offse
+00001900: 7472 6e00 0000 7214 0000 0072 1400 0000  trn...r....r....
+00001910: 7215 0000 0072 7c00 0000 d800 0000 7306  r....r|.......s.
+00001920: 0000 0000 0108 0106 017a 0f51 7565 7279  .........z.Query
+00001930: 5365 742e 6f66 6673 6574 6301 0000 0000  Set.offsetc.....
+00001940: 0000 0002 0000 0002 0000 0043 0000 0073  ...........C...s
+00001950: 1200 0000 7c00 6a00 8300 7d01 6401 7c01  ....|.j...}.d.|.
+00001960: 5f01 7c01 5300 2902 4e54 2902 726f 0000  _.|.S.).NT).ro..
+00001970: 0072 6700 0000 2902 7213 0000 0072 6e00  .rg...).r....rn.
+00001980: 0000 7214 0000 0072 1400 0000 7215 0000  ..r....r....r...
+00001990: 00da 0864 6973 7469 6e63 74dd 0000 0073  ...distinct....s
+000019a0: 0600 0000 0001 0801 0601 7a11 5175 6572  ..........z.Quer
+000019b0: 7953 6574 2e64 6973 7469 6e63 7463 0100  ySet.distinctc..
+000019c0: 0000 0000 0000 0600 0000 0600 0000 4b00  ..............K.
+000019d0: 0000 735e 0000 007c 006a 0083 007d 0278  ..s^...|.j...}.x
+000019e0: 507c 016a 0183 0044 005d 445c 027d 037d  P|.j...D.]D\.}.}
+000019f0: 0474 027c 0474 0383 0273 2c74 0464 0183  .t.|.t...s,t.d..
+00001a00: 0182 017c 047c 026a 057c 033c 0064 0264  ...|.|.j.|.<.d.d
+00001a10: 036c 066d 077d 0501 007c 026a 086a 097c  .l.m.}...|.j.j.|
+00001a20: 057c 0364 007c 0383 0383 0101 0071 1257  .|.d.|.......q.W
+00001a30: 007c 0253 0029 044e 7a2a 7661 6c75 6520  .|.S.).Nz*value 
+00001a40: 6973 2065 7870 6563 7465 6420 746f 2062  is expected to b
+00001a50: 6520 4167 6772 6567 6174 6520 696e 7374  e Aggregate inst
+00001a60: 616e 6365 7201 0000 0029 01da 1567 6574  ancer....)...get
+00001a70: 5f66 696c 7465 7273 5f66 6f72 5f66 6965  _filters_for_fie
+00001a80: 6c64 290a 726f 0000 0072 2a00 0000 723b  ld).ro...r*...r;
+00001a90: 0000 0072 0800 0000 7270 0000 0072 6800  ...r....rp...rh.
+00001aa0: 0000 da0f 746f 7274 6f69 7365 2e6d 6f64  ....tortoise.mod
+00001ab0: 656c 7372 7e00 0000 726a 0000 00da 0675  elsr~...rj.....u
+00001ac0: 7064 6174 6529 0672 1300 0000 7274 0000  pdate).r....rt..
+00001ad0: 0072 6e00 0000 7236 0000 0072 3800 0000  .rn...r6...r8...
+00001ae0: 727e 0000 0072 1400 0000 7214 0000 0072  r~...r....r....r
+00001af0: 1500 0000 da08 616e 6e6f 7461 7465 e200  ......annotate..
+00001b00: 0000 7310 0000 0000 0108 0112 010a 0108  ..s.............
+00001b10: 010a 010c 0118 017a 1151 7565 7279 5365  .......z.QuerySe
+00001b20: 742e 616e 6e6f 7461 7465 4629 01da 0466  t.annotateF)...f
+00001b30: 6c61 7463 0100 0000 0100 0000 0300 0000  latc............
+00001b40: 0f00 0000 4700 0000 7338 0000 0074 007c  ....G...s8...t.|
+00001b50: 006a 017c 006a 027c 006a 037c 006a 047c  .j.|.j.|.j.|.j.|
+00001b60: 017c 027c 006a 057c 006a 067c 006a 077c  .|.|.j.|.j.|.j.|
+00001b70: 006a 087c 006a 097c 006a 0a7c 006a 0b64  .j.|.j.|.j.|.j.d
+00001b80: 018d 0d53 0029 024e 290d da02 6462 7212  ...S.).N)...dbr.
+00001b90: 0000 0072 3000 0000 7231 0000 0072 8200  ...r0...r1...r..
+00001ba0: 0000 da16 6669 656c 6473 5f66 6f72 5f73  ....fields_for_s
+00001bb0: 656c 6563 745f 6c69 7374 727d 0000 0072  elect_listr}...r
+00001bc0: 7b00 0000 727c 0000 0072 5000 0000 7232  {...r|...rP...r2
+00001bd0: 0000 0072 2f00 0000 7233 0000 0029 0cda  ...r/...r3...)..
+00001be0: 0f56 616c 7565 734c 6973 7451 7565 7279  .ValuesListQuery
+00001bf0: 7261 0000 0072 1200 0000 7264 0000 0072  ra...r....rd...r
+00001c00: 6600 0000 7267 0000 0072 6200 0000 7263  f...rg...rb...rc
+00001c10: 0000 0072 6500 0000 7268 0000 0072 6900  ...re...rh...ri.
+00001c20: 0000 726a 0000 0029 0372 1300 0000 7282  ..rj...).r....r.
+00001c30: 0000 0072 0700 0000 7214 0000 0072 1400  ...r....r....r..
+00001c40: 0000 7215 0000 00da 0b76 616c 7565 735f  ..r......values_
+00001c50: 6c69 7374 ec00 0000 731c 0000 0000 0102  list....s.......
+00001c60: 0104 0104 0104 0104 0102 0102 0104 0104  ................
+00001c70: 0104 0104 0104 0104 017a 1451 7565 7279  .........z.Query
+00001c80: 5365 742e 7661 6c75 6573 5f6c 6973 7463  Set.values_listc
+00001c90: 0100 0000 0000 0000 0600 0000 0e00 0000  ................
+00001ca0: 4f00 0000 739a 0000 0069 007d 0378 2a7c  O...s....i.}.x*|
+00001cb0: 0144 005d 227d 047c 047c 036b 0672 2474  .D.]"}.|.|.k.r$t
+00001cc0: 0064 016a 017c 0483 0183 0182 017c 047c  .d.j.|.......|.|
+00001cd0: 037c 043c 0071 0a57 0078 327c 026a 0283  .|.<.q.W.x2|.j..
+00001ce0: 0044 005d 265c 027d 057d 047c 057c 036b  .D.]&\.}.}.|.|.k
+00001cf0: 0672 5874 0064 016a 017c 0583 0183 0182  .rXt.d.j.|......
+00001d00: 017c 047c 037c 053c 0071 3a57 0074 037c  .|.|.|.<.q:W.t.|
+00001d10: 006a 047c 006a 057c 006a 067c 006a 077c  .j.|.j.|.j.|.j.|
+00001d20: 037c 006a 087c 006a 097c 006a 0a7c 006a  .|.j.|.j.|.j.|.j
+00001d30: 0b7c 006a 0c7c 006a 0d7c 006a 0e64 028d  .|.j.|.j.|.j.d..
+00001d40: 0c53 0029 034e 7a10 4475 706c 6963 6174  .S.).Nz.Duplicat
+00001d50: 6520 6b65 7920 7b7d 290c 7283 0000 0072  e key {}).r....r
+00001d60: 1200 0000 7230 0000 0072 3100 0000 da11  ....r0...r1.....
+00001d70: 6669 656c 6473 5f66 6f72 5f73 656c 6563  fields_for_selec
+00001d80: 7472 7d00 0000 727b 0000 0072 7c00 0000  tr}...r{...r|...
+00001d90: 7250 0000 0072 3200 0000 722f 0000 0072  rP...r2...r/...r
+00001da0: 3300 0000 290f 720a 0000 0072 4200 0000  3...).r....rB...
+00001db0: 722a 0000 00da 0b56 616c 7565 7351 7565  r*.....ValuesQue
+00001dc0: 7279 7261 0000 0072 1200 0000 7264 0000  ryra...r....rd..
+00001dd0: 0072 6600 0000 7267 0000 0072 6200 0000  .rf...rg...rb...
+00001de0: 7263 0000 0072 6500 0000 7268 0000 0072  rc...re...rh...r
+00001df0: 6900 0000 726a 0000 0029 0672 1300 0000  i...rj...).r....
+00001e00: 7273 0000 0072 7400 0000 7287 0000 0072  rs...rt...r....r
+00001e10: 1b00 0000 da09 7265 7475 726e 5f61 7372  ......return_asr
+00001e20: 1400 0000 7214 0000 0072 1500 0000 da06  ....r....r......
+00001e30: 7661 6c75 6573 fd00 0000 732c 0000 0000  values....s,....
+00001e40: 0104 010a 0108 010e 010c 0212 0108 010e  ................
+00001e50: 010c 0202 0104 0104 0104 0104 0102 0104  ................
+00001e60: 0104 0104 0104 0104 0104 017a 0f51 7565  ...........z.Que
+00001e70: 7279 5365 742e 7661 6c75 6573 6301 0000  rySet.valuesc...
+00001e80: 0000 0000 0001 0000 0009 0000 0043 0000  .............C..
+00001e90: 0073 2400 0000 7400 7c00 6a01 7c00 6a02  .s$...t.|.j.|.j.
+00001ea0: 7c00 6a03 7c00 6a04 7c00 6a05 7c00 6a06  |.j.|.j.|.j.|.j.
+00001eb0: 7c00 6a07 6401 8d07 5300 2902 4e29 0772  |.j.d...S.).N).r
+00001ec0: 8300 0000 7212 0000 0072 3000 0000 7231  ....r....r0...r1
+00001ed0: 0000 0072 3200 0000 722f 0000 0072 3300  ...r2...r/...r3.
+00001ee0: 0000 2908 da0b 4465 6c65 7465 5175 6572  ..)...DeleteQuer
+00001ef0: 7972 6100 0000 7212 0000 0072 6400 0000  yra...r....rd...
+00001f00: 7266 0000 0072 6800 0000 7269 0000 0072  rf...rh...ri...r
+00001f10: 6a00 0000 2901 7213 0000 0072 1400 0000  j...).r....r....
+00001f20: 7214 0000 0072 1500 0000 da06 6465 6c65  r....r......dele
+00001f30: 7465 1801 0000 7310 0000 0000 0102 0104  te....s.........
+00001f40: 0104 0104 0104 0104 0104 017a 0f51 7565  ...........z.Que
+00001f50: 7279 5365 742e 6465 6c65 7465 6301 0000  rySet.deletec...
+00001f60: 0000 0000 0002 0000 000a 0000 004b 0000  .............K..
+00001f70: 0073 2600 0000 7400 7c00 6a01 7c00 6a02  .s&...t.|.j.|.j.
+00001f80: 7c00 6a03 7c01 7c00 6a04 7c00 6a05 7c00  |.j.|.|.j.|.j.|.
+00001f90: 6a06 7c00 6a07 6401 8d08 5300 2902 4e29  j.|.j.d...S.).N)
+00001fa0: 0872 8300 0000 7212 0000 0072 3000 0000  .r....r....r0...
+00001fb0: da0d 7570 6461 7465 5f6b 7761 7267 7372  ..update_kwargsr
+00001fc0: 3100 0000 7232 0000 0072 2f00 0000 7233  1...r2...r/...r3
+00001fd0: 0000 0029 08da 0b55 7064 6174 6551 7565  ...)...UpdateQue
+00001fe0: 7279 7261 0000 0072 1200 0000 7264 0000  ryra...r....rd..
+00001ff0: 0072 6600 0000 7268 0000 0072 6900 0000  .rf...rh...ri...
+00002000: 726a 0000 0029 0272 1300 0000 7274 0000  rj...).r....rt..
+00002010: 0072 1400 0000 7214 0000 0072 1500 0000  .r....r....r....
+00002020: 7280 0000 0023 0100 0073 1200 0000 0001  r....#...s......
+00002030: 0201 0401 0401 0401 0201 0401 0401 0401  ................
+00002040: 7a0f 5175 6572 7953 6574 2e75 7064 6174  z.QuerySet.updat
+00002050: 6563 0100 0000 0000 0000 0100 0000 0900  ec..............
+00002060: 0000 4300 0000 7324 0000 0074 007c 006a  ..C...s$...t.|.j
+00002070: 017c 006a 027c 006a 037c 006a 047c 006a  .|.j.|.j.|.j.|.j
+00002080: 057c 006a 067c 006a 0764 018d 0753 0029  .|.j.|.j.d...S.)
+00002090: 024e 2907 7283 0000 0072 1200 0000 7230  .N).r....r....r0
+000020a0: 0000 0072 3100 0000 7232 0000 0072 2f00  ...r1...r2...r/.
+000020b0: 0000 7233 0000 0029 08da 0a43 6f75 6e74  ..r3...)...Count
+000020c0: 5175 6572 7972 6100 0000 7212 0000 0072  Queryra...r....r
+000020d0: 6400 0000 7266 0000 0072 6800 0000 7269  d...rf...rh...ri
+000020e0: 0000 0072 6a00 0000 2901 7213 0000 0072  ...rj...).r....r
+000020f0: 1400 0000 7214 0000 0072 1500 0000 da05  ....r....r......
+00002100: 636f 756e 742f 0100 0073 1000 0000 0001  count/...s......
+00002110: 0201 0401 0401 0401 0401 0401 0401 7a0e  ..............z.
+00002120: 5175 6572 7953 6574 2e63 6f75 6e74 6301  QuerySet.countc.
+00002130: 0000 0000 0000 0001 0000 0001 0000 0043  ...............C
+00002140: 0000 0073 0800 0000 7c00 6a00 8300 5300  ...s....|.j...S.
+00002150: 2901 4e29 0172 6f00 0000 2901 7213 0000  ).N).ro...).r...
+00002160: 0072 1400 0000 7214 0000 0072 1500 0000  .r....r....r....
+00002170: da03 616c 6c3a 0100 0073 0200 0000 0001  ..all:...s......
+00002180: 7a0c 5175 6572 7953 6574 2e61 6c6c 6301  z.QuerySet.allc.
+00002190: 0000 0000 0000 0002 0000 0002 0000 0043  ...............C
+000021a0: 0000 0073 1800 0000 7c00 6a00 8300 7d01  ...s....|.j...}.
+000021b0: 6401 7c01 5f01 6402 7c01 5f02 7c01 5300  d.|._.d.|._.|.S.
+000021c0: 2903 4e72 2500 0000 5429 0372 6f00 0000  ).Nr%...T).ro...
+000021d0: 7262 0000 0072 5f00 0000 2902 7213 0000  rb...r_...).r...
+000021e0: 0072 6e00 0000 7214 0000 0072 1400 0000  .rn...r....r....
+000021f0: 7215 0000 00da 0566 6972 7374 3d01 0000  r......first=...
+00002200: 7308 0000 0000 0108 0106 0106 017a 0e51  s............z.Q
+00002210: 7565 7279 5365 742e 6669 7273 7463 0300  uerySet.firstc..
+00002220: 0000 0000 0000 0300 0000 0100 0000 4300  ..............C.
+00002230: 0000 7304 0000 0064 0053 0029 014e 7214  ..s....d.S.).Nr.
+00002240: 0000 0029 0372 1300 0000 726e 0000 005a  ...).r....rn...Z
+00002250: 0870 7265 6665 7463 6872 1400 0000 7214  .prefetchr....r.
+00002260: 0000 0072 1500 0000 da18 5f72 6573 6f6c  ...r......_resol
+00002270: 7665 5f70 7265 6665 7463 685f 6f62 6a65  ve_prefetch_obje
+00002280: 6374 4301 0000 7302 0000 0000 017a 2151  ctC...s......z!Q
+00002290: 7565 7279 5365 742e 5f72 6573 6f6c 7665  uerySet._resolve
+000022a0: 5f70 7265 6665 7463 685f 6f62 6a65 6374  _prefetch_object
+000022b0: 6301 0000 0000 0000 0007 0000 0005 0000  c...............
+000022c0: 0047 0000 0073 ac00 0000 7c00 6a00 8300  .G...s....|.j...
+000022d0: 7d02 6900 7c02 5f01 7898 7c01 4400 5d90  }.i.|._.x.|.D.].
+000022e0: 7d03 7402 7c03 7403 8302 722e 7c03 6a04  }.t.|.t...r.|.j.
+000022f0: 7c02 8301 0100 7114 7c03 6a05 6401 8301  |.....q.|.j.d...
+00002300: 7d04 7c04 6402 1900 7d05 7c05 7c00 6a06  }.|.d...}.|.|.j.
+00002310: 6a07 6a08 6b07 7264 7409 6403 6a0a 7c05  j.j.k.rdt.d.j.|.
+00002320: 7c00 6a06 6a07 6a0b 8302 8301 8201 7c05  |.j.j.j.......|.
+00002330: 7c02 6a01 6a0c 8300 6b07 727e 740d 8300  |.j.j...k.r~t...
+00002340: 7c02 6a01 7c05 3c00 6401 6a0e 7c04 6404  |.j.|.<.d.j.|.d.
+00002350: 6400 8502 1900 8301 7d06 7c06 7214 7c02  d.......}.|.r.|.
+00002360: 6a01 7c05 1900 6a0f 7c06 8301 0100 7114  j.|...j.|.....q.
+00002370: 5700 7c02 5300 2905 4e72 4800 0000 7201  W.|.S.).NrH...r.
+00002380: 0000 007a 1c72 656c 6174 696f 6e20 7b7d  ...z.relation {}
+00002390: 2066 6f72 207b 7d20 6e6f 7420 666f 756e   for {} not foun
+000023a0: 6472 2500 0000 2910 726f 0000 0072 5d00  dr%...).ro...r].
+000023b0: 0000 723b 0000 0072 0c00 0000 5a14 7265  ..r;...r....Z.re
+000023c0: 736f 6c76 655f 666f 725f 7175 6572 7973  solve_for_querys
+000023d0: 6574 724c 0000 0072 1200 0000 7227 0000  etrL...r....r'..
+000023e0: 0072 4a00 0000 720a 0000 0072 4200 0000  .rJ...r....rB...
+000023f0: 7217 0000 00da 046b 6579 73da 0373 6574  r......keys..set
+00002400: 721c 0000 00da 0361 6464 2907 7213 0000  r......add).r...
+00002410: 0072 7300 0000 726e 0000 00da 0872 656c  .rs...rn.....rel
+00002420: 6174 696f 6eda 0e72 656c 6174 696f 6e5f  ation..relation_
+00002430: 7370 6c69 74da 1166 6972 7374 5f6c 6576  split..first_lev
+00002440: 656c 5f66 6965 6c64 da12 666f 7277 6172  el_field..forwar
+00002450: 6465 645f 7072 6566 6574 6368 7214 0000  ded_prefetchr...
+00002460: 0072 1400 0000 7215 0000 00da 1070 7265  .r....r......pre
+00002470: 6665 7463 685f 7265 6c61 7465 6446 0100  fetch_relatedF..
+00002480: 0073 2400 0000 0001 0801 0602 0a01 0a01  .s$.............
+00002490: 0a01 0201 0a01 0801 0e01 0201 0401 1003  ................
+000024a0: 0e01 0c01 1201 0401 1401 7a19 5175 6572  ..........z.Quer
+000024b0: 7953 6574 2e70 7265 6665 7463 685f 7265  ySet.prefetch_re
+000024c0: 6c61 7465 6429 0172 6100 0000 6302 0000  lated).ra...c...
+000024d0: 0000 0000 0003 0000 0002 0000 0043 0000  .............C..
+000024e0: 0073 1200 0000 7c00 6a00 8300 7d02 7c01  .s....|.j...}.|.
+000024f0: 7c02 5f01 7c02 5300 2901 4e29 0272 6f00  |._.|.S.).N).ro.
+00002500: 0000 7261 0000 0029 0372 1300 0000 7261  ..ra...).r....ra
+00002510: 0000 0072 6e00 0000 7214 0000 0072 1400  ...rn...r....r..
+00002520: 0000 7215 0000 00da 0875 7369 6e67 5f64  ..r......using_d
+00002530: 625d 0100 0073 0600 0000 0001 0801 0601  b]...s..........
+00002540: 7a11 5175 6572 7953 6574 2e75 7369 6e67  z.QuerySet.using
+00002550: 5f64 6263 0100 0000 0000 0000 0600 0000  _dbc............
+00002560: 0400 0000 4300 0000 7384 0000 007c 006a  ....C...s....|.j
+00002570: 0073 0a64 0053 0074 017c 006a 026a 036a  .s.d.S.t.|.j.j.j
+00002580: 0483 017d 017c 006a 056a 067c 016a 0783  ...}.|.j.j.|.j..
+00002590: 017c 005f 0578 567c 006a 006a 0883 0044  .|._.xV|.j.j...D
+000025a0: 005d 485c 027d 027d 037c 036a 097c 006a  .]H\.}.}.|.j.|.j
+000025b0: 0283 017d 0478 1a7c 0464 0119 0044 005d  ...}.x.|.d...D.]
+000025c0: 0e7d 057c 006a 0a7c 058e 0001 0071 5257  .}.|.j.|.....qRW
+000025d0: 007c 006a 056a 0b7c 0464 0219 006a 0c7c  .|.j.j.|.d...j.|
+000025e0: 0283 0183 017c 005f 0571 3457 0064 0053  .....|._.q4W.d.S
+000025f0: 0029 034e 5a05 6a6f 696e 7372 1b00 0000  .).NZ.joinsr....
+00002600: 290d 7268 0000 0072 0500 0000 7212 0000  ).rh...r....r...
+00002610: 0072 2700 0000 7217 0000 0072 1100 0000  .r'...r....r....
+00002620: da07 6772 6f75 7062 7972 1f00 0000 722a  ..groupbyr....r*
+00002630: 0000 0072 2800 0000 7247 0000 00da 0673  ...r(...rG.....s
+00002640: 656c 6563 74da 0361 735f 2906 7213 0000  elect..as_).r...
+00002650: 0072 1700 0000 7236 0000 005a 0961 6767  .r....r6...Z.agg
+00002660: 7265 6761 7465 7239 0000 0072 1c00 0000  regater9...r....
+00002670: 7214 0000 0072 1400 0000 7215 0000 00da  r....r....r.....
+00002680: 115f 7265 736f 6c76 655f 616e 6e6f 7461  ._resolve_annota
+00002690: 7465 6201 0000 7312 0000 0000 0106 0104  teb...s.........
+000026a0: 010e 0110 0114 010c 010e 010e 017a 1a51  .............z.Q
+000026b0: 7565 7279 5365 742e 5f72 6573 6f6c 7665  uerySet._resolve
+000026c0: 5f61 6e6e 6f74 6174 6563 0100 0000 0000  _annotatec......
+000026d0: 0000 0300 0000 0800 0000 4300 0000 73bc  ..........C...s.
+000026e0: 0000 007c 006a 0072 0c7c 006a 006e 087c  ...|.j.r.|.j.n.|
+000026f0: 006a 016a 026a 037d 0174 047c 006a 016a  .j.j.j.}.t.|.j.j
+00002700: 026a 0583 017d 027c 016a 066a 077c 0283  .j...}.|.j.j.|..
+00002710: 016a 087c 006a 098e 007c 005f 0a7c 006a  .j.|.j...|._.|.j
+00002720: 0b83 0001 007c 006a 0c7c 006a 017c 006a  .....|.j.|.j.|.j
+00002730: 0d7c 006a 0e7c 006a 0f7c 006a 107c 006a  .|.j.|.j.|.j.|.j
+00002740: 1164 018d 0601 007c 006a 1272 7a7c 006a  .d.....|.j.rz|.j
+00002750: 0a6a 137c 006a 1283 017c 005f 0a7c 006a  .j.|.j...|._.|.j
+00002760: 1472 907c 006a 0a6a 157c 006a 1483 017c  .r.|.j.j.|.j...|
+00002770: 005f 0a7c 006a 1672 a27c 006a 0a6a 1783  ._.|.j.r.|.j.j..
+00002780: 007c 005f 0a7c 006a 187c 006a 017c 006a  .|._.|.j.|.j.|.j
+00002790: 197c 006a 0f83 0301 007c 006a 0a53 0029  .|.j.....|.j.S.)
+000027a0: 024e 2906 7212 0000 0072 3000 0000 7231  .N).r....r0...r1
+000027b0: 0000 0072 3200 0000 722f 0000 0072 3300  ...r2...r/...r3.
+000027c0: 0000 291a 7261 0000 0072 1200 0000 7227  ..).ra...r....r'
+000027d0: 0000 0072 8300 0000 7205 0000 0072 1700  ...r....r....r..
+000027e0: 0000 da0b 7175 6572 795f 636c 6173 7372  ....query_classr
+000027f0: 5c00 0000 729e 0000 0072 0700 0000 7211  \...r....r....r.
+00002800: 0000 0072 a000 0000 723a 0000 0072 6400  ...r....r:...rd.
+00002810: 0000 7266 0000 0072 6800 0000 7269 0000  ..rf...rh...ri..
+00002820: 0072 6a00 0000 7262 0000 0072 7b00 0000  .rj...rb...r{...
+00002830: 7263 0000 0072 7c00 0000 7267 0000 0072  rc...r|...rg...r
+00002840: 7d00 0000 724d 0000 0072 6500 0000 2903  }...rM...re...).
+00002850: 7213 0000 0072 8300 0000 7217 0000 0072  r....r....r....r
+00002860: 1400 0000 7214 0000 0072 1500 0000 da0b  ....r....r......
+00002870: 5f6d 616b 655f 7175 6572 796d 0100 0073  _make_querym...s
+00002880: 2600 0000 0001 1601 0e01 1601 0801 0401  &...............
+00002890: 0401 0401 0401 0401 0401 0a02 0601 1001  ................
+000028a0: 0601 1001 0601 0c01 1401 7a14 5175 6572  ..........z.Quer
+000028b0: 7953 6574 2e5f 6d61 6b65 5f71 7565 7279  ySet._make_query
+000028c0: 6301 0000 0000 0000 0003 0000 0006 0000  c...............
+000028d0: 00c3 0000 0073 7800 0000 7c00 6a00 8300  .....sx...|.j...
+000028e0: 7c00 5f01 7c00 6a02 7216 7c00 6a02 6e08  |._.|.j.r.|.j.n.
+000028f0: 7c00 6a03 6a04 6a05 7d01 7c01 6a06 7c00  |.j.j.j.}.|.j.|.
+00002900: 6a03 7c01 7c00 6a07 7c00 6a08 6401 8d04  j.|.|.j.|.j.d...
+00002910: 6a09 7c00 6a01 740a 7c00 6a0b 6a0c 8300  j.|.j.t.|.j.j...
+00002920: 8301 6402 8d02 4900 6400 4800 7d02 7c02  ..d...I.d.H.}.|.
+00002930: 7366 7c00 6a0d 7262 6400 5300 6700 5300  sf|.j.rbd.S.g.S.
+00002940: 7c00 6a0d 7274 7c02 6403 1900 5300 7c02  |.j.rt|.d...S.|.
+00002950: 5300 2904 4e29 0472 1200 0000 7283 0000  S.).N).r....r...
+00002960: 00da 0c70 7265 6665 7463 685f 6d61 70da  ...prefetch_map.
+00002970: 1070 7265 6665 7463 685f 7175 6572 6965  .prefetch_querie
+00002980: 7329 01da 0d63 7573 746f 6d5f 6669 656c  s)...custom_fiel
+00002990: 6473 7201 0000 0029 0e72 a200 0000 7211  dsr....).r....r.
+000029a0: 0000 0072 6100 0000 7212 0000 0072 2700  ...ra...r....r'.
+000029b0: 0000 7283 0000 00da 0e65 7865 6375 746f  ..r......executo
+000029c0: 725f 636c 6173 7372 5d00 0000 725e 0000  r_classr]...r^..
+000029d0: 00da 0e65 7865 6375 7465 5f73 656c 6563  ...execute_selec
+000029e0: 7472 6d00 0000 7268 0000 0072 9400 0000  trm...rh...r....
+000029f0: 725f 0000 0029 0372 1300 0000 7283 0000  r_...).r....r...
+00002a00: 00da 0d69 6e73 7461 6e63 655f 6c69 7374  ...instance_list
+00002a10: 7214 0000 0072 1400 0000 7215 0000 0072  r....r....r....r
+00002a20: 5300 0000 8301 0000 731e 0000 0000 010a  S.......s.......
+00002a30: 0116 0104 0104 0102 0104 010a 021c 0204  ................
+00002a40: 0106 0104 0104 0106 0108 017a 1151 7565  ...........z.Que
+00002a50: 7279 5365 742e 5f65 7865 6375 7465 6301  rySet._executec.
+00002a60: 0000 0000 0000 0001 0000 0002 0000 0043  ...............C
+00002a70: 0000 0073 0800 0000 7400 7c00 8301 5300  ...s....t.|...S.
+00002a80: 2901 4e29 0172 0e00 0000 2901 7213 0000  ).N).r....).r...
+00002a90: 0072 1400 0000 7214 0000 0072 1500 0000  .r....r....r....
+00002aa0: da09 5f5f 6169 7465 725f 5f96 0100 0073  ..__aiter__....s
+00002ab0: 0200 0000 0001 7a12 5175 6572 7953 6574  ......z.QuerySet
+00002ac0: 2e5f 5f61 6974 6572 5f5f 291b 724f 0000  .__aiter__).rO..
+00002ad0: 0072 5600 0000 7257 0000 0072 1600 0000  .rV...rW...r....
+00002ae0: 726f 0000 0072 7600 0000 727a 0000 0072  ro...rv...rz...r
+00002af0: 7b00 0000 727c 0000 0072 7d00 0000 7281  {...r|...r}...r.
+00002b00: 0000 0072 8600 0000 728a 0000 0072 8c00  ...r....r....r..
+00002b10: 0000 7280 0000 0072 9000 0000 7291 0000  ..r....r....r...
+00002b20: 0072 9200 0000 7293 0000 0072 9b00 0000  .r....r....r....
+00002b30: 7209 0000 0072 9c00 0000 72a0 0000 0072  r....r....r....r
+00002b40: a200 0000 7253 0000 0072 a900 0000 da0d  ....rS...r......
+00002b50: 5f5f 636c 6173 7363 656c 6c5f 5f72 1400  __classcell__r..
+00002b60: 0000 7214 0000 0029 0172 6b00 0000 7215  ..r....).rk...r.
+00002b70: 0000 0072 5800 0000 7d00 0000 732c 0000  ...rX...}...s,..
 00002b80: 0008 010c 1508 1308 1408 1908 0508 0508  ................
 00002b90: 0508 0a0e 1108 1b08 0b08 0c08 0b08 0308  ................
-00002ba0: 0608 0308 170e 0508 0b08 1608 1372 5700  .............rW.
+00002ba0: 0608 0308 170e 0508 0b08 1608 1372 5800  .............rX.
 00002bb0: 0000 6300 0000 0000 0000 0000 0000 0003  ..c.............
 00002bc0: 0000 0000 0000 0073 2400 0000 6500 5a01  .......s$...e.Z.
 00002bd0: 6400 5a02 8700 6601 6401 6402 8408 5a03  d.Z...f.d.d...Z.
 00002be0: 6403 6404 8400 5a04 8700 0400 5a05 5300  d.d...Z.....Z.S.
-00002bf0: 2905 728d 0000 0063 0900 0000 0000 0000  ).r....c........
-00002c00: 0e00 0000 0800 0000 0300 0000 73d4 0000  ............s...
+00002bf0: 2905 728e 0000 0063 0900 0000 0000 0000  ).r....c........
+00002c00: 0e00 0000 0800 0000 0300 0000 73d2 0000  ............s...
 00002c10: 0074 0083 006a 0183 0001 007c 0472 127c  .t...j.....|.r.|
 00002c20: 046e 067c 016a 026a 037c 005f 0474 057c  .n.|.j.j.|._.t.|
 00002c30: 016a 026a 0683 017d 097c 006a 046a 076a  .j.j...}.|.j.j.j
 00002c40: 087c 0983 017c 005f 097c 006a 0a7c 017c  .|...|._.|.j.|.|
 00002c50: 027c 057c 067c 077c 0864 018d 0601 0078  .|.|.|.|.d.....x
-00002c60: 807c 036a 0b83 0044 005d 745c 027d 0a7d  .|.j...D.]t\.}.}
+00002c60: 7e7c 036a 0b83 0044 005d 725c 027d 0a7d  ~|.j...D.]r\.}.}
 00002c70: 0b7c 016a 026a 0c6a 0d7c 0a83 017d 0c7c  .|.j.j.j.|...}.|
 00002c80: 0c73 8274 0e64 026a 0f7c 0a7c 0183 0283  .s.t.d.j.|.|....
-00002c90: 0182 017c 0c6a 100c 0073 9274 1164 0383  ...|.j...s.t.d..
-00002ca0: 0182 0174 127c 0c74 136a 1483 0272 b064  ...t.|.t.j...r.d
-00002cb0: 046a 0f7c 0a83 017d 0d7c 0b6a 157d 0b6e  .j.|...}.|.j.}.n
-00002cc0: 0c7c 016a 026a 167c 0a19 007d 0d7c 006a  .|.j.j.|...}.|.j
-00002cd0: 096a 177c 0d7c 0b83 027c 005f 0971 5857  .j.|.|...|._.qXW
-00002ce0: 0064 0053 0029 054e 2906 7211 0000 0072  .d.S.).N).r....r
-00002cf0: 2f00 0000 7230 0000 0072 3100 0000 722e  /...r0...r1...r.
-00002d00: 0000 0072 3200 0000 7a28 556e 6b6e 6f77  ...r2...z(Unknow
-00002d10: 6e20 6b65 7977 6f72 6420 6172 6775 6d65  n keyword argume
-00002d20: 6e74 207b 7d20 666f 7220 6d6f 6465 6c20  nt {} for model 
-00002d30: 7b7d 7a2c 4669 656c 6420 7b7d 2069 7320  {}z,Field {} is 
-00002d40: 6765 6e65 7261 7465 6420 616e 6420 6361  generated and ca
-00002d50: 6e20 6e6f 7420 6265 2075 7064 6174 6564  n not be updated
-00002d60: 7a05 7b7d 5f69 6429 1872 5800 0000 7215  z.{}_id).rX...r.
-00002d70: 0000 0072 2600 0000 7282 0000 0072 6000  ...r&...r....r`.
-00002d80: 0000 7205 0000 0072 1600 0000 72a0 0000  ..r....r....r...
-00002d90: 0072 7f00 0000 7210 0000 0072 3900 0000  .r....r....r9...
-00002da0: 7229 0000 0072 2c00 0000 722b 0000 0072  r)...r,...r+...r
-00002db0: 0a00 0000 7241 0000 00da 0967 656e 6572  ....rA.....gener
-00002dc0: 6174 6564 da0e 4173 7365 7274 696f 6e45  ated..AssertionE
-00002dd0: 7272 6f72 723a 0000 0072 0700 0000 da0f  rrorr:...r......
-00002de0: 466f 7265 6967 6e4b 6579 4669 656c 6472  ForeignKeyFieldr
-00002df0: 1e00 0000 da14 6669 656c 6473 5f64 625f  ......fields_db_
-00002e00: 7072 6f6a 6563 7469 6f6e 7294 0000 0029  projectionr....)
-00002e10: 0e72 1200 0000 7211 0000 0072 2f00 0000  .r....r....r/...
-00002e20: 728c 0000 0072 8200 0000 7230 0000 0072  r....r....r0...r
-00002e30: 3100 0000 722e 0000 0072 3200 0000 7216  1...r....r2...r.
-00002e40: 0000 0072 3500 0000 7222 0000 0072 3600  ...r5...r"...r6.
-00002e50: 0000 da08 6462 5f66 6965 6c64 2901 726a  ....db_field).rj
-00002e60: 0000 0072 1300 0000 7214 0000 0072 1500  ...r....r....r..
-00002e70: 0000 9c01 0000 732a 0000 0000 040a 0112  ......s*........
-00002e80: 010c 0110 0104 0102 0102 0102 0102 0102  ................
-00002e90: 0108 0312 010e 0104 0110 0110 010c 010a  ................
-00002ea0: 0108 020c 017a 1455 7064 6174 6551 7565  .....z.UpdateQue
-00002eb0: 7279 2e5f 5f69 6e69 745f 5f63 0100 0000  ry.__init__c....
-00002ec0: 0000 0000 0100 0000 0300 0000 c300 0000  ................
-00002ed0: 731c 0000 007c 006a 006a 0174 027c 006a  s....|.j.j.t.|.j
-00002ee0: 0383 0183 0149 0064 0048 0001 0064 0053  .....I.d.H...d.S
-00002ef0: 0029 014e 2904 7260 0000 00da 0d65 7865  .).N).r`.....exe
-00002f00: 6375 7465 5f71 7565 7279 da03 7374 7272  cute_query..strr
-00002f10: 1000 0000 2901 7212 0000 0072 1300 0000  ....).r....r....
-00002f20: 7213 0000 0072 1400 0000 7252 0000 00b9  r....r....rR....
-00002f30: 0100 0073 0200 0000 0001 7a14 5570 6461  ...s......z.Upda
-00002f40: 7465 5175 6572 792e 5f65 7865 6375 7465  teQuery._execute
-00002f50: 2906 724e 0000 0072 5500 0000 7256 0000  ).rN...rU...rV..
-00002f60: 0072 1500 0000 7252 0000 0072 aa00 0000  .r....rR...r....
-00002f70: 7213 0000 0072 1300 0000 2901 726a 0000  r....r....).rj..
-00002f80: 0072 1400 0000 728d 0000 009b 0100 0073  .r....r........s
-00002f90: 0400 0000 0801 0c1d 728d 0000 0063 0000  ........r....c..
-00002fa0: 0000 0000 0000 0000 0000 0300 0000 0000  ................
-00002fb0: 0000 7324 0000 0065 005a 0164 005a 0287  ..s$...e.Z.d.Z..
-00002fc0: 0066 0164 0164 0284 085a 0364 0364 0484  .f.d.d...Z.d.d..
-00002fd0: 005a 0487 0004 005a 0553 0029 0572 8a00  .Z.....Z.S.).r..
-00002fe0: 0000 6308 0000 0000 0000 0009 0000 0008  ..c.............
-00002ff0: 0000 0003 0000 0073 5e00 0000 7400 8300  .......s^...t...
-00003000: 6a01 8300 0100 7c03 7212 7c03 6e06 7c01  j.....|.r.|.n.|.
-00003010: 6a02 6a03 7c00 5f04 7405 7c01 6a02 6a06  j.j.|._.t.|.j.j.
-00003020: 8301 7d08 7c00 6a04 6a07 6a08 7c08 8301  ..}.|.j.j.j.|...
-00003030: 7c00 5f09 7c00 6a0a 7c01 7c02 7c04 7c05  |._.|.j.|.|.|.|.
-00003040: 7c06 7c07 6401 8d06 0100 7c00 6a09 6a0b  |.|.d.....|.j.j.
-00003050: 8300 7c00 5f09 6400 5300 2902 4e29 0672  ..|._.d.S.).N).r
-00003060: 1100 0000 722f 0000 0072 3000 0000 7231  ....r/...r0...r1
-00003070: 0000 0072 2e00 0000 7232 0000 0029 0c72  ...r....r2...).r
-00003080: 5800 0000 7215 0000 0072 2600 0000 7282  X...r....r&...r.
-00003090: 0000 0072 6000 0000 7205 0000 0072 1600  ...r`...r....r..
-000030a0: 0000 72a0 0000 0072 5b00 0000 7210 0000  ..r....r[...r...
-000030b0: 0072 3900 0000 728b 0000 0029 0972 1200  .r9...r....).r..
-000030c0: 0000 7211 0000 0072 2f00 0000 7282 0000  ..r....r/...r...
-000030d0: 0072 3000 0000 7231 0000 0072 2e00 0000  .r0...r1...r....
-000030e0: 7232 0000 0072 1600 0000 2901 726a 0000  r2...r....).rj..
-000030f0: 0072 1300 0000 7214 0000 0072 1500 0000  .r....r....r....
-00003100: be01 0000 7318 0000 0000 010a 0112 010c  ....s...........
-00003110: 0110 0104 0102 0102 0102 0102 0102 0108  ................
-00003120: 027a 1444 656c 6574 6551 7565 7279 2e5f  .z.DeleteQuery._
-00003130: 5f69 6e69 745f 5f63 0100 0000 0000 0000  _init__c........
-00003140: 0100 0000 0300 0000 c300 0000 731c 0000  ............s...
-00003150: 007c 006a 006a 0174 027c 006a 0383 0183  .|.j.j.t.|.j....
-00003160: 0149 0064 0048 0001 0064 0053 0029 014e  .I.d.H...d.S.).N
-00003170: 2904 7260 0000 0072 b000 0000 72b1 0000  ).r`...r....r...
-00003180: 0072 1000 0000 2901 7212 0000 0072 1300  .r....).r....r..
-00003190: 0000 7213 0000 0072 1400 0000 7252 0000  ..r....r....rR..
-000031a0: 00cd 0100 0073 0200 0000 0001 7a14 4465  .....s......z.De
-000031b0: 6c65 7465 5175 6572 792e 5f65 7865 6375  leteQuery._execu
-000031c0: 7465 2906 724e 0000 0072 5500 0000 7256  te).rN...rU...rV
-000031d0: 0000 0072 1500 0000 7252 0000 0072 aa00  ...r....rR...r..
-000031e0: 0000 7213 0000 0072 1300 0000 2901 726a  ..r....r....).rj
-000031f0: 0000 0072 1400 0000 728a 0000 00bd 0100  ...r....r.......
-00003200: 0073 0400 0000 0801 0c0f 728a 0000 0063  .s........r....c
-00003210: 0000 0000 0000 0000 0000 0000 0300 0000  ................
-00003220: 0000 0000 7324 0000 0065 005a 0164 005a  ....s$...e.Z.d.Z
-00003230: 0287 0066 0164 0164 0284 085a 0364 0364  ...f.d.d...Z.d.d
-00003240: 0484 005a 0487 0004 005a 0553 0029 0572  ...Z.....Z.S.).r
-00003250: 8e00 0000 6308 0000 0000 0000 0009 0000  ....c...........
-00003260: 0008 0000 0003 0000 0073 6600 0000 7400  .........sf...t.
-00003270: 8300 6a01 8300 0100 7c03 7212 7c03 6e06  ..j.....|.r.|.n.
-00003280: 7c01 6a02 6a03 7c00 5f04 7405 7c01 6a02  |.j.j.|._.t.|.j.
-00003290: 6a06 8301 7d08 7c00 6a04 6a07 6a08 7c08  j...}.|.j.j.j.|.
-000032a0: 8301 7c00 5f09 7c00 6a0a 7c01 7c02 7c04  ..|._.|.j.|.|.|.
-000032b0: 7c05 7c06 7c07 6401 8d06 0100 7c00 6a09  |.|.|.d.....|.j.
-000032c0: 6a0b 740c 7c08 6a0d 8301 8301 7c00 5f09  j.t.|.j.....|._.
-000032d0: 6400 5300 2902 4e29 0672 1100 0000 722f  d.S.).N).r....r/
-000032e0: 0000 0072 3000 0000 7231 0000 0072 2e00  ...r0...r1...r..
-000032f0: 0000 7232 0000 0029 0e72 5800 0000 7215  ..r2...).rX...r.
-00003300: 0000 0072 2600 0000 7282 0000 0072 6000  ...r&...r....r`.
-00003310: 0000 7205 0000 0072 1600 0000 72a0 0000  ..r....r....r...
-00003320: 0072 5b00 0000 7210 0000 0072 3900 0000  .r[...r....r9...
-00003330: 729d 0000 0072 0600 0000 da04 7374 6172  r....r......star
-00003340: 2909 7212 0000 0072 1100 0000 722f 0000  ).r....r....r/..
-00003350: 0072 8200 0000 7230 0000 0072 3100 0000  .r....r0...r1...
-00003360: 722e 0000 0072 3200 0000 7216 0000 0029  r....r2...r....)
-00003370: 0172 6a00 0000 7213 0000 0072 1400 0000  .rj...r....r....
-00003380: 7215 0000 00d2 0100 0073 1800 0000 0001  r........s......
-00003390: 0a01 1201 0c01 1001 0401 0201 0201 0201  ................
-000033a0: 0201 0201 0802 7a13 436f 756e 7451 7565  ......z.CountQue
-000033b0: 7279 2e5f 5f69 6e69 745f 5f63 0100 0000  ry.__init__c....
-000033c0: 0000 0000 0200 0000 0400 0000 c300 0000  ................
-000033d0: 7330 0000 007c 006a 006a 0174 027c 006a  s0...|.j.j.t.|.j
-000033e0: 0383 0183 0149 0064 0048 007d 0174 0474  .....I.d.H.}.t.t
-000033f0: 057c 0164 0119 0083 016a 0683 0083 0164  .|.d.....j.....d
-00003400: 0119 0053 0029 024e 7201 0000 0029 0772  ...S.).Nr....).r
-00003410: 6000 0000 72b0 0000 0072 b100 0000 7210  `...r....r....r.
-00003420: 0000 0072 6c00 0000 726b 0000 0072 8900  ...rl...rk...r..
-00003430: 0000 2902 7212 0000 0072 a800 0000 7213  ..).r....r....r.
-00003440: 0000 0072 1300 0000 7214 0000 0072 5200  ...r....r....rR.
-00003450: 0000 e101 0000 7304 0000 0000 0118 017a  ......s........z
-00003460: 1343 6f75 6e74 5175 6572 792e 5f65 7865  .CountQuery._exe
-00003470: 6375 7465 2906 724e 0000 0072 5500 0000  cute).rN...rU...
-00003480: 7256 0000 0072 1500 0000 7252 0000 0072  rV...r....rR...r
-00003490: aa00 0000 7213 0000 0072 1300 0000 2901  ....r....r....).
-000034a0: 726a 0000 0072 1400 0000 728e 0000 00d1  rj...r....r.....
-000034b0: 0100 0073 0400 0000 0801 0c0f 728e 0000  ...s........r...
-000034c0: 0063 0000 0000 0000 0000 0000 0000 0200  .c..............
-000034d0: 0000 4000 0000 7324 0000 0065 005a 0164  ..@...s$...e.Z.d
-000034e0: 005a 0264 0164 0284 005a 0364 0364 0484  .Z.d.d...Z.d.d..
-000034f0: 005a 0464 0564 0684 005a 0564 0753 0029  .Z.d.d...Z.d.S.)
-00003500: 08da 1046 6965 6c64 5365 6c65 6374 5175  ...FieldSelectQu
-00003510: 6572 7963 0400 0000 0000 0000 0800 0000  eryc............
-00003520: 0700 0000 4300 0000 73d6 0000 0074 007c  ....C...s....t.|
-00003530: 016a 016a 0283 017d 047c 027c 016a 016a  .j.j...}.|.|.j.j
-00003540: 036b 0672 327c 030c 0072 327c 016a 016a  .k.r2|...r2|.j.j
-00003550: 037c 0219 007d 057c 047c 0566 0253 007c  .|...}.|.|.f.S.|
-00003560: 027c 016a 016a 036b 0672 547c 0372 5474  .|.j.j.k.rT|.rTt
-00003570: 0464 016a 057c 027c 016a 0683 0283 0182  .d.j.|.|.j......
-00003580: 017c 027c 006a 076a 016a 086b 0672 767c  .|.|.j.j.j.k.rv|
-00003590: 030c 0072 7674 0964 026a 057c 0283 0183  ...rvt.d.j.|....
-000035a0: 0182 017c 016a 016a 0a6a 0b7c 0283 017d  ...|.j.j.j.|...}
-000035b0: 067c 0673 9a74 0464 036a 057c 027c 016a  .|.s.t.d.j.|.|.j
-000035c0: 0683 0283 0182 017c 006a 0c7c 047c 027c  .......|.j.|.|.|
-000035d0: 0683 0301 007c 036a 0d64 0483 017d 077c  .....|.j.d...}.|
-000035e0: 006a 0e7c 066a 0f7c 0764 0519 0064 046a  .j.|.j.|.d...d.j
-000035f0: 107c 0764 0664 0085 0219 0083 0164 078d  .|.d.d.......d..
-00003600: 0353 0029 084e 7a29 4669 656c 6420 227b  .S.).Nz)Field "{
-00003610: 7d22 2066 6f72 206d 6f64 656c 2022 7b7d  }" for model "{}
-00003620: 2220 6973 206e 6f74 2072 656c 6174 696f  " is not relatio
-00003630: 6e7a 4f53 656c 6563 7469 6e67 2072 656c  nzOSelecting rel
-00003640: 6174 696f 6e20 227b 7d22 2069 7320 6e6f  ation "{}" is no
-00003650: 7420 706f 7373 6962 6c65 2c20 7365 6c65  t possible, sele
-00003660: 6374 2063 6f6e 6372 6574 6520 6669 656c  ct concrete fiel
-00003670: 6420 6f6e 2072 656c 6174 6564 206d 6f64  d on related mod
-00003680: 656c 7a21 556e 6b6e 6f77 6e20 6669 656c  elz!Unknown fiel
-00003690: 6420 227b 7d22 2066 6f72 206d 6f64 656c  d "{}" for model
-000036a0: 2022 7b7d 2272 4700 0000 7201 0000 0072   "{}"rG...r....r
-000036b0: 2400 0000 2903 7211 0000 0072 1a00 0000  $...).r....r....
-000036c0: da10 666f 7277 6172 6465 645f 6669 656c  ..forwarded_fiel
-000036d0: 6473 2911 7205 0000 0072 2600 0000 7216  ds).r....r&...r.
-000036e0: 0000 0072 ae00 0000 720a 0000 0072 4100  ...r....r....rA.
-000036f0: 0000 724e 0000 0072 1100 0000 7249 0000  ..rN...r....rI..
-00003700: 0072 4a00 0000 722c 0000 0072 2b00 0000  .rJ...r,...r+...
-00003710: 7246 0000 0072 4b00 0000 da21 5f6a 6f69  rF...rK....!_joi
-00003720: 6e5f 7461 626c 655f 7769 7468 5f66 6f72  n_table_with_for
-00003730: 7761 7264 6564 5f66 6965 6c64 7372 3c00  warded_fieldsr<.
-00003740: 0000 721b 0000 0029 0872 1200 0000 7211  ..r....).r....r.
-00003750: 0000 0072 1a00 0000 72b4 0000 0072 1600  ...r....r....r..
-00003760: 0000 72af 0000 0072 3600 0000 5a16 666f  ..r....r6...Z.fo
-00003770: 7277 6172 6465 645f 6669 656c 6473 5f73  rwarded_fields_s
-00003780: 706c 6974 7213 0000 0072 1300 0000 7214  plitr....r....r.
-00003790: 0000 0072 b500 0000 e701 0000 7330 0000  ...r........s0..
-000037a0: 0000 010c 0112 010c 0108 0110 0102 0104  ................
-000037b0: 0102 010a 0414 0102 0104 0108 030e 0104  ................
-000037c0: 0106 0102 010a 030e 010a 0104 0104 0106  ................
-000037d0: 017a 3246 6965 6c64 5365 6c65 6374 5175  .z2FieldSelectQu
-000037e0: 6572 792e 5f6a 6f69 6e5f 7461 626c 655f  ery._join_table_
-000037f0: 7769 7468 5f66 6f72 7761 7264 6564 5f66  with_forwarded_f
-00003800: 6965 6c64 7363 0300 0000 0000 0000 0800  ieldsc..........
-00003810: 0000 0700 0000 4300 0000 73de 0000 0074  ......C...s....t
-00003820: 007c 006a 016a 026a 0383 017d 037c 017c  .|.j.j.j...}.|.|
-00003830: 006a 016a 026a 046b 0672 487c 006a 016a  .j.j.j.k.rH|.j.j
-00003840: 026a 047c 0119 007d 047c 006a 056a 0674  .j.|...}.|.j.j.t
-00003850: 077c 037c 0483 026a 087c 0283 0183 017c  .|.|...j.|.....|
-00003860: 005f 0564 0053 007c 017c 006a 016a 026a  ._.d.S.|.|.j.j.j
-00003870: 096b 0672 6474 0a64 016a 0b7c 0183 0183  .k.rdt.d.j.|....
-00003880: 0182 017c 016a 0c64 0283 017d 057c 0564  ...|.j.d...}.|.d
-00003890: 0319 007c 006a 016a 026a 096b 0672 c67c  ...|.j.j.j.k.r.|
-000038a0: 006a 0d7c 006a 017c 0564 0319 0064 026a  .j.|.j.|.d...d.j
-000038b0: 0e7c 0564 0464 0085 0219 0083 0164 058d  .|.d.d.......d..
-000038c0: 035c 027d 067d 077c 006a 056a 0674 077c  .\.}.}.|.j.j.t.|
-000038d0: 067c 0783 026a 087c 0283 0183 017c 005f  .|...j.|.....|._
-000038e0: 0564 0053 0074 0f64 066a 0b7c 017c 006a  .d.S.t.d.j.|.|.j
-000038f0: 016a 1083 0283 0182 0164 0053 0029 074e  .j.......d.S.).N
-00003900: 7a4f 5365 6c65 6374 696e 6720 7265 6c61  zOSelecting rela
-00003910: 7469 6f6e 2022 7b7d 2220 6973 206e 6f74  tion "{}" is not
-00003920: 2070 6f73 7369 626c 652c 2073 656c 6563   possible, selec
-00003930: 7420 636f 6e63 7265 7465 2066 6965 6c64  t concrete field
-00003940: 206f 6e20 7265 6c61 7465 6420 6d6f 6465   on related mode
-00003950: 6c72 4700 0000 7201 0000 0072 2400 0000  lrG...r....r$...
-00003960: 2903 7211 0000 0072 1a00 0000 72b4 0000  ).r....r....r...
-00003970: 007a 2155 6e6b 6e6f 776e 2066 6965 6c64  .z!Unknown field
-00003980: 2022 7b7d 2220 666f 7220 6d6f 6465 6c20   "{}" for model 
-00003990: 227b 7d22 2911 7205 0000 0072 1100 0000  "{}").r....r....
-000039a0: 7226 0000 0072 1600 0000 72ae 0000 0072  r&...r....r....r
-000039b0: 1000 0000 729d 0000 0072 1f00 0000 729e  ....r....r....r.
-000039c0: 0000 0072 4900 0000 724a 0000 0072 4100  ...rI...rJ...rA.
-000039d0: 0000 724b 0000 0072 b500 0000 721b 0000  ..rK...r....r...
-000039e0: 0072 0a00 0000 724e 0000 0029 0872 1200  .r....rN...).r..
-000039f0: 0000 721a 0000 0072 8800 0000 7216 0000  ..r....r....r...
-00003a00: 0072 af00 0000 da0b 6669 656c 645f 7370  .r......field_sp
-00003a10: 6c69 7472 4400 0000 5a10 7265 6c61 7465  litrD...Z.relate
-00003a20: 645f 6462 5f66 6965 6c64 7213 0000 0072  d_db_fieldr....r
-00003a30: 1300 0000 7214 0000 00da 1961 6464 5f66  ....r......add_f
-00003a40: 6965 6c64 5f74 6f5f 7365 6c65 6374 5f71  ield_to_select_q
-00003a50: 7565 7279 0902 0000 7328 0000 0000 010e  uery....s(......
-00003a60: 010e 010e 011a 0104 020e 0102 0104 0108  ................
-00003a70: 030a 0112 0104 0104 0106 011a 021a 0104  ................
-00003a80: 0206 0102 017a 2a46 6965 6c64 5365 6c65  .....z*FieldSele
-00003a90: 6374 5175 6572 792e 6164 645f 6669 656c  ctQuery.add_fiel
-00003aa0: 645f 746f 5f73 656c 6563 745f 7175 6572  d_to_select_quer
-00003ab0: 7963 0300 0000 0000 0000 0500 0000 0600  yc..............
-00003ac0: 0000 4300 0000 7388 0000 007c 027c 016a  ..C...s....|.|.j
-00003ad0: 006a 016b 0672 1464 0164 0284 0053 007c  .j.k.r.d.d...S.|
-00003ae0: 027c 016a 006a 026b 0672 2e7c 016a 006a  .|.j.j.k.r.|.j.j
-00003af0: 027c 0219 006a 0353 007c 026a 0464 0383  .|...j.S.|.j.d..
-00003b00: 017d 037c 0364 0419 007c 016a 006a 016b  .}.|.d...|.j.j.k
-00003b10: 0672 747c 016a 006a 027c 0364 0419 0019  .rt|.j.j.|.d....
-00003b20: 006a 057d 047c 006a 067c 0464 036a 077c  .j.}.|.j.|.d.j.|
-00003b30: 0364 0564 0085 0219 0083 0183 0253 0074  .d.d.........S.t
-00003b40: 0864 066a 097c 027c 0183 0283 0182 0164  .d.j.|.|.......d
-00003b50: 0053 0029 074e 6301 0000 0000 0000 0001  .S.).Nc.........
-00003b60: 0000 0001 0000 0053 0000 0073 0400 0000  .......S...s....
-00003b70: 7c00 5300 2901 4e72 1300 0000 2901 da01  |.S.).Nr....)...
-00003b80: 7872 1300 0000 7213 0000 0072 1400 0000  xr....r....r....
-00003b90: da08 3c6c 616d 6264 613e 2802 0000 7300  ..<lambda>(...s.
-00003ba0: 0000 007a 3a46 6965 6c64 5365 6c65 6374  ...z:FieldSelect
-00003bb0: 5175 6572 792e 7265 736f 6c76 655f 746f  Query.resolve_to
-00003bc0: 5f70 7974 686f 6e5f 7661 6c75 652e 3c6c  _python_value.<l
-00003bd0: 6f63 616c 733e 2e3c 6c61 6d62 6461 3e72  ocals>.<lambda>r
-00003be0: 4700 0000 7201 0000 0072 2400 0000 7a21  G...r....r$...z!
-00003bf0: 556e 6b6e 6f77 6e20 6669 656c 6420 227b  Unknown field "{
-00003c00: 7d22 2066 6f72 206d 6f64 656c 2022 7b7d  }" for model "{}
-00003c10: 2229 0a72 2600 0000 7249 0000 0072 2c00  ").r&...rI...r,.
-00003c20: 0000 da0f 746f 5f70 7974 686f 6e5f 7661  ....to_python_va
-00003c30: 6c75 6572 4b00 0000 723c 0000 00da 1772  luerK...r<.....r
-00003c40: 6573 6f6c 7665 5f74 6f5f 7079 7468 6f6e  esolve_to_python
-00003c50: 5f76 616c 7565 721b 0000 0072 0a00 0000  _valuer....r....
-00003c60: 7241 0000 0029 0572 1200 0000 7211 0000  rA...).r....r...
-00003c70: 0072 1a00 0000 72b6 0000 005a 096e 6577  .r....r....Z.new
-00003c80: 5f6d 6f64 656c 7213 0000 0072 1300 0000  _modelr....r....
-00003c90: 7214 0000 0072 bb00 0000 2502 0000 7316  r....r....%...s.
-00003ca0: 0000 0000 010c 0208 020c 010e 020a 0110  ................
-00003cb0: 0112 011a 0206 0102 017a 2846 6965 6c64  .........z(Field
-00003cc0: 5365 6c65 6374 5175 6572 792e 7265 736f  SelectQuery.reso
-00003cd0: 6c76 655f 746f 5f70 7974 686f 6e5f 7661  lve_to_python_va
-00003ce0: 6c75 654e 2906 724e 0000 0072 5500 0000  lueN).rN...rU...
-00003cf0: 7256 0000 0072 b500 0000 72b7 0000 0072  rV...r....r....r
-00003d00: bb00 0000 7213 0000 0072 1300 0000 7213  ....r....r....r.
-00003d10: 0000 0072 1400 0000 72b3 0000 00e6 0100  ...r....r.......
-00003d20: 0073 0600 0000 0801 0822 081c 72b3 0000  .s......."..r...
-00003d30: 0063 0000 0000 0000 0000 0000 0000 0300  .c..............
-00003d40: 0000 0000 0000 7324 0000 0065 005a 0164  ......s$...e.Z.d
-00003d50: 005a 0287 0066 0164 0164 0284 085a 0364  .Z...f.d.d...Z.d
-00003d60: 0364 0484 005a 0487 0004 005a 0553 0029  .d...Z.....Z.S.)
-00003d70: 0572 8400 0000 630e 0000 0000 0000 0012  .r....c.........
-00003d80: 0000 0008 0000 0003 0000 0073 f200 0000  ...........s....
-00003d90: 7400 8300 6a01 8300 0100 7c0a 7222 7402  t...j.....|.r"t.
-00003da0: 7c05 8301 6401 6b03 7222 7403 6402 8301  |...d.k.r"t.d...
-00003db0: 8201 7c01 7c00 5f04 7405 7c01 6a06 6a07  ..|.|._.t.|.j.j.
-00003dc0: 8301 7d0e 7c03 723c 7c03 6e06 7c01 6a06  ..}.|.r<|.n.|.j.
-00003dd0: 6a08 7c00 5f09 7c00 6a09 6a0a 6a0b 7c0e  j.|._.|.j.j.j.|.
-00003de0: 8301 7c00 5f0c 6403 6404 8400 740d 7c05  ..|._.d.d...t.|.
-00003df0: 8301 4400 8301 7d0f 7820 7c0f 6a0e 8300  ..D...}.x |.j...
-00003e00: 4400 5d14 5c02 7d10 7d11 7c00 6a0f 7c11  D.].\.}.}.|.j.|.
-00003e10: 7c10 8302 0100 7172 5700 7c00 6a10 7c01  |.....qrW.|.j.|.
-00003e20: 7c02 7c04 7c0b 7c0c 7c0d 6405 8d06 0100  |.|.|.|.|.d.....
-00003e30: 7c06 72b2 7c00 6a0c 6a11 7c06 8301 7c00  |.r.|.j.j.|...|.
-00003e40: 5f0c 7c07 72c4 7c00 6a0c 6a12 7c07 8301  _.|.r.|.j.j.|...
-00003e50: 7c00 5f0c 7c08 72d4 7c00 6a0c 6a13 8300  |._.|.r.|.j.j...
-00003e60: 7c00 5f0c 7c00 6a14 7c01 7c09 7c0b 8303  |._.|.j.|.|.|...
-00003e70: 0100 7c0a 7c00 5f15 7c0f 7c00 5f16 6400  ..|.|._.|.|._.d.
-00003e80: 5300 2906 4e72 2400 0000 7a32 596f 7520  S.).Nr$...z2You 
-00003e90: 6361 6e20 666c 6174 2076 616c 7565 5f6c  can flat value_l
-00003ea0: 6973 7420 6f6e 6c79 2069 6620 636f 6e74  ist only if cont
-00003eb0: 6169 6e73 206f 6e65 2066 6965 6c64 6301  ains one fieldc.
-00003ec0: 0000 0000 0000 0003 0000 0005 0000 0053  ...............S
-00003ed0: 0000 0073 1a00 0000 6900 7c00 5d12 5c02  ...s....i.|.].\.
-00003ee0: 7d01 7d02 7c02 7400 7c01 8301 9302 7104  }.}.|.t.|.....q.
-00003ef0: 5300 7213 0000 0029 0172 b100 0000 2903  S.r....).r....).
-00003f00: da02 2e30 da01 6972 1a00 0000 7213 0000  ...0..ir....r...
-00003f10: 0072 1300 0000 7214 0000 00fa 0a3c 6469  .r....r......<di
-00003f20: 6374 636f 6d70 3e45 0200 0073 0200 0000  ctcomp>E...s....
-00003f30: 0600 7a2c 5661 6c75 6573 4c69 7374 5175  ..z,ValuesListQu
-00003f40: 6572 792e 5f5f 696e 6974 5f5f 2e3c 6c6f  ery.__init__.<lo
-00003f50: 6361 6c73 3e2e 3c64 6963 7463 6f6d 703e  cals>.<dictcomp>
-00003f60: 2906 7211 0000 0072 2f00 0000 7230 0000  ).r....r/...r0..
-00003f70: 0072 3100 0000 722e 0000 0072 3200 0000  .r1...r....r2...
-00003f80: 2917 7258 0000 0072 1500 0000 da03 6c65  ).rX...r......le
-00003f90: 6e72 6f00 0000 7211 0000 0072 0500 0000  nro...r....r....
-00003fa0: 7226 0000 0072 1600 0000 7282 0000 0072  r&...r....r....r
-00003fb0: 6000 0000 72a0 0000 0072 5b00 0000 7210  `...r....r[...r.
-00003fc0: 0000 00da 0965 6e75 6d65 7261 7465 7229  .....enumerater)
-00003fd0: 0000 0072 b700 0000 7239 0000 0072 7a00  ...r....r9...rz.
-00003fe0: 0000 727b 0000 0072 7c00 0000 724c 0000  ..r{...r|...rL..
-00003ff0: 0072 8100 0000 7207 0000 0029 1272 1200  .r....r....).r..
-00004000: 0000 7211 0000 0072 2f00 0000 7282 0000  ..r....r/...r...
-00004010: 0072 3000 0000 7283 0000 0072 7a00 0000  .r0...r....rz...
-00004020: 727b 0000 0072 7c00 0000 724f 0000 0072  r{...r|...rO...r
-00004030: 8100 0000 7231 0000 0072 2e00 0000 7232  ....r1...r....r2
-00004040: 0000 0072 1600 0000 7286 0000 005a 1170  ...r....r....Z.p
-00004050: 6f73 6974 696f 6e61 6c5f 6e75 6d62 6572  ositional_number
-00004060: 721a 0000 0029 0172 6a00 0000 7213 0000  r....).rj...r...
-00004070: 0072 1400 0000 7215 0000 0039 0200 0073  .r....r....9...s
-00004080: 3400 0000 0004 0a01 1001 0802 0601 0c01  4...............
-00004090: 1201 1001 1202 1201 1002 0401 0201 0201  ................
-000040a0: 0201 0201 0201 0802 0401 0e01 0401 0e01  ................
-000040b0: 0401 0c01 0e01 0601 7a18 5661 6c75 6573  ........z.Values
-000040c0: 4c69 7374 5175 6572 792e 5f5f 696e 6974  ListQuery.__init
-000040d0: 5f5f 6301 0000 0000 0000 0002 0000 0004  __c.............
-000040e0: 0000 0083 0000 0073 6e00 0000 8802 6a00  .......sn.....j.
-000040f0: 6a01 7402 8802 6a03 8301 8301 4900 6400  j.t...j.....I.d.
-00004100: 4800 7d01 8702 6601 6401 6402 8408 7404  H.}...f.d.d...t.
-00004110: 7405 8802 6a06 6a07 8300 8301 8301 4400  t...j.j.......D.
-00004120: 8301 8900 8802 6a08 725c 8800 6403 1900  ......j.r\..d...
-00004130: 6404 1900 8901 8701 6601 6405 6402 8408  d.......f.d.d...
-00004140: 7c01 4400 8301 5300 8700 6601 6406 6402  |.D...S...f.d.d.
-00004150: 8408 7c01 4400 8301 5300 2907 4e63 0100  ..|.D...S.).Nc..
-00004160: 0000 0000 0000 0300 0000 0600 0000 1300  ................
-00004170: 0000 7322 0000 0067 007c 005d 1a5c 027d  ..s"...g.|.].\.}
-00004180: 017d 027c 0188 006a 0088 006a 017c 0283  .}.|...j...j.|..
-00004190: 0266 0291 0271 0453 0072 1300 0000 2902  .f...q.S.r....).
-000041a0: 72bb 0000 0072 1100 0000 2903 72bc 0000  r....r....).r...
-000041b0: 0072 3500 0000 da04 6e61 6d65 2901 7212  .r5.....name).r.
-000041c0: 0000 0072 1300 0000 7214 0000 00fa 0a3c  ...r....r......<
-000041d0: 6c69 7374 636f 6d70 3e5f 0200 0073 0200  listcomp>_...s..
-000041e0: 0000 0601 7a2c 5661 6c75 6573 4c69 7374  ....z,ValuesList
-000041f0: 5175 6572 792e 5f65 7865 6375 7465 2e3c  Query._execute.<
-00004200: 6c6f 6361 6c73 3e2e 3c6c 6973 7463 6f6d  locals>.<listcom
-00004210: 703e 7201 0000 0072 2400 0000 6301 0000  p>r....r$...c...
-00004220: 0000 0000 0002 0000 0005 0000 0013 0000  ................
-00004230: 0073 1800 0000 6700 7c00 5d10 7d01 8800  .s....g.|.].}...
-00004240: 7c01 6400 1900 8301 9102 7104 5300 2901  |.d.......q.S.).
-00004250: da01 3072 1300 0000 2902 72bc 0000 00da  ..0r....).r.....
-00004260: 0565 6e74 7279 2901 da04 6675 6e63 7213  .entry)...funcr.
-00004270: 0000 0072 1400 0000 72c2 0000 0064 0200  ...r....r....d..
-00004280: 0073 0200 0000 0600 6301 0000 0000 0000  .s......c.......
-00004290: 0001 0000 0005 0000 0013 0000 0073 1e00  .............s..
-000042a0: 0000 6700 7c00 5d16 8900 8700 6601 6400  ..g.|.].....f.d.
-000042b0: 6401 8408 8801 4400 8301 9102 7104 5300  d.....D.....q.S.
-000042c0: 2902 6301 0000 0000 0000 0003 0000 0004  ).c.............
-000042d0: 0000 0033 0000 0073 1e00 0000 7c00 5d16  ...3...s....|.].
-000042e0: 5c02 7d01 7d02 7c02 8800 7c01 1900 8301  \.}.}.|...|.....
-000042f0: 5600 0100 7102 6400 5300 2901 4e72 1300  V...q.d.S.).Nr..
-00004300: 0000 2903 72bc 0000 00da 0663 6f6c 756d  ..).r......colum
-00004310: 6e72 c500 0000 2901 72c4 0000 0072 1300  nr....).r....r..
-00004320: 0000 7214 0000 00fa 093c 6765 6e65 7870  ..r......<genexp
-00004330: 723e 6502 0000 7302 0000 0004 007a 3656  r>e...s......z6V
-00004340: 616c 7565 734c 6973 7451 7565 7279 2e5f  aluesListQuery._
-00004350: 6578 6563 7574 652e 3c6c 6f63 616c 733e  execute.<locals>
-00004360: 2e3c 6c69 7374 636f 6d70 3e2e 3c67 656e  .<listcomp>.<gen
-00004370: 6578 7072 3e72 1300 0000 2901 72bc 0000  expr>r....).r...
-00004380: 0029 01da 0763 6f6c 756d 6e73 2901 72c4  .)...columns).r.
-00004390: 0000 0072 1400 0000 72c2 0000 0065 0200  ...r....r....e..
-000043a0: 0073 0200 0000 0600 2909 7260 0000 0072  .s......).r`...r
-000043b0: b000 0000 72b1 0000 0072 1000 0000 da06  ....r....r......
-000043c0: 736f 7274 6564 726c 0000 0072 0700 0000  sortedrl...r....
-000043d0: 7229 0000 0072 8100 0000 2902 7212 0000  r)...r....).r...
-000043e0: 0072 a800 0000 7213 0000 0029 0372 c800  .r....r....).r..
-000043f0: 0000 72c5 0000 0072 1200 0000 7214 0000  ..r....r....r...
-00004400: 0072 5200 0000 5c02 0000 730e 0000 0000  .rR...\...s.....
-00004410: 0118 020a 0116 0206 010c 0112 017a 1856  .............z.V
-00004420: 616c 7565 734c 6973 7451 7565 7279 2e5f  aluesListQuery._
-00004430: 6578 6563 7574 6529 0672 4e00 0000 7255  execute).rN...rU
-00004440: 0000 0072 5600 0000 7215 0000 0072 5200  ...rV...r....rR.
-00004450: 0000 72aa 0000 0072 1300 0000 7213 0000  ..r....r....r...
-00004460: 0029 0172 6a00 0000 7214 0000 0072 8400  .).rj...r....r..
-00004470: 0000 3802 0000 7304 0000 0008 010c 2372  ..8...s.......#r
-00004480: 8400 0000 6300 0000 0000 0000 0000 0000  ....c...........
-00004490: 0003 0000 0000 0000 0073 2400 0000 6500  .........s$...e.
-000044a0: 5a01 6400 5a02 8700 6601 6401 6402 8408  Z.d.Z...f.d.d...
-000044b0: 5a03 6403 6404 8400 5a04 8700 0400 5a05  Z.d.d...Z.....Z.
-000044c0: 5300 2905 7287 0000 0063 0d00 0000 0000  S.).r....c......
-000044d0: 0000 1100 0000 0800 0000 0300 0000 73ea  ..............s.
-000044e0: 0000 0074 0083 006a 0183 0001 007c 017c  ...t...j.....|.|
-000044f0: 005f 0274 037c 016a 046a 0583 017d 0d7c  ._.t.|.j.j...}.|
-00004500: 0372 247c 036e 067c 016a 046a 067c 005f  .r$|.n.|.j.j.|._
-00004510: 077c 006a 076a 086a 097c 0d83 017c 005f  .|.j.j.j.|...|._
-00004520: 0a78 207c 056a 0b83 0044 005d 145c 027d  .x |.j...D.].\.}
-00004530: 0e7d 0f7c 006a 0c7c 0f7c 0e83 0201 0071  .}.|.j.|.|.....q
-00004540: 4857 007c 006a 0d7c 017c 027c 047c 0a7c  HW.|.j.|.|.|.|.|
-00004550: 0b7c 0c64 018d 0601 007c 0672 887c 006a  .|.d.....|.r.|.j
-00004560: 0a6a 0e7c 0683 017c 005f 0a7c 0772 9a7c  .j.|...|._.|.r.|
-00004570: 006a 0a6a 0f7c 0783 017c 005f 0a7c 0872  .j.j.|...|._.|.r
-00004580: aa7c 006a 0a6a 1083 007c 005f 0a78 267c  .|.j.j...|._.x&|
-00004590: 0944 005d 1e7d 107c 006a 0a6a 117c 1064  .D.].}.|.j.j.|.d
-000045a0: 0219 007c 1064 0319 0064 048d 027c 005f  ...|.d...d...|._
-000045b0: 0a71 b057 007c 006a 127c 017c 097c 0a83  .q.W.|.j.|.|.|..
-000045c0: 0301 007c 057c 005f 1364 0053 0029 054e  ...|.|._.d.S.).N
-000045d0: 2906 7211 0000 0072 2f00 0000 7230 0000  ).r....r/...r0..
-000045e0: 0072 3100 0000 722e 0000 0072 3200 0000  .r1...r....r2...
-000045f0: 7201 0000 0072 2400 0000 2901 7248 0000  r....r$...).rH..
-00004600: 0029 1472 5800 0000 7215 0000 0072 1100  .).rX...r....r..
-00004610: 0000 7205 0000 0072 2600 0000 7216 0000  ..r....r&...r...
-00004620: 0072 8200 0000 7260 0000 0072 a000 0000  .r....r`...r....
-00004630: 725b 0000 0072 1000 0000 7229 0000 0072  r[...r....r)...r
-00004640: b700 0000 7239 0000 0072 7a00 0000 727b  ....r9...rz...r{
-00004650: 0000 0072 7c00 0000 724d 0000 0072 4c00  ...r|...rM...rL.
-00004660: 0000 7286 0000 0029 1172 1200 0000 7211  ..r....).r....r.
-00004670: 0000 0072 2f00 0000 7282 0000 0072 3000  ...r/...r....r0.
-00004680: 0000 7286 0000 0072 7a00 0000 727b 0000  ..r....rz...r{..
-00004690: 0072 7c00 0000 724f 0000 0072 3100 0000  .r|...rO...r1...
-000046a0: 722e 0000 0072 3200 0000 7216 0000 005a  r....r2...r....Z
-000046b0: 0a72 6574 7572 6e73 5f61 7372 1a00 0000  .returns_asr....
-000046c0: 7250 0000 0029 0172 6a00 0000 7213 0000  rP...).rj...r...
-000046d0: 0072 1400 0000 7215 0000 0069 0200 0073  .r....r....i...s
-000046e0: 3000 0000 0004 0a01 0601 0c01 1201 1001  0...............
-000046f0: 1201 1002 0401 0201 0201 0201 0201 0201  ................
-00004700: 0802 0401 0e01 0401 0e01 0401 0c01 0a01  ................
-00004710: 1e01 0e01 7a14 5661 6c75 6573 5175 6572  ....z.ValuesQuer
-00004720: 792e 5f5f 696e 6974 5f5f 6301 0000 0000  y.__init__c.....
-00004730: 0000 0002 0000 0003 0000 0083 0000 0073  ...............s
-00004740: 3e00 0000 8801 6a00 6a01 7402 8801 6a03  >.....j.j.t...j.
-00004750: 8301 8301 4900 6400 4800 7d01 8701 6601  ....I.d.H.}...f.
-00004760: 6401 6402 8408 8801 6a04 4400 8301 8900  d.d.....j.D.....
-00004770: 8700 6601 6403 6402 8408 7c01 4400 8301  ..f.d.d...|.D...
-00004780: 5300 2904 4e63 0100 0000 0000 0000 0200  S.).Nc..........
-00004790: 0000 0600 0000 1300 0000 731e 0000 0067  ..........s....g
-000047a0: 007c 005d 167d 017c 0188 006a 0088 006a  .|.].}.|...j...j
-000047b0: 017c 0183 0266 0291 0271 0453 0072 1300  .|...f...q.S.r..
-000047c0: 0000 2902 72bb 0000 0072 1100 0000 2902  ..).r....r....).
-000047d0: 72bc 0000 0072 c100 0000 2901 7212 0000  r....r....).r...
-000047e0: 0072 1300 0000 7214 0000 0072 c200 0000  .r....r....r....
-000047f0: 8b02 0000 7302 0000 0006 017a 2856 616c  ....s......z(Val
-00004800: 7565 7351 7565 7279 2e5f 6578 6563 7574  uesQuery._execut
-00004810: 652e 3c6c 6f63 616c 733e 2e3c 6c69 7374  e.<locals>.<list
-00004820: 636f 6d70 3e63 0100 0000 0000 0000 0100  comp>c..........
-00004830: 0000 0500 0000 1300 0000 731e 0000 0067  ..........s....g
-00004840: 007c 005d 1689 0087 0066 0164 0064 0184  .|.].....f.d.d..
-00004850: 0888 0144 0083 0191 0271 0453 0029 0263  ...D.....q.S.).c
-00004860: 0100 0000 0000 0000 0300 0000 0500 0000  ................
-00004870: 1300 0000 731e 0000 0069 007c 005d 165c  ....s....i.|.].\
-00004880: 027d 017d 027c 0288 007c 0119 0083 017c  .}.}.|...|.....|
-00004890: 0193 0271 0453 0072 1300 0000 7213 0000  ...q.S.r....r...
-000048a0: 0029 0372 bc00 0000 7235 0000 0072 c500  .).r....r5...r..
-000048b0: 0000 2901 72c4 0000 0072 1300 0000 7214  ..).r....r....r.
-000048c0: 0000 0072 be00 0000 8e02 0000 7302 0000  ...r........s...
-000048d0: 0006 007a 3356 616c 7565 7351 7565 7279  ...z3ValuesQuery
-000048e0: 2e5f 6578 6563 7574 652e 3c6c 6f63 616c  ._execute.<local
-000048f0: 733e 2e3c 6c69 7374 636f 6d70 3e2e 3c64  s>.<listcomp>.<d
-00004900: 6963 7463 6f6d 703e 7213 0000 0029 0172  ictcomp>r....).r
-00004910: bc00 0000 2901 72c8 0000 0029 0172 c400  ....).r....).r..
-00004920: 0000 7214 0000 0072 c200 0000 8e02 0000  ..r....r........
-00004930: 7302 0000 0006 0029 0572 6000 0000 72b0  s......).r`...r.
-00004940: 0000 0072 b100 0000 7210 0000 0072 8600  ...r....r....r..
-00004950: 0000 2902 7212 0000 0072 a800 0000 7213  ..).r....r....r.
-00004960: 0000 0029 0272 c800 0000 7212 0000 0072  ...).r....r....r
-00004970: 1400 0000 7252 0000 0088 0200 0073 0800  ....rR.......s..
-00004980: 0000 0001 1802 0a01 0a02 7a14 5661 6c75  ..........z.Valu
-00004990: 6573 5175 6572 792e 5f65 7865 6375 7465  esQuery._execute
-000049a0: 2906 724e 0000 0072 5500 0000 7256 0000  ).rN...rU...rV..
-000049b0: 0072 1500 0000 7252 0000 0072 aa00 0000  .r....rR...r....
-000049c0: 7213 0000 0072 1300 0000 2901 726a 0000  r....r....).rj..
-000049d0: 0072 1400 0000 7287 0000 0068 0200 0073  .r....r....h...s
-000049e0: 0400 0000 0801 0c1f 7287 0000 004e 291d  ........r....N).
-000049f0: da06 7079 7069 6b61 7202 0000 0072 0300  ..pypikar....r..
-00004a00: 0000 7204 0000 0072 5a00 0000 7205 0000  ..r....rZ...r...
-00004a10: 005a 1070 7970 696b 612e 6675 6e63 7469  .Z.pypika.functi
-00004a20: 6f6e 7372 0600 0000 da08 746f 7274 6f69  onsr......tortoi
-00004a30: 7365 7207 0000 005a 1474 6f72 746f 6973  ser....Z.tortois
-00004a40: 652e 6167 6772 6567 6174 696f 6e72 0800  e.aggregationr..
-00004a50: 0000 da1d 746f 7274 6f69 7365 2e62 6163  ....tortoise.bac
-00004a60: 6b65 6e64 732e 6261 7365 2e63 6c69 656e  kends.base.clien
-00004a70: 7472 0900 0000 da13 746f 7274 6f69 7365  tr......tortoise
-00004a80: 2e65 7863 6570 7469 6f6e 7372 0a00 0000  .exceptionsr....
-00004a90: 5a14 746f 7274 6f69 7365 2e71 7565 7279  Z.tortoise.query
-00004aa0: 5f75 7469 6c73 720b 0000 0072 0c00 0000  _utilsr....r....
-00004ab0: da0e 746f 7274 6f69 7365 2e75 7469 6c73  ..tortoise.utils
-00004ac0: 720d 0000 0072 0e00 0000 7257 0000 0072  r....r....rW...r
-00004ad0: 8d00 0000 728a 0000 0072 8e00 0000 72b3  ....r....r....r.
-00004ae0: 0000 0072 8400 0000 7287 0000 0072 1300  ...r....r....r..
-00004af0: 0000 7213 0000 0072 1300 0000 7214 0000  ..r....r....r...
-00004b00: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
-00004b10: 2600 0000 1001 0c01 0c01 0c02 0c01 0c01  &...............
-00004b20: 0c01 0c01 1001 0c03 0e6f 107f 007f 0020  .........o..... 
-00004b30: 1022 1014 1015 1052 1030                 .".....R.0
+00002c90: 0182 017c 0c6a 1072 9074 1164 0383 0182  ...|.j.r.t.d....
+00002ca0: 0174 127c 0c74 136a 1483 0272 ae64 046a  .t.|.t.j...r.d.j
+00002cb0: 0f7c 0a83 017d 0d7c 0b6a 157d 0b6e 0c7c  .|...}.|.j.}.n.|
+00002cc0: 016a 026a 167c 0a19 007d 0d7c 006a 096a  .j.j.|...}.|.j.j
+00002cd0: 177c 0d7c 0b83 027c 005f 0971 5857 0064  .|.|...|._.qXW.d
+00002ce0: 0053 0029 054e 2906 7212 0000 0072 3000  .S.).N).r....r0.
+00002cf0: 0000 7231 0000 0072 3200 0000 722f 0000  ..r1...r2...r/..
+00002d00: 0072 3300 0000 7a28 556e 6b6e 6f77 6e20  .r3...z(Unknown 
+00002d10: 6b65 7977 6f72 6420 6172 6775 6d65 6e74  keyword argument
+00002d20: 207b 7d20 666f 7220 6d6f 6465 6c20 7b7d   {} for model {}
+00002d30: 7a2c 4669 656c 6420 7b7d 2069 7320 6765  z,Field {} is ge
+00002d40: 6e65 7261 7465 6420 616e 6420 6361 6e20  nerated and can 
+00002d50: 6e6f 7420 6265 2075 7064 6174 6564 7a05  not be updatedz.
+00002d60: 7b7d 5f69 6429 1872 5900 0000 7216 0000  {}_id).rY...r...
+00002d70: 0072 2700 0000 7283 0000 0072 6100 0000  .r'...r....ra...
+00002d80: 7205 0000 0072 1700 0000 72a1 0000 0072  r....r....r....r
+00002d90: 8000 0000 7211 0000 0072 3a00 0000 722a  ....r....r:...r*
+00002da0: 0000 0072 2d00 0000 722c 0000 0072 0a00  ...r-...r,...r..
+00002db0: 0000 7242 0000 00da 0967 656e 6572 6174  ..rB.....generat
+00002dc0: 6564 720b 0000 0072 3b00 0000 7207 0000  edr....r;...r...
+00002dd0: 00da 0f46 6f72 6569 676e 4b65 7946 6965  ...ForeignKeyFie
+00002de0: 6c64 721f 0000 00da 1466 6965 6c64 735f  ldr......fields_
+00002df0: 6462 5f70 726f 6a65 6374 696f 6e72 9500  db_projectionr..
+00002e00: 0000 290e 7213 0000 0072 1200 0000 7230  ..).r....r....r0
+00002e10: 0000 0072 8d00 0000 7283 0000 0072 3100  ...r....r....r1.
+00002e20: 0000 7232 0000 0072 2f00 0000 7233 0000  ..r2...r/...r3..
+00002e30: 0072 1700 0000 7236 0000 0072 2300 0000  .r....r6...r#...
+00002e40: 7237 0000 00da 0864 625f 6669 656c 6429  r7.....db_field)
+00002e50: 0172 6b00 0000 7214 0000 0072 1500 0000  .rk...r....r....
+00002e60: 7216 0000 009b 0100 0073 2c00 0000 0004  r........s,.....
+00002e70: 0a01 1201 0c01 1001 0401 0201 0201 0201  ................
+00002e80: 0201 0201 0803 1201 0e01 0401 1001 0601  ................
+00002e90: 0801 0c01 0a01 0802 0c01 7a14 5570 6461  ..........z.Upda
+00002ea0: 7465 5175 6572 792e 5f5f 696e 6974 5f5f  teQuery.__init__
+00002eb0: 6301 0000 0000 0000 0001 0000 0003 0000  c...............
+00002ec0: 00c3 0000 0073 1c00 0000 7c00 6a00 6a01  .....s....|.j.j.
+00002ed0: 7402 7c00 6a03 8301 8301 4900 6400 4800  t.|.j.....I.d.H.
+00002ee0: 0100 6400 5300 2901 4e29 0472 6100 0000  ..d.S.).N).ra...
+00002ef0: da0d 6578 6563 7574 655f 7175 6572 79da  ..execute_query.
+00002f00: 0373 7472 7211 0000 0029 0172 1300 0000  .strr....).r....
+00002f10: 7214 0000 0072 1400 0000 7215 0000 0072  r....r....r....r
+00002f20: 5300 0000 b901 0000 7302 0000 0000 017a  S.......s......z
+00002f30: 1455 7064 6174 6551 7565 7279 2e5f 6578  .UpdateQuery._ex
+00002f40: 6563 7574 6529 0672 4f00 0000 7256 0000  ecute).rO...rV..
+00002f50: 0072 5700 0000 7216 0000 0072 5300 0000  .rW...r....rS...
+00002f60: 72aa 0000 0072 1400 0000 7214 0000 0029  r....r....r....)
+00002f70: 0172 6b00 0000 7215 0000 0072 8e00 0000  .rk...r....r....
+00002f80: 9a01 0000 7304 0000 0008 010c 1e72 8e00  ....s........r..
+00002f90: 0000 6300 0000 0000 0000 0000 0000 0003  ..c.............
+00002fa0: 0000 0000 0000 0073 2400 0000 6500 5a01  .......s$...e.Z.
+00002fb0: 6400 5a02 8700 6601 6401 6402 8408 5a03  d.Z...f.d.d...Z.
+00002fc0: 6403 6404 8400 5a04 8700 0400 5a05 5300  d.d...Z.....Z.S.
+00002fd0: 2905 728b 0000 0063 0800 0000 0000 0000  ).r....c........
+00002fe0: 0900 0000 0800 0000 0300 0000 735e 0000  ............s^..
+00002ff0: 0074 0083 006a 0183 0001 007c 0372 127c  .t...j.....|.r.|
+00003000: 036e 067c 016a 026a 037c 005f 0474 057c  .n.|.j.j.|._.t.|
+00003010: 016a 026a 0683 017d 087c 006a 046a 076a  .j.j...}.|.j.j.j
+00003020: 087c 0883 017c 005f 097c 006a 0a7c 017c  .|...|._.|.j.|.|
+00003030: 027c 047c 057c 067c 0764 018d 0601 007c  .|.|.|.|.d.....|
+00003040: 006a 096a 0b83 007c 005f 0964 0053 0029  .j.j...|._.d.S.)
+00003050: 024e 2906 7212 0000 0072 3000 0000 7231  .N).r....r0...r1
+00003060: 0000 0072 3200 0000 722f 0000 0072 3300  ...r2...r/...r3.
+00003070: 0000 290c 7259 0000 0072 1600 0000 7227  ..).rY...r....r'
+00003080: 0000 0072 8300 0000 7261 0000 0072 0500  ...r....ra...r..
+00003090: 0000 7217 0000 0072 a100 0000 725c 0000  ..r....r....r\..
+000030a0: 0072 1100 0000 723a 0000 0072 8c00 0000  .r....r:...r....
+000030b0: 2909 7213 0000 0072 1200 0000 7230 0000  ).r....r....r0..
+000030c0: 0072 8300 0000 7231 0000 0072 3200 0000  .r....r1...r2...
+000030d0: 722f 0000 0072 3300 0000 7217 0000 0029  r/...r3...r....)
+000030e0: 0172 6b00 0000 7214 0000 0072 1500 0000  .rk...r....r....
+000030f0: 7216 0000 00be 0100 0073 1800 0000 0001  r........s......
+00003100: 0a01 1201 0c01 1001 0401 0201 0201 0201  ................
+00003110: 0201 0201 0802 7a14 4465 6c65 7465 5175  ......z.DeleteQu
+00003120: 6572 792e 5f5f 696e 6974 5f5f 6301 0000  ery.__init__c...
+00003130: 0000 0000 0001 0000 0003 0000 00c3 0000  ................
+00003140: 0073 1c00 0000 7c00 6a00 6a01 7402 7c00  .s....|.j.j.t.|.
+00003150: 6a03 8301 8301 4900 6400 4800 0100 6400  j.....I.d.H...d.
+00003160: 5300 2901 4e29 0472 6100 0000 72af 0000  S.).N).ra...r...
+00003170: 0072 b000 0000 7211 0000 0029 0172 1300  .r....r....).r..
+00003180: 0000 7214 0000 0072 1400 0000 7215 0000  ..r....r....r...
+00003190: 0072 5300 0000 cd01 0000 7302 0000 0000  .rS.......s.....
+000031a0: 017a 1444 656c 6574 6551 7565 7279 2e5f  .z.DeleteQuery._
+000031b0: 6578 6563 7574 6529 0672 4f00 0000 7256  execute).rO...rV
+000031c0: 0000 0072 5700 0000 7216 0000 0072 5300  ...rW...r....rS.
+000031d0: 0000 72aa 0000 0072 1400 0000 7214 0000  ..r....r....r...
+000031e0: 0029 0172 6b00 0000 7215 0000 0072 8b00  .).rk...r....r..
+000031f0: 0000 bd01 0000 7304 0000 0008 010c 0f72  ......s........r
+00003200: 8b00 0000 6300 0000 0000 0000 0000 0000  ....c...........
+00003210: 0003 0000 0000 0000 0073 2400 0000 6500  .........s$...e.
+00003220: 5a01 6400 5a02 8700 6601 6401 6402 8408  Z.d.Z...f.d.d...
+00003230: 5a03 6403 6404 8400 5a04 8700 0400 5a05  Z.d.d...Z.....Z.
+00003240: 5300 2905 728f 0000 0063 0800 0000 0000  S.).r....c......
+00003250: 0000 0900 0000 0800 0000 0300 0000 7366  ..............sf
+00003260: 0000 0074 0083 006a 0183 0001 007c 0372  ...t...j.....|.r
+00003270: 127c 036e 067c 016a 026a 037c 005f 0474  .|.n.|.j.j.|._.t
+00003280: 057c 016a 026a 0683 017d 087c 006a 046a  .|.j.j...}.|.j.j
+00003290: 076a 087c 0883 017c 005f 097c 006a 0a7c  .j.|...|._.|.j.|
+000032a0: 017c 027c 047c 057c 067c 0764 018d 0601  .|.|.|.|.|.d....
+000032b0: 007c 006a 096a 0b74 0c7c 086a 0d83 0183  .|.j.j.t.|.j....
+000032c0: 017c 005f 0964 0053 0029 024e 2906 7212  .|._.d.S.).N).r.
+000032d0: 0000 0072 3000 0000 7231 0000 0072 3200  ...r0...r1...r2.
+000032e0: 0000 722f 0000 0072 3300 0000 290e 7259  ..r/...r3...).rY
+000032f0: 0000 0072 1600 0000 7227 0000 0072 8300  ...r....r'...r..
+00003300: 0000 7261 0000 0072 0500 0000 7217 0000  ..ra...r....r...
+00003310: 0072 a100 0000 725c 0000 0072 1100 0000  .r....r\...r....
+00003320: 723a 0000 0072 9e00 0000 7206 0000 00da  r:...r....r.....
+00003330: 0473 7461 7229 0972 1300 0000 7212 0000  .star).r....r...
+00003340: 0072 3000 0000 7283 0000 0072 3100 0000  .r0...r....r1...
+00003350: 7232 0000 0072 2f00 0000 7233 0000 0072  r2...r/...r3...r
+00003360: 1700 0000 2901 726b 0000 0072 1400 0000  ....).rk...r....
+00003370: 7215 0000 0072 1600 0000 d201 0000 7318  r....r........s.
+00003380: 0000 0000 010a 0112 010c 0110 0104 0102  ................
+00003390: 0102 0102 0102 0102 0108 027a 1343 6f75  ...........z.Cou
+000033a0: 6e74 5175 6572 792e 5f5f 696e 6974 5f5f  ntQuery.__init__
+000033b0: 6301 0000 0000 0000 0002 0000 0004 0000  c...............
+000033c0: 00c3 0000 0073 3000 0000 7c00 6a00 6a01  .....s0...|.j.j.
+000033d0: 7402 7c00 6a03 8301 8301 4900 6400 4800  t.|.j.....I.d.H.
+000033e0: 7d01 7404 7405 7c01 6401 1900 8301 6a06  }.t.t.|.d.....j.
+000033f0: 8300 8301 6401 1900 5300 2902 4e72 0100  ....d...S.).Nr..
+00003400: 0000 2907 7261 0000 0072 af00 0000 72b0  ..).ra...r....r.
+00003410: 0000 0072 1100 0000 726d 0000 0072 6c00  ...r....rm...rl.
+00003420: 0000 728a 0000 0029 0272 1300 0000 da06  ..r....).r......
+00003430: 7265 7375 6c74 7214 0000 0072 1400 0000  resultr....r....
+00003440: 7215 0000 0072 5300 0000 e101 0000 7304  r....rS.......s.
+00003450: 0000 0000 0118 017a 1343 6f75 6e74 5175  .......z.CountQu
+00003460: 6572 792e 5f65 7865 6375 7465 2906 724f  ery._execute).rO
+00003470: 0000 0072 5600 0000 7257 0000 0072 1600  ...rV...rW...r..
+00003480: 0000 7253 0000 0072 aa00 0000 7214 0000  ..rS...r....r...
+00003490: 0072 1400 0000 2901 726b 0000 0072 1500  .r....).rk...r..
+000034a0: 0000 728f 0000 00d1 0100 0073 0400 0000  ..r........s....
+000034b0: 0801 0c0f 728f 0000 0063 0000 0000 0000  ....r....c......
+000034c0: 0000 0000 0000 0200 0000 4000 0000 7324  ..........@...s$
+000034d0: 0000 0065 005a 0164 005a 0264 0164 0284  ...e.Z.d.Z.d.d..
+000034e0: 005a 0364 0364 0484 005a 0464 0564 0684  .Z.d.d...Z.d.d..
+000034f0: 005a 0564 0753 0029 08da 1046 6965 6c64  .Z.d.S.)...Field
+00003500: 5365 6c65 6374 5175 6572 7963 0400 0000  SelectQueryc....
+00003510: 0000 0000 0800 0000 0700 0000 4300 0000  ............C...
+00003520: 73d6 0000 0074 007c 016a 016a 0283 017d  s....t.|.j.j...}
+00003530: 047c 027c 016a 016a 036b 0672 327c 030c  .|.|.j.j.k.r2|..
+00003540: 0072 327c 016a 016a 037c 0219 007d 057c  .r2|.j.j.|...}.|
+00003550: 047c 0566 0253 007c 027c 016a 016a 036b  .|.f.S.|.|.j.j.k
+00003560: 0672 547c 0372 5474 0464 016a 057c 027c  .rT|.rTt.d.j.|.|
+00003570: 016a 0683 0283 0182 017c 027c 006a 076a  .j.......|.|.j.j
+00003580: 016a 086b 0672 767c 030c 0072 7674 0964  .j.k.rv|...rvt.d
+00003590: 026a 057c 0283 0183 0182 017c 016a 016a  .j.|.......|.j.j
+000035a0: 0a6a 0b7c 0283 017d 067c 0673 9a74 0464  .j.|...}.|.s.t.d
+000035b0: 036a 057c 027c 016a 0683 0283 0182 017c  .j.|.|.j.......|
+000035c0: 006a 0c7c 047c 027c 0683 0301 007c 036a  .j.|.|.|.....|.j
+000035d0: 0d64 0483 017d 077c 006a 0e7c 066a 0f7c  .d...}.|.j.|.j.|
+000035e0: 0764 0519 0064 046a 107c 0764 0664 0085  .d...d.j.|.d.d..
+000035f0: 0219 0083 0164 078d 0353 0029 084e 7a29  .....d...S.).Nz)
+00003600: 4669 656c 6420 227b 7d22 2066 6f72 206d  Field "{}" for m
+00003610: 6f64 656c 2022 7b7d 2220 6973 206e 6f74  odel "{}" is not
+00003620: 2072 656c 6174 696f 6e7a 4f53 656c 6563   relationzOSelec
+00003630: 7469 6e67 2072 656c 6174 696f 6e20 227b  ting relation "{
+00003640: 7d22 2069 7320 6e6f 7420 706f 7373 6962  }" is not possib
+00003650: 6c65 2c20 7365 6c65 6374 2063 6f6e 6372  le, select concr
+00003660: 6574 6520 6669 656c 6420 6f6e 2072 656c  ete field on rel
+00003670: 6174 6564 206d 6f64 656c 7a21 556e 6b6e  ated modelz!Unkn
+00003680: 6f77 6e20 6669 656c 6420 227b 7d22 2066  own field "{}" f
+00003690: 6f72 206d 6f64 656c 2022 7b7d 2272 4800  or model "{}"rH.
+000036a0: 0000 7201 0000 0072 2500 0000 2903 7212  ..r....r%...).r.
+000036b0: 0000 0072 1b00 0000 da10 666f 7277 6172  ...r......forwar
+000036c0: 6465 645f 6669 656c 6473 2911 7205 0000  ded_fields).r...
+000036d0: 0072 2700 0000 7217 0000 0072 ad00 0000  .r'...r....r....
+000036e0: 720a 0000 0072 4200 0000 724f 0000 0072  r....rB...rO...r
+000036f0: 1200 0000 724a 0000 0072 4b00 0000 722d  ....rJ...rK...r-
+00003700: 0000 0072 2c00 0000 7247 0000 0072 4c00  ...r,...rG...rL.
+00003710: 0000 da21 5f6a 6f69 6e5f 7461 626c 655f  ...!_join_table_
+00003720: 7769 7468 5f66 6f72 7761 7264 6564 5f66  with_forwarded_f
+00003730: 6965 6c64 7372 3d00 0000 721c 0000 0029  ieldsr=...r....)
+00003740: 0872 1300 0000 7212 0000 0072 1b00 0000  .r....r....r....
+00003750: 72b4 0000 0072 1700 0000 72ae 0000 0072  r....r....r....r
+00003760: 3700 0000 5a16 666f 7277 6172 6465 645f  7...Z.forwarded_
+00003770: 6669 656c 6473 5f73 706c 6974 7214 0000  fields_splitr...
+00003780: 0072 1400 0000 7215 0000 0072 b500 0000  .r....r....r....
+00003790: e701 0000 7330 0000 0000 010c 0112 010c  ....s0..........
+000037a0: 0108 0110 0102 0104 0102 010a 0414 0102  ................
+000037b0: 0104 0108 030e 0104 0106 0102 010a 030e  ................
+000037c0: 010a 0104 0104 0106 017a 3246 6965 6c64  .........z2Field
+000037d0: 5365 6c65 6374 5175 6572 792e 5f6a 6f69  SelectQuery._joi
+000037e0: 6e5f 7461 626c 655f 7769 7468 5f66 6f72  n_table_with_for
+000037f0: 7761 7264 6564 5f66 6965 6c64 7363 0300  warded_fieldsc..
+00003800: 0000 0000 0000 0800 0000 0700 0000 4300  ..............C.
+00003810: 0000 73de 0000 0074 007c 006a 016a 026a  ..s....t.|.j.j.j
+00003820: 0383 017d 037c 017c 006a 016a 026a 046b  ...}.|.|.j.j.j.k
+00003830: 0672 487c 006a 016a 026a 047c 0119 007d  .rH|.j.j.j.|...}
+00003840: 047c 006a 056a 0674 077c 037c 0483 026a  .|.j.j.t.|.|...j
+00003850: 087c 0283 0183 017c 005f 0564 0053 007c  .|.....|._.d.S.|
+00003860: 017c 006a 016a 026a 096b 0672 6474 0a64  .|.j.j.j.k.rdt.d
+00003870: 016a 0b7c 0183 0183 0182 017c 016a 0c64  .j.|.......|.j.d
+00003880: 0283 017d 057c 0564 0319 007c 006a 016a  ...}.|.d...|.j.j
+00003890: 026a 096b 0672 c67c 006a 0d7c 006a 017c  .j.k.r.|.j.|.j.|
+000038a0: 0564 0319 0064 026a 0e7c 0564 0464 0085  .d...d.j.|.d.d..
+000038b0: 0219 0083 0164 058d 035c 027d 067d 077c  .....d...\.}.}.|
+000038c0: 006a 056a 0674 077c 067c 0783 026a 087c  .j.j.t.|.|...j.|
+000038d0: 0283 0183 017c 005f 0564 0053 0074 0f64  .....|._.d.S.t.d
+000038e0: 066a 0b7c 017c 006a 016a 1083 0283 0182  .j.|.|.j.j......
+000038f0: 0164 0053 0029 074e 7a4f 5365 6c65 6374  .d.S.).NzOSelect
+00003900: 696e 6720 7265 6c61 7469 6f6e 2022 7b7d  ing relation "{}
+00003910: 2220 6973 206e 6f74 2070 6f73 7369 626c  " is not possibl
+00003920: 652c 2073 656c 6563 7420 636f 6e63 7265  e, select concre
+00003930: 7465 2066 6965 6c64 206f 6e20 7265 6c61  te field on rela
+00003940: 7465 6420 6d6f 6465 6c72 4800 0000 7201  ted modelrH...r.
+00003950: 0000 0072 2500 0000 2903 7212 0000 0072  ...r%...).r....r
+00003960: 1b00 0000 72b4 0000 007a 2155 6e6b 6e6f  ....r....z!Unkno
+00003970: 776e 2066 6965 6c64 2022 7b7d 2220 666f  wn field "{}" fo
+00003980: 7220 6d6f 6465 6c20 227b 7d22 2911 7205  r model "{}").r.
+00003990: 0000 0072 1200 0000 7227 0000 0072 1700  ...r....r'...r..
+000039a0: 0000 72ad 0000 0072 1100 0000 729e 0000  ..r....r....r...
+000039b0: 0072 2000 0000 729f 0000 0072 4a00 0000  .r ...r....rJ...
+000039c0: 724b 0000 0072 4200 0000 724c 0000 0072  rK...rB...rL...r
+000039d0: b500 0000 721c 0000 0072 0a00 0000 724f  ....r....r....rO
+000039e0: 0000 0029 0872 1300 0000 721b 0000 0072  ...).r....r....r
+000039f0: 8900 0000 7217 0000 0072 ae00 0000 da0b  ....r....r......
+00003a00: 6669 656c 645f 7370 6c69 7472 4500 0000  field_splitrE...
+00003a10: 5a10 7265 6c61 7465 645f 6462 5f66 6965  Z.related_db_fie
+00003a20: 6c64 7214 0000 0072 1400 0000 7215 0000  ldr....r....r...
+00003a30: 00da 1961 6464 5f66 6965 6c64 5f74 6f5f  ...add_field_to_
+00003a40: 7365 6c65 6374 5f71 7565 7279 0902 0000  select_query....
+00003a50: 7328 0000 0000 010e 010e 010e 011a 0104  s(..............
+00003a60: 020e 0102 0104 0108 030a 0112 0104 0104  ................
+00003a70: 0106 011a 021a 0104 0206 0102 017a 2a46  .............z*F
+00003a80: 6965 6c64 5365 6c65 6374 5175 6572 792e  ieldSelectQuery.
+00003a90: 6164 645f 6669 656c 645f 746f 5f73 656c  add_field_to_sel
+00003aa0: 6563 745f 7175 6572 7963 0300 0000 0000  ect_queryc......
+00003ab0: 0000 0500 0000 0600 0000 4300 0000 7388  ..........C...s.
+00003ac0: 0000 007c 027c 016a 006a 016b 0672 1464  ...|.|.j.j.k.r.d
+00003ad0: 0164 0284 0053 007c 027c 016a 006a 026b  .d...S.|.|.j.j.k
+00003ae0: 0672 2e7c 016a 006a 027c 0219 006a 0353  .r.|.j.j.|...j.S
+00003af0: 007c 026a 0464 0383 017d 037c 0364 0419  .|.j.d...}.|.d..
+00003b00: 007c 016a 006a 016b 0672 747c 016a 006a  .|.j.j.k.rt|.j.j
+00003b10: 027c 0364 0419 0019 006a 057d 047c 006a  .|.d.....j.}.|.j
+00003b20: 067c 0464 036a 077c 0364 0564 0085 0219  .|.d.j.|.d.d....
+00003b30: 0083 0183 0253 0074 0864 066a 097c 027c  .....S.t.d.j.|.|
+00003b40: 0183 0283 0182 0164 0053 0029 074e 6301  .......d.S.).Nc.
+00003b50: 0000 0000 0000 0001 0000 0001 0000 0053  ...............S
+00003b60: 0000 0073 0400 0000 7c00 5300 2901 4e72  ...s....|.S.).Nr
+00003b70: 1400 0000 2901 da01 7872 1400 0000 7214  ....)...xr....r.
+00003b80: 0000 0072 1500 0000 da08 3c6c 616d 6264  ...r......<lambd
+00003b90: 613e 2802 0000 7300 0000 007a 3a46 6965  a>(...s....z:Fie
+00003ba0: 6c64 5365 6c65 6374 5175 6572 792e 7265  ldSelectQuery.re
+00003bb0: 736f 6c76 655f 746f 5f70 7974 686f 6e5f  solve_to_python_
+00003bc0: 7661 6c75 652e 3c6c 6f63 616c 733e 2e3c  value.<locals>.<
+00003bd0: 6c61 6d62 6461 3e72 4800 0000 7201 0000  lambda>rH...r...
+00003be0: 0072 2500 0000 7a21 556e 6b6e 6f77 6e20  .r%...z!Unknown 
+00003bf0: 6669 656c 6420 227b 7d22 2066 6f72 206d  field "{}" for m
+00003c00: 6f64 656c 2022 7b7d 2229 0a72 2700 0000  odel "{}").r'...
+00003c10: 724a 0000 0072 2d00 0000 da0f 746f 5f70  rJ...r-.....to_p
+00003c20: 7974 686f 6e5f 7661 6c75 6572 4c00 0000  ython_valuerL...
+00003c30: 723d 0000 00da 1772 6573 6f6c 7665 5f74  r=.....resolve_t
+00003c40: 6f5f 7079 7468 6f6e 5f76 616c 7565 721c  o_python_valuer.
+00003c50: 0000 0072 0a00 0000 7242 0000 0029 0572  ...r....rB...).r
+00003c60: 1300 0000 7212 0000 0072 1b00 0000 72b6  ....r....r....r.
+00003c70: 0000 005a 096e 6577 5f6d 6f64 656c 7214  ...Z.new_modelr.
+00003c80: 0000 0072 1400 0000 7215 0000 0072 bb00  ...r....r....r..
+00003c90: 0000 2502 0000 7316 0000 0000 010c 0208  ..%...s.........
+00003ca0: 020c 010e 020a 0110 0112 011a 0206 0102  ................
+00003cb0: 017a 2846 6965 6c64 5365 6c65 6374 5175  .z(FieldSelectQu
+00003cc0: 6572 792e 7265 736f 6c76 655f 746f 5f70  ery.resolve_to_p
+00003cd0: 7974 686f 6e5f 7661 6c75 654e 2906 724f  ython_valueN).rO
+00003ce0: 0000 0072 5600 0000 7257 0000 0072 b500  ...rV...rW...r..
+00003cf0: 0000 72b7 0000 0072 bb00 0000 7214 0000  ..r....r....r...
+00003d00: 0072 1400 0000 7214 0000 0072 1500 0000  .r....r....r....
+00003d10: 72b3 0000 00e6 0100 0073 0600 0000 0801  r........s......
+00003d20: 0822 081c 72b3 0000 0063 0000 0000 0000  ."..r....c......
+00003d30: 0000 0000 0000 0300 0000 0000 0000 7324  ..............s$
+00003d40: 0000 0065 005a 0164 005a 0287 0066 0164  ...e.Z.d.Z...f.d
+00003d50: 0164 0284 085a 0364 0364 0484 005a 0487  .d...Z.d.d...Z..
+00003d60: 0004 005a 0553 0029 0572 8500 0000 630e  ...Z.S.).r....c.
+00003d70: 0000 0000 0000 0012 0000 0008 0000 0003  ................
+00003d80: 0000 0073 f200 0000 7400 8300 6a01 8300  ...s....t...j...
+00003d90: 0100 7c0a 7222 7402 7c05 8301 6401 6b03  ..|.r"t.|...d.k.
+00003da0: 7222 7403 6402 8301 8201 7c01 7c00 5f04  r"t.d.....|.|._.
+00003db0: 7405 7c01 6a06 6a07 8301 7d0e 7c03 723c  t.|.j.j...}.|.r<
+00003dc0: 7c03 6e06 7c01 6a06 6a08 7c00 5f09 7c00  |.n.|.j.j.|._.|.
+00003dd0: 6a09 6a0a 6a0b 7c0e 8301 7c00 5f0c 6403  j.j.j.|...|._.d.
+00003de0: 6404 8400 740d 7c05 8301 4400 8301 7d0f  d...t.|...D...}.
+00003df0: 7820 7c0f 6a0e 8300 4400 5d14 5c02 7d10  x |.j...D.].\.}.
+00003e00: 7d11 7c00 6a0f 7c11 7c10 8302 0100 7172  }.|.j.|.|.....qr
+00003e10: 5700 7c00 6a10 7c01 7c02 7c04 7c0b 7c0c  W.|.j.|.|.|.|.|.
+00003e20: 7c0d 6405 8d06 0100 7c06 72b2 7c00 6a0c  |.d.....|.r.|.j.
+00003e30: 6a11 7c06 8301 7c00 5f0c 7c07 72c4 7c00  j.|...|._.|.r.|.
+00003e40: 6a0c 6a12 7c07 8301 7c00 5f0c 7c08 72d4  j.j.|...|._.|.r.
+00003e50: 7c00 6a0c 6a13 8300 7c00 5f0c 7c00 6a14  |.j.j...|._.|.j.
+00003e60: 7c01 7c09 7c0b 8303 0100 7c0a 7c00 5f15  |.|.|.....|.|._.
+00003e70: 7c0f 7c00 5f16 6400 5300 2906 4e72 2500  |.|._.d.S.).Nr%.
+00003e80: 0000 7a32 596f 7520 6361 6e20 666c 6174  ..z2You can flat
+00003e90: 2076 616c 7565 5f6c 6973 7420 6f6e 6c79   value_list only
+00003ea0: 2069 6620 636f 6e74 6169 6e73 206f 6e65   if contains one
+00003eb0: 2066 6965 6c64 6301 0000 0000 0000 0003   fieldc.........
+00003ec0: 0000 0005 0000 0053 0000 0073 1a00 0000  .......S...s....
+00003ed0: 6900 7c00 5d12 5c02 7d01 7d02 7c02 7400  i.|.].\.}.}.|.t.
+00003ee0: 7c01 8301 9302 7104 5300 7214 0000 0029  |.....q.S.r....)
+00003ef0: 0172 b000 0000 2903 da02 2e30 da01 6972  .r....)....0..ir
+00003f00: 1b00 0000 7214 0000 0072 1400 0000 7215  ....r....r....r.
+00003f10: 0000 00fa 0a3c 6469 6374 636f 6d70 3e45  .....<dictcomp>E
+00003f20: 0200 0073 0200 0000 0600 7a2c 5661 6c75  ...s......z,Valu
+00003f30: 6573 4c69 7374 5175 6572 792e 5f5f 696e  esListQuery.__in
+00003f40: 6974 5f5f 2e3c 6c6f 6361 6c73 3e2e 3c64  it__.<locals>.<d
+00003f50: 6963 7463 6f6d 703e 2906 7212 0000 0072  ictcomp>).r....r
+00003f60: 3000 0000 7231 0000 0072 3200 0000 722f  0...r1...r2...r/
+00003f70: 0000 0072 3300 0000 2917 7259 0000 0072  ...r3...).rY...r
+00003f80: 1600 0000 da03 6c65 6e72 7000 0000 7212  ......lenrp...r.
+00003f90: 0000 0072 0500 0000 7227 0000 0072 1700  ...r....r'...r..
+00003fa0: 0000 7283 0000 0072 6100 0000 72a1 0000  ..r....ra...r...
+00003fb0: 0072 5c00 0000 7211 0000 00da 0965 6e75  .r\...r......enu
+00003fc0: 6d65 7261 7465 722a 0000 0072 b700 0000  merater*...r....
+00003fd0: 723a 0000 0072 7b00 0000 727c 0000 0072  r:...r{...r|...r
+00003fe0: 7d00 0000 724d 0000 0072 8200 0000 7207  }...rM...r....r.
+00003ff0: 0000 0029 1272 1300 0000 7212 0000 0072  ...).r....r....r
+00004000: 3000 0000 7283 0000 0072 3100 0000 7284  0...r....r1...r.
+00004010: 0000 0072 7b00 0000 727c 0000 0072 7d00  ...r{...r|...r}.
+00004020: 0000 7250 0000 0072 8200 0000 7232 0000  ..rP...r....r2..
+00004030: 0072 2f00 0000 7233 0000 0072 1700 0000  .r/...r3...r....
+00004040: 7287 0000 005a 1170 6f73 6974 696f 6e61  r....Z.positiona
+00004050: 6c5f 6e75 6d62 6572 721b 0000 0029 0172  l_numberr....).r
+00004060: 6b00 0000 7214 0000 0072 1500 0000 7216  k...r....r....r.
+00004070: 0000 0039 0200 0073 3400 0000 0004 0a01  ...9...s4.......
+00004080: 1001 0802 0601 0c01 1201 1001 1202 1201  ................
+00004090: 1002 0401 0201 0201 0201 0201 0201 0802  ................
+000040a0: 0401 0e01 0401 0e01 0401 0c01 0e01 0601  ................
+000040b0: 7a18 5661 6c75 6573 4c69 7374 5175 6572  z.ValuesListQuer
+000040c0: 792e 5f5f 696e 6974 5f5f 6301 0000 0000  y.__init__c.....
+000040d0: 0000 0002 0000 0004 0000 0083 0000 0073  ...............s
+000040e0: 6e00 0000 8802 6a00 6a01 7402 8802 6a03  n.....j.j.t...j.
+000040f0: 8301 8301 4900 6400 4800 7d01 8702 6601  ....I.d.H.}...f.
+00004100: 6401 6402 8408 7404 7405 8802 6a06 6a07  d.d...t.t...j.j.
+00004110: 8300 8301 8301 4400 8301 8900 8802 6a08  ......D.......j.
+00004120: 725c 8800 6403 1900 6404 1900 8901 8701  r\..d...d.......
+00004130: 6601 6405 6402 8408 7c01 4400 8301 5300  f.d.d...|.D...S.
+00004140: 8700 6601 6406 6402 8408 7c01 4400 8301  ..f.d.d...|.D...
+00004150: 5300 2907 4e63 0100 0000 0000 0000 0300  S.).Nc..........
+00004160: 0000 0600 0000 1300 0000 7322 0000 0067  ..........s"...g
+00004170: 007c 005d 1a5c 027d 017d 027c 0188 006a  .|.].\.}.}.|...j
+00004180: 0088 006a 017c 0283 0266 0291 0271 0453  ...j.|...f...q.S
+00004190: 0072 1400 0000 2902 72bb 0000 0072 1200  .r....).r....r..
+000041a0: 0000 2903 72bc 0000 0072 3600 0000 da04  ..).r....r6.....
+000041b0: 6e61 6d65 2901 7213 0000 0072 1400 0000  name).r....r....
+000041c0: 7215 0000 00fa 0a3c 6c69 7374 636f 6d70  r......<listcomp
+000041d0: 3e5f 0200 0073 0200 0000 0601 7a2c 5661  >_...s......z,Va
+000041e0: 6c75 6573 4c69 7374 5175 6572 792e 5f65  luesListQuery._e
+000041f0: 7865 6375 7465 2e3c 6c6f 6361 6c73 3e2e  xecute.<locals>.
+00004200: 3c6c 6973 7463 6f6d 703e 7201 0000 0072  <listcomp>r....r
+00004210: 2500 0000 6301 0000 0000 0000 0002 0000  %...c...........
+00004220: 0005 0000 0013 0000 0073 1800 0000 6700  .........s....g.
+00004230: 7c00 5d10 7d01 8800 7c01 6400 1900 8301  |.].}...|.d.....
+00004240: 9102 7104 5300 2901 da01 3072 1400 0000  ..q.S.)...0r....
+00004250: 2902 72bc 0000 00da 0565 6e74 7279 2901  ).r......entry).
+00004260: da04 6675 6e63 7214 0000 0072 1500 0000  ..funcr....r....
+00004270: 72c2 0000 0064 0200 0073 0200 0000 0600  r....d...s......
+00004280: 6301 0000 0000 0000 0001 0000 0005 0000  c...............
+00004290: 0013 0000 0073 1e00 0000 6700 7c00 5d16  .....s....g.|.].
+000042a0: 8900 8700 6601 6400 6401 8408 8801 4400  ....f.d.d.....D.
+000042b0: 8301 9102 7104 5300 2902 6301 0000 0000  ....q.S.).c.....
+000042c0: 0000 0003 0000 0004 0000 0033 0000 0073  ...........3...s
+000042d0: 1e00 0000 7c00 5d16 5c02 7d01 7d02 7c02  ....|.].\.}.}.|.
+000042e0: 8800 7c01 1900 8301 5600 0100 7102 6400  ..|.....V...q.d.
+000042f0: 5300 2901 4e72 1400 0000 2903 72bc 0000  S.).Nr....).r...
+00004300: 00da 0663 6f6c 756d 6e72 c500 0000 2901  ...columnr....).
+00004310: 72c4 0000 0072 1400 0000 7215 0000 00fa  r....r....r.....
+00004320: 093c 6765 6e65 7870 723e 6502 0000 7302  .<genexpr>e...s.
+00004330: 0000 0004 007a 3656 616c 7565 734c 6973  .....z6ValuesLis
+00004340: 7451 7565 7279 2e5f 6578 6563 7574 652e  tQuery._execute.
+00004350: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
+00004360: 6d70 3e2e 3c67 656e 6578 7072 3e72 1400  mp>.<genexpr>r..
+00004370: 0000 2901 72bc 0000 0029 01da 0763 6f6c  ..).r....)...col
+00004380: 756d 6e73 2901 72c4 0000 0072 1500 0000  umns).r....r....
+00004390: 72c2 0000 0065 0200 0073 0200 0000 0600  r....e...s......
+000043a0: 2909 7261 0000 0072 af00 0000 72b0 0000  ).ra...r....r...
+000043b0: 0072 1100 0000 da06 736f 7274 6564 726d  .r......sortedrm
+000043c0: 0000 0072 0700 0000 722a 0000 0072 8200  ...r....r*...r..
+000043d0: 0000 2902 7213 0000 0072 b200 0000 7214  ..).r....r....r.
+000043e0: 0000 0029 0372 c800 0000 72c5 0000 0072  ...).r....r....r
+000043f0: 1300 0000 7215 0000 0072 5300 0000 5c02  ....r....rS...\.
+00004400: 0000 730e 0000 0000 0118 020a 0116 0206  ..s.............
+00004410: 010c 0112 017a 1856 616c 7565 734c 6973  .....z.ValuesLis
+00004420: 7451 7565 7279 2e5f 6578 6563 7574 6529  tQuery._execute)
+00004430: 0672 4f00 0000 7256 0000 0072 5700 0000  .rO...rV...rW...
+00004440: 7216 0000 0072 5300 0000 72aa 0000 0072  r....rS...r....r
+00004450: 1400 0000 7214 0000 0029 0172 6b00 0000  ....r....).rk...
+00004460: 7215 0000 0072 8500 0000 3802 0000 7304  r....r....8...s.
+00004470: 0000 0008 010c 2372 8500 0000 6300 0000  ......#r....c...
+00004480: 0000 0000 0000 0000 0003 0000 0000 0000  ................
+00004490: 0073 2400 0000 6500 5a01 6400 5a02 8700  .s$...e.Z.d.Z...
+000044a0: 6601 6401 6402 8408 5a03 6403 6404 8400  f.d.d...Z.d.d...
+000044b0: 5a04 8700 0400 5a05 5300 2905 7288 0000  Z.....Z.S.).r...
+000044c0: 0063 0d00 0000 0000 0000 1100 0000 0800  .c..............
+000044d0: 0000 0300 0000 73ea 0000 0074 0083 006a  ......s....t...j
+000044e0: 0183 0001 007c 017c 005f 0274 037c 016a  .....|.|._.t.|.j
+000044f0: 046a 0583 017d 0d7c 0372 247c 036e 067c  .j...}.|.r$|.n.|
+00004500: 016a 046a 067c 005f 077c 006a 076a 086a  .j.j.|._.|.j.j.j
+00004510: 097c 0d83 017c 005f 0a78 207c 056a 0b83  .|...|._.x |.j..
+00004520: 0044 005d 145c 027d 0e7d 0f7c 006a 0c7c  .D.].\.}.}.|.j.|
+00004530: 0f7c 0e83 0201 0071 4857 007c 006a 0d7c  .|.....qHW.|.j.|
+00004540: 017c 027c 047c 0a7c 0b7c 0c64 018d 0601  .|.|.|.|.|.d....
+00004550: 007c 0672 887c 006a 0a6a 0e7c 0683 017c  .|.r.|.j.j.|...|
+00004560: 005f 0a7c 0772 9a7c 006a 0a6a 0f7c 0783  ._.|.r.|.j.j.|..
+00004570: 017c 005f 0a7c 0872 aa7c 006a 0a6a 1083  .|._.|.r.|.j.j..
+00004580: 007c 005f 0a78 267c 0944 005d 1e7d 107c  .|._.x&|.D.].}.|
+00004590: 006a 0a6a 117c 1064 0219 007c 1064 0319  .j.j.|.d...|.d..
+000045a0: 0064 048d 027c 005f 0a71 b057 007c 006a  .d...|._.q.W.|.j
+000045b0: 127c 017c 097c 0a83 0301 007c 057c 005f  .|.|.|.....|.|._
+000045c0: 1364 0053 0029 054e 2906 7212 0000 0072  .d.S.).N).r....r
+000045d0: 3000 0000 7231 0000 0072 3200 0000 722f  0...r1...r2...r/
+000045e0: 0000 0072 3300 0000 7201 0000 0072 2500  ...r3...r....r%.
+000045f0: 0000 2901 7249 0000 0029 1472 5900 0000  ..).rI...).rY...
+00004600: 7216 0000 0072 1200 0000 7205 0000 0072  r....r....r....r
+00004610: 2700 0000 7217 0000 0072 8300 0000 7261  '...r....r....ra
+00004620: 0000 0072 a100 0000 725c 0000 0072 1100  ...r....r\...r..
+00004630: 0000 722a 0000 0072 b700 0000 723a 0000  ..r*...r....r:..
+00004640: 0072 7b00 0000 727c 0000 0072 7d00 0000  .r{...r|...r}...
+00004650: 724e 0000 0072 4d00 0000 7287 0000 0029  rN...rM...r....)
+00004660: 1172 1300 0000 7212 0000 0072 3000 0000  .r....r....r0...
+00004670: 7283 0000 0072 3100 0000 7287 0000 0072  r....r1...r....r
+00004680: 7b00 0000 727c 0000 0072 7d00 0000 7250  {...r|...r}...rP
+00004690: 0000 0072 3200 0000 722f 0000 0072 3300  ...r2...r/...r3.
+000046a0: 0000 7217 0000 005a 0a72 6574 7572 6e73  ..r....Z.returns
+000046b0: 5f61 7372 1b00 0000 7251 0000 0029 0172  _asr....rQ...).r
+000046c0: 6b00 0000 7214 0000 0072 1500 0000 7216  k...r....r....r.
+000046d0: 0000 0069 0200 0073 3000 0000 0004 0a01  ...i...s0.......
+000046e0: 0601 0c01 1201 1001 1201 1002 0401 0201  ................
+000046f0: 0201 0201 0201 0201 0802 0401 0e01 0401  ................
+00004700: 0e01 0401 0c01 0a01 1e01 0e01 7a14 5661  ............z.Va
+00004710: 6c75 6573 5175 6572 792e 5f5f 696e 6974  luesQuery.__init
+00004720: 5f5f 6301 0000 0000 0000 0002 0000 0003  __c.............
+00004730: 0000 0083 0000 0073 3e00 0000 8801 6a00  .......s>.....j.
+00004740: 6a01 7402 8801 6a03 8301 8301 4900 6400  j.t...j.....I.d.
+00004750: 4800 7d01 8701 6601 6401 6402 8408 8801  H.}...f.d.d.....
+00004760: 6a04 4400 8301 8900 8700 6601 6403 6402  j.D.......f.d.d.
+00004770: 8408 7c01 4400 8301 5300 2904 4e63 0100  ..|.D...S.).Nc..
+00004780: 0000 0000 0000 0200 0000 0600 0000 1300  ................
+00004790: 0000 731e 0000 0067 007c 005d 167d 017c  ..s....g.|.].}.|
+000047a0: 0188 006a 0088 006a 017c 0183 0266 0291  ...j...j.|...f..
+000047b0: 0271 0453 0072 1400 0000 2902 72bb 0000  .q.S.r....).r...
+000047c0: 0072 1200 0000 2902 72bc 0000 0072 c100  .r....).r....r..
+000047d0: 0000 2901 7213 0000 0072 1400 0000 7215  ..).r....r....r.
+000047e0: 0000 0072 c200 0000 8b02 0000 7302 0000  ...r........s...
+000047f0: 0006 017a 2856 616c 7565 7351 7565 7279  ...z(ValuesQuery
+00004800: 2e5f 6578 6563 7574 652e 3c6c 6f63 616c  ._execute.<local
+00004810: 733e 2e3c 6c69 7374 636f 6d70 3e63 0100  s>.<listcomp>c..
+00004820: 0000 0000 0000 0100 0000 0500 0000 1300  ................
+00004830: 0000 731e 0000 0067 007c 005d 1689 0087  ..s....g.|.]....
+00004840: 0066 0164 0064 0184 0888 0144 0083 0191  .f.d.d.....D....
+00004850: 0271 0453 0029 0263 0100 0000 0000 0000  .q.S.).c........
+00004860: 0300 0000 0500 0000 1300 0000 731e 0000  ............s...
+00004870: 0069 007c 005d 165c 027d 017d 027c 0288  .i.|.].\.}.}.|..
+00004880: 007c 0119 0083 017c 0193 0271 0453 0072  .|.....|...q.S.r
+00004890: 1400 0000 7214 0000 0029 0372 bc00 0000  ....r....).r....
+000048a0: 7236 0000 0072 c500 0000 2901 72c4 0000  r6...r....).r...
+000048b0: 0072 1400 0000 7215 0000 0072 be00 0000  .r....r....r....
+000048c0: 8e02 0000 7302 0000 0006 007a 3356 616c  ....s......z3Val
+000048d0: 7565 7351 7565 7279 2e5f 6578 6563 7574  uesQuery._execut
+000048e0: 652e 3c6c 6f63 616c 733e 2e3c 6c69 7374  e.<locals>.<list
+000048f0: 636f 6d70 3e2e 3c64 6963 7463 6f6d 703e  comp>.<dictcomp>
+00004900: 7214 0000 0029 0172 bc00 0000 2901 72c8  r....).r....).r.
+00004910: 0000 0029 0172 c400 0000 7215 0000 0072  ...).r....r....r
+00004920: c200 0000 8e02 0000 7302 0000 0006 0029  ........s......)
+00004930: 0572 6100 0000 72af 0000 0072 b000 0000  .ra...r....r....
+00004940: 7211 0000 0072 8700 0000 2902 7213 0000  r....r....).r...
+00004950: 0072 b200 0000 7214 0000 0029 0272 c800  .r....r....).r..
+00004960: 0000 7213 0000 0072 1500 0000 7253 0000  ..r....r....rS..
+00004970: 0088 0200 0073 0800 0000 0001 1802 0a01  .....s..........
+00004980: 0a02 7a14 5661 6c75 6573 5175 6572 792e  ..z.ValuesQuery.
+00004990: 5f65 7865 6375 7465 2906 724f 0000 0072  _execute).rO...r
+000049a0: 5600 0000 7257 0000 0072 1600 0000 7253  V...rW...r....rS
+000049b0: 0000 0072 aa00 0000 7214 0000 0072 1400  ...r....r....r..
+000049c0: 0000 2901 726b 0000 0072 1500 0000 7288  ..).rk...r....r.
+000049d0: 0000 0068 0200 0073 0400 0000 0801 0c1f  ...h...s........
+000049e0: 7288 0000 004e 291e da06 7079 7069 6b61  r....N)...pypika
+000049f0: 7202 0000 0072 0300 0000 7204 0000 0072  r....r....r....r
+00004a00: 5b00 0000 7205 0000 005a 1070 7970 696b  [...r....Z.pypik
+00004a10: 612e 6675 6e63 7469 6f6e 7372 0600 0000  a.functionsr....
+00004a20: da08 746f 7274 6f69 7365 7207 0000 005a  ..tortoiser....Z
+00004a30: 1474 6f72 746f 6973 652e 6167 6772 6567  .tortoise.aggreg
+00004a40: 6174 696f 6e72 0800 0000 da1d 746f 7274  ationr......tort
+00004a50: 6f69 7365 2e62 6163 6b65 6e64 732e 6261  oise.backends.ba
+00004a60: 7365 2e63 6c69 656e 7472 0900 0000 da13  se.clientr......
+00004a70: 746f 7274 6f69 7365 2e65 7863 6570 7469  tortoise.excepti
+00004a80: 6f6e 7372 0a00 0000 720b 0000 005a 1474  onsr....r....Z.t
+00004a90: 6f72 746f 6973 652e 7175 6572 795f 7574  ortoise.query_ut
+00004aa0: 696c 7372 0c00 0000 720d 0000 00da 0e74  ilsr....r......t
+00004ab0: 6f72 746f 6973 652e 7574 696c 7372 0e00  ortoise.utilsr..
+00004ac0: 0000 720f 0000 0072 5800 0000 728e 0000  ..r....rX...r...
+00004ad0: 0072 8b00 0000 728f 0000 0072 b300 0000  .r....r....r....
+00004ae0: 7285 0000 0072 8800 0000 7214 0000 0072  r....r....r....r
+00004af0: 1400 0000 7214 0000 0072 1500 0000 da08  ....r....r......
+00004b00: 3c6d 6f64 756c 653e 0100 0000 7326 0000  <module>....s&..
+00004b10: 0010 010c 010c 010c 020c 010c 010c 0110  ................
+00004b20: 0110 010c 030e 6f10 7f00 7f00 1f10 2310  ......o.......#.
+00004b30: 1410 1510 5210 30                        ....R.0
```

### Comparing `tortoise-orm-0.9.2/tortoise/__pycache__/models.cpython-36.pyc` & `tortoise-orm-0.9.4/tortoise/__pycache__/models.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.6 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 20% similar despite different names*

```diff
@@ -1,662 +1,675 @@
-00000000: 330d 0d0a 5576 3f5b 0338 0000 e300 0000  3...Uv?[.8......
+00000000: 330d 0d0a 549b 4b5b 8238 0000 e300 0000  3...T.K[.8......
 00000010: 0000 0000 0000 0000 0005 0000 0040 0000  .............@..
-00000020: 0073 fc00 0000 6400 6401 6c00 5a00 6400  .s....d.d.l.Z.d.
+00000020: 0073 1801 0000 6400 6401 6c00 5a00 6400  .s....d.d.l.Z.d.
 00000030: 6402 6c01 6d02 5a02 6d03 5a03 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6403 6c04 6d05 5a05 0100 6400 6404 6c06  d.l.m.Z...d.d.l.
 00000050: 6d07 5a07 0100 6400 6405 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
-00000060: 6d0a 5a0a 0100 6400 6406 6c0b 6d0c 5a0c  m.Z...d.d.l.m.Z.
-00000070: 0100 6407 6408 8400 5a0d 6409 640a 8400  ..d.d...Z.d.d...
-00000080: 5a0e 640b 640c 8400 5a0f 640d 640e 8400  Z.d.d...Z.d.d...
-00000090: 5a10 640f 6410 8400 5a11 6411 6412 8400  Z.d.d...Z.d.d...
-000000a0: 5a12 6413 6414 8400 5a13 6415 6416 8400  Z.d.d...Z.d.d...
-000000b0: 5a14 6417 6418 8400 5a15 6419 641a 8400  Z.d.d...Z.d.d...
-000000c0: 5a16 641b 641c 8400 5a17 641d 641e 8400  Z.d.d...Z.d.d...
-000000d0: 5a18 641f 6420 8400 5a19 651a 6507 6a1b  Z.d.d ..Z.e.e.j.
-000000e0: 651a 6421 9c03 6422 6423 8404 5a1c 4700  e.d!..d"d#..Z.G.
-000000f0: 6424 6425 8400 6425 8302 5a1d 4700 6426  d$d%..d%..Z.G.d&
-00000100: 6427 8400 6427 651e 8303 5a1f 4700 6428  d'..d'e...Z.G.d(
-00000110: 6429 8400 6429 651f 642a 8d03 5a20 6401  d)..d)e.d*..Z d.
-00000120: 5300 292b e900 0000 004e 2902 da05 5461  S.)+.....N)...Ta
-00000130: 626c 65da 0966 756e 6374 696f 6e73 2901  ble..functions).
-00000140: da08 5371 6c54 7970 6573 2901 da06 6669  ..SqlTypes)...fi
-00000150: 656c 6473 2902 da19 4d61 6e79 546f 4d61  elds)...ManyToMa
-00000160: 6e79 5265 6c61 7469 6f6e 4d61 6e61 6765  nyRelationManage
-00000170: 72da 1652 656c 6174 696f 6e51 7565 7279  r..RelationQuery
-00000180: 436f 6e74 6169 6e65 7229 01da 0851 7565  Container)...Que
-00000190: 7279 5365 7463 0200 0000 0000 0000 0200  rySetc..........
-000001a0: 0000 0200 0000 4300 0000 730a 0000 007c  ......C...s....|
-000001b0: 006a 007c 0183 0153 0029 014e 2901 da04  .j.|...S.).N)...
-000001c0: 6973 696e 2902 da05 6669 656c 64da 0576  isin)...field..v
-000001d0: 616c 7565 a900 720c 0000 00fa 432f 5573  alue..r.....C/Us
-000001e0: 6572 732f 616e 6472 6579 626f 6e64 6172  ers/andreybondar
-000001f0: 2f50 7943 6861 726d 5072 6f6a 6563 7473  /PyCharmProjects
-00000200: 2f74 6f72 746f 6973 652d 6f72 6d2f 746f  /tortoise-orm/to
-00000210: 7274 6f69 7365 2f6d 6f64 656c 732e 7079  rtoise/models.py
-00000220: da05 6973 5f69 6e0b 0000 0073 0200 0000  ..is_in....s....
-00000230: 0001 720e 0000 0063 0200 0000 0000 0000  ..r....c........
-00000240: 0200 0000 0200 0000 4300 0000 7312 0000  ........C...s...
-00000250: 007c 006a 007c 0183 017c 006a 0183 0042  .|.j.|...|.j...B
-00000260: 0053 0029 014e 2902 da05 6e6f 7469 6eda  .S.).N)...notin.
-00000270: 0669 736e 756c 6c29 0272 0a00 0000 720b  .isnull).r....r.
-00000280: 0000 0072 0c00 0000 720c 0000 0072 0d00  ...r....r....r..
-00000290: 0000 da06 6e6f 745f 696e 0f00 0000 7302  ....not_in....s.
-000002a0: 0000 0000 0172 1100 0000 6302 0000 0000  .....r....c.....
-000002b0: 0000 0002 0000 0002 0000 0043 0000 0073  ...........C...s
-000002c0: 1200 0000 7c00 6a00 7c01 8301 7c00 6a01  ....|.j.|...|.j.
-000002d0: 8300 4200 5300 2901 4e29 02da 026e 6572  ..B.S.).N)...ner
-000002e0: 1000 0000 2902 720a 0000 0072 0b00 0000  ....).r....r....
-000002f0: 720c 0000 0072 0c00 0000 720d 0000 00da  r....r....r.....
-00000300: 096e 6f74 5f65 7175 616c 1300 0000 7302  .not_equal....s.
-00000310: 0000 0000 0172 1300 0000 6302 0000 0000  .....r....c.....
-00000320: 0000 0002 0000 0001 0000 0043 0000 0073  ...........C...s
-00000330: 1800 0000 7c01 720c 7c00 6a00 8300 5300  ....|.r.|.j...S.
-00000340: 7c00 6a01 8300 5300 6400 5300 2901 4e29  |.j...S.d.S.).N)
-00000350: 0272 1000 0000 da07 6e6f 746e 756c 6c29  .r......notnull)
-00000360: 0272 0a00 0000 720b 0000 0072 0c00 0000  .r....r....r....
-00000370: 720c 0000 0072 0d00 0000 da07 6973 5f6e  r....r......is_n
-00000380: 756c 6c17 0000 0073 0600 0000 0001 0401  ull....s........
-00000390: 0802 7215 0000 0063 0200 0000 0000 0000  ..r....c........
-000003a0: 0200 0000 0100 0000 4300 0000 7318 0000  ........C...s...
-000003b0: 007c 0172 0c7c 006a 0083 0053 007c 006a  .|.r.|.j...S.|.j
-000003c0: 0183 0053 0064 0053 0029 014e 2902 7214  ...S.d.S.).N).r.
-000003d0: 0000 0072 1000 0000 2902 720a 0000 0072  ...r....).r....r
-000003e0: 0b00 0000 720c 0000 0072 0c00 0000 720d  ....r....r....r.
-000003f0: 0000 00da 086e 6f74 5f6e 756c 6c1e 0000  .....not_null...
-00000400: 0073 0600 0000 0001 0401 0802 7216 0000  .s..........r...
-00000410: 0063 0200 0000 0000 0000 0200 0000 0300  .c..............
-00000420: 0000 4300 0000 731a 0000 0074 006a 017c  ..C...s....t.j.|
-00000430: 0074 026a 0383 026a 0464 016a 057c 0183  .t.j...j.d.j.|..
-00000440: 0183 0153 0029 024e 7a04 257b 7d25 2906  ...S.).Nz.%{}%).
-00000450: 7203 0000 00da 0443 6173 7472 0400 0000  r......Castr....
-00000460: da07 5641 5243 4841 52da 046c 696b 65da  ..VARCHAR..like.
-00000470: 0666 6f72 6d61 7429 0272 0a00 0000 720b  .format).r....r.
-00000480: 0000 0072 0c00 0000 720c 0000 0072 0d00  ...r....r....r..
-00000490: 0000 da08 636f 6e74 6169 6e73 2500 0000  ....contains%...
-000004a0: 7302 0000 0000 0172 1b00 0000 6302 0000  s......r....c...
-000004b0: 0000 0000 0002 0000 0003 0000 0043 0000  .............C..
-000004c0: 0073 1a00 0000 7400 6a01 7c00 7402 6a03  .s....t.j.|.t.j.
-000004d0: 8302 6a04 6401 6a05 7c01 8301 8301 5300  ..j.d.j.|.....S.
-000004e0: 2902 4e7a 037b 7d25 2906 7203 0000 0072  ).Nz.{}%).r....r
-000004f0: 1700 0000 7204 0000 0072 1800 0000 7219  ....r....r....r.
-00000500: 0000 0072 1a00 0000 2902 720a 0000 0072  ...r....).r....r
-00000510: 0b00 0000 720c 0000 0072 0c00 0000 720d  ....r....r....r.
-00000520: 0000 00da 0b73 7461 7274 735f 7769 7468  .....starts_with
-00000530: 2900 0000 7302 0000 0000 0172 1c00 0000  )...s......r....
-00000540: 6302 0000 0000 0000 0002 0000 0003 0000  c...............
-00000550: 0043 0000 0073 1a00 0000 7400 6a01 7c00  .C...s....t.j.|.
-00000560: 7402 6a03 8302 6a04 6401 6a05 7c01 8301  t.j...j.d.j.|...
-00000570: 8301 5300 2902 4e7a 0325 7b7d 2906 7203  ..S.).Nz.%{}).r.
-00000580: 0000 0072 1700 0000 7204 0000 0072 1800  ...r....r....r..
-00000590: 0000 7219 0000 0072 1a00 0000 2902 720a  ..r....r....).r.
-000005a0: 0000 0072 0b00 0000 720c 0000 0072 0c00  ...r....r....r..
-000005b0: 0000 720d 0000 00da 0965 6e64 735f 7769  ..r......ends_wi
-000005c0: 7468 2d00 0000 7302 0000 0000 0172 1d00  th-...s......r..
-000005d0: 0000 6302 0000 0000 0000 0002 0000 0004  ..c.............
-000005e0: 0000 0043 0000 0073 2600 0000 7400 6a01  ...C...s&...t.j.
-000005f0: 7400 6a02 7c00 7403 6a04 8302 8301 6a05  t.j.|.t.j.....j.
-00000600: 7400 6a01 6401 6a06 7c01 8301 8301 8301  t.j.d.j.|.......
-00000610: 5300 2902 4e7a 0425 7b7d 2529 0772 0300  S.).Nz.%{}%).r..
-00000620: 0000 da05 5570 7065 7272 1700 0000 7204  ....Upperr....r.
-00000630: 0000 0072 1800 0000 7219 0000 0072 1a00  ...r....r....r..
-00000640: 0000 2902 720a 0000 0072 0b00 0000 720c  ..).r....r....r.
-00000650: 0000 0072 0c00 0000 720d 0000 00da 1469  ...r....r......i
-00000660: 6e73 656e 7369 7469 7665 5f63 6f6e 7461  nsensitive_conta
-00000670: 696e 7331 0000 0073 0400 0000 0001 1401  ins1...s........
-00000680: 721f 0000 0063 0200 0000 0000 0000 0200  r....c..........
-00000690: 0000 0400 0000 4300 0000 7326 0000 0074  ......C...s&...t
-000006a0: 006a 0174 006a 027c 0074 036a 0483 0283  .j.t.j.|.t.j....
-000006b0: 016a 0574 006a 0164 016a 067c 0183 0183  .j.t.j.d.j.|....
-000006c0: 0183 0153 0029 024e 7a03 7b7d 2529 0772  ...S.).Nz.{}%).r
-000006d0: 0300 0000 721e 0000 0072 1700 0000 7204  ....r....r....r.
-000006e0: 0000 0072 1800 0000 7219 0000 0072 1a00  ...r....r....r..
-000006f0: 0000 2902 720a 0000 0072 0b00 0000 720c  ..).r....r....r.
-00000700: 0000 0072 0c00 0000 720d 0000 00da 1769  ...r....r......i
-00000710: 6e73 656e 7369 7469 7665 5f73 7461 7274  nsensitive_start
-00000720: 735f 7769 7468 3700 0000 7304 0000 0000  s_with7...s.....
-00000730: 0114 0172 2000 0000 6302 0000 0000 0000  ...r ...c.......
-00000740: 0002 0000 0004 0000 0043 0000 0073 2600  .........C...s&.
-00000750: 0000 7400 6a01 7400 6a02 7c00 7403 6a04  ..t.j.t.j.|.t.j.
-00000760: 8302 8301 6a05 7400 6a01 6401 6a06 7c01  ....j.t.j.d.j.|.
-00000770: 8301 8301 8301 5300 2902 4e7a 0325 7b7d  ......S.).Nz.%{}
-00000780: 2907 7203 0000 0072 1e00 0000 7217 0000  ).r....r....r...
-00000790: 0072 0400 0000 7218 0000 0072 1900 0000  .r....r....r....
-000007a0: 721a 0000 0029 0272 0a00 0000 720b 0000  r....).r....r...
-000007b0: 0072 0c00 0000 720c 0000 0072 0d00 0000  .r....r....r....
-000007c0: da15 696e 7365 6e73 6974 6976 655f 656e  ..insensitive_en
-000007d0: 6473 5f77 6974 683d 0000 0073 0400 0000  ds_with=...s....
-000007e0: 0001 1401 7221 0000 0063 0200 0000 0000  ....r!...c......
-000007f0: 0000 0300 0000 0d00 0000 4300 0000 7380  ..........C...s.
-00000800: 0000 007c 007c 016a 007c 016a 0174 026a  ...|.|.j.|.j.t.j
-00000810: 0374 047c 016a 0583 0164 019c 0464 026a  .t.|.j...d...d.j
-00000820: 067c 0083 017c 016a 007c 016a 0174 0774  .|...|.j.|.j.t.t
-00000830: 047c 016a 0583 0164 019c 0464 036a 067c  .|.j...d...d.j.|
-00000840: 0083 017c 016a 007c 016a 0174 0874 047c  ...|.j.|.j.t.t.|
-00000850: 016a 0583 0174 0964 049c 0564 056a 067c  .j...t.d...d.j.|
-00000860: 0083 017c 016a 007c 016a 0174 0a74 047c  ...|.j.|.j.t.t.|
-00000870: 016a 0583 0174 0964 049c 0569 047d 027c  .j...t.d...i.}.|
-00000880: 0253 0029 064e 2904 720a 0000 00da 0c62  .S.).N).r......b
-00000890: 6163 6b77 6172 645f 6b65 79da 086f 7065  ackward_key..ope
-000008a0: 7261 746f 72da 0574 6162 6c65 7a07 7b7d  rator..tablez.{}
-000008b0: 5f5f 6e6f 747a 067b 7d5f 5f69 6e29 0572  __notz.{}__in).r
-000008c0: 0a00 0000 7222 0000 0072 2300 0000 7224  ....r"...r#...r$
-000008d0: 0000 00da 0d76 616c 7565 5f65 6e63 6f64  .....value_encod
-000008e0: 6572 7a0a 7b7d 5f5f 6e6f 745f 696e 290b  erz.{}__not_in).
-000008f0: da0b 666f 7277 6172 645f 6b65 7972 2200  ..forward_keyr".
-00000900: 0000 7223 0000 00da 0265 7172 0200 0000  ..r#.....eqr....
-00000910: da07 7468 726f 7567 6872 1a00 0000 7213  ..throughr....r.
-00000920: 0000 0072 0e00 0000 da04 6c69 7374 7211  ...r......listr.
-00000930: 0000 0029 03da 0a66 6965 6c64 5f6e 616d  ...)...field_nam
-00000940: 6572 0a00 0000 da07 6669 6c74 6572 7372  er......filtersr
-00000950: 0c00 0000 720c 0000 0072 0d00 0000 da0f  ....r....r......
-00000960: 6765 745f 6d32 6d5f 6669 6c74 6572 7343  get_m2m_filtersC
-00000970: 0000 0073 2e00 0000 0002 0201 0401 0401  ...s............
-00000980: 0401 0c02 0801 0401 0401 0201 0c02 0801  ................
-00000990: 0401 0401 0201 0801 0602 0801 0401 0401  ................
-000009a0: 0201 0801 0a03 722c 0000 0063 0200 0000  ......r,...c....
-000009b0: 0000 0000 0300 0000 0d00 0000 4300 0000  ............C...
-000009c0: 7388 0000 007c 0064 017c 016a 0074 016a  s....|.d.|.j.t.j
-000009d0: 0274 037c 016a 046a 056a 0683 0164 029c  .t.|.j.j.j...d..
-000009e0: 0464 036a 077c 0083 0164 017c 016a 0074  .d.j.|...d.|.j.t
-000009f0: 0874 037c 016a 046a 056a 0683 0164 029c  .t.|.j.j.j...d..
-00000a00: 0464 046a 077c 0083 0164 017c 016a 0074  .d.j.|...d.|.j.t
-00000a10: 0974 037c 016a 046a 056a 0683 0174 0a64  .t.|.j.j.j...t.d
-00000a20: 059c 0564 066a 077c 0083 0164 017c 016a  ...d.j.|...d.|.j
-00000a30: 0074 0b74 037c 016a 046a 056a 0683 0174  .t.t.|.j.j.j...t
-00000a40: 0a64 059c 0569 047d 027c 0253 0029 074e  .d...i.}.|.S.).N
-00000a50: da02 6964 2904 720a 0000 0072 2200 0000  ..id).r....r"...
-00000a60: 7223 0000 0072 2400 0000 7a07 7b7d 5f5f  r#...r$...z.{}__
-00000a70: 6e6f 747a 067b 7d5f 5f69 6e29 0572 0a00  notz.{}__in).r..
-00000a80: 0000 7222 0000 0072 2300 0000 7224 0000  ..r"...r#...r$..
-00000a90: 0072 2500 0000 7a0a 7b7d 5f5f 6e6f 745f  .r%...z.{}__not_
-00000aa0: 696e 290c da0e 7265 6c61 7469 6f6e 5f66  in)...relation_f
-00000ab0: 6965 6c64 7223 0000 0072 2700 0000 7202  ieldr#...r'...r.
-00000ac0: 0000 00da 0474 7970 65da 055f 6d65 7461  .....type.._meta
-00000ad0: 7224 0000 0072 1a00 0000 7213 0000 0072  r$...r....r....r
-00000ae0: 0e00 0000 7229 0000 0072 1100 0000 2903  ....r)...r....).
-00000af0: 722a 0000 0072 0a00 0000 722b 0000 0072  r*...r....r+...r
-00000b00: 0c00 0000 720c 0000 0072 0d00 0000 da17  ....r....r......
-00000b10: 6765 745f 6261 636b 7761 7264 5f66 6b5f  get_backward_fk_
-00000b20: 6669 6c74 6572 7363 0000 0073 2e00 0000  filtersc...s....
-00000b30: 0002 0201 0201 0401 0401 1002 0801 0201  ................
-00000b40: 0401 0201 1002 0801 0201 0401 0201 0c01  ................
-00000b50: 0602 0801 0201 0401 0201 0c01 0a03 7231  ..............r1
-00000b60: 0000 0029 0372 2a00 0000 720a 0000 00da  ...).r*...r.....
-00000b70: 0c73 6f75 7263 655f 6669 656c 6463 0300  .source_fieldc..
-00000b80: 0000 0000 0000 0400 0000 2200 0000 4300  .........."...C.
-00000b90: 0000 7326 0100 0074 007c 0174 016a 0283  ..s&...t.|.t.j..
-00000ba0: 0272 1674 037c 007c 0183 0253 007c 007c  .r.t.|.|...S.|.|
-00000bb0: 0274 046a 0564 019c 0264 026a 067c 0083  .t.j.d...d.j.|..
-00000bc0: 017c 0274 0764 019c 0264 036a 067c 0083  .|.t.d...d.j.|..
-00000bd0: 017c 0274 0874 0964 049c 0364 056a 067c  .|.t.t.d...d.j.|
-00000be0: 0083 017c 0274 0a74 0964 049c 0364 066a  ...|.t.t.d...d.j
-00000bf0: 067c 0083 017c 0274 0b64 019c 0264 076a  .|...|.t.d...d.j
-00000c00: 067c 0083 017c 0274 0c64 019c 0264 086a  .|...|.t.d...d.j
-00000c10: 067c 0083 017c 0274 046a 0d64 019c 0264  .|...|.t.j.d...d
-00000c20: 096a 067c 0083 017c 0274 046a 0e64 019c  .j.|...|.t.j.d..
-00000c30: 0264 0a6a 067c 0083 017c 0274 046a 0f64  .d.j.|...|.t.j.d
-00000c40: 019c 0264 0b6a 067c 0083 017c 0274 046a  ...d.j.|...|.t.j
-00000c50: 1064 019c 0264 0c6a 067c 0083 017c 0274  .d...d.j.|...|.t
-00000c60: 1164 019c 0264 0d6a 067c 0083 017c 0274  .d...d.j.|...|.t
-00000c70: 1264 019c 0264 0e6a 067c 0083 017c 0274  .d...d.j.|...|.t
-00000c80: 1364 019c 0264 0f6a 067c 0083 017c 0274  .d...d.j.|...|.t
-00000c90: 1464 019c 0264 106a 067c 0083 017c 0274  .d...d.j.|...|.t
-00000ca0: 1564 019c 0264 116a 067c 0083 017c 0274  .d...d.j.|...|.t
-00000cb0: 1664 019c 0269 107d 037c 0353 0029 124e  .d...i.}.|.S.).N
-00000cc0: 2902 720a 0000 0072 2300 0000 7a07 7b7d  ).r....r#...z.{}
-00000cd0: 5f5f 6e6f 747a 067b 7d5f 5f69 6e29 0372  __notz.{}__in).r
-00000ce0: 0a00 0000 7223 0000 0072 2500 0000 7a0a  ....r#...r%...z.
-00000cf0: 7b7d 5f5f 6e6f 745f 696e 7a0a 7b7d 5f5f  {}__not_inz.{}__
-00000d00: 6973 6e75 6c6c 7a0e 7b7d 5f5f 6e6f 745f  isnullz.{}__not_
-00000d10: 6973 6e75 6c6c 7a07 7b7d 5f5f 6774 657a  isnullz.{}__gtez
-00000d20: 077b 7d5f 5f6c 7465 7a06 7b7d 5f5f 6774  .{}__ltez.{}__gt
-00000d30: 7a06 7b7d 5f5f 6c74 7a0c 7b7d 5f5f 636f  z.{}__ltz.{}__co
-00000d40: 6e74 6169 6e73 7a0e 7b7d 5f5f 7374 6172  ntainsz.{}__star
-00000d50: 7473 7769 7468 7a0c 7b7d 5f5f 656e 6473  tswithz.{}__ends
-00000d60: 7769 7468 7a0d 7b7d 5f5f 6963 6f6e 7461  withz.{}__iconta
-00000d70: 696e 737a 0f7b 7d5f 5f69 7374 6172 7473  insz.{}__istarts
-00000d80: 7769 7468 7a0d 7b7d 5f5f 6965 6e64 7377  withz.{}__iendsw
-00000d90: 6974 6829 17da 0a69 7369 6e73 7461 6e63  ith)...isinstanc
-00000da0: 6572 0500 0000 da0f 4d61 6e79 546f 4d61  er......ManyToMa
-00000db0: 6e79 4669 656c 6472 2c00 0000 7223 0000  nyFieldr,...r#..
-00000dc0: 0072 2700 0000 721a 0000 0072 1300 0000  .r'...r....r....
-00000dd0: 720e 0000 0072 2900 0000 7211 0000 0072  r....r)...r....r
-00000de0: 1500 0000 7216 0000 00da 0267 65da 026c  ....r......ge..l
-00000df0: 65da 0267 74da 026c 7472 1b00 0000 721c  e..gt..ltr....r.
-00000e00: 0000 0072 1d00 0000 721f 0000 0072 2000  ...r....r....r .
-00000e10: 0000 7221 0000 0029 0472 2a00 0000 720a  ..r!...).r*...r.
-00000e20: 0000 0072 3200 0000 722b 0000 0072 0c00  ...r2...r+...r..
-00000e30: 0000 720c 0000 0072 0d00 0000 da15 6765  ..r....r......ge
-00000e40: 745f 6669 6c74 6572 735f 666f 725f 6669  t_filters_for_fi
-00000e50: 656c 6483 0000 0073 6a00 0000 0001 0c01  eld....sj.......
-00000e60: 0a02 0201 0201 0802 0801 0201 0602 0801  ................
-00000e70: 0201 0201 0602 0801 0201 0201 0602 0801  ................
-00000e80: 0201 0602 0801 0201 0602 0801 0201 0802  ................
-00000e90: 0801 0201 0802 0801 0201 0802 0801 0201  ................
-00000ea0: 0802 0801 0201 0602 0801 0201 0602 0801  ................
-00000eb0: 0201 0602 0801 0201 0602 0801 0201 0602  ................
-00000ec0: 0801 0201 0a03 7239 0000 0063 0000 0000  ......r9...c....
-00000ed0: 0000 0000 0000 0000 0200 0000 4000 0000  ............@...
-00000ee0: 7314 0000 0065 005a 0164 005a 0264 0164  s....e.Z.d.Z.d.d
-00000ef0: 0284 005a 0364 0353 0029 04da 084d 6574  ...Z.d.S.)...Met
-00000f00: 6149 6e66 6f63 0200 0000 0000 0000 0200  aInfoc..........
-00000f10: 0000 0400 0000 4300 0000 737c 0000 0074  ......C...s|...t
-00000f20: 007c 0164 0164 0283 037c 005f 0174 007c  .|.d.d...|._.t.|
-00000f30: 0164 0364 0083 037c 005f 0274 007c 0164  .d.d...|._.t.|.d
-00000f40: 0464 0583 037c 005f 0374 0483 007c 005f  .d...|._.t...|._
-00000f50: 0574 0483 007c 005f 0674 0483 007c 005f  .t...|._.t...|._
-00000f60: 0774 0483 007c 005f 0874 0483 007c 005f  .t...|._.t...|._
-00000f70: 0974 0483 007c 005f 0a69 007c 005f 0b69  .t...|._.i.|._.i
-00000f80: 007c 005f 0c69 007c 005f 0d69 007c 005f  .|._.i.|._.i.|._
-00000f90: 0e64 007c 005f 0f64 0053 0029 064e da08  .d.|._.d.S.).N..
-00000fa0: 6162 7374 7261 6374 4672 2400 0000 da03  abstractFr$.....
-00000fb0: 6170 705a 066d 6f64 656c 7329 10da 0767  appZ.models)...g
-00000fc0: 6574 6174 7472 723b 0000 0072 2400 0000  etattrr;...r$...
-00000fd0: 723c 0000 00da 0373 6574 7205 0000 00da  r<.....setr.....
-00000fe0: 0964 625f 6669 656c 6473 da0a 6d32 6d5f  .db_fields..m2m_
-00000ff0: 6669 656c 6473 da09 666b 5f66 6965 6c64  fields..fk_field
-00001000: 73da 1262 6163 6b77 6172 645f 666b 5f66  s..backward_fk_f
-00001010: 6965 6c64 73da 0c66 6574 6368 5f66 6965  ields..fetch_fie
-00001020: 6c64 73da 1466 6965 6c64 735f 6462 5f70  lds..fields_db_p
-00001030: 726f 6a65 6374 696f 6eda 1c66 6965 6c64  rojection..field
-00001040: 735f 6462 5f70 726f 6a65 6374 696f 6e5f  s_db_projection_
-00001050: 7265 7665 7273 6572 2b00 0000 da0a 6669  reverser+.....fi
-00001060: 656c 6473 5f6d 6170 da02 6462 2902 da04  elds_map..db)...
-00001070: 7365 6c66 da04 6d65 7461 720c 0000 0072  self..metar....r
-00001080: 0c00 0000 720d 0000 00da 085f 5f69 6e69  ....r......__ini
-00001090: 745f 5fce 0000 0073 1c00 0000 0001 0e01  t__....s........
-000010a0: 0e01 0e01 0801 0801 0801 0801 0801 0801  ................
-000010b0: 0601 0601 0601 0601 7a11 4d65 7461 496e  ........z.MetaIn
-000010c0: 666f 2e5f 5f69 6e69 745f 5f4e 2904 da08  fo.__init__N)...
-000010d0: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
-000010e0: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
-000010f0: 5f5f 724a 0000 0072 0c00 0000 720c 0000  __rJ...r....r...
-00001100: 0072 0c00 0000 720d 0000 0072 3a00 0000  .r....r....r:...
-00001110: cd00 0000 7302 0000 0008 0172 3a00 0000  ....s......r:...
-00001120: 6300 0000 0000 0000 0000 0000 0003 0000  c...............
-00001130: 0000 0000 0073 1c00 0000 6500 5a01 6400  .....s....e.Z.d.
-00001140: 5a02 8700 6601 6401 6402 8408 5a03 8700  Z...f.d.d...Z...
-00001150: 0400 5a04 5300 2903 da09 4d6f 6465 6c4d  ..Z.S.)...ModelM
-00001160: 6574 6163 0400 0000 0000 0000 1100 0000  etac............
-00001170: 0700 0000 0f00 0000 73c8 0100 0069 007d  ........s....i.}
-00001180: 0669 007d 0769 007d 0874 0083 007d 0974  .i.}.i.}.t...}.t
-00001190: 0083 007d 0a74 017c 036a 0264 0183 0183  ...}.t.|.j.d....
-000011a0: 017d 0b78 d07c 036a 0383 0044 005d c45c  .}.x.|.j...D.].\
-000011b0: 027d 0c7d 0d74 047c 0d74 056a 0683 0272  .}.}.t.|.t.j...r
-000011c0: 307c 0d7c 077c 0c3c 0074 047c 0d74 056a  0|.|.|.<.t.|.t.j
-000011d0: 0783 0272 ac64 026a 087c 0c83 017d 0e7c  ...r.d.j.|...}.|
-000011e0: 0e7c 0d5f 097c 0e7c 067c 0e3c 0074 056a  .|._.|.|.|.<.t.j
-000011f0: 0a7c 0d7c 0d6a 0b7c 0d6a 0c64 038d 037c  .|.|.j.|.j.d...|
-00001200: 077c 0e3c 007c 086a 0d74 0e7c 0e7c 077c  .|.<.|.j.t.|.|.|
-00001210: 0e19 007c 0e64 048d 0383 0101 007c 096a  ...|.d.......|.j
-00001220: 0f7c 0c83 0101 0071 3074 047c 0d74 056a  .|.....q0t.|.t.j
-00001230: 1083 0272 c47c 0a6a 0f7c 0c83 0101 0071  ...r.|.j.|.....q
-00001240: 307c 0d6a 0972 d07c 0d6a 096e 027c 0c7c  0|.j.r.|.j.n.|.|
-00001250: 067c 0c3c 007c 086a 0d74 0e7c 0c7c 077c  .|.<.|.j.t.|.|.|
-00001260: 0c19 007c 067c 0c19 0064 048d 0383 0101  ...|.|...d......
-00001270: 0071 3057 0074 1183 006a 127c 007c 017c  .q0W.t...j.|.|.|
-00001280: 027c 0383 047d 0f7c 0b7c 0f5f 137c 077c  .|...}.|.|._.|.|
-00001290: 0f6a 135f 147c 067c 0f6a 135f 1564 0564  .j._.|.|.j._.d.d
-000012a0: 0684 007c 066a 0383 0044 0083 017c 0f6a  ...|.j...D...|.j
-000012b0: 135f 1674 007c 076a 1783 0083 017c 0f6a  ._.t.|.j.....|.j
-000012c0: 135f 0574 007c 066a 1883 0083 017c 0f6a  ._.t.|.j.....|.j
-000012d0: 135f 197c 087c 0f6a 135f 1a7c 097c 0f6a  ._.|.|.j._.|.|.j
-000012e0: 135f 1b74 0083 007c 0f6a 135f 1c7c 0a7c  ._.t...|.j._.|.|
-000012f0: 0f6a 135f 1d7c 097c 0a42 007c 0f6a 135f  .j._.|.|.B.|.j._
-00001300: 1e64 007c 0f6a 135f 1f7c 0790 0173 9a64  .d.|.j._.|...s.d
-00001310: 077c 0f6a 135f 207c 0f6a 136a 2090 0173  .|.j._ |.j.j ..s
-00001320: c464 0864 096c 216d 227d 1001 007c 106a  .d.d.l!m"}...|.j
-00001330: 237c 0f6a 136a 247c 0f6a 257c 0f83 0301  #|.j.j$|.j%|....
-00001340: 007c 0f53 0029 0a4e da04 4d65 7461 7a05  .|.S.).N..Metaz.
-00001350: 7b7d 5f69 6429 03da 0972 6566 6572 656e  {}_id)...referen
-00001360: 6365 da04 6e75 6c6c da07 6465 6661 756c  ce..null..defaul
-00001370: 7429 0372 2a00 0000 720a 0000 0072 3200  t).r*...r....r2.
-00001380: 0000 6301 0000 0000 0000 0003 0000 0004  ..c.............
-00001390: 0000 0053 0000 0073 1600 0000 6900 7c00  ...S...s....i.|.
-000013a0: 5d0e 5c02 7d01 7d02 7c01 7c02 9302 7104  ].\.}.}.|.|...q.
-000013b0: 5300 720c 0000 0072 0c00 0000 2903 da02  S.r....r....)...
-000013c0: 2e30 da03 6b65 7972 0b00 0000 720c 0000  .0..keyr....r...
-000013d0: 0072 0c00 0000 720d 0000 00fa 0a3c 6469  .r....r......<di
-000013e0: 6374 636f 6d70 3e0c 0100 0073 0200 0000  ctcomp>....s....
-000013f0: 0602 7a25 4d6f 6465 6c4d 6574 612e 5f5f  ..z%ModelMeta.__
-00001400: 6e65 775f 5f2e 3c6c 6f63 616c 733e 2e3c  new__.<locals>.<
-00001410: 6469 6374 636f 6d70 3e54 7201 0000 0029  dictcomp>Tr....)
-00001420: 01da 0854 6f72 746f 6973 6529 2672 3e00  ...Tortoise)&r>.
-00001430: 0000 723a 0000 00da 0367 6574 da05 6974  ..r:.....get..it
-00001440: 656d 7372 3300 0000 7205 0000 00da 0546  emsr3...r......F
-00001450: 6965 6c64 da0f 466f 7265 6967 6e4b 6579  ield..ForeignKey
-00001460: 4669 656c 6472 1a00 0000 7232 0000 00da  Fieldr....r2....
-00001470: 0849 6e74 4669 656c 6472 5100 0000 7252  .IntFieldrQ...rR
-00001480: 0000 00da 0675 7064 6174 6572 3900 0000  .....updater9...
-00001490: da03 6164 6472 3400 0000 da05 7375 7065  ..addr4.....supe
-000014a0: 72da 075f 5f6e 6577 5f5f 7230 0000 0072  r..__new__r0...r
-000014b0: 4600 0000 7244 0000 0072 4500 0000 da04  F...rD...rE.....
-000014c0: 6b65 7973 da06 7661 6c75 6573 723f 0000  keys..valuesr?..
-000014d0: 0072 2b00 0000 7241 0000 0072 4200 0000  .r+...rA...rB...
-000014e0: 7240 0000 0072 4300 0000 7247 0000 0072  r@...rC...rG...r
-000014f0: 3b00 0000 da08 746f 7274 6f69 7365 7256  ;.....tortoiserV
-00001500: 0000 00da 0e72 6567 6973 7465 725f 6d6f  .....register_mo
-00001510: 6465 6c72 3c00 0000 724b 0000 0029 115a  delr<...rK...).Z
-00001520: 036d 6373 da04 6e61 6d65 da05 6261 7365  .mcs..name..base
-00001530: 73da 0561 7474 7273 da04 6172 6773 da06  s..attrs..args..
-00001540: 6b77 6172 6773 7244 0000 0072 4600 0000  kwargsrD...rF...
-00001550: 722b 0000 0072 4100 0000 7240 0000 0072  r+...rA...r@...r
-00001560: 4900 0000 7254 0000 0072 0b00 0000 5a09  I...rT...r....Z.
-00001570: 6b65 795f 6669 656c 64da 096e 6577 5f63  key_field..new_c
-00001580: 6c61 7373 7256 0000 0029 01da 095f 5f63  lassrV...)...__c
-00001590: 6c61 7373 5f5f 720c 0000 0072 0d00 0000  lass__r....r....
-000015a0: 725f 0000 00e0 0000 0073 6600 0000 0001  r_.......sf.....
-000015b0: 0401 0401 0401 0601 0601 0e02 1201 0c01  ................
-000015c0: 0801 0c01 0a01 0601 0801 0401 0201 0401  ................
-000015d0: 0e02 0401 0201 0201 0601 0a03 0c01 0c01  ................
-000015e0: 0c02 1401 0401 0201 0201 0601 1203 1202  ................
-000015f0: 0601 0801 0801 0602 1002 1001 1001 0801  ................
-00001600: 0801 0a01 0801 0c01 0801 0601 0801 0a01  ................
-00001610: 0c01 1401 7a11 4d6f 6465 6c4d 6574 612e  ....z.ModelMeta.
-00001620: 5f5f 6e65 775f 5f29 0572 4b00 0000 724c  __new__).rK...rL
-00001630: 0000 0072 4d00 0000 725f 0000 00da 0d5f  ...rM...r_....._
-00001640: 5f63 6c61 7373 6365 6c6c 5f5f 720c 0000  _classcell__r...
-00001650: 0072 0c00 0000 2901 726a 0000 0072 0d00  .r....).rj...r..
-00001660: 0000 724e 0000 00df 0000 0073 0200 0000  ..rN.......s....
-00001670: 0801 724e 0000 0063 0000 0000 0000 0000  ..rN...c........
-00001680: 0000 0000 0400 0000 4000 0000 73d2 0000  ........@...s...
-00001690: 0065 005a 0164 005a 0264 0164 0284 005a  .e.Z.d.Z.d.d...Z
-000016a0: 0364 2764 0464 0584 015a 0464 2864 0664  .d'd.d...Z.d(d.d
-000016b0: 0784 015a 0564 0864 0984 005a 0664 2964  ...Z.d.d...Z.d)d
-000016c0: 0a64 0b84 015a 0764 0364 0c9c 0164 0d64  .d...Z.d.d...d.d
-000016d0: 0e84 025a 0864 0f64 1084 005a 0964 1164  ...Z.d.d...Z.d.d
-000016e0: 1284 005a 0a64 1364 1484 005a 0b64 1564  ...Z.d.d...Z.d.d
-000016f0: 1684 005a 0c65 0d64 2a64 1764 1884 0183  ...Z.e.d*d.d....
-00001700: 015a 0e65 0d64 1964 1a84 0083 015a 0f65  .Z.e.d.d.....Z.e
-00001710: 0d64 1b64 1c84 0083 015a 1065 0d64 1d64  .d.d.....Z.e.d.d
-00001720: 1e84 0083 015a 1165 0d64 1f64 2084 0083  .....Z.e.d.d ...
-00001730: 015a 1265 0d64 2164 2284 0083 015a 1365  .Z.e.d!d"....Z.e
-00001740: 0d64 0364 0c9c 0164 2364 2484 0283 015a  .d.d...d#d$....Z
-00001750: 1447 0064 2564 2684 0064 2683 025a 1564  .G.d%d&..d&..Z.d
-00001760: 0353 0029 2bda 054d 6f64 656c 6301 0000  .S.)+..Modelc...
-00001770: 0000 0000 000a 0000 0009 0000 004f 0000  .............O..
-00001780: 0073 2002 0000 7400 7c02 6a01 6401 8301  .s ...t.|.j.d...
-00001790: 8301 0c00 7d03 788e 7c00 6a02 6a03 6a04  ....}.x.|.j.j.j.
-000017a0: 8300 4400 5d7e 5c02 7d04 7d05 7405 7c05  ..D.]~\.}.}.t.|.
-000017b0: 7406 6a07 8302 724e 7408 7c00 7c04 7409  t.j...rNt.|.|.t.
-000017c0: 7c05 6a0a 7c05 6a0b 7c00 7c03 8304 8303  |.j.|.j.|.|.....
-000017d0: 0100 711e 7405 7c05 7406 6a0c 8302 7274  ..q.t.|.t.j...rt
-000017e0: 7408 7c00 7c04 740d 7c05 6a0a 7c00 7c05  t.|.|.t.|.j.|.|.
-000017f0: 7c03 8304 8303 0100 711e 7405 7c05 7406  |.......q.t.|.t.
-00001800: 6a0e 8302 7290 7408 7c00 7c04 7c05 6a0f  j...r.t.|.|.|.j.
-00001810: 8303 0100 711e 7408 7c00 7c04 6400 8303  ....q.t.|.|.d...
-00001820: 0100 711e 5700 7410 7c02 6a11 8300 8301  ..q.W.t.|.j.....
-00001830: 7d06 9001 7806 7c02 6a04 8300 4400 5dfa  }...x.|.j...D.].
-00001840: 5c02 7d04 7d07 7c04 7c00 6a02 6a12 6b06  \.}.}.|.|.j.j.k.
-00001850: 9001 7210 7413 7c07 6401 8302 72de 7c07  ..r.t.|.d...r.|.
-00001860: 6a14 73ec 7415 6402 6a16 7c07 8301 8301  j.s.t.d.j.|.....
-00001870: 8201 6403 6a16 7c04 8301 7d08 7408 7c00  ..d.j.|...}.t.|.
-00001880: 7c08 7c07 6a14 8303 0100 7c06 6a17 7c08  |.|.j.....|.j.|.
-00001890: 8301 0100 71b8 7c04 7c00 6a02 6a18 6b06  ....q.|.|.j.j.k.
-000018a0: 9001 7228 7415 6404 8301 8201 71b8 7c04  ..r(t.d.....q.|.
-000018b0: 7c00 6a02 6a19 6b06 9001 7240 7415 6405  |.j.j.k...r@t.d.
-000018c0: 8301 8201 71b8 7c04 7c00 6a02 6a06 6b06  ....q.|.|.j.j.k.
-000018d0: 9001 7290 7c00 6a02 6a03 7c04 1900 7d09  ..r.|.j.j.|...}.
-000018e0: 7c07 6400 6b08 9001 727c 7c09 6a1a 0c00  |.d.k...r||.j...
-000018f0: 9001 727c 741b 6406 6a16 7c04 8301 8301  ..r|t.d.j.|.....
-00001900: 8201 7408 7c00 7c04 7c09 6a1c 7c07 8301  ..t.|.|.|.j.|...
-00001910: 8303 0100 71b8 7c04 7c00 6a02 6a1d 6b06  ....q.|.|.j.j.k.
-00001920: 72b8 7408 7c00 7c00 6a02 6a1e 6a01 7c04  r.t.|.|.j.j.j.|.
-00001930: 8301 7c07 8303 0100 71b8 5700 7864 7c00  ..|.....q.W.xd|.
-00001940: 6a02 6a03 6a04 8300 4400 5d54 5c02 7d04  j.j.j...D.]T\.}.
-00001950: 7d09 7c04 7c06 6b06 9001 73c4 7c04 7c00  }.|.|.k...s.|.|.
-00001960: 6a02 6a1f 6b06 9001 72ea 9001 71c4 6e2c  j.j.k...r...q.n,
-00001970: 7420 7c09 6a0f 8301 9002 7208 7408 7c00  t |.j.....r.t.|.
-00001980: 7c04 7c09 6a0f 8300 8303 0100 6e0e 7408  |.|.j.......n.t.
-00001990: 7c00 7c04 7c09 6a0f 8303 0100 9001 71c4  |.|.|.j.......q.
-000019a0: 5700 6400 5300 2907 4e72 2d00 0000 7a3a  W.d.S.).Nr-...z:
-000019b0: 596f 7520 7368 6f75 6c64 2066 6972 7374  You should first
-000019c0: 2063 616c 6c20 2e73 6176 6528 2920 6f6e   call .save() on
-000019d0: 207b 7d20 6265 666f 7265 2072 6566 6572   {} before refer
-000019e0: 7269 6e67 2074 6f20 6974 7a05 7b7d 5f69  ring to itz.{}_i
-000019f0: 647a 4b59 6f75 2063 616e 2774 2073 6574  dzKYou can't set
-00001a00: 2062 6163 6b77 6172 6420 7265 6c61 7469   backward relati
-00001a10: 6f6e 7320 7468 726f 7567 6820 696e 6974  ons through init
-00001a20: 2c20 6368 616e 6765 2072 656c 6174 6564  , change related
-00001a30: 206d 6f64 656c 2069 6e73 7465 6164 7a41   model insteadzA
-00001a40: 596f 7520 6361 6e27 7420 7365 7420 6d32  You can't set m2
-00001a50: 6d20 7265 6c61 7469 6f6e 7320 7468 726f  m relations thro
-00001a60: 7567 6820 696e 6974 2c20 7573 6520 6d32  ugh init, use m2
-00001a70: 6d5f 6d61 6e61 6765 7220 696e 7374 6561  m_manager instea
-00001a80: 647a 2d7b 7d20 6973 206e 6f6e 206e 756c  dz-{} is non nul
-00001a90: 6c61 626c 6520 6669 656c 642c 2062 7574  lable field, but
-00001aa0: 206e 756c 6c20 7761 7320 7061 7373 6564   null was passed
-00001ab0: 2921 da04 626f 6f6c 7257 0000 0072 3000  )!..boolrW...r0.
-00001ac0: 0000 7246 0000 0072 5800 0000 7233 0000  ..rF...rX...r3..
-00001ad0: 0072 0500 0000 da12 4261 636b 7761 7264  .r......Backward
-00001ae0: 464b 5265 6c61 7469 6f6e da07 7365 7461  FKRelation..seta
-00001af0: 7474 7272 0700 0000 722f 0000 0072 2e00  ttrr....r/...r..
-00001b00: 0000 7234 0000 0072 0600 0000 7259 0000  ..r4...r....rY..
-00001b10: 0072 5200 0000 723e 0000 0072 6000 0000  .rR...r>...r`...
-00001b20: 7241 0000 00da 0768 6173 6174 7472 722d  rA.....hasattrr-
-00001b30: 0000 00da 0e41 7373 6572 7469 6f6e 4572  .....AssertionEr
-00001b40: 726f 7272 1a00 0000 725d 0000 0072 4200  rorr....r]...rB.
-00001b50: 0000 7240 0000 0072 5100 0000 da0a 5661  ..r@...rQ.....Va
-00001b60: 6c75 6545 7272 6f72 da0f 746f 5f70 7974  lueError..to_pyt
-00001b70: 686f 6e5f 7661 6c75 6572 3f00 0000 7245  hon_valuer?...rE
-00001b80: 0000 0072 4300 0000 da08 6361 6c6c 6162  ...rC.....callab
-00001b90: 6c65 290a 7248 0000 0072 6700 0000 7268  le).rH...rg...rh
-00001ba0: 0000 00da 0669 735f 6e65 7772 5400 0000  .....is_newrT...
-00001bb0: 720a 0000 005a 0d70 6173 7365 645f 6669  r....Z.passed_fi
-00001bc0: 656c 6473 720b 0000 0072 2e00 0000 da0c  eldsr....r......
-00001bd0: 6669 656c 645f 6f62 6a65 6374 720c 0000  field_objectr...
-00001be0: 0072 0c00 0000 720d 0000 0072 4a00 0000  .r....r....rJ...
-00001bf0: 2101 0000 734c 0000 0000 0110 0216 010c  !...sL..........
-00001c00: 0102 0104 0116 020c 011a 010c 0110 0210  ................
-00001c10: 020c 0114 010e 0112 010c 020a 010e 010c  ................
-00001c20: 010e 0102 0108 020e 0102 0108 020e 010c  ................
-00001c30: 0114 010e 0114 010c 011a 0216 0118 0106  ................
-00001c40: 020c 0112 027a 0e4d 6f64 656c 2e5f 5f69  .....z.Model.__i
-00001c50: 6e69 745f 5f4e 6302 0000 0000 0000 0003  nit__Nc.........
-00001c60: 0000 0004 0000 00c3 0000 0073 3000 0000  ...........s0...
-00001c70: 7c01 7208 7c01 6e06 7c00 6a00 6a01 7d02  |.r.|.n.|.j.j.}.
-00001c80: 7c02 6a02 7c00 6a03 7c02 6401 8d02 6a04  |.j.|.j.|.d...j.
-00001c90: 7c00 8301 4900 6400 4800 0100 6400 5300  |...I.d.H...d.S.
-00001ca0: 2902 4e29 02da 056d 6f64 656c 7247 0000  ).N)...modelrG..
-00001cb0: 0029 0572 3000 0000 7247 0000 00da 0e65  .).r0...rG.....e
-00001cc0: 7865 6375 746f 725f 636c 6173 7372 6a00  xecutor_classrj.
-00001cd0: 0000 da0e 6578 6563 7574 655f 696e 7365  ....execute_inse
-00001ce0: 7274 2903 7248 0000 00da 0875 7369 6e67  rt).rH.....using
-00001cf0: 5f64 6272 4700 0000 720c 0000 0072 0c00  _dbrG...r....r..
-00001d00: 0000 720d 0000 00da 105f 696e 7365 7274  ..r......_insert
-00001d10: 5f69 6e73 7461 6e63 6553 0100 0073 0a00  _instanceS...s..
-00001d20: 0000 0001 1001 0401 0401 0801 7a16 4d6f  ............z.Mo
-00001d30: 6465 6c2e 5f69 6e73 6572 745f 696e 7374  del._insert_inst
-00001d40: 616e 6365 6302 0000 0000 0000 0003 0000  ancec...........
-00001d50: 0004 0000 00c3 0000 0073 3000 0000 7c01  .........s0...|.
-00001d60: 7208 7c01 6e06 7c00 6a00 6a01 7d02 7c02  r.|.n.|.j.j.}.|.
-00001d70: 6a02 7c00 6a03 7c02 6401 8d02 6a04 7c00  j.|.j.|.d...j.|.
-00001d80: 8301 4900 6400 4800 0100 6400 5300 2902  ..I.d.H...d.S.).
-00001d90: 4e29 0272 7700 0000 7247 0000 0029 0572  N).rw...rG...).r
-00001da0: 3000 0000 7247 0000 0072 7800 0000 726a  0...rG...rx...rj
-00001db0: 0000 00da 0e65 7865 6375 7465 5f75 7064  .....execute_upd
-00001dc0: 6174 6529 0372 4800 0000 727a 0000 0072  ate).rH...rz...r
-00001dd0: 4700 0000 720c 0000 0072 0c00 0000 720d  G...r....r....r.
-00001de0: 0000 00da 105f 7570 6461 7465 5f69 6e73  ....._update_ins
-00001df0: 7461 6e63 655a 0100 0073 0a00 0000 0001  tanceZ...s......
-00001e00: 1001 0401 0401 0801 7a16 4d6f 6465 6c2e  ........z.Model.
-00001e10: 5f75 7064 6174 655f 696e 7374 616e 6365  _update_instance
-00001e20: 6301 0000 0000 0000 0003 0000 0003 0000  c...............
-00001e30: 00cf 0000 0073 3000 0000 7c00 6a00 731a  .....s0...|.j.s.
-00001e40: 7c00 6a01 7c01 7c02 8e01 4900 6400 4800  |.j.|.|...I.d.H.
-00001e50: 0100 6e12 7c00 6a02 7c01 7c02 8e01 4900  ..n.|.j.|.|...I.
-00001e60: 6400 4800 0100 6400 5300 2901 4e29 0372  d.H...d.S.).N).r
-00001e70: 2d00 0000 727b 0000 0072 7d00 0000 2903  -...r{...r}...).
-00001e80: 7248 0000 0072 6700 0000 7268 0000 0072  rH...rg...rh...r
-00001e90: 0c00 0000 720c 0000 0072 0d00 0000 da04  ....r....r......
-00001ea0: 7361 7665 6101 0000 7306 0000 0000 0106  savea...s.......
-00001eb0: 0114 027a 0a4d 6f64 656c 2e73 6176 6563  ...z.Model.savec
-00001ec0: 0200 0000 0000 0000 0300 0000 0400 0000  ................
-00001ed0: c300 0000 733a 0000 007c 0172 087c 016e  ....s:...|.r.|.n
-00001ee0: 067c 006a 006a 017d 027c 006a 0273 1a64  .|.j.j.}.|.j.s.d
-00001ef0: 0053 007c 026a 037c 006a 047c 0264 018d  .S.|.j.|.j.|.d..
-00001f00: 026a 057c 0083 0149 0064 0048 0001 0064  .j.|...I.d.H...d
-00001f10: 0053 0029 024e 2902 7277 0000 0072 4700  .S.).N).rw...rG.
-00001f20: 0000 2906 7230 0000 0072 4700 0000 722d  ..).r0...rG...r-
-00001f30: 0000 0072 7800 0000 726a 0000 00da 0e65  ...rx...rj.....e
-00001f40: 7865 6375 7465 5f64 656c 6574 6529 0372  xecute_delete).r
-00001f50: 4800 0000 727a 0000 0072 4700 0000 720c  H...rz...rG...r.
-00001f60: 0000 0072 0c00 0000 720d 0000 00da 0664  ...r....r......d
-00001f70: 656c 6574 6567 0100 0073 0e00 0000 0001  eleteg...s......
-00001f80: 1001 0601 0401 0401 0401 0801 7a0c 4d6f  ............z.Mo
-00001f90: 6465 6c2e 6465 6c65 7465 2901 727a 0000  del.delete).rz..
-00001fa0: 0063 0100 0000 0100 0000 0400 0000 0400  .c..............
-00001fb0: 0000 c700 0000 7338 0000 007c 0172 087c  ......s8...|.r.|
-00001fc0: 016e 067c 006a 006a 017d 037c 036a 027c  .n.|.j.j.}.|.j.|
-00001fd0: 006a 037c 0364 018d 026a 047c 0067 0166  .j.|.d...j.|.g.f
-00001fe0: 017c 029e 028e 0049 0064 0048 0001 0064  .|.....I.d.H...d
-00001ff0: 0053 0029 024e 2902 7277 0000 0072 4700  .S.).N).rw...rG.
-00002000: 0000 2905 7230 0000 0072 4700 0000 7278  ..).r0...rG...rx
-00002010: 0000 0072 6a00 0000 da0e 6665 7463 685f  ...rj.....fetch_
-00002020: 666f 725f 6c69 7374 2904 7248 0000 0072  for_list).rH...r
-00002030: 7a00 0000 7267 0000 0072 4700 0000 720c  z...rg...rG...r.
-00002040: 0000 0072 0c00 0000 720d 0000 00da 0d66  ...r....r......f
-00002050: 6574 6368 5f72 656c 6174 6564 7001 0000  etch_relatedp...
-00002060: 730a 0000 0000 0110 0104 0104 0108 017a  s..............z
-00002070: 134d 6f64 656c 2e66 6574 6368 5f72 656c  .Model.fetch_rel
-00002080: 6174 6564 6301 0000 0000 0000 0001 0000  atedc...........
-00002090: 0001 0000 0043 0000 0073 0800 0000 7c00  .....C...s....|.
-000020a0: 6a00 6a01 5300 2901 4e29 0272 6a00 0000  j.j.S.).N).rj...
-000020b0: 724b 0000 0029 0172 4800 0000 720c 0000  rK...).rH...r...
-000020c0: 0072 0c00 0000 720d 0000 00da 075f 5f73  .r....r......__s
-000020d0: 7472 5f5f 7701 0000 7302 0000 0000 017a  tr__w...s......z
-000020e0: 0d4d 6f64 656c 2e5f 5f73 7472 5f5f 6301  .Model.__str__c.
-000020f0: 0000 0000 0000 0001 0000 0003 0000 0043  ...............C
-00002100: 0000 0073 1400 0000 6401 6a00 7c00 6a01  ...s....d.j.|.j.
-00002110: 6a02 7c00 6a03 8300 8302 5300 2902 4e7a  j.|.j.....S.).Nz
-00002120: 083c 7b7d 3a20 7b7d 3e29 0472 1a00 0000  .<{}: {}>).r....
-00002130: 726a 0000 0072 4b00 0000 7283 0000 0029  rj...rK...r....)
-00002140: 0172 4800 0000 720c 0000 0072 0c00 0000  .rH...r....r....
-00002150: 720d 0000 00da 085f 5f72 6570 725f 5f7a  r......__repr__z
-00002160: 0100 0073 0200 0000 0001 7a0e 4d6f 6465  ...s......z.Mode
-00002170: 6c2e 5f5f 7265 7072 5f5f 6301 0000 0000  l.__repr__c.....
-00002180: 0000 0001 0000 0002 0000 0043 0000 0073  ...........C...s
-00002190: 2600 0000 7400 7c00 6a01 8301 0c00 7314  &...t.|.j.....s.
-000021a0: 7c00 6a01 0c00 721c 7402 6401 8301 8201  |.j...r.t.d.....
-000021b0: 7403 7c00 6a01 8301 5300 2902 4e7a 294d  t.|.j...S.).Nz)M
-000021c0: 6f64 656c 2069 6e73 7461 6e63 6573 2077  odel instances w
-000021d0: 6974 686f 7574 2069 6420 6172 6520 756e  ithout id are un
-000021e0: 6861 7368 6162 6c65 2904 7270 0000 0072  hashable).rp...r
-000021f0: 2d00 0000 da09 5479 7065 4572 726f 72da  -.....TypeError.
-00002200: 0468 6173 6829 0172 4800 0000 720c 0000  .hash).rH...r...
-00002210: 0072 0c00 0000 720d 0000 00da 085f 5f68  .r....r......__h
-00002220: 6173 685f 5f7d 0100 0073 0600 0000 0001  ash__}...s......
-00002230: 1401 0801 7a0e 4d6f 6465 6c2e 5f5f 6861  ....z.Model.__ha
-00002240: 7368 5f5f 6302 0000 0000 0000 0002 0000  sh__c...........
-00002250: 0003 0000 0043 0000 0073 2400 0000 7400  .....C...s$...t.
-00002260: 7c00 8301 7400 7c01 8301 6b02 7220 7c00  |...t.|...k.r |.
-00002270: 6a01 7c01 6a01 6b02 7220 6401 5300 6402  j.|.j.k.r d.S.d.
-00002280: 5300 2903 4e54 4629 0272 2f00 0000 722d  S.).NTF).r/...r-
-00002290: 0000 0029 0272 4800 0000 da05 6f74 6865  ...).rH.....othe
-000022a0: 7272 0c00 0000 720c 0000 0072 0d00 0000  rr....r....r....
-000022b0: da06 5f5f 6571 5f5f 8201 0000 7306 0000  ..__eq__....s...
-000022c0: 0000 021c 0104 017a 0c4d 6f64 656c 2e5f  .......z.Model._
-000022d0: 5f65 715f 5f63 0300 0000 0000 0000 0500  _eq__c..........
-000022e0: 0000 0400 0000 cb00 0000 734a 0000 007c  ..........sJ...|
-000022f0: 0273 0869 007d 027c 006a 0066 007c 038e  .s.i.}.|.j.f.|..
-00002300: 016a 0183 0049 0064 0048 007d 047c 0472  .j...I.d.H.}.|.r
-00002310: 2a7c 0464 0166 0253 007c 0066 007c 027c  *|.d.f.S.|.f.|.|
-00002320: 0397 028e 016a 027c 0164 028d 0149 0064  .....j.|.d...I.d
-00002330: 0048 0064 0366 0253 0029 044e 4629 0172  .H.d.f.S.).NF).r
-00002340: 7a00 0000 5429 03da 0666 696c 7465 72da  z...T)...filter.
-00002350: 0566 6972 7374 727e 0000 0029 05da 0363  .firstr~...)...c
-00002360: 6c73 727a 0000 00da 0864 6566 6175 6c74  lsrz.....default
-00002370: 7372 6800 0000 da08 696e 7374 616e 6365  srh.....instance
-00002380: 720c 0000 0072 0c00 0000 720d 0000 00da  r....r....r.....
-00002390: 0d67 6574 5f6f 725f 6372 6561 7465 8801  .get_or_create..
-000023a0: 0000 730c 0000 0000 0204 0104 0116 0104  ..s.............
-000023b0: 0108 017a 134d 6f64 656c 2e67 6574 5f6f  ...z.Model.get_o
-000023c0: 725f 6372 6561 7465 6301 0000 0000 0000  r_createc.......
-000023d0: 0003 0000 0003 0000 00cb 0000 0073 2400  .............s$.
-000023e0: 0000 7c00 6600 7c01 8e01 7d02 7c02 6a00  ..|.f.|...}.|.j.
-000023f0: 7c01 6a01 6401 8301 8301 4900 6400 4800  |.j.d.....I.d.H.
-00002400: 0100 7c02 5300 2902 4e72 7a00 0000 2902  ..|.S.).Nrz...).
-00002410: 727e 0000 0072 5700 0000 2903 728c 0000  r~...rW...).r...
-00002420: 0072 6800 0000 728e 0000 0072 0c00 0000  .rh...r....r....
-00002430: 720c 0000 0072 0d00 0000 da06 6372 6561  r....r......crea
-00002440: 7465 9101 0000 7306 0000 0000 020a 0116  te....s.........
-00002450: 017a 0c4d 6f64 656c 2e63 7265 6174 6563  .z.Model.createc
-00002460: 0100 0000 0000 0000 0100 0000 0200 0000  ................
-00002470: 4300 0000 730c 0000 0074 007c 0083 016a  C...s....t.|...j
-00002480: 0183 0053 0029 014e 2902 7208 0000 0072  ...S.).N).r....r
-00002490: 8b00 0000 2901 728c 0000 0072 0c00 0000  ....).r....r....
-000024a0: 720c 0000 0072 0d00 0000 728b 0000 0097  r....r....r.....
-000024b0: 0100 0073 0200 0000 0002 7a0b 4d6f 6465  ...s......z.Mode
-000024c0: 6c2e 6669 7273 7463 0100 0000 0000 0000  l.firstc........
-000024d0: 0300 0000 0300 0000 4f00 0000 7310 0000  ........O...s...
-000024e0: 0074 007c 0083 016a 017c 017c 028e 0153  .t.|...j.|.|...S
-000024f0: 0029 014e 2902 7208 0000 0072 8a00 0000  .).N).r....r....
-00002500: 2903 728c 0000 0072 6700 0000 7268 0000  ).r....rg...rh..
-00002510: 0072 0c00 0000 720c 0000 0072 0d00 0000  .r....r....r....
-00002520: 728a 0000 009b 0100 0073 0200 0000 0002  r........s......
-00002530: 7a0c 4d6f 6465 6c2e 6669 6c74 6572 6301  z.Model.filterc.
-00002540: 0000 0000 0000 0001 0000 0002 0000 0043  ...............C
-00002550: 0000 0073 0800 0000 7400 7c00 8301 5300  ...s....t.|...S.
-00002560: 2901 4e29 0172 0800 0000 2901 728c 0000  ).N).r....).r...
-00002570: 0072 0c00 0000 720c 0000 0072 0d00 0000  .r....r....r....
-00002580: da03 616c 6c9f 0100 0073 0200 0000 0002  ..all....s......
-00002590: 7a09 4d6f 6465 6c2e 616c 6c63 0100 0000  z.Model.allc....
-000025a0: 0000 0000 0300 0000 0300 0000 4f00 0000  ............O...
-000025b0: 7314 0000 0074 007c 0083 016a 017c 017c  s....t.|...j.|.|
-000025c0: 028e 016a 0283 0053 0029 014e 2903 7208  ...j...S.).N).r.
-000025d0: 0000 0072 8a00 0000 728b 0000 0029 0372  ...r....r....).r
-000025e0: 8c00 0000 7267 0000 0072 6800 0000 720c  ....rg...rh...r.
-000025f0: 0000 0072 0c00 0000 720d 0000 0072 5700  ...r....r....rW.
-00002600: 0000 a301 0000 7302 0000 0000 037a 094d  ......s......z.M
-00002610: 6f64 656c 2e67 6574 6302 0000 0001 0000  odel.getc.......
-00002620: 0005 0000 0004 0000 00c7 0000 0073 3400  .............s4.
-00002630: 0000 7c02 7208 7c02 6e06 7c00 6a00 6a01  ..|.r.|.n.|.j.j.
-00002640: 7d04 7c04 6a02 7c00 7c04 6401 8d02 6a03  }.|.j.|.|.d...j.
-00002650: 7c01 6601 7c03 9e02 8e00 4900 6400 4800  |.f.|.....I.d.H.
-00002660: 0100 6400 5300 2902 4e29 0272 7700 0000  ..d.S.).N).rw...
-00002670: 7247 0000 0029 0472 3000 0000 7247 0000  rG...).r0...rG..
-00002680: 0072 7800 0000 7281 0000 0029 0572 8c00  .rx...r....).r..
-00002690: 0000 da0d 696e 7374 616e 6365 5f6c 6973  ....instance_lis
-000026a0: 7472 7a00 0000 7267 0000 0072 4700 0000  trz...rg...rG...
-000026b0: 720c 0000 0072 0c00 0000 720d 0000 0072  r....r....r....r
-000026c0: 8100 0000 a801 0000 730a 0000 0000 0210  ........s.......
-000026d0: 0104 0102 0108 017a 144d 6f64 656c 2e66  .......z.Model.f
-000026e0: 6574 6368 5f66 6f72 5f6c 6973 7463 0000  etch_for_listc..
-000026f0: 0000 0000 0000 0000 0000 0100 0000 4000  ..............@.
-00002700: 0000 730c 0000 0065 005a 0164 005a 0264  ..s....e.Z.d.Z.d
-00002710: 0153 0029 027a 0a4d 6f64 656c 2e4d 6574  .S.).z.Model.Met
-00002720: 614e 2903 724b 0000 0072 4c00 0000 724d  aN).rK...rL...rM
-00002730: 0000 0072 0c00 0000 720c 0000 0072 0c00  ...r....r....r..
-00002740: 0000 720d 0000 0072 4f00 0000 b001 0000  ..r....rO.......
-00002750: 7302 0000 0008 0172 4f00 0000 2901 4e29  s......rO...).N)
-00002760: 014e 2901 4e29 024e 4e29 1672 4b00 0000  .N).N).NN).rK...
-00002770: 724c 0000 0072 4d00 0000 724a 0000 0072  rL...rM...rJ...r
-00002780: 7b00 0000 727d 0000 0072 7e00 0000 7280  {...r}...r~...r.
-00002790: 0000 0072 8200 0000 7283 0000 0072 8400  ...r....r....r..
-000027a0: 0000 7287 0000 0072 8900 0000 da0b 636c  ..r....r......cl
-000027b0: 6173 736d 6574 686f 6472 8f00 0000 7290  assmethodr....r.
-000027c0: 0000 0072 8b00 0000 728a 0000 0072 9100  ...r....r....r..
-000027d0: 0000 7257 0000 0072 8100 0000 724f 0000  ..rW...r....rO..
-000027e0: 0072 0c00 0000 720c 0000 0072 0c00 0000  .r....r....r....
-000027f0: 720d 0000 0072 6c00 0000 2001 0000 7328  r....rl... ...s(
-00002800: 0000 0008 0108 320a 070a 0708 060a 090e  ......2.........
-00002810: 0708 0308 0308 0508 0602 010c 080c 060c  ................
-00002820: 040c 040c 040c 0502 0110 0772 6c00 0000  ...........rl...
-00002830: 2901 da09 6d65 7461 636c 6173 7329 2172  )...metaclass)!r
-00002840: 2300 0000 da06 7079 7069 6b61 7202 0000  #.....pypikar...
-00002850: 0072 0300 0000 da0c 7079 7069 6b61 2e65  .r......pypika.e
-00002860: 6e75 6d73 7204 0000 0072 6200 0000 7205  numsr....rb...r.
-00002870: 0000 00da 0f74 6f72 746f 6973 652e 6669  .....tortoise.fi
-00002880: 656c 6473 7206 0000 0072 0700 0000 da11  eldsr....r......
-00002890: 746f 7274 6f69 7365 2e71 7565 7279 7365  tortoise.queryse
-000028a0: 7472 0800 0000 720e 0000 0072 1100 0000  tr....r....r....
-000028b0: 7213 0000 0072 1500 0000 7216 0000 0072  r....r....r....r
-000028c0: 1b00 0000 721c 0000 0072 1d00 0000 721f  ....r....r....r.
-000028d0: 0000 0072 2000 0000 7221 0000 0072 2c00  ...r ...r!...r,.
-000028e0: 0000 7231 0000 00da 0373 7472 7259 0000  ..r1.....strrY..
-000028f0: 0072 3900 0000 723a 0000 0072 2f00 0000  .r9...r:...r/...
-00002900: 724e 0000 0072 6c00 0000 720c 0000 0072  rN...rl...r....r
-00002910: 0c00 0000 720c 0000 0072 0d00 0000 da08  ....r....r......
-00002920: 3c6d 6f64 756c 653e 0100 0000 732c 0000  <module>....s,..
-00002930: 0008 0210 010c 020c 0110 010c 0308 0408  ................
-00002940: 0408 0408 0708 0708 0408 0408 0408 0608  ................
-00002950: 0608 0608 2008 2014 4a0e 1210 41         .... . .J...A
+00000060: 0100 6400 6406 6c0a 6d0b 5a0b 6d0c 5a0c  ..d.d.l.m.Z.m.Z.
+00000070: 0100 6400 6407 6c0d 6d0e 5a0e 6d0f 5a0f  ..d.d.l.m.Z.m.Z.
+00000080: 0100 6400 6408 6c10 6d11 5a11 0100 6409  ..d.d.l.m.Z...d.
+00000090: 640a 8400 5a12 640b 640c 8400 5a13 640d  d...Z.d.d...Z.d.
+000000a0: 640e 8400 5a14 640f 6410 8400 5a15 6411  d...Z.d.d...Z.d.
+000000b0: 6412 8400 5a16 6413 6414 8400 5a17 6415  d...Z.d.d...Z.d.
+000000c0: 6416 8400 5a18 6417 6418 8400 5a19 6419  d...Z.d.d...Z.d.
+000000d0: 641a 8400 5a1a 641b 641c 8400 5a1b 641d  d...Z.d.d...Z.d.
+000000e0: 641e 8400 5a1c 641f 6420 8400 5a1d 6421  d...Z.d.d ..Z.d!
+000000f0: 6422 8400 5a1e 651f 6507 6a20 651f 6423  d"..Z.e.e.j e.d#
+00000100: 9c03 6424 6425 8404 5a21 4700 6426 6427  ..d$d%..Z!G.d&d'
+00000110: 8400 6427 8302 5a22 4700 6428 6429 8400  ..d'..Z"G.d(d)..
+00000120: 6429 6523 8303 5a24 4700 642a 642b 8400  d)e#..Z$G.d*d+..
+00000130: 642b 6524 642c 8d03 5a25 6401 5300 292d  d+e$d,..Z%d.S.)-
+00000140: e900 0000 004e 2902 da05 5461 626c 65da  .....N)...Table.
+00000150: 0966 756e 6374 696f 6e73 2901 da08 5371  .functions)...Sq
+00000160: 6c54 7970 6573 2901 da06 6669 656c 6473  lTypes)...fields
+00000170: 2901 da12 6375 7272 656e 745f 636f 6e6e  )...current_conn
+00000180: 6563 7469 6f6e 2902 da12 436f 6e66 6967  ection)...Config
+00000190: 7572 6174 696f 6e45 7272 6f72 da10 4f70  urationError..Op
+000001a0: 6572 6174 696f 6e61 6c45 7272 6f72 2902  erationalError).
+000001b0: da19 4d61 6e79 546f 4d61 6e79 5265 6c61  ..ManyToManyRela
+000001c0: 7469 6f6e 4d61 6e61 6765 72da 1652 656c  tionManager..Rel
+000001d0: 6174 696f 6e51 7565 7279 436f 6e74 6169  ationQueryContai
+000001e0: 6e65 7229 01da 0851 7565 7279 5365 7463  ner)...QuerySetc
+000001f0: 0200 0000 0000 0000 0200 0000 0200 0000  ................
+00000200: 4300 0000 730a 0000 007c 006a 007c 0183  C...s....|.j.|..
+00000210: 0153 0029 014e 2901 da04 6973 696e 2902  .S.).N)...isin).
+00000220: da05 6669 656c 64da 0576 616c 7565 a900  ..field..value..
+00000230: 720f 0000 00fa 432f 5573 6572 732f 616e  r.....C/Users/an
+00000240: 6472 6579 626f 6e64 6172 2f50 7943 6861  dreybondar/PyCha
+00000250: 726d 5072 6f6a 6563 7473 2f74 6f72 746f  rmProjects/torto
+00000260: 6973 652d 6f72 6d2f 746f 7274 6f69 7365  ise-orm/tortoise
+00000270: 2f6d 6f64 656c 732e 7079 da05 6973 5f69  /models.py..is_i
+00000280: 6e0d 0000 0073 0200 0000 0001 7211 0000  n....s......r...
+00000290: 0063 0200 0000 0000 0000 0200 0000 0200  .c..............
+000002a0: 0000 4300 0000 7312 0000 007c 006a 007c  ..C...s....|.j.|
+000002b0: 0183 017c 006a 0183 0042 0053 0029 014e  ...|.j...B.S.).N
+000002c0: 2902 da05 6e6f 7469 6eda 0669 736e 756c  )...notin..isnul
+000002d0: 6c29 0272 0d00 0000 720e 0000 0072 0f00  l).r....r....r..
+000002e0: 0000 720f 0000 0072 1000 0000 da06 6e6f  ..r....r......no
+000002f0: 745f 696e 1100 0000 7302 0000 0000 0172  t_in....s......r
+00000300: 1400 0000 6302 0000 0000 0000 0002 0000  ....c...........
+00000310: 0002 0000 0043 0000 0073 1200 0000 7c00  .....C...s....|.
+00000320: 6a00 7c01 8301 7c00 6a01 8300 4200 5300  j.|...|.j...B.S.
+00000330: 2901 4e29 02da 026e 6572 1300 0000 2902  ).N)...ner....).
+00000340: 720d 0000 0072 0e00 0000 720f 0000 0072  r....r....r....r
+00000350: 0f00 0000 7210 0000 00da 096e 6f74 5f65  ....r......not_e
+00000360: 7175 616c 1500 0000 7302 0000 0000 0172  qual....s......r
+00000370: 1600 0000 6302 0000 0000 0000 0002 0000  ....c...........
+00000380: 0001 0000 0043 0000 0073 1800 0000 7c01  .....C...s....|.
+00000390: 720c 7c00 6a00 8300 5300 7c00 6a01 8300  r.|.j...S.|.j...
+000003a0: 5300 6400 5300 2901 4e29 0272 1300 0000  S.d.S.).N).r....
+000003b0: da07 6e6f 746e 756c 6c29 0272 0d00 0000  ..notnull).r....
+000003c0: 720e 0000 0072 0f00 0000 720f 0000 0072  r....r....r....r
+000003d0: 1000 0000 da07 6973 5f6e 756c 6c19 0000  ......is_null...
+000003e0: 0073 0600 0000 0001 0401 0802 7218 0000  .s..........r...
+000003f0: 0063 0200 0000 0000 0000 0200 0000 0100  .c..............
+00000400: 0000 4300 0000 7318 0000 007c 0172 0c7c  ..C...s....|.r.|
+00000410: 006a 0083 0053 007c 006a 0183 0053 0064  .j...S.|.j...S.d
+00000420: 0053 0029 014e 2902 7217 0000 0072 1300  .S.).N).r....r..
+00000430: 0000 2902 720d 0000 0072 0e00 0000 720f  ..).r....r....r.
+00000440: 0000 0072 0f00 0000 7210 0000 00da 086e  ...r....r......n
+00000450: 6f74 5f6e 756c 6c20 0000 0073 0600 0000  ot_null ...s....
+00000460: 0001 0401 0802 7219 0000 0063 0200 0000  ......r....c....
+00000470: 0000 0000 0200 0000 0300 0000 4300 0000  ............C...
+00000480: 731a 0000 0074 006a 017c 0074 026a 0383  s....t.j.|.t.j..
+00000490: 026a 0464 016a 057c 0183 0183 0153 0029  .j.d.j.|.....S.)
+000004a0: 024e 7a04 257b 7d25 2906 7203 0000 00da  .Nz.%{}%).r.....
+000004b0: 0443 6173 7472 0400 0000 da07 5641 5243  .Castr......VARC
+000004c0: 4841 52da 046c 696b 65da 0666 6f72 6d61  HAR..like..forma
+000004d0: 7429 0272 0d00 0000 720e 0000 0072 0f00  t).r....r....r..
+000004e0: 0000 720f 0000 0072 1000 0000 da08 636f  ..r....r......co
+000004f0: 6e74 6169 6e73 2700 0000 7302 0000 0000  ntains'...s.....
+00000500: 0172 1e00 0000 6302 0000 0000 0000 0002  .r....c.........
+00000510: 0000 0003 0000 0043 0000 0073 1a00 0000  .......C...s....
+00000520: 7400 6a01 7c00 7402 6a03 8302 6a04 6401  t.j.|.t.j...j.d.
+00000530: 6a05 7c01 8301 8301 5300 2902 4e7a 037b  j.|.....S.).Nz.{
+00000540: 7d25 2906 7203 0000 0072 1a00 0000 7204  }%).r....r....r.
+00000550: 0000 0072 1b00 0000 721c 0000 0072 1d00  ...r....r....r..
+00000560: 0000 2902 720d 0000 0072 0e00 0000 720f  ..).r....r....r.
+00000570: 0000 0072 0f00 0000 7210 0000 00da 0b73  ...r....r......s
+00000580: 7461 7274 735f 7769 7468 2b00 0000 7302  tarts_with+...s.
+00000590: 0000 0000 0172 1f00 0000 6302 0000 0000  .....r....c.....
+000005a0: 0000 0002 0000 0003 0000 0043 0000 0073  ...........C...s
+000005b0: 1a00 0000 7400 6a01 7c00 7402 6a03 8302  ....t.j.|.t.j...
+000005c0: 6a04 6401 6a05 7c01 8301 8301 5300 2902  j.d.j.|.....S.).
+000005d0: 4e7a 0325 7b7d 2906 7203 0000 0072 1a00  Nz.%{}).r....r..
+000005e0: 0000 7204 0000 0072 1b00 0000 721c 0000  ..r....r....r...
+000005f0: 0072 1d00 0000 2902 720d 0000 0072 0e00  .r....).r....r..
+00000600: 0000 720f 0000 0072 0f00 0000 7210 0000  ..r....r....r...
+00000610: 00da 0965 6e64 735f 7769 7468 2f00 0000  ...ends_with/...
+00000620: 7302 0000 0000 0172 2000 0000 6302 0000  s......r ...c...
+00000630: 0000 0000 0002 0000 0004 0000 0043 0000  .............C..
+00000640: 0073 2600 0000 7400 6a01 7400 6a02 7c00  .s&...t.j.t.j.|.
+00000650: 7403 6a04 8302 8301 6a05 7400 6a01 6401  t.j.....j.t.j.d.
+00000660: 6a06 7c01 8301 8301 8301 5300 2902 4e7a  j.|.......S.).Nz
+00000670: 0425 7b7d 2529 0772 0300 0000 da05 5570  .%{}%).r......Up
+00000680: 7065 7272 1a00 0000 7204 0000 0072 1b00  perr....r....r..
+00000690: 0000 721c 0000 0072 1d00 0000 2902 720d  ..r....r....).r.
+000006a0: 0000 0072 0e00 0000 720f 0000 0072 0f00  ...r....r....r..
+000006b0: 0000 7210 0000 00da 1469 6e73 656e 7369  ..r......insensi
+000006c0: 7469 7665 5f63 6f6e 7461 696e 7333 0000  tive_contains3..
+000006d0: 0073 0400 0000 0001 1401 7222 0000 0063  .s........r"...c
+000006e0: 0200 0000 0000 0000 0200 0000 0400 0000  ................
+000006f0: 4300 0000 7326 0000 0074 006a 0174 006a  C...s&...t.j.t.j
+00000700: 027c 0074 036a 0483 0283 016a 0574 006a  .|.t.j.....j.t.j
+00000710: 0164 016a 067c 0183 0183 0183 0153 0029  .d.j.|.......S.)
+00000720: 024e 7a03 7b7d 2529 0772 0300 0000 7221  .Nz.{}%).r....r!
+00000730: 0000 0072 1a00 0000 7204 0000 0072 1b00  ...r....r....r..
+00000740: 0000 721c 0000 0072 1d00 0000 2902 720d  ..r....r....).r.
+00000750: 0000 0072 0e00 0000 720f 0000 0072 0f00  ...r....r....r..
+00000760: 0000 7210 0000 00da 1769 6e73 656e 7369  ..r......insensi
+00000770: 7469 7665 5f73 7461 7274 735f 7769 7468  tive_starts_with
+00000780: 3900 0000 7304 0000 0000 0114 0172 2300  9...s........r#.
+00000790: 0000 6302 0000 0000 0000 0002 0000 0004  ..c.............
+000007a0: 0000 0043 0000 0073 2600 0000 7400 6a01  ...C...s&...t.j.
+000007b0: 7400 6a02 7c00 7403 6a04 8302 8301 6a05  t.j.|.t.j.....j.
+000007c0: 7400 6a01 6401 6a06 7c01 8301 8301 8301  t.j.d.j.|.......
+000007d0: 5300 2902 4e7a 0325 7b7d 2907 7203 0000  S.).Nz.%{}).r...
+000007e0: 0072 2100 0000 721a 0000 0072 0400 0000  .r!...r....r....
+000007f0: 721b 0000 0072 1c00 0000 721d 0000 0029  r....r....r....)
+00000800: 0272 0d00 0000 720e 0000 0072 0f00 0000  .r....r....r....
+00000810: 720f 0000 0072 1000 0000 da15 696e 7365  r....r......inse
+00000820: 6e73 6974 6976 655f 656e 6473 5f77 6974  nsitive_ends_wit
+00000830: 683f 0000 0073 0400 0000 0001 1401 7224  h?...s........r$
+00000840: 0000 0063 0200 0000 0000 0000 0300 0000  ...c............
+00000850: 0d00 0000 4300 0000 7380 0000 007c 007c  ....C...s....|.|
+00000860: 016a 007c 016a 0174 026a 0374 047c 016a  .j.|.j.t.j.t.|.j
+00000870: 0583 0164 019c 0464 026a 067c 0083 017c  ...d...d.j.|...|
+00000880: 016a 007c 016a 0174 0774 047c 016a 0583  .j.|.j.t.t.|.j..
+00000890: 0164 019c 0464 036a 067c 0083 017c 016a  .d...d.j.|...|.j
+000008a0: 007c 016a 0174 0874 047c 016a 0583 0174  .|.j.t.t.|.j...t
+000008b0: 0964 049c 0564 056a 067c 0083 017c 016a  .d...d.j.|...|.j
+000008c0: 007c 016a 0174 0a74 047c 016a 0583 0174  .|.j.t.t.|.j...t
+000008d0: 0964 049c 0569 047d 027c 0253 0029 064e  .d...i.}.|.S.).N
+000008e0: 2904 720d 0000 00da 0c62 6163 6b77 6172  ).r......backwar
+000008f0: 645f 6b65 79da 086f 7065 7261 746f 72da  d_key..operator.
+00000900: 0574 6162 6c65 7a07 7b7d 5f5f 6e6f 747a  .tablez.{}__notz
+00000910: 067b 7d5f 5f69 6e29 0572 0d00 0000 7225  .{}__in).r....r%
+00000920: 0000 0072 2600 0000 7227 0000 00da 0d76  ...r&...r'.....v
+00000930: 616c 7565 5f65 6e63 6f64 6572 7a0a 7b7d  alue_encoderz.{}
+00000940: 5f5f 6e6f 745f 696e 290b da0b 666f 7277  __not_in)...forw
+00000950: 6172 645f 6b65 7972 2500 0000 7226 0000  ard_keyr%...r&..
+00000960: 00da 0265 7172 0200 0000 da07 7468 726f  ...eqr......thro
+00000970: 7567 6872 1d00 0000 7216 0000 0072 1100  ughr....r....r..
+00000980: 0000 da04 6c69 7374 7214 0000 0029 03da  ....listr....)..
+00000990: 0a66 6965 6c64 5f6e 616d 6572 0d00 0000  .field_namer....
+000009a0: da07 6669 6c74 6572 7372 0f00 0000 720f  ..filtersr....r.
+000009b0: 0000 0072 1000 0000 da0f 6765 745f 6d32  ...r......get_m2
+000009c0: 6d5f 6669 6c74 6572 7345 0000 0073 2e00  m_filtersE...s..
+000009d0: 0000 0002 0201 0401 0401 0401 0c02 0801  ................
+000009e0: 0401 0401 0201 0c02 0801 0401 0401 0201  ................
+000009f0: 0801 0602 0801 0401 0401 0201 0801 0a03  ................
+00000a00: 722f 0000 0063 0200 0000 0000 0000 0300  r/...c..........
+00000a10: 0000 0d00 0000 4300 0000 7388 0000 007c  ......C...s....|
+00000a20: 0064 017c 016a 0074 016a 0274 037c 016a  .d.|.j.t.j.t.|.j
+00000a30: 046a 056a 0683 0164 029c 0464 036a 077c  .j.j...d...d.j.|
+00000a40: 0083 0164 017c 016a 0074 0874 037c 016a  ...d.|.j.t.t.|.j
+00000a50: 046a 056a 0683 0164 029c 0464 046a 077c  .j.j...d...d.j.|
+00000a60: 0083 0164 017c 016a 0074 0974 037c 016a  ...d.|.j.t.t.|.j
+00000a70: 046a 056a 0683 0174 0a64 059c 0564 066a  .j.j...t.d...d.j
+00000a80: 077c 0083 0164 017c 016a 0074 0b74 037c  .|...d.|.j.t.t.|
+00000a90: 016a 046a 056a 0683 0174 0a64 059c 0569  .j.j.j...t.d...i
+00000aa0: 047d 027c 0253 0029 074e da02 6964 2904  .}.|.S.).N..id).
+00000ab0: 720d 0000 0072 2500 0000 7226 0000 0072  r....r%...r&...r
+00000ac0: 2700 0000 7a07 7b7d 5f5f 6e6f 747a 067b  '...z.{}__notz.{
+00000ad0: 7d5f 5f69 6e29 0572 0d00 0000 7225 0000  }__in).r....r%..
+00000ae0: 0072 2600 0000 7227 0000 0072 2800 0000  .r&...r'...r(...
+00000af0: 7a0a 7b7d 5f5f 6e6f 745f 696e 290c da0e  z.{}__not_in)...
+00000b00: 7265 6c61 7469 6f6e 5f66 6965 6c64 7226  relation_fieldr&
+00000b10: 0000 0072 2a00 0000 7202 0000 00da 0474  ...r*...r......t
+00000b20: 7970 65da 055f 6d65 7461 7227 0000 0072  ype.._metar'...r
+00000b30: 1d00 0000 7216 0000 0072 1100 0000 722c  ....r....r....r,
+00000b40: 0000 0072 1400 0000 2903 722d 0000 0072  ...r....).r-...r
+00000b50: 0d00 0000 722e 0000 0072 0f00 0000 720f  ....r....r....r.
+00000b60: 0000 0072 1000 0000 da17 6765 745f 6261  ...r......get_ba
+00000b70: 636b 7761 7264 5f66 6b5f 6669 6c74 6572  ckward_fk_filter
+00000b80: 7365 0000 0073 2e00 0000 0002 0201 0201  se...s..........
+00000b90: 0401 0401 1002 0801 0201 0401 0201 1002  ................
+00000ba0: 0801 0201 0401 0201 0c01 0602 0801 0201  ................
+00000bb0: 0401 0201 0c01 0a03 7234 0000 0029 0372  ........r4...).r
+00000bc0: 2d00 0000 720d 0000 00da 0c73 6f75 7263  -...r......sourc
+00000bd0: 655f 6669 656c 6463 0300 0000 0000 0000  e_fieldc........
+00000be0: 0400 0000 2200 0000 4300 0000 7326 0100  ...."...C...s&..
+00000bf0: 0074 007c 0174 016a 0283 0272 1674 037c  .t.|.t.j...r.t.|
+00000c00: 007c 0183 0253 007c 007c 0274 046a 0564  .|...S.|.|.t.j.d
+00000c10: 019c 0264 026a 067c 0083 017c 0274 0764  ...d.j.|...|.t.d
+00000c20: 019c 0264 036a 067c 0083 017c 0274 0874  ...d.j.|...|.t.t
+00000c30: 0964 049c 0364 056a 067c 0083 017c 0274  .d...d.j.|...|.t
+00000c40: 0a74 0964 049c 0364 066a 067c 0083 017c  .t.d...d.j.|...|
+00000c50: 0274 0b64 019c 0264 076a 067c 0083 017c  .t.d...d.j.|...|
+00000c60: 0274 0c64 019c 0264 086a 067c 0083 017c  .t.d...d.j.|...|
+00000c70: 0274 046a 0d64 019c 0264 096a 067c 0083  .t.j.d...d.j.|..
+00000c80: 017c 0274 046a 0e64 019c 0264 0a6a 067c  .|.t.j.d...d.j.|
+00000c90: 0083 017c 0274 046a 0f64 019c 0264 0b6a  ...|.t.j.d...d.j
+00000ca0: 067c 0083 017c 0274 046a 1064 019c 0264  .|...|.t.j.d...d
+00000cb0: 0c6a 067c 0083 017c 0274 1164 019c 0264  .j.|...|.t.d...d
+00000cc0: 0d6a 067c 0083 017c 0274 1264 019c 0264  .j.|...|.t.d...d
+00000cd0: 0e6a 067c 0083 017c 0274 1364 019c 0264  .j.|...|.t.d...d
+00000ce0: 0f6a 067c 0083 017c 0274 1464 019c 0264  .j.|...|.t.d...d
+00000cf0: 106a 067c 0083 017c 0274 1564 019c 0264  .j.|...|.t.d...d
+00000d00: 116a 067c 0083 017c 0274 1664 019c 0269  .j.|...|.t.d...i
+00000d10: 107d 037c 0353 0029 124e 2902 720d 0000  .}.|.S.).N).r...
+00000d20: 0072 2600 0000 7a07 7b7d 5f5f 6e6f 747a  .r&...z.{}__notz
+00000d30: 067b 7d5f 5f69 6e29 0372 0d00 0000 7226  .{}__in).r....r&
+00000d40: 0000 0072 2800 0000 7a0a 7b7d 5f5f 6e6f  ...r(...z.{}__no
+00000d50: 745f 696e 7a0a 7b7d 5f5f 6973 6e75 6c6c  t_inz.{}__isnull
+00000d60: 7a0e 7b7d 5f5f 6e6f 745f 6973 6e75 6c6c  z.{}__not_isnull
+00000d70: 7a07 7b7d 5f5f 6774 657a 077b 7d5f 5f6c  z.{}__gtez.{}__l
+00000d80: 7465 7a06 7b7d 5f5f 6774 7a06 7b7d 5f5f  tez.{}__gtz.{}__
+00000d90: 6c74 7a0c 7b7d 5f5f 636f 6e74 6169 6e73  ltz.{}__contains
+00000da0: 7a0e 7b7d 5f5f 7374 6172 7473 7769 7468  z.{}__startswith
+00000db0: 7a0c 7b7d 5f5f 656e 6473 7769 7468 7a0d  z.{}__endswithz.
+00000dc0: 7b7d 5f5f 6963 6f6e 7461 696e 737a 0f7b  {}__icontainsz.{
+00000dd0: 7d5f 5f69 7374 6172 7473 7769 7468 7a0d  }__istartswithz.
+00000de0: 7b7d 5f5f 6965 6e64 7377 6974 6829 17da  {}__iendswith)..
+00000df0: 0a69 7369 6e73 7461 6e63 6572 0500 0000  .isinstancer....
+00000e00: da0f 4d61 6e79 546f 4d61 6e79 4669 656c  ..ManyToManyFiel
+00000e10: 6472 2f00 0000 7226 0000 0072 2a00 0000  dr/...r&...r*...
+00000e20: 721d 0000 0072 1600 0000 7211 0000 0072  r....r....r....r
+00000e30: 2c00 0000 7214 0000 0072 1800 0000 7219  ,...r....r....r.
+00000e40: 0000 00da 0267 65da 026c 65da 0267 74da  .....ge..le..gt.
+00000e50: 026c 7472 1e00 0000 721f 0000 0072 2000  .ltr....r....r .
+00000e60: 0000 7222 0000 0072 2300 0000 7224 0000  ..r"...r#...r$..
+00000e70: 0029 0472 2d00 0000 720d 0000 0072 3500  .).r-...r....r5.
+00000e80: 0000 722e 0000 0072 0f00 0000 720f 0000  ..r....r....r...
+00000e90: 0072 1000 0000 da15 6765 745f 6669 6c74  .r......get_filt
+00000ea0: 6572 735f 666f 725f 6669 656c 6485 0000  ers_for_field...
+00000eb0: 0073 6a00 0000 0001 0c01 0a02 0201 0201  .sj.............
+00000ec0: 0802 0801 0201 0602 0801 0201 0201 0602  ................
+00000ed0: 0801 0201 0201 0602 0801 0201 0602 0801  ................
+00000ee0: 0201 0602 0801 0201 0802 0801 0201 0802  ................
+00000ef0: 0801 0201 0802 0801 0201 0802 0801 0201  ................
+00000f00: 0602 0801 0201 0602 0801 0201 0602 0801  ................
+00000f10: 0201 0602 0801 0201 0602 0801 0201 0a03  ................
+00000f20: 723c 0000 0063 0000 0000 0000 0000 0000  r<...c..........
+00000f30: 0000 0300 0000 4000 0000 7320 0000 0065  ......@...s ...e
+00000f40: 005a 0164 005a 0264 0164 0284 005a 0365  .Z.d.Z.d.d...Z.e
+00000f50: 0464 0364 0484 0083 015a 0564 0553 0029  .d.d.....Z.d.S.)
+00000f60: 06da 084d 6574 6149 6e66 6f63 0200 0000  ...MetaInfoc....
+00000f70: 0000 0000 0200 0000 0400 0000 4300 0000  ............C...
+00000f80: 737c 0000 0074 007c 0164 0164 0283 037c  s|...t.|.d.d...|
+00000f90: 005f 0174 007c 0164 0364 0083 037c 005f  ._.t.|.d.d...|._
+00000fa0: 0274 007c 0164 0464 0083 037c 005f 0374  .t.|.d.d...|._.t
+00000fb0: 0483 007c 005f 0574 0483 007c 005f 0674  ...|._.t...|._.t
+00000fc0: 0483 007c 005f 0774 0483 007c 005f 0874  ...|._.t...|._.t
+00000fd0: 0483 007c 005f 0974 0483 007c 005f 0a69  ...|._.t...|._.i
+00000fe0: 007c 005f 0b69 007c 005f 0c69 007c 005f  .|._.i.|._.i.|._
+00000ff0: 0d69 007c 005f 0e64 007c 005f 0f64 0053  .i.|._.d.|._.d.S
+00001000: 0029 054e da08 6162 7374 7261 6374 4672  .).N..abstractFr
+00001010: 2700 0000 da03 6170 7029 10da 0767 6574  '.....app)...get
+00001020: 6174 7472 723e 0000 0072 2700 0000 723f  attrr>...r'...r?
+00001030: 0000 00da 0373 6574 7205 0000 00da 0964  .....setr......d
+00001040: 625f 6669 656c 6473 da0a 6d32 6d5f 6669  b_fields..m2m_fi
+00001050: 656c 6473 da09 666b 5f66 6965 6c64 73da  elds..fk_fields.
+00001060: 1262 6163 6b77 6172 645f 666b 5f66 6965  .backward_fk_fie
+00001070: 6c64 73da 0c66 6574 6368 5f66 6965 6c64  lds..fetch_field
+00001080: 73da 1466 6965 6c64 735f 6462 5f70 726f  s..fields_db_pro
+00001090: 6a65 6374 696f 6eda 1c66 6965 6c64 735f  jection..fields_
+000010a0: 6462 5f70 726f 6a65 6374 696f 6e5f 7265  db_projection_re
+000010b0: 7665 7273 6572 2e00 0000 da0a 6669 656c  verser......fiel
+000010c0: 6473 5f6d 6170 da0a 6465 6661 756c 745f  ds_map..default_
+000010d0: 6462 2902 da04 7365 6c66 da04 6d65 7461  db)...self..meta
+000010e0: 720f 0000 0072 0f00 0000 7210 0000 00da  r....r....r.....
+000010f0: 085f 5f69 6e69 745f 5fd0 0000 0073 1c00  .__init__....s..
+00001100: 0000 0001 0e01 0e01 0e01 0801 0801 0801  ................
+00001110: 0801 0801 0801 0601 0601 0601 0601 7a11  ..............z.
+00001120: 4d65 7461 496e 666f 2e5f 5f69 6e69 745f  MetaInfo.__init_
+00001130: 5f63 0100 0000 0000 0000 0100 0000 0100  _c..............
+00001140: 0000 4300 0000 730e 0000 0074 006a 0183  ..C...s....t.j..
+00001150: 0070 0c7c 006a 0253 0029 014e 2903 7206  .p.|.j.S.).N).r.
+00001160: 0000 00da 0367 6574 724a 0000 0029 0172  .....getrJ...).r
+00001170: 4b00 0000 720f 0000 0072 0f00 0000 7210  K...r....r....r.
+00001180: 0000 00da 0264 62e0 0000 0073 0200 0000  .....db....s....
+00001190: 0002 7a0b 4d65 7461 496e 666f 2e64 624e  ..z.MetaInfo.dbN
+000011a0: 2906 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
+000011b0: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
+000011c0: 6e61 6d65 5f5f 724d 0000 00da 0870 726f  name__rM.....pro
+000011d0: 7065 7274 7972 4f00 0000 720f 0000 0072  pertyrO...r....r
+000011e0: 0f00 0000 720f 0000 0072 1000 0000 723d  ....r....r....r=
+000011f0: 0000 00cf 0000 0073 0400 0000 0801 0810  .......s........
+00001200: 723d 0000 0063 0000 0000 0000 0000 0000  r=...c..........
+00001210: 0000 0300 0000 0000 0000 731c 0000 0065  ..........s....e
+00001220: 005a 0164 005a 0287 0066 0164 0164 0284  .Z.d.Z...f.d.d..
+00001230: 085a 0387 0004 005a 0453 0029 03da 094d  .Z.....Z.S.)...M
+00001240: 6f64 656c 4d65 7461 6304 0000 0000 0000  odelMetac.......
+00001250: 0010 0000 0007 0000 000f 0000 0073 a601  .............s..
+00001260: 0000 6900 7d06 6900 7d07 6900 7d08 7400  ..i.}.i.}.i.}.t.
+00001270: 8300 7d09 7400 8300 7d0a 7401 7c03 6a02  ..}.t...}.t.|.j.
+00001280: 6401 8301 8301 7d0b 78d0 7c03 6a03 8300  d.....}.x.|.j...
+00001290: 4400 5dc4 5c02 7d0c 7d0d 7404 7c0d 7405  D.].\.}.}.t.|.t.
+000012a0: 6a06 8302 7230 7c0d 7c07 7c0c 3c00 7404  j...r0|.|.|.<.t.
+000012b0: 7c0d 7405 6a07 8302 72ac 6402 6a08 7c0c  |.t.j...r.d.j.|.
+000012c0: 8301 7d0e 7c0e 7c0d 5f09 7c0e 7c06 7c0e  ..}.|.|._.|.|.|.
+000012d0: 3c00 7405 6a0a 7c0d 7c0d 6a0b 7c0d 6a0c  <.t.j.|.|.j.|.j.
+000012e0: 6403 8d03 7c07 7c0e 3c00 7c08 6a0d 740e  d...|.|.<.|.j.t.
+000012f0: 7c0e 7c07 7c0e 1900 7c0e 6404 8d03 8301  |.|.|...|.d.....
+00001300: 0100 7c09 6a0f 7c0c 8301 0100 7130 7404  ..|.j.|.....q0t.
+00001310: 7c0d 7405 6a10 8302 72c4 7c0a 6a0f 7c0c  |.t.j...r.|.j.|.
+00001320: 8301 0100 7130 7c0d 6a09 72d0 7c0d 6a09  ....q0|.j.r.|.j.
+00001330: 6e02 7c0c 7c06 7c0c 3c00 7c08 6a0d 740e  n.|.|.|.<.|.j.t.
+00001340: 7c0c 7c07 7c0c 1900 7c06 7c0c 1900 6404  |.|.|...|.|...d.
+00001350: 8d03 8301 0100 7130 5700 7411 8300 6a12  ......q0W.t...j.
+00001360: 7c00 7c01 7c02 7c03 8304 7d0f 7c0b 7c0f  |.|.|.|...}.|.|.
+00001370: 5f13 7c07 7c0f 6a13 5f14 7c06 7c0f 6a13  _.|.|.j._.|.|.j.
+00001380: 5f15 6405 6406 8400 7c06 6a03 8300 4400  _.d.d...|.j...D.
+00001390: 8301 7c0f 6a13 5f16 7400 7c07 6a17 8300  ..|.j._.t.|.j...
+000013a0: 8301 7c0f 6a13 5f05 7400 7c06 6a18 8300  ..|.j._.t.|.j...
+000013b0: 8301 7c0f 6a13 5f19 7c08 7c0f 6a13 5f1a  ..|.j._.|.|.j._.
+000013c0: 7c09 7c0f 6a13 5f1b 7400 8300 7c0f 6a13  |.|.j._.t...|.j.
+000013d0: 5f1c 7c0a 7c0f 6a13 5f1d 7c09 7c0a 4200  _.|.|.j._.|.|.B.
+000013e0: 7c0f 6a13 5f1e 6400 7c0f 6a13 5f1f 6407  |.j._.d.|.j._.d.
+000013f0: 7c0f 6a13 5f20 7c07 9001 73a2 6408 7c0f  |.j._ |...s.d.|.
+00001400: 6a13 5f21 7c0f 5300 2909 4eda 044d 6574  j._!|.S.).N..Met
+00001410: 617a 057b 7d5f 6964 2903 da09 7265 6665  az.{}_id)...refe
+00001420: 7265 6e63 65da 046e 756c 6cda 0764 6566  rence..null..def
+00001430: 6175 6c74 2903 722d 0000 0072 0d00 0000  ault).r-...r....
+00001440: 7235 0000 0063 0100 0000 0000 0000 0300  r5...c..........
+00001450: 0000 0400 0000 5300 0000 7316 0000 0069  ......S...s....i
+00001460: 007c 005d 0e5c 027d 017d 027c 017c 0293  .|.].\.}.}.|.|..
+00001470: 0271 0453 0072 0f00 0000 720f 0000 0029  .q.S.r....r....)
+00001480: 03da 022e 30da 036b 6579 720e 0000 0072  ....0..keyr....r
+00001490: 0f00 0000 720f 0000 0072 1000 0000 fa0a  ....r....r......
+000014a0: 3c64 6963 7463 6f6d 703e 1201 0000 7302  <dictcomp>....s.
+000014b0: 0000 0006 027a 254d 6f64 656c 4d65 7461  .....z%ModelMeta
+000014c0: 2e5f 5f6e 6577 5f5f 2e3c 6c6f 6361 6c73  .__new__.<locals
+000014d0: 3e2e 3c64 6963 7463 6f6d 703e 4654 2922  >.<dictcomp>FT)"
+000014e0: 7241 0000 0072 3d00 0000 724e 0000 00da  rA...r=...rN....
+000014f0: 0569 7465 6d73 7236 0000 0072 0500 0000  .itemsr6...r....
+00001500: da05 4669 656c 64da 0f46 6f72 6569 676e  ..Field..Foreign
+00001510: 4b65 7946 6965 6c64 721d 0000 0072 3500  KeyFieldr....r5.
+00001520: 0000 da08 496e 7446 6965 6c64 7257 0000  ....IntFieldrW..
+00001530: 0072 5800 0000 da06 7570 6461 7465 723c  .rX.....updater<
+00001540: 0000 00da 0361 6464 7237 0000 00da 0573  .....addr7.....s
+00001550: 7570 6572 da07 5f5f 6e65 775f 5f72 3300  uper..__new__r3.
+00001560: 0000 7249 0000 0072 4700 0000 7248 0000  ..rI...rG...rH..
+00001570: 00da 046b 6579 73da 0676 616c 7565 7372  ...keys..valuesr
+00001580: 4200 0000 722e 0000 0072 4400 0000 7245  B...r....rD...rE
+00001590: 0000 0072 4300 0000 7246 0000 0072 4a00  ...rC...rF...rJ.
+000015a0: 0000 da07 5f69 6e69 7465 6472 3e00 0000  ...._initedr>...
+000015b0: 2910 5a03 6d63 73da 046e 616d 65da 0562  ).Z.mcs..name..b
+000015c0: 6173 6573 da05 6174 7472 73da 0461 7267  ases..attrs..arg
+000015d0: 73da 066b 7761 7267 7372 4700 0000 7249  s..kwargsrG...rI
+000015e0: 0000 0072 2e00 0000 7244 0000 0072 4300  ...r....rD...rC.
+000015f0: 0000 724c 0000 0072 5a00 0000 720e 0000  ..rL...rZ...r...
+00001600: 005a 096b 6579 5f66 6965 6c64 da09 6e65  .Z.key_field..ne
+00001610: 775f 636c 6173 7329 01da 095f 5f63 6c61  w_class)...__cla
+00001620: 7373 5f5f 720f 0000 0072 1000 0000 7263  ss__r....r....rc
+00001630: 0000 00e6 0000 0073 6200 0000 0001 0401  .......sb.......
+00001640: 0401 0401 0601 0601 0e02 1201 0c01 0801  ................
+00001650: 0c01 0a01 0601 0801 0401 0201 0401 0e02  ................
+00001660: 0401 0201 0201 0601 0a03 0c01 0c01 0c02  ................
+00001670: 1401 0401 0201 0201 0601 1203 1202 0601  ................
+00001680: 0801 0801 0602 1002 1001 1001 0801 0801  ................
+00001690: 0a01 0801 0c01 0801 0801 0601 0801 7a11  ..............z.
+000016a0: 4d6f 6465 6c4d 6574 612e 5f5f 6e65 775f  ModelMeta.__new_
+000016b0: 5f29 0572 5000 0000 7251 0000 0072 5200  _).rP...rQ...rR.
+000016c0: 0000 7263 0000 00da 0d5f 5f63 6c61 7373  ..rc.....__class
+000016d0: 6365 6c6c 5f5f 720f 0000 0072 0f00 0000  cell__r....r....
+000016e0: 2901 726d 0000 0072 1000 0000 7254 0000  ).rm...r....rT..
+000016f0: 00e5 0000 0073 0200 0000 0801 7254 0000  .....s......rT..
+00001700: 0063 0000 0000 0000 0000 0000 0000 0400  .c..............
+00001710: 0000 4000 0000 73d2 0000 0065 005a 0164  ..@...s....e.Z.d
+00001720: 005a 0264 0164 0284 005a 0364 2764 0464  .Z.d.d...Z.d'd.d
+00001730: 0584 015a 0464 2864 0664 0784 015a 0564  ...Z.d(d.d...Z.d
+00001740: 0864 0984 005a 0664 2964 0a64 0b84 015a  .d...Z.d)d.d...Z
+00001750: 0764 0364 0c9c 0164 0d64 0e84 025a 0864  .d.d...d.d...Z.d
+00001760: 0f64 1084 005a 0964 1164 1284 005a 0a64  .d...Z.d.d...Z.d
+00001770: 1364 1484 005a 0b64 1564 1684 005a 0c65  .d...Z.d.d...Z.e
+00001780: 0d64 2a64 1764 1884 0183 015a 0e65 0d64  .d*d.d.....Z.e.d
+00001790: 1964 1a84 0083 015a 0f65 0d64 1b64 1c84  .d.....Z.e.d.d..
+000017a0: 0083 015a 1065 0d64 1d64 1e84 0083 015a  ...Z.e.d.d.....Z
+000017b0: 1165 0d64 1f64 2084 0083 015a 1265 0d64  .e.d.d ....Z.e.d
+000017c0: 2164 2284 0083 015a 1365 0d64 0364 0c9c  !d"....Z.e.d.d..
+000017d0: 0164 2364 2484 0283 015a 1447 0064 2564  .d#d$....Z.G.d%d
+000017e0: 2684 0064 2683 025a 1564 0353 0029 2bda  &..d&..Z.d.S.)+.
+000017f0: 054d 6f64 656c 6301 0000 0000 0000 000a  .Modelc.........
+00001800: 0000 0009 0000 004f 0000 0073 2202 0000  .......O...s"...
+00001810: 7400 7c02 6a01 6401 8301 8301 0c00 7d03  t.|.j.d.......}.
+00001820: 788e 7c00 6a02 6a03 6a04 8300 4400 5d7e  x.|.j.j.j...D.]~
+00001830: 5c02 7d04 7d05 7405 7c05 7406 6a07 8302  \.}.}.t.|.t.j...
+00001840: 724e 7408 7c00 7c04 7409 7c05 6a0a 7c05  rNt.|.|.t.|.j.|.
+00001850: 6a0b 7c00 7c03 8304 8303 0100 711e 7405  j.|.|.......q.t.
+00001860: 7c05 7406 6a0c 8302 7274 7408 7c00 7c04  |.t.j...rtt.|.|.
+00001870: 740d 7c05 6a0a 7c00 7c05 7c03 8304 8303  t.|.j.|.|.|.....
+00001880: 0100 711e 7405 7c05 7406 6a0e 8302 7290  ..q.t.|.t.j...r.
+00001890: 7408 7c00 7c04 7c05 6a0f 8303 0100 711e  t.|.|.|.j.....q.
+000018a0: 7408 7c00 7c04 6400 8303 0100 711e 5700  t.|.|.d.....q.W.
+000018b0: 7410 7c02 6a11 8300 8301 7d06 9001 7808  t.|.j.....}...x.
+000018c0: 7c02 6a04 8300 4400 5dfc 5c02 7d04 7d07  |.j...D.].\.}.}.
+000018d0: 7c04 7c00 6a02 6a12 6b06 9001 7212 7413  |.|.j.j.k...r.t.
+000018e0: 7c07 6401 8302 72ee 7c07 6a14 0c00 72ee  |.d...r.|.j...r.
+000018f0: 7415 6402 6a16 7c07 8301 8301 8201 6403  t.d.j.|.......d.
+00001900: 6a16 7c04 8301 7d08 7408 7c00 7c08 7c07  j.|...}.t.|.|.|.
+00001910: 6a14 8303 0100 7c06 6a17 7c08 8301 0100  j.....|.j.|.....
+00001920: 71b8 7c04 7c00 6a02 6a18 6b06 9001 722a  q.|.|.j.j.k...r*
+00001930: 7419 6404 8301 8201 71b8 7c04 7c00 6a02  t.d.....q.|.|.j.
+00001940: 6a1a 6b06 9001 7242 7419 6405 8301 8201  j.k...rBt.d.....
+00001950: 71b8 7c04 7c00 6a02 6a06 6b06 9001 7292  q.|.|.j.j.k...r.
+00001960: 7c00 6a02 6a03 7c04 1900 7d09 7c07 6400  |.j.j.|...}.|.d.
+00001970: 6b08 9001 727e 7c09 6a1b 0c00 9001 727e  k...r~|.j.....r~
+00001980: 741c 6406 6a16 7c04 8301 8301 8201 7408  t.d.j.|.......t.
+00001990: 7c00 7c04 7c09 6a1d 7c07 8301 8303 0100  |.|.|.j.|.......
+000019a0: 71b8 7c04 7c00 6a02 6a1e 6b06 72b8 7408  q.|.|.j.j.k.r.t.
+000019b0: 7c00 7c00 6a02 6a1f 6a01 7c04 8301 7c07  |.|.j.j.j.|...|.
+000019c0: 8303 0100 71b8 5700 7864 7c00 6a02 6a03  ....q.W.xd|.j.j.
+000019d0: 6a04 8300 4400 5d54 5c02 7d04 7d09 7c04  j...D.]T\.}.}.|.
+000019e0: 7c06 6b06 9001 73c6 7c04 7c00 6a02 6a20  |.k...s.|.|.j.j 
+000019f0: 6b06 9001 72ec 9001 71c6 6e2c 7421 7c09  k...r...q.n,t!|.
+00001a00: 6a0f 8301 9002 720a 7408 7c00 7c04 7c09  j.....r.t.|.|.|.
+00001a10: 6a0f 8300 8303 0100 6e0e 7408 7c00 7c04  j.......n.t.|.|.
+00001a20: 7c09 6a0f 8303 0100 9001 71c6 5700 6400  |.j.......q.W.d.
+00001a30: 5300 2907 4e72 3000 0000 7a3a 596f 7520  S.).Nr0...z:You 
+00001a40: 7368 6f75 6c64 2066 6972 7374 2063 616c  should first cal
+00001a50: 6c20 2e73 6176 6528 2920 6f6e 207b 7d20  l .save() on {} 
+00001a60: 6265 666f 7265 2072 6566 6572 7269 6e67  before referring
+00001a70: 2074 6f20 6974 7a05 7b7d 5f69 647a 4b59   to itz.{}_idzKY
+00001a80: 6f75 2063 616e 2774 2073 6574 2062 6163  ou can't set bac
+00001a90: 6b77 6172 6420 7265 6c61 7469 6f6e 7320  kward relations 
+00001aa0: 7468 726f 7567 6820 696e 6974 2c20 6368  through init, ch
+00001ab0: 616e 6765 2072 656c 6174 6564 206d 6f64  ange related mod
+00001ac0: 656c 2069 6e73 7465 6164 7a41 596f 7520  el insteadzAYou 
+00001ad0: 6361 6e27 7420 7365 7420 6d32 6d20 7265  can't set m2m re
+00001ae0: 6c61 7469 6f6e 7320 7468 726f 7567 6820  lations through 
+00001af0: 696e 6974 2c20 7573 6520 6d32 6d5f 6d61  init, use m2m_ma
+00001b00: 6e61 6765 7220 696e 7374 6561 647a 2d7b  nager insteadz-{
+00001b10: 7d20 6973 206e 6f6e 206e 756c 6c61 626c  } is non nullabl
+00001b20: 6520 6669 656c 642c 2062 7574 206e 756c  e field, but nul
+00001b30: 6c20 7761 7320 7061 7373 6564 2922 da04  l was passed)"..
+00001b40: 626f 6f6c 724e 0000 0072 3300 0000 7249  boolrN...r3...rI
+00001b50: 0000 0072 5c00 0000 7236 0000 0072 0500  ...r\...r6...r..
+00001b60: 0000 da12 4261 636b 7761 7264 464b 5265  ....BackwardFKRe
+00001b70: 6c61 7469 6f6e da07 7365 7461 7474 7272  lation..setattrr
+00001b80: 0a00 0000 7232 0000 0072 3100 0000 7237  ....r2...r1...r7
+00001b90: 0000 0072 0900 0000 725d 0000 0072 5800  ...r....r]...rX.
+00001ba0: 0000 7241 0000 0072 6400 0000 7244 0000  ..rA...rd...rD..
+00001bb0: 00da 0768 6173 6174 7472 7230 0000 0072  ...hasattrr0...r
+00001bc0: 0800 0000 721d 0000 0072 6100 0000 7245  ....r....ra...rE
+00001bd0: 0000 0072 0700 0000 7243 0000 0072 5700  ...r....rC...rW.
+00001be0: 0000 da0a 5661 6c75 6545 7272 6f72 da0f  ....ValueError..
+00001bf0: 746f 5f70 7974 686f 6e5f 7661 6c75 6572  to_python_valuer
+00001c00: 4200 0000 7248 0000 0072 4600 0000 da08  B...rH...rF.....
+00001c10: 6361 6c6c 6162 6c65 290a 724b 0000 0072  callable).rK...r
+00001c20: 6a00 0000 726b 0000 00da 0669 735f 6e65  j...rk.....is_ne
+00001c30: 7772 5a00 0000 720d 0000 005a 0d70 6173  wrZ...r....Z.pas
+00001c40: 7365 645f 6669 656c 6473 720e 0000 0072  sed_fieldsr....r
+00001c50: 3100 0000 da0c 6669 656c 645f 6f62 6a65  1.....field_obje
+00001c60: 6374 720f 0000 0072 0f00 0000 7210 0000  ctr....r....r...
+00001c70: 0072 4d00 0000 2501 0000 734e 0000 0000  .rM...%...sN....
+00001c80: 0110 0216 010c 0102 0104 0116 020c 011a  ................
+00001c90: 010c 0110 0210 020c 0114 010e 0112 0102  ................
+00001ca0: 010c 010a 010e 010c 010e 0102 0108 020e  ................
+00001cb0: 0102 0108 020e 010c 0114 010e 0114 010c  ................
+00001cc0: 011a 0216 0118 0106 020c 0112 027a 0e4d  .............z.M
+00001cd0: 6f64 656c 2e5f 5f69 6e69 745f 5f4e 6302  odel.__init__Nc.
+00001ce0: 0000 0000 0000 0003 0000 0004 0000 00c3  ................
+00001cf0: 0000 0073 3000 0000 7c01 7208 7c01 6e06  ...s0...|.r.|.n.
+00001d00: 7c00 6a00 6a01 7d02 7c02 6a02 7c00 6a03  |.j.j.}.|.j.|.j.
+00001d10: 7c02 6401 8d02 6a04 7c00 8301 4900 6400  |.d...j.|...I.d.
+00001d20: 4800 0100 6400 5300 2902 4e29 02da 056d  H...d.S.).N)...m
+00001d30: 6f64 656c 724f 0000 0029 0572 3300 0000  odelrO...).r3...
+00001d40: 724f 0000 00da 0e65 7865 6375 746f 725f  rO.....executor_
+00001d50: 636c 6173 7372 6d00 0000 da0e 6578 6563  classrm.....exec
+00001d60: 7574 655f 696e 7365 7274 2903 724b 0000  ute_insert).rK..
+00001d70: 00da 0875 7369 6e67 5f64 6272 4f00 0000  ...using_dbrO...
+00001d80: 720f 0000 0072 0f00 0000 7210 0000 00da  r....r....r.....
+00001d90: 105f 696e 7365 7274 5f69 6e73 7461 6e63  ._insert_instanc
+00001da0: 6557 0100 0073 0a00 0000 0001 1001 0401  eW...s..........
+00001db0: 0401 0801 7a16 4d6f 6465 6c2e 5f69 6e73  ....z.Model._ins
+00001dc0: 6572 745f 696e 7374 616e 6365 6302 0000  ert_instancec...
+00001dd0: 0000 0000 0003 0000 0004 0000 00c3 0000  ................
+00001de0: 0073 3000 0000 7c01 7208 7c01 6e06 7c00  .s0...|.r.|.n.|.
+00001df0: 6a00 6a01 7d02 7c02 6a02 7c00 6a03 7c02  j.j.}.|.j.|.j.|.
+00001e00: 6401 8d02 6a04 7c00 8301 4900 6400 4800  d...j.|...I.d.H.
+00001e10: 0100 6400 5300 2902 4e29 0272 7900 0000  ..d.S.).N).ry...
+00001e20: 724f 0000 0029 0572 3300 0000 724f 0000  rO...).r3...rO..
+00001e30: 0072 7a00 0000 726d 0000 00da 0e65 7865  .rz...rm.....exe
+00001e40: 6375 7465 5f75 7064 6174 6529 0372 4b00  cute_update).rK.
+00001e50: 0000 727c 0000 0072 4f00 0000 720f 0000  ..r|...rO...r...
+00001e60: 0072 0f00 0000 7210 0000 00da 105f 7570  .r....r......_up
+00001e70: 6461 7465 5f69 6e73 7461 6e63 655e 0100  date_instance^..
+00001e80: 0073 0a00 0000 0001 1001 0401 0401 0801  .s..............
+00001e90: 7a16 4d6f 6465 6c2e 5f75 7064 6174 655f  z.Model._update_
+00001ea0: 696e 7374 616e 6365 6301 0000 0000 0000  instancec.......
+00001eb0: 0003 0000 0003 0000 00cf 0000 0073 3000  .............s0.
+00001ec0: 0000 7c00 6a00 731a 7c00 6a01 7c01 7c02  ..|.j.s.|.j.|.|.
+00001ed0: 8e01 4900 6400 4800 0100 6e12 7c00 6a02  ..I.d.H...n.|.j.
+00001ee0: 7c01 7c02 8e01 4900 6400 4800 0100 6400  |.|...I.d.H...d.
+00001ef0: 5300 2901 4e29 0372 3000 0000 727d 0000  S.).N).r0...r}..
+00001f00: 0072 7f00 0000 2903 724b 0000 0072 6a00  .r....).rK...rj.
+00001f10: 0000 726b 0000 0072 0f00 0000 720f 0000  ..rk...r....r...
+00001f20: 0072 1000 0000 da04 7361 7665 6501 0000  .r......savee...
+00001f30: 7306 0000 0000 0106 0114 027a 0a4d 6f64  s..........z.Mod
+00001f40: 656c 2e73 6176 6563 0200 0000 0000 0000  el.savec........
+00001f50: 0300 0000 0400 0000 c300 0000 733a 0000  ............s:..
+00001f60: 007c 0172 087c 016e 067c 006a 006a 017d  .|.r.|.n.|.j.j.}
+00001f70: 027c 006a 0273 1a64 0053 007c 026a 037c  .|.j.s.d.S.|.j.|
+00001f80: 006a 047c 0264 018d 026a 057c 0083 0149  .j.|.d...j.|...I
+00001f90: 0064 0048 0001 0064 0053 0029 024e 2902  .d.H...d.S.).N).
+00001fa0: 7279 0000 0072 4f00 0000 2906 7233 0000  ry...rO...).r3..
+00001fb0: 0072 4f00 0000 7230 0000 0072 7a00 0000  .rO...r0...rz...
+00001fc0: 726d 0000 00da 0e65 7865 6375 7465 5f64  rm.....execute_d
+00001fd0: 656c 6574 6529 0372 4b00 0000 727c 0000  elete).rK...r|..
+00001fe0: 0072 4f00 0000 720f 0000 0072 0f00 0000  .rO...r....r....
+00001ff0: 7210 0000 00da 0664 656c 6574 656b 0100  r......deletek..
+00002000: 0073 0e00 0000 0001 1001 0601 0401 0401  .s..............
+00002010: 0401 0801 7a0c 4d6f 6465 6c2e 6465 6c65  ....z.Model.dele
+00002020: 7465 2901 727c 0000 0063 0100 0000 0100  te).r|...c......
+00002030: 0000 0400 0000 0400 0000 c700 0000 7338  ..............s8
+00002040: 0000 007c 0172 087c 016e 067c 006a 006a  ...|.r.|.n.|.j.j
+00002050: 017d 037c 036a 027c 006a 037c 0364 018d  .}.|.j.|.j.|.d..
+00002060: 026a 047c 0067 0166 017c 029e 028e 0049  .j.|.g.f.|.....I
+00002070: 0064 0048 0001 0064 0053 0029 024e 2902  .d.H...d.S.).N).
+00002080: 7279 0000 0072 4f00 0000 2905 7233 0000  ry...rO...).r3..
+00002090: 0072 4f00 0000 727a 0000 0072 6d00 0000  .rO...rz...rm...
+000020a0: da0e 6665 7463 685f 666f 725f 6c69 7374  ..fetch_for_list
+000020b0: 2904 724b 0000 0072 7c00 0000 726a 0000  ).rK...r|...rj..
+000020c0: 0072 4f00 0000 720f 0000 0072 0f00 0000  .rO...r....r....
+000020d0: 7210 0000 00da 0d66 6574 6368 5f72 656c  r......fetch_rel
+000020e0: 6174 6564 7401 0000 730a 0000 0000 0110  atedt...s.......
+000020f0: 0104 0104 0108 017a 134d 6f64 656c 2e66  .......z.Model.f
+00002100: 6574 6368 5f72 656c 6174 6564 6301 0000  etch_relatedc...
+00002110: 0000 0000 0001 0000 0001 0000 0043 0000  .............C..
+00002120: 0073 0800 0000 7c00 6a00 6a01 5300 2901  .s....|.j.j.S.).
+00002130: 4e29 0272 6d00 0000 7250 0000 0029 0172  N).rm...rP...).r
+00002140: 4b00 0000 720f 0000 0072 0f00 0000 7210  K...r....r....r.
+00002150: 0000 00da 075f 5f73 7472 5f5f 7b01 0000  .....__str__{...
+00002160: 7302 0000 0000 017a 0d4d 6f64 656c 2e5f  s......z.Model._
+00002170: 5f73 7472 5f5f 6301 0000 0000 0000 0001  _str__c.........
+00002180: 0000 0003 0000 0043 0000 0073 1400 0000  .......C...s....
+00002190: 6401 6a00 7c00 6a01 6a02 7c00 6a03 8300  d.j.|.j.j.|.j...
+000021a0: 8302 5300 2902 4e7a 083c 7b7d 3a20 7b7d  ..S.).Nz.<{}: {}
+000021b0: 3e29 0472 1d00 0000 726d 0000 0072 5000  >).r....rm...rP.
+000021c0: 0000 7285 0000 0029 0172 4b00 0000 720f  ..r....).rK...r.
+000021d0: 0000 0072 0f00 0000 7210 0000 00da 085f  ...r....r......_
+000021e0: 5f72 6570 725f 5f7e 0100 0073 0200 0000  _repr__~...s....
+000021f0: 0001 7a0e 4d6f 6465 6c2e 5f5f 7265 7072  ..z.Model.__repr
+00002200: 5f5f 6301 0000 0000 0000 0001 0000 0002  __c.............
+00002210: 0000 0043 0000 0073 2600 0000 7400 7c00  ...C...s&...t.|.
+00002220: 6a01 8301 0c00 7314 7c00 6a01 0c00 721c  j.....s.|.j...r.
+00002230: 7402 6401 8301 8201 7403 7c00 6a01 8301  t.d.....t.|.j...
+00002240: 5300 2902 4e7a 294d 6f64 656c 2069 6e73  S.).Nz)Model ins
+00002250: 7461 6e63 6573 2077 6974 686f 7574 2069  tances without i
+00002260: 6420 6172 6520 756e 6861 7368 6162 6c65  d are unhashable
+00002270: 2904 7273 0000 0072 3000 0000 da09 5479  ).rs...r0.....Ty
+00002280: 7065 4572 726f 72da 0468 6173 6829 0172  peError..hash).r
+00002290: 4b00 0000 720f 0000 0072 0f00 0000 7210  K...r....r....r.
+000022a0: 0000 00da 085f 5f68 6173 685f 5f81 0100  .....__hash__...
+000022b0: 0073 0600 0000 0001 1401 0801 7a0e 4d6f  .s..........z.Mo
+000022c0: 6465 6c2e 5f5f 6861 7368 5f5f 6302 0000  del.__hash__c...
+000022d0: 0000 0000 0002 0000 0003 0000 0043 0000  .............C..
+000022e0: 0073 2400 0000 7400 7c00 8301 7400 7c01  .s$...t.|...t.|.
+000022f0: 8301 6b02 7220 7c00 6a01 7c01 6a01 6b02  ..k.r |.j.|.j.k.
+00002300: 7220 6401 5300 6402 5300 2903 4e54 4629  r d.S.d.S.).NTF)
+00002310: 0272 3200 0000 7230 0000 0029 0272 4b00  .r2...r0...).rK.
+00002320: 0000 da05 6f74 6865 7272 0f00 0000 720f  ....otherr....r.
+00002330: 0000 0072 1000 0000 da06 5f5f 6571 5f5f  ...r......__eq__
+00002340: 8601 0000 7306 0000 0000 021c 0104 017a  ....s..........z
+00002350: 0c4d 6f64 656c 2e5f 5f65 715f 5f63 0300  .Model.__eq__c..
+00002360: 0000 0000 0000 0500 0000 0400 0000 cb00  ................
+00002370: 0000 734a 0000 007c 0273 0869 007d 027c  ..sJ...|.s.i.}.|
+00002380: 006a 0066 007c 038e 016a 0183 0049 0064  .j.f.|...j...I.d
+00002390: 0048 007d 047c 0472 2a7c 0464 0166 0253  .H.}.|.r*|.d.f.S
+000023a0: 007c 0066 007c 027c 0397 028e 016a 027c  .|.f.|.|.....j.|
+000023b0: 0164 028d 0149 0064 0048 0064 0366 0253  .d...I.d.H.d.f.S
+000023c0: 0029 044e 4629 0172 7c00 0000 5429 03da  .).NF).r|...T)..
+000023d0: 0666 696c 7465 72da 0566 6972 7374 7280  .filter..firstr.
+000023e0: 0000 0029 05da 0363 6c73 727c 0000 00da  ...)...clsr|....
+000023f0: 0864 6566 6175 6c74 7372 6b00 0000 da08  .defaultsrk.....
+00002400: 696e 7374 616e 6365 720f 0000 0072 0f00  instancer....r..
+00002410: 0000 7210 0000 00da 0d67 6574 5f6f 725f  ..r......get_or_
+00002420: 6372 6561 7465 8c01 0000 730c 0000 0000  create....s.....
+00002430: 0204 0104 0116 0104 0108 017a 134d 6f64  ...........z.Mod
+00002440: 656c 2e67 6574 5f6f 725f 6372 6561 7465  el.get_or_create
+00002450: 6301 0000 0000 0000 0003 0000 0003 0000  c...............
+00002460: 00cb 0000 0073 2400 0000 7c00 6600 7c01  .....s$...|.f.|.
+00002470: 8e01 7d02 7c02 6a00 7c01 6a01 6401 8301  ..}.|.j.|.j.d...
+00002480: 8301 4900 6400 4800 0100 7c02 5300 2902  ..I.d.H...|.S.).
+00002490: 4e72 7c00 0000 2902 7280 0000 0072 4e00  Nr|...).r....rN.
+000024a0: 0000 2903 728e 0000 0072 6b00 0000 7290  ..).r....rk...r.
+000024b0: 0000 0072 0f00 0000 720f 0000 0072 1000  ...r....r....r..
+000024c0: 0000 da06 6372 6561 7465 9501 0000 7306  ....create....s.
+000024d0: 0000 0000 020a 0116 017a 0c4d 6f64 656c  .........z.Model
+000024e0: 2e63 7265 6174 6563 0100 0000 0000 0000  .createc........
+000024f0: 0100 0000 0200 0000 4300 0000 730c 0000  ........C...s...
+00002500: 0074 007c 0083 016a 0183 0053 0029 014e  .t.|...j...S.).N
+00002510: 2902 720b 0000 0072 8d00 0000 2901 728e  ).r....r....).r.
+00002520: 0000 0072 0f00 0000 720f 0000 0072 1000  ...r....r....r..
+00002530: 0000 728d 0000 009b 0100 0073 0200 0000  ..r........s....
+00002540: 0002 7a0b 4d6f 6465 6c2e 6669 7273 7463  ..z.Model.firstc
+00002550: 0100 0000 0000 0000 0300 0000 0300 0000  ................
+00002560: 4f00 0000 7310 0000 0074 007c 0083 016a  O...s....t.|...j
+00002570: 017c 017c 028e 0153 0029 014e 2902 720b  .|.|...S.).N).r.
+00002580: 0000 0072 8c00 0000 2903 728e 0000 0072  ...r....).r....r
+00002590: 6a00 0000 726b 0000 0072 0f00 0000 720f  j...rk...r....r.
+000025a0: 0000 0072 1000 0000 728c 0000 009f 0100  ...r....r.......
+000025b0: 0073 0200 0000 0002 7a0c 4d6f 6465 6c2e  .s......z.Model.
+000025c0: 6669 6c74 6572 6301 0000 0000 0000 0001  filterc.........
+000025d0: 0000 0002 0000 0043 0000 0073 0800 0000  .......C...s....
+000025e0: 7400 7c00 8301 5300 2901 4e29 0172 0b00  t.|...S.).N).r..
+000025f0: 0000 2901 728e 0000 0072 0f00 0000 720f  ..).r....r....r.
+00002600: 0000 0072 1000 0000 da03 616c 6ca3 0100  ...r......all...
+00002610: 0073 0200 0000 0002 7a09 4d6f 6465 6c2e  .s......z.Model.
+00002620: 616c 6c63 0100 0000 0000 0000 0300 0000  allc............
+00002630: 0300 0000 4f00 0000 7314 0000 0074 007c  ....O...s....t.|
+00002640: 0083 016a 017c 017c 028e 016a 0283 0053  ...j.|.|...j...S
+00002650: 0029 014e 2903 720b 0000 0072 8c00 0000  .).N).r....r....
+00002660: 728d 0000 0029 0372 8e00 0000 726a 0000  r....).r....rj..
+00002670: 0072 6b00 0000 720f 0000 0072 0f00 0000  .rk...r....r....
+00002680: 7210 0000 0072 4e00 0000 a701 0000 7302  r....rN.......s.
+00002690: 0000 0000 037a 094d 6f64 656c 2e67 6574  .....z.Model.get
+000026a0: 6302 0000 0001 0000 0005 0000 0004 0000  c...............
+000026b0: 00c7 0000 0073 3400 0000 7c02 7208 7c02  .....s4...|.r.|.
+000026c0: 6e06 7c00 6a00 6a01 7d04 7c04 6a02 7c00  n.|.j.j.}.|.j.|.
+000026d0: 7c04 6401 8d02 6a03 7c01 6601 7c03 9e02  |.d...j.|.f.|...
+000026e0: 8e00 4900 6400 4800 0100 6400 5300 2902  ..I.d.H...d.S.).
+000026f0: 4e29 0272 7900 0000 724f 0000 0029 0472  N).ry...rO...).r
+00002700: 3300 0000 724f 0000 0072 7a00 0000 7283  3...rO...rz...r.
+00002710: 0000 0029 0572 8e00 0000 da0d 696e 7374  ...).r......inst
+00002720: 616e 6365 5f6c 6973 7472 7c00 0000 726a  ance_listr|...rj
+00002730: 0000 0072 4f00 0000 720f 0000 0072 0f00  ...rO...r....r..
+00002740: 0000 7210 0000 0072 8300 0000 ac01 0000  ..r....r........
+00002750: 730a 0000 0000 0210 0104 0102 0108 017a  s..............z
+00002760: 144d 6f64 656c 2e66 6574 6368 5f66 6f72  .Model.fetch_for
+00002770: 5f6c 6973 7463 0000 0000 0000 0000 0000  _listc..........
+00002780: 0000 0100 0000 4000 0000 730c 0000 0065  ......@...s....e
+00002790: 005a 0164 005a 0264 0153 0029 027a 0a4d  .Z.d.Z.d.S.).z.M
+000027a0: 6f64 656c 2e4d 6574 614e 2903 7250 0000  odel.MetaN).rP..
+000027b0: 0072 5100 0000 7252 0000 0072 0f00 0000  .rQ...rR...r....
+000027c0: 720f 0000 0072 0f00 0000 7210 0000 0072  r....r....r....r
+000027d0: 5500 0000 b401 0000 7302 0000 0008 0172  U.......s......r
+000027e0: 5500 0000 2901 4e29 014e 2901 4e29 024e  U...).N).N).N).N
+000027f0: 4e29 1672 5000 0000 7251 0000 0072 5200  N).rP...rQ...rR.
+00002800: 0000 724d 0000 0072 7d00 0000 727f 0000  ..rM...r}...r...
+00002810: 0072 8000 0000 7282 0000 0072 8400 0000  .r....r....r....
+00002820: 7285 0000 0072 8600 0000 7289 0000 0072  r....r....r....r
+00002830: 8b00 0000 da0b 636c 6173 736d 6574 686f  ......classmetho
+00002840: 6472 9100 0000 7292 0000 0072 8d00 0000  dr....r....r....
+00002850: 728c 0000 0072 9300 0000 724e 0000 0072  r....r....rN...r
+00002860: 8300 0000 7255 0000 0072 0f00 0000 720f  ....rU...r....r.
+00002870: 0000 0072 0f00 0000 7210 0000 0072 6f00  ...r....r....ro.
+00002880: 0000 2401 0000 7328 0000 0008 0108 320a  ..$...s(......2.
+00002890: 070a 0708 060a 090e 0708 0308 0308 0508  ................
+000028a0: 0602 010c 080c 060c 040c 040c 040c 0502  ................
+000028b0: 0110 0772 6f00 0000 2901 da09 6d65 7461  ...ro...)...meta
+000028c0: 636c 6173 7329 2672 2600 0000 da06 7079  class)&r&.....py
+000028d0: 7069 6b61 7202 0000 0072 0300 0000 da0c  pikar....r......
+000028e0: 7079 7069 6b61 2e65 6e75 6d73 7204 0000  pypika.enumsr...
+000028f0: 00da 0874 6f72 746f 6973 6572 0500 0000  ...tortoiser....
+00002900: da10 746f 7274 6f69 7365 2e63 6f6e 7465  ..tortoise.conte
+00002910: 7874 7206 0000 00da 1374 6f72 746f 6973  xtr......tortois
+00002920: 652e 6578 6365 7074 696f 6e73 7207 0000  e.exceptionsr...
+00002930: 0072 0800 0000 da0f 746f 7274 6f69 7365  .r......tortoise
+00002940: 2e66 6965 6c64 7372 0900 0000 720a 0000  .fieldsr....r...
+00002950: 00da 1174 6f72 746f 6973 652e 7175 6572  ...tortoise.quer
+00002960: 7973 6574 720b 0000 0072 1100 0000 7214  ysetr....r....r.
+00002970: 0000 0072 1600 0000 7218 0000 0072 1900  ...r....r....r..
+00002980: 0000 721e 0000 0072 1f00 0000 7220 0000  ..r....r....r ..
+00002990: 0072 2200 0000 7223 0000 0072 2400 0000  .r"...r#...r$...
+000029a0: 722f 0000 0072 3400 0000 da03 7374 7272  r/...r4.....strr
+000029b0: 5d00 0000 723c 0000 0072 3d00 0000 7232  ]...r<...r=...r2
+000029c0: 0000 0072 5400 0000 726f 0000 0072 0f00  ...rT...ro...r..
+000029d0: 0000 720f 0000 0072 0f00 0000 7210 0000  ..r....r....r...
+000029e0: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
+000029f0: 3000 0000 0802 1001 0c02 0c01 0c01 1001  0...............
+00002a00: 1001 0c03 0804 0804 0804 0807 0807 0804  ................
+00002a10: 0804 0804 0806 0806 0806 0820 0820 144a  ........... . .J
+00002a20: 0e16 103f                                ...?
```

### Comparing `tortoise-orm-0.9.2/tortoise/__pycache__/fields.cpython-36.pyc` & `tortoise-orm-0.9.4/tortoise/__pycache__/fields.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.6 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,795 +1,821 @@
-00000000: 330d 0d0a 5576 3f5b 782a 0000 e300 0000  3...Uv?[x*......
+00000000: 330d 0d0a dc7e 445b 8d2c 0000 e300 0000  3....~D[.,......
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 7801 0000 6400 6401 6c00 5a00 6400  .sx...d.d.l.Z.d.
+00000020: 0073 7c01 0000 6400 6401 6c00 5a00 6400  .s|...d.d.l.Z.d.
 00000030: 6401 6c01 5a01 6400 6401 6c02 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c03 6d04 5a04 0100 6400 6403 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6400 6401 6c07 5a07 6400  m.Z...d.d.l.Z.d.
-00000060: 6404 6c08 6d09 5a09 6d0a 5a0a 0100 6400  d.l.m.Z.m.Z...d.
-00000070: 6405 6c0b 6d0c 5a0c 0100 6406 5a0d 6407  d.l.m.Z...d.Z.d.
-00000080: 5a0e 6408 5a0f 6409 5a10 6501 6a11 6502  Z.d.Z.d.Z.e.j.e.
-00000090: 6a12 642d 640c 8d02 5a13 6502 6a14 5a15  j.d-d...Z.e.j.Z.
-000000a0: 4700 640d 640e 8400 640e 8302 5a16 4700  G.d.d...d...Z.G.
-000000b0: 640f 6410 8400 6410 6516 8303 5a17 4700  d.d...d.e...Z.G.
-000000c0: 6411 6412 8400 6412 6516 8303 5a18 4700  d.d...d.e...Z.G.
-000000d0: 6413 6414 8400 6414 6516 8303 5a19 4700  d.d...d.e...Z.G.
-000000e0: 6415 6416 8400 6416 6516 8303 5a1a 4700  d.d...d.e...Z.G.
-000000f0: 6417 6418 8400 6418 6516 8303 5a1b 4700  d.d...d.e...Z.G.
-00000100: 6419 641a 8400 641a 6516 8303 5a1c 4700  d.d...d.e...Z.G.
-00000110: 641b 641c 8400 641c 6516 8303 5a1d 4700  d.d...d.e...Z.G.
-00000120: 641d 641e 8400 641e 6516 8303 5a1e 4700  d.d...d.e...Z.G.
-00000130: 641f 6420 8400 6420 6516 8303 5a1f 4700  d.d ..d e...Z.G.
-00000140: 6421 6422 8400 6422 6516 8303 5a20 4700  d!d"..d"e...Z G.
-00000150: 6423 6424 8400 6424 6516 8303 5a21 4700  d#d$..d$e...Z!G.
-00000160: 6425 6426 8400 6426 6516 8303 5a22 4700  d%d&..d&e...Z"G.
-00000170: 6427 6428 8400 6428 8302 5a23 4700 6429  d'd(..d(..Z#G.d)
-00000180: 642a 8400 642a 8302 5a24 4700 642b 642c  d*..d*..Z$G.d+d,
-00000190: 8400 642c 6524 8303 5a25 6401 5300 292e  ..d,e$..Z%d.S.).
-000001a0: e900 0000 004e 2901 da07 4465 6369 6d61  .....N)...Decima
-000001b0: 6c29 01da 0554 6162 6c65 2902 da12 436f  l)...Table)...Co
-000001c0: 6e66 6967 7572 6174 696f 6e45 7272 6f72  nfigurationError
-000001d0: da0f 4e6f 5661 6c75 6573 4665 7463 6865  ..NoValuesFetche
-000001e0: 6429 01da 1441 7379 6e63 4974 6572 6174  d)...AsyncIterat
-000001f0: 6f72 5772 6170 7065 72da 0743 4153 4341  orWrapper..CASCA
-00000200: 4445 da08 5245 5354 5249 4354 7a08 5345  DE..RESTRICTz.SE
-00000210: 5420 4e55 4c4c 7a0b 5345 5420 4445 4641  T NULLz.SET DEFA
-00000220: 554c 54fa 012c fa01 3a29 01da 0a73 6570  ULT..,..:)...sep
-00000230: 6172 6174 6f72 7363 0000 0000 0000 0000  aratorsc........
-00000240: 0000 0000 0700 0000 4000 0000 7326 0000  ........@...s&..
-00000250: 0065 005a 0164 005a 0264 0964 0364 0484  .e.Z.d.Z.d.d.d..
-00000260: 015a 0364 0564 0684 005a 0464 0764 0884  .Z.d.d...Z.d.d..
-00000270: 005a 0564 0153 0029 0ada 0546 6965 6c64  .Z.d.S.)...Field
-00000280: 4e46 6308 0000 0000 0000 0009 0000 0002  NFc.............
-00000290: 0000 004b 0000 0073 2e00 0000 7c01 7c00  ...K...s....|.|.
-000002a0: 5f00 7c02 7c00 5f01 7c03 7c00 5f02 7c04  _.|.|._.|.|._.|.
-000002b0: 7c00 5f03 7c06 7c00 5f04 7c05 7c00 5f05  |._.|.|._.|.|._.
-000002c0: 7c07 7c00 5f06 6400 5300 2901 4e29 07da  |.|._.d.S.).N)..
-000002d0: 0474 7970 65da 0c73 6f75 7263 655f 6669  .type..source_fi
-000002e0: 656c 64da 0967 656e 6572 6174 6564 da02  eld..generated..
-000002f0: 706b da07 6465 6661 756c 74da 046e 756c  pk..default..nul
-00000300: 6cda 0675 6e69 7175 6529 09da 0473 656c  l..unique)...sel
-00000310: 6672 0d00 0000 720e 0000 0072 0f00 0000  fr....r....r....
-00000320: 7210 0000 0072 1200 0000 7211 0000 0072  r....r....r....r
-00000330: 1300 0000 da06 6b77 6172 6773 a900 7216  ......kwargs..r.
-00000340: 0000 00fa 432f 5573 6572 732f 616e 6472  ....C/Users/andr
-00000350: 6579 626f 6e64 6172 2f50 7943 6861 726d  eybondar/PyCharm
-00000360: 5072 6f6a 6563 7473 2f74 6f72 746f 6973  Projects/tortois
-00000370: 652d 6f72 6d2f 746f 7274 6f69 7365 2f66  e-orm/tortoise/f
-00000380: 6965 6c64 732e 7079 da08 5f5f 696e 6974  ields.py..__init
-00000390: 5f5f 1a00 0000 730e 0000 0000 0b06 0106  __....s.........
-000003a0: 0106 0106 0106 0106 017a 0e46 6965 6c64  .........z.Field
-000003b0: 2e5f 5f69 6e69 745f 5f63 0200 0000 0000  .__init__c......
-000003c0: 0000 0200 0000 0100 0000 4300 0000 7304  ..........C...s.
-000003d0: 0000 007c 0153 0029 014e 7216 0000 0029  ...|.S.).Nr....)
-000003e0: 0272 1400 0000 da05 7661 6c75 6572 1600  .r......valuer..
-000003f0: 0000 7216 0000 0072 1700 0000 da0b 746f  ..r....r......to
-00000400: 5f64 625f 7661 6c75 652d 0000 0073 0200  _db_value-...s..
-00000410: 0000 0001 7a11 4669 656c 642e 746f 5f64  ....z.Field.to_d
-00000420: 625f 7661 6c75 6563 0200 0000 0000 0000  b_valuec........
-00000430: 0200 0000 0300 0000 4300 0000 7322 0000  ........C...s"..
-00000440: 007c 0164 006b 0873 1474 007c 017c 006a  .|.d.k.s.t.|.|.j
-00000450: 0183 0272 187c 0153 007c 006a 017c 0183  ...r.|.S.|.j.|..
-00000460: 0153 0029 014e 2902 da0a 6973 696e 7374  .S.).N)...isinst
-00000470: 616e 6365 720d 0000 0029 0272 1400 0000  ancer....).r....
-00000480: 7219 0000 0072 1600 0000 7216 0000 0072  r....r....r....r
-00000490: 1700 0000 da0f 746f 5f70 7974 686f 6e5f  ......to_python_
-000004a0: 7661 6c75 6530 0000 0073 0600 0000 0001  value0...s......
-000004b0: 1401 0401 7a15 4669 656c 642e 746f 5f70  ....z.Field.to_p
-000004c0: 7974 686f 6e5f 7661 6c75 6529 074e 4e46  ython_value).NNF
-000004d0: 4646 4e46 2906 da08 5f5f 6e61 6d65 5f5f  FFNF)...__name__
-000004e0: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
-000004f0: 7175 616c 6e61 6d65 5f5f 7218 0000 0072  qualname__r....r
-00000500: 1a00 0000 721c 0000 0072 1600 0000 7216  ....r....r....r.
-00000510: 0000 0072 1600 0000 7217 0000 0072 0c00  ...r....r....r..
-00000520: 0000 1900 0000 7312 0000 0008 0300 0100  ......s.........
-00000530: 0100 0100 0100 0100 010a 0b08 0372 0c00  .............r..
-00000540: 0000 6300 0000 0000 0000 0000 0000 0004  ..c.............
-00000550: 0000 0000 0000 0073 1e00 0000 6500 5a01  .......s....e.Z.
-00000560: 6400 5a02 6405 8700 6601 6403 6404 8409  d.Z.d...f.d.d...
-00000570: 5a03 8700 0400 5a04 5300 2906 da08 496e  Z.....Z.S.)...In
-00000580: 7446 6965 6c64 4e46 6303 0000 0000 0000  tFieldNFc.......
-00000590: 0004 0000 0003 0000 000b 0000 0073 3e00  .............s>.
-000005a0: 0000 7400 7c03 6a01 6401 8301 8301 7c02  ..t.|.j.d.....|.
-000005b0: 4200 7c03 6401 3c00 7402 8300 6a03 7404  B.|.d.<.t...j.t.
-000005c0: 7c01 6602 7c03 8e01 0100 7c03 6a01 6402  |.f.|.....|.j.d.
-000005d0: 8301 7c00 5f05 7c02 7c00 5f06 6400 5300  ..|._.|.|._.d.S.
-000005e0: 2903 4e72 0f00 0000 da09 7265 6665 7265  ).Nr......refere
-000005f0: 6e63 6529 07da 0462 6f6f 6cda 0367 6574  nce)...bool..get
-00000600: da05 7375 7065 7272 1800 0000 da03 696e  ..superr......in
-00000610: 7472 2100 0000 7210 0000 0029 0472 1400  tr!...r....).r..
-00000620: 0000 720e 0000 0072 1000 0000 7215 0000  ..r....r....r...
-00000630: 0029 01da 095f 5f63 6c61 7373 5f5f 7216  .)...__class__r.
-00000640: 0000 0072 1700 0000 7218 0000 0037 0000  ...r....r....7..
-00000650: 0073 0800 0000 0001 1601 1201 0c01 7a11  .s............z.
-00000660: 496e 7446 6965 6c64 2e5f 5f69 6e69 745f  IntField.__init_
-00000670: 5f29 024e 4629 0572 1d00 0000 721e 0000  _).NF).r....r...
-00000680: 0072 1f00 0000 7218 0000 00da 0d5f 5f63  .r....r......__c
-00000690: 6c61 7373 6365 6c6c 5f5f 7216 0000 0072  lasscell__r....r
-000006a0: 1600 0000 2901 7226 0000 0072 1700 0000  ....).r&...r....
-000006b0: 7220 0000 0036 0000 0073 0200 0000 0801  r ...6...s......
-000006c0: 7220 0000 0063 0000 0000 0000 0000 0000  r ...c..........
-000006d0: 0000 0300 0000 0000 0000 731c 0000 0065  ..........s....e
-000006e0: 005a 0164 005a 0287 0066 0164 0164 0284  .Z.d.Z...f.d.d..
-000006f0: 085a 0387 0004 005a 0453 0029 03da 0d53  .Z.....Z.S.)...S
-00000700: 6d61 6c6c 496e 7446 6965 6c64 6301 0000  mallIntFieldc...
-00000710: 0000 0000 0002 0000 0003 0000 000b 0000  ................
-00000720: 0073 1400 0000 7400 8300 6a01 7402 6601  .s....t...j.t.f.
-00000730: 7c01 8e01 0100 6400 5300 2901 4e29 0372  |.....d.S.).N).r
-00000740: 2400 0000 7218 0000 0072 2500 0000 2902  $...r....r%...).
-00000750: 7214 0000 0072 1500 0000 2901 7226 0000  r....r....).r&..
-00000760: 0072 1600 0000 7217 0000 0072 1800 0000  .r....r....r....
-00000770: 3f00 0000 7302 0000 0000 017a 1653 6d61  ?...s......z.Sma
-00000780: 6c6c 496e 7446 6965 6c64 2e5f 5f69 6e69  llIntField.__ini
-00000790: 745f 5f29 0572 1d00 0000 721e 0000 0072  t__).r....r....r
-000007a0: 1f00 0000 7218 0000 0072 2700 0000 7216  ....r....r'...r.
-000007b0: 0000 0072 1600 0000 2901 7226 0000 0072  ...r....).r&...r
-000007c0: 1700 0000 7228 0000 003e 0000 0073 0200  ....r(...>...s..
-000007d0: 0000 0801 7228 0000 0063 0000 0000 0000  ....r(...c......
-000007e0: 0000 0000 0000 0400 0000 0000 0000 731e  ..............s.
-000007f0: 0000 0065 005a 0164 005a 0264 0487 0066  ...e.Z.d.Z.d...f
-00000800: 0164 0264 0384 095a 0387 0004 005a 0453  .d.d...Z.....Z.S
-00000810: 0029 05da 0943 6861 7246 6965 6c64 7201  .)...CharFieldr.
-00000820: 0000 0063 0200 0000 0000 0000 0300 0000  ...c............
-00000830: 0300 0000 0b00 0000 7332 0000 0074 007c  ........s2...t.|
-00000840: 0183 0164 016b 0072 1474 0164 0283 0182  ...d.k.r.t.d....
-00000850: 0174 007c 0183 017c 005f 0274 0383 006a  .t.|...|._.t...j
-00000860: 0474 0566 017c 028e 0101 0064 0053 0029  .t.f.|.....d.S.)
-00000870: 034e e901 0000 007a 176d 6178 5f64 6967  .N.....z.max_dig
-00000880: 6974 7320 6d75 7374 2062 6520 3e3d 2031  its must be >= 1
-00000890: 2906 7225 0000 0072 0400 0000 da0a 6d61  ).r%...r......ma
-000008a0: 785f 6c65 6e67 7468 7224 0000 0072 1800  x_lengthr$...r..
-000008b0: 0000 da03 7374 7229 0372 1400 0000 722b  ....str).r....r+
-000008c0: 0000 0072 1500 0000 2901 7226 0000 0072  ...r....).r&...r
-000008d0: 1600 0000 7217 0000 0072 1800 0000 4400  ....r....r....D.
-000008e0: 0000 7308 0000 0000 010c 0108 010a 017a  ..s............z
-000008f0: 1243 6861 7246 6965 6c64 2e5f 5f69 6e69  .CharField.__ini
-00000900: 745f 5f29 0172 0100 0000 2905 721d 0000  t__).r....).r...
-00000910: 0072 1e00 0000 721f 0000 0072 1800 0000  .r....r....r....
-00000920: 7227 0000 0072 1600 0000 7216 0000 0029  r'...r....r....)
-00000930: 0172 2600 0000 7217 0000 0072 2900 0000  .r&...r....r)...
-00000940: 4300 0000 7302 0000 0008 0172 2900 0000  C...s......r)...
-00000950: 6300 0000 0000 0000 0000 0000 0003 0000  c...............
-00000960: 0000 0000 0073 1c00 0000 6500 5a01 6400  .....s....e.Z.d.
-00000970: 5a02 8700 6601 6401 6402 8408 5a03 8700  Z...f.d.d...Z...
-00000980: 0400 5a04 5300 2903 da09 5465 7874 4669  ..Z.S.)...TextFi
-00000990: 656c 6463 0100 0000 0000 0000 0200 0000  eldc............
-000009a0: 0300 0000 0b00 0000 7314 0000 0074 0083  ........s....t..
-000009b0: 006a 0174 0266 017c 018e 0101 0064 0053  .j.t.f.|.....d.S
-000009c0: 0029 014e 2903 7224 0000 0072 1800 0000  .).N).r$...r....
-000009d0: 722c 0000 0029 0272 1400 0000 7215 0000  r,...).r....r...
-000009e0: 0029 0172 2600 0000 7216 0000 0072 1700  .).r&...r....r..
-000009f0: 0000 7218 0000 004c 0000 0073 0200 0000  ..r....L...s....
-00000a00: 0001 7a12 5465 7874 4669 656c 642e 5f5f  ..z.TextField.__
-00000a10: 696e 6974 5f5f 2905 721d 0000 0072 1e00  init__).r....r..
-00000a20: 0000 721f 0000 0072 1800 0000 7227 0000  ..r....r....r'..
-00000a30: 0072 1600 0000 7216 0000 0029 0172 2600  .r....r....).r&.
-00000a40: 0000 7217 0000 0072 2d00 0000 4b00 0000  ..r....r-...K...
-00000a50: 7302 0000 0008 0172 2d00 0000 6300 0000  s......r-...c...
-00000a60: 0000 0000 0000 0000 0003 0000 0000 0000  ................
-00000a70: 0073 1c00 0000 6500 5a01 6400 5a02 8700  .s....e.Z.d.Z...
-00000a80: 6601 6401 6402 8408 5a03 8700 0400 5a04  f.d.d...Z.....Z.
-00000a90: 5300 2903 da0c 426f 6f6c 6561 6e46 6965  S.)...BooleanFie
-00000aa0: 6c64 6301 0000 0000 0000 0002 0000 0003  ldc.............
-00000ab0: 0000 000b 0000 0073 1400 0000 7400 8300  .......s....t...
-00000ac0: 6a01 7402 6601 7c01 8e01 0100 6400 5300  j.t.f.|.....d.S.
-00000ad0: 2901 4e29 0372 2400 0000 7218 0000 0072  ).N).r$...r....r
-00000ae0: 2200 0000 2902 7214 0000 0072 1500 0000  "...).r....r....
-00000af0: 2901 7226 0000 0072 1600 0000 7217 0000  ).r&...r....r...
-00000b00: 0072 1800 0000 5100 0000 7302 0000 0000  .r....Q...s.....
-00000b10: 017a 1542 6f6f 6c65 616e 4669 656c 642e  .z.BooleanField.
-00000b20: 5f5f 696e 6974 5f5f 2905 721d 0000 0072  __init__).r....r
-00000b30: 1e00 0000 721f 0000 0072 1800 0000 7227  ....r....r....r'
-00000b40: 0000 0072 1600 0000 7216 0000 0029 0172  ...r....r....).r
-00000b50: 2600 0000 7217 0000 0072 2e00 0000 5000  &...r....r....P.
-00000b60: 0000 7302 0000 0008 0172 2e00 0000 6300  ..s......r....c.
-00000b70: 0000 0000 0000 0000 0000 0004 0000 0000  ................
-00000b80: 0000 0073 1e00 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
-00000b90: 6406 8700 6601 6403 6404 8409 5a03 8700  d...f.d.d...Z...
-00000ba0: 0400 5a04 5300 2907 da0c 4465 6369 6d61  ..Z.S.)...Decima
-00000bb0: 6c46 6965 6c64 7201 0000 0072 2a00 0000  lFieldr....r*...
-00000bc0: 6303 0000 0000 0000 0004 0000 0003 0000  c...............
-00000bd0: 000b 0000 0073 4800 0000 7400 7c01 8301  .....sH...t.|...
-00000be0: 6401 6b00 7214 7401 6402 8301 8201 7400  d.k.r.t.d.....t.
-00000bf0: 7c02 8301 6403 6b00 7228 7401 6404 8301  |...d.k.r(t.d...
-00000c00: 8201 7402 8300 6a03 7404 6601 7c03 8e01  ..t...j.t.f.|...
-00000c10: 0100 7c01 7c00 5f05 7c02 7c00 5f06 6400  ..|.|._.|.|._.d.
-00000c20: 5300 2905 4e72 2a00 0000 7a17 6d61 785f  S.).Nr*...z.max_
-00000c30: 6469 6769 7473 206d 7573 7420 6265 203e  digits must be >
-00000c40: 3d20 3172 0100 0000 7a1b 6465 6369 6d61  = 1r....z.decima
-00000c50: 6c5f 706c 6163 6573 206d 7573 7420 6265  l_places must be
-00000c60: 203e 3d20 3029 0772 2500 0000 7204 0000   >= 0).r%...r...
-00000c70: 0072 2400 0000 7218 0000 0072 0200 0000  .r$...r....r....
-00000c80: da0a 6d61 785f 6469 6769 7473 da0e 6465  ..max_digits..de
-00000c90: 6369 6d61 6c5f 706c 6163 6573 2904 7214  cimal_places).r.
-00000ca0: 0000 0072 3000 0000 7231 0000 0072 1500  ...r0...r1...r..
-00000cb0: 0000 2901 7226 0000 0072 1600 0000 7217  ..).r&...r....r.
-00000cc0: 0000 0072 1800 0000 5600 0000 730e 0000  ...r....V...s...
-00000cd0: 0000 010c 0108 010c 0108 0110 0106 017a  ...............z
-00000ce0: 1544 6563 696d 616c 4669 656c 642e 5f5f  .DecimalField.__
-00000cf0: 696e 6974 5f5f e9ff ffff ff29 0272 0100  init__.....).r..
-00000d00: 0000 7232 0000 0029 0572 1d00 0000 721e  ..r2...).r....r.
-00000d10: 0000 0072 1f00 0000 7218 0000 0072 2700  ...r....r....r'.
-00000d20: 0000 7216 0000 0072 1600 0000 2901 7226  ..r....r....).r&
-00000d30: 0000 0072 1700 0000 722f 0000 0055 0000  ...r....r/...U..
-00000d40: 0073 0200 0000 0801 722f 0000 0063 0000  .s......r/...c..
-00000d50: 0000 0000 0000 0000 0000 0400 0000 0000  ................
-00000d60: 0000 7326 0000 0065 005a 0164 005a 0264  ..s&...e.Z.d.Z.d
-00000d70: 0687 0066 0164 0264 0384 095a 0364 0464  ...f.d.d...Z.d.d
-00000d80: 0584 005a 0487 0004 005a 0553 0029 07da  ...Z.....Z.S.)..
-00000d90: 0d44 6174 6574 696d 6546 6965 6c64 4663  .DatetimeFieldFc
-00000da0: 0300 0000 0000 0000 0400 0000 0300 0000  ................
-00000db0: 0b00 0000 7350 0000 007c 0272 107c 0172  ....sP...|.r.|.r
-00000dc0: 1074 0064 0183 0182 017c 027c 0142 007d  .t.d.....|.|.B.}
-00000dd0: 0274 017c 036a 0264 0283 0183 017c 0242  .t.|.j.d.....|.B
-00000de0: 007c 0364 023c 0074 0383 006a 0474 056a  .|.d.<.t...j.t.j
-00000df0: 0566 017c 038e 0101 007c 017c 005f 067c  .f.|.....|.|._.|
-00000e00: 027c 005f 0764 0053 0029 034e 7a2c 596f  .|._.d.S.).Nz,Yo
-00000e10: 7520 6361 6e20 6368 6f6f 7365 206f 6e6c  u can choose onl
-00000e20: 7920 6175 746f 5f6e 6f77 206f 7220 6175  y auto_now or au
-00000e30: 746f 5f6e 6f77 5f61 6464 720f 0000 0029  to_now_addr....)
-00000e40: 0872 0400 0000 7222 0000 0072 2300 0000  .r....r"...r#...
-00000e50: 7224 0000 0072 1800 0000 da08 6461 7465  r$...r......date
-00000e60: 7469 6d65 da08 6175 746f 5f6e 6f77 da0c  time..auto_now..
-00000e70: 6175 746f 5f6e 6f77 5f61 6464 2904 7214  auto_now_add).r.
-00000e80: 0000 0072 3500 0000 7236 0000 0072 1500  ...r5...r6...r..
-00000e90: 0000 2901 7226 0000 0072 1600 0000 7217  ..).r&...r....r.
-00000ea0: 0000 0072 1800 0000 6100 0000 730e 0000  ...r....a...s...
-00000eb0: 0000 0108 0108 0108 0116 0112 0106 017a  ...............z
-00000ec0: 1644 6174 6574 696d 6546 6965 6c64 2e5f  .DatetimeField._
-00000ed0: 5f69 6e69 745f 5f63 0200 0000 0000 0000  _init__c........
-00000ee0: 0200 0000 0300 0000 4300 0000 7322 0000  ........C...s"..
-00000ef0: 007c 0164 006b 0873 1474 007c 017c 006a  .|.d.k.s.t.|.|.j
-00000f00: 0183 0272 187c 0153 0074 026a 037c 0183  ...r.|.S.t.j.|..
-00000f10: 0153 0029 014e 2904 721b 0000 0072 0d00  .S.).N).r....r..
-00000f20: 0000 da08 6369 736f 3836 3031 da0e 7061  ....ciso8601..pa
-00000f30: 7273 655f 6461 7465 7469 6d65 2902 7214  rse_datetime).r.
-00000f40: 0000 0072 1900 0000 7216 0000 0072 1600  ...r....r....r..
-00000f50: 0000 7217 0000 0072 1c00 0000 6a00 0000  ..r....r....j...
-00000f60: 7306 0000 0000 0114 0104 017a 1d44 6174  s..........z.Dat
-00000f70: 6574 696d 6546 6965 6c64 2e74 6f5f 7079  etimeField.to_py
-00000f80: 7468 6f6e 5f76 616c 7565 2902 4646 2906  thon_value).FF).
-00000f90: 721d 0000 0072 1e00 0000 721f 0000 0072  r....r....r....r
-00000fa0: 1800 0000 721c 0000 0072 2700 0000 7216  ....r....r'...r.
-00000fb0: 0000 0072 1600 0000 2901 7226 0000 0072  ...r....).r&...r
-00000fc0: 1700 0000 7233 0000 0060 0000 0073 0400  ....r3...`...s..
-00000fd0: 0000 0801 0e09 7233 0000 0063 0000 0000  ......r3...c....
-00000fe0: 0000 0000 0000 0000 0300 0000 0000 0000  ................
-00000ff0: 7324 0000 0065 005a 0164 005a 0287 0066  s$...e.Z.d.Z...f
-00001000: 0164 0164 0284 085a 0364 0364 0484 005a  .d.d...Z.d.d...Z
-00001010: 0487 0004 005a 0553 0029 05da 0944 6174  .....Z.S.)...Dat
-00001020: 6546 6965 6c64 6301 0000 0000 0000 0002  eFieldc.........
-00001030: 0000 0003 0000 000b 0000 0073 1600 0000  ...........s....
-00001040: 7400 8300 6a01 7402 6a03 6601 7c01 8e01  t...j.t.j.f.|...
-00001050: 0100 6400 5300 2901 4e29 0472 2400 0000  ..d.S.).N).r$...
-00001060: 7218 0000 0072 3400 0000 da04 6461 7465  r....r4.....date
-00001070: 2902 7214 0000 0072 1500 0000 2901 7226  ).r....r....).r&
-00001080: 0000 0072 1600 0000 7217 0000 0072 1800  ...r....r....r..
-00001090: 0000 7100 0000 7302 0000 0000 017a 1244  ..q...s......z.D
-000010a0: 6174 6546 6965 6c64 2e5f 5f69 6e69 745f  ateField.__init_
-000010b0: 5f63 0200 0000 0000 0000 0200 0000 0300  _c..............
-000010c0: 0000 4300 0000 7326 0000 007c 0164 006b  ..C...s&...|.d.k
-000010d0: 0873 1474 007c 017c 006a 0183 0272 187c  .s.t.|.|.j...r.|
-000010e0: 0153 0074 026a 037c 0183 016a 0483 0053  .S.t.j.|...j...S
-000010f0: 0029 014e 2905 721b 0000 0072 0d00 0000  .).N).r....r....
-00001100: 7237 0000 0072 3800 0000 723a 0000 0029  r7...r8...r:...)
-00001110: 0272 1400 0000 7219 0000 0072 1600 0000  .r....r....r....
-00001120: 7216 0000 0072 1700 0000 721c 0000 0074  r....r....r....t
-00001130: 0000 0073 0600 0000 0001 1401 0401 7a19  ...s..........z.
-00001140: 4461 7465 4669 656c 642e 746f 5f70 7974  DateField.to_pyt
-00001150: 686f 6e5f 7661 6c75 6529 0672 1d00 0000  hon_value).r....
-00001160: 721e 0000 0072 1f00 0000 7218 0000 0072  r....r....r....r
-00001170: 1c00 0000 7227 0000 0072 1600 0000 7216  ....r'...r....r.
-00001180: 0000 0029 0172 2600 0000 7217 0000 0072  ...).r&...r....r
-00001190: 3900 0000 7000 0000 7304 0000 0008 010c  9...p...s.......
-000011a0: 0372 3900 0000 6300 0000 0000 0000 0000  .r9...c.........
-000011b0: 0000 0003 0000 0000 0000 0073 1c00 0000  ...........s....
-000011c0: 6500 5a01 6400 5a02 8700 6601 6401 6402  e.Z.d.Z...f.d.d.
-000011d0: 8408 5a03 8700 0400 5a04 5300 2903 da0a  ..Z.....Z.S.)...
-000011e0: 466c 6f61 7446 6965 6c64 6301 0000 0000  FloatFieldc.....
-000011f0: 0000 0002 0000 0003 0000 000b 0000 0073  ...............s
-00001200: 1400 0000 7400 8300 6a01 7402 6601 7c01  ....t...j.t.f.|.
-00001210: 8e01 0100 6400 5300 2901 4e29 0372 2400  ....d.S.).N).r$.
-00001220: 0000 7218 0000 00da 0566 6c6f 6174 2902  ..r......float).
-00001230: 7214 0000 0072 1500 0000 2901 7226 0000  r....r....).r&..
-00001240: 0072 1600 0000 7217 0000 0072 1800 0000  .r....r....r....
-00001250: 7b00 0000 7302 0000 0000 017a 1346 6c6f  {...s......z.Flo
-00001260: 6174 4669 656c 642e 5f5f 696e 6974 5f5f  atField.__init__
-00001270: 2905 721d 0000 0072 1e00 0000 721f 0000  ).r....r....r...
-00001280: 0072 1800 0000 7227 0000 0072 1600 0000  .r....r'...r....
-00001290: 7216 0000 0029 0172 2600 0000 7217 0000  r....).r&...r...
-000012a0: 0072 3b00 0000 7a00 0000 7302 0000 0008  .r;...z...s.....
-000012b0: 0172 3b00 0000 6300 0000 0000 0000 0000  .r;...c.........
-000012c0: 0000 0004 0000 0000 0000 0073 3200 0000  ...........s2...
-000012d0: 6500 5a01 6400 5a02 6503 6504 6602 8700  e.Z.d.Z.e.e.f...
-000012e0: 6601 6401 6402 8409 5a05 6403 6404 8400  f.d.d...Z.d.d...
-000012f0: 5a06 6405 6406 8400 5a07 8700 0400 5a08  Z.d.d...Z.....Z.
-00001300: 5300 2907 da09 4a53 4f4e 4669 656c 6463  S.)...JSONFieldc
-00001310: 0300 0000 0000 0000 0400 0000 0300 0000  ................
-00001320: 0b00 0000 7324 0000 0074 0083 006a 0174  ....s$...t...j.t
-00001330: 0274 0366 0266 017c 038e 0101 007c 017c  .t.f.f.|.....|.|
-00001340: 005f 047c 027c 005f 0564 0053 0029 014e  ._.|.|._.d.S.).N
-00001350: 2906 7224 0000 0072 1800 0000 da04 6469  ).r$...r......di
-00001360: 6374 da04 6c69 7374 da07 656e 636f 6465  ct..list..encode
-00001370: 72da 0764 6563 6f64 6572 2904 7214 0000  r..decoder).r...
-00001380: 0072 4000 0000 7241 0000 0072 1500 0000  .r@...rA...r....
-00001390: 2901 7226 0000 0072 1600 0000 7217 0000  ).r&...r....r...
-000013a0: 0072 1800 0000 8000 0000 7306 0000 0000  .r........s.....
-000013b0: 0114 0106 017a 124a 534f 4e46 6965 6c64  .....z.JSONField
-000013c0: 2e5f 5f69 6e69 745f 5f63 0200 0000 0000  .__init__c......
-000013d0: 0000 0200 0000 0200 0000 4300 0000 7316  ..........C...s.
-000013e0: 0000 007c 0164 006b 0872 0c7c 0153 007c  ...|.d.k.r.|.S.|
-000013f0: 006a 007c 0183 0153 0029 014e 2901 7240  .j.|...S.).N).r@
-00001400: 0000 0029 0272 1400 0000 7219 0000 0072  ...).r....r....r
-00001410: 1600 0000 7216 0000 0072 1700 0000 721a  ....r....r....r.
-00001420: 0000 0085 0000 0073 0600 0000 0001 0801  .......s........
-00001430: 0401 7a15 4a53 4f4e 4669 656c 642e 746f  ..z.JSONField.to
-00001440: 5f64 625f 7661 6c75 6563 0200 0000 0000  _db_valuec......
-00001450: 0000 0200 0000 0300 0000 4300 0000 7322  ..........C...s"
-00001460: 0000 007c 0164 006b 0873 1474 007c 017c  ...|.d.k.s.t.|.|
-00001470: 006a 0183 0272 187c 0153 007c 006a 027c  .j...r.|.S.|.j.|
-00001480: 0183 0153 0029 014e 2903 721b 0000 0072  ...S.).N).r....r
-00001490: 0d00 0000 7241 0000 0029 0272 1400 0000  ....rA...).r....
-000014a0: 7219 0000 0072 1600 0000 7216 0000 0072  r....r....r....r
-000014b0: 1700 0000 721c 0000 008a 0000 0073 0600  ....r........s..
-000014c0: 0000 0001 1401 0401 7a19 4a53 4f4e 4669  ........z.JSONFi
-000014d0: 656c 642e 746f 5f70 7974 686f 6e5f 7661  eld.to_python_va
-000014e0: 6c75 6529 0972 1d00 0000 721e 0000 0072  lue).r....r....r
-000014f0: 1f00 0000 da0a 4a53 4f4e 5f44 554d 5053  ......JSON_DUMPS
-00001500: da0a 4a53 4f4e 5f4c 4f41 4453 7218 0000  ..JSON_LOADSr...
-00001510: 0072 1a00 0000 721c 0000 0072 2700 0000  .r....r....r'...
-00001520: 7216 0000 0072 1600 0000 2901 7226 0000  r....r....).r&..
-00001530: 0072 1700 0000 723d 0000 007f 0000 0073  .r....r=.......s
-00001540: 0600 0000 0801 1205 0805 723d 0000 0063  ..........r=...c
-00001550: 0000 0000 0000 0000 0000 0000 0400 0000  ................
-00001560: 0000 0000 7322 0000 0065 005a 0164 005a  ....s"...e.Z.d.Z
-00001570: 0264 0165 0366 0287 0066 0164 0264 0384  .d.e.f...f.d.d..
-00001580: 095a 0487 0004 005a 0553 0029 04da 0f46  .Z.....Z.S.)...F
-00001590: 6f72 6569 676e 4b65 7946 6965 6c64 4e63  oreignKeyFieldNc
-000015a0: 0400 0000 0000 0000 0500 0000 0400 0000  ................
-000015b0: 0b00 0000 737c 0000 0074 0083 006a 0166  ....s|...t...j.f
-000015c0: 007c 048e 0101 0074 027c 0174 0383 0272  .|.....t.|.t...r
-000015d0: 2a74 047c 016a 0564 0183 0183 0164 026b  *t.|.j.d.....d.k
-000015e0: 0273 3274 0664 0383 0182 017c 017c 005f  .s2t.d.....|.|._
-000015f0: 077c 027c 005f 087c 0374 0974 0a74 0b68  .|.|._.|.t.t.t.h
-00001600: 036b 0673 5074 0682 017c 0374 0b6b 0274  .k.sPt...|.t.k.t
-00001610: 0c7c 046a 0d64 0483 0183 016b 0273 727c  .|.j.d.....k.sr|
-00001620: 0374 0b6b 0373 7274 0682 017c 037c 005f  .t.k.srt...|.|._
-00001630: 0e64 0053 0029 054e da01 2ee9 0200 0000  .d.S.).N........
-00001640: 7a34 466f 7265 6967 6e20 6b65 7920 6163  z4Foreign key ac
-00001650: 6365 7074 7320 6d6f 6465 6c20 6e61 6d65  cepts model name
-00001660: 2069 6e20 666f 726d 6174 2022 6170 702e   in format "app.
-00001670: 4d6f 6465 6c22 7212 0000 0029 0f72 2400  Model"r....).r$.
-00001680: 0000 7218 0000 0072 1b00 0000 722c 0000  ..r....r....r,..
-00001690: 00da 036c 656e da05 7370 6c69 74da 0e41  ...len..split..A
-000016a0: 7373 6572 7469 6f6e 4572 726f 72da 0a6d  ssertionError..m
-000016b0: 6f64 656c 5f6e 616d 65da 0c72 656c 6174  odel_name..relat
-000016c0: 6564 5f6e 616d 6572 0700 0000 7208 0000  ed_namer....r...
-000016d0: 00da 0853 4554 5f4e 554c 4c72 2200 0000  ...SET_NULLr"...
-000016e0: 7223 0000 00da 096f 6e5f 6465 6c65 7465  r#.....on_delete
-000016f0: 2905 7214 0000 0072 4a00 0000 724b 0000  ).r....rJ...rK..
-00001700: 0072 4d00 0000 7215 0000 0029 0172 2600  .rM...r....).r&.
-00001710: 0000 7216 0000 0072 1700 0000 7218 0000  ..r....r....r...
-00001720: 0091 0000 0073 1000 0000 0001 0e01 1e01  .....s..........
-00001730: 0601 0601 0601 1201 2201 7a18 466f 7265  ........".z.Fore
-00001740: 6967 6e4b 6579 4669 656c 642e 5f5f 696e  ignKeyField.__in
-00001750: 6974 5f5f 2906 721d 0000 0072 1e00 0000  it__).r....r....
-00001760: 721f 0000 0072 0700 0000 7218 0000 0072  r....r....r....r
-00001770: 2700 0000 7216 0000 0072 1600 0000 2901  '...r....r....).
-00001780: 7226 0000 0072 1700 0000 7244 0000 0090  r&...r....rD....
-00001790: 0000 0073 0200 0000 0801 7244 0000 0063  ...s......rD...c
-000017a0: 0000 0000 0000 0000 0000 0000 0400 0000  ................
-000017b0: 0000 0000 731e 0000 0065 005a 0164 005a  ....s....e.Z.d.Z
-000017c0: 0264 0487 0066 0164 0264 0384 095a 0387  .d...f.d.d...Z..
-000017d0: 0004 005a 0453 0029 05da 0f4d 616e 7954  ...Z.S.)...ManyT
-000017e0: 6f4d 616e 7946 6965 6c64 4e63 0600 0000  oManyFieldNc....
-000017f0: 0000 0000 0700 0000 0300 0000 0b00 0000  ................
-00001800: 736c 0000 0074 0083 006a 0166 007c 068e  sl...t...j.f.|..
-00001810: 0101 0074 027c 016a 0364 0183 0183 0164  ...t.|.j.d.....d
-00001820: 026b 0273 2874 0464 0383 0182 017c 017c  .k.s(t.d.....|.|
-00001830: 005f 057c 057c 005f 067c 0372 3c7c 036e  ._.|.|._.|.r<|.n
-00001840: 1664 046a 077c 016a 0364 0183 0164 0519  .d.j.|.j.d...d..
-00001850: 006a 0883 0083 017c 005f 097c 047c 005f  .j.....|._.|.|._
-00001860: 0a7c 027c 005f 0b64 067c 005f 0c64 0053  .|.|._.d.|._.d.S
-00001870: 0029 074e 7245 0000 0072 4600 0000 7a34  .).NrE...rF...z4
-00001880: 466f 7265 6967 6e20 6b65 7920 6163 6365  Foreign key acce
-00001890: 7074 7320 6d6f 6465 6c20 6e61 6d65 2069  pts model name i
-000018a0: 6e20 666f 726d 6174 2022 6170 702e 4d6f  n format "app.Mo
-000018b0: 6465 6c22 7a05 7b7d 5f69 6472 2a00 0000  del"z.{}_idr*...
-000018c0: 4629 0d72 2400 0000 7218 0000 0072 4700  F).r$...r....rG.
-000018d0: 0000 7248 0000 0072 4900 0000 724a 0000  ..rH...rI...rJ..
-000018e0: 0072 4b00 0000 da06 666f 726d 6174 da05  .rK.....format..
-000018f0: 6c6f 7765 72da 0b66 6f72 7761 7264 5f6b  lower..forward_k
-00001900: 6579 da0c 6261 636b 7761 7264 5f6b 6579  ey..backward_key
-00001910: da07 7468 726f 7567 68da 0a5f 6765 6e65  ..through.._gene
-00001920: 7261 7465 6429 0772 1400 0000 724a 0000  rated).r....rJ..
-00001930: 0072 5300 0000 7251 0000 0072 5200 0000  .rS...rQ...rR...
-00001940: 724b 0000 0072 1500 0000 2901 7226 0000  rK...r....).r&..
-00001950: 0072 1600 0000 7217 0000 0072 1800 0000  .r....r....r....
-00001960: 9d00 0000 7314 0000 0000 090e 010c 010e  ....s...........
-00001970: 0106 0106 010c 0116 0206 0106 017a 184d  .............z.M
-00001980: 616e 7954 6f4d 616e 7946 6965 6c64 2e5f  anyToManyField._
-00001990: 5f69 6e69 745f 5f29 044e 4e4e 4e29 0572  _init__).NNNN).r
-000019a0: 1d00 0000 721e 0000 0072 1f00 0000 7218  ....r....r....r.
-000019b0: 0000 0072 2700 0000 7216 0000 0072 1600  ...r'...r....r..
-000019c0: 0000 2901 7226 0000 0072 1700 0000 724e  ..).r&...r....rN
-000019d0: 0000 009c 0000 0073 0800 0000 0804 0001  .......s........
-000019e0: 0001 0001 724e 0000 0063 0000 0000 0000  ....rN...c......
-000019f0: 0000 0000 0000 0200 0000 4000 0000 7314  ..........@...s.
-00001a00: 0000 0065 005a 0164 005a 0264 0164 0284  ...e.Z.d.Z.d.d..
-00001a10: 005a 0364 0353 0029 04da 1242 6163 6b77  .Z.d.S.)...Backw
-00001a20: 6172 6446 4b52 656c 6174 696f 6e63 0300  ardFKRelationc..
-00001a30: 0000 0000 0000 0400 0000 0200 0000 4b00  ..............K.
-00001a40: 0000 7310 0000 007c 017c 005f 007c 027c  ..s....|.|._.|.|
-00001a50: 005f 0164 0053 0029 014e 2902 720d 0000  ._.d.S.).N).r...
-00001a60: 00da 0e72 656c 6174 696f 6e5f 6669 656c  ...relation_fiel
-00001a70: 6429 0472 1400 0000 720d 0000 0072 5600  d).r....r....rV.
-00001a80: 0000 7215 0000 0072 1600 0000 7216 0000  ..r....r....r...
-00001a90: 0072 1700 0000 7218 0000 00b4 0000 0073  .r....r........s
-00001aa0: 0400 0000 0001 0601 7a1b 4261 636b 7761  ........z.Backwa
-00001ab0: 7264 464b 5265 6c61 7469 6f6e 2e5f 5f69  rdFKRelation.__i
-00001ac0: 6e69 745f 5f4e 2904 721d 0000 0072 1e00  nit__N).r....r..
-00001ad0: 0000 721f 0000 0072 1800 0000 7216 0000  ..r....r....r...
-00001ae0: 0072 1600 0000 7216 0000 0072 1700 0000  .r....r....r....
-00001af0: 7255 0000 00b3 0000 0073 0200 0000 0801  rU.......s......
-00001b00: 7255 0000 0063 0000 0000 0000 0000 0000  rU...c..........
-00001b10: 0000 0300 0000 4000 0000 7388 0000 0065  ......@...s....e
-00001b20: 005a 0164 005a 0264 0164 0284 005a 0365  .Z.d.Z.d.d...Z.e
-00001b30: 0464 0364 0484 0083 015a 0564 0564 0684  .d.d.....Z.d.d..
-00001b40: 005a 0664 0764 0884 005a 0764 0964 0a84  .Z.d.d...Z.d.d..
-00001b50: 005a 0864 0b64 0c84 005a 0964 0d64 0e84  .Z.d.d...Z.d.d..
-00001b60: 005a 0a64 0f64 1084 005a 0b64 1164 1284  .Z.d.d...Z.d.d..
-00001b70: 005a 0c64 1364 1484 005a 0d64 1564 1684  .Z.d.d...Z.d.d..
-00001b80: 005a 0e64 1764 1884 005a 0f64 1964 1a84  .Z.d.d...Z.d.d..
-00001b90: 005a 1064 1b64 1c84 005a 1164 1d64 1e84  .Z.d.d...Z.d.d..
-00001ba0: 005a 1264 1f53 0029 20da 1652 656c 6174  .Z.d.S.) ..Relat
-00001bb0: 696f 6e51 7565 7279 436f 6e74 6169 6e65  ionQueryContaine
-00001bc0: 7263 0500 0000 0000 0000 0500 0000 0200  rc..............
-00001bd0: 0000 4300 0000 7328 0000 007c 017c 005f  ..C...s(...|.|._
-00001be0: 007c 027c 005f 017c 037c 005f 027c 047c  .|.|._.|.|._.|.|
-00001bf0: 005f 0364 017c 005f 0467 007c 005f 0564  ._.d.|._.g.|._.d
-00001c00: 0053 0029 024e 4629 06da 056d 6f64 656c  .S.).NF)...model
-00001c10: 7256 0000 00da 0869 6e73 7461 6e63 65da  rV.....instance.
-00001c20: 085f 6665 7463 6865 645a 0d5f 6375 7374  ._fetchedZ._cust
-00001c30: 6f6d 5f71 7565 7279 da0f 7265 6c61 7465  om_query..relate
-00001c40: 645f 6f62 6a65 6374 7329 0572 1400 0000  d_objects).r....
-00001c50: 7258 0000 0072 5600 0000 7259 0000 00da  rX...rV...rY....
-00001c60: 0669 735f 6e65 7772 1600 0000 7216 0000  .is_newr....r...
-00001c70: 0072 1700 0000 7218 0000 00ba 0000 0073  .r....r........s
-00001c80: 0c00 0000 0001 0601 0601 0601 0601 0601  ................
-00001c90: 7a1f 5265 6c61 7469 6f6e 5175 6572 7943  z.RelationQueryC
-00001ca0: 6f6e 7461 696e 6572 2e5f 5f69 6e69 745f  ontainer.__init_
-00001cb0: 5f63 0100 0000 0000 0000 0100 0000 0400  _c..............
-00001cc0: 0000 4300 0000 7328 0000 007c 006a 006a  ..C...s(...|.j.j
-00001cd0: 0173 1074 0264 0183 0182 017c 006a 036a  .s.t.d.....|.j.j
-00001ce0: 0466 007c 006a 057c 006a 006a 0169 018e  .f.|.j.|.j.j.i..
-00001cf0: 0153 0029 024e 7a4f 5468 6973 206f 626a  .S.).NzOThis obj
-00001d00: 6563 7473 2068 6173 6e27 7420 6265 656e  ects hasn't been
-00001d10: 2069 6e73 7461 6e63 6564 2c20 6361 6c6c   instanced, call
-00001d20: 202e 7361 7665 2829 2062 6566 6f72 6520   .save() before 
-00001d30: 6361 6c6c 696e 6720 7265 6c61 7465 6420  calling related 
-00001d40: 7175 6572 6965 7329 0672 5900 0000 da02  queries).rY.....
-00001d50: 6964 7249 0000 0072 5800 0000 da06 6669  idrI...rX.....fi
-00001d60: 6c74 6572 7256 0000 0029 0172 1400 0000  lterrV...).r....
-00001d70: 7216 0000 0072 1600 0000 7217 0000 00da  r....r....r.....
-00001d80: 065f 7175 6572 79c2 0000 0073 0600 0000  ._query....s....
-00001d90: 0002 0a01 0602 7a1d 5265 6c61 7469 6f6e  ......z.Relation
-00001da0: 5175 6572 7943 6f6e 7461 696e 6572 2e5f  QueryContainer._
-00001db0: 7175 6572 7963 0200 0000 0000 0000 0200  queryc..........
-00001dc0: 0000 0200 0000 4300 0000 7318 0000 007c  ......C...s....|
-00001dd0: 006a 0073 0e74 0164 0183 0182 017c 017c  .j.s.t.d.....|.|
-00001de0: 006a 026b 0653 0029 024e 7a44 4e6f 2076  .j.k.S.).NzDNo v
-00001df0: 616c 7565 7320 7765 7265 2066 6574 6368  alues were fetch
-00001e00: 6564 2066 6f72 2074 6869 7320 7265 6c61  ed for this rela
-00001e10: 7469 6f6e 2c20 6669 7273 7420 7573 6520  tion, first use 
-00001e20: 2e66 6574 6368 5f72 656c 6174 6564 2829  .fetch_related()
-00001e30: 2903 725a 0000 0072 0500 0000 725b 0000  ).rZ...r....r[..
-00001e40: 0029 0272 1400 0000 da04 6974 656d 7216  .).r......itemr.
-00001e50: 0000 0072 1600 0000 7217 0000 00da 0c5f  ...r....r......_
-00001e60: 5f63 6f6e 7461 696e 735f 5fc9 0000 0073  _contains__....s
-00001e70: 0800 0000 0001 0601 0201 0602 7a23 5265  ............z#Re
-00001e80: 6c61 7469 6f6e 5175 6572 7943 6f6e 7461  lationQueryConta
-00001e90: 696e 6572 2e5f 5f63 6f6e 7461 696e 735f  iner.__contains_
-00001ea0: 5f63 0100 0000 0000 0000 0100 0000 0200  _c..............
-00001eb0: 0000 4300 0000 7318 0000 007c 006a 0073  ..C...s....|.j.s
-00001ec0: 0e74 0164 0183 0182 017c 006a 026a 0383  .t.d.....|.j.j..
-00001ed0: 0053 0029 024e 7a44 4e6f 2076 616c 7565  .S.).NzDNo value
-00001ee0: 7320 7765 7265 2066 6574 6368 6564 2066  s were fetched f
-00001ef0: 6f72 2074 6869 7320 7265 6c61 7469 6f6e  or this relation
-00001f00: 2c20 6669 7273 7420 7573 6520 2e66 6574  , first use .fet
-00001f10: 6368 5f72 656c 6174 6564 2829 2904 725a  ch_related()).rZ
-00001f20: 0000 0072 0500 0000 725b 0000 00da 085f  ...r....r[....._
-00001f30: 5f69 7465 725f 5f29 0172 1400 0000 7216  _iter__).r....r.
-00001f40: 0000 0072 1600 0000 7217 0000 0072 6200  ...r....r....rb.
-00001f50: 0000 d000 0000 7308 0000 0000 0106 0102  ......s.........
-00001f60: 0106 027a 1f52 656c 6174 696f 6e51 7565  ...z.RelationQue
-00001f70: 7279 436f 6e74 6169 6e65 722e 5f5f 6974  ryContainer.__it
-00001f80: 6572 5f5f 6301 0000 0000 0000 0001 0000  er__c...........
-00001f90: 0002 0000 0043 0000 0073 1800 0000 7c00  .....C...s....|.
-00001fa0: 6a00 730e 7401 6401 8301 8201 7402 7c00  j.s.t.d.....t.|.
-00001fb0: 6a03 8301 5300 2902 4e7a 444e 6f20 7661  j...S.).NzDNo va
-00001fc0: 6c75 6573 2077 6572 6520 6665 7463 6865  lues were fetche
-00001fd0: 6420 666f 7220 7468 6973 2072 656c 6174  d for this relat
-00001fe0: 696f 6e2c 2066 6972 7374 2075 7365 202e  ion, first use .
-00001ff0: 6665 7463 685f 7265 6c61 7465 6428 2929  fetch_related())
-00002000: 0472 5a00 0000 7205 0000 0072 4700 0000  .rZ...r....rG...
-00002010: 725b 0000 0029 0172 1400 0000 7216 0000  r[...).r....r...
-00002020: 0072 1600 0000 7217 0000 00da 075f 5f6c  .r....r......__l
-00002030: 656e 5f5f d700 0000 7308 0000 0000 0106  en__....s.......
-00002040: 0102 0106 027a 1e52 656c 6174 696f 6e51  .....z.RelationQ
-00002050: 7565 7279 436f 6e74 6169 6e65 722e 5f5f  ueryContainer.__
-00002060: 6c65 6e5f 5f63 0100 0000 0000 0000 0100  len__c..........
-00002070: 0000 0200 0000 4300 0000 7318 0000 007c  ......C...s....|
-00002080: 006a 0073 0e74 0164 0183 0182 0174 027c  .j.s.t.d.....t.|
-00002090: 006a 0383 0153 0029 024e 7a44 4e6f 2076  .j...S.).NzDNo v
-000020a0: 616c 7565 7320 7765 7265 2066 6574 6368  alues were fetch
-000020b0: 6564 2066 6f72 2074 6869 7320 7265 6c61  ed for this rela
-000020c0: 7469 6f6e 2c20 6669 7273 7420 7573 6520  tion, first use 
-000020d0: 2e66 6574 6368 5f72 656c 6174 6564 2829  .fetch_related()
-000020e0: 2904 725a 0000 0072 0500 0000 7222 0000  ).rZ...r....r"..
-000020f0: 0072 5b00 0000 2901 7214 0000 0072 1600  .r[...).r....r..
-00002100: 0000 7216 0000 0072 1700 0000 da08 5f5f  ..r....r......__
-00002110: 626f 6f6c 5f5f de00 0000 7308 0000 0000  bool__....s.....
-00002120: 0106 0102 0106 027a 1f52 656c 6174 696f  .......z.Relatio
-00002130: 6e51 7565 7279 436f 6e74 6169 6e65 722e  nQueryContainer.
-00002140: 5f5f 626f 6f6c 5f5f 6302 0000 0000 0000  __bool__c.......
-00002150: 0002 0000 0002 0000 0043 0000 0073 1800  .........C...s..
-00002160: 0000 7c00 6a00 730e 7401 6401 8301 8201  ..|.j.s.t.d.....
-00002170: 7c00 6a02 7c01 1900 5300 2902 4e7a 444e  |.j.|...S.).NzDN
-00002180: 6f20 7661 6c75 6573 2077 6572 6520 6665  o values were fe
-00002190: 7463 6865 6420 666f 7220 7468 6973 2072  tched for this r
-000021a0: 656c 6174 696f 6e2c 2066 6972 7374 2075  elation, first u
-000021b0: 7365 202e 6665 7463 685f 7265 6c61 7465  se .fetch_relate
-000021c0: 6428 2929 0372 5a00 0000 7205 0000 0072  d()).rZ...r....r
-000021d0: 5b00 0000 2902 7214 0000 0072 6000 0000  [...).r....r`...
-000021e0: 7216 0000 0072 1600 0000 7217 0000 00da  r....r....r.....
-000021f0: 0b5f 5f67 6574 6974 656d 5f5f e500 0000  .__getitem__....
-00002200: 7308 0000 0000 0106 0102 0106 027a 2252  s............z"R
-00002210: 656c 6174 696f 6e51 7565 7279 436f 6e74  elationQueryCont
-00002220: 6169 6e65 722e 5f5f 6765 7469 7465 6d5f  ainer.__getitem_
-00002230: 5f63 0100 0000 0000 0000 0100 0000 0200  _c..............
-00002240: 0000 c300 0000 731e 0000 007c 006a 0049  ......s....|.j.I
-00002250: 0064 0048 007c 005f 0164 017c 005f 0274  .d.H.|._.d.|._.t
-00002260: 037c 006a 0183 0153 0029 024e 5429 0472  .|.j...S.).NT).r
-00002270: 5f00 0000 725b 0000 0072 5a00 0000 7206  _...r[...rZ...r.
-00002280: 0000 0029 0172 1400 0000 7216 0000 0072  ...).r....r....r
-00002290: 1600 0000 7217 0000 00da 095f 5f61 6974  ....r......__ait
-000022a0: 6572 5f5f ec00 0000 7306 0000 0000 010e  er__....s.......
-000022b0: 0106 017a 2052 656c 6174 696f 6e51 7565  ...z RelationQue
-000022c0: 7279 436f 6e74 6169 6e65 722e 5f5f 6169  ryContainer.__ai
-000022d0: 7465 725f 5f63 0100 0000 0000 0000 0300  ter__c..........
-000022e0: 0000 0300 0000 4f00 0000 730e 0000 007c  ......O...s....|
-000022f0: 006a 006a 017c 017c 028e 0153 0029 014e  .j.j.|.|...S.).N
-00002300: 2902 725f 0000 0072 5e00 0000 2903 7214  ).r_...r^...).r.
-00002310: 0000 00da 0461 7267 7372 1500 0000 7216  .....argsr....r.
-00002320: 0000 0072 1600 0000 7217 0000 0072 5e00  ...r....r....r^.
-00002330: 0000 f100 0000 7302 0000 0000 017a 1d52  ......s......z.R
-00002340: 656c 6174 696f 6e51 7565 7279 436f 6e74  elationQueryCont
-00002350: 6169 6e65 722e 6669 6c74 6572 6301 0000  ainer.filterc...
-00002360: 0000 0000 0001 0000 0001 0000 0043 0000  .............C..
-00002370: 0073 0400 0000 7c00 5300 2901 4e72 1600  .s....|.S.).Nr..
-00002380: 0000 2901 7214 0000 0072 1600 0000 7216  ..).r....r....r.
-00002390: 0000 0072 1700 0000 da03 616c 6cf4 0000  ...r......all...
-000023a0: 0073 0200 0000 0001 7a1a 5265 6c61 7469  .s......z.Relati
-000023b0: 6f6e 5175 6572 7943 6f6e 7461 696e 6572  onQueryContainer
-000023c0: 2e61 6c6c 6301 0000 0000 0000 0003 0000  .allc...........
-000023d0: 0003 0000 004f 0000 0073 0e00 0000 7c00  .....O...s....|.
-000023e0: 6a00 6a01 7c01 7c02 8e01 5300 2901 4e29  j.j.|.|...S.).N)
-000023f0: 0272 5f00 0000 da08 6f72 6465 725f 6279  .r_.....order_by
-00002400: 2903 7214 0000 0072 6700 0000 7215 0000  ).r....rg...r...
-00002410: 0072 1600 0000 7216 0000 0072 1700 0000  .r....r....r....
-00002420: 7269 0000 00f7 0000 0073 0200 0000 0001  ri.......s......
-00002430: 7a1f 5265 6c61 7469 6f6e 5175 6572 7943  z.RelationQueryC
-00002440: 6f6e 7461 696e 6572 2e6f 7264 6572 5f62  ontainer.order_b
-00002450: 7963 0100 0000 0000 0000 0300 0000 0300  yc..............
-00002460: 0000 4f00 0000 730e 0000 007c 006a 006a  ..O...s....|.j.j
-00002470: 017c 017c 028e 0153 0029 014e 2902 725f  .|.|...S.).N).r_
-00002480: 0000 00da 056c 696d 6974 2903 7214 0000  .....limit).r...
-00002490: 0072 6700 0000 7215 0000 0072 1600 0000  .rg...r....r....
-000024a0: 7216 0000 0072 1700 0000 726a 0000 00fa  r....r....rj....
-000024b0: 0000 0073 0200 0000 0001 7a1c 5265 6c61  ...s......z.Rela
-000024c0: 7469 6f6e 5175 6572 7943 6f6e 7461 696e  tionQueryContain
-000024d0: 6572 2e6c 696d 6974 6301 0000 0000 0000  er.limitc.......
-000024e0: 0003 0000 0003 0000 004f 0000 0073 0e00  .........O...s..
-000024f0: 0000 7c00 6a00 6a01 7c01 7c02 8e01 5300  ..|.j.j.|.|...S.
-00002500: 2901 4e29 0272 5f00 0000 da06 6f66 6673  ).N).r_.....offs
-00002510: 6574 2903 7214 0000 0072 6700 0000 7215  et).r....rg...r.
-00002520: 0000 0072 1600 0000 7216 0000 0072 1700  ...r....r....r..
-00002530: 0000 726b 0000 00fd 0000 0073 0200 0000  ..rk.......s....
-00002540: 0001 7a1d 5265 6c61 7469 6f6e 5175 6572  ..z.RelationQuer
-00002550: 7943 6f6e 7461 696e 6572 2e6f 6666 7365  yContainer.offse
-00002560: 7463 0100 0000 0000 0000 0300 0000 0300  tc..............
-00002570: 0000 4f00 0000 730e 0000 007c 006a 006a  ..O...s....|.j.j
-00002580: 017c 017c 028e 0153 0029 014e 2902 725f  .|.|...S.).N).r_
-00002590: 0000 00da 0864 6973 7469 6e63 7429 0372  .....distinct).r
-000025a0: 1400 0000 7267 0000 0072 1500 0000 7216  ....rg...r....r.
-000025b0: 0000 0072 1600 0000 7217 0000 0072 6c00  ...r....r....rl.
-000025c0: 0000 0001 0000 7302 0000 0000 017a 1f52  ......s......z.R
-000025d0: 656c 6174 696f 6e51 7565 7279 436f 6e74  elationQueryCont
-000025e0: 6169 6e65 722e 6469 7374 696e 6374 6302  ainer.distinctc.
-000025f0: 0000 0000 0000 0003 0000 0004 0000 0043  ...............C
-00002600: 0000 0073 2e00 0000 781c 7c01 4400 5d14  ...s....x.|.D.].
-00002610: 7d02 7400 7c02 7c00 6a01 8302 7306 7402  }.t.|.|.j...s.t.
-00002620: 8201 7106 5700 6401 7c00 5f03 7c01 7c00  ..q.W.d.|._.|.|.
-00002630: 5f04 6400 5300 2902 4e54 2905 721b 0000  _.d.S.).NT).r...
-00002640: 0072 5800 0000 7249 0000 0072 5a00 0000  .rX...rI...rZ...
-00002650: 725b 0000 0029 0372 1400 0000 da08 7365  r[...).r......se
-00002660: 7175 656e 6365 7260 0000 0072 1600 0000  quencer`...r....
-00002670: 7216 0000 0072 1700 0000 da15 5f73 6574  r....r......_set
-00002680: 5f72 6573 756c 745f 666f 725f 7175 6572  _result_for_quer
-00002690: 7903 0100 0073 0800 0000 0001 0a01 1401  y....s..........
-000026a0: 0601 7a2c 5265 6c61 7469 6f6e 5175 6572  ..z,RelationQuer
-000026b0: 7943 6f6e 7461 696e 6572 2e5f 7365 745f  yContainer._set_
-000026c0: 7265 7375 6c74 5f66 6f72 5f71 7565 7279  result_for_query
-000026d0: 4e29 1372 1d00 0000 721e 0000 0072 1f00  N).r....r....r..
-000026e0: 0000 7218 0000 00da 0870 726f 7065 7274  ..r......propert
-000026f0: 7972 5f00 0000 7261 0000 0072 6200 0000  yr_...ra...rb...
-00002700: 7263 0000 0072 6400 0000 7265 0000 0072  rc...rd...re...r
-00002710: 6600 0000 725e 0000 0072 6800 0000 7269  f...r^...rh...ri
-00002720: 0000 0072 6a00 0000 726b 0000 0072 6c00  ...rj...rk...rl.
-00002730: 0000 726e 0000 0072 1600 0000 7216 0000  ..rn...r....r...
-00002740: 0072 1600 0000 7217 0000 0072 5700 0000  .r....r....rW...
-00002750: b900 0000 731e 0000 0008 0108 080c 0708  ....s...........
-00002760: 0708 0708 0708 0708 0708 0508 0308 0308  ................
-00002770: 0308 0308 0308 0372 5700 0000 6300 0000  .......rW...c...
-00002780: 0000 0000 0000 0000 0003 0000 0000 0000  ................
-00002790: 0073 4200 0000 6500 5a01 6400 5a02 8700  .sB...e.Z.d.Z...
-000027a0: 6601 6401 6402 8408 5a03 6403 6404 9c01  f.d.d...Z.d.d...
-000027b0: 6405 6406 8402 5a04 640b 6407 6408 8401  d.d...Z.d.d.d...
-000027c0: 5a05 6403 6404 9c01 6409 640a 8402 5a06  Z.d.d...d.d...Z.
-000027d0: 8700 0400 5a07 5300 290c da19 4d61 6e79  ....Z.S.)...Many
-000027e0: 546f 4d61 6e79 5265 6c61 7469 6f6e 4d61  ToManyRelationMa
-000027f0: 6e61 6765 7263 0500 0000 0000 0000 0500  nagerc..........
-00002800: 0000 0500 0000 0300 0000 7338 0000 0074  ..........s8...t
-00002810: 0083 006a 017c 017c 036a 027c 027c 0483  ...j.|.|.j.|.|..
-00002820: 0401 007c 037c 005f 037c 036a 047c 005f  ...|.|._.|.j.|._
-00002830: 057c 027c 005f 067c 006a 056a 076a 087c  .|.|._.|.j.j.j.|
-00002840: 005f 0964 0053 0029 014e 290a 7224 0000  ._.d.S.).N).r$..
-00002850: 0072 1800 0000 724b 0000 00da 0566 6965  .r....rK.....fie
-00002860: 6c64 720d 0000 0072 5800 0000 7259 0000  ldr....rX...rY..
-00002870: 00da 055f 6d65 7461 da02 6462 da03 5f64  ..._meta..db.._d
-00002880: 6229 0572 1400 0000 7258 0000 0072 5900  b).r....rX...rY.
-00002890: 0000 5a09 6d32 6d5f 6669 656c 6472 5c00  ..Z.m2m_fieldr\.
-000028a0: 0000 2901 7226 0000 0072 1600 0000 7217  ..).r&...r....r.
-000028b0: 0000 0072 1800 0000 0b01 0000 730a 0000  ...r........s...
-000028c0: 0000 0114 0106 0108 0106 017a 224d 616e  ...........z"Man
-000028d0: 7954 6f4d 616e 7952 656c 6174 696f 6e4d  yToManyRelationM
-000028e0: 616e 6167 6572 2e5f 5f69 6e69 745f 5f4e  anager.__init__N
-000028f0: 2901 da08 7573 696e 675f 6462 6301 0000  )...using_dbc...
-00002900: 0001 0000 000c 0000 0005 0000 0087 0000  ................
-00002910: 0073 5801 0000 7c02 7308 6400 5300 7c01  .sX...|.s.d.S.|.
-00002920: 7210 7c01 6e04 8800 6a00 7d03 7401 8800  r.|.n...j.}.t...
-00002930: 6a02 6a03 8301 7d04 7c03 6a04 6a05 7c04  j.j...}.|.j.j.|.
-00002940: 8301 6a06 7407 7c04 8800 6a02 6a08 8302  ..j.t.|...j.j...
-00002950: 8800 6a09 6a0a 6b02 8301 6a0b 8800 6a02  ..j.j.k...j...j.
-00002960: 6a08 8800 6a02 6a0c 8302 7d05 7c03 6a04  j...j.j...}.|.j.
-00002970: 6a0d 7c04 8301 6a0e 7407 7c04 8800 6a02  j.|...j.t.|...j.
-00002980: 6a0c 8302 7407 7c04 8800 6a02 6a08 8302  j...t.|...j.j...
-00002990: 8302 7d06 7407 7c04 8800 6a02 6a0c 8302  ..}.t.|...j.j...
-000029a0: 7c02 6401 1900 6a0a 6b02 7d07 782c 7c02  |.d...j.k.}.x,|.
-000029b0: 6402 6400 8502 1900 4400 5d1c 7d08 7c07  d.d.....D.].}.|.
-000029c0: 7407 7c04 8800 6a02 6a0c 8302 7c08 6a0a  t.|...j.j...|.j.
-000029d0: 6b02 4f00 7d07 71a4 5700 7c05 6a06 7c07  k.O.}.q.W.|.j.|.
-000029e0: 8301 7d05 7c03 6a0f 7410 7c05 8301 8301  ..}.|.j.t.|.....
-000029f0: 4900 6400 4800 7d09 7411 8700 6601 6403  I.d.H.}.t...f.d.
-00002a00: 6404 8408 7c09 4400 8301 8301 7d0a 6405  d...|.D.....}.d.
-00002a10: 7d0b 783c 7c02 4400 5d34 7d08 8800 6a09  }.x<|.D.]4}...j.
-00002a20: 6a0a 7c08 6a0a 6602 7c0a 6b06 9001 721e  j.|.j.f.|.k...r.
-00002a30: 9001 7102 7c06 6a12 7c08 6a0a 8800 6a09  ..q.|.j.|.j...j.
-00002a40: 6a0a 8302 7d06 6406 7d0b 9001 7102 5700  j...}.d.}...q.W.
-00002a50: 7c0b 9001 7254 7c03 6a0f 7410 7c06 8301  |...rT|.j.t.|...
-00002a60: 8301 4900 6400 4800 0100 6400 5300 2907  ..I.d.H...d.S.).
-00002a70: 4e72 0100 0000 722a 0000 0063 0100 0000  Nr....r*...c....
-00002a80: 0000 0000 0200 0000 0400 0000 3300 0000  ............3...
-00002a90: 7326 0000 007c 005d 1e7d 017c 0188 006a  s&...|.].}.|...j
-00002aa0: 006a 0119 007c 0188 006a 006a 0219 0066  .j...|...j.j...f
-00002ab0: 0256 0001 0071 0264 0053 0029 014e 2903  .V...q.d.S.).N).
-00002ac0: 7271 0000 0072 5200 0000 7251 0000 0029  rq...rR...rQ...)
-00002ad0: 02da 022e 30da 0172 2901 7214 0000 0072  ....0..r).r....r
-00002ae0: 1600 0000 7217 0000 00fa 093c 6765 6e65  ....r......<gene
-00002af0: 7870 723e 2401 0000 7302 0000 0004 017a  xpr>$...s......z
-00002b00: 304d 616e 7954 6f4d 616e 7952 656c 6174  0ManyToManyRelat
-00002b10: 696f 6e4d 616e 6167 6572 2e61 6464 2e3c  ionManager.add.<
-00002b20: 6c6f 6361 6c73 3e2e 3c67 656e 6578 7072  locals>.<genexpr
-00002b30: 3e46 5429 1372 7400 0000 7203 0000 0072  >FT).rt...r....r
-00002b40: 7100 0000 7253 0000 00da 0b71 7565 7279  q...rS.....query
-00002b50: 5f63 6c61 7373 da05 6672 6f6d 5fda 0577  _class..from_..w
-00002b60: 6865 7265 da07 6765 7461 7474 7272 5200  here..getattrrR.
-00002b70: 0000 7259 0000 0072 5d00 0000 da06 7365  ..rY...r].....se
-00002b80: 6c65 6374 7251 0000 005a 0469 6e74 6fda  lectrQ...Z.into.
-00002b90: 0763 6f6c 756d 6e73 da0d 6578 6563 7574  .columns..execut
-00002ba0: 655f 7175 6572 7972 2c00 0000 da03 7365  e_queryr,.....se
-00002bb0: 74da 0669 6e73 6572 7429 0c72 1400 0000  t..insert).r....
-00002bc0: 7275 0000 00da 0969 6e73 7461 6e63 6573  ru.....instances
-00002bd0: 7273 0000 00da 0d74 6872 6f75 6768 5f74  rs.....through_t
-00002be0: 6162 6c65 5a0c 7365 6c65 6374 5f71 7565  ableZ.select_que
-00002bf0: 7279 da05 7175 6572 795a 0963 7269 7465  ry..queryZ.crite
-00002c00: 7269 6f6e 5a0f 696e 7374 616e 6365 5f74  rionZ.instance_t
-00002c10: 6f5f 6164 645a 1e61 6c72 6561 6479 5f65  o_addZ.already_e
-00002c20: 7869 7374 696e 675f 7265 6c61 7469 6f6e  xisting_relation
-00002c30: 735f 7261 775a 1a61 6c72 6561 6479 5f65  s_rawZ.already_e
-00002c40: 7869 7374 696e 675f 7265 6c61 7469 6f6e  xisting_relation
-00002c50: 735a 1269 6e73 6572 745f 6973 5f72 6571  sZ.insert_is_req
-00002c60: 7569 7265 6472 1600 0000 2901 7214 0000  uiredr....).r...
-00002c70: 0072 1700 0000 da03 6164 6412 0100 0073  .r......add....s
-00002c80: 3200 0000 0001 0401 0401 0e01 0c01 0c01  2...............
-00002c90: 1801 1001 0c01 0c01 1002 1801 1201 1c01  ................
-00002ca0: 0a02 1401 0c01 0a02 0401 0a01 1401 0401  ................
-00002cb0: 1201 0a01 0601 7a1d 4d61 6e79 546f 4d61  ......z.ManyToMa
-00002cc0: 6e79 5265 6c61 7469 6f6e 4d61 6e61 6765  nyRelationManage
-00002cd0: 722e 6164 6463 0200 0000 0000 0000 0500  r.addc..........
-00002ce0: 0000 0400 0000 c300 0000 735a 0000 007c  ..........sZ...|
-00002cf0: 0172 087c 016e 047c 006a 007d 0274 017c  .r.|.n.|.j.}.t.|
-00002d00: 006a 026a 0383 017d 037c 026a 046a 057c  .j.j...}.|.j.j.|
-00002d10: 0383 016a 0674 077c 037c 006a 026a 0883  ...j.t.|.|.j.j..
-00002d20: 027c 006a 096a 0a6b 0283 016a 0b83 007d  .|.j.j.k...j...}
-00002d30: 047c 026a 0c74 0d7c 0483 0183 0149 0064  .|.j.t.|.....I.d
-00002d40: 0048 0001 0064 0053 0029 014e 290e 7274  .H...d.S.).N).rt
-00002d50: 0000 0072 0300 0000 7271 0000 0072 5300  ...r....rq...rS.
-00002d60: 0000 7279 0000 0072 7a00 0000 727b 0000  ..ry...rz...r{..
-00002d70: 0072 7c00 0000 7252 0000 0072 5900 0000  .r|...rR...rY...
-00002d80: 725d 0000 00da 0664 656c 6574 6572 7f00  r].....deleter..
-00002d90: 0000 722c 0000 0029 0572 1400 0000 7275  ..r,...).r....ru
-00002da0: 0000 0072 7300 0000 7283 0000 0072 8400  ...rs...r....r..
-00002db0: 0000 7216 0000 0072 1600 0000 7217 0000  ..r....r....r...
-00002dc0: 00da 0563 6c65 6172 3001 0000 730a 0000  ...clear0...s...
-00002dd0: 0000 010e 010c 010c 011c 027a 1f4d 616e  ...........z.Man
-00002de0: 7954 6f4d 616e 7952 656c 6174 696f 6e4d  yToManyRelationM
-00002df0: 616e 6167 6572 2e63 6c65 6172 6301 0000  anager.clearc...
-00002e00: 0001 0000 0008 0000 0007 0000 00c7 0000  ................
-00002e10: 0073 da00 0000 7c01 7208 7c01 6e04 7c00  .s....|.r.|.n.|.
-00002e20: 6a00 7d03 7c02 7316 7401 8201 7402 7c00  j.}.|.s.t...t.|.
-00002e30: 6a03 6a04 8301 7d04 7405 7c04 7c00 6a03  j.j...}.t.|.|.j.
-00002e40: 6a06 8302 7c02 6401 1900 6a07 7405 7c04  j...|.d...j.t.|.
-00002e50: 7c00 6a03 6a08 8302 4000 0400 0300 6b02  |.j.j...@.....k.
-00002e60: 6f56 7c00 6a09 6a07 6b02 6e04 0200 0100  oV|.j.j.k.n.....
-00002e70: 7d05 784e 7c02 6402 6400 8502 1900 4400  }.xN|.d.d.....D.
-00002e80: 5d3e 7d06 7c05 7405 7c04 7c00 6a03 6a06  ]>}.|.t.|.|.j.j.
-00002e90: 8302 7c06 6a07 7405 7c04 7c00 6a03 6a08  ..|.j.t.|.|.j.j.
-00002ea0: 8302 4000 0400 0300 6b02 6fa0 7c00 6a09  ..@.....k.o.|.j.
-00002eb0: 6a07 6b02 6e04 0200 0100 4f00 7d05 716a  j.k.n.....O.}.qj
-00002ec0: 5700 7c03 6a0a 6a0b 7c04 8301 6a0c 7c05  W.|.j.j.|...j.|.
-00002ed0: 8301 6a0d 8300 7d07 7c03 6a0e 740f 7c07  ..j...}.|.j.t.|.
-00002ee0: 8301 8301 4900 6400 4800 0100 6400 5300  ....I.d.H...d.S.
-00002ef0: 2903 4e72 0100 0000 722a 0000 0029 1072  ).Nr....r*...).r
-00002f00: 7400 0000 7249 0000 0072 0300 0000 7271  t...rI...r....rq
-00002f10: 0000 0072 5300 0000 727c 0000 0072 5100  ...rS...r|...rQ.
-00002f20: 0000 725d 0000 0072 5200 0000 7259 0000  ..r]...rR...rY..
-00002f30: 0072 7900 0000 727a 0000 0072 7b00 0000  .ry...rz...r{...
-00002f40: 7286 0000 0072 7f00 0000 722c 0000 0029  r....r....r,...)
-00002f50: 0872 1400 0000 7275 0000 0072 8200 0000  .r....ru...r....
-00002f60: 7273 0000 0072 8300 0000 da09 636f 6e64  rs...r......cond
-00002f70: 6974 696f 6e5a 1269 6e73 7461 6e63 655f  itionZ.instance_
-00002f80: 746f 5f72 656d 6f76 6572 8400 0000 7216  to_remover....r.
-00002f90: 0000 0072 1600 0000 7217 0000 00da 0672  ...r....r......r
-00002fa0: 656d 6f76 6538 0100 0073 1600 0000 0001  emove8...s......
-00002fb0: 0e01 0801 0c02 1401 2602 1201 0201 1001  ........&.......
-00002fc0: 2c02 1601 7a20 4d61 6e79 546f 4d61 6e79  ,...z ManyToMany
-00002fd0: 5265 6c61 7469 6f6e 4d61 6e61 6765 722e  RelationManager.
-00002fe0: 7265 6d6f 7665 2901 4e29 0872 1d00 0000  remove).N).r....
-00002ff0: 721e 0000 0072 1f00 0000 7218 0000 0072  r....r....r....r
-00003000: 8500 0000 7287 0000 0072 8900 0000 7227  ....r....r....r'
-00003010: 0000 0072 1600 0000 7216 0000 0029 0172  ...r....r....).r
-00003020: 2600 0000 7217 0000 0072 7000 0000 0a01  &...r....rp.....
-00003030: 0000 7308 0000 0008 010c 070e 1e0a 0872  ..s............r
-00003040: 7000 0000 2902 7209 0000 0072 0a00 0000  p...).r....r....
-00003050: 2926 7234 0000 00da 0966 756e 6374 6f6f  )&r4.....functoo
-00003060: 6c73 da04 6a73 6f6e 5a07 6465 6369 6d61  ls..jsonZ.decima
-00003070: 6c72 0200 0000 5a06 7079 7069 6b61 7203  lr....Z.pypikar.
-00003080: 0000 0072 3700 0000 da13 746f 7274 6f69  ...r7.....tortoi
-00003090: 7365 2e65 7863 6570 7469 6f6e 7372 0400  se.exceptionsr..
-000030a0: 0000 7205 0000 005a 0e74 6f72 746f 6973  ..r....Z.tortois
-000030b0: 652e 7574 696c 7372 0600 0000 7207 0000  e.utilsr....r...
-000030c0: 0072 0800 0000 724c 0000 005a 0b53 4554  .r....rL...Z.SET
-000030d0: 5f44 4546 4155 4c54 da07 7061 7274 6961  _DEFAULT..partia
-000030e0: 6cda 0564 756d 7073 7242 0000 00da 056c  l..dumpsrB.....l
-000030f0: 6f61 6473 7243 0000 0072 0c00 0000 7220  oadsrC...r....r 
-00003100: 0000 0072 2800 0000 7229 0000 0072 2d00  ...r(...r)...r-.
-00003110: 0000 722e 0000 0072 2f00 0000 7233 0000  ..r....r/...r3..
-00003120: 0072 3900 0000 723b 0000 0072 3d00 0000  .r9...r;...r=...
-00003130: 7244 0000 0072 4e00 0000 7255 0000 0072  rD...rN...rU...r
-00003140: 5700 0000 7270 0000 0072 1600 0000 7216  W...rp...r....r.
-00003150: 0000 0072 1600 0000 7217 0000 00da 083c  ...r....r......<
-00003160: 6d6f 6475 6c65 3e01 0000 0073 3e00 0000  module>....s>...
-00003170: 0801 0801 0801 0c02 0c02 0801 1001 0c02  ................
-00003180: 0401 0401 0401 0403 0401 0401 0802 0603  ................
-00003190: 0e1d 1008 1005 1008 1005 1005 100b 1010  ................
-000031a0: 100a 1005 1011 100c 1017 0e06 0e51       .............Q
+00000060: 6404 6c08 6d09 5a09 6d0a 5a0a 6d0b 5a0b  d.l.m.Z.m.Z.m.Z.
+00000070: 0100 6400 6405 6c0c 6d0d 5a0d 0100 6406  ..d.d.l.m.Z...d.
+00000080: 5a0e 6407 5a0f 6408 5a10 6409 5a11 6501  Z.d.Z.d.Z.d.Z.e.
+00000090: 6a12 6502 6a13 642d 640c 8d02 5a14 6502  j.e.j.d-d...Z.e.
+000000a0: 6a15 5a16 4700 640d 640e 8400 640e 8302  j.Z.G.d.d...d...
+000000b0: 5a17 4700 640f 6410 8400 6410 6517 8303  Z.G.d.d...d.e...
+000000c0: 5a18 4700 6411 6412 8400 6412 6517 8303  Z.G.d.d...d.e...
+000000d0: 5a19 4700 6413 6414 8400 6414 6517 8303  Z.G.d.d...d.e...
+000000e0: 5a1a 4700 6415 6416 8400 6416 6517 8303  Z.G.d.d...d.e...
+000000f0: 5a1b 4700 6417 6418 8400 6418 6517 8303  Z.G.d.d...d.e...
+00000100: 5a1c 4700 6419 641a 8400 641a 6517 8303  Z.G.d.d...d.e...
+00000110: 5a1d 4700 641b 641c 8400 641c 6517 8303  Z.G.d.d...d.e...
+00000120: 5a1e 4700 641d 641e 8400 641e 6517 8303  Z.G.d.d...d.e...
+00000130: 5a1f 4700 641f 6420 8400 6420 6517 8303  Z.G.d.d ..d e...
+00000140: 5a20 4700 6421 6422 8400 6422 6517 8303  Z G.d!d"..d"e...
+00000150: 5a21 4700 6423 6424 8400 6424 6517 8303  Z!G.d#d$..d$e...
+00000160: 5a22 4700 6425 6426 8400 6426 6517 8303  Z"G.d%d&..d&e...
+00000170: 5a23 4700 6427 6428 8400 6428 8302 5a24  Z#G.d'd(..d(..Z$
+00000180: 4700 6429 642a 8400 642a 8302 5a25 4700  G.d)d*..d*..Z%G.
+00000190: 642b 642c 8400 642c 6525 8303 5a26 6401  d+d,..d,e%..Z&d.
+000001a0: 5300 292e e900 0000 004e 2901 da07 4465  S.)......N)...De
+000001b0: 6369 6d61 6c29 01da 0554 6162 6c65 2903  cimal)...Table).
+000001c0: da12 436f 6e66 6967 7572 6174 696f 6e45  ..ConfigurationE
+000001d0: 7272 6f72 da0f 4e6f 5661 6c75 6573 4665  rror..NoValuesFe
+000001e0: 7463 6865 64da 104f 7065 7261 7469 6f6e  tched..Operation
+000001f0: 616c 4572 726f 7229 01da 1251 7565 7279  alError)...Query
+00000200: 4173 796e 6349 7465 7261 746f 72da 0743  AsyncIterator..C
+00000210: 4153 4341 4445 da08 5245 5354 5249 4354  ASCADE..RESTRICT
+00000220: 7a08 5345 5420 4e55 4c4c 7a0b 5345 5420  z.SET NULLz.SET 
+00000230: 4445 4641 554c 54fa 012c fa01 3a29 015a  DEFAULT..,..:).Z
+00000240: 0a73 6570 6172 6174 6f72 7363 0000 0000  .separatorsc....
+00000250: 0000 0000 0000 0000 0700 0000 4000 0000  ............@...
+00000260: 7326 0000 0065 005a 0164 005a 0264 0964  s&...e.Z.d.Z.d.d
+00000270: 0364 0484 015a 0364 0564 0684 005a 0464  .d...Z.d.d...Z.d
+00000280: 0764 0884 005a 0564 0153 0029 0ada 0546  .d...Z.d.S.)...F
+00000290: 6965 6c64 4e46 6308 0000 0000 0000 0009  ieldNFc.........
+000002a0: 0000 0002 0000 004b 0000 0073 2e00 0000  .......K...s....
+000002b0: 7c01 7c00 5f00 7c02 7c00 5f01 7c03 7c00  |.|._.|.|._.|.|.
+000002c0: 5f02 7c04 7c00 5f03 7c06 7c00 5f04 7c05  _.|.|._.|.|._.|.
+000002d0: 7c00 5f05 7c07 7c00 5f06 6400 5300 2901  |._.|.|._.d.S.).
+000002e0: 4e29 07da 0474 7970 65da 0c73 6f75 7263  N)...type..sourc
+000002f0: 655f 6669 656c 64da 0967 656e 6572 6174  e_field..generat
+00000300: 6564 da02 706b da07 6465 6661 756c 74da  ed..pk..default.
+00000310: 046e 756c 6cda 0675 6e69 7175 6529 09da  .null..unique)..
+00000320: 0473 656c 6672 0d00 0000 720e 0000 0072  .selfr....r....r
+00000330: 0f00 0000 7210 0000 0072 1200 0000 7211  ....r....r....r.
+00000340: 0000 0072 1300 0000 da06 6b77 6172 6773  ...r......kwargs
+00000350: a900 7216 0000 00fa 432f 5573 6572 732f  ..r.....C/Users/
+00000360: 616e 6472 6579 626f 6e64 6172 2f50 7943  andreybondar/PyC
+00000370: 6861 726d 5072 6f6a 6563 7473 2f74 6f72  harmProjects/tor
+00000380: 746f 6973 652d 6f72 6d2f 746f 7274 6f69  toise-orm/tortoi
+00000390: 7365 2f66 6965 6c64 732e 7079 da08 5f5f  se/fields.py..__
+000003a0: 696e 6974 5f5f 1a00 0000 730e 0000 0000  init__....s.....
+000003b0: 0b06 0106 0106 0106 0106 0106 017a 0e46  .............z.F
+000003c0: 6965 6c64 2e5f 5f69 6e69 745f 5f63 0200  ield.__init__c..
+000003d0: 0000 0000 0000 0200 0000 0100 0000 4300  ..............C.
+000003e0: 0000 7304 0000 007c 0153 0029 014e 7216  ..s....|.S.).Nr.
+000003f0: 0000 0029 0272 1400 0000 da05 7661 6c75  ...).r......valu
+00000400: 6572 1600 0000 7216 0000 0072 1700 0000  er....r....r....
+00000410: da0b 746f 5f64 625f 7661 6c75 652d 0000  ..to_db_value-..
+00000420: 0073 0200 0000 0001 7a11 4669 656c 642e  .s......z.Field.
+00000430: 746f 5f64 625f 7661 6c75 6563 0200 0000  to_db_valuec....
+00000440: 0000 0000 0200 0000 0300 0000 4300 0000  ............C...
+00000450: 7322 0000 007c 0164 006b 0873 1474 007c  s"...|.d.k.s.t.|
+00000460: 017c 006a 0183 0272 187c 0153 007c 006a  .|.j...r.|.S.|.j
+00000470: 017c 0183 0153 0029 014e 2902 da0a 6973  .|...S.).N)...is
+00000480: 696e 7374 616e 6365 720d 0000 0029 0272  instancer....).r
+00000490: 1400 0000 7219 0000 0072 1600 0000 7216  ....r....r....r.
+000004a0: 0000 0072 1700 0000 da0f 746f 5f70 7974  ...r......to_pyt
+000004b0: 686f 6e5f 7661 6c75 6530 0000 0073 0600  hon_value0...s..
+000004c0: 0000 0001 1401 0401 7a15 4669 656c 642e  ........z.Field.
+000004d0: 746f 5f70 7974 686f 6e5f 7661 6c75 6529  to_python_value)
+000004e0: 074e 4e46 4646 4e46 2906 da08 5f5f 6e61  .NNFFFNF)...__na
+000004f0: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
+00000500: da0c 5f5f 7175 616c 6e61 6d65 5f5f 7218  ..__qualname__r.
+00000510: 0000 0072 1a00 0000 721c 0000 0072 1600  ...r....r....r..
+00000520: 0000 7216 0000 0072 1600 0000 7217 0000  ..r....r....r...
+00000530: 0072 0c00 0000 1900 0000 7312 0000 0008  .r........s.....
+00000540: 0300 0100 0100 0100 0100 0100 010a 0b08  ................
+00000550: 0372 0c00 0000 6300 0000 0000 0000 0000  .r....c.........
+00000560: 0000 0004 0000 0000 0000 0073 1e00 0000  ...........s....
+00000570: 6500 5a01 6400 5a02 6405 8700 6601 6403  e.Z.d.Z.d...f.d.
+00000580: 6404 8409 5a03 8700 0400 5a04 5300 2906  d...Z.....Z.S.).
+00000590: da08 496e 7446 6965 6c64 4e46 6303 0000  ..IntFieldNFc...
+000005a0: 0000 0000 0004 0000 0003 0000 000b 0000  ................
+000005b0: 0073 3e00 0000 7400 7c03 6a01 6401 8301  .s>...t.|.j.d...
+000005c0: 8301 7c02 4200 7c03 6401 3c00 7402 8300  ..|.B.|.d.<.t...
+000005d0: 6a03 7404 7c01 6602 7c03 8e01 0100 7c03  j.t.|.f.|.....|.
+000005e0: 6a01 6402 8301 7c00 5f05 7c02 7c00 5f06  j.d...|._.|.|._.
+000005f0: 6400 5300 2903 4e72 0f00 0000 da09 7265  d.S.).Nr......re
+00000600: 6665 7265 6e63 6529 07da 0462 6f6f 6cda  ference)...bool.
+00000610: 0367 6574 da05 7375 7065 7272 1800 0000  .get..superr....
+00000620: da03 696e 7472 2100 0000 7210 0000 0029  ..intr!...r....)
+00000630: 0472 1400 0000 720e 0000 0072 1000 0000  .r....r....r....
+00000640: 7215 0000 0029 01da 095f 5f63 6c61 7373  r....)...__class
+00000650: 5f5f 7216 0000 0072 1700 0000 7218 0000  __r....r....r...
+00000660: 0037 0000 0073 0800 0000 0001 1601 1201  .7...s..........
+00000670: 0c01 7a11 496e 7446 6965 6c64 2e5f 5f69  ..z.IntField.__i
+00000680: 6e69 745f 5f29 024e 4629 0572 1d00 0000  nit__).NF).r....
+00000690: 721e 0000 0072 1f00 0000 7218 0000 00da  r....r....r.....
+000006a0: 0d5f 5f63 6c61 7373 6365 6c6c 5f5f 7216  .__classcell__r.
+000006b0: 0000 0072 1600 0000 2901 7226 0000 0072  ...r....).r&...r
+000006c0: 1700 0000 7220 0000 0036 0000 0073 0200  ....r ...6...s..
+000006d0: 0000 0801 7220 0000 0063 0000 0000 0000  ....r ...c......
+000006e0: 0000 0000 0000 0300 0000 0000 0000 731c  ..............s.
+000006f0: 0000 0065 005a 0164 005a 0287 0066 0164  ...e.Z.d.Z...f.d
+00000700: 0164 0284 085a 0387 0004 005a 0453 0029  .d...Z.....Z.S.)
+00000710: 03da 0d53 6d61 6c6c 496e 7446 6965 6c64  ...SmallIntField
+00000720: 6301 0000 0000 0000 0002 0000 0003 0000  c...............
+00000730: 000b 0000 0073 1400 0000 7400 8300 6a01  .....s....t...j.
+00000740: 7402 6601 7c01 8e01 0100 6400 5300 2901  t.f.|.....d.S.).
+00000750: 4e29 0372 2400 0000 7218 0000 0072 2500  N).r$...r....r%.
+00000760: 0000 2902 7214 0000 0072 1500 0000 2901  ..).r....r....).
+00000770: 7226 0000 0072 1600 0000 7217 0000 0072  r&...r....r....r
+00000780: 1800 0000 3f00 0000 7302 0000 0000 017a  ....?...s......z
+00000790: 1653 6d61 6c6c 496e 7446 6965 6c64 2e5f  .SmallIntField._
+000007a0: 5f69 6e69 745f 5f29 0572 1d00 0000 721e  _init__).r....r.
+000007b0: 0000 0072 1f00 0000 7218 0000 0072 2700  ...r....r....r'.
+000007c0: 0000 7216 0000 0072 1600 0000 2901 7226  ..r....r....).r&
+000007d0: 0000 0072 1700 0000 7228 0000 003e 0000  ...r....r(...>..
+000007e0: 0073 0200 0000 0801 7228 0000 0063 0000  .s......r(...c..
+000007f0: 0000 0000 0000 0000 0000 0400 0000 0000  ................
+00000800: 0000 731e 0000 0065 005a 0164 005a 0264  ..s....e.Z.d.Z.d
+00000810: 0487 0066 0164 0264 0384 095a 0387 0004  ...f.d.d...Z....
+00000820: 005a 0453 0029 05da 0943 6861 7246 6965  .Z.S.)...CharFie
+00000830: 6c64 7201 0000 0063 0200 0000 0000 0000  ldr....c........
+00000840: 0300 0000 0300 0000 0b00 0000 7332 0000  ............s2..
+00000850: 0074 007c 0183 0164 016b 0072 1474 0164  .t.|...d.k.r.t.d
+00000860: 0283 0182 0174 007c 0183 017c 005f 0274  .....t.|...|._.t
+00000870: 0383 006a 0474 0566 017c 028e 0101 0064  ...j.t.f.|.....d
+00000880: 0053 0029 034e e901 0000 007a 176d 6178  .S.).N.....z.max
+00000890: 5f64 6967 6974 7320 6d75 7374 2062 6520  _digits must be 
+000008a0: 3e3d 2031 2906 7225 0000 0072 0400 0000  >= 1).r%...r....
+000008b0: da0a 6d61 785f 6c65 6e67 7468 7224 0000  ..max_lengthr$..
+000008c0: 0072 1800 0000 da03 7374 7229 0372 1400  .r......str).r..
+000008d0: 0000 722b 0000 0072 1500 0000 2901 7226  ..r+...r....).r&
+000008e0: 0000 0072 1600 0000 7217 0000 0072 1800  ...r....r....r..
+000008f0: 0000 4400 0000 7308 0000 0000 010c 0108  ..D...s.........
+00000900: 010a 017a 1243 6861 7246 6965 6c64 2e5f  ...z.CharField._
+00000910: 5f69 6e69 745f 5f29 0172 0100 0000 2905  _init__).r....).
+00000920: 721d 0000 0072 1e00 0000 721f 0000 0072  r....r....r....r
+00000930: 1800 0000 7227 0000 0072 1600 0000 7216  ....r'...r....r.
+00000940: 0000 0029 0172 2600 0000 7217 0000 0072  ...).r&...r....r
+00000950: 2900 0000 4300 0000 7302 0000 0008 0172  )...C...s......r
+00000960: 2900 0000 6300 0000 0000 0000 0000 0000  )...c...........
+00000970: 0003 0000 0000 0000 0073 1c00 0000 6500  .........s....e.
+00000980: 5a01 6400 5a02 8700 6601 6401 6402 8408  Z.d.Z...f.d.d...
+00000990: 5a03 8700 0400 5a04 5300 2903 da09 5465  Z.....Z.S.)...Te
+000009a0: 7874 4669 656c 6463 0100 0000 0000 0000  xtFieldc........
+000009b0: 0200 0000 0300 0000 0b00 0000 7314 0000  ............s...
+000009c0: 0074 0083 006a 0174 0266 017c 018e 0101  .t...j.t.f.|....
+000009d0: 0064 0053 0029 014e 2903 7224 0000 0072  .d.S.).N).r$...r
+000009e0: 1800 0000 722c 0000 0029 0272 1400 0000  ....r,...).r....
+000009f0: 7215 0000 0029 0172 2600 0000 7216 0000  r....).r&...r...
+00000a00: 0072 1700 0000 7218 0000 004c 0000 0073  .r....r....L...s
+00000a10: 0200 0000 0001 7a12 5465 7874 4669 656c  ......z.TextFiel
+00000a20: 642e 5f5f 696e 6974 5f5f 2905 721d 0000  d.__init__).r...
+00000a30: 0072 1e00 0000 721f 0000 0072 1800 0000  .r....r....r....
+00000a40: 7227 0000 0072 1600 0000 7216 0000 0029  r'...r....r....)
+00000a50: 0172 2600 0000 7217 0000 0072 2d00 0000  .r&...r....r-...
+00000a60: 4b00 0000 7302 0000 0008 0172 2d00 0000  K...s......r-...
+00000a70: 6300 0000 0000 0000 0000 0000 0003 0000  c...............
+00000a80: 0000 0000 0073 1c00 0000 6500 5a01 6400  .....s....e.Z.d.
+00000a90: 5a02 8700 6601 6401 6402 8408 5a03 8700  Z...f.d.d...Z...
+00000aa0: 0400 5a04 5300 2903 da0c 426f 6f6c 6561  ..Z.S.)...Boolea
+00000ab0: 6e46 6965 6c64 6301 0000 0000 0000 0002  nFieldc.........
+00000ac0: 0000 0003 0000 000b 0000 0073 1400 0000  ...........s....
+00000ad0: 7400 8300 6a01 7402 6601 7c01 8e01 0100  t...j.t.f.|.....
+00000ae0: 6400 5300 2901 4e29 0372 2400 0000 7218  d.S.).N).r$...r.
+00000af0: 0000 0072 2200 0000 2902 7214 0000 0072  ...r"...).r....r
+00000b00: 1500 0000 2901 7226 0000 0072 1600 0000  ....).r&...r....
+00000b10: 7217 0000 0072 1800 0000 5100 0000 7302  r....r....Q...s.
+00000b20: 0000 0000 017a 1542 6f6f 6c65 616e 4669  .....z.BooleanFi
+00000b30: 656c 642e 5f5f 696e 6974 5f5f 2905 721d  eld.__init__).r.
+00000b40: 0000 0072 1e00 0000 721f 0000 0072 1800  ...r....r....r..
+00000b50: 0000 7227 0000 0072 1600 0000 7216 0000  ..r'...r....r...
+00000b60: 0029 0172 2600 0000 7217 0000 0072 2e00  .).r&...r....r..
+00000b70: 0000 5000 0000 7302 0000 0008 0172 2e00  ..P...s......r..
+00000b80: 0000 6300 0000 0000 0000 0000 0000 0004  ..c.............
+00000b90: 0000 0000 0000 0073 1e00 0000 6500 5a01  .......s....e.Z.
+00000ba0: 6400 5a02 6406 8700 6601 6403 6404 8409  d.Z.d...f.d.d...
+00000bb0: 5a03 8700 0400 5a04 5300 2907 da0c 4465  Z.....Z.S.)...De
+00000bc0: 6369 6d61 6c46 6965 6c64 7201 0000 0072  cimalFieldr....r
+00000bd0: 2a00 0000 6303 0000 0000 0000 0004 0000  *...c...........
+00000be0: 0003 0000 000b 0000 0073 4800 0000 7400  .........sH...t.
+00000bf0: 7c01 8301 6401 6b00 7214 7401 6402 8301  |...d.k.r.t.d...
+00000c00: 8201 7400 7c02 8301 6403 6b00 7228 7401  ..t.|...d.k.r(t.
+00000c10: 6404 8301 8201 7402 8300 6a03 7404 6601  d.....t...j.t.f.
+00000c20: 7c03 8e01 0100 7c01 7c00 5f05 7c02 7c00  |.....|.|._.|.|.
+00000c30: 5f06 6400 5300 2905 4e72 2a00 0000 7a17  _.d.S.).Nr*...z.
+00000c40: 6d61 785f 6469 6769 7473 206d 7573 7420  max_digits must 
+00000c50: 6265 203e 3d20 3172 0100 0000 7a1b 6465  be >= 1r....z.de
+00000c60: 6369 6d61 6c5f 706c 6163 6573 206d 7573  cimal_places mus
+00000c70: 7420 6265 203e 3d20 3029 0772 2500 0000  t be >= 0).r%...
+00000c80: 7204 0000 0072 2400 0000 7218 0000 0072  r....r$...r....r
+00000c90: 0200 0000 da0a 6d61 785f 6469 6769 7473  ......max_digits
+00000ca0: da0e 6465 6369 6d61 6c5f 706c 6163 6573  ..decimal_places
+00000cb0: 2904 7214 0000 0072 3000 0000 7231 0000  ).r....r0...r1..
+00000cc0: 0072 1500 0000 2901 7226 0000 0072 1600  .r....).r&...r..
+00000cd0: 0000 7217 0000 0072 1800 0000 5600 0000  ..r....r....V...
+00000ce0: 730e 0000 0000 010c 0108 010c 0108 0110  s...............
+00000cf0: 0106 017a 1544 6563 696d 616c 4669 656c  ...z.DecimalFiel
+00000d00: 642e 5f5f 696e 6974 5f5f e9ff ffff ff29  d.__init__.....)
+00000d10: 0272 0100 0000 7232 0000 0029 0572 1d00  .r....r2...).r..
+00000d20: 0000 721e 0000 0072 1f00 0000 7218 0000  ..r....r....r...
+00000d30: 0072 2700 0000 7216 0000 0072 1600 0000  .r'...r....r....
+00000d40: 2901 7226 0000 0072 1700 0000 722f 0000  ).r&...r....r/..
+00000d50: 0055 0000 0073 0200 0000 0801 722f 0000  .U...s......r/..
+00000d60: 0063 0000 0000 0000 0000 0000 0000 0400  .c..............
+00000d70: 0000 0000 0000 7326 0000 0065 005a 0164  ......s&...e.Z.d
+00000d80: 005a 0264 0687 0066 0164 0264 0384 095a  .Z.d...f.d.d...Z
+00000d90: 0364 0464 0584 005a 0487 0004 005a 0553  .d.d...Z.....Z.S
+00000da0: 0029 07da 0d44 6174 6574 696d 6546 6965  .)...DatetimeFie
+00000db0: 6c64 4663 0300 0000 0000 0000 0400 0000  ldFc............
+00000dc0: 0300 0000 0b00 0000 7350 0000 007c 0272  ........sP...|.r
+00000dd0: 107c 0172 1074 0064 0183 0182 017c 027c  .|.r.t.d.....|.|
+00000de0: 0142 007d 0274 017c 036a 0264 0283 0183  .B.}.t.|.j.d....
+00000df0: 017c 0242 007c 0364 023c 0074 0383 006a  .|.B.|.d.<.t...j
+00000e00: 0474 056a 0566 017c 038e 0101 007c 017c  .t.j.f.|.....|.|
+00000e10: 005f 067c 027c 005f 0764 0053 0029 034e  ._.|.|._.d.S.).N
+00000e20: 7a2c 596f 7520 6361 6e20 6368 6f6f 7365  z,You can choose
+00000e30: 206f 6e6c 7920 6175 746f 5f6e 6f77 206f   only auto_now o
+00000e40: 7220 6175 746f 5f6e 6f77 5f61 6464 720f  r auto_now_addr.
+00000e50: 0000 0029 0872 0400 0000 7222 0000 0072  ...).r....r"...r
+00000e60: 2300 0000 7224 0000 0072 1800 0000 da08  #...r$...r......
+00000e70: 6461 7465 7469 6d65 da08 6175 746f 5f6e  datetime..auto_n
+00000e80: 6f77 da0c 6175 746f 5f6e 6f77 5f61 6464  ow..auto_now_add
+00000e90: 2904 7214 0000 0072 3500 0000 7236 0000  ).r....r5...r6..
+00000ea0: 0072 1500 0000 2901 7226 0000 0072 1600  .r....).r&...r..
+00000eb0: 0000 7217 0000 0072 1800 0000 6100 0000  ..r....r....a...
+00000ec0: 730e 0000 0000 0108 0108 0108 0116 0112  s...............
+00000ed0: 0106 017a 1644 6174 6574 696d 6546 6965  ...z.DatetimeFie
+00000ee0: 6c64 2e5f 5f69 6e69 745f 5f63 0200 0000  ld.__init__c....
+00000ef0: 0000 0000 0200 0000 0300 0000 4300 0000  ............C...
+00000f00: 7322 0000 007c 0164 006b 0873 1474 007c  s"...|.d.k.s.t.|
+00000f10: 017c 006a 0183 0272 187c 0153 0074 026a  .|.j...r.|.S.t.j
+00000f20: 037c 0183 0153 0029 014e 2904 721b 0000  .|...S.).N).r...
+00000f30: 0072 0d00 0000 da08 6369 736f 3836 3031  .r......ciso8601
+00000f40: da0e 7061 7273 655f 6461 7465 7469 6d65  ..parse_datetime
+00000f50: 2902 7214 0000 0072 1900 0000 7216 0000  ).r....r....r...
+00000f60: 0072 1600 0000 7217 0000 0072 1c00 0000  .r....r....r....
+00000f70: 6a00 0000 7306 0000 0000 0114 0104 017a  j...s..........z
+00000f80: 1d44 6174 6574 696d 6546 6965 6c64 2e74  .DatetimeField.t
+00000f90: 6f5f 7079 7468 6f6e 5f76 616c 7565 2902  o_python_value).
+00000fa0: 4646 2906 721d 0000 0072 1e00 0000 721f  FF).r....r....r.
+00000fb0: 0000 0072 1800 0000 721c 0000 0072 2700  ...r....r....r'.
+00000fc0: 0000 7216 0000 0072 1600 0000 2901 7226  ..r....r....).r&
+00000fd0: 0000 0072 1700 0000 7233 0000 0060 0000  ...r....r3...`..
+00000fe0: 0073 0400 0000 0801 0e09 7233 0000 0063  .s........r3...c
+00000ff0: 0000 0000 0000 0000 0000 0000 0300 0000  ................
+00001000: 0000 0000 7324 0000 0065 005a 0164 005a  ....s$...e.Z.d.Z
+00001010: 0287 0066 0164 0164 0284 085a 0364 0364  ...f.d.d...Z.d.d
+00001020: 0484 005a 0487 0004 005a 0553 0029 05da  ...Z.....Z.S.)..
+00001030: 0944 6174 6546 6965 6c64 6301 0000 0000  .DateFieldc.....
+00001040: 0000 0002 0000 0003 0000 000b 0000 0073  ...............s
+00001050: 1600 0000 7400 8300 6a01 7402 6a03 6601  ....t...j.t.j.f.
+00001060: 7c01 8e01 0100 6400 5300 2901 4e29 0472  |.....d.S.).N).r
+00001070: 2400 0000 7218 0000 0072 3400 0000 da04  $...r....r4.....
+00001080: 6461 7465 2902 7214 0000 0072 1500 0000  date).r....r....
+00001090: 2901 7226 0000 0072 1600 0000 7217 0000  ).r&...r....r...
+000010a0: 0072 1800 0000 7100 0000 7302 0000 0000  .r....q...s.....
+000010b0: 017a 1244 6174 6546 6965 6c64 2e5f 5f69  .z.DateField.__i
+000010c0: 6e69 745f 5f63 0200 0000 0000 0000 0200  nit__c..........
+000010d0: 0000 0300 0000 4300 0000 7326 0000 007c  ......C...s&...|
+000010e0: 0164 006b 0873 1474 007c 017c 006a 0183  .d.k.s.t.|.|.j..
+000010f0: 0272 187c 0153 0074 026a 037c 0183 016a  .r.|.S.t.j.|...j
+00001100: 0483 0053 0029 014e 2905 721b 0000 0072  ...S.).N).r....r
+00001110: 0d00 0000 7237 0000 0072 3800 0000 723a  ....r7...r8...r:
+00001120: 0000 0029 0272 1400 0000 7219 0000 0072  ...).r....r....r
+00001130: 1600 0000 7216 0000 0072 1700 0000 721c  ....r....r....r.
+00001140: 0000 0074 0000 0073 0600 0000 0001 1401  ...t...s........
+00001150: 0401 7a19 4461 7465 4669 656c 642e 746f  ..z.DateField.to
+00001160: 5f70 7974 686f 6e5f 7661 6c75 6529 0672  _python_value).r
+00001170: 1d00 0000 721e 0000 0072 1f00 0000 7218  ....r....r....r.
+00001180: 0000 0072 1c00 0000 7227 0000 0072 1600  ...r....r'...r..
+00001190: 0000 7216 0000 0029 0172 2600 0000 7217  ..r....).r&...r.
+000011a0: 0000 0072 3900 0000 7000 0000 7304 0000  ...r9...p...s...
+000011b0: 0008 010c 0372 3900 0000 6300 0000 0000  .....r9...c.....
+000011c0: 0000 0000 0000 0003 0000 0000 0000 0073  ...............s
+000011d0: 1c00 0000 6500 5a01 6400 5a02 8700 6601  ....e.Z.d.Z...f.
+000011e0: 6401 6402 8408 5a03 8700 0400 5a04 5300  d.d...Z.....Z.S.
+000011f0: 2903 da0a 466c 6f61 7446 6965 6c64 6301  )...FloatFieldc.
+00001200: 0000 0000 0000 0002 0000 0003 0000 000b  ................
+00001210: 0000 0073 1400 0000 7400 8300 6a01 7402  ...s....t...j.t.
+00001220: 6601 7c01 8e01 0100 6400 5300 2901 4e29  f.|.....d.S.).N)
+00001230: 0372 2400 0000 7218 0000 00da 0566 6c6f  .r$...r......flo
+00001240: 6174 2902 7214 0000 0072 1500 0000 2901  at).r....r....).
+00001250: 7226 0000 0072 1600 0000 7217 0000 0072  r&...r....r....r
+00001260: 1800 0000 7b00 0000 7302 0000 0000 017a  ....{...s......z
+00001270: 1346 6c6f 6174 4669 656c 642e 5f5f 696e  .FloatField.__in
+00001280: 6974 5f5f 2905 721d 0000 0072 1e00 0000  it__).r....r....
+00001290: 721f 0000 0072 1800 0000 7227 0000 0072  r....r....r'...r
+000012a0: 1600 0000 7216 0000 0029 0172 2600 0000  ....r....).r&...
+000012b0: 7217 0000 0072 3b00 0000 7a00 0000 7302  r....r;...z...s.
+000012c0: 0000 0008 0172 3b00 0000 6300 0000 0000  .....r;...c.....
+000012d0: 0000 0000 0000 0004 0000 0000 0000 0073  ...............s
+000012e0: 3200 0000 6500 5a01 6400 5a02 6503 6504  2...e.Z.d.Z.e.e.
+000012f0: 6602 8700 6601 6401 6402 8409 5a05 6403  f...f.d.d...Z.d.
+00001300: 6404 8400 5a06 6405 6406 8400 5a07 8700  d...Z.d.d...Z...
+00001310: 0400 5a08 5300 2907 da09 4a53 4f4e 4669  ..Z.S.)...JSONFi
+00001320: 656c 6463 0300 0000 0000 0000 0400 0000  eldc............
+00001330: 0300 0000 0b00 0000 7324 0000 0074 0083  ........s$...t..
+00001340: 006a 0174 0274 0366 0266 017c 038e 0101  .j.t.t.f.f.|....
+00001350: 007c 017c 005f 047c 027c 005f 0564 0053  .|.|._.|.|._.d.S
+00001360: 0029 014e 2906 7224 0000 0072 1800 0000  .).N).r$...r....
+00001370: da04 6469 6374 da04 6c69 7374 da07 656e  ..dict..list..en
+00001380: 636f 6465 72da 0764 6563 6f64 6572 2904  coder..decoder).
+00001390: 7214 0000 0072 4000 0000 7241 0000 0072  r....r@...rA...r
+000013a0: 1500 0000 2901 7226 0000 0072 1600 0000  ....).r&...r....
+000013b0: 7217 0000 0072 1800 0000 8000 0000 7306  r....r........s.
+000013c0: 0000 0000 0114 0106 017a 124a 534f 4e46  .........z.JSONF
+000013d0: 6965 6c64 2e5f 5f69 6e69 745f 5f63 0200  ield.__init__c..
+000013e0: 0000 0000 0000 0200 0000 0200 0000 4300  ..............C.
+000013f0: 0000 7316 0000 007c 0164 006b 0872 0c7c  ..s....|.d.k.r.|
+00001400: 0153 007c 006a 007c 0183 0153 0029 014e  .S.|.j.|...S.).N
+00001410: 2901 7240 0000 0029 0272 1400 0000 7219  ).r@...).r....r.
+00001420: 0000 0072 1600 0000 7216 0000 0072 1700  ...r....r....r..
+00001430: 0000 721a 0000 0085 0000 0073 0600 0000  ..r........s....
+00001440: 0001 0801 0401 7a15 4a53 4f4e 4669 656c  ......z.JSONFiel
+00001450: 642e 746f 5f64 625f 7661 6c75 6563 0200  d.to_db_valuec..
+00001460: 0000 0000 0000 0200 0000 0300 0000 4300  ..............C.
+00001470: 0000 7322 0000 007c 0164 006b 0873 1474  ..s"...|.d.k.s.t
+00001480: 007c 017c 006a 0183 0272 187c 0153 007c  .|.|.j...r.|.S.|
+00001490: 006a 027c 0183 0153 0029 014e 2903 721b  .j.|...S.).N).r.
+000014a0: 0000 0072 0d00 0000 7241 0000 0029 0272  ...r....rA...).r
+000014b0: 1400 0000 7219 0000 0072 1600 0000 7216  ....r....r....r.
+000014c0: 0000 0072 1700 0000 721c 0000 008a 0000  ...r....r.......
+000014d0: 0073 0600 0000 0001 1401 0401 7a19 4a53  .s..........z.JS
+000014e0: 4f4e 4669 656c 642e 746f 5f70 7974 686f  ONField.to_pytho
+000014f0: 6e5f 7661 6c75 6529 0972 1d00 0000 721e  n_value).r....r.
+00001500: 0000 0072 1f00 0000 da0a 4a53 4f4e 5f44  ...r......JSON_D
+00001510: 554d 5053 da0a 4a53 4f4e 5f4c 4f41 4453  UMPS..JSON_LOADS
+00001520: 7218 0000 0072 1a00 0000 721c 0000 0072  r....r....r....r
+00001530: 2700 0000 7216 0000 0072 1600 0000 2901  '...r....r....).
+00001540: 7226 0000 0072 1700 0000 723d 0000 007f  r&...r....r=....
+00001550: 0000 0073 0600 0000 0801 1205 0805 723d  ...s..........r=
+00001560: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+00001570: 0400 0000 0000 0000 7322 0000 0065 005a  ........s"...e.Z
+00001580: 0164 005a 0264 0165 0366 0287 0066 0164  .d.Z.d.e.f...f.d
+00001590: 0264 0384 095a 0487 0004 005a 0553 0029  .d...Z.....Z.S.)
+000015a0: 04da 0f46 6f72 6569 676e 4b65 7946 6965  ...ForeignKeyFie
+000015b0: 6c64 4e63 0400 0000 0000 0000 0500 0000  ldNc............
+000015c0: 0400 0000 0b00 0000 737e 0000 0074 0083  ........s~...t..
+000015d0: 006a 0166 007c 048e 0101 0074 027c 0174  .j.f.|.....t.|.t
+000015e0: 0383 0272 3274 047c 016a 0564 0183 0183  ...r2t.|.j.d....
+000015f0: 0164 026b 0372 3274 0664 0383 0182 017c  .d.k.r2t.d.....|
+00001600: 017c 005f 077c 027c 005f 087c 0374 0974  .|._.|.|._.|.t.t
+00001610: 0a74 0b68 036b 0772 5474 0664 0483 0182  .t.h.k.rTt.d....
+00001620: 017c 0374 0b6b 0272 7474 0c7c 046a 0d64  .|.t.k.rtt.|.j.d
+00001630: 0583 0183 010c 0072 7474 0664 0683 0182  .......rtt.d....
+00001640: 017c 037c 005f 0e64 0053 0029 074e da01  .|.|._.d.S.).N..
+00001650: 2ee9 0200 0000 7a34 466f 7265 6967 6e20  ......z4Foreign 
+00001660: 6b65 7920 6163 6365 7074 7320 6d6f 6465  key accepts mode
+00001670: 6c20 6e61 6d65 2069 6e20 666f 726d 6174  l name in format
+00001680: 2022 6170 702e 4d6f 6465 6c22 7a33 6f6e   "app.Model"z3on
+00001690: 5f64 656c 6574 6520 6361 6e20 6f6e 6c79  _delete can only
+000016a0: 2062 6520 4341 5343 4144 452c 2052 4553   be CASCADE, RES
+000016b0: 5452 4943 5420 6f72 2053 4554 5f4e 554c  TRICT or SET_NUL
+000016c0: 4c72 1200 0000 7a3c 4966 206f 6e5f 6465  Lr....z<If on_de
+000016d0: 6c65 7465 2069 7320 5345 545f 4e55 4c4c  lete is SET_NULL
+000016e0: 2c20 7468 656e 2066 6965 6c64 206d 7573  , then field mus
+000016f0: 7420 6861 7665 206e 756c 6c3d 5472 7565  t have null=True
+00001700: 2073 6574 290f 7224 0000 0072 1800 0000   set).r$...r....
+00001710: 721b 0000 0072 2c00 0000 da03 6c65 6eda  r....r,.....len.
+00001720: 0573 706c 6974 7204 0000 00da 0a6d 6f64  .splitr......mod
+00001730: 656c 5f6e 616d 65da 0c72 656c 6174 6564  el_name..related
+00001740: 5f6e 616d 6572 0800 0000 7209 0000 00da  _namer....r.....
+00001750: 0853 4554 5f4e 554c 4c72 2200 0000 7223  .SET_NULLr"...r#
+00001760: 0000 00da 096f 6e5f 6465 6c65 7465 2905  .....on_delete).
+00001770: 7214 0000 0072 4900 0000 724a 0000 0072  r....rI...rJ...r
+00001780: 4c00 0000 7215 0000 0029 0172 2600 0000  L...r....).r&...
+00001790: 7216 0000 0072 1700 0000 7218 0000 0091  r....r....r.....
+000017a0: 0000 0073 1400 0000 0001 0e01 1c01 0801  ...s............
+000017b0: 0601 0601 0e01 0801 1801 0801 7a18 466f  ............z.Fo
+000017c0: 7265 6967 6e4b 6579 4669 656c 642e 5f5f  reignKeyField.__
+000017d0: 696e 6974 5f5f 2906 721d 0000 0072 1e00  init__).r....r..
+000017e0: 0000 721f 0000 0072 0800 0000 7218 0000  ..r....r....r...
+000017f0: 0072 2700 0000 7216 0000 0072 1600 0000  .r'...r....r....
+00001800: 2901 7226 0000 0072 1700 0000 7244 0000  ).r&...r....rD..
+00001810: 0090 0000 0073 0200 0000 0801 7244 0000  .....s......rD..
+00001820: 0063 0000 0000 0000 0000 0000 0000 0400  .c..............
+00001830: 0000 0000 0000 731e 0000 0065 005a 0164  ......s....e.Z.d
+00001840: 005a 0264 0487 0066 0164 0264 0384 095a  .Z.d...f.d.d...Z
+00001850: 0387 0004 005a 0453 0029 05da 0f4d 616e  .....Z.S.)...Man
+00001860: 7954 6f4d 616e 7946 6965 6c64 4e63 0600  yToManyFieldNc..
+00001870: 0000 0000 0000 0700 0000 0300 0000 0b00  ................
+00001880: 0000 736c 0000 0074 0083 006a 0166 007c  ..sl...t...j.f.|
+00001890: 068e 0101 0074 027c 016a 0364 0183 0183  .....t.|.j.d....
+000018a0: 0164 026b 0372 2874 0464 0383 0182 017c  .d.k.r(t.d.....|
+000018b0: 017c 005f 057c 057c 005f 067c 0372 3c7c  .|._.|.|._.|.r<|
+000018c0: 036e 1664 046a 077c 016a 0364 0183 0164  .n.d.j.|.j.d...d
+000018d0: 0519 006a 0883 0083 017c 005f 097c 047c  ...j.....|._.|.|
+000018e0: 005f 0a7c 027c 005f 0b64 067c 005f 0c64  ._.|.|._.d.|._.d
+000018f0: 0053 0029 074e 7245 0000 0072 4600 0000  .S.).NrE...rF...
+00001900: 7a34 466f 7265 6967 6e20 6b65 7920 6163  z4Foreign key ac
+00001910: 6365 7074 7320 6d6f 6465 6c20 6e61 6d65  cepts model name
+00001920: 2069 6e20 666f 726d 6174 2022 6170 702e   in format "app.
+00001930: 4d6f 6465 6c22 7a05 7b7d 5f69 6472 2a00  Model"z.{}_idr*.
+00001940: 0000 4629 0d72 2400 0000 7218 0000 0072  ..F).r$...r....r
+00001950: 4700 0000 7248 0000 0072 0400 0000 7249  G...rH...r....rI
+00001960: 0000 0072 4a00 0000 da06 666f 726d 6174  ...rJ.....format
+00001970: da05 6c6f 7765 72da 0b66 6f72 7761 7264  ..lower..forward
+00001980: 5f6b 6579 da0c 6261 636b 7761 7264 5f6b  _key..backward_k
+00001990: 6579 da07 7468 726f 7567 68da 0a5f 6765  ey..through.._ge
+000019a0: 6e65 7261 7465 6429 0772 1400 0000 7249  nerated).r....rI
+000019b0: 0000 0072 5200 0000 7250 0000 0072 5100  ...rR...rP...rQ.
+000019c0: 0000 724a 0000 0072 1500 0000 2901 7226  ..rJ...r....).r&
+000019d0: 0000 0072 1600 0000 7217 0000 0072 1800  ...r....r....r..
+000019e0: 0000 9f00 0000 7314 0000 0000 090e 0112  ......s.........
+000019f0: 0108 0106 0106 010c 0116 0206 0106 017a  ...............z
+00001a00: 184d 616e 7954 6f4d 616e 7946 6965 6c64  .ManyToManyField
+00001a10: 2e5f 5f69 6e69 745f 5f29 044e 4e4e 4e29  .__init__).NNNN)
+00001a20: 0572 1d00 0000 721e 0000 0072 1f00 0000  .r....r....r....
+00001a30: 7218 0000 0072 2700 0000 7216 0000 0072  r....r'...r....r
+00001a40: 1600 0000 2901 7226 0000 0072 1700 0000  ....).r&...r....
+00001a50: 724d 0000 009e 0000 0073 0800 0000 0804  rM.......s......
+00001a60: 0001 0001 0001 724d 0000 0063 0000 0000  ......rM...c....
+00001a70: 0000 0000 0000 0000 0200 0000 4000 0000  ............@...
+00001a80: 7314 0000 0065 005a 0164 005a 0264 0164  s....e.Z.d.Z.d.d
+00001a90: 0284 005a 0364 0353 0029 04da 1242 6163  ...Z.d.S.)...Bac
+00001aa0: 6b77 6172 6446 4b52 656c 6174 696f 6e63  kwardFKRelationc
+00001ab0: 0300 0000 0000 0000 0400 0000 0200 0000  ................
+00001ac0: 4b00 0000 7310 0000 007c 017c 005f 007c  K...s....|.|._.|
+00001ad0: 027c 005f 0164 0053 0029 014e 2902 720d  .|._.d.S.).N).r.
+00001ae0: 0000 00da 0e72 656c 6174 696f 6e5f 6669  .....relation_fi
+00001af0: 656c 6429 0472 1400 0000 720d 0000 0072  eld).r....r....r
+00001b00: 5500 0000 7215 0000 0072 1600 0000 7216  U...r....r....r.
+00001b10: 0000 0072 1700 0000 7218 0000 00b6 0000  ...r....r.......
+00001b20: 0073 0400 0000 0001 0601 7a1b 4261 636b  .s........z.Back
+00001b30: 7761 7264 464b 5265 6c61 7469 6f6e 2e5f  wardFKRelation._
+00001b40: 5f69 6e69 745f 5f4e 2904 721d 0000 0072  _init__N).r....r
+00001b50: 1e00 0000 721f 0000 0072 1800 0000 7216  ....r....r....r.
+00001b60: 0000 0072 1600 0000 7216 0000 0072 1700  ...r....r....r..
+00001b70: 0000 7254 0000 00b5 0000 0073 0200 0000  ..rT.......s....
+00001b80: 0801 7254 0000 0063 0000 0000 0000 0000  ..rT...c........
+00001b90: 0000 0000 0300 0000 4000 0000 7388 0000  ........@...s...
+00001ba0: 0065 005a 0164 005a 0264 0164 0284 005a  .e.Z.d.Z.d.d...Z
+00001bb0: 0365 0464 0364 0484 0083 015a 0564 0564  .e.d.d.....Z.d.d
+00001bc0: 0684 005a 0664 0764 0884 005a 0764 0964  ...Z.d.d...Z.d.d
+00001bd0: 0a84 005a 0864 0b64 0c84 005a 0964 0d64  ...Z.d.d...Z.d.d
+00001be0: 0e84 005a 0a64 0f64 1084 005a 0b64 1164  ...Z.d.d...Z.d.d
+00001bf0: 1284 005a 0c64 1364 1484 005a 0d64 1564  ...Z.d.d...Z.d.d
+00001c00: 1684 005a 0e64 1764 1884 005a 0f64 1964  ...Z.d.d...Z.d.d
+00001c10: 1a84 005a 1064 1b64 1c84 005a 1164 1d64  ...Z.d.d...Z.d.d
+00001c20: 1e84 005a 1264 1f53 0029 20da 1652 656c  ...Z.d.S.) ..Rel
+00001c30: 6174 696f 6e51 7565 7279 436f 6e74 6169  ationQueryContai
+00001c40: 6e65 7263 0500 0000 0000 0000 0500 0000  nerc............
+00001c50: 0200 0000 4300 0000 7328 0000 007c 017c  ....C...s(...|.|
+00001c60: 005f 007c 027c 005f 017c 037c 005f 027c  ._.|.|._.|.|._.|
+00001c70: 047c 005f 0364 017c 005f 0467 007c 005f  .|._.d.|._.g.|._
+00001c80: 0564 0053 0029 024e 4629 06da 056d 6f64  .d.S.).NF)...mod
+00001c90: 656c 7255 0000 00da 0869 6e73 7461 6e63  elrU.....instanc
+00001ca0: 65da 085f 6665 7463 6865 645a 0d5f 6375  e.._fetchedZ._cu
+00001cb0: 7374 6f6d 5f71 7565 7279 da0f 7265 6c61  stom_query..rela
+00001cc0: 7465 645f 6f62 6a65 6374 7329 0572 1400  ted_objects).r..
+00001cd0: 0000 7257 0000 0072 5500 0000 7258 0000  ..rW...rU...rX..
+00001ce0: 00da 0669 735f 6e65 7772 1600 0000 7216  ...is_newr....r.
+00001cf0: 0000 0072 1700 0000 7218 0000 00bc 0000  ...r....r.......
+00001d00: 0073 0c00 0000 0001 0601 0601 0601 0601  .s..............
+00001d10: 0601 7a1f 5265 6c61 7469 6f6e 5175 6572  ..z.RelationQuer
+00001d20: 7943 6f6e 7461 696e 6572 2e5f 5f69 6e69  yContainer.__ini
+00001d30: 745f 5f63 0100 0000 0000 0000 0100 0000  t__c............
+00001d40: 0400 0000 4300 0000 7328 0000 007c 006a  ....C...s(...|.j
+00001d50: 006a 0173 1074 0264 0183 0182 017c 006a  .j.s.t.d.....|.j
+00001d60: 036a 0466 007c 006a 057c 006a 006a 0169  .j.f.|.j.|.j.j.i
+00001d70: 018e 0153 0029 024e 7a4f 5468 6973 206f  ...S.).NzOThis o
+00001d80: 626a 6563 7473 2068 6173 6e27 7420 6265  bjects hasn't be
+00001d90: 656e 2069 6e73 7461 6e63 6564 2c20 6361  en instanced, ca
+00001da0: 6c6c 202e 7361 7665 2829 2062 6566 6f72  ll .save() befor
+00001db0: 6520 6361 6c6c 696e 6720 7265 6c61 7465  e calling relate
+00001dc0: 6420 7175 6572 6965 7329 0672 5800 0000  d queries).rX...
+00001dd0: da02 6964 7206 0000 0072 5700 0000 da06  ..idr....rW.....
+00001de0: 6669 6c74 6572 7255 0000 0029 0172 1400  filterrU...).r..
+00001df0: 0000 7216 0000 0072 1600 0000 7217 0000  ..r....r....r...
+00001e00: 00da 065f 7175 6572 79c4 0000 0073 0600  ..._query....s..
+00001e10: 0000 0002 0801 0802 7a1d 5265 6c61 7469  ........z.Relati
+00001e20: 6f6e 5175 6572 7943 6f6e 7461 696e 6572  onQueryContainer
+00001e30: 2e5f 7175 6572 7963 0200 0000 0000 0000  ._queryc........
+00001e40: 0200 0000 0200 0000 4300 0000 7318 0000  ........C...s...
+00001e50: 007c 006a 0073 0e74 0164 0183 0182 017c  .|.j.s.t.d.....|
+00001e60: 017c 006a 026b 0653 0029 024e 7a44 4e6f  .|.j.k.S.).NzDNo
+00001e70: 2076 616c 7565 7320 7765 7265 2066 6574   values were fet
+00001e80: 6368 6564 2066 6f72 2074 6869 7320 7265  ched for this re
+00001e90: 6c61 7469 6f6e 2c20 6669 7273 7420 7573  lation, first us
+00001ea0: 6520 2e66 6574 6368 5f72 656c 6174 6564  e .fetch_related
+00001eb0: 2829 2903 7259 0000 0072 0500 0000 725a  ()).rY...r....rZ
+00001ec0: 0000 0029 0272 1400 0000 da04 6974 656d  ...).r......item
+00001ed0: 7216 0000 0072 1600 0000 7217 0000 00da  r....r....r.....
+00001ee0: 0c5f 5f63 6f6e 7461 696e 735f 5fcb 0000  .__contains__...
+00001ef0: 0073 0800 0000 0001 0601 0201 0602 7a23  .s............z#
+00001f00: 5265 6c61 7469 6f6e 5175 6572 7943 6f6e  RelationQueryCon
+00001f10: 7461 696e 6572 2e5f 5f63 6f6e 7461 696e  tainer.__contain
+00001f20: 735f 5f63 0100 0000 0000 0000 0100 0000  s__c............
+00001f30: 0200 0000 4300 0000 7318 0000 007c 006a  ....C...s....|.j
+00001f40: 0073 0e74 0164 0183 0182 017c 006a 026a  .s.t.d.....|.j.j
+00001f50: 0383 0053 0029 024e 7a44 4e6f 2076 616c  ...S.).NzDNo val
+00001f60: 7565 7320 7765 7265 2066 6574 6368 6564  ues were fetched
+00001f70: 2066 6f72 2074 6869 7320 7265 6c61 7469   for this relati
+00001f80: 6f6e 2c20 6669 7273 7420 7573 6520 2e66  on, first use .f
+00001f90: 6574 6368 5f72 656c 6174 6564 2829 2904  etch_related()).
+00001fa0: 7259 0000 0072 0500 0000 725a 0000 00da  rY...r....rZ....
+00001fb0: 085f 5f69 7465 725f 5f29 0172 1400 0000  .__iter__).r....
+00001fc0: 7216 0000 0072 1600 0000 7217 0000 0072  r....r....r....r
+00001fd0: 6100 0000 d200 0000 7308 0000 0000 0106  a.......s.......
+00001fe0: 0102 0106 027a 1f52 656c 6174 696f 6e51  .....z.RelationQ
+00001ff0: 7565 7279 436f 6e74 6169 6e65 722e 5f5f  ueryContainer.__
+00002000: 6974 6572 5f5f 6301 0000 0000 0000 0001  iter__c.........
+00002010: 0000 0002 0000 0043 0000 0073 1800 0000  .......C...s....
+00002020: 7c00 6a00 730e 7401 6401 8301 8201 7402  |.j.s.t.d.....t.
+00002030: 7c00 6a03 8301 5300 2902 4e7a 444e 6f20  |.j...S.).NzDNo 
+00002040: 7661 6c75 6573 2077 6572 6520 6665 7463  values were fetc
+00002050: 6865 6420 666f 7220 7468 6973 2072 656c  hed for this rel
+00002060: 6174 696f 6e2c 2066 6972 7374 2075 7365  ation, first use
+00002070: 202e 6665 7463 685f 7265 6c61 7465 6428   .fetch_related(
+00002080: 2929 0472 5900 0000 7205 0000 0072 4700  )).rY...r....rG.
+00002090: 0000 725a 0000 0029 0172 1400 0000 7216  ..rZ...).r....r.
+000020a0: 0000 0072 1600 0000 7217 0000 00da 075f  ...r....r......_
+000020b0: 5f6c 656e 5f5f d900 0000 7308 0000 0000  _len__....s.....
+000020c0: 0106 0102 0106 027a 1e52 656c 6174 696f  .......z.Relatio
+000020d0: 6e51 7565 7279 436f 6e74 6169 6e65 722e  nQueryContainer.
+000020e0: 5f5f 6c65 6e5f 5f63 0100 0000 0000 0000  __len__c........
+000020f0: 0100 0000 0200 0000 4300 0000 7318 0000  ........C...s...
+00002100: 007c 006a 0073 0e74 0164 0183 0182 0174  .|.j.s.t.d.....t
+00002110: 027c 006a 0383 0153 0029 024e 7a44 4e6f  .|.j...S.).NzDNo
+00002120: 2076 616c 7565 7320 7765 7265 2066 6574   values were fet
+00002130: 6368 6564 2066 6f72 2074 6869 7320 7265  ched for this re
+00002140: 6c61 7469 6f6e 2c20 6669 7273 7420 7573  lation, first us
+00002150: 6520 2e66 6574 6368 5f72 656c 6174 6564  e .fetch_related
+00002160: 2829 2904 7259 0000 0072 0500 0000 7222  ()).rY...r....r"
+00002170: 0000 0072 5a00 0000 2901 7214 0000 0072  ...rZ...).r....r
+00002180: 1600 0000 7216 0000 0072 1700 0000 da08  ....r....r......
+00002190: 5f5f 626f 6f6c 5f5f e000 0000 7308 0000  __bool__....s...
+000021a0: 0000 0106 0102 0106 027a 1f52 656c 6174  .........z.Relat
+000021b0: 696f 6e51 7565 7279 436f 6e74 6169 6e65  ionQueryContaine
+000021c0: 722e 5f5f 626f 6f6c 5f5f 6302 0000 0000  r.__bool__c.....
+000021d0: 0000 0002 0000 0002 0000 0043 0000 0073  ...........C...s
+000021e0: 1800 0000 7c00 6a00 730e 7401 6401 8301  ....|.j.s.t.d...
+000021f0: 8201 7c00 6a02 7c01 1900 5300 2902 4e7a  ..|.j.|...S.).Nz
+00002200: 444e 6f20 7661 6c75 6573 2077 6572 6520  DNo values were 
+00002210: 6665 7463 6865 6420 666f 7220 7468 6973  fetched for this
+00002220: 2072 656c 6174 696f 6e2c 2066 6972 7374   relation, first
+00002230: 2075 7365 202e 6665 7463 685f 7265 6c61   use .fetch_rela
+00002240: 7465 6428 2929 0372 5900 0000 7205 0000  ted()).rY...r...
+00002250: 0072 5a00 0000 2902 7214 0000 0072 5f00  .rZ...).r....r_.
+00002260: 0000 7216 0000 0072 1600 0000 7217 0000  ..r....r....r...
+00002270: 00da 0b5f 5f67 6574 6974 656d 5f5f e700  ...__getitem__..
+00002280: 0000 7308 0000 0000 0106 0102 0106 027a  ..s............z
+00002290: 2252 656c 6174 696f 6e51 7565 7279 436f  "RelationQueryCo
+000022a0: 6e74 6169 6e65 722e 5f5f 6765 7469 7465  ntainer.__getite
+000022b0: 6d5f 5f63 0100 0000 0000 0000 0200 0000  m__c............
+000022c0: 0400 0000 0300 0000 731a 0000 0087 0066  ........s......f
+000022d0: 0164 0164 0284 087d 0174 0088 006a 017c  .d.d...}.t...j.|
+000022e0: 0164 038d 0253 0029 044e 6301 0000 0000  .d...S.).Nc.....
+000022f0: 0000 0001 0000 0002 0000 0093 0000 0073  ...............s
+00002300: 1200 0000 6401 8800 5f00 7c00 6a01 8800  ....d..._.|.j...
+00002310: 5f02 6400 5300 2902 4e54 2903 7259 0000  _.d.S.).NT).rY..
+00002320: 00da 0873 6571 7565 6e63 6572 5a00 0000  ...sequencerZ...
+00002330: 2901 5a10 6974 6572 6174 6f72 5f77 7261  ).Z.iterator_wra
+00002340: 7070 6572 2901 7214 0000 0072 1600 0000  pper).r....r....
+00002350: 7217 0000 00da 1066 6574 6368 6564 5f63  r......fetched_c
+00002360: 616c 6c62 6163 6bef 0000 0073 0400 0000  allback....s....
+00002370: 0001 0601 7a3a 5265 6c61 7469 6f6e 5175  ....z:RelationQu
+00002380: 6572 7943 6f6e 7461 696e 6572 2e5f 5f61  eryContainer.__a
+00002390: 6974 6572 5f5f 2e3c 6c6f 6361 6c73 3e2e  iter__.<locals>.
+000023a0: 6665 7463 6865 645f 6361 6c6c 6261 636b  fetched_callback
+000023b0: 2901 da08 6361 6c6c 6261 636b 2902 7207  )...callback).r.
+000023c0: 0000 0072 5e00 0000 2902 7214 0000 0072  ...r^...).r....r
+000023d0: 6600 0000 7216 0000 0029 0172 1400 0000  f...r....).r....
+000023e0: 7217 0000 00da 095f 5f61 6974 6572 5f5f  r......__aiter__
+000023f0: ee00 0000 7304 0000 0000 010c 047a 2052  ....s........z R
+00002400: 656c 6174 696f 6e51 7565 7279 436f 6e74  elationQueryCont
+00002410: 6169 6e65 722e 5f5f 6169 7465 725f 5f63  ainer.__aiter__c
+00002420: 0100 0000 0000 0000 0300 0000 0300 0000  ................
+00002430: 4f00 0000 730e 0000 007c 006a 006a 017c  O...s....|.j.j.|
+00002440: 017c 028e 0153 0029 014e 2902 725e 0000  .|...S.).N).r^..
+00002450: 0072 5d00 0000 2903 7214 0000 00da 0461  .r]...).r......a
+00002460: 7267 7372 1500 0000 7216 0000 0072 1600  rgsr....r....r..
+00002470: 0000 7217 0000 0072 5d00 0000 f500 0000  ..r....r].......
+00002480: 7302 0000 0000 017a 1d52 656c 6174 696f  s......z.Relatio
+00002490: 6e51 7565 7279 436f 6e74 6169 6e65 722e  nQueryContainer.
+000024a0: 6669 6c74 6572 6301 0000 0000 0000 0001  filterc.........
+000024b0: 0000 0001 0000 0043 0000 0073 0400 0000  .......C...s....
+000024c0: 7c00 5300 2901 4e72 1600 0000 2901 7214  |.S.).Nr....).r.
+000024d0: 0000 0072 1600 0000 7216 0000 0072 1700  ...r....r....r..
+000024e0: 0000 da03 616c 6cf8 0000 0073 0200 0000  ....all....s....
+000024f0: 0001 7a1a 5265 6c61 7469 6f6e 5175 6572  ..z.RelationQuer
+00002500: 7943 6f6e 7461 696e 6572 2e61 6c6c 6301  yContainer.allc.
+00002510: 0000 0000 0000 0003 0000 0003 0000 004f  ...............O
+00002520: 0000 0073 0e00 0000 7c00 6a00 6a01 7c01  ...s....|.j.j.|.
+00002530: 7c02 8e01 5300 2901 4e29 0272 5e00 0000  |...S.).N).r^...
+00002540: da08 6f72 6465 725f 6279 2903 7214 0000  ..order_by).r...
+00002550: 0072 6900 0000 7215 0000 0072 1600 0000  .ri...r....r....
+00002560: 7216 0000 0072 1700 0000 726b 0000 00fb  r....r....rk....
+00002570: 0000 0073 0200 0000 0001 7a1f 5265 6c61  ...s......z.Rela
+00002580: 7469 6f6e 5175 6572 7943 6f6e 7461 696e  tionQueryContain
+00002590: 6572 2e6f 7264 6572 5f62 7963 0100 0000  er.order_byc....
+000025a0: 0000 0000 0300 0000 0300 0000 4f00 0000  ............O...
+000025b0: 730e 0000 007c 006a 006a 017c 017c 028e  s....|.j.j.|.|..
+000025c0: 0153 0029 014e 2902 725e 0000 00da 056c  .S.).N).r^.....l
+000025d0: 696d 6974 2903 7214 0000 0072 6900 0000  imit).r....ri...
+000025e0: 7215 0000 0072 1600 0000 7216 0000 0072  r....r....r....r
+000025f0: 1700 0000 726c 0000 00fe 0000 0073 0200  ....rl.......s..
+00002600: 0000 0001 7a1c 5265 6c61 7469 6f6e 5175  ....z.RelationQu
+00002610: 6572 7943 6f6e 7461 696e 6572 2e6c 696d  eryContainer.lim
+00002620: 6974 6301 0000 0000 0000 0003 0000 0003  itc.............
+00002630: 0000 004f 0000 0073 0e00 0000 7c00 6a00  ...O...s....|.j.
+00002640: 6a01 7c01 7c02 8e01 5300 2901 4e29 0272  j.|.|...S.).N).r
+00002650: 5e00 0000 da06 6f66 6673 6574 2903 7214  ^.....offset).r.
+00002660: 0000 0072 6900 0000 7215 0000 0072 1600  ...ri...r....r..
+00002670: 0000 7216 0000 0072 1700 0000 726d 0000  ..r....r....rm..
+00002680: 0001 0100 0073 0200 0000 0001 7a1d 5265  .....s......z.Re
+00002690: 6c61 7469 6f6e 5175 6572 7943 6f6e 7461  lationQueryConta
+000026a0: 696e 6572 2e6f 6666 7365 7463 0100 0000  iner.offsetc....
+000026b0: 0000 0000 0300 0000 0300 0000 4f00 0000  ............O...
+000026c0: 730e 0000 007c 006a 006a 017c 017c 028e  s....|.j.j.|.|..
+000026d0: 0153 0029 014e 2902 725e 0000 00da 0864  .S.).N).r^.....d
+000026e0: 6973 7469 6e63 7429 0372 1400 0000 7269  istinct).r....ri
+000026f0: 0000 0072 1500 0000 7216 0000 0072 1600  ...r....r....r..
+00002700: 0000 7217 0000 0072 6e00 0000 0401 0000  ..r....rn.......
+00002710: 7302 0000 0000 017a 1f52 656c 6174 696f  s......z.Relatio
+00002720: 6e51 7565 7279 436f 6e74 6169 6e65 722e  nQueryContainer.
+00002730: 6469 7374 696e 6374 6302 0000 0000 0000  distinctc.......
+00002740: 0003 0000 0005 0000 0043 0000 0073 3c00  .........C...s<.
+00002750: 0000 782a 7c01 4400 5d22 7d02 7400 7c02  ..x*|.D.]"}.t.|.
+00002760: 7c00 6a01 8302 7306 7402 6401 6a03 7c02  |.j...s.t.d.j.|.
+00002770: 7c00 6a01 8302 8301 0100 7106 5700 6402  |.j.......q.W.d.
+00002780: 7c00 5f04 7c01 7c00 5f05 6400 5300 2903  |._.|.|._.d.S.).
+00002790: 4e7a 0f7b 7d20 6973 206e 6f74 206f 6620  Nz.{} is not of 
+000027a0: 7b7d 5429 0672 1b00 0000 7257 0000 0072  {}T).r....rW...r
+000027b0: 0600 0000 724e 0000 0072 5900 0000 725a  ....rN...rY...rZ
+000027c0: 0000 0029 0372 1400 0000 7265 0000 0072  ...).r....re...r
+000027d0: 5f00 0000 7216 0000 0072 1600 0000 7217  _...r....r....r.
+000027e0: 0000 00da 155f 7365 745f 7265 7375 6c74  ....._set_result
+000027f0: 5f66 6f72 5f71 7565 7279 0701 0000 730a  _for_query....s.
+00002800: 0000 0000 020a 010c 0116 0206 017a 2c52  .............z,R
+00002810: 656c 6174 696f 6e51 7565 7279 436f 6e74  elationQueryCont
+00002820: 6169 6e65 722e 5f73 6574 5f72 6573 756c  ainer._set_resul
+00002830: 745f 666f 725f 7175 6572 794e 2913 721d  t_for_queryN).r.
+00002840: 0000 0072 1e00 0000 721f 0000 0072 1800  ...r....r....r..
+00002850: 0000 da08 7072 6f70 6572 7479 725e 0000  ....propertyr^..
+00002860: 0072 6000 0000 7261 0000 0072 6200 0000  .r`...ra...rb...
+00002870: 7263 0000 0072 6400 0000 7268 0000 0072  rc...rd...rh...r
+00002880: 5d00 0000 726a 0000 0072 6b00 0000 726c  ]...rj...rk...rl
+00002890: 0000 0072 6d00 0000 726e 0000 0072 6f00  ...rm...rn...ro.
+000028a0: 0000 7216 0000 0072 1600 0000 7216 0000  ..r....r....r...
+000028b0: 0072 1700 0000 7256 0000 00bb 0000 0073  .r....rV.......s
+000028c0: 1e00 0000 0801 0808 0c07 0807 0807 0807  ................
+000028d0: 0807 0807 0807 0803 0803 0803 0803 0803  ................
+000028e0: 0803 7256 0000 0063 0000 0000 0000 0000  ..rV...c........
+000028f0: 0000 0000 0300 0000 0000 0000 7342 0000  ............sB..
+00002900: 0065 005a 0164 005a 0287 0066 0164 0164  .e.Z.d.Z...f.d.d
+00002910: 0284 085a 0364 0364 049c 0164 0564 0684  ...Z.d.d...d.d..
+00002920: 025a 0464 0b64 0764 0884 015a 0564 0364  .Z.d.d.d...Z.d.d
+00002930: 049c 0164 0964 0a84 025a 0687 0004 005a  ...d.d...Z.....Z
+00002940: 0753 0029 0cda 194d 616e 7954 6f4d 616e  .S.)...ManyToMan
+00002950: 7952 656c 6174 696f 6e4d 616e 6167 6572  yRelationManager
+00002960: 6305 0000 0000 0000 0005 0000 0005 0000  c...............
+00002970: 0003 0000 0073 3800 0000 7400 8300 6a01  .....s8...t...j.
+00002980: 7c01 7c03 6a02 7c02 7c04 8304 0100 7c03  |.|.j.|.|.....|.
+00002990: 7c00 5f03 7c03 6a04 7c00 5f05 7c02 7c00  |._.|.j.|._.|.|.
+000029a0: 5f06 7c00 6a05 6a07 6a08 7c00 5f09 6400  _.|.j.j.j.|._.d.
+000029b0: 5300 2901 4e29 0a72 2400 0000 7218 0000  S.).N).r$...r...
+000029c0: 0072 4a00 0000 da05 6669 656c 6472 0d00  .rJ.....fieldr..
+000029d0: 0000 7257 0000 0072 5800 0000 da05 5f6d  ..rW...rX....._m
+000029e0: 6574 61da 0264 62da 035f 6462 2905 7214  eta..db.._db).r.
+000029f0: 0000 0072 5700 0000 7258 0000 005a 096d  ...rW...rX...Z.m
+00002a00: 326d 5f66 6965 6c64 725b 0000 0029 0172  2m_fieldr[...).r
+00002a10: 2600 0000 7216 0000 0072 1700 0000 7218  &...r....r....r.
+00002a20: 0000 0012 0100 0073 0a00 0000 0001 1401  .......s........
+00002a30: 0601 0801 0601 7a22 4d61 6e79 546f 4d61  ......z"ManyToMa
+00002a40: 6e79 5265 6c61 7469 6f6e 4d61 6e61 6765  nyRelationManage
+00002a50: 722e 5f5f 696e 6974 5f5f 4e29 01da 0875  r.__init__N)...u
+00002a60: 7369 6e67 5f64 6263 0100 0000 0100 0000  sing_dbc........
+00002a70: 0c00 0000 0500 0000 8700 0000 7358 0100  ............sX..
+00002a80: 007c 0273 0864 0053 007c 0172 107c 016e  .|.s.d.S.|.r.|.n
+00002a90: 0488 006a 007d 0374 0188 006a 026a 0383  ...j.}.t...j.j..
+00002aa0: 017d 047c 036a 046a 057c 0483 016a 0674  .}.|.j.j.|...j.t
+00002ab0: 077c 0488 006a 026a 0883 0288 006a 096a  .|...j.j.....j.j
+00002ac0: 0a6b 0283 016a 0b88 006a 026a 0888 006a  .k...j...j.j...j
+00002ad0: 026a 0c83 027d 057c 036a 046a 0d7c 0483  .j...}.|.j.j.|..
+00002ae0: 016a 0e74 077c 0488 006a 026a 0c83 0274  .j.t.|...j.j...t
+00002af0: 077c 0488 006a 026a 0883 0283 027d 0674  .|...j.j.....}.t
+00002b00: 077c 0488 006a 026a 0c83 027c 0264 0119  .|...j.j...|.d..
+00002b10: 006a 0a6b 027d 0778 2c7c 0264 0264 0085  .j.k.}.x,|.d.d..
+00002b20: 0219 0044 005d 1c7d 087c 0774 077c 0488  ...D.].}.|.t.|..
+00002b30: 006a 026a 0c83 027c 086a 0a6b 024f 007d  .j.j...|.j.k.O.}
+00002b40: 0771 a457 007c 056a 067c 0783 017d 057c  .q.W.|.j.|...}.|
+00002b50: 036a 0f74 107c 0583 0183 0149 0064 0048  .j.t.|.....I.d.H
+00002b60: 007d 0974 1187 0066 0164 0364 0484 087c  .}.t...f.d.d...|
+00002b70: 0944 0083 0183 017d 0a64 057d 0b78 3c7c  .D.....}.d.}.x<|
+00002b80: 0244 005d 347d 0888 006a 096a 0a7c 086a  .D.]4}...j.j.|.j
+00002b90: 0a66 027c 0a6b 0690 0172 1e90 0171 027c  .f.|.k...r...q.|
+00002ba0: 066a 127c 086a 0a88 006a 096a 0a83 027d  .j.|.j...j.j...}
+00002bb0: 0664 067d 0b90 0171 0257 007c 0b90 0172  .d.}...q.W.|...r
+00002bc0: 547c 036a 0f74 107c 0683 0183 0149 0064  T|.j.t.|.....I.d
+00002bd0: 0048 0001 0064 0053 0029 074e 7201 0000  .H...d.S.).Nr...
+00002be0: 0072 2a00 0000 6301 0000 0000 0000 0002  .r*...c.........
+00002bf0: 0000 0004 0000 0033 0000 0073 2600 0000  .......3...s&...
+00002c00: 7c00 5d1e 7d01 7c01 8800 6a00 6a01 1900  |.].}.|...j.j...
+00002c10: 7c01 8800 6a00 6a02 1900 6602 5600 0100  |...j.j...f.V...
+00002c20: 7102 6400 5300 2901 4e29 0372 7200 0000  q.d.S.).N).rr...
+00002c30: 7251 0000 0072 5000 0000 2902 da02 2e30  rQ...rP...)....0
+00002c40: da01 7229 0172 1400 0000 7216 0000 0072  ..r).r....r....r
+00002c50: 1700 0000 fa09 3c67 656e 6578 7072 3e2b  ......<genexpr>+
+00002c60: 0100 0073 0200 0000 0401 7a30 4d61 6e79  ...s......z0Many
+00002c70: 546f 4d61 6e79 5265 6c61 7469 6f6e 4d61  ToManyRelationMa
+00002c80: 6e61 6765 722e 6164 642e 3c6c 6f63 616c  nager.add.<local
+00002c90: 733e 2e3c 6765 6e65 7870 723e 4654 2913  s>.<genexpr>FT).
+00002ca0: 7275 0000 0072 0300 0000 7272 0000 0072  ru...r....rr...r
+00002cb0: 5200 0000 da0b 7175 6572 795f 636c 6173  R.....query_clas
+00002cc0: 73da 0566 726f 6d5f da05 7768 6572 65da  s..from_..where.
+00002cd0: 0767 6574 6174 7472 7251 0000 0072 5800  .getattrrQ...rX.
+00002ce0: 0000 725c 0000 005a 0673 656c 6563 7472  ..r\...Z.selectr
+00002cf0: 5000 0000 5a04 696e 746f da07 636f 6c75  P...Z.into..colu
+00002d00: 6d6e 73da 0d65 7865 6375 7465 5f71 7565  mns..execute_que
+00002d10: 7279 722c 0000 00da 0373 6574 da06 696e  ryr,.....set..in
+00002d20: 7365 7274 290c 7214 0000 0072 7600 0000  sert).r....rv...
+00002d30: da09 696e 7374 616e 6365 7372 7400 0000  ..instancesrt...
+00002d40: da0d 7468 726f 7567 685f 7461 626c 655a  ..through_tableZ
+00002d50: 0c73 656c 6563 745f 7175 6572 79da 0571  .select_query..q
+00002d60: 7565 7279 5a09 6372 6974 6572 696f 6e5a  ueryZ.criterionZ
+00002d70: 0f69 6e73 7461 6e63 655f 746f 5f61 6464  .instance_to_add
+00002d80: 5a1e 616c 7265 6164 795f 6578 6973 7469  Z.already_existi
+00002d90: 6e67 5f72 656c 6174 696f 6e73 5f72 6177  ng_relations_raw
+00002da0: 5a1a 616c 7265 6164 795f 6578 6973 7469  Z.already_existi
+00002db0: 6e67 5f72 656c 6174 696f 6e73 5a12 696e  ng_relationsZ.in
+00002dc0: 7365 7274 5f69 735f 7265 7175 6972 6564  sert_is_required
+00002dd0: 7216 0000 0029 0172 1400 0000 7217 0000  r....).r....r...
+00002de0: 00da 0361 6464 1901 0000 7332 0000 0000  ...add....s2....
+00002df0: 0104 0104 010e 010c 010c 0118 0110 010c  ................
+00002e00: 010c 0110 0218 0112 011c 010a 0214 010c  ................
+00002e10: 010a 0204 010a 0114 0104 0112 010a 0106  ................
+00002e20: 017a 1d4d 616e 7954 6f4d 616e 7952 656c  .z.ManyToManyRel
+00002e30: 6174 696f 6e4d 616e 6167 6572 2e61 6464  ationManager.add
+00002e40: 6302 0000 0000 0000 0005 0000 0004 0000  c...............
+00002e50: 00c3 0000 0073 5a00 0000 7c01 7208 7c01  .....sZ...|.r.|.
+00002e60: 6e04 7c00 6a00 7d02 7401 7c00 6a02 6a03  n.|.j.}.t.|.j.j.
+00002e70: 8301 7d03 7c02 6a04 6a05 7c03 8301 6a06  ..}.|.j.j.|...j.
+00002e80: 7407 7c03 7c00 6a02 6a08 8302 7c00 6a09  t.|.|.j.j...|.j.
+00002e90: 6a0a 6b02 8301 6a0b 8300 7d04 7c02 6a0c  j.k...j...}.|.j.
+00002ea0: 740d 7c04 8301 8301 4900 6400 4800 0100  t.|.....I.d.H...
+00002eb0: 6400 5300 2901 4e29 0e72 7500 0000 7203  d.S.).N).ru...r.
+00002ec0: 0000 0072 7200 0000 7252 0000 0072 7a00  ...rr...rR...rz.
+00002ed0: 0000 727b 0000 0072 7c00 0000 727d 0000  ..r{...r|...r}..
+00002ee0: 0072 5100 0000 7258 0000 0072 5c00 0000  .rQ...rX...r\...
+00002ef0: da06 6465 6c65 7465 727f 0000 0072 2c00  ..deleter....r,.
+00002f00: 0000 2905 7214 0000 0072 7600 0000 7274  ..).r....rv...rt
+00002f10: 0000 0072 8300 0000 7284 0000 0072 1600  ...r....r....r..
+00002f20: 0000 7216 0000 0072 1700 0000 da05 636c  ..r....r......cl
+00002f30: 6561 7237 0100 0073 0a00 0000 0001 0e01  ear7...s........
+00002f40: 0c01 0c01 1c02 7a1f 4d61 6e79 546f 4d61  ......z.ManyToMa
+00002f50: 6e79 5265 6c61 7469 6f6e 4d61 6e61 6765  nyRelationManage
+00002f60: 722e 636c 6561 7263 0100 0000 0100 0000  r.clearc........
+00002f70: 0800 0000 0700 0000 c700 0000 73de 0000  ............s...
+00002f80: 007c 0172 087c 016e 047c 006a 007d 037c  .|.r.|.n.|.j.}.|
+00002f90: 0273 1a74 0164 0183 0182 0174 027c 006a  .s.t.d.....t.|.j
+00002fa0: 036a 0483 017d 0474 057c 047c 006a 036a  .j...}.t.|.|.j.j
+00002fb0: 0683 027c 0264 0219 006a 0774 057c 047c  ...|.d...j.t.|.|
+00002fc0: 006a 036a 0883 0240 0004 0003 006b 026f  .j.j...@.....k.o
+00002fd0: 5a7c 006a 096a 076b 026e 0402 0001 007d  Z|.j.j.k.n.....}
+00002fe0: 0578 4e7c 0264 0364 0085 0219 0044 005d  .xN|.d.d.....D.]
+00002ff0: 3e7d 067c 0574 057c 047c 006a 036a 0683  >}.|.t.|.|.j.j..
+00003000: 027c 066a 0774 057c 047c 006a 036a 0883  .|.j.t.|.|.j.j..
+00003010: 0240 0004 0003 006b 026f a47c 006a 096a  .@.....k.o.|.j.j
+00003020: 076b 026e 0402 0001 004f 007d 0571 6e57  .k.n.....O.}.qnW
+00003030: 007c 036a 0a6a 0b7c 0483 016a 0c7c 0583  .|.j.j.|...j.|..
+00003040: 016a 0d83 007d 077c 036a 0e74 0f7c 0783  .j...}.|.j.t.|..
+00003050: 0183 0149 0064 0048 0001 0064 0053 0029  ...I.d.H...d.S.)
+00003060: 044e 7a1f 7265 6d6f 7665 2829 2063 616c  .Nz.remove() cal
+00003070: 6c65 6420 6f6e 206e 6f20 696e 7374 616e  led on no instan
+00003080: 6365 7372 0100 0000 722a 0000 0029 1072  cesr....r*...).r
+00003090: 7500 0000 7206 0000 0072 0300 0000 7272  u...r....r....rr
+000030a0: 0000 0072 5200 0000 727d 0000 0072 5000  ...rR...r}...rP.
+000030b0: 0000 725c 0000 0072 5100 0000 7258 0000  ..r\...rQ...rX..
+000030c0: 0072 7a00 0000 727b 0000 0072 7c00 0000  .rz...r{...r|...
+000030d0: 7286 0000 0072 7f00 0000 722c 0000 0029  r....r....r,...)
+000030e0: 0872 1400 0000 7276 0000 0072 8200 0000  .r....rv...r....
+000030f0: 7274 0000 0072 8300 0000 5a09 636f 6e64  rt...r....Z.cond
+00003100: 6974 696f 6e5a 1269 6e73 7461 6e63 655f  itionZ.instance_
+00003110: 746f 5f72 656d 6f76 6572 8400 0000 7216  to_remover....r.
+00003120: 0000 0072 1600 0000 7217 0000 00da 0672  ...r....r......r
+00003130: 656d 6f76 653f 0100 0073 1800 0000 0001  emove?...s......
+00003140: 0e01 0401 0801 0c02 1401 2602 1201 0201  ..........&.....
+00003150: 1001 2c02 1601 7a20 4d61 6e79 546f 4d61  ..,...z ManyToMa
+00003160: 6e79 5265 6c61 7469 6f6e 4d61 6e61 6765  nyRelationManage
+00003170: 722e 7265 6d6f 7665 2901 4e29 0872 1d00  r.remove).N).r..
+00003180: 0000 721e 0000 0072 1f00 0000 7218 0000  ..r....r....r...
+00003190: 0072 8500 0000 7287 0000 0072 8800 0000  .r....r....r....
+000031a0: 7227 0000 0072 1600 0000 7216 0000 0029  r'...r....r....)
+000031b0: 0172 2600 0000 7217 0000 0072 7100 0000  .r&...r....rq...
+000031c0: 1101 0000 7308 0000 0008 010c 070e 1e0a  ....s...........
+000031d0: 0872 7100 0000 2902 720a 0000 0072 0b00  .rq...).r....r..
+000031e0: 0000 2927 7234 0000 00da 0966 756e 6374  ..)'r4.....funct
+000031f0: 6f6f 6c73 5a04 6a73 6f6e 5a07 6465 6369  oolsZ.jsonZ.deci
+00003200: 6d61 6c72 0200 0000 5a06 7079 7069 6b61  malr....Z.pypika
+00003210: 7203 0000 0072 3700 0000 da13 746f 7274  r....r7.....tort
+00003220: 6f69 7365 2e65 7863 6570 7469 6f6e 7372  oise.exceptionsr
+00003230: 0400 0000 7205 0000 0072 0600 0000 da0e  ....r....r......
+00003240: 746f 7274 6f69 7365 2e75 7469 6c73 7207  tortoise.utilsr.
+00003250: 0000 0072 0800 0000 7209 0000 0072 4b00  ...r....r....rK.
+00003260: 0000 5a0b 5345 545f 4445 4641 554c 54da  ..Z.SET_DEFAULT.
+00003270: 0770 6172 7469 616c da05 6475 6d70 7372  .partial..dumpsr
+00003280: 4200 0000 da05 6c6f 6164 7372 4300 0000  B.....loadsrC...
+00003290: 720c 0000 0072 2000 0000 7228 0000 0072  r....r ...r(...r
+000032a0: 2900 0000 722d 0000 0072 2e00 0000 722f  )...r-...r....r/
+000032b0: 0000 0072 3300 0000 7239 0000 0072 3b00  ...r3...r9...r;.
+000032c0: 0000 723d 0000 0072 4400 0000 724d 0000  ..r=...rD...rM..
+000032d0: 0072 5400 0000 7256 0000 0072 7100 0000  .rT...rV...rq...
+000032e0: 7216 0000 0072 1600 0000 7216 0000 0072  r....r....r....r
+000032f0: 1700 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
+00003300: 0000 733e 0000 0008 0108 0108 010c 020c  ..s>............
+00003310: 0208 0114 010c 0204 0104 0104 0104 0304  ................
+00003320: 0104 0108 0206 030e 1d10 0810 0510 0810  ................
+00003330: 0510 0510 0b10 1010 0a10 0510 1110 0e10  ................
+00003340: 170e 060e 56                             ....V
```

### Comparing `tortoise-orm-0.9.2/tortoise/contrib/pylint/__init__.py` & `tortoise-orm-0.9.4/tortoise/contrib/pylint/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """
 Tortoise PyLint plugin
 """
-import astroid
 from astroid import MANAGER, inference_tip, nodes, scoped_nodes
 from astroid.node_classes import Assign
 from astroid.nodes import ClassDef
 
 MODELS = {}  # type: dict
 FUTURE_RELATIONS = {}  # type: dict
 
@@ -38,15 +37,15 @@
         for mcls in cls.get_children():
             if isinstance(mcls, ClassDef):
                 for attr in mcls.get_children():
                     if isinstance(attr, Assign):
                         if attr.targets[0].name == 'app':
                             appname = attr.value.value
 
-        mname = '%s.%s' % (appname, cls.name)
+        mname = '{}.{}'.format(appname, cls.name)
         MODELS[mname] = cls
 
         for relname, relval in FUTURE_RELATIONS.get(mname, []):
             cls.locals[relname] = relval
 
         for attr in cls.get_children():
             if isinstance(attr, Assign):
@@ -54,17 +53,18 @@
                     attrname = attr.value.func.attrname
                 except AttributeError:
                     pass
                 else:
                     if attrname in ['ForeignKeyField', 'ManyToManyField']:
                         tomodel = attr.value.args[0].value
                         relname = ''
-                        for keyword in attr.value.keywords:
-                            if keyword.arg == 'related_name':
-                                relname = keyword.value.value
+                        if attr.value.keywords:
+                            for keyword in attr.value.keywords:
+                                if keyword.arg == 'related_name':
+                                    relname = keyword.value.value
 
                         if relname:
                             # Injected model attributes need to also have the relation manager
                             if attrname == 'ManyToManyField':
                                 relval = [
                                     attr.value.func,
                                     MANAGER.ast_from_module_name('tortoise.fields')
@@ -82,15 +82,15 @@
                             else:
                                 FUTURE_RELATIONS.setdefault(tomodel, []).append((relname, relval))
 
     cls.locals['_meta'] = [
         MANAGER.ast_from_module_name('tortoise.models').lookup('MetaInfo')[1][0].instantiate_class()
     ]
     if 'id' not in cls.locals:
-        cls.locals['id'] = [astroid.Class('id', None)]
+        cls.locals['id'] = [nodes.ClassDef('id', None)]
 
 
 def is_model_field(cls):
     """
     Guard to apply this transform to Model Fields only
     """
     return cls.qname().startswith('tortoise.fields')
@@ -121,9 +121,9 @@
                                                   ).lookup('ManyToManyRelationManager')
     else:
         return iter([cls])
 
     return iter([cls] + base_nodes[1])
 
 
-MANAGER.register_transform(nodes.Class, inference_tip(apply_type_shim), is_model_field)
-MANAGER.register_transform(astroid.Class, transform_model, is_model)
+MANAGER.register_transform(nodes.ClassDef, inference_tip(apply_type_shim), is_model_field)
+MANAGER.register_transform(nodes.ClassDef, transform_model, is_model)
```

### Comparing `tortoise-orm-0.9.2/tortoise/contrib/test/__pycache__/__init__.cpython-36.pyc` & `tortoise-orm-0.9.4/tortoise/contrib/test/__pycache__/__init__.cpython-37.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.6 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 18% similar despite different names*

```diff
@@ -1,140 +1,140 @@
-00000000: 330d 0d0a 7781 3c5b 1c08 0000 e300 0000  3...w.<[........
-00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 6c00 0000 6400 6401 6c00 5a00 6400  .sl...d.d.l.Z.d.
-00000030: 6401 6c01 5a01 6400 6401 6c02 5a02 6400  d.l.Z.d.d.l.Z.d.
-00000040: 6402 6c03 6d04 5a04 0100 6400 6403 6c05  d.l.m.Z...d.d.l.
-00000050: 6d06 5a06 0100 6400 6404 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
-00000060: 0100 6400 6405 6c09 6d0a 5a0a 0100 6501  ..d.d.l.m.Z...e.
-00000070: 6a0b 6a0c 6406 6407 8302 5a0d 4700 6408  j.j.d.d...Z.G.d.
-00000080: 6409 8400 6409 6502 6a0e 8303 5a0e 6401  d...d.e.j...Z.d.
-00000090: 5300 290a e900 0000 004e 2901 da08 546f  S.)......N)...To
-000000a0: 7274 6f69 7365 2901 da11 4261 7365 4442  rtoise)...BaseDB
-000000b0: 4173 796e 6343 6c69 656e 7429 01da 0d65  AsyncClient)...e
-000000c0: 7870 616e 645f 6462 5f75 726c 2901 da0f  xpand_db_url)...
-000000d0: 6765 6e65 7261 7465 5f73 6368 656d 61da  generate_schema.
-000000e0: 1054 4f52 544f 4953 455f 5445 5354 5f44  .TORTOISE_TEST_D
-000000f0: 427a 1c73 716c 6974 653a 2f2f 2f74 6d70  Bz.sqlite:///tmp
-00000100: 2f74 6573 742d 7b7d 2e73 716c 6974 6563  /test-{}.sqlitec
-00000110: 0000 0000 0000 0000 0000 0000 0300 0000  ................
-00000120: 4000 0000 7350 0000 0065 005a 0164 005a  @...sP...e.Z.d.Z
-00000130: 0264 015a 0365 0464 029c 0164 0364 0484  .d.Z.e.d...d.d..
-00000140: 045a 0564 0564 0684 005a 0664 0764 029c  .Z.d.d...Z.d.d..
-00000150: 0164 0864 0984 045a 0764 0764 029c 0164  .d.d...Z.d.d...d
-00000160: 0a64 0b84 045a 0864 0764 029c 0164 0c64  .d...Z.d.d...d.d
-00000170: 0d84 045a 0964 0753 0029 0eda 0854 6573  ...Z.d.S.)...Tes
-00000180: 7443 6173 657a 8e0a 2020 2020 416e 2061  tCasez..    An a
-00000190: 7379 6e63 696f 2063 6170 6162 6c65 2054  syncio capable T
-000001a0: 6573 7443 6173 6520 7468 6174 2077 696c  estCase that wil
-000001b0: 6c20 656e 7375 7265 2074 6861 7420 616e  l ensure that an
-000001c0: 2069 736f 6c61 7465 6420 7465 7374 2064   isolated test d
-000001d0: 620a 2020 2020 2020 6973 2061 7661 696c  b.      is avail
-000001e0: 6162 6c65 2066 6f72 2065 6163 6820 7465  able for each te
-000001f0: 7374 2e0a 0a20 2020 2042 6173 6564 206f  st...    Based o
-00000200: 6e20 6060 6173 796e 6374 6573 7460 602e  n ``asynctest``.
-00000210: 0a20 2020 2029 01da 0672 6574 7572 6e63  .    )...returnc
-00000220: 0100 0000 0000 0000 0300 0000 0400 0000  ................
-00000230: c300 0000 733e 0000 0074 0074 0164 0164  ....s>...t.t.d.d
-00000240: 028d 027d 017c 0164 0319 0066 007c 0164  ...}.|.d...f.|.d
-00000250: 0419 008e 017d 027c 026a 0283 0049 0064  .....}.|.j...I.d
-00000260: 0048 0001 007c 026a 0383 0049 0064 0048  .H...|.j...I.d.H
-00000270: 0001 007c 0253 0029 054e 5429 01da 0774  ...|.S.).NT)...t
-00000280: 6573 7469 6e67 da06 636c 6965 6e74 da06  esting..client..
-00000290: 7061 7261 6d73 2904 7204 0000 0072 0600  params).r....r..
-000002a0: 0000 da09 6462 5f63 7265 6174 65da 1163  ....db_create..c
-000002b0: 7265 6174 655f 636f 6e6e 6563 7469 6f6e  reate_connection
-000002c0: 2903 da04 7365 6c66 5a06 6462 636f 6e66  )...selfZ.dbconf
-000002d0: da02 6462 a900 7210 0000 00fa 522f 5573  ..db..r.....R/Us
-000002e0: 6572 732f 616e 6472 6579 626f 6e64 6172  ers/andreybondar
-000002f0: 2f50 7943 6861 726d 5072 6f6a 6563 7473  /PyCharmProjects
-00000300: 2f74 6f72 746f 6973 652d 6f72 6d2f 746f  /tortoise-orm/to
-00000310: 7274 6f69 7365 2f63 6f6e 7472 6962 2f74  rtoise/contrib/t
-00000320: 6573 742f 5f5f 696e 6974 5f5f 2e70 79da  est/__init__.py.
-00000330: 0567 6574 4442 1700 0000 730a 0000 0000  .getDB....s.....
-00000340: 010c 0112 010e 010e 027a 0e54 6573 7443  .........z.TestC
-00000350: 6173 652e 6765 7444 4263 0100 0000 0000  ase.getDBc......
-00000360: 0000 0100 0000 0200 0000 c300 0000 7344  ..............sD
-00000370: 0000 007c 006a 0083 0049 0064 0048 007c  ...|.j...I.d.H.|
-00000380: 005f 0174 026a 0373 2474 026a 047c 006a  ._.t.j.s$t.j.|.j
-00000390: 0183 0101 006e 0c74 026a 057c 006a 0183  .....n.t.j.|.j..
-000003a0: 0101 0074 067c 006a 0183 0149 0064 0048  ...t.|.j...I.d.H
-000003b0: 0001 0064 0053 0029 014e 2907 7212 0000  ...d.S.).N).r...
-000003c0: 0072 0f00 0000 7202 0000 00da 075f 696e  .r....r......_in
-000003d0: 6974 6564 da04 696e 6974 da0f 5f63 6c69  ited..init.._cli
-000003e0: 656e 745f 726f 7574 696e 6772 0500 0000  ent_routingr....
-000003f0: 2901 720e 0000 0072 1000 0000 7210 0000  ).r....r....r...
-00000400: 0072 1100 0000 da08 5f73 6574 5570 4442  .r......_setUpDB
-00000410: 1f00 0000 730a 0000 0000 0110 0106 010e  ....s...........
-00000420: 020c 017a 1154 6573 7443 6173 652e 5f73  ...z.TestCase._s
-00000430: 6574 5570 4442 4e63 0100 0000 0000 0000  etUpDBNc........
-00000440: 0100 0000 0200 0000 c300 0000 7324 0000  ............s$..
-00000450: 007c 006a 006a 0183 0049 0064 0048 0001  .|.j.j...I.d.H..
-00000460: 007c 006a 006a 0283 0049 0064 0048 0001  .|.j.j...I.d.H..
-00000470: 0064 0053 0029 014e 2903 720f 0000 00da  .d.S.).N).r.....
-00000480: 0563 6c6f 7365 da09 6462 5f64 656c 6574  .close..db_delet
-00000490: 6529 0172 0e00 0000 7210 0000 0072 1000  e).r....r....r..
-000004a0: 0000 7211 0000 00da 0b5f 7465 6172 446f  ..r......_tearDo
-000004b0: 776e 4442 2700 0000 7304 0000 0000 0110  wnDB'...s.......
-000004c0: 017a 1454 6573 7443 6173 652e 5f74 6561  .z.TestCase._tea
-000004d0: 7244 6f77 6e44 4263 0100 0000 0000 0000  rDownDBc........
-000004e0: 0300 0000 0400 0000 4300 0000 7382 0000  ........C...s...
-000004f0: 007c 006a 0083 0001 0074 017c 007c 006a  .|.j.....t.|.|.j
-00000500: 0283 027d 0174 017c 0174 036a 046a 0564  ...}.t.|.t.j.j.d
-00000510: 0083 037d 027c 0270 3074 036a 046a 0483  ...}.|.p0t.j.j..
-00000520: 007c 005f 067c 006a 066a 077c 0083 0101  .|._.|.j.j.|....
-00000530: 007c 006a 086a 097c 006a 0a83 0083 0101  .|.j.j.|.j......
-00000540: 0074 0b6a 0c7c 006a 0d83 0172 6e7c 006a  .t.j.|.j...rn|.j
-00000550: 086a 097c 006a 0d83 0083 0101 006e 087c  .j.|.j.......n.|
-00000560: 006a 0d83 0001 0064 017c 006a 085f 0e64  .j.....d.|.j._.d
-00000570: 0053 0029 024e 4629 0f5a 0a5f 696e 6974  .S.).NF).Z._init
-00000580: 5f6c 6f6f 70da 0767 6574 6174 7472 da0f  _loop..getattr..
-00000590: 5f74 6573 744d 6574 686f 644e 616d 65da  _testMethodName.
-000005a0: 0961 7379 6e63 7465 7374 5a08 5f66 6169  .asynctestZ._fai
-000005b0: 6c5f 6f6e 5a0d 5f46 4149 4c5f 4f4e 5f41  l_onZ._FAIL_ON_A
-000005c0: 5454 52da 085f 6368 6563 6b65 725a 0b62  TTR.._checkerZ.b
-000005d0: 6566 6f72 655f 7465 7374 da04 6c6f 6f70  efore_test..loop
-000005e0: da12 7275 6e5f 756e 7469 6c5f 636f 6d70  ..run_until_comp
-000005f0: 6c65 7465 7216 0000 00da 0761 7379 6e63  leter......async
-00000600: 696f da13 6973 636f 726f 7574 696e 6566  io..iscoroutinef
-00000610: 756e 6374 696f 6eda 0573 6574 5570 5a0e  unction..setUpZ.
-00000620: 5f61 7379 6e63 7465 7374 5f72 616e 2903  _asynctest_ran).
-00000630: 720e 0000 00da 0474 6573 74da 0763 6865  r......test..che
-00000640: 636b 6572 7210 0000 0072 1000 0000 7211  ckerr....r....r.
-00000650: 0000 00da 065f 7365 7455 702b 0000 0073  ....._setUp+...s
-00000660: 1400 0000 0001 0803 0c01 1001 1001 0c02  ................
-00000670: 1001 0c01 1202 0803 7a0f 5465 7374 4361  ........z.TestCa
-00000680: 7365 2e5f 7365 7455 7063 0100 0000 0000  se._setUpc......
-00000690: 0000 0100 0000 0200 0000 4300 0000 7346  ..........C...sF
-000006a0: 0000 007c 006a 006a 017c 006a 0283 0083  ...|.j.j.|.j....
-000006b0: 0101 0074 036a 047c 006a 0583 0172 2e7c  ...t.j.|.j...r.|
-000006c0: 006a 006a 017c 006a 0583 0083 0101 006e  .j.j.|.j.......n
-000006d0: 087c 006a 0583 0001 007c 006a 066a 077c  .|.j.....|.j.j.|
-000006e0: 0083 0101 0064 0053 0029 014e 2908 721e  .....d.S.).N).r.
-000006f0: 0000 0072 1f00 0000 7219 0000 0072 2000  ...r....r....r .
-00000700: 0000 7221 0000 00da 0874 6561 7244 6f77  ..r!.....tearDow
-00000710: 6e72 1d00 0000 5a0a 6368 6563 6b5f 7465  nr....Z.check_te
-00000720: 7374 2901 720e 0000 0072 1000 0000 7210  st).r....r....r.
-00000730: 0000 0072 1100 0000 da09 5f74 6561 7244  ...r......_tearD
-00000740: 6f77 6e3d 0000 0073 0a00 0000 0001 1001  own=...s........
-00000750: 0c01 1202 0803 7a12 5465 7374 4361 7365  ......z.TestCase
-00000760: 2e5f 7465 6172 446f 776e 290a da08 5f5f  ._tearDown)...__
-00000770: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
-00000780: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
-00000790: da07 5f5f 646f 635f 5f72 0300 0000 7212  ..__doc__r....r.
-000007a0: 0000 0072 1600 0000 7219 0000 0072 2500  ...r....r....r%.
-000007b0: 0000 7227 0000 0072 1000 0000 7210 0000  ..r'...r....r...
-000007c0: 0072 1000 0000 7211 0000 0072 0700 0000  .r....r....r....
-000007d0: 0e00 0000 730c 0000 0008 0604 030e 0808  ....s...........
-000007e0: 080e 040e 1272 0700 0000 290f 7220 0000  .....r....).r ..
-000007f0: 00da 026f 7372 1c00 0000 da08 746f 7274  ...osr......tort
-00000800: 6f69 7365 7202 0000 00da 1d74 6f72 746f  oiser......torto
-00000810: 6973 652e 6261 636b 656e 6473 2e62 6173  ise.backends.bas
-00000820: 652e 636c 6965 6e74 7203 0000 005a 1d74  e.clientr....Z.t
-00000830: 6f72 746f 6973 652e 6261 636b 656e 6473  ortoise.backends
-00000840: 2e62 6173 652e 6462 5f75 726c 7204 0000  .base.db_urlr...
-00000850: 00da 0e74 6f72 746f 6973 652e 7574 696c  ...tortoise.util
-00000860: 7372 0500 0000 da07 656e 7669 726f 6eda  sr......environ.
-00000870: 0367 6574 7206 0000 0072 0700 0000 7210  .getr....r....r.
-00000880: 0000 0072 1000 0000 7210 0000 0072 1100  ...r....r....r..
-00000890: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
-000008a0: 7310 0000 0008 0108 0208 020c 010c 010c  s...............
-000008b0: 010c 020e 03                             .....
+00000000: 420d 0d0a 0000 0000 7781 3c5b 1c08 0000  B.......w.<[....
+00000010: e300 0000 0000 0000 0000 0000 0004 0000  ................
+00000020: 0040 0000 0073 6c00 0000 6400 6401 6c00  .@...sl...d.d.l.
+00000030: 5a00 6400 6401 6c01 5a01 6400 6401 6c02  Z.d.d.l.Z.d.d.l.
+00000040: 5a02 6400 6402 6c03 6d04 5a04 0100 6400  Z.d.d.l.m.Z...d.
+00000050: 6403 6c05 6d06 5a06 0100 6400 6404 6c07  d.l.m.Z...d.d.l.
+00000060: 6d08 5a08 0100 6400 6405 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
+00000070: 0100 6501 6a0b a00c 6406 6407 a102 5a0d  ..e.j...d.d...Z.
+00000080: 4700 6408 6409 8400 6409 6502 6a0e 8303  G.d.d...d.e.j...
+00000090: 5a0e 6401 5300 290a e900 0000 004e 2901  Z.d.S.)......N).
+000000a0: da08 546f 7274 6f69 7365 2901 da11 4261  ..Tortoise)...Ba
+000000b0: 7365 4442 4173 796e 6343 6c69 656e 7429  seDBAsyncClient)
+000000c0: 01da 0d65 7870 616e 645f 6462 5f75 726c  ...expand_db_url
+000000d0: 2901 da0f 6765 6e65 7261 7465 5f73 6368  )...generate_sch
+000000e0: 656d 61da 1054 4f52 544f 4953 455f 5445  ema..TORTOISE_TE
+000000f0: 5354 5f44 427a 1c73 716c 6974 653a 2f2f  ST_DBz.sqlite://
+00000100: 2f74 6d70 2f74 6573 742d 7b7d 2e73 716c  /tmp/test-{}.sql
+00000110: 6974 6563 0000 0000 0000 0000 0000 0000  itec............
+00000120: 0300 0000 4000 0000 7350 0000 0065 005a  ....@...sP...e.Z
+00000130: 0164 005a 0264 015a 0365 0464 029c 0164  .d.Z.d.Z.e.d...d
+00000140: 0364 0484 045a 0564 0564 0684 005a 0664  .d...Z.d.d...Z.d
+00000150: 0764 029c 0164 0864 0984 045a 0764 0764  .d...d.d...Z.d.d
+00000160: 029c 0164 0a64 0b84 045a 0864 0764 029c  ...d.d...Z.d.d..
+00000170: 0164 0c64 0d84 045a 0964 0753 0029 0eda  .d.d...Z.d.S.)..
+00000180: 0854 6573 7443 6173 657a 8e0a 2020 2020  .TestCasez..    
+00000190: 416e 2061 7379 6e63 696f 2063 6170 6162  An asyncio capab
+000001a0: 6c65 2054 6573 7443 6173 6520 7468 6174  le TestCase that
+000001b0: 2077 696c 6c20 656e 7375 7265 2074 6861   will ensure tha
+000001c0: 7420 616e 2069 736f 6c61 7465 6420 7465  t an isolated te
+000001d0: 7374 2064 620a 2020 2020 2020 6973 2061  st db.      is a
+000001e0: 7661 696c 6162 6c65 2066 6f72 2065 6163  vailable for eac
+000001f0: 6820 7465 7374 2e0a 0a20 2020 2042 6173  h test...    Bas
+00000200: 6564 206f 6e20 6060 6173 796e 6374 6573  ed on ``asynctes
+00000210: 7460 602e 0a20 2020 2029 01da 0672 6574  t``..    )...ret
+00000220: 7572 6e63 0100 0000 0000 0000 0300 0000  urnc............
+00000230: 0400 0000 c300 0000 733e 0000 0074 0074  ........s>...t.t
+00000240: 0164 0164 028d 027d 017c 0164 0319 0066  .d.d...}.|.d...f
+00000250: 007c 0164 0419 008e 017d 027c 02a0 02a1  .|.d.....}.|....
+00000260: 0049 0064 0048 0001 007c 02a0 03a1 0049  .I.d.H...|.....I
+00000270: 0064 0048 0001 007c 0253 0029 054e 5429  .d.H...|.S.).NT)
+00000280: 01da 0774 6573 7469 6e67 da06 636c 6965  ...testing..clie
+00000290: 6e74 da06 7061 7261 6d73 2904 7204 0000  nt..params).r...
+000002a0: 0072 0600 0000 da09 6462 5f63 7265 6174  .r......db_creat
+000002b0: 65da 1163 7265 6174 655f 636f 6e6e 6563  e..create_connec
+000002c0: 7469 6f6e 2903 da04 7365 6c66 5a06 6462  tion)...selfZ.db
+000002d0: 636f 6e66 da02 6462 a900 7210 0000 00fa  conf..db..r.....
+000002e0: 522f 5573 6572 732f 616e 6472 6579 626f  R/Users/andreybo
+000002f0: 6e64 6172 2f50 7943 6861 726d 5072 6f6a  ndar/PyCharmProj
+00000300: 6563 7473 2f74 6f72 746f 6973 652d 6f72  ects/tortoise-or
+00000310: 6d2f 746f 7274 6f69 7365 2f63 6f6e 7472  m/tortoise/contr
+00000320: 6962 2f74 6573 742f 5f5f 696e 6974 5f5f  ib/test/__init__
+00000330: 2e70 79da 0567 6574 4442 1700 0000 730a  .py..getDB....s.
+00000340: 0000 0000 010c 0112 010e 010e 027a 0e54  .............z.T
+00000350: 6573 7443 6173 652e 6765 7444 4263 0100  estCase.getDBc..
+00000360: 0000 0000 0000 0100 0000 0300 0000 c300  ................
+00000370: 0000 7344 0000 007c 00a0 00a1 0049 0064  ..sD...|.....I.d
+00000380: 0048 007c 005f 0174 026a 0373 2474 02a0  .H.|._.t.j.s$t..
+00000390: 047c 006a 01a1 0101 006e 0c74 02a0 057c  .|.j.....n.t...|
+000003a0: 006a 01a1 0101 0074 067c 006a 0183 0149  .j.....t.|.j...I
+000003b0: 0064 0048 0001 0064 0053 0029 014e 2907  .d.H...d.S.).N).
+000003c0: 7212 0000 0072 0f00 0000 7202 0000 00da  r....r....r.....
+000003d0: 075f 696e 6974 6564 da04 696e 6974 da0f  ._inited..init..
+000003e0: 5f63 6c69 656e 745f 726f 7574 696e 6772  _client_routingr
+000003f0: 0500 0000 2901 720e 0000 0072 1000 0000  ....).r....r....
+00000400: 7210 0000 0072 1100 0000 da08 5f73 6574  r....r......_set
+00000410: 5570 4442 1f00 0000 730a 0000 0000 0110  UpDB....s.......
+00000420: 0106 010e 020c 017a 1154 6573 7443 6173  .......z.TestCas
+00000430: 652e 5f73 6574 5570 4442 4e63 0100 0000  e._setUpDBNc....
+00000440: 0000 0000 0100 0000 0200 0000 c300 0000  ................
+00000450: 7324 0000 007c 006a 00a0 01a1 0049 0064  s$...|.j.....I.d
+00000460: 0048 0001 007c 006a 00a0 02a1 0049 0064  .H...|.j.....I.d
+00000470: 0048 0001 0064 0053 0029 014e 2903 720f  .H...d.S.).N).r.
+00000480: 0000 00da 0563 6c6f 7365 da09 6462 5f64  .....close..db_d
+00000490: 656c 6574 6529 0172 0e00 0000 7210 0000  elete).r....r...
+000004a0: 0072 1000 0000 7211 0000 00da 0b5f 7465  .r....r......_te
+000004b0: 6172 446f 776e 4442 2700 0000 7304 0000  arDownDB'...s...
+000004c0: 0000 0110 017a 1454 6573 7443 6173 652e  .....z.TestCase.
+000004d0: 5f74 6561 7244 6f77 6e44 4263 0100 0000  _tearDownDBc....
+000004e0: 0000 0000 0300 0000 0400 0000 4300 0000  ............C...
+000004f0: 7382 0000 007c 00a0 00a1 0001 0074 017c  s....|.......t.|
+00000500: 007c 006a 0283 027d 0174 017c 0174 036a  .|.j...}.t.|.t.j
+00000510: 046a 0564 0083 037d 027c 0270 3074 036a  .j.d...}.|.p0t.j
+00000520: 04a0 04a1 007c 005f 067c 006a 06a0 077c  .....|._.|.j...|
+00000530: 00a1 0101 007c 006a 08a0 097c 00a0 0aa1  .....|.j...|....
+00000540: 00a1 0101 0074 0ba0 0c7c 006a 0da1 0172  .....t...|.j...r
+00000550: 6e7c 006a 08a0 097c 00a0 0da1 00a1 0101  n|.j...|........
+00000560: 006e 087c 00a0 0da1 0001 0064 017c 006a  .n.|.......d.|.j
+00000570: 085f 0e64 0053 0029 024e 4629 0f5a 0a5f  ._.d.S.).NF).Z._
+00000580: 696e 6974 5f6c 6f6f 70da 0767 6574 6174  init_loop..getat
+00000590: 7472 da0f 5f74 6573 744d 6574 686f 644e  tr.._testMethodN
+000005a0: 616d 65da 0961 7379 6e63 7465 7374 5a08  ame..asynctestZ.
+000005b0: 5f66 6169 6c5f 6f6e 5a0d 5f46 4149 4c5f  _fail_onZ._FAIL_
+000005c0: 4f4e 5f41 5454 52da 085f 6368 6563 6b65  ON_ATTR.._checke
+000005d0: 725a 0b62 6566 6f72 655f 7465 7374 da04  rZ.before_test..
+000005e0: 6c6f 6f70 da12 7275 6e5f 756e 7469 6c5f  loop..run_until_
+000005f0: 636f 6d70 6c65 7465 7216 0000 00da 0761  completer......a
+00000600: 7379 6e63 696f da13 6973 636f 726f 7574  syncio..iscorout
+00000610: 696e 6566 756e 6374 696f 6eda 0573 6574  inefunction..set
+00000620: 5570 5a0e 5f61 7379 6e63 7465 7374 5f72  UpZ._asynctest_r
+00000630: 616e 2903 720e 0000 00da 0474 6573 74da  an).r......test.
+00000640: 0763 6865 636b 6572 7210 0000 0072 1000  .checkerr....r..
+00000650: 0000 7211 0000 00da 065f 7365 7455 702b  ..r......_setUp+
+00000660: 0000 0073 1400 0000 0001 0803 0c01 1001  ...s............
+00000670: 1001 0c02 1001 0c01 1202 0803 7a0f 5465  ............z.Te
+00000680: 7374 4361 7365 2e5f 7365 7455 7063 0100  stCase._setUpc..
+00000690: 0000 0000 0000 0100 0000 0400 0000 4300  ..............C.
+000006a0: 0000 7346 0000 007c 006a 00a0 017c 00a0  ..sF...|.j...|..
+000006b0: 02a1 00a1 0101 0074 03a0 047c 006a 05a1  .......t...|.j..
+000006c0: 0172 2e7c 006a 00a0 017c 00a0 05a1 00a1  .r.|.j...|......
+000006d0: 0101 006e 087c 00a0 05a1 0001 007c 006a  ...n.|.......|.j
+000006e0: 06a0 077c 00a1 0101 0064 0053 0029 014e  ...|.....d.S.).N
+000006f0: 2908 721e 0000 0072 1f00 0000 7219 0000  ).r....r....r...
+00000700: 0072 2000 0000 7221 0000 00da 0874 6561  .r ...r!.....tea
+00000710: 7244 6f77 6e72 1d00 0000 5a0a 6368 6563  rDownr....Z.chec
+00000720: 6b5f 7465 7374 2901 720e 0000 0072 1000  k_test).r....r..
+00000730: 0000 7210 0000 0072 1100 0000 da09 5f74  ..r....r......_t
+00000740: 6561 7244 6f77 6e3d 0000 0073 0a00 0000  earDown=...s....
+00000750: 0001 1001 0c01 1202 0803 7a12 5465 7374  ..........z.Test
+00000760: 4361 7365 2e5f 7465 6172 446f 776e 290a  Case._tearDown).
+00000770: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
+00000780: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
+00000790: 6d65 5f5f da07 5f5f 646f 635f 5f72 0300  me__..__doc__r..
+000007a0: 0000 7212 0000 0072 1600 0000 7219 0000  ..r....r....r...
+000007b0: 0072 2500 0000 7227 0000 0072 1000 0000  .r%...r'...r....
+000007c0: 7210 0000 0072 1000 0000 7211 0000 0072  r....r....r....r
+000007d0: 0700 0000 0e00 0000 730c 0000 0008 0604  ........s.......
+000007e0: 030e 0808 080e 040e 1272 0700 0000 290f  .........r....).
+000007f0: 7220 0000 00da 026f 7372 1c00 0000 da08  r .....osr......
+00000800: 746f 7274 6f69 7365 7202 0000 00da 1d74  tortoiser......t
+00000810: 6f72 746f 6973 652e 6261 636b 656e 6473  ortoise.backends
+00000820: 2e62 6173 652e 636c 6965 6e74 7203 0000  .base.clientr...
+00000830: 005a 1d74 6f72 746f 6973 652e 6261 636b  .Z.tortoise.back
+00000840: 656e 6473 2e62 6173 652e 6462 5f75 726c  ends.base.db_url
+00000850: 7204 0000 00da 0e74 6f72 746f 6973 652e  r......tortoise.
+00000860: 7574 696c 7372 0500 0000 da07 656e 7669  utilsr......envi
+00000870: 726f 6eda 0367 6574 7206 0000 0072 0700  ron..getr....r..
+00000880: 0000 7210 0000 0072 1000 0000 7210 0000  ..r....r....r...
+00000890: 0072 1100 0000 da08 3c6d 6f64 756c 653e  .r......<module>
+000008a0: 0100 0000 7310 0000 0008 0108 0208 020c  ....s...........
+000008b0: 010c 010c 010c 020e 03                   .........
```

### Comparing `tortoise-orm-0.9.2/tortoise/queryset.py` & `tortoise-orm-0.9.4/tortoise/queryset.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,25 @@
+from typing import Any, Dict, List, Optional, Set  # noqa
+
 from pypika import JoinType, Order
 from pypika import PostgreSQLQuery as Query
 from pypika import Table
 from pypika.functions import Count
 
 from tortoise import fields
 from tortoise.aggregation import Aggregate
 from tortoise.backends.base.client import BaseDBAsyncClient
-from tortoise.exceptions import FieldError
+from tortoise.exceptions import DoesNotExist, FieldError, IntegrityError, MultipleObjectsReturned
 from tortoise.query_utils import Prefetch, Q
-from tortoise.utils import AsyncIteratorWrapper
+from tortoise.utils import QueryAsyncIterator
 
 
 class AwaitableQuery:
+    __slots__ = ('_joined_tables', 'query', 'model')
+
     def __init__(self):
         self._joined_tables = []
         self.query = None
         self.model = None
 
     def _filter_from_related_table(self, table, param, value):
         if param['table'] not in self._joined_tables:
@@ -87,15 +91,15 @@
                 self._joined_tables.append(related_table)
 
     def resolve_ordering(self, model, orderings, annotations):
         table = Table(model._meta.table)
         for ordering in orderings:
             field_name = ordering[0]
             if field_name in model._meta.fetch_fields:
-                raise ValueError(
+                raise FieldError(
                     "Filtering by relation is not possible filter by nested field of related model"
                 )
             elif field_name.split('__')[0] in model._meta.fetch_fields:
                 related_field_name = field_name.split('__')[0]
                 related_field = model._meta.fields_map[related_field_name]
                 self._join_table_by_field(table, related_field_name, related_field)
                 self.resolve_ordering(
@@ -119,55 +123,70 @@
         return self._execute().__await__()
 
     async def _execute(self):
         raise NotImplementedError()  # pragma: nocoverage
 
 
 class QuerySet(AwaitableQuery):
+    __slots__ = ('_joined_tables', 'query', 'model', 'fields', '_prefetch_map', '_prefetch_queries',
+                 '_single', '_get', '_count', '_db', '_limit', '_offset', '_filter_kwargs',
+                 '_orderings', '_q_objects_for_resolve', '_distinct',
+                 '_annotations', '_having', '_available_custom_filters')
+
     def __init__(self, model):
         super().__init__()
         self.fields = model._meta.db_fields
         self.model = model
         self.query = Query.from_(model._meta.table)
-        self._prefetch_map = {}
-        self._prefetch_queries = {}
-        self._single = False
-        self._count = False
-        self._db = None
-        self._limit = None
-        self._offset = None
-        self._filter_kwargs = {}
-        self._orderings = []
-        self._joined_tables = []
-        self._q_objects_for_resolve = []
-        self._distinct = False
-        self._annotations = {}
-        self._having = {}
-        self._available_custom_filters = {}
+        self._prefetch_map = {}  # type: Dict[str, Set[str]]
+        self._prefetch_queries = {}  # type: Dict[str, QuerySet]
+        self._single = False  # type: bool
+        self._get = False  # type: bool
+        self._count = False  # type: bool
+        self._db = None  # type: Optional[BaseDBAsyncClient]
+        self._limit = None  # type: Optional[int]
+        self._offset = None  # type: Optional[int]
+        self._filter_kwargs = {}  # type: Dict[str, Any]
+        self._orderings = []  # type: List[str]
+        self._q_objects_for_resolve = []  # type: List[Q]
+        self._distinct = False  # type: bool
+        self._annotations = {}  # type: Dict[str, Aggregate]
+        self._having = {}  # type: Dict[str, Any]
+        self._available_custom_filters = {}  # type: Dict[str, dict]
 
     def _clone(self):
         queryset = self.__class__(self.model)
         queryset._prefetch_map = self._prefetch_map
         queryset._prefetch_queries = self._prefetch_queries
         queryset._single = self._single
+        queryset._get = self._get
         queryset._count = self._count
         queryset._db = self._db
         queryset._limit = self._limit
         queryset._offset = self._offset
-        queryset._filter_kwargs = dict(self._filter_kwargs)
-        queryset._orderings = list(self._orderings)
-        queryset._joined_tables = list(self._joined_tables)
-        queryset._q_objects_for_resolve = list(self._q_objects_for_resolve)
+        queryset._filter_kwargs = self._filter_kwargs
+        queryset._orderings = self._orderings
+        queryset._joined_tables = self._joined_tables
+        queryset._q_objects_for_resolve = self._q_objects_for_resolve
         queryset._distinct = self._distinct
         queryset._annotations = self._annotations
         queryset._having = self._having
         queryset._available_custom_filters = self._available_custom_filters
         return queryset
 
     def filter(self, *args, **kwargs):
+        """
+        Filters QuerySet by given kwargs. You can filter by related objects like this:
+
+        .. code-block:: python3
+
+            Team.filter(events__tournament__name='Test')
+
+        You can also pass Q objects to filters as args.
+        """
         queryset = self._clone()
         for arg in args:
             if not isinstance(arg, Q):
                 raise TypeError('expected Q objects as args')
             queryset._q_objects_for_resolve.append(arg)
         for key, value in kwargs.items():
             if key in queryset.model._meta.filters:
@@ -179,15 +198,24 @@
                 queryset._q_objects_for_resolve.append(Q(**{key: value}))
             elif key in self._available_custom_filters:
                 queryset._having[key] = value
             else:
                 raise FieldError('unknown filter param {}'.format(key))
         return queryset
 
-    def order_by(self, *orderings):
+    def order_by(self, *orderings: str):
+        """
+        Accept args to filter by in format like this:
+
+        .. code-block:: python3
+
+            .order_by('name', '-tournament__name')
+
+        Supports ordering by related models too.
+        """
         queryset = self._clone()
         new_ordering = []
         for ordering in orderings:
             order_type = Order.asc
             if ordering[0] == '-':
                 field_name = ordering[1:]
                 order_type = Order.desc
@@ -204,40 +232,56 @@
                         self.model.__name__,
                     )
                 )
             new_ordering.append((field_name, order_type))
         queryset._orderings = new_ordering
         return queryset
 
-    def limit(self, limit):
+    def limit(self, limit: int):
+        """
+        Limits QuerySet to given length.
+        """
         queryset = self._clone()
         queryset._limit = limit
         return queryset
 
-    def offset(self, offset):
+    def offset(self, offset: int):
+        """
+        Query offset for QuerySet.
+        """
         queryset = self._clone()
         queryset._offset = offset
         return queryset
 
     def distinct(self):
+        """
+        Make QuerySet distinct.
+        """
         queryset = self._clone()
         queryset._distinct = True
         return queryset
 
     def annotate(self, **kwargs):
+        """
+        Annotate result with aggregation result.
+        """
         queryset = self._clone()
         for key, aggregation in kwargs.items():
             if not isinstance(aggregation, Aggregate):
                 raise TypeError('value is expected to be Aggregate instance')
             queryset._annotations[key] = aggregation
             from tortoise.models import get_filters_for_field
             queryset._available_custom_filters.update(get_filters_for_field(key, None, key))
         return queryset
 
-    def values_list(self, *fields, flat=False):
+    def values_list(self, *fields: str, flat: bool = False):
+        """
+        Make QuerySet returns list of tuples for given args instead of objects.
+        If ```flat=True`` and only one arg is passed can return flat list.
+        """
         return ValuesListQuery(
             db=self._db,
             model=self.model,
             filter_kwargs=self._filter_kwargs,
             q_objects=self._q_objects_for_resolve,
             flat=flat,
             fields_for_select_list=fields,
@@ -246,16 +290,19 @@
             offset=self._offset,
             orderings=self._orderings,
             annotations=self._annotations,
             having=self._having,
             custom_filters=self._available_custom_filters,
         )
 
-    def values(self, *args, **kwargs):
-        fields_for_select = {}
+    def values(self, *args: str, **kwargs: str):
+        """
+        Make QuerySet return dicts instead of objects.
+        """
+        fields_for_select = {}  # type: Dict[str, str]
         for field in args:
             if field in fields_for_select:
                 raise FieldError('Duplicate key {}'.format(field))
             fields_for_select[field] = field
 
         for return_as, field in kwargs.items():
             if return_as in fields_for_select:
@@ -274,60 +321,85 @@
             orderings=self._orderings,
             annotations=self._annotations,
             having=self._having,
             custom_filters=self._available_custom_filters,
         )
 
     def delete(self):
+        """
+        Delete all objects in QuerySet.
+        """
         return DeleteQuery(
             db=self._db,
             model=self.model,
             filter_kwargs=self._filter_kwargs,
             q_objects=self._q_objects_for_resolve,
             annotations=self._annotations,
             having=self._having,
             custom_filters=self._available_custom_filters,
         )
 
     def update(self, **kwargs):
+        """
+        Update all objects in QuerySet with given kwargs.
+        """
         return UpdateQuery(
             db=self._db,
             model=self.model,
             filter_kwargs=self._filter_kwargs,
             update_kwargs=kwargs,
             q_objects=self._q_objects_for_resolve,
             annotations=self._annotations,
             having=self._having,
             custom_filters=self._available_custom_filters,
         )
 
     def count(self):
+        """
+        Return count of objects in queryset instead of objects.
+        """
         return CountQuery(
             db=self._db,
             model=self.model,
             filter_kwargs=self._filter_kwargs,
             q_objects=self._q_objects_for_resolve,
             annotations=self._annotations,
             having=self._having,
             custom_filters=self._available_custom_filters,
         )
 
     def all(self):
+        """
+        Return the whole QuerySet.
+        Essentially a no-op except as the only operation.
+        """
         return self._clone()
 
     def first(self):
+        """
+        Limit queryset to one object and return one object instead of list.
+        """
         queryset = self._clone()
         queryset._limit = 1
         queryset._single = True
         return queryset
 
-    def _resolve_prefetch_object(self, queryset, prefetch):
-        pass
+    def get(self, *args, **kwargs):
+        """
+        Fetch exactly one object matching the parameters.
+        """
+        queryset = self.filter(*args, **kwargs)
+        queryset._limit = 2
+        queryset._get = True
+        return queryset
 
-    def prefetch_related(self, *args):
+    def prefetch_related(self, *args: str):
+        """
+        Like ``.fetch_related()`` on instance, but works on all objects in QuerySet.
+        """
         queryset = self._clone()
         queryset._prefetch_map = {}
 
         for relation in args:
             if isinstance(relation, Prefetch):
                 relation.resolve_for_queryset(queryset)
                 continue
@@ -343,14 +415,18 @@
                 queryset._prefetch_map[first_level_field] = set()
             forwarded_prefetch = '__'.join(relation_split[1:])
             if forwarded_prefetch:
                 queryset._prefetch_map[first_level_field].add(forwarded_prefetch)
         return queryset
 
     def using_db(self, _db: BaseDBAsyncClient):
+        """
+        Executes query in provided db client.
+        Useful for transactions workaround.
+        """
         queryset = self._clone()
         queryset._db = _db
         return queryset
 
     def _resolve_annotate(self):
         if not self._annotations:
             return
@@ -392,24 +468,29 @@
             db=db,
             prefetch_map=self._prefetch_map,
             prefetch_queries=self._prefetch_queries,
         ).execute_select(
             self.query, custom_fields=list(self._annotations.keys())
         )
         if not instance_list:
+            if self._get:
+                raise DoesNotExist('Object does not exist')
             if self._single:
                 return None
             return []
+        elif self._get:
+            if len(instance_list) > 1:
+                raise MultipleObjectsReturned('Multiple objects returned, expected exactly one')
+            return instance_list[0]
         elif self._single:
             return instance_list[0]
         return instance_list
 
-    async def __aiter__(self):
-        result = await self
-        return AsyncIteratorWrapper(result)
+    def __aiter__(self):
+        return QueryAsyncIterator(self)
 
 
 class UpdateQuery(AwaitableQuery):
     def __init__(
         self, model, filter_kwargs, update_kwargs, db, q_objects, annotations, having,
         custom_filters
     ):
@@ -426,15 +507,16 @@
             custom_filters=custom_filters
         )
 
         for key, value in update_kwargs.items():
             field_object = model._meta.fields_map.get(key)
             if not field_object:
                 raise FieldError('Unknown keyword argument {} for model {}'.format(key, model))
-            assert not field_object.generated, 'Field {} is generated and can not be updated'
+            if field_object.generated:
+                raise IntegrityError('Field {} is generated and can not be updated')
             if isinstance(field_object, fields.ForeignKeyField):
                 db_field = '{}_id'.format(key)
                 value = value.id
             else:
                 db_field = model._meta.fields_db_projection[key]
             self.query = self.query.set(db_field, value)
```

### Comparing `tortoise-orm-0.9.2/tortoise/query_utils.py` & `tortoise-orm-0.9.4/tortoise/query_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 from pypika import Table
 
 from tortoise import fields
+from tortoise.exceptions import OperationalError
 
 
 class Q:  # pylint: disable=C0103
     AND = 'AND'
     OR = 'OR'
 
     def __init__(self, *args, join_type=AND, **kwargs):
-        assert not (bool(args)
-                    and bool(kwargs)), 'you can pass only Q nodes or filter kwargs in one Q node'
-        assert all(isinstance(node, Q) for node in args)
+        if args and kwargs:
+            raise OperationalError('You can pass only Q nodes or filter kwargs in one Q node')
+        if not all(isinstance(node, Q) for node in args):
+            raise OperationalError('All ordered arguments must be Q nodes')
         self.children = args
         self.filters = kwargs
-        assert join_type in {self.AND, self.OR}
+        if join_type not in {self.AND, self.OR}:
+            raise OperationalError('join_type must be AND or OR')
         self.join_type = join_type
 
     def __and__(self, other):
-        assert isinstance(other, Q)
+        if not isinstance(other, Q):
+            raise OperationalError('AND operation requires a Q node')
         return Q(self, other, join_type=self.AND)
 
     def __or__(self, other):
-        assert isinstance(other, Q)
+        if not isinstance(other, Q):
+            raise OperationalError('OR operation requires a Q node')
         return Q(self, other, join_type=self.OR)
 
     def _get_from_related_table(self, table, param, value):
         join = (param['table'], table.id == getattr(param['table'], param['backward_key']))
         criterion = param['operator'](getattr(param['table'], param['field']), value)
         return criterion, join
 
@@ -119,17 +124,17 @@
     def __init__(self, relation, queryset):
         self.relation = relation
         self.queryset = queryset
 
     def resolve_for_queryset(self, queryset):
         relation_split = self.relation.split('__')
         first_level_field = relation_split[0]
-        assert (
-            first_level_field in queryset.model._meta.fetch_fields
-        ), 'relation {} for {} not found'.format(first_level_field, queryset.model._meta.table)
+        if first_level_field not in queryset.model._meta.fetch_fields:
+            raise OperationalError('relation {} for {} not found'.format(
+                first_level_field, queryset.model._meta.table))
         forwarded_prefetch = '__'.join(relation_split[1:])
         if forwarded_prefetch:
             if first_level_field not in queryset._prefetch_map.keys():
                 queryset._prefetch_map[first_level_field] = set()
             queryset._prefetch_map[first_level_field].add(
                 Prefetch(forwarded_prefetch, self.queryset)
             )
```

