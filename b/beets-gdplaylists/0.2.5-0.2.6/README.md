# Comparing `tmp/beets_gdplaylists-0.2.5.tar.gz` & `tmp/beets_gdplaylists-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beets_gdplaylists-0.2.5.tar", last modified: Sat May 25 09:51:47 2024, max compression
+gzip compressed data, was "beets_gdplaylists-0.2.6.tar", last modified: Sat May 25 09:58:21 2024, max compression
```

## Comparing `beets_gdplaylists-0.2.5.tar` & `beets_gdplaylists-0.2.6.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 09:51:47.229195 beets_gdplaylists-0.2.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 09:51:47.217195 beets_gdplaylists-0.2.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 09:51:47.217195 beets_gdplaylists-0.2.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-05-25 09:51:37.000000 beets_gdplaylists-0.2.5/.github/workflows/createrelease.yml
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-25 09:51:37.000000 beets_gdplaylists-0.2.5/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-25 09:51:37.000000 beets_gdplaylists-0.2.5/.github/workflows/testpythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-25 09:51:37.000000 beets_gdplaylists-0.2.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-25 09:51:37.000000 beets_gdplaylists-0.2.5/.python-version
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-25 09:51:37.000000 beets_gdplaylists-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-25 09:51:37.000000 beets_gdplaylists-0.2.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-25 09:51:47.229195 beets_gdplaylists-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-25 09:51:37.000000 beets_gdplaylists-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 09:51:47.229195 beets_gdplaylists-0.2.5/beets_gdplaylists.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-25 09:51:47.000000 beets_gdplaylists-0.2.5/beets_gdplaylists.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-05-25 09:51:47.000000 beets_gdplaylists-0.2.5/beets_gdplaylists.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 09:51:47.000000 beets_gdplaylists-0.2.5/beets_gdplaylists.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-25 09:51:47.000000 beets_gdplaylists-0.2.5/beets_gdplaylists.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-25 09:51:47.000000 beets_gdplaylists-0.2.5/beets_gdplaylists.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 09:51:47.221195 beets_gdplaylists-0.2.5/beetsplug/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-25 09:51:37.000000 beets_gdplaylists-0.2.5/beetsplug/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 09:51:47.221195 beets_gdplaylists-0.2.5/beetsplug/gdplaylists/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-25 09:51:37.000000 beets_gdplaylists-0.2.5/beetsplug/gdplaylists/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 09:51:47.221195 beets_gdplaylists-0.2.5/beetsplug/gdplaylists/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-25 09:51:37.000000 beets_gdplaylists-0.2.5/beetsplug/gdplaylists/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (127)     5598 2024-05-25 09:51:37.000000 beets_gdplaylists-0.2.5/beetsplug/gdplaylists/__pycache__/gdplex.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (127)     5668 2024-05-25 09:51:37.000000 beets_gdplaylists-0.2.5/beetsplug/gdplaylists/gdplex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 09:51:47.229195 beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/
--rw-r--r--   0 runner    (1001) docker     (127)     3947 2024-05-25 09:51:37.000000 beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1969-11-02.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5072 2024-05-25 09:51:37.000000 beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1969-12-26.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5532 2024-05-25 09:51:37.000000 beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1970-01-02.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3979 2024-05-25 09:51:37.000000 beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1970-01-03.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-05-25 09:51:37.000000 beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1971-10-24.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6452 2024-05-25 09:51:37.000000 beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1971-11-20.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5230 2024-05-25 09:51:37.000000 beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1971-12-09.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6940 2024-05-25 09:51:37.000000 beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1971-12-10.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-05-25 09:51:37.000000 beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1972-09-03.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6383 2024-05-25 09:51:37.000000 beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1972-09-09.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-25 09:51:37.000000 beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1972-09-19.yml
--rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-05-25 09:51:37.000000 beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1972-10-17.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5931 2024-05-25 09:51:37.000000 beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1972-10-18.yml
--rw-r--r--   0 runner    (1001) docker     (127)     7206 2024-05-25 09:51:37.000000 beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1972-10-19.yml
--rw-r--r--   0 runner    (1001) docker     (127)     8404 2024-05-25 09:51:37.000000 beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1973-03-24.yml
--rw-r--r--   0 runner    (1001) docker     (127)     7631 2024-05-25 09:51:37.000000 beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1973-06-22.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6930 2024-05-25 09:51:37.000000 beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1973-06-24.yml
--rw-r--r--   0 runner    (1001) docker     (127)     7671 2024-05-25 09:51:37.000000 beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1973-06-26.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-05-25 09:51:37.000000 beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1973-09-07.yml
--rw-r--r--   0 runner    (1001) docker     (127)     7582 2024-05-25 09:51:37.000000 beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1973-09-08.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6231 2024-05-25 09:51:37.000000 beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1973-10-29.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5527 2024-05-25 09:51:37.000000 beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1973-10-30.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2823 2024-05-25 09:51:37.000000 beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1974-02-22.yml
--rw-r--r--   0 runner    (1001) docker     (127)     7584 2024-05-25 09:51:37.000000 beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1974-02-23.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6677 2024-05-25 09:51:37.000000 beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1974-05-17.yml
--rw-r--r--   0 runner    (1001) docker     (127)     7755 2024-05-25 09:51:37.000000 beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1974-05-19.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5905 2024-05-25 09:51:37.000000 beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1974-05-21.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-05-25 09:51:37.000000 beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1974-06-22.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6606 2024-05-25 09:51:37.000000 beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1974-06-23.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6189 2024-05-25 09:51:37.000000 beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1977-05-03.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-05-25 09:51:37.000000 beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1977-05-04.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5919 2024-05-25 09:51:37.000000 beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1977-05-26.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5927 2024-05-25 09:51:37.000000 beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1977-10-01.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-05-25 09:51:37.000000 beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1977-10-02.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6257 2024-05-25 09:51:37.000000 beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1977-10-29.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4914 2024-05-25 09:51:37.000000 beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1978-04-15.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-05-25 09:51:37.000000 beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1978-04-18.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6355 2024-05-25 09:51:37.000000 beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1978-12-31.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6063 2024-05-25 09:51:37.000000 beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1979-12-03.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-05-25 09:51:37.000000 beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1979-12-04.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6704 2024-05-25 09:51:37.000000 beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1979-12-09.yml
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-25 09:51:37.000000 beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1983-04-15.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-05-25 09:51:37.000000 beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1983-04-25.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-05-25 09:51:37.000000 beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1983-04-26.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-05-25 09:51:37.000000 beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1984-04-19.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5551 2024-05-25 09:51:37.000000 beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1984-04-20.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6329 2024-05-25 09:51:37.000000 beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1985-04-27.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-05-25 09:51:37.000000 beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1985-04-28.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5896 2024-05-25 09:51:37.000000 beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1987-03-26.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5348 2024-05-25 09:51:37.000000 beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1987-03-27.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5503 2024-05-25 09:51:37.000000 beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1990-06-23.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5888 2024-05-25 09:51:37.000000 beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1990-07-18.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5277 2024-05-25 09:51:37.000000 beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1990-07-19.yml
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-25 09:51:37.000000 beets_gdplaylists-0.2.5/justfile
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-25 09:51:37.000000 beets_gdplaylists-0.2.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 09:51:47.229195 beets_gdplaylists-0.2.5/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-05-25 09:51:37.000000 beets_gdplaylists-0.2.5/scripts/mbdl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-05-25 09:51:37.000000 beets_gdplaylists-0.2.5/scripts/releases.yml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 09:51:47.229195 beets_gdplaylists-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-25 09:51:37.000000 beets_gdplaylists-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 09:58:21.273518 beets_gdplaylists-0.2.6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 09:58:21.257518 beets_gdplaylists-0.2.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 09:58:21.261518 beets_gdplaylists-0.2.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-05-25 09:58:12.000000 beets_gdplaylists-0.2.6/.github/workflows/createrelease.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-25 09:58:12.000000 beets_gdplaylists-0.2.6/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-25 09:58:12.000000 beets_gdplaylists-0.2.6/.github/workflows/testpythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-25 09:58:12.000000 beets_gdplaylists-0.2.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-25 09:58:12.000000 beets_gdplaylists-0.2.6/.python-version
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-25 09:58:12.000000 beets_gdplaylists-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-25 09:58:12.000000 beets_gdplaylists-0.2.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-25 09:58:21.273518 beets_gdplaylists-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-25 09:58:12.000000 beets_gdplaylists-0.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 09:58:21.269518 beets_gdplaylists-0.2.6/beets_gdplaylists.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-25 09:58:21.000000 beets_gdplaylists-0.2.6/beets_gdplaylists.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-05-25 09:58:21.000000 beets_gdplaylists-0.2.6/beets_gdplaylists.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 09:58:21.000000 beets_gdplaylists-0.2.6/beets_gdplaylists.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-25 09:58:21.000000 beets_gdplaylists-0.2.6/beets_gdplaylists.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-25 09:58:21.000000 beets_gdplaylists-0.2.6/beets_gdplaylists.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 09:58:21.261518 beets_gdplaylists-0.2.6/beetsplug/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-25 09:58:12.000000 beets_gdplaylists-0.2.6/beetsplug/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 09:58:21.261518 beets_gdplaylists-0.2.6/beetsplug/gdplaylists/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-25 09:58:12.000000 beets_gdplaylists-0.2.6/beetsplug/gdplaylists/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 09:58:21.261518 beets_gdplaylists-0.2.6/beetsplug/gdplaylists/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-25 09:58:12.000000 beets_gdplaylists-0.2.6/beetsplug/gdplaylists/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)     5598 2024-05-25 09:58:12.000000 beets_gdplaylists-0.2.6/beetsplug/gdplaylists/__pycache__/gdplex.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)     5668 2024-05-25 09:58:12.000000 beets_gdplaylists-0.2.6/beetsplug/gdplaylists/gdplex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 09:58:21.269518 beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/
+-rw-r--r--   0 runner    (1001) docker     (127)     3947 2024-05-25 09:58:12.000000 beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1969-11-02.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5072 2024-05-25 09:58:12.000000 beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1969-12-26.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5532 2024-05-25 09:58:12.000000 beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1970-01-02.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3979 2024-05-25 09:58:12.000000 beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1970-01-03.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-05-25 09:58:12.000000 beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1971-10-24.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6452 2024-05-25 09:58:12.000000 beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1971-11-20.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5230 2024-05-25 09:58:12.000000 beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1971-12-09.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6940 2024-05-25 09:58:12.000000 beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1971-12-10.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-05-25 09:58:12.000000 beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1972-09-03.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6383 2024-05-25 09:58:12.000000 beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1972-09-09.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-25 09:58:12.000000 beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1972-09-19.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-05-25 09:58:12.000000 beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1972-10-17.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5931 2024-05-25 09:58:12.000000 beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1972-10-18.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     7206 2024-05-25 09:58:12.000000 beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1972-10-19.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     8404 2024-05-25 09:58:12.000000 beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1973-03-24.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     7631 2024-05-25 09:58:12.000000 beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1973-06-22.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6930 2024-05-25 09:58:12.000000 beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1973-06-24.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     7671 2024-05-25 09:58:12.000000 beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1973-06-26.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-05-25 09:58:12.000000 beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1973-09-07.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     7582 2024-05-25 09:58:12.000000 beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1973-09-08.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6231 2024-05-25 09:58:12.000000 beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1973-10-29.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5527 2024-05-25 09:58:12.000000 beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1973-10-30.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2823 2024-05-25 09:58:12.000000 beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1974-02-22.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     7584 2024-05-25 09:58:12.000000 beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1974-02-23.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6677 2024-05-25 09:58:12.000000 beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1974-05-17.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     7755 2024-05-25 09:58:12.000000 beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1974-05-19.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5905 2024-05-25 09:58:12.000000 beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1974-05-21.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-05-25 09:58:12.000000 beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1974-06-22.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6606 2024-05-25 09:58:12.000000 beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1974-06-23.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6189 2024-05-25 09:58:12.000000 beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1977-05-03.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-05-25 09:58:12.000000 beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1977-05-04.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5919 2024-05-25 09:58:12.000000 beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1977-05-26.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5927 2024-05-25 09:58:12.000000 beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1977-10-01.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-05-25 09:58:12.000000 beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1977-10-02.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6257 2024-05-25 09:58:12.000000 beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1977-10-29.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4914 2024-05-25 09:58:12.000000 beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1978-04-15.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-05-25 09:58:12.000000 beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1978-04-18.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6355 2024-05-25 09:58:12.000000 beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1978-12-31.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6063 2024-05-25 09:58:12.000000 beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1979-12-03.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-05-25 09:58:12.000000 beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1979-12-04.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6704 2024-05-25 09:58:12.000000 beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1979-12-09.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-25 09:58:12.000000 beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1983-04-15.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-05-25 09:58:12.000000 beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1983-04-25.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-05-25 09:58:12.000000 beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1983-04-26.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-05-25 09:58:12.000000 beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1984-04-19.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5551 2024-05-25 09:58:12.000000 beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1984-04-20.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6329 2024-05-25 09:58:12.000000 beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1985-04-27.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-05-25 09:58:12.000000 beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1985-04-28.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5896 2024-05-25 09:58:12.000000 beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1987-03-26.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5348 2024-05-25 09:58:12.000000 beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1987-03-27.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5503 2024-05-25 09:58:12.000000 beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1990-06-23.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5888 2024-05-25 09:58:12.000000 beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1990-07-18.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5277 2024-05-25 09:58:12.000000 beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1990-07-19.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-25 09:58:12.000000 beets_gdplaylists-0.2.6/justfile
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-25 09:58:12.000000 beets_gdplaylists-0.2.6/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 09:58:21.269518 beets_gdplaylists-0.2.6/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-05-25 09:58:12.000000 beets_gdplaylists-0.2.6/scripts/mbdl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-05-25 09:58:12.000000 beets_gdplaylists-0.2.6/scripts/releases.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 09:58:21.273518 beets_gdplaylists-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-25 09:58:12.000000 beets_gdplaylists-0.2.6/setup.py
```

### Comparing `beets_gdplaylists-0.2.5/.github/workflows/createrelease.yml` & `beets_gdplaylists-0.2.6/.github/workflows/createrelease.yml`

 * *Files 5% similar despite different names*

```diff
@@ -24,14 +24,16 @@
         run: |
           raw=$(git branch -r --contains ${{ github.ref }})
           branch="$(echo ${raw//origin\//} | tr -d '\n')"
           echo "{name}=branch" >> $GITHUB_OUTPUT
           echo "Branches where this tag exists : $branch."
 
   create-release:
+    permissions:
+      contents: write
     runs-on: ubuntu-latest
     needs: check-current-branch
     if: contains(${{ needs.check.outputs.branch }}, 'main')`
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python
         uses: actions/setup-python@v4
```

### Comparing `beets_gdplaylists-0.2.5/.github/workflows/pythonpublish.yml` & `beets_gdplaylists-0.2.6/.github/workflows/pythonpublish.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.5/.github/workflows/testpythonpublish.yml` & `beets_gdplaylists-0.2.6/.github/workflows/testpythonpublish.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.5/LICENSE` & `beets_gdplaylists-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.5/PKG-INFO` & `beets_gdplaylists-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beets-gdplaylists
-Version: 0.2.5
+Version: 0.2.6
 Summary: beets plugin to create Grateful Dead playlists
 Author-email: Ross Hendry <rhendry@gmail.com>
 Project-URL: Repository, https://github.com/chooban/beets-gogd
 Keywords: beets,grateful dead,plex,playlists
 Platform: ALL
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `beets_gdplaylists-0.2.5/beets_gdplaylists.egg-info/PKG-INFO` & `beets_gdplaylists-0.2.6/beets_gdplaylists.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beets-gdplaylists
-Version: 0.2.5
+Version: 0.2.6
 Summary: beets plugin to create Grateful Dead playlists
 Author-email: Ross Hendry <rhendry@gmail.com>
 Project-URL: Repository, https://github.com/chooban/beets-gogd
 Keywords: beets,grateful dead,plex,playlists
 Platform: ALL
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `beets_gdplaylists-0.2.5/beets_gdplaylists.egg-info/SOURCES.txt` & `beets_gdplaylists-0.2.6/beets_gdplaylists.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.5/beetsplug/gdplaylists/__pycache__/gdplex.cpython-310.pyc` & `beets_gdplaylists-0.2.6/beetsplug/gdplaylists/__pycache__/gdplex.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.5/beetsplug/gdplaylists/gdplex.py` & `beets_gdplaylists-0.2.6/beetsplug/gdplaylists/gdplex.py`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1969-11-02.yml` & `beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1969-11-02.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1969-12-26.yml` & `beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1969-12-26.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1970-01-02.yml` & `beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1970-01-02.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1970-01-03.yml` & `beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1970-01-03.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1971-10-24.yml` & `beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1971-10-24.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1971-11-20.yml` & `beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1971-11-20.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1971-12-09.yml` & `beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1971-12-09.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1971-12-10.yml` & `beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1971-12-10.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1972-09-03.yml` & `beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1972-09-03.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1972-09-09.yml` & `beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1972-09-09.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1972-09-19.yml` & `beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1972-09-19.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1972-10-17.yml` & `beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1972-10-17.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1972-10-18.yml` & `beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1972-10-18.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1972-10-19.yml` & `beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1972-10-19.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1973-03-24.yml` & `beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1973-03-24.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1973-06-22.yml` & `beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1973-06-22.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1973-06-24.yml` & `beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1973-06-24.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1973-06-26.yml` & `beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1973-06-26.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1973-09-07.yml` & `beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1973-09-07.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1973-09-08.yml` & `beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1973-09-08.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1973-10-29.yml` & `beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1973-10-29.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1973-10-30.yml` & `beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1973-10-30.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1974-02-22.yml` & `beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1974-02-22.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1974-02-23.yml` & `beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1974-02-23.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1974-05-17.yml` & `beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1974-05-17.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1974-05-19.yml` & `beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1974-05-19.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1974-05-21.yml` & `beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1974-05-21.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1974-06-22.yml` & `beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1974-06-22.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1974-06-23.yml` & `beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1974-06-23.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1977-05-03.yml` & `beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1977-05-03.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1977-05-04.yml` & `beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1977-05-04.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1977-05-26.yml` & `beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1977-05-26.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1977-10-01.yml` & `beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1977-10-01.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1977-10-02.yml` & `beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1977-10-02.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1977-10-29.yml` & `beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1977-10-29.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1978-04-15.yml` & `beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1978-04-15.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1978-04-18.yml` & `beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1978-04-18.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1978-12-31.yml` & `beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1978-12-31.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1979-12-03.yml` & `beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1979-12-03.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1979-12-04.yml` & `beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1979-12-04.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1979-12-09.yml` & `beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1979-12-09.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1983-04-15.yml` & `beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1983-04-15.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1983-04-25.yml` & `beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1983-04-25.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1983-04-26.yml` & `beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1983-04-26.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1984-04-19.yml` & `beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1984-04-19.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1984-04-20.yml` & `beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1984-04-20.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1985-04-27.yml` & `beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1985-04-27.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1985-04-28.yml` & `beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1985-04-28.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1987-03-26.yml` & `beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1987-03-26.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1987-03-27.yml` & `beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1987-03-27.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1990-06-23.yml` & `beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1990-06-23.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1990-07-18.yml` & `beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1990-07-18.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.5/beetsplug/gdplaylists/playlists/1990-07-19.yml` & `beets_gdplaylists-0.2.6/beetsplug/gdplaylists/playlists/1990-07-19.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.5/pyproject.toml` & `beets_gdplaylists-0.2.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.5/scripts/mbdl.py` & `beets_gdplaylists-0.2.6/scripts/mbdl.py`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.5/scripts/releases.yml` & `beets_gdplaylists-0.2.6/scripts/releases.yml`

 * *Files identical despite different names*

