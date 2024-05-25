# Comparing `tmp/beets_gdplaylists-0.2.3.tar.gz` & `tmp/beets_gdplaylists-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beets_gdplaylists-0.2.3.tar", last modified: Fri May 24 21:12:59 2024, max compression
+gzip compressed data, was "beets_gdplaylists-0.2.4.tar", last modified: Sat May 25 09:38:38 2024, max compression
```

## Comparing `beets_gdplaylists-0.2.3.tar` & `beets_gdplaylists-0.2.4.tar`

### file list

```diff
@@ -1,72 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 21:12:59.851270 beets_gdplaylists-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-24 21:12:59.851270 beets_gdplaylists-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 21:12:59.851270 beets_gdplaylists-0.2.3/beets_gdplaylists.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-24 21:12:59.000000 beets_gdplaylists-0.2.3/beets_gdplaylists.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-24 21:12:59.000000 beets_gdplaylists-0.2.3/beets_gdplaylists.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 21:12:59.000000 beets_gdplaylists-0.2.3/beets_gdplaylists.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-24 21:12:59.000000 beets_gdplaylists-0.2.3/beets_gdplaylists.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-24 21:12:59.000000 beets_gdplaylists-0.2.3/beets_gdplaylists.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 21:12:59.839270 beets_gdplaylists-0.2.3/beetsplug/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 21:12:59.839270 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5668 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/gdplex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 21:12:59.851270 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/
--rw-r--r--   0 runner    (1001) docker     (127)     3947 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1969-11-02.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5072 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1969-12-26.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5532 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1970-01-02.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3979 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1970-01-03.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1971-10-24.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6452 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1971-11-20.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5230 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1971-12-09.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6940 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1971-12-10.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1972-09-03.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6383 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1972-09-09.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1972-09-19.yml
--rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1972-10-17.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5931 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1972-10-18.yml
--rw-r--r--   0 runner    (1001) docker     (127)     7206 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1972-10-19.yml
--rw-r--r--   0 runner    (1001) docker     (127)     8404 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1973-03-24.yml
--rw-r--r--   0 runner    (1001) docker     (127)     7631 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1973-06-22.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6930 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1973-06-24.yml
--rw-r--r--   0 runner    (1001) docker     (127)     7671 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1973-06-26.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1973-09-07.yml
--rw-r--r--   0 runner    (1001) docker     (127)     7582 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1973-09-08.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6231 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1973-10-29.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5527 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1973-10-30.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2823 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1974-02-22.yml
--rw-r--r--   0 runner    (1001) docker     (127)     7584 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1974-02-23.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6677 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1974-05-17.yml
--rw-r--r--   0 runner    (1001) docker     (127)     7755 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1974-05-19.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5905 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1974-05-21.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1974-06-22.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6606 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1974-06-23.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6189 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1977-05-03.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1977-05-04.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5919 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1977-05-26.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5927 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1977-10-01.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1977-10-02.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6257 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1977-10-29.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4914 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1978-04-15.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1978-04-18.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6355 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1978-12-31.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6063 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1979-12-03.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1979-12-04.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6704 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1979-12-09.yml
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1983-04-15.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1983-04-25.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1983-04-26.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1984-04-19.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5551 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1984-04-20.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6329 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1985-04-27.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1985-04-28.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5896 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1987-03-26.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5348 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1987-03-27.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5503 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1990-06-23.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5888 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1990-07-18.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5277 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1990-07-19.yml
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 21:12:59.851270 beets_gdplaylists-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 09:38:38.723204 beets_gdplaylists-0.2.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 09:38:38.707204 beets_gdplaylists-0.2.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 09:38:38.707204 beets_gdplaylists-0.2.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-25 09:38:29.000000 beets_gdplaylists-0.2.4/.github/workflows/createrelease.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-25 09:38:29.000000 beets_gdplaylists-0.2.4/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-25 09:38:29.000000 beets_gdplaylists-0.2.4/.github/workflows/testpythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-25 09:38:29.000000 beets_gdplaylists-0.2.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-25 09:38:29.000000 beets_gdplaylists-0.2.4/.python-version
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-25 09:38:29.000000 beets_gdplaylists-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-25 09:38:29.000000 beets_gdplaylists-0.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-25 09:38:38.723204 beets_gdplaylists-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-25 09:38:29.000000 beets_gdplaylists-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 09:38:38.723204 beets_gdplaylists-0.2.4/beets_gdplaylists.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-25 09:38:38.000000 beets_gdplaylists-0.2.4/beets_gdplaylists.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-05-25 09:38:38.000000 beets_gdplaylists-0.2.4/beets_gdplaylists.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 09:38:38.000000 beets_gdplaylists-0.2.4/beets_gdplaylists.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-25 09:38:38.000000 beets_gdplaylists-0.2.4/beets_gdplaylists.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-25 09:38:38.000000 beets_gdplaylists-0.2.4/beets_gdplaylists.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 09:38:38.711204 beets_gdplaylists-0.2.4/beetsplug/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-25 09:38:29.000000 beets_gdplaylists-0.2.4/beetsplug/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 09:38:38.711204 beets_gdplaylists-0.2.4/beetsplug/gdplaylists/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-25 09:38:29.000000 beets_gdplaylists-0.2.4/beetsplug/gdplaylists/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 09:38:38.711204 beets_gdplaylists-0.2.4/beetsplug/gdplaylists/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-25 09:38:29.000000 beets_gdplaylists-0.2.4/beetsplug/gdplaylists/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)     5598 2024-05-25 09:38:29.000000 beets_gdplaylists-0.2.4/beetsplug/gdplaylists/__pycache__/gdplex.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)     5668 2024-05-25 09:38:29.000000 beets_gdplaylists-0.2.4/beetsplug/gdplaylists/gdplex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 09:38:38.719204 beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/
+-rw-r--r--   0 runner    (1001) docker     (127)     3947 2024-05-25 09:38:29.000000 beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1969-11-02.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5072 2024-05-25 09:38:29.000000 beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1969-12-26.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5532 2024-05-25 09:38:29.000000 beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1970-01-02.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3979 2024-05-25 09:38:29.000000 beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1970-01-03.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-05-25 09:38:29.000000 beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1971-10-24.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6452 2024-05-25 09:38:29.000000 beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1971-11-20.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5230 2024-05-25 09:38:29.000000 beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1971-12-09.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6940 2024-05-25 09:38:29.000000 beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1971-12-10.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-05-25 09:38:29.000000 beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1972-09-03.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6383 2024-05-25 09:38:29.000000 beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1972-09-09.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-25 09:38:29.000000 beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1972-09-19.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-05-25 09:38:29.000000 beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1972-10-17.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5931 2024-05-25 09:38:29.000000 beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1972-10-18.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     7206 2024-05-25 09:38:29.000000 beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1972-10-19.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     8404 2024-05-25 09:38:29.000000 beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1973-03-24.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     7631 2024-05-25 09:38:29.000000 beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1973-06-22.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6930 2024-05-25 09:38:29.000000 beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1973-06-24.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     7671 2024-05-25 09:38:29.000000 beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1973-06-26.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-05-25 09:38:29.000000 beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1973-09-07.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     7582 2024-05-25 09:38:29.000000 beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1973-09-08.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6231 2024-05-25 09:38:29.000000 beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1973-10-29.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5527 2024-05-25 09:38:29.000000 beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1973-10-30.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2823 2024-05-25 09:38:29.000000 beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1974-02-22.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     7584 2024-05-25 09:38:29.000000 beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1974-02-23.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6677 2024-05-25 09:38:29.000000 beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1974-05-17.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     7755 2024-05-25 09:38:29.000000 beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1974-05-19.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5905 2024-05-25 09:38:29.000000 beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1974-05-21.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-05-25 09:38:29.000000 beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1974-06-22.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6606 2024-05-25 09:38:29.000000 beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1974-06-23.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6189 2024-05-25 09:38:29.000000 beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1977-05-03.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-05-25 09:38:29.000000 beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1977-05-04.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5919 2024-05-25 09:38:29.000000 beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1977-05-26.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5927 2024-05-25 09:38:29.000000 beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1977-10-01.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-05-25 09:38:29.000000 beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1977-10-02.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6257 2024-05-25 09:38:29.000000 beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1977-10-29.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4914 2024-05-25 09:38:29.000000 beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1978-04-15.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-05-25 09:38:29.000000 beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1978-04-18.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6355 2024-05-25 09:38:29.000000 beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1978-12-31.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6063 2024-05-25 09:38:29.000000 beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1979-12-03.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-05-25 09:38:29.000000 beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1979-12-04.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6704 2024-05-25 09:38:29.000000 beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1979-12-09.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-25 09:38:29.000000 beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1983-04-15.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-05-25 09:38:29.000000 beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1983-04-25.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-05-25 09:38:29.000000 beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1983-04-26.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-05-25 09:38:29.000000 beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1984-04-19.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5551 2024-05-25 09:38:29.000000 beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1984-04-20.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6329 2024-05-25 09:38:29.000000 beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1985-04-27.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-05-25 09:38:29.000000 beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1985-04-28.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5896 2024-05-25 09:38:29.000000 beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1987-03-26.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5348 2024-05-25 09:38:29.000000 beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1987-03-27.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5503 2024-05-25 09:38:29.000000 beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1990-06-23.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5888 2024-05-25 09:38:29.000000 beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1990-07-18.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5277 2024-05-25 09:38:29.000000 beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1990-07-19.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-25 09:38:29.000000 beets_gdplaylists-0.2.4/justfile
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-25 09:38:29.000000 beets_gdplaylists-0.2.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 09:38:38.723204 beets_gdplaylists-0.2.4/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-05-25 09:38:29.000000 beets_gdplaylists-0.2.4/scripts/mbdl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-05-25 09:38:29.000000 beets_gdplaylists-0.2.4/scripts/releases.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 09:38:38.723204 beets_gdplaylists-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-25 09:38:29.000000 beets_gdplaylists-0.2.4/setup.py
```

### Comparing `beets_gdplaylists-0.2.3/LICENSE` & `beets_gdplaylists-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.3/PKG-INFO` & `beets_gdplaylists-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beets-gdplaylists
-Version: 0.2.3
+Version: 0.2.4
 Summary: beets plugin to create Grateful Dead playlists
 Author-email: Ross Hendry <rhendry@gmail.com>
 Project-URL: Repository, https://github.com/chooban/beets-gogd
 Keywords: beets,grateful dead,plex,playlists
 Platform: ALL
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `beets_gdplaylists-0.2.3/beets_gdplaylists.egg-info/PKG-INFO` & `beets_gdplaylists-0.2.4/beets_gdplaylists.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beets-gdplaylists
-Version: 0.2.3
+Version: 0.2.4
 Summary: beets plugin to create Grateful Dead playlists
 Author-email: Ross Hendry <rhendry@gmail.com>
 Project-URL: Repository, https://github.com/chooban/beets-gogd
 Keywords: beets,grateful dead,plex,playlists
 Platform: ALL
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `beets_gdplaylists-0.2.3/beets_gdplaylists.egg-info/SOURCES.txt` & `beets_gdplaylists-0.2.4/beets_gdplaylists.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,28 @@
+.gitignore
+.python-version
 LICENSE
 MANIFEST.in
 README.md
+justfile
 pyproject.toml
 setup.py
+.github/workflows/createrelease.yml
+.github/workflows/pythonpublish.yml
+.github/workflows/testpythonpublish.yml
 beets_gdplaylists.egg-info/PKG-INFO
 beets_gdplaylists.egg-info/SOURCES.txt
 beets_gdplaylists.egg-info/dependency_links.txt
 beets_gdplaylists.egg-info/requires.txt
 beets_gdplaylists.egg-info/top_level.txt
+beetsplug/__init__.py
 beetsplug/gdplaylists/__init__.py
 beetsplug/gdplaylists/gdplex.py
+beetsplug/gdplaylists/__pycache__/__init__.cpython-310.pyc
+beetsplug/gdplaylists/__pycache__/gdplex.cpython-310.pyc
 beetsplug/gdplaylists/playlists/1969-11-02.yml
 beetsplug/gdplaylists/playlists/1969-12-26.yml
 beetsplug/gdplaylists/playlists/1970-01-02.yml
 beetsplug/gdplaylists/playlists/1970-01-03.yml
 beetsplug/gdplaylists/playlists/1971-10-24.yml
 beetsplug/gdplaylists/playlists/1971-11-20.yml
 beetsplug/gdplaylists/playlists/1971-12-09.yml
@@ -58,8 +67,10 @@
 beetsplug/gdplaylists/playlists/1984-04-20.yml
 beetsplug/gdplaylists/playlists/1985-04-27.yml
 beetsplug/gdplaylists/playlists/1985-04-28.yml
 beetsplug/gdplaylists/playlists/1987-03-26.yml
 beetsplug/gdplaylists/playlists/1987-03-27.yml
 beetsplug/gdplaylists/playlists/1990-06-23.yml
 beetsplug/gdplaylists/playlists/1990-07-18.yml
-beetsplug/gdplaylists/playlists/1990-07-19.yml
+beetsplug/gdplaylists/playlists/1990-07-19.yml
+scripts/mbdl.py
+scripts/releases.yml
```

### Comparing `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/gdplex.py` & `beets_gdplaylists-0.2.4/beetsplug/gdplaylists/gdplex.py`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1969-11-02.yml` & `beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1969-11-02.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1969-12-26.yml` & `beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1969-12-26.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1970-01-02.yml` & `beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1970-01-02.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1970-01-03.yml` & `beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1970-01-03.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1971-10-24.yml` & `beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1971-10-24.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1971-11-20.yml` & `beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1971-11-20.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1971-12-09.yml` & `beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1971-12-09.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1971-12-10.yml` & `beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1971-12-10.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1972-09-03.yml` & `beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1972-09-03.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1972-09-09.yml` & `beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1972-09-09.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1972-09-19.yml` & `beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1972-09-19.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1972-10-17.yml` & `beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1972-10-17.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1972-10-18.yml` & `beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1972-10-18.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1972-10-19.yml` & `beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1972-10-19.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1973-03-24.yml` & `beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1973-03-24.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1973-06-22.yml` & `beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1973-06-22.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1973-06-24.yml` & `beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1973-06-24.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1973-06-26.yml` & `beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1973-06-26.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1973-09-07.yml` & `beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1973-09-07.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1973-09-08.yml` & `beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1973-09-08.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1973-10-29.yml` & `beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1973-10-29.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1973-10-30.yml` & `beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1973-10-30.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1974-02-22.yml` & `beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1974-02-22.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1974-02-23.yml` & `beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1974-02-23.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1974-05-17.yml` & `beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1974-05-17.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1974-05-19.yml` & `beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1974-05-19.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1974-05-21.yml` & `beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1974-05-21.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1974-06-22.yml` & `beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1974-06-22.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1974-06-23.yml` & `beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1974-06-23.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1977-05-03.yml` & `beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1977-05-03.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1977-05-04.yml` & `beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1977-05-04.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1977-05-26.yml` & `beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1977-05-26.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1977-10-01.yml` & `beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1977-10-01.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1977-10-02.yml` & `beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1977-10-02.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1977-10-29.yml` & `beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1977-10-29.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1978-04-15.yml` & `beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1978-04-15.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1978-04-18.yml` & `beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1978-04-18.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1978-12-31.yml` & `beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1978-12-31.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1979-12-03.yml` & `beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1979-12-03.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1979-12-04.yml` & `beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1979-12-04.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1979-12-09.yml` & `beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1979-12-09.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1983-04-15.yml` & `beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1983-04-15.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1983-04-25.yml` & `beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1983-04-25.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1983-04-26.yml` & `beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1983-04-26.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1984-04-19.yml` & `beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1984-04-19.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1984-04-20.yml` & `beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1984-04-20.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1985-04-27.yml` & `beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1985-04-27.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1985-04-28.yml` & `beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1985-04-28.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1987-03-26.yml` & `beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1987-03-26.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1987-03-27.yml` & `beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1987-03-27.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1990-06-23.yml` & `beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1990-06-23.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1990-07-18.yml` & `beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1990-07-18.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1990-07-19.yml` & `beets_gdplaylists-0.2.4/beetsplug/gdplaylists/playlists/1990-07-19.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.3/pyproject.toml` & `beets_gdplaylists-0.2.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
-requires = ["setuptools >= 61.0"]
+requires = ["setuptools >= 61.0", "setuptools_scm>=8"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name="beets-gdplaylists"
-version="0.2.3"
-dynamic=["dependencies"]
+# version="0.2.3"
+dynamic=["dependencies", "version"]
 description="beets plugin to create Grateful Dead playlists"
 readme="README.md"
 authors=[{name="Ross Hendry", email="rhendry@gmail.com"}]
 keywords=["beets", "grateful dead", "plex", "playlists"]
 classifiers=[
   'Topic :: Multimedia :: Sound/Audio',
   'License :: OSI Approved :: MIT License',
@@ -23,7 +23,10 @@
 ]
 
 [project.urls]
 Repository="https://github.com/chooban/beets-gogd"
 
 [tool.setuptools]
 include-package-data=true
+
+[tool.setuptools_scm]
+# version = {attr = "beets-gdplaylists.VERSION"}
```

