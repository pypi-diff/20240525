# Comparing `tmp/moveread_dfy-0.1.7.tar.gz` & `tmp/moveread_dfy-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moveread_dfy-0.1.7.tar", last modified: Sat May 25 13:54:45 2024, max compression
+gzip compressed data, was "moveread_dfy-0.1.8.tar", last modified: Sat May 25 14:16:37 2024, max compression
```

## Comparing `moveread_dfy-0.1.7.tar` & `moveread_dfy-0.1.8.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 13:54:45.572825 moveread_dfy-0.1.7/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1227 2024-05-25 13:54:45.572825 moveread_dfy-0.1.7/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       50 2024-04-29 07:55:04.000000 moveread_dfy-0.1.7/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1056 2024-05-25 13:54:42.000000 moveread_dfy-0.1.7/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-25 13:54:45.572825 moveread_dfy-0.1.7/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 13:54:45.562825 moveread_dfy-0.1.7/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 13:54:45.552825 moveread_dfy-0.1.7/src/moveread/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 13:54:45.562825 moveread_dfy-0.1.7/src/moveread/dfy/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      155 2024-04-29 10:13:40.000000 moveread_dfy-0.1.7/src/moveread/dfy/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      310 2024-05-09 04:41:09.000000 moveread_dfy-0.1.7/src/moveread/dfy/__init__.pyi
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 13:54:45.562825 moveread_dfy-0.1.7/src/moveread/dfy/doer/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-07 14:51:57.000000 moveread_dfy-0.1.7/src/moveread/dfy/doer/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      132 2024-05-24 16:36:04.000000 moveread_dfy-0.1.7/src/moveread/dfy/doer/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2366 2024-05-24 18:43:15.000000 moveread_dfy-0.1.7/src/moveread/dfy/doer/_puller.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1475 2024-05-24 17:46:14.000000 moveread_dfy-0.1.7/src/moveread/dfy/doer/_pusher.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     4351 2024-05-25 13:51:00.000000 moveread_dfy-0.1.7/src/moveread/dfy/doer/cli.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1303 2024-05-24 17:46:33.000000 moveread_dfy-0.1.7/src/moveread/dfy/doer/main.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 13:54:45.562825 moveread_dfy-0.1.7/src/moveread/dfy/lib/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-25 07:39:23.000000 moveread_dfy-0.1.7/src/moveread/dfy/lib/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      304 2024-05-25 09:44:58.000000 moveread_dfy-0.1.7/src/moveread/dfy/lib/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      136 2024-05-25 08:53:17.000000 moveread_dfy-0.1.7/src/moveread/dfy/lib/misc.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 13:54:45.562825 moveread_dfy-0.1.7/src/moveread/dfy/lib/mock/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-25 09:44:41.000000 moveread_dfy-0.1.7/src/moveread/dfy/lib/mock/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      174 2024-05-25 09:45:45.000000 moveread_dfy-0.1.7/src/moveread/dfy/lib/mock/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1972 2024-05-25 09:45:27.000000 moveread_dfy-0.1.7/src/moveread/dfy/lib/mock/core.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      639 2024-05-25 09:45:13.000000 moveread_dfy-0.1.7/src/moveread/dfy/lib/mock/tournament.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2292 2024-05-25 08:55:05.000000 moveread_dfy-0.1.7/src/moveread/dfy/lib/pairings.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 13:54:45.562825 moveread_dfy-0.1.7/src/moveread/dfy/lib/queries/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-25 07:44:00.000000 moveread_dfy-0.1.7/src/moveread/dfy/lib/queries/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      314 2024-05-25 08:36:04.000000 moveread_dfy-0.1.7/src/moveread/dfy/lib/queries/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1202 2024-05-25 08:35:52.000000 moveread_dfy-0.1.7/src/moveread/dfy/lib/queries/queries.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 13:54:45.562825 moveread_dfy-0.1.7/src/moveread/dfy/lib/tokens/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-25 08:58:49.000000 moveread_dfy-0.1.7/src/moveread/dfy/lib/tokens/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       81 2024-05-25 08:59:19.000000 moveread_dfy-0.1.7/src/moveread/dfy/lib/tokens/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      606 2024-05-25 08:59:12.000000 moveread_dfy-0.1.7/src/moveread/dfy/lib/tokens/_tokens.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 13:54:45.562825 moveread_dfy-0.1.7/src/moveread/dfy/scripts/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        0 2024-04-29 12:24:37.000000 moveread_dfy-0.1.7/src/moveread/dfy/scripts/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1814 2024-05-21 09:37:53.000000 moveread_dfy-0.1.7/src/moveread/dfy/scripts/api_cli.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      482 2024-05-12 10:50:26.000000 moveread_dfy-0.1.7/src/moveread/dfy/scripts/clientgen_cli.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1745 2024-05-07 17:15:46.000000 moveread_dfy-0.1.7/src/moveread/dfy/scripts/connect_cli.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3909 2024-05-24 18:15:00.000000 moveread_dfy-0.1.7/src/moveread/dfy/scripts/doer_cli.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 13:54:45.572825 moveread_dfy-0.1.7/src/moveread/dfy/server/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-08 07:12:36.000000 moveread_dfy-0.1.7/src/moveread/dfy/server/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      112 2024-05-07 10:08:12.000000 moveread_dfy-0.1.7/src/moveread/dfy/server/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     4868 2024-05-25 09:54:24.000000 moveread_dfy-0.1.7/src/moveread/dfy/server/api.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1711 2024-05-25 09:52:00.000000 moveread_dfy-0.1.7/src/moveread/dfy/server/cli.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      573 2024-05-12 09:12:38.000000 moveread_dfy-0.1.7/src/moveread/dfy/server/main.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      922 2024-05-21 10:23:37.000000 moveread_dfy-0.1.7/src/moveread/dfy/server/pgns.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     4661 2024-05-25 09:35:02.000000 moveread_dfy-0.1.7/src/moveread/dfy/server/sdk.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2920 2024-05-25 08:56:39.000000 moveread_dfy-0.1.7/src/moveread/dfy/types.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 13:54:45.572825 moveread_dfy-0.1.7/src/moveread_dfy.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1227 2024-05-25 13:54:45.000000 moveread_dfy-0.1.7/src/moveread_dfy.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1490 2024-05-25 13:54:45.000000 moveread_dfy-0.1.7/src/moveread_dfy.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-25 13:54:45.000000 moveread_dfy-0.1.7/src/moveread_dfy.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      216 2024-05-25 13:54:45.000000 moveread_dfy-0.1.7/src/moveread_dfy.egg-info/entry_points.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      284 2024-05-25 13:54:45.000000 moveread_dfy-0.1.7/src/moveread_dfy.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-25 13:54:45.000000 moveread_dfy-0.1.7/src/moveread_dfy.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:16:37.088214 moveread_dfy-0.1.8/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1227 2024-05-25 14:16:37.088214 moveread_dfy-0.1.8/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       50 2024-04-29 07:55:04.000000 moveread_dfy-0.1.8/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1056 2024-05-25 14:16:33.000000 moveread_dfy-0.1.8/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-25 14:16:37.088214 moveread_dfy-0.1.8/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:16:37.058216 moveread_dfy-0.1.8/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:16:37.048216 moveread_dfy-0.1.8/src/moveread/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:16:37.058216 moveread_dfy-0.1.8/src/moveread/dfy/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      155 2024-04-29 10:13:40.000000 moveread_dfy-0.1.8/src/moveread/dfy/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      310 2024-05-09 04:41:09.000000 moveread_dfy-0.1.8/src/moveread/dfy/__init__.pyi
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:16:37.068215 moveread_dfy-0.1.8/src/moveread/dfy/doer/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-07 14:51:57.000000 moveread_dfy-0.1.8/src/moveread/dfy/doer/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      132 2024-05-24 16:36:04.000000 moveread_dfy-0.1.8/src/moveread/dfy/doer/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2366 2024-05-24 18:43:15.000000 moveread_dfy-0.1.8/src/moveread/dfy/doer/_puller.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1475 2024-05-24 17:46:14.000000 moveread_dfy-0.1.8/src/moveread/dfy/doer/_pusher.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     4768 2024-05-25 14:16:09.000000 moveread_dfy-0.1.8/src/moveread/dfy/doer/cli.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1303 2024-05-24 17:46:33.000000 moveread_dfy-0.1.8/src/moveread/dfy/doer/main.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:16:37.068215 moveread_dfy-0.1.8/src/moveread/dfy/lib/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-25 07:39:23.000000 moveread_dfy-0.1.8/src/moveread/dfy/lib/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      304 2024-05-25 09:44:58.000000 moveread_dfy-0.1.8/src/moveread/dfy/lib/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      136 2024-05-25 08:53:17.000000 moveread_dfy-0.1.8/src/moveread/dfy/lib/misc.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:16:37.068215 moveread_dfy-0.1.8/src/moveread/dfy/lib/mock/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-25 09:44:41.000000 moveread_dfy-0.1.8/src/moveread/dfy/lib/mock/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      174 2024-05-25 09:45:45.000000 moveread_dfy-0.1.8/src/moveread/dfy/lib/mock/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1972 2024-05-25 09:45:27.000000 moveread_dfy-0.1.8/src/moveread/dfy/lib/mock/core.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      639 2024-05-25 09:45:13.000000 moveread_dfy-0.1.8/src/moveread/dfy/lib/mock/tournament.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2292 2024-05-25 08:55:05.000000 moveread_dfy-0.1.8/src/moveread/dfy/lib/pairings.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:16:37.068215 moveread_dfy-0.1.8/src/moveread/dfy/lib/queries/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-25 07:44:00.000000 moveread_dfy-0.1.8/src/moveread/dfy/lib/queries/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      314 2024-05-25 08:36:04.000000 moveread_dfy-0.1.8/src/moveread/dfy/lib/queries/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1202 2024-05-25 08:35:52.000000 moveread_dfy-0.1.8/src/moveread/dfy/lib/queries/queries.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:16:37.078215 moveread_dfy-0.1.8/src/moveread/dfy/lib/tokens/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-25 08:58:49.000000 moveread_dfy-0.1.8/src/moveread/dfy/lib/tokens/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       81 2024-05-25 08:59:19.000000 moveread_dfy-0.1.8/src/moveread/dfy/lib/tokens/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      606 2024-05-25 08:59:12.000000 moveread_dfy-0.1.8/src/moveread/dfy/lib/tokens/_tokens.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:16:37.078215 moveread_dfy-0.1.8/src/moveread/dfy/scripts/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        0 2024-04-29 12:24:37.000000 moveread_dfy-0.1.8/src/moveread/dfy/scripts/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1814 2024-05-21 09:37:53.000000 moveread_dfy-0.1.8/src/moveread/dfy/scripts/api_cli.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      482 2024-05-12 10:50:26.000000 moveread_dfy-0.1.8/src/moveread/dfy/scripts/clientgen_cli.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1745 2024-05-07 17:15:46.000000 moveread_dfy-0.1.8/src/moveread/dfy/scripts/connect_cli.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3909 2024-05-24 18:15:00.000000 moveread_dfy-0.1.8/src/moveread/dfy/scripts/doer_cli.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:16:37.078215 moveread_dfy-0.1.8/src/moveread/dfy/server/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-08 07:12:36.000000 moveread_dfy-0.1.8/src/moveread/dfy/server/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      112 2024-05-07 10:08:12.000000 moveread_dfy-0.1.8/src/moveread/dfy/server/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     4868 2024-05-25 09:54:24.000000 moveread_dfy-0.1.8/src/moveread/dfy/server/api.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1711 2024-05-25 09:52:00.000000 moveread_dfy-0.1.8/src/moveread/dfy/server/cli.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      573 2024-05-12 09:12:38.000000 moveread_dfy-0.1.8/src/moveread/dfy/server/main.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      922 2024-05-21 10:23:37.000000 moveread_dfy-0.1.8/src/moveread/dfy/server/pgns.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     4661 2024-05-25 09:35:02.000000 moveread_dfy-0.1.8/src/moveread/dfy/server/sdk.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2920 2024-05-25 08:56:39.000000 moveread_dfy-0.1.8/src/moveread/dfy/types.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:16:37.088214 moveread_dfy-0.1.8/src/moveread_dfy.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1227 2024-05-25 14:16:37.000000 moveread_dfy-0.1.8/src/moveread_dfy.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1490 2024-05-25 14:16:37.000000 moveread_dfy-0.1.8/src/moveread_dfy.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-25 14:16:37.000000 moveread_dfy-0.1.8/src/moveread_dfy.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      216 2024-05-25 14:16:37.000000 moveread_dfy-0.1.8/src/moveread_dfy.egg-info/entry_points.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      284 2024-05-25 14:16:37.000000 moveread_dfy-0.1.8/src/moveread_dfy.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-25 14:16:37.000000 moveread_dfy-0.1.8/src/moveread_dfy.egg-info/top_level.txt
```

### Comparing `moveread_dfy-0.1.7/PKG-INFO` & `moveread_dfy-0.1.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moveread-dfy
-Version: 0.1.7
+Version: 0.1.8
 Summary: Moveread DFY data models and API
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/moveread-dfy.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: lazy-loader
 Requires-Dist: pydantic
```

### Comparing `moveread_dfy-0.1.7/pyproject.toml` & `moveread_dfy-0.1.8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "moveread-dfy"
-version = "0.1.7"
+version = "0.1.8"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Moveread DFY data models and API"
 dependencies = [
   "lazy-loader", "pydantic",
   "chess-pairings", "dslog",
```

### Comparing `moveread_dfy-0.1.7/src/moveread/dfy/doer/_puller.py` & `moveread_dfy-0.1.8/src/moveread/dfy/doer/_puller.py`

 * *Files identical despite different names*

### Comparing `moveread_dfy-0.1.7/src/moveread/dfy/doer/_pusher.py` & `moveread_dfy-0.1.8/src/moveread/dfy/doer/_pusher.py`

 * *Files identical despite different names*

### Comparing `moveread_dfy-0.1.7/src/moveread/dfy/doer/cli.py` & `moveread_dfy-0.1.8/src/moveread/dfy/doer/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from argparse import ArgumentParser
 import os
 
-def env(variable: str) -> dict:
-  if (value := os.getenv(variable)) is not None:
+def env(variable: str, *, default = None, required: bool = True) -> dict:
+  if (value := os.getenv(variable, default)) is not None:
     return dict(default=value)
-  return dict(required=True)
+  return dict(required=required)
 
 def main():
   parser = ArgumentParser()
   parser.add_argument('--dfy-db', **env('DFY_DB'), help='Database URL')
-  parser.add_argument('--dfy-images', type=str, help='KV conn str to DFY images')
+  parser.add_argument('--dfy-images', **env('DFY_IMAGES'), type=str, help='KV conn str to DFY images')
   parser.add_argument('--doer-db', **env('DOER_DB'), help='Internal database URL, for queues and stuff')
   parser.add_argument('--doer-images', **env('DOER_IMAGES'), type=str, help='KV conn str to doer images')
   parser.add_argument('--core-games', **env('CORE_GAMES'), type=str, help='KV conn str to output Core games')
   parser.add_argument('--core-blobs', **env('CORE_BLOBS'), type=str, help='KV conn str to output Core blobs')
+  parser.add_argument('--tf-host', **env('TF_HOST', required=False), type=str)
+  parser.add_argument('--tf-port', **env('TF_PORT', required=False), type=str)
 
   parser.add_argument('-p', '--port', default=8000, type=int)
   parser.add_argument('--host', default='0.0.0.0', type=str)
 
   args = parser.parse_args()
 
   from dslog import Logger
@@ -43,14 +45,15 @@
   from multiprocessing import Process
   import uvicorn
   from sqlmodel import create_engine
   from kv.api import KV
   from kv.fs import FilesystemKV
   from kv.sql import SQLKV
   from q.kv import QueueKV
+  import tf.serving as tfs
   from moveread.core import CoreAPI
   import moveread.pipelines.preprocess as pre
   from moveread.pipelines.game_preprocess import Game
   from moveread.pipelines.dfy import Workflow, Result
   from moveread.dfy.doer.main import artifacts
   
   online_engine = create_engine(dfy_db)
@@ -68,22 +71,27 @@
   local_images = KV.of(doer_images)
   if isinstance(local_images, FilesystemKV):
     images_path = local_images.base_path
   else:
     images_path = None
 
   core = CoreAPI.of(core_games, core_blobs)
+
+  tfserving = tfs.Params()
+  if args.tf_host: tfserving['host'] = args.tf_host
+  if args.tf_port: tfserving['port'] = args.tf_port
   
   artifs = artifacts(Qout=Qout, **queues)(
     online_images=online_images,
     images=local_images, images_path=images_path,
     games=SQLKV(Game, engine, 'games'),
     imgGameIds=SQLKV(str, engine, 'game-ids'),
     received_imgs=SQLKV(dict[str, pre.Result], engine, 'received-imgs'),
     engine=online_engine, output_core=core,
+    tfserving=tfserving
   )
 
   ps = {
     id: Process(target=asyncio.run, args=(f,)) for id, f in artifs.processes.items()
   } | {
     'api': Process(target=uvicorn.run, args=(artifs.api,), kwargs={'host': args.host, 'port': args.port})
   }
```

### Comparing `moveread_dfy-0.1.7/src/moveread/dfy/doer/main.py` & `moveread_dfy-0.1.8/src/moveread/dfy/doer/main.py`

 * *Files identical despite different names*

### Comparing `moveread_dfy-0.1.7/src/moveread/dfy/lib/mock/core.py` & `moveread_dfy-0.1.8/src/moveread/dfy/lib/mock/core.py`

 * *Files identical despite different names*

### Comparing `moveread_dfy-0.1.7/src/moveread/dfy/lib/mock/tournament.py` & `moveread_dfy-0.1.8/src/moveread/dfy/lib/mock/tournament.py`

 * *Files identical despite different names*

### Comparing `moveread_dfy-0.1.7/src/moveread/dfy/lib/pairings.py` & `moveread_dfy-0.1.8/src/moveread/dfy/lib/pairings.py`

 * *Files identical despite different names*

### Comparing `moveread_dfy-0.1.7/src/moveread/dfy/lib/queries/queries.py` & `moveread_dfy-0.1.8/src/moveread/dfy/lib/queries/queries.py`

 * *Files identical despite different names*

### Comparing `moveread_dfy-0.1.7/src/moveread/dfy/lib/tokens/_tokens.py` & `moveread_dfy-0.1.8/src/moveread/dfy/lib/tokens/_tokens.py`

 * *Files identical despite different names*

### Comparing `moveread_dfy-0.1.7/src/moveread/dfy/scripts/api_cli.py` & `moveread_dfy-0.1.8/src/moveread/dfy/scripts/api_cli.py`

 * *Files identical despite different names*

### Comparing `moveread_dfy-0.1.7/src/moveread/dfy/scripts/connect_cli.py` & `moveread_dfy-0.1.8/src/moveread/dfy/scripts/connect_cli.py`

 * *Files identical despite different names*

### Comparing `moveread_dfy-0.1.7/src/moveread/dfy/scripts/doer_cli.py` & `moveread_dfy-0.1.8/src/moveread/dfy/scripts/doer_cli.py`

 * *Files identical despite different names*

### Comparing `moveread_dfy-0.1.7/src/moveread/dfy/server/api.py` & `moveread_dfy-0.1.8/src/moveread/dfy/server/api.py`

 * *Files identical despite different names*

### Comparing `moveread_dfy-0.1.7/src/moveread/dfy/server/cli.py` & `moveread_dfy-0.1.8/src/moveread/dfy/server/cli.py`

 * *Files identical despite different names*

### Comparing `moveread_dfy-0.1.7/src/moveread/dfy/server/main.py` & `moveread_dfy-0.1.8/src/moveread/dfy/server/main.py`

 * *Files identical despite different names*

### Comparing `moveread_dfy-0.1.7/src/moveread/dfy/server/pgns.py` & `moveread_dfy-0.1.8/src/moveread/dfy/server/pgns.py`

 * *Files identical despite different names*

### Comparing `moveread_dfy-0.1.7/src/moveread/dfy/server/sdk.py` & `moveread_dfy-0.1.8/src/moveread/dfy/server/sdk.py`

 * *Files identical despite different names*

### Comparing `moveread_dfy-0.1.7/src/moveread/dfy/types.py` & `moveread_dfy-0.1.8/src/moveread/dfy/types.py`

 * *Files identical despite different names*

### Comparing `moveread_dfy-0.1.7/src/moveread_dfy.egg-info/PKG-INFO` & `moveread_dfy-0.1.8/src/moveread_dfy.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moveread-dfy
-Version: 0.1.7
+Version: 0.1.8
 Summary: Moveread DFY data models and API
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/moveread-dfy.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: lazy-loader
 Requires-Dist: pydantic
```

### Comparing `moveread_dfy-0.1.7/src/moveread_dfy.egg-info/SOURCES.txt` & `moveread_dfy-0.1.8/src/moveread_dfy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

