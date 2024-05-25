# Comparing `tmp/botocore-a-la-carte-1.34.98.tar.gz` & `tmp/botocore-a-la-carte-1.34.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-1.34.98.tar", last modified: Sat May  4 01:01:48 2024, max compression
+gzip compressed data, was "botocore-a-la-carte-1.34.99.tar", last modified: Tue May  7 01:02:50 2024, max compression
```

## Comparing `botocore-a-la-carte-1.34.98.tar` & `botocore-a-la-carte-1.34.99.tar`

### file list

```diff
@@ -1,2010 +1,2010 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:48.034327 botocore-a-la-carte-1.34.98/
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-05-04 01:01:48.034327 botocore-a-la-carte-1.34.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-04 01:01:47.000000 botocore-a-la-carte-1.34.98/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.886326 botocore-a-la-carte-1.34.98/botocore/
--rw-r--r--   0 runner    (1001) docker     (127)     4914 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/botocore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30640 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/botocore/args.py
--rw-r--r--   0 runner    (1001) docker     (127)    43803 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/botocore/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    23156 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/botocore/awsrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)   266617 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/botocore/cacert.pem
--rw-r--r--   0 runner    (1001) docker     (127)    51753 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/botocore/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    11091 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/botocore/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4430 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/botocore/compress.py
--rw-r--r--   0 runner    (1001) docker     (127)    15601 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/botocore/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    10039 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/botocore/configloader.py
--rw-r--r--   0 runner    (1001) docker     (127)    37230 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/botocore/configprovider.py
--rw-r--r--   0 runner    (1001) docker     (127)    84795 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/botocore/credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.886326 botocore-a-la-carte-1.34.98/botocore/crt/
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/botocore/crt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25318 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/botocore/crt/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.886326 botocore-a-la-carte-1.34.98/botocore/data/
--rw-r--r--   0 runner    (1001) docker     (127)     7025 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/botocore/data/_retry.json
--rw-r--r--   0 runner    (1001) docker     (127)   879830 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/botocore/data/endpoints.json
--rw-r--r--   0 runner    (1001) docker     (127)     5765 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/botocore/data/partitions.json
--rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/botocore/data/sdk-default-configuration.json
--rw-r--r--   0 runner    (1001) docker     (127)    11075 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/botocore/discovery.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.890326 botocore-a-la-carte-1.34.98/botocore/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/botocore/docs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.890326 botocore-a-la-carte-1.34.98/botocore/docs/bcdoc/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/botocore/docs/bcdoc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10207 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/botocore/docs/bcdoc/docstringparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     9698 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/botocore/docs/bcdoc/restdoc.py
--rw-r--r--   0 runner    (1001) docker     (127)    13148 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/botocore/docs/bcdoc/style.py
--rw-r--r--   0 runner    (1001) docker     (127)    17380 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/botocore/docs/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/botocore/docs/docstring.py
--rw-r--r--   0 runner    (1001) docker     (127)     8949 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/botocore/docs/example.py
--rw-r--r--   0 runner    (1001) docker     (127)    12058 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/botocore/docs/method.py
--rw-r--r--   0 runner    (1001) docker     (127)     9020 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/botocore/docs/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    11760 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/botocore/docs/params.py
--rw-r--r--   0 runner    (1001) docker     (127)     4990 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/botocore/docs/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     5198 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/botocore/docs/shape.py
--rw-r--r--   0 runner    (1001) docker     (127)     9214 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/botocore/docs/sharedexample.py
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/botocore/docs/translator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7292 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/botocore/docs/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6626 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/botocore/docs/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)    16441 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/botocore/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)    22934 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/botocore/endpoint_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     3722 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/botocore/errorfactory.py
--rw-r--r--   0 runner    (1001) docker     (127)    20449 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/botocore/eventstream.py
--rw-r--r--   0 runner    (1001) docker     (127)    22804 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/botocore/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    55288 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/botocore/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/botocore/history.py
--rw-r--r--   0 runner    (1001) docker     (127)    25060 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/botocore/hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)    16292 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/botocore/httpchecksum.py
--rw-r--r--   0 runner    (1001) docker     (127)    18582 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/botocore/httpsession.py
--rw-r--r--   0 runner    (1001) docker     (127)    18833 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/botocore/loaders.py
--rw-r--r--   0 runner    (1001) docker     (127)    30619 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/botocore/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    20597 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/botocore/monitoring.py
--rw-r--r--   0 runner    (1001) docker     (127)    27392 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/botocore/paginate.py
--rw-r--r--   0 runner    (1001) docker     (127)    45607 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/botocore/parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)    32426 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/botocore/regions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7227 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/botocore/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.890326 botocore-a-la-carte-1.34.98/botocore/retries/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/botocore/retries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4207 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/botocore/retries/adaptive.py
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/botocore/retries/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3993 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/botocore/retries/bucket.py
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/botocore/retries/quota.py
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/botocore/retries/special.py
--rw-r--r--   0 runner    (1001) docker     (127)    19974 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/botocore/retries/standard.py
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/botocore/retries/throttling.py
--rw-r--r--   0 runner    (1001) docker     (127)    14700 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/botocore/retryhandler.py
--rw-r--r--   0 runner    (1001) docker     (127)    33122 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/botocore/serialize.py
--rw-r--r--   0 runner    (1001) docker     (127)    49184 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/botocore/session.py
--rw-r--r--   0 runner    (1001) docker     (127)    30965 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/botocore/signers.py
--rw-r--r--   0 runner    (1001) docker     (127)    15152 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/botocore/stub.py
--rw-r--r--   0 runner    (1001) docker     (127)    10910 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/botocore/tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/botocore/translate.py
--rw-r--r--   0 runner    (1001) docker     (127)    18305 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/botocore/useragent.py
--rw-r--r--   0 runner    (1001) docker     (127)   135065 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/botocore/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13767 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/botocore/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.890326 botocore-a-la-carte-1.34.98/botocore/vendored/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/botocore/vendored/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.890326 botocore-a-la-carte-1.34.98/botocore/vendored/requests/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/botocore/vendored/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/botocore/vendored/requests/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.890326 botocore-a-la-carte-1.34.98/botocore/vendored/requests/packages/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/botocore/vendored/requests/packages/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.890326 botocore-a-la-carte-1.34.98/botocore/vendored/requests/packages/urllib3/
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/botocore/vendored/requests/packages/urllib3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/botocore/vendored/requests/packages/urllib3/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    34549 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/botocore/vendored/six.py
--rw-r--r--   0 runner    (1001) docker     (127)    14290 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/botocore/waiter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.890326 botocore-a-la-carte-1.34.98/botocore_a_la_carte.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-05-04 01:01:47.000000 botocore-a-la-carte-1.34.98/botocore_a_la_carte.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    91711 2024-05-04 01:01:47.000000 botocore-a-la-carte-1.34.98/botocore_a_la_carte.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 01:01:47.000000 botocore-a-la-carte-1.34.98/botocore_a_la_carte.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-04 01:01:47.000000 botocore-a-la-carte-1.34.98/botocore_a_la_carte.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-04 01:01:47.000000 botocore-a-la-carte-1.34.98/botocore_a_la_carte.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.890326 botocore-a-la-carte-1.34.98/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     5657 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     5109 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.890326 botocore-a-la-carte-1.34.98/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.890326 botocore-a-la-carte-1.34.98/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/docs/source/_static/404.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.890326 botocore-a-la-carte-1.34.98/docs/source/_static/css/
--rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/docs/source/_static/css/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.890326 botocore-a-la-carte-1.34.98/docs/source/_static/js/
--rw-r--r--   0 runner    (1001) docker     (127)     7600 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/docs/source/_static/js/custom.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.890326 botocore-a-la-carte-1.34.98/docs/source/_static/logos/
--rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/docs/source/_static/logos/aws_dark_theme_logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3399 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/docs/source/_static/logos/aws_light_theme_logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)   136184 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/docs/source/_static/shortbreadv1.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.890326 botocore-a-la-carte-1.34.98/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)    13300 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/docs/source/_templates/page.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.894326 botocore-a-la-carte-1.34.98/docs/source/_templates/sidebar/
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/docs/source/_templates/sidebar/close-icon.html
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/docs/source/_templates/sidebar/feedback.html
--rw-r--r--   0 runner    (1001) docker     (127)     8369 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/docs/source/client_upgrades.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9883 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.894326 botocore-a-la-carte-1.34.98/docs/source/development/
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/docs/source/development/changesfor10.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/docs/source/development/designnotes.rst
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/docs/source/development/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9302 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.894326 botocore-a-la-carte-1.34.98/docs/source/reference/
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/docs/source/reference/awsrequest.rst
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/docs/source/reference/config.rst
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/docs/source/reference/eventstream.rst
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/docs/source/reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/docs/source/reference/loaders.rst
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/docs/source/reference/response.rst
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/docs/source/reference/stubber.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.894326 botocore-a-la-carte-1.34.98/docs/source/topics/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/docs/source/topics/document_type.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/docs/source/topics/events.rst
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/docs/source/topics/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/docs/source/topics/paginators.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.894326 botocore-a-la-carte-1.34.98/docs/source/tutorial/
--rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/docs/source/tutorial/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)    21852 2024-05-04 01:01:48.034327 botocore-a-la-carte-1.34.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-05-04 01:01:47.000000 botocore-a-la-carte-1.34.98/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.894326 botocore-a-la-carte-1.34.98/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    18817 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.850325 botocore-a-la-carte-1.34.98/tests/acceptance/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.894326 botocore-a-la-carte-1.34.98/tests/acceptance/features/
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/acceptance/features/environment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.854325 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.894326 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/acm/
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/acm/acm.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.894326 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/autoscaling/
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/autoscaling/autoscaling.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.894326 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/cloudformation/
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/cloudformation/cloudformation.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.894326 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/cloudfront/
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/cloudfront/cloudfront.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.894326 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/cloudhsm/
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/cloudhsm/cloudhsm.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.894326 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/cloudsearch/
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/cloudsearch/cloudsearch.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.894326 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/cloudtrail/
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/cloudtrail/cloudtrail.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.894326 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/cloudwatch/
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/cloudwatch/cloudwatch.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.894326 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/cloudwatchlogs/
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/cloudwatchlogs/cloudwatchlogs.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.894326 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/codecommit/
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/codecommit/codecommit.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.894326 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/codedeploy/
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/codedeploy/codedeploy.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.894326 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/codepipeline/
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/codepipeline/codepipeline.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.894326 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/cognitoidentity/
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/cognitoidentity/cognitoidentity.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.894326 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/cognitosync/
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/cognitosync/cognitosync.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.894326 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/configservice/
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/configservice/configservice.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.894326 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/datapipeline/
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/datapipeline/datapipeline.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.894326 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/devicefarm/
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/devicefarm/devicefarm.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.894326 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/directconnect/
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/directconnect/directconnect.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.894326 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/directoryservice/
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/directoryservice/directoryservice.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.894326 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/dynamodb/
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/dynamodb/dynamodb.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.894326 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/dynamodbstreams/
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/dynamodbstreams/dynamodbstreams.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.894326 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/ec2/
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/ec2/ec2.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.894326 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/ecs/
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/ecs/ecs.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.894326 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/efs/
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/efs/efs.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.898326 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/elasticache/
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/elasticache/elasticache.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.898326 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/elasticbeanstalk/
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/elasticbeanstalk/elasticbeanstalk.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.898326 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/elasticloadbalancing/
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/elasticloadbalancing/elasticloadbalancing.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.898326 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/elastictranscoder/
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/elastictranscoder/elastictranscoder.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.898326 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/emr/
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/emr/emr.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.898326 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/es/
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/es/es.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.898326 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/glacier/
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/glacier/glacier.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.898326 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/iam/
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/iam/iam.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.898326 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/importexport/
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/importexport/importexport.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.898326 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/kinesis/
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/kinesis/kinesis.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.898326 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/kms/
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/kms/kms.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.898326 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/lambda/
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/lambda/lambda.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.898326 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/machinelearning/
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/machinelearning/machinelearning.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.898326 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/opsworks/
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/opsworks/opsworks.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.898326 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/rds/
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/rds/rds.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.898326 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/redshift/
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/redshift/redshift.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.898326 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/route53/
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/route53/route53.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.898326 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/route53domains/
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/route53domains/route53domains.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.898326 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/ses/
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/ses/ses.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.898326 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/sns/
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/sns/sns.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.898326 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/sqs/
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/sqs/sqs.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.898326 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/ssm/
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/ssm/ssm.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.898326 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/storagegateway/
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/storagegateway/storagegateway.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.898326 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/sts/
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/sts/sts.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.898326 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/support/
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/support/support.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.898326 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/swf/
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/swf/swf.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.898326 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/waf/
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/waf/waf.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.898326 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/workspaces/
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/workspaces/workspaces.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.898326 botocore-a-la-carte-1.34.98/tests/acceptance/features/steps/
--rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/acceptance/features/steps/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8444 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/cmd-runner
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.906326 botocore-a-la-carte-1.34.98/tests/functional/
--rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.906326 botocore-a-la-carte-1.34.98/tests/functional/configured_endpoint_urls/
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/configured_endpoint_urls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20184 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/configured_endpoint_urls/profile-tests.json
--rw-r--r--   0 runner    (1001) docker     (127)     7578 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/configured_endpoint_urls/test_configured_endpoint_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.906326 botocore-a-la-carte-1.34.98/tests/functional/crt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/crt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.906326 botocore-a-la-carte-1.34.98/tests/functional/csm/
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/csm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32068 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/csm/cases.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.854325 botocore-a-la-carte-1.34.98/tests/functional/csm/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.854325 botocore-a-la-carte-1.34.98/tests/functional/csm/data/csmtest/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.906326 botocore-a-la-carte-1.34.98/tests/functional/csm/data/csmtest/2018-06-19/
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/csm/data/csmtest/2018-06-19/service-2.json
--rw-r--r--   0 runner    (1001) docker     (127)     6741 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/csm/test_monitoring.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.906326 botocore-a-la-carte-1.34.98/tests/functional/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     5588 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/docs/test_alias.py
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/docs/test_autoscaling.py
--rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/docs/test_ec2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/docs/test_glacier.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/docs/test_lex.py
--rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/docs/test_s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/docs/test_secretsmanager.py
--rw-r--r--   0 runner    (1001) docker     (127)     5333 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/docs/test_shared_example_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/docs/test_streaming_body.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.874326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.906326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/accessanalyzer/
--rw-r--r--   0 runner    (1001) docker     (127)    22841 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/accessanalyzer/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.906326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/account/
--rw-r--r--   0 runner    (1001) docker     (127)    12812 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/account/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.906326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/acm/
--rw-r--r--   0 runner    (1001) docker     (127)    21886 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/acm/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.906326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/acm-pca/
--rw-r--r--   0 runner    (1001) docker     (127)    22050 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/acm-pca/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.906326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/alexaforbusiness/
--rw-r--r--   0 runner    (1001) docker     (127)    10458 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/alexaforbusiness/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.906326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/amp/
--rw-r--r--   0 runner    (1001) docker     (127)    14268 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/amp/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.906326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/amplify/
--rw-r--r--   0 runner    (1001) docker     (127)    18190 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/amplify/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.906326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/amplifybackend/
--rw-r--r--   0 runner    (1001) docker     (127)    17569 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/amplifybackend/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.906326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/amplifyuibuilder/
--rw-r--r--   0 runner    (1001) docker     (127)    17633 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/amplifyuibuilder/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.906326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/apigateway/
--rw-r--r--   0 runner    (1001) docker     (127)    20036 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/apigateway/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.906326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/apigatewaymanagementapi/
--rw-r--r--   0 runner    (1001) docker     (127)    10586 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/apigatewaymanagementapi/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.906326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/apigatewayv2/
--rw-r--r--   0 runner    (1001) docker     (127)    20036 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/apigatewayv2/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.910326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/appconfig/
--rw-r--r--   0 runner    (1001) docker     (127)    21296 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/appconfig/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.910326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/appconfigdata/
--rw-r--r--   0 runner    (1001) docker     (127)    20581 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/appconfigdata/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.910326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/appfabric/
--rw-r--r--   0 runner    (1001) docker     (127)    10554 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/appfabric/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.910326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/appflow/
--rw-r--r--   0 runner    (1001) docker     (127)    16921 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/appflow/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.910326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/appintegrations/
--rw-r--r--   0 runner    (1001) docker     (127)    14617 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/appintegrations/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.910326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/application-autoscaling/
--rw-r--r--   0 runner    (1001) docker     (127)    21870 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/application-autoscaling/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.910326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/application-insights/
--rw-r--r--   0 runner    (1001) docker     (127)    20378 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/application-insights/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.910326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/applicationcostprofiler/
--rw-r--r--   0 runner    (1001) docker     (127)    10810 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/applicationcostprofiler/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.910326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/appmesh/
--rw-r--r--   0 runner    (1001) docker     (127)    27442 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/appmesh/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.910326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/apprunner/
--rw-r--r--   0 runner    (1001) docker     (127)    13113 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/apprunner/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.910326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/appstream/
--rw-r--r--   0 runner    (1001) docker     (127)    16617 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/appstream/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.910326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/appsync/
--rw-r--r--   0 runner    (1001) docker     (127)    19065 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/appsync/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.910326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/arc-zonal-shift/
--rw-r--r--   0 runner    (1001) docker     (127)    10650 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/arc-zonal-shift/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.910326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/artifact/
--rw-r--r--   0 runner    (1001) docker     (127)    10538 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/artifact/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.910326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/athena/
--rw-r--r--   0 runner    (1001) docker     (127)    21588 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/athena/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.910326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/auditmanager/
--rw-r--r--   0 runner    (1001) docker     (127)    15354 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/auditmanager/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.910326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/autoscaling/
--rw-r--r--   0 runner    (1001) docker     (127)    20943 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/autoscaling/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.910326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/autoscaling-plans/
--rw-r--r--   0 runner    (1001) docker     (127)    20748 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/autoscaling-plans/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.910326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/b2bi/
--rw-r--r--   0 runner    (1001) docker     (127)    10474 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/b2bi/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.910326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/backup/
--rw-r--r--   0 runner    (1001) docker     (127)    20319 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/backup/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.910326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/backup-gateway/
--rw-r--r--   0 runner    (1001) docker     (127)    19742 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/backup-gateway/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.910326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/backupstorage/
--rw-r--r--   0 runner    (1001) docker     (127)    10618 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/backupstorage/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.910326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/batch/
--rw-r--r--   0 runner    (1001) docker     (127)    21970 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/batch/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.910326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/bcm-data-exports/
--rw-r--r--   0 runner    (1001) docker     (127)     4942 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/bcm-data-exports/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.910326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/bedrock/
--rw-r--r--   0 runner    (1001) docker     (127)    10522 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/bedrock/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.910326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/bedrock-agent/
--rw-r--r--   0 runner    (1001) docker     (127)    10618 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/bedrock-agent/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.910326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/bedrock-agent-runtime/
--rw-r--r--   0 runner    (1001) docker     (127)    10746 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/bedrock-agent-runtime/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.910326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/bedrock-runtime/
--rw-r--r--   0 runner    (1001) docker     (127)    10650 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/bedrock-runtime/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.910326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/billingconductor/
--rw-r--r--   0 runner    (1001) docker     (127)    11824 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/billingconductor/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.910326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/braket/
--rw-r--r--   0 runner    (1001) docker     (127)    11766 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/braket/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.910326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/budgets/
--rw-r--r--   0 runner    (1001) docker     (127)    12762 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/budgets/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.910326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/ce/
--rw-r--r--   0 runner    (1001) docker     (127)    12702 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/ce/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.910326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/chatbot/
--rw-r--r--   0 runner    (1001) docker     (127)    10522 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/chatbot/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.910326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/chime/
--rw-r--r--   0 runner    (1001) docker     (127)    11615 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/chime/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.910326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/chime-sdk-identity/
--rw-r--r--   0 runner    (1001) docker     (127)    11071 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/chime-sdk-identity/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.910326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/chime-sdk-media-pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)    12513 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/chime-sdk-media-pipelines/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.914326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/chime-sdk-meetings/
--rw-r--r--   0 runner    (1001) docker     (127)    13256 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/chime-sdk-meetings/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.914326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/chime-sdk-messaging/
--rw-r--r--   0 runner    (1001) docker     (127)    11088 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/chime-sdk-messaging/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.914326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/chime-sdk-voice/
--rw-r--r--   0 runner    (1001) docker     (127)    10586 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/chime-sdk-voice/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.914326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/cleanrooms/
--rw-r--r--   0 runner    (1001) docker     (127)    10570 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/cleanrooms/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.914326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/cleanroomsml/
--rw-r--r--   0 runner    (1001) docker     (127)    10618 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/cleanroomsml/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.914326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/cloud9/
--rw-r--r--   0 runner    (1001) docker     (127)    19014 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/cloud9/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.914326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/cloudcontrol/
--rw-r--r--   0 runner    (1001) docker     (127)    22851 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/cloudcontrol/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.914326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/clouddirectory/
--rw-r--r--   0 runner    (1001) docker     (127)    14979 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/clouddirectory/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.914326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/cloudformation/
--rw-r--r--   0 runner    (1001) docker     (127)    22794 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/cloudformation/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.914326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/cloudfront/
--rw-r--r--   0 runner    (1001) docker     (127)    13981 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/cloudfront/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.914326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/cloudfront-keyvaluestore/
--rw-r--r--   0 runner    (1001) docker     (127)     8023 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/cloudfront-keyvaluestore/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.914326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/cloudhsm/
--rw-r--r--   0 runner    (1001) docker     (127)    10972 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/cloudhsm/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.914326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/cloudhsmv2/
--rw-r--r--   0 runner    (1001) docker     (127)    19594 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/cloudhsmv2/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.914326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/cloudsearch/
--rw-r--r--   0 runner    (1001) docker     (127)    14480 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/cloudsearch/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.914326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/cloudsearchdomain/
--rw-r--r--   0 runner    (1001) docker     (127)    10682 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/cloudsearchdomain/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.914326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/cloudtrail/
--rw-r--r--   0 runner    (1001) docker     (127)    22618 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/cloudtrail/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.914326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/cloudtrail-data/
--rw-r--r--   0 runner    (1001) docker     (127)    10650 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/cloudtrail-data/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.914326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/cloudwatch/
--rw-r--r--   0 runner    (1001) docker     (127)    22618 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/cloudwatch/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.914326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/codeartifact/
--rw-r--r--   0 runner    (1001) docker     (127)    15777 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/codeartifact/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.914326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/codebuild/
--rw-r--r--   0 runner    (1001) docker     (127)    22152 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/codebuild/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.914326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/codecatalyst/
--rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/codecatalyst/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.914326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/codecommit/
--rw-r--r--   0 runner    (1001) docker     (127)    22192 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/codecommit/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.914326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/codeconnections/
--rw-r--r--   0 runner    (1001) docker     (127)    10650 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/codeconnections/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.914326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/codedeploy/
--rw-r--r--   0 runner    (1001) docker     (127)    22628 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/codedeploy/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.914326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/codeguru-reviewer/
--rw-r--r--   0 runner    (1001) docker     (127)    14618 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/codeguru-reviewer/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.914326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/codeguru-security/
--rw-r--r--   0 runner    (1001) docker     (127)    10682 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/codeguru-security/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.914326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/codeguruprofiler/
--rw-r--r--   0 runner    (1001) docker     (127)    10682 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/codeguruprofiler/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.914326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/codepipeline/
--rw-r--r--   0 runner    (1001) docker     (127)    20979 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/codepipeline/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.914326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/codestar/
--rw-r--r--   0 runner    (1001) docker     (127)    15683 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/codestar/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.914326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/codestar-connections/
--rw-r--r--   0 runner    (1001) docker     (127)    17324 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/codestar-connections/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.914326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/codestar-notifications/
--rw-r--r--   0 runner    (1001) docker     (127)    10762 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/codestar-notifications/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.914326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/cognito-identity/
--rw-r--r--   0 runner    (1001) docker     (127)    19386 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/cognito-identity/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.914326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/cognito-idp/
--rw-r--r--   0 runner    (1001) docker     (127)    19634 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/cognito-idp/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.914326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/cognito-sync/
--rw-r--r--   0 runner    (1001) docker     (127)    14934 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/cognito-sync/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.914326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/comprehend/
--rw-r--r--   0 runner    (1001) docker     (127)    17044 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/comprehend/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.914326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/comprehendmedical/
--rw-r--r--   0 runner    (1001) docker     (127)    15049 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/comprehendmedical/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.914326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/compute-optimizer/
--rw-r--r--   0 runner    (1001) docker     (127)    17680 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/compute-optimizer/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.918326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/config/
--rw-r--r--   0 runner    (1001) docker     (127)    22442 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/config/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.918326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/connect/
--rw-r--r--   0 runner    (1001) docker     (127)    15251 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/connect/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.918326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/connect-contact-lens/
--rw-r--r--   0 runner    (1001) docker     (127)    13647 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/connect-contact-lens/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.918326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/connectcampaigns/
--rw-r--r--   0 runner    (1001) docker     (127)    11990 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/connectcampaigns/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.918326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/connectcases/
--rw-r--r--   0 runner    (1001) docker     (127)    10490 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/connectcases/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.918326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/connectparticipant/
--rw-r--r--   0 runner    (1001) docker     (127)    11597 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/connectparticipant/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.918326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/controlcatalog/
--rw-r--r--   0 runner    (1001) docker     (127)    10634 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/controlcatalog/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.918326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/controltower/
--rw-r--r--   0 runner    (1001) docker     (127)    17946 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/controltower/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.918326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/cost-optimization-hub/
--rw-r--r--   0 runner    (1001) docker     (127)    10746 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/cost-optimization-hub/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.918326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/cur/
--rw-r--r--   0 runner    (1001) docker     (127)    10893 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/cur/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.918326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/customer-profiles/
--rw-r--r--   0 runner    (1001) docker     (127)    14392 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/customer-profiles/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.918326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/databrew/
--rw-r--r--   0 runner    (1001) docker     (127)    19530 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/databrew/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.918326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/dataexchange/
--rw-r--r--   0 runner    (1001) docker     (127)    14931 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/dataexchange/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.918326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/datapipeline/
--rw-r--r--   0 runner    (1001) docker     (127)    12336 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/datapipeline/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.918326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/datasync/
--rw-r--r--   0 runner    (1001) docker     (127)    22103 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/datasync/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.918326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/datazone/
--rw-r--r--   0 runner    (1001) docker     (127)     3782 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/datazone/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.918326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/dax/
--rw-r--r--   0 runner    (1001) docker     (127)    15954 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/dax/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.918326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/deadline/
--rw-r--r--   0 runner    (1001) docker     (127)    10538 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/deadline/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.918326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/detective/
--rw-r--r--   0 runner    (1001) docker     (127)    20995 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/detective/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.918326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/devicefarm/
--rw-r--r--   0 runner    (1001) docker     (127)    10994 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/devicefarm/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.918326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/devops-guru/
--rw-r--r--   0 runner    (1001) docker     (127)    14899 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/devops-guru/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.918326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/directconnect/
--rw-r--r--   0 runner    (1001) docker     (127)    22318 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/directconnect/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.918326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/discovery/
--rw-r--r--   0 runner    (1001) docker     (127)    13131 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/discovery/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.918326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/dlm/
--rw-r--r--   0 runner    (1001) docker     (127)    20624 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/dlm/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.918326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/dms/
--rw-r--r--   0 runner    (1001) docker     (127)    22724 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/dms/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.918326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/docdb/
--rw-r--r--   0 runner    (1001) docker     (127)    22739 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/docdb/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.918326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/docdb-elastic/
--rw-r--r--   0 runner    (1001) docker     (127)    10618 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/docdb-elastic/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.918326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/drs/
--rw-r--r--   0 runner    (1001) docker     (127)    18906 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/drs/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.918326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/ds/
--rw-r--r--   0 runner    (1001) docker     (127)    21848 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/ds/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.918326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/dynamodb/
--rw-r--r--   0 runner    (1001) docker     (127)    23714 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/dynamodb/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.918326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/dynamodbstreams/
--rw-r--r--   0 runner    (1001) docker     (127)    21894 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/dynamodbstreams/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.918326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/ebs/
--rw-r--r--   0 runner    (1001) docker     (127)    21891 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/ebs/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.918326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/ec2/
--rw-r--r--   0 runner    (1001) docker     (127)    24360 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/ec2/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.918326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/ec2-instance-connect/
--rw-r--r--   0 runner    (1001) docker     (127)    10730 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/ec2-instance-connect/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.918326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/ecr/
--rw-r--r--   0 runner    (1001) docker     (127)    22472 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/ecr/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.918326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/ecr-public/
--rw-r--r--   0 runner    (1001) docker     (127)    10634 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/ecr-public/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.922326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/ecs/
--rw-r--r--   0 runner    (1001) docker     (127)    22320 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/ecs/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.922326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/efs/
--rw-r--r--   0 runner    (1001) docker     (127)    30883 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/efs/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.922326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/eks/
--rw-r--r--   0 runner    (1001) docker     (127)    21884 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/eks/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.922326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/eks-auth/
--rw-r--r--   0 runner    (1001) docker     (127)     3782 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/eks-auth/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.922326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/elastic-inference/
--rw-r--r--   0 runner    (1001) docker     (127)    12951 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/elastic-inference/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.922326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/elasticache/
--rw-r--r--   0 runner    (1001) docker     (127)    22662 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/elasticache/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.922326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/elasticbeanstalk/
--rw-r--r--   0 runner    (1001) docker     (127)    22443 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/elasticbeanstalk/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.922326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/elastictranscoder/
--rw-r--r--   0 runner    (1001) docker     (127)    13747 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/elastictranscoder/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.922326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/elb/
--rw-r--r--   0 runner    (1001) docker     (127)    60943 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/elb/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.922326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/elbv2/
--rw-r--r--   0 runner    (1001) docker     (127)    23058 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/elbv2/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.922326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/emr/
--rw-r--r--   0 runner    (1001) docker     (127)    23324 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/emr/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.922326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/emr-containers/
--rw-r--r--   0 runner    (1001) docker     (127)    19317 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/emr-containers/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.922326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/emr-serverless/
--rw-r--r--   0 runner    (1001) docker     (127)    12364 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/emr-serverless/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.922326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/entityresolution/
--rw-r--r--   0 runner    (1001) docker     (127)    10666 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/entityresolution/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.922326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/es/
--rw-r--r--   0 runner    (1001) docker     (127)    22279 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/es/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.922326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/events/
--rw-r--r--   0 runner    (1001) docker     (127)    27931 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/events/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.922326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/evidently/
--rw-r--r--   0 runner    (1001) docker     (127)    13995 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/evidently/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.922326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/finspace/
--rw-r--r--   0 runner    (1001) docker     (127)    12235 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/finspace/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.922326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/finspace-data/
--rw-r--r--   0 runner    (1001) docker     (127)    12315 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/finspace-data/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.922326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/firehose/
--rw-r--r--   0 runner    (1001) docker     (127)    22109 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/firehose/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.922326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/fis/
--rw-r--r--   0 runner    (1001) docker     (127)    11309 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/fis/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.922326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/fms/
--rw-r--r--   0 runner    (1001) docker     (127)    27852 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/fms/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.922326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/forecast/
--rw-r--r--   0 runner    (1001) docker     (127)    15258 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/forecast/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.922326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/forecastquery/
--rw-r--r--   0 runner    (1001) docker     (127)    15393 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/forecastquery/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.922326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/frauddetector/
--rw-r--r--   0 runner    (1001) docker     (127)    12783 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/frauddetector/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.922326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/freetier/
--rw-r--r--   0 runner    (1001) docker     (127)     5640 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/freetier/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.922326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/fsx/
--rw-r--r--   0 runner    (1001) docker     (127)    21891 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/fsx/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.922326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/gamelift/
--rw-r--r--   0 runner    (1001) docker     (127)    19526 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/gamelift/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.922326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/glacier/
--rw-r--r--   0 runner    (1001) docker     (127)    22919 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/glacier/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.922326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/globalaccelerator/
--rw-r--r--   0 runner    (1001) docker     (127)    10682 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/globalaccelerator/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.922326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/glue/
--rw-r--r--   0 runner    (1001) docker     (127)    21504 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/glue/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.922326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/grafana/
--rw-r--r--   0 runner    (1001) docker     (127)    14380 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/grafana/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.922326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/greengrass/
--rw-r--r--   0 runner    (1001) docker     (127)    17830 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/greengrass/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.922326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/greengrassv2/
--rw-r--r--   0 runner    (1001) docker     (127)    17830 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/greengrassv2/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.922326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/groundstation/
--rw-r--r--   0 runner    (1001) docker     (127)    15796 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/groundstation/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.926326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/guardduty/
--rw-r--r--   0 runner    (1001) docker     (127)    22142 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/guardduty/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.926326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/health/
--rw-r--r--   0 runner    (1001) docker     (127)    12064 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/health/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.926326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/healthlake/
--rw-r--r--   0 runner    (1001) docker     (127)    11418 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/healthlake/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.926326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/honeycode/
--rw-r--r--   0 runner    (1001) docker     (127)    10977 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/honeycode/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.926326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/iam/
--rw-r--r--   0 runner    (1001) docker     (127)    19907 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/iam/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.926326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/identitystore/
--rw-r--r--   0 runner    (1001) docker     (127)    16697 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/identitystore/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.926326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/imagebuilder/
--rw-r--r--   0 runner    (1001) docker     (127)    11471 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/imagebuilder/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.926326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/importexport/
--rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/importexport/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.926326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/inspector/
--rw-r--r--   0 runner    (1001) docker     (127)    17418 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/inspector/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.926326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/inspector-scan/
--rw-r--r--   0 runner    (1001) docker     (127)    10634 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/inspector-scan/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.926326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/inspector2/
--rw-r--r--   0 runner    (1001) docker     (127)    18292 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/inspector2/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.926326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/internetmonitor/
--rw-r--r--   0 runner    (1001) docker     (127)    10650 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/internetmonitor/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.926326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/iot/
--rw-r--r--   0 runner    (1001) docker     (127)    20619 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/iot/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.926326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/iot-data/
--rw-r--r--   0 runner    (1001) docker     (127)    20951 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/iot-data/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.926326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/iot-jobs-data/
--rw-r--r--   0 runner    (1001) docker     (127)    21019 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/iot-jobs-data/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.926326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/iot1click-devices/
--rw-r--r--   0 runner    (1001) docker     (127)    10682 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/iot1click-devices/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.926326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/iot1click-projects/
--rw-r--r--   0 runner    (1001) docker     (127)    13314 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/iot1click-projects/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.926326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/iotanalytics/
--rw-r--r--   0 runner    (1001) docker     (127)    13626 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/iotanalytics/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.926326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/iotdeviceadvisor/
--rw-r--r--   0 runner    (1001) docker     (127)    12047 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/iotdeviceadvisor/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.926326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/iotevents/
--rw-r--r--   0 runner    (1001) docker     (127)    15723 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/iotevents/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.926326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/iotevents-data/
--rw-r--r--   0 runner    (1001) docker     (127)    10634 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/iotevents-data/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.926326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/iotfleethub/
--rw-r--r--   0 runner    (1001) docker     (127)    17218 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/iotfleethub/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.926326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/iotfleetwise/
--rw-r--r--   0 runner    (1001) docker     (127)    11037 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/iotfleetwise/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.926326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/iotsecuretunneling/
--rw-r--r--   0 runner    (1001) docker     (127)    21179 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/iotsecuretunneling/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.926326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/iotsitewise/
--rw-r--r--   0 runner    (1001) docker     (127)    17087 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/iotsitewise/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.926326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/iotthingsgraph/
--rw-r--r--   0 runner    (1001) docker     (127)    12819 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/iotthingsgraph/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.926326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/iottwinmaker/
--rw-r--r--   0 runner    (1001) docker     (127)    12771 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/iottwinmaker/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.926326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/iotwireless/
--rw-r--r--   0 runner    (1001) docker     (127)    12396 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/iotwireless/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.926326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/ivs/
--rw-r--r--   0 runner    (1001) docker     (127)    13002 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/ivs/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.926326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/ivs-realtime/
--rw-r--r--   0 runner    (1001) docker     (127)    10586 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/ivs-realtime/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.926326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/ivschat/
--rw-r--r--   0 runner    (1001) docker     (127)    11364 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/ivschat/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.926326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/kafka/
--rw-r--r--   0 runner    (1001) docker     (127)    20270 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/kafka/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.926326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/kafkaconnect/
--rw-r--r--   0 runner    (1001) docker     (127)    17076 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/kafkaconnect/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.926326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/kendra/
--rw-r--r--   0 runner    (1001) docker     (127)    14778 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/kendra/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.926326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/kendra-ranking/
--rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/kendra-ranking/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.926326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/keyspaces/
--rw-r--r--   0 runner    (1001) docker     (127)    19121 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/keyspaces/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.930326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/kinesis/
--rw-r--r--   0 runner    (1001) docker     (127)    82124 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/kinesis/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.930326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/kinesis-video-archived-media/
--rw-r--r--   0 runner    (1001) docker     (127)    17076 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/kinesis-video-archived-media/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.930326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/kinesis-video-media/
--rw-r--r--   0 runner    (1001) docker     (127)    17076 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/kinesis-video-media/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.930326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/kinesis-video-signaling/
--rw-r--r--   0 runner    (1001) docker     (127)    17076 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/kinesis-video-signaling/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.930326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/kinesis-video-webrtc-storage/
--rw-r--r--   0 runner    (1001) docker     (127)    10602 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/kinesis-video-webrtc-storage/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.930326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/kinesisanalytics/
--rw-r--r--   0 runner    (1001) docker     (127)    20264 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/kinesisanalytics/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.930326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/kinesisanalyticsv2/
--rw-r--r--   0 runner    (1001) docker     (127)    20264 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/kinesisanalyticsv2/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.930326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/kinesisvideo/
--rw-r--r--   0 runner    (1001) docker     (127)    17076 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/kinesisvideo/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.930326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/kms/
--rw-r--r--   0 runner    (1001) docker     (127)    30432 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/kms/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.930326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/lakeformation/
--rw-r--r--   0 runner    (1001) docker     (127)    21882 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/lakeformation/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.930326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/lambda/
--rw-r--r--   0 runner    (1001) docker     (127)    31675 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/lambda/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.930326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/launch-wizard/
--rw-r--r--   0 runner    (1001) docker     (127)    10977 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/launch-wizard/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.930326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/lex-models/
--rw-r--r--   0 runner    (1001) docker     (127)    14894 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/lex-models/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.930326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/lex-runtime/
--rw-r--r--   0 runner    (1001) docker     (127)    16869 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/lex-runtime/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.930326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/lexv2-models/
--rw-r--r--   0 runner    (1001) docker     (127)    14969 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/lexv2-models/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.930326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/lexv2-runtime/
--rw-r--r--   0 runner    (1001) docker     (127)    14995 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/lexv2-runtime/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.930326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/license-manager/
--rw-r--r--   0 runner    (1001) docker     (127)    22410 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/license-manager/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.930326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/license-manager-linux-subscriptions/
--rw-r--r--   0 runner    (1001) docker     (127)    10970 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/license-manager-linux-subscriptions/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.930326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/license-manager-user-subscriptions/
--rw-r--r--   0 runner    (1001) docker     (127)    10954 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/license-manager-user-subscriptions/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.930326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/lightsail/
--rw-r--r--   0 runner    (1001) docker     (127)    16137 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/lightsail/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.930326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/location/
--rw-r--r--   0 runner    (1001) docker     (127)    10458 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/location/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.930326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/logs/
--rw-r--r--   0 runner    (1001) docker     (127)    22354 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/logs/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.930326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/lookoutequipment/
--rw-r--r--   0 runner    (1001) docker     (127)    11541 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/lookoutequipment/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.930326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/lookoutmetrics/
--rw-r--r--   0 runner    (1001) docker     (127)    14115 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/lookoutmetrics/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.930326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/lookoutvision/
--rw-r--r--   0 runner    (1001) docker     (127)    13219 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/lookoutvision/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.930326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/m2/
--rw-r--r--   0 runner    (1001) docker     (127)    12971 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/m2/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.930326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/machinelearning/
--rw-r--r--   0 runner    (1001) docker     (127)    11079 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/machinelearning/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.930326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/macie2/
--rw-r--r--   0 runner    (1001) docker     (127)    20283 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/macie2/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.930326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/managedblockchain/
--rw-r--r--   0 runner    (1001) docker     (127)    12882 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/managedblockchain/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.930326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/managedblockchain-query/
--rw-r--r--   0 runner    (1001) docker     (127)    10778 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/managedblockchain-query/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.930326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/marketplace-agreement/
--rw-r--r--   0 runner    (1001) docker     (127)    10746 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/marketplace-agreement/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.930326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/marketplace-catalog/
--rw-r--r--   0 runner    (1001) docker     (127)    10714 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/marketplace-catalog/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.930326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/marketplace-deployment/
--rw-r--r--   0 runner    (1001) docker     (127)    10762 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/marketplace-deployment/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.930326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/marketplace-entitlement/
--rw-r--r--   0 runner    (1001) docker     (127)    11233 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/marketplace-entitlement/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.930326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/marketplacecommerceanalytics/
--rw-r--r--   0 runner    (1001) docker     (127)    10858 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/marketplacecommerceanalytics/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.930326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/mediaconnect/
--rw-r--r--   0 runner    (1001) docker     (127)    17067 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/mediaconnect/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.934326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/mediaconvert/
--rw-r--r--   0 runner    (1001) docker     (127)    20124 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/mediaconvert/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.934326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/medialive/
--rw-r--r--   0 runner    (1001) docker     (127)    16980 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/medialive/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.934326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/mediapackage/
--rw-r--r--   0 runner    (1001) docker     (127)    16641 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/mediapackage/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.934326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/mediapackage-vod/
--rw-r--r--   0 runner    (1001) docker     (127)    16761 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/mediapackage-vod/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.934326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/mediapackagev2/
--rw-r--r--   0 runner    (1001) docker     (127)    10634 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/mediapackagev2/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.934326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/mediastore/
--rw-r--r--   0 runner    (1001) docker     (127)    14019 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/mediastore/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.934326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/mediastore-data/
--rw-r--r--   0 runner    (1001) docker     (127)    14139 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/mediastore-data/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.934326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/mediatailor/
--rw-r--r--   0 runner    (1001) docker     (127)    13278 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/mediatailor/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.934326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/medical-imaging/
--rw-r--r--   0 runner    (1001) docker     (127)    10650 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/medical-imaging/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.934326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/memorydb/
--rw-r--r--   0 runner    (1001) docker     (127)    18197 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/memorydb/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.934326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/meteringmarketplace/
--rw-r--r--   0 runner    (1001) docker     (127)    20413 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/meteringmarketplace/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.934326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/mgh/
--rw-r--r--   0 runner    (1001) docker     (127)    13157 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/mgh/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.934326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/mgn/
--rw-r--r--   0 runner    (1001) docker     (127)    18906 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/mgn/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.934326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/migration-hub-refactor-spaces/
--rw-r--r--   0 runner    (1001) docker     (127)    10650 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/migration-hub-refactor-spaces/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.934326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/migrationhub-config/
--rw-r--r--   0 runner    (1001) docker     (127)    10714 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/migrationhub-config/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.934326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/migrationhuborchestrator/
--rw-r--r--   0 runner    (1001) docker     (127)    10810 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/migrationhuborchestrator/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.934326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/migrationhubstrategy/
--rw-r--r--   0 runner    (1001) docker     (127)    13395 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/migrationhubstrategy/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.934326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/mobile/
--rw-r--r--   0 runner    (1001) docker     (127)    10506 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/mobile/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.934326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/mq/
--rw-r--r--   0 runner    (1001) docker     (127)    21851 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/mq/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.934326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/mturk/
--rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/mturk/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.934326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/mwaa/
--rw-r--r--   0 runner    (1001) docker     (127)    16500 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/mwaa/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.934326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/neptune/
--rw-r--r--   0 runner    (1001) docker     (127)    23114 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/neptune/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.934326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/neptune-graph/
--rw-r--r--   0 runner    (1001) docker     (127)    35316 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/neptune-graph/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.934326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/neptunedata/
--rw-r--r--   0 runner    (1001) docker     (127)    10570 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/neptunedata/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.934326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/network-firewall/
--rw-r--r--   0 runner    (1001) docker     (127)    22002 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/network-firewall/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.934326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/networkmanager/
--rw-r--r--   0 runner    (1001) docker     (127)    12964 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/networkmanager/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.934326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/networkmonitor/
--rw-r--r--   0 runner    (1001) docker     (127)    10634 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/networkmonitor/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.934326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/nimble/
--rw-r--r--   0 runner    (1001) docker     (127)    12645 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/nimble/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.934326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/oam/
--rw-r--r--   0 runner    (1001) docker     (127)    10458 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/oam/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.934326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/omics/
--rw-r--r--   0 runner    (1001) docker     (127)    10490 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/omics/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.934326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/opensearch/
--rw-r--r--   0 runner    (1001) docker     (127)    22279 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/opensearch/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.934326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/opensearchserverless/
--rw-r--r--   0 runner    (1001) docker     (127)    10849 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/opensearchserverless/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.934326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/opsworks/
--rw-r--r--   0 runner    (1001) docker     (127)    16527 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/opsworks/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.934326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/opsworkscm/
--rw-r--r--   0 runner    (1001) docker     (127)    14040 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/opsworkscm/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.934326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/organizations/
--rw-r--r--   0 runner    (1001) docker     (127)    17605 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/organizations/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.934326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/osis/
--rw-r--r--   0 runner    (1001) docker     (127)    10474 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/osis/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.938326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/outposts/
--rw-r--r--   0 runner    (1001) docker     (127)    21656 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/outposts/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.938326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/panorama/
--rw-r--r--   0 runner    (1001) docker     (127)    10538 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/panorama/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.938326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/payment-cryptography/
--rw-r--r--   0 runner    (1001) docker     (127)    10938 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/payment-cryptography/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.938326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/payment-cryptography-data/
--rw-r--r--   0 runner    (1001) docker     (127)    10890 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/payment-cryptography-data/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.938326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/pca-connector-ad/
--rw-r--r--   0 runner    (1001) docker     (127)    10666 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/pca-connector-ad/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.938326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/personalize/
--rw-r--r--   0 runner    (1001) docker     (127)    14917 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/personalize/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.938326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/personalize-events/
--rw-r--r--   0 runner    (1001) docker     (127)    10698 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/personalize-events/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.938326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/personalize-runtime/
--rw-r--r--   0 runner    (1001) docker     (127)    10714 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/personalize-runtime/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.938326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/pi/
--rw-r--r--   0 runner    (1001) docker     (127)    19304 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/pi/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.938326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/pinpoint/
--rw-r--r--   0 runner    (1001) docker     (127)    16135 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/pinpoint/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.938326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/pinpoint-email/
--rw-r--r--   0 runner    (1001) docker     (127)    19846 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/pinpoint-email/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.938326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/pinpoint-sms-voice/
--rw-r--r--   0 runner    (1001) docker     (127)    10081 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/pinpoint-sms-voice/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.938326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/pinpoint-sms-voice-v2/
--rw-r--r--   0 runner    (1001) docker     (127)    14862 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/pinpoint-sms-voice-v2/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.938326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/pipes/
--rw-r--r--   0 runner    (1001) docker     (127)    10490 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/pipes/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.938326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/polly/
--rw-r--r--   0 runner    (1001) docker     (127)    20690 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/polly/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.938326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/pricing/
--rw-r--r--   0 runner    (1001) docker     (127)    11014 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/pricing/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.938326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/privatenetworks/
--rw-r--r--   0 runner    (1001) docker     (127)    10666 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/privatenetworks/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.938326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/proton/
--rw-r--r--   0 runner    (1001) docker     (127)    12201 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/proton/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.938326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/qbusiness/
--rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/qbusiness/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.938326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/qconnect/
--rw-r--r--   0 runner    (1001) docker     (127)    10506 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/qconnect/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.938326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/qldb/
--rw-r--r--   0 runner    (1001) docker     (127)    16004 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/qldb/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.938326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/qldb-session/
--rw-r--r--   0 runner    (1001) docker     (127)    15798 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/qldb-session/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.938326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/quicksight/
--rw-r--r--   0 runner    (1001) docker     (127)    16987 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/quicksight/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.938326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/ram/
--rw-r--r--   0 runner    (1001) docker     (127)    22313 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/ram/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.938326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/rbin/
--rw-r--r--   0 runner    (1001) docker     (127)    18942 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/rbin/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.938326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/rds/
--rw-r--r--   0 runner    (1001) docker     (127)    22739 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/rds/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.938326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/rds-data/
--rw-r--r--   0 runner    (1001) docker     (127)    10538 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/rds-data/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.938326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/redshift/
--rw-r--r--   0 runner    (1001) docker     (127)    22964 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/redshift/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.938326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/redshift-data/
--rw-r--r--   0 runner    (1001) docker     (127)    10618 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/redshift-data/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.938326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/redshift-serverless/
--rw-r--r--   0 runner    (1001) docker     (127)    15116 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/redshift-serverless/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.938326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/rekognition/
--rw-r--r--   0 runner    (1001) docker     (127)    18365 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/rekognition/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.938326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/repostspace/
--rw-r--r--   0 runner    (1001) docker     (127)    10586 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/repostspace/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.938326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/resiliencehub/
--rw-r--r--   0 runner    (1001) docker     (127)    18824 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/resiliencehub/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.938326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/resource-explorer-2/
--rw-r--r--   0 runner    (1001) docker     (127)    10714 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/resource-explorer-2/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.938326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/resource-groups/
--rw-r--r--   0 runner    (1001) docker     (127)    22400 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/resource-groups/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.938326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/resourcegroupstaggingapi/
--rw-r--r--   0 runner    (1001) docker     (127)    20358 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/resourcegroupstaggingapi/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.942326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/robomaker/
--rw-r--r--   0 runner    (1001) docker     (127)    13566 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/robomaker/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.942326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/rolesanywhere/
--rw-r--r--   0 runner    (1001) docker     (127)    18406 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/rolesanywhere/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.942326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/route53/
--rw-r--r--   0 runner    (1001) docker     (127)    19968 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/route53/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.942326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/route53-recovery-cluster/
--rw-r--r--   0 runner    (1001) docker     (127)    10794 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/route53-recovery-cluster/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.942326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/route53-recovery-control-config/
--rw-r--r--   0 runner    (1001) docker     (127)    11731 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/route53-recovery-control-config/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.942326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/route53-recovery-readiness/
--rw-r--r--   0 runner    (1001) docker     (127)    10826 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/route53-recovery-readiness/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.942326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/route53domains/
--rw-r--r--   0 runner    (1001) docker     (127)    10634 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/route53domains/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.942326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/route53profiles/
--rw-r--r--   0 runner    (1001) docker     (127)    10650 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/route53profiles/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.942326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/route53resolver/
--rw-r--r--   0 runner    (1001) docker     (127)    21104 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/route53resolver/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.942326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/rum/
--rw-r--r--   0 runner    (1001) docker     (127)    14268 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/rum/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.942326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/s3/
--rw-r--r--   0 runner    (1001) docker     (127)   321152 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/s3/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.942326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/s3control/
--rw-r--r--   0 runner    (1001) docker     (127)   148079 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/s3control/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.942326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/s3outposts/
--rw-r--r--   0 runner    (1001) docker     (127)    19194 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/s3outposts/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.942326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/sagemaker/
--rw-r--r--   0 runner    (1001) docker     (127)    21872 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/sagemaker/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.942326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/sagemaker-a2i-runtime/
--rw-r--r--   0 runner    (1001) docker     (127)    10746 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/sagemaker-a2i-runtime/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.942326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/sagemaker-edge/
--rw-r--r--   0 runner    (1001) docker     (127)    12798 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/sagemaker-edge/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.942326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/sagemaker-featurestore-runtime/
--rw-r--r--   0 runner    (1001) docker     (127)    10890 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/sagemaker-featurestore-runtime/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.942326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/sagemaker-geospatial/
--rw-r--r--   0 runner    (1001) docker     (127)    10730 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/sagemaker-geospatial/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.942326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/sagemaker-metrics/
--rw-r--r--   0 runner    (1001) docker     (127)    10682 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/sagemaker-metrics/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.942326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/sagemaker-runtime/
--rw-r--r--   0 runner    (1001) docker     (127)    22040 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/sagemaker-runtime/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.942326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/savingsplans/
--rw-r--r--   0 runner    (1001) docker     (127)    11728 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/savingsplans/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.942326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/scheduler/
--rw-r--r--   0 runner    (1001) docker     (127)    10554 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/scheduler/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.942326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    17342 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/schemas/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.942326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/sdb/
--rw-r--r--   0 runner    (1001) docker     (127)    14829 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/sdb/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.942326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/secretsmanager/
--rw-r--r--   0 runner    (1001) docker     (127)    22819 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/secretsmanager/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.942326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/securityhub/
--rw-r--r--   0 runner    (1001) docker     (127)    22238 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/securityhub/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.942326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/securitylake/
--rw-r--r--   0 runner    (1001) docker     (127)    10602 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/securitylake/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.942326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/serverlessrepo/
--rw-r--r--   0 runner    (1001) docker     (127)    19316 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/serverlessrepo/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.942326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/service-quotas/
--rw-r--r--   0 runner    (1001) docker     (127)    20579 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/service-quotas/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.942326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/servicecatalog/
--rw-r--r--   0 runner    (1001) docker     (127)    22367 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/servicecatalog/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.942326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/servicecatalog-appregistry/
--rw-r--r--   0 runner    (1001) docker     (127)    22417 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/servicecatalog-appregistry/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.946326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/servicediscovery/
--rw-r--r--   0 runner    (1001) docker     (127)    22005 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/servicediscovery/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.946326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/ses/
--rw-r--r--   0 runner    (1001) docker     (127)    19846 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/ses/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.946326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/sesv2/
--rw-r--r--   0 runner    (1001) docker     (127)    19846 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/sesv2/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.946326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/shield/
--rw-r--r--   0 runner    (1001) docker     (127)    12765 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/shield/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.946326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/signer/
--rw-r--r--   0 runner    (1001) docker     (127)    10506 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/signer/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.946326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/simspaceweaver/
--rw-r--r--   0 runner    (1001) docker     (127)    10634 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/simspaceweaver/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.946326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/sms/
--rw-r--r--   0 runner    (1001) docker     (127)    21030 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/sms/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.946326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/sms-voice/
--rw-r--r--   0 runner    (1001) docker     (127)    10081 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/sms-voice/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.946326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/snow-device-management/
--rw-r--r--   0 runner    (1001) docker     (127)    10762 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/snow-device-management/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.946326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/snowball/
--rw-r--r--   0 runner    (1001) docker     (127)    26886 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/snowball/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.946326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/sns/
--rw-r--r--   0 runner    (1001) docker     (127)    22310 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/sns/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.946326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/sqs/
--rw-r--r--   0 runner    (1001) docker     (127)    21883 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/sqs/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.946326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/ssm/
--rw-r--r--   0 runner    (1001) docker     (127)    22313 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/ssm/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.946326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/ssm-contacts/
--rw-r--r--   0 runner    (1001) docker     (127)    10602 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/ssm-contacts/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.946326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/ssm-incidents/
--rw-r--r--   0 runner    (1001) docker     (127)    17107 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/ssm-incidents/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.946326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/ssm-sap/
--rw-r--r--   0 runner    (1001) docker     (127)    10522 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/ssm-sap/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.946326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/sso/
--rw-r--r--   0 runner    (1001) docker     (127)    18738 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/sso/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.946326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/sso-admin/
--rw-r--r--   0 runner    (1001) docker     (127)    18920 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/sso-admin/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.946326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/sso-oidc/
--rw-r--r--   0 runner    (1001) docker     (127)    18528 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/sso-oidc/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.946326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/stepfunctions/
--rw-r--r--   0 runner    (1001) docker     (127)    22447 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/stepfunctions/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.946326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/storagegateway/
--rw-r--r--   0 runner    (1001) docker     (127)    22807 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/storagegateway/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.946326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/sts/
--rw-r--r--   0 runner    (1001) docker     (127)    43190 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/sts/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.946326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/supplychain/
--rw-r--r--   0 runner    (1001) docker     (127)    10458 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/supplychain/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.946326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/support/
--rw-r--r--   0 runner    (1001) docker     (127)    17409 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/support/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.946326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/support-app/
--rw-r--r--   0 runner    (1001) docker     (127)    10570 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/support-app/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.946326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/swf/
--rw-r--r--   0 runner    (1001) docker     (127)    22310 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/swf/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.946326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/synthetics/
--rw-r--r--   0 runner    (1001) docker     (127)    22195 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/synthetics/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.946326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/textract/
--rw-r--r--   0 runner    (1001) docker     (127)    18248 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/textract/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.946326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/timestream-influxdb/
--rw-r--r--   0 runner    (1001) docker     (127)    10714 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/timestream-influxdb/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.946326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/timestream-query/
--rw-r--r--   0 runner    (1001) docker     (127)    10666 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/timestream-query/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.946326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/timestream-write/
--rw-r--r--   0 runner    (1001) docker     (127)    11561 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/timestream-write/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.946326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/tnb/
--rw-r--r--   0 runner    (1001) docker     (127)    10458 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/tnb/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.946326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/transcribe/
--rw-r--r--   0 runner    (1001) docker     (127)    21332 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/transcribe/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.946326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/transfer/
--rw-r--r--   0 runner    (1001) docker     (127)    22106 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/transfer/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.946326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/translate/
--rw-r--r--   0 runner    (1001) docker     (127)    18708 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/translate/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.946326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/trustedadvisor/
--rw-r--r--   0 runner    (1001) docker     (127)    10634 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/trustedadvisor/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.950326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/verifiedpermissions/
--rw-r--r--   0 runner    (1001) docker     (127)    10714 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/verifiedpermissions/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.950326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/voice-id/
--rw-r--r--   0 runner    (1001) docker     (127)    13102 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/voice-id/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.950326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/vpc-lattice/
--rw-r--r--   0 runner    (1001) docker     (127)    10586 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/vpc-lattice/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.950326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/waf/
--rw-r--r--   0 runner    (1001) docker     (127)    12659 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/waf/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.950326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/waf-regional/
--rw-r--r--   0 runner    (1001) docker     (127)    30573 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/waf-regional/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.950326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/wafv2/
--rw-r--r--   0 runner    (1001) docker     (127)    30139 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/wafv2/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.950326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/wellarchitected/
--rw-r--r--   0 runner    (1001) docker     (127)    18030 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/wellarchitected/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.950326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/wisdom/
--rw-r--r--   0 runner    (1001) docker     (127)    12645 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/wisdom/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.950326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/workdocs/
--rw-r--r--   0 runner    (1001) docker     (127)    13118 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/workdocs/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.950326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/worklink/
--rw-r--r--   0 runner    (1001) docker     (127)    10538 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/worklink/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.950326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/workmail/
--rw-r--r--   0 runner    (1001) docker     (127)    11382 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/workmail/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.950326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/workmailmessageflow/
--rw-r--r--   0 runner    (1001) docker     (127)    10714 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/workmailmessageflow/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.950326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/workspaces/
--rw-r--r--   0 runner    (1001) docker     (127)    17059 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/workspaces/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.950326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/workspaces-thin-client/
--rw-r--r--   0 runner    (1001) docker     (127)    10570 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/workspaces-thin-client/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.950326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/workspaces-web/
--rw-r--r--   0 runner    (1001) docker     (127)    11490 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/workspaces-web/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.950326 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/xray/
--rw-r--r--   0 runner    (1001) docker     (127)    21937 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/xray/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.950326 botocore-a-la-carte-1.34.98/tests/functional/leak/
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/leak/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/leak/test_resource_leaks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.950326 botocore-a-la-carte-1.34.98/tests/functional/models/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.874326 botocore-a-la-carte-1.34.98/tests/functional/models/custom-acm/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.950326 botocore-a-la-carte-1.34.98/tests/functional/models/custom-acm/2015-12-08/
--rw-r--r--   0 runner    (1001) docker     (127)    14695 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/models/custom-acm/2015-12-08/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/models/custom-acm/2015-12-08/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/models/custom-acm/2015-12-08/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (127)    57976 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/models/custom-acm/2015-12-08/service-2.json
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/models/custom-acm/2015-12-08/waiters-2.json
--rw-r--r--   0 runner    (1001) docker     (127)    77688 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/models/endpoints.json
--rw-r--r--   0 runner    (1001) docker     (127)     4358 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/models/sdk-default-configuration.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.874326 botocore-a-la-carte-1.34.98/tests/functional/models/test-discovery-endpoint/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.950326 botocore-a-la-carte-1.34.98/tests/functional/models/test-discovery-endpoint/2020-08-20/
--rw-r--r--   0 runner    (1001) docker     (127)     4677 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/models/test-discovery-endpoint/2020-08-20/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.950326 botocore-a-la-carte-1.34.98/tests/functional/retries/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/retries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3928 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/retries/test_bucket.py
--rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/retries/test_quota.py
--rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/test_alias.py
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/test_apigateway.py
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/test_client_class_names.py
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/test_client_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/test_cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/test_cloudsearchdomain.py
--rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/test_cognito_idp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/test_compress.py
--rw-r--r--   0 runner    (1001) docker     (127)     4831 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/test_config_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)    19034 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/test_context_params.py
--rw-r--r--   0 runner    (1001) docker     (127)    44807 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    16098 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/test_discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/test_docdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/test_dynamodb.py
--rw-r--r--   0 runner    (1001) docker     (127)     5692 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/test_ec2.py
--rw-r--r--   0 runner    (1001) docker     (127)    11682 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/test_endpoint_rulesets.py
--rw-r--r--   0 runner    (1001) docker     (127)     4841 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/test_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)    14597 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/test_event_alias.py
--rw-r--r--   0 runner    (1001) docker     (127)    12116 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/test_eventbridge.py
--rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/test_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/test_h2_required.py
--rw-r--r--   0 runner    (1001) docker     (127)     5235 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/test_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/test_importexport.py
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/test_iot_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/test_kinesis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/test_lex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/test_loaders.py
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/test_machinelearning.py
--rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/test_model_backcompat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/test_model_completeness.py
--rw-r--r--   0 runner    (1001) docker     (127)     6769 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/test_modeled_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/test_mturk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/test_neptune.py
--rw-r--r--   0 runner    (1001) docker     (127)     8288 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/test_paginate.py
--rw-r--r--   0 runner    (1001) docker     (127)    11866 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/test_paginator_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/test_public_apis.py
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/test_qbusiness.py
--rw-r--r--   0 runner    (1001) docker     (127)     4117 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/test_rds.py
--rw-r--r--   0 runner    (1001) docker     (127)    28286 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/test_regions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/test_response_shadowing.py
--rw-r--r--   0 runner    (1001) docker     (127)    14043 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/test_retry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/test_route53.py
--rw-r--r--   0 runner    (1001) docker     (127)   133985 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/test_s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/test_s3_control.py
--rw-r--r--   0 runner    (1001) docker     (127)    18188 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/test_s3_control_redirects.py
--rw-r--r--   0 runner    (1001) docker     (127)    11135 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/test_s3express.py
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/test_sagemaker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/test_service_alias.py
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/test_service_names.py
--rw-r--r--   0 runner    (1001) docker     (127)     4558 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/test_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/test_six_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/test_six_threading.py
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/test_sqs.py
--rw-r--r--   0 runner    (1001) docker     (127)    12521 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/test_sts.py
--rw-r--r--   0 runner    (1001) docker     (127)    14292 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/test_stub.py
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/test_tagged_unions_unknown.py
--rw-r--r--   0 runner    (1001) docker     (127)    11554 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/test_useragent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7380 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/test_waiter_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.950326 botocore-a-la-carte-1.34.98/tests/functional/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/functional/utils/credentialprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.954326 botocore-a-la-carte-1.34.98/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/integration/test-credentials
--rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/integration/test_apigateway.py
--rw-r--r--   0 runner    (1001) docker     (127)     6452 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/integration/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    10489 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/integration/test_client_http.py
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/integration/test_cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/integration/test_cognito_identity.py
--rw-r--r--   0 runner    (1001) docker     (127)    14122 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/integration/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/integration/test_ec2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/integration/test_elastictranscoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/integration/test_emr.py
--rw-r--r--   0 runner    (1001) docker     (127)     3038 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/integration/test_glacier.py
--rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/integration/test_loaders.py
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/integration/test_rds.py
--rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/integration/test_route53.py
--rw-r--r--   0 runner    (1001) docker     (127)    53990 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/integration/test_s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/integration/test_session.py
--rw-r--r--   0 runner    (1001) docker     (127)    12697 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/integration/test_smoke.py
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/integration/test_sts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/integration/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/integration/test_waiters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.958326 botocore-a-la-carte-1.34.98/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.958326 botocore-a-la-carte-1.34.98/tests/unit/auth/
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.958326 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/NOTICE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.962326 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-header-key-duplicate/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-header-key-duplicate/get-header-key-duplicate.authz
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-header-key-duplicate/get-header-key-duplicate.creq
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-header-key-duplicate/get-header-key-duplicate.req
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-header-key-duplicate/get-header-key-duplicate.sreq
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-header-key-duplicate/get-header-key-duplicate.sts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.962326 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-header-value-multiline/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-header-value-multiline/get-header-value-multiline.authz
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-header-value-multiline/get-header-value-multiline.creq
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-header-value-multiline/get-header-value-multiline.req
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-header-value-multiline/get-header-value-multiline.sreq
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-header-value-multiline/get-header-value-multiline.sts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.962326 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-header-value-order/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-header-value-order/get-header-value-order.authz
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-header-value-order/get-header-value-order.creq
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-header-value-order/get-header-value-order.req
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-header-value-order/get-header-value-order.sreq
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-header-value-order/get-header-value-order.sts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.962326 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-header-value-trim/
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-header-value-trim/get-header-value-trim.authz
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-header-value-trim/get-header-value-trim.creq
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-header-value-trim/get-header-value-trim.req
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-header-value-trim/get-header-value-trim.sreq
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-header-value-trim/get-header-value-trim.sts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.962326 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-unreserved/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-unreserved/get-unreserved.authz
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-unreserved/get-unreserved.creq
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-unreserved/get-unreserved.req
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-unreserved/get-unreserved.sreq
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-unreserved/get-unreserved.sts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.962326 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-utf8/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-utf8/get-utf8.authz
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-utf8/get-utf8.creq
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-utf8/get-utf8.req
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-utf8/get-utf8.sreq
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-utf8/get-utf8.sts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.962326 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-vanilla/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-vanilla/get-vanilla.authz
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-vanilla/get-vanilla.creq
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-vanilla/get-vanilla.req
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-vanilla/get-vanilla.sreq
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-vanilla/get-vanilla.sts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.962326 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-vanilla-empty-query-key/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-vanilla-empty-query-key/get-vanilla-empty-query-key.authz
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-vanilla-empty-query-key/get-vanilla-empty-query-key.creq
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-vanilla-empty-query-key/get-vanilla-empty-query-key.req
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-vanilla-empty-query-key/get-vanilla-empty-query-key.sreq
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-vanilla-empty-query-key/get-vanilla-empty-query-key.sts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.962326 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-vanilla-query/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-vanilla-query/get-vanilla-query.authz
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-vanilla-query/get-vanilla-query.creq
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-vanilla-query/get-vanilla-query.req
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-vanilla-query/get-vanilla-query.sreq
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-vanilla-query/get-vanilla-query.sts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.966326 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-encoded/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-encoded/get-vanilla-query-order-encoded.authz
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-encoded/get-vanilla-query-order-encoded.creq
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-encoded/get-vanilla-query-order-encoded.req
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-encoded/get-vanilla-query-order-encoded.sreq
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-encoded/get-vanilla-query-order-encoded.sts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.966326 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-key/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-key/get-vanilla-query-order-key.authz
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-key/get-vanilla-query-order-key.creq
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-key/get-vanilla-query-order-key.req
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-key/get-vanilla-query-order-key.sreq
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-key/get-vanilla-query-order-key.sts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.966326 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-key-case/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-key-case/get-vanilla-query-order-key-case.authz
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-key-case/get-vanilla-query-order-key-case.creq
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-key-case/get-vanilla-query-order-key-case.req
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-key-case/get-vanilla-query-order-key-case.sreq
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-key-case/get-vanilla-query-order-key-case.sts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.966326 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-value/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-value/get-vanilla-query-order-value.authz
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-value/get-vanilla-query-order-value.creq
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-value/get-vanilla-query-order-value.req
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-value/get-vanilla-query-order-value.sreq
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-value/get-vanilla-query-order-value.sts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.966326 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-vanilla-query-unreserved/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-vanilla-query-unreserved/get-vanilla-query-unreserved.authz
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-vanilla-query-unreserved/get-vanilla-query-unreserved.creq
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-vanilla-query-unreserved/get-vanilla-query-unreserved.req
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-vanilla-query-unreserved/get-vanilla-query-unreserved.sreq
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-vanilla-query-unreserved/get-vanilla-query-unreserved.sts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.966326 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-vanilla-utf8-query/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-vanilla-utf8-query/get-vanilla-utf8-query.authz
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-vanilla-utf8-query/get-vanilla-utf8-query.creq
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-vanilla-utf8-query/get-vanilla-utf8-query.req
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-vanilla-utf8-query/get-vanilla-utf8-query.sreq
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-vanilla-utf8-query/get-vanilla-utf8-query.sts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.966326 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-vanilla-with-session-token/
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-vanilla-with-session-token/get-vanilla-with-session-token.authz
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-vanilla-with-session-token/get-vanilla-with-session-token.creq
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-vanilla-with-session-token/get-vanilla-with-session-token.req
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-vanilla-with-session-token/get-vanilla-with-session-token.sreq
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/get-vanilla-with-session-token/get-vanilla-with-session-token.sts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.966326 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/normalize-path/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.966326 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/normalize-path/get-relative/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/normalize-path/get-relative/get-relative.authz
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/normalize-path/get-relative/get-relative.creq
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/normalize-path/get-relative/get-relative.req
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/normalize-path/get-relative/get-relative.sreq
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/normalize-path/get-relative/get-relative.sts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.970327 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/normalize-path/get-relative-relative/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/normalize-path/get-relative-relative/get-relative-relative.authz
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/normalize-path/get-relative-relative/get-relative-relative.creq
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/normalize-path/get-relative-relative/get-relative-relative.req
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/normalize-path/get-relative-relative/get-relative-relative.sreq
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/normalize-path/get-relative-relative/get-relative-relative.sts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.970327 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/normalize-path/get-slash/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/normalize-path/get-slash/get-slash.authz
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/normalize-path/get-slash/get-slash.creq
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/normalize-path/get-slash/get-slash.req
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/normalize-path/get-slash/get-slash.sreq
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/normalize-path/get-slash/get-slash.sts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.970327 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/normalize-path/get-slash-dot-slash/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/normalize-path/get-slash-dot-slash/get-slash-dot-slash.authz
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/normalize-path/get-slash-dot-slash/get-slash-dot-slash.creq
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/normalize-path/get-slash-dot-slash/get-slash-dot-slash.req
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/normalize-path/get-slash-dot-slash/get-slash-dot-slash.sreq
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/normalize-path/get-slash-dot-slash/get-slash-dot-slash.sts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.970327 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/normalize-path/get-slash-pointless-dot/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/normalize-path/get-slash-pointless-dot/get-slash-pointless-dot.authz
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/normalize-path/get-slash-pointless-dot/get-slash-pointless-dot.creq
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/normalize-path/get-slash-pointless-dot/get-slash-pointless-dot.req
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/normalize-path/get-slash-pointless-dot/get-slash-pointless-dot.sreq
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/normalize-path/get-slash-pointless-dot/get-slash-pointless-dot.sts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.970327 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/normalize-path/get-slashes/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/normalize-path/get-slashes/get-slashes.authz
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/normalize-path/get-slashes/get-slashes.creq
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/normalize-path/get-slashes/get-slashes.req
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/normalize-path/get-slashes/get-slashes.sreq
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/normalize-path/get-slashes/get-slashes.sts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.970327 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/normalize-path/get-space/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/normalize-path/get-space/get-space.authz
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/normalize-path/get-space/get-space.creq
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/normalize-path/get-space/get-space.req
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/normalize-path/get-space/get-space.sreq
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/normalize-path/get-space/get-space.sts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.970327 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/normalize-path/get-special-character/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/normalize-path/get-special-character/get-special-character.authz
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/normalize-path/get-special-character/get-special-character.creq
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/normalize-path/get-special-character/get-special-character.req
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/normalize-path/get-special-character/get-special-character.sreq
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/normalize-path/get-special-character/get-special-character.sts
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/normalize-path/normalize-path.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.970327 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/post-header-key-case/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/post-header-key-case/post-header-key-case.authz
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/post-header-key-case/post-header-key-case.creq
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/post-header-key-case/post-header-key-case.req
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/post-header-key-case/post-header-key-case.sreq
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/post-header-key-case/post-header-key-case.sts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.970327 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/post-header-key-sort/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/post-header-key-sort/post-header-key-sort.authz
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/post-header-key-sort/post-header-key-sort.creq
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/post-header-key-sort/post-header-key-sort.req
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/post-header-key-sort/post-header-key-sort.sreq
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/post-header-key-sort/post-header-key-sort.sts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.974326 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/post-header-value-case/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/post-header-value-case/post-header-value-case.authz
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/post-header-value-case/post-header-value-case.creq
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/post-header-value-case/post-header-value-case.req
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/post-header-value-case/post-header-value-case.sreq
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/post-header-value-case/post-header-value-case.sts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.974326 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/post-sts-token/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.974326 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/post-sts-token/post-sts-header-after/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/post-sts-token/post-sts-header-after/post-sts-header-after.authz
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/post-sts-token/post-sts-header-after/post-sts-header-after.creq
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/post-sts-token/post-sts-header-after/post-sts-header-after.req
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/post-sts-token/post-sts-header-after/post-sts-header-after.sreq
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/post-sts-token/post-sts-header-after/post-sts-header-after.sts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.974326 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/post-sts-token/post-sts-header-before/
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/post-sts-token/post-sts-header-before/post-sts-header-before.authz
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/post-sts-token/post-sts-header-before/post-sts-header-before.creq
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/post-sts-token/post-sts-header-before/post-sts-header-before.req
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/post-sts-token/post-sts-header-before/post-sts-header-before.sreq
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/post-sts-token/post-sts-header-before/post-sts-header-before.sts
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/post-sts-token/readme.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.974326 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/post-vanilla/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/post-vanilla/post-vanilla.authz
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/post-vanilla/post-vanilla.creq
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/post-vanilla/post-vanilla.req
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/post-vanilla/post-vanilla.sreq
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/post-vanilla/post-vanilla.sts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.974326 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/post-vanilla-empty-query-value/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/post-vanilla-empty-query-value/post-vanilla-empty-query-value.authz
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/post-vanilla-empty-query-value/post-vanilla-empty-query-value.creq
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/post-vanilla-empty-query-value/post-vanilla-empty-query-value.req
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/post-vanilla-empty-query-value/post-vanilla-empty-query-value.sreq
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/post-vanilla-empty-query-value/post-vanilla-empty-query-value.sts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.974326 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/post-vanilla-query/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/post-vanilla-query/post-vanilla-query.authz
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/post-vanilla-query/post-vanilla-query.creq
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/post-vanilla-query/post-vanilla-query.req
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/post-vanilla-query/post-vanilla-query.sreq
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/post-vanilla-query/post-vanilla-query.sts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.974326 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/post-x-www-form-urlencoded/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/post-x-www-form-urlencoded/post-x-www-form-urlencoded.authz
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/post-x-www-form-urlencoded/post-x-www-form-urlencoded.creq
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/post-x-www-form-urlencoded/post-x-www-form-urlencoded.req
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/post-x-www-form-urlencoded/post-x-www-form-urlencoded.sreq
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/post-x-www-form-urlencoded/post-x-www-form-urlencoded.sts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.974326 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/post-x-www-form-urlencoded-parameters/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/post-x-www-form-urlencoded-parameters/post-x-www-form-urlencoded-parameters.authz
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/post-x-www-form-urlencoded-parameters/post-x-www-form-urlencoded-parameters.creq
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/post-x-www-form-urlencoded-parameters/post-x-www-form-urlencoded-parameters.req
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/post-x-www-form-urlencoded-parameters/post-x-www-form-urlencoded-parameters.sreq
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/post-x-www-form-urlencoded-parameters/post-x-www-form-urlencoded-parameters.sts
--rw-r--r--   0 runner    (1001) docker     (127)    45993 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/test_signers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6559 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/auth/test_sigv4.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.978326 botocore-a-la-carte-1.34.98/tests/unit/cfg/
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/cfg/aws_bad_profile
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/cfg/aws_config
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/cfg/aws_config_bad
--rw-r--r--   0 runner    (1001) docker     (127)    51200 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/cfg/aws_config_badbytes
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/cfg/aws_config_nested
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/cfg/aws_config_nested_bad
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/cfg/aws_config_nocreds
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/cfg/aws_config_other
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/cfg/aws_credentials
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/cfg/aws_services_config
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/cfg/aws_sso_session_config
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/cfg/aws_third_config
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/cfg/boto_config
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/cfg/boto_config_empty
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/cfg/foo_config
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.978326 botocore-a-la-carte-1.34.98/tests/unit/crt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/crt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.978326 botocore-a-la-carte-1.34.98/tests/unit/crt/auth/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/crt/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/crt/auth/test_crt_signers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/crt/auth/test_crt_sigv4.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.978326 botocore-a-la-carte-1.34.98/tests/unit/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.878326 botocore-a-la-carte-1.34.98/tests/unit/data/aws/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.978326 botocore-a-la-carte-1.34.98/tests/unit/data/aws/s3/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/data/aws/s3/2006-03-01.normal.json
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/data/baz.json
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/data/compressed.json.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.878326 botocore-a-la-carte-1.34.98/tests/unit/data/endpoints/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.978326 botocore-a-la-carte-1.34.98/tests/unit/data/endpoints/test-cases/
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/data/endpoints/test-cases/aws-region.json
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/data/endpoints/test-cases/default-values.json
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/data/endpoints/test-cases/eventbridge.json
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/data/endpoints/test-cases/fns.json
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/data/endpoints/test-cases/headers.json
--rw-r--r--   0 runner    (1001) docker     (127)     3725 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/data/endpoints/test-cases/is-virtual-hostable-s3-bucket.json
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/data/endpoints/test-cases/local-region-override.json
--rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/data/endpoints/test-cases/parse-arn.json
--rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/data/endpoints/test-cases/parse-url.json
--rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/data/endpoints/test-cases/partition-fn.json
--rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/data/endpoints/test-cases/substring.json
--rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/data/endpoints/test-cases/uri-encode.json
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/data/endpoints/test-cases/valid-hostlabel.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.982327 botocore-a-la-carte-1.34.98/tests/unit/data/endpoints/valid-rules/
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/data/endpoints/valid-rules/aws-region.json
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/data/endpoints/valid-rules/default-values.json
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/data/endpoints/valid-rules/deprecated-param.json
--rw-r--r--   0 runner    (1001) docker     (127)     8502 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/data/endpoints/valid-rules/eventbridge.json
--rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/data/endpoints/valid-rules/fns.json
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/data/endpoints/valid-rules/get-attr-type-inference.json
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/data/endpoints/valid-rules/headers.json
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/data/endpoints/valid-rules/is-virtual-hostable-s3-bucket.json
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/data/endpoints/valid-rules/local-region-override.json
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/data/endpoints/valid-rules/minimal-ruleset.json
--rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/data/endpoints/valid-rules/parse-arn.json
--rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/data/endpoints/valid-rules/parse-url.json
--rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/data/endpoints/valid-rules/partition-fn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/data/endpoints/valid-rules/substring.json
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/data/endpoints/valid-rules/uri-encode.json
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/data/endpoints/valid-rules/valid-hostlabel.json
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/data/foo.json
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/data/non_ascii.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.982327 botocore-a-la-carte-1.34.98/tests/unit/data/someservice/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/data/someservice/2012-10-01.normal.json
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/data/someservice/2013-08-21.normal.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.982327 botocore-a-la-carte-1.34.98/tests/unit/data/sub/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/data/sub/fie.normal.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.878326 botocore-a-la-carte-1.34.98/tests/unit/data_overrides/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.982327 botocore-a-la-carte-1.34.98/tests/unit/data_overrides/someservice/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/data_overrides/someservice/2012-10-01.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.982327 botocore-a-la-carte-1.34.98/tests/unit/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     9486 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/docs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.982327 botocore-a-la-carte-1.34.98/tests/unit/docs/bcdoc/
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/docs/bcdoc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13206 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/docs/bcdoc/test_docstringparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     6294 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/docs/bcdoc/test_document.py
--rw-r--r--   0 runner    (1001) docker     (127)    12421 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/docs/bcdoc/test_style.py
--rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/docs/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/docs/test_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/docs/test_docstring.py
--rw-r--r--   0 runner    (1001) docker     (127)    16138 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/docs/test_example.py
--rw-r--r--   0 runner    (1001) docker     (127)    15898 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/docs/test_method.py
--rw-r--r--   0 runner    (1001) docker     (127)     4110 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/docs/test_paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    13495 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/docs/test_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     4833 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/docs/test_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     8454 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/docs/test_sharedexample.py
--rw-r--r--   0 runner    (1001) docker     (127)     8470 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/docs/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/docs/test_waiter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.878326 botocore-a-la-carte-1.34.98/tests/unit/protocols/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.986327 botocore-a-la-carte-1.34.98/tests/unit/protocols/input/
--rw-r--r--   0 runner    (1001) docker     (127)    12019 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/protocols/input/ec2.json
--rw-r--r--   0 runner    (1001) docker     (127)    21711 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/protocols/input/json.json
--rw-r--r--   0 runner    (1001) docker     (127)    23390 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/protocols/input/query.json
--rw-r--r--   0 runner    (1001) docker     (127)    51262 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/protocols/input/rest-json.json
--rw-r--r--   0 runner    (1001) docker     (127)    46773 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/protocols/input/rest-xml.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.986327 botocore-a-la-carte-1.34.98/tests/unit/protocols/output/
--rw-r--r--   0 runner    (1001) docker     (127)    14002 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/protocols/output/ec2.json
--rw-r--r--   0 runner    (1001) docker     (127)    19354 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/protocols/output/json.json
--rw-r--r--   0 runner    (1001) docker     (127)    23397 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/protocols/output/query.json
--rw-r--r--   0 runner    (1001) docker     (127)    29610 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/protocols/output/rest-json.json
--rw-r--r--   0 runner    (1001) docker     (127)    31012 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/protocols/output/rest-xml.json
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/put_object_data
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.986327 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.878326 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/json/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.986327 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/json/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/json/errors/datapipeline-create-pipeline.json
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/json/errors/directconnect-delete-connection.json
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/json/errors/dynamodb-put-item.json
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/json/errors/elastictranscoder-delete-pipeline.json
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/json/errors/opsworks-delete-stack.json
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/json/errors/storagegateway-delete-gateway.json
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/json/errors/swf-deprecate-domain.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.986327 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/json/expected/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/json/expected/datapipeline-create-pipeline.json
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/json/expected/directconnect-delete-connection.json
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/json/expected/dynamodb-put-item.json
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/json/expected/elastictranscoder-delete-pipeline.json
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/json/expected/elastictranscoder-list-pipelines.json
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/json/expected/opsworks-delete-stack.json
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/json/expected/storagegateway-delete-gateway.json
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/json/expected/swf-deprecate-domain.json
--rw-r--r--   0 runner    (1001) docker     (127)     7442 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/test_response_parsing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.878326 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:47.990327 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/errors/autoscaling-delete-policy.json
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/errors/autoscaling-delete-policy.xml
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/errors/cloudformation-cancel-update-stack.json
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/errors/cloudformation-cancel-update-stack.xml
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/errors/cloudwatch-describe-alarm-history.json
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/errors/cloudwatch-describe-alarm-history.xml
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/errors/ec2-describe-instances.json
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/errors/ec2-describe-instances.xml
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/errors/elb-describe-load-balancers.json
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/errors/elb-describe-load-balancers.xml
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/errors/iam-get-user.json
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/errors/iam-get-user.xml
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/errors/importexport-get-status.json
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/errors/importexport-get-status.xml
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/errors/rds-describe-db-instances.json
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/errors/rds-describe-db-instances.xml
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/errors/route53-get-hosted-zone.json
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/errors/route53-get-hosted-zone.xml
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/errors/s3-create-bucket.json
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/errors/s3-create-bucket.xml
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/errors/s3-list-objects.json
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/errors/s3-list-objects.xml
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/errors/ses-delete-identity.json
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/errors/ses-delete-identity.xml
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/errors/sns-delete-topic.json
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/errors/sns-delete-topic.xml
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/errors/sqs-delete-queue.json
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/errors/sts-get-session-token.json
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/errors/sts-get-session-token.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:48.030327 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/autoscaling-describe-adjustment-types.json
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/autoscaling-describe-adjustment-types.xml
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/autoscaling-describe-auto-scaling-groups.json
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/autoscaling-describe-auto-scaling-groups.xml
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/autoscaling-describe-auto-scaling-instances.json
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/autoscaling-describe-auto-scaling-instances.xml
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/autoscaling-describe-auto-scaling-notification-types.json
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/autoscaling-describe-auto-scaling-notification-types.xml
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/autoscaling-describe-launch-configurations.json
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/autoscaling-describe-launch-configurations.xml
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/autoscaling-describe-metric-collection-types.json
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/autoscaling-describe-metric-collection-types.xml
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/autoscaling-describe-notification-configurations.json
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/autoscaling-describe-notification-configurations.xml
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/autoscaling-describe-policies.json
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/autoscaling-describe-policies.xml
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/autoscaling-describe-scaling-activities.json
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/autoscaling-describe-scaling-activities.xml
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/autoscaling-describe-scaling-process-types.json
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/autoscaling-describe-scaling-process-types.xml
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/autoscaling-describe-scheduled-actions.json
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/autoscaling-describe-scheduled-actions.xml
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/autoscaling-describe-tags.json
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/autoscaling-describe-tags.xml
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/autoscaling-describe-termination-policy-types.json
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/autoscaling-describe-termination-policy-types.xml
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/cloudformation-describe-stacks.json
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/cloudformation-describe-stacks.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5985 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/cloudformation-get-template.json
--rw-r--r--   0 runner    (1001) docker     (127)     5222 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/cloudformation-get-template.xml
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/cloudformation-list-stacks.json
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/cloudformation-list-stacks.xml
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/cloudfront-get-cloud-front-origin-access-identity.json
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/cloudfront-get-cloud-front-origin-access-identity.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4562 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/cloudfront-get-distribution.json
--rw-r--r--   0 runner    (1001) docker     (127)     4769 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/cloudfront-get-distribution.xml
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/cloudfront-get-invalidation.json
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/cloudfront-get-invalidation.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/cloudfront-get-streaming-distribution.json
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/cloudfront-get-streaming-distribution.xml
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/cloudfront-list-cloud-front-origin-access-identities.json
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/cloudfront-list-cloud-front-origin-access-identities.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3943 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/cloudfront-list-distributions.json
--rw-r--r--   0 runner    (1001) docker     (127)     4181 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/cloudfront-list-distributions.xml
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/cloudfront-list-invalidations.json
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/cloudfront-list-invalidations.xml
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/cloudfront-list-streaming-distributions.json
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/cloudfront-list-streaming-distributions.xml
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/cloudwatch-describe-alarm-history.json
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/cloudwatch-describe-alarm-history.xml
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/cloudwatch-describe-alarms.json
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/cloudwatch-describe-alarms.xml
--rw-r--r--   0 runner    (1001) docker     (127)    21940 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/cloudwatch-list-metrics.json
--rw-r--r--   0 runner    (1001) docker     (127)    22671 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/cloudwatch-list-metrics.xml
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-allocate-address.json
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-allocate-address.xml
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-assign-private-ip-addresses.json
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-assign-private-ip-addresses.xml
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-associate-address.json
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-associate-address.xml
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-associate-route-table.json
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-associate-route-table.xml
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-attach-volume.json
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-attach-volume.xml
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-attach-vpn-gateway.json
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-attach-vpn-gateway.xml
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-bundle-instance.json
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-bundle-instance.xml
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-cancel-bundle-task.json
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-cancel-bundle-task.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-cancel-reserved-instances-listing.json
--rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-cancel-reserved-instances-listing.xml
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-cancel-spot-instance-requests.json
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-cancel-spot-instance-requests.xml
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-confirm-product-instance.json
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-confirm-product-instance.xml
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-copy-snapshot.json
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-copy-snapshot.xml
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-create-customer-gateway.json
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-create-customer-gateway.xml
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-create-dhcp-options.json
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-create-dhcp-options.xml
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-create-instance-export-task.json
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-create-instance-export-task.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-create-key-pair.json
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-create-key-pair.xml
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-create-network-acl.json
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-create-network-acl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-create-network-interface.json
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-create-network-interface.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-create-reserved-instances-listing.json
--rw-r--r--   0 runner    (1001) docker     (127)     3860 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-create-reserved-instances-listing.xml
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-create-route-table.json
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-create-route-table.xml
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-create-snapshot.json
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-create-snapshot.xml
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-create-spot-datafeed-subscription.json
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-create-spot-datafeed-subscription.xml
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-create-subnet.json
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-create-subnet.xml
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-create-volume.json
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-create-volume.xml
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-create-vpc.json
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-create-vpc.xml
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-create-vpn-gateway.json
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-create-vpn-gateway.xml
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-delete-internet-gateway.json
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-delete-internet-gateway.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-account-attributes.json
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-account-attributes.xml
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-addresses.json
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-addresses.xml
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-availability-zones.json
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-availability-zones.xml
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-bundle-tasks.json
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-bundle-tasks.xml
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-customer-gateways.json
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-customer-gateways.xml
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-dhcp-options.json
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-dhcp-options.xml
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-export-tasks.json
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-export-tasks.xml
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-instance-attribute.json
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-instance-attribute.xml
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-instance-status.json
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-instance-status.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-instances.json
--rw-r--r--   0 runner    (1001) docker     (127)     6389 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-instances.xml
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-internet-gateways.json
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-internet-gateways.xml
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-key-pairs.json
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-key-pairs.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-network-acls.json
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-network-acls.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-network-interfaces.json
--rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-network-interfaces.xml
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-placement-groups.json
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-placement-groups.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-regions.json
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-regions.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-reserved-instances-offerings.json
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-reserved-instances-offerings.xml
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-reserved-instances.json
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-reserved-instances.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-route-tables.json
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-route-tables.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5264 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-security-groups.json
--rw-r--r--   0 runner    (1001) docker     (127)     6128 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-security-groups.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-snapshots.json
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-snapshots.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-spot-instance-requests.json
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-spot-instance-requests.xml
--rw-r--r--   0 runner    (1001) docker     (127)   248956 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-spot-price-history.json
--rw-r--r--   0 runner    (1001) docker     (127)   314117 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-spot-price-history.xml
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-subnets.json
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-subnets.xml
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-tags.json
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-tags.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-volume-status.json
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-volume-status.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-volumes.json
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-volumes.xml
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-vpcs.json
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-vpcs.xml
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-vpn-connections.json
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-vpn-connections.xml
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-vpn-gateways.json
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-vpn-gateways.xml
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-detach-network-interface.json
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-detach-network-interface.xml
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-detach-volume.json
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-detach-volume.xml
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-get-password-data.json
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-get-password-data.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-import-instance.json
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-import-instance.xml
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-import-key-pair.json
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-import-key-pair.xml
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-import-volume.json
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-import-volume.xml
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-modify-snapshot-attribute.json
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-modify-snapshot-attribute.xml
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-monitor-instances.json
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-monitor-instances.xml
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-register-image.json
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-register-image.xml
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-replace-network-acl-association.json
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-replace-network-acl-association.xml
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-request-spot-instances.json
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-request-spot-instances.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-run-instances.json
--rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-run-instances.xml
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-start-instances.json
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-start-instances.xml
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-stop-instances.json
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-stop-instances.xml
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-unmonitor-instances.json
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-unmonitor-instances.xml
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/elasticbeanstalk-check-dns-availability.json
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/elasticbeanstalk-check-dns-availability.xml
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/elasticbeanstalk-create-application-version.json
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/elasticbeanstalk-create-application-version.xml
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/elasticbeanstalk-create-application.json
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/elasticbeanstalk-create-application.xml
--rw-r--r--   0 runner    (1001) docker     (127)     7362 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/elasticbeanstalk-create-configuration-template.json
--rw-r--r--   0 runner    (1001) docker     (127)     7328 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/elasticbeanstalk-create-configuration-template.xml
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/elasticbeanstalk-create-environment.json
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/elasticbeanstalk-create-environment.xml
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/elasticbeanstalk-create-storage-location.json
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/elasticbeanstalk-create-storage-location.xml
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/elasticbeanstalk-delete-application.json
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/elasticbeanstalk-delete-application.xml
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/elasticbeanstalk-describe-application-versions.json
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/elasticbeanstalk-describe-application-versions.xml
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/elasticbeanstalk-describe-applications.json
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/elasticbeanstalk-describe-applications.xml
--rw-r--r--   0 runner    (1001) docker     (127)    16850 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/elasticbeanstalk-describe-configuration-options.json
--rw-r--r--   0 runner    (1001) docker     (127)    19126 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/elasticbeanstalk-describe-configuration-options.xml
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/elasticbeanstalk-describe-environments.json
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/elasticbeanstalk-describe-environments.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/elasticbeanstalk-describe-events.json
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/elasticbeanstalk-describe-events.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/elasticbeanstalk-list-available-solution-stacks.json
--rw-r--r--   0 runner    (1001) docker     (127)     5492 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/elasticbeanstalk-list-available-solution-stacks.xml
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/elasticbeanstalk-retrieve-environment-info.json
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/elasticbeanstalk-retrieve-environment-info.xml
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/elasticbeanstalk-terminate-environment.json
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/elasticbeanstalk-terminate-environment.xml
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/elasticbeanstalk-update-application-version.json
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/elasticbeanstalk-update-application-version.xml
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/elasticbeanstalk-update-application.json
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/elasticbeanstalk-update-application.xml
--rw-r--r--   0 runner    (1001) docker     (127)    17788 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/elb-describe-load-balancer-policies.json
--rw-r--r--   0 runner    (1001) docker     (127)    19095 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/elb-describe-load-balancer-policies.xml
--rw-r--r--   0 runner    (1001) docker     (127)    21850 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/elb-describe-load-balancer-policy-types.json
--rw-r--r--   0 runner    (1001) docker     (127)    22855 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/elb-describe-load-balancer-policy-types.xml
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/elb-describe-load-balancers.json
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/elb-describe-load-balancers.xml
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/iam-create-virtual-mfa-device.json
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/iam-create-virtual-mfa-device.xml
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/iam-get-account-summary.json
--rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/iam-get-account-summary.xml
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/iam-get-group.json
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/iam-get-group.xml
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/iam-get-user-policy.json
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/iam-get-user-policy.xml
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/iam-get-user.json
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/iam-get-user.xml
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/iam-list-access-keys.json
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/iam-list-access-keys.xml
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/iam-list-account-aliases.json
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/iam-list-account-aliases.xml
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/iam-list-groups.json
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/iam-list-groups.xml
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/iam-list-instance-profiles.json
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/iam-list-instance-profiles.xml
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/iam-list-mfa-devices.json
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/iam-list-mfa-devices.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/iam-list-roles.json
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/iam-list-roles.xml
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/iam-list-server-certificates.json
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/iam-list-server-certificates.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/iam-list-signing-certificates.json
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/iam-list-signing-certificates.xml
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/iam-list-users.json
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/iam-list-users.xml
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/iam-list-virtual-mfa-devices.json
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/iam-list-virtual-mfa-devices.xml
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/importexport-list-jobs.json
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/importexport-list-jobs.xml
--rw-r--r--   0 runner    (1001) docker     (127)     6666 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/rds-describe-db-engine-versions.json
--rw-r--r--   0 runner    (1001) docker     (127)     8608 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/rds-describe-db-engine-versions.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/rds-describe-db-instances.json
--rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/rds-describe-db-instances.xml
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/rds-describe-db-parameter-groups.json
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/rds-describe-db-parameter-groups.xml
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/rds-describe-db-security-groups.json
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/rds-describe-db-security-groups.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/rds-describe-db-snapshots.json
--rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/rds-describe-db-snapshots.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/rds-describe-db-subnet-groups.json
--rw-r--r--   0 runner    (1001) docker     (127)     3431 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/rds-describe-db-subnet-groups.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/rds-describe-event-categories.json
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/rds-describe-event-categories.xml
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/rds-describe-event-subscriptions.json
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/rds-describe-event-subscriptions.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/rds-describe-events.json
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/rds-describe-events.xml
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/rds-describe-option-groups.json
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/rds-describe-option-groups.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/rds-describe-reserved-db-instances-offerings.json
--rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/rds-describe-reserved-db-instances-offerings.xml
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/rds-describe-reserved-db-instances.json
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/rds-describe-reserved-db-instances.xml
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-authorize-cluster-security-group-ingress.json
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-authorize-cluster-security-group-ingress.xml
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-copy-cluster-snapshot.json
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-copy-cluster-snapshot.xml
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-create-cluster-parameter-group.json
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-create-cluster-parameter-group.xml
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-create-cluster-security-group.json
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-create-cluster-security-group.xml
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-create-cluster-snapshot.json
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-create-cluster-snapshot.xml
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-create-cluster-subnet-group.json
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-create-cluster-subnet-group.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-create-cluster.json
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-create-cluster.xml
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-delete-cluster-parameter-group.json
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-delete-cluster-parameter-group.xml
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-delete-cluster-snapshot.json
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-delete-cluster-snapshot.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-delete-cluster.json
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-delete-cluster.xml
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-parameter-groups.json
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-parameter-groups.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-parameters.json
--rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-parameters.xml
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-security-groups.json
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-security-groups.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-snapshots.json
--rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-snapshots.xml
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-subnet-groups.json
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-subnet-groups.xml
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-versions.json
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-versions.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-describe-clusters.json
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-describe-clusters.xml
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-describe-events.json
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-describe-events.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-describe-orderable-cluster-options.json
--rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-describe-orderable-cluster-options.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-describe-reserved-node-offerings.json
--rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-describe-reserved-node-offerings.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-describe-reserved-nodes.json
--rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-describe-reserved-nodes.xml
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-describe-resize.json
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-describe-resize.xml
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-modify-cluster-parameter-group.json
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-modify-cluster-parameter-group.xml
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-purchase-reserved-node-offering.json
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-purchase-reserved-node-offering.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-reboot-cluster.json
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-reboot-cluster.xml
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-reset-cluster-parameter-group.json
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-reset-cluster-parameter-group.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-restore-from-cluster-snapshot.json
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-restore-from-cluster-snapshot.xml
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-revoke-cluster-security-group-ingress.json
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-revoke-cluster-security-group-ingress.xml
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/s3-get-bucket-acl.json
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/s3-get-bucket-acl.xml
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/s3-get-bucket-location.json
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/s3-get-bucket-location.xml
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/s3-get-bucket-logging.json
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/s3-get-bucket-logging.xml
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/s3-get-bucket-policy.json
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/s3-get-bucket-policy.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5077 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/s3-list-buckets.json
--rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/s3-list-buckets.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/s3-list-multipart-uploads#2.json
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/s3-list-multipart-uploads#2.xml
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/s3-list-multipart-uploads.json
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/s3-list-multipart-uploads.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/s3-list-object-versions.json
--rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/s3-list-object-versions.xml
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/s3-list-objects.json
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/s3-list-objects.xml
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ses-delete-identity.json
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ses-delete-identity.xml
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ses-get-identity-dkim-attributes.json
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ses-get-identity-dkim-attributes.xml
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ses-get-identity-notification-attributes.json
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ses-get-identity-notification-attributes.xml
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ses-get-identity-verification-attributes.json
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ses-get-identity-verification-attributes.xml
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ses-get-send-quota.json
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ses-get-send-quota.xml
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ses-get-send-statistics.json
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ses-get-send-statistics.xml
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ses-list-identities.json
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ses-list-identities.xml
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ses-send-email.json
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ses-send-email.xml
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ses-send-raw-email.json
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ses-send-raw-email.xml
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ses-set-identity-dkim-enabled.json
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ses-set-identity-dkim-enabled.xml
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ses-verify-domain-dkim.json
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ses-verify-domain-dkim.xml
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ses-verify-domain-identity.json
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ses-verify-domain-identity.xml
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/sns-add-permission.json
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/sns-add-permission.xml
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/sns-confirm-subscription.json
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/sns-confirm-subscription.xml
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/sns-create-topic.json
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/sns-create-topic.xml
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/sns-get-subscription-attributes.json
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/sns-get-subscription-attributes.xml
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/sns-get-topic-attributes.json
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/sns-get-topic-attributes.xml
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/sns-list-subscriptions-by-topic.json
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/sns-list-subscriptions-by-topic.xml
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/sns-list-subscriptions.json
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/sns-list-subscriptions.xml
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/sns-list-topics.json
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/sns-list-topics.xml
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/sns-publish.json
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/sns-publish.xml
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/sns-subscribe.json
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/sns-subscribe.xml
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/sqs-add-permission.json
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/sqs-change-message-visibility-batch.json
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/sqs-create-queue.json
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/sqs-delete-message-batch.json
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/sqs-get-queue-attributes.json
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/sqs-get-queue-url.json
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/sqs-list-queues.json
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/sqs-receive-message.json
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/sqs-send-message-batch.json
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/sqs-send-message.json
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/sts-get-session-token.json
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/sts-get-session-token.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:48.034327 botocore-a-la-carte-1.34.98/tests/unit/retries/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/retries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6630 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/retries/test_adaptive.py
--rw-r--r--   0 runner    (1001) docker     (127)     4602 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/retries/test_bucket.py
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/retries/test_quota.py
--rw-r--r--   0 runner    (1001) docker     (127)     4763 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/retries/test_special.py
--rw-r--r--   0 runner    (1001) docker     (127)    26367 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/retries/test_standard.py
--rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/retries/test_throttling.py
--rw-r--r--   0 runner    (1001) docker     (127)    35112 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/test_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/test_auth_bearer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/test_auth_sigv4.py
--rw-r--r--   0 runner    (1001) docker     (127)    30747 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/test_awsrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)    93962 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7070 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/test_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     9524 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/test_compress.py
--rw-r--r--   0 runner    (1001) docker     (127)    39978 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/test_config_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     8695 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/test_configloader.py
--rw-r--r--   0 runner    (1001) docker     (127)   139891 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    20712 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/test_discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)    18355 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/test_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)    15094 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/test_endpoint_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     5613 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/test_errorfactory.py
--rw-r--r--   0 runner    (1001) docker     (127)    15485 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/test_eventstream.py
--rw-r--r--   0 runner    (1001) docker     (127)     6399 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    63533 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/test_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/test_history.py
--rw-r--r--   0 runner    (1001) docker     (127)    27457 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/test_hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/test_http_client_exception_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)    19734 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/test_http_session.py
--rw-r--r--   0 runner    (1001) docker     (127)    27402 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/test_httpchecksum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/test_idempotency.py
--rw-r--r--   0 runner    (1001) docker     (127)    19334 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/test_loaders.py
--rw-r--r--   0 runner    (1001) docker     (127)    47606 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/test_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    35401 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/test_monitoring.py
--rw-r--r--   0 runner    (1001) docker     (127)    57408 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/test_paginate.py
--rw-r--r--   0 runner    (1001) docker     (127)    58705 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/test_parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)    17041 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/test_protocols.py
--rw-r--r--   0 runner    (1001) docker     (127)    50089 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/test_regions.py
--rw-r--r--   0 runner    (1001) docker     (127)    14405 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/test_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    15360 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/test_retryhandler.py
--rw-r--r--   0 runner    (1001) docker     (127)     9458 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/test_s3_addressing.py
--rw-r--r--   0 runner    (1001) docker     (127)    19004 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/test_serialize.py
--rw-r--r--   0 runner    (1001) docker     (127)    40114 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/test_session.py
--rw-r--r--   0 runner    (1001) docker     (127)    35707 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/test_session_legacy.py
--rw-r--r--   0 runner    (1001) docker     (127)    43689 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/test_signers.py
--rw-r--r--   0 runner    (1001) docker     (127)     8655 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/test_stub.py
--rw-r--r--   0 runner    (1001) docker     (127)    11901 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/test_tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     4321 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/test_translate.py
--rw-r--r--   0 runner    (1001) docker     (127)     6462 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/test_useragent.py
--rw-r--r--   0 runner    (1001) docker     (127)   126991 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    21414 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/test_validate.py
--rw-r--r--   0 runner    (1001) docker     (127)    33648 2024-05-04 01:01:11.000000 botocore-a-la-carte-1.34.98/tests/unit/test_waiters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.300086 botocore-a-la-carte-1.34.99/
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-05-07 01:02:10.000000 botocore-a-la-carte-1.34.99/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-07 01:02:10.000000 botocore-a-la-carte-1.34.99/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-05-07 01:02:10.000000 botocore-a-la-carte-1.34.99/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-05-07 01:02:50.300086 botocore-a-la-carte-1.34.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-07 01:02:49.000000 botocore-a-la-carte-1.34.99/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.148086 botocore-a-la-carte-1.34.99/botocore/
+-rw-r--r--   0 runner    (1001) docker     (127)     4914 2024-05-07 01:02:10.000000 botocore-a-la-carte-1.34.99/botocore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30640 2024-05-07 01:02:10.000000 botocore-a-la-carte-1.34.99/botocore/args.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43803 2024-05-07 01:02:10.000000 botocore-a-la-carte-1.34.99/botocore/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23156 2024-05-07 01:02:10.000000 botocore-a-la-carte-1.34.99/botocore/awsrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)   266617 2024-05-07 01:02:10.000000 botocore-a-la-carte-1.34.99/botocore/cacert.pem
+-rw-r--r--   0 runner    (1001) docker     (127)    51753 2024-05-07 01:02:10.000000 botocore-a-la-carte-1.34.99/botocore/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11091 2024-05-07 01:02:10.000000 botocore-a-la-carte-1.34.99/botocore/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4430 2024-05-07 01:02:10.000000 botocore-a-la-carte-1.34.99/botocore/compress.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15601 2024-05-07 01:02:10.000000 botocore-a-la-carte-1.34.99/botocore/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10039 2024-05-07 01:02:10.000000 botocore-a-la-carte-1.34.99/botocore/configloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37230 2024-05-07 01:02:10.000000 botocore-a-la-carte-1.34.99/botocore/configprovider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    84795 2024-05-07 01:02:10.000000 botocore-a-la-carte-1.34.99/botocore/credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.148086 botocore-a-la-carte-1.34.99/botocore/crt/
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-07 01:02:10.000000 botocore-a-la-carte-1.34.99/botocore/crt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25318 2024-05-07 01:02:10.000000 botocore-a-la-carte-1.34.99/botocore/crt/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.148086 botocore-a-la-carte-1.34.99/botocore/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     7025 2024-05-07 01:02:10.000000 botocore-a-la-carte-1.34.99/botocore/data/_retry.json
+-rw-r--r--   0 runner    (1001) docker     (127)   881041 2024-05-07 01:02:10.000000 botocore-a-la-carte-1.34.99/botocore/data/endpoints.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5765 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/botocore/data/partitions.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/botocore/data/sdk-default-configuration.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11075 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/botocore/discovery.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.152086 botocore-a-la-carte-1.34.99/botocore/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/botocore/docs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.152086 botocore-a-la-carte-1.34.99/botocore/docs/bcdoc/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/botocore/docs/bcdoc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10207 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/botocore/docs/bcdoc/docstringparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9698 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/botocore/docs/bcdoc/restdoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13148 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/botocore/docs/bcdoc/style.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17380 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/botocore/docs/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/botocore/docs/docstring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8949 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/botocore/docs/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12058 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/botocore/docs/method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9020 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/botocore/docs/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11760 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/botocore/docs/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4990 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/botocore/docs/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5198 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/botocore/docs/shape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9214 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/botocore/docs/sharedexample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/botocore/docs/translator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7292 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/botocore/docs/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6626 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/botocore/docs/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16441 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/botocore/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22934 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/botocore/endpoint_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3722 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/botocore/errorfactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20449 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/botocore/eventstream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22804 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/botocore/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55288 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/botocore/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/botocore/history.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25060 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/botocore/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16292 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/botocore/httpchecksum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18582 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/botocore/httpsession.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18833 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/botocore/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30619 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/botocore/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20597 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/botocore/monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27392 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/botocore/paginate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45607 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/botocore/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32426 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/botocore/regions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7227 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/botocore/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.152086 botocore-a-la-carte-1.34.99/botocore/retries/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/botocore/retries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4207 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/botocore/retries/adaptive.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/botocore/retries/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3993 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/botocore/retries/bucket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/botocore/retries/quota.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/botocore/retries/special.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19974 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/botocore/retries/standard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/botocore/retries/throttling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14700 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/botocore/retryhandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33122 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/botocore/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49184 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/botocore/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30965 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/botocore/signers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15152 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/botocore/stub.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10910 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/botocore/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/botocore/translate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18305 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/botocore/useragent.py
+-rw-r--r--   0 runner    (1001) docker     (127)   135065 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/botocore/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13767 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/botocore/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.152086 botocore-a-la-carte-1.34.99/botocore/vendored/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/botocore/vendored/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.152086 botocore-a-la-carte-1.34.99/botocore/vendored/requests/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/botocore/vendored/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/botocore/vendored/requests/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.152086 botocore-a-la-carte-1.34.99/botocore/vendored/requests/packages/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/botocore/vendored/requests/packages/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.152086 botocore-a-la-carte-1.34.99/botocore/vendored/requests/packages/urllib3/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/botocore/vendored/requests/packages/urllib3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/botocore/vendored/requests/packages/urllib3/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34549 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/botocore/vendored/six.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14290 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/botocore/waiter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.152086 botocore-a-la-carte-1.34.99/botocore_a_la_carte.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-05-07 01:02:50.000000 botocore-a-la-carte-1.34.99/botocore_a_la_carte.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    91711 2024-05-07 01:02:50.000000 botocore-a-la-carte-1.34.99/botocore_a_la_carte.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 01:02:50.000000 botocore-a-la-carte-1.34.99/botocore_a_la_carte.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-07 01:02:50.000000 botocore-a-la-carte-1.34.99/botocore_a_la_carte.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-07 01:02:50.000000 botocore-a-la-carte-1.34.99/botocore_a_la_carte.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.152086 botocore-a-la-carte-1.34.99/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     5657 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5109 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.152086 botocore-a-la-carte-1.34.99/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.156086 botocore-a-la-carte-1.34.99/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/docs/source/_static/404.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.156086 botocore-a-la-carte-1.34.99/docs/source/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/docs/source/_static/css/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.156086 botocore-a-la-carte-1.34.99/docs/source/_static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     7600 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/docs/source/_static/js/custom.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.156086 botocore-a-la-carte-1.34.99/docs/source/_static/logos/
+-rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/docs/source/_static/logos/aws_dark_theme_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3399 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/docs/source/_static/logos/aws_light_theme_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   136184 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/docs/source/_static/shortbreadv1.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.156086 botocore-a-la-carte-1.34.99/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)    13300 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/docs/source/_templates/page.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.156086 botocore-a-la-carte-1.34.99/docs/source/_templates/sidebar/
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/docs/source/_templates/sidebar/close-icon.html
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/docs/source/_templates/sidebar/feedback.html
+-rw-r--r--   0 runner    (1001) docker     (127)     8369 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/docs/source/client_upgrades.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9883 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.156086 botocore-a-la-carte-1.34.99/docs/source/development/
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/docs/source/development/changesfor10.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/docs/source/development/designnotes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/docs/source/development/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9302 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.156086 botocore-a-la-carte-1.34.99/docs/source/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/docs/source/reference/awsrequest.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/docs/source/reference/config.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/docs/source/reference/eventstream.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/docs/source/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/docs/source/reference/loaders.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/docs/source/reference/response.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/docs/source/reference/stubber.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.156086 botocore-a-la-carte-1.34.99/docs/source/topics/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/docs/source/topics/document_type.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/docs/source/topics/events.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/docs/source/topics/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/docs/source/topics/paginators.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.156086 botocore-a-la-carte-1.34.99/docs/source/tutorial/
+-rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/docs/source/tutorial/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    21852 2024-05-07 01:02:50.300086 botocore-a-la-carte-1.34.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-05-07 01:02:49.000000 botocore-a-la-carte-1.34.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.156086 botocore-a-la-carte-1.34.99/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    18817 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.112086 botocore-a-la-carte-1.34.99/tests/acceptance/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.156086 botocore-a-la-carte-1.34.99/tests/acceptance/features/
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/acceptance/features/environment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.116086 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.156086 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/acm/
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/acm/acm.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.156086 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/autoscaling/
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/autoscaling/autoscaling.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.156086 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/cloudformation/
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/cloudformation/cloudformation.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.156086 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/cloudfront/
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/cloudfront/cloudfront.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.156086 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/cloudhsm/
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/cloudhsm/cloudhsm.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.156086 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/cloudsearch/
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/cloudsearch/cloudsearch.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.156086 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/cloudtrail/
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/cloudtrail/cloudtrail.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.156086 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/cloudwatch/
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/cloudwatch/cloudwatch.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.156086 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/cloudwatchlogs/
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/cloudwatchlogs/cloudwatchlogs.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.156086 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/codecommit/
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/codecommit/codecommit.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.156086 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/codedeploy/
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/codedeploy/codedeploy.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.156086 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/codepipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/codepipeline/codepipeline.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.160086 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/cognitoidentity/
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/cognitoidentity/cognitoidentity.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.160086 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/cognitosync/
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/cognitosync/cognitosync.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.160086 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/configservice/
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/configservice/configservice.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.160086 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/datapipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/datapipeline/datapipeline.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.160086 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/devicefarm/
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/devicefarm/devicefarm.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.160086 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/directconnect/
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/directconnect/directconnect.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.160086 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/directoryservice/
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/directoryservice/directoryservice.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.160086 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/dynamodb/
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/dynamodb/dynamodb.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.160086 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/dynamodbstreams/
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/dynamodbstreams/dynamodbstreams.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.160086 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/ec2/
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/ec2/ec2.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.160086 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/ecs/
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/ecs/ecs.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.160086 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/efs/
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/efs/efs.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.160086 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/elasticache/
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/elasticache/elasticache.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.160086 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/elasticbeanstalk/
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/elasticbeanstalk/elasticbeanstalk.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.160086 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/elasticloadbalancing/
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/elasticloadbalancing/elasticloadbalancing.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.160086 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/elastictranscoder/
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/elastictranscoder/elastictranscoder.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.160086 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/emr/
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/emr/emr.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.160086 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/es/
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/es/es.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.160086 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/glacier/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/glacier/glacier.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.160086 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/iam/
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/iam/iam.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.160086 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/importexport/
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/importexport/importexport.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.160086 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/kinesis/
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/kinesis/kinesis.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.160086 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/kms/
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/kms/kms.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.160086 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/lambda/
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/lambda/lambda.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.160086 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/machinelearning/
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/machinelearning/machinelearning.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.160086 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/opsworks/
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/opsworks/opsworks.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.160086 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/rds/
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/rds/rds.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.160086 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/redshift/
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/redshift/redshift.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.160086 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/route53/
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/route53/route53.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.160086 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/route53domains/
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/route53domains/route53domains.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.160086 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/ses/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/ses/ses.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.160086 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/sns/
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/sns/sns.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.160086 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/sqs/
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/sqs/sqs.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.160086 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/ssm/
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/ssm/ssm.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.160086 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/storagegateway/
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/storagegateway/storagegateway.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.160086 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/sts/
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/sts/sts.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.160086 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/support/
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/support/support.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.160086 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/swf/
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/swf/swf.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.160086 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/waf/
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/waf/waf.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.160086 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/workspaces/
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/workspaces/workspaces.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.160086 botocore-a-la-carte-1.34.99/tests/acceptance/features/steps/
+-rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/acceptance/features/steps/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8444 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/cmd-runner
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.168086 botocore-a-la-carte-1.34.99/tests/functional/
+-rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.168086 botocore-a-la-carte-1.34.99/tests/functional/configured_endpoint_urls/
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/configured_endpoint_urls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20184 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/configured_endpoint_urls/profile-tests.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7578 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/configured_endpoint_urls/test_configured_endpoint_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.168086 botocore-a-la-carte-1.34.99/tests/functional/crt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/crt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.168086 botocore-a-la-carte-1.34.99/tests/functional/csm/
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/csm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32068 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/csm/cases.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.116086 botocore-a-la-carte-1.34.99/tests/functional/csm/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.116086 botocore-a-la-carte-1.34.99/tests/functional/csm/data/csmtest/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.168086 botocore-a-la-carte-1.34.99/tests/functional/csm/data/csmtest/2018-06-19/
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/csm/data/csmtest/2018-06-19/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6741 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/csm/test_monitoring.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.168086 botocore-a-la-carte-1.34.99/tests/functional/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     5588 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/docs/test_alias.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/docs/test_autoscaling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/docs/test_ec2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/docs/test_glacier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/docs/test_lex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/docs/test_s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/docs/test_secretsmanager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5333 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/docs/test_shared_example_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/docs/test_streaming_body.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.136086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.172086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/accessanalyzer/
+-rw-r--r--   0 runner    (1001) docker     (127)    22841 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/accessanalyzer/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.172086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/account/
+-rw-r--r--   0 runner    (1001) docker     (127)    12812 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/account/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.172086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/acm/
+-rw-r--r--   0 runner    (1001) docker     (127)    21886 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/acm/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.172086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/acm-pca/
+-rw-r--r--   0 runner    (1001) docker     (127)    22050 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/acm-pca/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.172086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/alexaforbusiness/
+-rw-r--r--   0 runner    (1001) docker     (127)    10458 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/alexaforbusiness/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.172086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/amp/
+-rw-r--r--   0 runner    (1001) docker     (127)    14268 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/amp/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.172086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/amplify/
+-rw-r--r--   0 runner    (1001) docker     (127)    18190 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/amplify/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.172086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/amplifybackend/
+-rw-r--r--   0 runner    (1001) docker     (127)    17569 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/amplifybackend/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.172086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/amplifyuibuilder/
+-rw-r--r--   0 runner    (1001) docker     (127)    17633 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/amplifyuibuilder/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.172086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/apigateway/
+-rw-r--r--   0 runner    (1001) docker     (127)    20036 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/apigateway/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.172086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/apigatewaymanagementapi/
+-rw-r--r--   0 runner    (1001) docker     (127)    10586 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/apigatewaymanagementapi/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.172086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/apigatewayv2/
+-rw-r--r--   0 runner    (1001) docker     (127)    20036 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/apigatewayv2/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.172086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/appconfig/
+-rw-r--r--   0 runner    (1001) docker     (127)    21296 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/appconfig/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.172086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/appconfigdata/
+-rw-r--r--   0 runner    (1001) docker     (127)    20581 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/appconfigdata/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.172086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/appfabric/
+-rw-r--r--   0 runner    (1001) docker     (127)    10554 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/appfabric/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.172086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/appflow/
+-rw-r--r--   0 runner    (1001) docker     (127)    16921 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/appflow/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.172086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/appintegrations/
+-rw-r--r--   0 runner    (1001) docker     (127)    14617 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/appintegrations/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.172086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/application-autoscaling/
+-rw-r--r--   0 runner    (1001) docker     (127)    21870 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/application-autoscaling/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.172086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/application-insights/
+-rw-r--r--   0 runner    (1001) docker     (127)    20378 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/application-insights/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.172086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/applicationcostprofiler/
+-rw-r--r--   0 runner    (1001) docker     (127)    10810 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/applicationcostprofiler/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.172086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/appmesh/
+-rw-r--r--   0 runner    (1001) docker     (127)    27442 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/appmesh/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.172086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/apprunner/
+-rw-r--r--   0 runner    (1001) docker     (127)    13113 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/apprunner/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.172086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/appstream/
+-rw-r--r--   0 runner    (1001) docker     (127)    16617 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/appstream/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.172086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/appsync/
+-rw-r--r--   0 runner    (1001) docker     (127)    19065 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/appsync/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.172086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/arc-zonal-shift/
+-rw-r--r--   0 runner    (1001) docker     (127)    10650 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/arc-zonal-shift/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.172086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/artifact/
+-rw-r--r--   0 runner    (1001) docker     (127)    10538 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/artifact/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.172086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/athena/
+-rw-r--r--   0 runner    (1001) docker     (127)    21588 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/athena/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.172086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/auditmanager/
+-rw-r--r--   0 runner    (1001) docker     (127)    15354 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/auditmanager/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.172086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/autoscaling/
+-rw-r--r--   0 runner    (1001) docker     (127)    20943 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/autoscaling/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.172086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/autoscaling-plans/
+-rw-r--r--   0 runner    (1001) docker     (127)    20748 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/autoscaling-plans/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.172086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/b2bi/
+-rw-r--r--   0 runner    (1001) docker     (127)    10474 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/b2bi/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.172086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/backup/
+-rw-r--r--   0 runner    (1001) docker     (127)    20319 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/backup/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.172086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/backup-gateway/
+-rw-r--r--   0 runner    (1001) docker     (127)    19742 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/backup-gateway/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.172086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/backupstorage/
+-rw-r--r--   0 runner    (1001) docker     (127)    10618 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/backupstorage/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.176086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/batch/
+-rw-r--r--   0 runner    (1001) docker     (127)    21970 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/batch/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.176086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/bcm-data-exports/
+-rw-r--r--   0 runner    (1001) docker     (127)     4942 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/bcm-data-exports/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.176086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/bedrock/
+-rw-r--r--   0 runner    (1001) docker     (127)    10522 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/bedrock/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.176086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/bedrock-agent/
+-rw-r--r--   0 runner    (1001) docker     (127)    10618 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/bedrock-agent/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.176086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/bedrock-agent-runtime/
+-rw-r--r--   0 runner    (1001) docker     (127)    10746 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/bedrock-agent-runtime/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.176086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/bedrock-runtime/
+-rw-r--r--   0 runner    (1001) docker     (127)    10650 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/bedrock-runtime/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.176086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/billingconductor/
+-rw-r--r--   0 runner    (1001) docker     (127)    11824 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/billingconductor/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.176086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/braket/
+-rw-r--r--   0 runner    (1001) docker     (127)    11766 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/braket/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.176086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/budgets/
+-rw-r--r--   0 runner    (1001) docker     (127)    12762 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/budgets/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.176086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/ce/
+-rw-r--r--   0 runner    (1001) docker     (127)    12702 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/ce/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.176086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/chatbot/
+-rw-r--r--   0 runner    (1001) docker     (127)    10522 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/chatbot/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.176086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/chime/
+-rw-r--r--   0 runner    (1001) docker     (127)    11615 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/chime/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.176086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/chime-sdk-identity/
+-rw-r--r--   0 runner    (1001) docker     (127)    11071 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/chime-sdk-identity/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.176086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/chime-sdk-media-pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)    12513 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/chime-sdk-media-pipelines/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.176086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/chime-sdk-meetings/
+-rw-r--r--   0 runner    (1001) docker     (127)    13256 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/chime-sdk-meetings/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.176086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/chime-sdk-messaging/
+-rw-r--r--   0 runner    (1001) docker     (127)    11088 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/chime-sdk-messaging/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.176086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/chime-sdk-voice/
+-rw-r--r--   0 runner    (1001) docker     (127)    10586 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/chime-sdk-voice/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.176086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/cleanrooms/
+-rw-r--r--   0 runner    (1001) docker     (127)    10570 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/cleanrooms/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.176086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/cleanroomsml/
+-rw-r--r--   0 runner    (1001) docker     (127)    10618 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/cleanroomsml/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.176086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/cloud9/
+-rw-r--r--   0 runner    (1001) docker     (127)    19014 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/cloud9/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.176086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/cloudcontrol/
+-rw-r--r--   0 runner    (1001) docker     (127)    22851 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/cloudcontrol/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.176086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/clouddirectory/
+-rw-r--r--   0 runner    (1001) docker     (127)    14979 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/clouddirectory/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.176086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/cloudformation/
+-rw-r--r--   0 runner    (1001) docker     (127)    22794 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/cloudformation/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.176086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/cloudfront/
+-rw-r--r--   0 runner    (1001) docker     (127)    13981 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/cloudfront/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.176086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/cloudfront-keyvaluestore/
+-rw-r--r--   0 runner    (1001) docker     (127)     8023 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/cloudfront-keyvaluestore/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.176086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/cloudhsm/
+-rw-r--r--   0 runner    (1001) docker     (127)    10972 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/cloudhsm/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.176086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/cloudhsmv2/
+-rw-r--r--   0 runner    (1001) docker     (127)    19594 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/cloudhsmv2/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.176086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/cloudsearch/
+-rw-r--r--   0 runner    (1001) docker     (127)    14480 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/cloudsearch/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.176086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/cloudsearchdomain/
+-rw-r--r--   0 runner    (1001) docker     (127)    10682 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/cloudsearchdomain/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.176086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/cloudtrail/
+-rw-r--r--   0 runner    (1001) docker     (127)    22618 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/cloudtrail/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.176086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/cloudtrail-data/
+-rw-r--r--   0 runner    (1001) docker     (127)    10650 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/cloudtrail-data/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.176086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/cloudwatch/
+-rw-r--r--   0 runner    (1001) docker     (127)    22618 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/cloudwatch/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.176086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/codeartifact/
+-rw-r--r--   0 runner    (1001) docker     (127)    15777 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/codeartifact/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.176086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/codebuild/
+-rw-r--r--   0 runner    (1001) docker     (127)    22152 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/codebuild/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.176086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/codecatalyst/
+-rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/codecatalyst/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.176086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/codecommit/
+-rw-r--r--   0 runner    (1001) docker     (127)    22192 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/codecommit/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.180086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/codeconnections/
+-rw-r--r--   0 runner    (1001) docker     (127)    10650 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/codeconnections/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.180086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/codedeploy/
+-rw-r--r--   0 runner    (1001) docker     (127)    22628 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/codedeploy/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.180086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/codeguru-reviewer/
+-rw-r--r--   0 runner    (1001) docker     (127)    14618 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/codeguru-reviewer/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.180086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/codeguru-security/
+-rw-r--r--   0 runner    (1001) docker     (127)    10682 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/codeguru-security/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.180086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/codeguruprofiler/
+-rw-r--r--   0 runner    (1001) docker     (127)    10682 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/codeguruprofiler/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.180086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/codepipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)    20979 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/codepipeline/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.180086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/codestar/
+-rw-r--r--   0 runner    (1001) docker     (127)    15683 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/codestar/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.180086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/codestar-connections/
+-rw-r--r--   0 runner    (1001) docker     (127)    17324 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/codestar-connections/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.180086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/codestar-notifications/
+-rw-r--r--   0 runner    (1001) docker     (127)    10762 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/codestar-notifications/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.180086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/cognito-identity/
+-rw-r--r--   0 runner    (1001) docker     (127)    19386 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/cognito-identity/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.180086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/cognito-idp/
+-rw-r--r--   0 runner    (1001) docker     (127)    19634 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/cognito-idp/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.180086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/cognito-sync/
+-rw-r--r--   0 runner    (1001) docker     (127)    14934 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/cognito-sync/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.180086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/comprehend/
+-rw-r--r--   0 runner    (1001) docker     (127)    17044 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/comprehend/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.180086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/comprehendmedical/
+-rw-r--r--   0 runner    (1001) docker     (127)    15049 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/comprehendmedical/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.180086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/compute-optimizer/
+-rw-r--r--   0 runner    (1001) docker     (127)    17680 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/compute-optimizer/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.180086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/config/
+-rw-r--r--   0 runner    (1001) docker     (127)    22442 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/config/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.180086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/connect/
+-rw-r--r--   0 runner    (1001) docker     (127)    15251 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/connect/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.180086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/connect-contact-lens/
+-rw-r--r--   0 runner    (1001) docker     (127)    13647 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/connect-contact-lens/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.180086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/connectcampaigns/
+-rw-r--r--   0 runner    (1001) docker     (127)    11990 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/connectcampaigns/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.180086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/connectcases/
+-rw-r--r--   0 runner    (1001) docker     (127)    10490 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/connectcases/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.180086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/connectparticipant/
+-rw-r--r--   0 runner    (1001) docker     (127)    11597 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/connectparticipant/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.180086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/controlcatalog/
+-rw-r--r--   0 runner    (1001) docker     (127)    10634 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/controlcatalog/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.180086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/controltower/
+-rw-r--r--   0 runner    (1001) docker     (127)    17946 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/controltower/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.180086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/cost-optimization-hub/
+-rw-r--r--   0 runner    (1001) docker     (127)    10746 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/cost-optimization-hub/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.180086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/cur/
+-rw-r--r--   0 runner    (1001) docker     (127)    10893 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/cur/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.180086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/customer-profiles/
+-rw-r--r--   0 runner    (1001) docker     (127)    14392 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/customer-profiles/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.180086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/databrew/
+-rw-r--r--   0 runner    (1001) docker     (127)    19530 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/databrew/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.180086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/dataexchange/
+-rw-r--r--   0 runner    (1001) docker     (127)    14931 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/dataexchange/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.180086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/datapipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)    12336 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/datapipeline/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.180086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/datasync/
+-rw-r--r--   0 runner    (1001) docker     (127)    22103 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/datasync/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.180086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/datazone/
+-rw-r--r--   0 runner    (1001) docker     (127)     3782 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/datazone/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.180086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/dax/
+-rw-r--r--   0 runner    (1001) docker     (127)    15954 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/dax/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.180086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/deadline/
+-rw-r--r--   0 runner    (1001) docker     (127)    10538 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/deadline/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.180086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/detective/
+-rw-r--r--   0 runner    (1001) docker     (127)    20995 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/detective/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.180086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/devicefarm/
+-rw-r--r--   0 runner    (1001) docker     (127)    10994 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/devicefarm/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.184086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/devops-guru/
+-rw-r--r--   0 runner    (1001) docker     (127)    14899 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/devops-guru/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.184086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/directconnect/
+-rw-r--r--   0 runner    (1001) docker     (127)    22318 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/directconnect/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.184086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/discovery/
+-rw-r--r--   0 runner    (1001) docker     (127)    13131 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/discovery/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.184086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/dlm/
+-rw-r--r--   0 runner    (1001) docker     (127)    20624 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/dlm/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.184086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/dms/
+-rw-r--r--   0 runner    (1001) docker     (127)    22724 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/dms/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.184086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/docdb/
+-rw-r--r--   0 runner    (1001) docker     (127)    22739 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/docdb/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.184086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/docdb-elastic/
+-rw-r--r--   0 runner    (1001) docker     (127)    10618 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/docdb-elastic/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.184086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/drs/
+-rw-r--r--   0 runner    (1001) docker     (127)    18906 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/drs/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.184086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/ds/
+-rw-r--r--   0 runner    (1001) docker     (127)    21848 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/ds/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.184086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/dynamodb/
+-rw-r--r--   0 runner    (1001) docker     (127)    23714 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/dynamodb/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.184086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/dynamodbstreams/
+-rw-r--r--   0 runner    (1001) docker     (127)    21894 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/dynamodbstreams/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.184086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/ebs/
+-rw-r--r--   0 runner    (1001) docker     (127)    21891 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/ebs/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.184086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/ec2/
+-rw-r--r--   0 runner    (1001) docker     (127)    24360 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/ec2/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.184086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/ec2-instance-connect/
+-rw-r--r--   0 runner    (1001) docker     (127)    10730 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/ec2-instance-connect/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.184086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/ecr/
+-rw-r--r--   0 runner    (1001) docker     (127)    22472 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/ecr/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.184086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/ecr-public/
+-rw-r--r--   0 runner    (1001) docker     (127)    10634 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/ecr-public/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.184086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/ecs/
+-rw-r--r--   0 runner    (1001) docker     (127)    22320 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/ecs/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.184086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/efs/
+-rw-r--r--   0 runner    (1001) docker     (127)    30883 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/efs/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.184086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/eks/
+-rw-r--r--   0 runner    (1001) docker     (127)    21884 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/eks/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.184086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/eks-auth/
+-rw-r--r--   0 runner    (1001) docker     (127)     3782 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/eks-auth/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.184086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/elastic-inference/
+-rw-r--r--   0 runner    (1001) docker     (127)    12951 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/elastic-inference/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.184086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/elasticache/
+-rw-r--r--   0 runner    (1001) docker     (127)    22662 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/elasticache/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.184086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/elasticbeanstalk/
+-rw-r--r--   0 runner    (1001) docker     (127)    22443 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/elasticbeanstalk/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.184086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/elastictranscoder/
+-rw-r--r--   0 runner    (1001) docker     (127)    13747 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/elastictranscoder/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.184086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/elb/
+-rw-r--r--   0 runner    (1001) docker     (127)    60943 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/elb/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.184086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/elbv2/
+-rw-r--r--   0 runner    (1001) docker     (127)    23058 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/elbv2/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.184086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/emr/
+-rw-r--r--   0 runner    (1001) docker     (127)    23324 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/emr/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.184086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/emr-containers/
+-rw-r--r--   0 runner    (1001) docker     (127)    19317 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/emr-containers/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.184086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/emr-serverless/
+-rw-r--r--   0 runner    (1001) docker     (127)    12364 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/emr-serverless/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.184086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/entityresolution/
+-rw-r--r--   0 runner    (1001) docker     (127)    10666 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/entityresolution/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.184086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/es/
+-rw-r--r--   0 runner    (1001) docker     (127)    22279 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/es/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.184086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/events/
+-rw-r--r--   0 runner    (1001) docker     (127)    27931 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/events/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.184086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/evidently/
+-rw-r--r--   0 runner    (1001) docker     (127)    13995 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/evidently/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.184086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/finspace/
+-rw-r--r--   0 runner    (1001) docker     (127)    12235 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/finspace/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.188086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/finspace-data/
+-rw-r--r--   0 runner    (1001) docker     (127)    12315 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/finspace-data/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.188086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/firehose/
+-rw-r--r--   0 runner    (1001) docker     (127)    22109 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/firehose/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.188086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/fis/
+-rw-r--r--   0 runner    (1001) docker     (127)    11309 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/fis/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.188086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/fms/
+-rw-r--r--   0 runner    (1001) docker     (127)    27852 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/fms/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.188086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/forecast/
+-rw-r--r--   0 runner    (1001) docker     (127)    15258 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/forecast/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.188086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/forecastquery/
+-rw-r--r--   0 runner    (1001) docker     (127)    15393 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/forecastquery/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.188086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/frauddetector/
+-rw-r--r--   0 runner    (1001) docker     (127)    12783 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/frauddetector/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.188086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/freetier/
+-rw-r--r--   0 runner    (1001) docker     (127)     5640 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/freetier/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.188086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/fsx/
+-rw-r--r--   0 runner    (1001) docker     (127)    21891 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/fsx/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.188086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/gamelift/
+-rw-r--r--   0 runner    (1001) docker     (127)    19526 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/gamelift/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.188086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/glacier/
+-rw-r--r--   0 runner    (1001) docker     (127)    22919 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/glacier/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.188086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/globalaccelerator/
+-rw-r--r--   0 runner    (1001) docker     (127)    10682 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/globalaccelerator/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.188086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/glue/
+-rw-r--r--   0 runner    (1001) docker     (127)    21504 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/glue/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.188086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/grafana/
+-rw-r--r--   0 runner    (1001) docker     (127)    14380 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/grafana/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.188086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/greengrass/
+-rw-r--r--   0 runner    (1001) docker     (127)    17830 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/greengrass/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.188086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/greengrassv2/
+-rw-r--r--   0 runner    (1001) docker     (127)    17830 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/greengrassv2/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.188086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/groundstation/
+-rw-r--r--   0 runner    (1001) docker     (127)    15796 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/groundstation/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.188086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/guardduty/
+-rw-r--r--   0 runner    (1001) docker     (127)    22142 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/guardduty/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.188086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/health/
+-rw-r--r--   0 runner    (1001) docker     (127)    12064 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/health/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.188086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/healthlake/
+-rw-r--r--   0 runner    (1001) docker     (127)    11418 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/healthlake/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.188086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/honeycode/
+-rw-r--r--   0 runner    (1001) docker     (127)    10977 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/honeycode/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.188086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/iam/
+-rw-r--r--   0 runner    (1001) docker     (127)    19907 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/iam/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.188086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/identitystore/
+-rw-r--r--   0 runner    (1001) docker     (127)    16697 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/identitystore/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.188086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/imagebuilder/
+-rw-r--r--   0 runner    (1001) docker     (127)    11471 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/imagebuilder/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.188086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/importexport/
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/importexport/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.188086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/inspector/
+-rw-r--r--   0 runner    (1001) docker     (127)    17418 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/inspector/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.188086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/inspector-scan/
+-rw-r--r--   0 runner    (1001) docker     (127)    10634 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/inspector-scan/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.188086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/inspector2/
+-rw-r--r--   0 runner    (1001) docker     (127)    18292 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/inspector2/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.188086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/internetmonitor/
+-rw-r--r--   0 runner    (1001) docker     (127)    10650 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/internetmonitor/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.188086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/iot/
+-rw-r--r--   0 runner    (1001) docker     (127)    20619 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/iot/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.188086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/iot-data/
+-rw-r--r--   0 runner    (1001) docker     (127)    20951 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/iot-data/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.188086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/iot-jobs-data/
+-rw-r--r--   0 runner    (1001) docker     (127)    21019 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/iot-jobs-data/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.188086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/iot1click-devices/
+-rw-r--r--   0 runner    (1001) docker     (127)    10682 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/iot1click-devices/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.188086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/iot1click-projects/
+-rw-r--r--   0 runner    (1001) docker     (127)    13314 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/iot1click-projects/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.188086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/iotanalytics/
+-rw-r--r--   0 runner    (1001) docker     (127)    13626 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/iotanalytics/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.192086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/iotdeviceadvisor/
+-rw-r--r--   0 runner    (1001) docker     (127)    12047 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/iotdeviceadvisor/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.192086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/iotevents/
+-rw-r--r--   0 runner    (1001) docker     (127)    15723 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/iotevents/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.192086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/iotevents-data/
+-rw-r--r--   0 runner    (1001) docker     (127)    10634 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/iotevents-data/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.192086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/iotfleethub/
+-rw-r--r--   0 runner    (1001) docker     (127)    17218 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/iotfleethub/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.192086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/iotfleetwise/
+-rw-r--r--   0 runner    (1001) docker     (127)    11037 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/iotfleetwise/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.192086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/iotsecuretunneling/
+-rw-r--r--   0 runner    (1001) docker     (127)    21179 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/iotsecuretunneling/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.192086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/iotsitewise/
+-rw-r--r--   0 runner    (1001) docker     (127)    17087 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/iotsitewise/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.192086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/iotthingsgraph/
+-rw-r--r--   0 runner    (1001) docker     (127)    12819 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/iotthingsgraph/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.192086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/iottwinmaker/
+-rw-r--r--   0 runner    (1001) docker     (127)    12771 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/iottwinmaker/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.192086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/iotwireless/
+-rw-r--r--   0 runner    (1001) docker     (127)    12396 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/iotwireless/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.192086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/ivs/
+-rw-r--r--   0 runner    (1001) docker     (127)    13002 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/ivs/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.192086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/ivs-realtime/
+-rw-r--r--   0 runner    (1001) docker     (127)    10586 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/ivs-realtime/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.192086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/ivschat/
+-rw-r--r--   0 runner    (1001) docker     (127)    11364 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/ivschat/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.192086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/kafka/
+-rw-r--r--   0 runner    (1001) docker     (127)    20270 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/kafka/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.192086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/kafkaconnect/
+-rw-r--r--   0 runner    (1001) docker     (127)    17076 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/kafkaconnect/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.192086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/kendra/
+-rw-r--r--   0 runner    (1001) docker     (127)    14778 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/kendra/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.192086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/kendra-ranking/
+-rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/kendra-ranking/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.192086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/keyspaces/
+-rw-r--r--   0 runner    (1001) docker     (127)    19121 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/keyspaces/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.192086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/kinesis/
+-rw-r--r--   0 runner    (1001) docker     (127)    82124 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/kinesis/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.192086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/kinesis-video-archived-media/
+-rw-r--r--   0 runner    (1001) docker     (127)    17076 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/kinesis-video-archived-media/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.192086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/kinesis-video-media/
+-rw-r--r--   0 runner    (1001) docker     (127)    17076 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/kinesis-video-media/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.192086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/kinesis-video-signaling/
+-rw-r--r--   0 runner    (1001) docker     (127)    17076 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/kinesis-video-signaling/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.192086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/kinesis-video-webrtc-storage/
+-rw-r--r--   0 runner    (1001) docker     (127)    10602 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/kinesis-video-webrtc-storage/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.192086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/kinesisanalytics/
+-rw-r--r--   0 runner    (1001) docker     (127)    20264 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/kinesisanalytics/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.192086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/kinesisanalyticsv2/
+-rw-r--r--   0 runner    (1001) docker     (127)    20264 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/kinesisanalyticsv2/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.192086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/kinesisvideo/
+-rw-r--r--   0 runner    (1001) docker     (127)    17076 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/kinesisvideo/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.192086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/kms/
+-rw-r--r--   0 runner    (1001) docker     (127)    30432 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/kms/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.192086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/lakeformation/
+-rw-r--r--   0 runner    (1001) docker     (127)    21882 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/lakeformation/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.192086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/lambda/
+-rw-r--r--   0 runner    (1001) docker     (127)    31675 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/lambda/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.192086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/launch-wizard/
+-rw-r--r--   0 runner    (1001) docker     (127)    10977 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/launch-wizard/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.192086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/lex-models/
+-rw-r--r--   0 runner    (1001) docker     (127)    14894 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/lex-models/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.192086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/lex-runtime/
+-rw-r--r--   0 runner    (1001) docker     (127)    16869 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/lex-runtime/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.196086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/lexv2-models/
+-rw-r--r--   0 runner    (1001) docker     (127)    14969 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/lexv2-models/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.196086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/lexv2-runtime/
+-rw-r--r--   0 runner    (1001) docker     (127)    14995 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/lexv2-runtime/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.196086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/license-manager/
+-rw-r--r--   0 runner    (1001) docker     (127)    22410 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/license-manager/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.196086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/license-manager-linux-subscriptions/
+-rw-r--r--   0 runner    (1001) docker     (127)    10970 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/license-manager-linux-subscriptions/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.196086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/license-manager-user-subscriptions/
+-rw-r--r--   0 runner    (1001) docker     (127)    10954 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/license-manager-user-subscriptions/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.196086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/lightsail/
+-rw-r--r--   0 runner    (1001) docker     (127)    16137 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/lightsail/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.196086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/location/
+-rw-r--r--   0 runner    (1001) docker     (127)    10458 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/location/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.196086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/logs/
+-rw-r--r--   0 runner    (1001) docker     (127)    22354 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/logs/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.196086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/lookoutequipment/
+-rw-r--r--   0 runner    (1001) docker     (127)    11541 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/lookoutequipment/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.196086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/lookoutmetrics/
+-rw-r--r--   0 runner    (1001) docker     (127)    14115 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/lookoutmetrics/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.196086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/lookoutvision/
+-rw-r--r--   0 runner    (1001) docker     (127)    13219 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/lookoutvision/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.196086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/m2/
+-rw-r--r--   0 runner    (1001) docker     (127)    12971 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/m2/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.196086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/machinelearning/
+-rw-r--r--   0 runner    (1001) docker     (127)    11079 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/machinelearning/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.196086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/macie2/
+-rw-r--r--   0 runner    (1001) docker     (127)    20283 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/macie2/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.196086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/managedblockchain/
+-rw-r--r--   0 runner    (1001) docker     (127)    12882 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/managedblockchain/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.196086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/managedblockchain-query/
+-rw-r--r--   0 runner    (1001) docker     (127)    10778 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/managedblockchain-query/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.196086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/marketplace-agreement/
+-rw-r--r--   0 runner    (1001) docker     (127)    10746 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/marketplace-agreement/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.196086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/marketplace-catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)    10714 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/marketplace-catalog/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.196086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/marketplace-deployment/
+-rw-r--r--   0 runner    (1001) docker     (127)    10762 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/marketplace-deployment/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.196086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/marketplace-entitlement/
+-rw-r--r--   0 runner    (1001) docker     (127)    11233 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/marketplace-entitlement/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.196086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/marketplacecommerceanalytics/
+-rw-r--r--   0 runner    (1001) docker     (127)    10858 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/marketplacecommerceanalytics/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.196086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/mediaconnect/
+-rw-r--r--   0 runner    (1001) docker     (127)    17067 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/mediaconnect/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.196086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/mediaconvert/
+-rw-r--r--   0 runner    (1001) docker     (127)    20124 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/mediaconvert/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.196086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/medialive/
+-rw-r--r--   0 runner    (1001) docker     (127)    16980 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/medialive/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.196086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/mediapackage/
+-rw-r--r--   0 runner    (1001) docker     (127)    16641 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/mediapackage/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.196086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/mediapackage-vod/
+-rw-r--r--   0 runner    (1001) docker     (127)    16761 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/mediapackage-vod/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.196086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/mediapackagev2/
+-rw-r--r--   0 runner    (1001) docker     (127)    10634 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/mediapackagev2/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.196086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/mediastore/
+-rw-r--r--   0 runner    (1001) docker     (127)    14019 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/mediastore/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.196086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/mediastore-data/
+-rw-r--r--   0 runner    (1001) docker     (127)    14139 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/mediastore-data/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.196086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/mediatailor/
+-rw-r--r--   0 runner    (1001) docker     (127)    13278 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/mediatailor/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.196086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/medical-imaging/
+-rw-r--r--   0 runner    (1001) docker     (127)    10650 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/medical-imaging/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.196086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/memorydb/
+-rw-r--r--   0 runner    (1001) docker     (127)    18197 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/memorydb/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.196086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/meteringmarketplace/
+-rw-r--r--   0 runner    (1001) docker     (127)    20413 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/meteringmarketplace/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.196086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/mgh/
+-rw-r--r--   0 runner    (1001) docker     (127)    13157 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/mgh/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.196086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/mgn/
+-rw-r--r--   0 runner    (1001) docker     (127)    18906 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/mgn/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.196086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/migration-hub-refactor-spaces/
+-rw-r--r--   0 runner    (1001) docker     (127)    10650 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/migration-hub-refactor-spaces/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.200086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/migrationhub-config/
+-rw-r--r--   0 runner    (1001) docker     (127)    10714 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/migrationhub-config/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.200086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/migrationhuborchestrator/
+-rw-r--r--   0 runner    (1001) docker     (127)    10810 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/migrationhuborchestrator/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.200086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/migrationhubstrategy/
+-rw-r--r--   0 runner    (1001) docker     (127)    13395 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/migrationhubstrategy/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.200086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/mobile/
+-rw-r--r--   0 runner    (1001) docker     (127)    10506 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/mobile/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.200086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/mq/
+-rw-r--r--   0 runner    (1001) docker     (127)    21851 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/mq/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.200086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/mturk/
+-rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/mturk/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.200086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/mwaa/
+-rw-r--r--   0 runner    (1001) docker     (127)    16500 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/mwaa/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.200086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/neptune/
+-rw-r--r--   0 runner    (1001) docker     (127)    23114 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/neptune/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.200086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/neptune-graph/
+-rw-r--r--   0 runner    (1001) docker     (127)    35316 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/neptune-graph/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.200086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/neptunedata/
+-rw-r--r--   0 runner    (1001) docker     (127)    10570 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/neptunedata/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.200086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/network-firewall/
+-rw-r--r--   0 runner    (1001) docker     (127)    22002 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/network-firewall/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.200086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/networkmanager/
+-rw-r--r--   0 runner    (1001) docker     (127)    12964 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/networkmanager/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.200086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/networkmonitor/
+-rw-r--r--   0 runner    (1001) docker     (127)    10634 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/networkmonitor/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.200086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/nimble/
+-rw-r--r--   0 runner    (1001) docker     (127)    12645 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/nimble/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.200086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/oam/
+-rw-r--r--   0 runner    (1001) docker     (127)    10458 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/oam/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.200086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/omics/
+-rw-r--r--   0 runner    (1001) docker     (127)    10490 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/omics/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.200086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/opensearch/
+-rw-r--r--   0 runner    (1001) docker     (127)    22279 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/opensearch/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.200086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/opensearchserverless/
+-rw-r--r--   0 runner    (1001) docker     (127)    10849 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/opensearchserverless/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.200086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/opsworks/
+-rw-r--r--   0 runner    (1001) docker     (127)    16527 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/opsworks/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.200086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/opsworkscm/
+-rw-r--r--   0 runner    (1001) docker     (127)    14040 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/opsworkscm/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.200086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/organizations/
+-rw-r--r--   0 runner    (1001) docker     (127)    17605 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/organizations/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.200086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/osis/
+-rw-r--r--   0 runner    (1001) docker     (127)    10474 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/osis/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.200086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/outposts/
+-rw-r--r--   0 runner    (1001) docker     (127)    21656 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/outposts/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.200086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/panorama/
+-rw-r--r--   0 runner    (1001) docker     (127)    10538 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/panorama/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.200086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/payment-cryptography/
+-rw-r--r--   0 runner    (1001) docker     (127)    10938 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/payment-cryptography/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.200086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/payment-cryptography-data/
+-rw-r--r--   0 runner    (1001) docker     (127)    10890 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/payment-cryptography-data/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.200086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/pca-connector-ad/
+-rw-r--r--   0 runner    (1001) docker     (127)    10666 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/pca-connector-ad/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.200086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/personalize/
+-rw-r--r--   0 runner    (1001) docker     (127)    14917 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/personalize/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.200086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/personalize-events/
+-rw-r--r--   0 runner    (1001) docker     (127)    10698 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/personalize-events/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.200086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/personalize-runtime/
+-rw-r--r--   0 runner    (1001) docker     (127)    10714 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/personalize-runtime/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.200086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/pi/
+-rw-r--r--   0 runner    (1001) docker     (127)    19304 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/pi/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.200086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/pinpoint/
+-rw-r--r--   0 runner    (1001) docker     (127)    16135 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/pinpoint/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.200086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/pinpoint-email/
+-rw-r--r--   0 runner    (1001) docker     (127)    19846 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/pinpoint-email/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.200086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/pinpoint-sms-voice/
+-rw-r--r--   0 runner    (1001) docker     (127)    10081 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/pinpoint-sms-voice/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.200086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/pinpoint-sms-voice-v2/
+-rw-r--r--   0 runner    (1001) docker     (127)    14862 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/pinpoint-sms-voice-v2/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.200086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/pipes/
+-rw-r--r--   0 runner    (1001) docker     (127)    10490 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/pipes/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.204086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/polly/
+-rw-r--r--   0 runner    (1001) docker     (127)    20690 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/polly/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.204086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/pricing/
+-rw-r--r--   0 runner    (1001) docker     (127)    11014 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/pricing/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.204086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/privatenetworks/
+-rw-r--r--   0 runner    (1001) docker     (127)    10666 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/privatenetworks/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.204086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/proton/
+-rw-r--r--   0 runner    (1001) docker     (127)    12201 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/proton/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.204086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/qbusiness/
+-rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/qbusiness/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.204086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/qconnect/
+-rw-r--r--   0 runner    (1001) docker     (127)    10506 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/qconnect/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.204086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/qldb/
+-rw-r--r--   0 runner    (1001) docker     (127)    16004 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/qldb/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.204086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/qldb-session/
+-rw-r--r--   0 runner    (1001) docker     (127)    15798 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/qldb-session/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.204086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/quicksight/
+-rw-r--r--   0 runner    (1001) docker     (127)    16987 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/quicksight/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.204086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/ram/
+-rw-r--r--   0 runner    (1001) docker     (127)    22313 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/ram/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.204086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/rbin/
+-rw-r--r--   0 runner    (1001) docker     (127)    18942 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/rbin/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.204086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/rds/
+-rw-r--r--   0 runner    (1001) docker     (127)    22739 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/rds/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.204086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/rds-data/
+-rw-r--r--   0 runner    (1001) docker     (127)    10538 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/rds-data/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.204086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/redshift/
+-rw-r--r--   0 runner    (1001) docker     (127)    22964 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/redshift/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.204086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/redshift-data/
+-rw-r--r--   0 runner    (1001) docker     (127)    10618 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/redshift-data/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.204086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/redshift-serverless/
+-rw-r--r--   0 runner    (1001) docker     (127)    15116 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/redshift-serverless/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.204086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/rekognition/
+-rw-r--r--   0 runner    (1001) docker     (127)    18365 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/rekognition/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.204086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/repostspace/
+-rw-r--r--   0 runner    (1001) docker     (127)    10586 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/repostspace/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.204086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/resiliencehub/
+-rw-r--r--   0 runner    (1001) docker     (127)    18824 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/resiliencehub/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.204086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/resource-explorer-2/
+-rw-r--r--   0 runner    (1001) docker     (127)    10714 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/resource-explorer-2/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.204086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/resource-groups/
+-rw-r--r--   0 runner    (1001) docker     (127)    22400 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/resource-groups/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.204086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/resourcegroupstaggingapi/
+-rw-r--r--   0 runner    (1001) docker     (127)    20358 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/resourcegroupstaggingapi/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.204086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/robomaker/
+-rw-r--r--   0 runner    (1001) docker     (127)    13566 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/robomaker/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.204086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/rolesanywhere/
+-rw-r--r--   0 runner    (1001) docker     (127)    18406 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/rolesanywhere/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.204086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/route53/
+-rw-r--r--   0 runner    (1001) docker     (127)    19968 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/route53/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.204086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/route53-recovery-cluster/
+-rw-r--r--   0 runner    (1001) docker     (127)    10794 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/route53-recovery-cluster/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.204086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/route53-recovery-control-config/
+-rw-r--r--   0 runner    (1001) docker     (127)    11731 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/route53-recovery-control-config/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.204086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/route53-recovery-readiness/
+-rw-r--r--   0 runner    (1001) docker     (127)    10826 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/route53-recovery-readiness/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.204086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/route53domains/
+-rw-r--r--   0 runner    (1001) docker     (127)    10634 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/route53domains/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.204086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/route53profiles/
+-rw-r--r--   0 runner    (1001) docker     (127)    10650 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/route53profiles/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.204086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/route53resolver/
+-rw-r--r--   0 runner    (1001) docker     (127)    21104 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/route53resolver/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.204086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/rum/
+-rw-r--r--   0 runner    (1001) docker     (127)    14268 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/rum/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.204086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/s3/
+-rw-r--r--   0 runner    (1001) docker     (127)   321152 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/s3/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.208086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/s3control/
+-rw-r--r--   0 runner    (1001) docker     (127)   148079 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/s3control/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.208086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/s3outposts/
+-rw-r--r--   0 runner    (1001) docker     (127)    19194 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/s3outposts/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.208086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/sagemaker/
+-rw-r--r--   0 runner    (1001) docker     (127)    21872 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/sagemaker/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.208086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/sagemaker-a2i-runtime/
+-rw-r--r--   0 runner    (1001) docker     (127)    10746 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/sagemaker-a2i-runtime/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.208086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/sagemaker-edge/
+-rw-r--r--   0 runner    (1001) docker     (127)    12798 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/sagemaker-edge/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.208086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/sagemaker-featurestore-runtime/
+-rw-r--r--   0 runner    (1001) docker     (127)    10890 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/sagemaker-featurestore-runtime/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.208086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/sagemaker-geospatial/
+-rw-r--r--   0 runner    (1001) docker     (127)    10730 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/sagemaker-geospatial/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.208086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/sagemaker-metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)    10682 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/sagemaker-metrics/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.208086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/sagemaker-runtime/
+-rw-r--r--   0 runner    (1001) docker     (127)    22040 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/sagemaker-runtime/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.208086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/savingsplans/
+-rw-r--r--   0 runner    (1001) docker     (127)    11728 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/savingsplans/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.208086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)    10554 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/scheduler/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.208086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    17342 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/schemas/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.208086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/sdb/
+-rw-r--r--   0 runner    (1001) docker     (127)    14829 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/sdb/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.208086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/secretsmanager/
+-rw-r--r--   0 runner    (1001) docker     (127)    22819 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/secretsmanager/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.208086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/securityhub/
+-rw-r--r--   0 runner    (1001) docker     (127)    22238 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/securityhub/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.208086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/securitylake/
+-rw-r--r--   0 runner    (1001) docker     (127)    10602 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/securitylake/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.208086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/serverlessrepo/
+-rw-r--r--   0 runner    (1001) docker     (127)    19316 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/serverlessrepo/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.208086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/service-quotas/
+-rw-r--r--   0 runner    (1001) docker     (127)    20579 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/service-quotas/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.208086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/servicecatalog/
+-rw-r--r--   0 runner    (1001) docker     (127)    22367 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/servicecatalog/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.208086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/servicecatalog-appregistry/
+-rw-r--r--   0 runner    (1001) docker     (127)    22417 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/servicecatalog-appregistry/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.208086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/servicediscovery/
+-rw-r--r--   0 runner    (1001) docker     (127)    22005 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/servicediscovery/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.208086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/ses/
+-rw-r--r--   0 runner    (1001) docker     (127)    19846 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/ses/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.208086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/sesv2/
+-rw-r--r--   0 runner    (1001) docker     (127)    19846 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/sesv2/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.208086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/shield/
+-rw-r--r--   0 runner    (1001) docker     (127)    12765 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/shield/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.208086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/signer/
+-rw-r--r--   0 runner    (1001) docker     (127)    10506 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/signer/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.208086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/simspaceweaver/
+-rw-r--r--   0 runner    (1001) docker     (127)    10634 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/simspaceweaver/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.208086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/sms/
+-rw-r--r--   0 runner    (1001) docker     (127)    21030 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/sms/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.208086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/sms-voice/
+-rw-r--r--   0 runner    (1001) docker     (127)    10081 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/sms-voice/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.208086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/snow-device-management/
+-rw-r--r--   0 runner    (1001) docker     (127)    10762 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/snow-device-management/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.208086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/snowball/
+-rw-r--r--   0 runner    (1001) docker     (127)    26886 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/snowball/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.208086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/sns/
+-rw-r--r--   0 runner    (1001) docker     (127)    22310 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/sns/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.208086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/sqs/
+-rw-r--r--   0 runner    (1001) docker     (127)    21883 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/sqs/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.212086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/ssm/
+-rw-r--r--   0 runner    (1001) docker     (127)    22313 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/ssm/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.212086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/ssm-contacts/
+-rw-r--r--   0 runner    (1001) docker     (127)    10602 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/ssm-contacts/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.212086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/ssm-incidents/
+-rw-r--r--   0 runner    (1001) docker     (127)    17107 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/ssm-incidents/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.212086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/ssm-sap/
+-rw-r--r--   0 runner    (1001) docker     (127)    10522 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/ssm-sap/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.212086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/sso/
+-rw-r--r--   0 runner    (1001) docker     (127)    18738 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/sso/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.212086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/sso-admin/
+-rw-r--r--   0 runner    (1001) docker     (127)    18920 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/sso-admin/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.212086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/sso-oidc/
+-rw-r--r--   0 runner    (1001) docker     (127)    18528 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/sso-oidc/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.212086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/stepfunctions/
+-rw-r--r--   0 runner    (1001) docker     (127)    22447 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/stepfunctions/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.212086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/storagegateway/
+-rw-r--r--   0 runner    (1001) docker     (127)    22807 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/storagegateway/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.212086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/sts/
+-rw-r--r--   0 runner    (1001) docker     (127)    43190 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/sts/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.212086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/supplychain/
+-rw-r--r--   0 runner    (1001) docker     (127)    10458 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/supplychain/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.212086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/support/
+-rw-r--r--   0 runner    (1001) docker     (127)    17409 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/support/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.212086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/support-app/
+-rw-r--r--   0 runner    (1001) docker     (127)    10570 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/support-app/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.212086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/swf/
+-rw-r--r--   0 runner    (1001) docker     (127)    22310 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/swf/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.212086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/synthetics/
+-rw-r--r--   0 runner    (1001) docker     (127)    22195 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/synthetics/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.212086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/textract/
+-rw-r--r--   0 runner    (1001) docker     (127)    18248 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/textract/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.212086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/timestream-influxdb/
+-rw-r--r--   0 runner    (1001) docker     (127)    10714 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/timestream-influxdb/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.212086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/timestream-query/
+-rw-r--r--   0 runner    (1001) docker     (127)    10666 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/timestream-query/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.212086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/timestream-write/
+-rw-r--r--   0 runner    (1001) docker     (127)    11561 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/timestream-write/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.212086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/tnb/
+-rw-r--r--   0 runner    (1001) docker     (127)    10458 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/tnb/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.212086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/transcribe/
+-rw-r--r--   0 runner    (1001) docker     (127)    21332 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/transcribe/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.212086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/transfer/
+-rw-r--r--   0 runner    (1001) docker     (127)    22106 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/transfer/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.212086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/translate/
+-rw-r--r--   0 runner    (1001) docker     (127)    18708 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/translate/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.212086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/trustedadvisor/
+-rw-r--r--   0 runner    (1001) docker     (127)    10634 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/trustedadvisor/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.212086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/verifiedpermissions/
+-rw-r--r--   0 runner    (1001) docker     (127)    10714 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/verifiedpermissions/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.212086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/voice-id/
+-rw-r--r--   0 runner    (1001) docker     (127)    13102 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/voice-id/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.212086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/vpc-lattice/
+-rw-r--r--   0 runner    (1001) docker     (127)    10586 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/vpc-lattice/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.212086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/waf/
+-rw-r--r--   0 runner    (1001) docker     (127)    12659 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/waf/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.212086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/waf-regional/
+-rw-r--r--   0 runner    (1001) docker     (127)    30573 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/waf-regional/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.212086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/wafv2/
+-rw-r--r--   0 runner    (1001) docker     (127)    30139 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/wafv2/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.212086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/wellarchitected/
+-rw-r--r--   0 runner    (1001) docker     (127)    18030 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/wellarchitected/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.212086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/wisdom/
+-rw-r--r--   0 runner    (1001) docker     (127)    12645 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/wisdom/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.212086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/workdocs/
+-rw-r--r--   0 runner    (1001) docker     (127)    13118 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/workdocs/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.212086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/worklink/
+-rw-r--r--   0 runner    (1001) docker     (127)    10538 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/worklink/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.216086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/workmail/
+-rw-r--r--   0 runner    (1001) docker     (127)    11382 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/workmail/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.216086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/workmailmessageflow/
+-rw-r--r--   0 runner    (1001) docker     (127)    10714 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/workmailmessageflow/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.216086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/workspaces/
+-rw-r--r--   0 runner    (1001) docker     (127)    17059 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/workspaces/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.216086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/workspaces-thin-client/
+-rw-r--r--   0 runner    (1001) docker     (127)    10570 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/workspaces-thin-client/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.216086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/workspaces-web/
+-rw-r--r--   0 runner    (1001) docker     (127)    11490 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/workspaces-web/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.216086 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/xray/
+-rw-r--r--   0 runner    (1001) docker     (127)    21937 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/xray/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.216086 botocore-a-la-carte-1.34.99/tests/functional/leak/
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/leak/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/leak/test_resource_leaks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.216086 botocore-a-la-carte-1.34.99/tests/functional/models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.140086 botocore-a-la-carte-1.34.99/tests/functional/models/custom-acm/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.216086 botocore-a-la-carte-1.34.99/tests/functional/models/custom-acm/2015-12-08/
+-rw-r--r--   0 runner    (1001) docker     (127)    14695 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/models/custom-acm/2015-12-08/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/models/custom-acm/2015-12-08/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/models/custom-acm/2015-12-08/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    57976 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/models/custom-acm/2015-12-08/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/models/custom-acm/2015-12-08/waiters-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)    77688 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/models/endpoints.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4358 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/models/sdk-default-configuration.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.140086 botocore-a-la-carte-1.34.99/tests/functional/models/test-discovery-endpoint/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.216086 botocore-a-la-carte-1.34.99/tests/functional/models/test-discovery-endpoint/2020-08-20/
+-rw-r--r--   0 runner    (1001) docker     (127)     4677 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/models/test-discovery-endpoint/2020-08-20/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.216086 botocore-a-la-carte-1.34.99/tests/functional/retries/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/retries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3928 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/retries/test_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/retries/test_quota.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/test_alias.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/test_apigateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/test_client_class_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/test_client_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/test_cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/test_cloudsearchdomain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/test_cognito_idp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/test_compress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4831 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/test_config_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19034 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/test_context_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44807 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16098 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/test_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/test_docdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/test_dynamodb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5692 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/test_ec2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11682 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/test_endpoint_rulesets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4841 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/test_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14597 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/test_event_alias.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12116 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/test_eventbridge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/test_h2_required.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5235 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/test_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/test_importexport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/test_iot_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/test_kinesis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/test_lex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/test_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/test_machinelearning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/test_model_backcompat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/test_model_completeness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6769 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/test_modeled_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/test_mturk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/test_neptune.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8288 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/test_paginate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11866 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/test_paginator_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/test_public_apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/test_qbusiness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4117 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/test_rds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28286 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/test_regions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/test_response_shadowing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14043 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/test_retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/test_route53.py
+-rw-r--r--   0 runner    (1001) docker     (127)   133985 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/test_s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/test_s3_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18188 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/test_s3_control_redirects.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11135 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/test_s3express.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/test_sagemaker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/test_service_alias.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/test_service_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4558 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/test_six_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/test_six_threading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/test_sqs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12521 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/test_sts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14292 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/test_stub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/test_tagged_unions_unknown.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11554 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/test_useragent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7380 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/test_waiter_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.216086 botocore-a-la-carte-1.34.99/tests/functional/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/functional/utils/credentialprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.220086 botocore-a-la-carte-1.34.99/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/integration/test-credentials
+-rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/integration/test_apigateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6452 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/integration/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10489 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/integration/test_client_http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/integration/test_cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/integration/test_cognito_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14122 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/integration/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/integration/test_ec2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/integration/test_elastictranscoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/integration/test_emr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3038 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/integration/test_glacier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/integration/test_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/integration/test_rds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/integration/test_route53.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53990 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/integration/test_s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/integration/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12697 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/integration/test_smoke.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/integration/test_sts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/integration/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/integration/test_waiters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.224086 botocore-a-la-carte-1.34.99/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.224086 botocore-a-la-carte-1.34.99/tests/unit/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.224086 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/NOTICE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.224086 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-header-key-duplicate/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-header-key-duplicate/get-header-key-duplicate.authz
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-header-key-duplicate/get-header-key-duplicate.creq
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-header-key-duplicate/get-header-key-duplicate.req
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-header-key-duplicate/get-header-key-duplicate.sreq
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-header-key-duplicate/get-header-key-duplicate.sts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.224086 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-header-value-multiline/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-header-value-multiline/get-header-value-multiline.authz
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-header-value-multiline/get-header-value-multiline.creq
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-header-value-multiline/get-header-value-multiline.req
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-header-value-multiline/get-header-value-multiline.sreq
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-header-value-multiline/get-header-value-multiline.sts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.228086 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-header-value-order/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-header-value-order/get-header-value-order.authz
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-header-value-order/get-header-value-order.creq
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-header-value-order/get-header-value-order.req
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-header-value-order/get-header-value-order.sreq
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-header-value-order/get-header-value-order.sts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.228086 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-header-value-trim/
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-header-value-trim/get-header-value-trim.authz
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-header-value-trim/get-header-value-trim.creq
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-header-value-trim/get-header-value-trim.req
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-header-value-trim/get-header-value-trim.sreq
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-header-value-trim/get-header-value-trim.sts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.228086 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-unreserved/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-unreserved/get-unreserved.authz
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-unreserved/get-unreserved.creq
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-unreserved/get-unreserved.req
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-unreserved/get-unreserved.sreq
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-unreserved/get-unreserved.sts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.228086 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-utf8/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-utf8/get-utf8.authz
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-utf8/get-utf8.creq
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-utf8/get-utf8.req
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-utf8/get-utf8.sreq
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-utf8/get-utf8.sts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.228086 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-vanilla/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-vanilla/get-vanilla.authz
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-vanilla/get-vanilla.creq
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-vanilla/get-vanilla.req
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-vanilla/get-vanilla.sreq
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-vanilla/get-vanilla.sts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.228086 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-vanilla-empty-query-key/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-vanilla-empty-query-key/get-vanilla-empty-query-key.authz
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-vanilla-empty-query-key/get-vanilla-empty-query-key.creq
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-vanilla-empty-query-key/get-vanilla-empty-query-key.req
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-vanilla-empty-query-key/get-vanilla-empty-query-key.sreq
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-vanilla-empty-query-key/get-vanilla-empty-query-key.sts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.228086 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-vanilla-query/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-vanilla-query/get-vanilla-query.authz
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-vanilla-query/get-vanilla-query.creq
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-vanilla-query/get-vanilla-query.req
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-vanilla-query/get-vanilla-query.sreq
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-vanilla-query/get-vanilla-query.sts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.228086 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-encoded/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-encoded/get-vanilla-query-order-encoded.authz
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-encoded/get-vanilla-query-order-encoded.creq
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-encoded/get-vanilla-query-order-encoded.req
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-encoded/get-vanilla-query-order-encoded.sreq
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-encoded/get-vanilla-query-order-encoded.sts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.228086 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-key/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-key/get-vanilla-query-order-key.authz
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-key/get-vanilla-query-order-key.creq
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-key/get-vanilla-query-order-key.req
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-key/get-vanilla-query-order-key.sreq
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-key/get-vanilla-query-order-key.sts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.232086 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-key-case/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-key-case/get-vanilla-query-order-key-case.authz
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-key-case/get-vanilla-query-order-key-case.creq
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-key-case/get-vanilla-query-order-key-case.req
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-key-case/get-vanilla-query-order-key-case.sreq
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-key-case/get-vanilla-query-order-key-case.sts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.232086 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-value/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-value/get-vanilla-query-order-value.authz
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-value/get-vanilla-query-order-value.creq
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-value/get-vanilla-query-order-value.req
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-value/get-vanilla-query-order-value.sreq
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-value/get-vanilla-query-order-value.sts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.232086 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-vanilla-query-unreserved/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-vanilla-query-unreserved/get-vanilla-query-unreserved.authz
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-vanilla-query-unreserved/get-vanilla-query-unreserved.creq
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-vanilla-query-unreserved/get-vanilla-query-unreserved.req
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-vanilla-query-unreserved/get-vanilla-query-unreserved.sreq
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-vanilla-query-unreserved/get-vanilla-query-unreserved.sts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.232086 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-vanilla-utf8-query/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-vanilla-utf8-query/get-vanilla-utf8-query.authz
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-vanilla-utf8-query/get-vanilla-utf8-query.creq
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-vanilla-utf8-query/get-vanilla-utf8-query.req
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-vanilla-utf8-query/get-vanilla-utf8-query.sreq
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-vanilla-utf8-query/get-vanilla-utf8-query.sts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.232086 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-vanilla-with-session-token/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-vanilla-with-session-token/get-vanilla-with-session-token.authz
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-vanilla-with-session-token/get-vanilla-with-session-token.creq
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-vanilla-with-session-token/get-vanilla-with-session-token.req
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-vanilla-with-session-token/get-vanilla-with-session-token.sreq
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/get-vanilla-with-session-token/get-vanilla-with-session-token.sts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.232086 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/normalize-path/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.232086 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/normalize-path/get-relative/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/normalize-path/get-relative/get-relative.authz
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/normalize-path/get-relative/get-relative.creq
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/normalize-path/get-relative/get-relative.req
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/normalize-path/get-relative/get-relative.sreq
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/normalize-path/get-relative/get-relative.sts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.232086 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/normalize-path/get-relative-relative/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/normalize-path/get-relative-relative/get-relative-relative.authz
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/normalize-path/get-relative-relative/get-relative-relative.creq
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/normalize-path/get-relative-relative/get-relative-relative.req
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/normalize-path/get-relative-relative/get-relative-relative.sreq
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/normalize-path/get-relative-relative/get-relative-relative.sts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.232086 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/normalize-path/get-slash/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/normalize-path/get-slash/get-slash.authz
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/normalize-path/get-slash/get-slash.creq
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/normalize-path/get-slash/get-slash.req
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/normalize-path/get-slash/get-slash.sreq
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/normalize-path/get-slash/get-slash.sts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.236086 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/normalize-path/get-slash-dot-slash/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/normalize-path/get-slash-dot-slash/get-slash-dot-slash.authz
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/normalize-path/get-slash-dot-slash/get-slash-dot-slash.creq
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/normalize-path/get-slash-dot-slash/get-slash-dot-slash.req
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/normalize-path/get-slash-dot-slash/get-slash-dot-slash.sreq
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/normalize-path/get-slash-dot-slash/get-slash-dot-slash.sts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.236086 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/normalize-path/get-slash-pointless-dot/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/normalize-path/get-slash-pointless-dot/get-slash-pointless-dot.authz
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/normalize-path/get-slash-pointless-dot/get-slash-pointless-dot.creq
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/normalize-path/get-slash-pointless-dot/get-slash-pointless-dot.req
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/normalize-path/get-slash-pointless-dot/get-slash-pointless-dot.sreq
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/normalize-path/get-slash-pointless-dot/get-slash-pointless-dot.sts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.236086 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/normalize-path/get-slashes/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/normalize-path/get-slashes/get-slashes.authz
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/normalize-path/get-slashes/get-slashes.creq
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/normalize-path/get-slashes/get-slashes.req
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/normalize-path/get-slashes/get-slashes.sreq
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/normalize-path/get-slashes/get-slashes.sts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.236086 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/normalize-path/get-space/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/normalize-path/get-space/get-space.authz
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/normalize-path/get-space/get-space.creq
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/normalize-path/get-space/get-space.req
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/normalize-path/get-space/get-space.sreq
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/normalize-path/get-space/get-space.sts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.236086 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/normalize-path/get-special-character/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/normalize-path/get-special-character/get-special-character.authz
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/normalize-path/get-special-character/get-special-character.creq
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/normalize-path/get-special-character/get-special-character.req
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/normalize-path/get-special-character/get-special-character.sreq
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/normalize-path/get-special-character/get-special-character.sts
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/normalize-path/normalize-path.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.236086 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/post-header-key-case/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/post-header-key-case/post-header-key-case.authz
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/post-header-key-case/post-header-key-case.creq
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/post-header-key-case/post-header-key-case.req
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/post-header-key-case/post-header-key-case.sreq
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/post-header-key-case/post-header-key-case.sts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.236086 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/post-header-key-sort/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/post-header-key-sort/post-header-key-sort.authz
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/post-header-key-sort/post-header-key-sort.creq
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/post-header-key-sort/post-header-key-sort.req
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/post-header-key-sort/post-header-key-sort.sreq
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/post-header-key-sort/post-header-key-sort.sts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.236086 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/post-header-value-case/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/post-header-value-case/post-header-value-case.authz
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/post-header-value-case/post-header-value-case.creq
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/post-header-value-case/post-header-value-case.req
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/post-header-value-case/post-header-value-case.sreq
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/post-header-value-case/post-header-value-case.sts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.236086 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/post-sts-token/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.240086 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/post-sts-token/post-sts-header-after/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/post-sts-token/post-sts-header-after/post-sts-header-after.authz
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/post-sts-token/post-sts-header-after/post-sts-header-after.creq
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/post-sts-token/post-sts-header-after/post-sts-header-after.req
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/post-sts-token/post-sts-header-after/post-sts-header-after.sreq
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/post-sts-token/post-sts-header-after/post-sts-header-after.sts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.240086 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/post-sts-token/post-sts-header-before/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/post-sts-token/post-sts-header-before/post-sts-header-before.authz
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/post-sts-token/post-sts-header-before/post-sts-header-before.creq
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/post-sts-token/post-sts-header-before/post-sts-header-before.req
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/post-sts-token/post-sts-header-before/post-sts-header-before.sreq
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/post-sts-token/post-sts-header-before/post-sts-header-before.sts
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/post-sts-token/readme.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.240086 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/post-vanilla/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/post-vanilla/post-vanilla.authz
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/post-vanilla/post-vanilla.creq
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/post-vanilla/post-vanilla.req
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/post-vanilla/post-vanilla.sreq
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/post-vanilla/post-vanilla.sts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.240086 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/post-vanilla-empty-query-value/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/post-vanilla-empty-query-value/post-vanilla-empty-query-value.authz
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/post-vanilla-empty-query-value/post-vanilla-empty-query-value.creq
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/post-vanilla-empty-query-value/post-vanilla-empty-query-value.req
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/post-vanilla-empty-query-value/post-vanilla-empty-query-value.sreq
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/post-vanilla-empty-query-value/post-vanilla-empty-query-value.sts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.240086 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/post-vanilla-query/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/post-vanilla-query/post-vanilla-query.authz
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/post-vanilla-query/post-vanilla-query.creq
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/post-vanilla-query/post-vanilla-query.req
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/post-vanilla-query/post-vanilla-query.sreq
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/post-vanilla-query/post-vanilla-query.sts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.240086 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/post-x-www-form-urlencoded/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/post-x-www-form-urlencoded/post-x-www-form-urlencoded.authz
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/post-x-www-form-urlencoded/post-x-www-form-urlencoded.creq
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/post-x-www-form-urlencoded/post-x-www-form-urlencoded.req
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/post-x-www-form-urlencoded/post-x-www-form-urlencoded.sreq
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/post-x-www-form-urlencoded/post-x-www-form-urlencoded.sts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.240086 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/post-x-www-form-urlencoded-parameters/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/post-x-www-form-urlencoded-parameters/post-x-www-form-urlencoded-parameters.authz
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/post-x-www-form-urlencoded-parameters/post-x-www-form-urlencoded-parameters.creq
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/post-x-www-form-urlencoded-parameters/post-x-www-form-urlencoded-parameters.req
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/post-x-www-form-urlencoded-parameters/post-x-www-form-urlencoded-parameters.sreq
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/post-x-www-form-urlencoded-parameters/post-x-www-form-urlencoded-parameters.sts
+-rw-r--r--   0 runner    (1001) docker     (127)    45993 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/test_signers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6559 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/auth/test_sigv4.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.244086 botocore-a-la-carte-1.34.99/tests/unit/cfg/
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/cfg/aws_bad_profile
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/cfg/aws_config
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/cfg/aws_config_bad
+-rw-r--r--   0 runner    (1001) docker     (127)    51200 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/cfg/aws_config_badbytes
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/cfg/aws_config_nested
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/cfg/aws_config_nested_bad
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/cfg/aws_config_nocreds
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/cfg/aws_config_other
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/cfg/aws_credentials
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/cfg/aws_services_config
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/cfg/aws_sso_session_config
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/cfg/aws_third_config
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/cfg/boto_config
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/cfg/boto_config_empty
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/cfg/foo_config
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.244086 botocore-a-la-carte-1.34.99/tests/unit/crt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/crt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.244086 botocore-a-la-carte-1.34.99/tests/unit/crt/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/crt/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/crt/auth/test_crt_signers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/crt/auth/test_crt_sigv4.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.244086 botocore-a-la-carte-1.34.99/tests/unit/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.140086 botocore-a-la-carte-1.34.99/tests/unit/data/aws/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.244086 botocore-a-la-carte-1.34.99/tests/unit/data/aws/s3/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/data/aws/s3/2006-03-01.normal.json
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/data/baz.json
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/data/compressed.json.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.140086 botocore-a-la-carte-1.34.99/tests/unit/data/endpoints/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.244086 botocore-a-la-carte-1.34.99/tests/unit/data/endpoints/test-cases/
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/data/endpoints/test-cases/aws-region.json
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/data/endpoints/test-cases/default-values.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/data/endpoints/test-cases/eventbridge.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/data/endpoints/test-cases/fns.json
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/data/endpoints/test-cases/headers.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3725 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/data/endpoints/test-cases/is-virtual-hostable-s3-bucket.json
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/data/endpoints/test-cases/local-region-override.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/data/endpoints/test-cases/parse-arn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/data/endpoints/test-cases/parse-url.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/data/endpoints/test-cases/partition-fn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/data/endpoints/test-cases/substring.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/data/endpoints/test-cases/uri-encode.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/data/endpoints/test-cases/valid-hostlabel.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.248086 botocore-a-la-carte-1.34.99/tests/unit/data/endpoints/valid-rules/
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/data/endpoints/valid-rules/aws-region.json
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/data/endpoints/valid-rules/default-values.json
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/data/endpoints/valid-rules/deprecated-param.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8502 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/data/endpoints/valid-rules/eventbridge.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/data/endpoints/valid-rules/fns.json
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/data/endpoints/valid-rules/get-attr-type-inference.json
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/data/endpoints/valid-rules/headers.json
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/data/endpoints/valid-rules/is-virtual-hostable-s3-bucket.json
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/data/endpoints/valid-rules/local-region-override.json
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/data/endpoints/valid-rules/minimal-ruleset.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/data/endpoints/valid-rules/parse-arn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/data/endpoints/valid-rules/parse-url.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/data/endpoints/valid-rules/partition-fn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/data/endpoints/valid-rules/substring.json
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/data/endpoints/valid-rules/uri-encode.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/data/endpoints/valid-rules/valid-hostlabel.json
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/data/foo.json
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/data/non_ascii.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.248086 botocore-a-la-carte-1.34.99/tests/unit/data/someservice/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/data/someservice/2012-10-01.normal.json
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/data/someservice/2013-08-21.normal.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.248086 botocore-a-la-carte-1.34.99/tests/unit/data/sub/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/data/sub/fie.normal.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.140086 botocore-a-la-carte-1.34.99/tests/unit/data_overrides/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.248086 botocore-a-la-carte-1.34.99/tests/unit/data_overrides/someservice/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/data_overrides/someservice/2012-10-01.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.248086 botocore-a-la-carte-1.34.99/tests/unit/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     9486 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/docs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.248086 botocore-a-la-carte-1.34.99/tests/unit/docs/bcdoc/
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/docs/bcdoc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13206 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/docs/bcdoc/test_docstringparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6294 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/docs/bcdoc/test_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12421 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/docs/bcdoc/test_style.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/docs/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/docs/test_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/docs/test_docstring.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16138 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/docs/test_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15898 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/docs/test_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4110 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/docs/test_paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13495 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/docs/test_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4833 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/docs/test_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8454 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/docs/test_sharedexample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8470 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/docs/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/docs/test_waiter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.140086 botocore-a-la-carte-1.34.99/tests/unit/protocols/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.248086 botocore-a-la-carte-1.34.99/tests/unit/protocols/input/
+-rw-r--r--   0 runner    (1001) docker     (127)    12019 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/protocols/input/ec2.json
+-rw-r--r--   0 runner    (1001) docker     (127)    21711 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/protocols/input/json.json
+-rw-r--r--   0 runner    (1001) docker     (127)    23390 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/protocols/input/query.json
+-rw-r--r--   0 runner    (1001) docker     (127)    51262 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/protocols/input/rest-json.json
+-rw-r--r--   0 runner    (1001) docker     (127)    46773 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/protocols/input/rest-xml.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.248086 botocore-a-la-carte-1.34.99/tests/unit/protocols/output/
+-rw-r--r--   0 runner    (1001) docker     (127)    14002 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/protocols/output/ec2.json
+-rw-r--r--   0 runner    (1001) docker     (127)    19354 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/protocols/output/json.json
+-rw-r--r--   0 runner    (1001) docker     (127)    23397 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/protocols/output/query.json
+-rw-r--r--   0 runner    (1001) docker     (127)    29610 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/protocols/output/rest-json.json
+-rw-r--r--   0 runner    (1001) docker     (127)    31012 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/protocols/output/rest-xml.json
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/put_object_data
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.248086 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.140086 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/json/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.252086 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/json/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/json/errors/datapipeline-create-pipeline.json
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/json/errors/directconnect-delete-connection.json
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/json/errors/dynamodb-put-item.json
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/json/errors/elastictranscoder-delete-pipeline.json
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/json/errors/opsworks-delete-stack.json
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/json/errors/storagegateway-delete-gateway.json
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/json/errors/swf-deprecate-domain.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.252086 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/json/expected/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/json/expected/datapipeline-create-pipeline.json
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/json/expected/directconnect-delete-connection.json
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/json/expected/dynamodb-put-item.json
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/json/expected/elastictranscoder-delete-pipeline.json
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/json/expected/elastictranscoder-list-pipelines.json
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/json/expected/opsworks-delete-stack.json
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/json/expected/storagegateway-delete-gateway.json
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/json/expected/swf-deprecate-domain.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7442 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/test_response_parsing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.140086 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.252086 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/errors/autoscaling-delete-policy.json
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/errors/autoscaling-delete-policy.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/errors/cloudformation-cancel-update-stack.json
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/errors/cloudformation-cancel-update-stack.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/errors/cloudwatch-describe-alarm-history.json
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/errors/cloudwatch-describe-alarm-history.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/errors/ec2-describe-instances.json
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/errors/ec2-describe-instances.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/errors/elb-describe-load-balancers.json
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/errors/elb-describe-load-balancers.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/errors/iam-get-user.json
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/errors/iam-get-user.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/errors/importexport-get-status.json
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/errors/importexport-get-status.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/errors/rds-describe-db-instances.json
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/errors/rds-describe-db-instances.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/errors/route53-get-hosted-zone.json
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/errors/route53-get-hosted-zone.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/errors/s3-create-bucket.json
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/errors/s3-create-bucket.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/errors/s3-list-objects.json
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/errors/s3-list-objects.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/errors/ses-delete-identity.json
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/errors/ses-delete-identity.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/errors/sns-delete-topic.json
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/errors/sns-delete-topic.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/errors/sqs-delete-queue.json
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/errors/sts-get-session-token.json
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/errors/sts-get-session-token.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.296085 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/autoscaling-describe-adjustment-types.json
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/autoscaling-describe-adjustment-types.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/autoscaling-describe-auto-scaling-groups.json
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/autoscaling-describe-auto-scaling-groups.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/autoscaling-describe-auto-scaling-instances.json
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/autoscaling-describe-auto-scaling-instances.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/autoscaling-describe-auto-scaling-notification-types.json
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/autoscaling-describe-auto-scaling-notification-types.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/autoscaling-describe-launch-configurations.json
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/autoscaling-describe-launch-configurations.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/autoscaling-describe-metric-collection-types.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/autoscaling-describe-metric-collection-types.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/autoscaling-describe-notification-configurations.json
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/autoscaling-describe-notification-configurations.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/autoscaling-describe-policies.json
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/autoscaling-describe-policies.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/autoscaling-describe-scaling-activities.json
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/autoscaling-describe-scaling-activities.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/autoscaling-describe-scaling-process-types.json
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/autoscaling-describe-scaling-process-types.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/autoscaling-describe-scheduled-actions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/autoscaling-describe-scheduled-actions.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/autoscaling-describe-tags.json
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/autoscaling-describe-tags.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/autoscaling-describe-termination-policy-types.json
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/autoscaling-describe-termination-policy-types.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/cloudformation-describe-stacks.json
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/cloudformation-describe-stacks.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5985 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/cloudformation-get-template.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5222 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/cloudformation-get-template.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/cloudformation-list-stacks.json
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/cloudformation-list-stacks.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/cloudfront-get-cloud-front-origin-access-identity.json
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/cloudfront-get-cloud-front-origin-access-identity.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4562 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/cloudfront-get-distribution.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4769 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/cloudfront-get-distribution.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/cloudfront-get-invalidation.json
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/cloudfront-get-invalidation.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/cloudfront-get-streaming-distribution.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/cloudfront-get-streaming-distribution.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/cloudfront-list-cloud-front-origin-access-identities.json
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/cloudfront-list-cloud-front-origin-access-identities.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3943 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/cloudfront-list-distributions.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4181 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/cloudfront-list-distributions.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/cloudfront-list-invalidations.json
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/cloudfront-list-invalidations.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/cloudfront-list-streaming-distributions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/cloudfront-list-streaming-distributions.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/cloudwatch-describe-alarm-history.json
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/cloudwatch-describe-alarm-history.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/cloudwatch-describe-alarms.json
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/cloudwatch-describe-alarms.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    21940 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/cloudwatch-list-metrics.json
+-rw-r--r--   0 runner    (1001) docker     (127)    22671 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/cloudwatch-list-metrics.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-allocate-address.json
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-allocate-address.xml
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-assign-private-ip-addresses.json
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-assign-private-ip-addresses.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-associate-address.json
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-associate-address.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-associate-route-table.json
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-associate-route-table.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-attach-volume.json
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-attach-volume.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-attach-vpn-gateway.json
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-attach-vpn-gateway.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-bundle-instance.json
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-bundle-instance.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-cancel-bundle-task.json
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-cancel-bundle-task.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-cancel-reserved-instances-listing.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-cancel-reserved-instances-listing.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-cancel-spot-instance-requests.json
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-cancel-spot-instance-requests.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-confirm-product-instance.json
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-confirm-product-instance.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-copy-snapshot.json
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-copy-snapshot.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-create-customer-gateway.json
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-create-customer-gateway.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-create-dhcp-options.json
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-create-dhcp-options.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-create-instance-export-task.json
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-create-instance-export-task.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-create-key-pair.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-create-key-pair.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-create-network-acl.json
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-create-network-acl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-create-network-interface.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-create-network-interface.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-create-reserved-instances-listing.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3860 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-create-reserved-instances-listing.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-create-route-table.json
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-create-route-table.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-create-snapshot.json
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-create-snapshot.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-create-spot-datafeed-subscription.json
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-create-spot-datafeed-subscription.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-create-subnet.json
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-create-subnet.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-create-volume.json
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-create-volume.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-create-vpc.json
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-create-vpc.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-create-vpn-gateway.json
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-create-vpn-gateway.xml
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-delete-internet-gateway.json
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-delete-internet-gateway.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-account-attributes.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-account-attributes.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-addresses.json
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-addresses.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-availability-zones.json
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-availability-zones.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-bundle-tasks.json
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-bundle-tasks.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-customer-gateways.json
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-customer-gateways.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-dhcp-options.json
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-dhcp-options.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-export-tasks.json
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-export-tasks.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-instance-attribute.json
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-instance-attribute.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-instance-status.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-instance-status.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-instances.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6389 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-instances.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-internet-gateways.json
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-internet-gateways.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-key-pairs.json
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-key-pairs.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-network-acls.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-network-acls.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-network-interfaces.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-network-interfaces.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-placement-groups.json
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-placement-groups.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-regions.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-regions.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-reserved-instances-offerings.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-reserved-instances-offerings.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-reserved-instances.json
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-reserved-instances.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-route-tables.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-route-tables.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5264 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-security-groups.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6128 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-security-groups.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-snapshots.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-snapshots.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-spot-instance-requests.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-spot-instance-requests.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   248956 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-spot-price-history.json
+-rw-r--r--   0 runner    (1001) docker     (127)   314117 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-spot-price-history.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-subnets.json
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-subnets.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-tags.json
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-tags.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-volume-status.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-volume-status.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-volumes.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-volumes.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-vpcs.json
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-vpcs.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-vpn-connections.json
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-vpn-connections.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-vpn-gateways.json
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-vpn-gateways.xml
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-detach-network-interface.json
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-detach-network-interface.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-detach-volume.json
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-detach-volume.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-get-password-data.json
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-get-password-data.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-import-instance.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-import-instance.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-import-key-pair.json
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-import-key-pair.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-import-volume.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-import-volume.xml
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-modify-snapshot-attribute.json
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-modify-snapshot-attribute.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-monitor-instances.json
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-monitor-instances.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-register-image.json
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-register-image.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-replace-network-acl-association.json
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-replace-network-acl-association.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-request-spot-instances.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-request-spot-instances.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-run-instances.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-run-instances.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-start-instances.json
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-start-instances.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-stop-instances.json
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-stop-instances.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-unmonitor-instances.json
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-unmonitor-instances.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/elasticbeanstalk-check-dns-availability.json
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/elasticbeanstalk-check-dns-availability.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/elasticbeanstalk-create-application-version.json
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/elasticbeanstalk-create-application-version.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/elasticbeanstalk-create-application.json
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/elasticbeanstalk-create-application.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     7362 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/elasticbeanstalk-create-configuration-template.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7328 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/elasticbeanstalk-create-configuration-template.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/elasticbeanstalk-create-environment.json
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/elasticbeanstalk-create-environment.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/elasticbeanstalk-create-storage-location.json
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/elasticbeanstalk-create-storage-location.xml
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/elasticbeanstalk-delete-application.json
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/elasticbeanstalk-delete-application.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/elasticbeanstalk-describe-application-versions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/elasticbeanstalk-describe-application-versions.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/elasticbeanstalk-describe-applications.json
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/elasticbeanstalk-describe-applications.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    16850 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/elasticbeanstalk-describe-configuration-options.json
+-rw-r--r--   0 runner    (1001) docker     (127)    19126 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/elasticbeanstalk-describe-configuration-options.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/elasticbeanstalk-describe-environments.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/elasticbeanstalk-describe-environments.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/elasticbeanstalk-describe-events.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/elasticbeanstalk-describe-events.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/elasticbeanstalk-list-available-solution-stacks.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5492 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/elasticbeanstalk-list-available-solution-stacks.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/elasticbeanstalk-retrieve-environment-info.json
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/elasticbeanstalk-retrieve-environment-info.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/elasticbeanstalk-terminate-environment.json
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/elasticbeanstalk-terminate-environment.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/elasticbeanstalk-update-application-version.json
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/elasticbeanstalk-update-application-version.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/elasticbeanstalk-update-application.json
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/elasticbeanstalk-update-application.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    17788 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/elb-describe-load-balancer-policies.json
+-rw-r--r--   0 runner    (1001) docker     (127)    19095 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/elb-describe-load-balancer-policies.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    21850 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/elb-describe-load-balancer-policy-types.json
+-rw-r--r--   0 runner    (1001) docker     (127)    22855 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/elb-describe-load-balancer-policy-types.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/elb-describe-load-balancers.json
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/elb-describe-load-balancers.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/iam-create-virtual-mfa-device.json
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/iam-create-virtual-mfa-device.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/iam-get-account-summary.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/iam-get-account-summary.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/iam-get-group.json
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/iam-get-group.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/iam-get-user-policy.json
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/iam-get-user-policy.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/iam-get-user.json
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/iam-get-user.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/iam-list-access-keys.json
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/iam-list-access-keys.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/iam-list-account-aliases.json
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/iam-list-account-aliases.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/iam-list-groups.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/iam-list-groups.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/iam-list-instance-profiles.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/iam-list-instance-profiles.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/iam-list-mfa-devices.json
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/iam-list-mfa-devices.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/iam-list-roles.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/iam-list-roles.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/iam-list-server-certificates.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/iam-list-server-certificates.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/iam-list-signing-certificates.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/iam-list-signing-certificates.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/iam-list-users.json
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/iam-list-users.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/iam-list-virtual-mfa-devices.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/iam-list-virtual-mfa-devices.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/importexport-list-jobs.json
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/importexport-list-jobs.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     6666 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/rds-describe-db-engine-versions.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8608 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/rds-describe-db-engine-versions.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/rds-describe-db-instances.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/rds-describe-db-instances.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/rds-describe-db-parameter-groups.json
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/rds-describe-db-parameter-groups.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/rds-describe-db-security-groups.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/rds-describe-db-security-groups.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/rds-describe-db-snapshots.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/rds-describe-db-snapshots.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/rds-describe-db-subnet-groups.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3431 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/rds-describe-db-subnet-groups.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/rds-describe-event-categories.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/rds-describe-event-categories.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/rds-describe-event-subscriptions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/rds-describe-event-subscriptions.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/rds-describe-events.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/rds-describe-events.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/rds-describe-option-groups.json
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/rds-describe-option-groups.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/rds-describe-reserved-db-instances-offerings.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/rds-describe-reserved-db-instances-offerings.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/rds-describe-reserved-db-instances.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/rds-describe-reserved-db-instances.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-authorize-cluster-security-group-ingress.json
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-authorize-cluster-security-group-ingress.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-copy-cluster-snapshot.json
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-copy-cluster-snapshot.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-create-cluster-parameter-group.json
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-create-cluster-parameter-group.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-create-cluster-security-group.json
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-create-cluster-security-group.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-create-cluster-snapshot.json
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-create-cluster-snapshot.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-create-cluster-subnet-group.json
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-create-cluster-subnet-group.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-create-cluster.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-create-cluster.xml
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-delete-cluster-parameter-group.json
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-delete-cluster-parameter-group.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-delete-cluster-snapshot.json
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-delete-cluster-snapshot.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-delete-cluster.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-delete-cluster.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-parameter-groups.json
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-parameter-groups.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-parameters.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-parameters.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-security-groups.json
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-security-groups.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-snapshots.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-snapshots.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-subnet-groups.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-subnet-groups.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-versions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-versions.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-describe-clusters.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-describe-clusters.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-describe-events.json
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-describe-events.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-describe-orderable-cluster-options.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-describe-orderable-cluster-options.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-describe-reserved-node-offerings.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-describe-reserved-node-offerings.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-describe-reserved-nodes.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-describe-reserved-nodes.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-describe-resize.json
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-describe-resize.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-modify-cluster-parameter-group.json
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-modify-cluster-parameter-group.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-purchase-reserved-node-offering.json
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-purchase-reserved-node-offering.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-reboot-cluster.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-reboot-cluster.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-reset-cluster-parameter-group.json
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-reset-cluster-parameter-group.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-restore-from-cluster-snapshot.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-restore-from-cluster-snapshot.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-revoke-cluster-security-group-ingress.json
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-revoke-cluster-security-group-ingress.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/s3-get-bucket-acl.json
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/s3-get-bucket-acl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/s3-get-bucket-location.json
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/s3-get-bucket-location.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/s3-get-bucket-logging.json
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/s3-get-bucket-logging.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/s3-get-bucket-policy.json
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/s3-get-bucket-policy.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5077 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/s3-list-buckets.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/s3-list-buckets.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/s3-list-multipart-uploads#2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/s3-list-multipart-uploads#2.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/s3-list-multipart-uploads.json
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/s3-list-multipart-uploads.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/s3-list-object-versions.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/s3-list-object-versions.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/s3-list-objects.json
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/s3-list-objects.xml
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ses-delete-identity.json
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ses-delete-identity.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ses-get-identity-dkim-attributes.json
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ses-get-identity-dkim-attributes.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ses-get-identity-notification-attributes.json
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ses-get-identity-notification-attributes.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ses-get-identity-verification-attributes.json
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ses-get-identity-verification-attributes.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ses-get-send-quota.json
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ses-get-send-quota.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ses-get-send-statistics.json
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ses-get-send-statistics.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ses-list-identities.json
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ses-list-identities.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ses-send-email.json
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ses-send-email.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ses-send-raw-email.json
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ses-send-raw-email.xml
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ses-set-identity-dkim-enabled.json
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ses-set-identity-dkim-enabled.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ses-verify-domain-dkim.json
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ses-verify-domain-dkim.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ses-verify-domain-identity.json
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ses-verify-domain-identity.xml
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/sns-add-permission.json
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/sns-add-permission.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/sns-confirm-subscription.json
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/sns-confirm-subscription.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/sns-create-topic.json
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/sns-create-topic.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/sns-get-subscription-attributes.json
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/sns-get-subscription-attributes.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/sns-get-topic-attributes.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/sns-get-topic-attributes.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/sns-list-subscriptions-by-topic.json
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/sns-list-subscriptions-by-topic.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/sns-list-subscriptions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/sns-list-subscriptions.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/sns-list-topics.json
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/sns-list-topics.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/sns-publish.json
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/sns-publish.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/sns-subscribe.json
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/sns-subscribe.xml
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/sqs-add-permission.json
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/sqs-change-message-visibility-batch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/sqs-create-queue.json
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/sqs-delete-message-batch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/sqs-get-queue-attributes.json
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/sqs-get-queue-url.json
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/sqs-list-queues.json
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/sqs-receive-message.json
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/sqs-send-message-batch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/sqs-send-message.json
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/sts-get-session-token.json
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/sts-get-session-token.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:50.296085 botocore-a-la-carte-1.34.99/tests/unit/retries/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/retries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6630 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/retries/test_adaptive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4602 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/retries/test_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/retries/test_quota.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4763 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/retries/test_special.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26367 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/retries/test_standard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/retries/test_throttling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35112 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/test_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/test_auth_bearer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/test_auth_sigv4.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30747 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/test_awsrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    93962 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7070 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/test_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9524 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/test_compress.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39978 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/test_config_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8695 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/test_configloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)   139891 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20712 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/test_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18355 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/test_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15094 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/test_endpoint_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5613 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/test_errorfactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15485 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/test_eventstream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6399 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63533 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/test_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/test_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27457 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/test_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/test_http_client_exception_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19734 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/test_http_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27402 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/test_httpchecksum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/test_idempotency.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19334 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/test_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47606 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35401 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/test_monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57408 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/test_paginate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58705 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/test_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17041 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/test_protocols.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50089 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/test_regions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14405 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/test_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15360 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/test_retryhandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9458 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/test_s3_addressing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19004 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/test_serialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40114 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35707 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/test_session_legacy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43689 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/test_signers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8655 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/test_stub.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11901 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/test_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4321 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/test_translate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6462 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/test_useragent.py
+-rw-r--r--   0 runner    (1001) docker     (127)   126991 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21414 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/test_validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33648 2024-05-07 01:02:11.000000 botocore-a-la-carte-1.34.99/tests/unit/test_waiters.py
```

### Comparing `botocore-a-la-carte-1.34.98/LICENSE.txt` & `botocore-a-la-carte-1.34.99/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/NOTICE` & `botocore-a-la-carte-1.34.99/NOTICE`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/PKG-INFO` & `botocore-a-la-carte-1.34.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte
-Version: 1.34.98
+Version: 1.34.99
 Summary: botocore re-uploaded with a-la-carte data packages.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-1.34.98/README.rst` & `botocore-a-la-carte-1.34.99/README.rst`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/botocore/__init__.py` & `botocore-a-la-carte-1.34.99/botocore/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # ANY KIND, either express or implied. See the License for the specific
 # language governing permissions and limitations under the License.
 
 import logging
 import os
 import re
 
-__version__ = '1.34.98'
+__version__ = '1.34.99'
 
 
 class NullHandler(logging.Handler):
     def emit(self, record):
         pass
```

### Comparing `botocore-a-la-carte-1.34.98/botocore/args.py` & `botocore-a-la-carte-1.34.99/botocore/args.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/botocore/auth.py` & `botocore-a-la-carte-1.34.99/botocore/auth.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/botocore/awsrequest.py` & `botocore-a-la-carte-1.34.99/botocore/awsrequest.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/botocore/cacert.pem` & `botocore-a-la-carte-1.34.99/botocore/cacert.pem`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/botocore/client.py` & `botocore-a-la-carte-1.34.99/botocore/client.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/botocore/compat.py` & `botocore-a-la-carte-1.34.99/botocore/compat.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/botocore/compress.py` & `botocore-a-la-carte-1.34.99/botocore/compress.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/botocore/config.py` & `botocore-a-la-carte-1.34.99/botocore/config.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/botocore/configloader.py` & `botocore-a-la-carte-1.34.99/botocore/configloader.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/botocore/configprovider.py` & `botocore-a-la-carte-1.34.99/botocore/configprovider.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/botocore/credentials.py` & `botocore-a-la-carte-1.34.99/botocore/credentials.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/botocore/crt/__init__.py` & `botocore-a-la-carte-1.34.99/botocore/crt/__init__.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/botocore/crt/auth.py` & `botocore-a-la-carte-1.34.99/botocore/crt/auth.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/botocore/data/_retry.json` & `botocore-a-la-carte-1.34.99/botocore/data/_retry.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/botocore/data/endpoints.json` & `botocore-a-la-carte-1.34.99/botocore/data/endpoints.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999999758519118%*

 * *Differences: {"'partitions'": "{0: {'services': {'controltower': {'endpoints': {'ca-west-1': "*

 * *                 "OrderedDict([('variants', [OrderedDict([('hostname', "*

 * *                 "'controltower-fips.ca-west-1.amazonaws.com'), ('tags', ['fips'])])])]), "*

 * *                 "'ca-west-1-fips': OrderedDict([('credentialScope', OrderedDict([('region', "*

 * *                 "'ca-west-1')])), ('deprecated', True), ('hostname', "*

 * *                 "'controltower-fips.ca-west-1.amazonaws.com')])}}, 'fms': {'endpoints': "*

 * *        […]*

```diff
@@ -5287,14 +5287,31 @@
                         "ca-central-1-fips": {
                             "credentialScope": {
                                 "region": "ca-central-1"
                             },
                             "deprecated": true,
                             "hostname": "controltower-fips.ca-central-1.amazonaws.com"
                         },
+                        "ca-west-1": {
+                            "variants": [
+                                {
+                                    "hostname": "controltower-fips.ca-west-1.amazonaws.com",
+                                    "tags": [
+                                        "fips"
+                                    ]
+                                }
+                            ]
+                        },
+                        "ca-west-1-fips": {
+                            "credentialScope": {
+                                "region": "ca-west-1"
+                            },
+                            "deprecated": true,
+                            "hostname": "controltower-fips.ca-west-1.amazonaws.com"
+                        },
                         "eu-central-1": {},
                         "eu-central-2": {},
                         "eu-north-1": {},
                         "eu-south-1": {},
                         "eu-south-2": {},
                         "eu-west-1": {},
                         "eu-west-2": {},
@@ -9542,14 +9559,24 @@
                                     "hostname": "fms-fips.ca-central-1.amazonaws.com",
                                     "tags": [
                                         "fips"
                                     ]
                                 }
                             ]
                         },
+                        "ca-west-1": {
+                            "variants": [
+                                {
+                                    "hostname": "fms-fips.ca-west-1.amazonaws.com",
+                                    "tags": [
+                                        "fips"
+                                    ]
+                                }
+                            ]
+                        },
                         "eu-central-1": {
                             "variants": [
                                 {
                                     "hostname": "fms-fips.eu-central-1.amazonaws.com",
                                     "tags": [
                                         "fips"
                                     ]
@@ -9651,14 +9678,21 @@
                         "fips-ca-central-1": {
                             "credentialScope": {
                                 "region": "ca-central-1"
                             },
                             "deprecated": true,
                             "hostname": "fms-fips.ca-central-1.amazonaws.com"
                         },
+                        "fips-ca-west-1": {
+                            "credentialScope": {
+                                "region": "ca-west-1"
+                            },
+                            "deprecated": true,
+                            "hostname": "fms-fips.ca-west-1.amazonaws.com"
+                        },
                         "fips-eu-central-1": {
                             "credentialScope": {
                                 "region": "eu-central-1"
                             },
                             "deprecated": true,
                             "hostname": "fms-fips.eu-central-1.amazonaws.com"
                         },
@@ -23684,15 +23718,24 @@
                                     "hostname": "transfer-fips.ca-central-1.amazonaws.com",
                                     "tags": [
                                         "fips"
                                     ]
                                 }
                             ]
                         },
-                        "ca-west-1": {},
+                        "ca-west-1": {
+                            "variants": [
+                                {
+                                    "hostname": "transfer-fips.ca-west-1.amazonaws.com",
+                                    "tags": [
+                                        "fips"
+                                    ]
+                                }
+                            ]
+                        },
                         "eu-central-1": {},
                         "eu-central-2": {},
                         "eu-north-1": {},
                         "eu-south-1": {},
                         "eu-south-2": {},
                         "eu-west-1": {},
                         "eu-west-2": {},
@@ -23700,14 +23743,21 @@
                         "fips-ca-central-1": {
                             "credentialScope": {
                                 "region": "ca-central-1"
                             },
                             "deprecated": true,
                             "hostname": "transfer-fips.ca-central-1.amazonaws.com"
                         },
+                        "fips-ca-west-1": {
+                            "credentialScope": {
+                                "region": "ca-west-1"
+                            },
+                            "deprecated": true,
+                            "hostname": "transfer-fips.ca-west-1.amazonaws.com"
+                        },
                         "fips-us-east-1": {
                             "credentialScope": {
                                 "region": "us-east-1"
                             },
                             "deprecated": true,
                             "hostname": "transfer-fips.us-east-1.amazonaws.com"
                         },
```

### Comparing `botocore-a-la-carte-1.34.98/botocore/data/partitions.json` & `botocore-a-la-carte-1.34.99/botocore/data/partitions.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/botocore/data/sdk-default-configuration.json` & `botocore-a-la-carte-1.34.99/botocore/data/sdk-default-configuration.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/botocore/discovery.py` & `botocore-a-la-carte-1.34.99/botocore/discovery.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/botocore/docs/__init__.py` & `botocore-a-la-carte-1.34.99/botocore/docs/__init__.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/botocore/docs/bcdoc/__init__.py` & `botocore-a-la-carte-1.34.99/botocore/docs/bcdoc/__init__.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/botocore/docs/bcdoc/docstringparser.py` & `botocore-a-la-carte-1.34.99/botocore/docs/bcdoc/docstringparser.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/botocore/docs/bcdoc/restdoc.py` & `botocore-a-la-carte-1.34.99/botocore/docs/bcdoc/restdoc.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/botocore/docs/bcdoc/style.py` & `botocore-a-la-carte-1.34.99/botocore/docs/bcdoc/style.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/botocore/docs/client.py` & `botocore-a-la-carte-1.34.99/botocore/docs/client.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/botocore/docs/docstring.py` & `botocore-a-la-carte-1.34.99/botocore/docs/docstring.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/botocore/docs/example.py` & `botocore-a-la-carte-1.34.99/botocore/docs/example.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/botocore/docs/method.py` & `botocore-a-la-carte-1.34.99/botocore/docs/method.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/botocore/docs/paginator.py` & `botocore-a-la-carte-1.34.99/botocore/docs/paginator.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/botocore/docs/params.py` & `botocore-a-la-carte-1.34.99/botocore/docs/params.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/botocore/docs/service.py` & `botocore-a-la-carte-1.34.99/botocore/docs/service.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/botocore/docs/shape.py` & `botocore-a-la-carte-1.34.99/botocore/docs/shape.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/botocore/docs/sharedexample.py` & `botocore-a-la-carte-1.34.99/botocore/docs/sharedexample.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/botocore/docs/translator.py` & `botocore-a-la-carte-1.34.99/botocore/docs/translator.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/botocore/docs/utils.py` & `botocore-a-la-carte-1.34.99/botocore/docs/utils.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/botocore/docs/waiter.py` & `botocore-a-la-carte-1.34.99/botocore/docs/waiter.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/botocore/endpoint.py` & `botocore-a-la-carte-1.34.99/botocore/endpoint.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/botocore/endpoint_provider.py` & `botocore-a-la-carte-1.34.99/botocore/endpoint_provider.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/botocore/errorfactory.py` & `botocore-a-la-carte-1.34.99/botocore/errorfactory.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/botocore/eventstream.py` & `botocore-a-la-carte-1.34.99/botocore/eventstream.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/botocore/exceptions.py` & `botocore-a-la-carte-1.34.99/botocore/exceptions.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/botocore/handlers.py` & `botocore-a-la-carte-1.34.99/botocore/handlers.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/botocore/history.py` & `botocore-a-la-carte-1.34.99/botocore/history.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/botocore/hooks.py` & `botocore-a-la-carte-1.34.99/botocore/hooks.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/botocore/httpchecksum.py` & `botocore-a-la-carte-1.34.99/botocore/httpchecksum.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/botocore/httpsession.py` & `botocore-a-la-carte-1.34.99/botocore/httpsession.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/botocore/loaders.py` & `botocore-a-la-carte-1.34.99/botocore/loaders.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/botocore/model.py` & `botocore-a-la-carte-1.34.99/botocore/model.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/botocore/monitoring.py` & `botocore-a-la-carte-1.34.99/botocore/monitoring.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/botocore/paginate.py` & `botocore-a-la-carte-1.34.99/botocore/paginate.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/botocore/parsers.py` & `botocore-a-la-carte-1.34.99/botocore/parsers.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/botocore/regions.py` & `botocore-a-la-carte-1.34.99/botocore/regions.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/botocore/response.py` & `botocore-a-la-carte-1.34.99/botocore/response.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/botocore/retries/adaptive.py` & `botocore-a-la-carte-1.34.99/botocore/retries/adaptive.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/botocore/retries/base.py` & `botocore-a-la-carte-1.34.99/botocore/retries/base.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/botocore/retries/bucket.py` & `botocore-a-la-carte-1.34.99/botocore/retries/bucket.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/botocore/retries/quota.py` & `botocore-a-la-carte-1.34.99/botocore/retries/quota.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/botocore/retries/special.py` & `botocore-a-la-carte-1.34.99/botocore/retries/special.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/botocore/retries/standard.py` & `botocore-a-la-carte-1.34.99/botocore/retries/standard.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/botocore/retries/throttling.py` & `botocore-a-la-carte-1.34.99/botocore/retries/throttling.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/botocore/retryhandler.py` & `botocore-a-la-carte-1.34.99/botocore/retryhandler.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/botocore/serialize.py` & `botocore-a-la-carte-1.34.99/botocore/serialize.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/botocore/session.py` & `botocore-a-la-carte-1.34.99/botocore/session.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/botocore/signers.py` & `botocore-a-la-carte-1.34.99/botocore/signers.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/botocore/stub.py` & `botocore-a-la-carte-1.34.99/botocore/stub.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/botocore/tokens.py` & `botocore-a-la-carte-1.34.99/botocore/tokens.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/botocore/translate.py` & `botocore-a-la-carte-1.34.99/botocore/translate.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/botocore/useragent.py` & `botocore-a-la-carte-1.34.99/botocore/useragent.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/botocore/utils.py` & `botocore-a-la-carte-1.34.99/botocore/utils.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/botocore/validate.py` & `botocore-a-la-carte-1.34.99/botocore/validate.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/botocore/vendored/requests/exceptions.py` & `botocore-a-la-carte-1.34.99/botocore/vendored/requests/exceptions.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/botocore/vendored/requests/packages/urllib3/exceptions.py` & `botocore-a-la-carte-1.34.99/botocore/vendored/requests/packages/urllib3/exceptions.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/botocore/vendored/six.py` & `botocore-a-la-carte-1.34.99/botocore/vendored/six.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/botocore/waiter.py` & `botocore-a-la-carte-1.34.99/botocore/waiter.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/botocore_a_la_carte.egg-info/PKG-INFO` & `botocore-a-la-carte-1.34.99/botocore_a_la_carte.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte
-Version: 1.34.98
+Version: 1.34.99
 Summary: botocore re-uploaded with a-la-carte data packages.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-1.34.98/botocore_a_la_carte.egg-info/SOURCES.txt` & `botocore-a-la-carte-1.34.99/botocore_a_la_carte.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/docs/Makefile` & `botocore-a-la-carte-1.34.99/docs/Makefile`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/docs/make.bat` & `botocore-a-la-carte-1.34.99/docs/make.bat`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/docs/source/_static/404.html` & `botocore-a-la-carte-1.34.99/docs/source/_static/404.html`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/docs/source/_static/css/custom.css` & `botocore-a-la-carte-1.34.99/docs/source/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/docs/source/_static/js/custom.js` & `botocore-a-la-carte-1.34.99/docs/source/_static/js/custom.js`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/docs/source/_static/logos/aws_dark_theme_logo.svg` & `botocore-a-la-carte-1.34.99/docs/source/_static/logos/aws_dark_theme_logo.svg`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/docs/source/_static/logos/aws_light_theme_logo.svg` & `botocore-a-la-carte-1.34.99/docs/source/_static/logos/aws_light_theme_logo.svg`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/docs/source/_static/shortbreadv1.js` & `botocore-a-la-carte-1.34.99/docs/source/_static/shortbreadv1.js`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/docs/source/_templates/page.html` & `botocore-a-la-carte-1.34.99/docs/source/_templates/page.html`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/docs/source/client_upgrades.rst` & `botocore-a-la-carte-1.34.99/docs/source/client_upgrades.rst`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/docs/source/conf.py` & `botocore-a-la-carte-1.34.99/docs/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
 version = '1.34.'
 # The full version, including alpha/beta/rc tags.
-release = '1.34.98'
+release = '1.34.99'
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #language = None
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
```

### Comparing `botocore-a-la-carte-1.34.98/docs/source/development/designnotes.rst` & `botocore-a-la-carte-1.34.99/docs/source/development/designnotes.rst`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/docs/source/index.rst` & `botocore-a-la-carte-1.34.99/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/docs/source/topics/events.rst` & `botocore-a-la-carte-1.34.99/docs/source/topics/events.rst`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/docs/source/topics/paginators.rst` & `botocore-a-la-carte-1.34.99/docs/source/topics/paginators.rst`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/docs/source/tutorial/index.rst` & `botocore-a-la-carte-1.34.99/docs/source/tutorial/index.rst`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/setup.cfg` & `botocore-a-la-carte-1.34.99/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -6,397 +6,397 @@
 	jmespath>=0.7.1,<2.0.0
 	python-dateutil>=2.1,<3.0.0
 	urllib3>=1.25.4,<1.27; python_version<"3.10"
 	urllib3>=1.25.4,!=2.2.0,<3; python_version>="3.10"
 
 [options.extras_require]
 crt = awscrt==0.20.9
-accessanalyzer = botocore-a-la-carte-accessanalyzer==1.34.98
-account = botocore-a-la-carte-account==1.34.98
-acm = botocore-a-la-carte-acm==1.34.98
-acm-pca = botocore-a-la-carte-acm-pca==1.34.98
-alexaforbusiness = botocore-a-la-carte-alexaforbusiness==1.34.98
-amp = botocore-a-la-carte-amp==1.34.98
-amplify = botocore-a-la-carte-amplify==1.34.98
-amplifybackend = botocore-a-la-carte-amplifybackend==1.34.98
-amplifyuibuilder = botocore-a-la-carte-amplifyuibuilder==1.34.98
-apigateway = botocore-a-la-carte-apigateway==1.34.98
-apigatewaymanagementapi = botocore-a-la-carte-apigatewaymanagementapi==1.34.98
-apigatewayv2 = botocore-a-la-carte-apigatewayv2==1.34.98
-appconfig = botocore-a-la-carte-appconfig==1.34.98
-appconfigdata = botocore-a-la-carte-appconfigdata==1.34.98
-appfabric = botocore-a-la-carte-appfabric==1.34.98
-appflow = botocore-a-la-carte-appflow==1.34.98
-appintegrations = botocore-a-la-carte-appintegrations==1.34.98
-application-autoscaling = botocore-a-la-carte-application-autoscaling==1.34.98
-application-insights = botocore-a-la-carte-application-insights==1.34.98
-applicationcostprofiler = botocore-a-la-carte-applicationcostprofiler==1.34.98
-appmesh = botocore-a-la-carte-appmesh==1.34.98
-apprunner = botocore-a-la-carte-apprunner==1.34.98
-appstream = botocore-a-la-carte-appstream==1.34.98
-appsync = botocore-a-la-carte-appsync==1.34.98
-arc-zonal-shift = botocore-a-la-carte-arc-zonal-shift==1.34.98
-artifact = botocore-a-la-carte-artifact==1.34.98
-athena = botocore-a-la-carte-athena==1.34.98
-auditmanager = botocore-a-la-carte-auditmanager==1.34.98
-autoscaling = botocore-a-la-carte-autoscaling==1.34.98
-autoscaling-plans = botocore-a-la-carte-autoscaling-plans==1.34.98
-b2bi = botocore-a-la-carte-b2bi==1.34.98
-backup = botocore-a-la-carte-backup==1.34.98
-backup-gateway = botocore-a-la-carte-backup-gateway==1.34.98
-backupstorage = botocore-a-la-carte-backupstorage==1.34.98
-batch = botocore-a-la-carte-batch==1.34.98
-bcm-data-exports = botocore-a-la-carte-bcm-data-exports==1.34.98
-bedrock = botocore-a-la-carte-bedrock==1.34.98
-bedrock-agent = botocore-a-la-carte-bedrock-agent==1.34.98
-bedrock-agent-runtime = botocore-a-la-carte-bedrock-agent-runtime==1.34.98
-bedrock-runtime = botocore-a-la-carte-bedrock-runtime==1.34.98
-billingconductor = botocore-a-la-carte-billingconductor==1.34.98
-braket = botocore-a-la-carte-braket==1.34.98
-budgets = botocore-a-la-carte-budgets==1.34.98
-ce = botocore-a-la-carte-ce==1.34.98
-chatbot = botocore-a-la-carte-chatbot==1.34.98
-chime = botocore-a-la-carte-chime==1.34.98
-chime-sdk-identity = botocore-a-la-carte-chime-sdk-identity==1.34.98
-chime-sdk-media-pipelines = botocore-a-la-carte-chime-sdk-media-pipelines==1.34.98
-chime-sdk-meetings = botocore-a-la-carte-chime-sdk-meetings==1.34.98
-chime-sdk-messaging = botocore-a-la-carte-chime-sdk-messaging==1.34.98
-chime-sdk-voice = botocore-a-la-carte-chime-sdk-voice==1.34.98
-cleanrooms = botocore-a-la-carte-cleanrooms==1.34.98
-cleanroomsml = botocore-a-la-carte-cleanroomsml==1.34.98
-cloud9 = botocore-a-la-carte-cloud9==1.34.98
-cloudcontrol = botocore-a-la-carte-cloudcontrol==1.34.98
-clouddirectory = botocore-a-la-carte-clouddirectory==1.34.98
-cloudformation = botocore-a-la-carte-cloudformation==1.34.98
-cloudfront = botocore-a-la-carte-cloudfront==1.34.98
-cloudfront-keyvaluestore = botocore-a-la-carte-cloudfront-keyvaluestore==1.34.98
-cloudhsm = botocore-a-la-carte-cloudhsm==1.34.98
-cloudhsmv2 = botocore-a-la-carte-cloudhsmv2==1.34.98
-cloudsearch = botocore-a-la-carte-cloudsearch==1.34.98
-cloudsearchdomain = botocore-a-la-carte-cloudsearchdomain==1.34.98
-cloudtrail = botocore-a-la-carte-cloudtrail==1.34.98
-cloudtrail-data = botocore-a-la-carte-cloudtrail-data==1.34.98
-cloudwatch = botocore-a-la-carte-cloudwatch==1.34.98
-codeartifact = botocore-a-la-carte-codeartifact==1.34.98
-codebuild = botocore-a-la-carte-codebuild==1.34.98
-codecatalyst = botocore-a-la-carte-codecatalyst==1.34.98
-codecommit = botocore-a-la-carte-codecommit==1.34.98
-codeconnections = botocore-a-la-carte-codeconnections==1.34.98
-codedeploy = botocore-a-la-carte-codedeploy==1.34.98
-codeguru-reviewer = botocore-a-la-carte-codeguru-reviewer==1.34.98
-codeguru-security = botocore-a-la-carte-codeguru-security==1.34.98
-codeguruprofiler = botocore-a-la-carte-codeguruprofiler==1.34.98
-codepipeline = botocore-a-la-carte-codepipeline==1.34.98
-codestar = botocore-a-la-carte-codestar==1.34.98
-codestar-connections = botocore-a-la-carte-codestar-connections==1.34.98
-codestar-notifications = botocore-a-la-carte-codestar-notifications==1.34.98
-cognito-identity = botocore-a-la-carte-cognito-identity==1.34.98
-cognito-idp = botocore-a-la-carte-cognito-idp==1.34.98
-cognito-sync = botocore-a-la-carte-cognito-sync==1.34.98
-comprehend = botocore-a-la-carte-comprehend==1.34.98
-comprehendmedical = botocore-a-la-carte-comprehendmedical==1.34.98
-compute-optimizer = botocore-a-la-carte-compute-optimizer==1.34.98
-config = botocore-a-la-carte-config==1.34.98
-connect = botocore-a-la-carte-connect==1.34.98
-connect-contact-lens = botocore-a-la-carte-connect-contact-lens==1.34.98
-connectcampaigns = botocore-a-la-carte-connectcampaigns==1.34.98
-connectcases = botocore-a-la-carte-connectcases==1.34.98
-connectparticipant = botocore-a-la-carte-connectparticipant==1.34.98
-controlcatalog = botocore-a-la-carte-controlcatalog==1.34.98
-controltower = botocore-a-la-carte-controltower==1.34.98
-cost-optimization-hub = botocore-a-la-carte-cost-optimization-hub==1.34.98
-cur = botocore-a-la-carte-cur==1.34.98
-customer-profiles = botocore-a-la-carte-customer-profiles==1.34.98
-databrew = botocore-a-la-carte-databrew==1.34.98
-dataexchange = botocore-a-la-carte-dataexchange==1.34.98
-datapipeline = botocore-a-la-carte-datapipeline==1.34.98
-datasync = botocore-a-la-carte-datasync==1.34.98
-datazone = botocore-a-la-carte-datazone==1.34.98
-dax = botocore-a-la-carte-dax==1.34.98
-deadline = botocore-a-la-carte-deadline==1.34.98
-detective = botocore-a-la-carte-detective==1.34.98
-devicefarm = botocore-a-la-carte-devicefarm==1.34.98
-devops-guru = botocore-a-la-carte-devops-guru==1.34.98
-directconnect = botocore-a-la-carte-directconnect==1.34.98
-discovery = botocore-a-la-carte-discovery==1.34.98
-dlm = botocore-a-la-carte-dlm==1.34.98
-dms = botocore-a-la-carte-dms==1.34.98
-docdb = botocore-a-la-carte-docdb==1.34.98
-docdb-elastic = botocore-a-la-carte-docdb-elastic==1.34.98
-drs = botocore-a-la-carte-drs==1.34.98
-ds = botocore-a-la-carte-ds==1.34.98
-dynamodb = botocore-a-la-carte-dynamodb==1.34.98
-dynamodbstreams = botocore-a-la-carte-dynamodbstreams==1.34.98
-ebs = botocore-a-la-carte-ebs==1.34.98
-ec2 = botocore-a-la-carte-ec2==1.34.98
-ec2-instance-connect = botocore-a-la-carte-ec2-instance-connect==1.34.98
-ecr = botocore-a-la-carte-ecr==1.34.98
-ecr-public = botocore-a-la-carte-ecr-public==1.34.98
-ecs = botocore-a-la-carte-ecs==1.34.98
-efs = botocore-a-la-carte-efs==1.34.98
-eks = botocore-a-la-carte-eks==1.34.98
-eks-auth = botocore-a-la-carte-eks-auth==1.34.98
-elastic-inference = botocore-a-la-carte-elastic-inference==1.34.98
-elasticache = botocore-a-la-carte-elasticache==1.34.98
-elasticbeanstalk = botocore-a-la-carte-elasticbeanstalk==1.34.98
-elastictranscoder = botocore-a-la-carte-elastictranscoder==1.34.98
-elb = botocore-a-la-carte-elb==1.34.98
-elbv2 = botocore-a-la-carte-elbv2==1.34.98
-emr = botocore-a-la-carte-emr==1.34.98
-emr-containers = botocore-a-la-carte-emr-containers==1.34.98
-emr-serverless = botocore-a-la-carte-emr-serverless==1.34.98
-entityresolution = botocore-a-la-carte-entityresolution==1.34.98
-es = botocore-a-la-carte-es==1.34.98
-events = botocore-a-la-carte-events==1.34.98
-evidently = botocore-a-la-carte-evidently==1.34.98
-finspace = botocore-a-la-carte-finspace==1.34.98
-finspace-data = botocore-a-la-carte-finspace-data==1.34.98
-firehose = botocore-a-la-carte-firehose==1.34.98
-fis = botocore-a-la-carte-fis==1.34.98
-fms = botocore-a-la-carte-fms==1.34.98
-forecast = botocore-a-la-carte-forecast==1.34.98
-forecastquery = botocore-a-la-carte-forecastquery==1.34.98
-frauddetector = botocore-a-la-carte-frauddetector==1.34.98
-freetier = botocore-a-la-carte-freetier==1.34.98
-fsx = botocore-a-la-carte-fsx==1.34.98
-gamelift = botocore-a-la-carte-gamelift==1.34.98
-glacier = botocore-a-la-carte-glacier==1.34.98
-globalaccelerator = botocore-a-la-carte-globalaccelerator==1.34.98
-glue = botocore-a-la-carte-glue==1.34.98
-grafana = botocore-a-la-carte-grafana==1.34.98
-greengrass = botocore-a-la-carte-greengrass==1.34.98
-greengrassv2 = botocore-a-la-carte-greengrassv2==1.34.98
-groundstation = botocore-a-la-carte-groundstation==1.34.98
-guardduty = botocore-a-la-carte-guardduty==1.34.98
-health = botocore-a-la-carte-health==1.34.98
-healthlake = botocore-a-la-carte-healthlake==1.34.98
-honeycode = botocore-a-la-carte-honeycode==1.34.98
-iam = botocore-a-la-carte-iam==1.34.98
-identitystore = botocore-a-la-carte-identitystore==1.34.98
-imagebuilder = botocore-a-la-carte-imagebuilder==1.34.98
-importexport = botocore-a-la-carte-importexport==1.34.98
-inspector = botocore-a-la-carte-inspector==1.34.98
-inspector-scan = botocore-a-la-carte-inspector-scan==1.34.98
-inspector2 = botocore-a-la-carte-inspector2==1.34.98
-internetmonitor = botocore-a-la-carte-internetmonitor==1.34.98
-iot = botocore-a-la-carte-iot==1.34.98
-iot-data = botocore-a-la-carte-iot-data==1.34.98
-iot-jobs-data = botocore-a-la-carte-iot-jobs-data==1.34.98
-iot1click-devices = botocore-a-la-carte-iot1click-devices==1.34.98
-iot1click-projects = botocore-a-la-carte-iot1click-projects==1.34.98
-iotanalytics = botocore-a-la-carte-iotanalytics==1.34.98
-iotdeviceadvisor = botocore-a-la-carte-iotdeviceadvisor==1.34.98
-iotevents = botocore-a-la-carte-iotevents==1.34.98
-iotevents-data = botocore-a-la-carte-iotevents-data==1.34.98
-iotfleethub = botocore-a-la-carte-iotfleethub==1.34.98
-iotfleetwise = botocore-a-la-carte-iotfleetwise==1.34.98
-iotsecuretunneling = botocore-a-la-carte-iotsecuretunneling==1.34.98
-iotsitewise = botocore-a-la-carte-iotsitewise==1.34.98
-iotthingsgraph = botocore-a-la-carte-iotthingsgraph==1.34.98
-iottwinmaker = botocore-a-la-carte-iottwinmaker==1.34.98
-iotwireless = botocore-a-la-carte-iotwireless==1.34.98
-ivs = botocore-a-la-carte-ivs==1.34.98
-ivs-realtime = botocore-a-la-carte-ivs-realtime==1.34.98
-ivschat = botocore-a-la-carte-ivschat==1.34.98
-kafka = botocore-a-la-carte-kafka==1.34.98
-kafkaconnect = botocore-a-la-carte-kafkaconnect==1.34.98
-kendra = botocore-a-la-carte-kendra==1.34.98
-kendra-ranking = botocore-a-la-carte-kendra-ranking==1.34.98
-keyspaces = botocore-a-la-carte-keyspaces==1.34.98
-kinesis = botocore-a-la-carte-kinesis==1.34.98
-kinesis-video-archived-media = botocore-a-la-carte-kinesis-video-archived-media==1.34.98
-kinesis-video-media = botocore-a-la-carte-kinesis-video-media==1.34.98
-kinesis-video-signaling = botocore-a-la-carte-kinesis-video-signaling==1.34.98
-kinesis-video-webrtc-storage = botocore-a-la-carte-kinesis-video-webrtc-storage==1.34.98
-kinesisanalytics = botocore-a-la-carte-kinesisanalytics==1.34.98
-kinesisanalyticsv2 = botocore-a-la-carte-kinesisanalyticsv2==1.34.98
-kinesisvideo = botocore-a-la-carte-kinesisvideo==1.34.98
-kms = botocore-a-la-carte-kms==1.34.98
-lakeformation = botocore-a-la-carte-lakeformation==1.34.98
-lambda = botocore-a-la-carte-lambda==1.34.98
-launch-wizard = botocore-a-la-carte-launch-wizard==1.34.98
-lex-models = botocore-a-la-carte-lex-models==1.34.98
-lex-runtime = botocore-a-la-carte-lex-runtime==1.34.98
-lexv2-models = botocore-a-la-carte-lexv2-models==1.34.98
-lexv2-runtime = botocore-a-la-carte-lexv2-runtime==1.34.98
-license-manager = botocore-a-la-carte-license-manager==1.34.98
-license-manager-linux-subscriptions = botocore-a-la-carte-license-manager-linux-subscriptions==1.34.98
-license-manager-user-subscriptions = botocore-a-la-carte-license-manager-user-subscriptions==1.34.98
-lightsail = botocore-a-la-carte-lightsail==1.34.98
-location = botocore-a-la-carte-location==1.34.98
-logs = botocore-a-la-carte-logs==1.34.98
-lookoutequipment = botocore-a-la-carte-lookoutequipment==1.34.98
-lookoutmetrics = botocore-a-la-carte-lookoutmetrics==1.34.98
-lookoutvision = botocore-a-la-carte-lookoutvision==1.34.98
-m2 = botocore-a-la-carte-m2==1.34.98
-machinelearning = botocore-a-la-carte-machinelearning==1.34.98
-macie2 = botocore-a-la-carte-macie2==1.34.98
-managedblockchain = botocore-a-la-carte-managedblockchain==1.34.98
-managedblockchain-query = botocore-a-la-carte-managedblockchain-query==1.34.98
-marketplace-agreement = botocore-a-la-carte-marketplace-agreement==1.34.98
-marketplace-catalog = botocore-a-la-carte-marketplace-catalog==1.34.98
-marketplace-deployment = botocore-a-la-carte-marketplace-deployment==1.34.98
-marketplace-entitlement = botocore-a-la-carte-marketplace-entitlement==1.34.98
-marketplacecommerceanalytics = botocore-a-la-carte-marketplacecommerceanalytics==1.34.98
-mediaconnect = botocore-a-la-carte-mediaconnect==1.34.98
-mediaconvert = botocore-a-la-carte-mediaconvert==1.34.98
-medialive = botocore-a-la-carte-medialive==1.34.98
-mediapackage = botocore-a-la-carte-mediapackage==1.34.98
-mediapackage-vod = botocore-a-la-carte-mediapackage-vod==1.34.98
-mediapackagev2 = botocore-a-la-carte-mediapackagev2==1.34.98
-mediastore = botocore-a-la-carte-mediastore==1.34.98
-mediastore-data = botocore-a-la-carte-mediastore-data==1.34.98
-mediatailor = botocore-a-la-carte-mediatailor==1.34.98
-medical-imaging = botocore-a-la-carte-medical-imaging==1.34.98
-memorydb = botocore-a-la-carte-memorydb==1.34.98
-meteringmarketplace = botocore-a-la-carte-meteringmarketplace==1.34.98
-mgh = botocore-a-la-carte-mgh==1.34.98
-mgn = botocore-a-la-carte-mgn==1.34.98
-migration-hub-refactor-spaces = botocore-a-la-carte-migration-hub-refactor-spaces==1.34.98
-migrationhub-config = botocore-a-la-carte-migrationhub-config==1.34.98
-migrationhuborchestrator = botocore-a-la-carte-migrationhuborchestrator==1.34.98
-migrationhubstrategy = botocore-a-la-carte-migrationhubstrategy==1.34.98
-mobile = botocore-a-la-carte-mobile==1.34.98
-mq = botocore-a-la-carte-mq==1.34.98
-mturk = botocore-a-la-carte-mturk==1.34.98
-mwaa = botocore-a-la-carte-mwaa==1.34.98
-neptune = botocore-a-la-carte-neptune==1.34.98
-neptune-graph = botocore-a-la-carte-neptune-graph==1.34.98
-neptunedata = botocore-a-la-carte-neptunedata==1.34.98
-network-firewall = botocore-a-la-carte-network-firewall==1.34.98
-networkmanager = botocore-a-la-carte-networkmanager==1.34.98
-networkmonitor = botocore-a-la-carte-networkmonitor==1.34.98
-nimble = botocore-a-la-carte-nimble==1.34.98
-oam = botocore-a-la-carte-oam==1.34.98
-omics = botocore-a-la-carte-omics==1.34.98
-opensearch = botocore-a-la-carte-opensearch==1.34.98
-opensearchserverless = botocore-a-la-carte-opensearchserverless==1.34.98
-opsworks = botocore-a-la-carte-opsworks==1.34.98
-opsworkscm = botocore-a-la-carte-opsworkscm==1.34.98
-organizations = botocore-a-la-carte-organizations==1.34.98
-osis = botocore-a-la-carte-osis==1.34.98
-outposts = botocore-a-la-carte-outposts==1.34.98
-panorama = botocore-a-la-carte-panorama==1.34.98
-payment-cryptography = botocore-a-la-carte-payment-cryptography==1.34.98
-payment-cryptography-data = botocore-a-la-carte-payment-cryptography-data==1.34.98
-pca-connector-ad = botocore-a-la-carte-pca-connector-ad==1.34.98
-personalize = botocore-a-la-carte-personalize==1.34.98
-personalize-events = botocore-a-la-carte-personalize-events==1.34.98
-personalize-runtime = botocore-a-la-carte-personalize-runtime==1.34.98
-pi = botocore-a-la-carte-pi==1.34.98
-pinpoint = botocore-a-la-carte-pinpoint==1.34.98
-pinpoint-email = botocore-a-la-carte-pinpoint-email==1.34.98
-pinpoint-sms-voice = botocore-a-la-carte-pinpoint-sms-voice==1.34.98
-pinpoint-sms-voice-v2 = botocore-a-la-carte-pinpoint-sms-voice-v2==1.34.98
-pipes = botocore-a-la-carte-pipes==1.34.98
-polly = botocore-a-la-carte-polly==1.34.98
-pricing = botocore-a-la-carte-pricing==1.34.98
-privatenetworks = botocore-a-la-carte-privatenetworks==1.34.98
-proton = botocore-a-la-carte-proton==1.34.98
-qbusiness = botocore-a-la-carte-qbusiness==1.34.98
-qconnect = botocore-a-la-carte-qconnect==1.34.98
-qldb = botocore-a-la-carte-qldb==1.34.98
-qldb-session = botocore-a-la-carte-qldb-session==1.34.98
-quicksight = botocore-a-la-carte-quicksight==1.34.98
-ram = botocore-a-la-carte-ram==1.34.98
-rbin = botocore-a-la-carte-rbin==1.34.98
-rds = botocore-a-la-carte-rds==1.34.98
-rds-data = botocore-a-la-carte-rds-data==1.34.98
-redshift = botocore-a-la-carte-redshift==1.34.98
-redshift-data = botocore-a-la-carte-redshift-data==1.34.98
-redshift-serverless = botocore-a-la-carte-redshift-serverless==1.34.98
-rekognition = botocore-a-la-carte-rekognition==1.34.98
-repostspace = botocore-a-la-carte-repostspace==1.34.98
-resiliencehub = botocore-a-la-carte-resiliencehub==1.34.98
-resource-explorer-2 = botocore-a-la-carte-resource-explorer-2==1.34.98
-resource-groups = botocore-a-la-carte-resource-groups==1.34.98
-resourcegroupstaggingapi = botocore-a-la-carte-resourcegroupstaggingapi==1.34.98
-robomaker = botocore-a-la-carte-robomaker==1.34.98
-rolesanywhere = botocore-a-la-carte-rolesanywhere==1.34.98
-route53 = botocore-a-la-carte-route53==1.34.98
-route53-recovery-cluster = botocore-a-la-carte-route53-recovery-cluster==1.34.98
-route53-recovery-control-config = botocore-a-la-carte-route53-recovery-control-config==1.34.98
-route53-recovery-readiness = botocore-a-la-carte-route53-recovery-readiness==1.34.98
-route53domains = botocore-a-la-carte-route53domains==1.34.98
-route53profiles = botocore-a-la-carte-route53profiles==1.34.98
-route53resolver = botocore-a-la-carte-route53resolver==1.34.98
-rum = botocore-a-la-carte-rum==1.34.98
-s3 = botocore-a-la-carte-s3==1.34.98
-s3control = botocore-a-la-carte-s3control==1.34.98
-s3outposts = botocore-a-la-carte-s3outposts==1.34.98
-sagemaker = botocore-a-la-carte-sagemaker==1.34.98
-sagemaker-a2i-runtime = botocore-a-la-carte-sagemaker-a2i-runtime==1.34.98
-sagemaker-edge = botocore-a-la-carte-sagemaker-edge==1.34.98
-sagemaker-featurestore-runtime = botocore-a-la-carte-sagemaker-featurestore-runtime==1.34.98
-sagemaker-geospatial = botocore-a-la-carte-sagemaker-geospatial==1.34.98
-sagemaker-metrics = botocore-a-la-carte-sagemaker-metrics==1.34.98
-sagemaker-runtime = botocore-a-la-carte-sagemaker-runtime==1.34.98
-savingsplans = botocore-a-la-carte-savingsplans==1.34.98
-scheduler = botocore-a-la-carte-scheduler==1.34.98
-schemas = botocore-a-la-carte-schemas==1.34.98
-sdb = botocore-a-la-carte-sdb==1.34.98
-secretsmanager = botocore-a-la-carte-secretsmanager==1.34.98
-securityhub = botocore-a-la-carte-securityhub==1.34.98
-securitylake = botocore-a-la-carte-securitylake==1.34.98
-serverlessrepo = botocore-a-la-carte-serverlessrepo==1.34.98
-service-quotas = botocore-a-la-carte-service-quotas==1.34.98
-servicecatalog = botocore-a-la-carte-servicecatalog==1.34.98
-servicecatalog-appregistry = botocore-a-la-carte-servicecatalog-appregistry==1.34.98
-servicediscovery = botocore-a-la-carte-servicediscovery==1.34.98
-ses = botocore-a-la-carte-ses==1.34.98
-sesv2 = botocore-a-la-carte-sesv2==1.34.98
-shield = botocore-a-la-carte-shield==1.34.98
-signer = botocore-a-la-carte-signer==1.34.98
-simspaceweaver = botocore-a-la-carte-simspaceweaver==1.34.98
-sms = botocore-a-la-carte-sms==1.34.98
-sms-voice = botocore-a-la-carte-sms-voice==1.34.98
-snow-device-management = botocore-a-la-carte-snow-device-management==1.34.98
-snowball = botocore-a-la-carte-snowball==1.34.98
-sns = botocore-a-la-carte-sns==1.34.98
-sqs = botocore-a-la-carte-sqs==1.34.98
-ssm = botocore-a-la-carte-ssm==1.34.98
-ssm-contacts = botocore-a-la-carte-ssm-contacts==1.34.98
-ssm-incidents = botocore-a-la-carte-ssm-incidents==1.34.98
-ssm-sap = botocore-a-la-carte-ssm-sap==1.34.98
-sso = botocore-a-la-carte-sso==1.34.98
-sso-admin = botocore-a-la-carte-sso-admin==1.34.98
-sso-oidc = botocore-a-la-carte-sso-oidc==1.34.98
-stepfunctions = botocore-a-la-carte-stepfunctions==1.34.98
-storagegateway = botocore-a-la-carte-storagegateway==1.34.98
-sts = botocore-a-la-carte-sts==1.34.98
-supplychain = botocore-a-la-carte-supplychain==1.34.98
-support = botocore-a-la-carte-support==1.34.98
-support-app = botocore-a-la-carte-support-app==1.34.98
-swf = botocore-a-la-carte-swf==1.34.98
-synthetics = botocore-a-la-carte-synthetics==1.34.98
-textract = botocore-a-la-carte-textract==1.34.98
-timestream-influxdb = botocore-a-la-carte-timestream-influxdb==1.34.98
-timestream-query = botocore-a-la-carte-timestream-query==1.34.98
-timestream-write = botocore-a-la-carte-timestream-write==1.34.98
-tnb = botocore-a-la-carte-tnb==1.34.98
-transcribe = botocore-a-la-carte-transcribe==1.34.98
-transfer = botocore-a-la-carte-transfer==1.34.98
-translate = botocore-a-la-carte-translate==1.34.98
-trustedadvisor = botocore-a-la-carte-trustedadvisor==1.34.98
-verifiedpermissions = botocore-a-la-carte-verifiedpermissions==1.34.98
-voice-id = botocore-a-la-carte-voice-id==1.34.98
-vpc-lattice = botocore-a-la-carte-vpc-lattice==1.34.98
-waf = botocore-a-la-carte-waf==1.34.98
-waf-regional = botocore-a-la-carte-waf-regional==1.34.98
-wafv2 = botocore-a-la-carte-wafv2==1.34.98
-wellarchitected = botocore-a-la-carte-wellarchitected==1.34.98
-wisdom = botocore-a-la-carte-wisdom==1.34.98
-workdocs = botocore-a-la-carte-workdocs==1.34.98
-worklink = botocore-a-la-carte-worklink==1.34.98
-workmail = botocore-a-la-carte-workmail==1.34.98
-workmailmessageflow = botocore-a-la-carte-workmailmessageflow==1.34.98
-workspaces = botocore-a-la-carte-workspaces==1.34.98
-workspaces-thin-client = botocore-a-la-carte-workspaces-thin-client==1.34.98
-workspaces-web = botocore-a-la-carte-workspaces-web==1.34.98
-xray = botocore-a-la-carte-xray==1.34.98
+accessanalyzer = botocore-a-la-carte-accessanalyzer==1.34.99
+account = botocore-a-la-carte-account==1.34.99
+acm = botocore-a-la-carte-acm==1.34.99
+acm-pca = botocore-a-la-carte-acm-pca==1.34.99
+alexaforbusiness = botocore-a-la-carte-alexaforbusiness==1.34.99
+amp = botocore-a-la-carte-amp==1.34.99
+amplify = botocore-a-la-carte-amplify==1.34.99
+amplifybackend = botocore-a-la-carte-amplifybackend==1.34.99
+amplifyuibuilder = botocore-a-la-carte-amplifyuibuilder==1.34.99
+apigateway = botocore-a-la-carte-apigateway==1.34.99
+apigatewaymanagementapi = botocore-a-la-carte-apigatewaymanagementapi==1.34.99
+apigatewayv2 = botocore-a-la-carte-apigatewayv2==1.34.99
+appconfig = botocore-a-la-carte-appconfig==1.34.99
+appconfigdata = botocore-a-la-carte-appconfigdata==1.34.99
+appfabric = botocore-a-la-carte-appfabric==1.34.99
+appflow = botocore-a-la-carte-appflow==1.34.99
+appintegrations = botocore-a-la-carte-appintegrations==1.34.99
+application-autoscaling = botocore-a-la-carte-application-autoscaling==1.34.99
+application-insights = botocore-a-la-carte-application-insights==1.34.99
+applicationcostprofiler = botocore-a-la-carte-applicationcostprofiler==1.34.99
+appmesh = botocore-a-la-carte-appmesh==1.34.99
+apprunner = botocore-a-la-carte-apprunner==1.34.99
+appstream = botocore-a-la-carte-appstream==1.34.99
+appsync = botocore-a-la-carte-appsync==1.34.99
+arc-zonal-shift = botocore-a-la-carte-arc-zonal-shift==1.34.99
+artifact = botocore-a-la-carte-artifact==1.34.99
+athena = botocore-a-la-carte-athena==1.34.99
+auditmanager = botocore-a-la-carte-auditmanager==1.34.99
+autoscaling = botocore-a-la-carte-autoscaling==1.34.99
+autoscaling-plans = botocore-a-la-carte-autoscaling-plans==1.34.99
+b2bi = botocore-a-la-carte-b2bi==1.34.99
+backup = botocore-a-la-carte-backup==1.34.99
+backup-gateway = botocore-a-la-carte-backup-gateway==1.34.99
+backupstorage = botocore-a-la-carte-backupstorage==1.34.99
+batch = botocore-a-la-carte-batch==1.34.99
+bcm-data-exports = botocore-a-la-carte-bcm-data-exports==1.34.99
+bedrock = botocore-a-la-carte-bedrock==1.34.99
+bedrock-agent = botocore-a-la-carte-bedrock-agent==1.34.99
+bedrock-agent-runtime = botocore-a-la-carte-bedrock-agent-runtime==1.34.99
+bedrock-runtime = botocore-a-la-carte-bedrock-runtime==1.34.99
+billingconductor = botocore-a-la-carte-billingconductor==1.34.99
+braket = botocore-a-la-carte-braket==1.34.99
+budgets = botocore-a-la-carte-budgets==1.34.99
+ce = botocore-a-la-carte-ce==1.34.99
+chatbot = botocore-a-la-carte-chatbot==1.34.99
+chime = botocore-a-la-carte-chime==1.34.99
+chime-sdk-identity = botocore-a-la-carte-chime-sdk-identity==1.34.99
+chime-sdk-media-pipelines = botocore-a-la-carte-chime-sdk-media-pipelines==1.34.99
+chime-sdk-meetings = botocore-a-la-carte-chime-sdk-meetings==1.34.99
+chime-sdk-messaging = botocore-a-la-carte-chime-sdk-messaging==1.34.99
+chime-sdk-voice = botocore-a-la-carte-chime-sdk-voice==1.34.99
+cleanrooms = botocore-a-la-carte-cleanrooms==1.34.99
+cleanroomsml = botocore-a-la-carte-cleanroomsml==1.34.99
+cloud9 = botocore-a-la-carte-cloud9==1.34.99
+cloudcontrol = botocore-a-la-carte-cloudcontrol==1.34.99
+clouddirectory = botocore-a-la-carte-clouddirectory==1.34.99
+cloudformation = botocore-a-la-carte-cloudformation==1.34.99
+cloudfront = botocore-a-la-carte-cloudfront==1.34.99
+cloudfront-keyvaluestore = botocore-a-la-carte-cloudfront-keyvaluestore==1.34.99
+cloudhsm = botocore-a-la-carte-cloudhsm==1.34.99
+cloudhsmv2 = botocore-a-la-carte-cloudhsmv2==1.34.99
+cloudsearch = botocore-a-la-carte-cloudsearch==1.34.99
+cloudsearchdomain = botocore-a-la-carte-cloudsearchdomain==1.34.99
+cloudtrail = botocore-a-la-carte-cloudtrail==1.34.99
+cloudtrail-data = botocore-a-la-carte-cloudtrail-data==1.34.99
+cloudwatch = botocore-a-la-carte-cloudwatch==1.34.99
+codeartifact = botocore-a-la-carte-codeartifact==1.34.99
+codebuild = botocore-a-la-carte-codebuild==1.34.99
+codecatalyst = botocore-a-la-carte-codecatalyst==1.34.99
+codecommit = botocore-a-la-carte-codecommit==1.34.99
+codeconnections = botocore-a-la-carte-codeconnections==1.34.99
+codedeploy = botocore-a-la-carte-codedeploy==1.34.99
+codeguru-reviewer = botocore-a-la-carte-codeguru-reviewer==1.34.99
+codeguru-security = botocore-a-la-carte-codeguru-security==1.34.99
+codeguruprofiler = botocore-a-la-carte-codeguruprofiler==1.34.99
+codepipeline = botocore-a-la-carte-codepipeline==1.34.99
+codestar = botocore-a-la-carte-codestar==1.34.99
+codestar-connections = botocore-a-la-carte-codestar-connections==1.34.99
+codestar-notifications = botocore-a-la-carte-codestar-notifications==1.34.99
+cognito-identity = botocore-a-la-carte-cognito-identity==1.34.99
+cognito-idp = botocore-a-la-carte-cognito-idp==1.34.99
+cognito-sync = botocore-a-la-carte-cognito-sync==1.34.99
+comprehend = botocore-a-la-carte-comprehend==1.34.99
+comprehendmedical = botocore-a-la-carte-comprehendmedical==1.34.99
+compute-optimizer = botocore-a-la-carte-compute-optimizer==1.34.99
+config = botocore-a-la-carte-config==1.34.99
+connect = botocore-a-la-carte-connect==1.34.99
+connect-contact-lens = botocore-a-la-carte-connect-contact-lens==1.34.99
+connectcampaigns = botocore-a-la-carte-connectcampaigns==1.34.99
+connectcases = botocore-a-la-carte-connectcases==1.34.99
+connectparticipant = botocore-a-la-carte-connectparticipant==1.34.99
+controlcatalog = botocore-a-la-carte-controlcatalog==1.34.99
+controltower = botocore-a-la-carte-controltower==1.34.99
+cost-optimization-hub = botocore-a-la-carte-cost-optimization-hub==1.34.99
+cur = botocore-a-la-carte-cur==1.34.99
+customer-profiles = botocore-a-la-carte-customer-profiles==1.34.99
+databrew = botocore-a-la-carte-databrew==1.34.99
+dataexchange = botocore-a-la-carte-dataexchange==1.34.99
+datapipeline = botocore-a-la-carte-datapipeline==1.34.99
+datasync = botocore-a-la-carte-datasync==1.34.99
+datazone = botocore-a-la-carte-datazone==1.34.99
+dax = botocore-a-la-carte-dax==1.34.99
+deadline = botocore-a-la-carte-deadline==1.34.99
+detective = botocore-a-la-carte-detective==1.34.99
+devicefarm = botocore-a-la-carte-devicefarm==1.34.99
+devops-guru = botocore-a-la-carte-devops-guru==1.34.99
+directconnect = botocore-a-la-carte-directconnect==1.34.99
+discovery = botocore-a-la-carte-discovery==1.34.99
+dlm = botocore-a-la-carte-dlm==1.34.99
+dms = botocore-a-la-carte-dms==1.34.99
+docdb = botocore-a-la-carte-docdb==1.34.99
+docdb-elastic = botocore-a-la-carte-docdb-elastic==1.34.99
+drs = botocore-a-la-carte-drs==1.34.99
+ds = botocore-a-la-carte-ds==1.34.99
+dynamodb = botocore-a-la-carte-dynamodb==1.34.99
+dynamodbstreams = botocore-a-la-carte-dynamodbstreams==1.34.99
+ebs = botocore-a-la-carte-ebs==1.34.99
+ec2 = botocore-a-la-carte-ec2==1.34.99
+ec2-instance-connect = botocore-a-la-carte-ec2-instance-connect==1.34.99
+ecr = botocore-a-la-carte-ecr==1.34.99
+ecr-public = botocore-a-la-carte-ecr-public==1.34.99
+ecs = botocore-a-la-carte-ecs==1.34.99
+efs = botocore-a-la-carte-efs==1.34.99
+eks = botocore-a-la-carte-eks==1.34.99
+eks-auth = botocore-a-la-carte-eks-auth==1.34.99
+elastic-inference = botocore-a-la-carte-elastic-inference==1.34.99
+elasticache = botocore-a-la-carte-elasticache==1.34.99
+elasticbeanstalk = botocore-a-la-carte-elasticbeanstalk==1.34.99
+elastictranscoder = botocore-a-la-carte-elastictranscoder==1.34.99
+elb = botocore-a-la-carte-elb==1.34.99
+elbv2 = botocore-a-la-carte-elbv2==1.34.99
+emr = botocore-a-la-carte-emr==1.34.99
+emr-containers = botocore-a-la-carte-emr-containers==1.34.99
+emr-serverless = botocore-a-la-carte-emr-serverless==1.34.99
+entityresolution = botocore-a-la-carte-entityresolution==1.34.99
+es = botocore-a-la-carte-es==1.34.99
+events = botocore-a-la-carte-events==1.34.99
+evidently = botocore-a-la-carte-evidently==1.34.99
+finspace = botocore-a-la-carte-finspace==1.34.99
+finspace-data = botocore-a-la-carte-finspace-data==1.34.99
+firehose = botocore-a-la-carte-firehose==1.34.99
+fis = botocore-a-la-carte-fis==1.34.99
+fms = botocore-a-la-carte-fms==1.34.99
+forecast = botocore-a-la-carte-forecast==1.34.99
+forecastquery = botocore-a-la-carte-forecastquery==1.34.99
+frauddetector = botocore-a-la-carte-frauddetector==1.34.99
+freetier = botocore-a-la-carte-freetier==1.34.99
+fsx = botocore-a-la-carte-fsx==1.34.99
+gamelift = botocore-a-la-carte-gamelift==1.34.99
+glacier = botocore-a-la-carte-glacier==1.34.99
+globalaccelerator = botocore-a-la-carte-globalaccelerator==1.34.99
+glue = botocore-a-la-carte-glue==1.34.99
+grafana = botocore-a-la-carte-grafana==1.34.99
+greengrass = botocore-a-la-carte-greengrass==1.34.99
+greengrassv2 = botocore-a-la-carte-greengrassv2==1.34.99
+groundstation = botocore-a-la-carte-groundstation==1.34.99
+guardduty = botocore-a-la-carte-guardduty==1.34.99
+health = botocore-a-la-carte-health==1.34.99
+healthlake = botocore-a-la-carte-healthlake==1.34.99
+honeycode = botocore-a-la-carte-honeycode==1.34.99
+iam = botocore-a-la-carte-iam==1.34.99
+identitystore = botocore-a-la-carte-identitystore==1.34.99
+imagebuilder = botocore-a-la-carte-imagebuilder==1.34.99
+importexport = botocore-a-la-carte-importexport==1.34.99
+inspector = botocore-a-la-carte-inspector==1.34.99
+inspector-scan = botocore-a-la-carte-inspector-scan==1.34.99
+inspector2 = botocore-a-la-carte-inspector2==1.34.99
+internetmonitor = botocore-a-la-carte-internetmonitor==1.34.99
+iot = botocore-a-la-carte-iot==1.34.99
+iot-data = botocore-a-la-carte-iot-data==1.34.99
+iot-jobs-data = botocore-a-la-carte-iot-jobs-data==1.34.99
+iot1click-devices = botocore-a-la-carte-iot1click-devices==1.34.99
+iot1click-projects = botocore-a-la-carte-iot1click-projects==1.34.99
+iotanalytics = botocore-a-la-carte-iotanalytics==1.34.99
+iotdeviceadvisor = botocore-a-la-carte-iotdeviceadvisor==1.34.99
+iotevents = botocore-a-la-carte-iotevents==1.34.99
+iotevents-data = botocore-a-la-carte-iotevents-data==1.34.99
+iotfleethub = botocore-a-la-carte-iotfleethub==1.34.99
+iotfleetwise = botocore-a-la-carte-iotfleetwise==1.34.99
+iotsecuretunneling = botocore-a-la-carte-iotsecuretunneling==1.34.99
+iotsitewise = botocore-a-la-carte-iotsitewise==1.34.99
+iotthingsgraph = botocore-a-la-carte-iotthingsgraph==1.34.99
+iottwinmaker = botocore-a-la-carte-iottwinmaker==1.34.99
+iotwireless = botocore-a-la-carte-iotwireless==1.34.99
+ivs = botocore-a-la-carte-ivs==1.34.99
+ivs-realtime = botocore-a-la-carte-ivs-realtime==1.34.99
+ivschat = botocore-a-la-carte-ivschat==1.34.99
+kafka = botocore-a-la-carte-kafka==1.34.99
+kafkaconnect = botocore-a-la-carte-kafkaconnect==1.34.99
+kendra = botocore-a-la-carte-kendra==1.34.99
+kendra-ranking = botocore-a-la-carte-kendra-ranking==1.34.99
+keyspaces = botocore-a-la-carte-keyspaces==1.34.99
+kinesis = botocore-a-la-carte-kinesis==1.34.99
+kinesis-video-archived-media = botocore-a-la-carte-kinesis-video-archived-media==1.34.99
+kinesis-video-media = botocore-a-la-carte-kinesis-video-media==1.34.99
+kinesis-video-signaling = botocore-a-la-carte-kinesis-video-signaling==1.34.99
+kinesis-video-webrtc-storage = botocore-a-la-carte-kinesis-video-webrtc-storage==1.34.99
+kinesisanalytics = botocore-a-la-carte-kinesisanalytics==1.34.99
+kinesisanalyticsv2 = botocore-a-la-carte-kinesisanalyticsv2==1.34.99
+kinesisvideo = botocore-a-la-carte-kinesisvideo==1.34.99
+kms = botocore-a-la-carte-kms==1.34.99
+lakeformation = botocore-a-la-carte-lakeformation==1.34.99
+lambda = botocore-a-la-carte-lambda==1.34.99
+launch-wizard = botocore-a-la-carte-launch-wizard==1.34.99
+lex-models = botocore-a-la-carte-lex-models==1.34.99
+lex-runtime = botocore-a-la-carte-lex-runtime==1.34.99
+lexv2-models = botocore-a-la-carte-lexv2-models==1.34.99
+lexv2-runtime = botocore-a-la-carte-lexv2-runtime==1.34.99
+license-manager = botocore-a-la-carte-license-manager==1.34.99
+license-manager-linux-subscriptions = botocore-a-la-carte-license-manager-linux-subscriptions==1.34.99
+license-manager-user-subscriptions = botocore-a-la-carte-license-manager-user-subscriptions==1.34.99
+lightsail = botocore-a-la-carte-lightsail==1.34.99
+location = botocore-a-la-carte-location==1.34.99
+logs = botocore-a-la-carte-logs==1.34.99
+lookoutequipment = botocore-a-la-carte-lookoutequipment==1.34.99
+lookoutmetrics = botocore-a-la-carte-lookoutmetrics==1.34.99
+lookoutvision = botocore-a-la-carte-lookoutvision==1.34.99
+m2 = botocore-a-la-carte-m2==1.34.99
+machinelearning = botocore-a-la-carte-machinelearning==1.34.99
+macie2 = botocore-a-la-carte-macie2==1.34.99
+managedblockchain = botocore-a-la-carte-managedblockchain==1.34.99
+managedblockchain-query = botocore-a-la-carte-managedblockchain-query==1.34.99
+marketplace-agreement = botocore-a-la-carte-marketplace-agreement==1.34.99
+marketplace-catalog = botocore-a-la-carte-marketplace-catalog==1.34.99
+marketplace-deployment = botocore-a-la-carte-marketplace-deployment==1.34.99
+marketplace-entitlement = botocore-a-la-carte-marketplace-entitlement==1.34.99
+marketplacecommerceanalytics = botocore-a-la-carte-marketplacecommerceanalytics==1.34.99
+mediaconnect = botocore-a-la-carte-mediaconnect==1.34.99
+mediaconvert = botocore-a-la-carte-mediaconvert==1.34.99
+medialive = botocore-a-la-carte-medialive==1.34.99
+mediapackage = botocore-a-la-carte-mediapackage==1.34.99
+mediapackage-vod = botocore-a-la-carte-mediapackage-vod==1.34.99
+mediapackagev2 = botocore-a-la-carte-mediapackagev2==1.34.99
+mediastore = botocore-a-la-carte-mediastore==1.34.99
+mediastore-data = botocore-a-la-carte-mediastore-data==1.34.99
+mediatailor = botocore-a-la-carte-mediatailor==1.34.99
+medical-imaging = botocore-a-la-carte-medical-imaging==1.34.99
+memorydb = botocore-a-la-carte-memorydb==1.34.99
+meteringmarketplace = botocore-a-la-carte-meteringmarketplace==1.34.99
+mgh = botocore-a-la-carte-mgh==1.34.99
+mgn = botocore-a-la-carte-mgn==1.34.99
+migration-hub-refactor-spaces = botocore-a-la-carte-migration-hub-refactor-spaces==1.34.99
+migrationhub-config = botocore-a-la-carte-migrationhub-config==1.34.99
+migrationhuborchestrator = botocore-a-la-carte-migrationhuborchestrator==1.34.99
+migrationhubstrategy = botocore-a-la-carte-migrationhubstrategy==1.34.99
+mobile = botocore-a-la-carte-mobile==1.34.99
+mq = botocore-a-la-carte-mq==1.34.99
+mturk = botocore-a-la-carte-mturk==1.34.99
+mwaa = botocore-a-la-carte-mwaa==1.34.99
+neptune = botocore-a-la-carte-neptune==1.34.99
+neptune-graph = botocore-a-la-carte-neptune-graph==1.34.99
+neptunedata = botocore-a-la-carte-neptunedata==1.34.99
+network-firewall = botocore-a-la-carte-network-firewall==1.34.99
+networkmanager = botocore-a-la-carte-networkmanager==1.34.99
+networkmonitor = botocore-a-la-carte-networkmonitor==1.34.99
+nimble = botocore-a-la-carte-nimble==1.34.99
+oam = botocore-a-la-carte-oam==1.34.99
+omics = botocore-a-la-carte-omics==1.34.99
+opensearch = botocore-a-la-carte-opensearch==1.34.99
+opensearchserverless = botocore-a-la-carte-opensearchserverless==1.34.99
+opsworks = botocore-a-la-carte-opsworks==1.34.99
+opsworkscm = botocore-a-la-carte-opsworkscm==1.34.99
+organizations = botocore-a-la-carte-organizations==1.34.99
+osis = botocore-a-la-carte-osis==1.34.99
+outposts = botocore-a-la-carte-outposts==1.34.99
+panorama = botocore-a-la-carte-panorama==1.34.99
+payment-cryptography = botocore-a-la-carte-payment-cryptography==1.34.99
+payment-cryptography-data = botocore-a-la-carte-payment-cryptography-data==1.34.99
+pca-connector-ad = botocore-a-la-carte-pca-connector-ad==1.34.99
+personalize = botocore-a-la-carte-personalize==1.34.99
+personalize-events = botocore-a-la-carte-personalize-events==1.34.99
+personalize-runtime = botocore-a-la-carte-personalize-runtime==1.34.99
+pi = botocore-a-la-carte-pi==1.34.99
+pinpoint = botocore-a-la-carte-pinpoint==1.34.99
+pinpoint-email = botocore-a-la-carte-pinpoint-email==1.34.99
+pinpoint-sms-voice = botocore-a-la-carte-pinpoint-sms-voice==1.34.99
+pinpoint-sms-voice-v2 = botocore-a-la-carte-pinpoint-sms-voice-v2==1.34.99
+pipes = botocore-a-la-carte-pipes==1.34.99
+polly = botocore-a-la-carte-polly==1.34.99
+pricing = botocore-a-la-carte-pricing==1.34.99
+privatenetworks = botocore-a-la-carte-privatenetworks==1.34.99
+proton = botocore-a-la-carte-proton==1.34.99
+qbusiness = botocore-a-la-carte-qbusiness==1.34.99
+qconnect = botocore-a-la-carte-qconnect==1.34.99
+qldb = botocore-a-la-carte-qldb==1.34.99
+qldb-session = botocore-a-la-carte-qldb-session==1.34.99
+quicksight = botocore-a-la-carte-quicksight==1.34.99
+ram = botocore-a-la-carte-ram==1.34.99
+rbin = botocore-a-la-carte-rbin==1.34.99
+rds = botocore-a-la-carte-rds==1.34.99
+rds-data = botocore-a-la-carte-rds-data==1.34.99
+redshift = botocore-a-la-carte-redshift==1.34.99
+redshift-data = botocore-a-la-carte-redshift-data==1.34.99
+redshift-serverless = botocore-a-la-carte-redshift-serverless==1.34.99
+rekognition = botocore-a-la-carte-rekognition==1.34.99
+repostspace = botocore-a-la-carte-repostspace==1.34.99
+resiliencehub = botocore-a-la-carte-resiliencehub==1.34.99
+resource-explorer-2 = botocore-a-la-carte-resource-explorer-2==1.34.99
+resource-groups = botocore-a-la-carte-resource-groups==1.34.99
+resourcegroupstaggingapi = botocore-a-la-carte-resourcegroupstaggingapi==1.34.99
+robomaker = botocore-a-la-carte-robomaker==1.34.99
+rolesanywhere = botocore-a-la-carte-rolesanywhere==1.34.99
+route53 = botocore-a-la-carte-route53==1.34.99
+route53-recovery-cluster = botocore-a-la-carte-route53-recovery-cluster==1.34.99
+route53-recovery-control-config = botocore-a-la-carte-route53-recovery-control-config==1.34.99
+route53-recovery-readiness = botocore-a-la-carte-route53-recovery-readiness==1.34.99
+route53domains = botocore-a-la-carte-route53domains==1.34.99
+route53profiles = botocore-a-la-carte-route53profiles==1.34.99
+route53resolver = botocore-a-la-carte-route53resolver==1.34.99
+rum = botocore-a-la-carte-rum==1.34.99
+s3 = botocore-a-la-carte-s3==1.34.99
+s3control = botocore-a-la-carte-s3control==1.34.99
+s3outposts = botocore-a-la-carte-s3outposts==1.34.99
+sagemaker = botocore-a-la-carte-sagemaker==1.34.99
+sagemaker-a2i-runtime = botocore-a-la-carte-sagemaker-a2i-runtime==1.34.99
+sagemaker-edge = botocore-a-la-carte-sagemaker-edge==1.34.99
+sagemaker-featurestore-runtime = botocore-a-la-carte-sagemaker-featurestore-runtime==1.34.99
+sagemaker-geospatial = botocore-a-la-carte-sagemaker-geospatial==1.34.99
+sagemaker-metrics = botocore-a-la-carte-sagemaker-metrics==1.34.99
+sagemaker-runtime = botocore-a-la-carte-sagemaker-runtime==1.34.99
+savingsplans = botocore-a-la-carte-savingsplans==1.34.99
+scheduler = botocore-a-la-carte-scheduler==1.34.99
+schemas = botocore-a-la-carte-schemas==1.34.99
+sdb = botocore-a-la-carte-sdb==1.34.99
+secretsmanager = botocore-a-la-carte-secretsmanager==1.34.99
+securityhub = botocore-a-la-carte-securityhub==1.34.99
+securitylake = botocore-a-la-carte-securitylake==1.34.99
+serverlessrepo = botocore-a-la-carte-serverlessrepo==1.34.99
+service-quotas = botocore-a-la-carte-service-quotas==1.34.99
+servicecatalog = botocore-a-la-carte-servicecatalog==1.34.99
+servicecatalog-appregistry = botocore-a-la-carte-servicecatalog-appregistry==1.34.99
+servicediscovery = botocore-a-la-carte-servicediscovery==1.34.99
+ses = botocore-a-la-carte-ses==1.34.99
+sesv2 = botocore-a-la-carte-sesv2==1.34.99
+shield = botocore-a-la-carte-shield==1.34.99
+signer = botocore-a-la-carte-signer==1.34.99
+simspaceweaver = botocore-a-la-carte-simspaceweaver==1.34.99
+sms = botocore-a-la-carte-sms==1.34.99
+sms-voice = botocore-a-la-carte-sms-voice==1.34.99
+snow-device-management = botocore-a-la-carte-snow-device-management==1.34.99
+snowball = botocore-a-la-carte-snowball==1.34.99
+sns = botocore-a-la-carte-sns==1.34.99
+sqs = botocore-a-la-carte-sqs==1.34.99
+ssm = botocore-a-la-carte-ssm==1.34.99
+ssm-contacts = botocore-a-la-carte-ssm-contacts==1.34.99
+ssm-incidents = botocore-a-la-carte-ssm-incidents==1.34.99
+ssm-sap = botocore-a-la-carte-ssm-sap==1.34.99
+sso = botocore-a-la-carte-sso==1.34.99
+sso-admin = botocore-a-la-carte-sso-admin==1.34.99
+sso-oidc = botocore-a-la-carte-sso-oidc==1.34.99
+stepfunctions = botocore-a-la-carte-stepfunctions==1.34.99
+storagegateway = botocore-a-la-carte-storagegateway==1.34.99
+sts = botocore-a-la-carte-sts==1.34.99
+supplychain = botocore-a-la-carte-supplychain==1.34.99
+support = botocore-a-la-carte-support==1.34.99
+support-app = botocore-a-la-carte-support-app==1.34.99
+swf = botocore-a-la-carte-swf==1.34.99
+synthetics = botocore-a-la-carte-synthetics==1.34.99
+textract = botocore-a-la-carte-textract==1.34.99
+timestream-influxdb = botocore-a-la-carte-timestream-influxdb==1.34.99
+timestream-query = botocore-a-la-carte-timestream-query==1.34.99
+timestream-write = botocore-a-la-carte-timestream-write==1.34.99
+tnb = botocore-a-la-carte-tnb==1.34.99
+transcribe = botocore-a-la-carte-transcribe==1.34.99
+transfer = botocore-a-la-carte-transfer==1.34.99
+translate = botocore-a-la-carte-translate==1.34.99
+trustedadvisor = botocore-a-la-carte-trustedadvisor==1.34.99
+verifiedpermissions = botocore-a-la-carte-verifiedpermissions==1.34.99
+voice-id = botocore-a-la-carte-voice-id==1.34.99
+vpc-lattice = botocore-a-la-carte-vpc-lattice==1.34.99
+waf = botocore-a-la-carte-waf==1.34.99
+waf-regional = botocore-a-la-carte-waf-regional==1.34.99
+wafv2 = botocore-a-la-carte-wafv2==1.34.99
+wellarchitected = botocore-a-la-carte-wellarchitected==1.34.99
+wisdom = botocore-a-la-carte-wisdom==1.34.99
+workdocs = botocore-a-la-carte-workdocs==1.34.99
+worklink = botocore-a-la-carte-worklink==1.34.99
+workmail = botocore-a-la-carte-workmail==1.34.99
+workmailmessageflow = botocore-a-la-carte-workmailmessageflow==1.34.99
+workspaces = botocore-a-la-carte-workspaces==1.34.99
+workspaces-thin-client = botocore-a-la-carte-workspaces-thin-client==1.34.99
+workspaces-web = botocore-a-la-carte-workspaces-web==1.34.99
+xray = botocore-a-la-carte-xray==1.34.99
 
 [flake8]
 ignore = E203,E226,E501,E731,W503,W504
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `botocore-a-la-carte-1.34.98/setup.py` & `botocore-a-la-carte-1.34.99/setup.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/__init__.py` & `botocore-a-la-carte-1.34.99/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/acceptance/features/environment.py` & `botocore-a-la-carte-1.34.99/tests/acceptance/features/environment.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/autoscaling/autoscaling.feature` & `botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/autoscaling/autoscaling.feature`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/cognitoidentity/cognitoidentity.feature` & `botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/cognitoidentity/cognitoidentity.feature`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/acceptance/features/smoke/support/support.feature` & `botocore-a-la-carte-1.34.99/tests/acceptance/features/smoke/support/support.feature`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/acceptance/features/steps/base.py` & `botocore-a-la-carte-1.34.99/tests/acceptance/features/steps/base.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/cmd-runner` & `botocore-a-la-carte-1.34.99/tests/cmd-runner`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/__init__.py` & `botocore-a-la-carte-1.34.99/tests/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/configured_endpoint_urls/__init__.py` & `botocore-a-la-carte-1.34.99/tests/functional/configured_endpoint_urls/__init__.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/configured_endpoint_urls/profile-tests.json` & `botocore-a-la-carte-1.34.99/tests/functional/configured_endpoint_urls/profile-tests.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/configured_endpoint_urls/test_configured_endpoint_url.py` & `botocore-a-la-carte-1.34.99/tests/functional/configured_endpoint_urls/test_configured_endpoint_url.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/conftest.py` & `botocore-a-la-carte-1.34.99/tests/functional/conftest.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/csm/__init__.py` & `botocore-a-la-carte-1.34.99/tests/functional/csm/__init__.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/csm/cases.json` & `botocore-a-la-carte-1.34.99/tests/functional/csm/cases.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/csm/data/csmtest/2018-06-19/service-2.json` & `botocore-a-la-carte-1.34.99/tests/functional/csm/data/csmtest/2018-06-19/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/csm/test_monitoring.py` & `botocore-a-la-carte-1.34.99/tests/functional/csm/test_monitoring.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/docs/__init__.py` & `botocore-a-la-carte-1.34.99/tests/functional/docs/__init__.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/docs/test_alias.py` & `botocore-a-la-carte-1.34.99/tests/functional/docs/test_alias.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/docs/test_autoscaling.py` & `botocore-a-la-carte-1.34.99/tests/functional/docs/test_autoscaling.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/docs/test_ec2.py` & `botocore-a-la-carte-1.34.99/tests/functional/docs/test_ec2.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/docs/test_glacier.py` & `botocore-a-la-carte-1.34.99/tests/functional/docs/test_glacier.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/docs/test_lex.py` & `botocore-a-la-carte-1.34.99/tests/functional/docs/test_lex.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/docs/test_s3.py` & `botocore-a-la-carte-1.34.99/tests/functional/docs/test_s3.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/docs/test_secretsmanager.py` & `botocore-a-la-carte-1.34.99/tests/functional/docs/test_secretsmanager.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/docs/test_shared_example_config.py` & `botocore-a-la-carte-1.34.99/tests/functional/docs/test_shared_example_config.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/docs/test_streaming_body.py` & `botocore-a-la-carte-1.34.99/tests/functional/docs/test_streaming_body.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/accessanalyzer/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/accessanalyzer/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/account/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/account/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/acm/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/acm/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/acm-pca/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/acm-pca/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/alexaforbusiness/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/alexaforbusiness/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/amp/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/amp/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/amplify/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/amplify/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/amplifybackend/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/amplifybackend/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/amplifyuibuilder/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/amplifyuibuilder/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/apigateway/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/apigateway/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/apigatewaymanagementapi/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/apigatewaymanagementapi/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/apigatewayv2/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/apigatewayv2/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/appconfig/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/appconfig/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/appconfigdata/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/appconfigdata/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/appfabric/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/appfabric/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/appflow/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/appflow/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/appintegrations/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/appintegrations/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/application-autoscaling/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/application-autoscaling/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/application-insights/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/application-insights/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/applicationcostprofiler/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/applicationcostprofiler/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/appmesh/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/appmesh/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/apprunner/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/apprunner/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/appstream/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/appstream/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/appsync/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/appsync/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/arc-zonal-shift/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/arc-zonal-shift/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/artifact/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/artifact/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/athena/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/athena/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/auditmanager/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/auditmanager/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/autoscaling/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/autoscaling/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/autoscaling-plans/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/autoscaling-plans/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/b2bi/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/b2bi/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/backup/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/backup/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/backup-gateway/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/backup-gateway/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/backupstorage/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/backupstorage/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/batch/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/batch/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/bcm-data-exports/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/bcm-data-exports/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/bedrock/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/bedrock/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/bedrock-agent/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/bedrock-agent/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/bedrock-agent-runtime/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/bedrock-agent-runtime/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/bedrock-runtime/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/bedrock-runtime/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/billingconductor/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/billingconductor/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/braket/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/braket/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/budgets/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/budgets/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/ce/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/ce/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/chatbot/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/chatbot/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/chime/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/chime/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/chime-sdk-identity/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/chime-sdk-identity/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/chime-sdk-media-pipelines/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/chime-sdk-media-pipelines/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/chime-sdk-meetings/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/chime-sdk-meetings/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/chime-sdk-messaging/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/chime-sdk-messaging/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/chime-sdk-voice/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/chime-sdk-voice/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/cleanrooms/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/cleanrooms/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/cleanroomsml/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/cleanroomsml/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/cloud9/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/cloud9/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/cloudcontrol/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/cloudcontrol/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/clouddirectory/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/clouddirectory/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/cloudformation/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/cloudformation/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/cloudfront/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/cloudfront/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/cloudfront-keyvaluestore/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/cloudfront-keyvaluestore/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/cloudhsm/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/cloudhsm/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/cloudhsmv2/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/cloudhsmv2/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/cloudsearch/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/cloudsearch/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/cloudsearchdomain/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/cloudsearchdomain/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/cloudtrail/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/cloudtrail/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/cloudtrail-data/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/cloudtrail-data/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/cloudwatch/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/cloudwatch/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/codeartifact/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/codeartifact/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/codebuild/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/codebuild/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/codecatalyst/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/codecatalyst/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/codecommit/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/codecommit/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/codeconnections/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/codeconnections/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/codedeploy/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/codedeploy/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/codeguru-reviewer/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/codeguru-reviewer/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/codeguru-security/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/codeguru-security/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/codeguruprofiler/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/codeguruprofiler/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/codepipeline/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/codepipeline/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/codestar/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/codestar/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/codestar-connections/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/codestar-connections/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/codestar-notifications/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/codestar-notifications/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/cognito-identity/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/cognito-identity/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/cognito-idp/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/cognito-idp/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/cognito-sync/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/cognito-sync/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/comprehend/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/comprehend/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/comprehendmedical/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/comprehendmedical/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/compute-optimizer/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/compute-optimizer/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/config/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/config/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/connect/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/connect/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/connect-contact-lens/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/connect-contact-lens/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/connectcampaigns/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/connectcampaigns/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/connectcases/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/connectcases/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/connectparticipant/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/connectparticipant/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/controlcatalog/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/controlcatalog/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/controltower/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/controltower/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/cost-optimization-hub/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/cost-optimization-hub/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/cur/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/cur/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/customer-profiles/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/customer-profiles/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/databrew/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/databrew/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/dataexchange/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/dataexchange/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/datapipeline/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/datapipeline/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/datasync/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/datasync/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/datazone/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/datazone/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/dax/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/dax/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/deadline/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/deadline/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/detective/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/detective/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/devicefarm/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/devicefarm/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/devops-guru/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/devops-guru/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/directconnect/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/directconnect/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/discovery/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/discovery/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/dlm/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/dlm/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/dms/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/dms/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/docdb/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/docdb/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/docdb-elastic/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/docdb-elastic/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/drs/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/drs/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/ds/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/ds/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/dynamodb/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/dynamodb/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/dynamodbstreams/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/dynamodbstreams/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/ebs/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/ebs/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/ec2/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/ec2/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/ec2-instance-connect/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/ec2-instance-connect/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/ecr/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/ecr/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/ecr-public/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/ecr-public/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/ecs/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/ecs/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/efs/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/efs/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/eks/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/eks/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/eks-auth/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/eks-auth/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/elastic-inference/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/elastic-inference/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/elasticache/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/elasticache/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/elasticbeanstalk/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/elasticbeanstalk/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/elastictranscoder/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/elastictranscoder/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/elb/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/elb/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/elbv2/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/elbv2/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/emr/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/emr/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/emr-containers/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/emr-containers/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/emr-serverless/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/emr-serverless/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/entityresolution/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/entityresolution/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/es/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/es/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/events/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/events/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/evidently/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/evidently/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/finspace/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/finspace/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/finspace-data/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/finspace-data/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/firehose/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/firehose/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/fis/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/fis/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/fms/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/fms/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/forecast/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/forecast/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/forecastquery/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/forecastquery/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/frauddetector/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/frauddetector/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/freetier/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/freetier/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/fsx/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/fsx/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/gamelift/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/gamelift/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/glacier/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/glacier/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/globalaccelerator/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/globalaccelerator/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/glue/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/glue/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/grafana/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/grafana/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/greengrass/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/greengrass/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/greengrassv2/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/greengrassv2/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/groundstation/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/groundstation/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/guardduty/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/guardduty/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/health/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/health/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/healthlake/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/healthlake/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/honeycode/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/honeycode/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/iam/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/iam/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/identitystore/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/identitystore/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/imagebuilder/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/imagebuilder/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/importexport/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/importexport/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/inspector/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/inspector/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/inspector-scan/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/inspector-scan/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/inspector2/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/inspector2/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/internetmonitor/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/internetmonitor/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/iot/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/iot/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/iot-data/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/iot-data/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/iot-jobs-data/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/iot-jobs-data/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/iot1click-devices/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/iot1click-devices/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/iot1click-projects/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/iot1click-projects/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/iotanalytics/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/iotanalytics/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/iotdeviceadvisor/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/iotdeviceadvisor/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/iotevents/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/iotevents/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/iotevents-data/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/iotevents-data/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/iotfleethub/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/iotfleethub/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/iotfleetwise/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/iotfleetwise/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/iotsecuretunneling/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/iotsecuretunneling/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/iotsitewise/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/iotsitewise/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/iotthingsgraph/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/iotthingsgraph/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/iottwinmaker/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/iottwinmaker/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/iotwireless/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/iotwireless/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/ivs/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/ivs/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/ivs-realtime/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/ivs-realtime/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/ivschat/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/ivschat/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/kafka/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/kafka/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/kafkaconnect/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/kafkaconnect/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/kendra/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/kendra/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/kendra-ranking/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/kendra-ranking/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/keyspaces/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/keyspaces/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/kinesis/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/kinesis/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/kinesis-video-archived-media/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/kinesis-video-archived-media/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/kinesis-video-media/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/kinesis-video-media/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/kinesis-video-signaling/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/kinesis-video-signaling/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/kinesis-video-webrtc-storage/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/kinesis-video-webrtc-storage/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/kinesisanalytics/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/kinesisanalytics/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/kinesisanalyticsv2/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/kinesisanalyticsv2/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/kinesisvideo/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/kinesisvideo/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/kms/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/kms/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/lakeformation/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/lakeformation/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/lambda/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/lambda/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/launch-wizard/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/launch-wizard/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/lex-models/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/lex-models/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/lex-runtime/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/lex-runtime/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/lexv2-models/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/lexv2-models/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/lexv2-runtime/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/lexv2-runtime/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/license-manager/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/license-manager/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/license-manager-linux-subscriptions/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/license-manager-linux-subscriptions/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/license-manager-user-subscriptions/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/license-manager-user-subscriptions/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/lightsail/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/lightsail/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/location/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/location/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/logs/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/logs/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/lookoutequipment/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/lookoutequipment/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/lookoutmetrics/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/lookoutmetrics/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/lookoutvision/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/lookoutvision/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/m2/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/m2/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/machinelearning/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/machinelearning/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/macie2/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/macie2/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/managedblockchain/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/managedblockchain/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/managedblockchain-query/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/managedblockchain-query/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/marketplace-agreement/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/marketplace-agreement/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/marketplace-catalog/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/marketplace-catalog/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/marketplace-deployment/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/marketplace-deployment/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/marketplace-entitlement/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/marketplace-entitlement/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/marketplacecommerceanalytics/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/marketplacecommerceanalytics/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/mediaconnect/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/mediaconnect/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/mediaconvert/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/mediaconvert/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/medialive/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/medialive/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/mediapackage/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/mediapackage/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/mediapackage-vod/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/mediapackage-vod/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/mediapackagev2/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/mediapackagev2/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/mediastore/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/mediastore/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/mediastore-data/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/mediastore-data/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/mediatailor/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/mediatailor/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/medical-imaging/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/medical-imaging/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/memorydb/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/memorydb/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/meteringmarketplace/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/meteringmarketplace/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/mgh/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/mgh/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/mgn/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/mgn/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/migration-hub-refactor-spaces/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/migration-hub-refactor-spaces/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/migrationhub-config/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/migrationhub-config/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/migrationhuborchestrator/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/migrationhuborchestrator/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/migrationhubstrategy/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/migrationhubstrategy/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/mobile/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/mobile/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/mq/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/mq/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/mturk/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/mturk/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/mwaa/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/mwaa/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/neptune/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/neptune/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/neptune-graph/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/neptune-graph/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/neptunedata/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/neptunedata/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/network-firewall/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/network-firewall/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/networkmanager/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/networkmanager/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/networkmonitor/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/networkmonitor/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/nimble/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/nimble/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/oam/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/oam/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/omics/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/omics/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/opensearch/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/opensearch/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/opensearchserverless/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/opensearchserverless/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/opsworks/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/opsworks/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/opsworkscm/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/opsworkscm/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/organizations/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/organizations/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/osis/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/osis/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/outposts/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/outposts/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/panorama/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/panorama/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/payment-cryptography/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/payment-cryptography/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/payment-cryptography-data/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/payment-cryptography-data/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/pca-connector-ad/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/pca-connector-ad/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/personalize/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/personalize/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/personalize-events/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/personalize-events/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/personalize-runtime/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/personalize-runtime/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/pi/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/pi/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/pinpoint/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/pinpoint/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/pinpoint-email/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/pinpoint-email/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/pinpoint-sms-voice/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/pinpoint-sms-voice/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/pinpoint-sms-voice-v2/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/pinpoint-sms-voice-v2/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/pipes/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/pipes/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/polly/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/polly/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/pricing/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/pricing/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/privatenetworks/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/privatenetworks/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/proton/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/proton/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/qbusiness/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/qbusiness/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/qconnect/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/qconnect/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/qldb/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/qldb/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/qldb-session/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/qldb-session/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/quicksight/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/quicksight/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/ram/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/ram/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/rbin/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/rbin/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/rds/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/rds/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/rds-data/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/rds-data/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/redshift/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/redshift/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/redshift-data/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/redshift-data/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/redshift-serverless/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/redshift-serverless/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/rekognition/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/rekognition/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/repostspace/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/repostspace/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/resiliencehub/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/resiliencehub/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/resource-explorer-2/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/resource-explorer-2/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/resource-groups/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/resource-groups/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/resourcegroupstaggingapi/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/resourcegroupstaggingapi/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/robomaker/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/robomaker/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/rolesanywhere/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/rolesanywhere/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/route53/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/route53/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/route53-recovery-cluster/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/route53-recovery-cluster/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/route53-recovery-control-config/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/route53-recovery-control-config/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/route53-recovery-readiness/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/route53-recovery-readiness/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/route53domains/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/route53domains/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/route53profiles/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/route53profiles/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/route53resolver/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/route53resolver/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/rum/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/rum/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/s3/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/s3/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/s3control/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/s3control/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/s3outposts/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/s3outposts/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/sagemaker/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/sagemaker/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/sagemaker-a2i-runtime/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/sagemaker-a2i-runtime/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/sagemaker-edge/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/sagemaker-edge/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/sagemaker-featurestore-runtime/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/sagemaker-featurestore-runtime/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/sagemaker-geospatial/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/sagemaker-geospatial/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/sagemaker-metrics/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/sagemaker-metrics/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/sagemaker-runtime/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/sagemaker-runtime/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/savingsplans/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/savingsplans/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/scheduler/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/scheduler/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/schemas/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/schemas/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/sdb/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/sdb/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/secretsmanager/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/secretsmanager/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/securityhub/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/securityhub/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/securitylake/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/securitylake/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/serverlessrepo/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/serverlessrepo/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/service-quotas/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/service-quotas/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/servicecatalog/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/servicecatalog/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/servicecatalog-appregistry/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/servicecatalog-appregistry/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/servicediscovery/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/servicediscovery/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/ses/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/ses/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/sesv2/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/sesv2/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/shield/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/shield/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/signer/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/signer/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/simspaceweaver/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/simspaceweaver/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/sms/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/sms/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/sms-voice/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/sms-voice/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/snow-device-management/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/snow-device-management/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/snowball/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/snowball/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/sns/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/sns/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/sqs/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/sqs/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/ssm/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/ssm/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/ssm-contacts/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/ssm-contacts/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/ssm-incidents/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/ssm-incidents/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/ssm-sap/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/ssm-sap/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/sso/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/sso/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/sso-admin/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/sso-admin/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/sso-oidc/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/sso-oidc/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/stepfunctions/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/stepfunctions/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/storagegateway/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/storagegateway/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/sts/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/sts/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/supplychain/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/supplychain/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/support/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/support/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/support-app/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/support-app/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/swf/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/swf/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/synthetics/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/synthetics/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/textract/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/textract/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/timestream-influxdb/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/timestream-influxdb/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/timestream-query/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/timestream-query/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/timestream-write/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/timestream-write/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/tnb/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/tnb/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/transcribe/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/transcribe/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/transfer/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/transfer/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/translate/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/translate/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/trustedadvisor/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/trustedadvisor/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/verifiedpermissions/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/verifiedpermissions/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/voice-id/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/voice-id/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/vpc-lattice/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/vpc-lattice/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/waf/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/waf/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/waf-regional/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/waf-regional/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/wafv2/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/wafv2/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/wellarchitected/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/wellarchitected/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/wisdom/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/wisdom/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/workdocs/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/workdocs/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/worklink/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/worklink/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/workmail/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/workmail/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/workmailmessageflow/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/workmailmessageflow/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/workspaces/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/workspaces/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/workspaces-thin-client/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/workspaces-thin-client/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/workspaces-web/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/workspaces-web/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/endpoint-rules/xray/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/endpoint-rules/xray/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/leak/__init__.py` & `botocore-a-la-carte-1.34.99/tests/functional/leak/__init__.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/leak/test_resource_leaks.py` & `botocore-a-la-carte-1.34.99/tests/functional/leak/test_resource_leaks.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/models/custom-acm/2015-12-08/endpoint-rule-set-1.json` & `botocore-a-la-carte-1.34.99/tests/functional/models/custom-acm/2015-12-08/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/models/custom-acm/2015-12-08/service-2.json` & `botocore-a-la-carte-1.34.99/tests/functional/models/custom-acm/2015-12-08/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/models/custom-acm/2015-12-08/waiters-2.json` & `botocore-a-la-carte-1.34.99/tests/functional/models/custom-acm/2015-12-08/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/models/endpoints.json` & `botocore-a-la-carte-1.34.99/tests/functional/models/endpoints.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/models/sdk-default-configuration.json` & `botocore-a-la-carte-1.34.99/tests/functional/models/sdk-default-configuration.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/models/test-discovery-endpoint/2020-08-20/service-2.json` & `botocore-a-la-carte-1.34.99/tests/functional/models/test-discovery-endpoint/2020-08-20/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/retries/test_bucket.py` & `botocore-a-la-carte-1.34.99/tests/functional/retries/test_bucket.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/retries/test_quota.py` & `botocore-a-la-carte-1.34.99/tests/functional/retries/test_quota.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/test_alias.py` & `botocore-a-la-carte-1.34.99/tests/functional/test_alias.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/test_apigateway.py` & `botocore-a-la-carte-1.34.99/tests/functional/test_apigateway.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/test_client.py` & `botocore-a-la-carte-1.34.99/tests/functional/test_client.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/test_client_class_names.py` & `botocore-a-la-carte-1.34.99/tests/functional/test_client_class_names.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/test_client_metadata.py` & `botocore-a-la-carte-1.34.99/tests/functional/test_client_metadata.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/test_cloudformation.py` & `botocore-a-la-carte-1.34.99/tests/functional/test_cloudformation.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/test_cloudsearchdomain.py` & `botocore-a-la-carte-1.34.99/tests/functional/test_cloudsearchdomain.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/test_cognito_idp.py` & `botocore-a-la-carte-1.34.99/tests/functional/test_cognito_idp.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/test_compress.py` & `botocore-a-la-carte-1.34.99/tests/functional/test_compress.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/test_config_provider.py` & `botocore-a-la-carte-1.34.99/tests/functional/test_config_provider.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/test_context_params.py` & `botocore-a-la-carte-1.34.99/tests/functional/test_context_params.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/test_credentials.py` & `botocore-a-la-carte-1.34.99/tests/functional/test_credentials.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/test_discovery.py` & `botocore-a-la-carte-1.34.99/tests/functional/test_discovery.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/test_docdb.py` & `botocore-a-la-carte-1.34.99/tests/functional/test_docdb.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/test_dynamodb.py` & `botocore-a-la-carte-1.34.99/tests/functional/test_dynamodb.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/test_ec2.py` & `botocore-a-la-carte-1.34.99/tests/functional/test_ec2.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/test_endpoint_rulesets.py` & `botocore-a-la-carte-1.34.99/tests/functional/test_endpoint_rulesets.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/test_endpoints.py` & `botocore-a-la-carte-1.34.99/tests/functional/test_endpoints.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/test_event_alias.py` & `botocore-a-la-carte-1.34.99/tests/functional/test_event_alias.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/test_eventbridge.py` & `botocore-a-la-carte-1.34.99/tests/functional/test_eventbridge.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/test_events.py` & `botocore-a-la-carte-1.34.99/tests/functional/test_events.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/test_h2_required.py` & `botocore-a-la-carte-1.34.99/tests/functional/test_h2_required.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/test_history.py` & `botocore-a-la-carte-1.34.99/tests/functional/test_history.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/test_importexport.py` & `botocore-a-la-carte-1.34.99/tests/functional/test_importexport.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/test_iot_data.py` & `botocore-a-la-carte-1.34.99/tests/functional/test_iot_data.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/test_kinesis.py` & `botocore-a-la-carte-1.34.99/tests/functional/test_kinesis.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/test_lex.py` & `botocore-a-la-carte-1.34.99/tests/functional/test_lex.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/test_loaders.py` & `botocore-a-la-carte-1.34.99/tests/functional/test_loaders.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/test_machinelearning.py` & `botocore-a-la-carte-1.34.99/tests/functional/test_machinelearning.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/test_model_backcompat.py` & `botocore-a-la-carte-1.34.99/tests/functional/test_model_backcompat.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/test_model_completeness.py` & `botocore-a-la-carte-1.34.99/tests/functional/test_model_completeness.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/test_modeled_exceptions.py` & `botocore-a-la-carte-1.34.99/tests/functional/test_modeled_exceptions.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/test_mturk.py` & `botocore-a-la-carte-1.34.99/tests/functional/test_mturk.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/test_neptune.py` & `botocore-a-la-carte-1.34.99/tests/functional/test_neptune.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/test_paginate.py` & `botocore-a-la-carte-1.34.99/tests/functional/test_paginate.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/test_paginator_config.py` & `botocore-a-la-carte-1.34.99/tests/functional/test_paginator_config.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/test_public_apis.py` & `botocore-a-la-carte-1.34.99/tests/functional/test_public_apis.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/test_qbusiness.py` & `botocore-a-la-carte-1.34.99/tests/functional/test_qbusiness.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/test_rds.py` & `botocore-a-la-carte-1.34.99/tests/functional/test_rds.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/test_regions.py` & `botocore-a-la-carte-1.34.99/tests/functional/test_regions.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/test_response_shadowing.py` & `botocore-a-la-carte-1.34.99/tests/functional/test_response_shadowing.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/test_retry.py` & `botocore-a-la-carte-1.34.99/tests/functional/test_retry.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/test_route53.py` & `botocore-a-la-carte-1.34.99/tests/functional/test_route53.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/test_s3.py` & `botocore-a-la-carte-1.34.99/tests/functional/test_s3.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/test_s3_control.py` & `botocore-a-la-carte-1.34.99/tests/functional/test_s3_control.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/test_s3_control_redirects.py` & `botocore-a-la-carte-1.34.99/tests/functional/test_s3_control_redirects.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/test_s3express.py` & `botocore-a-la-carte-1.34.99/tests/functional/test_s3express.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/test_sagemaker.py` & `botocore-a-la-carte-1.34.99/tests/functional/test_sagemaker.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/test_service_alias.py` & `botocore-a-la-carte-1.34.99/tests/functional/test_service_alias.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/test_service_names.py` & `botocore-a-la-carte-1.34.99/tests/functional/test_service_names.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/test_session.py` & `botocore-a-la-carte-1.34.99/tests/functional/test_session.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/test_six_imports.py` & `botocore-a-la-carte-1.34.99/tests/functional/test_six_imports.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/test_six_threading.py` & `botocore-a-la-carte-1.34.99/tests/functional/test_six_threading.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/test_sqs.py` & `botocore-a-la-carte-1.34.99/tests/functional/test_sqs.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/test_sts.py` & `botocore-a-la-carte-1.34.99/tests/functional/test_sts.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/test_stub.py` & `botocore-a-la-carte-1.34.99/tests/functional/test_stub.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/test_tagged_unions_unknown.py` & `botocore-a-la-carte-1.34.99/tests/functional/test_tagged_unions_unknown.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/test_useragent.py` & `botocore-a-la-carte-1.34.99/tests/functional/test_useragent.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/test_utils.py` & `botocore-a-la-carte-1.34.99/tests/functional/test_utils.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/test_waiter_config.py` & `botocore-a-la-carte-1.34.99/tests/functional/test_waiter_config.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/utils/__init__.py` & `botocore-a-la-carte-1.34.99/tests/functional/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/functional/utils/credentialprocess.py` & `botocore-a-la-carte-1.34.99/tests/functional/utils/credentialprocess.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/integration/__init__.py` & `botocore-a-la-carte-1.34.99/tests/integration/__init__.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/integration/test_apigateway.py` & `botocore-a-la-carte-1.34.99/tests/integration/test_apigateway.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/integration/test_client.py` & `botocore-a-la-carte-1.34.99/tests/integration/test_client.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/integration/test_client_http.py` & `botocore-a-la-carte-1.34.99/tests/integration/test_client_http.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/integration/test_cloudformation.py` & `botocore-a-la-carte-1.34.99/tests/integration/test_cloudformation.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/integration/test_cognito_identity.py` & `botocore-a-la-carte-1.34.99/tests/integration/test_cognito_identity.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/integration/test_credentials.py` & `botocore-a-la-carte-1.34.99/tests/integration/test_credentials.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/integration/test_ec2.py` & `botocore-a-la-carte-1.34.99/tests/integration/test_ec2.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/integration/test_elastictranscoder.py` & `botocore-a-la-carte-1.34.99/tests/integration/test_elastictranscoder.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/integration/test_emr.py` & `botocore-a-la-carte-1.34.99/tests/integration/test_emr.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/integration/test_glacier.py` & `botocore-a-la-carte-1.34.99/tests/integration/test_glacier.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/integration/test_loaders.py` & `botocore-a-la-carte-1.34.99/tests/integration/test_loaders.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/integration/test_rds.py` & `botocore-a-la-carte-1.34.99/tests/integration/test_rds.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/integration/test_route53.py` & `botocore-a-la-carte-1.34.99/tests/integration/test_route53.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/integration/test_s3.py` & `botocore-a-la-carte-1.34.99/tests/integration/test_s3.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/integration/test_session.py` & `botocore-a-la-carte-1.34.99/tests/integration/test_session.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/integration/test_smoke.py` & `botocore-a-la-carte-1.34.99/tests/integration/test_smoke.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/integration/test_sts.py` & `botocore-a-la-carte-1.34.99/tests/integration/test_sts.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/integration/test_utils.py` & `botocore-a-la-carte-1.34.99/tests/integration/test_utils.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/integration/test_waiters.py` & `botocore-a-la-carte-1.34.99/tests/integration/test_waiters.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/__init__.py` & `botocore-a-la-carte-1.34.99/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/auth/__init__.py` & `botocore-a-la-carte-1.34.99/tests/unit/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/LICENSE` & `botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/LICENSE`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/normalize-path/normalize-path.txt` & `botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/normalize-path/normalize-path.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/post-sts-token/post-sts-header-after/post-sts-header-after.sreq` & `botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/post-sts-token/post-sts-header-after/post-sts-header-after.sreq`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/post-sts-token/post-sts-header-before/post-sts-header-before.creq` & `botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/post-sts-token/post-sts-header-before/post-sts-header-before.creq`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/post-sts-token/post-sts-header-before/post-sts-header-before.sreq` & `botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/post-sts-token/post-sts-header-before/post-sts-header-before.sreq`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/auth/aws4_testsuite/post-sts-token/readme.txt` & `botocore-a-la-carte-1.34.99/tests/unit/auth/aws4_testsuite/post-sts-token/readme.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/auth/test_signers.py` & `botocore-a-la-carte-1.34.99/tests/unit/auth/test_signers.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/auth/test_sigv4.py` & `botocore-a-la-carte-1.34.99/tests/unit/auth/test_sigv4.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/cfg/aws_config_badbytes` & `botocore-a-la-carte-1.34.99/tests/unit/cfg/aws_config_badbytes`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/crt/auth/test_crt_signers.py` & `botocore-a-la-carte-1.34.99/tests/unit/crt/auth/test_crt_signers.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/crt/auth/test_crt_sigv4.py` & `botocore-a-la-carte-1.34.99/tests/unit/crt/auth/test_crt_sigv4.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/data/endpoints/test-cases/aws-region.json` & `botocore-a-la-carte-1.34.99/tests/unit/data/endpoints/test-cases/aws-region.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/data/endpoints/test-cases/default-values.json` & `botocore-a-la-carte-1.34.99/tests/unit/data/endpoints/test-cases/default-values.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/data/endpoints/test-cases/eventbridge.json` & `botocore-a-la-carte-1.34.99/tests/unit/data/endpoints/test-cases/eventbridge.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/data/endpoints/test-cases/fns.json` & `botocore-a-la-carte-1.34.99/tests/unit/data/endpoints/test-cases/fns.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/data/endpoints/test-cases/is-virtual-hostable-s3-bucket.json` & `botocore-a-la-carte-1.34.99/tests/unit/data/endpoints/test-cases/is-virtual-hostable-s3-bucket.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/data/endpoints/test-cases/parse-arn.json` & `botocore-a-la-carte-1.34.99/tests/unit/data/endpoints/test-cases/parse-arn.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/data/endpoints/test-cases/parse-url.json` & `botocore-a-la-carte-1.34.99/tests/unit/data/endpoints/test-cases/parse-url.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/data/endpoints/test-cases/partition-fn.json` & `botocore-a-la-carte-1.34.99/tests/unit/data/endpoints/test-cases/partition-fn.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/data/endpoints/test-cases/substring.json` & `botocore-a-la-carte-1.34.99/tests/unit/data/endpoints/test-cases/substring.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/data/endpoints/test-cases/uri-encode.json` & `botocore-a-la-carte-1.34.99/tests/unit/data/endpoints/test-cases/uri-encode.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/data/endpoints/test-cases/valid-hostlabel.json` & `botocore-a-la-carte-1.34.99/tests/unit/data/endpoints/test-cases/valid-hostlabel.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/data/endpoints/valid-rules/aws-region.json` & `botocore-a-la-carte-1.34.99/tests/unit/data/endpoints/valid-rules/aws-region.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/data/endpoints/valid-rules/default-values.json` & `botocore-a-la-carte-1.34.99/tests/unit/data/endpoints/valid-rules/default-values.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/data/endpoints/valid-rules/deprecated-param.json` & `botocore-a-la-carte-1.34.99/tests/unit/data/endpoints/valid-rules/deprecated-param.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/data/endpoints/valid-rules/eventbridge.json` & `botocore-a-la-carte-1.34.99/tests/unit/data/endpoints/valid-rules/eventbridge.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/data/endpoints/valid-rules/fns.json` & `botocore-a-la-carte-1.34.99/tests/unit/data/endpoints/valid-rules/fns.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/data/endpoints/valid-rules/get-attr-type-inference.json` & `botocore-a-la-carte-1.34.99/tests/unit/data/endpoints/valid-rules/get-attr-type-inference.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/data/endpoints/valid-rules/headers.json` & `botocore-a-la-carte-1.34.99/tests/unit/data/endpoints/valid-rules/headers.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/data/endpoints/valid-rules/is-virtual-hostable-s3-bucket.json` & `botocore-a-la-carte-1.34.99/tests/unit/data/endpoints/valid-rules/is-virtual-hostable-s3-bucket.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/data/endpoints/valid-rules/local-region-override.json` & `botocore-a-la-carte-1.34.99/tests/unit/data/endpoints/valid-rules/local-region-override.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/data/endpoints/valid-rules/minimal-ruleset.json` & `botocore-a-la-carte-1.34.99/tests/unit/data/endpoints/valid-rules/minimal-ruleset.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/data/endpoints/valid-rules/parse-arn.json` & `botocore-a-la-carte-1.34.99/tests/unit/data/endpoints/valid-rules/parse-arn.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/data/endpoints/valid-rules/parse-url.json` & `botocore-a-la-carte-1.34.99/tests/unit/data/endpoints/valid-rules/parse-url.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/data/endpoints/valid-rules/partition-fn.json` & `botocore-a-la-carte-1.34.99/tests/unit/data/endpoints/valid-rules/partition-fn.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/data/endpoints/valid-rules/substring.json` & `botocore-a-la-carte-1.34.99/tests/unit/data/endpoints/valid-rules/substring.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/data/endpoints/valid-rules/uri-encode.json` & `botocore-a-la-carte-1.34.99/tests/unit/data/endpoints/valid-rules/uri-encode.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/data/endpoints/valid-rules/valid-hostlabel.json` & `botocore-a-la-carte-1.34.99/tests/unit/data/endpoints/valid-rules/valid-hostlabel.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/docs/__init__.py` & `botocore-a-la-carte-1.34.99/tests/unit/docs/__init__.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/docs/bcdoc/__init__.py` & `botocore-a-la-carte-1.34.99/tests/unit/docs/bcdoc/__init__.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/docs/bcdoc/test_docstringparser.py` & `botocore-a-la-carte-1.34.99/tests/unit/docs/bcdoc/test_docstringparser.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/docs/bcdoc/test_document.py` & `botocore-a-la-carte-1.34.99/tests/unit/docs/bcdoc/test_document.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/docs/bcdoc/test_style.py` & `botocore-a-la-carte-1.34.99/tests/unit/docs/bcdoc/test_style.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/docs/test_client.py` & `botocore-a-la-carte-1.34.99/tests/unit/docs/test_client.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/docs/test_docs.py` & `botocore-a-la-carte-1.34.99/tests/unit/docs/test_docs.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/docs/test_docstring.py` & `botocore-a-la-carte-1.34.99/tests/unit/docs/test_docstring.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/docs/test_example.py` & `botocore-a-la-carte-1.34.99/tests/unit/docs/test_example.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/docs/test_method.py` & `botocore-a-la-carte-1.34.99/tests/unit/docs/test_method.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/docs/test_paginator.py` & `botocore-a-la-carte-1.34.99/tests/unit/docs/test_paginator.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/docs/test_params.py` & `botocore-a-la-carte-1.34.99/tests/unit/docs/test_params.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/docs/test_service.py` & `botocore-a-la-carte-1.34.99/tests/unit/docs/test_service.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/docs/test_sharedexample.py` & `botocore-a-la-carte-1.34.99/tests/unit/docs/test_sharedexample.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/docs/test_utils.py` & `botocore-a-la-carte-1.34.99/tests/unit/docs/test_utils.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/docs/test_waiter.py` & `botocore-a-la-carte-1.34.99/tests/unit/docs/test_waiter.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/protocols/input/ec2.json` & `botocore-a-la-carte-1.34.99/tests/unit/protocols/input/ec2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/protocols/input/json.json` & `botocore-a-la-carte-1.34.99/tests/unit/protocols/input/json.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/protocols/input/query.json` & `botocore-a-la-carte-1.34.99/tests/unit/protocols/input/query.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/protocols/input/rest-json.json` & `botocore-a-la-carte-1.34.99/tests/unit/protocols/input/rest-json.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/protocols/input/rest-xml.json` & `botocore-a-la-carte-1.34.99/tests/unit/protocols/input/rest-xml.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/protocols/output/ec2.json` & `botocore-a-la-carte-1.34.99/tests/unit/protocols/output/ec2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/protocols/output/json.json` & `botocore-a-la-carte-1.34.99/tests/unit/protocols/output/json.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/protocols/output/query.json` & `botocore-a-la-carte-1.34.99/tests/unit/protocols/output/query.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/protocols/output/rest-json.json` & `botocore-a-la-carte-1.34.99/tests/unit/protocols/output/rest-json.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/protocols/output/rest-xml.json` & `botocore-a-la-carte-1.34.99/tests/unit/protocols/output/rest-xml.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/README.rst` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/README.rst`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/__init__.py` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/json/expected/elastictranscoder-list-pipelines.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/json/expected/elastictranscoder-list-pipelines.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/test_response_parsing.py` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/test_response_parsing.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/autoscaling-describe-adjustment-types.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/autoscaling-describe-adjustment-types.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/autoscaling-describe-auto-scaling-notification-types.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/autoscaling-describe-auto-scaling-notification-types.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/autoscaling-describe-metric-collection-types.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/autoscaling-describe-metric-collection-types.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/autoscaling-describe-scaling-process-types.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/autoscaling-describe-scaling-process-types.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/autoscaling-describe-termination-policy-types.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/autoscaling-describe-termination-policy-types.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/cloudformation-get-template.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/cloudformation-get-template.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/cloudformation-get-template.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/cloudformation-get-template.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/cloudfront-get-distribution.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/cloudfront-get-distribution.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/cloudfront-get-distribution.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/cloudfront-get-distribution.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/cloudfront-get-invalidation.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/cloudfront-get-invalidation.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/cloudfront-get-streaming-distribution.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/cloudfront-get-streaming-distribution.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/cloudfront-get-streaming-distribution.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/cloudfront-get-streaming-distribution.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/cloudfront-list-cloud-front-origin-access-identities.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/cloudfront-list-cloud-front-origin-access-identities.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/cloudfront-list-cloud-front-origin-access-identities.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/cloudfront-list-cloud-front-origin-access-identities.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/cloudfront-list-distributions.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/cloudfront-list-distributions.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/cloudfront-list-distributions.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/cloudfront-list-distributions.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/cloudfront-list-invalidations.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/cloudfront-list-invalidations.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/cloudfront-list-streaming-distributions.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/cloudfront-list-streaming-distributions.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/cloudfront-list-streaming-distributions.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/cloudfront-list-streaming-distributions.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/cloudwatch-list-metrics.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/cloudwatch-list-metrics.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/cloudwatch-list-metrics.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/cloudwatch-list-metrics.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-bundle-instance.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-bundle-instance.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-cancel-bundle-task.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-cancel-bundle-task.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-cancel-reserved-instances-listing.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-cancel-reserved-instances-listing.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-cancel-reserved-instances-listing.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-cancel-reserved-instances-listing.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-create-dhcp-options.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-create-dhcp-options.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-create-dhcp-options.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-create-dhcp-options.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-create-instance-export-task.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-create-instance-export-task.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-create-instance-export-task.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-create-instance-export-task.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-create-key-pair.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-create-key-pair.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-create-key-pair.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-create-key-pair.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-create-network-acl.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-create-network-acl.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-create-network-acl.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-create-network-acl.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-create-network-interface.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-create-network-interface.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-create-network-interface.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-create-network-interface.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-create-reserved-instances-listing.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-create-reserved-instances-listing.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-create-reserved-instances-listing.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-create-reserved-instances-listing.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-create-route-table.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-create-route-table.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-account-attributes.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-account-attributes.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-account-attributes.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-account-attributes.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-addresses.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-addresses.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-availability-zones.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-availability-zones.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-availability-zones.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-availability-zones.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-bundle-tasks.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-bundle-tasks.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-dhcp-options.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-dhcp-options.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-dhcp-options.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-dhcp-options.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-export-tasks.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-export-tasks.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-export-tasks.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-export-tasks.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-instance-status.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-instance-status.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-instance-status.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-instance-status.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-instances.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-instances.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-instances.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-instances.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-internet-gateways.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-internet-gateways.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-network-acls.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-network-acls.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-network-acls.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-network-acls.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-network-interfaces.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-network-interfaces.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-network-interfaces.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-network-interfaces.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-regions.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-regions.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-regions.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-regions.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-reserved-instances-offerings.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-reserved-instances-offerings.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-reserved-instances-offerings.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-reserved-instances-offerings.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-reserved-instances.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-reserved-instances.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-reserved-instances.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-reserved-instances.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-route-tables.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-route-tables.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-route-tables.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-route-tables.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-security-groups.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-security-groups.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-security-groups.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-security-groups.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-snapshots.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-snapshots.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-snapshots.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-snapshots.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-spot-instance-requests.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-spot-instance-requests.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-spot-instance-requests.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-spot-instance-requests.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-spot-price-history.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-spot-price-history.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-spot-price-history.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-spot-price-history.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-subnets.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-subnets.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-volume-status.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-volume-status.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-volume-status.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-volume-status.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-volumes.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-volumes.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-volumes.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-volumes.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-vpcs.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-vpcs.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-vpn-connections.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-vpn-connections.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-describe-vpn-gateways.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-describe-vpn-gateways.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-import-instance.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-import-instance.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-import-instance.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-import-instance.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-import-volume.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-import-volume.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-import-volume.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-import-volume.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-request-spot-instances.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-request-spot-instances.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-request-spot-instances.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-request-spot-instances.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-run-instances.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-run-instances.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-run-instances.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-run-instances.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ec2-unmonitor-instances.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ec2-unmonitor-instances.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/elasticbeanstalk-create-application-version.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/elasticbeanstalk-create-application-version.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/elasticbeanstalk-create-application.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/elasticbeanstalk-create-application.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/elasticbeanstalk-create-configuration-template.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/elasticbeanstalk-create-configuration-template.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/elasticbeanstalk-create-configuration-template.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/elasticbeanstalk-create-configuration-template.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/elasticbeanstalk-create-environment.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/elasticbeanstalk-create-environment.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/elasticbeanstalk-describe-application-versions.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/elasticbeanstalk-describe-application-versions.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/elasticbeanstalk-describe-application-versions.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/elasticbeanstalk-describe-application-versions.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/elasticbeanstalk-describe-applications.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/elasticbeanstalk-describe-applications.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/elasticbeanstalk-describe-configuration-options.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/elasticbeanstalk-describe-configuration-options.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/elasticbeanstalk-describe-configuration-options.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/elasticbeanstalk-describe-configuration-options.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/elasticbeanstalk-describe-environments.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/elasticbeanstalk-describe-environments.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/elasticbeanstalk-describe-environments.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/elasticbeanstalk-describe-environments.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/elasticbeanstalk-describe-events.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/elasticbeanstalk-describe-events.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/elasticbeanstalk-describe-events.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/elasticbeanstalk-describe-events.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/elasticbeanstalk-list-available-solution-stacks.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/elasticbeanstalk-list-available-solution-stacks.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/elasticbeanstalk-list-available-solution-stacks.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/elasticbeanstalk-list-available-solution-stacks.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/elasticbeanstalk-retrieve-environment-info.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/elasticbeanstalk-retrieve-environment-info.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/elasticbeanstalk-terminate-environment.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/elasticbeanstalk-terminate-environment.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/elasticbeanstalk-terminate-environment.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/elasticbeanstalk-terminate-environment.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/elasticbeanstalk-update-application-version.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/elasticbeanstalk-update-application-version.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/elasticbeanstalk-update-application.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/elasticbeanstalk-update-application.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/elb-describe-load-balancer-policies.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/elb-describe-load-balancer-policies.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/elb-describe-load-balancer-policies.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/elb-describe-load-balancer-policies.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/elb-describe-load-balancer-policy-types.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/elb-describe-load-balancer-policy-types.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/elb-describe-load-balancer-policy-types.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/elb-describe-load-balancer-policy-types.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/iam-create-virtual-mfa-device.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/iam-create-virtual-mfa-device.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/iam-get-account-summary.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/iam-get-account-summary.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/iam-get-account-summary.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/iam-get-account-summary.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/iam-get-group.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/iam-get-group.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/iam-get-group.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/iam-get-group.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/iam-get-user-policy.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/iam-get-user-policy.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/iam-get-user-policy.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/iam-get-user-policy.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/iam-list-access-keys.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/iam-list-access-keys.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/iam-list-groups.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/iam-list-groups.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/iam-list-groups.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/iam-list-groups.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/iam-list-instance-profiles.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/iam-list-instance-profiles.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/iam-list-instance-profiles.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/iam-list-instance-profiles.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/iam-list-roles.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/iam-list-roles.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/iam-list-roles.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/iam-list-roles.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/iam-list-server-certificates.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/iam-list-server-certificates.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/iam-list-server-certificates.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/iam-list-server-certificates.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/iam-list-signing-certificates.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/iam-list-signing-certificates.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/iam-list-signing-certificates.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/iam-list-signing-certificates.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/iam-list-users.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/iam-list-users.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/iam-list-users.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/iam-list-users.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/iam-list-virtual-mfa-devices.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/iam-list-virtual-mfa-devices.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/iam-list-virtual-mfa-devices.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/iam-list-virtual-mfa-devices.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/importexport-list-jobs.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/importexport-list-jobs.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/rds-describe-db-engine-versions.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/rds-describe-db-engine-versions.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/rds-describe-db-engine-versions.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/rds-describe-db-engine-versions.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/rds-describe-db-instances.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/rds-describe-db-instances.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/rds-describe-db-instances.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/rds-describe-db-instances.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/rds-describe-db-parameter-groups.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/rds-describe-db-parameter-groups.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/rds-describe-db-security-groups.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/rds-describe-db-security-groups.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/rds-describe-db-security-groups.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/rds-describe-db-security-groups.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/rds-describe-db-snapshots.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/rds-describe-db-snapshots.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/rds-describe-db-snapshots.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/rds-describe-db-snapshots.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/rds-describe-db-subnet-groups.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/rds-describe-db-subnet-groups.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/rds-describe-db-subnet-groups.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/rds-describe-db-subnet-groups.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/rds-describe-event-categories.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/rds-describe-event-categories.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/rds-describe-event-categories.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/rds-describe-event-categories.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/rds-describe-events.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/rds-describe-events.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/rds-describe-events.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/rds-describe-events.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/rds-describe-option-groups.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/rds-describe-option-groups.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/rds-describe-reserved-db-instances-offerings.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/rds-describe-reserved-db-instances-offerings.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/rds-describe-reserved-db-instances-offerings.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/rds-describe-reserved-db-instances-offerings.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/rds-describe-reserved-db-instances.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/rds-describe-reserved-db-instances.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/rds-describe-reserved-db-instances.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/rds-describe-reserved-db-instances.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-authorize-cluster-security-group-ingress.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-authorize-cluster-security-group-ingress.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-copy-cluster-snapshot.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-copy-cluster-snapshot.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-copy-cluster-snapshot.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-copy-cluster-snapshot.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-create-cluster-parameter-group.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-create-cluster-parameter-group.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-create-cluster-security-group.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-create-cluster-security-group.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-create-cluster-snapshot.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-create-cluster-snapshot.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-create-cluster-snapshot.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-create-cluster-snapshot.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-create-cluster-subnet-group.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-create-cluster-subnet-group.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-create-cluster-subnet-group.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-create-cluster-subnet-group.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-create-cluster.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-create-cluster.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-create-cluster.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-create-cluster.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-delete-cluster-snapshot.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-delete-cluster-snapshot.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-delete-cluster-snapshot.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-delete-cluster-snapshot.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-delete-cluster.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-delete-cluster.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-delete-cluster.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-delete-cluster.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-parameter-groups.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-parameter-groups.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-parameters.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-parameters.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-parameters.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-parameters.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-security-groups.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-security-groups.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-security-groups.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-security-groups.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-snapshots.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-snapshots.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-snapshots.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-snapshots.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-subnet-groups.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-subnet-groups.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-subnet-groups.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-subnet-groups.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-versions.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-versions.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-describe-clusters.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-describe-clusters.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-describe-clusters.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-describe-clusters.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-describe-events.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-describe-events.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-describe-orderable-cluster-options.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-describe-orderable-cluster-options.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-describe-orderable-cluster-options.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-describe-orderable-cluster-options.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-describe-reserved-node-offerings.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-describe-reserved-node-offerings.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-describe-reserved-node-offerings.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-describe-reserved-node-offerings.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-describe-reserved-nodes.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-describe-reserved-nodes.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-describe-reserved-nodes.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-describe-reserved-nodes.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-modify-cluster-parameter-group.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-modify-cluster-parameter-group.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-purchase-reserved-node-offering.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-purchase-reserved-node-offering.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-purchase-reserved-node-offering.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-purchase-reserved-node-offering.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-reboot-cluster.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-reboot-cluster.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-reboot-cluster.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-reboot-cluster.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-reset-cluster-parameter-group.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-reset-cluster-parameter-group.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-restore-from-cluster-snapshot.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-restore-from-cluster-snapshot.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-restore-from-cluster-snapshot.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-restore-from-cluster-snapshot.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/redshift-revoke-cluster-security-group-ingress.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/redshift-revoke-cluster-security-group-ingress.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/s3-get-bucket-acl.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/s3-get-bucket-acl.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/s3-get-bucket-logging.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/s3-get-bucket-logging.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/s3-list-buckets.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/s3-list-buckets.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/s3-list-buckets.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/s3-list-buckets.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/s3-list-multipart-uploads#2.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/s3-list-multipart-uploads#2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/s3-list-multipart-uploads#2.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/s3-list-multipart-uploads#2.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/s3-list-multipart-uploads.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/s3-list-multipart-uploads.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/s3-list-object-versions.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/s3-list-object-versions.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/s3-list-object-versions.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/s3-list-object-versions.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/s3-list-objects.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/s3-list-objects.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/s3-list-objects.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/s3-list-objects.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ses-get-identity-dkim-attributes.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ses-get-identity-dkim-attributes.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ses-get-identity-notification-attributes.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ses-get-identity-notification-attributes.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ses-get-identity-verification-attributes.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ses-get-identity-verification-attributes.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/ses-get-send-statistics.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/ses-get-send-statistics.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/sns-get-subscription-attributes.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/sns-get-subscription-attributes.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/sns-get-topic-attributes.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/sns-get-topic-attributes.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/sns-get-topic-attributes.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/sns-get-topic-attributes.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/sns-list-subscriptions-by-topic.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/sns-list-subscriptions-by-topic.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/sns-list-subscriptions.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/sns-list-subscriptions.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/sqs-get-queue-attributes.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/sqs-get-queue-attributes.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/sqs-receive-message.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/sqs-receive-message.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/sts-get-session-token.json` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/sts-get-session-token.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/response_parsing/xml/responses/sts-get-session-token.xml` & `botocore-a-la-carte-1.34.99/tests/unit/response_parsing/xml/responses/sts-get-session-token.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/retries/test_adaptive.py` & `botocore-a-la-carte-1.34.99/tests/unit/retries/test_adaptive.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/retries/test_bucket.py` & `botocore-a-la-carte-1.34.99/tests/unit/retries/test_bucket.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/retries/test_quota.py` & `botocore-a-la-carte-1.34.99/tests/unit/retries/test_quota.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/retries/test_special.py` & `botocore-a-la-carte-1.34.99/tests/unit/retries/test_special.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/retries/test_standard.py` & `botocore-a-la-carte-1.34.99/tests/unit/retries/test_standard.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/retries/test_throttling.py` & `botocore-a-la-carte-1.34.99/tests/unit/retries/test_throttling.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/test_args.py` & `botocore-a-la-carte-1.34.99/tests/unit/test_args.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/test_auth_bearer.py` & `botocore-a-la-carte-1.34.99/tests/unit/test_auth_bearer.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/test_auth_sigv4.py` & `botocore-a-la-carte-1.34.99/tests/unit/test_auth_sigv4.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/test_awsrequest.py` & `botocore-a-la-carte-1.34.99/tests/unit/test_awsrequest.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/test_client.py` & `botocore-a-la-carte-1.34.99/tests/unit/test_client.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/test_compat.py` & `botocore-a-la-carte-1.34.99/tests/unit/test_compat.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/test_compress.py` & `botocore-a-la-carte-1.34.99/tests/unit/test_compress.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/test_config_provider.py` & `botocore-a-la-carte-1.34.99/tests/unit/test_config_provider.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/test_configloader.py` & `botocore-a-la-carte-1.34.99/tests/unit/test_configloader.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/test_credentials.py` & `botocore-a-la-carte-1.34.99/tests/unit/test_credentials.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/test_discovery.py` & `botocore-a-la-carte-1.34.99/tests/unit/test_discovery.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/test_endpoint.py` & `botocore-a-la-carte-1.34.99/tests/unit/test_endpoint.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/test_endpoint_provider.py` & `botocore-a-la-carte-1.34.99/tests/unit/test_endpoint_provider.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/test_errorfactory.py` & `botocore-a-la-carte-1.34.99/tests/unit/test_errorfactory.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/test_eventstream.py` & `botocore-a-la-carte-1.34.99/tests/unit/test_eventstream.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/test_exceptions.py` & `botocore-a-la-carte-1.34.99/tests/unit/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/test_handlers.py` & `botocore-a-la-carte-1.34.99/tests/unit/test_handlers.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/test_history.py` & `botocore-a-la-carte-1.34.99/tests/unit/test_history.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/test_hooks.py` & `botocore-a-la-carte-1.34.99/tests/unit/test_hooks.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/test_http_client_exception_mapping.py` & `botocore-a-la-carte-1.34.99/tests/unit/test_http_client_exception_mapping.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/test_http_session.py` & `botocore-a-la-carte-1.34.99/tests/unit/test_http_session.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/test_httpchecksum.py` & `botocore-a-la-carte-1.34.99/tests/unit/test_httpchecksum.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/test_idempotency.py` & `botocore-a-la-carte-1.34.99/tests/unit/test_idempotency.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/test_loaders.py` & `botocore-a-la-carte-1.34.99/tests/unit/test_loaders.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/test_model.py` & `botocore-a-la-carte-1.34.99/tests/unit/test_model.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/test_monitoring.py` & `botocore-a-la-carte-1.34.99/tests/unit/test_monitoring.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/test_paginate.py` & `botocore-a-la-carte-1.34.99/tests/unit/test_paginate.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/test_parsers.py` & `botocore-a-la-carte-1.34.99/tests/unit/test_parsers.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/test_protocols.py` & `botocore-a-la-carte-1.34.99/tests/unit/test_protocols.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/test_regions.py` & `botocore-a-la-carte-1.34.99/tests/unit/test_regions.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/test_response.py` & `botocore-a-la-carte-1.34.99/tests/unit/test_response.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/test_retryhandler.py` & `botocore-a-la-carte-1.34.99/tests/unit/test_retryhandler.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/test_s3_addressing.py` & `botocore-a-la-carte-1.34.99/tests/unit/test_s3_addressing.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/test_serialize.py` & `botocore-a-la-carte-1.34.99/tests/unit/test_serialize.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/test_session.py` & `botocore-a-la-carte-1.34.99/tests/unit/test_session.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/test_session_legacy.py` & `botocore-a-la-carte-1.34.99/tests/unit/test_session_legacy.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/test_signers.py` & `botocore-a-la-carte-1.34.99/tests/unit/test_signers.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/test_stub.py` & `botocore-a-la-carte-1.34.99/tests/unit/test_stub.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/test_tokens.py` & `botocore-a-la-carte-1.34.99/tests/unit/test_tokens.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/test_translate.py` & `botocore-a-la-carte-1.34.99/tests/unit/test_translate.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/test_useragent.py` & `botocore-a-la-carte-1.34.99/tests/unit/test_useragent.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/test_utils.py` & `botocore-a-la-carte-1.34.99/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/test_validate.py` & `botocore-a-la-carte-1.34.99/tests/unit/test_validate.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.98/tests/unit/test_waiters.py` & `botocore-a-la-carte-1.34.99/tests/unit/test_waiters.py`

 * *Files identical despite different names*

