# Comparing `tmp/hydra_cache-0.1.0.tar.gz` & `tmp/hydra_cache-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydra_cache-0.1.0.tar", last modified: Sat May 25 05:49:49 2024, max compression
+gzip compressed data, was "hydra_cache-0.1.1.tar", last modified: Sat May 25 06:47:32 2024, max compression
```

## Comparing `hydra_cache-0.1.0.tar` & `hydra_cache-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 harshvardhangoswami   (501) staff       (20)        0 2024-05-25 05:49:49.273460 hydra_cache-0.1.0/
--rw-r--r--   0 harshvardhangoswami   (501) staff       (20)        0 2024-05-25 04:49:07.000000 hydra_cache-0.1.0/LICENSE
--rw-r--r--   0 harshvardhangoswami   (501) staff       (20)     7397 2024-05-25 05:49:49.273176 hydra_cache-0.1.0/PKG-INFO
--rw-r--r--   0 harshvardhangoswami   (501) staff       (20)     6628 2024-05-25 05:42:50.000000 hydra_cache-0.1.0/README.md
--rw-r--r--   0 harshvardhangoswami   (501) staff       (20)       38 2024-05-25 05:49:49.273567 hydra_cache-0.1.0/setup.cfg
--rw-r--r--   0 harshvardhangoswami   (501) staff       (20)     1084 2024-05-25 05:44:23.000000 hydra_cache-0.1.0/setup.py
-drwxr-xr-x   0 harshvardhangoswami   (501) staff       (20)        0 2024-05-25 05:49:49.269249 hydra_cache-0.1.0/src/
-drwxr-xr-x   0 harshvardhangoswami   (501) staff       (20)        0 2024-05-25 05:49:49.270526 hydra_cache-0.1.0/src/hydra_cache/
--rw-r--r--   0 harshvardhangoswami   (501) staff       (20)        0 2024-05-25 04:49:59.000000 hydra_cache-0.1.0/src/hydra_cache/__init__.py
--rw-r--r--   0 harshvardhangoswami   (501) staff       (20)     2045 2024-05-25 05:01:45.000000 hydra_cache-0.1.0/src/hydra_cache/mixins.py
-drwxr-xr-x   0 harshvardhangoswami   (501) staff       (20)        0 2024-05-25 05:49:49.272285 hydra_cache-0.1.0/src/hydra_cache/utils/
--rw-r--r--   0 harshvardhangoswami   (501) staff       (20)        0 2024-05-25 04:59:07.000000 hydra_cache-0.1.0/src/hydra_cache/utils/__init__.py
--rw-r--r--   0 harshvardhangoswami   (501) staff       (20)      953 2024-05-25 05:03:38.000000 hydra_cache-0.1.0/src/hydra_cache/utils/cache.py
--rw-r--r--   0 harshvardhangoswami   (501) staff       (20)      271 2024-05-25 05:03:38.000000 hydra_cache-0.1.0/src/hydra_cache/utils/hasher.py
-drwxr-xr-x   0 harshvardhangoswami   (501) staff       (20)        0 2024-05-25 05:49:49.272552 hydra_cache-0.1.0/src/hydra_cache.egg-info/
--rw-r--r--   0 harshvardhangoswami   (501) staff       (20)     7397 2024-05-25 05:49:49.000000 hydra_cache-0.1.0/src/hydra_cache.egg-info/PKG-INFO
--rw-r--r--   0 harshvardhangoswami   (501) staff       (20)      371 2024-05-25 05:49:49.000000 hydra_cache-0.1.0/src/hydra_cache.egg-info/SOURCES.txt
--rw-r--r--   0 harshvardhangoswami   (501) staff       (20)        1 2024-05-25 05:49:49.000000 hydra_cache-0.1.0/src/hydra_cache.egg-info/dependency_links.txt
--rw-r--r--   0 harshvardhangoswami   (501) staff       (20)       15 2024-05-25 05:49:49.000000 hydra_cache-0.1.0/src/hydra_cache.egg-info/requires.txt
--rw-r--r--   0 harshvardhangoswami   (501) staff       (20)       12 2024-05-25 05:49:49.000000 hydra_cache-0.1.0/src/hydra_cache.egg-info/top_level.txt
+drwxr-xr-x   0 harshvardhangoswami   (501) staff       (20)        0 2024-05-25 06:47:32.980756 hydra_cache-0.1.1/
+-rw-r--r--   0 harshvardhangoswami   (501) staff       (20)        0 2024-05-25 04:49:07.000000 hydra_cache-0.1.1/LICENSE
+-rw-r--r--   0 harshvardhangoswami   (501) staff       (20)     7397 2024-05-25 06:47:32.980571 hydra_cache-0.1.1/PKG-INFO
+-rw-r--r--   0 harshvardhangoswami   (501) staff       (20)     6628 2024-05-25 05:42:50.000000 hydra_cache-0.1.1/README.md
+-rw-r--r--   0 harshvardhangoswami   (501) staff       (20)       38 2024-05-25 06:47:32.980806 hydra_cache-0.1.1/setup.cfg
+-rw-r--r--   0 harshvardhangoswami   (501) staff       (20)     1084 2024-05-25 06:41:24.000000 hydra_cache-0.1.1/setup.py
+drwxr-xr-x   0 harshvardhangoswami   (501) staff       (20)        0 2024-05-25 06:47:32.977944 hydra_cache-0.1.1/src/
+drwxr-xr-x   0 harshvardhangoswami   (501) staff       (20)        0 2024-05-25 06:47:32.978659 hydra_cache-0.1.1/src/hydra_cache/
+-rw-r--r--   0 harshvardhangoswami   (501) staff       (20)        0 2024-05-25 04:49:59.000000 hydra_cache-0.1.1/src/hydra_cache/__init__.py
+-rw-r--r--   0 harshvardhangoswami   (501) staff       (20)     2427 2024-05-25 06:46:56.000000 hydra_cache-0.1.1/src/hydra_cache/mixins.py
+drwxr-xr-x   0 harshvardhangoswami   (501) staff       (20)        0 2024-05-25 06:47:32.979994 hydra_cache-0.1.1/src/hydra_cache/utils/
+-rw-r--r--   0 harshvardhangoswami   (501) staff       (20)        0 2024-05-25 04:59:07.000000 hydra_cache-0.1.1/src/hydra_cache/utils/__init__.py
+-rw-r--r--   0 harshvardhangoswami   (501) staff       (20)      949 2024-05-25 06:41:46.000000 hydra_cache-0.1.1/src/hydra_cache/utils/cache.py
+-rw-r--r--   0 harshvardhangoswami   (501) staff       (20)      271 2024-05-25 05:03:38.000000 hydra_cache-0.1.1/src/hydra_cache/utils/hasher.py
+drwxr-xr-x   0 harshvardhangoswami   (501) staff       (20)        0 2024-05-25 06:47:32.980319 hydra_cache-0.1.1/src/hydra_cache.egg-info/
+-rw-r--r--   0 harshvardhangoswami   (501) staff       (20)     7397 2024-05-25 06:47:32.000000 hydra_cache-0.1.1/src/hydra_cache.egg-info/PKG-INFO
+-rw-r--r--   0 harshvardhangoswami   (501) staff       (20)      371 2024-05-25 06:47:32.000000 hydra_cache-0.1.1/src/hydra_cache.egg-info/SOURCES.txt
+-rw-r--r--   0 harshvardhangoswami   (501) staff       (20)        1 2024-05-25 06:47:32.000000 hydra_cache-0.1.1/src/hydra_cache.egg-info/dependency_links.txt
+-rw-r--r--   0 harshvardhangoswami   (501) staff       (20)       15 2024-05-25 06:47:32.000000 hydra_cache-0.1.1/src/hydra_cache.egg-info/requires.txt
+-rw-r--r--   0 harshvardhangoswami   (501) staff       (20)       12 2024-05-25 06:47:32.000000 hydra_cache-0.1.1/src/hydra_cache.egg-info/top_level.txt
```

### Comparing `hydra_cache-0.1.0/PKG-INFO` & `hydra_cache-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydra_cache
-Version: 0.1.0
+Version: 0.1.1
 Summary: A mixin that unleash the Kraken of DJANGO Caching Power
 Home-page: https://github.com/iamharshdev/hydra_cache
 Author: Harsh Vardhan Goswami
 Author-email: me@iamharsh.dev
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `hydra_cache-0.1.0/README.md` & `hydra_cache-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `hydra_cache-0.1.0/setup.py` & `hydra_cache-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="hydra_cache",
-    version="0.1.0",
+    version="0.1.1",
     author="Harsh Vardhan Goswami",
     author_email="me@iamharsh.dev",
     description="A mixin that unleash the Kraken of DJANGO Caching Power",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/iamharshdev/hydra_cache",
     packages=find_packages("src"),
```

### Comparing `hydra_cache-0.1.0/src/hydra_cache/mixins.py` & `hydra_cache-0.1.1/src/hydra_cache/mixins.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,33 @@
 from django.conf import settings
+from django.core.cache import cache
+from django.utils.cache import get_cache_key
 from django.views.decorators.cache import cache_page
 from django.views.decorators.vary import vary_on_headers
-from src.hydra_cache.utils.cache import flush_cache_for_keys
+from hydra_cache.utils.cache import flush_cache_for_keys
 
 
 class HydraCacheMixin:
     """
    A mixin that provides cache control functionality for Django views.
    """
     cache_key_prefix = None  # The prefix for the cache key
     disable_cache = False  # Flag to disable caching for the view
     cache_timeout = settings.CACHE_TIMEOUT  # Cache timeout in seconds
     vary_on_header = 'X-CustomHeader'  # HTTP header to vary the cache on
     match_on_cache_key = False  # Whether to use the generated cache key for cache clearing
     clear_cache_keys = []  # List of cache keys to clear on POST, PUT, DELETE, PATCH
     cache_hash_header = True  # Whether to use the header value in the cache key hash
 
+    def get_cache_key(self, request):
+        """
+        Return the cache key for the request.
+        """
+        return get_cache_key(request, self.cache_key_prefix, "GET", cache=cache)
+
     @classmethod
     def as_view(cls, **initkwargs):
         """
        Wrap the view with cache_page decorator and vary_on_headers if needed.
        """
         view = super().as_view(**initkwargs)
         if cls.disable_cache:
@@ -27,19 +35,22 @@
         view = vary_on_headers(cls.vary_on_header)(view) if cls.vary_on_header else view
         return cache_page(cls.cache_timeout, key_prefix=cls.cache_key_prefix)(view)
 
     def clear_cache(self, request):
         """
        Clear the cache for the current request.
        """
-        cache_keys = self.clear_cache_keys if self.clear_cache_keys else [self.cache_key_prefix]
+
+        cache_keys = self.clear_cache_keys if len(self.clear_cache_keys) > 0 else [self.cache_key_prefix]
         if self.match_on_cache_key:
             cache_key = self.cache_key_prefix
             cache_keys = [cache_key]
-        flush_cache_for_keys(cache_keys, request.META.get(f'HTTP_{self.vary_on_header.replace("-", "_").upper()}', ''))
+        else:
+            cache_keys = [self.get_cache_key(request)]
+        flush_cache_for_keys(cache_keys, request.META.get(f'HTTP_{self.vary_on_header.replace("-", "_").upper()}', '') if self.cache_hash_header else None)
 
     def dispatch(self, request, *args, **kwargs):
         """
        Dispatch the request and clear the cache if necessary.
        """
         response = super().dispatch(request, *args, **kwargs)
         if request.method in ["POST", "PUT", "DELETE", "PATCH"]:
```

### Comparing `hydra_cache-0.1.0/src/hydra_cache/utils/cache.py` & `hydra_cache-0.1.1/src/hydra_cache/utils/cache.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from django.core.cache import cache
 
-from src.hydra_cache.utils.hasher import md5
+from hydra_cache.utils.hasher import md5
 
 
 def flush_cache_for_keys(_keys, pre_hash=None):
     """
         Flushes the cache for the given keys.
 
         Args:
```

### Comparing `hydra_cache-0.1.0/src/hydra_cache.egg-info/PKG-INFO` & `hydra_cache-0.1.1/src/hydra_cache.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydra_cache
-Version: 0.1.0
+Version: 0.1.1
 Summary: A mixin that unleash the Kraken of DJANGO Caching Power
 Home-page: https://github.com/iamharshdev/hydra_cache
 Author: Harsh Vardhan Goswami
 Author-email: me@iamharsh.dev
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

