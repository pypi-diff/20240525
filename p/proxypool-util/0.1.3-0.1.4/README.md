# Comparing `tmp/proxypool_util-0.1.3.tar.gz` & `tmp/proxypool_util-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proxypool_util-0.1.3.tar", last modified: Thu May 23 17:09:38 2024, max compression
+gzip compressed data, was "proxypool_util-0.1.4.tar", last modified: Sat May 25 16:31:02 2024, max compression
```

## Comparing `proxypool_util-0.1.3.tar` & `proxypool_util-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 17:09:38.591871 proxypool_util-0.1.3/
--rw-rw-rw-   0        0        0     1093 2024-05-14 13:07:57.000000 proxypool_util-0.1.3/LICENCE
--rw-rw-rw-   0        0        0     2039 2024-05-23 17:09:38.590860 proxypool_util-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     1487 2024-05-14 14:21:10.000000 proxypool_util-0.1.3/README.md
--rw-rw-rw-   0        0        0      626 2024-05-23 17:09:11.000000 proxypool_util-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-23 17:09:38.591871 proxypool_util-0.1.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-23 17:09:38.534641 proxypool_util-0.1.3/src/
-drwxrwxrwx   0        0        0        0 2024-05-23 17:09:38.561932 proxypool_util-0.1.3/src/ProxyPool/
--rw-rw-rw-   0        0        0      234 2024-05-13 17:42:56.000000 proxypool_util-0.1.3/src/ProxyPool/ProxyExceptions.py
--rw-rw-rw-   0        0        0     5397 2024-05-23 17:09:11.000000 proxypool_util-0.1.3/src/ProxyPool/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 17:09:38.589019 proxypool_util-0.1.3/src/proxypool_util.egg-info/
--rw-rw-rw-   0        0        0     2039 2024-05-23 17:09:38.000000 proxypool_util-0.1.3/src/proxypool_util.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      303 2024-05-23 17:09:38.000000 proxypool_util-0.1.3/src/proxypool_util.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 17:09:38.000000 proxypool_util-0.1.3/src/proxypool_util.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-05-23 17:09:38.000000 proxypool_util-0.1.3/src/proxypool_util.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-23 17:09:38.586756 proxypool_util-0.1.3/tests/
--rw-rw-rw-   0        0        0     2658 2024-05-14 12:41:58.000000 proxypool_util-0.1.3/tests/test_Proxy.py
--rw-rw-rw-   0        0        0     2473 2024-05-14 12:41:58.000000 proxypool_util-0.1.3/tests/test_ProxyPool.py
+drwxrwxrwx   0        0        0        0 2024-05-25 16:31:02.835526 proxypool_util-0.1.4/
+-rw-rw-rw-   0        0        0     1093 2024-05-14 13:07:57.000000 proxypool_util-0.1.4/LICENCE
+-rw-rw-rw-   0        0        0     2039 2024-05-25 16:31:02.833518 proxypool_util-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1487 2024-05-14 14:21:10.000000 proxypool_util-0.1.4/README.md
+-rw-rw-rw-   0        0        0      626 2024-05-25 16:30:37.000000 proxypool_util-0.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-25 16:31:02.835526 proxypool_util-0.1.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-25 16:31:02.748791 proxypool_util-0.1.4/src/
+drwxrwxrwx   0        0        0        0 2024-05-25 16:31:02.775975 proxypool_util-0.1.4/src/ProxyPool/
+-rw-rw-rw-   0        0        0      234 2024-05-13 17:42:56.000000 proxypool_util-0.1.4/src/ProxyPool/ProxyExceptions.py
+-rw-rw-rw-   0        0        0     6455 2024-05-25 16:21:48.000000 proxypool_util-0.1.4/src/ProxyPool/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-25 16:31:02.833011 proxypool_util-0.1.4/src/proxypool_util.egg-info/
+-rw-rw-rw-   0        0        0     2039 2024-05-25 16:31:02.000000 proxypool_util-0.1.4/src/proxypool_util.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      303 2024-05-25 16:31:02.000000 proxypool_util-0.1.4/src/proxypool_util.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 16:31:02.000000 proxypool_util-0.1.4/src/proxypool_util.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-25 16:31:02.000000 proxypool_util-0.1.4/src/proxypool_util.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-25 16:31:02.830493 proxypool_util-0.1.4/tests/
+-rw-rw-rw-   0        0        0     2658 2024-05-14 12:41:58.000000 proxypool_util-0.1.4/tests/test_Proxy.py
+-rw-rw-rw-   0        0        0     4657 2024-05-25 16:30:19.000000 proxypool_util-0.1.4/tests/test_ProxyPool.py
```

### Comparing `proxypool_util-0.1.3/LICENCE` & `proxypool_util-0.1.4/LICENCE`

 * *Files identical despite different names*

### Comparing `proxypool_util-0.1.3/PKG-INFO` & `proxypool_util-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proxypool_util
-Version: 0.1.3
+Version: 0.1.4
 Summary: Proxy pool to rotate and manage proxies
 Author-email: Mykhailo Razbeiko <mykhailo.razb@gmail.com>
 Project-URL: Homepage, https://github.com/MykhailoRp/proxypool_util
 Project-URL: Issues, https://github.com/MykhailoRp/proxypool_util/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `proxypool_util-0.1.3/README.md` & `proxypool_util-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `proxypool_util-0.1.3/pyproject.toml` & `proxypool_util-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "proxypool_util"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   { name="Mykhailo Razbeiko", email="mykhailo.razb@gmail.com" },
 ]
 description = "Proxy pool to rotate and manage proxies"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `proxypool_util-0.1.3/src/ProxyPool/__init__.py` & `proxypool_util-0.1.4/src/ProxyPool/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 import time
+from threading import Lock, Condition
 from . import ProxyExceptions
 
 class _ProxyDict(dict):
     def __getitem__(self, item):
         try:
             return dict.__getitem__(self, item)
         except KeyError:
             raise ProxyExceptions.UnknownProxy(f"Unknown proxy: {item}")
 
 class ProxyPool:
 
-    def __init__(self, proxy_list: [str], *, max_give_outs = 0, max_time_outs = 0, max_uses = 0, time_out_on_use = 0):
+    def __init__(self, proxy_list: [str], *, max_give_outs = 0, max_time_outs = 0, max_uses = 0, time_out_on_use = 0, replenish_proxies_func = None):
 
         self.max_give_outs = max_give_outs
         self.max_time_outs = max_time_outs
         self.max_uses = max_uses
         self.time_out_on_use = time_out_on_use
 
+        self._replenish_condition = Condition()
+        self._replenish_lock = Lock()
+
+        self.replenish_proxies_func = replenish_proxies_func
+
         self._proxy_dict = _ProxyDict({
             a: ProxyData() for a in proxy_list
         })
 
     def __getitem__(self, item):
         return self._proxy_dict[item]
 
@@ -51,15 +57,19 @@
                 prox_counter += 1
 
         return prox_counter
 
     def Proxy(self, proxy = None):
         return Proxy(self, proxy)
 
-    def get_proxy(self, prev_proxy: str = None) -> str:
+    def get_proxy(self, prev_proxy: str = None, *, _replenish = True) -> str:
+
+        with self._replenish_condition:
+            while self._replenish_lock.locked():
+                self._replenish_condition.wait()
 
         min_timeout = None
 
         for proxy_str, prox_data in self._proxy_dict.items():
 
             if self.proxy_valid_to_give(prox_data):
 
@@ -71,14 +81,31 @@
                 return proxy_str
 
             if self.proxy_valid_to_give(prox_data, ignore_timeout=True):
                 assert isinstance(prox_data, ProxyData)
                 min_timeout = prox_data.timeout if min_timeout is None else min(min_timeout, prox_data.timeout)
 
         if min_timeout is None:
+
+            if self.replenish_proxies_func is not None and _replenish:
+                with self._replenish_condition:
+
+                    self._replenish_lock.acquire()
+
+                    try:
+                        self.replenish_proxies_func(self)
+                        self._replenish_lock.release()
+                        self._replenish_condition.notify_all()
+                    except Exception as e:
+                        self._replenish_lock.release()
+                        self._replenish_condition.notify_all()
+                        raise e
+
+                return self.get_proxy(prev_proxy = prev_proxy, _replenish = False)
+
             raise ProxyExceptions.NoValidProxies("No valid proxies available")
         else:
             raise ProxyExceptions.ProxiesTimeout(f"One proxy will be available at {min_timeout}", min_timeout)
 
 
     def proxy_valid_to_give(self, proxy, ignore_timeout = False):
```

### Comparing `proxypool_util-0.1.3/src/proxypool_util.egg-info/PKG-INFO` & `proxypool_util-0.1.4/src/proxypool_util.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proxypool_util
-Version: 0.1.3
+Version: 0.1.4
 Summary: Proxy pool to rotate and manage proxies
 Author-email: Mykhailo Razbeiko <mykhailo.razb@gmail.com>
 Project-URL: Homepage, https://github.com/MykhailoRp/proxypool_util
 Project-URL: Issues, https://github.com/MykhailoRp/proxypool_util/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `proxypool_util-0.1.3/tests/test_Proxy.py` & `proxypool_util-0.1.4/tests/test_Proxy.py`

 * *Files identical despite different names*

