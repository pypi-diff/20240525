# Comparing `tmp/nonebot_plugin_authrespond-1.6.tar.gz` & `tmp/nonebot_plugin_authrespond-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_authrespond-1.6.tar", last modified: Sat May 25 01:06:57 2024, max compression
+gzip compressed data, was "nonebot_plugin_authrespond-1.6.1.tar", last modified: Sat May 25 10:28:26 2024, max compression
```

## Comparing `nonebot_plugin_authrespond-1.6.tar` & `nonebot_plugin_authrespond-1.6.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 01:06:57.337774 nonebot_plugin_authrespond-1.6/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-25 01:06:53.000000 nonebot_plugin_authrespond-1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    44162 2024-05-25 01:06:57.337774 nonebot_plugin_authrespond-1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-05-25 01:06:53.000000 nonebot_plugin_authrespond-1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 01:06:57.337774 nonebot_plugin_authrespond-1.6/nonebot_plugin_authrespond/
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-25 01:06:53.000000 nonebot_plugin_authrespond-1.6/nonebot_plugin_authrespond/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-25 01:06:53.000000 nonebot_plugin_authrespond-1.6/nonebot_plugin_authrespond/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-05-25 01:06:53.000000 nonebot_plugin_authrespond-1.6/nonebot_plugin_authrespond/cubp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-05-25 01:06:53.000000 nonebot_plugin_authrespond-1.6/nonebot_plugin_authrespond/perm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-05-25 01:06:53.000000 nonebot_plugin_authrespond-1.6/nonebot_plugin_authrespond/plugins_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-05-25 01:06:53.000000 nonebot_plugin_authrespond-1.6/nonebot_plugin_authrespond/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 01:06:57.337774 nonebot_plugin_authrespond-1.6/nonebot_plugin_authrespond.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    44162 2024-05-25 01:06:57.000000 nonebot_plugin_authrespond-1.6/nonebot_plugin_authrespond.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-25 01:06:57.000000 nonebot_plugin_authrespond-1.6/nonebot_plugin_authrespond.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 01:06:57.000000 nonebot_plugin_authrespond-1.6/nonebot_plugin_authrespond.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-25 01:06:57.000000 nonebot_plugin_authrespond-1.6/nonebot_plugin_authrespond.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-25 01:06:57.000000 nonebot_plugin_authrespond-1.6/nonebot_plugin_authrespond.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-25 01:06:53.000000 nonebot_plugin_authrespond-1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 01:06:57.337774 nonebot_plugin_authrespond-1.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:28:26.137580 nonebot_plugin_authrespond-1.6.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-25 10:28:22.000000 nonebot_plugin_authrespond-1.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    44164 2024-05-25 10:28:26.137580 nonebot_plugin_authrespond-1.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-05-25 10:28:22.000000 nonebot_plugin_authrespond-1.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:28:26.137580 nonebot_plugin_authrespond-1.6.1/nonebot_plugin_authrespond/
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-25 10:28:22.000000 nonebot_plugin_authrespond-1.6.1/nonebot_plugin_authrespond/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-25 10:28:22.000000 nonebot_plugin_authrespond-1.6.1/nonebot_plugin_authrespond/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-05-25 10:28:22.000000 nonebot_plugin_authrespond-1.6.1/nonebot_plugin_authrespond/cubp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-05-25 10:28:22.000000 nonebot_plugin_authrespond-1.6.1/nonebot_plugin_authrespond/perm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-05-25 10:28:22.000000 nonebot_plugin_authrespond-1.6.1/nonebot_plugin_authrespond/plugins_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-05-25 10:28:22.000000 nonebot_plugin_authrespond-1.6.1/nonebot_plugin_authrespond/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:28:26.137580 nonebot_plugin_authrespond-1.6.1/nonebot_plugin_authrespond.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    44164 2024-05-25 10:28:26.000000 nonebot_plugin_authrespond-1.6.1/nonebot_plugin_authrespond.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-25 10:28:26.000000 nonebot_plugin_authrespond-1.6.1/nonebot_plugin_authrespond.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 10:28:26.000000 nonebot_plugin_authrespond-1.6.1/nonebot_plugin_authrespond.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-25 10:28:26.000000 nonebot_plugin_authrespond-1.6.1/nonebot_plugin_authrespond.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-25 10:28:26.000000 nonebot_plugin_authrespond-1.6.1/nonebot_plugin_authrespond.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-25 10:28:22.000000 nonebot_plugin_authrespond-1.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 10:28:26.137580 nonebot_plugin_authrespond-1.6.1/setup.cfg
```

### Comparing `nonebot_plugin_authrespond-1.6/LICENSE` & `nonebot_plugin_authrespond-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_authrespond-1.6/PKG-INFO` & `nonebot_plugin_authrespond-1.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-authrespond
-Version: 1.6
+Version: 1.6.1
 Summary: nonebot简单易用的黑名单插件，实现分插件拉黑用户/群聊/全局
 Author: cubstaryow
 Author-email: cub_staryow@outlook.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `nonebot_plugin_authrespond-1.6/README.md` & `nonebot_plugin_authrespond-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_authrespond-1.6/nonebot_plugin_authrespond/__init__.py` & `nonebot_plugin_authrespond-1.6.1/nonebot_plugin_authrespond/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,16 @@
     homepage="https://github.com/cubstaryow/nonebot-plugin-authrespond",
     # 发布必填。
 
     config=cubplugins_permission,
     # 插件配置项类，如无需配置可不填写。
     supported_adapters=inherit_supported_adapters(
         "nonebot_plugin_alconna",
-        "nonebot_plugin_session"
+        "nonebot_plugin_session",
+        "nonebot_plugin_localstore"
     )
     # 支持的适配器集合，其中 `~` 在此处代表前缀 `nonebot.adapters.`，其余适配器亦按此格式填写。
     # 若插件可以保证兼容所有适配器（即仅使用基本适配器功能）可不填写，否则应该列出插件支持的适配器。
 )
 
 from .run import *
```

### Comparing `nonebot_plugin_authrespond-1.6/nonebot_plugin_authrespond/cubp.py` & `nonebot_plugin_authrespond-1.6.1/nonebot_plugin_authrespond/cubp.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_authrespond-1.6/nonebot_plugin_authrespond/perm.py` & `nonebot_plugin_authrespond-1.6.1/nonebot_plugin_authrespond/perm.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_authrespond-1.6/nonebot_plugin_authrespond/plugins_data.py` & `nonebot_plugin_authrespond-1.6.1/nonebot_plugin_authrespond/plugins_data.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_authrespond-1.6/nonebot_plugin_authrespond/run.py` & `nonebot_plugin_authrespond-1.6.1/nonebot_plugin_authrespond/run.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_authrespond-1.6/nonebot_plugin_authrespond.egg-info/PKG-INFO` & `nonebot_plugin_authrespond-1.6.1/nonebot_plugin_authrespond.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-authrespond
-Version: 1.6
+Version: 1.6.1
 Summary: nonebot简单易用的黑名单插件，实现分插件拉黑用户/群聊/全局
 Author: cubstaryow
 Author-email: cub_staryow@outlook.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `nonebot_plugin_authrespond-1.6/pyproject.toml` & `nonebot_plugin_authrespond-1.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-authrespond"
-version = "1.6"
+version = "1.6.1"
 description = "nonebot简单易用的黑名单插件，实现分插件拉黑用户/群聊/全局"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {file = "LICENSE"}
 keywords = ["egg", "bacon", "sausage", "tomatoes", "Lobster Thermidor"]
 authors = [
   {email = "cub_staryow@outlook.com"},
```

