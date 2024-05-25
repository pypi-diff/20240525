# Comparing `tmp/fiftyone_devicedetection_onpremise-4.4.8.tar.gz` & `tmp/fiftyone_devicedetection_onpremise-4.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fiftyone_devicedetection_onpremise-4.4.8.tar", last modified: Tue Jul 26 08:21:14 2022, max compression
+gzip compressed data, was "dist/fiftyone_devicedetection_onpremise-4.4.9.tar", last modified: Wed Aug 10 09:13:05 2022, max compression
```

## Comparing `fiftyone_devicedetection_onpremise-4.4.8.tar` & `fiftyone_devicedetection_onpremise-4.4.9.tar`

### file list

```diff
@@ -1,214 +1,214 @@
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2022-07-26 08:21:14.000000 fiftyone_devicedetection_onpremise-4.4.8/
--rw-r--r--   0 vsts      (1001) docker     (116)      267 2022-07-26 08:20:46.000000 fiftyone_devicedetection_onpremise-4.4.8/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (116)     4271 2022-07-26 08:21:14.000000 fiftyone_devicedetection_onpremise-4.4.8/PKG-INFO
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2022-07-26 08:21:13.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/
--rw-r--r--   0 vsts      (1001) docker     (116)    47677 2022-07-26 08:20:46.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/DeviceDetectionHashEngineModule.py
--rw-r--r--   0 vsts      (1001) docker     (116)        0 2022-07-26 08:20:46.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (116)     2369 2022-07-26 08:20:46.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/constants.py
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2022-07-26 08:21:13.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2022-07-26 08:21:13.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/
--rw-r--r--   0 vsts      (1001) docker     (116)     2062 2022-07-26 08:20:49.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/ConfigDeviceDetection.cpp
--rw-r--r--   0 vsts      (1001) docker     (116)     4741 2022-07-26 08:20:49.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/ConfigDeviceDetection.hpp
--rw-r--r--   0 vsts      (1001) docker     (116)     1610 2022-07-26 08:20:49.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/ConfigDeviceDetection.i
--rw-r--r--   0 vsts      (1001) docker     (116)     1840 2022-07-26 08:20:49.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/EngineDeviceDetection.cpp
--rw-r--r--   0 vsts      (1001) docker     (116)     4901 2022-07-26 08:20:49.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/EngineDeviceDetection.hpp
--rw-r--r--   0 vsts      (1001) docker     (116)     1702 2022-07-26 08:20:49.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/EngineDeviceDetection.i
--rw-r--r--   0 vsts      (1001) docker     (116)     1654 2022-07-26 08:20:49.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/EvidenceDeviceDetection.cpp
--rw-r--r--   0 vsts      (1001) docker     (116)     2781 2022-07-26 08:20:49.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/EvidenceDeviceDetection.hpp
--rw-r--r--   0 vsts      (1001) docker     (116)     1420 2022-07-26 08:20:49.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/EvidenceDeviceDetection.i
--rw-r--r--   0 vsts      (1001) docker     (116)     1603 2022-07-26 08:20:49.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/FiftyoneDegrees.hpp
--rw-r--r--   0 vsts      (1001) docker     (116)     1565 2022-07-26 08:20:49.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/ResultsDeviceDetection.cpp
--rw-r--r--   0 vsts      (1001) docker     (116)     4236 2022-07-26 08:20:49.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/ResultsDeviceDetection.hpp
--rw-r--r--   0 vsts      (1001) docker     (116)     1527 2022-07-26 08:20:49.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/ResultsDeviceDetection.i
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2022-07-26 08:21:14.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/
--rw-r--r--   0 vsts      (1001) docker     (116)     3998 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/Collection.hpp
--rw-r--r--   0 vsts      (1001) docker     (116)     1409 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/Collection.i
--rw-r--r--   0 vsts      (1001) docker     (116)     2344 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/CollectionConfig.cpp
--rw-r--r--   0 vsts      (1001) docker     (116)     3937 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/CollectionConfig.hpp
--rw-r--r--   0 vsts      (1001) docker     (116)     1504 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/CollectionConfig.i
--rw-r--r--   0 vsts      (1001) docker     (116)     2135 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/ComponentMetaData.cpp
--rw-r--r--   0 vsts      (1001) docker     (116)     3203 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/ComponentMetaData.hpp
--rw-r--r--   0 vsts      (1001) docker     (116)     1406 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/ComponentMetaData.i
--rw-r--r--   0 vsts      (1001) docker     (116)     2640 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/ConfigBase.cpp
--rw-r--r--   0 vsts      (1001) docker     (116)     5582 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/ConfigBase.hpp
--rw-r--r--   0 vsts      (1001) docker     (116)     1706 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/ConfigBase.i
--rw-r--r--   0 vsts      (1001) docker     (116)     1349 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/Coordinate.i
--rw-r--r--   0 vsts      (1001) docker     (116)     1651 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/CsTypes.i
--rw-r--r--   0 vsts      (1001) docker     (116)     1552 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/Date.cpp
--rw-r--r--   0 vsts      (1001) docker     (116)     2704 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/Date.hpp
--rw-r--r--   0 vsts      (1001) docker     (116)     1278 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/Date.i
--rw-r--r--   0 vsts      (1001) docker     (116)     4758 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/EngineBase.cpp
--rw-r--r--   0 vsts      (1001) docker     (116)     9509 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/EngineBase.hpp
--rw-r--r--   0 vsts      (1001) docker     (116)     2238 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/EngineBase.i
--rw-r--r--   0 vsts      (1001) docker     (116)     3071 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/EntityMetaData.hpp
--rw-r--r--   0 vsts      (1001) docker     (116)     2659 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/EntityMetaDataBuilder.hpp
--rw-r--r--   0 vsts      (1001) docker     (116)     2635 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/EvidenceBase.cpp
--rw-r--r--   0 vsts      (1001) docker     (116)     4021 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/EvidenceBase.hpp
--rw-r--r--   0 vsts      (1001) docker     (116)     1378 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/EvidenceBase.i
--rw-r--r--   0 vsts      (1001) docker     (116)     3299 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/Exceptions.cpp
--rw-r--r--   0 vsts      (1001) docker     (116)     4768 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/Exceptions.hpp
--rw-r--r--   0 vsts      (1001) docker     (116)     2054 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/Exceptions.i
--rw-r--r--   0 vsts      (1001) docker     (116)     1448 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/FiftyoneDegrees.hpp
--rw-r--r--   0 vsts      (1001) docker     (116)     4116 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/JavaTypes.i
--rw-r--r--   0 vsts      (1001) docker     (116)     1969 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/MapStringStringIterator.i
--rw-r--r--   0 vsts      (1001) docker     (116)     1788 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/MetaData.cpp
--rw-r--r--   0 vsts      (1001) docker     (116)     8088 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/MetaData.hpp
--rw-r--r--   0 vsts      (1001) docker     (116)     3087 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/MetaData.i
--rw-r--r--   0 vsts      (1001) docker     (116)     1840 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/ProfileMetaData.cpp
--rw-r--r--   0 vsts      (1001) docker     (116)     2778 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/ProfileMetaData.hpp
--rw-r--r--   0 vsts      (1001) docker     (116)     1348 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/ProfileMetaData.i
--rw-r--r--   0 vsts      (1001) docker     (116)     4253 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/PropertyMetaData.cpp
--rw-r--r--   0 vsts      (1001) docker     (116)     7978 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/PropertyMetaData.hpp
--rw-r--r--   0 vsts      (1001) docker     (116)     1684 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/PropertyMetaData.i
--rw-r--r--   0 vsts      (1001) docker     (116)     4414 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/RequiredPropertiesConfig.cpp
--rw-r--r--   0 vsts      (1001) docker     (116)     5326 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/RequiredPropertiesConfig.hpp
--rw-r--r--   0 vsts      (1001) docker     (116)     1571 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/RequiredPropertiesConfig.i
--rw-r--r--   0 vsts      (1001) docker     (116)     8176 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/ResultsBase.cpp
--rw-r--r--   0 vsts      (1001) docker     (116)    16639 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/ResultsBase.hpp
--rw-r--r--   0 vsts      (1001) docker     (116)     2209 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/ResultsBase.i
--rw-r--r--   0 vsts      (1001) docker     (116)     1392 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/Types.i
--rw-r--r--   0 vsts      (1001) docker     (116)     6224 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/Value.hpp
--rw-r--r--   0 vsts      (1001) docker     (116)     1563 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/Value.i
--rw-r--r--   0 vsts      (1001) docker     (116)     3464 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/ValueMetaData.cpp
--rw-r--r--   0 vsts      (1001) docker     (116)     4936 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/ValueMetaData.hpp
--rw-r--r--   0 vsts      (1001) docker     (116)     1641 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/ValueMetaData.i
--rw-r--r--   0 vsts      (1001) docker     (116)     2676 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/array.h
--rw-r--r--   0 vsts      (1001) docker     (116)     1751 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/bool.h
--rw-r--r--   0 vsts      (1001) docker     (116)    12861 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/cache.c
--rw-r--r--   0 vsts      (1001) docker     (116)    10543 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/cache.h
--rw-r--r--   0 vsts      (1001) docker     (116)    33990 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/collection.c
--rw-r--r--   0 vsts      (1001) docker     (116)    29281 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/collection.h
--rw-r--r--   0 vsts      (1001) docker     (116)     1568 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/common.h
--rw-r--r--   0 vsts      (1001) docker     (116)     3826 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/component.c
--rw-r--r--   0 vsts      (1001) docker     (116)     6697 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/component.h
--rw-r--r--   0 vsts      (1001) docker     (116)     4344 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/config.h
--rw-r--r--   0 vsts      (1001) docker     (116)     2566 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/coordinate.h
--rw-r--r--   0 vsts      (1001) docker     (116)     1727 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/data.c
--rw-r--r--   0 vsts      (1001) docker     (116)     4547 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/data.h
--rw-r--r--   0 vsts      (1001) docker     (116)    10232 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/dataset.c
--rw-r--r--   0 vsts      (1001) docker     (116)    18728 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/dataset.h
--rw-r--r--   0 vsts      (1001) docker     (116)     2247 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/date.h
--rw-r--r--   0 vsts      (1001) docker     (116)     5656 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/evidence.c
--rw-r--r--   0 vsts      (1001) docker     (116)     9692 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/evidence.h
--rw-r--r--   0 vsts      (1001) docker     (116)     6994 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/exceptions.h
--rw-r--r--   0 vsts      (1001) docker     (116)     2776 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/exceptionsc.c
--rw-r--r--   0 vsts      (1001) docker     (116)    32828 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/fiftyone.h
--rw-r--r--   0 vsts      (1001) docker     (116)    29063 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/file.c
--rw-r--r--   0 vsts      (1001) docker     (116)    18100 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/file.h
--rw-r--r--   0 vsts      (1001) docker     (116)     5139 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/float.c
--rw-r--r--   0 vsts      (1001) docker     (116)     7348 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/float.h
--rw-r--r--   0 vsts      (1001) docker     (116)    11885 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/headers.c
--rw-r--r--   0 vsts      (1001) docker     (116)     8284 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/headers.h
--rw-r--r--   0 vsts      (1001) docker     (116)     7452 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/ip.c
--rw-r--r--   0 vsts      (1001) docker     (116)     4847 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/ip.h
--rw-r--r--   0 vsts      (1001) docker     (116)     2357 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/list.c
--rw-r--r--   0 vsts      (1001) docker     (116)     5593 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/list.h
--rw-r--r--   0 vsts      (1001) docker     (116)     8984 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/memory.c
--rw-r--r--   0 vsts      (1001) docker     (116)     7639 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/memory.h
--rw-r--r--   0 vsts      (1001) docker     (116)    12916 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/overrides.c
--rw-r--r--   0 vsts      (1001) docker     (116)    10180 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/overrides.h
--rw-r--r--   0 vsts      (1001) docker     (116)     1418 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/pair.h
--rw-r--r--   0 vsts      (1001) docker     (116)     4611 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/pool.c
--rw-r--r--   0 vsts      (1001) docker     (116)     9648 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/pool.h
--rw-r--r--   0 vsts      (1001) docker     (116)     1544 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/process.c
--rw-r--r--   0 vsts      (1001) docker     (116)     1429 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/process.h
--rw-r--r--   0 vsts      (1001) docker     (116)     9403 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/profile.c
--rw-r--r--   0 vsts      (1001) docker     (116)     9813 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/profile.h
--rw-r--r--   0 vsts      (1001) docker     (116)    14964 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/properties.c
--rw-r--r--   0 vsts      (1001) docker     (116)    13395 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/properties.h
--rw-r--r--   0 vsts      (1001) docker     (116)     4708 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/property.c
--rw-r--r--   0 vsts      (1001) docker     (116)    10041 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/property.h
--rw-r--r--   0 vsts      (1001) docker     (116)     9458 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/pseudoheader.c
--rw-r--r--   0 vsts      (1001) docker     (116)     3606 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/pseudoheader.h
--rw-r--r--   0 vsts      (1001) docker     (116)    12300 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/resource.c
--rw-r--r--   0 vsts      (1001) docker     (116)     9878 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/resource.h
--rw-r--r--   0 vsts      (1001) docker     (116)     1388 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/results.c
--rw-r--r--   0 vsts      (1001) docker     (116)     4351 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/results.h
--rw-r--r--   0 vsts      (1001) docker     (116)     1571 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/snprintf.h
--rw-r--r--   0 vsts      (1001) docker     (116)     6158 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/status.c
--rw-r--r--   0 vsts      (1001) docker     (116)     7434 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/status.h
--rw-r--r--   0 vsts      (1001) docker     (116)     2915 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/string.c
--rw-r--r--   0 vsts      (1001) docker     (116)     6596 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/string.h
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2022-07-26 08:21:14.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/tests/
--rw-r--r--   0 vsts      (1001) docker     (116)     3900 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/tests/Base.hpp
--rw-r--r--   0 vsts      (1001) docker     (116)     3698 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/tests/EngineTests.hpp
--rw-r--r--   0 vsts      (1001) docker     (116)     2482 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/tests/EvidenceTests.hpp
--rw-r--r--   0 vsts      (1001) docker     (116)     1398 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/tests/ExampleTests.hpp
--rw-r--r--   0 vsts      (1001) docker     (116)     1747 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/tests/FileHandle.hpp
--rw-r--r--   0 vsts      (1001) docker     (116)     2137 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/tests/PseudoHeaderTests.hpp
--rw-r--r--   0 vsts      (1001) docker     (116)     2046 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/tests/StringCollection.hpp
--rw-r--r--   0 vsts      (1001) docker     (116)     1355 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/tests/TestStrings.hpp
--rw-r--r--   0 vsts      (1001) docker     (116)     1541 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/tests/pch.h
--rw-r--r--   0 vsts      (1001) docker     (116)     3499 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/textfile.c
--rw-r--r--   0 vsts      (1001) docker     (116)     2932 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/textfile.h
--rw-r--r--   0 vsts      (1001) docker     (116)     3734 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/threading.c
--rw-r--r--   0 vsts      (1001) docker     (116)    14531 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/threading.h
--rw-r--r--   0 vsts      (1001) docker     (116)    10109 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/tree.c
--rw-r--r--   0 vsts      (1001) docker     (116)     6469 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/tree.h
--rw-r--r--   0 vsts      (1001) docker     (116)     7116 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/value.c
--rw-r--r--   0 vsts      (1001) docker     (116)     7404 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/value.h
--rw-r--r--   0 vsts      (1001) docker     (116)     4063 2022-07-26 08:20:58.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/yamlfile.h
--rw-r--r--   0 vsts      (1001) docker     (116)     3660 2022-07-26 08:20:49.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/config-dd.h
--rw-r--r--   0 vsts      (1001) docker     (116)     3122 2022-07-26 08:20:49.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/dataset-dd.c
--rw-r--r--   0 vsts      (1001) docker     (116)     4480 2022-07-26 08:20:49.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/dataset-dd.h
--rw-r--r--   0 vsts      (1001) docker     (116)     3440 2022-07-26 08:20:49.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/fiftyone.h
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2022-07-26 08:21:14.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/
--rw-r--r--   0 vsts      (1001) docker     (116)     1974 2022-07-26 08:20:49.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ComponentMetaDataBuilderHash.cpp
--rw-r--r--   0 vsts      (1001) docker     (116)     2374 2022-07-26 08:20:49.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ComponentMetaDataBuilderHash.hpp
--rw-r--r--   0 vsts      (1001) docker     (116)     2554 2022-07-26 08:20:49.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ComponentMetaDataCollectionHash.cpp
--rw-r--r--   0 vsts      (1001) docker     (116)     2724 2022-07-26 08:20:49.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ComponentMetaDataCollectionHash.hpp
--rw-r--r--   0 vsts      (1001) docker     (116)     5422 2022-07-26 08:20:49.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ConfigHash.cpp
--rw-r--r--   0 vsts      (1001) docker     (116)    10458 2022-07-26 08:20:49.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ConfigHash.hpp
--rw-r--r--   0 vsts      (1001) docker     (116)     2103 2022-07-26 08:20:49.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ConfigHash.i
--rw-r--r--   0 vsts      (1001) docker     (116)     7613 2022-07-26 08:20:49.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/EngineHash.cpp
--rw-r--r--   0 vsts      (1001) docker     (116)     6743 2022-07-26 08:20:49.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/EngineHash.hpp
--rw-r--r--   0 vsts      (1001) docker     (116)     2172 2022-07-26 08:20:49.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/EngineHash.i
--rw-r--r--   0 vsts      (1001) docker     (116)     4522 2022-07-26 08:20:49.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/MetaDataHash.cpp
--rw-r--r--   0 vsts      (1001) docker     (116)     3586 2022-07-26 08:20:49.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/MetaDataHash.hpp
--rw-r--r--   0 vsts      (1001) docker     (116)     1617 2022-07-26 08:20:49.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ProfileMetaDataBuilderHash.cpp
--rw-r--r--   0 vsts      (1001) docker     (116)     2348 2022-07-26 08:20:49.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ProfileMetaDataBuilderHash.hpp
--rw-r--r--   0 vsts      (1001) docker     (116)     2823 2022-07-26 08:20:49.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ProfileMetaDataCollectionHash.cpp
--rw-r--r--   0 vsts      (1001) docker     (116)     2829 2022-07-26 08:20:49.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ProfileMetaDataCollectionHash.hpp
--rw-r--r--   0 vsts      (1001) docker     (116)     5489 2022-07-26 08:20:49.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/PropertyMetaDataBuilderHash.cpp
--rw-r--r--   0 vsts      (1001) docker     (116)     4476 2022-07-26 08:20:49.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/PropertyMetaDataBuilderHash.hpp
--rw-r--r--   0 vsts      (1001) docker     (116)     3179 2022-07-26 08:20:49.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/PropertyMetaDataCollectionForComponentHash.cpp
--rw-r--r--   0 vsts      (1001) docker     (116)     3033 2022-07-26 08:20:49.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/PropertyMetaDataCollectionForComponentHash.hpp
--rw-r--r--   0 vsts      (1001) docker     (116)     2957 2022-07-26 08:20:49.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/PropertyMetaDataCollectionForPropertyHash.cpp
--rw-r--r--   0 vsts      (1001) docker     (116)     2525 2022-07-26 08:20:49.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/PropertyMetaDataCollectionForPropertyHash.hpp
--rw-r--r--   0 vsts      (1001) docker     (116)     2810 2022-07-26 08:20:49.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/PropertyMetaDataCollectionHash.cpp
--rw-r--r--   0 vsts      (1001) docker     (116)     2714 2022-07-26 08:20:49.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/PropertyMetaDataCollectionHash.hpp
--rw-r--r--   0 vsts      (1001) docker     (116)     7319 2022-07-26 08:20:49.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ResultsHash.cpp
--rw-r--r--   0 vsts      (1001) docker     (116)     6726 2022-07-26 08:20:49.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ResultsHash.hpp
--rw-r--r--   0 vsts      (1001) docker     (116)     1790 2022-07-26 08:20:49.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ResultsHash.i
--rw-r--r--   0 vsts      (1001) docker     (116)     2133 2022-07-26 08:20:49.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ValueMetaDataBuilderHash.cpp
--rw-r--r--   0 vsts      (1001) docker     (116)     2318 2022-07-26 08:20:49.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ValueMetaDataBuilderHash.hpp
--rw-r--r--   0 vsts      (1001) docker     (116)     2577 2022-07-26 08:20:49.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ValueMetaDataCollectionBaseHash.cpp
--rw-r--r--   0 vsts      (1001) docker     (116)     2564 2022-07-26 08:20:49.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ValueMetaDataCollectionBaseHash.hpp
--rw-r--r--   0 vsts      (1001) docker     (116)     4508 2022-07-26 08:20:49.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ValueMetaDataCollectionForProfileHash.cpp
--rw-r--r--   0 vsts      (1001) docker     (116)     3404 2022-07-26 08:20:49.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ValueMetaDataCollectionForProfileHash.hpp
--rw-r--r--   0 vsts      (1001) docker     (116)     3265 2022-07-26 08:20:49.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ValueMetaDataCollectionForPropertyHash.cpp
--rw-r--r--   0 vsts      (1001) docker     (116)     3057 2022-07-26 08:20:49.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ValueMetaDataCollectionForPropertyHash.hpp
--rw-r--r--   0 vsts      (1001) docker     (116)     2219 2022-07-26 08:20:49.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ValueMetaDataCollectionHash.cpp
--rw-r--r--   0 vsts      (1001) docker     (116)     2482 2022-07-26 08:20:49.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ValueMetaDataCollectionHash.hpp
--rw-r--r--   0 vsts      (1001) docker     (116)     7710 2022-07-26 08:20:49.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/fiftyone.h
--rw-r--r--   0 vsts      (1001) docker     (116)    10280 2022-07-26 08:20:49.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/graph.c
--rw-r--r--   0 vsts      (1001) docker     (116)    13280 2022-07-26 08:20:49.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/graph.h
--rw-r--r--   0 vsts      (1001) docker     (116)   101660 2022-07-26 08:20:49.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/hash.c
--rw-r--r--   0 vsts      (1001) docker     (116)    38142 2022-07-26 08:20:49.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/hash.h
--rw-r--r--   0 vsts      (1001) docker     (116)     1826 2022-07-26 08:20:49.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/hash.i
--rw-r--r--   0 vsts      (1001) docker     (116)     2846 2022-07-26 08:20:49.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/results-dd.c
--rw-r--r--   0 vsts      (1001) docker     (116)     5261 2022-07-26 08:20:49.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/results-dd.h
--rw-r--r--   0 vsts      (1001) docker     (116)     3677 2022-07-26 08:20:46.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/devicedetection_datafile.py
--rw-r--r--   0 vsts      (1001) docker     (116)    15789 2022-07-26 08:20:46.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/devicedetection_onpremise.py
--rw-r--r--   0 vsts      (1001) docker     (116)     6975 2022-07-26 08:20:46.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/devicedetection_onpremise_pipelinebuilder.py
--rw-r--r--   0 vsts      (1001) docker     (116)   818429 2022-07-26 08:20:46.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/hash_python_wrap.cxx
--rw-r--r--   0 vsts      (1001) docker     (116)     5451 2022-07-26 08:20:46.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/swig_data.py
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2022-07-26 08:21:13.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (116)     4271 2022-07-26 08:21:13.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (116)    16937 2022-07-26 08:21:13.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (116)        1 2022-07-26 08:21:13.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (116)       67 2022-07-26 08:21:13.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (116)       68 2022-07-26 08:21:13.000000 fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (116)       38 2022-07-26 08:21:14.000000 fiftyone_devicedetection_onpremise-4.4.8/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (116)    13632 2022-07-26 08:20:46.000000 fiftyone_devicedetection_onpremise-4.4.8/setup.py
--rw-r--r--   0 vsts      (1001) docker     (116)        6 2022-07-26 08:21:13.000000 fiftyone_devicedetection_onpremise-4.4.8/version.txt
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2022-08-10 09:13:05.000000 fiftyone_devicedetection_onpremise-4.4.9/
+-rw-r--r--   0 vsts      (1001) docker     (116)      267 2022-08-10 09:12:36.000000 fiftyone_devicedetection_onpremise-4.4.9/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (116)     4271 2022-08-10 09:13:05.000000 fiftyone_devicedetection_onpremise-4.4.9/PKG-INFO
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2022-08-10 09:13:05.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/
+-rw-r--r--   0 vsts      (1001) docker     (116)    47677 2022-08-10 09:12:36.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/DeviceDetectionHashEngineModule.py
+-rw-r--r--   0 vsts      (1001) docker     (116)        0 2022-08-10 09:12:36.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     2369 2022-08-10 09:12:36.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/constants.py
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2022-08-10 09:13:05.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2022-08-10 09:13:05.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/
+-rw-r--r--   0 vsts      (1001) docker     (116)     2062 2022-08-10 09:12:39.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/ConfigDeviceDetection.cpp
+-rw-r--r--   0 vsts      (1001) docker     (116)     4741 2022-08-10 09:12:39.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/ConfigDeviceDetection.hpp
+-rw-r--r--   0 vsts      (1001) docker     (116)     1610 2022-08-10 09:12:39.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/ConfigDeviceDetection.i
+-rw-r--r--   0 vsts      (1001) docker     (116)     1840 2022-08-10 09:12:39.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/EngineDeviceDetection.cpp
+-rw-r--r--   0 vsts      (1001) docker     (116)     4901 2022-08-10 09:12:39.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/EngineDeviceDetection.hpp
+-rw-r--r--   0 vsts      (1001) docker     (116)     1702 2022-08-10 09:12:39.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/EngineDeviceDetection.i
+-rw-r--r--   0 vsts      (1001) docker     (116)     1654 2022-08-10 09:12:39.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/EvidenceDeviceDetection.cpp
+-rw-r--r--   0 vsts      (1001) docker     (116)     2781 2022-08-10 09:12:39.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/EvidenceDeviceDetection.hpp
+-rw-r--r--   0 vsts      (1001) docker     (116)     1420 2022-08-10 09:12:39.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/EvidenceDeviceDetection.i
+-rw-r--r--   0 vsts      (1001) docker     (116)     1603 2022-08-10 09:12:39.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/FiftyoneDegrees.hpp
+-rw-r--r--   0 vsts      (1001) docker     (116)     1565 2022-08-10 09:12:39.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/ResultsDeviceDetection.cpp
+-rw-r--r--   0 vsts      (1001) docker     (116)     4236 2022-08-10 09:12:39.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/ResultsDeviceDetection.hpp
+-rw-r--r--   0 vsts      (1001) docker     (116)     1527 2022-08-10 09:12:39.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/ResultsDeviceDetection.i
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2022-08-10 09:13:05.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/
+-rw-r--r--   0 vsts      (1001) docker     (116)     3998 2022-08-10 09:12:48.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/Collection.hpp
+-rw-r--r--   0 vsts      (1001) docker     (116)     1409 2022-08-10 09:12:48.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/Collection.i
+-rw-r--r--   0 vsts      (1001) docker     (116)     2344 2022-08-10 09:12:48.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/CollectionConfig.cpp
+-rw-r--r--   0 vsts      (1001) docker     (116)     3937 2022-08-10 09:12:48.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/CollectionConfig.hpp
+-rw-r--r--   0 vsts      (1001) docker     (116)     1504 2022-08-10 09:12:48.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/CollectionConfig.i
+-rw-r--r--   0 vsts      (1001) docker     (116)     2135 2022-08-10 09:12:48.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/ComponentMetaData.cpp
+-rw-r--r--   0 vsts      (1001) docker     (116)     3203 2022-08-10 09:12:48.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/ComponentMetaData.hpp
+-rw-r--r--   0 vsts      (1001) docker     (116)     1406 2022-08-10 09:12:48.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/ComponentMetaData.i
+-rw-r--r--   0 vsts      (1001) docker     (116)     2640 2022-08-10 09:12:48.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/ConfigBase.cpp
+-rw-r--r--   0 vsts      (1001) docker     (116)     5582 2022-08-10 09:12:48.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/ConfigBase.hpp
+-rw-r--r--   0 vsts      (1001) docker     (116)     1706 2022-08-10 09:12:48.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/ConfigBase.i
+-rw-r--r--   0 vsts      (1001) docker     (116)     1349 2022-08-10 09:12:48.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/Coordinate.i
+-rw-r--r--   0 vsts      (1001) docker     (116)     1651 2022-08-10 09:12:48.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/CsTypes.i
+-rw-r--r--   0 vsts      (1001) docker     (116)     1552 2022-08-10 09:12:48.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/Date.cpp
+-rw-r--r--   0 vsts      (1001) docker     (116)     2704 2022-08-10 09:12:48.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/Date.hpp
+-rw-r--r--   0 vsts      (1001) docker     (116)     1278 2022-08-10 09:12:48.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/Date.i
+-rw-r--r--   0 vsts      (1001) docker     (116)     4758 2022-08-10 09:12:48.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/EngineBase.cpp
+-rw-r--r--   0 vsts      (1001) docker     (116)     9509 2022-08-10 09:12:48.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/EngineBase.hpp
+-rw-r--r--   0 vsts      (1001) docker     (116)     2238 2022-08-10 09:12:48.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/EngineBase.i
+-rw-r--r--   0 vsts      (1001) docker     (116)     3071 2022-08-10 09:12:48.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/EntityMetaData.hpp
+-rw-r--r--   0 vsts      (1001) docker     (116)     2659 2022-08-10 09:12:48.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/EntityMetaDataBuilder.hpp
+-rw-r--r--   0 vsts      (1001) docker     (116)     2635 2022-08-10 09:12:48.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/EvidenceBase.cpp
+-rw-r--r--   0 vsts      (1001) docker     (116)     4021 2022-08-10 09:12:48.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/EvidenceBase.hpp
+-rw-r--r--   0 vsts      (1001) docker     (116)     1378 2022-08-10 09:12:48.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/EvidenceBase.i
+-rw-r--r--   0 vsts      (1001) docker     (116)     3299 2022-08-10 09:12:48.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/Exceptions.cpp
+-rw-r--r--   0 vsts      (1001) docker     (116)     4768 2022-08-10 09:12:48.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/Exceptions.hpp
+-rw-r--r--   0 vsts      (1001) docker     (116)     2054 2022-08-10 09:12:48.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/Exceptions.i
+-rw-r--r--   0 vsts      (1001) docker     (116)     1448 2022-08-10 09:12:48.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/FiftyoneDegrees.hpp
+-rw-r--r--   0 vsts      (1001) docker     (116)     4116 2022-08-10 09:12:48.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/JavaTypes.i
+-rw-r--r--   0 vsts      (1001) docker     (116)     1969 2022-08-10 09:12:48.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/MapStringStringIterator.i
+-rw-r--r--   0 vsts      (1001) docker     (116)     1788 2022-08-10 09:12:48.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/MetaData.cpp
+-rw-r--r--   0 vsts      (1001) docker     (116)     8088 2022-08-10 09:12:48.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/MetaData.hpp
+-rw-r--r--   0 vsts      (1001) docker     (116)     3087 2022-08-10 09:12:48.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/MetaData.i
+-rw-r--r--   0 vsts      (1001) docker     (116)     1840 2022-08-10 09:12:48.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/ProfileMetaData.cpp
+-rw-r--r--   0 vsts      (1001) docker     (116)     2778 2022-08-10 09:12:48.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/ProfileMetaData.hpp
+-rw-r--r--   0 vsts      (1001) docker     (116)     1348 2022-08-10 09:12:48.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/ProfileMetaData.i
+-rw-r--r--   0 vsts      (1001) docker     (116)     4253 2022-08-10 09:12:48.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/PropertyMetaData.cpp
+-rw-r--r--   0 vsts      (1001) docker     (116)     7978 2022-08-10 09:12:48.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/PropertyMetaData.hpp
+-rw-r--r--   0 vsts      (1001) docker     (116)     1684 2022-08-10 09:12:48.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/PropertyMetaData.i
+-rw-r--r--   0 vsts      (1001) docker     (116)     4414 2022-08-10 09:12:48.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/RequiredPropertiesConfig.cpp
+-rw-r--r--   0 vsts      (1001) docker     (116)     5326 2022-08-10 09:12:48.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/RequiredPropertiesConfig.hpp
+-rw-r--r--   0 vsts      (1001) docker     (116)     1571 2022-08-10 09:12:48.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/RequiredPropertiesConfig.i
+-rw-r--r--   0 vsts      (1001) docker     (116)     8176 2022-08-10 09:12:48.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/ResultsBase.cpp
+-rw-r--r--   0 vsts      (1001) docker     (116)    16639 2022-08-10 09:12:48.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/ResultsBase.hpp
+-rw-r--r--   0 vsts      (1001) docker     (116)     2209 2022-08-10 09:12:48.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/ResultsBase.i
+-rw-r--r--   0 vsts      (1001) docker     (116)     1392 2022-08-10 09:12:48.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/Types.i
+-rw-r--r--   0 vsts      (1001) docker     (116)     6224 2022-08-10 09:12:48.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/Value.hpp
+-rw-r--r--   0 vsts      (1001) docker     (116)     1563 2022-08-10 09:12:48.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/Value.i
+-rw-r--r--   0 vsts      (1001) docker     (116)     3464 2022-08-10 09:12:48.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/ValueMetaData.cpp
+-rw-r--r--   0 vsts      (1001) docker     (116)     4936 2022-08-10 09:12:48.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/ValueMetaData.hpp
+-rw-r--r--   0 vsts      (1001) docker     (116)     1641 2022-08-10 09:12:48.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/ValueMetaData.i
+-rw-r--r--   0 vsts      (1001) docker     (116)     2676 2022-08-10 09:12:48.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/array.h
+-rw-r--r--   0 vsts      (1001) docker     (116)     1751 2022-08-10 09:12:48.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/bool.h
+-rw-r--r--   0 vsts      (1001) docker     (116)    12861 2022-08-10 09:12:48.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/cache.c
+-rw-r--r--   0 vsts      (1001) docker     (116)    10543 2022-08-10 09:12:48.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/cache.h
+-rw-r--r--   0 vsts      (1001) docker     (116)    33990 2022-08-10 09:12:48.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/collection.c
+-rw-r--r--   0 vsts      (1001) docker     (116)    29281 2022-08-10 09:12:48.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/collection.h
+-rw-r--r--   0 vsts      (1001) docker     (116)     1568 2022-08-10 09:12:48.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/common.h
+-rw-r--r--   0 vsts      (1001) docker     (116)     3826 2022-08-10 09:12:48.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/component.c
+-rw-r--r--   0 vsts      (1001) docker     (116)     6697 2022-08-10 09:12:48.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/component.h
+-rw-r--r--   0 vsts      (1001) docker     (116)     4344 2022-08-10 09:12:48.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/config.h
+-rw-r--r--   0 vsts      (1001) docker     (116)     2566 2022-08-10 09:12:48.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/coordinate.h
+-rw-r--r--   0 vsts      (1001) docker     (116)     1727 2022-08-10 09:12:48.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/data.c
+-rw-r--r--   0 vsts      (1001) docker     (116)     4547 2022-08-10 09:12:48.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/data.h
+-rw-r--r--   0 vsts      (1001) docker     (116)    10232 2022-08-10 09:12:48.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/dataset.c
+-rw-r--r--   0 vsts      (1001) docker     (116)    18728 2022-08-10 09:12:48.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/dataset.h
+-rw-r--r--   0 vsts      (1001) docker     (116)     2247 2022-08-10 09:12:48.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/date.h
+-rw-r--r--   0 vsts      (1001) docker     (116)     5656 2022-08-10 09:12:49.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/evidence.c
+-rw-r--r--   0 vsts      (1001) docker     (116)     9692 2022-08-10 09:12:49.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/evidence.h
+-rw-r--r--   0 vsts      (1001) docker     (116)     6994 2022-08-10 09:12:49.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/exceptions.h
+-rw-r--r--   0 vsts      (1001) docker     (116)     2776 2022-08-10 09:12:49.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/exceptionsc.c
+-rw-r--r--   0 vsts      (1001) docker     (116)    32828 2022-08-10 09:12:49.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/fiftyone.h
+-rw-r--r--   0 vsts      (1001) docker     (116)    29063 2022-08-10 09:12:49.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/file.c
+-rw-r--r--   0 vsts      (1001) docker     (116)    18100 2022-08-10 09:12:49.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/file.h
+-rw-r--r--   0 vsts      (1001) docker     (116)     5139 2022-08-10 09:12:49.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/float.c
+-rw-r--r--   0 vsts      (1001) docker     (116)     7348 2022-08-10 09:12:49.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/float.h
+-rw-r--r--   0 vsts      (1001) docker     (116)    11885 2022-08-10 09:12:49.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/headers.c
+-rw-r--r--   0 vsts      (1001) docker     (116)     8284 2022-08-10 09:12:49.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/headers.h
+-rw-r--r--   0 vsts      (1001) docker     (116)     7452 2022-08-10 09:12:49.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/ip.c
+-rw-r--r--   0 vsts      (1001) docker     (116)     4847 2022-08-10 09:12:49.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/ip.h
+-rw-r--r--   0 vsts      (1001) docker     (116)     2357 2022-08-10 09:12:49.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/list.c
+-rw-r--r--   0 vsts      (1001) docker     (116)     5593 2022-08-10 09:12:49.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/list.h
+-rw-r--r--   0 vsts      (1001) docker     (116)     8984 2022-08-10 09:12:49.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/memory.c
+-rw-r--r--   0 vsts      (1001) docker     (116)     7639 2022-08-10 09:12:49.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/memory.h
+-rw-r--r--   0 vsts      (1001) docker     (116)    12916 2022-08-10 09:12:49.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/overrides.c
+-rw-r--r--   0 vsts      (1001) docker     (116)    10180 2022-08-10 09:12:49.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/overrides.h
+-rw-r--r--   0 vsts      (1001) docker     (116)     1418 2022-08-10 09:12:49.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/pair.h
+-rw-r--r--   0 vsts      (1001) docker     (116)     4611 2022-08-10 09:12:49.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/pool.c
+-rw-r--r--   0 vsts      (1001) docker     (116)     9648 2022-08-10 09:12:49.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/pool.h
+-rw-r--r--   0 vsts      (1001) docker     (116)     1544 2022-08-10 09:12:49.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/process.c
+-rw-r--r--   0 vsts      (1001) docker     (116)     1429 2022-08-10 09:12:49.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/process.h
+-rw-r--r--   0 vsts      (1001) docker     (116)     9403 2022-08-10 09:12:49.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/profile.c
+-rw-r--r--   0 vsts      (1001) docker     (116)     9813 2022-08-10 09:12:49.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/profile.h
+-rw-r--r--   0 vsts      (1001) docker     (116)    14964 2022-08-10 09:12:49.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/properties.c
+-rw-r--r--   0 vsts      (1001) docker     (116)    13395 2022-08-10 09:12:49.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/properties.h
+-rw-r--r--   0 vsts      (1001) docker     (116)     4708 2022-08-10 09:12:49.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/property.c
+-rw-r--r--   0 vsts      (1001) docker     (116)    10041 2022-08-10 09:12:49.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/property.h
+-rw-r--r--   0 vsts      (1001) docker     (116)     9458 2022-08-10 09:12:49.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/pseudoheader.c
+-rw-r--r--   0 vsts      (1001) docker     (116)     3606 2022-08-10 09:12:49.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/pseudoheader.h
+-rw-r--r--   0 vsts      (1001) docker     (116)    12300 2022-08-10 09:12:49.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/resource.c
+-rw-r--r--   0 vsts      (1001) docker     (116)     9878 2022-08-10 09:12:49.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/resource.h
+-rw-r--r--   0 vsts      (1001) docker     (116)     1388 2022-08-10 09:12:49.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/results.c
+-rw-r--r--   0 vsts      (1001) docker     (116)     4351 2022-08-10 09:12:49.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/results.h
+-rw-r--r--   0 vsts      (1001) docker     (116)     1571 2022-08-10 09:12:49.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/snprintf.h
+-rw-r--r--   0 vsts      (1001) docker     (116)     6158 2022-08-10 09:12:49.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/status.c
+-rw-r--r--   0 vsts      (1001) docker     (116)     7434 2022-08-10 09:12:49.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/status.h
+-rw-r--r--   0 vsts      (1001) docker     (116)     2915 2022-08-10 09:12:49.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/string.c
+-rw-r--r--   0 vsts      (1001) docker     (116)     6596 2022-08-10 09:12:49.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/string.h
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2022-08-10 09:13:05.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/tests/
+-rw-r--r--   0 vsts      (1001) docker     (116)     3900 2022-08-10 09:12:49.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/tests/Base.hpp
+-rw-r--r--   0 vsts      (1001) docker     (116)     3698 2022-08-10 09:12:49.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/tests/EngineTests.hpp
+-rw-r--r--   0 vsts      (1001) docker     (116)     2482 2022-08-10 09:12:49.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/tests/EvidenceTests.hpp
+-rw-r--r--   0 vsts      (1001) docker     (116)     1398 2022-08-10 09:12:49.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/tests/ExampleTests.hpp
+-rw-r--r--   0 vsts      (1001) docker     (116)     1747 2022-08-10 09:12:49.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/tests/FileHandle.hpp
+-rw-r--r--   0 vsts      (1001) docker     (116)     2137 2022-08-10 09:12:49.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/tests/PseudoHeaderTests.hpp
+-rw-r--r--   0 vsts      (1001) docker     (116)     2046 2022-08-10 09:12:49.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/tests/StringCollection.hpp
+-rw-r--r--   0 vsts      (1001) docker     (116)     1355 2022-08-10 09:12:49.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/tests/TestStrings.hpp
+-rw-r--r--   0 vsts      (1001) docker     (116)     1541 2022-08-10 09:12:49.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/tests/pch.h
+-rw-r--r--   0 vsts      (1001) docker     (116)     3499 2022-08-10 09:12:49.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/textfile.c
+-rw-r--r--   0 vsts      (1001) docker     (116)     2932 2022-08-10 09:12:49.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/textfile.h
+-rw-r--r--   0 vsts      (1001) docker     (116)     3734 2022-08-10 09:12:49.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/threading.c
+-rw-r--r--   0 vsts      (1001) docker     (116)    14531 2022-08-10 09:12:49.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/threading.h
+-rw-r--r--   0 vsts      (1001) docker     (116)    10109 2022-08-10 09:12:49.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/tree.c
+-rw-r--r--   0 vsts      (1001) docker     (116)     6469 2022-08-10 09:12:49.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/tree.h
+-rw-r--r--   0 vsts      (1001) docker     (116)     7116 2022-08-10 09:12:49.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/value.c
+-rw-r--r--   0 vsts      (1001) docker     (116)     7404 2022-08-10 09:12:49.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/value.h
+-rw-r--r--   0 vsts      (1001) docker     (116)     4063 2022-08-10 09:12:49.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/yamlfile.h
+-rw-r--r--   0 vsts      (1001) docker     (116)     3660 2022-08-10 09:12:39.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/config-dd.h
+-rw-r--r--   0 vsts      (1001) docker     (116)     3122 2022-08-10 09:12:39.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/dataset-dd.c
+-rw-r--r--   0 vsts      (1001) docker     (116)     4480 2022-08-10 09:12:39.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/dataset-dd.h
+-rw-r--r--   0 vsts      (1001) docker     (116)     3440 2022-08-10 09:12:39.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/fiftyone.h
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2022-08-10 09:13:05.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/
+-rw-r--r--   0 vsts      (1001) docker     (116)     1974 2022-08-10 09:12:39.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ComponentMetaDataBuilderHash.cpp
+-rw-r--r--   0 vsts      (1001) docker     (116)     2374 2022-08-10 09:12:39.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ComponentMetaDataBuilderHash.hpp
+-rw-r--r--   0 vsts      (1001) docker     (116)     2554 2022-08-10 09:12:39.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ComponentMetaDataCollectionHash.cpp
+-rw-r--r--   0 vsts      (1001) docker     (116)     2724 2022-08-10 09:12:39.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ComponentMetaDataCollectionHash.hpp
+-rw-r--r--   0 vsts      (1001) docker     (116)     5422 2022-08-10 09:12:39.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ConfigHash.cpp
+-rw-r--r--   0 vsts      (1001) docker     (116)    10458 2022-08-10 09:12:39.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ConfigHash.hpp
+-rw-r--r--   0 vsts      (1001) docker     (116)     2103 2022-08-10 09:12:39.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ConfigHash.i
+-rw-r--r--   0 vsts      (1001) docker     (116)     7613 2022-08-10 09:12:39.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/EngineHash.cpp
+-rw-r--r--   0 vsts      (1001) docker     (116)     6743 2022-08-10 09:12:39.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/EngineHash.hpp
+-rw-r--r--   0 vsts      (1001) docker     (116)     2172 2022-08-10 09:12:39.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/EngineHash.i
+-rw-r--r--   0 vsts      (1001) docker     (116)     4522 2022-08-10 09:12:39.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/MetaDataHash.cpp
+-rw-r--r--   0 vsts      (1001) docker     (116)     3586 2022-08-10 09:12:39.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/MetaDataHash.hpp
+-rw-r--r--   0 vsts      (1001) docker     (116)     1617 2022-08-10 09:12:39.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ProfileMetaDataBuilderHash.cpp
+-rw-r--r--   0 vsts      (1001) docker     (116)     2348 2022-08-10 09:12:39.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ProfileMetaDataBuilderHash.hpp
+-rw-r--r--   0 vsts      (1001) docker     (116)     2823 2022-08-10 09:12:39.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ProfileMetaDataCollectionHash.cpp
+-rw-r--r--   0 vsts      (1001) docker     (116)     2829 2022-08-10 09:12:39.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ProfileMetaDataCollectionHash.hpp
+-rw-r--r--   0 vsts      (1001) docker     (116)     5489 2022-08-10 09:12:39.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/PropertyMetaDataBuilderHash.cpp
+-rw-r--r--   0 vsts      (1001) docker     (116)     4476 2022-08-10 09:12:39.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/PropertyMetaDataBuilderHash.hpp
+-rw-r--r--   0 vsts      (1001) docker     (116)     3179 2022-08-10 09:12:39.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/PropertyMetaDataCollectionForComponentHash.cpp
+-rw-r--r--   0 vsts      (1001) docker     (116)     3033 2022-08-10 09:12:39.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/PropertyMetaDataCollectionForComponentHash.hpp
+-rw-r--r--   0 vsts      (1001) docker     (116)     2957 2022-08-10 09:12:39.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/PropertyMetaDataCollectionForPropertyHash.cpp
+-rw-r--r--   0 vsts      (1001) docker     (116)     2525 2022-08-10 09:12:39.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/PropertyMetaDataCollectionForPropertyHash.hpp
+-rw-r--r--   0 vsts      (1001) docker     (116)     2810 2022-08-10 09:12:39.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/PropertyMetaDataCollectionHash.cpp
+-rw-r--r--   0 vsts      (1001) docker     (116)     2714 2022-08-10 09:12:39.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/PropertyMetaDataCollectionHash.hpp
+-rw-r--r--   0 vsts      (1001) docker     (116)     7319 2022-08-10 09:12:39.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ResultsHash.cpp
+-rw-r--r--   0 vsts      (1001) docker     (116)     6726 2022-08-10 09:12:39.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ResultsHash.hpp
+-rw-r--r--   0 vsts      (1001) docker     (116)     1790 2022-08-10 09:12:39.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ResultsHash.i
+-rw-r--r--   0 vsts      (1001) docker     (116)     2133 2022-08-10 09:12:39.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ValueMetaDataBuilderHash.cpp
+-rw-r--r--   0 vsts      (1001) docker     (116)     2318 2022-08-10 09:12:39.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ValueMetaDataBuilderHash.hpp
+-rw-r--r--   0 vsts      (1001) docker     (116)     2577 2022-08-10 09:12:39.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ValueMetaDataCollectionBaseHash.cpp
+-rw-r--r--   0 vsts      (1001) docker     (116)     2564 2022-08-10 09:12:39.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ValueMetaDataCollectionBaseHash.hpp
+-rw-r--r--   0 vsts      (1001) docker     (116)     4508 2022-08-10 09:12:39.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ValueMetaDataCollectionForProfileHash.cpp
+-rw-r--r--   0 vsts      (1001) docker     (116)     3404 2022-08-10 09:12:39.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ValueMetaDataCollectionForProfileHash.hpp
+-rw-r--r--   0 vsts      (1001) docker     (116)     3265 2022-08-10 09:12:39.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ValueMetaDataCollectionForPropertyHash.cpp
+-rw-r--r--   0 vsts      (1001) docker     (116)     3057 2022-08-10 09:12:39.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ValueMetaDataCollectionForPropertyHash.hpp
+-rw-r--r--   0 vsts      (1001) docker     (116)     2219 2022-08-10 09:12:39.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ValueMetaDataCollectionHash.cpp
+-rw-r--r--   0 vsts      (1001) docker     (116)     2482 2022-08-10 09:12:39.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ValueMetaDataCollectionHash.hpp
+-rw-r--r--   0 vsts      (1001) docker     (116)     7710 2022-08-10 09:12:39.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/fiftyone.h
+-rw-r--r--   0 vsts      (1001) docker     (116)    10280 2022-08-10 09:12:39.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/graph.c
+-rw-r--r--   0 vsts      (1001) docker     (116)    13280 2022-08-10 09:12:39.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/graph.h
+-rw-r--r--   0 vsts      (1001) docker     (116)   101660 2022-08-10 09:12:39.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/hash.c
+-rw-r--r--   0 vsts      (1001) docker     (116)    38142 2022-08-10 09:12:39.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/hash.h
+-rw-r--r--   0 vsts      (1001) docker     (116)     1826 2022-08-10 09:12:39.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/hash.i
+-rw-r--r--   0 vsts      (1001) docker     (116)     2846 2022-08-10 09:12:39.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/results-dd.c
+-rw-r--r--   0 vsts      (1001) docker     (116)     5261 2022-08-10 09:12:39.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/results-dd.h
+-rw-r--r--   0 vsts      (1001) docker     (116)     3677 2022-08-10 09:12:36.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/devicedetection_datafile.py
+-rw-r--r--   0 vsts      (1001) docker     (116)    15789 2022-08-10 09:12:36.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/devicedetection_onpremise.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     7149 2022-08-10 09:12:36.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/devicedetection_onpremise_pipelinebuilder.py
+-rw-r--r--   0 vsts      (1001) docker     (116)   818429 2022-08-10 09:12:36.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/hash_python_wrap.cxx
+-rw-r--r--   0 vsts      (1001) docker     (116)     5451 2022-08-10 09:12:36.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/swig_data.py
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2022-08-10 09:13:05.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (116)     4271 2022-08-10 09:13:05.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (116)    16937 2022-08-10 09:13:05.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (116)        1 2022-08-10 09:13:05.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (116)       67 2022-08-10 09:13:05.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (116)       68 2022-08-10 09:13:05.000000 fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (116)       38 2022-08-10 09:13:05.000000 fiftyone_devicedetection_onpremise-4.4.9/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (116)    13632 2022-08-10 09:12:36.000000 fiftyone_devicedetection_onpremise-4.4.9/setup.py
+-rw-r--r--   0 vsts      (1001) docker     (116)        6 2022-08-10 09:13:04.000000 fiftyone_devicedetection_onpremise-4.4.9/version.txt
```

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/PKG-INFO` & `fiftyone_devicedetection_onpremise-4.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiftyone_devicedetection_onpremise
-Version: 4.4.8
+Version: 4.4.9
 Summary: This project contains 51Degrees Device Detection OnPremise engine that can be used with the Pipeline API.The Pipeline is a generic web request intelligence and data processing solution with the ability to add a range of 51Degrees and/or custom plug ins (Engines)
 Home-page: UNKNOWN
 Author: 51Degrees.com
 Author-email: support@51degrees.com
 License: EUPL-1.2
 Description: # 51Degrees Device Detection Engines - On-Premise
```

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/DeviceDetectionHashEngineModule.py` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/DeviceDetectionHashEngineModule.py`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/constants.py` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/constants.py`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/ConfigDeviceDetection.cpp` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/ConfigDeviceDetection.cpp`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/ConfigDeviceDetection.hpp` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/ConfigDeviceDetection.hpp`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/ConfigDeviceDetection.i` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/ConfigDeviceDetection.i`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/EngineDeviceDetection.cpp` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/EngineDeviceDetection.cpp`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/EngineDeviceDetection.hpp` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/EngineDeviceDetection.hpp`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/EngineDeviceDetection.i` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/EngineDeviceDetection.i`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/EvidenceDeviceDetection.cpp` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/EvidenceDeviceDetection.cpp`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/EvidenceDeviceDetection.hpp` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/EvidenceDeviceDetection.hpp`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/EvidenceDeviceDetection.i` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/EvidenceDeviceDetection.i`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/FiftyoneDegrees.hpp` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/FiftyoneDegrees.hpp`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/ResultsDeviceDetection.cpp` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/ResultsDeviceDetection.cpp`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/ResultsDeviceDetection.hpp` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/ResultsDeviceDetection.hpp`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/ResultsDeviceDetection.i` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/ResultsDeviceDetection.i`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/Collection.hpp` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/Collection.hpp`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/Collection.i` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/Collection.i`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/CollectionConfig.cpp` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/CollectionConfig.cpp`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/CollectionConfig.hpp` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/CollectionConfig.hpp`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/CollectionConfig.i` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/CollectionConfig.i`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/ComponentMetaData.cpp` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/ComponentMetaData.cpp`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/ComponentMetaData.hpp` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/ComponentMetaData.hpp`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/ComponentMetaData.i` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/ComponentMetaData.i`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/ConfigBase.cpp` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/ConfigBase.cpp`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/ConfigBase.hpp` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/ConfigBase.hpp`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/ConfigBase.i` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/ConfigBase.i`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/Coordinate.i` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/Coordinate.i`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/CsTypes.i` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/CsTypes.i`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/Date.cpp` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/Date.cpp`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/Date.hpp` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/Date.hpp`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/Date.i` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/Date.i`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/EngineBase.cpp` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/EngineBase.cpp`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/EngineBase.hpp` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/EngineBase.hpp`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/EngineBase.i` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/EngineBase.i`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/EntityMetaData.hpp` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/EntityMetaData.hpp`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/EntityMetaDataBuilder.hpp` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/EntityMetaDataBuilder.hpp`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/EvidenceBase.cpp` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/EvidenceBase.cpp`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/EvidenceBase.hpp` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/EvidenceBase.hpp`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/EvidenceBase.i` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/EvidenceBase.i`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/Exceptions.cpp` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/Exceptions.cpp`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/Exceptions.hpp` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/Exceptions.hpp`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/Exceptions.i` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/Exceptions.i`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/FiftyoneDegrees.hpp` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/FiftyoneDegrees.hpp`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/JavaTypes.i` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/JavaTypes.i`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/MapStringStringIterator.i` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/MapStringStringIterator.i`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/MetaData.cpp` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/MetaData.cpp`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/MetaData.hpp` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/MetaData.hpp`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/MetaData.i` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/MetaData.i`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/ProfileMetaData.cpp` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/ProfileMetaData.cpp`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/ProfileMetaData.hpp` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/ProfileMetaData.hpp`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/ProfileMetaData.i` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/ProfileMetaData.i`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/PropertyMetaData.cpp` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/PropertyMetaData.cpp`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/PropertyMetaData.hpp` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/PropertyMetaData.hpp`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/PropertyMetaData.i` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/PropertyMetaData.i`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/RequiredPropertiesConfig.cpp` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/RequiredPropertiesConfig.cpp`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/RequiredPropertiesConfig.hpp` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/RequiredPropertiesConfig.hpp`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/RequiredPropertiesConfig.i` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/RequiredPropertiesConfig.i`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/ResultsBase.cpp` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/ResultsBase.cpp`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/ResultsBase.hpp` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/ResultsBase.hpp`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/ResultsBase.i` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/ResultsBase.i`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/Types.i` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/Types.i`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/Value.hpp` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/Value.hpp`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/Value.i` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/Value.i`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/ValueMetaData.cpp` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/ValueMetaData.cpp`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/ValueMetaData.hpp` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/ValueMetaData.hpp`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/ValueMetaData.i` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/ValueMetaData.i`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/array.h` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/array.h`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/bool.h` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/bool.h`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/cache.c` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/cache.c`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/cache.h` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/cache.h`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/collection.c` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/collection.c`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/collection.h` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/collection.h`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/common.h` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/common.h`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/component.c` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/component.c`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/component.h` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/component.h`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/config.h` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/config.h`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/coordinate.h` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/coordinate.h`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/data.c` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/data.c`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/data.h` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/data.h`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/dataset.c` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/dataset.c`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/dataset.h` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/dataset.h`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/date.h` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/date.h`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/evidence.c` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/evidence.c`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/evidence.h` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/evidence.h`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/exceptions.h` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/exceptions.h`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/exceptionsc.c` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/exceptionsc.c`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/fiftyone.h` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/fiftyone.h`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/file.c` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/file.c`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/file.h` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/file.h`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/float.c` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/float.c`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/float.h` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/float.h`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/headers.c` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/headers.c`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/headers.h` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/headers.h`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/ip.c` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/ip.c`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/ip.h` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/ip.h`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/list.c` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/list.c`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/list.h` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/list.h`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/memory.c` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/memory.c`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/memory.h` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/memory.h`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/overrides.c` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/overrides.c`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/overrides.h` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/overrides.h`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/pair.h` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/pair.h`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/pool.c` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/pool.c`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/pool.h` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/pool.h`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/process.c` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/process.c`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/process.h` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/process.h`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/profile.c` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/profile.c`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/profile.h` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/profile.h`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/properties.c` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/properties.c`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/properties.h` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/properties.h`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/property.c` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/property.c`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/property.h` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/property.h`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/pseudoheader.c` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/pseudoheader.c`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/pseudoheader.h` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/pseudoheader.h`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/resource.c` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/resource.c`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/resource.h` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/resource.h`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/results.c` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/results.c`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/results.h` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/results.h`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/snprintf.h` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/snprintf.h`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/status.c` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/status.c`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/status.h` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/status.h`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/string.c` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/string.c`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/string.h` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/string.h`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/tests/Base.hpp` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/tests/Base.hpp`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/tests/EngineTests.hpp` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/tests/EngineTests.hpp`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/tests/EvidenceTests.hpp` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/tests/EvidenceTests.hpp`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/tests/ExampleTests.hpp` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/tests/ExampleTests.hpp`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/tests/FileHandle.hpp` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/tests/FileHandle.hpp`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/tests/PseudoHeaderTests.hpp` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/tests/PseudoHeaderTests.hpp`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/tests/StringCollection.hpp` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/tests/StringCollection.hpp`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/tests/TestStrings.hpp` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/tests/TestStrings.hpp`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/tests/pch.h` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/tests/pch.h`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/textfile.c` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/textfile.c`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/textfile.h` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/textfile.h`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/threading.c` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/threading.c`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/threading.h` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/threading.h`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/tree.c` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/tree.c`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/tree.h` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/tree.h`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/value.c` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/value.c`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/value.h` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/value.h`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/yamlfile.h` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/common-cxx/yamlfile.h`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/config-dd.h` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/config-dd.h`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/dataset-dd.c` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/dataset-dd.c`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/dataset-dd.h` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/dataset-dd.h`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/fiftyone.h` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/fiftyone.h`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ComponentMetaDataBuilderHash.cpp` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ComponentMetaDataBuilderHash.cpp`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ComponentMetaDataBuilderHash.hpp` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ComponentMetaDataBuilderHash.hpp`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ComponentMetaDataCollectionHash.cpp` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ComponentMetaDataCollectionHash.cpp`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ComponentMetaDataCollectionHash.hpp` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ComponentMetaDataCollectionHash.hpp`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ConfigHash.cpp` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ConfigHash.cpp`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ConfigHash.hpp` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ConfigHash.hpp`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ConfigHash.i` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ConfigHash.i`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/EngineHash.cpp` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/EngineHash.cpp`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/EngineHash.hpp` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/EngineHash.hpp`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/EngineHash.i` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/EngineHash.i`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/MetaDataHash.cpp` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/MetaDataHash.cpp`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/MetaDataHash.hpp` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/MetaDataHash.hpp`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ProfileMetaDataBuilderHash.cpp` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ProfileMetaDataBuilderHash.cpp`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ProfileMetaDataBuilderHash.hpp` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ProfileMetaDataBuilderHash.hpp`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ProfileMetaDataCollectionHash.cpp` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ProfileMetaDataCollectionHash.cpp`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ProfileMetaDataCollectionHash.hpp` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ProfileMetaDataCollectionHash.hpp`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/PropertyMetaDataBuilderHash.cpp` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/PropertyMetaDataBuilderHash.cpp`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/PropertyMetaDataBuilderHash.hpp` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/PropertyMetaDataBuilderHash.hpp`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/PropertyMetaDataCollectionForComponentHash.cpp` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/PropertyMetaDataCollectionForComponentHash.cpp`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/PropertyMetaDataCollectionForComponentHash.hpp` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/PropertyMetaDataCollectionForComponentHash.hpp`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/PropertyMetaDataCollectionForPropertyHash.cpp` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/PropertyMetaDataCollectionForPropertyHash.cpp`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/PropertyMetaDataCollectionForPropertyHash.hpp` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/PropertyMetaDataCollectionForPropertyHash.hpp`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/PropertyMetaDataCollectionHash.cpp` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/PropertyMetaDataCollectionHash.cpp`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/PropertyMetaDataCollectionHash.hpp` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/PropertyMetaDataCollectionHash.hpp`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ResultsHash.cpp` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ResultsHash.cpp`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ResultsHash.hpp` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ResultsHash.hpp`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ResultsHash.i` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ResultsHash.i`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ValueMetaDataBuilderHash.cpp` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ValueMetaDataBuilderHash.cpp`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ValueMetaDataBuilderHash.hpp` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ValueMetaDataBuilderHash.hpp`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ValueMetaDataCollectionBaseHash.cpp` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ValueMetaDataCollectionBaseHash.cpp`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ValueMetaDataCollectionBaseHash.hpp` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ValueMetaDataCollectionBaseHash.hpp`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ValueMetaDataCollectionForProfileHash.cpp` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ValueMetaDataCollectionForProfileHash.cpp`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ValueMetaDataCollectionForProfileHash.hpp` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ValueMetaDataCollectionForProfileHash.hpp`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ValueMetaDataCollectionForPropertyHash.cpp` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ValueMetaDataCollectionForPropertyHash.cpp`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ValueMetaDataCollectionForPropertyHash.hpp` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ValueMetaDataCollectionForPropertyHash.hpp`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ValueMetaDataCollectionHash.cpp` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ValueMetaDataCollectionHash.cpp`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ValueMetaDataCollectionHash.hpp` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/ValueMetaDataCollectionHash.hpp`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/fiftyone.h` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/fiftyone.h`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/graph.c` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/graph.c`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/graph.h` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/graph.h`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/hash.c` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/hash.c`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/hash.h` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/hash.h`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/hash.i` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/hash/hash.i`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/results-dd.c` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/results-dd.c`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/device-detection-cxx/src/results-dd.h` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/device-detection-cxx/src/results-dd.h`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/devicedetection_datafile.py` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/devicedetection_datafile.py`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/devicedetection_onpremise.py` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/devicedetection_onpremise.py`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/devicedetection_onpremise_pipelinebuilder.py` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/devicedetection_onpremise_pipelinebuilder.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,15 +106,16 @@
         @param update_time_maximum_randomisation :
         Maximum randomisation offset in seconds to polling time interval
         @type verify_md5 : bool
         @type create_temp_copy: bool
         @param create_temp_copy: whether to copy datafile to temporary location when updating
         @type data_file_update_base_url: string
         @param data_file_update_base_url: base url for the datafile update service
-
+        @param data_file_update_service: service for the pipeline to use for auto updates instead of the default
+        @type data_file_update_service: DataFileUpdateService
         """
         if settings is None:
             settings = {}
             
         settings = merge_two_dicts(dict(**kwargs), locals())
 
         settings = merge_two_dicts(settings, settings["settings"])
```

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/hash_python_wrap.cxx` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/hash_python_wrap.cxx`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise/swig_data.py` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise/swig_data.py`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise.egg-info/PKG-INFO` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiftyone-devicedetection-onpremise
-Version: 4.4.8
+Version: 4.4.9
 Summary: This project contains 51Degrees Device Detection OnPremise engine that can be used with the Pipeline API.The Pipeline is a generic web request intelligence and data processing solution with the ability to add a range of 51Degrees and/or custom plug ins (Engines)
 Home-page: UNKNOWN
 Author: 51Degrees.com
 Author-email: support@51degrees.com
 License: EUPL-1.2
 Description: # 51Degrees Device Detection Engines - On-Premise
```

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/fiftyone_devicedetection_onpremise.egg-info/SOURCES.txt` & `fiftyone_devicedetection_onpremise-4.4.9/fiftyone_devicedetection_onpremise.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fiftyone_devicedetection_onpremise-4.4.8/setup.py` & `fiftyone_devicedetection_onpremise-4.4.9/setup.py`

 * *Files identical despite different names*

