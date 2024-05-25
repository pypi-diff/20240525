# Comparing `tmp/botocore-a-la-carte-cloudfront-1.34.98.tar.gz` & `tmp/botocore-a-la-carte-cloudfront-1.34.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-cloudfront-1.34.98.tar", last modified: Sat May  4 01:01:17 2024, max compression
+gzip compressed data, was "botocore-a-la-carte-cloudfront-1.34.99.tar", last modified: Tue May  7 01:02:19 2024, max compression
```

## Comparing `botocore-a-la-carte-cloudfront-1.34.98.tar` & `botocore-a-la-carte-cloudfront-1.34.99.tar`

### file list

```diff
@@ -1,118 +1,118 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:17.802063 botocore-a-la-carte-cloudfront-1.34.98/
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-05-04 01:01:17.000000 botocore-a-la-carte-cloudfront-1.34.98/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-04 01:01:17.802063 botocore-a-la-carte-cloudfront-1.34.98/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:17.778063 botocore-a-la-carte-cloudfront-1.34.98/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:17.778063 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:17.782063 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:17.782063 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2014-05-31/
--rw-r--r--   0 runner    (1001) docker     (127)    40823 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2014-05-31/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2014-05-31/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (127)   144492 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2014-05-31/service-2.json
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2014-05-31/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:17.782063 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2014-10-21/
--rw-r--r--   0 runner    (1001) docker     (127)    40823 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2014-10-21/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2014-10-21/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (127)   147479 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2014-10-21/service-2.json
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2014-10-21/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:17.782063 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2014-11-06/
--rw-r--r--   0 runner    (1001) docker     (127)    40823 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2014-11-06/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2014-11-06/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (127)   147700 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2014-11-06/service-2.json
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2014-11-06/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:17.786063 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2015-04-17/
--rw-r--r--   0 runner    (1001) docker     (127)    40823 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2015-04-17/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2015-04-17/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (127)   150842 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2015-04-17/service-2.json
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2015-04-17/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:17.786063 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2015-07-27/
--rw-r--r--   0 runner    (1001) docker     (127)    40823 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2015-07-27/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2015-07-27/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (127)   154636 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2015-07-27/service-2.json
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2015-07-27/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:17.786063 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2015-09-17/
--rw-r--r--   0 runner    (1001) docker     (127)    40823 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2015-09-17/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2015-09-17/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (127)   130784 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2015-09-17/service-2.json
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2015-09-17/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:17.786063 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2016-01-13/
--rw-r--r--   0 runner    (1001) docker     (127)    40823 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2016-01-13/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2016-01-13/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (127)   133880 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2016-01-13/service-2.json
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2016-01-13/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:17.790063 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2016-01-28/
--rw-r--r--   0 runner    (1001) docker     (127)    26040 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2016-01-28/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2016-01-28/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2016-01-28/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (127)   133424 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2016-01-28/service-2.json
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2016-01-28/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:17.790063 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2016-08-01/
--rw-r--r--   0 runner    (1001) docker     (127)    26040 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2016-08-01/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2016-08-01/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2016-08-01/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (127)   148384 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2016-08-01/service-2.json
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2016-08-01/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:17.790063 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2016-08-20/
--rw-r--r--   0 runner    (1001) docker     (127)    26040 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2016-08-20/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2016-08-20/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (127)   150982 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2016-08-20/service-2.json
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2016-08-20/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:17.790063 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2016-09-07/
--rw-r--r--   0 runner    (1001) docker     (127)    26040 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2016-09-07/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2016-09-07/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2016-09-07/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (127)   151766 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2016-09-07/service-2.json
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2016-09-07/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:17.790063 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2016-09-29/
--rw-r--r--   0 runner    (1001) docker     (127)    26040 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2016-09-29/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2016-09-29/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2016-09-29/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (127)   194806 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2016-09-29/service-2.json
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2016-09-29/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:17.794063 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2016-11-25/
--rw-r--r--   0 runner    (1001) docker     (127)    26040 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2016-11-25/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2016-11-25/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2016-11-25/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (127)   197970 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2016-11-25/service-2.json
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2016-11-25/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:17.794063 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2017-03-25/
--rw-r--r--   0 runner    (1001) docker     (127)    26040 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2017-03-25/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2017-03-25/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (127)   206093 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2017-03-25/service-2.json
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2017-03-25/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:17.794063 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2017-10-30/
--rw-r--r--   0 runner    (1001) docker     (127)    26040 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2017-10-30/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2017-10-30/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2017-10-30/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (127)   264716 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2017-10-30/service-2.json
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2017-10-30/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:17.794063 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2018-06-18/
--rw-r--r--   0 runner    (1001) docker     (127)    26040 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2018-06-18/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2018-06-18/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2018-06-18/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (127)   267331 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2018-06-18/service-2.json
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2018-06-18/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:17.798063 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2018-11-05/
--rw-r--r--   0 runner    (1001) docker     (127)    26040 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2018-11-05/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2018-11-05/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2018-11-05/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (127)   273141 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2018-11-05/service-2.json
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2018-11-05/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:17.798063 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2019-03-26/
--rw-r--r--   0 runner    (1001) docker     (127)    26040 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2019-03-26/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2019-03-26/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2019-03-26/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (127)   281937 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2019-03-26/service-2.json
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2019-03-26/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:17.798063 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2020-05-31/
--rw-r--r--   0 runner    (1001) docker     (127)    20918 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2020-05-31/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2020-05-31/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2020-05-31/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (127)   590197 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2020-05-31/service-2.json
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-04 01:01:11.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2020-05-31/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:17.802063 botocore-a-la-carte-cloudfront-1.34.98/botocore_a_la_carte_cloudfront.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-04 01:01:17.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore_a_la_carte_cloudfront.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4879 2024-05-04 01:01:17.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore_a_la_carte_cloudfront.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 01:01:17.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore_a_la_carte_cloudfront.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-04 01:01:17.000000 botocore-a-la-carte-cloudfront-1.34.98/botocore_a_la_carte_cloudfront.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 01:01:17.802063 botocore-a-la-carte-cloudfront-1.34.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-04 01:01:17.000000 botocore-a-la-carte-cloudfront-1.34.98/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:19.916097 botocore-a-la-carte-cloudfront-1.34.99/
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-05-07 01:02:19.000000 botocore-a-la-carte-cloudfront-1.34.99/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-07 01:02:19.916097 botocore-a-la-carte-cloudfront-1.34.99/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:19.892096 botocore-a-la-carte-cloudfront-1.34.99/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:19.892096 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:19.892096 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:19.896097 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2014-05-31/
+-rw-r--r--   0 runner    (1001) docker     (127)    40823 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2014-05-31/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2014-05-31/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)   144492 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2014-05-31/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2014-05-31/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:19.896097 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2014-10-21/
+-rw-r--r--   0 runner    (1001) docker     (127)    40823 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2014-10-21/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2014-10-21/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)   147479 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2014-10-21/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2014-10-21/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:19.896097 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2014-11-06/
+-rw-r--r--   0 runner    (1001) docker     (127)    40823 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2014-11-06/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2014-11-06/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)   147700 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2014-11-06/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2014-11-06/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:19.896097 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2015-04-17/
+-rw-r--r--   0 runner    (1001) docker     (127)    40823 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2015-04-17/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2015-04-17/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)   150842 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2015-04-17/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2015-04-17/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:19.900097 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2015-07-27/
+-rw-r--r--   0 runner    (1001) docker     (127)    40823 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2015-07-27/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2015-07-27/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)   154636 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2015-07-27/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2015-07-27/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:19.900097 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2015-09-17/
+-rw-r--r--   0 runner    (1001) docker     (127)    40823 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2015-09-17/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2015-09-17/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)   130784 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2015-09-17/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2015-09-17/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:19.900097 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2016-01-13/
+-rw-r--r--   0 runner    (1001) docker     (127)    40823 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2016-01-13/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2016-01-13/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)   133880 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2016-01-13/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2016-01-13/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:19.900097 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2016-01-28/
+-rw-r--r--   0 runner    (1001) docker     (127)    26040 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2016-01-28/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2016-01-28/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2016-01-28/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)   133424 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2016-01-28/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2016-01-28/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:19.904096 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2016-08-01/
+-rw-r--r--   0 runner    (1001) docker     (127)    26040 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2016-08-01/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2016-08-01/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2016-08-01/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)   148384 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2016-08-01/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2016-08-01/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:19.904096 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2016-08-20/
+-rw-r--r--   0 runner    (1001) docker     (127)    26040 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2016-08-20/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2016-08-20/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)   150982 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2016-08-20/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2016-08-20/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:19.904096 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2016-09-07/
+-rw-r--r--   0 runner    (1001) docker     (127)    26040 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2016-09-07/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2016-09-07/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2016-09-07/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)   151766 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2016-09-07/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2016-09-07/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:19.908097 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2016-09-29/
+-rw-r--r--   0 runner    (1001) docker     (127)    26040 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2016-09-29/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2016-09-29/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2016-09-29/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)   194806 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2016-09-29/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2016-09-29/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:19.908097 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2016-11-25/
+-rw-r--r--   0 runner    (1001) docker     (127)    26040 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2016-11-25/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2016-11-25/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2016-11-25/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)   197970 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2016-11-25/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2016-11-25/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:19.908097 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2017-03-25/
+-rw-r--r--   0 runner    (1001) docker     (127)    26040 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2017-03-25/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2017-03-25/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)   206093 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2017-03-25/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2017-03-25/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:19.908097 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2017-10-30/
+-rw-r--r--   0 runner    (1001) docker     (127)    26040 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2017-10-30/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2017-10-30/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2017-10-30/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)   264716 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2017-10-30/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2017-10-30/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:19.912097 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2018-06-18/
+-rw-r--r--   0 runner    (1001) docker     (127)    26040 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2018-06-18/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2018-06-18/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2018-06-18/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)   267331 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2018-06-18/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2018-06-18/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:19.912097 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2018-11-05/
+-rw-r--r--   0 runner    (1001) docker     (127)    26040 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2018-11-05/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2018-11-05/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2018-11-05/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)   273141 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2018-11-05/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2018-11-05/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:19.912097 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2019-03-26/
+-rw-r--r--   0 runner    (1001) docker     (127)    26040 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2019-03-26/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2019-03-26/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2019-03-26/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)   281937 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2019-03-26/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2019-03-26/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:19.916097 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2020-05-31/
+-rw-r--r--   0 runner    (1001) docker     (127)    20918 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2020-05-31/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2020-05-31/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2020-05-31/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)   590197 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2020-05-31/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-07 01:02:10.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2020-05-31/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:19.916097 botocore-a-la-carte-cloudfront-1.34.99/botocore_a_la_carte_cloudfront.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-07 01:02:19.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore_a_la_carte_cloudfront.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4879 2024-05-07 01:02:19.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore_a_la_carte_cloudfront.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 01:02:19.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore_a_la_carte_cloudfront.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-07 01:02:19.000000 botocore-a-la-carte-cloudfront-1.34.99/botocore_a_la_carte_cloudfront.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 01:02:19.916097 botocore-a-la-carte-cloudfront-1.34.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-07 01:02:19.000000 botocore-a-la-carte-cloudfront-1.34.99/setup.py
```

### Comparing `botocore-a-la-carte-cloudfront-1.34.98/LICENSE.txt` & `botocore-a-la-carte-cloudfront-1.34.99/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.34.98/PKG-INFO` & `botocore-a-la-carte-cloudfront-1.34.99/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-cloudfront
-Version: 1.34.98
+Version: 1.34.99
 Summary: cloudfront data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2014-05-31/endpoint-rule-set-1.json` & `botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2014-05-31/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2014-05-31/paginators-1.json` & `botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2014-05-31/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2014-05-31/service-2.json` & `botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2014-05-31/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2014-05-31/waiters-2.json` & `botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2014-05-31/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2014-10-21/endpoint-rule-set-1.json` & `botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2014-10-21/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2014-10-21/paginators-1.json` & `botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2014-10-21/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2014-10-21/service-2.json` & `botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2014-10-21/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2014-10-21/waiters-2.json` & `botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2014-10-21/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2014-11-06/endpoint-rule-set-1.json` & `botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2014-11-06/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2014-11-06/paginators-1.json` & `botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2014-11-06/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2014-11-06/service-2.json` & `botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2014-11-06/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2014-11-06/waiters-2.json` & `botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2014-11-06/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2015-04-17/endpoint-rule-set-1.json` & `botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2015-04-17/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2015-04-17/paginators-1.json` & `botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2015-04-17/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2015-04-17/service-2.json` & `botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2015-04-17/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2015-04-17/waiters-2.json` & `botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2015-04-17/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2015-07-27/endpoint-rule-set-1.json` & `botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2015-07-27/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2015-07-27/paginators-1.json` & `botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2015-07-27/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2015-07-27/service-2.json` & `botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2015-07-27/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2015-07-27/waiters-2.json` & `botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2015-07-27/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2015-09-17/endpoint-rule-set-1.json` & `botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2015-09-17/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2015-09-17/paginators-1.json` & `botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2015-09-17/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2015-09-17/service-2.json` & `botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2015-09-17/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2015-09-17/waiters-2.json` & `botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2015-09-17/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2016-01-13/endpoint-rule-set-1.json` & `botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2016-01-13/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2016-01-13/paginators-1.json` & `botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2016-01-13/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2016-01-13/service-2.json` & `botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2016-01-13/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2016-01-13/waiters-2.json` & `botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2016-01-13/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2016-01-28/endpoint-rule-set-1.json` & `botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2016-01-28/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2016-01-28/paginators-1.json` & `botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2016-01-28/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2016-01-28/service-2.json` & `botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2016-01-28/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2016-01-28/waiters-2.json` & `botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2016-01-28/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2016-08-01/endpoint-rule-set-1.json` & `botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2016-08-01/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2016-08-01/paginators-1.json` & `botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2016-08-01/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2016-08-01/service-2.json` & `botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2016-08-01/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2016-08-01/waiters-2.json` & `botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2016-08-01/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2016-08-20/endpoint-rule-set-1.json` & `botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2016-08-20/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2016-08-20/paginators-1.json` & `botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2016-08-20/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2016-08-20/service-2.json` & `botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2016-08-20/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2016-08-20/waiters-2.json` & `botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2016-08-20/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2016-09-07/endpoint-rule-set-1.json` & `botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2016-09-07/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2016-09-07/paginators-1.json` & `botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2016-09-07/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2016-09-07/service-2.json` & `botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2016-09-07/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2016-09-07/waiters-2.json` & `botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2016-09-07/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2016-09-29/endpoint-rule-set-1.json` & `botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2016-09-29/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2016-09-29/paginators-1.json` & `botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2016-09-29/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2016-09-29/service-2.json` & `botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2016-09-29/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2016-09-29/waiters-2.json` & `botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2016-09-29/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2016-11-25/endpoint-rule-set-1.json` & `botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2016-11-25/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2016-11-25/paginators-1.json` & `botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2016-11-25/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2016-11-25/service-2.json` & `botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2016-11-25/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2016-11-25/waiters-2.json` & `botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2016-11-25/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2017-03-25/endpoint-rule-set-1.json` & `botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2017-03-25/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2017-03-25/paginators-1.json` & `botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2017-03-25/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2017-03-25/service-2.json` & `botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2017-03-25/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2017-03-25/waiters-2.json` & `botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2017-03-25/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2017-10-30/endpoint-rule-set-1.json` & `botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2017-10-30/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2017-10-30/paginators-1.json` & `botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2017-10-30/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2017-10-30/service-2.json` & `botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2017-10-30/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2017-10-30/waiters-2.json` & `botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2017-10-30/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2018-06-18/endpoint-rule-set-1.json` & `botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2018-06-18/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2018-06-18/paginators-1.json` & `botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2018-06-18/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2018-06-18/service-2.json` & `botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2018-06-18/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2018-06-18/waiters-2.json` & `botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2018-06-18/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2018-11-05/endpoint-rule-set-1.json` & `botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2018-11-05/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2018-11-05/paginators-1.json` & `botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2018-11-05/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2018-11-05/service-2.json` & `botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2018-11-05/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2018-11-05/waiters-2.json` & `botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2018-11-05/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2019-03-26/endpoint-rule-set-1.json` & `botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2019-03-26/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2019-03-26/paginators-1.json` & `botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2019-03-26/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2019-03-26/service-2.json` & `botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2019-03-26/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2019-03-26/waiters-2.json` & `botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2019-03-26/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2020-05-31/endpoint-rule-set-1.json` & `botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2020-05-31/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2020-05-31/paginators-1.json` & `botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2020-05-31/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2020-05-31/service-2.json` & `botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2020-05-31/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.34.98/botocore/data/cloudfront/2020-05-31/waiters-2.json` & `botocore-a-la-carte-cloudfront-1.34.99/botocore/data/cloudfront/2020-05-31/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.34.98/botocore_a_la_carte_cloudfront.egg-info/PKG-INFO` & `botocore-a-la-carte-cloudfront-1.34.99/botocore_a_la_carte_cloudfront.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-cloudfront
-Version: 1.34.98
+Version: 1.34.99
 Summary: cloudfront data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-cloudfront-1.34.98/botocore_a_la_carte_cloudfront.egg-info/SOURCES.txt` & `botocore-a-la-carte-cloudfront-1.34.99/botocore_a_la_carte_cloudfront.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.34.98/setup.py` & `botocore-a-la-carte-cloudfront-1.34.99/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-cloudfront',
-    version="1.34.98",
+    version="1.34.99",
     description='cloudfront data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/cloudfront/*/*.json'],
```

