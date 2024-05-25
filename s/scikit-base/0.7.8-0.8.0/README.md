# Comparing `tmp/scikit_base-0.7.8.tar.gz` & `tmp/scikit_base-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scikit_base-0.7.8.tar", last modified: Fri May 10 00:43:19 2024, max compression
+gzip compressed data, was "scikit_base-0.8.0.tar", last modified: Sat May 25 19:30:23 2024, max compression
```

## Comparing `scikit_base-0.7.8.tar` & `scikit_base-0.8.0.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:43:19.117724 scikit_base-0.7.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-10 00:43:13.000000 scikit_base-0.7.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8774 2024-05-10 00:43:19.117724 scikit_base-0.7.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3739 2024-05-10 00:43:13.000000 scikit_base-0.7.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:43:19.101724 scikit_base-0.7.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:43:19.105724 scikit_base-0.7.8/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)     9951 2024-05-10 00:43:13.000000 scikit_base-0.7.8/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-05-10 00:43:13.000000 scikit_base-0.7.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:43:19.113724 scikit_base-0.7.8/scikit_base.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8774 2024-05-10 00:43:19.000000 scikit_base-0.7.8/scikit_base.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-10 00:43:19.000000 scikit_base-0.7.8/scikit_base.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 00:43:19.000000 scikit_base-0.7.8/scikit_base.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-10 00:43:19.000000 scikit_base-0.7.8/scikit_base.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-10 00:43:19.000000 scikit_base-0.7.8/scikit_base.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 00:43:16.000000 scikit_base-0.7.8/scikit_base.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-10 00:43:19.117724 scikit_base-0.7.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:43:19.105724 scikit_base-0.7.8/skbase/
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/_nopytest_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:43:19.105724 scikit_base-0.7.8/skbase/base/
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    53490 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/base/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    38815 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/base/_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:43:19.105724 scikit_base-0.7.8/skbase/base/_pretty_printing/
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/base/_pretty_printing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11677 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/base/_pretty_printing/_object_html_repr.py
--rw-r--r--   0 runner    (1001) docker     (127)    15634 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/base/_pretty_printing/_pprint.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:43:19.109724 scikit_base-0.7.8/skbase/base/_pretty_printing/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/base/_pretty_printing/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/base/_pretty_printing/tests/test_pprint.py
--rw-r--r--   0 runner    (1001) docker     (127)     7289 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/base/_tagmanager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:43:19.109724 scikit_base-0.7.8/skbase/lookup/
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/lookup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    39864 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/lookup/_lookup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:43:19.109724 scikit_base-0.7.8/skbase/lookup/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/lookup/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38218 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/lookup/tests/test_lookup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:43:19.109724 scikit_base-0.7.8/skbase/testing/
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36166 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/testing/test_all_objects.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:43:19.109724 scikit_base-0.7.8/skbase/testing/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/testing/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9890 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/testing/utils/_conditional_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/testing/utils/inspect.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:43:19.109724 scikit_base-0.7.8/skbase/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9330 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:43:19.109724 scikit_base-0.7.8/skbase/tests/mock_package/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/tests/mock_package/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/tests/mock_package/test_mock_package.py
--rw-r--r--   0 runner    (1001) docker     (127)    50648 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4731 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/tests/test_baseestimator.py
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5662 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/tests/test_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:43:19.109724 scikit_base-0.7.8/skbase/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/utils/_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     7653 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/utils/_iter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4566 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/utils/_nested_iter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/utils/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:43:19.113724 scikit_base-0.7.8/skbase/utils/deep_equals/
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/utils/deep_equals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/utils/deep_equals/_common.py
--rw-r--r--   0 runner    (1001) docker     (127)    19151 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/utils/deep_equals/_deep_equals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:43:19.113724 scikit_base-0.7.8/skbase/utils/dependencies/
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/utils/dependencies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14502 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/utils/dependencies/_dependencies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:43:19.113724 scikit_base-0.7.8/skbase/utils/dependencies/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/utils/dependencies/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/utils/dependencies/tests/test_check_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)     5127 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/utils/random_state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:43:19.113724 scikit_base-0.7.8/skbase/utils/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/utils/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/utils/tests/test_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/utils/tests/test_deep_equals.py
--rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/utils/tests/test_iter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/utils/tests/test_nested_iter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/utils/tests/test_random_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/utils/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:43:19.113724 scikit_base-0.7.8/skbase/validate/
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/validate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12957 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/validate/_named_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)    12121 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/validate/_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:43:19.113724 scikit_base-0.7.8/skbase/validate/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/validate/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7438 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/validate/tests/test_iterable_named_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)    14131 2024-05-10 00:43:13.000000 scikit_base-0.7.8/skbase/validate/tests/test_type_validations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:30:23.886237 scikit_base-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-25 19:30:14.000000 scikit_base-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8482 2024-05-25 19:30:23.886237 scikit_base-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-05-25 19:30:14.000000 scikit_base-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:30:23.870237 scikit_base-0.8.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:30:23.874237 scikit_base-0.8.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)     9951 2024-05-25 19:30:14.000000 scikit_base-0.8.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-05-25 19:30:14.000000 scikit_base-0.8.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:30:23.882237 scikit_base-0.8.0/scikit_base.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8482 2024-05-25 19:30:23.000000 scikit_base-0.8.0/scikit_base.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-25 19:30:23.000000 scikit_base-0.8.0/scikit_base.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 19:30:23.000000 scikit_base-0.8.0/scikit_base.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-25 19:30:23.000000 scikit_base-0.8.0/scikit_base.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-25 19:30:23.000000 scikit_base-0.8.0/scikit_base.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 19:30:20.000000 scikit_base-0.8.0/scikit_base.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-25 19:30:23.886237 scikit_base-0.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:30:23.874237 scikit_base-0.8.0/skbase/
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-25 19:30:14.000000 scikit_base-0.8.0/skbase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-25 19:30:14.000000 scikit_base-0.8.0/skbase/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-25 19:30:14.000000 scikit_base-0.8.0/skbase/_nopytest_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:30:23.878237 scikit_base-0.8.0/skbase/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-25 19:30:14.000000 scikit_base-0.8.0/skbase/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53490 2024-05-25 19:30:14.000000 scikit_base-0.8.0/skbase/base/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38815 2024-05-25 19:30:14.000000 scikit_base-0.8.0/skbase/base/_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:30:23.878237 scikit_base-0.8.0/skbase/base/_pretty_printing/
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-25 19:30:14.000000 scikit_base-0.8.0/skbase/base/_pretty_printing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11677 2024-05-25 19:30:14.000000 scikit_base-0.8.0/skbase/base/_pretty_printing/_object_html_repr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15634 2024-05-25 19:30:14.000000 scikit_base-0.8.0/skbase/base/_pretty_printing/_pprint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:30:23.878237 scikit_base-0.8.0/skbase/base/_pretty_printing/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-25 19:30:14.000000 scikit_base-0.8.0/skbase/base/_pretty_printing/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-25 19:30:14.000000 scikit_base-0.8.0/skbase/base/_pretty_printing/tests/test_pprint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7289 2024-05-25 19:30:14.000000 scikit_base-0.8.0/skbase/base/_tagmanager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:30:23.878237 scikit_base-0.8.0/skbase/lookup/
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-25 19:30:14.000000 scikit_base-0.8.0/skbase/lookup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45083 2024-05-25 19:30:14.000000 scikit_base-0.8.0/skbase/lookup/_lookup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:30:23.878237 scikit_base-0.8.0/skbase/lookup/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-25 19:30:14.000000 scikit_base-0.8.0/skbase/lookup/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39743 2024-05-25 19:30:14.000000 scikit_base-0.8.0/skbase/lookup/tests/test_lookup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:30:23.878237 scikit_base-0.8.0/skbase/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-25 19:30:14.000000 scikit_base-0.8.0/skbase/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36166 2024-05-25 19:30:14.000000 scikit_base-0.8.0/skbase/testing/test_all_objects.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:30:23.878237 scikit_base-0.8.0/skbase/testing/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-25 19:30:14.000000 scikit_base-0.8.0/skbase/testing/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9890 2024-05-25 19:30:14.000000 scikit_base-0.8.0/skbase/testing/utils/_conditional_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-25 19:30:14.000000 scikit_base-0.8.0/skbase/testing/utils/inspect.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:30:23.878237 scikit_base-0.8.0/skbase/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-25 19:30:14.000000 scikit_base-0.8.0/skbase/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9375 2024-05-25 19:30:14.000000 scikit_base-0.8.0/skbase/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:30:23.878237 scikit_base-0.8.0/skbase/tests/mock_package/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-25 19:30:14.000000 scikit_base-0.8.0/skbase/tests/mock_package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-05-25 19:30:14.000000 scikit_base-0.8.0/skbase/tests/mock_package/test_mock_package.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50648 2024-05-25 19:30:14.000000 scikit_base-0.8.0/skbase/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4731 2024-05-25 19:30:14.000000 scikit_base-0.8.0/skbase/tests/test_baseestimator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-25 19:30:14.000000 scikit_base-0.8.0/skbase/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5662 2024-05-25 19:30:14.000000 scikit_base-0.8.0/skbase/tests/test_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:30:23.882237 scikit_base-0.8.0/skbase/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-25 19:30:14.000000 scikit_base-0.8.0/skbase/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-25 19:30:14.000000 scikit_base-0.8.0/skbase/utils/_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7653 2024-05-25 19:30:14.000000 scikit_base-0.8.0/skbase/utils/_iter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4566 2024-05-25 19:30:14.000000 scikit_base-0.8.0/skbase/utils/_nested_iter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-05-25 19:30:14.000000 scikit_base-0.8.0/skbase/utils/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:30:23.882237 scikit_base-0.8.0/skbase/utils/deep_equals/
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-25 19:30:14.000000 scikit_base-0.8.0/skbase/utils/deep_equals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-05-25 19:30:14.000000 scikit_base-0.8.0/skbase/utils/deep_equals/_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19151 2024-05-25 19:30:14.000000 scikit_base-0.8.0/skbase/utils/deep_equals/_deep_equals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:30:23.882237 scikit_base-0.8.0/skbase/utils/dependencies/
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-25 19:30:14.000000 scikit_base-0.8.0/skbase/utils/dependencies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14502 2024-05-25 19:30:14.000000 scikit_base-0.8.0/skbase/utils/dependencies/_dependencies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:30:23.882237 scikit_base-0.8.0/skbase/utils/dependencies/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-25 19:30:14.000000 scikit_base-0.8.0/skbase/utils/dependencies/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-05-25 19:30:14.000000 scikit_base-0.8.0/skbase/utils/dependencies/tests/test_check_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5127 2024-05-25 19:30:14.000000 scikit_base-0.8.0/skbase/utils/random_state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:30:23.882237 scikit_base-0.8.0/skbase/utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-25 19:30:14.000000 scikit_base-0.8.0/skbase/utils/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-05-25 19:30:14.000000 scikit_base-0.8.0/skbase/utils/tests/test_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-05-25 19:30:14.000000 scikit_base-0.8.0/skbase/utils/tests/test_deep_equals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-05-25 19:30:14.000000 scikit_base-0.8.0/skbase/utils/tests/test_iter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-25 19:30:14.000000 scikit_base-0.8.0/skbase/utils/tests/test_nested_iter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-05-25 19:30:14.000000 scikit_base-0.8.0/skbase/utils/tests/test_random_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-25 19:30:14.000000 scikit_base-0.8.0/skbase/utils/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:30:23.882237 scikit_base-0.8.0/skbase/validate/
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-25 19:30:14.000000 scikit_base-0.8.0/skbase/validate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12957 2024-05-25 19:30:14.000000 scikit_base-0.8.0/skbase/validate/_named_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12121 2024-05-25 19:30:14.000000 scikit_base-0.8.0/skbase/validate/_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:30:23.882237 scikit_base-0.8.0/skbase/validate/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-25 19:30:14.000000 scikit_base-0.8.0/skbase/validate/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7438 2024-05-25 19:30:14.000000 scikit_base-0.8.0/skbase/validate/tests/test_iterable_named_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14131 2024-05-25 19:30:14.000000 scikit_base-0.8.0/skbase/validate/tests/test_type_validations.py
```

### Comparing `scikit_base-0.7.8/LICENSE` & `scikit_base-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit_base-0.7.8/PKG-INFO` & `scikit_base-0.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-base
-Version: 0.7.8
+Version: 0.8.0
 Summary: Base classes for sklearn-like parametric objects
 Author-email: sktime developers <sktime.toolbox@gmail.com>
 Maintainer: Franz Király
 Maintainer-email: sktime developers <sktime.toolbox@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, skbase Developers
@@ -88,15 +88,15 @@
 Requires-Dist: myst-parser; extra == "docs"
 Requires-Dist: nbsphinx>=0.8.6; extra == "docs"
 Requires-Dist: numpydoc; extra == "docs"
 Requires-Dist: pydata-sphinx-theme; extra == "docs"
 Requires-Dist: sphinx-issues<5.0.0; extra == "docs"
 Requires-Dist: sphinx-gallery<0.17.0; extra == "docs"
 Requires-Dist: sphinx-panels; extra == "docs"
-Requires-Dist: sphinx-design<0.6.0; extra == "docs"
+Requires-Dist: sphinx-design<0.7.0; extra == "docs"
 Requires-Dist: Sphinx!=7.2.0,<8.0.0; extra == "docs"
 Requires-Dist: tabulate; extra == "docs"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: coverage; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: safety; extra == "test"
@@ -110,22 +110,22 @@
 # Welcome to skbase
 
 > A framework factory for scikit-learn-like and sktime-like parametric objects
 
 `skbase` provides base classes for creating scikit-learn-like parametric objects,
 along with tools to make it easier to build your own packages that follow these design patterns.
 
-:rocket: Version 0.7.8 is now available. Check out our
+:rocket: Version 0.8.0 is now available. Check out our
 [release notes](https://skbase.readthedocs.io/en/latest/changelog.html).
 
 | Overview | |
 |---|---|
 | **CI/CD** | [![Tests](https://github.com/sktime/skbase/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/sktime/skbase/actions/workflows/test.yml) [![codecov](https://codecov.io/gh/sktime/skbase/branch/main/graph/badge.svg?token=2J424NLO82)](https://codecov.io/gh/sktime/skbase) [![Documentation Status](https://readthedocs.org/projects/skbase/badge/?version=latest)](https://skbase.readthedocs.io/en/latest/?badge=latest) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/sktime/skbase/main.svg)](https://results.pre-commit.ci/latest/github/sktime/skbase/main) |
 | **Code** |  [![!pypi](https://img.shields.io/pypi/v/scikit-base?color=orange)](https://pypi.org/project/scikit-base/)  [![!python-versions](https://img.shields.io/pypi/pyversions/scikit-base)](https://www.python.org/) [![!black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit) |
-| **Downloads** | [![Downloads](https://static.pepy.tech/personalized-badge/scikit-base?period=week&units=international_system&left_color=grey&right_color=blue&left_text=weekly%20(pypi))](https://pepy.tech/project/scikit-base) [![Downloads](https://static.pepy.tech/personalized-badge/scikit-base?period=month&units=international_system&left_color=grey&right_color=blue&left_text=monthly%20(pypi))](https://pepy.tech/project/scikit-base) [![Downloads](https://static.pepy.tech/personalized-badge/scikit-base?period=total&units=international_system&left_color=grey&right_color=blue&left_text=cumulative%20(pypi))](https://pepy.tech/project/scikit-base) |
+| **Downloads** | ![PyPI - Downloads](https://img.shields.io/pypi/dw/scikit-base) ![PyPI - Downloads](https://img.shields.io/pypi/dm/scikit-base) [![Downloads](https://static.pepy.tech/personalized-badge/scikit-base?period=total&units=international_system&left_color=grey&right_color=blue&left_text=cumulative%20(pypi))](https://pepy.tech/project/scikit-base) |
 | **Citation** | [![DOI](https://zenodo.org/badge/494649836.svg)](https://zenodo.org/doi/10.5281/zenodo.10980557) |
 
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
 [![All Contributors](https://img.shields.io/badge/all_contributors-13-orange.svg?style=flat-square)](#contributors)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
 ## Documentation and Tutorials
```

### Comparing `scikit_base-0.7.8/README.md` & `scikit_base-0.8.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 # Welcome to skbase
 
 > A framework factory for scikit-learn-like and sktime-like parametric objects
 
 `skbase` provides base classes for creating scikit-learn-like parametric objects,
 along with tools to make it easier to build your own packages that follow these design patterns.
 
-:rocket: Version 0.7.8 is now available. Check out our
+:rocket: Version 0.8.0 is now available. Check out our
 [release notes](https://skbase.readthedocs.io/en/latest/changelog.html).
 
 | Overview | |
 |---|---|
 | **CI/CD** | [![Tests](https://github.com/sktime/skbase/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/sktime/skbase/actions/workflows/test.yml) [![codecov](https://codecov.io/gh/sktime/skbase/branch/main/graph/badge.svg?token=2J424NLO82)](https://codecov.io/gh/sktime/skbase) [![Documentation Status](https://readthedocs.org/projects/skbase/badge/?version=latest)](https://skbase.readthedocs.io/en/latest/?badge=latest) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/sktime/skbase/main.svg)](https://results.pre-commit.ci/latest/github/sktime/skbase/main) |
 | **Code** |  [![!pypi](https://img.shields.io/pypi/v/scikit-base?color=orange)](https://pypi.org/project/scikit-base/)  [![!python-versions](https://img.shields.io/pypi/pyversions/scikit-base)](https://www.python.org/) [![!black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit) |
-| **Downloads** | [![Downloads](https://static.pepy.tech/personalized-badge/scikit-base?period=week&units=international_system&left_color=grey&right_color=blue&left_text=weekly%20(pypi))](https://pepy.tech/project/scikit-base) [![Downloads](https://static.pepy.tech/personalized-badge/scikit-base?period=month&units=international_system&left_color=grey&right_color=blue&left_text=monthly%20(pypi))](https://pepy.tech/project/scikit-base) [![Downloads](https://static.pepy.tech/personalized-badge/scikit-base?period=total&units=international_system&left_color=grey&right_color=blue&left_text=cumulative%20(pypi))](https://pepy.tech/project/scikit-base) |
+| **Downloads** | ![PyPI - Downloads](https://img.shields.io/pypi/dw/scikit-base) ![PyPI - Downloads](https://img.shields.io/pypi/dm/scikit-base) [![Downloads](https://static.pepy.tech/personalized-badge/scikit-base?period=total&units=international_system&left_color=grey&right_color=blue&left_text=cumulative%20(pypi))](https://pepy.tech/project/scikit-base) |
 | **Citation** | [![DOI](https://zenodo.org/badge/494649836.svg)](https://zenodo.org/doi/10.5281/zenodo.10980557) |
 
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
 [![All Contributors](https://img.shields.io/badge/all_contributors-13-orange.svg?style=flat-square)](#contributors)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
 ## Documentation and Tutorials
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_s_k_t_i_m_e_/_s_k_b_a_s_e_/_b_l_o_b_/_m_a_i_n_/_d_o_c_s_/_s_o_u_r_c_e_/_i_m_a_g_e_s_/_s_k_b_a_s_e_-_l_o_g_o_-
 _w_i_t_h_-_n_a_m_e_._p_n_g_]# Welcome to skbase > A framework factory for scikit-learn-like
 and sktime-like parametric objects `skbase` provides base classes for creating
 scikit-learn-like parametric objects, along with tools to make it easier to
 build your own packages that follow these design patterns. :rocket: Version
-0.7.8 is now available. Check out our [release notes](https://
+0.8.0 is now available. Check out our [release notes](https://
 skbase.readthedocs.io/en/latest/changelog.html). | Overview | | |---|---| |
 **CI/CD** | [![Tests](https://github.com/sktime/skbase/actions/workflows/
 test.yml/badge.svg?branch=main)](https://github.com/sktime/skbase/actions/
 workflows/test.yml) [![codecov](https://codecov.io/gh/sktime/skbase/branch/
 main/graph/badge.svg?token=2J424NLO82)](https://codecov.io/gh/sktime/skbase) [!
 [Documentation Status](https://readthedocs.org/projects/skbase/badge/
 ?version=latest)](https://skbase.readthedocs.io/en/latest/?badge=latest) [!
@@ -15,20 +15,16 @@
 skbase/main.svg)](https://results.pre-commit.ci/latest/github/sktime/skbase/
 main) | | **Code** | [![!pypi](https://img.shields.io/pypi/v/scikit-
 base?color=orange)](https://pypi.org/project/scikit-base/) [![!python-versions]
 (https://img.shields.io/pypi/pyversions/scikit-base)](https://www.python.org/)
 [![!black](https://img.shields.io/badge/code%20style-black-000000.svg)](https:/
 /github.com/psf/black) [![security: bandit](https://img.shields.io/badge/
 security-bandit-yellow.svg)](https://github.com/PyCQA/bandit) | | **Downloads**
-| [![Downloads](https://static.pepy.tech/personalized-badge/scikit-
-base?period=week&units=international_system&left_color=grey&right_color=blue&left_text=weekly%20
-(pypi))](https://pepy.tech/project/scikit-base) [![Downloads](https://
-static.pepy.tech/personalized-badge/scikit-
-base?period=month&units=international_system&left_color=grey&right_color=blue&left_text=monthly%20
-(pypi))](https://pepy.tech/project/scikit-base) [![Downloads](https://
+| ![PyPI - Downloads](https://img.shields.io/pypi/dw/scikit-base) ![PyPI -
+Downloads](https://img.shields.io/pypi/dm/scikit-base) [![Downloads](https://
 static.pepy.tech/personalized-badge/scikit-
 base?period=total&units=international_system&left_color=grey&right_color=blue&left_text=cumulative%20
 (pypi))](https://pepy.tech/project/scikit-base) | | **Citation** | [![DOI]
 (https://zenodo.org/badge/494649836.svg)](https://zenodo.org/doi/10.5281/
 zenodo.10980557) | [![All Contributors](https://img.shields.io/badge/
 all_contributors-13-orange.svg?style=flat-square)](#contributors) ##
 Documentation and Tutorials To learn more about the package check out: * our
```

### Comparing `scikit_base-0.7.8/docs/source/conf.py` & `scikit_base-0.8.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `scikit_base-0.7.8/pyproject.toml` & `scikit_base-0.8.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "scikit-base"
-version = "0.7.8"
+version = "0.8.0"
 description = "Base classes for sklearn-like parametric objects"
 authors = [
     {name = "sktime developers", email = "sktime.toolbox@gmail.com"},
 ]
 maintainers = [
     {name = "sktime developers", email = "sktime.toolbox@gmail.com"},
     {name = "Franz Király"},
@@ -69,15 +69,15 @@
     "myst-parser",
     "nbsphinx>=0.8.6",
     "numpydoc",
     "pydata-sphinx-theme",
     "sphinx-issues<5.0.0",
     "sphinx-gallery<0.17.0",
     "sphinx-panels",
-    "sphinx-design<0.6.0",
+    "sphinx-design<0.7.0",
     "Sphinx<8.0.0,!=7.2.0",
     "tabulate",
 ]
 
 test = [
     "pytest",
     "coverage",
```

### Comparing `scikit_base-0.7.8/scikit_base.egg-info/PKG-INFO` & `scikit_base-0.8.0/scikit_base.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-base
-Version: 0.7.8
+Version: 0.8.0
 Summary: Base classes for sklearn-like parametric objects
 Author-email: sktime developers <sktime.toolbox@gmail.com>
 Maintainer: Franz Király
 Maintainer-email: sktime developers <sktime.toolbox@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, skbase Developers
@@ -88,15 +88,15 @@
 Requires-Dist: myst-parser; extra == "docs"
 Requires-Dist: nbsphinx>=0.8.6; extra == "docs"
 Requires-Dist: numpydoc; extra == "docs"
 Requires-Dist: pydata-sphinx-theme; extra == "docs"
 Requires-Dist: sphinx-issues<5.0.0; extra == "docs"
 Requires-Dist: sphinx-gallery<0.17.0; extra == "docs"
 Requires-Dist: sphinx-panels; extra == "docs"
-Requires-Dist: sphinx-design<0.6.0; extra == "docs"
+Requires-Dist: sphinx-design<0.7.0; extra == "docs"
 Requires-Dist: Sphinx!=7.2.0,<8.0.0; extra == "docs"
 Requires-Dist: tabulate; extra == "docs"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: coverage; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: safety; extra == "test"
@@ -110,22 +110,22 @@
 # Welcome to skbase
 
 > A framework factory for scikit-learn-like and sktime-like parametric objects
 
 `skbase` provides base classes for creating scikit-learn-like parametric objects,
 along with tools to make it easier to build your own packages that follow these design patterns.
 
-:rocket: Version 0.7.8 is now available. Check out our
+:rocket: Version 0.8.0 is now available. Check out our
 [release notes](https://skbase.readthedocs.io/en/latest/changelog.html).
 
 | Overview | |
 |---|---|
 | **CI/CD** | [![Tests](https://github.com/sktime/skbase/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/sktime/skbase/actions/workflows/test.yml) [![codecov](https://codecov.io/gh/sktime/skbase/branch/main/graph/badge.svg?token=2J424NLO82)](https://codecov.io/gh/sktime/skbase) [![Documentation Status](https://readthedocs.org/projects/skbase/badge/?version=latest)](https://skbase.readthedocs.io/en/latest/?badge=latest) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/sktime/skbase/main.svg)](https://results.pre-commit.ci/latest/github/sktime/skbase/main) |
 | **Code** |  [![!pypi](https://img.shields.io/pypi/v/scikit-base?color=orange)](https://pypi.org/project/scikit-base/)  [![!python-versions](https://img.shields.io/pypi/pyversions/scikit-base)](https://www.python.org/) [![!black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit) |
-| **Downloads** | [![Downloads](https://static.pepy.tech/personalized-badge/scikit-base?period=week&units=international_system&left_color=grey&right_color=blue&left_text=weekly%20(pypi))](https://pepy.tech/project/scikit-base) [![Downloads](https://static.pepy.tech/personalized-badge/scikit-base?period=month&units=international_system&left_color=grey&right_color=blue&left_text=monthly%20(pypi))](https://pepy.tech/project/scikit-base) [![Downloads](https://static.pepy.tech/personalized-badge/scikit-base?period=total&units=international_system&left_color=grey&right_color=blue&left_text=cumulative%20(pypi))](https://pepy.tech/project/scikit-base) |
+| **Downloads** | ![PyPI - Downloads](https://img.shields.io/pypi/dw/scikit-base) ![PyPI - Downloads](https://img.shields.io/pypi/dm/scikit-base) [![Downloads](https://static.pepy.tech/personalized-badge/scikit-base?period=total&units=international_system&left_color=grey&right_color=blue&left_text=cumulative%20(pypi))](https://pepy.tech/project/scikit-base) |
 | **Citation** | [![DOI](https://zenodo.org/badge/494649836.svg)](https://zenodo.org/doi/10.5281/zenodo.10980557) |
 
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
 [![All Contributors](https://img.shields.io/badge/all_contributors-13-orange.svg?style=flat-square)](#contributors)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
 ## Documentation and Tutorials
```

### Comparing `scikit_base-0.7.8/scikit_base.egg-info/SOURCES.txt` & `scikit_base-0.8.0/scikit_base.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scikit_base-0.7.8/scikit_base.egg-info/requires.txt` & `scikit_base-0.8.0/scikit_base.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 myst-parser
 nbsphinx>=0.8.6
 numpydoc
 pydata-sphinx-theme
 sphinx-issues<5.0.0
 sphinx-gallery<0.17.0
 sphinx-panels
-sphinx-design<0.6.0
+sphinx-design<0.7.0
 Sphinx!=7.2.0,<8.0.0
 tabulate
 
 [linters]
 mypy
 isort
 flake8
```

### Comparing `scikit_base-0.7.8/skbase/_exceptions.py` & `scikit_base-0.8.0/skbase/_exceptions.py`

 * *Files identical despite different names*

### Comparing `scikit_base-0.7.8/skbase/_nopytest_tests.py` & `scikit_base-0.8.0/skbase/_nopytest_tests.py`

 * *Files identical despite different names*

### Comparing `scikit_base-0.7.8/skbase/base/__init__.py` & `scikit_base-0.8.0/skbase/base/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit_base-0.7.8/skbase/base/_base.py` & `scikit_base-0.8.0/skbase/base/_base.py`

 * *Files identical despite different names*

### Comparing `scikit_base-0.7.8/skbase/base/_meta.py` & `scikit_base-0.8.0/skbase/base/_meta.py`

 * *Files identical despite different names*

### Comparing `scikit_base-0.7.8/skbase/base/_pretty_printing/_object_html_repr.py` & `scikit_base-0.8.0/skbase/base/_pretty_printing/_object_html_repr.py`

 * *Files identical despite different names*

### Comparing `scikit_base-0.7.8/skbase/base/_pretty_printing/_pprint.py` & `scikit_base-0.8.0/skbase/base/_pretty_printing/_pprint.py`

 * *Files identical despite different names*

### Comparing `scikit_base-0.7.8/skbase/base/_pretty_printing/tests/test_pprint.py` & `scikit_base-0.8.0/skbase/base/_pretty_printing/tests/test_pprint.py`

 * *Files identical despite different names*

### Comparing `scikit_base-0.7.8/skbase/base/_tagmanager.py` & `scikit_base-0.8.0/skbase/base/_tagmanager.py`

 * *Files identical despite different names*

### Comparing `scikit_base-0.7.8/skbase/lookup/__init__.py` & `scikit_base-0.8.0/skbase/lookup/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit_base-0.7.8/skbase/lookup/_lookup.py` & `scikit_base-0.8.0/skbase/lookup/_lookup.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,18 +16,20 @@
 # https://github.com/sktime/sktime/blob/main/LICENSE
 import importlib
 import inspect
 import io
 import os
 import pathlib
 import pkgutil
+import re
 import sys
 import warnings
 from collections.abc import Iterable
 from copy import deepcopy
+from functools import lru_cache
 from operator import itemgetter
 from types import ModuleType
 from typing import Any, List, Mapping, MutableMapping, Optional, Sequence, Tuple, Union
 
 from skbase.base import BaseObject
 from skbase.validate import check_sequence
 
@@ -185,56 +187,94 @@
     -------
     cond_sat: bool, whether estimator satisfies condition in `tag_filter`
         if `tag_filter` was None, returns `True`
     """
     if tag_filter is None:
         return True
 
+    type_msg = (
+        "filter_tags argument of all_objects must be "
+        "a dict with str or re.Pattern keys, "
+        "str, or iterable of str, "
+        "but found"
+    )
+
     if not isinstance(tag_filter, (str, Iterable, dict)):
-        raise TypeError(
-            "tag_filter argument of _filter_by_tags must be "
-            "a dict with str keys, str, or iterable of str, "
-            f"but found tag_filter of type {type(tag_filter)}"
-        )
+        raise TypeError(f"{type_msg} type {type(tag_filter)}")
 
     if not hasattr(obj, "get_class_tag"):
         return False
 
     klass_tags = obj.get_class_tags().keys()
 
+    # todo 0.9.0: remove the warning message
+    # i.e., this message and all warnings referring to it
+    warn_msg = (
+        "The meaning of filter_tags arguments in all_objects of type str "
+        "and iterable of str will change from scikit-base 0.9.0. "
+        "Currently, str or iterable of str arguments select objects that possess the "
+        "tag(s) with the specified name, of any value. "
+        "From 0.9.0 onwards, str or iterable of str "
+        "will select objects that possess the tag with the specified name, "
+        "with the value True (boolean). See scikit-base issue #326 for the rationale "
+        "behind this change. "
+        "To retain previous behaviour, that is, "
+        "to select objects that possess the tag with the specified name, of any value, "
+        "use a dict with the tag name as key, and re.Pattern('*?') as value. "
+        "That is, from re import Pattern, and pass {tag_name: Pattern('*?')} "
+        "as filter_tags, and similarly with multiple tag names. "
+    )
+
     # case: tag_filter is string
     if isinstance(tag_filter, str):
+        # todo 0.9.0: reomove this warning
+        warnings.warn(warn_msg, DeprecationWarning, stacklevel=2)
+        # todo 0.9.0: replace this line
         return tag_filter in klass_tags
+        # by this line
+        # tag_filter = {tag_filter: True}
 
     # case: tag_filter is iterable of str but not dict
     # If a iterable of strings is provided, check that all are in the returned tag_dict
     if isinstance(tag_filter, Iterable) and not isinstance(tag_filter, dict):
         if not all(isinstance(t, str) for t in tag_filter):
-            raise ValueError(
-                "tag_filter argument of _filter_by_tags must be "
-                f"a dict with str keys, str, or iterable of str, but found {tag_filter}"
-            )
+            raise ValueError(f"{type_msg} {tag_filter}")
+        # todo 0.9.0: reomove this warning
+        warnings.warn(warn_msg, DeprecationWarning, stacklevel=2)
+        # todo 0.9.0: replace this line
         return all(tag in klass_tags for tag in tag_filter)
+        # by this line
+        # tag_filter = {tag: True for tag in tag_filter}
 
     # case: tag_filter is dict
+    # check that all keys are str
     if not all(isinstance(t, str) for t in tag_filter.keys()):
-        raise ValueError(
-            "tag_filter argument of _filter_by_tags must be "
-            f"a dict with str keys, str, or iterable of str, but found {tag_filter}"
-        )
+        raise ValueError(f"{type_msg} {tag_filter}")
 
     cond_sat = True
 
     for key, search_value in tag_filter.items():
         if not isinstance(search_value, list):
             search_value = [search_value]
+
+        # split search_value into strings/other and re.Pattern
+        search_re = [s for s in search_value if isinstance(s, re.Pattern)]
+        search_str = [s for s in search_value if not isinstance(s, re.Pattern)]
+
         tag_value = obj.get_class_tag(key)
         if not isinstance(tag_value, list):
             tag_value = [tag_value]
-        cond_sat = cond_sat and len(set(search_value).intersection(tag_value)) > 0
+
+        # search value matches tag value iff
+        # at least one element of search value matches at least one element of tag value
+        str_match = len(set(search_str).intersection(tag_value)) > 0
+        re_match = any(s.fullmatch(str(tag)) for s in search_re for tag in tag_value)
+        match = str_match or re_match
+
+        cond_sat = cond_sat and match
 
     return cond_sat
 
 
 def _walk(root, exclude=None, prefix=""):
     """Recursively return all modules and sub-modules as list of strings.
 
@@ -291,39 +331,23 @@
         raise ValueError(
             "`module` should be string module name or instance of "
             "importlib.machinery.SourceFileLoader."
         )
 
     # if suppress_import_stdout:
     # setup text trap, import
-    if suppress_import_stdout:
-        temp_stdout = sys.stdout
-        sys.stdout = io.StringIO()
-
-    try:
+    with StdoutMute(active=suppress_import_stdout):
         if isinstance(module, str):
             imported_mod = importlib.import_module(module)
         elif isinstance(module, importlib.machinery.SourceFileLoader):
             spec = importlib.util.spec_from_file_location(module.name, module.path)
             imported_mod = importlib.util.module_from_spec(spec)
 
             loader = spec.loader
             loader.exec_module(imported_mod)
-        exc = None
-    except Exception as e:
-        # we store the exception so we can restore the stdout first
-        exc = e
-
-    # if we set up a text trap, restore it to the initial value
-    if suppress_import_stdout:
-        sys.stdout = temp_stdout
-
-    # if we encountered an exception, now raise it
-    if exc is not None:
-        raise exc
 
     return imported_mod
 
 
 def _determine_module_path(
     package_name: str, path: Optional[Union[str, pathlib.Path]] = None
 ) -> Tuple[ModuleType, str, importlib.machinery.SourceFileLoader]:
@@ -685,207 +709,186 @@
                         suppress_import_stdout=suppress_import_stdout,
                     )
                 )
 
     return module_info
 
 
+# todo 0.9.0: change docstring to reflect handling of filter_tags
+# in case of str or iterable of str
 def all_objects(
     object_types=None,
     filter_tags=None,
     exclude_objects=None,
     return_names=True,
     as_dataframe=False,
     return_tags=None,
     suppress_import_stdout=True,
     package_name="skbase",
     path: Optional[str] = None,
     modules_to_ignore=None,
     class_lookup=None,
 ):
-    """Get a list of all objects in a package with name `package_name`.
+    """Get a list of all objects in a package, optionally filtered by type and tags.
 
     This function crawls the package/module to retrieve all classes
-    that are descendents of BaseObject. By default it does this for the `skbase`
-    package, but users can specify `package_name` or `path` to another project
-    and `all_objects` will crawl and retrieve BaseObjects found in that project.
+    that are descendents of ``BaseObject``, or another specified class,
+    from a module and all submodules, specified by  ``package_name`` oand``path``.
+
+    The retrieved objects can be filtered by type, tags, and excluded by name.
+
+    ``all_objects`` will crawl and return references to the retrieved classes.
 
     Parameters
     ----------
-    object_types: class or list of classes, default=None
+    object_types: class or tuple, list of classes, default=None
 
         - If class_lookup is provided, can also be str or list of str
           which kind of objects should be returned.
         - If None, no filter is applied and all estimators are returned.
         - If class or list of class, estimators are filtered to inherit from
           one of these.
         - If str or list of str, classes can be aliased by strings, as long
           as `class_lookup` parameter is passed a lookup dict.
 
     return_names: bool, default=True
 
-        - If True, estimator class name is included in the all_estimators()
+        - If True, estimator class name is included in the ``all_objects``
           return in the order: name, estimator class, optional tags, either as
-          a tuple or as pandas.DataFrame columns.
-        - If False, estimator class name is removed from the all_estimators()
-          return.
+          a tuple or as ``pandas.DataFrame`` columns.
+        - If False, estimator class name is removed from the ``all_objects`` return.
 
     filter_tags: str, list[str] or dict[str, Any], default=None
-        Filter used to determine if `klass` has tag or expected tag values.
+        Filter used to determine if ``klass`` has tag or expected tag values.
 
         - If a str or list of strings is provided, the return will be filtered
           to keep classes that have all the tag(s) specified by the strings.
-        - If a dict is provided, the return will be filtered to keep classes
-          that have all dict keys as tags. Tag values are also checked such that:
-
-          - If a dict key maps to a single value only classes with tag values equal
-            to the value are returned.
-          - If a dict key maps to multiple values (e.g., list) only classes with
-            tag values in these values are returned.
-          - If tag values are iterable,
-            condition is "at least one search value is contained in tag values".
+        - If a dict is provided, the return will be filtered to keep exactly the classes
+          where tags satisfy all the filter conditions specified by ``filter_tags``.
+          Filter conditions are as follows, for ``tag_name: search_value`` pairs in
+          the ``filter_tags`` dict.
+
+          - If ``klass`` does not have a tag with name ``tag_name``, it is excluded.
+            Otherwise, let ``tag_value`` be the value of the tag with name ``tag_name``.
+          - If ``search_value`` is a string, and ``tag_value`` is a string,
+            the filter condition is that ``search_value`` must match the tag value.
+          - If ``search_value`` is a string, and ``tag_value`` is a list,
+            the filter condition is that ``search_value`` is contained in ``tag_value``.
+          - If ``search_value`` is a ``re.Pattern``, and ``tag_value`` is a string,
+            the filter condition is that ``search_value.fullmatch(tag_value)``
+            is true, i.e., the regex matches the tag value.
+          - If ``search_value`` is a ``re.Pattern``, and ``tag_value`` is a list,
+            the filter condition is that at least one element of ``tag_value``
+            matches the regex.
+          - If ``search_value`` is iterable, then the filter condition is that
+            at least one element of ``search_value`` satisfies the above conditions,
+            applied to ``tag_value``.
 
     exclude_objects: str or list[str], default=None
         Names of estimators to exclude.
+
     as_dataframe: bool, default=False
 
         - If False, `all_objects` will return a list (either a list of
           `skbase` objects or a list of tuples, see Returns).
         - If True, `all_objects` will return a `pandas.DataFrame` with named
             columns for all of the attributes being returned.
             this requires soft dependency `pandas` to be installed.
 
     return_tags: str or list of str, default=None
         Names of tags to fetch and return each object's value of. The tag values
         named in return_tags will be fetched for each object and will be appended
         as either columns or tuple entries.
+
     package_name : str, default="skbase".
         Should be set to default to package or module name that objects will
-        be retrieved from. Objects will be searched inside `package_name`,
-        including in sub-modules (e.g., in package_name, package_name.module1,
-        package.module2, and package.module1.module3).
+        be retrieved from. Objects will be searched inside ``package_name``,
+        including in sub-modules (e.g., in ``package_name``, ``package_name.module1``,
+        ``package.module2``, and ``package.module1.module3``).
+
     path : str, default=None
         If provided, this should be the path that should be used as root
         to find `package_name` and start the search for any submodules/packages.
         This can be left at the default value (None) if searching in an installed
         package.
+
     modules_to_ignore : str or list[str], default=None
         The modules that should be ignored when searching across the modules to
-        gather objects. If passed, `all_objects` ignores modules or submodules
+        gather objects. If passed, ``all_objects`` ignores modules or submodules
         of a module whose name is in the provided string(s). E.g., if
-        `modules_to_ignore` contains the string `"foo"`, then `"bar.foo"`,
-        `"foo"`, `"foo.bar"`, `"bar.foo.bar"` are ignored.
+        ``modules_to_ignore`` contains the string ``"foo"``, then ``"bar.foo"``,
+        ``"foo"``, ``"foo.bar"``, ``"bar.foo.bar"`` are ignored.
 
     class_lookup : dict[str, class], default=None
         Dictionary of string aliases for classes used in object_types. If provided,
-        `object_types` can accept str values or a list of string values.
+        ``object_types`` can accept str values or a list of string values.
 
-    Other Parameters
-    ----------------
     suppress_import_stdout : bool, default=True
         Whether to suppress stdout printout upon import.
+        If True, ``all_objects`` will suppress any stdout printout internally.
+        If False, ``all_objects`` will not suppress any stdout printout arising
+        from crawling the package.
 
     Returns
     -------
-    all_estimators will return one of the following:
+    ``all_objects`` will return one of the following:
 
-    - a pandas.DataFrame if `as_dataframe=True`, with columns:
+    - a pandas.DataFrame if ``as_dataframe=True``, with columns:
 
-      - "names" with the returned class names if `return_name=True`
+      - "names" with the returned class names if ``return_name=True``
       - "objects" with returned classes.
-      - optional columns named based on tags passed in `return_tags`
-        if `return_tags is not None`.
+      - optional columns named based on tags passed in ``return_tags``
+        if ``return_tags is not None``.
 
-    - a list if `as_dataframe=False`, where list elements are:
+    - a list if ``as_dataframe=False``, where list elements are:
 
-      - classes (that inherit from BaseObject) in alphabetic order by class name
-        if `return_names=False` and `return_tags=None.
-      - (name, class) tuples in alphabetic order by name if `return_names=True`
-        and `return_tags=None`.
+      - classes (that inherit from ``BaseObject``) in alphabetic order by class name
+        if ``return_names=False`` and ``return_tags=None``.
+      - (name, class) tuples in alphabetic order by name if ``return_names=True``
+        and ``return_tags=None``.
       - (name, class, tag-value1, ..., tag-valueN) tuples in alphabetic order by name
-        if `return_names=True` and `return_tags is not None`.
+        if ``return_names=True`` and ``return_tags is not None``.
       - (class, tag-value1, ..., tag-valueN) tuples in alphabetic order by
-        class name if `return_names=False` and `return_tags is not None`.
+        class name if ``return_names=False`` and ``return_tags is not None``.
 
     References
     ----------
-    Modified version of scikit-learn's and sktime's `all_estimators()` to allow
-    users to find BaseObjects in `skbase` and other packages.
+    Modified version of ``scikit-learn``'s and sktime's ``all_estimators`` to allow
+    users to find ``BaseObject`` descendants in ``skbase`` and other packages.
     """
-    module, root, _ = _determine_module_path(package_name, path)
-    if modules_to_ignore is None:
-        modules_to_ignore = []
-    if exclude_objects is None:
-        exclude_objects = []
+    _, root, _ = _determine_module_path(package_name, path)
+    modules_to_ignore = _coerce_to_tuple(modules_to_ignore)
+    exclude_objects = _coerce_to_tuple(exclude_objects)
 
-    all_estimators = []
-
-    def _is_base_class(name):
-        return name.startswith("_") or name.startswith("Base")
-
-    def _is_estimator(name, klass):
-        # Check if klass is subclass of base estimators, not a base class itself and
-        # not an abstract class
-        if object_types is None:
-            return issubclass(klass, BaseObject) and not _is_base_class(name)
-        else:
-            return not _is_base_class(name)
+    if object_types is None:
+        obj_types = BaseObject
+    else:
+        obj_types = _check_object_types(object_types, class_lookup)
 
     # Ignore deprecation warnings triggered at import time and from walking packages
-    with warnings.catch_warnings():
+    with warnings.catch_warnings(), StdoutMute(active=suppress_import_stdout):
         warnings.simplefilter("ignore", category=FutureWarning)
         warnings.simplefilter("module", category=ImportWarning)
         warnings.filterwarnings(
             "ignore", category=UserWarning, message=".*has been moved to.*"
         )
-        prefix = f"{package_name}."
-        for module_name, _, _ in _walk(
-            root=root, exclude=modules_to_ignore, prefix=prefix
-        ):
-            # Filter modules
-            if _is_non_public_module(module_name):
-                continue
-
-            try:
-                if suppress_import_stdout:
-                    # setup text trap, import, then restore
-                    sys.stdout = io.StringIO()
-                    module = importlib.import_module(module_name)
-                    sys.stdout = sys.__stdout__
-                else:
-                    module = importlib.import_module(module_name)
-                classes = inspect.getmembers(module, inspect.isclass)
-                # Filter classes
-                estimators = [
-                    (klass.__name__, klass)
-                    for _, klass in classes
-                    if _is_estimator(klass.__name__, klass)
-                ]
-                all_estimators.extend(estimators)
-            except ModuleNotFoundError as e:
-                # Skip missing soft dependencies
-                if "soft dependency" not in str(e):
-                    raise e
-                warnings.warn(str(e), ImportWarning, stacklevel=2)
-
-    # Drop duplicates
-    all_estimators = set(all_estimators)
+        all_estimators = _walk_and_retrieve_all_objs(
+            root=root, package_name=package_name, modules_to_ignore=modules_to_ignore
+        )
 
     # Filter based on given estimator types
-    if object_types:
-        obj_types = _check_object_types(object_types, class_lookup)
-        all_estimators = [
-            (n, est) for (n, est) in all_estimators if _filter_by_class(est, obj_types)
-        ]
+    all_estimators = [
+        (n, est) for (n, est) in all_estimators if _filter_by_class(est, obj_types)
+    ]
 
     # Filter based on given exclude list
     if exclude_objects:
         exclude_objects = check_sequence(
             exclude_objects,
-            sequence_type=list,
+            sequence_type=tuple,
             element_type=str,
             coerce_scalar_input=True,
             sequence_name="exclude_object",
         )
         all_estimators = [
             (name, estimator)
             for name, estimator in all_estimators
@@ -1016,7 +1019,127 @@
     """Create pandas.DataFrame from all_objects.
 
     Kept as a separate function with import to isolate the pandas dependency.
     """
     import pandas as pd
 
     return pd.DataFrame(all_objects, columns=columns)
+
+
+class StdoutMute:
+    """A context manager to suppress stdout.
+
+    This class is used to suppress stdout when importing modules.
+
+    Also downgrades any ModuleNotFoundError to a warning if the error message
+    contains the substring "soft dependency".
+
+    Parameters
+    ----------
+    active : bool, default=True
+        Whether to suppress stdout or not.
+        If True, stdout is suppressed.
+        If False, stdout is not suppressed, and the context manager does nothing
+        except catch and suppress ModuleNotFoundError.
+    """
+
+    def __init__(self, active=True):
+        self.active = active
+
+    def __enter__(self):
+        """Context manager entry point."""
+        # capture stdout if active
+        # store the original stdout so it can be restored in __exit__
+        if self.active:
+            self._stdout = sys.stdout
+            sys.stdout = io.StringIO()
+
+    def __exit__(self, type, value, traceback):  # noqa: A002
+        """Context manager exit point."""
+        # restore stdout if active
+        # if not active, nothing needs to be done, since stdout was not replaced
+        if self.active:
+            sys.stdout = self._stdout
+
+        if type is not None:
+            # if a ModuleNotFoundError is raised,
+            # we suppress to a warning if "soft dependency" is in the error message
+            # otherwise, raise
+            if type is ModuleNotFoundError:
+                if "soft dependency" not in str(value):
+                    return False
+                warnings.warn(str(value), ImportWarning, stacklevel=2)
+                return True
+
+            # all other exceptions are raised
+            return False
+        # if no exception was raised, return True to indicate successful exit
+        # return statement not needed as type was None, but included for clarity
+        return True
+
+
+def _coerce_to_tuple(x):
+    if x is None:
+        return ()
+    elif isinstance(x, tuple):
+        return x
+    elif isinstance(x, list):
+        return tuple(x)
+    else:
+        return (x,)
+
+
+@lru_cache(maxsize=100)
+def _walk_and_retrieve_all_objs(root, package_name, modules_to_ignore):
+    """Walk through the package and retrieve all BaseObject descendants.
+
+    Excludes objects:
+
+    * located in modules with a subpath starting with underscore
+    * located in modules with a subpath in ``modules_to_ignore``
+    * whose name starts with an underscore or ``"Base"``
+
+    Parameters
+    ----------
+    root : str or path-like
+        Root path in which to look for submodules. Can be a string path,
+        pathlib.Path or other path-like object.
+    package_name : str
+        The name of the package/module to return metadata for.
+    modules_to_ignore : tuple[str]
+        The modules that should be ignored when searching across the modules to
+        gather objects. If passed, `all_objects` ignores modules or submodules
+        of a module whose name is in the provided string(s). E.g., if
+        `modules_to_ignore` contains the string `"foo"`, then `"bar.foo"`,
+        `"foo"`, `"foo.bar"`, `"bar.foo.bar"` are ignored.
+
+    Returns
+    -------
+    all_estimators : tuple of (str, class) tuples
+        List of all estimators found in the package.
+    """
+    prefix = f"{package_name}."
+
+    def _is_base_class(name):
+        return name.startswith("_") or name.startswith("Base")
+
+    all_estimators = []
+
+    for module_name, _, _ in _walk(root=root, exclude=modules_to_ignore, prefix=prefix):
+        # Filter modules
+        if _is_non_public_module(module_name):
+            continue
+
+        module = importlib.import_module(module_name)
+        classes = inspect.getmembers(module, inspect.isclass)
+        # Filter classes
+        estimators = [
+            (klass.__name__, klass)
+            for _, klass in classes
+            if not _is_base_class(klass.__name__)
+        ]
+        all_estimators.extend(estimators)
+
+    # Drop duplicates
+    all_estimators = set(all_estimators)
+    all_estimators = tuple(all_estimators)
+    return all_estimators
```

### Comparing `scikit_base-0.7.8/skbase/lookup/tests/test_lookup.py` & `scikit_base-0.8.0/skbase/lookup/tests/test_lookup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # copyright: skbase developers, BSD-3-Clause License (see LICENSE file)
 """Tests for skbase lookup functionality."""
 # Elements of the lookup tests reuse code developed in sktime. These elements
 # are copyrighted by the sktime developers, BSD-3-Clause License. For
 # conditions see https://github.com/sktime/sktime/blob/main/LICENSE
 import importlib
 import pathlib
+import sys
 from copy import deepcopy
 from types import ModuleType
 from typing import List
 
 import pandas as pd
 import pytest
 
@@ -38,15 +39,15 @@
 )
 from skbase.tests.mock_package.test_mock_package import (
     MOCK_PACKAGE_OBJECTS,
     CompositionDummy,
     NotABaseObject,
 )
 
-__author__: List[str] = ["RNKuhns"]
+__author__: List[str] = ["RNKuhns", "fkiraly"]
 __all__: List[str] = []
 
 
 MODULE_METADATA_EXPECTED_KEYS = (
     "path",
     "name",
     "classes",
@@ -391,23 +392,23 @@
     assert _filter_by_tags(Parent, {"A": "1", "B": 2}) is True
     # All keys in dict are in tag_filter, but at least 1 value doesn't match
     assert _filter_by_tags(Parent, {"A": 1, "B": 2}) is False
     # At least 1 key in dict is not in tag_filter
     assert _filter_by_tags(Parent, {"E": 1, "B": 2}) is False
 
     # Iterable tags should be all strings
-    with pytest.raises(ValueError, match=r"tag_filter"):
+    with pytest.raises(ValueError, match=r"filter_tags"):
         assert _filter_by_tags(Parent, ("A", "B", 3))
 
     # Tags that aren't iterable have to be strings
-    with pytest.raises(TypeError, match=r"tag_filter"):
+    with pytest.raises(TypeError, match=r"filter_tags"):
         assert _filter_by_tags(Parent, 7.0)
 
     # Dictionary tags should have string keys
-    with pytest.raises(ValueError, match=r"tag_filter"):
+    with pytest.raises(ValueError, match=r"filter_tags"):
         assert _filter_by_tags(Parent, {7: 11})
 
 
 def test_walk_returns_expected_format(fixture_skbase_root_path):
     """Check walk function returns expected format."""
 
     def _test_walk_return(p):
@@ -844,24 +845,36 @@
     as_dataframe,
     return_names,
     return_tags,
     modules_to_ignore,
     exclude_objects,
     suppress_import_stdout,
 ):
-    """Test that all_objects return argument has correct type."""
+    """Test that all_objects return argument has correct type.
+
+    Also tested: sys.stdout is unchanged after function call, see bug #327.
+    """
+    # we will check later that sys.stdout is unchanged
+    initial_stdout = sys.stdout
+
+    # call all_objects
     objs = all_objects(
         package_name="skbase",
         exclude_objects=exclude_objects,
         return_names=return_names,
         as_dataframe=as_dataframe,
         return_tags=return_tags,
         modules_to_ignore=modules_to_ignore,
         suppress_import_stdout=suppress_import_stdout,
     )
+
+    # verify sys.stdout is unchanged
+    assert sys.stdout == initial_stdout
+
+    # verify output has expected types
     if isinstance(modules_to_ignore, str):
         modules_to_ignore = (modules_to_ignore,)
     if (
         modules_to_ignore is not None
         and "tests" in modules_to_ignore
         # and "mock_package" in modules_to_ignore
     ):
@@ -980,14 +993,51 @@
     if tag_filter is None:
         assert len(unfiltered_classes) == len(filtered_classes)
         assert unfiltered_classes == filtered_classes
     else:
         assert len(unfiltered_classes) > len(filtered_classes)
 
 
+def test_all_object_tag_filter_regex():
+    """Test all_objects filters by tag as expected, when using regex."""
+    import re
+
+    # search for class where "A" has at least one 1, and "C" has "23" in the tag value
+    # this sohuld find Parent but not Child
+    filter_tags = {"A": re.compile(r"^(?=.*1).*$"), "C": re.compile(r".+23.+")}
+
+    # Results applying filter
+    objs = all_objects(
+        package_name="skbase",
+        return_names=True,
+        as_dataframe=True,
+        return_tags=None,
+        filter_tags=filter_tags,
+    )
+    filtered_classes = objs.iloc[:, 1].tolist()
+    # Verify filtered results have right output type
+    _check_all_object_output_types(
+        objs, as_dataframe=True, return_names=True, return_tags=None
+    )
+
+    # Results without filter
+    objs = all_objects(
+        package_name="skbase",
+        return_names=True,
+        as_dataframe=True,
+        return_tags=None,
+    )
+    unfiltered_classes = objs.iloc[:, 1].tolist()
+
+    # as stated above, we should find only Parent (and not Child)
+    assert len(unfiltered_classes) > len(filtered_classes)
+    names = [kls.__name__ for kls in filtered_classes]
+    assert "Parent" in names
+
+
 @pytest.mark.parametrize("class_lookup", [{"base_object": BaseObject}])
 @pytest.mark.parametrize("class_filter", [None, "base_object"])
 def test_all_object_class_lookup(class_lookup, class_filter):
     """Test all_objects class_lookup parameter works as expected.."""
     # Results applying filter
     objs = all_objects(
         package_name="skbase",
```

### Comparing `scikit_base-0.7.8/skbase/testing/test_all_objects.py` & `scikit_base-0.8.0/skbase/testing/test_all_objects.py`

 * *Files identical despite different names*

### Comparing `scikit_base-0.7.8/skbase/testing/utils/_conditional_fixtures.py` & `scikit_base-0.8.0/skbase/testing/utils/_conditional_fixtures.py`

 * *Files identical despite different names*

### Comparing `scikit_base-0.7.8/skbase/testing/utils/inspect.py` & `scikit_base-0.8.0/skbase/testing/utils/inspect.py`

 * *Files identical despite different names*

### Comparing `scikit_base-0.7.8/skbase/tests/conftest.py` & `scikit_base-0.8.0/skbase/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,15 +95,15 @@
     "skbase.base._meta": (
         "BaseMetaObject",
         "BaseMetaObjectMixin",
         "BaseMetaEstimator",
         "BaseMetaEstimatorMixin",
     ),
     "skbase.base._pretty_printing._pprint": ("KeyValTuple", "KeyValTupleParam"),
-    "skbase.lookup._lookup": (),
+    "skbase.lookup._lookup": ("StdoutMute",),
     "skbase.testing": ("BaseFixtureGenerator", "QuickTester", "TestAllObjects"),
     "skbase.testing.test_all_objects": (
         "BaseFixtureGenerator",
         "QuickTester",
         "TestAllObjects",
     ),
 }
@@ -199,14 +199,15 @@
             "_make_dataframe",
             "_walk",
             "_filter_by_tags",
             "_filter_by_class",
             "_import_module",
             "_check_object_types",
             "_get_module_info",
+            "_coerce_to_tuple",
         ),
         "skbase.testing.utils.inspect": ("_get_args",),
         "skbase.utils._check": ("_is_scalar_nan",),
         "skbase.utils.dependencies": (
             "_check_soft_dependencies",
             "_check_python_version",
             "_check_estimator_deps",
```

### Comparing `scikit_base-0.7.8/skbase/tests/mock_package/test_mock_package.py` & `scikit_base-0.8.0/skbase/tests/mock_package/test_mock_package.py`

 * *Files identical despite different names*

### Comparing `scikit_base-0.7.8/skbase/tests/test_base.py` & `scikit_base-0.8.0/skbase/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `scikit_base-0.7.8/skbase/tests/test_baseestimator.py` & `scikit_base-0.8.0/skbase/tests/test_baseestimator.py`

 * *Files identical despite different names*

### Comparing `scikit_base-0.7.8/skbase/tests/test_exceptions.py` & `scikit_base-0.8.0/skbase/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `scikit_base-0.7.8/skbase/tests/test_meta.py` & `scikit_base-0.8.0/skbase/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `scikit_base-0.7.8/skbase/utils/__init__.py` & `scikit_base-0.8.0/skbase/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit_base-0.7.8/skbase/utils/_check.py` & `scikit_base-0.8.0/skbase/utils/_check.py`

 * *Files identical despite different names*

### Comparing `scikit_base-0.7.8/skbase/utils/_iter.py` & `scikit_base-0.8.0/skbase/utils/_iter.py`

 * *Files identical despite different names*

### Comparing `scikit_base-0.7.8/skbase/utils/_nested_iter.py` & `scikit_base-0.8.0/skbase/utils/_nested_iter.py`

 * *Files identical despite different names*

### Comparing `scikit_base-0.7.8/skbase/utils/_utils.py` & `scikit_base-0.8.0/skbase/utils/_utils.py`

 * *Files identical despite different names*

### Comparing `scikit_base-0.7.8/skbase/utils/deep_equals/_common.py` & `scikit_base-0.8.0/skbase/utils/deep_equals/_common.py`

 * *Files identical despite different names*

### Comparing `scikit_base-0.7.8/skbase/utils/deep_equals/_deep_equals.py` & `scikit_base-0.8.0/skbase/utils/deep_equals/_deep_equals.py`

 * *Files identical despite different names*

### Comparing `scikit_base-0.7.8/skbase/utils/dependencies/_dependencies.py` & `scikit_base-0.8.0/skbase/utils/dependencies/_dependencies.py`

 * *Files identical despite different names*

### Comparing `scikit_base-0.7.8/skbase/utils/dependencies/tests/test_check_dependencies.py` & `scikit_base-0.8.0/skbase/utils/dependencies/tests/test_check_dependencies.py`

 * *Files identical despite different names*

### Comparing `scikit_base-0.7.8/skbase/utils/random_state.py` & `scikit_base-0.8.0/skbase/utils/random_state.py`

 * *Files identical despite different names*

### Comparing `scikit_base-0.7.8/skbase/utils/tests/test_check.py` & `scikit_base-0.8.0/skbase/utils/tests/test_check.py`

 * *Files identical despite different names*

### Comparing `scikit_base-0.7.8/skbase/utils/tests/test_deep_equals.py` & `scikit_base-0.8.0/skbase/utils/tests/test_deep_equals.py`

 * *Files identical despite different names*

### Comparing `scikit_base-0.7.8/skbase/utils/tests/test_iter.py` & `scikit_base-0.8.0/skbase/utils/tests/test_iter.py`

 * *Files identical despite different names*

### Comparing `scikit_base-0.7.8/skbase/utils/tests/test_nested_iter.py` & `scikit_base-0.8.0/skbase/utils/tests/test_nested_iter.py`

 * *Files identical despite different names*

### Comparing `scikit_base-0.7.8/skbase/utils/tests/test_random_state.py` & `scikit_base-0.8.0/skbase/utils/tests/test_random_state.py`

 * *Files identical despite different names*

### Comparing `scikit_base-0.7.8/skbase/utils/tests/test_utils.py` & `scikit_base-0.8.0/skbase/utils/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `scikit_base-0.7.8/skbase/validate/__init__.py` & `scikit_base-0.8.0/skbase/validate/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit_base-0.7.8/skbase/validate/_named_objects.py` & `scikit_base-0.8.0/skbase/validate/_named_objects.py`

 * *Files identical despite different names*

### Comparing `scikit_base-0.7.8/skbase/validate/_types.py` & `scikit_base-0.8.0/skbase/validate/_types.py`

 * *Files identical despite different names*

### Comparing `scikit_base-0.7.8/skbase/validate/tests/test_iterable_named_objects.py` & `scikit_base-0.8.0/skbase/validate/tests/test_iterable_named_objects.py`

 * *Files identical despite different names*

### Comparing `scikit_base-0.7.8/skbase/validate/tests/test_type_validations.py` & `scikit_base-0.8.0/skbase/validate/tests/test_type_validations.py`

 * *Files identical despite different names*

