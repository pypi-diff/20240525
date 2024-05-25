# Comparing `tmp/aioreactive-0.8.0.tar.gz` & `tmp/aioreactive-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aioreactive-0.8.0.tar", last modified: Sun Nov 22 21:53:42 2020, max compression
+gzip compressed data, was "dist/aioreactive-0.9.0.tar", last modified: Mon Nov 23 23:03:30 2020, max compression
```

## Comparing `aioreactive-0.8.0.tar` & `aioreactive-0.9.0.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-22 21:53:42.732620 aioreactive-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (116)       54 2020-11-22 21:53:32.000000 aioreactive-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)    19559 2020-11-22 21:53:42.732620 aioreactive-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)    15689 2020-11-22 21:53:32.000000 aioreactive-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-22 21:53:42.732620 aioreactive-0.8.0/aioreactive/
--rw-r--r--   0 runner    (1001) docker     (116)    20419 2020-11-22 21:53:32.000000 aioreactive-0.8.0/aioreactive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      497 2020-11-22 21:53:42.732620 aioreactive-0.8.0/aioreactive/_version.py
--rw-r--r--   0 runner    (1001) docker     (116)    13323 2020-11-22 21:53:32.000000 aioreactive-0.8.0/aioreactive/combine.py
--rw-r--r--   0 runner    (1001) docker     (116)     5731 2020-11-22 21:53:32.000000 aioreactive-0.8.0/aioreactive/create.py
--rw-r--r--   0 runner    (1001) docker     (116)    14502 2020-11-22 21:53:32.000000 aioreactive-0.8.0/aioreactive/filtering.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-22 21:53:42.728620 aioreactive-0.8.0/aioreactive/iterable/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-11-22 21:53:32.000000 aioreactive-0.8.0/aioreactive/iterable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      513 2020-11-22 21:53:32.000000 aioreactive-0.8.0/aioreactive/iterable/to_async_observable.py
--rw-r--r--   0 runner    (1001) docker     (116)      571 2020-11-22 21:53:32.000000 aioreactive-0.8.0/aioreactive/leave.py
--rw-r--r--   0 runner    (1001) docker     (116)     4249 2020-11-22 21:53:32.000000 aioreactive-0.8.0/aioreactive/msg.py
--rw-r--r--   0 runner    (1001) docker     (116)     5625 2020-11-22 21:53:32.000000 aioreactive-0.8.0/aioreactive/notification.py
--rw-r--r--   0 runner    (1001) docker     (116)     1632 2020-11-22 21:53:32.000000 aioreactive-0.8.0/aioreactive/observables.py
--rw-r--r--   0 runner    (1001) docker     (116)     9368 2020-11-22 21:53:32.000000 aioreactive-0.8.0/aioreactive/observers.py
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-11-22 21:53:32.000000 aioreactive-0.8.0/aioreactive/py.typed
--rw-r--r--   0 runner    (1001) docker     (116)     4535 2020-11-22 21:53:32.000000 aioreactive-0.8.0/aioreactive/subject.py
--rw-r--r--   0 runner    (1001) docker     (116)     1767 2020-11-22 21:53:32.000000 aioreactive-0.8.0/aioreactive/subscription.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-22 21:53:42.728620 aioreactive-0.8.0/aioreactive/testing/
--rw-r--r--   0 runner    (1001) docker     (116)      361 2020-11-22 21:53:32.000000 aioreactive-0.8.0/aioreactive/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2201 2020-11-22 21:53:32.000000 aioreactive-0.8.0/aioreactive/testing/observer.py
--rw-r--r--   0 runner    (1001) docker     (116)     2484 2020-11-22 21:53:32.000000 aioreactive-0.8.0/aioreactive/testing/subject.py
--rw-r--r--   0 runner    (1001) docker     (116)      150 2020-11-22 21:53:32.000000 aioreactive-0.8.0/aioreactive/testing/utils.py
--rw-r--r--   0 runner    (1001) docker     (116)     4403 2020-11-22 21:53:32.000000 aioreactive-0.8.0/aioreactive/testing/virtual_events.py
--rw-r--r--   0 runner    (1001) docker     (116)     5863 2020-11-22 21:53:32.000000 aioreactive-0.8.0/aioreactive/timeshift.py
--rw-r--r--   0 runner    (1001) docker     (116)    13204 2020-11-22 21:53:32.000000 aioreactive-0.8.0/aioreactive/transform.py
--rw-r--r--   0 runner    (1001) docker     (116)     1092 2020-11-22 21:53:32.000000 aioreactive-0.8.0/aioreactive/types.py
--rw-r--r--   0 runner    (1001) docker     (116)      754 2020-11-22 21:53:32.000000 aioreactive-0.8.0/aioreactive/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-22 21:53:42.728620 aioreactive-0.8.0/aioreactive.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)    19559 2020-11-22 21:53:42.000000 aioreactive-0.8.0/aioreactive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1367 2020-11-22 21:53:42.000000 aioreactive-0.8.0/aioreactive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-11-22 21:53:42.000000 aioreactive-0.8.0/aioreactive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       11 2020-11-22 21:53:42.000000 aioreactive-0.8.0/aioreactive.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       17 2020-11-22 21:53:42.000000 aioreactive-0.8.0/aioreactive.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-11-22 21:53:42.000000 aioreactive-0.8.0/aioreactive.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)      269 2020-11-22 21:53:42.732620 aioreactive-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1641 2020-11-22 21:53:32.000000 aioreactive-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-22 21:53:42.732620 aioreactive-0.8.0/test/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-11-22 21:53:32.000000 aioreactive-0.8.0/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1972 2020-11-22 21:53:32.000000 aioreactive-0.8.0/test/test_async_iteration.py
--rw-r--r--   0 runner    (1001) docker     (116)     2080 2020-11-22 21:53:32.000000 aioreactive-0.8.0/test/test_chain.py
--rw-r--r--   0 runner    (1001) docker     (116)      545 2020-11-22 21:53:32.000000 aioreactive-0.8.0/test/test_concat.py
--rw-r--r--   0 runner    (1001) docker     (116)     1520 2020-11-22 21:53:32.000000 aioreactive-0.8.0/test/test_debounce.py
--rw-r--r--   0 runner    (1001) docker     (116)     1821 2020-11-22 21:53:32.000000 aioreactive-0.8.0/test/test_delay.py
--rw-r--r--   0 runner    (1001) docker     (116)     1184 2020-11-22 21:53:32.000000 aioreactive-0.8.0/test/test_distinct_until_changed.py
--rw-r--r--   0 runner    (1001) docker     (116)     1879 2020-11-22 21:53:32.000000 aioreactive-0.8.0/test/test_eventloop.py
--rw-r--r--   0 runner    (1001) docker     (116)     1311 2020-11-22 21:53:32.000000 aioreactive-0.8.0/test/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (116)     2446 2020-11-22 21:53:32.000000 aioreactive-0.8.0/test/test_flat_map.py
--rw-r--r--   0 runner    (1001) docker     (116)     1994 2020-11-22 21:53:32.000000 aioreactive-0.8.0/test/test_forward_pipe.py
--rw-r--r--   0 runner    (1001) docker     (116)     1751 2020-11-22 21:53:32.000000 aioreactive-0.8.0/test/test_from_iterable.py
--rw-r--r--   0 runner    (1001) docker     (116)     2531 2020-11-22 21:53:32.000000 aioreactive-0.8.0/test/test_map.py
--rw-r--r--   0 runner    (1001) docker     (116)     2346 2020-11-22 21:53:32.000000 aioreactive-0.8.0/test/test_merge.py
--rw-r--r--   0 runner    (1001) docker     (116)     2074 2020-11-22 21:53:32.000000 aioreactive-0.8.0/test/test_pipe.py
--rw-r--r--   0 runner    (1001) docker     (116)     3150 2020-11-22 21:53:32.000000 aioreactive-0.8.0/test/test_single.py
--rw-r--r--   0 runner    (1001) docker     (116)     5473 2020-11-22 21:53:32.000000 aioreactive-0.8.0/test/test_single_stream.py
--rw-r--r--   0 runner    (1001) docker     (116)     1147 2020-11-22 21:53:32.000000 aioreactive-0.8.0/test/test_slice.py
--rw-r--r--   0 runner    (1001) docker     (116)     4126 2020-11-22 21:53:32.000000 aioreactive-0.8.0/test/test_stream.py
--rw-r--r--   0 runner    (1001) docker     (116)     1536 2020-11-22 21:53:32.000000 aioreactive-0.8.0/test/test_take.py
--rw-r--r--   0 runner    (1001) docker     (116)     1984 2020-11-22 21:53:32.000000 aioreactive-0.8.0/test/test_with_latest_from.py
--rw-r--r--   0 runner    (1001) docker     (116)    68611 2020-11-22 21:53:32.000000 aioreactive-0.8.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-23 23:03:30.500197 aioreactive-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (116)       54 2020-11-23 23:03:20.000000 aioreactive-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)    19968 2020-11-23 23:03:30.500197 aioreactive-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)    16056 2020-11-23 23:03:20.000000 aioreactive-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-23 23:03:30.500197 aioreactive-0.9.0/aioreactive/
+-rw-r--r--   0 runner    (1001) docker     (116)    26287 2020-11-23 23:03:20.000000 aioreactive-0.9.0/aioreactive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      497 2020-11-23 23:03:30.500197 aioreactive-0.9.0/aioreactive/_version.py
+-rw-r--r--   0 runner    (1001) docker     (116)    13323 2020-11-23 23:03:20.000000 aioreactive-0.9.0/aioreactive/combine.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5731 2020-11-23 23:03:20.000000 aioreactive-0.9.0/aioreactive/create.py
+-rw-r--r--   0 runner    (1001) docker     (116)    13053 2020-11-23 23:03:20.000000 aioreactive-0.9.0/aioreactive/filtering.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-23 23:03:30.496197 aioreactive-0.9.0/aioreactive/iterable/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-11-23 23:03:20.000000 aioreactive-0.9.0/aioreactive/iterable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      513 2020-11-23 23:03:20.000000 aioreactive-0.9.0/aioreactive/iterable/to_async_observable.py
+-rw-r--r--   0 runner    (1001) docker     (116)      571 2020-11-23 23:03:20.000000 aioreactive-0.9.0/aioreactive/leave.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4249 2020-11-23 23:03:20.000000 aioreactive-0.9.0/aioreactive/msg.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5625 2020-11-23 23:03:20.000000 aioreactive-0.9.0/aioreactive/notification.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1681 2020-11-23 23:03:20.000000 aioreactive-0.9.0/aioreactive/observables.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9368 2020-11-23 23:03:20.000000 aioreactive-0.9.0/aioreactive/observers.py
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-11-23 23:03:20.000000 aioreactive-0.9.0/aioreactive/py.typed
+-rw-r--r--   0 runner    (1001) docker     (116)     4535 2020-11-23 23:03:20.000000 aioreactive-0.9.0/aioreactive/subject.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1767 2020-11-23 23:03:20.000000 aioreactive-0.9.0/aioreactive/subscription.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-23 23:03:30.496197 aioreactive-0.9.0/aioreactive/testing/
+-rw-r--r--   0 runner    (1001) docker     (116)      361 2020-11-23 23:03:20.000000 aioreactive-0.9.0/aioreactive/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2201 2020-11-23 23:03:20.000000 aioreactive-0.9.0/aioreactive/testing/observer.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2484 2020-11-23 23:03:20.000000 aioreactive-0.9.0/aioreactive/testing/subject.py
+-rw-r--r--   0 runner    (1001) docker     (116)      150 2020-11-23 23:03:20.000000 aioreactive-0.9.0/aioreactive/testing/utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4403 2020-11-23 23:03:20.000000 aioreactive-0.9.0/aioreactive/testing/virtual_events.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5863 2020-11-23 23:03:20.000000 aioreactive-0.9.0/aioreactive/timeshift.py
+-rw-r--r--   0 runner    (1001) docker     (116)    13204 2020-11-23 23:03:20.000000 aioreactive-0.9.0/aioreactive/transform.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1092 2020-11-23 23:03:20.000000 aioreactive-0.9.0/aioreactive/types.py
+-rw-r--r--   0 runner    (1001) docker     (116)      754 2020-11-23 23:03:20.000000 aioreactive-0.9.0/aioreactive/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-23 23:03:30.496197 aioreactive-0.9.0/aioreactive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)    19968 2020-11-23 23:03:30.000000 aioreactive-0.9.0/aioreactive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     1367 2020-11-23 23:03:30.000000 aioreactive-0.9.0/aioreactive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-11-23 23:03:30.000000 aioreactive-0.9.0/aioreactive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       11 2020-11-23 23:03:30.000000 aioreactive-0.9.0/aioreactive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       17 2020-11-23 23:03:30.000000 aioreactive-0.9.0/aioreactive.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-11-23 23:03:30.000000 aioreactive-0.9.0/aioreactive.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (116)      269 2020-11-23 23:03:30.500197 aioreactive-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     1641 2020-11-23 23:03:20.000000 aioreactive-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-23 23:03:30.500197 aioreactive-0.9.0/test/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-11-23 23:03:20.000000 aioreactive-0.9.0/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1972 2020-11-23 23:03:20.000000 aioreactive-0.9.0/test/test_async_iteration.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2080 2020-11-23 23:03:20.000000 aioreactive-0.9.0/test/test_chain.py
+-rw-r--r--   0 runner    (1001) docker     (116)      545 2020-11-23 23:03:20.000000 aioreactive-0.9.0/test/test_concat.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1520 2020-11-23 23:03:20.000000 aioreactive-0.9.0/test/test_debounce.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1821 2020-11-23 23:03:20.000000 aioreactive-0.9.0/test/test_delay.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1184 2020-11-23 23:03:20.000000 aioreactive-0.9.0/test/test_distinct_until_changed.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1879 2020-11-23 23:03:20.000000 aioreactive-0.9.0/test/test_eventloop.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1311 2020-11-23 23:03:20.000000 aioreactive-0.9.0/test/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2446 2020-11-23 23:03:20.000000 aioreactive-0.9.0/test/test_flat_map.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1994 2020-11-23 23:03:20.000000 aioreactive-0.9.0/test/test_forward_pipe.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1751 2020-11-23 23:03:20.000000 aioreactive-0.9.0/test/test_from_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2531 2020-11-23 23:03:20.000000 aioreactive-0.9.0/test/test_map.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2346 2020-11-23 23:03:20.000000 aioreactive-0.9.0/test/test_merge.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2074 2020-11-23 23:03:20.000000 aioreactive-0.9.0/test/test_pipe.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3150 2020-11-23 23:03:20.000000 aioreactive-0.9.0/test/test_single.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5473 2020-11-23 23:03:20.000000 aioreactive-0.9.0/test/test_single_stream.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1147 2020-11-23 23:03:20.000000 aioreactive-0.9.0/test/test_slice.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4126 2020-11-23 23:03:20.000000 aioreactive-0.9.0/test/test_stream.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1536 2020-11-23 23:03:20.000000 aioreactive-0.9.0/test/test_take.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1984 2020-11-23 23:03:20.000000 aioreactive-0.9.0/test/test_with_latest_from.py
+-rw-r--r--   0 runner    (1001) docker     (116)    68611 2020-11-23 23:03:20.000000 aioreactive-0.9.0/versioneer.py
```

### Comparing `aioreactive-0.8.0/PKG-INFO` & `aioreactive-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioreactive
-Version: 0.8.0
+Version: 0.9.0
 Summary: Async/await Reactive Tools for Python 3.9+
 Home-page: https://github.com/dbrattli/aioreactive
 Author: Børge Lanes & Dag Brattli
 Author-email: dag@brattli.net
 License: MIT License
 Download-URL: https://github.com/dbrattli/aioreactive
 Description: 
@@ -200,23 +200,29 @@
         apply them to an observable and compose it into a transformed, filtered,
         aggregated or combined observable. This transformed observable can be
         streamed into an observer.
         
             Observable -> Operator -> Operator -> Operator -> Observer
         
         Aioreactive contains many of the same operators as you know from RxPY.
-        Our goal is not to implement them all, but to have the most essential
+        Our goal is not to implement them all, but to provide the most essential
         ones.
         
         * **concat** -- Concatenates two or more observables.
+        * **choose** -- Filters and/or transforms the observable.
+        * **choose_asnc** -- Asynchronously filters and/or transforms the observable.
         * **debounce** -- Throttles an observable.
         * **delay** -- delays the items within an observable.
         * **distinct_until_changed** -- an observable with continuously distinct values.
         * **filter** -- filters an observable.
+        * **filteri** -- filters an observable with index.
         * **flat_map** -- transforms an observable into a stream of observables and flattens the resulting observable.
+        * **flat_map_latest** -- transforms an observable into a stream of
+          observables and flattens the resulting observable by producing values
+          from the latest observable.
         * **from_iterable** -- Create an observable from an (async) iterable.
         * **subscribe** -- Subscribes an observer to an observable. Returns a subscription.
         * **map** -- transforms an observable.
         * **mapi** -- transforms an observable with index.
         * **map_async** -- transforms an observable asynchronously.
         * **mapi_async** -- transforms an observable asynchronously with index.
         * **merge_inner** -- Merges an observable of observables.
@@ -289,15 +295,15 @@
         
             assert result == 4
             assert values == [2, 3, 4]
         ```
         
         # Fluent and chained programming style
         
-        An alternative to pipelining is to use classic and fluent method
+        An alternative to pipelining is to use the classic and fluent method
         chaining as we know from [ReactiveX](http://reactivex.io).
         
         An `AsyncObservable` created from class methods such as
         `AsyncRx.from_iterable()` returns a `AsyncChainedObservable`.
         where we may use methods such as `.filter()` and `.map()`.
         
         ```python
@@ -327,17 +333,17 @@
         ```
         
         # Virtual time testing
         
         Aioreactive also provides a virtual time event loop
         (`VirtualTimeEventLoop`) that enables you to write asyncio unit-tests
         that run in virtual time. Virtual time means that time is emulated, so
-        tests run as quickly as possible even if they sleep or awaits long lived
+        tests run as quickly as possible even if they sleep or awaits long-lived
         operations. A test using virtual time still gives the same result as it
-        would have done if it had been run in real time.
+        would have done if it had been run in real-time.
         
         For example the following test still gives the correct result even if it
         takes 0 seconds to run:
         
         ```python
         @pytest.yield_fixture()
         def event_loop():
@@ -356,15 +362,15 @@
             loop.call_later(10, partial(action, 1))
             loop.call_later(1, partial(action, 2))
             loop.call_later(5, partial(action, 3))
             await asyncio.sleep(10)
             assert result == [2, 3, 1]
         ```
         
-        The `aioreactive.testing` module provides a test `AsyncSubject` that may
+        The aioreactive testing module provides a test `AsyncSubject` that may
         delay sending values, and a test `AsyncTestObserver` that records all
         events. These two classes helps you with testing in virtual time.
         
         ```python
         @pytest.yield_fixture()
         def event_loop():
             loop = VirtualTimeEventLoop()
```

### Comparing `aioreactive-0.8.0/README.md` & `aioreactive-0.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -191,23 +191,29 @@
 apply them to an observable and compose it into a transformed, filtered,
 aggregated or combined observable. This transformed observable can be
 streamed into an observer.
 
     Observable -> Operator -> Operator -> Operator -> Observer
 
 Aioreactive contains many of the same operators as you know from RxPY.
-Our goal is not to implement them all, but to have the most essential
+Our goal is not to implement them all, but to provide the most essential
 ones.
 
 * **concat** -- Concatenates two or more observables.
+* **choose** -- Filters and/or transforms the observable.
+* **choose_asnc** -- Asynchronously filters and/or transforms the observable.
 * **debounce** -- Throttles an observable.
 * **delay** -- delays the items within an observable.
 * **distinct_until_changed** -- an observable with continuously distinct values.
 * **filter** -- filters an observable.
+* **filteri** -- filters an observable with index.
 * **flat_map** -- transforms an observable into a stream of observables and flattens the resulting observable.
+* **flat_map_latest** -- transforms an observable into a stream of
+  observables and flattens the resulting observable by producing values
+  from the latest observable.
 * **from_iterable** -- Create an observable from an (async) iterable.
 * **subscribe** -- Subscribes an observer to an observable. Returns a subscription.
 * **map** -- transforms an observable.
 * **mapi** -- transforms an observable with index.
 * **map_async** -- transforms an observable asynchronously.
 * **mapi_async** -- transforms an observable asynchronously with index.
 * **merge_inner** -- Merges an observable of observables.
@@ -280,15 +286,15 @@
 
     assert result == 4
     assert values == [2, 3, 4]
 ```
 
 # Fluent and chained programming style
 
-An alternative to pipelining is to use classic and fluent method
+An alternative to pipelining is to use the classic and fluent method
 chaining as we know from [ReactiveX](http://reactivex.io).
 
 An `AsyncObservable` created from class methods such as
 `AsyncRx.from_iterable()` returns a `AsyncChainedObservable`.
 where we may use methods such as `.filter()` and `.map()`.
 
 ```python
@@ -318,17 +324,17 @@
 ```
 
 # Virtual time testing
 
 Aioreactive also provides a virtual time event loop
 (`VirtualTimeEventLoop`) that enables you to write asyncio unit-tests
 that run in virtual time. Virtual time means that time is emulated, so
-tests run as quickly as possible even if they sleep or awaits long lived
+tests run as quickly as possible even if they sleep or awaits long-lived
 operations. A test using virtual time still gives the same result as it
-would have done if it had been run in real time.
+would have done if it had been run in real-time.
 
 For example the following test still gives the correct result even if it
 takes 0 seconds to run:
 
 ```python
 @pytest.yield_fixture()
 def event_loop():
@@ -347,15 +353,15 @@
     loop.call_later(10, partial(action, 1))
     loop.call_later(1, partial(action, 2))
     loop.call_later(5, partial(action, 3))
     await asyncio.sleep(10)
     assert result == [2, 3, 1]
 ```
 
-The `aioreactive.testing` module provides a test `AsyncSubject` that may
+The aioreactive testing module provides a test `AsyncSubject` that may
 delay sending values, and a test `AsyncTestObserver` that records all
 events. These two classes helps you with testing in virtual time.
 
 ```python
 @pytest.yield_fixture()
 def event_loop():
     loop = VirtualTimeEventLoop()
```

### Comparing `aioreactive-0.8.0/aioreactive/__init__.py` & `aioreactive-0.9.0/aioreactive/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,21 @@
-"""Aioreactive module"""
+"""Aioreactive module.
 
+Contains the AsyncRx chained obserable that allows method chaining of all operators.
+
+Also contains all operators as plain functions.
+
+To use this module:
+
+Example:
+    >>> import aioreactive as rx
+    >>> xs = rx.from_iterable([1, 2, 3])
+    >>> ...
+
+"""
 from typing import Any, AsyncIterable, Awaitable, Callable, Iterable, Tuple, TypeVar, Union
 
 from expression.core import Option, pipe
 from expression.system.disposable import AsyncDisposable
 
 from .observables import AsyncAnonymousObservable, AsyncIterableObservable, AsyncObservable
 from .observers import AsyncAnonymousObserver, AsyncAwaitableObserver, AsyncIteratorObserver, AsyncNotificationObserver
@@ -27,42 +39,56 @@
     All methods are lazy imported.
     """
 
     def __init__(self, source: AsyncObservable[TSource]) -> None:
         self._source = source
 
     async def subscribe_async(self, observer: AsyncObserver[TSource]) -> AsyncDisposable:
+        """Subscribe to the async observable.
+
+        Uses the given observer to subscribe asynchronously to the async
+        observable.
+
+        Args:
+            observer: The async observer to subscribe.
+
+        Returns:
+            An async disposable that can be used to dispose the
+            subscription.
+        """
         return await self._source.subscribe_async(observer)
 
     def __getitem__(self, key: Union[slice, int]) -> "AsyncRx[TSource]":
         """Slices the given source stream using Python slice notation.
-         The arguments to slice is start, stop and step given within
-         brackets [] and separated with the ':' character. It is
-         basically a wrapper around the operators skip(), skip_last(),
-         take(), take_last() and filter().
-
-         This marble diagram helps you remember how slices works with
-         streams. Positive numbers is relative to the start of the
-         events, while negative numbers are relative to the end
-         (on_completed) of the stream.
+        The arguments to slice is start, stop and step given within
+        brackets [] and separated with the ':' character. It is
+        basically a wrapper around the operators skip(), skip_last(),
+        take(), take_last() and filter().
+
+        This marble diagram helps you remember how slices works with
+        streams. Positive numbers is relative to the start of the
+        events, while negative numbers are relative to the end
+        (on_completed) of the stream.
 
          r---e---a---c---t---i---v---e---|
          0   1   2   3   4   5   6   7   8
         -8  -7  -6  -5  -4  -3  -2  -1
 
-         Example:
-         result = source[1:10]
-         result = source[1:-2]
-         result = source[1:-1:2]
-
-         Keyword arguments:
-         self -- Source to slice
-         key -- Slice object
+        Example:
+        >>> result = source[1:10]
+        >>> result = source[1:-2]
+        >>> result = source[1:-1:2]
 
-         Returne a sliced source stream."""
+        Args:
+            self: Source to slice
+            key: A slice object
+
+        Returns:
+            The sliced source stream.
+        """
 
         from .filtering import slice as _slice
 
         if isinstance(key, slice):
             start, stop, step = key.start, key.stop, key.step
         else:
             start, stop, step = key, key + 1, 1
@@ -76,33 +102,61 @@
         Helper method for creating an `AsyncChainedObservable` to the
         the generic type rightly inferred by Pylance (__init__ returns None).
         """
         return cls(source)
 
     @classmethod
     def empty(cls) -> "AsyncRx[TSource]":
-        from .create import empty
-
         return AsyncRx(empty())
 
     @classmethod
     def from_iterable(cls, iter: Iterable[TSource]) -> "AsyncRx[TSource]":
-        from .create import of_seq
-
-        return AsyncRx(of_seq(iter))
+        return AsyncRx(from_iterable(iter))
 
     @classmethod
     def single(cls, value: TSource) -> "AsyncRx[TSource]":
         from .create import single
 
         return AsyncRx(single(value))
 
     def as_async_observable(self) -> AsyncObservable[TSource]:
         return AsyncAnonymousObservable(self.subscribe_async)
 
+    def choose(self, chooser: Callable[[TSource], Option[TSource]]) -> AsyncObservable[TSource]:
+        """Choose.
+
+        Applies the given function to each element of the stream and returns
+        the stream comprised of the results for each element where the
+        function returns Some with some value.
+
+        Args:
+            chooser: A function to transform or filter the stream
+                by returning `Some(value)` or `Nothing`.
+
+        Returns:
+            The filtered and/or transformed stream.
+        """
+        return AsyncRx(pipe(self, choose(chooser)))
+
+    def choose_async(self, chooser: Callable[[TSource], Awaitable[Option[TSource]]]) -> AsyncObservable[TSource]:
+        """Choose async.
+
+        Applies the given async function to each element of the stream and
+        returns the stream comprised of the results for each element where
+        the function returns Some with some value.
+
+        Args:
+            chooser: A function to transform or filter the stream
+                asynchronously by returning `Some(value)` or `Nothing`.
+
+        Returns:
+            The filtered and transformed stream.
+        """
+        return AsyncRx(pipe(self, choose_async(chooser)))
+
     def combine_latest(self, other: TOther) -> "AsyncRx[Tuple[TSource, TOther]]":
         from .combine import combine_latest
 
         return AsyncRx.create(pipe(self, combine_latest(other)))
 
     def concat(self, other: AsyncObservable[TSource]) -> AsyncObservable[TSource]:
         from .combine import concat_seq
@@ -135,18 +189,48 @@
 
     def distinct_until_changed(self) -> AsyncObservable[TSource]:
         from .filtering import distinct_until_changed
 
         return AsyncRx(distinct_until_changed(self))
 
     def filter(self, predicate: Callable[[TSource], bool]) -> "AsyncRx[TSource]":
+        """Filter stream.
+
+        Filters the elements of an observable sequence based on a predicate.
+        Returns an observable sequence that contains elements from the input
+        sequence that satisfy the condition.
+
+        Args:
+            predicate:
+                A function to filter the stream by returning `True` to
+                keep the item, or `False` to filter and remove the item.
+
+        Returns:
+            The filtered stream.
+        """
+
         from .filtering import filter as _filter
 
         return AsyncRx(pipe(self, _filter(predicate)))
 
+    def filteri(self, predicate: Callable[[TSource, int], bool]) -> AsyncObservable[TSource]:
+        """Filter with index.
+
+        Filters the elements of an observable sequence based on a predicate
+        and incorporating the element's index on each element of the source.
+
+        Args:
+            predicate: Function to test each element.
+
+        Returns:
+            An observable sequence that contains elements from the input
+            sequence that satisfy the condition.
+        """
+        return AsyncRx(pipe(self, filteri(predicate)))
+
     def filter_async(self, predicate: Callable[[TSource], Awaitable[bool]]) -> "AsyncRx[TSource]":
         from .filtering import filter_async
 
         return AsyncRx(pipe(self, filter_async(predicate)))
 
     def flat_map(self, selector: Callable[[TSource], AsyncObservable[TResult]]) -> "AsyncRx[TResult]":
         from .transform import flat_map
@@ -154,14 +238,32 @@
         return pipe(self, flat_map(selector), AsyncRx.create)
 
     def flat_map_async(self, selector: Callable[[TSource], Awaitable[AsyncObservable[TResult]]]) -> "AsyncRx[TResult]":
         from .transform import flat_map_async
 
         return pipe(self, flat_map_async(selector), AsyncRx.create)
 
+    def flat_map_latest_async(
+        self, mapper: Callable[[TSource], Awaitable[AsyncObservable[TResult]]]
+    ) -> "AsyncRx[TResult]":
+        """Flat map latest async.
+
+        Asynchronosly transforms the items emitted by an source sequence
+        into observable streams, and mirror those items emitted by the
+        most-recently transformed observable sequence.
+
+        Args:
+            mapper (Callable[[TSource]): [description]
+            Awaitable ([type]): [description]
+
+        Returns:
+            Stream[TSource, TResult]: [description]
+        """
+        return AsyncRx(pipe(self, flat_map_latest_async(mapper)))
+
     def map(self, selector: Callable[[TSource], TResult]) -> "AsyncRx[TResult]":
         from .transform import map
 
         return AsyncRx(pipe(self, map(selector), AsyncRx.create))
 
     def merge(self, other: AsyncObservable[TSource]) -> "AsyncRx[TSource]":
         from .combine import merge_inner
@@ -178,37 +280,33 @@
 
         Args:
             count: Items to skip
 
         Returns:
             Stream[TSource, TSource]: [description]
         """
-        from .filtering import skip
-
         return AsyncRx(pipe(self, skip(count)))
 
     def starfilter(self, predicate: Callable[..., bool]) -> AsyncObservable[Tuple[TSource, int]]:
         """Filter and spread the arguments to the predicate.
 
         Filters the elements of an observable sequence based on a predicate.
         Returns:
             An observable sequence that contains elements from the input
             sequence that satisfy the condition.
         """
-        from .filtering import starfilter
-
         return AsyncRx.create(pipe(self, starfilter(predicate)))
 
     def starmap(self, mapper: Callable[..., TResult]) -> AsyncObservable[TResult]:
         """Map and spread the arguments to the mapper.
 
-        Returns an observable sequence whose elements are the result of
-        invoking the mapper function on each element of the source."""
-
-        from .transform import starmap
+        Returns:
+            An observable sequence whose elements are the result of
+            invoking the mapper function on each element of the source.
+        """
 
         return AsyncRx(pipe(self, starmap(mapper)))
 
     def take(self, count: int) -> AsyncObservable[TSource]:
         """Take the first elements from the stream.
 
         Returns a specified number of contiguous elements from the start of
@@ -272,20 +370,48 @@
 
 
 def as_chained(source: AsyncObservable[TSource]) -> AsyncRx[TSource]:
     return AsyncRx(source)
 
 
 def choose(chooser: Callable[[TSource], Option[TSource]]) -> Stream[TSource, TSource]:
+    """Choose.
+
+    Applies the given function to each element of the stream and returns
+    the stream comprised of the results for each element where the
+    function returns Some with some value.
+
+    Args:
+        chooser: A function to transform or filter the stream
+            by returning `Some(value)` or `Nothing`.
+
+    Returns:
+        The filtered and/or transformed stream.
+    """
+
     from .filtering import choose
 
     return choose(chooser)
 
 
 def choose_async(chooser: Callable[[TSource], Awaitable[Option[TSource]]]) -> Stream[TSource, TSource]:
+    """Choose async.
+
+    Applies the given async function to each element of the stream and
+    returns the stream comprised of the results for each element where
+    the function returns Some with some value.
+
+    Args:
+        chooser: An async function to transform or filter the stream
+            by returning `Some(value)` or `Nothing`.
+
+    Returns:
+        The filtered and/or transformed stream.
+    """
+
     from .filtering import choose_async
 
     return choose_async(chooser)
 
 
 def combine_latest(other: AsyncObservable[TOther]) -> Stream[TSource, Tuple[TSource, TOther]]:
     from .combine import combine_latest
@@ -296,21 +422,23 @@
 def debounce(seconds: float) -> Stream[TSource, TSource]:
     """Debounce source stream.
 
     Ignores values from a source stream which are followed by another
     value before seconds has elapsed.
 
     Example:
-    partial = debounce(5) # 5 seconds
+        >>> partial = debounce(5) # 5 seconds
 
-    Keyword arguments:
-    seconds -- Duration of the throttle period for each value
+    Args:
+        seconds: Duration of the throttle period for each value
 
-    Returns a partially applied function that takes a source stream to
-    debounce."""
+    Returns:
+        A partially applied debounce function that takes the source
+        observable to debounce.
+    """
 
     from .timeshift import debounce
 
     return debounce(seconds)
 
 
 def catch(handler: Callable[[Exception], AsyncObservable[TSource]]) -> Stream[TSource, TSource]:
@@ -362,20 +490,49 @@
 def empty() -> "AsyncObservable[TSource]":
     from .create import empty
 
     return empty()
 
 
 def filter(predicate: Callable[[TSource], bool]) -> Callable[[AsyncObservable[TSource]], AsyncObservable[TSource]]:
+    """Filter stream.
+
+    Filters the elements of an observable sequence based on a predicate.
+    Returns an observable sequence that contains elements from the input
+    sequence that satisfy the condition.
+
+    Args:
+        predicate:
+            A function to filter the stream by returning `True` to
+            keep the item, or `False` to filter and remove the item.
+
+    Returns:
+        The filtered stream.
+    """
     from .filtering import filter as _filter
 
     return _filter(predicate)
 
 
-print(filter)
+def filteri(predicate: Callable[[TSource, int], bool]) -> Stream[TSource, TSource]:
+    """Filter with index.
+
+    Filters the elements of an observable sequence based on a predicate
+    and incorporating the element's index on each element of the source.
+
+    Args:
+        predicate: Function to test each element.
+
+    Returns:
+        An observable sequence that contains elements from the input
+        sequence that satisfy the condition.
+    """
+    from .filtering import filteri
+
+    return filteri(predicate)
 
 
 def filter_async(
     predicate: Callable[[TSource], Awaitable[bool]]
 ) -> Callable[[AsyncObservable[TSource]], AsyncObservable[TSource]]:
     from .filtering import filter_async
 
@@ -387,18 +544,21 @@
 
     return of_async(worker)
 
 
 def from_iterable(iterable: Iterable[TSource]) -> AsyncObservable[TSource]:
     """Convert an iterable to a source stream.
 
-    1 - xs = from_iterable([1,2,3])
+    Example:
+        >>> xs = from_iterable([1,2,3])
 
-    Returns the source stream whose elements are pulled from the given
-    (async) iterable sequence."""
+    Returns:
+        The source stream whose elements are pulled from the given
+        (async) iterable sequence.
+    """
     from .create import of_seq
 
     return of_seq(iterable)
 
 
 def flat_map(mapper: Callable[[TSource], AsyncObservable[TResult]]) -> Stream[TSource, TResult]:
     from .transform import flat_map
@@ -428,14 +588,33 @@
         Stream[TSource, TResult]: [description]
     """
     from .transform import flat_map_async
 
     return flat_map_async(mapper)
 
 
+def flat_map_latest_async(mapper: Callable[[TSource], Awaitable[AsyncObservable[TResult]]]) -> Stream[TSource, TResult]:
+    """Flat map latest async.
+
+    Asynchronosly transforms the items emitted by an source sequence
+    into observable streams, and mirror those items emitted by the
+    most-recently transformed observable sequence.
+
+    Args:
+        mapper (Callable[[TSource]): [description]
+        Awaitable ([type]): [description]
+
+    Returns:
+        Stream[TSource, TResult]: [description]
+    """
+    from .transform import flat_map_latest_async
+
+    return flat_map_latest_async(mapper)
+
+
 def from_async_iterable(iter: Iterable[TSource]) -> "AsyncObservable[TSource]":
     from aioreactive.operators.from_async_iterable import from_async_iterable
 
     from .create import from_async_iterable
 
     return AsyncRx(from_async_iterable(iter))
 
@@ -549,15 +728,15 @@
     Bypasses a specified number of elements in an observable sequence
     and then returns the remaining elements.
 
     Args:
         count (int): Items to skip
 
     Returns:
-        Stream[TSource, TSource]: [description]
+        The result stream with skipped items.
     """
     from .filtering import skip
 
     return skip(count)
 
 
 def starfilter(predicate: Callable[..., bool]) -> Stream[TSource, Tuple[Any, ...]]:
@@ -639,15 +818,16 @@
     from .filtering import take_until
 
     return take_until(other)
 
 
 def timer(due_time: float) -> AsyncObservable[int]:
     """Returns an observable sequence that triggers the value 0
-    after the given duetime in milliseconds."""
+    after the given duetime in milliseconds.
+    """
     from .create import timer
 
     return timer(due_time)
 
 
 def to_async_iterable(source: AsyncObservable[TSource]) -> AsyncIterable[TSource]:
     from .leave import to_async_iterable
@@ -677,17 +857,23 @@
     "choose",
     "choose_async",
     "combine_latest",
     "concat",
     "concat_seq" "delay",
     "empty",
     "filter",
-    "filteri" "filter_async",
+    "filteri",
+    "filter_async",
     "from_async",
     "from_iterable",
+    "flat_map",
+    "flat_mapi",
+    "flat_map_async",
+    "flat_mapi_async",
+    "flat_map_latest_async",
     "map",
     "map_async",
     "merge",
     "merge_inner",
     "merge_seq",
     "never",
     "retry",
@@ -696,12 +882,14 @@
     "starfilter",
     "starmap",
     "Stream",
     "switch_latest",
     "to_async_iterable",
 ]
 
-# type: ignore
+
+# flake8: noqa
 from ._version import get_versions
 
-__version__ = get_versions()["version"]
+__version__ = get_versions()["version"]  # type: ignore
+
 del get_versions
```

### Comparing `aioreactive-0.8.0/aioreactive/combine.py` & `aioreactive-0.9.0/aioreactive/combine.py`

 * *Files identical despite different names*

### Comparing `aioreactive-0.8.0/aioreactive/create.py` & `aioreactive-0.9.0/aioreactive/create.py`

 * *Files identical despite different names*

### Comparing `aioreactive-0.8.0/aioreactive/filtering.py` & `aioreactive-0.9.0/aioreactive/filtering.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,49 +14,23 @@
 from .types import AsyncObservable, AsyncObserver, Stream
 
 TSource = TypeVar("TSource")
 TResult = TypeVar("TResult")
 
 
 def choose_async(chooser: Callable[[TSource], Awaitable[Option[TResult]]]) -> Stream[TSource, TResult]:
-    """Choose async.
-
-    Applies the given async function to each element of the stream and
-    returns the stream comprised of the results for each element where
-    the function returns Some with some value.
-
-    Args:
-        chooser (Callable[[TSource], Awaitable[Option[TResult]]]): [description]
-
-    Returns:
-        Stream[TSource, TResult]: [description]
-    """
-
     async def handler(next: Callable[[TResult], Awaitable[None]], xs: TSource) -> None:
         result = await chooser(xs)
         for x in result.to_list():
             await next(x)
 
     return transform(handler)
 
 
 def choose(chooser: Callable[[TSource], Option[TResult]]) -> Stream[TSource, TResult]:
-    """Choose.
-
-    Applies the given function to each element of the stream and returns
-    the stream comprised of the results for each element where the
-    function returns Some with some value.
-
-    Args:
-        chooser (Callable[[TSource], Option[TResult]]): [description]
-
-    Returns:
-        Stream[TSource, TResult]: [description]
-    """
-
     def handler(next: Callable[[TResult], Awaitable[None]], xs: TSource) -> Awaitable[None]:
         for x in chooser(xs).to_list():
             return next(x)
         return aiotools.empty()
 
     return transform(handler)
 
@@ -79,28 +53,14 @@
         if await predicate(x):
             return await next(x)
 
     return transform(handler)
 
 
 def filter(predicate: Callable[[TSource], bool]) -> Stream[TSource, TSource]:
-    """Filter stream.
-
-    Filters the elements of an observable sequence based on a predicate.
-    Returns an observable sequence that contains elements from the input
-    sequence that satisfy the condition.
-
-
-    Args:
-        predicate (Callable[[TSource], bool]): [description]
-
-    Returns:
-        Stream[TSource, TSource]: [description]
-    """
-
     def handler(next: Callable[[TSource], Awaitable[None]], x: TSource) -> Awaitable[None]:
         if predicate(x):
             return next(x)
         return aiotools.empty()
 
     return transform(handler)
 
@@ -124,27 +84,14 @@
             return next(args)
         return aiotools.empty()
 
     return transform(handler)
 
 
 def filteri(predicate: Callable[[TSource, int], bool]) -> Stream[TSource, TSource]:
-    """Filter with index.
-
-    Filters the elements of an observable sequence based on a predicate
-    and incorporating the element's index on each element of the source.
-
-    Args:
-        predicate: Function to test each element.
-
-    Returns:
-        An observable sequence that contains elements from the input
-        sequence that satisfy the condition.
-    """
-
     return compose(
         zip_seq(seq.infinite()),
         starfilter(predicate),
         map(fst),
     )
```

### Comparing `aioreactive-0.8.0/aioreactive/iterable/to_async_observable.py` & `aioreactive-0.9.0/aioreactive/iterable/to_async_observable.py`

 * *Files identical despite different names*

### Comparing `aioreactive-0.8.0/aioreactive/leave.py` & `aioreactive-0.9.0/aioreactive/leave.py`

 * *Files identical despite different names*

### Comparing `aioreactive-0.8.0/aioreactive/msg.py` & `aioreactive-0.9.0/aioreactive/msg.py`

 * *Files identical despite different names*

### Comparing `aioreactive-0.8.0/aioreactive/notification.py` & `aioreactive-0.9.0/aioreactive/notification.py`

 * *Files identical despite different names*

### Comparing `aioreactive-0.8.0/aioreactive/observables.py` & `aioreactive-0.9.0/aioreactive/observables.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,12 +40,15 @@
 
     def __aiter__(self) -> AsyncIterator[TSource]:
         """Iterate asynchronously.
 
         Transforms the async source to an async iterable. The source
         will await for the iterator to pick up the value before
         continuing to avoid queuing values.
+
+        Returns:
+            An async iterator.
         """
 
         obv: AsyncIteratorObserver[TSource] = AsyncIteratorObserver(self)
 
         return obv
```

### Comparing `aioreactive-0.8.0/aioreactive/observers.py` & `aioreactive-0.9.0/aioreactive/observers.py`

 * *Files identical despite different names*

### Comparing `aioreactive-0.8.0/aioreactive/subject.py` & `aioreactive-0.9.0/aioreactive/subject.py`

 * *Files identical despite different names*

### Comparing `aioreactive-0.8.0/aioreactive/subscription.py` & `aioreactive-0.9.0/aioreactive/subscription.py`

 * *Files identical despite different names*

### Comparing `aioreactive-0.8.0/aioreactive/testing/observer.py` & `aioreactive-0.9.0/aioreactive/testing/observer.py`

 * *Files identical despite different names*

### Comparing `aioreactive-0.8.0/aioreactive/testing/subject.py` & `aioreactive-0.9.0/aioreactive/testing/subject.py`

 * *Files identical despite different names*

### Comparing `aioreactive-0.8.0/aioreactive/testing/virtual_events.py` & `aioreactive-0.9.0/aioreactive/testing/virtual_events.py`

 * *Files identical despite different names*

### Comparing `aioreactive-0.8.0/aioreactive/timeshift.py` & `aioreactive-0.9.0/aioreactive/timeshift.py`

 * *Files identical despite different names*

### Comparing `aioreactive-0.8.0/aioreactive/transform.py` & `aioreactive-0.9.0/aioreactive/transform.py`

 * *Files identical despite different names*

### Comparing `aioreactive-0.8.0/aioreactive/types.py` & `aioreactive-0.9.0/aioreactive/types.py`

 * *Files identical despite different names*

### Comparing `aioreactive-0.8.0/aioreactive/utils.py` & `aioreactive-0.9.0/aioreactive/utils.py`

 * *Files identical despite different names*

### Comparing `aioreactive-0.8.0/aioreactive.egg-info/PKG-INFO` & `aioreactive-0.9.0/aioreactive.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioreactive
-Version: 0.8.0
+Version: 0.9.0
 Summary: Async/await Reactive Tools for Python 3.9+
 Home-page: https://github.com/dbrattli/aioreactive
 Author: Børge Lanes & Dag Brattli
 Author-email: dag@brattli.net
 License: MIT License
 Download-URL: https://github.com/dbrattli/aioreactive
 Description: 
@@ -200,23 +200,29 @@
         apply them to an observable and compose it into a transformed, filtered,
         aggregated or combined observable. This transformed observable can be
         streamed into an observer.
         
             Observable -> Operator -> Operator -> Operator -> Observer
         
         Aioreactive contains many of the same operators as you know from RxPY.
-        Our goal is not to implement them all, but to have the most essential
+        Our goal is not to implement them all, but to provide the most essential
         ones.
         
         * **concat** -- Concatenates two or more observables.
+        * **choose** -- Filters and/or transforms the observable.
+        * **choose_asnc** -- Asynchronously filters and/or transforms the observable.
         * **debounce** -- Throttles an observable.
         * **delay** -- delays the items within an observable.
         * **distinct_until_changed** -- an observable with continuously distinct values.
         * **filter** -- filters an observable.
+        * **filteri** -- filters an observable with index.
         * **flat_map** -- transforms an observable into a stream of observables and flattens the resulting observable.
+        * **flat_map_latest** -- transforms an observable into a stream of
+          observables and flattens the resulting observable by producing values
+          from the latest observable.
         * **from_iterable** -- Create an observable from an (async) iterable.
         * **subscribe** -- Subscribes an observer to an observable. Returns a subscription.
         * **map** -- transforms an observable.
         * **mapi** -- transforms an observable with index.
         * **map_async** -- transforms an observable asynchronously.
         * **mapi_async** -- transforms an observable asynchronously with index.
         * **merge_inner** -- Merges an observable of observables.
@@ -289,15 +295,15 @@
         
             assert result == 4
             assert values == [2, 3, 4]
         ```
         
         # Fluent and chained programming style
         
-        An alternative to pipelining is to use classic and fluent method
+        An alternative to pipelining is to use the classic and fluent method
         chaining as we know from [ReactiveX](http://reactivex.io).
         
         An `AsyncObservable` created from class methods such as
         `AsyncRx.from_iterable()` returns a `AsyncChainedObservable`.
         where we may use methods such as `.filter()` and `.map()`.
         
         ```python
@@ -327,17 +333,17 @@
         ```
         
         # Virtual time testing
         
         Aioreactive also provides a virtual time event loop
         (`VirtualTimeEventLoop`) that enables you to write asyncio unit-tests
         that run in virtual time. Virtual time means that time is emulated, so
-        tests run as quickly as possible even if they sleep or awaits long lived
+        tests run as quickly as possible even if they sleep or awaits long-lived
         operations. A test using virtual time still gives the same result as it
-        would have done if it had been run in real time.
+        would have done if it had been run in real-time.
         
         For example the following test still gives the correct result even if it
         takes 0 seconds to run:
         
         ```python
         @pytest.yield_fixture()
         def event_loop():
@@ -356,15 +362,15 @@
             loop.call_later(10, partial(action, 1))
             loop.call_later(1, partial(action, 2))
             loop.call_later(5, partial(action, 3))
             await asyncio.sleep(10)
             assert result == [2, 3, 1]
         ```
         
-        The `aioreactive.testing` module provides a test `AsyncSubject` that may
+        The aioreactive testing module provides a test `AsyncSubject` that may
         delay sending values, and a test `AsyncTestObserver` that records all
         events. These two classes helps you with testing in virtual time.
         
         ```python
         @pytest.yield_fixture()
         def event_loop():
             loop = VirtualTimeEventLoop()
```

### Comparing `aioreactive-0.8.0/aioreactive.egg-info/SOURCES.txt` & `aioreactive-0.9.0/aioreactive.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aioreactive-0.8.0/setup.py` & `aioreactive-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `aioreactive-0.8.0/test/test_async_iteration.py` & `aioreactive-0.9.0/test/test_async_iteration.py`

 * *Files identical despite different names*

### Comparing `aioreactive-0.8.0/test/test_chain.py` & `aioreactive-0.9.0/test/test_chain.py`

 * *Files identical despite different names*

### Comparing `aioreactive-0.8.0/test/test_concat.py` & `aioreactive-0.9.0/test/test_concat.py`

 * *Files identical despite different names*

### Comparing `aioreactive-0.8.0/test/test_debounce.py` & `aioreactive-0.9.0/test/test_debounce.py`

 * *Files identical despite different names*

### Comparing `aioreactive-0.8.0/test/test_delay.py` & `aioreactive-0.9.0/test/test_delay.py`

 * *Files identical despite different names*

### Comparing `aioreactive-0.8.0/test/test_distinct_until_changed.py` & `aioreactive-0.9.0/test/test_distinct_until_changed.py`

 * *Files identical despite different names*

### Comparing `aioreactive-0.8.0/test/test_eventloop.py` & `aioreactive-0.9.0/test/test_eventloop.py`

 * *Files identical despite different names*

### Comparing `aioreactive-0.8.0/test/test_filter.py` & `aioreactive-0.9.0/test/test_filter.py`

 * *Files identical despite different names*

### Comparing `aioreactive-0.8.0/test/test_flat_map.py` & `aioreactive-0.9.0/test/test_flat_map.py`

 * *Files identical despite different names*

### Comparing `aioreactive-0.8.0/test/test_forward_pipe.py` & `aioreactive-0.9.0/test/test_forward_pipe.py`

 * *Files identical despite different names*

### Comparing `aioreactive-0.8.0/test/test_from_iterable.py` & `aioreactive-0.9.0/test/test_from_iterable.py`

 * *Files identical despite different names*

### Comparing `aioreactive-0.8.0/test/test_map.py` & `aioreactive-0.9.0/test/test_map.py`

 * *Files identical despite different names*

### Comparing `aioreactive-0.8.0/test/test_merge.py` & `aioreactive-0.9.0/test/test_merge.py`

 * *Files identical despite different names*

### Comparing `aioreactive-0.8.0/test/test_pipe.py` & `aioreactive-0.9.0/test/test_pipe.py`

 * *Files identical despite different names*

### Comparing `aioreactive-0.8.0/test/test_single.py` & `aioreactive-0.9.0/test/test_single.py`

 * *Files identical despite different names*

### Comparing `aioreactive-0.8.0/test/test_single_stream.py` & `aioreactive-0.9.0/test/test_single_stream.py`

 * *Files identical despite different names*

### Comparing `aioreactive-0.8.0/test/test_slice.py` & `aioreactive-0.9.0/test/test_slice.py`

 * *Files identical despite different names*

### Comparing `aioreactive-0.8.0/test/test_stream.py` & `aioreactive-0.9.0/test/test_stream.py`

 * *Files identical despite different names*

### Comparing `aioreactive-0.8.0/test/test_take.py` & `aioreactive-0.9.0/test/test_take.py`

 * *Files identical despite different names*

### Comparing `aioreactive-0.8.0/test/test_with_latest_from.py` & `aioreactive-0.9.0/test/test_with_latest_from.py`

 * *Files identical despite different names*

### Comparing `aioreactive-0.8.0/versioneer.py` & `aioreactive-0.9.0/versioneer.py`

 * *Files identical despite different names*

