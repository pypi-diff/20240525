# Comparing `tmp/mhyy.py-2.0.0.tar.gz` & `tmp/mhyy_py-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mhyy.py-2.0.0.tar", last modified: Tue Feb  6 07:58:33 2024, max compression
+gzip compressed data, was "mhyy_py-2.1.0.tar", last modified: Sat May 25 08:23:37 2024, max compression
```

## Comparing `mhyy.py-2.0.0.tar` & `mhyy_py-2.1.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 07:58:33.511514 mhyy.py-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-02-06 07:58:24.000000 mhyy.py-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-02-06 07:58:33.511514 mhyy.py-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-02-06 07:58:24.000000 mhyy.py-2.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-02-06 07:58:24.000000 mhyy.py-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-06 07:58:33.511514 mhyy.py-2.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 07:58:33.507514 mhyy.py-2.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 07:58:33.511514 mhyy.py-2.0.0/src/mhyy/
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-02-06 07:58:24.000000 mhyy.py-2.0.0/src/mhyy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-02-06 07:58:24.000000 mhyy.py-2.0.0/src/mhyy/_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6789 2024-02-06 07:58:24.000000 mhyy.py-2.0.0/src/mhyy/_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-02-06 07:58:24.000000 mhyy.py-2.0.0/src/mhyy/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-02-06 07:58:24.000000 mhyy.py-2.0.0/src/mhyy/_notification.py
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-02-06 07:58:24.000000 mhyy.py-2.0.0/src/mhyy/_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-02-06 07:58:24.000000 mhyy.py-2.0.0/src/mhyy/_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-02-06 07:58:24.000000 mhyy.py-2.0.0/src/mhyy/_wallet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 07:58:33.511514 mhyy.py-2.0.0/src/mhyy.py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-02-06 07:58:33.000000 mhyy.py-2.0.0/src/mhyy.py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-02-06 07:58:33.000000 mhyy.py-2.0.0/src/mhyy.py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-06 07:58:33.000000 mhyy.py-2.0.0/src/mhyy.py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-06 07:58:33.000000 mhyy.py-2.0.0/src/mhyy.py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-06 07:58:33.000000 mhyy.py-2.0.0/src/mhyy.py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 08:23:37.482647 mhyy_py-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-25 08:23:32.000000 mhyy_py-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-25 08:23:37.482647 mhyy_py-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-25 08:23:32.000000 mhyy_py-2.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-25 08:23:32.000000 mhyy_py-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 08:23:37.482647 mhyy_py-2.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 08:23:37.478647 mhyy_py-2.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 08:23:37.482647 mhyy_py-2.1.0/src/mhyy/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-25 08:23:32.000000 mhyy_py-2.1.0/src/mhyy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-05-25 08:23:32.000000 mhyy_py-2.1.0/src/mhyy/_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6941 2024-05-25 08:23:32.000000 mhyy_py-2.1.0/src/mhyy/_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-25 08:23:32.000000 mhyy_py-2.1.0/src/mhyy/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-05-25 08:23:32.000000 mhyy_py-2.1.0/src/mhyy/_notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-25 08:23:32.000000 mhyy_py-2.1.0/src/mhyy/_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-05-25 08:23:32.000000 mhyy_py-2.1.0/src/mhyy/_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-05-25 08:23:32.000000 mhyy_py-2.1.0/src/mhyy/_wallet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 08:23:37.482647 mhyy_py-2.1.0/src/mhyy.py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-25 08:23:37.000000 mhyy_py-2.1.0/src/mhyy.py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-25 08:23:37.000000 mhyy_py-2.1.0/src/mhyy.py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 08:23:37.000000 mhyy_py-2.1.0/src/mhyy.py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-25 08:23:37.000000 mhyy_py-2.1.0/src/mhyy.py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-25 08:23:37.000000 mhyy_py-2.1.0/src/mhyy.py.egg-info/top_level.txt
```

### Comparing `mhyy.py-2.0.0/LICENSE` & `mhyy_py-2.1.0/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2023, Guang_Chen_
+Copyright (c) 2023-2024, Guang_Chen_
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
```

### Comparing `mhyy.py-2.0.0/PKG-INFO` & `mhyy_py-2.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mhyy.py
-Version: 2.0.0
+Version: 2.1.0
 Summary: Python API for miHoYo Cloud Gaming (Genshin Impact Cloud, Honkai:StarRail Cloud)
 Author-email: GuangChen2333 <guangchenworks@outlook.com>
 Project-URL: Homepage, https://github.com/GuangChen2333/mhyy.py
 Project-URL: Bug Tracker, https://github.com/GuangChen2333/mhyy.py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
@@ -18,15 +18,15 @@
 
 ![LICENSE](https://img.shields.io/github/license/GuangChen2333/mhyy.py?style=flat-square)
 ![Downloads](https://img.shields.io/pypi/dm/mhyy.py?style=flat-square)
 ![PyP](https://img.shields.io/pypi/v/mhyy.py?style=flat-square)
 ![Python](https://img.shields.io/pypi/pyversions/mhyy.py?style=flat-square)
 ![STARS](https://img.shields.io/github/stars/GuangChen2333/mhyy.py?style=flat-square)
 
-Python 米哈云游（云原神）签到功能与相关方法的API
+Python 米哈云游（云·原神、云·星穷铁道）签到功能与相关方法的API
 
 ## 安装
 
 - 从 `PyPi` 安装 `mhyy.py`
 
 ```shell
 pip install mhyy.py
@@ -34,8 +34,10 @@
 
 ## 文档
 
 访问 https://guangchen2333.github.io/mhyy.py/ 获取更多细节
 
 ## 关于
 
-欢迎协作本项目，如果你有任何意见或想法，请提出Issue。如果你喜欢，请给该仓库点一个Star
+欢迎协作本项目，如果你有任何意见或想法，请提出Issue。
+
+如果你喜欢此项目，请给该仓库点一个 Star 或提供一定的[捐助](https://afdian.net/a/GuangChen2333)。
```

### Comparing `mhyy.py-2.0.0/README.md` & `mhyy_py-2.1.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 ![LICENSE](https://img.shields.io/github/license/GuangChen2333/mhyy.py?style=flat-square)
 ![Downloads](https://img.shields.io/pypi/dm/mhyy.py?style=flat-square)
 ![PyP](https://img.shields.io/pypi/v/mhyy.py?style=flat-square)
 ![Python](https://img.shields.io/pypi/pyversions/mhyy.py?style=flat-square)
 ![STARS](https://img.shields.io/github/stars/GuangChen2333/mhyy.py?style=flat-square)
 
-Python 米哈云游（云原神）签到功能与相关方法的API
+Python 米哈云游（云·原神、云·星穷铁道）签到功能与相关方法的API
 
 ## 安装
 
 - 从 `PyPi` 安装 `mhyy.py`
 
 ```shell
 pip install mhyy.py
@@ -18,8 +18,10 @@
 
 ## 文档
 
 访问 https://guangchen2333.github.io/mhyy.py/ 获取更多细节
 
 ## 关于
 
-欢迎协作本项目，如果你有任何意见或想法，请提出Issue。如果你喜欢，请给该仓库点一个Star
+欢迎协作本项目，如果你有任何意见或想法，请提出Issue。
+
+如果你喜欢此项目，请给该仓库点一个 Star 或提供一定的[捐助](https://afdian.net/a/GuangChen2333)。
```

### Comparing `mhyy.py-2.0.0/pyproject.toml` & `mhyy_py-2.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mhyy.py"
-version = "2.0.0"
+version = "2.1.0"
 authors = [
     { name = "GuangChen2333", email = "guangchenworks@outlook.com" },
 ]
 description = "Python API for miHoYo Cloud Gaming (Genshin Impact Cloud, Honkai:StarRail Cloud)"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `mhyy.py-2.0.0/src/mhyy/_api.py` & `mhyy_py-2.1.0/src/mhyy/_api.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ._types import GameType, UserChannel
+from ._types import GameType, UserChannel, UserClientType
 
 
 class API:
     @staticmethod
     def get_launcher_key(game_type: GameType) -> str:
         return {
             GameType.GenshinImpact: "eYd89JmJ",
@@ -20,57 +20,71 @@
     def get_game_version_url(game_type: GameType) -> str:
         return {
             GameType.GenshinImpact: "https://sdk-static.mihoyo.com/hk4e_cn/mdk/launcher/api/resource",
             GameType.StarRail: "https://api-launcher.mihoyo.com/hkrpg_cn/mdk/launcher/api/resource"
         }[game_type]
 
     @staticmethod
-    def get_app_id(game_type: GameType) -> str:
+    def get_app_id(game_type: GameType, client_type: UserClientType) -> str:
         return {
-            GameType.GenshinImpact: "1953439974",
-            GameType.StarRail: "1953445976"
-        }[game_type]
+            UserClientType.Android: {
+                GameType.GenshinImpact: "1953439974",
+                GameType.StarRail: "1953445976",
+            },
+            UserClientType.PCWeb: {
+                GameType.GenshinImpact: "4",
+                GameType.StarRail: "8"
+            }
+        }[client_type][game_type]
 
     @staticmethod
-    def get_vendor_id(game_type: GameType) -> str:
+    def get_vendor_id(game_type: GameType, client_type: UserClientType) -> str:
         return {
-            GameType.GenshinImpact: "1",
-            GameType.StarRail: "2"
-        }[game_type]
+            UserClientType.Android: {
+                GameType.GenshinImpact: "1",
+                GameType.StarRail: "2",
+            },
+            UserClientType.PCWeb: {
+                GameType.GenshinImpact: "2",
+                GameType.StarRail: "2"
+            }
+        }[client_type][game_type]
 
     @staticmethod
     def get_cg_game_biz(game_type: GameType) -> str:
         return {
             GameType.GenshinImpact: "hk4e_cn",
-            GameType.StarRail: "hkrpg_cn"
+            GameType.StarRail: "hkrpg_cn",
         }[game_type]
 
     @staticmethod
     def get_op_biz(game_type: GameType) -> str:
         return {
             GameType.GenshinImpact: "clgm_cn",
-            GameType.StarRail: "clgm_hkrpg-cn"
+            GameType.StarRail: "clgm_hkrpg-cn",
         }[game_type]
 
     @staticmethod
-    def get_cps(game_type: GameType) -> str:
+    def get_cps(game_type: GameType, client_type: UserClientType) -> str:
         return {
-            GameType.GenshinImpact: "cyydmihoyo",
-            GameType.StarRail: "gw_An_C"
-        }[game_type]
+            UserClientType.Android: {
+                GameType.GenshinImpact: "mihoyo",
+                GameType.StarRail: "mihoyo",
+            },
+            UserClientType.PCWeb: {
+                GameType.GenshinImpact: "mihoyo",
+                GameType.StarRail: "mihoyo"
+            }
+        }[client_type][game_type]
 
     @staticmethod
-    def get_channel_id(user_channel: UserChannel, game_type: GameType) -> str:
-        channels = {
-            UserChannel.Official: {
-                GameType.GenshinImpact: "cyydmihoyo",
-                GameType.StarRail: "gw_An_C"
-            }
-        }
-        return channels[user_channel][game_type]
+    def get_channel_id(user_channel: UserChannel) -> str:
+        return {
+            UserChannel.Official: "mihoyo"
+        }[user_channel]
 
     @staticmethod
     def get_wallet_data_url(game_type: GameType) -> str:
         return {
             GameType.GenshinImpact: "https://api-cloudgame.mihoyo.com/hk4e_cg_cn/wallet/wallet/get",
             GameType.StarRail: "https://cg-hkrpg-api.mihoyo.com/hkrpg_cn/cg/wallet/wallet/get"
         }[game_type]
```

### Comparing `mhyy.py-2.0.0/src/mhyy/_client.py` & `mhyy_py-2.1.0/src/mhyy/_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from enum import Enum
 from typing import Optional, List
-from ._types import GameType, NotificationType, NotificationStatus
+from ._types import GameType, NotificationType, NotificationStatus, UserClientType
 from ._api import API
 from ._user import User
 from ._exceptions import WebRequestError, APIRequestError
 from ._wallet import WalletData
 from ._notification import Notification
 import httpx
 
@@ -63,31 +63,32 @@
         resp = self._client.get(version_url, params={
             "key": API.get_launcher_key(game_type),
             "launcher_id": API.get_launcher_id(game_type)
         }).json()
 
         self._versions[game_type] = resp["data"]["game"]["latest"]["version"]
 
-    def _get_common_headers(self, game_type: GameType) -> dict:
+    def _get_common_headers(self, game_type: GameType, client_type: UserClientType) -> dict:
         """
         获取指定游戏类型的 headers 常量。
 
         Args:
             game_type (GameType): 需要获取 headers 的游戏类型。
+            client_type (UserClientType): 用户的客户端类型。
 
         Returns:
             一个字典，包含了指定游戏的 headers。
         """
         return {
             "x-rpc-app_version": self._versions[game_type],
-            "x-rpc-app_id": API.get_app_id(game_type),
-            "x-rpc-vendor_id": API.get_vendor_id(game_type),
+            "x-rpc-app_id": API.get_app_id(game_type, client_type),
+            "x-rpc-vendor_id": API.get_vendor_id(game_type, client_type),
             "x-rpc-cg_game_biz": API.get_cg_game_biz(game_type),
             "x-rpc-op_biz": API.get_op_biz(game_type),
-            "x-rpc-cps": API.get_cps(game_type)
+            "x-rpc-cps": API.get_cps(game_type, client_type)
         }
 
     def _user_web_get(self, user: User, url: str, params: Optional[dict] = None) -> httpx.Response:
         """
         附带用户 headers 的 get 类型请求。
 
         Args:
@@ -108,21 +109,22 @@
             self._update_version(user.game_type)
 
         # Update client state.
         if self._status != ClientStatus.OPENED:
             self._status = ClientStatus.OPENED
 
         # Get the special common headers of the game.
-        headers: dict = self._get_common_headers(user.game_type)
+        headers: dict = self._get_common_headers(user.game_type, user.client_type)
 
         user_headers: dict = user.get_user_headers()
-        user_headers["x-rpc-channel"] = API.get_channel_id(user.channel, user.game_type)
 
         headers.update(user_headers)
 
+        headers["x-rpc-channel"] = API.get_channel_id(user.channel)
+
         resp = self._client.get(url, headers=headers, params=params)
 
         if resp.status_code != 200:
             raise WebRequestError(
                 f"An error occurred in the network request, status code: {resp.status_code}",
                 resp.status_code
             )
```

### Comparing `mhyy.py-2.0.0/src/mhyy/_exceptions.py` & `mhyy_py-2.1.0/src/mhyy/_exceptions.py`

 * *Files identical despite different names*

### Comparing `mhyy.py-2.0.0/src/mhyy/_notification.py` & `mhyy_py-2.1.0/src/mhyy/_notification.py`

 * *Files identical despite different names*

### Comparing `mhyy.py-2.0.0/src/mhyy/_types.py` & `mhyy_py-2.1.0/src/mhyy/_types.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,16 +16,18 @@
 
 class UserClientType(Enum):
     """
     客户端类型。
 
     Attributes:
         Android: 安卓。
+        PCWeb: PC 网页版。
     """
     Android = 2
+    PCWeb = 16
 
 
 class UserChannel(Enum):
     """
     游戏渠道。
 
     Attributes:
```

### Comparing `mhyy.py-2.0.0/src/mhyy/_user.py` & `mhyy_py-2.1.0/src/mhyy/_user.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,24 +4,25 @@
 from ._exceptions import ComboTokenInvalidError
 
 
 class User:
     """
     用户类。
     """
+
     def __init__(
             self,
             combo_token: str,
             sys_version: str,
             device_id: str,
             device_name: str,
             device_model: str,
             *,
             game_type: Optional[GameType] = None,
-            client_type: Optional[UserClientType] = UserClientType.Android,
+            client_type: Optional[UserClientType] = None,
             channel: Optional[UserChannel] = UserChannel.Official
     ):
         """
         创建一个用户。
 
         Args:
             combo_token (str): 对应 headers 中的 x-rpc-combo_token。
@@ -53,22 +54,30 @@
             )
 
         detected_game_type = {
             "hk4e_cn": GameType.GenshinImpact,
             "hkrpg_cn": GameType.StarRail
         }[bi]
 
+        if self._client_type is None:
+            self._client_type = UserClientType.Android
+            warnings.warn(
+                "In future versions, unspecified client_type will no longer be supported.",
+                UserWarning
+            )
+
         if self._game_type is None:
             self._game_type = detected_game_type
         else:
             if self._game_type != detected_game_type:
                 warnings.warn(
                     "The program detected a difference between the GameType you entered and the GameType it detected. "
                     "This time, it will use your input as the standard. So the data may be incorrect.”"
-                    "Please pay attention to the GameType."
+                    "Please pay attention to the GameType.",
+                    SyntaxWarning
                 )
 
     def get_user_headers(self) -> dict:
         """
         获取该用户的 headers。
 
         Returns:
```

### Comparing `mhyy.py-2.0.0/src/mhyy/_wallet.py` & `mhyy_py-2.1.0/src/mhyy/_wallet.py`

 * *Files identical despite different names*

### Comparing `mhyy.py-2.0.0/src/mhyy.py.egg-info/PKG-INFO` & `mhyy_py-2.1.0/src/mhyy.py.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mhyy.py
-Version: 2.0.0
+Version: 2.1.0
 Summary: Python API for miHoYo Cloud Gaming (Genshin Impact Cloud, Honkai:StarRail Cloud)
 Author-email: GuangChen2333 <guangchenworks@outlook.com>
 Project-URL: Homepage, https://github.com/GuangChen2333/mhyy.py
 Project-URL: Bug Tracker, https://github.com/GuangChen2333/mhyy.py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
@@ -18,15 +18,15 @@
 
 ![LICENSE](https://img.shields.io/github/license/GuangChen2333/mhyy.py?style=flat-square)
 ![Downloads](https://img.shields.io/pypi/dm/mhyy.py?style=flat-square)
 ![PyP](https://img.shields.io/pypi/v/mhyy.py?style=flat-square)
 ![Python](https://img.shields.io/pypi/pyversions/mhyy.py?style=flat-square)
 ![STARS](https://img.shields.io/github/stars/GuangChen2333/mhyy.py?style=flat-square)
 
-Python 米哈云游（云原神）签到功能与相关方法的API
+Python 米哈云游（云·原神、云·星穷铁道）签到功能与相关方法的API
 
 ## 安装
 
 - 从 `PyPi` 安装 `mhyy.py`
 
 ```shell
 pip install mhyy.py
@@ -34,8 +34,10 @@
 
 ## 文档
 
 访问 https://guangchen2333.github.io/mhyy.py/ 获取更多细节
 
 ## 关于
 
-欢迎协作本项目，如果你有任何意见或想法，请提出Issue。如果你喜欢，请给该仓库点一个Star
+欢迎协作本项目，如果你有任何意见或想法，请提出Issue。
+
+如果你喜欢此项目，请给该仓库点一个 Star 或提供一定的[捐助](https://afdian.net/a/GuangChen2333)。
```

