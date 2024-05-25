# Comparing `tmp/botocore-a-la-carte-ec2-1.34.98.tar.gz` & `tmp/botocore-a-la-carte-ec2-1.34.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-ec2-1.34.98.tar", last modified: Sat May  4 01:01:30 2024, max compression
+gzip compressed data, was "botocore-a-la-carte-ec2-1.34.99.tar", last modified: Tue May  7 01:02:32 2024, max compression
```

## Comparing `botocore-a-la-carte-ec2-1.34.98.tar` & `botocore-a-la-carte-ec2-1.34.99.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:30.110169 botocore-a-la-carte-ec2-1.34.98/
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-05-04 01:01:29.000000 botocore-a-la-carte-ec2-1.34.98/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-04 01:01:30.110169 botocore-a-la-carte-ec2-1.34.98/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:30.086169 botocore-a-la-carte-ec2-1.34.98/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:30.086169 botocore-a-la-carte-ec2-1.34.98/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:30.086169 botocore-a-la-carte-ec2-1.34.98/botocore/data/ec2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:30.090169 botocore-a-la-carte-ec2-1.34.98/botocore/data/ec2/2014-09-01/
--rw-r--r--   0 runner    (1001) docker     (127)    14695 2024-05-04 01:01:11.000000 botocore-a-la-carte-ec2-1.34.98/botocore/data/ec2/2014-09-01/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-04 01:01:11.000000 botocore-a-la-carte-ec2-1.34.98/botocore/data/ec2/2014-09-01/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (127)   539923 2024-05-04 01:01:11.000000 botocore-a-la-carte-ec2-1.34.98/botocore/data/ec2/2014-09-01/service-2.json
--rw-r--r--   0 runner    (1001) docker     (127)     8548 2024-05-04 01:01:11.000000 botocore-a-la-carte-ec2-1.34.98/botocore/data/ec2/2014-09-01/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:30.090169 botocore-a-la-carte-ec2-1.34.98/botocore/data/ec2/2014-10-01/
--rw-r--r--   0 runner    (1001) docker     (127)    14695 2024-05-04 01:01:11.000000 botocore-a-la-carte-ec2-1.34.98/botocore/data/ec2/2014-10-01/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-05-04 01:01:11.000000 botocore-a-la-carte-ec2-1.34.98/botocore/data/ec2/2014-10-01/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (127)   566499 2024-05-04 01:01:11.000000 botocore-a-la-carte-ec2-1.34.98/botocore/data/ec2/2014-10-01/service-2.json
--rw-r--r--   0 runner    (1001) docker     (127)    11040 2024-05-04 01:01:11.000000 botocore-a-la-carte-ec2-1.34.98/botocore/data/ec2/2014-10-01/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:30.090169 botocore-a-la-carte-ec2-1.34.98/botocore/data/ec2/2015-03-01/
--rw-r--r--   0 runner    (1001) docker     (127)    14695 2024-05-04 01:01:11.000000 botocore-a-la-carte-ec2-1.34.98/botocore/data/ec2/2015-03-01/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-05-04 01:01:11.000000 botocore-a-la-carte-ec2-1.34.98/botocore/data/ec2/2015-03-01/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (127)   588390 2024-05-04 01:01:11.000000 botocore-a-la-carte-ec2-1.34.98/botocore/data/ec2/2015-03-01/service-2.json
--rw-r--r--   0 runner    (1001) docker     (127)    11040 2024-05-04 01:01:11.000000 botocore-a-la-carte-ec2-1.34.98/botocore/data/ec2/2015-03-01/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:30.094169 botocore-a-la-carte-ec2-1.34.98/botocore/data/ec2/2015-04-15/
--rw-r--r--   0 runner    (1001) docker     (127)    14695 2024-05-04 01:01:11.000000 botocore-a-la-carte-ec2-1.34.98/botocore/data/ec2/2015-04-15/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-05-04 01:01:11.000000 botocore-a-la-carte-ec2-1.34.98/botocore/data/ec2/2015-04-15/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (127)   715324 2024-05-04 01:01:11.000000 botocore-a-la-carte-ec2-1.34.98/botocore/data/ec2/2015-04-15/service-2.json
--rw-r--r--   0 runner    (1001) docker     (127)    11546 2024-05-04 01:01:11.000000 botocore-a-la-carte-ec2-1.34.98/botocore/data/ec2/2015-04-15/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:30.094169 botocore-a-la-carte-ec2-1.34.98/botocore/data/ec2/2015-10-01/
--rw-r--r--   0 runner    (1001) docker     (127)    19575 2024-05-04 01:01:11.000000 botocore-a-la-carte-ec2-1.34.98/botocore/data/ec2/2015-10-01/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-04 01:01:11.000000 botocore-a-la-carte-ec2-1.34.98/botocore/data/ec2/2015-10-01/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-04 01:01:11.000000 botocore-a-la-carte-ec2-1.34.98/botocore/data/ec2/2015-10-01/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (127)   847080 2024-05-04 01:01:11.000000 botocore-a-la-carte-ec2-1.34.98/botocore/data/ec2/2015-10-01/service-2.json
--rw-r--r--   0 runner    (1001) docker     (127)    14823 2024-05-04 01:01:11.000000 botocore-a-la-carte-ec2-1.34.98/botocore/data/ec2/2015-10-01/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:30.098169 botocore-a-la-carte-ec2-1.34.98/botocore/data/ec2/2016-04-01/
--rw-r--r--   0 runner    (1001) docker     (127)    19575 2024-05-04 01:01:11.000000 botocore-a-la-carte-ec2-1.34.98/botocore/data/ec2/2016-04-01/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)   109914 2024-05-04 01:01:11.000000 botocore-a-la-carte-ec2-1.34.98/botocore/data/ec2/2016-04-01/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-04 01:01:11.000000 botocore-a-la-carte-ec2-1.34.98/botocore/data/ec2/2016-04-01/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (127)   878250 2024-05-04 01:01:11.000000 botocore-a-la-carte-ec2-1.34.98/botocore/data/ec2/2016-04-01/service-2.json
--rw-r--r--   0 runner    (1001) docker     (127)    15259 2024-05-04 01:01:11.000000 botocore-a-la-carte-ec2-1.34.98/botocore/data/ec2/2016-04-01/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:30.102169 botocore-a-la-carte-ec2-1.34.98/botocore/data/ec2/2016-09-15/
--rw-r--r--   0 runner    (1001) docker     (127)    19575 2024-05-04 01:01:11.000000 botocore-a-la-carte-ec2-1.34.98/botocore/data/ec2/2016-09-15/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)   110174 2024-05-04 01:01:11.000000 botocore-a-la-carte-ec2-1.34.98/botocore/data/ec2/2016-09-15/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-04 01:01:11.000000 botocore-a-la-carte-ec2-1.34.98/botocore/data/ec2/2016-09-15/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (127)   891280 2024-05-04 01:01:11.000000 botocore-a-la-carte-ec2-1.34.98/botocore/data/ec2/2016-09-15/service-2.json
--rw-r--r--   0 runner    (1001) docker     (127)    14875 2024-05-04 01:01:11.000000 botocore-a-la-carte-ec2-1.34.98/botocore/data/ec2/2016-09-15/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:30.106169 botocore-a-la-carte-ec2-1.34.98/botocore/data/ec2/2016-11-15/
--rw-r--r--   0 runner    (1001) docker     (127)    15277 2024-05-04 01:01:11.000000 botocore-a-la-carte-ec2-1.34.98/botocore/data/ec2/2016-11-15/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)   147949 2024-05-04 01:01:11.000000 botocore-a-la-carte-ec2-1.34.98/botocore/data/ec2/2016-11-15/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (127)    26822 2024-05-04 01:01:11.000000 botocore-a-la-carte-ec2-1.34.98/botocore/data/ec2/2016-11-15/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-04 01:01:11.000000 botocore-a-la-carte-ec2-1.34.98/botocore/data/ec2/2016-11-15/paginators-1.sdk-extras.json
--rw-r--r--   0 runner    (1001) docker     (127)  3056651 2024-05-04 01:01:11.000000 botocore-a-la-carte-ec2-1.34.98/botocore/data/ec2/2016-11-15/service-2.json
--rw-r--r--   0 runner    (1001) docker     (127)    18443 2024-05-04 01:01:11.000000 botocore-a-la-carte-ec2-1.34.98/botocore/data/ec2/2016-11-15/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:30.110169 botocore-a-la-carte-ec2-1.34.98/botocore_a_la_carte_ec2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-04 01:01:30.000000 botocore-a-la-carte-ec2-1.34.98/botocore_a_la_carte_ec2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-04 01:01:30.000000 botocore-a-la-carte-ec2-1.34.98/botocore_a_la_carte_ec2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 01:01:30.000000 botocore-a-la-carte-ec2-1.34.98/botocore_a_la_carte_ec2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-04 01:01:30.000000 botocore-a-la-carte-ec2-1.34.98/botocore_a_la_carte_ec2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 01:01:30.110169 botocore-a-la-carte-ec2-1.34.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-04 01:01:29.000000 botocore-a-la-carte-ec2-1.34.98/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:32.116095 botocore-a-la-carte-ec2-1.34.99/
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-05-07 01:02:31.000000 botocore-a-la-carte-ec2-1.34.99/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-07 01:02:32.116095 botocore-a-la-carte-ec2-1.34.99/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:32.096095 botocore-a-la-carte-ec2-1.34.99/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:32.096095 botocore-a-la-carte-ec2-1.34.99/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:32.096095 botocore-a-la-carte-ec2-1.34.99/botocore/data/ec2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:32.096095 botocore-a-la-carte-ec2-1.34.99/botocore/data/ec2/2014-09-01/
+-rw-r--r--   0 runner    (1001) docker     (127)    14695 2024-05-07 01:02:10.000000 botocore-a-la-carte-ec2-1.34.99/botocore/data/ec2/2014-09-01/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-07 01:02:10.000000 botocore-a-la-carte-ec2-1.34.99/botocore/data/ec2/2014-09-01/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)   539923 2024-05-07 01:02:10.000000 botocore-a-la-carte-ec2-1.34.99/botocore/data/ec2/2014-09-01/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8548 2024-05-07 01:02:10.000000 botocore-a-la-carte-ec2-1.34.99/botocore/data/ec2/2014-09-01/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:32.100096 botocore-a-la-carte-ec2-1.34.99/botocore/data/ec2/2014-10-01/
+-rw-r--r--   0 runner    (1001) docker     (127)    14695 2024-05-07 01:02:10.000000 botocore-a-la-carte-ec2-1.34.99/botocore/data/ec2/2014-10-01/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-05-07 01:02:10.000000 botocore-a-la-carte-ec2-1.34.99/botocore/data/ec2/2014-10-01/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)   566499 2024-05-07 01:02:10.000000 botocore-a-la-carte-ec2-1.34.99/botocore/data/ec2/2014-10-01/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11040 2024-05-07 01:02:10.000000 botocore-a-la-carte-ec2-1.34.99/botocore/data/ec2/2014-10-01/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:32.100096 botocore-a-la-carte-ec2-1.34.99/botocore/data/ec2/2015-03-01/
+-rw-r--r--   0 runner    (1001) docker     (127)    14695 2024-05-07 01:02:10.000000 botocore-a-la-carte-ec2-1.34.99/botocore/data/ec2/2015-03-01/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-05-07 01:02:10.000000 botocore-a-la-carte-ec2-1.34.99/botocore/data/ec2/2015-03-01/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)   588390 2024-05-07 01:02:10.000000 botocore-a-la-carte-ec2-1.34.99/botocore/data/ec2/2015-03-01/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11040 2024-05-07 01:02:10.000000 botocore-a-la-carte-ec2-1.34.99/botocore/data/ec2/2015-03-01/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:32.104096 botocore-a-la-carte-ec2-1.34.99/botocore/data/ec2/2015-04-15/
+-rw-r--r--   0 runner    (1001) docker     (127)    14695 2024-05-07 01:02:10.000000 botocore-a-la-carte-ec2-1.34.99/botocore/data/ec2/2015-04-15/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-05-07 01:02:10.000000 botocore-a-la-carte-ec2-1.34.99/botocore/data/ec2/2015-04-15/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)   715324 2024-05-07 01:02:10.000000 botocore-a-la-carte-ec2-1.34.99/botocore/data/ec2/2015-04-15/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11546 2024-05-07 01:02:10.000000 botocore-a-la-carte-ec2-1.34.99/botocore/data/ec2/2015-04-15/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:32.104096 botocore-a-la-carte-ec2-1.34.99/botocore/data/ec2/2015-10-01/
+-rw-r--r--   0 runner    (1001) docker     (127)    19575 2024-05-07 01:02:10.000000 botocore-a-la-carte-ec2-1.34.99/botocore/data/ec2/2015-10-01/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-07 01:02:10.000000 botocore-a-la-carte-ec2-1.34.99/botocore/data/ec2/2015-10-01/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-07 01:02:10.000000 botocore-a-la-carte-ec2-1.34.99/botocore/data/ec2/2015-10-01/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)   847080 2024-05-07 01:02:10.000000 botocore-a-la-carte-ec2-1.34.99/botocore/data/ec2/2015-10-01/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14823 2024-05-07 01:02:10.000000 botocore-a-la-carte-ec2-1.34.99/botocore/data/ec2/2015-10-01/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:32.108096 botocore-a-la-carte-ec2-1.34.99/botocore/data/ec2/2016-04-01/
+-rw-r--r--   0 runner    (1001) docker     (127)    19575 2024-05-07 01:02:10.000000 botocore-a-la-carte-ec2-1.34.99/botocore/data/ec2/2016-04-01/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)   109914 2024-05-07 01:02:10.000000 botocore-a-la-carte-ec2-1.34.99/botocore/data/ec2/2016-04-01/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-07 01:02:10.000000 botocore-a-la-carte-ec2-1.34.99/botocore/data/ec2/2016-04-01/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)   878250 2024-05-07 01:02:10.000000 botocore-a-la-carte-ec2-1.34.99/botocore/data/ec2/2016-04-01/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15259 2024-05-07 01:02:10.000000 botocore-a-la-carte-ec2-1.34.99/botocore/data/ec2/2016-04-01/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:32.108096 botocore-a-la-carte-ec2-1.34.99/botocore/data/ec2/2016-09-15/
+-rw-r--r--   0 runner    (1001) docker     (127)    19575 2024-05-07 01:02:10.000000 botocore-a-la-carte-ec2-1.34.99/botocore/data/ec2/2016-09-15/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)   110174 2024-05-07 01:02:10.000000 botocore-a-la-carte-ec2-1.34.99/botocore/data/ec2/2016-09-15/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-07 01:02:10.000000 botocore-a-la-carte-ec2-1.34.99/botocore/data/ec2/2016-09-15/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)   891280 2024-05-07 01:02:10.000000 botocore-a-la-carte-ec2-1.34.99/botocore/data/ec2/2016-09-15/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14875 2024-05-07 01:02:10.000000 botocore-a-la-carte-ec2-1.34.99/botocore/data/ec2/2016-09-15/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:32.116095 botocore-a-la-carte-ec2-1.34.99/botocore/data/ec2/2016-11-15/
+-rw-r--r--   0 runner    (1001) docker     (127)    15277 2024-05-07 01:02:10.000000 botocore-a-la-carte-ec2-1.34.99/botocore/data/ec2/2016-11-15/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)   147949 2024-05-07 01:02:10.000000 botocore-a-la-carte-ec2-1.34.99/botocore/data/ec2/2016-11-15/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    26822 2024-05-07 01:02:10.000000 botocore-a-la-carte-ec2-1.34.99/botocore/data/ec2/2016-11-15/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-07 01:02:10.000000 botocore-a-la-carte-ec2-1.34.99/botocore/data/ec2/2016-11-15/paginators-1.sdk-extras.json
+-rw-r--r--   0 runner    (1001) docker     (127)  3056651 2024-05-07 01:02:10.000000 botocore-a-la-carte-ec2-1.34.99/botocore/data/ec2/2016-11-15/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)    18443 2024-05-07 01:02:10.000000 botocore-a-la-carte-ec2-1.34.99/botocore/data/ec2/2016-11-15/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:32.116095 botocore-a-la-carte-ec2-1.34.99/botocore_a_la_carte_ec2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-07 01:02:32.000000 botocore-a-la-carte-ec2-1.34.99/botocore_a_la_carte_ec2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-07 01:02:32.000000 botocore-a-la-carte-ec2-1.34.99/botocore_a_la_carte_ec2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 01:02:32.000000 botocore-a-la-carte-ec2-1.34.99/botocore_a_la_carte_ec2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-07 01:02:32.000000 botocore-a-la-carte-ec2-1.34.99/botocore_a_la_carte_ec2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 01:02:32.116095 botocore-a-la-carte-ec2-1.34.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-07 01:02:31.000000 botocore-a-la-carte-ec2-1.34.99/setup.py
```

### Comparing `botocore-a-la-carte-ec2-1.34.98/LICENSE.txt` & `botocore-a-la-carte-ec2-1.34.99/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.34.98/PKG-INFO` & `botocore-a-la-carte-ec2-1.34.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-ec2
-Version: 1.34.98
+Version: 1.34.99
 Summary: ec2 data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-ec2-1.34.98/botocore/data/ec2/2014-09-01/endpoint-rule-set-1.json` & `botocore-a-la-carte-ec2-1.34.99/botocore/data/ec2/2014-09-01/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.34.98/botocore/data/ec2/2014-09-01/paginators-1.json` & `botocore-a-la-carte-ec2-1.34.99/botocore/data/ec2/2014-09-01/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.34.98/botocore/data/ec2/2014-09-01/service-2.json` & `botocore-a-la-carte-ec2-1.34.99/botocore/data/ec2/2014-09-01/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.34.98/botocore/data/ec2/2014-09-01/waiters-2.json` & `botocore-a-la-carte-ec2-1.34.99/botocore/data/ec2/2014-09-01/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.34.98/botocore/data/ec2/2014-10-01/endpoint-rule-set-1.json` & `botocore-a-la-carte-ec2-1.34.99/botocore/data/ec2/2014-10-01/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.34.98/botocore/data/ec2/2014-10-01/paginators-1.json` & `botocore-a-la-carte-ec2-1.34.99/botocore/data/ec2/2014-10-01/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.34.98/botocore/data/ec2/2014-10-01/service-2.json` & `botocore-a-la-carte-ec2-1.34.99/botocore/data/ec2/2014-10-01/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.34.98/botocore/data/ec2/2014-10-01/waiters-2.json` & `botocore-a-la-carte-ec2-1.34.99/botocore/data/ec2/2014-10-01/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.34.98/botocore/data/ec2/2015-03-01/endpoint-rule-set-1.json` & `botocore-a-la-carte-ec2-1.34.99/botocore/data/ec2/2015-03-01/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.34.98/botocore/data/ec2/2015-03-01/paginators-1.json` & `botocore-a-la-carte-ec2-1.34.99/botocore/data/ec2/2015-03-01/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.34.98/botocore/data/ec2/2015-03-01/service-2.json` & `botocore-a-la-carte-ec2-1.34.99/botocore/data/ec2/2015-03-01/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.34.98/botocore/data/ec2/2015-03-01/waiters-2.json` & `botocore-a-la-carte-ec2-1.34.99/botocore/data/ec2/2015-03-01/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.34.98/botocore/data/ec2/2015-04-15/endpoint-rule-set-1.json` & `botocore-a-la-carte-ec2-1.34.99/botocore/data/ec2/2015-04-15/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.34.98/botocore/data/ec2/2015-04-15/paginators-1.json` & `botocore-a-la-carte-ec2-1.34.99/botocore/data/ec2/2015-04-15/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.34.98/botocore/data/ec2/2015-04-15/service-2.json` & `botocore-a-la-carte-ec2-1.34.99/botocore/data/ec2/2015-04-15/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.34.98/botocore/data/ec2/2015-04-15/waiters-2.json` & `botocore-a-la-carte-ec2-1.34.99/botocore/data/ec2/2015-04-15/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.34.98/botocore/data/ec2/2015-10-01/endpoint-rule-set-1.json` & `botocore-a-la-carte-ec2-1.34.99/botocore/data/ec2/2015-10-01/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.34.98/botocore/data/ec2/2015-10-01/paginators-1.json` & `botocore-a-la-carte-ec2-1.34.99/botocore/data/ec2/2015-10-01/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.34.98/botocore/data/ec2/2015-10-01/service-2.json` & `botocore-a-la-carte-ec2-1.34.99/botocore/data/ec2/2015-10-01/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.34.98/botocore/data/ec2/2015-10-01/waiters-2.json` & `botocore-a-la-carte-ec2-1.34.99/botocore/data/ec2/2015-10-01/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.34.98/botocore/data/ec2/2016-04-01/endpoint-rule-set-1.json` & `botocore-a-la-carte-ec2-1.34.99/botocore/data/ec2/2016-04-01/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.34.98/botocore/data/ec2/2016-04-01/examples-1.json` & `botocore-a-la-carte-ec2-1.34.99/botocore/data/ec2/2016-04-01/examples-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.34.98/botocore/data/ec2/2016-04-01/paginators-1.json` & `botocore-a-la-carte-ec2-1.34.99/botocore/data/ec2/2016-04-01/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.34.98/botocore/data/ec2/2016-04-01/service-2.json` & `botocore-a-la-carte-ec2-1.34.99/botocore/data/ec2/2016-04-01/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.34.98/botocore/data/ec2/2016-04-01/waiters-2.json` & `botocore-a-la-carte-ec2-1.34.99/botocore/data/ec2/2016-04-01/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.34.98/botocore/data/ec2/2016-09-15/endpoint-rule-set-1.json` & `botocore-a-la-carte-ec2-1.34.99/botocore/data/ec2/2016-09-15/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.34.98/botocore/data/ec2/2016-09-15/examples-1.json` & `botocore-a-la-carte-ec2-1.34.99/botocore/data/ec2/2016-09-15/examples-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.34.98/botocore/data/ec2/2016-09-15/paginators-1.json` & `botocore-a-la-carte-ec2-1.34.99/botocore/data/ec2/2016-09-15/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.34.98/botocore/data/ec2/2016-09-15/service-2.json` & `botocore-a-la-carte-ec2-1.34.99/botocore/data/ec2/2016-09-15/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.34.98/botocore/data/ec2/2016-09-15/waiters-2.json` & `botocore-a-la-carte-ec2-1.34.99/botocore/data/ec2/2016-09-15/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.34.98/botocore/data/ec2/2016-11-15/endpoint-rule-set-1.json` & `botocore-a-la-carte-ec2-1.34.99/botocore/data/ec2/2016-11-15/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.34.98/botocore/data/ec2/2016-11-15/examples-1.json` & `botocore-a-la-carte-ec2-1.34.99/botocore/data/ec2/2016-11-15/examples-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.34.98/botocore/data/ec2/2016-11-15/paginators-1.json` & `botocore-a-la-carte-ec2-1.34.99/botocore/data/ec2/2016-11-15/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.34.98/botocore/data/ec2/2016-11-15/service-2.json` & `botocore-a-la-carte-ec2-1.34.99/botocore/data/ec2/2016-11-15/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.34.98/botocore/data/ec2/2016-11-15/waiters-2.json` & `botocore-a-la-carte-ec2-1.34.99/botocore/data/ec2/2016-11-15/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.34.98/botocore_a_la_carte_ec2.egg-info/PKG-INFO` & `botocore-a-la-carte-ec2-1.34.99/botocore_a_la_carte_ec2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-ec2
-Version: 1.34.98
+Version: 1.34.99
 Summary: ec2 data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-ec2-1.34.98/botocore_a_la_carte_ec2.egg-info/SOURCES.txt` & `botocore-a-la-carte-ec2-1.34.99/botocore_a_la_carte_ec2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.34.98/setup.py` & `botocore-a-la-carte-ec2-1.34.99/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-ec2',
-    version="1.34.98",
+    version="1.34.99",
     description='ec2 data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/ec2/*/*.json'],
```

