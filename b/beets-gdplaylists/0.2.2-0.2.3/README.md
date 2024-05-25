# Comparing `tmp/beets_gdplaylists-0.2.2.tar.gz` & `tmp/beets_gdplaylists-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beets_gdplaylists-0.2.2.tar", last modified: Thu May 23 21:01:12 2024, max compression
+gzip compressed data, was "beets_gdplaylists-0.2.3.tar", last modified: Fri May 24 21:12:59 2024, max compression
```

## Comparing `beets_gdplaylists-0.2.2.tar` & `beets_gdplaylists-0.2.3.tar`

### file list

```diff
@@ -1,64 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:01:12.310676 beets_gdplaylists-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-23 21:01:03.000000 beets_gdplaylists-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-23 21:01:03.000000 beets_gdplaylists-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-23 21:01:12.310676 beets_gdplaylists-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-23 21:01:03.000000 beets_gdplaylists-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:01:12.310676 beets_gdplaylists-0.2.2/beets_gdplaylists.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-23 21:01:12.000000 beets_gdplaylists-0.2.2/beets_gdplaylists.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-05-23 21:01:12.000000 beets_gdplaylists-0.2.2/beets_gdplaylists.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 21:01:12.000000 beets_gdplaylists-0.2.2/beets_gdplaylists.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-23 21:01:12.000000 beets_gdplaylists-0.2.2/beets_gdplaylists.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-23 21:01:12.000000 beets_gdplaylists-0.2.2/beets_gdplaylists.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:01:12.298676 beets_gdplaylists-0.2.2/beetsplug/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:01:12.302676 beets_gdplaylists-0.2.2/beetsplug/gdplaylists/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-23 21:01:03.000000 beets_gdplaylists-0.2.2/beetsplug/gdplaylists/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5668 2024-05-23 21:01:03.000000 beets_gdplaylists-0.2.2/beetsplug/gdplaylists/gdplex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:01:12.310676 beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/
--rw-r--r--   0 runner    (1001) docker     (127)     3947 2024-05-23 21:01:03.000000 beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1969-11-02.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5072 2024-05-23 21:01:03.000000 beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1969-12-26.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-05-23 21:01:03.000000 beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1971-10-24.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6452 2024-05-23 21:01:03.000000 beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1971-11-20.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5230 2024-05-23 21:01:03.000000 beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1971-12-09.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6940 2024-05-23 21:01:03.000000 beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1971-12-10.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-05-23 21:01:03.000000 beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1972-09-03.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6383 2024-05-23 21:01:03.000000 beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1972-09-09.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-23 21:01:03.000000 beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1972-09-19.yml
--rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-05-23 21:01:03.000000 beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1972-10-17.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5931 2024-05-23 21:01:03.000000 beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1972-10-18.yml
--rw-r--r--   0 runner    (1001) docker     (127)     7206 2024-05-23 21:01:03.000000 beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1972-10-19.yml
--rw-r--r--   0 runner    (1001) docker     (127)     7631 2024-05-23 21:01:03.000000 beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1973-06-22.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6930 2024-05-23 21:01:03.000000 beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1973-06-24.yml
--rw-r--r--   0 runner    (1001) docker     (127)     7671 2024-05-23 21:01:03.000000 beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1973-06-26.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-05-23 21:01:03.000000 beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1973-09-07.yml
--rw-r--r--   0 runner    (1001) docker     (127)     7582 2024-05-23 21:01:03.000000 beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1973-09-08.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6231 2024-05-23 21:01:03.000000 beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1973-10-29.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5527 2024-05-23 21:01:03.000000 beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1973-10-30.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2823 2024-05-23 21:01:03.000000 beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1974-02-22.yml
--rw-r--r--   0 runner    (1001) docker     (127)     7584 2024-05-23 21:01:03.000000 beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1974-02-23.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6677 2024-05-23 21:01:03.000000 beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1974-05-17.yml
--rw-r--r--   0 runner    (1001) docker     (127)     7755 2024-05-23 21:01:03.000000 beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1974-05-19.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5905 2024-05-23 21:01:03.000000 beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1974-05-21.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6189 2024-05-23 21:01:03.000000 beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1977-05-03.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-05-23 21:01:03.000000 beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1977-05-04.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5919 2024-05-23 21:01:03.000000 beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1977-05-26.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5927 2024-05-23 21:01:03.000000 beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1977-10-01.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-05-23 21:01:03.000000 beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1977-10-02.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4914 2024-05-23 21:01:03.000000 beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1978-04-15.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-05-23 21:01:03.000000 beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1978-04-18.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-23 21:01:03.000000 beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1979-12-04.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6704 2024-05-23 21:01:03.000000 beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1979-12-09.yml
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-23 21:01:03.000000 beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1983-04-15.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-05-23 21:01:03.000000 beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1983-04-25.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-05-23 21:01:03.000000 beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1983-04-26.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-05-23 21:01:03.000000 beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1984-04-19.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5551 2024-05-23 21:01:03.000000 beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1984-04-20.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6329 2024-05-23 21:01:03.000000 beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1985-04-27.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-05-23 21:01:03.000000 beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1985-04-28.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5896 2024-05-23 21:01:03.000000 beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1987-03-26.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5348 2024-05-23 21:01:03.000000 beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1987-03-27.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5503 2024-05-23 21:01:03.000000 beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1990-06-23.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5888 2024-05-23 21:01:03.000000 beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1990-07-18.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5277 2024-05-23 21:01:03.000000 beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1990-07-19.yml
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-23 21:01:03.000000 beets_gdplaylists-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 21:01:12.310676 beets_gdplaylists-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-23 21:01:03.000000 beets_gdplaylists-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 21:12:59.851270 beets_gdplaylists-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-24 21:12:59.851270 beets_gdplaylists-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 21:12:59.851270 beets_gdplaylists-0.2.3/beets_gdplaylists.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-24 21:12:59.000000 beets_gdplaylists-0.2.3/beets_gdplaylists.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-24 21:12:59.000000 beets_gdplaylists-0.2.3/beets_gdplaylists.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 21:12:59.000000 beets_gdplaylists-0.2.3/beets_gdplaylists.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-24 21:12:59.000000 beets_gdplaylists-0.2.3/beets_gdplaylists.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-24 21:12:59.000000 beets_gdplaylists-0.2.3/beets_gdplaylists.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 21:12:59.839270 beets_gdplaylists-0.2.3/beetsplug/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 21:12:59.839270 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5668 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/gdplex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 21:12:59.851270 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/
+-rw-r--r--   0 runner    (1001) docker     (127)     3947 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1969-11-02.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5072 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1969-12-26.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5532 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1970-01-02.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3979 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1970-01-03.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1971-10-24.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6452 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1971-11-20.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5230 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1971-12-09.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6940 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1971-12-10.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1972-09-03.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6383 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1972-09-09.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1972-09-19.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1972-10-17.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5931 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1972-10-18.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     7206 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1972-10-19.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     8404 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1973-03-24.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     7631 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1973-06-22.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6930 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1973-06-24.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     7671 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1973-06-26.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1973-09-07.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     7582 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1973-09-08.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6231 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1973-10-29.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5527 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1973-10-30.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2823 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1974-02-22.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     7584 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1974-02-23.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6677 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1974-05-17.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     7755 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1974-05-19.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5905 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1974-05-21.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1974-06-22.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6606 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1974-06-23.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6189 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1977-05-03.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1977-05-04.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5919 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1977-05-26.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5927 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1977-10-01.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1977-10-02.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6257 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1977-10-29.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4914 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1978-04-15.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1978-04-18.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6355 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1978-12-31.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6063 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1979-12-03.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1979-12-04.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6704 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1979-12-09.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1983-04-15.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1983-04-25.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1983-04-26.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1984-04-19.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5551 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1984-04-20.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6329 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1985-04-27.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1985-04-28.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5896 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1987-03-26.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5348 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1987-03-27.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5503 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1990-06-23.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5888 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1990-07-18.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5277 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1990-07-19.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 21:12:59.851270 beets_gdplaylists-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-24 21:12:51.000000 beets_gdplaylists-0.2.3/setup.py
```

### Comparing `beets_gdplaylists-0.2.2/LICENSE` & `beets_gdplaylists-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.2/PKG-INFO` & `beets_gdplaylists-0.2.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beets-gdplaylists
-Version: 0.2.2
+Version: 0.2.3
 Summary: beets plugin to create Grateful Dead playlists
 Author-email: Ross Hendry <rhendry@gmail.com>
 Project-URL: Repository, https://github.com/chooban/beets-gogd
 Keywords: beets,grateful dead,plex,playlists
 Platform: ALL
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `beets_gdplaylists-0.2.2/beets_gdplaylists.egg-info/PKG-INFO` & `beets_gdplaylists-0.2.3/beets_gdplaylists.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beets-gdplaylists
-Version: 0.2.2
+Version: 0.2.3
 Summary: beets plugin to create Grateful Dead playlists
 Author-email: Ross Hendry <rhendry@gmail.com>
 Project-URL: Repository, https://github.com/chooban/beets-gogd
 Keywords: beets,grateful dead,plex,playlists
 Platform: ALL
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `beets_gdplaylists-0.2.2/beets_gdplaylists.egg-info/SOURCES.txt` & `beets_gdplaylists-0.2.3/beets_gdplaylists.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -8,43 +8,51 @@
 beets_gdplaylists.egg-info/dependency_links.txt
 beets_gdplaylists.egg-info/requires.txt
 beets_gdplaylists.egg-info/top_level.txt
 beetsplug/gdplaylists/__init__.py
 beetsplug/gdplaylists/gdplex.py
 beetsplug/gdplaylists/playlists/1969-11-02.yml
 beetsplug/gdplaylists/playlists/1969-12-26.yml
+beetsplug/gdplaylists/playlists/1970-01-02.yml
+beetsplug/gdplaylists/playlists/1970-01-03.yml
 beetsplug/gdplaylists/playlists/1971-10-24.yml
 beetsplug/gdplaylists/playlists/1971-11-20.yml
 beetsplug/gdplaylists/playlists/1971-12-09.yml
 beetsplug/gdplaylists/playlists/1971-12-10.yml
 beetsplug/gdplaylists/playlists/1972-09-03.yml
 beetsplug/gdplaylists/playlists/1972-09-09.yml
 beetsplug/gdplaylists/playlists/1972-09-19.yml
 beetsplug/gdplaylists/playlists/1972-10-17.yml
 beetsplug/gdplaylists/playlists/1972-10-18.yml
 beetsplug/gdplaylists/playlists/1972-10-19.yml
+beetsplug/gdplaylists/playlists/1973-03-24.yml
 beetsplug/gdplaylists/playlists/1973-06-22.yml
 beetsplug/gdplaylists/playlists/1973-06-24.yml
 beetsplug/gdplaylists/playlists/1973-06-26.yml
 beetsplug/gdplaylists/playlists/1973-09-07.yml
 beetsplug/gdplaylists/playlists/1973-09-08.yml
 beetsplug/gdplaylists/playlists/1973-10-29.yml
 beetsplug/gdplaylists/playlists/1973-10-30.yml
 beetsplug/gdplaylists/playlists/1974-02-22.yml
 beetsplug/gdplaylists/playlists/1974-02-23.yml
 beetsplug/gdplaylists/playlists/1974-05-17.yml
 beetsplug/gdplaylists/playlists/1974-05-19.yml
 beetsplug/gdplaylists/playlists/1974-05-21.yml
+beetsplug/gdplaylists/playlists/1974-06-22.yml
+beetsplug/gdplaylists/playlists/1974-06-23.yml
 beetsplug/gdplaylists/playlists/1977-05-03.yml
 beetsplug/gdplaylists/playlists/1977-05-04.yml
 beetsplug/gdplaylists/playlists/1977-05-26.yml
 beetsplug/gdplaylists/playlists/1977-10-01.yml
 beetsplug/gdplaylists/playlists/1977-10-02.yml
+beetsplug/gdplaylists/playlists/1977-10-29.yml
 beetsplug/gdplaylists/playlists/1978-04-15.yml
 beetsplug/gdplaylists/playlists/1978-04-18.yml
+beetsplug/gdplaylists/playlists/1978-12-31.yml
+beetsplug/gdplaylists/playlists/1979-12-03.yml
 beetsplug/gdplaylists/playlists/1979-12-04.yml
 beetsplug/gdplaylists/playlists/1979-12-09.yml
 beetsplug/gdplaylists/playlists/1983-04-15.yml
 beetsplug/gdplaylists/playlists/1983-04-25.yml
 beetsplug/gdplaylists/playlists/1983-04-26.yml
 beetsplug/gdplaylists/playlists/1984-04-19.yml
 beetsplug/gdplaylists/playlists/1984-04-20.yml
```

### Comparing `beets_gdplaylists-0.2.2/beetsplug/gdplaylists/gdplex.py` & `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/gdplex.py`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1969-11-02.yml` & `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1969-11-02.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1969-12-26.yml` & `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1969-12-26.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1971-10-24.yml` & `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1971-10-24.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1971-11-20.yml` & `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1971-11-20.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1971-12-09.yml` & `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1971-12-09.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1971-12-10.yml` & `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1971-12-10.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1972-09-03.yml` & `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1972-09-03.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1972-09-09.yml` & `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1972-09-09.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1972-09-19.yml` & `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1972-09-19.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1972-10-17.yml` & `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1972-10-17.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1972-10-18.yml` & `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1972-10-18.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1972-10-19.yml` & `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1972-10-19.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1973-06-22.yml` & `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1973-06-22.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1973-06-24.yml` & `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1973-06-24.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1973-06-26.yml` & `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1973-06-26.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1973-09-07.yml` & `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1973-09-07.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1973-09-08.yml` & `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1973-09-08.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1973-10-29.yml` & `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1973-10-29.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1973-10-30.yml` & `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1973-10-30.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1974-02-22.yml` & `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1974-02-22.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1974-02-23.yml` & `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1974-02-23.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1974-05-17.yml` & `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1974-05-17.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1974-05-19.yml` & `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1974-05-19.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1974-05-21.yml` & `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1974-05-21.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1977-05-03.yml` & `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1977-05-03.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1977-05-04.yml` & `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1977-05-04.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1977-05-26.yml` & `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1977-05-26.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1977-10-01.yml` & `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1977-10-01.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1977-10-02.yml` & `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1977-10-02.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1978-04-15.yml` & `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1978-04-15.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1978-04-18.yml` & `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1978-04-18.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1979-12-09.yml` & `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1979-12-09.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1983-04-15.yml` & `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1983-04-15.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1983-04-25.yml` & `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1983-04-25.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1983-04-26.yml` & `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1983-04-26.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1984-04-19.yml` & `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1984-04-19.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1984-04-20.yml` & `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1984-04-20.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1985-04-27.yml` & `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1985-04-27.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1985-04-28.yml` & `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1985-04-28.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1987-03-26.yml` & `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1987-03-26.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1987-03-27.yml` & `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1987-03-27.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1990-06-23.yml` & `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1990-06-23.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1990-07-18.yml` & `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1990-07-18.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.2/beetsplug/gdplaylists/playlists/1990-07-19.yml` & `beets_gdplaylists-0.2.3/beetsplug/gdplaylists/playlists/1990-07-19.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.2/pyproject.toml` & `beets_gdplaylists-0.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name="beets-gdplaylists"
-version="0.2.2"
+version="0.2.3"
 dynamic=["dependencies"]
 description="beets plugin to create Grateful Dead playlists"
 readme="README.md"
 authors=[{name="Ross Hendry", email="rhendry@gmail.com"}]
 keywords=["beets", "grateful dead", "plex", "playlists"]
 classifiers=[
   'Topic :: Multimedia :: Sound/Audio',
```

