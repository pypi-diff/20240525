# Comparing `tmp/yoto_api-1.8.0.tar.gz` & `tmp/yoto_api-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yoto_api-1.8.0.tar", last modified: Wed May  8 01:58:49 2024, max compression
+gzip compressed data, was "yoto_api-1.9.0.tar", last modified: Wed May  8 03:49:38 2024, max compression
```

## Comparing `yoto_api-1.8.0.tar` & `yoto_api-1.9.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:58:49.033391 yoto_api-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-08 01:58:28.000000 yoto_api-1.8.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-05-08 01:58:28.000000 yoto_api-1.8.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-08 01:58:28.000000 yoto_api-1.8.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-08 01:58:28.000000 yoto_api-1.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-08 01:58:28.000000 yoto_api-1.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-05-08 01:58:49.033391 yoto_api-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-05-08 01:58:28.000000 yoto_api-1.8.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-08 01:58:28.000000 yoto_api-1.8.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 01:58:49.033391 yoto_api-1.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-08 01:58:43.000000 yoto_api-1.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:58:49.029391 yoto_api-1.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 01:58:28.000000 yoto_api-1.8.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-08 01:58:28.000000 yoto_api-1.8.0/tests/login_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:58:49.033391 yoto_api-1.8.0/yoto_api/
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-05-08 01:58:28.000000 yoto_api-1.8.0/yoto_api/Card.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-08 01:58:28.000000 yoto_api-1.8.0/yoto_api/Token.py
--rw-r--r--   0 runner    (1001) docker     (127)    23967 2024-05-08 01:58:28.000000 yoto_api-1.8.0/yoto_api/YotoAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)     3601 2024-05-08 01:58:28.000000 yoto_api-1.8.0/yoto_api/YotoMQTTClient.py
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-08 01:58:28.000000 yoto_api-1.8.0/yoto_api/YotoManager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-05-08 01:58:28.000000 yoto_api-1.8.0/yoto_api/YotoPlayer.py
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-08 01:58:28.000000 yoto_api-1.8.0/yoto_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-08 01:58:28.000000 yoto_api-1.8.0/yoto_api/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-08 01:58:28.000000 yoto_api-1.8.0/yoto_api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:58:49.033391 yoto_api-1.8.0/yoto_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-05-08 01:58:49.000000 yoto_api-1.8.0/yoto_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-08 01:58:49.000000 yoto_api-1.8.0/yoto_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 01:58:49.000000 yoto_api-1.8.0/yoto_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 01:58:48.000000 yoto_api-1.8.0/yoto_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-08 01:58:49.000000 yoto_api-1.8.0/yoto_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-08 01:58:49.000000 yoto_api-1.8.0/yoto_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:49:38.011398 yoto_api-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-08 03:49:17.000000 yoto_api-1.9.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-05-08 03:49:17.000000 yoto_api-1.9.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-08 03:49:17.000000 yoto_api-1.9.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-08 03:49:17.000000 yoto_api-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-08 03:49:17.000000 yoto_api-1.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-05-08 03:49:38.011398 yoto_api-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-05-08 03:49:17.000000 yoto_api-1.9.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-08 03:49:17.000000 yoto_api-1.9.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 03:49:38.011398 yoto_api-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-08 03:49:32.000000 yoto_api-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:49:38.007398 yoto_api-1.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 03:49:17.000000 yoto_api-1.9.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-08 03:49:17.000000 yoto_api-1.9.0/tests/login_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:49:38.007398 yoto_api-1.9.0/yoto_api/
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-05-08 03:49:17.000000 yoto_api-1.9.0/yoto_api/Card.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-08 03:49:17.000000 yoto_api-1.9.0/yoto_api/Token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23967 2024-05-08 03:49:17.000000 yoto_api-1.9.0/yoto_api/YotoAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-05-08 03:49:17.000000 yoto_api-1.9.0/yoto_api/YotoMQTTClient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-08 03:49:17.000000 yoto_api-1.9.0/yoto_api/YotoManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-05-08 03:49:17.000000 yoto_api-1.9.0/yoto_api/YotoPlayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-08 03:49:17.000000 yoto_api-1.9.0/yoto_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-08 03:49:17.000000 yoto_api-1.9.0/yoto_api/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-08 03:49:17.000000 yoto_api-1.9.0/yoto_api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:49:38.011398 yoto_api-1.9.0/yoto_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-05-08 03:49:37.000000 yoto_api-1.9.0/yoto_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-08 03:49:38.000000 yoto_api-1.9.0/yoto_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 03:49:37.000000 yoto_api-1.9.0/yoto_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 03:49:37.000000 yoto_api-1.9.0/yoto_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-08 03:49:37.000000 yoto_api-1.9.0/yoto_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-08 03:49:37.000000 yoto_api-1.9.0/yoto_api.egg-info/top_level.txt
```

### Comparing `yoto_api-1.8.0/CONTRIBUTING.rst` & `yoto_api-1.9.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `yoto_api-1.8.0/LICENSE` & `yoto_api-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yoto_api-1.8.0/PKG-INFO` & `yoto_api-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yoto_api
-Version: 1.8.0
+Version: 1.9.0
 Summary: A python package that makes it a bit easier to work with the yoto play API. Not associated with Yoto in any way.
 Home-page: https://github.com/cdnninja/yoto_api
 Author: cdnninja
 Author-email: 
 License: MIT license
 Keywords: yoto_api
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `yoto_api-1.8.0/README.rst` & `yoto_api-1.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `yoto_api-1.8.0/setup.py` & `yoto_api-1.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,10 +38,10 @@
     include_package_data=True,
     keywords="yoto_api",
     name="yoto_api",
     packages=find_packages(include=["yoto_api", "yoto_api.*"]),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/cdnninja/yoto_api",
-    version="1.8.0",
+    version="1.9.0",
     zip_safe=False,
 )
```

### Comparing `yoto_api-1.8.0/yoto_api/Card.py` & `yoto_api-1.9.0/yoto_api/Card.py`

 * *Files identical despite different names*

### Comparing `yoto_api-1.8.0/yoto_api/YotoAPI.py` & `yoto_api-1.9.0/yoto_api/YotoAPI.py`

 * *Files identical despite different names*

### Comparing `yoto_api-1.8.0/yoto_api/YotoMQTTClient.py` & `yoto_api-1.9.0/yoto_api/YotoMQTTClient.py`

 * *Files 11% similar despite different names*

```diff
@@ -52,19 +52,22 @@
         self._publish_command(self, self.client, topic, "card-play")
         # MQTT Message: {"status":{"card-play":"OK","req_body":"{\"uri\":\"https://yoto.io/7JtVV\",\"secondsIn\":0,\"cutOff\":0,\"chapterKey\":\"01\",\"trackKey\":\"01\",\"requestId\":\"5385910e-f853-4f34-99a4-d2ed94f02f6d\"}"}}
 
     def _publish_command(self, topic, payload):
         self.client.publish(topic, payload)
 
     def _parse_status_message(self, message, player):
-        _LOGGER.debug(f"{DOMAIN} - Parsing Status: {message}")
+        pass
 
     def _parse_events_message(self, message, player):
-        _LOGGER.debug(f"{DOMAIN} - Parsing Event: {message}")
         player.repeat_all = get_child_value(message, "repeatAll")
+        player.volume = get_child_value(message, "volume")
+        player.volume_max = get_child_value(message, "volumeMax")
+        player.online = get_child_value(message, "online")
+        player.chapter_title = get_child_value(message, "chapterTitle")
 
     # {"repeatAll":true,"volume":6,"volumeMax":6,"cardId":"none","playbackStatus":"stopped","streaming":false,"playbackWait":false,"sleepTimerActive":false,"eventUtc":1714960275}
 
     def _on_message(self, client, player, message):
         # Process MQTT Message
         _LOGGER.debug(
             f"{DOMAIN} - MQTT Message: {str(message.payload.decode('utf-8'))}"
```

### Comparing `yoto_api-1.8.0/yoto_api/YotoManager.py` & `yoto_api-1.9.0/yoto_api/YotoManager.py`

 * *Files identical despite different names*

### Comparing `yoto_api-1.8.0/yoto_api/YotoPlayer.py` & `yoto_api-1.9.0/yoto_api/YotoPlayer.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,14 +29,17 @@
     audio_device_connected: bool = None
     firmware_version: str = None
     wifi_strength: int = None
     power_source: str = None
 
     # MQTT
     repeat_all: bool = None
+    volume_max: int = None
+    volume: int = None
+    chapter_title: str = None
 
 
 # {'devices': [{'deviceId': 'XXXX', 'name': 'Yoto Player', 'description': 'nameless.limit', 'online': False, 'releaseChannel': 'general', 'deviceType': 'v3', 'deviceFamily': 'v3', 'deviceGroup': '', 'hasUserGivenName': False}]}
 # Device Status API: {'activeCard': 'none', 'ambientLightSensorReading': 0, 'averageDownloadSpeedBytesSecond': 0, 'batteryLevelPercentage': 100, 'buzzErrors': 0, 'cardInsertionState': 2, 'dayMode': 0, 'deviceId': 'XXXX', 'errorsLogged': 210, 'firmwareVersion': 'v2.17.5', 'freeDiskSpaceBytes': 30250544, 'isAudioDeviceConnected': False, 'isBackgroundDownloadActive': False, 'isBluetoothAudioConnected': False, 'isCharging': False, 'isOnline': True, 'networkSsid': 'XXXX', 'nightlightMode': '0x000000', 'playingSource': 0, 'powerCapabilities': '0x02', 'powerSource': 2, 'systemVolumePercentage': 47, 'taskWatchdogTimeoutCount': 0, 'temperatureCelcius': '20', 'totalDiskSpaceBytes': 31385600, 'updatedAt': '2024-04-23T01:26:19.927Z', 'uptime': 252342, 'userVolumePercentage': 50, 'utcOffsetSeconds': -21600, 'utcTime': 1713835609, 'wifiStrength': -61}
 # Mqtt response:
 
 {
```

### Comparing `yoto_api-1.8.0/yoto_api/utils.py` & `yoto_api-1.9.0/yoto_api/utils.py`

 * *Files identical despite different names*

### Comparing `yoto_api-1.8.0/yoto_api.egg-info/PKG-INFO` & `yoto_api-1.9.0/yoto_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yoto_api
-Version: 1.8.0
+Version: 1.9.0
 Summary: A python package that makes it a bit easier to work with the yoto play API. Not associated with Yoto in any way.
 Home-page: https://github.com/cdnninja/yoto_api
 Author: cdnninja
 Author-email: 
 License: MIT license
 Keywords: yoto_api
 Classifier: Development Status :: 2 - Pre-Alpha
```

