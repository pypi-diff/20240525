# Comparing `tmp/aioqzone-1.8.2.dev3.tar.gz` & `tmp/aioqzone-1.8.3.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioqzone-1.8.2.dev3.tar", max compression
+gzip compressed data, was "aioqzone-1.8.3.dev1.tar", max compression
```

## Comparing `aioqzone-1.8.2.dev3.tar` & `aioqzone-1.8.3.dev1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0    34523 2024-05-19 05:55:11.669037 aioqzone-1.8.2.dev3/LICENSE
--rw-r--r--   0        0        0     3057 2024-05-19 05:55:11.669037 aioqzone-1.8.2.dev3/README.md
--rw-r--r--   0        0        0     2311 2024-05-19 05:55:11.673037 aioqzone-1.8.2.dev3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-19 05:55:11.673037 aioqzone-1.8.2.dev3/src/aioqzone/__init__.py
--rw-r--r--   0        0        0      175 2024-05-19 05:55:11.673037 aioqzone-1.8.2.dev3/src/aioqzone/api/__init__.py
--rw-r--r--   0        0        0       56 2024-05-19 05:55:11.673037 aioqzone-1.8.2.dev3/src/aioqzone/api/h5/__init__.py
--rw-r--r--   0        0        0     8707 2024-05-19 05:55:11.673037 aioqzone-1.8.2.dev3/src/aioqzone/api/h5/model.py
--rw-r--r--   0        0        0     6334 2024-05-19 05:55:11.673037 aioqzone-1.8.2.dev3/src/aioqzone/api/login/__init__.py
--rw-r--r--   0        0        0     2597 2024-05-19 05:55:11.673037 aioqzone-1.8.2.dev3/src/aioqzone/api/login/_base.py
--rw-r--r--   0        0        0      639 2024-05-19 05:55:11.673037 aioqzone-1.8.2.dev3/src/aioqzone/exception.py
--rw-r--r--   0        0        0      551 2024-05-19 05:55:11.673037 aioqzone-1.8.2.dev3/src/aioqzone/message.py
--rw-r--r--   0        0        0      164 2024-05-19 05:55:11.673037 aioqzone-1.8.2.dev3/src/aioqzone/model/__init__.py
--rw-r--r--   0        0        0     4475 2024-05-19 05:55:11.673037 aioqzone-1.8.2.dev3/src/aioqzone/model/api/__init__.py
--rw-r--r--   0        0        0     5696 2024-05-19 05:55:11.673037 aioqzone-1.8.2.dev3/src/aioqzone/model/api/feed.py
--rw-r--r--   0        0        0     2674 2024-05-19 05:55:11.673037 aioqzone-1.8.2.dev3/src/aioqzone/model/api/profile.py
--rw-r--r--   0        0        0     5864 2024-05-19 05:55:11.673037 aioqzone-1.8.2.dev3/src/aioqzone/model/api/request.py
--rw-r--r--   0        0        0     7895 2024-05-19 05:55:11.673037 aioqzone-1.8.2.dev3/src/aioqzone/model/api/response.py
--rw-r--r--   0        0        0     1439 2024-05-19 05:55:11.673037 aioqzone-1.8.2.dev3/src/aioqzone/model/protocol/__init__.py
--rw-r--r--   0        0        0      631 2024-05-19 05:55:11.673037 aioqzone-1.8.2.dev3/src/aioqzone/model/protocol/config.py
--rw-r--r--   0        0        0     1618 2024-05-19 05:55:11.673037 aioqzone-1.8.2.dev3/src/aioqzone/model/protocol/entity.py
--rw-r--r--   0        0        0       39 2024-05-19 05:55:11.673037 aioqzone-1.8.2.dev3/src/aioqzone/utils/__init__.py
--rw-r--r--   0        0        0     2654 2024-05-19 05:55:11.673037 aioqzone-1.8.2.dev3/src/aioqzone/utils/entity.py
--rw-r--r--   0        0        0      592 2024-05-19 05:55:11.673037 aioqzone-1.8.2.dev3/src/aioqzone/utils/regex.py
--rw-r--r--   0        0        0      940 2024-05-19 05:55:11.673037 aioqzone-1.8.2.dev3/src/aioqzone/utils/retry.py
--rw-r--r--   0        0        0     2769 2024-05-19 05:55:11.677037 aioqzone-1.8.2.dev3/src/aioqzone/utils/time.py
--rw-r--r--   0        0        0      146 2024-05-19 05:55:11.677037 aioqzone-1.8.2.dev3/src/qqqr/__init__.py
--rw-r--r--   0        0        0     4577 2024-05-19 05:55:11.677037 aioqzone-1.8.2.dev3/src/qqqr/base.py
--rw-r--r--   0        0        0     1440 2024-05-19 05:55:11.677037 aioqzone-1.8.2.dev3/src/qqqr/constant.py
--rw-r--r--   0        0        0     1361 2024-05-19 05:55:11.677037 aioqzone-1.8.2.dev3/src/qqqr/exception.py
--rw-r--r--   0        0        0     1667 2024-05-19 05:55:11.677037 aioqzone-1.8.2.dev3/src/qqqr/message.py
--rw-r--r--   0        0        0        8 2024-05-19 05:55:11.677037 aioqzone-1.8.2.dev3/src/qqqr/py.typed
--rw-r--r--   0        0        0     7513 2024-05-19 05:55:11.677037 aioqzone-1.8.2.dev3/src/qqqr/qr/__init__.py
--rw-r--r--   0        0        0      591 2024-05-19 05:55:11.677037 aioqzone-1.8.2.dev3/src/qqqr/qr/type.py
--rw-r--r--   0        0        0      611 2024-05-19 05:55:11.677037 aioqzone-1.8.2.dev3/src/qqqr/type.py
--rw-r--r--   0        0        0       93 2024-05-19 05:55:11.677037 aioqzone-1.8.2.dev3/src/qqqr/up/__init__.py
--rw-r--r--   0        0        0      892 2024-05-19 05:55:11.677037 aioqzone-1.8.2.dev3/src/qqqr/up/_model.py
--rw-r--r--   0        0        0     6128 2024-05-19 05:55:11.677037 aioqzone-1.8.2.dev3/src/qqqr/up/captcha/__init__.py
--rw-r--r--   0        0        0     1649 2024-05-19 05:55:11.677037 aioqzone-1.8.2.dev3/src/qqqr/up/captcha/_model.py
--rw-r--r--   0        0        0     3318 2024-05-19 05:55:11.677037 aioqzone-1.8.2.dev3/src/qqqr/up/captcha/capsess.py
--rw-r--r--   0        0        0      288 2024-05-19 05:55:11.677037 aioqzone-1.8.2.dev3/src/qqqr/up/captcha/pil_utils.py
--rw-r--r--   0        0        0       77 2024-05-19 05:55:11.677037 aioqzone-1.8.2.dev3/src/qqqr/up/captcha/select/__init__.py
--rw-r--r--   0        0        0     2935 2024-05-19 05:55:11.677037 aioqzone-1.8.2.dev3/src/qqqr/up/captcha/select/_types.py
--rw-r--r--   0        0        0       75 2024-05-19 05:55:11.677037 aioqzone-1.8.2.dev3/src/qqqr/up/captcha/slide/__init__.py
--rw-r--r--   0        0        0     5232 2024-05-19 05:55:11.677037 aioqzone-1.8.2.dev3/src/qqqr/up/captcha/slide/_types.py
--rw-r--r--   0        0        0     5249 2024-05-19 05:55:11.677037 aioqzone-1.8.2.dev3/src/qqqr/up/encrypt.py
--rw-r--r--   0        0        0     2489 2024-05-19 05:55:11.677037 aioqzone-1.8.2.dev3/src/qqqr/up/h5.py
--rw-r--r--   0        0        0    10320 2024-05-19 05:55:11.677037 aioqzone-1.8.2.dev3/src/qqqr/up/web.py
--rw-r--r--   0        0        0      204 2024-05-19 05:55:11.677037 aioqzone-1.8.2.dev3/src/qqqr/utils/encrypt.py
--rw-r--r--   0        0        0      726 2024-05-19 05:55:11.677037 aioqzone-1.8.2.dev3/src/qqqr/utils/iter.py
--rw-r--r--   0        0        0     2062 2024-05-19 05:55:11.677037 aioqzone-1.8.2.dev3/src/qqqr/utils/jsjson.py
--rw-r--r--   0        0        0     1511 2024-05-19 05:55:11.677037 aioqzone-1.8.2.dev3/src/qqqr/utils/net.py
--rw-r--r--   0        0        0     4694 1970-01-01 00:00:00.000000 aioqzone-1.8.2.dev3/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-05-25 08:56:08.607707 aioqzone-1.8.3.dev1/LICENSE
+-rw-r--r--   0        0        0     3057 2024-05-25 08:56:08.607707 aioqzone-1.8.3.dev1/README.md
+-rw-r--r--   0        0        0     2311 2024-05-25 08:56:08.611707 aioqzone-1.8.3.dev1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-25 08:56:08.611707 aioqzone-1.8.3.dev1/src/aioqzone/__init__.py
+-rw-r--r--   0        0        0      175 2024-05-25 08:56:08.611707 aioqzone-1.8.3.dev1/src/aioqzone/api/__init__.py
+-rw-r--r--   0        0        0       56 2024-05-25 08:56:08.611707 aioqzone-1.8.3.dev1/src/aioqzone/api/h5/__init__.py
+-rw-r--r--   0        0        0     8707 2024-05-25 08:56:08.615707 aioqzone-1.8.3.dev1/src/aioqzone/api/h5/model.py
+-rw-r--r--   0        0        0     6334 2024-05-25 08:56:08.615707 aioqzone-1.8.3.dev1/src/aioqzone/api/login/__init__.py
+-rw-r--r--   0        0        0     2597 2024-05-25 08:56:08.615707 aioqzone-1.8.3.dev1/src/aioqzone/api/login/_base.py
+-rw-r--r--   0        0        0      639 2024-05-25 08:56:08.615707 aioqzone-1.8.3.dev1/src/aioqzone/exception.py
+-rw-r--r--   0        0        0      551 2024-05-25 08:56:08.615707 aioqzone-1.8.3.dev1/src/aioqzone/message.py
+-rw-r--r--   0        0        0      164 2024-05-25 08:56:08.615707 aioqzone-1.8.3.dev1/src/aioqzone/model/__init__.py
+-rw-r--r--   0        0        0     4475 2024-05-25 08:56:08.615707 aioqzone-1.8.3.dev1/src/aioqzone/model/api/__init__.py
+-rw-r--r--   0        0        0     5696 2024-05-25 08:56:08.615707 aioqzone-1.8.3.dev1/src/aioqzone/model/api/feed.py
+-rw-r--r--   0        0        0     2674 2024-05-25 08:56:08.615707 aioqzone-1.8.3.dev1/src/aioqzone/model/api/profile.py
+-rw-r--r--   0        0        0     5864 2024-05-25 08:56:08.615707 aioqzone-1.8.3.dev1/src/aioqzone/model/api/request.py
+-rw-r--r--   0        0        0     7895 2024-05-25 08:56:08.615707 aioqzone-1.8.3.dev1/src/aioqzone/model/api/response.py
+-rw-r--r--   0        0        0     1439 2024-05-25 08:56:08.615707 aioqzone-1.8.3.dev1/src/aioqzone/model/protocol/__init__.py
+-rw-r--r--   0        0        0      716 2024-05-25 08:56:08.615707 aioqzone-1.8.3.dev1/src/aioqzone/model/protocol/config.py
+-rw-r--r--   0        0        0     1618 2024-05-25 08:56:08.615707 aioqzone-1.8.3.dev1/src/aioqzone/model/protocol/entity.py
+-rw-r--r--   0        0        0       39 2024-05-25 08:56:08.615707 aioqzone-1.8.3.dev1/src/aioqzone/utils/__init__.py
+-rw-r--r--   0        0        0     2654 2024-05-25 08:56:08.615707 aioqzone-1.8.3.dev1/src/aioqzone/utils/entity.py
+-rw-r--r--   0        0        0      592 2024-05-25 08:56:08.615707 aioqzone-1.8.3.dev1/src/aioqzone/utils/regex.py
+-rw-r--r--   0        0        0      940 2024-05-25 08:56:08.615707 aioqzone-1.8.3.dev1/src/aioqzone/utils/retry.py
+-rw-r--r--   0        0        0     2769 2024-05-25 08:56:08.615707 aioqzone-1.8.3.dev1/src/aioqzone/utils/time.py
+-rw-r--r--   0        0        0      179 2024-05-25 08:56:08.615707 aioqzone-1.8.3.dev1/src/qqqr/__init__.py
+-rw-r--r--   0        0        0     4577 2024-05-25 08:56:08.615707 aioqzone-1.8.3.dev1/src/qqqr/base.py
+-rw-r--r--   0        0        0     1440 2024-05-25 08:56:08.615707 aioqzone-1.8.3.dev1/src/qqqr/constant.py
+-rw-r--r--   0        0        0     1361 2024-05-25 08:56:08.615707 aioqzone-1.8.3.dev1/src/qqqr/exception.py
+-rw-r--r--   0        0        0     1667 2024-05-25 08:56:08.615707 aioqzone-1.8.3.dev1/src/qqqr/message.py
+-rw-r--r--   0        0        0        8 2024-05-25 08:56:08.615707 aioqzone-1.8.3.dev1/src/qqqr/py.typed
+-rw-r--r--   0        0        0     9228 2024-05-25 08:56:08.615707 aioqzone-1.8.3.dev1/src/qqqr/qr/__init__.py
+-rw-r--r--   0        0        0      591 2024-05-25 08:56:08.615707 aioqzone-1.8.3.dev1/src/qqqr/qr/type.py
+-rw-r--r--   0        0        0      611 2024-05-25 08:56:08.615707 aioqzone-1.8.3.dev1/src/qqqr/type.py
+-rw-r--r--   0        0        0       93 2024-05-25 08:56:08.615707 aioqzone-1.8.3.dev1/src/qqqr/up/__init__.py
+-rw-r--r--   0        0        0      892 2024-05-25 08:56:08.615707 aioqzone-1.8.3.dev1/src/qqqr/up/_model.py
+-rw-r--r--   0        0        0     6128 2024-05-25 08:56:08.615707 aioqzone-1.8.3.dev1/src/qqqr/up/captcha/__init__.py
+-rw-r--r--   0        0        0     1649 2024-05-25 08:56:08.615707 aioqzone-1.8.3.dev1/src/qqqr/up/captcha/_model.py
+-rw-r--r--   0        0        0     3318 2024-05-25 08:56:08.615707 aioqzone-1.8.3.dev1/src/qqqr/up/captcha/capsess.py
+-rw-r--r--   0        0        0      288 2024-05-25 08:56:08.615707 aioqzone-1.8.3.dev1/src/qqqr/up/captcha/pil_utils.py
+-rw-r--r--   0        0        0       77 2024-05-25 08:56:08.615707 aioqzone-1.8.3.dev1/src/qqqr/up/captcha/select/__init__.py
+-rw-r--r--   0        0        0     2935 2024-05-25 08:56:08.615707 aioqzone-1.8.3.dev1/src/qqqr/up/captcha/select/_types.py
+-rw-r--r--   0        0        0       75 2024-05-25 08:56:08.615707 aioqzone-1.8.3.dev1/src/qqqr/up/captcha/slide/__init__.py
+-rw-r--r--   0        0        0     5232 2024-05-25 08:56:08.615707 aioqzone-1.8.3.dev1/src/qqqr/up/captcha/slide/_types.py
+-rw-r--r--   0        0        0     5249 2024-05-25 08:56:08.615707 aioqzone-1.8.3.dev1/src/qqqr/up/encrypt.py
+-rw-r--r--   0        0        0     2489 2024-05-25 08:56:08.615707 aioqzone-1.8.3.dev1/src/qqqr/up/h5.py
+-rw-r--r--   0        0        0    10566 2024-05-25 08:56:08.615707 aioqzone-1.8.3.dev1/src/qqqr/up/web.py
+-rw-r--r--   0        0        0      204 2024-05-25 08:56:08.615707 aioqzone-1.8.3.dev1/src/qqqr/utils/encrypt.py
+-rw-r--r--   0        0        0      726 2024-05-25 08:56:08.615707 aioqzone-1.8.3.dev1/src/qqqr/utils/iter.py
+-rw-r--r--   0        0        0     2062 2024-05-25 08:56:08.615707 aioqzone-1.8.3.dev1/src/qqqr/utils/jsjson.py
+-rw-r--r--   0        0        0     1511 2024-05-25 08:56:08.615707 aioqzone-1.8.3.dev1/src/qqqr/utils/net.py
+-rw-r--r--   0        0        0     4694 1970-01-01 00:00:00.000000 aioqzone-1.8.3.dev1/PKG-INFO
```

### Comparing `aioqzone-1.8.2.dev3/LICENSE` & `aioqzone-1.8.3.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `aioqzone-1.8.2.dev3/README.md` & `aioqzone-1.8.3.dev1/README.md`

 * *Files identical despite different names*

### Comparing `aioqzone-1.8.2.dev3/pyproject.toml` & `aioqzone-1.8.3.dev1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aioqzone"
-version = "1.8.2.dev3"
+version = "1.8.3.dev1"
 description = "A Python wrapper for Qzone login and H5 APIs."
 authors = ["aioqzone <zzzzss990315@gmail.com>"]
 license = "AGPL-3.0"
 readme = "README.md"
 homepage = "https://github.com/aioqzone/aioqzone"
 repository = "https://github.com/aioqzone/aioqzone"
 documentation = "https://aioqzone.github.io/aioqzone"
```

### Comparing `aioqzone-1.8.2.dev3/src/aioqzone/api/h5/model.py` & `aioqzone-1.8.3.dev1/src/aioqzone/api/h5/model.py`

 * *Files identical despite different names*

### Comparing `aioqzone-1.8.2.dev3/src/aioqzone/api/login/__init__.py` & `aioqzone-1.8.3.dev1/src/aioqzone/api/login/__init__.py`

 * *Files identical despite different names*

### Comparing `aioqzone-1.8.2.dev3/src/aioqzone/api/login/_base.py` & `aioqzone-1.8.3.dev1/src/aioqzone/api/login/_base.py`

 * *Files identical despite different names*

### Comparing `aioqzone-1.8.2.dev3/src/aioqzone/exception.py` & `aioqzone-1.8.3.dev1/src/aioqzone/exception.py`

 * *Files identical despite different names*

### Comparing `aioqzone-1.8.2.dev3/src/aioqzone/message.py` & `aioqzone-1.8.3.dev1/src/aioqzone/message.py`

 * *Files identical despite different names*

### Comparing `aioqzone-1.8.2.dev3/src/aioqzone/model/api/__init__.py` & `aioqzone-1.8.3.dev1/src/aioqzone/model/api/__init__.py`

 * *Files identical despite different names*

### Comparing `aioqzone-1.8.2.dev3/src/aioqzone/model/api/feed.py` & `aioqzone-1.8.3.dev1/src/aioqzone/model/api/feed.py`

 * *Files identical despite different names*

### Comparing `aioqzone-1.8.2.dev3/src/aioqzone/model/api/profile.py` & `aioqzone-1.8.3.dev1/src/aioqzone/model/api/profile.py`

 * *Files identical despite different names*

### Comparing `aioqzone-1.8.2.dev3/src/aioqzone/model/api/request.py` & `aioqzone-1.8.3.dev1/src/aioqzone/model/api/request.py`

 * *Files identical despite different names*

### Comparing `aioqzone-1.8.2.dev3/src/aioqzone/model/api/response.py` & `aioqzone-1.8.3.dev1/src/aioqzone/model/api/response.py`

 * *Files identical despite different names*

### Comparing `aioqzone-1.8.2.dev3/src/aioqzone/model/protocol/__init__.py` & `aioqzone-1.8.3.dev1/src/aioqzone/model/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `aioqzone-1.8.2.dev3/src/aioqzone/model/protocol/config.py` & `aioqzone-1.8.3.dev1/src/aioqzone/model/protocol/config.py`

 * *Files 24% similar despite different names*

```diff
@@ -22,7 +22,9 @@
 
 
 class QrLoginConfig(LoginConfig):
     max_refresh_times: int = 6
     """Maximum QR code refresh times."""
     poll_freq: float = 3
     """QR status polling interval."""
+    no_push: bool = False
+    """Do not try to push the QR code to user's client."""
```

### Comparing `aioqzone-1.8.2.dev3/src/aioqzone/model/protocol/entity.py` & `aioqzone-1.8.3.dev1/src/aioqzone/model/protocol/entity.py`

 * *Files identical despite different names*

### Comparing `aioqzone-1.8.2.dev3/src/aioqzone/utils/entity.py` & `aioqzone-1.8.3.dev1/src/aioqzone/utils/entity.py`

 * *Files identical despite different names*

### Comparing `aioqzone-1.8.2.dev3/src/aioqzone/utils/regex.py` & `aioqzone-1.8.3.dev1/src/aioqzone/utils/regex.py`

 * *Files identical despite different names*

### Comparing `aioqzone-1.8.2.dev3/src/aioqzone/utils/retry.py` & `aioqzone-1.8.3.dev1/src/aioqzone/utils/retry.py`

 * *Files identical despite different names*

### Comparing `aioqzone-1.8.2.dev3/src/aioqzone/utils/time.py` & `aioqzone-1.8.3.dev1/src/aioqzone/utils/time.py`

 * *Files identical despite different names*

### Comparing `aioqzone-1.8.2.dev3/src/qqqr/base.py` & `aioqzone-1.8.3.dev1/src/qqqr/base.py`

 * *Files identical despite different names*

### Comparing `aioqzone-1.8.2.dev3/src/qqqr/constant.py` & `aioqzone-1.8.3.dev1/src/qqqr/constant.py`

 * *Files identical despite different names*

### Comparing `aioqzone-1.8.2.dev3/src/qqqr/exception.py` & `aioqzone-1.8.3.dev1/src/qqqr/exception.py`

 * *Files identical despite different names*

### Comparing `aioqzone-1.8.2.dev3/src/qqqr/message.py` & `aioqzone-1.8.3.dev1/src/qqqr/message.py`

 * *Files identical despite different names*

### Comparing `aioqzone-1.8.2.dev3/src/qqqr/qr/__init__.py` & `aioqzone-1.8.3.dev1/src/qqqr/qr/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,55 +24,84 @@
 RECENT_UIN_URL = "https://ssl.ptlogin2.qq.com/pt_fetch_dev_uin"
 
 PTLOGIN2 = URL("https://ptlogin2.qq.com")
 
 
 @dataclass(unsafe_hash=True)
 class QR:
+    """Class :class:`QR` represents a QR code."""
+
     png: t.Optional[bytes]
-    """If None, the QR is pushed to user's client."""
+    """QR code content. If None, the QR is pushed to user's client."""
     sig: str
     expired: bool = False
+    """Whether the QR code is expired."""
 
     @property
     def pushed(self):
+        """Whether the QR code is pushed to user's client."""
         return self.png is None
 
 
 class QrSession(LoginSession):
     def __init__(
         self,
         first_qr: QR,
         login_sig: str,
         *,
         create_time: t.Optional[float] = None,
         refresh_times: int = 0,
     ) -> None:
         super().__init__(login_sig=login_sig, create_time=create_time)
         self.refreshed = refresh_times
+        """QR code refresh times counter."""
         self.current_qr = first_qr
+        """A :class:`QrSession` keeps a :class:`QR` object as current QR code."""
 
     def new_qr(self, qr: QR):
+        """Add a new QR code to this session."""
         self.current_qr.expired = True
         self.current_qr = qr
         self.refreshed += 1
 
 
 class _QrHookMixin:
     def __init__(self, *args, **kwds) -> None:
         super().__init__(*args, **kwds)
         self.qr_fetched = MT.qr_fetched.with_timeout(60)
+        """This emitter is triggered when a QR code is fetched."""
         self.qr_cancelled = MT.qr_cancelled()
+        """This emitter is triggered when QR login is cancelled."""
         self.cancel = asyncio.Event()
+        """Async-event indicating whether the loop should cancel the QR login."""
         self.refresh = asyncio.Event()
+        """Async-event indicating whether the loop should refresh the QR code immediately."""
 
 
 class QrLogin(LoginBase[QrSession], _QrHookMixin):
-    async def new(self) -> QrSession:
+    async def new(self, no_push=False) -> QrSession:
+        """Create a :class:`QrSession`. This method will:
+
+        1. GET ``xlogin`` url to get ``pt_login_sig`` cookie;
+
+        #. Try "quick login" (the QR code is pushed to user's client);
+
+        #. Whether the QR code is pushed or not, a :class:`QR` object is created
+           and is hold by the returned :class:`QrSession`.
+
+        :param no_push: Do not try to push the QR code to user's client.
+        :return: a :class:`QrSession`
+
+        .. versionchanged:: 1.8.3
+
+            Added :obj:`no_push` param.
+        """
         login_sig = await self._pt_login_sig()
+        if no_push:
+            return QrSession(await self.show(), login_sig=login_sig)
 
         cookie = self.client.cookie_jar.filter_cookies(PTLOGIN2).get("pt_guid_sig")
         push_qr = False
         if cookie is None or not cookie.value:
             log.debug("pt_guid_sig not found, skip pt_fetch_dev_uin")
         else:
             params = dict(r=random(), pt_guid_token=hash33(cookie.value))
@@ -84,17 +113,18 @@
             if m:
                 r = FetchDevUinResp.model_validate_json(m.group(1))
                 push_qr = r.code == 22028 and dev_mid_sig is not None and self.uin in r.uin_list
 
         return QrSession(await self.show(push_qr), login_sig=login_sig)
 
     async def show(self, push_qr=False) -> QR:
-        """``ptqrshow`` api.
+        """This method will call ``ptqrshow`` api and wrap the response QR bytes into :class:`QR`.
 
         :param push_qr: push QR to mobile client.
+        :return: a :class:`QR` object.
         """
         data = {
             "appid": self.app.appid,
             "daid": self.app.daid,
             "pt_3rd_aid": 0,
             "t": random(),
             "u1": self.proxy.s_url,
@@ -166,34 +196,45 @@
         return resp
 
     async def login(
         self,
         *,
         refresh_times: int = 6,
         poll_freq: float = 3,
+        no_push=False,
     ):
-        """Loop until cookie is returned or max `refresh_times` exceeds.
+        """Loop until cookie is returned or max :obj:`refresh_times` exceeds.
+
         - This method will emit :obj:`.qr_fetched` event if a new qrcode is fetched.
-        - If qr is not scanned after `refresh_times`, it will raise :exc:`UserTimeout`.
+
+        - If the QR code is not scanned after :obj:`refresh_times`,
+          it will raise :exc:`~qqqr.exception.UserTimeout`.
+
         - If :obj:`.refresh` is set, it will refresh qrcode at once without increasing expire counter.
-        - If :obj:`.cancel` is set, it will raise :exc:`UserBreak` before next polling.
+
+        - If :obj:`.cancel` is set, it will raise :exc:`~qqqr.exception.UserBreak` before next polling.
 
         :meta public:
         :param refresh_times: max qr expire times.
         :param poll_freq: interval between two status polling, in seconds, default as 3.
+        :param no_push: Do not try to push the QR code to user's client.
 
-        :raise `UserTimeout`: if qr is not scanned after `refresh_times` expires.
+        :raise `UserTimeout`: if the QR code is not scanned after :obj:`refresh_times` expires.
         :raise `UserBreak`: if :obj:`.cancel` is set.
+
+        .. versionchanged:: 1.8.3
+
+            Added :obj:`no_push` param.
         """
         self.refresh.clear()
         self.cancel.clear()
 
         cnt_expire = 0
         renew = False
-        sess = await self.new()
+        sess = await self.new(no_push)
 
         while cnt_expire < refresh_times:
             # BUG: should we wrap hook errors here?
             await self.qr_fetched.emit_suppress_timeout(
                 png=sess.current_qr.png, times=cnt_expire, qr_renew=renew
             )
             renew = False
@@ -202,14 +243,15 @@
                 if self.cancel.is_set():
                     await self.qr_cancelled.emit()
                     raise UserBreak
 
                 await asyncio.sleep(poll_freq)
                 stat = await self.poll(sess)
                 if stat.code == StatusCode.Expired:
+                    sess.current_qr.expired = True
                     cnt_expire += 1
                     break
                 elif stat.code == StatusCode.Authenticated:
                     sess.login_url = str(stat.url)
                     return await self._get_login_url(
                         sess,
                         cur_cookies=stat.cookies and stat.cookies.model_dump(),
```

### Comparing `aioqzone-1.8.2.dev3/src/qqqr/qr/type.py` & `aioqzone-1.8.3.dev1/src/qqqr/qr/type.py`

 * *Files identical despite different names*

### Comparing `aioqzone-1.8.2.dev3/src/qqqr/type.py` & `aioqzone-1.8.3.dev1/src/qqqr/type.py`

 * *Files identical despite different names*

### Comparing `aioqzone-1.8.2.dev3/src/qqqr/up/_model.py` & `aioqzone-1.8.3.dev1/src/qqqr/up/_model.py`

 * *Files identical despite different names*

### Comparing `aioqzone-1.8.2.dev3/src/qqqr/up/captcha/__init__.py` & `aioqzone-1.8.3.dev1/src/qqqr/up/captcha/__init__.py`

 * *Files identical despite different names*

### Comparing `aioqzone-1.8.2.dev3/src/qqqr/up/captcha/_model.py` & `aioqzone-1.8.3.dev1/src/qqqr/up/captcha/_model.py`

 * *Files identical despite different names*

### Comparing `aioqzone-1.8.2.dev3/src/qqqr/up/captcha/capsess.py` & `aioqzone-1.8.3.dev1/src/qqqr/up/captcha/capsess.py`

 * *Files identical despite different names*

### Comparing `aioqzone-1.8.2.dev3/src/qqqr/up/captcha/select/_types.py` & `aioqzone-1.8.3.dev1/src/qqqr/up/captcha/select/_types.py`

 * *Files identical despite different names*

### Comparing `aioqzone-1.8.2.dev3/src/qqqr/up/captcha/slide/_types.py` & `aioqzone-1.8.3.dev1/src/qqqr/up/captcha/slide/_types.py`

 * *Files identical despite different names*

### Comparing `aioqzone-1.8.2.dev3/src/qqqr/up/encrypt.py` & `aioqzone-1.8.3.dev1/src/qqqr/up/encrypt.py`

 * *Files identical despite different names*

### Comparing `aioqzone-1.8.2.dev3/src/qqqr/up/h5.py` & `aioqzone-1.8.3.dev1/src/qqqr/up/h5.py`

 * *Files identical despite different names*

### Comparing `aioqzone-1.8.2.dev3/src/qqqr/up/web.py` & `aioqzone-1.8.3.dev1/src/qqqr/up/web.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,14 +95,15 @@
         log.info("成功通过验证码")
 
 
 class _UpHookMixin:
     def __init__(self, *args, **kwds) -> None:
         super().__init__(*args, **kwds)
         self.sms_code_input = MT.sms_code_input.with_timeout(60)
+        """This emitter is triggered when SMS verify code is needed during login."""
 
 
 class UpWebLogin(LoginBase[UpWebSession], _UpHookMixin):
     """
     .. versionchanged:: 0.12.4
 
         `TeaEncoder` is used as the default password encoder. A `legacy_encoder` paramater is added to force
@@ -128,25 +129,29 @@
         super().__init__(client, uin=uin, h5=h5, app=app, proxy=proxy, info=info)
         self.pwd = pwd
         self.pwder = TeaEncoder(pwd)
         self.captcha = Captcha(
             self.client, self.app.appid, str(self.login_page_url), fake_ip=fake_ip
         )
 
-    async def new(self):
-        """Create a :class:`UpWebSession`. This will call `check` api of Qzone, and receive result
-        about whether this login needs a captcha, sms verification, etc.
+    async def new(self) -> UpWebSession:
+        """Create a :class:`UpWebSession`. This will trigger a GET to ``xlogin`` url.
 
         :raise `aiohttp.ClientResponseError`: if response status != 200
 
         :return: a up login session
         """
         return UpWebSession(await self._pt_login_sig())
 
     async def check(self, sess: UpWebSession):
+        """This will call ``check`` api of Qzone, and receive result about
+        whether this login needs a captcha, sms verification, etc.
+
+        :param sess: Session got from :meth:`~UpWebLogin.new`.
+        """
         data = {
             "regmaster": "",
             "pt_tea": 2,
             "pt_vcode": 1,
             "uin": self.uin,
             "appid": self.app.appid,
             # 'js_ver': 21072114,
@@ -213,15 +218,15 @@
             "ptdrvs": sess.check_rst.ptdrvs,
             "sid": sess.check_rst.session,
             "o1vId": await self.deviceId(),
         }
         data.update(const)
         return data
 
-    async def try_login(self, sess: UpWebSession):
+    async def try_login(self, sess: UpWebSession) -> LoginResp:
         """
         Check if current session meets the login condition.
         It takes a session object and returns response of this try.
 
         :param sess: Store the session information
         :return: A login response
         """
```

### Comparing `aioqzone-1.8.2.dev3/src/qqqr/utils/iter.py` & `aioqzone-1.8.3.dev1/src/qqqr/utils/iter.py`

 * *Files identical despite different names*

### Comparing `aioqzone-1.8.2.dev3/src/qqqr/utils/jsjson.py` & `aioqzone-1.8.3.dev1/src/qqqr/utils/jsjson.py`

 * *Files identical despite different names*

### Comparing `aioqzone-1.8.2.dev3/src/qqqr/utils/net.py` & `aioqzone-1.8.3.dev1/src/qqqr/utils/net.py`

 * *Files identical despite different names*

### Comparing `aioqzone-1.8.2.dev3/PKG-INFO` & `aioqzone-1.8.3.dev1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioqzone
-Version: 1.8.2.dev3
+Version: 1.8.3.dev1
 Summary: A Python wrapper for Qzone login and H5 APIs.
 Home-page: https://github.com/aioqzone/aioqzone
 License: AGPL-3.0
 Keywords: qzone-api,autologin,asyncio-spider
 Author: aioqzone
 Author-email: zzzzss990315@gmail.com
 Requires-Python: >=3.8,<4.0
```

