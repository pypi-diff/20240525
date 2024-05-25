# Comparing `tmp/botocore-a-la-carte-medialive-1.34.98.tar.gz` & `tmp/botocore-a-la-carte-medialive-1.34.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-medialive-1.34.98.tar", last modified: Sat May  4 01:01:35 2024, max compression
+gzip compressed data, was "botocore-a-la-carte-medialive-1.34.99.tar", last modified: Tue May  7 01:02:37 2024, max compression
```

## Comparing `botocore-a-la-carte-medialive-1.34.98.tar` & `botocore-a-la-carte-medialive-1.34.99.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:35.630218 botocore-a-la-carte-medialive-1.34.98/
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-05-04 01:01:35.000000 botocore-a-la-carte-medialive-1.34.98/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-04 01:01:35.630218 botocore-a-la-carte-medialive-1.34.98/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:35.626217 botocore-a-la-carte-medialive-1.34.98/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:35.626217 botocore-a-la-carte-medialive-1.34.98/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:35.626217 botocore-a-la-carte-medialive-1.34.98/botocore/data/medialive/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:35.630218 botocore-a-la-carte-medialive-1.34.98/botocore/data/medialive/2017-10-14/
--rw-r--r--   0 runner    (1001) docker     (127)    13738 2024-05-04 01:01:11.000000 botocore-a-la-carte-medialive-1.34.98/botocore/data/medialive/2017-10-14/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-05-04 01:01:11.000000 botocore-a-la-carte-medialive-1.34.98/botocore/data/medialive/2017-10-14/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (127)   877528 2024-05-04 01:01:11.000000 botocore-a-la-carte-medialive-1.34.98/botocore/data/medialive/2017-10-14/service-2.json
--rw-r--r--   0 runner    (1001) docker     (127)    10479 2024-05-04 01:01:11.000000 botocore-a-la-carte-medialive-1.34.98/botocore/data/medialive/2017-10-14/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:01:35.630218 botocore-a-la-carte-medialive-1.34.98/botocore_a_la_carte_medialive.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-04 01:01:35.000000 botocore-a-la-carte-medialive-1.34.98/botocore_a_la_carte_medialive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-04 01:01:35.000000 botocore-a-la-carte-medialive-1.34.98/botocore_a_la_carte_medialive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 01:01:35.000000 botocore-a-la-carte-medialive-1.34.98/botocore_a_la_carte_medialive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-04 01:01:35.000000 botocore-a-la-carte-medialive-1.34.98/botocore_a_la_carte_medialive.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 01:01:35.630218 botocore-a-la-carte-medialive-1.34.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-04 01:01:35.000000 botocore-a-la-carte-medialive-1.34.98/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:37.740095 botocore-a-la-carte-medialive-1.34.99/
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-05-07 01:02:37.000000 botocore-a-la-carte-medialive-1.34.99/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-07 01:02:37.740095 botocore-a-la-carte-medialive-1.34.99/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:37.736095 botocore-a-la-carte-medialive-1.34.99/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:37.736095 botocore-a-la-carte-medialive-1.34.99/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:37.736095 botocore-a-la-carte-medialive-1.34.99/botocore/data/medialive/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:37.740095 botocore-a-la-carte-medialive-1.34.99/botocore/data/medialive/2017-10-14/
+-rw-r--r--   0 runner    (1001) docker     (127)    13738 2024-05-07 01:02:11.000000 botocore-a-la-carte-medialive-1.34.99/botocore/data/medialive/2017-10-14/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-05-07 01:02:11.000000 botocore-a-la-carte-medialive-1.34.99/botocore/data/medialive/2017-10-14/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)   878562 2024-05-07 01:02:11.000000 botocore-a-la-carte-medialive-1.34.99/botocore/data/medialive/2017-10-14/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10479 2024-05-07 01:02:11.000000 botocore-a-la-carte-medialive-1.34.99/botocore/data/medialive/2017-10-14/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:02:37.740095 botocore-a-la-carte-medialive-1.34.99/botocore_a_la_carte_medialive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-07 01:02:37.000000 botocore-a-la-carte-medialive-1.34.99/botocore_a_la_carte_medialive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-07 01:02:37.000000 botocore-a-la-carte-medialive-1.34.99/botocore_a_la_carte_medialive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 01:02:37.000000 botocore-a-la-carte-medialive-1.34.99/botocore_a_la_carte_medialive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-07 01:02:37.000000 botocore-a-la-carte-medialive-1.34.99/botocore_a_la_carte_medialive.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 01:02:37.740095 botocore-a-la-carte-medialive-1.34.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-07 01:02:37.000000 botocore-a-la-carte-medialive-1.34.99/setup.py
```

### Comparing `botocore-a-la-carte-medialive-1.34.98/LICENSE.txt` & `botocore-a-la-carte-medialive-1.34.99/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-medialive-1.34.98/PKG-INFO` & `botocore-a-la-carte-medialive-1.34.99/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-medialive
-Version: 1.34.98
+Version: 1.34.99
 Summary: medialive data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-medialive-1.34.98/botocore/data/medialive/2017-10-14/endpoint-rule-set-1.json` & `botocore-a-la-carte-medialive-1.34.99/botocore/data/medialive/2017-10-14/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-medialive-1.34.98/botocore/data/medialive/2017-10-14/paginators-1.json` & `botocore-a-la-carte-medialive-1.34.99/botocore/data/medialive/2017-10-14/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-medialive-1.34.98/botocore/data/medialive/2017-10-14/service-2.json` & `botocore-a-la-carte-medialive-1.34.99/botocore/data/medialive/2017-10-14/service-2.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998733381971465%*

 * *Differences: {"'shapes'": "{'AvailConfiguration': {'members': {'Scte35SegmentationScope': "*

 * *             "OrderedDict([('shape', 'Scte35SegmentationScope'), ('locationName', "*

 * *             "'scte35SegmentationScope'), ('documentation', 'Configures whether SCTE 35 "*

 * *             'passthrough triggers segment breaks in all output groups that use segmented outputs. '*

 * *             'Insertion of a SCTE 35 message typically results in a segment break, in addition to '*

 * *             'the regular cadence of breaks. The segment b […]*

```diff
@@ -5013,14 +5013,19 @@
         "AvailConfiguration": {
             "documentation": "Avail Configuration",
             "members": {
                 "AvailSettings": {
                     "documentation": "Controls how SCTE-35 messages create cues. Splice Insert mode treats all segmentation signals traditionally. With Time Signal APOS mode only Time Signal Placement Opportunity and Break messages create segment breaks. With ESAM mode, signals are forwarded to an ESAM server for possible update.",
                     "locationName": "availSettings",
                     "shape": "AvailSettings"
+                },
+                "Scte35SegmentationScope": {
+                    "documentation": "Configures whether SCTE 35 passthrough triggers segment breaks in all output groups that use segmented outputs. Insertion of a SCTE 35 message typically results in a segment break, in addition to the regular cadence of breaks. The segment breaks appear in video outputs, audio outputs, and captions outputs (if any).\n\nALL_OUTPUT_GROUPS: Default. Insert the segment break in in all output groups that have segmented outputs. This is the legacy behavior.\nSCTE35_ENABLED_OUTPUT_GROUPS: Insert the segment break only in output groups that have SCTE 35 passthrough enabled. This is the recommended value, because it reduces unnecessary segment breaks.",
+                    "locationName": "scte35SegmentationScope",
+                    "shape": "Scte35SegmentationScope"
                 }
             },
             "type": "structure"
         },
         "AvailSettings": {
             "documentation": "Avail Settings",
             "members": {
@@ -18789,14 +18794,22 @@
             },
             "required": [
                 "SegmentationEventId",
                 "SegmentationCancelIndicator"
             ],
             "type": "structure"
         },
+        "Scte35SegmentationScope": {
+            "documentation": "Scte35 Segmentation Scope",
+            "enum": [
+                "ALL_OUTPUT_GROUPS",
+                "SCTE35_ENABLED_OUTPUT_GROUPS"
+            ],
+            "type": "string"
+        },
         "Scte35SpliceInsert": {
             "documentation": "Typical configuration that applies breaks on splice inserts in addition to time signal placement opportunities, breaks, and advertisements.",
             "members": {
                 "AdAvailOffset": {
                     "documentation": "When specified, this offset (in milliseconds) is added to the input Ad Avail PTS time. This only applies to embedded SCTE 104/35 messages and does not apply to OOB messages.",
                     "locationName": "adAvailOffset",
                     "shape": "__integerMinNegative1000Max1000"
```

### Comparing `botocore-a-la-carte-medialive-1.34.98/botocore/data/medialive/2017-10-14/waiters-2.json` & `botocore-a-la-carte-medialive-1.34.99/botocore/data/medialive/2017-10-14/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-medialive-1.34.98/botocore_a_la_carte_medialive.egg-info/PKG-INFO` & `botocore-a-la-carte-medialive-1.34.99/botocore_a_la_carte_medialive.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-medialive
-Version: 1.34.98
+Version: 1.34.99
 Summary: medialive data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-medialive-1.34.98/setup.py` & `botocore-a-la-carte-medialive-1.34.99/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-medialive',
-    version="1.34.98",
+    version="1.34.99",
     description='medialive data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/medialive/*/*.json'],
```

