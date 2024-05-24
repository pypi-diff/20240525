# Comparing `tmp/hikari_arc-1.3.1.tar.gz` & `tmp/hikari_arc-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hikari_arc-1.3.1.tar", last modified: Wed May 22 19:36:47 2024, max compression
+gzip compressed data, was "hikari_arc-1.3.2.tar", last modified: Fri May 24 22:41:56 2024, max compression
```

## Comparing `hikari_arc-1.3.1.tar` & `hikari_arc-1.3.2.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:36:47.397700 hikari_arc-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-05-22 19:36:47.397700 hikari_arc-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:36:47.381700 hikari_arc-1.3.1/arc/
--rw-r--r--   0 runner    (1001) docker     (127)     6029 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:36:47.385700 hikari_arc-1.3.1/arc/abc/
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/abc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    54162 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/abc/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    28769 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/abc/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     4666 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/abc/concurrency_limiting.py
--rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/abc/error_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5486 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/abc/hookable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/abc/limiter.py
--rw-r--r--   0 runner    (1001) docker     (127)    12982 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/abc/option.py
--rw-r--r--   0 runner    (1001) docker     (127)    19703 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/abc/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)    17852 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:36:47.385700 hikari_arc-1.3.1/arc/command/
--rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5944 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/command/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:36:47.385700 hikari_arc-1.3.1/arc/command/option/
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/command/option/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/command/option/attachment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/command/option/bool.py
--rw-r--r--   0 runner    (1001) docker     (127)     3761 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/command/option/channel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:36:47.389700 hikari_arc-1.3.1/arc/command/option/custom/
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/command/option/custom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3517 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/command/option/custom/color.py
--rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/command/option/custom/member.py
--rw-r--r--   0 runner    (1001) docker     (127)     5185 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/command/option/float.py
--rw-r--r--   0 runner    (1001) docker     (127)     5135 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/command/option/int.py
--rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/command/option/mentionable.py
--rw-r--r--   0 runner    (1001) docker     (127)     2977 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/command/option/role.py
--rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/command/option/str.py
--rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/command/option/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    35485 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/command/slash.py
--rw-r--r--   0 runner    (1001) docker     (127)     5996 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/command/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:36:47.389700 hikari_arc-1.3.1/arc/context/
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/context/autocomplete.py
--rw-r--r--   0 runner    (1001) docker     (127)    39977 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/context/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6802 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/events.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:36:47.389700 hikari_arc-1.3.1/arc/ext/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/extension.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:36:47.389700 hikari_arc-1.3.1/arc/internal/
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/internal/about.py
--rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/internal/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/internal/options.py
--rw-r--r--   0 runner    (1001) docker     (127)    13518 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/internal/sigparse.py
--rw-r--r--   0 runner    (1001) docker     (127)    12589 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/internal/sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     4365 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/internal/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/internal/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4921 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/locale.py
--rw-r--r--   0 runner    (1001) docker     (127)     8624 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:36:47.389700 hikari_arc-1.3.1/arc/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12965 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/utils/concurrency_limiter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:36:47.389700 hikari_arc-1.3.1/arc/utils/hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/utils/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5894 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/utils/hooks/basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     7496 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/utils/hooks/limiters.py
--rw-r--r--   0 runner    (1001) docker     (127)    12064 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/utils/loops.py
--rw-r--r--   0 runner    (1001) docker     (127)     9477 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/utils/ratelimiter.py
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/cron_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/dev_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/doc_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:36:47.393700 hikari_arc-1.3.1/hikari_arc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-05-22 19:36:47.000000 hikari_arc-1.3.1/hikari_arc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-22 19:36:47.000000 hikari_arc-1.3.1/hikari_arc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 19:36:47.000000 hikari_arc-1.3.1/hikari_arc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 19:36:47.000000 hikari_arc-1.3.1/hikari_arc.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-22 19:36:47.000000 hikari_arc-1.3.1/hikari_arc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-22 19:36:47.000000 hikari_arc-1.3.1/hikari_arc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/rest_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 19:36:47.397700 hikari_arc-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:36:47.393700 hikari_arc-1.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/tests/test_context_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/tests/test_di.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/tests/test_inheritance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/tests/test_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     7395 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/tests/test_sigparse.py
--rw-r--r--   0 runner    (1001) docker     (127)     5785 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/tests/test_slash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:41:56.375348 hikari_arc-1.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-05-24 22:41:56.375348 hikari_arc-1.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:41:56.363348 hikari_arc-1.3.2/arc/
+-rw-r--r--   0 runner    (1001) docker     (127)     6029 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:41:56.363348 hikari_arc-1.3.2/arc/abc/
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/abc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54147 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/abc/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28769 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/abc/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4665 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/abc/concurrency_limiting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3701 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/abc/error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/abc/hookable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/abc/limiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12981 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/abc/option.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19700 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/abc/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17850 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:41:56.363348 hikari_arc-1.3.2/arc/command/
+-rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5943 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/command/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:41:56.367348 hikari_arc-1.3.2/arc/command/option/
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/command/option/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/command/option/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/command/option/bool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/command/option/channel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:41:56.367348 hikari_arc-1.3.2/arc/command/option/custom/
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/command/option/custom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/command/option/custom/color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/command/option/custom/member.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5142 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/command/option/float.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5092 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/command/option/int.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/command/option/mentionable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/command/option/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5267 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/command/option/str.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/command/option/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35491 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/command/slash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5995 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/command/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:41:56.367348 hikari_arc-1.3.2/arc/context/
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/context/autocomplete.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39976 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/context/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6802 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/events.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:41:56.367348 hikari_arc-1.3.2/arc/ext/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/extension.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:41:56.367348 hikari_arc-1.3.2/arc/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/internal/about.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/internal/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/internal/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13518 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/internal/sigparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12589 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/internal/sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4365 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/internal/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/internal/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4921 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/locale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8622 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:41:56.371348 hikari_arc-1.3.2/arc/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12959 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/utils/concurrency_limiter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:41:56.371348 hikari_arc-1.3.2/arc/utils/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/utils/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5889 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/utils/hooks/basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7490 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/utils/hooks/limiters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14009 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/utils/loops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9477 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/utils/ratelimiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/cron_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/dev_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/doc_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:41:56.371348 hikari_arc-1.3.2/hikari_arc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-05-24 22:41:56.000000 hikari_arc-1.3.2/hikari_arc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-24 22:41:56.000000 hikari_arc-1.3.2/hikari_arc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 22:41:56.000000 hikari_arc-1.3.2/hikari_arc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 22:41:56.000000 hikari_arc-1.3.2/hikari_arc.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-24 22:41:56.000000 hikari_arc-1.3.2/hikari_arc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-24 22:41:56.000000 hikari_arc-1.3.2/hikari_arc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/rest_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 22:41:56.375348 hikari_arc-1.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:41:56.371348 hikari_arc-1.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/tests/test_context_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/tests/test_di.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/tests/test_inheritance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/tests/test_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7395 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/tests/test_sigparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5785 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/tests/test_slash.py
```

### Comparing `hikari_arc-1.3.1/LICENSE` & `hikari_arc-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.1/PKG-INFO` & `hikari_arc-1.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hikari-arc
-Version: 1.3.1
+Version: 1.3.2
 Summary: A command handler for hikari with a focus on type-safety and correctness.
 Home-page: https://github.com/hypergonial/hikari-arc
 Author: hypergonial
 Author-email: git@hypergonial.com
 Maintainer: hypergonial
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
@@ -26,20 +26,20 @@
 Requires-Dist: hikari>=2.0.0.dev122
 Requires-Dist: alluka<0.4,>=0.3.0
 Requires-Dist: attrs>=23.1
 Requires-Dist: colorama; sys_platform == "win32"
 Provides-Extra: docs
 Requires-Dist: mkdocs-material[imaging]~=9.5.24; extra == "docs"
 Requires-Dist: mkdocs~=1.6.0; extra == "docs"
-Requires-Dist: mkdocstrings-python~=1.10.2; extra == "docs"
+Requires-Dist: mkdocstrings-python~=1.10.3; extra == "docs"
 Requires-Dist: black~=24.4.2; extra == "docs"
 Requires-Dist: griffe-inherited-docstrings~=1.0.0; extra == "docs"
 Requires-Dist: mkdocs-glightbox~=0.4.0; extra == "docs"
 Provides-Extra: dev
-Requires-Dist: ruff==0.4.4; extra == "dev"
+Requires-Dist: ruff==0.4.5; extra == "dev"
 Requires-Dist: pyright==1.1.364; extra == "dev"
 Requires-Dist: nox==2024.4.15; extra == "dev"
 Requires-Dist: typing_extensions==4.11.0; extra == "dev"
 Requires-Dist: pytest==8.2.1; extra == "dev"
 Requires-Dist: pytest-asyncio==0.23.7; extra == "dev"
 Requires-Dist: slotscheck==0.19.0; extra == "dev"
 Provides-Extra: rest
```

### Comparing `hikari_arc-1.3.1/README.md` & `hikari_arc-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.1/arc/__init__.py` & `hikari_arc-1.3.2/arc/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.1/arc/__main__.py` & `hikari_arc-1.3.2/arc/__main__.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.1/arc/abc/__init__.py` & `hikari_arc-1.3.2/arc/abc/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.1/arc/abc/client.py` & `hikari_arc-1.3.2/arc/abc/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -479,15 +479,15 @@
             This is only applicable to slash commands.
 
         Yields
         ------
         CommandT[te.Self]
             The next command that matches the given criteria.
 
-        Examples
+        Example
         --------
         ```py
         for cmd in plugin.walk_commands(hikari.CommandType.SLASH):
             print(cmd.name)
         ```
 
         !!! tip
@@ -557,15 +557,15 @@
             The command to add.
 
         Raises
         ------
         RuntimeError
             If the command is already added to a plugin.
 
-        Examples
+        Example
         --------
         ```py
         @client.include # Add the command to the client.
         @arc.slash_command("cmd", "A command.")
         async def cmd(ctx: arc.GatewayContext) -> None:
             ...
         ```
@@ -633,15 +633,15 @@
         -------
         SlashGroup[te.Self]
             The slash command group that was created.
 
         !!! note
             Parameters left as `hikari.UNDEFINED` will be inherited from the parent client.
 
-        Examples
+        Example
         --------
         ```py
         group = client.include_slash_group("Group", "A group of commands.")
 
         @group.include
         @arc.slash_subcommand(name="Command", description="A command.")
         async def cmd(ctx: arc.GatewayContext) -> None:
@@ -887,15 +887,15 @@
             The error handler to set.
 
         Returns
         -------
         te.Self
             The client for chaining calls.
 
-        Examples
+        Example
         --------
         ```py
         @client.set_error_handler
         async def error_handler_func(ctx: arc.GatewayContext, exception: Exception) -> None:
             await ctx.respond(f"❌ Something went wrong: {exception}")
         ```
 
@@ -938,15 +938,15 @@
             The startup hook to add.
 
         Returns
         -------
         te.Self
             The client for chaining calls.
 
-        Examples
+        Example
         --------
         ```py
         @client.add_startup_hook
         async def startup_hook(client: arc.GatewayClient) -> None:
             print("Client started up!")
         ```
 
@@ -985,15 +985,15 @@
             The shutdown hook to add.
 
         Returns
         -------
         te.Self
             The client for chaining calls.
 
-        Examples
+        Example
         --------
         ```py
         @client.add_shutdown_hook
         async def shutdown_hook(client: arc.GatewayClient) -> None:
             print("Client shut down!")
         ```
 
@@ -1036,15 +1036,15 @@
             The startup hook to set.
 
         Returns
         -------
         te.Self
             The client for chaining calls.
 
-        Examples
+        Example
         --------
         ```py
         @client.set_startup_hook
         async def startup_hook(client: arc.GatewayClient) -> None:
             print("Client started up!")
         ```
 
@@ -1088,15 +1088,15 @@
             The shutdown hook to set.
 
         Returns
         -------
         te.Self
             The client for chaining calls.
 
-        Examples
+        Example
         --------
         ```py
         @client.set_shutdown_hook
         async def shutdown_hook(client: arc.GatewayClient) -> None:
             print("Client shut down!")
         ```
 
@@ -1136,15 +1136,15 @@
             The command locale provider to set.
 
         Returns
         -------
         te.Self
             The client for chaining calls.
 
-        Examples
+        Example
         --------
         ```py
         @client.set_command_locale_provider
         def command_locale_provider(request: arc.CommandLocaleRequest) -> arc.LocaleResponse:
             ...
         ```
 
@@ -1183,15 +1183,15 @@
             The option locale provider to set.
 
         Returns
         -------
         te.Self
             The client for chaining calls.
 
-        Examples
+        Example
         --------
         ```py
         @client.set_option_locale_provider
         def option_locale_provider(request: arc.OptionLocaleRequest) -> arc.LocaleResponse:
             ...
         ```
 
@@ -1225,15 +1225,15 @@
         This will be called for each custom locale request performed via [`Context.loc()`][arc.context.base.Context.loc].
 
         Parameters
         ----------
         provider : CustomLocaleRequestT
             The custom locale provider to set.
 
-        Examples
+        Example
         --------
         ```py
         @client.set_custom_locale_provider
         def custom_locale_provider(request: arc.CustomLocaleRequest) -> str:
             ...
         ```
 
@@ -1268,15 +1268,15 @@
             The client for chaining calls.
 
         Raises
         ------
         ValueError
             If the module does not have a loader.
 
-        Examples
+        Example
         --------
         ```py
         client = arc.GatewayClient(...)
         client.load_extension("extension")
 
         # In extension.py
 
@@ -1333,15 +1333,15 @@
         Raises
         ------
         ExtensionLoadError
             If `dir_path` does not exist or is not a directory.
         ExtensionLoadError
             If a module does not have a loader defined.
 
-        Examples
+        Example
         --------
         ```py
         client = arc.GatewayClient(...)
         client.load_extensions_from("extensions/foo")
         ```
 
         See Also
@@ -1434,15 +1434,15 @@
             The instance of the dependency.
 
         Returns
         -------
         te.Self
             The client for chaining calls.
 
-        Examples
+        Example
         --------
         ```py
         class MyDependency:
             def __init__(self, value: str):
                 self.value = value
 
         client.set_type_dependency(MyDependency, MyDependency("Hello!"))
@@ -1509,15 +1509,15 @@
     ) -> t.Callable[P, T] | t.Callable[[t.Callable[P, T]], t.Callable[P, T]]:
         """Decorator to inject dependencies into the decorated function.
 
         !!! note
             Command callbacks are automatically injected with dependencies,
             thus this decorator is not needed for them.
 
-        Examples
+        Example
         --------
         ```py
         class MyDependency:
             def __init__(self, value: str):
                 self.value = value
 
         client.set_type_dependency(MyDependency, MyDependency("Hello!"))
```

### Comparing `hikari_arc-1.3.1/arc/abc/command.py` & `hikari_arc-1.3.2/arc/abc/command.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.1/arc/abc/concurrency_limiting.py` & `hikari_arc-1.3.2/arc/abc/concurrency_limiting.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
         The concurrency limiter to use.
 
     Returns
     -------
     t.Callable[[HasConcurrencyLimiterT], HasConcurrencyLimiterT]
         The object with the concurrency limiter set.
 
-    Examples
+    Example
     --------
     ```py
     @client.include
     # Max 5 users can use this command at a time.
     @arc.with_concurrency_limit(arc.user_concurrency(5))
     @arc.slash_command(...)
     async def foo(ctx: arc.GatewayContext) -> None:
```

### Comparing `hikari_arc-1.3.1/arc/abc/error_handler.py` & `hikari_arc-1.3.2/arc/abc/error_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     def set_error_handler(
         self, callback: ErrorHandlerCallbackT[ClientT] | None = None
     ) -> ErrorHandlerCallbackT[ClientT] | t.Callable[[ErrorHandlerCallbackT[ClientT]], ErrorHandlerCallbackT[ClientT]]:
         """Decorator to set an error handler for this object. This can be added to commands, groups, or plugins.
 
         This function will be called when an exception is raised during the invocation of a command.
 
-        Examples
+        Example
         --------
         ```py
         @client.include
         @arc.slash_command("foo", "Foo command description")
         async def foo(ctx: arc.GatewayContext) -> None:
             raise RuntimeError("foo")
```

### Comparing `hikari_arc-1.3.1/arc/abc/hookable.py` & `hikari_arc-1.3.2/arc/abc/hookable.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,15 +93,15 @@
 def with_hook(hook: HookT[ClientT]) -> t.Callable[[HookableT], HookableT]:
     """Add a new pre-execution hook to a hookable object. It will run before the command callback.
 
     Any function that takes a [`Context`][arc.context.base.Context] as its sole parameter
     and returns either a [`HookResult`][arc.abc.hookable.HookResult] or
     `None` can be used as a hook.
 
-    Examples
+    Example
     --------
     ```py
     @client.include
     @arc.with_hook(arc.guild_only) # Add a pre-execution hook to a command
     @arc.slash_command("foo", "Foo command description")
     async def foo(ctx: arc.GatewayContext) -> None:
         ...
@@ -123,15 +123,15 @@
 
     Post-execution hooks are not executed if a pre-execution hook aborts the execution of the command.
 
     !!! warning
         Post-execution hooks **are** called even if the command callback raises an exception.
         You can see if the command callback failed by checking [`Context.has_command_failed`][arc.context.base.Context.has_command_failed].
 
-    Examples
+    Example
     --------
     ```py
     @client.include
     @arc.with_post_hook(arc.guild_only) # Add a post-execution hook to a command
     @arc.slash_command("foo", "Foo command description")
     async def foo(ctx: arc.GatewayContext) -> None:
         ...
```

### Comparing `hikari_arc-1.3.1/arc/abc/limiter.py` & `hikari_arc-1.3.2/arc/abc/limiter.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.1/arc/abc/option.py` & `hikari_arc-1.3.2/arc/abc/option.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 T = t.TypeVar("T")
 OriginT = t.TypeVar("OriginT")
 
 Option = t.Annotated
 """Alias for typing.Annotated.
 
-Examples
+Example
 --------
 ```py
 arc.Option[type, arc.TypeParams(...)]
 ```
 
 So for example, to create an `int` option, you would do:
```

### Comparing `hikari_arc-1.3.1/arc/abc/plugin.py` & `hikari_arc-1.3.2/arc/abc/plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -291,15 +291,15 @@
         -------
         SlashGroup[te.Self]
             The slash command group that was created.
 
         !!! note
             Parameters left as `hikari.UNDEFINED` will be inherited from the parent plugin or client.
 
-        Examples
+        Example
         --------
         ```py
         group = client.include_slash_group("Group", "A group of commands.")
 
         @group.include
         @arc.slash_subcommand(name="Command", description="A command.")
         async def cmd(ctx: arc.GatewayContext) -> None:
@@ -336,15 +336,15 @@
         !!! warning
             This makes functions uncallable if the plugin is not added to a client.
 
         !!! note
             Command callbacks are automatically injected with dependencies,
             thus this decorator is not needed for them.
 
-        Examples
+        Example
         --------
         ```py
         class MyDependency:
             def __init__(self, value: str):
                 self.value = value
 
         client = arc.GatewayClient(...)
@@ -435,15 +435,15 @@
             If True, command groups and subgroups will be skipped.
 
         Yields
         ------
         CommandT[ClientT]
             The next command that matches the given criteria.
 
-        Examples
+        Example
         --------
         ```py
         for cmd in plugin.walk_commands(hikari.CommandType.SLASH):
             print(cmd.name)
         ```
 
         !!! tip
```

### Comparing `hikari_arc-1.3.1/arc/client.py` & `hikari_arc-1.3.2/arc/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -340,15 +340,15 @@
         This applies to all commands, and can be overridden on a per-command basis.
     provided_locales : t.Sequence[hikari.Locale] | None
         The locales that will be provided to the client by locale provider callbacks
     injector : alluka.abc.Client | None
         If you already have an injector instance, you may pass it here.
         Otherwise, a new one will be created by default.
 
-    Examples
+    Example
     --------
     ```py
     import hikari
     import arc
 
     bot = hikari.GatewayBot("TOKEN")
     client = arc.GatewayClient(bot)
@@ -386,15 +386,15 @@
     provided_locales : t.Sequence[hikari.Locale] | None
         The locales that will be provided to the client by locale provider callbacks
     injector : alluka.abc.Client | None
         If you already have an injector instance, you may pass it here.
         Otherwise, a new one will be created by default.
 
 
-    Examples
+    Example
     --------
     ```py
     import hikari
     import arc
 
     bot = hikari.RESTBot("TOKEN")
     client = arc.RESTClient(bot)
```

### Comparing `hikari_arc-1.3.1/arc/command/__init__.py` & `hikari_arc-1.3.2/arc/command/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.1/arc/command/message.py` & `hikari_arc-1.3.2/arc/command/message.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,15 @@
         If True, this command will be automatically deferred if it takes longer than 2 seconds to respond
     default_permissions : hikari.Permissions | hikari.UndefinedType
         The default permissions for this command.
         Keep in mind that guild administrators can change this, it should only be used to provide safe defaults.
     name_localizations : t.Mapping[hikari.Locale, str] | None
         The localizations for this command's name.
 
-    Examples
+    Example
     --------
     ```py
     @client.include
     @arc.message_command(name="Say Hi", description="Say hi!")
     async def hi_msg(
         ctx: arc.GatewayContext, message: hikari.Message
     ) -> None:
```

### Comparing `hikari_arc-1.3.1/arc/command/option/__init__.py` & `hikari_arc-1.3.2/arc/command/option/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.1/arc/command/option/attachment.py` & `hikari_arc-1.3.2/arc/command/option/attachment.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,17 +18,14 @@
 class AttachmentParams(OptionParams[hikari.Attachment]):
     """The parameters for an attachment option.
 
     Parameters
     ----------
     description : str
         The description of the option
-
-    Other Parameters
-    ----------------
     name : str
         The name of the option. If not provided, the name of the parameter will be used.
     name_localizations : Mapping[hikari.Locale, str] | None
         The name of the option in different locales
     description_localizations : Mapping[hikari.Locale, str] | None
         The description of the option in different locales
     """
```

### Comparing `hikari_arc-1.3.1/arc/command/option/bool.py` & `hikari_arc-1.3.2/arc/command/option/bool.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,17 +17,14 @@
 class BoolParams(OptionParams[bool]):
     """The parameters for a bool option.
 
     Parameters
     ----------
     description : str
         The description of the option
-
-    Other Parameters
-    ----------------
     name : str
         The name of the option. If not provided, the name of the parameter will be used.
     name_localizations : t.Optional[t.Mapping[str, str]]
         The localizations for the name of the option
     description_localizations : t.Optional[t.Mapping[str, str]]
         The localizations for the description of the option
     """
```

### Comparing `hikari_arc-1.3.1/arc/command/option/channel.py` & `hikari_arc-1.3.2/arc/command/option/channel.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,17 +24,14 @@
         hikari.ChannelType.GUILD_PRIVATE_THREAD |
         hikari.ChannelType.GUILD_NEWS_THREAD`.
 
     Parameters
     ----------
     description : str
         The description of the option
-
-    Other Parameters
-    ----------------
     name : str
         The name of the option. If not provided, the name of the parameter will be used.
     name_localizations : Mapping[hikari.Locale, str]
         The name of the option in different locales
     description_localizations : Mapping[hikari.Locale, str]
         The description of the option in different locales
     """
```

### Comparing `hikari_arc-1.3.1/arc/command/option/custom/color.py` & `hikari_arc-1.3.2/arc/command/option/custom/color.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,17 +20,14 @@
 class ColorParams(OptionParams[hikari.Color]):
     """The parameters for a color option.
 
     Parameters
     ----------
     description : str
         The description of the option
-
-    Other Parameters
-    ----------------
     name : str
         The name of the option. If not provided, the name of the parameter will be used.
     name_localizations : Mapping[hikari.Locale, str] | None
         The name of the option in different locales
     description_localizations : Mapping[hikari.Locale, str] | None
         The description of the option in different locales
     """
```

### Comparing `hikari_arc-1.3.1/arc/command/option/custom/member.py` & `hikari_arc-1.3.2/arc/command/option/custom/member.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,17 +20,14 @@
 class MemberParams(OptionParams[hikari.InteractionMember]):
     """The parameters for a member option.
 
     Parameters
     ----------
     description : str
         The description of the option
-
-    Other Parameters
-    ----------------
     name : str
         The name of the option. If not provided, the name of the parameter will be used.
     name_localizations : Mapping[hikari.Locale, str] | None
         The name of the option in different locales
     description_localizations : Mapping[hikari.Locale, str] | None
         The description of the option in different locales
     """
```

### Comparing `hikari_arc-1.3.1/arc/command/option/float.py` & `hikari_arc-1.3.2/arc/command/option/float.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,17 +23,14 @@
     !!! warning
         You cannot provide both `choices` and `autocomplete_with` at the same time.
 
     Parameters
     ----------
     description : str
         The description of the option
-
-    Other Parameters
-    ----------------
     name : str
         The name of the option. If not provided, the name of the parameter will be used.
     name_localizations : Mapping[hikari.Locale, str] | None
         The name of the option in different locales
     description_localizations : Mapping[hikari.Locale, str] | None
         The description of the option in different locales
     min : float | None
```

### Comparing `hikari_arc-1.3.1/arc/command/option/int.py` & `hikari_arc-1.3.2/arc/command/option/int.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,17 +23,14 @@
     !!! warning
         You cannot provide both `choices` and `autocomplete_with` at the same time.
 
     Parameters
     ----------
     description : str
         The description of the option
-
-    Other Parameters
-    ----------------
     name : str
         The name of the option. If not provided, the name of the parameter will be used.
     name_localizations : Mapping[hikari.Locale, str] | None
         The name of the option in different locales
     description_localizations : Mapping[hikari.Locale, str] | None
         The description of the option in different locales
     min : int | None
```

### Comparing `hikari_arc-1.3.1/arc/command/option/mentionable.py` & `hikari_arc-1.3.2/arc/command/option/mentionable.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,17 +19,14 @@
     """The parameters for a mentionable option.
     This is an option of type `hikari.Role | hikari.User`.
 
     Parameters
     ----------
     description : str
         The description of the option
-
-    Other Parameters
-    ----------------
     name : str
         The name of the option. If not provided, the name of the parameter will be used.
     name_localizations : Mapping[hikari.Locale, str] | None
         The name of the option in different locales
     description_localizations : Mapping[hikari.Locale, str] | None
         The description of the option in different locales
     """
```

### Comparing `hikari_arc-1.3.1/arc/command/option/role.py` & `hikari_arc-1.3.2/arc/command/option/role.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,17 +18,14 @@
 class RoleParams(OptionParams[hikari.Role]):
     """The parameters for a user option.
 
     Parameters
     ----------
     description : str
         The description of the option
-
-    Other Parameters
-    ----------------
     name : str
         The name of the option. If not provided, the name of the parameter will be used.
     name_localizations : t.Optional[t.Mapping[str, str]]
         The localizations for the name of the option
     description_localizations : t.Optional[t.Mapping[str, str]]
         The localizations for the description of the option
     """
```

### Comparing `hikari_arc-1.3.1/arc/command/option/str.py` & `hikari_arc-1.3.2/arc/command/option/str.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,17 +24,14 @@
     !!! warning
         You cannot provide both `choices` and `autocomplete_with` at the same time.
 
     Parameters
     ----------
     description : str
         The description of the option
-
-    Other Parameters
-    ----------------
     name : str
         The name of the option. If not provided, the name of the parameter will be used.
     name_localizations : Mapping[hikari.Locale, str]
         The name of the option in different locales
     description_localizations : Mapping[hikari.Locale, str]
         The description of the option in different locales
     min_length : int | None
```

### Comparing `hikari_arc-1.3.1/arc/command/option/user.py` & `hikari_arc-1.3.2/arc/command/option/user.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,17 +19,14 @@
 class UserParams(OptionParams[hikari.User]):
     """The parameters for a user option.
 
     Parameters
     ----------
     description : str
         The description of the option
-
-    Other Parameters
-    ----------------
     name : str
         The name of the option. If not provided, the name of the parameter will be used.
     name_localizations : Mapping[hikari.Locale, str] | None
         The name of the option in different locales
     description_localizations : Mapping[hikari.Locale, str] | None
         The description of the option in different locales
     """
```

### Comparing `hikari_arc-1.3.1/arc/command/slash.py` & `hikari_arc-1.3.2/arc/command/slash.py`

 * *Files 0% similar despite different names*

```diff
@@ -542,15 +542,15 @@
         try:
             if self.error_handler:
                 await ctx._injection_ctx.call_with_async_di(self.error_handler, ctx, exc)
             else:
                 raise exc
         except Exception as exc:
             assert self._parent is not None
-            await ctx._injection_ctx.call_with_async_di(self._parent._handle_exception, ctx, exc)
+            await self._parent._handle_exception(ctx, exc)
 
     def _request_option_locale(self, client: Client[t.Any], command: CommandProto) -> None:
         super()._request_option_locale(client, command)
 
         for subcommand in self.children.values():
             subcommand._request_option_locale(client, command)
 
@@ -690,20 +690,20 @@
     def _resolve_concurrency_limiter(self) -> ConcurrencyLimiterProto[ClientT] | None:
         assert self._parent is not None
         return self._parent._resolve_concurrency_limiter()
 
     async def _handle_exception(self, ctx: Context[ClientT], exc: Exception) -> None:
         try:
             if self.error_handler:
-                await self.error_handler(ctx, exc)
+                await ctx._injection_ctx.call_with_async_di(self.error_handler, ctx, exc)
             else:
                 raise exc
         except Exception as e:
             assert self._parent is not None
-            await self._handle_exception(ctx, e)
+            await self._parent._handle_exception(ctx, e)
 
     def _request_option_locale(self, client: Client[t.Any], command: CommandProto) -> None:
         super()._request_option_locale(client, command)
 
         for option in self.options.values():
             option._request_option_locale(client, command)
 
@@ -773,15 +773,15 @@
     -------
     t.Callable[[t.Callable[t.Concatenate[Context[ClientT], ...], t.Awaitable[None]]], SlashCommand[ClientT]]
         The decorated slash command.
 
     !!! note
         Parameters left as `hikari.UNDEFINED` will be inherited from the parent plugin or client.
 
-    Examples
+    Example
     --------
     ```py
     @client.include
     @arc.slash_command("hi", "Say hi!")
     async def hi_slash(
         ctx: arc.GatewayContext,
         user: arc.Option[hikari.User, arc.UserParams("The user to say hi to.")]
@@ -839,15 +839,15 @@
     -------
     t.Callable[[t.Callable[t.Concatenate[Context[ClientT], ...], t.Awaitable[None]]], SlashCommand[ClientT]]
         The decorated slash command.
 
     !!! note
         Parameters left as `hikari.UNDEFINED` will be inherited from the parent group, plugin or client.
 
-    Examples
+    Example
     --------
     ```py
     group = client.include_slash_group("group", "A group of slash commands.")
 
     @group.include
     @arc.slash_subcommand(name="hi", description="Say hi!")
     async def hi_slashsub(
```

### Comparing `hikari_arc-1.3.1/arc/command/user.py` & `hikari_arc-1.3.2/arc/command/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,15 +95,15 @@
         If True, this command will be automatically deferred if it takes longer than 2 seconds to respond
     default_permissions : hikari.Permissions | hikari.UndefinedType
         The default permissions for this command.
         Keep in mind that guild administrators can change this, it should only be used to provide safe defaults.
     name_localizations : t.Mapping[hikari.Locale, str] | None
         The localizations for this command's name.
 
-    Examples
+    Example
     --------
     ```py
     @client.include
     @arc.user_command(name="Say Hi", description="Say hi!")
     async def hi_user(ctx: arc.GatewayContext, user: hikari.User) -> None:
         await ctx.respond(f"Hey {user.mention}!")
     ```
```

### Comparing `hikari_arc-1.3.1/arc/context/__init__.py` & `hikari_arc-1.3.2/arc/context/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.1/arc/context/autocomplete.py` & `hikari_arc-1.3.2/arc/context/autocomplete.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.1/arc/context/base.py` & `hikari_arc-1.3.2/arc/context/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -464,15 +464,15 @@
             The type of the option.
 
         Returns
         -------
         ValueT | None
             The value of the option, or None if it does not exist, or is not of the correct type.
 
-        Examples
+        Example
         --------
         ```py
         value = ctx.get_option("name", arc.OptionType.STRING)
         if value is None:
             # Option does not exist or is not a string
 
         # Do something with the value
```

### Comparing `hikari_arc-1.3.1/arc/errors.py` & `hikari_arc-1.3.2/arc/errors.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.1/arc/events.py` & `hikari_arc-1.3.2/arc/events.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.1/arc/extension.py` & `hikari_arc-1.3.2/arc/extension.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 
 def loader(
     callback: t.Callable[[ClientT], None] | None = None,
 ) -> t.Callable[[ClientT], None] | t.Callable[[t.Callable[[ClientT], None]], t.Callable[[ClientT], None]]:
     """Decorator to set the load callback for this module.
 
-    Examples
+    Example
     --------
     ```py
     client.load_extension("my_extension")
 
     # In my_extension.py:
 
     @arc.loader
@@ -57,15 +57,15 @@
 
 
 def unloader(
     callback: t.Callable[[ClientT], None] | None = None,
 ) -> t.Callable[[ClientT], None] | t.Callable[[t.Callable[[ClientT], None]], t.Callable[[ClientT], None]]:
     """Decorator to set the unload callback for this module.
 
-    Examples
+    Example
     --------
     ```py
     client.unload_extension("my_extension")
 
     # In my_extension.py:
 
     @arc.unloader
```

### Comparing `hikari_arc-1.3.1/arc/internal/__init__.py` & `hikari_arc-1.3.2/arc/internal/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.1/arc/internal/about.py` & `hikari_arc-1.3.2/arc/internal/about.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import typing as t
 
 __author__: t.Final[str] = "hypergonial"
 __author_email__: t.Final[str] = "git@hypergonial.com"
 __maintainer__: t.Final[str] = "hypergonial"
 __license__: t.Final[str] = "MIT"
 __url__: t.Final[str] = "https://github.com/hypergonial/hikari-arc"
-__version__: t.Final[str] = "1.3.1"
+__version__: t.Final[str] = "1.3.2"
 
 # MIT License
 #
 # Copyright (c) 2023-present hypergonial
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
```

### Comparing `hikari_arc-1.3.1/arc/internal/deprecation.py` & `hikari_arc-1.3.2/arc/internal/deprecation.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.1/arc/internal/options.py` & `hikari_arc-1.3.2/arc/internal/options.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.1/arc/internal/sigparse.py` & `hikari_arc-1.3.2/arc/internal/sigparse.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.1/arc/internal/sync.py` & `hikari_arc-1.3.2/arc/internal/sync.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.1/arc/internal/types.py` & `hikari_arc-1.3.2/arc/internal/types.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.1/arc/internal/version.py` & `hikari_arc-1.3.2/arc/internal/version.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.1/arc/locale.py` & `hikari_arc-1.3.2/arc/locale.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.1/arc/plugin.py` & `hikari_arc-1.3.2/arc/plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         This can be overridden on a per-command basis.
     default_permissions : hikari.Permissions | hikari.UndefinedType
         The default permissions for this plugin
         This can be overridden on a per-command basis.
     is_nsfw : bool | hikari.UndefinedType
         Whether this plugin is only usable in NSFW channels
 
-    Examples
+    Example
     --------
     ```py
     plugin = arc.RESTPlugin("MyPlugin")
 
     @plugin.include
     @arc.slash_command("ping", "Ping the bot.")
     async def ping(ctx: arc.RESTContext) -> None:
@@ -86,15 +86,15 @@
         This can be overridden on a per-command basis.
     default_permissions : hikari.Permissions | hikari.UndefinedType
         The default permissions for this plugin
         This can be overridden on a per-command basis.
     is_nsfw : bool | hikari.UndefinedType
         Whether this plugin is only usable in NSFW channels
 
-    Examples
+    Example
     --------
     ```py
     plugin = arc.GatewayPlugin("MyPlugin")
 
     @plugin.include
     @arc.slash_command("ping", "Ping the bot.")
     async def ping(ctx: arc.GatewayContext) -> None:
```

### Comparing `hikari_arc-1.3.1/arc/utils/__init__.py` & `hikari_arc-1.3.2/arc/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.1/arc/utils/concurrency_limiter.py` & `hikari_arc-1.3.2/arc/utils/concurrency_limiter.py`

 * *Files 1% similar despite different names*

```diff
@@ -252,15 +252,15 @@
         The maximum amount of concurrently running command instances.
 
     Returns
     -------
     CommandConcurrencyLimiter[t.Any]
         A concurrency limiter for use with a command.
 
-    Examples
+    Example
     --------
     ```py
     @arc.with_concurrency_limit(arc.global_concurrency(1))
     ```
     """
     return CommandConcurrencyLimiter(limit, get_key_with=lambda _: "amongus")
 
@@ -274,15 +274,15 @@
         The maximum amount of concurrently running command instances.
 
     Returns
     -------
     CommandConcurrencyLimiter[t.Any]
         A concurrency limiter for use with a command.
 
-    Examples
+    Example
     --------
     ```py
     @arc.with_concurrency_limit(arc.guild_concurrency(1))
     ```
     """
     return CommandConcurrencyLimiter(limit, get_key_with=lambda ctx: str(ctx.guild_id))
 
@@ -296,15 +296,15 @@
         The maximum amount of concurrently running command instances.
 
     Returns
     -------
     CommandConcurrencyLimiter[t.Any]
         A concurrency limiter for use with a command.
 
-    Examples
+    Example
     --------
     ```py
     @arc.with_concurrency_limit(arc.channel_concurrency(1))
     ```
     """
     return CommandConcurrencyLimiter(limit, get_key_with=lambda ctx: str(ctx.channel_id))
 
@@ -318,15 +318,15 @@
         The maximum amount of concurrently running command instances.
 
     Returns
     -------
     CommandConcurrencyLimiter[t.Any]
         A concurrency limiter for use with a command.
 
-    Examples
+    Example
     --------
     ```py
     @arc.with_concurrency_limit(arc.user_concurrency(1))
     ```
     """
     return CommandConcurrencyLimiter(limit, get_key_with=lambda ctx: str(ctx.author.id))
 
@@ -340,15 +340,15 @@
         The maximum amount of concurrently running command instances.
 
     Returns
     -------
     CommandConcurrencyLimiter[t.Any]
         A concurrency limiter for use with a command.
 
-    Examples
+    Example
     --------
     ```py
     @arc.with_concurrency_limit(arc.member_concurrency(1))
     ```
     """
     return CommandConcurrencyLimiter(limit, get_key_with=lambda ctx: f"{ctx.guild_id}:{ctx.author.id}")
 
@@ -366,15 +366,15 @@
         A callable that returns a key for the concurrency limiter bucket.
 
     Returns
     -------
     CommandConcurrencyLimiter[t.Any]
         A concurrency limiter for use with a command.
 
-    Examples
+    Example
     --------
     ```py
     # This is identical to 'arc.guild_concurrency(1)'
     @arc.with_concurrency_limit(arc.custom_concurrency(1, lambda ctx: str(ctx.guild_id)))
     ```
     """
     return CommandConcurrencyLimiter(limit, get_key_with=get_key_with)
```

### Comparing `hikari_arc-1.3.1/arc/utils/hooks/__init__.py` & `hikari_arc-1.3.2/arc/utils/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.1/arc/utils/hooks/basic.py` & `hikari_arc-1.3.2/arc/utils/hooks/basic.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 if t.TYPE_CHECKING:
     from arc.context import Context
 
 
 def guild_only(ctx: Context[t.Any]) -> HookResult:
     """A pre-execution hook that aborts the execution of a command if it is invoked outside of a guild.
 
-    Examples
+    Example
     --------
     ```py
     @arc.with_hook(arc.guild_only)
     ```
 
     Raises
     ------
@@ -35,15 +35,15 @@
         raise GuildOnlyError("This command can only be used in a guild.")
     return HookResult()
 
 
 def dm_only(ctx: Context[t.Any]) -> HookResult:
     """A pre-execution hook that aborts the execution of a command if it is invoked outside of a DM.
 
-    Examples
+    Example
     --------
     ```py
     @arc.with_hook(arc.dm_only)
     ```
 
     Raises
     ------
@@ -54,15 +54,15 @@
         raise DMOnlyError("This command can only be used in a DM.")
     return HookResult()
 
 
 def owner_only(ctx: Context[t.Any]) -> HookResult:
     """A pre-execution hook that aborts the execution of a command if it is invoked by a non-owner.
 
-    Examples
+    Example
     --------
     ```py
     @arc.with_hook(arc.owner_only)
     ```
 
     Raises
     ------
@@ -101,15 +101,15 @@
     Raises
     ------
     GuildOnlyError
         If the command is invoked outside of a guild.
     InvokerMissingPermissionsError
         If the invoker is missing some of the specified permissions.
 
-    Examples
+    Example
     --------
     ```py
     @arc.with_hook(arc.has_permissions(hikari.Permissions.MANAGE_CHANNELS | hikari.Permissions.MANAGE_GUILD))
     ```
     You can combine permissions with the bitwise OR operator (`|`).
 
     !!! note
@@ -145,15 +145,15 @@
     Raises
     ------
     GuildOnlyError
         If the command is invoked outside of a guild.
     BotMissingPermissionsError
         If the bot is missing some of the specified permissions.
 
-    Examples
+    Example
     --------
     ```py
     @arc.with_hook(arc.bot_has_permissions(hikari.Permissions.MANAGE_CHANNELS | hikari.Permissions.MANAGE_GUILD))
     ```
     You can combine permissions with the bitwise OR operator (`|`).
 
     !!! note
```

### Comparing `hikari_arc-1.3.1/arc/utils/hooks/limiters.py` & `hikari_arc-1.3.2/arc/utils/hooks/limiters.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
         The amount of requests allowed in a bucket.
 
     Raises
     ------
     RateLimiterExhaustedError
         If the limiter is exhausted.
 
-    Examples
+    Example
     --------
     ```py
     @arc.with_hook(arc.global_limiter(5.0, 1))
     ```
     """
     return LimiterHook(period, limit, get_key_with=lambda _: "amongus")
 
@@ -104,15 +104,15 @@
         The amount of requests allowed in a bucket.
 
     Raises
     ------
     RateLimiterExhaustedError
         If the limiter is exhausted.
 
-    Examples
+    Example
     --------
     ```py
     @arc.with_hook(arc.guild_limiter(5.0, 1))
     ```
     """
     return LimiterHook(period, limit, get_key_with=lambda ctx: str(ctx.guild_id))
 
@@ -130,15 +130,15 @@
         The amount of requests allowed in a bucket.
 
     Raises
     ------
     RateLimiterExhaustedError
         If the limiter is exhausted.
 
-    Examples
+    Example
     --------
     ```py
     @arc.with_hook(arc.channel_limiter(5.0, 1))
     ```
     """
     return LimiterHook(period, limit, get_key_with=lambda ctx: str(ctx.channel_id))
 
@@ -156,15 +156,15 @@
         The amount of requests allowed in a bucket.
 
     Raises
     ------
     RateLimiterExhaustedError
         If the limiter is exhausted.
 
-    Examples
+    Example
     --------
     ```py
     @arc.with_hook(arc.user_limiter(5.0, 1))
     ```
     """
     return LimiterHook(period, limit, get_key_with=lambda ctx: str(ctx.author.id))
 
@@ -183,15 +183,15 @@
         The amount of requests allowed in a bucket.
 
     Raises
     ------
     RateLimiterExhaustedError
         If the limiter is exhausted.
 
-    Examples
+    Example
     --------
     ```py
     @arc.with_hook(arc.member_limiter(5.0, 1))
     ```
     """
     return LimiterHook(period, limit, get_key_with=lambda ctx: f"{ctx.author.id}:{ctx.guild_id}")
 
@@ -211,15 +211,15 @@
         you would use `lambda ctx: str(ctx.guild_id)`.
 
     Raises
     ------
     RateLimiterExhaustedError
         If the limiter is exhausted.
 
-    Examples
+    Example
     --------
     ```py
     # This is identical to 'arc.guild_limiter(5.0, 1)'
     @arc.with_hook(arc.custom_limiter(5.0, 1, lambda ctx: str(ctx.guild_id)))
     ```
     """
     return LimiterHook(period, limit, get_key_with=get_key_with)
```

### Comparing `hikari_arc-1.3.1/arc/utils/loops.py` & `hikari_arc-1.3.2/arc/utils/loops.py`

 * *Files 10% similar despite different names*

```diff
@@ -148,15 +148,15 @@
     Raises
     ------
     ValueError
         If no interval is specified.
     TypeError
         If the passed function is not a coroutine function.
 
-    Examples
+    Example
     --------
     ```py
     loop = IntervalLoop(my_coro, seconds=5)
     loop.start()
     ```
 
     You may also use the decorator [`@arc.utils.interval_loop`][arc.utils.loops.interval_loop] to
@@ -185,14 +185,58 @@
             days = hours or 0
 
         self._sleep: float = seconds + minutes * 60 + hours * 3600 + days * 24 * 3600
 
     def _get_next_run(self) -> float:
         return self._sleep
 
+    def set_interval(
+        self,
+        *,
+        seconds: float | None = None,
+        minutes: float | None = None,
+        hours: float | None = None,
+        days: float | None = None,
+    ):
+        """Set a new specified interval.
+
+        !!! note
+            You need to restart the loop if you want these changes to take effect immediately.
+
+        Parameters
+        ----------
+        seconds : float | None, optional
+            The number of seconds to wait before running the coroutine again.
+        minutes : float | None, optional
+            The number of minutes to wait before running the coroutine again.
+        hours : float | None, optional
+            The number of hours to wait before running the coroutine again.
+        days : float | None, optional
+            The number of days to wait before running the coroutine again.
+
+        Example
+        --------
+        ```py
+        loop = IntervalLoop(my_coro, seconds=5)
+        loop.start()
+        loop.set_interval(seconds=10)
+        loop.cancel()
+        loop.start()
+        ```
+        """
+        if not seconds and not minutes and not hours and not days:
+            raise ValueError("At least one of 'seconds', 'minutes', 'hours' or 'days' must be not None.")
+        else:
+            seconds = seconds or 0
+            minutes = minutes or 0
+            hours = hours or 0
+            days = hours or 0
+
+        self._sleep: float = seconds + minutes * 60 + hours * 3600 + days * 24 * 3600
+
 
 class CronLoop(_LoopBase[P]):
     """A simple interval loop that runs a coroutine at a specified interval.
 
     !!! warning
         To use this loop, you must install arc with the `cron` extra.
 
@@ -203,26 +247,26 @@
     Parameters
     ----------
     callback : t.Callable[P, t.Awaitable[None]]
         The coroutine to run at the specified interval.
     cron_format : str
         The cron format to use. See https://en.wikipedia.org/wiki/Cron for more information.
     timezone : datetime.timezone
-        The timezone to use for the cron format. Defaults to UTC.
+        The timezone to use for the cron loop. Defaults to UTC.
 
     Raises
     ------
     ImportError
         If the `croniter` package is not installed.
     croniter.CroniterBadCronError
         If the cron format is invalid.
     TypeError
         If the passed function is not a coroutine function.
 
-    Examples
+    Example
     --------
     ```py
     loop = CronLoop(my_coro, "*/5 * * * *")
     loop.start()
     ```
 
     You may also use the decorator [`@arc.utils.cron_loop`][arc.utils.loops.cron_loop] to
@@ -252,42 +296,50 @@
         return (
             self._iter.get_next(float, start_time=datetime.datetime.now(self._tz))
             - datetime.datetime.now(self._tz).timestamp()
         )
 
 
 def interval_loop(
-    *, seconds: float | None = None, minutes: float | None = None, hours: float | None = None, days: float | None = None
+    *,
+    seconds: float | None = None,
+    minutes: float | None = None,
+    hours: float | None = None,
+    days: float | None = None,
+    run_on_start: bool = True,
 ) -> t.Callable[[t.Callable[P, t.Awaitable[None]]], IntervalLoop[P]]:
     """A decorator to create an [`IntervalLoop`][arc.utils.loops.IntervalLoop] out of a coroutine function.
 
     Parameters
     ----------
     seconds : float, optional
         The number of seconds to wait before running the coroutine again.
     minutes : float, optional
         The number of minutes to wait before running the coroutine again.
     hours : float, optional
         The number of hours to wait before running the coroutine again.
     days : float, optional
         The number of days to wait before running the coroutine again.
+    run_on_start : bool, optional
+        Whether to run the callback immediately after starting the loop.
+        If set to false, the loop will wait for the specified interval before first running the callback.
 
     Returns
     -------
     t.Callable[[t.Callable[P, t.Awaitable[None]]], IntervalLoop[P]]
         The decorator.
 
     Raises
     ------
     ValueError
         If no interval is specified.
     TypeError
         If the decorated function is not a coroutine function.
 
-    Examples
+    Example
     --------
     ```py
     import arc
 
     # Run every 5 seconds.
     @arc.utils.interval_loop(seconds=5)
     async def my_loop():
@@ -296,33 +348,37 @@
     # Elsewhere...
 
     my_loop.start()
     ```
     """
 
     def decorator(coro: t.Callable[P, t.Awaitable[None]]) -> IntervalLoop[P]:
-        return IntervalLoop(coro, seconds=seconds, minutes=minutes, hours=hours, days=days)
+        return IntervalLoop(coro, seconds=seconds, minutes=minutes, hours=hours, days=days, run_on_start=run_on_start)
 
     return decorator
 
 
-def cron_loop(cron_format: str) -> t.Callable[[t.Callable[P, t.Awaitable[None]]], CronLoop[P]]:
+def cron_loop(
+    cron_format: str, timezone: datetime.timezone = datetime.timezone.utc
+) -> t.Callable[[t.Callable[P, t.Awaitable[None]]], CronLoop[P]]:
     """Decorator to create a [`CronLoop`][arc.utils.loops.CronLoop] out of a coroutine function.
 
     !!! warning
         To use this loop, you must install arc with the `cron` extra.
 
         ```sh
         pip install hikari-arc[cron]
         ```
 
     Parameters
     ----------
     cron_format : str
         The cron format to use. See https://en.wikipedia.org/wiki/Cron for more information.
+    timezone : datetime.timezone
+        The timezone to use for the cron loop. Defaults to UTC.
 
     Returns
     -------
     Callable[[t.Callable[P, t.Awaitable[None]]], CronLoop[P]]
         The decorator.
 
     Raises
@@ -330,15 +386,15 @@
     ImportError
         If the `croniter` package is not installed.
     croniter.CroniterBadCronError
         If the cron format is invalid.
     TypeError
         If the decorated function is not a coroutine function.
 
-    Examples
+    Example
     --------
     ```py
     import arc
 
     # Run every 5th minute of every hour.
     @arc.utils.cron_loop("*/5 * * * *")
     async def my_loop():
@@ -347,15 +403,15 @@
     # Elsewhere...
 
     my_loop.start()
     ```
     """
 
     def decorator(coro: t.Callable[P, t.Awaitable[None]]) -> CronLoop[P]:
-        return CronLoop(coro, cron_format)
+        return CronLoop(coro, cron_format, timezone=timezone)
 
     return decorator
 
 
 # MIT License
 #
 # Copyright (c) 2023-present hypergonial
```

### Comparing `hikari_arc-1.3.1/arc/utils/ratelimiter.py` & `hikari_arc-1.3.2/arc/utils/ratelimiter.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.1/hikari_arc.egg-info/PKG-INFO` & `hikari_arc-1.3.2/hikari_arc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hikari-arc
-Version: 1.3.1
+Version: 1.3.2
 Summary: A command handler for hikari with a focus on type-safety and correctness.
 Home-page: https://github.com/hypergonial/hikari-arc
 Author: hypergonial
 Author-email: git@hypergonial.com
 Maintainer: hypergonial
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
@@ -26,20 +26,20 @@
 Requires-Dist: hikari>=2.0.0.dev122
 Requires-Dist: alluka<0.4,>=0.3.0
 Requires-Dist: attrs>=23.1
 Requires-Dist: colorama; sys_platform == "win32"
 Provides-Extra: docs
 Requires-Dist: mkdocs-material[imaging]~=9.5.24; extra == "docs"
 Requires-Dist: mkdocs~=1.6.0; extra == "docs"
-Requires-Dist: mkdocstrings-python~=1.10.2; extra == "docs"
+Requires-Dist: mkdocstrings-python~=1.10.3; extra == "docs"
 Requires-Dist: black~=24.4.2; extra == "docs"
 Requires-Dist: griffe-inherited-docstrings~=1.0.0; extra == "docs"
 Requires-Dist: mkdocs-glightbox~=0.4.0; extra == "docs"
 Provides-Extra: dev
-Requires-Dist: ruff==0.4.4; extra == "dev"
+Requires-Dist: ruff==0.4.5; extra == "dev"
 Requires-Dist: pyright==1.1.364; extra == "dev"
 Requires-Dist: nox==2024.4.15; extra == "dev"
 Requires-Dist: typing_extensions==4.11.0; extra == "dev"
 Requires-Dist: pytest==8.2.1; extra == "dev"
 Requires-Dist: pytest-asyncio==0.23.7; extra == "dev"
 Requires-Dist: slotscheck==0.19.0; extra == "dev"
 Provides-Extra: rest
```

### Comparing `hikari_arc-1.3.1/hikari_arc.egg-info/SOURCES.txt` & `hikari_arc-1.3.2/hikari_arc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.1/pyproject.toml` & `hikari_arc-1.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.1/setup.py` & `hikari_arc-1.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.1/tests/test_client.py` & `hikari_arc-1.3.2/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.1/tests/test_context_command.py` & `hikari_arc-1.3.2/tests/test_context_command.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.1/tests/test_di.py` & `hikari_arc-1.3.2/tests/test_di.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.1/tests/test_inheritance.py` & `hikari_arc-1.3.2/tests/test_inheritance.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.1/tests/test_options.py` & `hikari_arc-1.3.2/tests/test_options.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.1/tests/test_sigparse.py` & `hikari_arc-1.3.2/tests/test_sigparse.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.1/tests/test_slash.py` & `hikari_arc-1.3.2/tests/test_slash.py`

 * *Files identical despite different names*

