# Comparing `tmp/py-ms-2.8.0.tar.gz` & `tmp/py_ms-2.9.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/py-ms-2.8.0.tar", last modified: Tue Jan 26 19:29:28 2021, max compression
+gzip compressed data, was "py_ms-2.9.0rc1.tar", max compression
```

## Comparing `py-ms-2.8.0.tar` & `py_ms-2.9.0rc1.tar`

### file list

```diff
@@ -1,141 +1,39 @@
-drwxrwxr-x   0 prometeo  (1000) prometeo  (1000)        0 2021-01-26 19:29:28.000000 py-ms-2.8.0/
--rw-r--r--   0 prometeo  (1000) prometeo  (1000)      207 2020-11-09 15:14:09.000000 py-ms-2.8.0/MANIFEST.in
--rw-rw-r--   0 prometeo  (1000) prometeo  (1000)     3833 2021-01-26 19:29:28.000000 py-ms-2.8.0/PKG-INFO
--rw-r--r--   0 prometeo  (1000) prometeo  (1000)     2580 2020-11-09 13:41:23.000000 py-ms-2.8.0/README.md
-drwxrwxr-x   0 prometeo  (1000) prometeo  (1000)        0 2021-01-26 19:29:28.000000 py-ms-2.8.0/py_ms.egg-info/
--rw-rw-r--   0 prometeo  (1000) prometeo  (1000)     3833 2021-01-26 19:29:28.000000 py-ms-2.8.0/py_ms.egg-info/PKG-INFO
--rw-rw-r--   0 prometeo  (1000) prometeo  (1000)     4492 2021-01-26 19:29:28.000000 py-ms-2.8.0/py_ms.egg-info/SOURCES.txt
--rw-rw-r--   0 prometeo  (1000) prometeo  (1000)        1 2021-01-26 19:29:28.000000 py-ms-2.8.0/py_ms.egg-info/dependency_links.txt
--rw-rw-r--   0 prometeo  (1000) prometeo  (1000)       48 2021-01-26 19:29:28.000000 py-ms-2.8.0/py_ms.egg-info/entry_points.txt
--rw-rw-r--   0 prometeo  (1000) prometeo  (1000)     1032 2021-01-26 19:29:28.000000 py-ms-2.8.0/py_ms.egg-info/requires.txt
--rw-rw-r--   0 prometeo  (1000) prometeo  (1000)        5 2021-01-26 19:29:28.000000 py-ms-2.8.0/py_ms.egg-info/top_level.txt
--rw-rw-r--   0 prometeo  (1000) prometeo  (1000)        1 2020-09-23 14:06:18.000000 py-ms-2.8.0/py_ms.egg-info/zip-safe
-drwxrwxr-x   0 prometeo  (1000) prometeo  (1000)        0 2021-01-26 19:29:28.000000 py-ms-2.8.0/pyms/
--rw-r--r--   0 prometeo  (1000) prometeo  (1000)       88 2021-01-26 19:28:21.000000 py-ms-2.8.0/pyms/__init__.py
-drwxrwxr-x   0 prometeo  (1000) prometeo  (1000)        0 2021-01-26 19:29:28.000000 py-ms-2.8.0/pyms/__pycache__/
--rw-r--r--   0 prometeo  (1000) prometeo  (1000)      242 2020-11-02 12:38:17.000000 py-ms-2.8.0/pyms/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0 prometeo  (1000) prometeo  (1000)      246 2021-01-26 19:29:28.000000 py-ms-2.8.0/pyms/__pycache__/__init__.cpython-37.pyc
--rw-rw-r--   0 prometeo  (1000) prometeo  (1000)      513 2020-10-15 16:21:47.000000 py-ms-2.8.0/pyms/__pycache__/constants.cpython-36.pyc
--rw-rw-r--   0 prometeo  (1000) prometeo  (1000)      635 2020-10-17 18:52:39.000000 py-ms-2.8.0/pyms/__pycache__/constants.cpython-37.pyc
--rw-r--r--   0 prometeo  (1000) prometeo  (1000)     1114 2020-09-28 16:20:50.000000 py-ms-2.8.0/pyms/__pycache__/exceptions.cpython-36.pyc
--rw-r--r--   0 prometeo  (1000) prometeo  (1000)     1277 2020-11-02 20:18:31.000000 py-ms-2.8.0/pyms/__pycache__/exceptions.cpython-37.pyc
-drwxrwxr-x   0 prometeo  (1000) prometeo  (1000)        0 2021-01-26 19:29:28.000000 py-ms-2.8.0/pyms/cloud/
-drwxrwxr-x   0 prometeo  (1000) prometeo  (1000)        0 2021-01-26 19:29:28.000000 py-ms-2.8.0/pyms/cloud/aws/
-drwxrwxr-x   0 prometeo  (1000) prometeo  (1000)        0 2021-01-26 19:29:28.000000 py-ms-2.8.0/pyms/cloud/aws/__pycache__/
--rw-rw-r--   0 prometeo  (1000) prometeo  (1000)     1928 2020-10-15 16:21:48.000000 py-ms-2.8.0/pyms/cloud/aws/__pycache__/kms.cpython-36.pyc
--rw-rw-r--   0 prometeo  (1000) prometeo  (1000)     1928 2020-11-09 15:06:34.000000 py-ms-2.8.0/pyms/cloud/aws/__pycache__/kms.cpython-37.pyc
--rw-rw-r--   0 prometeo  (1000) prometeo  (1000)     1517 2020-11-09 13:09:38.000000 py-ms-2.8.0/pyms/cloud/aws/kms.py
-drwxrwxr-x   0 prometeo  (1000) prometeo  (1000)        0 2021-01-26 19:29:28.000000 py-ms-2.8.0/pyms/cmd/
--rwxr-xr-x   0 prometeo  (1000) prometeo  (1000)       49 2020-11-09 13:09:38.000000 py-ms-2.8.0/pyms/cmd/__init__.py
-drwxrwxr-x   0 prometeo  (1000) prometeo  (1000)        0 2021-01-26 19:29:28.000000 py-ms-2.8.0/pyms/cmd/__pycache__/
--rw-r--r--   0 prometeo  (1000) prometeo  (1000)      211 2020-10-15 16:21:46.000000 py-ms-2.8.0/pyms/cmd/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0 prometeo  (1000) prometeo  (1000)      215 2020-11-09 15:06:33.000000 py-ms-2.8.0/pyms/cmd/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 prometeo  (1000) prometeo  (1000)     4432 2020-10-15 16:21:46.000000 py-ms-2.8.0/pyms/cmd/__pycache__/main.cpython-36.pyc
--rw-r--r--   0 prometeo  (1000) prometeo  (1000)     5390 2020-11-28 11:24:53.000000 py-ms-2.8.0/pyms/cmd/__pycache__/main.cpython-37.pyc
--rwxr-xr-x   0 prometeo  (1000) prometeo  (1000)     6964 2020-11-09 18:01:12.000000 py-ms-2.8.0/pyms/cmd/main.py
-drwxrwxr-x   0 prometeo  (1000) prometeo  (1000)        0 2021-01-26 19:29:28.000000 py-ms-2.8.0/pyms/config/
--rw-r--r--   0 prometeo  (1000) prometeo  (1000)      131 2020-11-09 18:01:12.000000 py-ms-2.8.0/pyms/config/__init__.py
-drwxrwxr-x   0 prometeo  (1000) prometeo  (1000)        0 2021-01-26 19:29:28.000000 py-ms-2.8.0/pyms/config/__pycache__/
--rw-r--r--   0 prometeo  (1000) prometeo  (1000)      262 2020-10-15 16:21:47.000000 py-ms-2.8.0/pyms/config/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0 prometeo  (1000) prometeo  (1000)      300 2020-11-10 18:46:37.000000 py-ms-2.8.0/pyms/config/__pycache__/__init__.cpython-37.pyc
--rw-rw-r--   0 prometeo  (1000) prometeo  (1000)     3394 2020-10-15 16:21:47.000000 py-ms-2.8.0/pyms/config/__pycache__/conf.cpython-36.pyc
--rw-rw-r--   0 prometeo  (1000) prometeo  (1000)     5370 2020-11-10 18:46:37.000000 py-ms-2.8.0/pyms/config/__pycache__/conf.cpython-37.pyc
--rw-rw-r--   0 prometeo  (1000) prometeo  (1000)     5086 2020-10-15 16:21:47.000000 py-ms-2.8.0/pyms/config/__pycache__/confile.cpython-36.pyc
--rw-rw-r--   0 prometeo  (1000) prometeo  (1000)     5453 2020-11-10 18:46:37.000000 py-ms-2.8.0/pyms/config/__pycache__/confile.cpython-37.pyc
--rw-rw-r--   0 prometeo  (1000) prometeo  (1000)      643 2020-10-15 16:21:47.000000 py-ms-2.8.0/pyms/config/__pycache__/resource.cpython-36.pyc
--rw-rw-r--   0 prometeo  (1000) prometeo  (1000)      669 2020-11-02 18:41:14.000000 py-ms-2.8.0/pyms/config/__pycache__/resource.cpython-37.pyc
--rw-rw-r--   0 prometeo  (1000) prometeo  (1000)     6591 2020-11-09 18:05:48.000000 py-ms-2.8.0/pyms/config/conf.py
--rw-rw-r--   0 prometeo  (1000) prometeo  (1000)     5565 2020-11-09 18:05:48.000000 py-ms-2.8.0/pyms/config/confile.py
--rw-rw-r--   0 prometeo  (1000) prometeo  (1000)      268 2020-11-01 16:55:53.000000 py-ms-2.8.0/pyms/config/resource.py
--rw-rw-r--   0 prometeo  (1000) prometeo  (1000)      450 2020-10-15 16:29:19.000000 py-ms-2.8.0/pyms/constants.py
-drwxrwxr-x   0 prometeo  (1000) prometeo  (1000)        0 2021-01-26 19:29:28.000000 py-ms-2.8.0/pyms/crypt/
--rw-rw-r--   0 prometeo  (1000) prometeo  (1000)        0 2020-03-24 19:08:18.000000 py-ms-2.8.0/pyms/crypt/__init__.py
-drwxrwxr-x   0 prometeo  (1000) prometeo  (1000)        0 2021-01-26 19:29:28.000000 py-ms-2.8.0/pyms/crypt/__pycache__/
--rw-rw-r--   0 prometeo  (1000) prometeo  (1000)      155 2020-09-28 16:20:50.000000 py-ms-2.8.0/pyms/crypt/__pycache__/__init__.cpython-36.pyc
--rw-rw-r--   0 prometeo  (1000) prometeo  (1000)      159 2020-09-23 17:23:31.000000 py-ms-2.8.0/pyms/crypt/__pycache__/__init__.cpython-37.pyc
--rw-rw-r--   0 prometeo  (1000) prometeo  (1000)     2377 2020-10-15 16:21:47.000000 py-ms-2.8.0/pyms/crypt/__pycache__/driver.cpython-36.pyc
--rw-rw-r--   0 prometeo  (1000) prometeo  (1000)     2381 2020-11-09 15:06:33.000000 py-ms-2.8.0/pyms/crypt/__pycache__/driver.cpython-37.pyc
--rw-rw-r--   0 prometeo  (1000) prometeo  (1000)     2505 2020-10-15 16:21:46.000000 py-ms-2.8.0/pyms/crypt/__pycache__/fernet.cpython-36.pyc
--rw-rw-r--   0 prometeo  (1000) prometeo  (1000)     2886 2020-11-28 11:24:54.000000 py-ms-2.8.0/pyms/crypt/__pycache__/fernet.cpython-37.pyc
--rw-rw-r--   0 prometeo  (1000) prometeo  (1000)     1587 2020-11-09 13:09:38.000000 py-ms-2.8.0/pyms/crypt/driver.py
--rw-rw-r--   0 prometeo  (1000) prometeo  (1000)     2754 2020-11-09 18:05:48.000000 py-ms-2.8.0/pyms/crypt/fernet.py
--rw-r--r--   0 prometeo  (1000) prometeo  (1000)      427 2020-11-02 20:18:25.000000 py-ms-2.8.0/pyms/exceptions.py
-drwxrwxr-x   0 prometeo  (1000) prometeo  (1000)        0 2021-01-26 19:29:28.000000 py-ms-2.8.0/pyms/flask/
--rw-r--r--   0 prometeo  (1000) prometeo  (1000)        0 2020-01-12 19:51:43.000000 py-ms-2.8.0/pyms/flask/__init__.py
-drwxrwxr-x   0 prometeo  (1000) prometeo  (1000)        0 2021-01-26 19:29:28.000000 py-ms-2.8.0/pyms/flask/__pycache__/
--rw-r--r--   0 prometeo  (1000) prometeo  (1000)      155 2020-09-28 16:20:50.000000 py-ms-2.8.0/pyms/flask/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0 prometeo  (1000) prometeo  (1000)      159 2020-09-23 17:23:30.000000 py-ms-2.8.0/pyms/flask/__pycache__/__init__.cpython-37.pyc
-drwxrwxr-x   0 prometeo  (1000) prometeo  (1000)        0 2021-01-26 19:29:28.000000 py-ms-2.8.0/pyms/flask/app/
--rw-r--r--   0 prometeo  (1000) prometeo  (1000)      109 2020-11-09 18:01:12.000000 py-ms-2.8.0/pyms/flask/app/__init__.py
-drwxrwxr-x   0 prometeo  (1000) prometeo  (1000)        0 2021-01-26 19:29:28.000000 py-ms-2.8.0/pyms/flask/app/__pycache__/
--rw-r--r--   0 prometeo  (1000) prometeo  (1000)      279 2020-10-15 16:21:48.000000 py-ms-2.8.0/pyms/flask/app/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0 prometeo  (1000) prometeo  (1000)      283 2020-11-10 18:46:37.000000 py-ms-2.8.0/pyms/flask/app/__pycache__/__init__.cpython-37.pyc
--rw-rw-r--   0 prometeo  (1000) prometeo  (1000)     8928 2020-10-15 16:21:48.000000 py-ms-2.8.0/pyms/flask/app/__pycache__/create_app.cpython-36.pyc
--rw-rw-r--   0 prometeo  (1000) prometeo  (1000)     6738 2020-11-12 21:02:53.000000 py-ms-2.8.0/pyms/flask/app/__pycache__/create_app.cpython-37.pyc
--rw-r--r--   0 prometeo  (1000) prometeo  (1000)      526 2020-09-28 16:20:51.000000 py-ms-2.8.0/pyms/flask/app/__pycache__/create_config.cpython-36.pyc
--rw-r--r--   0 prometeo  (1000) prometeo  (1000)      530 2020-09-23 17:23:31.000000 py-ms-2.8.0/pyms/flask/app/__pycache__/create_config.cpython-37.pyc
--rw-rw-r--   0 prometeo  (1000) prometeo  (1000)     2886 2020-10-15 16:21:48.000000 py-ms-2.8.0/pyms/flask/app/__pycache__/utils.cpython-36.pyc
--rw-rw-r--   0 prometeo  (1000) prometeo  (1000)     2961 2020-11-09 17:29:33.000000 py-ms-2.8.0/pyms/flask/app/__pycache__/utils.cpython-37.pyc
--rw-rw-r--   0 prometeo  (1000) prometeo  (1000)     6763 2020-11-12 08:39:39.000000 py-ms-2.8.0/pyms/flask/app/create_app.py
--rw-r--r--   0 prometeo  (1000) prometeo  (1000)      307 2020-02-16 22:12:15.000000 py-ms-2.8.0/pyms/flask/app/create_config.py
--rw-rw-r--   0 prometeo  (1000) prometeo  (1000)     2678 2020-11-09 17:26:13.000000 py-ms-2.8.0/pyms/flask/app/utils.py
-drwxrwxr-x   0 prometeo  (1000) prometeo  (1000)        0 2021-01-26 19:29:28.000000 py-ms-2.8.0/pyms/flask/configreload/
--rw-r--r--   0 prometeo  (1000) prometeo  (1000)       87 2020-11-09 18:01:12.000000 py-ms-2.8.0/pyms/flask/configreload/__init__.py
-drwxrwxr-x   0 prometeo  (1000) prometeo  (1000)        0 2021-01-26 19:29:28.000000 py-ms-2.8.0/pyms/flask/configreload/__pycache__/
--rw-r--r--   0 prometeo  (1000) prometeo  (1000)      249 2020-10-15 16:21:48.000000 py-ms-2.8.0/pyms/flask/configreload/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0 prometeo  (1000) prometeo  (1000)      253 2020-11-10 18:46:37.000000 py-ms-2.8.0/pyms/flask/configreload/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 prometeo  (1000) prometeo  (1000)      707 2020-10-15 16:21:48.000000 py-ms-2.8.0/pyms/flask/configreload/__pycache__/configreload.cpython-36.pyc
--rw-r--r--   0 prometeo  (1000) prometeo  (1000)      699 2020-11-10 18:46:37.000000 py-ms-2.8.0/pyms/flask/configreload/__pycache__/configreload.cpython-37.pyc
--rw-r--r--   0 prometeo  (1000) prometeo  (1000)      416 2020-11-09 18:05:48.000000 py-ms-2.8.0/pyms/flask/configreload/configreload.py
-drwxrwxr-x   0 prometeo  (1000) prometeo  (1000)        0 2021-01-26 19:29:28.000000 py-ms-2.8.0/pyms/flask/healthcheck/
--rw-r--r--   0 prometeo  (1000) prometeo  (1000)       84 2020-11-09 18:01:12.000000 py-ms-2.8.0/pyms/flask/healthcheck/__init__.py
-drwxrwxr-x   0 prometeo  (1000) prometeo  (1000)        0 2021-01-26 19:29:28.000000 py-ms-2.8.0/pyms/flask/healthcheck/__pycache__/
--rw-r--r--   0 prometeo  (1000) prometeo  (1000)      246 2020-10-15 16:21:48.000000 py-ms-2.8.0/pyms/flask/healthcheck/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0 prometeo  (1000) prometeo  (1000)      250 2020-11-10 18:46:37.000000 py-ms-2.8.0/pyms/flask/healthcheck/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 prometeo  (1000) prometeo  (1000)      686 2020-10-15 16:21:48.000000 py-ms-2.8.0/pyms/flask/healthcheck/__pycache__/healthcheck.cpython-36.pyc
--rw-r--r--   0 prometeo  (1000) prometeo  (1000)      690 2020-11-10 18:46:37.000000 py-ms-2.8.0/pyms/flask/healthcheck/__pycache__/healthcheck.cpython-37.pyc
--rw-r--r--   0 prometeo  (1000) prometeo  (1000)      428 2020-11-09 18:05:48.000000 py-ms-2.8.0/pyms/flask/healthcheck/healthcheck.py
-drwxrwxr-x   0 prometeo  (1000) prometeo  (1000)        0 2021-01-26 19:29:28.000000 py-ms-2.8.0/pyms/flask/services/
--rw-r--r--   0 prometeo  (1000) prometeo  (1000)        0 2020-01-12 19:51:43.000000 py-ms-2.8.0/pyms/flask/services/__init__.py
-drwxrwxr-x   0 prometeo  (1000) prometeo  (1000)        0 2021-01-26 19:29:28.000000 py-ms-2.8.0/pyms/flask/services/__pycache__/
--rw-r--r--   0 prometeo  (1000) prometeo  (1000)      164 2020-09-28 16:20:50.000000 py-ms-2.8.0/pyms/flask/services/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0 prometeo  (1000) prometeo  (1000)      168 2020-09-23 17:23:31.000000 py-ms-2.8.0/pyms/flask/services/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 prometeo  (1000) prometeo  (1000)     3460 2020-10-15 16:21:48.000000 py-ms-2.8.0/pyms/flask/services/__pycache__/driver.cpython-36.pyc
--rw-r--r--   0 prometeo  (1000) prometeo  (1000)     3098 2020-11-10 18:46:37.000000 py-ms-2.8.0/pyms/flask/services/__pycache__/driver.cpython-37.pyc
--rw-r--r--   0 prometeo  (1000) prometeo  (1000)     3592 2020-10-15 16:21:49.000000 py-ms-2.8.0/pyms/flask/services/__pycache__/metrics.cpython-36.pyc
--rw-r--r--   0 prometeo  (1000) prometeo  (1000)     4332 2020-11-28 11:24:55.000000 py-ms-2.8.0/pyms/flask/services/__pycache__/metrics.cpython-37.pyc
--rw-r--r--   0 prometeo  (1000) prometeo  (1000)    14244 2020-10-15 16:21:48.000000 py-ms-2.8.0/pyms/flask/services/__pycache__/requests.cpython-36.pyc
--rw-r--r--   0 prometeo  (1000) prometeo  (1000)    14605 2020-11-09 15:06:34.000000 py-ms-2.8.0/pyms/flask/services/__pycache__/requests.cpython-37.pyc
--rw-rw-r--   0 prometeo  (1000) prometeo  (1000)     2783 2020-11-28 11:24:55.000000 py-ms-2.8.0/pyms/flask/services/__pycache__/service_discovery.cpython-37.pyc
--rw-r--r--   0 prometeo  (1000) prometeo  (1000)     4071 2020-10-15 16:21:47.000000 py-ms-2.8.0/pyms/flask/services/__pycache__/swagger.cpython-36.pyc
--rw-r--r--   0 prometeo  (1000) prometeo  (1000)     4436 2020-11-28 11:24:54.000000 py-ms-2.8.0/pyms/flask/services/__pycache__/swagger.cpython-37.pyc
--rw-r--r--   0 prometeo  (1000) prometeo  (1000)     3294 2020-10-15 16:21:48.000000 py-ms-2.8.0/pyms/flask/services/__pycache__/tracer.cpython-36.pyc
--rw-r--r--   0 prometeo  (1000) prometeo  (1000)     3650 2020-11-10 18:46:38.000000 py-ms-2.8.0/pyms/flask/services/__pycache__/tracer.cpython-37.pyc
--rw-r--r--   0 prometeo  (1000) prometeo  (1000)     2376 2020-11-09 18:01:12.000000 py-ms-2.8.0/pyms/flask/services/driver.py
--rw-r--r--   0 prometeo  (1000) prometeo  (1000)     3652 2020-11-09 18:05:48.000000 py-ms-2.8.0/pyms/flask/services/metrics.py
--rw-r--r--   0 prometeo  (1000) prometeo  (1000)    15717 2020-11-09 13:09:38.000000 py-ms-2.8.0/pyms/flask/services/requests.py
--rw-rw-r--   0 prometeo  (1000) prometeo  (1000)     2126 2020-11-28 11:18:03.000000 py-ms-2.8.0/pyms/flask/services/service_discovery.py
--rw-r--r--   0 prometeo  (1000) prometeo  (1000)     4590 2020-11-28 11:24:09.000000 py-ms-2.8.0/pyms/flask/services/swagger.py
--rw-r--r--   0 prometeo  (1000) prometeo  (1000)     4165 2020-11-09 18:01:12.000000 py-ms-2.8.0/pyms/flask/services/tracer.py
-drwxrwxr-x   0 prometeo  (1000) prometeo  (1000)        0 2021-01-26 19:29:28.000000 py-ms-2.8.0/pyms/logger/
--rw-r--r--   0 prometeo  (1000) prometeo  (1000)       99 2020-11-09 13:09:38.000000 py-ms-2.8.0/pyms/logger/__init__.py
-drwxrwxr-x   0 prometeo  (1000) prometeo  (1000)        0 2021-01-26 19:29:28.000000 py-ms-2.8.0/pyms/logger/__pycache__/
--rw-r--r--   0 prometeo  (1000) prometeo  (1000)      255 2020-10-15 16:21:48.000000 py-ms-2.8.0/pyms/logger/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0 prometeo  (1000) prometeo  (1000)      259 2020-11-09 15:06:34.000000 py-ms-2.8.0/pyms/logger/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 prometeo  (1000) prometeo  (1000)     1568 2020-10-15 16:21:48.000000 py-ms-2.8.0/pyms/logger/__pycache__/logger.cpython-36.pyc
--rw-r--r--   0 prometeo  (1000) prometeo  (1000)     1572 2020-11-09 15:06:34.000000 py-ms-2.8.0/pyms/logger/__pycache__/logger.cpython-37.pyc
--rw-r--r--   0 prometeo  (1000) prometeo  (1000)     1422 2020-11-09 13:09:38.000000 py-ms-2.8.0/pyms/logger/logger.py
-drwxrwxr-x   0 prometeo  (1000) prometeo  (1000)        0 2021-01-26 19:29:28.000000 py-ms-2.8.0/pyms/utils/
--rw-r--r--   0 prometeo  (1000) prometeo  (1000)      138 2020-11-09 18:01:12.000000 py-ms-2.8.0/pyms/utils/__init__.py
-drwxrwxr-x   0 prometeo  (1000) prometeo  (1000)        0 2021-01-26 19:29:28.000000 py-ms-2.8.0/pyms/utils/__pycache__/
--rw-r--r--   0 prometeo  (1000) prometeo  (1000)      288 2020-10-15 16:21:47.000000 py-ms-2.8.0/pyms/utils/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0 prometeo  (1000) prometeo  (1000)      292 2020-11-10 18:46:37.000000 py-ms-2.8.0/pyms/utils/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 prometeo  (1000) prometeo  (1000)     2139 2020-10-15 16:21:47.000000 py-ms-2.8.0/pyms/utils/__pycache__/files.cpython-36.pyc
--rw-r--r--   0 prometeo  (1000) prometeo  (1000)     2159 2020-11-09 15:06:33.000000 py-ms-2.8.0/pyms/utils/__pycache__/files.cpython-37.pyc
--rw-r--r--   0 prometeo  (1000) prometeo  (1000)      963 2020-10-15 16:21:47.000000 py-ms-2.8.0/pyms/utils/__pycache__/utils.cpython-36.pyc
--rw-r--r--   0 prometeo  (1000) prometeo  (1000)     1811 2020-11-28 11:24:54.000000 py-ms-2.8.0/pyms/utils/__pycache__/utils.cpython-37.pyc
--rw-r--r--   0 prometeo  (1000) prometeo  (1000)     1991 2020-11-09 13:09:39.000000 py-ms-2.8.0/pyms/utils/files.py
--rw-r--r--   0 prometeo  (1000) prometeo  (1000)     1341 2020-11-28 11:16:03.000000 py-ms-2.8.0/pyms/utils/utils.py
--rw-rw-r--   0 prometeo  (1000) prometeo  (1000)      174 2020-10-19 07:45:56.000000 py-ms-2.8.0/pyproject.toml
--rw-r--r--   0 prometeo  (1000) prometeo  (1000)      327 2021-01-26 19:29:28.000000 py-ms-2.8.0/setup.cfg
--rw-r--r--   0 prometeo  (1000) prometeo  (1000)     3442 2021-01-26 19:03:35.000000 py-ms-2.8.0/setup.py
+-rw-r--r--   0        0        0      244 2024-05-25 10:18:44.709663 py_ms-2.9.0rc1/AUTHORS
+-rw-r--r--   0        0        0    35149 2024-05-25 10:18:44.709663 py_ms-2.9.0rc1/LICENSE
+-rw-r--r--   0        0        0     2644 2024-05-25 10:43:19.432778 py_ms-2.9.0rc1/README.md
+-rw-r--r--   0        0        0       91 2024-05-25 15:24:41.953107 py_ms-2.9.0rc1/pyms/__init__.py
+-rw-r--r--   0        0        0     1517 2024-05-25 10:18:44.709663 py_ms-2.9.0rc1/pyms/cloud/aws/kms.py
+-rwxr-xr-x   0        0        0       49 2024-05-25 10:18:44.709663 py_ms-2.9.0rc1/pyms/cmd/__init__.py
+-rwxr-xr-x   0        0        0     7209 2024-05-25 15:14:07.045761 py_ms-2.9.0rc1/pyms/cmd/main.py
+-rw-r--r--   0        0        0      131 2024-05-25 10:18:44.713663 py_ms-2.9.0rc1/pyms/config/__init__.py
+-rw-r--r--   0        0        0     6591 2024-05-25 10:18:44.713663 py_ms-2.9.0rc1/pyms/config/conf.py
+-rw-r--r--   0        0        0     5566 2024-05-25 13:42:34.182618 py_ms-2.9.0rc1/pyms/config/confile.py
+-rw-r--r--   0        0        0      268 2024-05-25 10:18:44.713663 py_ms-2.9.0rc1/pyms/config/resource.py
+-rw-r--r--   0        0        0      450 2024-05-25 10:18:44.713663 py_ms-2.9.0rc1/pyms/constants.py
+-rw-r--r--   0        0        0        0 2024-05-25 10:18:44.713663 py_ms-2.9.0rc1/pyms/crypt/__init__.py
+-rw-r--r--   0        0        0     1587 2024-05-25 10:18:44.713663 py_ms-2.9.0rc1/pyms/crypt/driver.py
+-rw-r--r--   0        0        0     2754 2024-05-25 10:18:44.713663 py_ms-2.9.0rc1/pyms/crypt/fernet.py
+-rw-r--r--   0        0        0      427 2024-05-25 10:18:44.713663 py_ms-2.9.0rc1/pyms/exceptions.py
+-rw-r--r--   0        0        0        0 2024-05-25 10:18:44.713663 py_ms-2.9.0rc1/pyms/flask/__init__.py
+-rw-r--r--   0        0        0      109 2024-05-25 10:18:44.713663 py_ms-2.9.0rc1/pyms/flask/app/__init__.py
+-rw-r--r--   0        0        0     7161 2024-05-25 13:43:25.922841 py_ms-2.9.0rc1/pyms/flask/app/create_app.py
+-rw-r--r--   0        0        0      307 2024-05-25 10:18:44.713663 py_ms-2.9.0rc1/pyms/flask/app/create_config.py
+-rw-r--r--   0        0        0     2678 2024-05-25 10:18:44.713663 py_ms-2.9.0rc1/pyms/flask/app/utils.py
+-rw-r--r--   0        0        0       87 2024-05-25 10:18:44.713663 py_ms-2.9.0rc1/pyms/flask/configreload/__init__.py
+-rw-r--r--   0        0        0      416 2024-05-25 10:18:44.713663 py_ms-2.9.0rc1/pyms/flask/configreload/configreload.py
+-rw-r--r--   0        0        0       84 2024-05-25 10:18:44.713663 py_ms-2.9.0rc1/pyms/flask/healthcheck/__init__.py
+-rw-r--r--   0        0        0      428 2024-05-25 10:18:44.713663 py_ms-2.9.0rc1/pyms/flask/healthcheck/healthcheck.py
+-rw-r--r--   0        0        0        0 2024-05-25 10:18:44.713663 py_ms-2.9.0rc1/pyms/flask/services/__init__.py
+-rw-r--r--   0        0        0     2376 2024-05-25 10:18:44.713663 py_ms-2.9.0rc1/pyms/flask/services/driver.py
+-rw-r--r--   0        0        0     3811 2024-05-25 15:00:58.046413 py_ms-2.9.0rc1/pyms/flask/services/metrics.py
+-rw-r--r--   0        0        0    16871 2024-05-25 13:42:34.262619 py_ms-2.9.0rc1/pyms/flask/services/requests.py
+-rw-r--r--   0        0        0     2126 2024-05-25 10:18:44.713663 py_ms-2.9.0rc1/pyms/flask/services/service_discovery.py
+-rw-r--r--   0        0        0     4708 2024-05-25 13:42:34.158619 py_ms-2.9.0rc1/pyms/flask/services/swagger.py
+-rw-r--r--   0        0        0     3807 2024-05-25 15:01:23.894522 py_ms-2.9.0rc1/pyms/flask/services/tracer.py
+-rw-r--r--   0        0        0      100 2024-05-25 13:42:34.074618 py_ms-2.9.0rc1/pyms/logger/__init__.py
+-rw-r--r--   0        0        0     1423 2024-05-25 13:42:34.114618 py_ms-2.9.0rc1/pyms/logger/logger.py
+-rw-r--r--   0        0        0      138 2024-05-25 10:18:44.713663 py_ms-2.9.0rc1/pyms/utils/__init__.py
+-rw-r--r--   0        0        0     1986 2024-05-25 10:18:44.713663 py_ms-2.9.0rc1/pyms/utils/files.py
+-rw-r--r--   0        0        0     1341 2024-05-25 10:18:44.713663 py_ms-2.9.0rc1/pyms/utils/utils.py
+-rw-r--r--   0        0        0     3390 2024-05-25 16:03:50.818358 py_ms-2.9.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     5130 1970-01-01 00:00:00.000000 py_ms-2.9.0rc1/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `py-ms-2.8.0/README.md` & `py_ms-2.9.0rc1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -15,18 +15,19 @@
 
 - Externalized configuration
 - Logging
 - Health checks
 - Metrics
 - Distributed tracing
 
-PyMS is powered by [Flask](https://flask.palletsprojects.com/en/1.1.x/), [Connexion](https://github.com/zalando/connexion)
+PyMS is powered by [Flask](https://flask.palletsprojects.com/en/1.1.x/), [Connexion](https://github.com/spec-first/connexion)
 and [Opentracing](https://opentracing.io/).
 
-Get started with [Installation](./docs/installation.md) and then get an overview with the [Quickstart](./docs/quickstart.md).
+Get started with [Installation](https://python-microservices.github.io/installation/)
+and then get an overview with the [Quickstart](https://python-microservices.github.io/quickstart/).
 
 ## Documentation
 
 To know how to use, install or build a project see the [docs](https://python-microservices.github.io/).
 
 ## Installation
 
@@ -41,8 +42,8 @@
 ## Create a project from scaffold
 
 See our [Create a project from scaffold webpage](https://python-microservices.github.io/quickstart/#create-a-project-from-scaffold)
 
 ## How To contribute
 
 We appreciate opening issues and pull requests to make PyMS even more stable & useful! See [This doc](https://python-microservices.github.io/contributing/)
-for more details.
+for more details.
```

### Comparing `py-ms-2.8.0/pyms/cloud/aws/kms.py` & `py_ms-2.9.0rc1/pyms/cloud/aws/kms.py`

 * *Files identical despite different names*

### Comparing `py-ms-2.8.0/pyms/cmd/main.py` & `py_ms-2.9.0rc1/pyms/cmd/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,33 @@
 #!/usr/bin/env python
 from __future__ import print_function, unicode_literals
 
 import argparse
 import os
 import sys
-from distutils.util import strtobool
 
 from pyms.config import create_conf_file
 from pyms.crypt.fernet import Crypt
 from pyms.flask.services.swagger import merge_swagger_file
 from pyms.utils import check_package_exists, import_from, utils
 
 
+def _asbool(value):
+    """Convert the given String to a boolean object.
+
+    Accepted values are `True` and `1`.
+    """
+    if value is None:
+        return False
+
+    if isinstance(value, bool):
+        return value
+
+    return value.lower() in ("true", "1")
+
 class Command:
     config = None
 
     parser = None
 
     args = []
 
@@ -142,18 +154,19 @@
         return True
 
     def yes_no_input(self, msg=""):  # pragma: no cover
         answer = input(  # nosec
             utils.colored_text(f'{msg}{"?" if not msg.endswith("?") else ""} [Y/n] :', utils.Colors.BLUE, True)
         )
         try:
-            return strtobool(answer)
+            return _asbool(answer)
         except ValueError:
             self.print_error('Invalid input, Please answer with a "Y" or "n"')
             self.yes_no_input(msg)
+        return False
 
     @staticmethod
     def print_ok(msg=""):
         print(utils.colored_text(msg, utils.Colors.BRIGHT_GREEN, True))
 
     def print_verbose(self, msg=""):  # pragma: no cover
         if self.verbose:
```

### Comparing `py-ms-2.8.0/pyms/config/conf.py` & `py_ms-2.9.0rc1/pyms/config/conf.py`

 * *Files identical despite different names*

### Comparing `py-ms-2.8.0/pyms/config/confile.py` & `py_ms-2.9.0rc1/pyms/config/confile.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Module to read yaml or json conf"""
+
 import logging
 import os
 import re
 from typing import Dict, Iterable, Text, Tuple, Union
 
 import anyconfig
```

### Comparing `py-ms-2.8.0/pyms/crypt/driver.py` & `py_ms-2.9.0rc1/pyms/crypt/driver.py`

 * *Files identical despite different names*

### Comparing `py-ms-2.8.0/pyms/crypt/fernet.py` & `py_ms-2.9.0rc1/pyms/crypt/fernet.py`

 * *Files identical despite different names*

### Comparing `py-ms-2.8.0/pyms/flask/app/create_app.py` & `py_ms-2.9.0rc1/pyms/flask/app/create_app.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from flask import Flask
 
 from pyms.config.conf import validate_conf
 from pyms.config.resource import ConfigResource
 from pyms.constants import CONFIG_BASE, LOGGER_NAME
 from pyms.crypt.driver import CryptResource
-from pyms.flask.app.utils import ReverseProxied, SingletonMeta
+from pyms.flask.app.utils import SingletonMeta
 from pyms.flask.configreload import configreload_blueprint
 from pyms.flask.healthcheck import healthcheck_blueprint
 from pyms.flask.services.driver import DriverService, ServicesResource
 from pyms.logger import CustomJsonFormatter
 from pyms.utils import check_package_exists
 
 logger = logging.getLogger(LOGGER_NAME)
@@ -94,18 +94,17 @@
 
     def init_logger(self) -> None:
         """
         Set a logger and return in JSON format.
         :return:
         """
         self.application.logger = logger
-        os.environ["WERKZEUG_RUN_MAIN"] = "true"
 
         formatter = CustomJsonFormatter()
-        formatter.add_service_name(self.application.config["APP_NAME"])
+        formatter.add_service_name(self.application.config.get("APP_NAME", "no_service_name"))
         log_handler = logging.StreamHandler()
         log_handler.setFormatter(formatter)
 
         self.application.logger.addHandler(log_handler)
 
         self.application.logger.propagate = False
 
@@ -127,16 +126,16 @@
                 __name__,
                 static_folder=os.path.join(self.path, "static"),
                 template_folder=os.path.join(self.path, "templates"),
             )
 
         application.root_path = self.path
 
-        # Fix connexion issue https://github.com/zalando/connexion/issues/527
-        application.wsgi_app = ReverseProxied(application.wsgi_app)
+        # Fix connexion issue https://github.com/spec-first/connexion/issues/527
+        # application.wsgi_app = ReverseProxied(application.wsgi_app)
 
         return application
 
     def reload_conf(self):
         self.delete_services()
         self.config.reload()
         self.services = []
@@ -148,20 +147,29 @@
         """Initialize the Flask app, register blueprints and initialize
         all libraries like Swagger, database,
         the trace system...
         return the app and the database objects.
         :return:
         """
         self.application = self.init_app()
-        self.application.config.from_object(self.config.to_flask())
-        self.application.ms = self
+        if hasattr(self.application, "connexion_app"):
+            self.application.connexion_app.app.config.from_object(self.config.to_flask())
+            self.application.ms = self
+
+            # Initialize Blueprints
+            self.application.connexion_app.app.register_blueprint(healthcheck_blueprint)
+            self.application.connexion_app.app.register_blueprint(configreload_blueprint)
 
-        # Initialize Blueprints
-        self.application.register_blueprint(healthcheck_blueprint)
-        self.application.register_blueprint(configreload_blueprint)
+        else:
+            self.application.config.from_object(self.config.to_flask())
+            self.application.ms = self
+
+            # Initialize Blueprints
+            self.application.register_blueprint(healthcheck_blueprint)
+            self.application.register_blueprint(configreload_blueprint)
 
         self.init_libs()
         self.add_error_handlers()
         self.init_logger()
 
         self.init_services_actions()
```

### Comparing `py-ms-2.8.0/pyms/flask/app/utils.py` & `py_ms-2.9.0rc1/pyms/flask/app/utils.py`

 * *Files identical despite different names*

### Comparing `py-ms-2.8.0/pyms/flask/services/driver.py` & `py_ms-2.9.0rc1/pyms/flask/services/driver.py`

 * *Files identical despite different names*

### Comparing `py-ms-2.8.0/pyms/flask/services/metrics.py` & `py_ms-2.9.0rc1/pyms/flask/services/metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,47 +1,51 @@
 import logging
 import time
 
 from flask import Blueprint, Flask, Response, request
 from prometheus_client import REGISTRY, CollectorRegistry, Counter, Histogram, generate_latest, multiprocess
 
-from pyms.flask.services.driver import DriverService
+from pyms.config.conf import get_conf
+from pyms.flask.services.driver import DriverService, get_service_name
 
 # Based on https://github.com/sbarratt/flask-prometheus
 # and https://github.com/korfuri/python-logging-prometheus/
 
-FLASK_REQUEST_LATENCY = Histogram(
-    "http_server_requests_seconds", "Flask Request Latency", ["service", "method", "uri", "status"]
-)
+METRICS_CONFIG = get_conf(service=get_service_name(service="metrics"), empty_init=True)
+
 FLASK_REQUEST_COUNT = Counter(
     "http_server_requests_count", "Flask Request Count", ["service", "method", "uri", "status"]
 )
 
+FLASK_REQUEST_LATENCY = Histogram(
+    "http_server_requests_seconds", "Flask Request Latency", ["service", "method", "uri", "status"]
+)
+
 LOGGER_TOTAL_MESSAGES = Counter(
     "logger_messages_total",
     "Count of log entries by service and level.",
     ["service", "level"],
 )
 
 
 class FlaskMetricsWrapper:
     def __init__(self, app_name):
         self.app_name = app_name
 
-    def before_request(self) -> None:  # pylint: disable=R0201
-        request.start_time = time.time()
+    def before_request(self) -> None:
+        request.start_time = time.time()  # pylint: disable=assigning-non-slot
 
     def after_request(self, response: Response) -> Response:
         if hasattr(request.url_rule, "rule"):
             path = request.url_rule.rule
         else:
             path = request.path
         request_latency = time.time() - request.start_time
-        FLASK_REQUEST_LATENCY.labels(self.app_name, request.method, path, response.status_code).observe(request_latency)
         FLASK_REQUEST_COUNT.labels(self.app_name, request.method, path, response.status_code).inc()
+        FLASK_REQUEST_LATENCY.labels(self.app_name, request.method, path, response.status_code).observe(request_latency)
 
         return response
 
 
 class Service(DriverService):
     """
     Adds [Prometheus](https://prometheus.io/) metrics using the [Prometheus Client Library](https://github.com/prometheus/client_python).
```

### Comparing `py-ms-2.8.0/pyms/flask/services/requests.py` & `py_ms-2.9.0rc1/pyms/flask/services/requests.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,35 @@
 """Encapsulate common rest operations between business services propagating trace headers if configured.
 """
+
 import logging
 from typing import Any
 
 import requests
 from flask import request
 from requests.adapters import HTTPAdapter, Response
 from urllib3.util.retry import Retry
 
+from pyms.config.conf import get_conf
 from pyms.constants import LOGGER_NAME
-from pyms.flask.services.driver import DriverService
+from pyms.flask.services.driver import DriverService, get_service_name
 from pyms.flask.services.tracer import inject_span_in_headers
 
+try:
+    from prometheus_client import Counter, Histogram
+
+    REQUESTS_COUNT = Counter(
+        "http_client_requests_count", "Python requests count", ["service", "method", "uri", "status"]
+    )
+    REQUESTS_LATENCY = Histogram(
+        "http_client_requests_seconds", "Python requests latency", ["service", "method", "uri", "status"]
+    )
+except ModuleNotFoundError:  # pragma: no cover
+    pass
+
 logger = logging.getLogger(LOGGER_NAME)
 
 DEFAULT_RETRIES = 3
 
 DEFAULT_STATUS_RETRIES = (500, 502, 504)
 
 
@@ -51,14 +65,17 @@
         "data": "",
         "retries": DEFAULT_RETRIES,
         "status_retries": DEFAULT_STATUS_RETRIES,
         "propagate_headers": False,
     }
     tracer = None
 
+    def init_action(self, microservice_instance):
+        self.app_name = microservice_instance.application.config["APP_NAME"]  # pylint: disable=W0201
+
     def requests(self, session: requests.Session) -> requests.Session:
         """
         A backoff factor to apply between attempts after the second try (most errors are resolved immediately by a
         second try without a delay). urllib3 will sleep for: {backoff factor} * (2 ^ ({number of total retries} - 1))
         seconds. If the backoff_factor is 0.1, then sleep() will sleep for [0.0s, 0.2s, 0.4s, ...] between retries.
         It will never be longer than Retry.BACKOFF_MAX. By default, backoff is disabled (set to 0).
         :param session:
@@ -71,14 +88,18 @@
             connect=self.retries,
             backoff_factor=0.3,
             status_forcelist=self.status_retries,
         )
         adapter = HTTPAdapter(max_retries=max_retries)
         session_r.mount("http://", adapter)
         session_r.mount("https://", adapter)
+
+        metrics_enabled = get_conf(service=get_service_name(service="metrics"), empty_init=True)
+        if metrics_enabled:
+            session_r.hooks["response"] = [self.observe_requests]
         return session_r
 
     @staticmethod
     def insert_trace_headers(headers: dict) -> dict:
         """Inject trace headers if enabled.
 
         :param headers: dictionary of HTTP Headers to send.
@@ -351,7 +372,13 @@
         logger.debug("Delete with url {}, headers {}, kwargs {}".format(full_url, headers, kwargs))
 
         session = requests.Session()
         response = self.requests(session=session).delete(full_url, headers=headers, **kwargs)
         logger.debug("Response {}".format(response))
 
         return response
+
+    def observe_requests(self, response, *args, **kwargs):
+        REQUESTS_COUNT.labels(self.app_name, response.request.method, response.url, response.status_code).inc()
+        REQUESTS_LATENCY.labels(self.app_name, response.request.method, response.url, response.status_code).observe(
+            float(response.elapsed.total_seconds())
+        )
```

### Comparing `py-ms-2.8.0/pyms/flask/services/service_discovery.py` & `py_ms-2.9.0rc1/pyms/flask/services/service_discovery.py`

 * *Files identical despite different names*

### Comparing `py-ms-2.8.0/pyms/flask/services/swagger.py` & `py_ms-2.9.0rc1/pyms/flask/services/swagger.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 from pathlib import Path
 from typing import Any, Dict
 
 import connexion
+from connexion.options import SwaggerUIOptions
 from connexion.resolver import RestyResolver
 from flask import Flask
 
 try:
     import prance
     from prance.util import formats, fs
 except ModuleNotFoundError:  # pragma: no cover
@@ -51,15 +52,15 @@
 
 class Service(DriverService):
     """The parameters you can add to your config are:
     * **path:** The relative or absolute route to your swagger yaml file. The default value is the current directory
     * **file:** The name of you swagger yaml file. The default value is `swagger.yaml`
     * **url:** The url where swagger run in your server. The default value is `/ui/`.
     * **project_dir:** Relative path of the project folder to automatic routing,
-      see [this link for more info](https://github.com/zalando/connexion#automatic-routing).
+      see [this link for more info](https://github.com/spec-first/connexion#automatic-routing).
       The default value is `project`
 
     All default values keys are created as class attributes in `DriverService`
     """
 
     config_resource = "swagger"
     default_values = {
@@ -77,15 +78,15 @@
             application_root = config.APPLICATION_ROOT
         except AttrDoesNotExistException:
             application_root = "/"
         return application_root
 
     def init_app(self, config, path: Path) -> Flask:
         """
-        Initialize Connexion App. See more info in [Connexion Github](https://github.com/zalando/connexion)
+        Initialize Connexion App. See more info in [Connexion Github](https://github.com/spec-first/connexion)
         :param config: The Flask configuration defined in the config.yaml:
         ```yaml
         pyms:
           services:
             requests: true
             swagger:
               path: ""
@@ -109,30 +110,31 @@
         specification_dir = self.path
         application_root = self._get_application_root(config)
         if not os.path.isabs(self.path):
             specification_dir = os.path.join(path, self.path)
 
         # Prepare params
         validator_map = {k: import_class(v) for k, v in self.validator_map.items()}
+        options = SwaggerUIOptions(swagger_ui_path=self.url)
         params = {
-            "specification": get_bundled_specs(Path(os.path.join(specification_dir, self.file)))
-            if prance
-            else self.file,
+            "specification": (
+                get_bundled_specs(Path(os.path.join(specification_dir, self.file))) if prance else self.file
+            ),
             "arguments": {"title": config.APP_NAME},
             "base_path": application_root,
-            "options": {"swagger_url": self.url},
+            "swagger_ui_options": options,
             "validator_map": validator_map,
             "validate_responses": self.validate_responses,
         }
 
-        # Fix Connexion issue https://github.com/zalando/connexion/issues/1135
-        if application_root == "/":
-            del params["base_path"]
+        # Fix Connexion issue https://github.com/spec-first/connexion/issues/1135
+        # if application_root == "/":
+        #     del params["base_path"]
 
         # Initialize connexion
-        app = connexion.App(__name__, specification_dir=specification_dir, resolver=RestyResolver(self.project_dir))
+        app = connexion.FlaskApp(__name__, swagger_ui_options=options, resolver=RestyResolver(self.project_dir))
         app.add_api(**params)
 
         # Invert the objects, instead connexion with a Flask object, a Flask object with
         application = app.app
         application.connexion_app = app
         return application
```

### Comparing `py-ms-2.8.0/pyms/flask/services/tracer.py` & `py_ms-2.9.0rc1/pyms/flask/services/tracer.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,22 @@
 import logging
 from typing import Union
 
-try:
-    import opentracing
-except ModuleNotFoundError:  # pragma: no cover
-    opentracing = None
-try:
-    from jaeger_client.metrics.prometheus import PrometheusMetricsFactory
-except ModuleNotFoundError:  # pragma: no cover
-    PrometheusMetricsFactory = None
-try:
-    from opentracing_instrumentation import get_current_span
-except ModuleNotFoundError:  # pragma: no cover
-    get_current_span = None
-
 from flask import current_app, has_request_context, request
 
-from pyms.config.conf import get_conf
 from pyms.constants import LOGGER_NAME
-from pyms.flask.services.driver import DriverService, get_service_name
+from pyms.flask.services.driver import DriverService
 from pyms.utils import check_package_exists, import_from, import_package
 
+opentracing = None
+
+PrometheusMetricsFactory = None
+
+get_current_span = None
+
 logger = logging.getLogger(LOGGER_NAME)
 
 JAEGER_CLIENT = "jaeger"
 LIGHT_CLIENT = "lightstep"
 
 DEFAULT_CLIENT = JAEGER_CLIENT
 
@@ -35,15 +27,15 @@
         tracer = current_app.tracer if getattr(current_app, "tracer") else None
         # Add traces
         span = None
         current_app.app_context()
         if tracer:
             span = tracer.get_span(request=request)
             if not span:  # pragma: no cover
-                span = get_current_span()
+                span = get_current_span
                 if not span:
                     span = tracer.tracer.start_span()
             context = span.context if span else None
             tracer.tracer.inject(context, opentracing.Format.HTTP_HEADERS, headers)
     return headers
 
 
@@ -55,17 +47,18 @@
 
     config_resource = "tracer"
     default_values = {
         "client": DEFAULT_CLIENT,
     }
 
     def init_action(self, microservice_instance):
-        FlaskTracing = import_from("flask_opentracing", "FlaskTracing")
-        client = self.get_client()
-        microservice_instance.application.tracer = FlaskTracing(client, True, microservice_instance.application)
+        # FlaskTracing = import_from("flask_opentracing", "FlaskTracing")
+        # client = self.get_client()
+        # microservice_instance.application.tracer = FlaskTracing(client, True, microservice_instance.application)
+        pass
 
     def get_client(self) -> Union[bool, type]:
         opentracing_tracer = False
         if self.config.client == JAEGER_CLIENT:
             opentracing_tracer = self.init_jaeger_tracer()
         elif self.config.client == LIGHT_CLIENT:
             opentracing_tracer = self.init_lightstep_tracer()
@@ -80,19 +73,19 @@
         :return: opentracing.Tracer
         """
         check_package_exists("jaeger_client")
         Config = import_from("jaeger_client", "Config")
         host = {}
         if self.host:
             host = {"local_agent": {"reporting_host": self.host}}
-        metrics_config = get_conf(service=get_service_name(service="metrics"), empty_init=True)
+        # metrics_config = get_conf(service=get_service_name(service="metrics"), empty_init=True)
         metrics = ""
-        if metrics_config:
-            service_name = self.component_name.lower().replace("-", "_").replace(" ", "_")
-            metrics = PrometheusMetricsFactory(service_name_label=service_name)
+        # if metrics_config:
+        #     service_name = self.component_name.lower().replace("-", "_").replace(" ", "_")
+        #     metrics = PrometheusMetricsFactory(service_name_label=service_name)
         config = Config(
             config={
                 **{
                     "sampler": {
                         "type": "const",
                         "param": 1,
                     },
```

### Comparing `py-ms-2.8.0/pyms/logger/logger.py` & `py_ms-2.9.0rc1/pyms/logger/logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Return a JSON as log to insert, i.e, elasticsearch
 """
+
 import datetime
 import logging
 
 from pythonjsonlogger import jsonlogger
 
 from pyms.constants import LOGGER_NAME
 from pyms.flask.services.tracer import inject_span_in_headers
```

### Comparing `py-ms-2.8.0/pyms/utils/files.py` & `py_ms-2.9.0rc1/pyms/utils/files.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,17 +19,16 @@
         self.default_file = default_filename
 
     def get_file(self, fn=None):
         return self._get_conf_from_env(fn) or self._get_conf_from_file(self.path, fn)
 
     def put_file(self, content, mode="w"):
         path = self.get_path_from_env()
-        file_to_write = open(path, mode)
-        file_to_write.write(content)  # The key is type bytes still
-        file_to_write.close()
+        with open(path, mode) as file_to_write:  # pylint: disable=unspecified-encoding
+            file_to_write.write(content)  # The key is type bytes still
 
     def get_path_from_env(self):
         config_file = os.environ.get(self.file_env_location, self.default_file)
         logger.debug("Searching file in ENV[{}]: {}...".format(self.file_env_location, config_file))
         return config_file
 
     def _get_conf_from_env(self, fn=None):
@@ -45,17 +44,16 @@
             return {}
         if path not in files_cached:
             logger.debug("[CONF] Configmap {} found".format(path))
             self.path = path
             if fn:
                 files_cached[path] = fn(path)
             else:
-                file_to_read = open(path, "rb")
-                content = file_to_read.read()  # The key will be type bytes
-                file_to_read.close()
+                with open(path, "rb") as file_to_read:
+                    content = file_to_read.read()  # The key will be type bytes
                 files_cached[path] = content
         return files_cached[path]
 
     def reload(self, fn=None):
         path = self.path or self.get_path_from_env()
         files_cached.pop(path, None)
         return self.get_file(fn)
```

### Comparing `py-ms-2.8.0/pyms/utils/utils.py` & `py_ms-2.9.0rc1/pyms/utils/utils.py`

 * *Files identical despite different names*

