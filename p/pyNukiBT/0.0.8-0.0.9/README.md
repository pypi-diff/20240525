# Comparing `tmp/pyNukiBT-0.0.8.tar.gz` & `tmp/pyNukiBT-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyNukiBT-0.0.8.tar", last modified: Thu Mar 28 21:56:43 2024, max compression
+gzip compressed data, was "pyNukiBT-0.0.9.tar", last modified: Sat Mar 30 19:37:46 2024, max compression
```

## Comparing `pyNukiBT-0.0.8.tar` & `pyNukiBT-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 21:56:43.712063 pyNukiBT-0.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 21:56:43.708063 pyNukiBT-0.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 21:56:43.712063 pyNukiBT-0.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-03-28 21:56:31.000000 pyNukiBT-0.0.8/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-03-28 21:56:31.000000 pyNukiBT-0.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-03-28 21:56:31.000000 pyNukiBT-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-03-28 21:56:43.712063 pyNukiBT-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-03-28 21:56:31.000000 pyNukiBT-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 21:56:43.712063 pyNukiBT-0.0.8/pyNukiBT/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-03-28 21:56:31.000000 pyNukiBT-0.0.8/pyNukiBT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    39005 2024-03-28 21:56:31.000000 pyNukiBT-0.0.8/pyNukiBT/const.py
--rw-r--r--   0 runner    (1001) docker     (127)    24727 2024-03-28 21:56:31.000000 pyNukiBT-0.0.8/pyNukiBT/nuki.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 21:56:43.712063 pyNukiBT-0.0.8/pyNukiBT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-03-28 21:56:43.000000 pyNukiBT-0.0.8/pyNukiBT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-03-28 21:56:43.000000 pyNukiBT-0.0.8/pyNukiBT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 21:56:43.000000 pyNukiBT-0.0.8/pyNukiBT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-28 21:56:43.000000 pyNukiBT-0.0.8/pyNukiBT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-28 21:56:43.000000 pyNukiBT-0.0.8/pyNukiBT.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-03-28 21:56:31.000000 pyNukiBT-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-28 21:56:31.000000 pyNukiBT-0.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 21:56:43.712063 pyNukiBT-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 19:37:46.105359 pyNukiBT-0.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 19:37:46.105359 pyNukiBT-0.0.9/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-03-30 19:37:41.000000 pyNukiBT-0.0.9/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 19:37:46.105359 pyNukiBT-0.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-03-30 19:37:41.000000 pyNukiBT-0.0.9/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-03-30 19:37:41.000000 pyNukiBT-0.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-03-30 19:37:41.000000 pyNukiBT-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-03-30 19:37:46.105359 pyNukiBT-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-03-30 19:37:41.000000 pyNukiBT-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 19:37:46.105359 pyNukiBT-0.0.9/pyNukiBT/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-03-30 19:37:41.000000 pyNukiBT-0.0.9/pyNukiBT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39005 2024-03-30 19:37:41.000000 pyNukiBT-0.0.9/pyNukiBT/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25024 2024-03-30 19:37:41.000000 pyNukiBT-0.0.9/pyNukiBT/nuki.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 19:37:46.105359 pyNukiBT-0.0.9/pyNukiBT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-03-30 19:37:46.000000 pyNukiBT-0.0.9/pyNukiBT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-03-30 19:37:46.000000 pyNukiBT-0.0.9/pyNukiBT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 19:37:46.000000 pyNukiBT-0.0.9/pyNukiBT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-30 19:37:46.000000 pyNukiBT-0.0.9/pyNukiBT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-30 19:37:46.000000 pyNukiBT-0.0.9/pyNukiBT.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-03-30 19:37:41.000000 pyNukiBT-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-30 19:37:41.000000 pyNukiBT-0.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-30 19:37:46.105359 pyNukiBT-0.0.9/setup.cfg
```

### Comparing `pyNukiBT-0.0.8/.github/workflows/python-publish.yml` & `pyNukiBT-0.0.9/.github/workflows/python-publish.yml`

 * *Files 6% similar despite different names*

```diff
@@ -29,11 +29,11 @@
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install build
     - name: Build package
       run: python -m build
     - name: Publish package
-      uses: pypa/gh-action-pypi-publish@27b31702a0e7fc50959f5ad993c78deac1bdfc29
+      uses: pypa/gh-action-pypi-publish@81e9d935c883d0b210363ab89cf05f3894778450
       with:
         user: __token__
         password: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `pyNukiBT-0.0.8/.gitignore` & `pyNukiBT-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `pyNukiBT-0.0.8/LICENSE` & `pyNukiBT-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyNukiBT-0.0.8/PKG-INFO` & `pyNukiBT-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyNukiBT
-Version: 0.0.8
+Version: 0.0.9
 Summary: Nuki Bluetooth API
 Author-email: Ronen Gruengras <ronengr@gmail.com>
 Project-URL: Homepage, https://github.com/ronengr/pyNukiBT
 Project-URL: Bug Tracker, https://github.com/ronengr/pyNukiBT/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyNukiBT-0.0.8/README.md` & `pyNukiBT-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pyNukiBT-0.0.8/pyNukiBT/const.py` & `pyNukiBT-0.0.9/pyNukiBT/const.py`

 * *Files identical despite different names*

### Comparing `pyNukiBT-0.0.8/pyNukiBT/nuki.py` & `pyNukiBT-0.0.9/pyNukiBT/nuki.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,19 @@
                 # Ignore HomeKit advertisement
                 return
             logger.debug(f"Nuki: {device.address}, RSSI: {advertisement_data.rssi}")
             tx_p = manufacturer_data[-1]
             if self.just_got_beacon:
                 logger.info(f"Ignoring duplicate beacon from Nuki {device.address}")
                 return
-            self.set_ble_device(device)
+
+            # Don't change the device if we are in the middle of connect.
+            # using self._connect_lock.locked() is safe, as there is no real multithreading in python.
+            if not self._connect_lock.locked():
+                self.set_ble_device(device)
             self.rssi = advertisement_data.rssi
             if not self.last_state or tx_p & 0x1:
                 self._poll_needed = True
             return
         else:
             logger.error(f"called with invalid address {device.address}")
 
@@ -377,18 +381,19 @@
         async with self._connect_lock:
             if not self._client:
                 self.set_ble_device()
             if self._client.is_connected:
                 logger.info("Connected")
                 return
             await self._client.connect()
-            logger.debug(f"Services {[str(s) for s in self._client.services]}")
-            logger.debug(
-                f"Characteristics {[str(v) for v in self._client.services.characteristics.values()]}"
-            )
+            if logger.isEnabledFor(logging.DEBUG):
+                logger.debug(f"Services {[str(s) for s in self._client.services]}")
+                logger.debug(
+                    f"Characteristics {[str(v) for v in self._client.services.characteristics.values()]}"
+                )
             if (not self._device_type or not self._const):
                 services = self._client.services
                 if services.get_characteristic(NukiOpenerConst.BLE_PAIRING_CHAR):
                     self._device_type = NukiConst.NukiDeviceType.OPENER
                     self._const = NukiOpenerConst
                 else:
                     self._device_type = NukiConst.NukiDeviceType.SMARTLOCK_1_2
```

### Comparing `pyNukiBT-0.0.8/pyNukiBT.egg-info/PKG-INFO` & `pyNukiBT-0.0.9/pyNukiBT.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyNukiBT
-Version: 0.0.8
+Version: 0.0.9
 Summary: Nuki Bluetooth API
 Author-email: Ronen Gruengras <ronengr@gmail.com>
 Project-URL: Homepage, https://github.com/ronengr/pyNukiBT
 Project-URL: Bug Tracker, https://github.com/ronengr/pyNukiBT/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyNukiBT-0.0.8/pyproject.toml` & `pyNukiBT-0.0.9/pyproject.toml`

 * *Files identical despite different names*

