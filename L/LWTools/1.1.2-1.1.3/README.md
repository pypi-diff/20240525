# Comparing `tmp/lwtools-1.1.2.tar.gz` & `tmp/lwtools-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lwtools-1.1.2.tar", last modified: Sat May 25 13:07:50 2024, max compression
+gzip compressed data, was "lwtools-1.1.3.tar", last modified: Sat May 25 13:13:25 2024, max compression
```

## Comparing `lwtools-1.1.2.tar` & `lwtools-1.1.3.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxrwxrwx   0        0        0        0 2024-05-25 13:07:50.107275 lwtools-1.1.2/
--rw-rw-rw-   0        0        0    35149 2023-07-20 12:51:38.000000 lwtools-1.1.2/LICENSE
-drwxrwxrwx   0        0        0        0 2024-05-25 13:07:49.188431 lwtools-1.1.2/LWT/
--rw-rw-rw-   0        0        0        0 2023-07-20 12:57:55.000000 lwtools-1.1.2/LWT/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-25 13:07:49.950736 lwtools-1.1.2/LWT/lmtanalysis/
--rw-rw-rw-   0        0        0    48218 2023-05-03 08:46:45.000000 lwtools-1.1.2/LWT/lmtanalysis/A-OldAnimal-.py
--rw-rw-rw-   0        0        0    46847 2024-01-19 13:24:49.000000 lwtools-1.1.2/LWT/lmtanalysis/Animal-.py
--rw-rw-rw-   0        0        0    57484 2024-01-19 13:24:49.000000 lwtools-1.1.2/LWT/lmtanalysis/Animal.py
--rw-rw-rw-   0        0        0     2057 2022-12-02 08:25:57.000000 lwtools-1.1.2/LWT/lmtanalysis/BehaviouralSequencesUtil.py
--rw-rw-rw-   0        0        0     2143 2024-01-19 12:46:39.000000 lwtools-1.1.2/LWT/lmtanalysis/BuildDataBaseIndex.py
--rw-rw-rw-   0        0        0     6013 2024-01-24 08:07:17.000000 lwtools-1.1.2/LWT/lmtanalysis/BuildEventApproachContact.py
--rw-rw-rw-   0        0        0     3454 2024-01-24 08:15:25.000000 lwtools-1.1.2/LWT/lmtanalysis/BuildEventApproachRear.py
--rw-rw-rw-   0        0        0     2805 2024-01-24 08:15:25.000000 lwtools-1.1.2/LWT/lmtanalysis/BuildEventCenterPeripheryLocation.py
--rw-rw-rw-   0        0        0     2402 2023-06-23 14:46:57.000000 lwtools-1.1.2/LWT/lmtanalysis/BuildEventDetection.py
--rw-rw-rw-   0        0        0        0 2023-06-07 12:33:53.000000 lwtools-1.1.2/LWT/lmtanalysis/BuildEventDistance.py
--rw-rw-rw-   0        0        0    11287 2024-01-24 08:15:25.000000 lwtools-1.1.2/LWT/lmtanalysis/BuildEventExclusiveCleanOralOralSideSideNoseAnogenitalContact.py
--rw-rw-rw-   0        0        0     4114 2024-01-24 08:06:29.000000 lwtools-1.1.2/LWT/lmtanalysis/BuildEventExclusiveMoveStopIsolated.py
--rw-rw-rw-   0        0        0     2260 2024-01-24 08:15:25.000000 lwtools-1.1.2/LWT/lmtanalysis/BuildEventExclusiveUndetected.py
--rw-rw-rw-   0        0        0     2046 2024-01-24 08:15:25.000000 lwtools-1.1.2/LWT/lmtanalysis/BuildEventFloorSniffing.py
--rw-rw-rw-   0        0        0     7773 2024-01-19 13:24:50.000000 lwtools-1.1.2/LWT/lmtanalysis/BuildEventFollowZone.py
--rw-rw-rw-   0        0        0     3391 2024-01-24 08:15:24.000000 lwtools-1.1.2/LWT/lmtanalysis/BuildEventGetAway.py
--rw-rw-rw-   0        0        0     3192 2024-01-24 08:15:25.000000 lwtools-1.1.2/LWT/lmtanalysis/BuildEventGroup2.py
--rw-rw-rw-   0        0        0     3648 2024-01-24 08:15:25.000000 lwtools-1.1.2/LWT/lmtanalysis/BuildEventGroup3.py
--rw-rw-rw-   0        0        0     3583 2024-01-24 08:15:24.000000 lwtools-1.1.2/LWT/lmtanalysis/BuildEventGroup3MakeBreak.py
--rw-rw-rw-   0        0        0     3496 2024-01-24 08:15:25.000000 lwtools-1.1.2/LWT/lmtanalysis/BuildEventGroup4.py
--rw-rw-rw-   0        0        0     4149 2024-01-24 08:15:24.000000 lwtools-1.1.2/LWT/lmtanalysis/BuildEventGroup4MakeBreak.py
--rw-rw-rw-   0        0        0     2072 2024-01-24 08:15:24.000000 lwtools-1.1.2/LWT/lmtanalysis/BuildEventHuddling.py
--rw-rw-rw-   0        0        0     6413 2024-01-24 08:15:25.000000 lwtools-1.1.2/LWT/lmtanalysis/BuildEventMove.py
--rw-rw-rw-   0        0        0     6036 2024-01-24 08:15:25.000000 lwtools-1.1.2/LWT/lmtanalysis/BuildEventNest3.py
--rw-rw-rw-   0        0        0    10885 2024-01-24 08:15:24.000000 lwtools-1.1.2/LWT/lmtanalysis/BuildEventNest4.py
--rw-rw-rw-   0        0        0     7603 2024-01-19 13:24:49.000000 lwtools-1.1.2/LWT/lmtanalysis/BuildEventNight.py
--rw-rw-rw-   0        0        0     5695 2024-01-24 08:15:25.000000 lwtools-1.1.2/LWT/lmtanalysis/BuildEventObjectSniffingNor.py
--rw-rw-rw-   0        0        0     7622 2024-01-24 08:15:24.000000 lwtools-1.1.2/LWT/lmtanalysis/BuildEventObjectSniffingNorAcquisitionWithConfig.py
--rw-rw-rw-   0        0        0     7709 2024-01-24 08:15:25.000000 lwtools-1.1.2/LWT/lmtanalysis/BuildEventObjectSniffingNorTestWithConfig.py
--rw-rw-rw-   0        0        0     5455 2024-01-19 13:24:49.000000 lwtools-1.1.2/LWT/lmtanalysis/BuildEventOnHouse.py
--rw-rw-rw-   0        0        0     2486 2024-01-24 08:15:25.000000 lwtools-1.1.2/LWT/lmtanalysis/BuildEventOralGenitalContact.py
--rw-rw-rw-   0        0        0     3196 2024-01-24 08:15:25.000000 lwtools-1.1.2/LWT/lmtanalysis/BuildEventOralOralContact.py
--rw-rw-rw-   0        0        0     5982 2024-01-24 08:15:25.000000 lwtools-1.1.2/LWT/lmtanalysis/BuildEventOralSideSequence.py
--rw-rw-rw-   0        0        0     3536 2024-01-24 08:15:25.000000 lwtools-1.1.2/LWT/lmtanalysis/BuildEventOtherContact.py
--rw-rw-rw-   0        0        0     2321 2024-01-24 08:15:25.000000 lwtools-1.1.2/LWT/lmtanalysis/BuildEventPassiveAnogenitalSniff.py
--rw-rw-rw-   0        0        0     3041 2024-01-24 08:15:24.000000 lwtools-1.1.2/LWT/lmtanalysis/BuildEventRear5.py
--rw-rw-rw-   0        0        0     2921 2024-01-24 08:15:25.000000 lwtools-1.1.2/LWT/lmtanalysis/BuildEventRearCenterPeriphery.py
--rw-rw-rw-   0        0        0     1791 2024-01-24 08:15:25.000000 lwtools-1.1.2/LWT/lmtanalysis/BuildEventSAP.py
--rw-rw-rw-   0        0        0     3480 2024-01-24 08:15:24.000000 lwtools-1.1.2/LWT/lmtanalysis/BuildEventSideBySide.py
--rw-rw-rw-   0        0        0     3765 2024-01-24 08:15:24.000000 lwtools-1.1.2/LWT/lmtanalysis/BuildEventSideBySideOpposite.py
--rw-rw-rw-   0        0        0     3998 2024-01-24 08:17:32.000000 lwtools-1.1.2/LWT/lmtanalysis/BuildEventSideWalk.py
--rw-rw-rw-   0        0        0     3152 2024-01-24 08:15:25.000000 lwtools-1.1.2/LWT/lmtanalysis/BuildEventSocialApproach.py
--rw-rw-rw-   0        0        0     3003 2024-01-24 08:15:24.000000 lwtools-1.1.2/LWT/lmtanalysis/BuildEventSocialEscape.py
--rw-rw-rw-   0        0        0     6249 2024-01-24 08:15:25.000000 lwtools-1.1.2/LWT/lmtanalysis/BuildEventStop.py
--rw-rw-rw-   0        0        0     2730 2024-01-24 08:15:25.000000 lwtools-1.1.2/LWT/lmtanalysis/BuildEventTrain2.py
--rw-rw-rw-   0        0        0     3880 2024-01-24 08:15:25.000000 lwtools-1.1.2/LWT/lmtanalysis/BuildEventTrain3.py
--rw-rw-rw-   0        0        0     4425 2024-01-24 08:15:24.000000 lwtools-1.1.2/LWT/lmtanalysis/BuildEventTrain4.py
--rw-rw-rw-   0        0        0     6496 2024-01-24 08:15:25.000000 lwtools-1.1.2/LWT/lmtanalysis/BuildEventWallJump.py
--rw-rw-rw-   0        0        0     3373 2024-01-24 08:15:25.000000 lwtools-1.1.2/LWT/lmtanalysis/BuildEventWaterPoint.py
--rw-rw-rw-   0        0        0     1141 2023-06-23 14:46:57.000000 lwtools-1.1.2/LWT/lmtanalysis/CheckWrongAnimal.py
--rw-rw-rw-   0        0        0      649 2023-06-23 14:46:57.000000 lwtools-1.1.2/LWT/lmtanalysis/Chronometer.py
--rw-rw-rw-   0        0        0     5056 2024-01-19 13:24:49.000000 lwtools-1.1.2/LWT/lmtanalysis/CorrectDetectionIntegrity.py
--rw-rw-rw-   0        0        0     4801 2024-01-19 13:24:49.000000 lwtools-1.1.2/LWT/lmtanalysis/Detection.py
--rw-rw-rw-   0        0        0    37541 2024-01-25 08:45:16.000000 lwtools-1.1.2/LWT/lmtanalysis/Event.py
--rw-rw-rw-   0        0        0     1837 2024-01-19 13:24:50.000000 lwtools-1.1.2/LWT/lmtanalysis/EventTimeLineCache.py
--rw-rw-rw-   0        0        0     4668 2022-12-02 08:25:57.000000 lwtools-1.1.2/LWT/lmtanalysis/Features.py
--rw-rw-rw-   0        0        0    12958 2024-01-31 13:56:41.000000 lwtools-1.1.2/LWT/lmtanalysis/FileUtil.py
--rw-rw-rw-   0        0        0     4540 2022-12-02 08:25:57.000000 lwtools-1.1.2/LWT/lmtanalysis/Mask.py
--rw-rw-rw-   0        0        0     2207 2022-12-02 08:25:57.000000 lwtools-1.1.2/LWT/lmtanalysis/Measure.py
--rw-rw-rw-   0        0        0      314 2022-12-02 08:25:57.000000 lwtools-1.1.2/LWT/lmtanalysis/Point.py
--rw-rw-rw-   0        0        0      375 2022-12-02 08:25:57.000000 lwtools-1.1.2/LWT/lmtanalysis/Rectangle.py
--rw-rw-rw-   0        0        0       91 2022-12-02 08:25:57.000000 lwtools-1.1.2/LWT/lmtanalysis/Settings.py
--rw-rw-rw-   0        0        0     3135 2024-01-19 13:07:58.000000 lwtools-1.1.2/LWT/lmtanalysis/TaskLogger.py
--rw-rw-rw-   0        0        0     9478 2024-01-19 13:06:18.000000 lwtools-1.1.2/LWT/lmtanalysis/Util.py
--rw-rw-rw-   0        0        0       49 2022-12-02 08:25:57.000000 lwtools-1.1.2/LWT/lmtanalysis/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-25 13:07:50.072771 lwtools-1.1.2/LWT/scripts/
--rw-rw-rw-   0        0        0     9202 2024-02-26 12:46:06.000000 lwtools-1.1.2/LWT/scripts/LMT_Widget_Tool.ipynb
--rw-rw-rw-   0        0        0     3472 2024-01-25 14:21:35.000000 lwtools-1.1.2/LWT/scripts/LWT_ChangeGenotype.py
--rw-rw-rw-   0        0        0     9124 2024-02-02 08:34:03.000000 lwtools-1.1.2/LWT/scripts/LWT_DataSplit.py
--rw-rw-rw-   0        0        0    24428 2024-01-25 08:26:15.000000 lwtools-1.1.2/LWT/scripts/LWT_Export.py
--rw-rw-rw-   0        0        0   100506 2024-02-12 08:34:52.000000 lwtools-1.1.2/LWT/scripts/LWT_Fonct.py
--rw-rw-rw-   0        0        0     4247 2024-01-31 14:28:58.000000 lwtools-1.1.2/LWT/scripts/LWT_Merge_csv.py
--rw-rw-rw-   0        0        0    32043 2024-02-02 14:29:28.000000 lwtools-1.1.2/LWT/scripts/LWT_Rebuild_Plus_Export.py
--rw-rw-rw-   0        0        0        0 2023-07-20 12:51:34.000000 lwtools-1.1.2/LWT/scripts/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-25 13:07:50.104018 lwtools-1.1.2/LWTools.egg-info/
--rw-rw-rw-   0        0        0     7900 2024-05-25 13:07:49.000000 lwtools-1.1.2/LWTools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2992 2024-05-25 13:07:49.000000 lwtools-1.1.2/LWTools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-25 13:07:49.000000 lwtools-1.1.2/LWTools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      238 2024-05-25 13:07:49.000000 lwtools-1.1.2/LWTools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-05-25 13:07:49.000000 lwtools-1.1.2/LWTools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       87 2023-07-24 12:37:26.000000 lwtools-1.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     7900 2024-05-25 13:07:50.107275 lwtools-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     6704 2023-11-24 07:55:36.000000 lwtools-1.1.2/README.md
--rw-rw-rw-   0        0        0       86 2024-05-25 13:07:50.107275 lwtools-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0     2420 2024-05-25 13:04:03.000000 lwtools-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-25 13:13:25.553585 lwtools-1.1.3/
+-rw-rw-rw-   0        0        0    35149 2023-07-20 12:51:38.000000 lwtools-1.1.3/LICENSE
+drwxrwxrwx   0        0        0        0 2024-05-25 13:13:25.412147 lwtools-1.1.3/LWT/
+-rw-rw-rw-   0        0        0        0 2023-07-20 12:57:55.000000 lwtools-1.1.3/LWT/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-25 13:13:25.522327 lwtools-1.1.3/LWT/lmtanalysis/
+-rw-rw-rw-   0        0        0    48218 2023-05-03 08:46:45.000000 lwtools-1.1.3/LWT/lmtanalysis/A-OldAnimal-.py
+-rw-rw-rw-   0        0        0    46847 2024-01-19 13:24:49.000000 lwtools-1.1.3/LWT/lmtanalysis/Animal-.py
+-rw-rw-rw-   0        0        0    57484 2024-01-19 13:24:49.000000 lwtools-1.1.3/LWT/lmtanalysis/Animal.py
+-rw-rw-rw-   0        0        0     2057 2022-12-02 08:25:57.000000 lwtools-1.1.3/LWT/lmtanalysis/BehaviouralSequencesUtil.py
+-rw-rw-rw-   0        0        0     2143 2024-01-19 12:46:39.000000 lwtools-1.1.3/LWT/lmtanalysis/BuildDataBaseIndex.py
+-rw-rw-rw-   0        0        0     6013 2024-01-24 08:07:17.000000 lwtools-1.1.3/LWT/lmtanalysis/BuildEventApproachContact.py
+-rw-rw-rw-   0        0        0     3454 2024-01-24 08:15:25.000000 lwtools-1.1.3/LWT/lmtanalysis/BuildEventApproachRear.py
+-rw-rw-rw-   0        0        0     2805 2024-01-24 08:15:25.000000 lwtools-1.1.3/LWT/lmtanalysis/BuildEventCenterPeripheryLocation.py
+-rw-rw-rw-   0        0        0     2402 2023-06-23 14:46:57.000000 lwtools-1.1.3/LWT/lmtanalysis/BuildEventDetection.py
+-rw-rw-rw-   0        0        0        0 2023-06-07 12:33:53.000000 lwtools-1.1.3/LWT/lmtanalysis/BuildEventDistance.py
+-rw-rw-rw-   0        0        0    11287 2024-01-24 08:15:25.000000 lwtools-1.1.3/LWT/lmtanalysis/BuildEventExclusiveCleanOralOralSideSideNoseAnogenitalContact.py
+-rw-rw-rw-   0        0        0     4114 2024-01-24 08:06:29.000000 lwtools-1.1.3/LWT/lmtanalysis/BuildEventExclusiveMoveStopIsolated.py
+-rw-rw-rw-   0        0        0     2260 2024-01-24 08:15:25.000000 lwtools-1.1.3/LWT/lmtanalysis/BuildEventExclusiveUndetected.py
+-rw-rw-rw-   0        0        0     2046 2024-01-24 08:15:25.000000 lwtools-1.1.3/LWT/lmtanalysis/BuildEventFloorSniffing.py
+-rw-rw-rw-   0        0        0     7773 2024-01-19 13:24:50.000000 lwtools-1.1.3/LWT/lmtanalysis/BuildEventFollowZone.py
+-rw-rw-rw-   0        0        0     3391 2024-01-24 08:15:24.000000 lwtools-1.1.3/LWT/lmtanalysis/BuildEventGetAway.py
+-rw-rw-rw-   0        0        0     3192 2024-01-24 08:15:25.000000 lwtools-1.1.3/LWT/lmtanalysis/BuildEventGroup2.py
+-rw-rw-rw-   0        0        0     3648 2024-01-24 08:15:25.000000 lwtools-1.1.3/LWT/lmtanalysis/BuildEventGroup3.py
+-rw-rw-rw-   0        0        0     3583 2024-01-24 08:15:24.000000 lwtools-1.1.3/LWT/lmtanalysis/BuildEventGroup3MakeBreak.py
+-rw-rw-rw-   0        0        0     3496 2024-01-24 08:15:25.000000 lwtools-1.1.3/LWT/lmtanalysis/BuildEventGroup4.py
+-rw-rw-rw-   0        0        0     4149 2024-01-24 08:15:24.000000 lwtools-1.1.3/LWT/lmtanalysis/BuildEventGroup4MakeBreak.py
+-rw-rw-rw-   0        0        0     2072 2024-01-24 08:15:24.000000 lwtools-1.1.3/LWT/lmtanalysis/BuildEventHuddling.py
+-rw-rw-rw-   0        0        0     6413 2024-01-24 08:15:25.000000 lwtools-1.1.3/LWT/lmtanalysis/BuildEventMove.py
+-rw-rw-rw-   0        0        0     6036 2024-01-24 08:15:25.000000 lwtools-1.1.3/LWT/lmtanalysis/BuildEventNest3.py
+-rw-rw-rw-   0        0        0    10885 2024-01-24 08:15:24.000000 lwtools-1.1.3/LWT/lmtanalysis/BuildEventNest4.py
+-rw-rw-rw-   0        0        0     7603 2024-01-19 13:24:49.000000 lwtools-1.1.3/LWT/lmtanalysis/BuildEventNight.py
+-rw-rw-rw-   0        0        0     5695 2024-01-24 08:15:25.000000 lwtools-1.1.3/LWT/lmtanalysis/BuildEventObjectSniffingNor.py
+-rw-rw-rw-   0        0        0     7622 2024-01-24 08:15:24.000000 lwtools-1.1.3/LWT/lmtanalysis/BuildEventObjectSniffingNorAcquisitionWithConfig.py
+-rw-rw-rw-   0        0        0     7709 2024-01-24 08:15:25.000000 lwtools-1.1.3/LWT/lmtanalysis/BuildEventObjectSniffingNorTestWithConfig.py
+-rw-rw-rw-   0        0        0     5455 2024-01-19 13:24:49.000000 lwtools-1.1.3/LWT/lmtanalysis/BuildEventOnHouse.py
+-rw-rw-rw-   0        0        0     2486 2024-01-24 08:15:25.000000 lwtools-1.1.3/LWT/lmtanalysis/BuildEventOralGenitalContact.py
+-rw-rw-rw-   0        0        0     3196 2024-01-24 08:15:25.000000 lwtools-1.1.3/LWT/lmtanalysis/BuildEventOralOralContact.py
+-rw-rw-rw-   0        0        0     5982 2024-01-24 08:15:25.000000 lwtools-1.1.3/LWT/lmtanalysis/BuildEventOralSideSequence.py
+-rw-rw-rw-   0        0        0     3536 2024-01-24 08:15:25.000000 lwtools-1.1.3/LWT/lmtanalysis/BuildEventOtherContact.py
+-rw-rw-rw-   0        0        0     2321 2024-01-24 08:15:25.000000 lwtools-1.1.3/LWT/lmtanalysis/BuildEventPassiveAnogenitalSniff.py
+-rw-rw-rw-   0        0        0     3041 2024-01-24 08:15:24.000000 lwtools-1.1.3/LWT/lmtanalysis/BuildEventRear5.py
+-rw-rw-rw-   0        0        0     2921 2024-01-24 08:15:25.000000 lwtools-1.1.3/LWT/lmtanalysis/BuildEventRearCenterPeriphery.py
+-rw-rw-rw-   0        0        0     1791 2024-01-24 08:15:25.000000 lwtools-1.1.3/LWT/lmtanalysis/BuildEventSAP.py
+-rw-rw-rw-   0        0        0     3480 2024-01-24 08:15:24.000000 lwtools-1.1.3/LWT/lmtanalysis/BuildEventSideBySide.py
+-rw-rw-rw-   0        0        0     3765 2024-01-24 08:15:24.000000 lwtools-1.1.3/LWT/lmtanalysis/BuildEventSideBySideOpposite.py
+-rw-rw-rw-   0        0        0     3998 2024-01-24 08:17:32.000000 lwtools-1.1.3/LWT/lmtanalysis/BuildEventSideWalk.py
+-rw-rw-rw-   0        0        0     3152 2024-01-24 08:15:25.000000 lwtools-1.1.3/LWT/lmtanalysis/BuildEventSocialApproach.py
+-rw-rw-rw-   0        0        0     3003 2024-01-24 08:15:24.000000 lwtools-1.1.3/LWT/lmtanalysis/BuildEventSocialEscape.py
+-rw-rw-rw-   0        0        0     6249 2024-01-24 08:15:25.000000 lwtools-1.1.3/LWT/lmtanalysis/BuildEventStop.py
+-rw-rw-rw-   0        0        0     2730 2024-01-24 08:15:25.000000 lwtools-1.1.3/LWT/lmtanalysis/BuildEventTrain2.py
+-rw-rw-rw-   0        0        0     3880 2024-01-24 08:15:25.000000 lwtools-1.1.3/LWT/lmtanalysis/BuildEventTrain3.py
+-rw-rw-rw-   0        0        0     4425 2024-01-24 08:15:24.000000 lwtools-1.1.3/LWT/lmtanalysis/BuildEventTrain4.py
+-rw-rw-rw-   0        0        0     6496 2024-01-24 08:15:25.000000 lwtools-1.1.3/LWT/lmtanalysis/BuildEventWallJump.py
+-rw-rw-rw-   0        0        0     3373 2024-01-24 08:15:25.000000 lwtools-1.1.3/LWT/lmtanalysis/BuildEventWaterPoint.py
+-rw-rw-rw-   0        0        0     1141 2023-06-23 14:46:57.000000 lwtools-1.1.3/LWT/lmtanalysis/CheckWrongAnimal.py
+-rw-rw-rw-   0        0        0      649 2023-06-23 14:46:57.000000 lwtools-1.1.3/LWT/lmtanalysis/Chronometer.py
+-rw-rw-rw-   0        0        0     5056 2024-01-19 13:24:49.000000 lwtools-1.1.3/LWT/lmtanalysis/CorrectDetectionIntegrity.py
+-rw-rw-rw-   0        0        0     4801 2024-01-19 13:24:49.000000 lwtools-1.1.3/LWT/lmtanalysis/Detection.py
+-rw-rw-rw-   0        0        0    37541 2024-01-25 08:45:16.000000 lwtools-1.1.3/LWT/lmtanalysis/Event.py
+-rw-rw-rw-   0        0        0     1837 2024-01-19 13:24:50.000000 lwtools-1.1.3/LWT/lmtanalysis/EventTimeLineCache.py
+-rw-rw-rw-   0        0        0     4668 2022-12-02 08:25:57.000000 lwtools-1.1.3/LWT/lmtanalysis/Features.py
+-rw-rw-rw-   0        0        0    12958 2024-01-31 13:56:41.000000 lwtools-1.1.3/LWT/lmtanalysis/FileUtil.py
+-rw-rw-rw-   0        0        0     4540 2022-12-02 08:25:57.000000 lwtools-1.1.3/LWT/lmtanalysis/Mask.py
+-rw-rw-rw-   0        0        0     2207 2022-12-02 08:25:57.000000 lwtools-1.1.3/LWT/lmtanalysis/Measure.py
+-rw-rw-rw-   0        0        0      314 2022-12-02 08:25:57.000000 lwtools-1.1.3/LWT/lmtanalysis/Point.py
+-rw-rw-rw-   0        0        0      375 2022-12-02 08:25:57.000000 lwtools-1.1.3/LWT/lmtanalysis/Rectangle.py
+-rw-rw-rw-   0        0        0       91 2022-12-02 08:25:57.000000 lwtools-1.1.3/LWT/lmtanalysis/Settings.py
+-rw-rw-rw-   0        0        0     3135 2024-01-19 13:07:58.000000 lwtools-1.1.3/LWT/lmtanalysis/TaskLogger.py
+-rw-rw-rw-   0        0        0     9478 2024-01-19 13:06:18.000000 lwtools-1.1.3/LWT/lmtanalysis/Util.py
+-rw-rw-rw-   0        0        0       49 2022-12-02 08:25:57.000000 lwtools-1.1.3/LWT/lmtanalysis/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-25 13:13:25.537951 lwtools-1.1.3/LWT/scripts/
+-rw-rw-rw-   0        0        0     9202 2024-02-26 12:46:06.000000 lwtools-1.1.3/LWT/scripts/LMT_Widget_Tool.ipynb
+-rw-rw-rw-   0        0        0     3472 2024-01-25 14:21:35.000000 lwtools-1.1.3/LWT/scripts/LWT_ChangeGenotype.py
+-rw-rw-rw-   0        0        0     9124 2024-02-02 08:34:03.000000 lwtools-1.1.3/LWT/scripts/LWT_DataSplit.py
+-rw-rw-rw-   0        0        0    24428 2024-01-25 08:26:15.000000 lwtools-1.1.3/LWT/scripts/LWT_Export.py
+-rw-rw-rw-   0        0        0   100506 2024-02-12 08:34:52.000000 lwtools-1.1.3/LWT/scripts/LWT_Fonct.py
+-rw-rw-rw-   0        0        0     4247 2024-01-31 14:28:58.000000 lwtools-1.1.3/LWT/scripts/LWT_Merge_csv.py
+-rw-rw-rw-   0        0        0    32043 2024-02-02 14:29:28.000000 lwtools-1.1.3/LWT/scripts/LWT_Rebuild_Plus_Export.py
+-rw-rw-rw-   0        0        0        0 2023-07-20 12:51:34.000000 lwtools-1.1.3/LWT/scripts/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-25 13:13:25.553585 lwtools-1.1.3/LWTools.egg-info/
+-rw-rw-rw-   0        0        0     7900 2024-05-25 13:13:25.000000 lwtools-1.1.3/LWTools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2992 2024-05-25 13:13:25.000000 lwtools-1.1.3/LWTools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 13:13:25.000000 lwtools-1.1.3/LWTools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      238 2024-05-25 13:13:25.000000 lwtools-1.1.3/LWTools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-05-25 13:13:25.000000 lwtools-1.1.3/LWTools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       87 2023-07-24 12:37:26.000000 lwtools-1.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     7900 2024-05-25 13:13:25.553585 lwtools-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     6704 2023-11-24 07:55:36.000000 lwtools-1.1.3/README.md
+-rw-rw-rw-   0        0        0       86 2024-05-25 13:13:25.553585 lwtools-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     2420 2024-05-25 13:11:56.000000 lwtools-1.1.3/setup.py
```

### Comparing `lwtools-1.1.2/LICENSE` & `lwtools-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lwtools-1.1.2/LWT/lmtanalysis/A-OldAnimal-.py` & `lwtools-1.1.3/LWT/lmtanalysis/A-OldAnimal-.py`

 * *Files identical despite different names*

### Comparing `lwtools-1.1.2/LWT/lmtanalysis/Animal-.py` & `lwtools-1.1.3/LWT/lmtanalysis/Animal-.py`

 * *Files identical despite different names*

### Comparing `lwtools-1.1.2/LWT/lmtanalysis/Animal.py` & `lwtools-1.1.3/LWT/lmtanalysis/Animal.py`

 * *Files identical despite different names*

### Comparing `lwtools-1.1.2/LWT/lmtanalysis/BehaviouralSequencesUtil.py` & `lwtools-1.1.3/LWT/lmtanalysis/BehaviouralSequencesUtil.py`

 * *Files identical despite different names*

### Comparing `lwtools-1.1.2/LWT/lmtanalysis/BuildDataBaseIndex.py` & `lwtools-1.1.3/LWT/lmtanalysis/BuildDataBaseIndex.py`

 * *Files identical despite different names*

### Comparing `lwtools-1.1.2/LWT/lmtanalysis/BuildEventApproachContact.py` & `lwtools-1.1.3/LWT/lmtanalysis/BuildEventApproachContact.py`

 * *Files identical despite different names*

### Comparing `lwtools-1.1.2/LWT/lmtanalysis/BuildEventApproachRear.py` & `lwtools-1.1.3/LWT/lmtanalysis/BuildEventApproachRear.py`

 * *Files identical despite different names*

### Comparing `lwtools-1.1.2/LWT/lmtanalysis/BuildEventCenterPeripheryLocation.py` & `lwtools-1.1.3/LWT/lmtanalysis/BuildEventCenterPeripheryLocation.py`

 * *Files identical despite different names*

### Comparing `lwtools-1.1.2/LWT/lmtanalysis/BuildEventDetection.py` & `lwtools-1.1.3/LWT/lmtanalysis/BuildEventDetection.py`

 * *Files identical despite different names*

### Comparing `lwtools-1.1.2/LWT/lmtanalysis/BuildEventExclusiveCleanOralOralSideSideNoseAnogenitalContact.py` & `lwtools-1.1.3/LWT/lmtanalysis/BuildEventExclusiveCleanOralOralSideSideNoseAnogenitalContact.py`

 * *Files identical despite different names*

### Comparing `lwtools-1.1.2/LWT/lmtanalysis/BuildEventExclusiveMoveStopIsolated.py` & `lwtools-1.1.3/LWT/lmtanalysis/BuildEventExclusiveMoveStopIsolated.py`

 * *Files identical despite different names*

### Comparing `lwtools-1.1.2/LWT/lmtanalysis/BuildEventExclusiveUndetected.py` & `lwtools-1.1.3/LWT/lmtanalysis/BuildEventExclusiveUndetected.py`

 * *Files identical despite different names*

### Comparing `lwtools-1.1.2/LWT/lmtanalysis/BuildEventFloorSniffing.py` & `lwtools-1.1.3/LWT/lmtanalysis/BuildEventFloorSniffing.py`

 * *Files identical despite different names*

### Comparing `lwtools-1.1.2/LWT/lmtanalysis/BuildEventFollowZone.py` & `lwtools-1.1.3/LWT/lmtanalysis/BuildEventFollowZone.py`

 * *Files identical despite different names*

### Comparing `lwtools-1.1.2/LWT/lmtanalysis/BuildEventGetAway.py` & `lwtools-1.1.3/LWT/lmtanalysis/BuildEventGetAway.py`

 * *Files identical despite different names*

### Comparing `lwtools-1.1.2/LWT/lmtanalysis/BuildEventGroup2.py` & `lwtools-1.1.3/LWT/lmtanalysis/BuildEventGroup2.py`

 * *Files identical despite different names*

### Comparing `lwtools-1.1.2/LWT/lmtanalysis/BuildEventGroup3.py` & `lwtools-1.1.3/LWT/lmtanalysis/BuildEventGroup3.py`

 * *Files identical despite different names*

### Comparing `lwtools-1.1.2/LWT/lmtanalysis/BuildEventGroup3MakeBreak.py` & `lwtools-1.1.3/LWT/lmtanalysis/BuildEventGroup3MakeBreak.py`

 * *Files identical despite different names*

### Comparing `lwtools-1.1.2/LWT/lmtanalysis/BuildEventGroup4.py` & `lwtools-1.1.3/LWT/lmtanalysis/BuildEventGroup4.py`

 * *Files identical despite different names*

### Comparing `lwtools-1.1.2/LWT/lmtanalysis/BuildEventGroup4MakeBreak.py` & `lwtools-1.1.3/LWT/lmtanalysis/BuildEventGroup4MakeBreak.py`

 * *Files identical despite different names*

### Comparing `lwtools-1.1.2/LWT/lmtanalysis/BuildEventHuddling.py` & `lwtools-1.1.3/LWT/lmtanalysis/BuildEventHuddling.py`

 * *Files identical despite different names*

### Comparing `lwtools-1.1.2/LWT/lmtanalysis/BuildEventMove.py` & `lwtools-1.1.3/LWT/lmtanalysis/BuildEventMove.py`

 * *Files identical despite different names*

### Comparing `lwtools-1.1.2/LWT/lmtanalysis/BuildEventNest3.py` & `lwtools-1.1.3/LWT/lmtanalysis/BuildEventNest3.py`

 * *Files identical despite different names*

### Comparing `lwtools-1.1.2/LWT/lmtanalysis/BuildEventNest4.py` & `lwtools-1.1.3/LWT/lmtanalysis/BuildEventNest4.py`

 * *Files identical despite different names*

### Comparing `lwtools-1.1.2/LWT/lmtanalysis/BuildEventNight.py` & `lwtools-1.1.3/LWT/lmtanalysis/BuildEventNight.py`

 * *Files identical despite different names*

### Comparing `lwtools-1.1.2/LWT/lmtanalysis/BuildEventObjectSniffingNor.py` & `lwtools-1.1.3/LWT/lmtanalysis/BuildEventObjectSniffingNor.py`

 * *Files identical despite different names*

### Comparing `lwtools-1.1.2/LWT/lmtanalysis/BuildEventObjectSniffingNorAcquisitionWithConfig.py` & `lwtools-1.1.3/LWT/lmtanalysis/BuildEventObjectSniffingNorAcquisitionWithConfig.py`

 * *Files identical despite different names*

### Comparing `lwtools-1.1.2/LWT/lmtanalysis/BuildEventObjectSniffingNorTestWithConfig.py` & `lwtools-1.1.3/LWT/lmtanalysis/BuildEventObjectSniffingNorTestWithConfig.py`

 * *Files identical despite different names*

### Comparing `lwtools-1.1.2/LWT/lmtanalysis/BuildEventOnHouse.py` & `lwtools-1.1.3/LWT/lmtanalysis/BuildEventOnHouse.py`

 * *Files identical despite different names*

### Comparing `lwtools-1.1.2/LWT/lmtanalysis/BuildEventOralGenitalContact.py` & `lwtools-1.1.3/LWT/lmtanalysis/BuildEventOralGenitalContact.py`

 * *Files identical despite different names*

### Comparing `lwtools-1.1.2/LWT/lmtanalysis/BuildEventOralOralContact.py` & `lwtools-1.1.3/LWT/lmtanalysis/BuildEventOralOralContact.py`

 * *Files identical despite different names*

### Comparing `lwtools-1.1.2/LWT/lmtanalysis/BuildEventOralSideSequence.py` & `lwtools-1.1.3/LWT/lmtanalysis/BuildEventOralSideSequence.py`

 * *Files identical despite different names*

### Comparing `lwtools-1.1.2/LWT/lmtanalysis/BuildEventOtherContact.py` & `lwtools-1.1.3/LWT/lmtanalysis/BuildEventOtherContact.py`

 * *Files identical despite different names*

### Comparing `lwtools-1.1.2/LWT/lmtanalysis/BuildEventPassiveAnogenitalSniff.py` & `lwtools-1.1.3/LWT/lmtanalysis/BuildEventPassiveAnogenitalSniff.py`

 * *Files identical despite different names*

### Comparing `lwtools-1.1.2/LWT/lmtanalysis/BuildEventRear5.py` & `lwtools-1.1.3/LWT/lmtanalysis/BuildEventRear5.py`

 * *Files identical despite different names*

### Comparing `lwtools-1.1.2/LWT/lmtanalysis/BuildEventRearCenterPeriphery.py` & `lwtools-1.1.3/LWT/lmtanalysis/BuildEventRearCenterPeriphery.py`

 * *Files identical despite different names*

### Comparing `lwtools-1.1.2/LWT/lmtanalysis/BuildEventSAP.py` & `lwtools-1.1.3/LWT/lmtanalysis/BuildEventSAP.py`

 * *Files identical despite different names*

### Comparing `lwtools-1.1.2/LWT/lmtanalysis/BuildEventSideBySide.py` & `lwtools-1.1.3/LWT/lmtanalysis/BuildEventSideBySide.py`

 * *Files identical despite different names*

### Comparing `lwtools-1.1.2/LWT/lmtanalysis/BuildEventSideBySideOpposite.py` & `lwtools-1.1.3/LWT/lmtanalysis/BuildEventSideBySideOpposite.py`

 * *Files identical despite different names*

### Comparing `lwtools-1.1.2/LWT/lmtanalysis/BuildEventSideWalk.py` & `lwtools-1.1.3/LWT/lmtanalysis/BuildEventSideWalk.py`

 * *Files identical despite different names*

### Comparing `lwtools-1.1.2/LWT/lmtanalysis/BuildEventSocialApproach.py` & `lwtools-1.1.3/LWT/lmtanalysis/BuildEventSocialApproach.py`

 * *Files identical despite different names*

### Comparing `lwtools-1.1.2/LWT/lmtanalysis/BuildEventSocialEscape.py` & `lwtools-1.1.3/LWT/lmtanalysis/BuildEventSocialEscape.py`

 * *Files identical despite different names*

### Comparing `lwtools-1.1.2/LWT/lmtanalysis/BuildEventStop.py` & `lwtools-1.1.3/LWT/lmtanalysis/BuildEventStop.py`

 * *Files identical despite different names*

### Comparing `lwtools-1.1.2/LWT/lmtanalysis/BuildEventTrain2.py` & `lwtools-1.1.3/LWT/lmtanalysis/BuildEventTrain2.py`

 * *Files identical despite different names*

### Comparing `lwtools-1.1.2/LWT/lmtanalysis/BuildEventTrain3.py` & `lwtools-1.1.3/LWT/lmtanalysis/BuildEventTrain3.py`

 * *Files identical despite different names*

### Comparing `lwtools-1.1.2/LWT/lmtanalysis/BuildEventTrain4.py` & `lwtools-1.1.3/LWT/lmtanalysis/BuildEventTrain4.py`

 * *Files identical despite different names*

### Comparing `lwtools-1.1.2/LWT/lmtanalysis/BuildEventWallJump.py` & `lwtools-1.1.3/LWT/lmtanalysis/BuildEventWallJump.py`

 * *Files identical despite different names*

### Comparing `lwtools-1.1.2/LWT/lmtanalysis/BuildEventWaterPoint.py` & `lwtools-1.1.3/LWT/lmtanalysis/BuildEventWaterPoint.py`

 * *Files identical despite different names*

### Comparing `lwtools-1.1.2/LWT/lmtanalysis/CheckWrongAnimal.py` & `lwtools-1.1.3/LWT/lmtanalysis/CheckWrongAnimal.py`

 * *Files identical despite different names*

### Comparing `lwtools-1.1.2/LWT/lmtanalysis/Chronometer.py` & `lwtools-1.1.3/LWT/lmtanalysis/Chronometer.py`

 * *Files identical despite different names*

### Comparing `lwtools-1.1.2/LWT/lmtanalysis/CorrectDetectionIntegrity.py` & `lwtools-1.1.3/LWT/lmtanalysis/CorrectDetectionIntegrity.py`

 * *Files identical despite different names*

### Comparing `lwtools-1.1.2/LWT/lmtanalysis/Detection.py` & `lwtools-1.1.3/LWT/lmtanalysis/Detection.py`

 * *Files identical despite different names*

### Comparing `lwtools-1.1.2/LWT/lmtanalysis/Event.py` & `lwtools-1.1.3/LWT/lmtanalysis/Event.py`

 * *Files identical despite different names*

### Comparing `lwtools-1.1.2/LWT/lmtanalysis/EventTimeLineCache.py` & `lwtools-1.1.3/LWT/lmtanalysis/EventTimeLineCache.py`

 * *Files identical despite different names*

### Comparing `lwtools-1.1.2/LWT/lmtanalysis/Features.py` & `lwtools-1.1.3/LWT/lmtanalysis/Features.py`

 * *Files identical despite different names*

### Comparing `lwtools-1.1.2/LWT/lmtanalysis/FileUtil.py` & `lwtools-1.1.3/LWT/lmtanalysis/FileUtil.py`

 * *Files identical despite different names*

### Comparing `lwtools-1.1.2/LWT/lmtanalysis/Mask.py` & `lwtools-1.1.3/LWT/lmtanalysis/Mask.py`

 * *Files identical despite different names*

### Comparing `lwtools-1.1.2/LWT/lmtanalysis/Measure.py` & `lwtools-1.1.3/LWT/lmtanalysis/Measure.py`

 * *Files identical despite different names*

### Comparing `lwtools-1.1.2/LWT/lmtanalysis/TaskLogger.py` & `lwtools-1.1.3/LWT/lmtanalysis/TaskLogger.py`

 * *Files identical despite different names*

### Comparing `lwtools-1.1.2/LWT/lmtanalysis/Util.py` & `lwtools-1.1.3/LWT/lmtanalysis/Util.py`

 * *Files identical despite different names*

### Comparing `lwtools-1.1.2/LWT/scripts/LMT_Widget_Tool.ipynb` & `lwtools-1.1.3/LWT/scripts/LMT_Widget_Tool.ipynb`

 * *Files identical despite different names*

### Comparing `lwtools-1.1.2/LWT/scripts/LWT_ChangeGenotype.py` & `lwtools-1.1.3/LWT/scripts/LWT_ChangeGenotype.py`

 * *Files identical despite different names*

### Comparing `lwtools-1.1.2/LWT/scripts/LWT_DataSplit.py` & `lwtools-1.1.3/LWT/scripts/LWT_DataSplit.py`

 * *Files identical despite different names*

### Comparing `lwtools-1.1.2/LWT/scripts/LWT_Export.py` & `lwtools-1.1.3/LWT/scripts/LWT_Export.py`

 * *Files identical despite different names*

### Comparing `lwtools-1.1.2/LWT/scripts/LWT_Fonct.py` & `lwtools-1.1.3/LWT/scripts/LWT_Fonct.py`

 * *Files identical despite different names*

### Comparing `lwtools-1.1.2/LWT/scripts/LWT_Merge_csv.py` & `lwtools-1.1.3/LWT/scripts/LWT_Merge_csv.py`

 * *Files identical despite different names*

### Comparing `lwtools-1.1.2/LWT/scripts/LWT_Rebuild_Plus_Export.py` & `lwtools-1.1.3/LWT/scripts/LWT_Rebuild_Plus_Export.py`

 * *Files identical despite different names*

### Comparing `lwtools-1.1.2/LWTools.egg-info/PKG-INFO` & `lwtools-1.1.3/LWTools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LWTools
-Version: 1.1.2
+Version: 1.1.3
 Summary: Tool for LMT data analysis
 Home-page: https://github.com/PaulCarrascosa/LMT_Widget_Tool-LWT
 Author: Paul Carrascosa, Damien Huzard
 Author-email: paul.carrascosa@igf.cnrs.fr
 License: GNU General Public License v3 (GPLv3)
 Keywords: Live Mouse Tracker,LMT,Tool,Data analysis
 Classifier: Programming Language :: Python :: 3.10
@@ -23,15 +23,15 @@
 Requires-Dist: seaborn==0.11.2
 Requires-Dist: dabest==2023.2.14
 Requires-Dist: statsmodels==0.13.2
 Requires-Dist: tabulate==0.8.10
 Requires-Dist: ipywidgets==8.0.3
 Requires-Dist: jupyterlab==3.5.0
 Requires-Dist: scipy==1.8.1
-Requires-Dist: numpy==1.23.1
+Requires-Dist: numpy==1.22.3
 
 # LMT Widget Tool (LWT)
 
 The LMT Widget Tool is as tool designed to facilitate the extraction and analysis of behavioral data from .sqlite databases from the Live Mouse Tracker (LMT).
 It helps users with no programming experience to easily visualize, analyze and extract relevant analysis.
 
 You will find more information about LMT on its [website](https://livemousetracker.org/) and [publication](https://www.nature.com/articles/s41551-019-0396-1.epdf?shared_access_token=8wpLBUUytAaGAtXL96vwIdRgN0jAjWel9jnR3ZoTv0MWp3GqbF86Gf14i30j-gtSG2ayVLmU-s57ZbhM2WJjw18inKlRYt31Cg_hLJbPCqlKdjWBImyT1OrH5tewfPqUthmWceoct6RVAL_Vt8H-Og%3D%3D).
```

### Comparing `lwtools-1.1.2/LWTools.egg-info/SOURCES.txt` & `lwtools-1.1.3/LWTools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lwtools-1.1.2/PKG-INFO` & `lwtools-1.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LWTools
-Version: 1.1.2
+Version: 1.1.3
 Summary: Tool for LMT data analysis
 Home-page: https://github.com/PaulCarrascosa/LMT_Widget_Tool-LWT
 Author: Paul Carrascosa, Damien Huzard
 Author-email: paul.carrascosa@igf.cnrs.fr
 License: GNU General Public License v3 (GPLv3)
 Keywords: Live Mouse Tracker,LMT,Tool,Data analysis
 Classifier: Programming Language :: Python :: 3.10
@@ -23,15 +23,15 @@
 Requires-Dist: seaborn==0.11.2
 Requires-Dist: dabest==2023.2.14
 Requires-Dist: statsmodels==0.13.2
 Requires-Dist: tabulate==0.8.10
 Requires-Dist: ipywidgets==8.0.3
 Requires-Dist: jupyterlab==3.5.0
 Requires-Dist: scipy==1.8.1
-Requires-Dist: numpy==1.23.1
+Requires-Dist: numpy==1.22.3
 
 # LMT Widget Tool (LWT)
 
 The LMT Widget Tool is as tool designed to facilitate the extraction and analysis of behavioral data from .sqlite databases from the Live Mouse Tracker (LMT).
 It helps users with no programming experience to easily visualize, analyze and extract relevant analysis.
 
 You will find more information about LMT on its [website](https://livemousetracker.org/) and [publication](https://www.nature.com/articles/s41551-019-0396-1.epdf?shared_access_token=8wpLBUUytAaGAtXL96vwIdRgN0jAjWel9jnR3ZoTv0MWp3GqbF86Gf14i30j-gtSG2ayVLmU-s57ZbhM2WJjw18inKlRYt31Cg_hLJbPCqlKdjWBImyT1OrH5tewfPqUthmWceoct6RVAL_Vt8H-Og%3D%3D).
```

### Comparing `lwtools-1.1.2/README.md` & `lwtools-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `lwtools-1.1.2/setup.py` & `lwtools-1.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 try:
     with open(os.path.join(path,'README.md'),encoding='utf-8') as readme:
         long_description=readme.read()
 except Exception:
     long_description=''
 
 
-setup(name='LWTools',version='1.1.2',author='Paul Carrascosa, Damien Huzard',
+setup(name='LWTools',version='1.1.3',author='Paul Carrascosa, Damien Huzard',
     author_email='paul.carrascosa@igf.cnrs.fr',
     description='Tool for LMT data analysis',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/PaulCarrascosa/LMT_Widget_Tool-LWT',
     packages=find_packages(),
     include_package_data=True,
@@ -57,11 +57,11 @@
     	'seaborn==0.11.2',
     	'dabest==2023.2.14',
     	'statsmodels==0.13.2',
     	'tabulate==0.8.10',
     	'ipywidgets==8.0.3',
     	'jupyterlab==3.5.0',
         'scipy==1.8.1',
-        'numpy==1.23.1',
+        'numpy==1.22.3',
         
     ]   
 )
```

