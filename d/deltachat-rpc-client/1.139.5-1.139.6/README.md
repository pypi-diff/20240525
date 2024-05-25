# Comparing `tmp/deltachat_rpc_client-1.139.5.tar.gz` & `tmp/deltachat_rpc_client-1.139.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deltachat_rpc_client-1.139.5.tar", last modified: Thu May 23 13:27:04 2024, max compression
+gzip compressed data, was "deltachat_rpc_client-1.139.6.tar", last modified: Sat May 25 07:07:54 2024, max compression
```

## Comparing `deltachat_rpc_client-1.139.5.tar` & `deltachat_rpc_client-1.139.6.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:27:04.353733 deltachat_rpc_client-1.139.5/
--rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-05-23 13:26:58.000000 deltachat_rpc_client-1.139.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-05-23 13:27:04.353733 deltachat_rpc_client-1.139.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-23 13:26:58.000000 deltachat_rpc_client-1.139.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-05-23 13:26:58.000000 deltachat_rpc_client-1.139.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 13:27:04.353733 deltachat_rpc_client-1.139.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:27:04.345734 deltachat_rpc_client-1.139.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:27:04.349733 deltachat_rpc_client-1.139.5/src/deltachat_rpc_client/
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-23 13:26:58.000000 deltachat_rpc_client-1.139.5/src/deltachat_rpc_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-05-23 13:26:58.000000 deltachat_rpc_client-1.139.5/src/deltachat_rpc_client/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13612 2024-05-23 13:26:58.000000 deltachat_rpc_client-1.139.5/src/deltachat_rpc_client/account.py
--rw-r--r--   0 runner    (1001) docker     (127)    10659 2024-05-23 13:26:58.000000 deltachat_rpc_client-1.139.5/src/deltachat_rpc_client/chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     7043 2024-05-23 13:26:58.000000 deltachat_rpc_client-1.139.5/src/deltachat_rpc_client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5360 2024-05-23 13:26:58.000000 deltachat_rpc_client-1.139.5/src/deltachat_rpc_client/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-05-23 13:26:58.000000 deltachat_rpc_client-1.139.5/src/deltachat_rpc_client/contact.py
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-23 13:26:58.000000 deltachat_rpc_client-1.139.5/src/deltachat_rpc_client/deltachat.py
--rw-r--r--   0 runner    (1001) docker     (127)     7808 2024-05-23 13:26:58.000000 deltachat_rpc_client-1.139.5/src/deltachat_rpc_client/direct_imap.py
--rw-r--r--   0 runner    (1001) docker     (127)     9877 2024-05-23 13:26:58.000000 deltachat_rpc_client-1.139.5/src/deltachat_rpc_client/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-05-23 13:26:58.000000 deltachat_rpc_client-1.139.5/src/deltachat_rpc_client/message.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-23 13:26:58.000000 deltachat_rpc_client-1.139.5/src/deltachat_rpc_client/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     4059 2024-05-23 13:26:58.000000 deltachat_rpc_client-1.139.5/src/deltachat_rpc_client/pytestplugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-05-23 13:26:58.000000 deltachat_rpc_client-1.139.5/src/deltachat_rpc_client/rpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:27:04.353733 deltachat_rpc_client-1.139.5/src/deltachat_rpc_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-05-23 13:27:04.000000 deltachat_rpc_client-1.139.5/src/deltachat_rpc_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-23 13:27:04.000000 deltachat_rpc_client-1.139.5/src/deltachat_rpc_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 13:27:04.000000 deltachat_rpc_client-1.139.5/src/deltachat_rpc_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-23 13:27:04.000000 deltachat_rpc_client-1.139.5/src/deltachat_rpc_client.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-23 13:27:04.000000 deltachat_rpc_client-1.139.5/src/deltachat_rpc_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-23 13:27:04.000000 deltachat_rpc_client-1.139.5/src/deltachat_rpc_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:27:04.353733 deltachat_rpc_client-1.139.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7409 2024-05-23 13:26:58.000000 deltachat_rpc_client-1.139.5/tests/test_chatlist_events.py
--rw-r--r--   0 runner    (1001) docker     (127)    24172 2024-05-23 13:26:58.000000 deltachat_rpc_client-1.139.5/tests/test_securejoin.py
--rw-r--r--   0 runner    (1001) docker     (127)    22129 2024-05-23 13:26:58.000000 deltachat_rpc_client-1.139.5/tests/test_something.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-23 13:26:58.000000 deltachat_rpc_client-1.139.5/tests/test_vcard.py
--rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-05-23 13:26:58.000000 deltachat_rpc_client-1.139.5/tests/test_webxdc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 07:07:54.358989 deltachat_rpc_client-1.139.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-05-25 07:07:45.000000 deltachat_rpc_client-1.139.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-05-25 07:07:54.358989 deltachat_rpc_client-1.139.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-25 07:07:45.000000 deltachat_rpc_client-1.139.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-05-25 07:07:45.000000 deltachat_rpc_client-1.139.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 07:07:54.358989 deltachat_rpc_client-1.139.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 07:07:54.354989 deltachat_rpc_client-1.139.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 07:07:54.354989 deltachat_rpc_client-1.139.6/src/deltachat_rpc_client/
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-25 07:07:45.000000 deltachat_rpc_client-1.139.6/src/deltachat_rpc_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-05-25 07:07:45.000000 deltachat_rpc_client-1.139.6/src/deltachat_rpc_client/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13612 2024-05-25 07:07:45.000000 deltachat_rpc_client-1.139.6/src/deltachat_rpc_client/account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10659 2024-05-25 07:07:45.000000 deltachat_rpc_client-1.139.6/src/deltachat_rpc_client/chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7043 2024-05-25 07:07:45.000000 deltachat_rpc_client-1.139.6/src/deltachat_rpc_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5360 2024-05-25 07:07:45.000000 deltachat_rpc_client-1.139.6/src/deltachat_rpc_client/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-05-25 07:07:45.000000 deltachat_rpc_client-1.139.6/src/deltachat_rpc_client/contact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-25 07:07:45.000000 deltachat_rpc_client-1.139.6/src/deltachat_rpc_client/deltachat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7808 2024-05-25 07:07:45.000000 deltachat_rpc_client-1.139.6/src/deltachat_rpc_client/direct_imap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9877 2024-05-25 07:07:45.000000 deltachat_rpc_client-1.139.6/src/deltachat_rpc_client/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-05-25 07:07:45.000000 deltachat_rpc_client-1.139.6/src/deltachat_rpc_client/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-25 07:07:45.000000 deltachat_rpc_client-1.139.6/src/deltachat_rpc_client/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     4059 2024-05-25 07:07:45.000000 deltachat_rpc_client-1.139.6/src/deltachat_rpc_client/pytestplugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-05-25 07:07:45.000000 deltachat_rpc_client-1.139.6/src/deltachat_rpc_client/rpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 07:07:54.358989 deltachat_rpc_client-1.139.6/src/deltachat_rpc_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-05-25 07:07:54.000000 deltachat_rpc_client-1.139.6/src/deltachat_rpc_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-25 07:07:54.000000 deltachat_rpc_client-1.139.6/src/deltachat_rpc_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 07:07:54.000000 deltachat_rpc_client-1.139.6/src/deltachat_rpc_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-25 07:07:54.000000 deltachat_rpc_client-1.139.6/src/deltachat_rpc_client.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-25 07:07:54.000000 deltachat_rpc_client-1.139.6/src/deltachat_rpc_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-25 07:07:54.000000 deltachat_rpc_client-1.139.6/src/deltachat_rpc_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 07:07:54.358989 deltachat_rpc_client-1.139.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7409 2024-05-25 07:07:45.000000 deltachat_rpc_client-1.139.6/tests/test_chatlist_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6220 2024-05-25 07:07:45.000000 deltachat_rpc_client-1.139.6/tests/test_iroh_webxdc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24172 2024-05-25 07:07:45.000000 deltachat_rpc_client-1.139.6/tests/test_securejoin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22129 2024-05-25 07:07:45.000000 deltachat_rpc_client-1.139.6/tests/test_something.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-25 07:07:45.000000 deltachat_rpc_client-1.139.6/tests/test_vcard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-05-25 07:07:45.000000 deltachat_rpc_client-1.139.6/tests/test_webxdc.py
```

### Comparing `deltachat_rpc_client-1.139.5/LICENSE` & `deltachat_rpc_client-1.139.6/LICENSE`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.139.5/PKG-INFO` & `deltachat_rpc_client-1.139.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deltachat-rpc-client
-Version: 1.139.5
+Version: 1.139.6
 Summary: Python client for Delta Chat core JSON-RPC interface
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python :: 3
```

### Comparing `deltachat_rpc_client-1.139.5/README.md` & `deltachat_rpc_client-1.139.6/README.md`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.139.5/pyproject.toml` & `deltachat_rpc_client-1.139.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=45"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "deltachat-rpc-client"
-version = "1.139.5"
+version = "1.139.6"
 description = "Python client for Delta Chat core JSON-RPC interface"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
     "Operating System :: POSIX :: Linux",
     "Operating System :: MacOS :: MacOS X",
```

### Comparing `deltachat_rpc_client-1.139.5/src/deltachat_rpc_client/__init__.py` & `deltachat_rpc_client-1.139.6/src/deltachat_rpc_client/__init__.py`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.139.5/src/deltachat_rpc_client/_utils.py` & `deltachat_rpc_client-1.139.6/src/deltachat_rpc_client/_utils.py`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.139.5/src/deltachat_rpc_client/account.py` & `deltachat_rpc_client-1.139.6/src/deltachat_rpc_client/account.py`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.139.5/src/deltachat_rpc_client/chat.py` & `deltachat_rpc_client-1.139.6/src/deltachat_rpc_client/chat.py`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.139.5/src/deltachat_rpc_client/client.py` & `deltachat_rpc_client-1.139.6/src/deltachat_rpc_client/client.py`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.139.5/src/deltachat_rpc_client/const.py` & `deltachat_rpc_client-1.139.6/src/deltachat_rpc_client/const.py`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.139.5/src/deltachat_rpc_client/contact.py` & `deltachat_rpc_client-1.139.6/src/deltachat_rpc_client/contact.py`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.139.5/src/deltachat_rpc_client/deltachat.py` & `deltachat_rpc_client-1.139.6/src/deltachat_rpc_client/deltachat.py`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.139.5/src/deltachat_rpc_client/direct_imap.py` & `deltachat_rpc_client-1.139.6/src/deltachat_rpc_client/direct_imap.py`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.139.5/src/deltachat_rpc_client/events.py` & `deltachat_rpc_client-1.139.6/src/deltachat_rpc_client/events.py`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.139.5/src/deltachat_rpc_client/message.py` & `deltachat_rpc_client-1.139.6/src/deltachat_rpc_client/message.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 from dataclasses import dataclass
 from typing import TYPE_CHECKING, Optional, Union
 
-from ._utils import AttrDict
+from ._utils import AttrDict, futuremethod
 from .const import EventType
 from .contact import Contact
 
 if TYPE_CHECKING:
     from .account import Account
     from .rpc import Rpc
 
@@ -67,12 +67,14 @@
     def wait_until_delivered(self) -> None:
         """Consume events until the message is delivered."""
         while True:
             event = self.account.wait_for_event()
             if event.kind == EventType.MSG_DELIVERED and event.msg_id == self.id:
                 break
 
-    def send_webxdc_realtime_advertisement(self) -> None:
-        self._rpc.send_webxdc_realtime_advertisement(self.account.id, self.id)
+    @futuremethod
+    def send_webxdc_realtime_advertisement(self):
+        yield self._rpc.send_webxdc_realtime_advertisement.future(self.account.id, self.id)
 
+    @futuremethod
     def send_webxdc_realtime_data(self, data) -> None:
-        self._rpc.send_webxdc_realtime_data(self.account.id, self.id, list(data))
+        yield self._rpc.send_webxdc_realtime_data.future(self.account.id, self.id, list(data))
```

### Comparing `deltachat_rpc_client-1.139.5/src/deltachat_rpc_client/pytestplugin.py` & `deltachat_rpc_client-1.139.6/src/deltachat_rpc_client/pytestplugin.py`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.139.5/src/deltachat_rpc_client/rpc.py` & `deltachat_rpc_client-1.139.6/src/deltachat_rpc_client/rpc.py`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.139.5/src/deltachat_rpc_client.egg-info/PKG-INFO` & `deltachat_rpc_client-1.139.6/src/deltachat_rpc_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deltachat-rpc-client
-Version: 1.139.5
+Version: 1.139.6
 Summary: Python client for Delta Chat core JSON-RPC interface
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python :: 3
```

### Comparing `deltachat_rpc_client-1.139.5/src/deltachat_rpc_client.egg-info/SOURCES.txt` & `deltachat_rpc_client-1.139.6/src/deltachat_rpc_client.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -18,11 +18,12 @@
 src/deltachat_rpc_client.egg-info/PKG-INFO
 src/deltachat_rpc_client.egg-info/SOURCES.txt
 src/deltachat_rpc_client.egg-info/dependency_links.txt
 src/deltachat_rpc_client.egg-info/entry_points.txt
 src/deltachat_rpc_client.egg-info/requires.txt
 src/deltachat_rpc_client.egg-info/top_level.txt
 tests/test_chatlist_events.py
+tests/test_iroh_webxdc.py
 tests/test_securejoin.py
 tests/test_something.py
 tests/test_vcard.py
 tests/test_webxdc.py
```

### Comparing `deltachat_rpc_client-1.139.5/tests/test_chatlist_events.py` & `deltachat_rpc_client-1.139.6/tests/test_chatlist_events.py`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.139.5/tests/test_securejoin.py` & `deltachat_rpc_client-1.139.6/tests/test_securejoin.py`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.139.5/tests/test_something.py` & `deltachat_rpc_client-1.139.6/tests/test_something.py`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.139.5/tests/test_vcard.py` & `deltachat_rpc_client-1.139.6/tests/test_vcard.py`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.139.5/tests/test_webxdc.py` & `deltachat_rpc_client-1.139.6/tests/test_webxdc.py`

 * *Files identical despite different names*

