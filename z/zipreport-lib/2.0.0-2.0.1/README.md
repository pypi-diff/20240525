# Comparing `tmp/zipreport-lib-2.0.0.tar.gz` & `tmp/zipreport-lib-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zipreport-lib-2.0.0.tar", last modified: Tue Nov 21 15:08:57 2023, max compression
+gzip compressed data, was "zipreport-lib-2.0.1.tar", last modified: Sat May 25 16:26:52 2024, max compression
```

## Comparing `zipreport-lib-2.0.0.tar` & `zipreport-lib-2.0.1.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 15:08:57.155031 zipreport-lib-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2023-11-21 15:08:50.000000 zipreport-lib-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5458 2023-11-21 15:08:57.155031 zipreport-lib-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4451 2023-11-21 15:08:50.000000 zipreport-lib-2.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2023-11-21 15:08:57.155031 zipreport-lib-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       37 2023-11-21 15:08:50.000000 zipreport-lib-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 15:08:57.147031 zipreport-lib-2.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 15:08:50.000000 zipreport-lib-2.0.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 15:08:57.147031 zipreport-lib-2.0.0/tests/fileutils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 15:08:50.000000 zipreport-lib-2.0.0/tests/fileutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5289 2023-11-21 15:08:50.000000 zipreport-lib-2.0.0/tests/fileutils/basefs.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2023-11-21 15:08:50.000000 zipreport-lib-2.0.0/tests/fileutils/basezip.py
--rw-r--r--   0 runner    (1001) docker     (127)     3478 2023-11-21 15:08:50.000000 zipreport-lib-2.0.0/tests/fileutils/test_diskfs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2023-11-21 15:08:50.000000 zipreport-lib-2.0.0/tests/fileutils/test_pathcache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2545 2023-11-21 15:08:50.000000 zipreport-lib-2.0.0/tests/fileutils/test_zip.py
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2023-11-21 15:08:50.000000 zipreport-lib-2.0.0/tests/fileutils/test_zipfs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 15:08:57.147031 zipreport-lib-2.0.0/tests/processors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 15:08:50.000000 zipreport-lib-2.0.0/tests/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2023-11-21 15:08:50.000000 zipreport-lib-2.0.0/tests/processors/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2843 2023-11-21 15:08:50.000000 zipreport-lib-2.0.0/tests/processors/test_mime.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 15:08:57.151031 zipreport-lib-2.0.0/tests/render/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 15:08:50.000000 zipreport-lib-2.0.0/tests/render/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      772 2023-11-21 15:08:50.000000 zipreport-lib-2.0.0/tests/render/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 15:08:57.151031 zipreport-lib-2.0.0/tests/render/filters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 15:08:50.000000 zipreport-lib-2.0.0/tests/render/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16027 2023-11-21 15:08:50.000000 zipreport-lib-2.0.0/tests/render/filters/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2023-11-21 15:08:50.000000 zipreport-lib-2.0.0/tests/render/filters/test_jinjafilters.py
--rw-r--r--   0 runner    (1001) docker     (127)      589 2023-11-21 15:08:50.000000 zipreport-lib-2.0.0/tests/render/test_jinjaloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2023-11-21 15:08:50.000000 zipreport-lib-2.0.0/tests/render/test_jinjarender.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 15:08:57.151031 zipreport-lib-2.0.0/tests/report/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 15:08:50.000000 zipreport-lib-2.0.0/tests/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3313 2023-11-21 15:08:50.000000 zipreport-lib-2.0.0/tests/report/test_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2023-11-21 15:08:50.000000 zipreport-lib-2.0.0/tests/report/test_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2023-11-21 15:08:50.000000 zipreport-lib-2.0.0/tests/report/test_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 15:08:57.151031 zipreport-lib-2.0.0/tests/server/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 15:08:50.000000 zipreport-lib-2.0.0/tests/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3847 2023-11-21 15:08:50.000000 zipreport-lib-2.0.0/tests/server/test_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      715 2023-11-21 15:08:50.000000 zipreport-lib-2.0.0/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 15:08:57.151031 zipreport-lib-2.0.0/zipreport/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2023-11-21 15:08:50.000000 zipreport-lib-2.0.0/zipreport/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 15:08:57.151031 zipreport-lib-2.0.0/zipreport/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-21 15:08:50.000000 zipreport-lib-2.0.0/zipreport/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5336 2023-11-21 15:08:50.000000 zipreport-lib-2.0.0/zipreport/cli/console.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 15:08:57.151031 zipreport-lib-2.0.0/zipreport/cli/debug/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 15:08:50.000000 zipreport-lib-2.0.0/zipreport/cli/debug/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8665 2023-11-21 15:08:50.000000 zipreport-lib-2.0.0/zipreport/cli/debug/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 15:08:57.151031 zipreport-lib-2.0.0/zipreport/fileutils/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2023-11-21 15:08:50.000000 zipreport-lib-2.0.0/zipreport/fileutils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 15:08:57.151031 zipreport-lib-2.0.0/zipreport/fileutils/backend/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 15:08:50.000000 zipreport-lib-2.0.0/zipreport/fileutils/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4170 2023-11-21 15:08:50.000000 zipreport-lib-2.0.0/zipreport/fileutils/backend/zip.py
--rw-r--r--   0 runner    (1001) docker     (127)     4937 2023-11-21 15:08:50.000000 zipreport-lib-2.0.0/zipreport/fileutils/diskfs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2023-11-21 15:08:50.000000 zipreport-lib-2.0.0/zipreport/fileutils/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     3631 2023-11-21 15:08:50.000000 zipreport-lib-2.0.0/zipreport/fileutils/pathcache.py
--rw-r--r--   0 runner    (1001) docker     (127)     3868 2023-11-21 15:08:50.000000 zipreport-lib-2.0.0/zipreport/fileutils/zipfs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 15:08:57.151031 zipreport-lib-2.0.0/zipreport/misc/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-11-21 15:08:50.000000 zipreport-lib-2.0.0/zipreport/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      655 2023-11-21 15:08:50.000000 zipreport-lib-2.0.0/zipreport/misc/html.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 15:08:57.155031 zipreport-lib-2.0.0/zipreport/processors/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2023-11-21 15:08:50.000000 zipreport-lib-2.0.0/zipreport/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      143 2023-11-21 15:08:50.000000 zipreport-lib-2.0.0/zipreport/processors/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     3013 2023-11-21 15:08:50.000000 zipreport-lib-2.0.0/zipreport/processors/mime.py
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2023-11-21 15:08:50.000000 zipreport-lib-2.0.0/zipreport/processors/weasyprint.py
--rw-r--r--   0 runner    (1001) docker     (127)     2365 2023-11-21 15:08:50.000000 zipreport-lib-2.0.0/zipreport/processors/zipreport.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 15:08:57.155031 zipreport-lib-2.0.0/zipreport/report/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2023-11-21 15:08:50.000000 zipreport-lib-2.0.0/zipreport/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6232 2023-11-21 15:08:50.000000 zipreport-lib-2.0.0/zipreport/report/builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1764 2023-11-21 15:08:50.000000 zipreport-lib-2.0.0/zipreport/report/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     4988 2023-11-21 15:08:50.000000 zipreport-lib-2.0.0/zipreport/report/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     2662 2023-11-21 15:08:50.000000 zipreport-lib-2.0.0/zipreport/report/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2023-11-21 15:08:50.000000 zipreport-lib-2.0.0/zipreport/report/reportfile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 15:08:57.155031 zipreport-lib-2.0.0/zipreport/template/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2023-11-21 15:08:50.000000 zipreport-lib-2.0.0/zipreport/template/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 15:08:57.155031 zipreport-lib-2.0.0/zipreport/template/jinja/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 15:08:50.000000 zipreport-lib-2.0.0/zipreport/template/jinja/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5029 2023-11-21 15:08:50.000000 zipreport-lib-2.0.0/zipreport/template/jinja/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2023-11-21 15:08:50.000000 zipreport-lib-2.0.0/zipreport/template/jinjaloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3327 2023-11-21 15:08:50.000000 zipreport-lib-2.0.0/zipreport/template/jinjarender.py
--rw-r--r--   0 runner    (1001) docker     (127)      126 2023-11-21 15:08:50.000000 zipreport-lib-2.0.0/zipreport/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2580 2023-11-21 15:08:50.000000 zipreport-lib-2.0.0/zipreport/zipreport.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 15:08:57.155031 zipreport-lib-2.0.0/zipreport_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5458 2023-11-21 15:08:57.000000 zipreport-lib-2.0.0/zipreport_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2023-11-21 15:08:57.000000 zipreport-lib-2.0.0/zipreport_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-21 15:08:57.000000 zipreport-lib-2.0.0/zipreport_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2023-11-21 15:08:57.000000 zipreport-lib-2.0.0/zipreport_lib.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-21 15:08:57.000000 zipreport-lib-2.0.0/zipreport_lib.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       55 2023-11-21 15:08:57.000000 zipreport-lib-2.0.0/zipreport_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-11-21 15:08:57.000000 zipreport-lib-2.0.0/zipreport_lib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:26:52.106203 zipreport-lib-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5285 2024-05-25 16:26:52.106203 zipreport-lib-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-25 16:26:52.106203 zipreport-lib-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:26:52.094203 zipreport-lib-2.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:26:52.098203 zipreport-lib-2.0.1/tests/fileutils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/tests/fileutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/tests/fileutils/basefs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/tests/fileutils/basezip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/tests/fileutils/test_diskfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/tests/fileutils/test_pathcache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/tests/fileutils/test_zip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/tests/fileutils/test_zipfs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:26:52.098203 zipreport-lib-2.0.1/tests/processors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/tests/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/tests/processors/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/tests/processors/test_mime.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:26:52.098203 zipreport-lib-2.0.1/tests/render/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/tests/render/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/tests/render/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:26:52.098203 zipreport-lib-2.0.1/tests/render/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/tests/render/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16027 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/tests/render/filters/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/tests/render/filters/test_jinjafilters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/tests/render/test_jinjaloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/tests/render/test_jinjarender.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:26:52.098203 zipreport-lib-2.0.1/tests/report/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/tests/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/tests/report/test_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/tests/report/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/tests/report/test_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:26:52.098203 zipreport-lib-2.0.1/tests/server/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/tests/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/tests/server/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:26:52.098203 zipreport-lib-2.0.1/zipreport/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/zipreport/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:26:52.098203 zipreport-lib-2.0.1/zipreport/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/zipreport/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5336 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/zipreport/cli/console.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:26:52.098203 zipreport-lib-2.0.1/zipreport/cli/debug/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/zipreport/cli/debug/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8665 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/zipreport/cli/debug/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:26:52.102203 zipreport-lib-2.0.1/zipreport/fileutils/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/zipreport/fileutils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:26:52.102203 zipreport-lib-2.0.1/zipreport/fileutils/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/zipreport/fileutils/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4170 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/zipreport/fileutils/backend/zip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/zipreport/fileutils/diskfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/zipreport/fileutils/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3631 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/zipreport/fileutils/pathcache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/zipreport/fileutils/zipfs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:26:52.102203 zipreport-lib-2.0.1/zipreport/misc/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/zipreport/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/zipreport/misc/html.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:26:52.102203 zipreport-lib-2.0.1/zipreport/processors/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/zipreport/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/zipreport/processors/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/zipreport/processors/mime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/zipreport/processors/weasyprint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/zipreport/processors/zipreport.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:26:52.102203 zipreport-lib-2.0.1/zipreport/report/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/zipreport/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6232 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/zipreport/report/builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/zipreport/report/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4988 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/zipreport/report/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/zipreport/report/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/zipreport/report/reportfile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:26:52.102203 zipreport-lib-2.0.1/zipreport/template/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/zipreport/template/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:26:52.102203 zipreport-lib-2.0.1/zipreport/template/jinja/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/zipreport/template/jinja/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5029 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/zipreport/template/jinja/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/zipreport/template/jinjaloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/zipreport/template/jinjarender.py
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/zipreport/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/zipreport/zipreport.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:26:52.106203 zipreport-lib-2.0.1/zipreport_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5285 2024-05-25 16:26:52.000000 zipreport-lib-2.0.1/zipreport_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-25 16:26:52.000000 zipreport-lib-2.0.1/zipreport_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 16:26:52.000000 zipreport-lib-2.0.1/zipreport_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-25 16:26:52.000000 zipreport-lib-2.0.1/zipreport_lib.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 16:26:52.000000 zipreport-lib-2.0.1/zipreport_lib.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-25 16:26:52.000000 zipreport-lib-2.0.1/zipreport_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-25 16:26:52.000000 zipreport-lib-2.0.1/zipreport_lib.egg-info/top_level.txt
```

### Comparing `zipreport-lib-2.0.0/LICENSE` & `zipreport-lib-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zipreport-lib-2.0.0/PKG-INFO` & `zipreport-lib-2.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zipreport-lib
-Version: 2.0.0
+Version: 2.0.1
 Summary: Python HTML to PDF reporting engine
 Home-page: https://github.com/zipreport/zipreport
 Author: João Pinheiro
 License: MIT
 Project-URL: Documentation, https://zipreport.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/zipreport/zipreport
 Classifier: Development Status :: 5 - Production/Stable
@@ -23,18 +23,23 @@
 Description-Content-Type: text/markdown
 Provides-Extra: redis
 License-File: LICENSE
 
 # ZipReport
 
 [![Tests](https://github.com/zipreport/zipreport/workflows/Tests/badge.svg?branch=master)](https://github.com/zipreport/zipreport/actions)
-[![docs](https://readthedocs.org/projects/zipreport/badge/?version=latest)](https://zipreport.readthedocs.io/en/latest/)
 [![pypi](https://img.shields.io/pypi/v/zipreport-lib.svg)](https://pypi.org/project/zipreport-lib/)
 [![license](https://img.shields.io/pypi/l/zipreport-lib.svg)](https://github.com/zipreport/zipreport/blob/master/LICENSE)
 
+---
+
+**Documentation:** [https://zipreport.github.io/zipreport/](https://zipreport.github.io/zipreport/)
+
+---
+
 Transform HTML templates into beautiful PDF or MIME reports, with full CSS and client Javascript support, under a
 permissive license.
 
 Want to see it in action? Check this [example](docs/samples/example_report.pdf)!
 
 **Highlights**:
 
@@ -143,12 +148,7 @@
 
 This backend is provided for compatibility. For new projects, please use zipreport-server.
 
 [WeasyPrint](https://weasyprint.org/) is a popular Python library to generate PDFs from HTML. It doesn't support JavaScript,
 and CSS is limited. 
 
 
-### Documentation
-
-Detailed documentation on usage and report building is available on the [project documentation](https://zipreport.readthedocs.io/en/latest/).
-
-
```

### Comparing `zipreport-lib-2.0.0/README.md` & `zipreport-lib-2.0.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 # ZipReport
 
 [![Tests](https://github.com/zipreport/zipreport/workflows/Tests/badge.svg?branch=master)](https://github.com/zipreport/zipreport/actions)
-[![docs](https://readthedocs.org/projects/zipreport/badge/?version=latest)](https://zipreport.readthedocs.io/en/latest/)
 [![pypi](https://img.shields.io/pypi/v/zipreport-lib.svg)](https://pypi.org/project/zipreport-lib/)
 [![license](https://img.shields.io/pypi/l/zipreport-lib.svg)](https://github.com/zipreport/zipreport/blob/master/LICENSE)
 
+---
+
+**Documentation:** [https://zipreport.github.io/zipreport/](https://zipreport.github.io/zipreport/)
+
+---
+
 Transform HTML templates into beautiful PDF or MIME reports, with full CSS and client Javascript support, under a
 permissive license.
 
 Want to see it in action? Check this [example](docs/samples/example_report.pdf)!
 
 **Highlights**:
 
@@ -117,12 +122,7 @@
 
 This backend is provided for compatibility. For new projects, please use zipreport-server.
 
 [WeasyPrint](https://weasyprint.org/) is a popular Python library to generate PDFs from HTML. It doesn't support JavaScript,
 and CSS is limited. 
 
 
-### Documentation
-
-Detailed documentation on usage and report building is available on the [project documentation](https://zipreport.readthedocs.io/en/latest/).
-
-
```

### Comparing `zipreport-lib-2.0.0/setup.cfg` & `zipreport-lib-2.0.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = zipreport-lib
-version = attr: zipreport.__version__
+version = attr: zipreport.version.__version__
 url = https://github.com/zipreport/zipreport
 author = João Pinheiro
 description = Python HTML to PDF reporting engine
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
 classifiers =
```

### Comparing `zipreport-lib-2.0.0/tests/fileutils/basefs.py` & `zipreport-lib-2.0.1/tests/fileutils/basefs.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-2.0.0/tests/fileutils/basezip.py` & `zipreport-lib-2.0.1/tests/fileutils/basezip.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-2.0.0/tests/fileutils/test_diskfs.py` & `zipreport-lib-2.0.1/tests/fileutils/test_diskfs.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-2.0.0/tests/fileutils/test_pathcache.py` & `zipreport-lib-2.0.1/tests/fileutils/test_pathcache.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-2.0.0/tests/fileutils/test_zip.py` & `zipreport-lib-2.0.1/tests/fileutils/test_zip.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-2.0.0/tests/fileutils/test_zipfs.py` & `zipreport-lib-2.0.1/tests/fileutils/test_zipfs.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-2.0.0/tests/processors/base.py` & `zipreport-lib-2.0.1/tests/processors/base.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-2.0.0/tests/processors/test_mime.py` & `zipreport-lib-2.0.1/tests/processors/test_mime.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-2.0.0/tests/render/base.py` & `zipreport-lib-2.0.1/tests/render/base.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-2.0.0/tests/render/filters/base.py` & `zipreport-lib-2.0.1/tests/render/filters/base.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-2.0.0/tests/render/filters/test_jinjafilters.py` & `zipreport-lib-2.0.1/tests/render/filters/test_jinjafilters.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-2.0.0/tests/render/test_jinjaloader.py` & `zipreport-lib-2.0.1/tests/render/test_jinjaloader.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-2.0.0/tests/render/test_jinjarender.py` & `zipreport-lib-2.0.1/tests/render/test_jinjarender.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-2.0.0/tests/report/test_builder.py` & `zipreport-lib-2.0.1/tests/report/test_builder.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-2.0.0/tests/report/test_job.py` & `zipreport-lib-2.0.1/tests/report/test_job.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-2.0.0/tests/report/test_loader.py` & `zipreport-lib-2.0.1/tests/report/test_loader.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-2.0.0/tests/server/test_server.py` & `zipreport-lib-2.0.1/tests/server/test_server.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-2.0.0/tests/utils.py` & `zipreport-lib-2.0.1/tests/utils.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-2.0.0/zipreport/cli/console.py` & `zipreport-lib-2.0.1/zipreport/cli/console.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-2.0.0/zipreport/cli/debug/server.py` & `zipreport-lib-2.0.1/zipreport/cli/debug/server.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-2.0.0/zipreport/fileutils/backend/zip.py` & `zipreport-lib-2.0.1/zipreport/fileutils/backend/zip.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-2.0.0/zipreport/fileutils/diskfs.py` & `zipreport-lib-2.0.1/zipreport/fileutils/diskfs.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-2.0.0/zipreport/fileutils/interface.py` & `zipreport-lib-2.0.1/zipreport/fileutils/interface.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-2.0.0/zipreport/fileutils/pathcache.py` & `zipreport-lib-2.0.1/zipreport/fileutils/pathcache.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-2.0.0/zipreport/fileutils/zipfs.py` & `zipreport-lib-2.0.1/zipreport/fileutils/zipfs.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-2.0.0/zipreport/misc/html.py` & `zipreport-lib-2.0.1/zipreport/misc/html.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-2.0.0/zipreport/processors/mime.py` & `zipreport-lib-2.0.1/zipreport/processors/mime.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-2.0.0/zipreport/processors/weasyprint.py` & `zipreport-lib-2.0.1/zipreport/processors/weasyprint.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-2.0.0/zipreport/processors/zipreport.py` & `zipreport-lib-2.0.1/zipreport/processors/zipreport.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-2.0.0/zipreport/report/builder.py` & `zipreport-lib-2.0.1/zipreport/report/builder.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-2.0.0/zipreport/report/const.py` & `zipreport-lib-2.0.1/zipreport/report/const.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-2.0.0/zipreport/report/job.py` & `zipreport-lib-2.0.1/zipreport/report/job.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-2.0.0/zipreport/report/loader.py` & `zipreport-lib-2.0.1/zipreport/report/loader.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-2.0.0/zipreport/report/reportfile.py` & `zipreport-lib-2.0.1/zipreport/report/reportfile.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-2.0.0/zipreport/template/jinja/filters.py` & `zipreport-lib-2.0.1/zipreport/template/jinja/filters.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-2.0.0/zipreport/template/jinjaloader.py` & `zipreport-lib-2.0.1/zipreport/template/jinjaloader.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-2.0.0/zipreport/template/jinjarender.py` & `zipreport-lib-2.0.1/zipreport/template/jinjarender.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-2.0.0/zipreport/zipreport.py` & `zipreport-lib-2.0.1/zipreport/zipreport.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-2.0.0/zipreport_lib.egg-info/PKG-INFO` & `zipreport-lib-2.0.1/zipreport_lib.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zipreport-lib
-Version: 2.0.0
+Version: 2.0.1
 Summary: Python HTML to PDF reporting engine
 Home-page: https://github.com/zipreport/zipreport
 Author: João Pinheiro
 License: MIT
 Project-URL: Documentation, https://zipreport.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/zipreport/zipreport
 Classifier: Development Status :: 5 - Production/Stable
@@ -23,18 +23,23 @@
 Description-Content-Type: text/markdown
 Provides-Extra: redis
 License-File: LICENSE
 
 # ZipReport
 
 [![Tests](https://github.com/zipreport/zipreport/workflows/Tests/badge.svg?branch=master)](https://github.com/zipreport/zipreport/actions)
-[![docs](https://readthedocs.org/projects/zipreport/badge/?version=latest)](https://zipreport.readthedocs.io/en/latest/)
 [![pypi](https://img.shields.io/pypi/v/zipreport-lib.svg)](https://pypi.org/project/zipreport-lib/)
 [![license](https://img.shields.io/pypi/l/zipreport-lib.svg)](https://github.com/zipreport/zipreport/blob/master/LICENSE)
 
+---
+
+**Documentation:** [https://zipreport.github.io/zipreport/](https://zipreport.github.io/zipreport/)
+
+---
+
 Transform HTML templates into beautiful PDF or MIME reports, with full CSS and client Javascript support, under a
 permissive license.
 
 Want to see it in action? Check this [example](docs/samples/example_report.pdf)!
 
 **Highlights**:
 
@@ -143,12 +148,7 @@
 
 This backend is provided for compatibility. For new projects, please use zipreport-server.
 
 [WeasyPrint](https://weasyprint.org/) is a popular Python library to generate PDFs from HTML. It doesn't support JavaScript,
 and CSS is limited. 
 
 
-### Documentation
-
-Detailed documentation on usage and report building is available on the [project documentation](https://zipreport.readthedocs.io/en/latest/).
-
-
```

### Comparing `zipreport-lib-2.0.0/zipreport_lib.egg-info/SOURCES.txt` & `zipreport-lib-2.0.1/zipreport_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

