# Comparing `tmp/jdmtool-0.0.4.tar.gz` & `tmp/jdmtool-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/dima/src/jdmtool/dist/.tmp-6qbvcsxc/jdmtool-0.0.4.tar", last modified: Sat Apr 13 00:32:55 2024, max compression
+gzip compressed data, was "/home/dima/src/jdmtool/dist/.tmp-e1pcazxp/jdmtool-0.1.tar", last modified: Sat May 25 08:27:55 2024, max compression
```

## Comparing `jdmtool-0.0.4.tar` & `jdmtool-0.1.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2024-04-13 00:32:55.000000 jdmtool-0.0.4/
--rw-r--r--   0 dima      (1000) dima      (1000)    11357 2023-03-28 17:09:03.000000 jdmtool-0.0.4/LICENSE
--rw-r--r--   0 dima      (1000) dima      (1000)     6975 2024-04-13 00:32:55.000000 jdmtool-0.0.4/PKG-INFO
--rw-r--r--   0 dima      (1000) dima      (1000)     6415 2023-04-14 02:01:35.000000 jdmtool-0.0.4/README.md
--rw-r--r--   0 dima      (1000) dima      (1000)      825 2024-04-13 00:31:22.000000 jdmtool-0.0.4/pyproject.toml
--rw-r--r--   0 dima      (1000) dima      (1000)       38 2024-04-13 00:32:55.000000 jdmtool-0.0.4/setup.cfg
-drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2024-04-13 00:32:55.000000 jdmtool-0.0.4/src/
-drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2024-04-13 00:32:55.000000 jdmtool-0.0.4/src/jdmtool/
--rw-r--r--   0 dima      (1000) dima      (1000)        0 2023-03-28 16:55:30.000000 jdmtool-0.0.4/src/jdmtool/__init__.py
--rw-r--r--   0 dima      (1000) dima      (1000)     2780 2024-04-13 00:27:00.000000 jdmtool-0.0.4/src/jdmtool/chartview.py
--rw-r--r--   0 dima      (1000) dima      (1000)     3700 2023-04-12 13:42:28.000000 jdmtool-0.0.4/src/jdmtool/device.py
--rw-r--r--   0 dima      (1000) dima      (1000)     8477 2024-04-13 00:29:55.000000 jdmtool-0.0.4/src/jdmtool/downloader.py
--rw-r--r--   0 dima      (1000) dima      (1000)    15242 2024-04-13 00:27:00.000000 jdmtool-0.0.4/src/jdmtool/main.py
-drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2024-04-13 00:32:55.000000 jdmtool-0.0.4/src/jdmtool.egg-info/
--rw-r--r--   0 dima      (1000) dima      (1000)     6975 2024-04-13 00:32:55.000000 jdmtool-0.0.4/src/jdmtool.egg-info/PKG-INFO
--rw-r--r--   0 dima      (1000) dima      (1000)      361 2024-04-13 00:32:55.000000 jdmtool-0.0.4/src/jdmtool.egg-info/SOURCES.txt
--rw-r--r--   0 dima      (1000) dima      (1000)        1 2024-04-13 00:32:55.000000 jdmtool-0.0.4/src/jdmtool.egg-info/dependency_links.txt
--rw-r--r--   0 dima      (1000) dima      (1000)       81 2024-04-13 00:32:55.000000 jdmtool-0.0.4/src/jdmtool.egg-info/entry_points.txt
--rw-r--r--   0 dima      (1000) dima      (1000)       64 2024-04-13 00:32:55.000000 jdmtool-0.0.4/src/jdmtool.egg-info/requires.txt
--rw-r--r--   0 dima      (1000) dima      (1000)        8 2024-04-13 00:32:55.000000 jdmtool-0.0.4/src/jdmtool.egg-info/top_level.txt
+drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2024-05-25 08:27:55.000000 jdmtool-0.1/
+-rw-r--r--   0 dima      (1000) dima      (1000)    11357 2023-03-28 17:09:03.000000 jdmtool-0.1/LICENSE
+-rw-r--r--   0 dima      (1000) dima      (1000)     8192 2024-05-25 08:27:55.000000 jdmtool-0.1/PKG-INFO
+-rw-r--r--   0 dima      (1000) dima      (1000)     7660 2024-05-25 08:17:35.000000 jdmtool-0.1/README.md
+-rw-r--r--   0 dima      (1000) dima      (1000)      982 2024-05-25 08:25:24.000000 jdmtool-0.1/pyproject.toml
+-rw-r--r--   0 dima      (1000) dima      (1000)       38 2024-05-25 08:27:55.000000 jdmtool-0.1/setup.cfg
+drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2024-05-25 08:27:55.000000 jdmtool-0.1/src/
+drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2024-05-25 08:27:55.000000 jdmtool-0.1/src/jdmtool/
+-rw-r--r--   0 dima      (1000) dima      (1000)        0 2023-03-28 16:55:30.000000 jdmtool-0.1/src/jdmtool/__init__.py
+-rw-r--r--   0 dima      (1000) dima      (1000)    14766 2024-05-25 04:48:59.000000 jdmtool-0.1/src/jdmtool/avidyne.py
+-rw-r--r--   0 dima      (1000) dima      (1000)     2780 2024-05-23 05:36:46.000000 jdmtool-0.1/src/jdmtool/chartview.py
+-rw-r--r--   0 dima      (1000) dima      (1000)     6421 2024-05-24 07:43:11.000000 jdmtool-0.1/src/jdmtool/downloader.py
+-rw-r--r--   0 dima      (1000) dima      (1000)    25689 2024-05-25 06:50:25.000000 jdmtool-0.1/src/jdmtool/main.py
+-rw-r--r--   0 dima      (1000) dima      (1000)     6670 2024-05-23 05:28:45.000000 jdmtool-0.1/src/jdmtool/service.py
+-rw-r--r--   0 dima      (1000) dima      (1000)     4498 2024-05-25 06:36:45.000000 jdmtool-0.1/src/jdmtool/skybound.py
+drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2024-05-25 08:27:55.000000 jdmtool-0.1/src/jdmtool.egg-info/
+-rw-r--r--   0 dima      (1000) dima      (1000)     8192 2024-05-25 08:27:55.000000 jdmtool-0.1/src/jdmtool.egg-info/PKG-INFO
+-rw-r--r--   0 dima      (1000) dima      (1000)      409 2024-05-25 08:27:55.000000 jdmtool-0.1/src/jdmtool.egg-info/SOURCES.txt
+-rw-r--r--   0 dima      (1000) dima      (1000)        1 2024-05-25 08:27:55.000000 jdmtool-0.1/src/jdmtool.egg-info/dependency_links.txt
+-rw-r--r--   0 dima      (1000) dima      (1000)       81 2024-05-25 08:27:55.000000 jdmtool-0.1/src/jdmtool.egg-info/entry_points.txt
+-rw-r--r--   0 dima      (1000) dima      (1000)      223 2024-05-25 08:27:55.000000 jdmtool-0.1/src/jdmtool.egg-info/requires.txt
+-rw-r--r--   0 dima      (1000) dima      (1000)        8 2024-05-25 08:27:55.000000 jdmtool-0.1/src/jdmtool.egg-info/top_level.txt
```

### Comparing `jdmtool-0.0.4/LICENSE` & `jdmtool-0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jdmtool-0.0.4/PKG-INFO` & `jdmtool-0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 Metadata-Version: 2.1
 Name: jdmtool
-Version: 0.0.4
-Summary: Tool for downloading Jeppesen databases and programming Garmin aviation data cards
+Version: 0.1
+Summary: Tool for downloading and transferring Jeppesen databases
 Author-email: Dima Ryazanov <dima@gmail.com>
 Project-URL: Homepage, https://github.com/dimaryaz/jdmtool
 Project-URL: Bug Tracker, https://github.com/dimaryaz/jdmtool/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # JdmTool
 
-A command-line tool for downloading Jeppesen databases and programming Garmin aviation data cards aiming to be compatible with [Jeppesen Distribution Manager](https://ww2.jeppesen.com/data-solutions/jeppesen-distribution-manager/).
+A command-line tool for downloading and transferring Jeppesen databases aiming to be compatible with [Jeppesen Distribution Manager](https://ww2.jeppesen.com/data-solutions/jeppesen-distribution-manager/).
 
-It requires:
-- Jeppesen subscription
-- A GNS 430/530 data card programmer (USB ID `0e39:1250`)
-- A 16MB data card
+It requires a Jeppesen subscription, and currenty supports the following services:
+- NavData for Garmin GNS 400/500 Series
+  - Requires a Skybound data card programmer (USB ID `0e39:1250`)
+  - Requires a 16MB NavData WAAS card or a 4MB NavData non-WAAS card
+    - If you have an 8MB data card, please [file a bug](https://github.com/dimaryaz/jdmtool/issues/)!
+- NavData and Obstacles for Avidyne IFD 400 Series
 
-Currently, it has only been tested on Linux with GNS 430 and a Jeppesen NavData database.
+It is mainly tested on Linux, but should work on OS X and Windows.
 
 ## Installing
 
 You may want to create a Python virtual environment using e.g. [virtualenvwrapper](https://pypi.org/project/virtualenvwrapper/).
 
 Install the latest `jdmtool` release:
 
@@ -35,43 +37,47 @@
 
 Or install the latest code from GitHub:
 
 ```
 pip3 install "git+https://github.com/dimaryaz/jdmtool.git#egg=jdmtool"
 ```
 
-Make sure you have access to the USB device. On Linux, you should copy `udev/50-garmin.rules` to `/etc/udev/rules.d/`.
+To program Garmin data cards, make sure you have access to the USB device. On Linux, you should copy `udev/50-garmin.rules` to `/etc/udev/rules.d/` and possibly reload the rules.
 
 ## Basic Usage
 
 ### Log in
 
+You only need to run this once (unless you change your password).
+
 ```
 $ jdmtool login
 Username: test@example.com
 Password: 
 Logged in successfully
 ```
 
 ### Refresh the list of available downloads
 
+Run this every time you want to download updates.
+
 ```
 $ jdmtool refresh
 Downloading services...
 Downloading keychain...
 Success
 ```
 
 ### View available downloads
 
 ```
 $ jdmtool list
 ID  Name                                                                    Coverage              Version   Start Date  End Date    Downloaded
- 0  Garmin GNS 400/500 Series WAAS - NavData                                Americas              2303      2023-03-23  2023-04-20  Y         
- 1  Garmin GNS 400/500 Series WAAS - NavData                                Americas              2304      2023-04-20  2023-05-18  Y         
+ 0  Garmin GNS 400/500 Series WAAS - NavData                                Americas              2303      2023-03-23  2023-04-20            
+ 1  Garmin GNS 400/500 Series WAAS - NavData                                Americas              2304      2023-04-20  2023-05-18            
 ```
 
 ### View detailed info
 
 ```
 $ jdmtool info 0
 Aircraft Manufacturer:        LOCKHEED
@@ -107,28 +113,42 @@
 
 ```
 $ jdmtool download 0
 Downloading: 100%|█████████████████████████████████████████████████| 8.44M/8.44M [00:03<00:00, 2.15MB/s]
 Downloaded to /home/user/.local/share/jdmtool/downloads/dgrw72_2303_eceb0273.bin
 ```
 
-### Transfer the database to the data card
+### Transfer the database to the data card (GNS 400/500)
 
 ```
 $ jdmtool transfer 0
 Found device: Bus 001 Device 052: ID 0e39:1250
+Detected data card: 16MB WAAS
 Transfer /home/user/.local/share/jdmtool/downloads/dgrw72_2303_eceb0273.bin to the data card? (y/n) y
 Erasing the database: 100%|████████████████████████████████████████| 8.59M/8.59M [02:15<00:00, 63.1KB/s]
 Writing the database: 100%|████████████████████████████████████████| 8.59M/8.59M [04:14<00:00, 40.5KB/s]
 Verifying the database: 100%|██████████████████████████████████████| 8.59M/8.59M [01:32<00:00, 92.5KB/s]
 Writing new metadata: {2303~12345678}
 Done
 ```
 
-## Advanced Features
+### Transfer the database to the USB drive (Avidyne IFD 440)
+
+Note: the final database file will contain the FAT32 volume ID of the USB drive - which means, it requires an actual FAT32-formatted device, not any random directory.
+
+```
+$ jdmtool transfer 0 /run/media/user/USB/
+Transfer databases to /run/media/user/USB/? (y/n) y
+Found volume ID: 1234abcd
+Writing to /run/media/user/USB/navdata.dsf: 100%|██████████████████| 38.0M/38.0M [00:15<00:00, 2.49MB/s]
+Updating .jdm...
+Done
+```
+
+## Advanced Features (GNS 400/500)
 
 ### Check that the tool can detect the device and the data card:
 
 ```
 $ jdmtool detect
 Found device: Bus 001 Device 049: ID 0e39:1250
 Firmware version: 20071203
@@ -139,58 +159,64 @@
 
 ("Unknown identifier" likely contains the information about what type of card this is, but
 I don't have enough information to decode it.)
 
 
 ### Read the metadata (should contain the cycle and the service ID):
 
+JDM seems to only write it to 16MB cards. Not clear if it's actually used for anything.
+
 ```
 $ jdmtool read-metadata
 Found device: Bus 001 Device 045: ID 0e39:1250
+Detected data card: 16MB WAAS
 Database metadata: {2303~12345678}
 ```
 
 ### Write the metadata (should probably keep the same format):
 
+JDM seems to only write it to 16MB cards. Not clear if it's actually used for anything.
+
 ```
 $ jdmtool write-metadata '{2303~12345678}'
 Found device: Bus 001 Device 045: ID 0e39:1250
+Detected data card: 16MB WAAS
 Done
 ```
 
 ### Read the current database from the data card:
 
 ```
 $ jdmtool read-database db.bin
 Found device: Bus 001 Device 044: ID 0e39:1250
+Detected data card: 16MB WAAS
 Reading the database: 100%|████████████████████████████████████████| 8.59M/8.59M [01:33<00:00, 91.6KB/s]
 Truncating the file...
 Done
 ```
 
 You should now have the database in `db.bin`:
 
 ```
 $ file db.bin
 db.bin: DOS/MBR boot sector, code offset 0x3c+2, OEM-ID "GARMIN10", sectors/cluster 8, FAT  1, root entries 512, sectors 32768 (volumes <=32 MB), sectors/FAT 16, sectors/track 63, heads 255, hidden sectors 63, serial number 0x1102, label: "GARMIN AT  ", FAT (16 bit)
 ```
 
-### Write a new database to the data card:
+It may not match the original downloaded file exactly. There is no way to know the size of the database on the data card, so either `db.bin` or the original file will likely contain extra `\xFF` bytes at the end.
 
-This will do some sanity checks to make sure the file is in fact a Garmin database. If it rejects your file, please file a bug to let me know.
+### Write a new database to the data card:
 
 ```
 $ jdmtool write-database dgrw72_2303_eceb0273.bin
 Found device: Bus 001 Device 045: ID 0e39:1250
+Detected data card: 16MB WAAS
 Transfer dgrw72_2303_eceb0273.bin to the data card? (y/n) y
 Erasing the database: 100%|████████████████████████████████████████| 8.59M/8.59M [02:15<00:00, 63.1KB/s]
 Writing the database: 100%|████████████████████████████████████████| 8.59M/8.59M [04:14<00:00, 40.5KB/s]
 Verifying the database: 100%|██████████████████████████████████████| 8.59M/8.59M [01:32<00:00, 92.5KB/s]
 Done
 ```
 
-After it is done, you may want to run `jdmtool write-metadata '{...-...}'` to save the new cycle number in the metadata.
-
 
 ## Bugs
 
-This has only been tested with a single card reader and two cards, so chances are, it won't work correctly for others. Please file a bug if you run into problems.
+Please [file a bug](https://github.com/dimaryaz/jdmtool/issues/) if you run into problems, or if you have a device/service that is not currently supported.
```

### Comparing `jdmtool-0.0.4/README.md` & `jdmtool-0.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # JdmTool
 
-A command-line tool for downloading Jeppesen databases and programming Garmin aviation data cards aiming to be compatible with [Jeppesen Distribution Manager](https://ww2.jeppesen.com/data-solutions/jeppesen-distribution-manager/).
+A command-line tool for downloading and transferring Jeppesen databases aiming to be compatible with [Jeppesen Distribution Manager](https://ww2.jeppesen.com/data-solutions/jeppesen-distribution-manager/).
 
-It requires:
-- Jeppesen subscription
-- A GNS 430/530 data card programmer (USB ID `0e39:1250`)
-- A 16MB data card
+It requires a Jeppesen subscription, and currenty supports the following services:
+- NavData for Garmin GNS 400/500 Series
+  - Requires a Skybound data card programmer (USB ID `0e39:1250`)
+  - Requires a 16MB NavData WAAS card or a 4MB NavData non-WAAS card
+    - If you have an 8MB data card, please [file a bug](https://github.com/dimaryaz/jdmtool/issues/)!
+- NavData and Obstacles for Avidyne IFD 400 Series
 
-Currently, it has only been tested on Linux with GNS 430 and a Jeppesen NavData database.
+It is mainly tested on Linux, but should work on OS X and Windows.
 
 ## Installing
 
 You may want to create a Python virtual environment using e.g. [virtualenvwrapper](https://pypi.org/project/virtualenvwrapper/).
 
 Install the latest `jdmtool` release:
 
@@ -21,43 +23,47 @@
 
 Or install the latest code from GitHub:
 
 ```
 pip3 install "git+https://github.com/dimaryaz/jdmtool.git#egg=jdmtool"
 ```
 
-Make sure you have access to the USB device. On Linux, you should copy `udev/50-garmin.rules` to `/etc/udev/rules.d/`.
+To program Garmin data cards, make sure you have access to the USB device. On Linux, you should copy `udev/50-garmin.rules` to `/etc/udev/rules.d/` and possibly reload the rules.
 
 ## Basic Usage
 
 ### Log in
 
+You only need to run this once (unless you change your password).
+
 ```
 $ jdmtool login
 Username: test@example.com
 Password: 
 Logged in successfully
 ```
 
 ### Refresh the list of available downloads
 
+Run this every time you want to download updates.
+
 ```
 $ jdmtool refresh
 Downloading services...
 Downloading keychain...
 Success
 ```
 
 ### View available downloads
 
 ```
 $ jdmtool list
 ID  Name                                                                    Coverage              Version   Start Date  End Date    Downloaded
- 0  Garmin GNS 400/500 Series WAAS - NavData                                Americas              2303      2023-03-23  2023-04-20  Y         
- 1  Garmin GNS 400/500 Series WAAS - NavData                                Americas              2304      2023-04-20  2023-05-18  Y         
+ 0  Garmin GNS 400/500 Series WAAS - NavData                                Americas              2303      2023-03-23  2023-04-20            
+ 1  Garmin GNS 400/500 Series WAAS - NavData                                Americas              2304      2023-04-20  2023-05-18            
 ```
 
 ### View detailed info
 
 ```
 $ jdmtool info 0
 Aircraft Manufacturer:        LOCKHEED
@@ -93,28 +99,42 @@
 
 ```
 $ jdmtool download 0
 Downloading: 100%|█████████████████████████████████████████████████| 8.44M/8.44M [00:03<00:00, 2.15MB/s]
 Downloaded to /home/user/.local/share/jdmtool/downloads/dgrw72_2303_eceb0273.bin
 ```
 
-### Transfer the database to the data card
+### Transfer the database to the data card (GNS 400/500)
 
 ```
 $ jdmtool transfer 0
 Found device: Bus 001 Device 052: ID 0e39:1250
+Detected data card: 16MB WAAS
 Transfer /home/user/.local/share/jdmtool/downloads/dgrw72_2303_eceb0273.bin to the data card? (y/n) y
 Erasing the database: 100%|████████████████████████████████████████| 8.59M/8.59M [02:15<00:00, 63.1KB/s]
 Writing the database: 100%|████████████████████████████████████████| 8.59M/8.59M [04:14<00:00, 40.5KB/s]
 Verifying the database: 100%|██████████████████████████████████████| 8.59M/8.59M [01:32<00:00, 92.5KB/s]
 Writing new metadata: {2303~12345678}
 Done
 ```
 
-## Advanced Features
+### Transfer the database to the USB drive (Avidyne IFD 440)
+
+Note: the final database file will contain the FAT32 volume ID of the USB drive - which means, it requires an actual FAT32-formatted device, not any random directory.
+
+```
+$ jdmtool transfer 0 /run/media/user/USB/
+Transfer databases to /run/media/user/USB/? (y/n) y
+Found volume ID: 1234abcd
+Writing to /run/media/user/USB/navdata.dsf: 100%|██████████████████| 38.0M/38.0M [00:15<00:00, 2.49MB/s]
+Updating .jdm...
+Done
+```
+
+## Advanced Features (GNS 400/500)
 
 ### Check that the tool can detect the device and the data card:
 
 ```
 $ jdmtool detect
 Found device: Bus 001 Device 049: ID 0e39:1250
 Firmware version: 20071203
@@ -125,58 +145,64 @@
 
 ("Unknown identifier" likely contains the information about what type of card this is, but
 I don't have enough information to decode it.)
 
 
 ### Read the metadata (should contain the cycle and the service ID):
 
+JDM seems to only write it to 16MB cards. Not clear if it's actually used for anything.
+
 ```
 $ jdmtool read-metadata
 Found device: Bus 001 Device 045: ID 0e39:1250
+Detected data card: 16MB WAAS
 Database metadata: {2303~12345678}
 ```
 
 ### Write the metadata (should probably keep the same format):
 
+JDM seems to only write it to 16MB cards. Not clear if it's actually used for anything.
+
 ```
 $ jdmtool write-metadata '{2303~12345678}'
 Found device: Bus 001 Device 045: ID 0e39:1250
+Detected data card: 16MB WAAS
 Done
 ```
 
 ### Read the current database from the data card:
 
 ```
 $ jdmtool read-database db.bin
 Found device: Bus 001 Device 044: ID 0e39:1250
+Detected data card: 16MB WAAS
 Reading the database: 100%|████████████████████████████████████████| 8.59M/8.59M [01:33<00:00, 91.6KB/s]
 Truncating the file...
 Done
 ```
 
 You should now have the database in `db.bin`:
 
 ```
 $ file db.bin
 db.bin: DOS/MBR boot sector, code offset 0x3c+2, OEM-ID "GARMIN10", sectors/cluster 8, FAT  1, root entries 512, sectors 32768 (volumes <=32 MB), sectors/FAT 16, sectors/track 63, heads 255, hidden sectors 63, serial number 0x1102, label: "GARMIN AT  ", FAT (16 bit)
 ```
 
-### Write a new database to the data card:
+It may not match the original downloaded file exactly. There is no way to know the size of the database on the data card, so either `db.bin` or the original file will likely contain extra `\xFF` bytes at the end.
 
-This will do some sanity checks to make sure the file is in fact a Garmin database. If it rejects your file, please file a bug to let me know.
+### Write a new database to the data card:
 
 ```
 $ jdmtool write-database dgrw72_2303_eceb0273.bin
 Found device: Bus 001 Device 045: ID 0e39:1250
+Detected data card: 16MB WAAS
 Transfer dgrw72_2303_eceb0273.bin to the data card? (y/n) y
 Erasing the database: 100%|████████████████████████████████████████| 8.59M/8.59M [02:15<00:00, 63.1KB/s]
 Writing the database: 100%|████████████████████████████████████████| 8.59M/8.59M [04:14<00:00, 40.5KB/s]
 Verifying the database: 100%|██████████████████████████████████████| 8.59M/8.59M [01:32<00:00, 92.5KB/s]
 Done
 ```
 
-After it is done, you may want to run `jdmtool write-metadata '{...-...}'` to save the new cycle number in the metadata.
-
 
 ## Bugs
 
-This has only been tested with a single card reader and two cards, so chances are, it won't work correctly for others. Please file a bug if you run into problems.
+Please [file a bug](https://github.com/dimaryaz/jdmtool/issues/) if you run into problems, or if you have a device/service that is not currently supported.
```

### Comparing `jdmtool-0.0.4/pyproject.toml` & `jdmtool-0.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jdmtool"
-version = "0.0.4"
+version = "0.1"
 authors = [
   { name="Dima Ryazanov", email="dima@gmail.com" },
 ]
-description = "Tool for downloading Jeppesen databases and programming Garmin aviation data cards"
+description = "Tool for downloading and transferring Jeppesen databases"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     'libusb1>=2.0.1',
+    'libscrc>=1.8.0',
     'platformdirs>=2.6.2',
+    'psutil>=5.9.4',
+    'pyudev>=0.24.3; sys_platform == "linux"',
+    'pywin32>=306; sys_platform == "win32"',
     'requests>=2.26.0',
     'tqdm>=4.1.0',
+    'typing_extensions; python_version < "3.11"',
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/dimaryaz/jdmtool"
 "Bug Tracker" = "https://github.com/dimaryaz/jdmtool/issues"
 
 [project.scripts]
```

### Comparing `jdmtool-0.0.4/src/jdmtool/chartview.py` & `jdmtool-0.1/src/jdmtool/chartview.py`

 * *Files identical despite different names*

### Comparing `jdmtool-0.0.4/src/jdmtool.egg-info/PKG-INFO` & `jdmtool-0.1/src/jdmtool.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 Metadata-Version: 2.1
 Name: jdmtool
-Version: 0.0.4
-Summary: Tool for downloading Jeppesen databases and programming Garmin aviation data cards
+Version: 0.1
+Summary: Tool for downloading and transferring Jeppesen databases
 Author-email: Dima Ryazanov <dima@gmail.com>
 Project-URL: Homepage, https://github.com/dimaryaz/jdmtool
 Project-URL: Bug Tracker, https://github.com/dimaryaz/jdmtool/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # JdmTool
 
-A command-line tool for downloading Jeppesen databases and programming Garmin aviation data cards aiming to be compatible with [Jeppesen Distribution Manager](https://ww2.jeppesen.com/data-solutions/jeppesen-distribution-manager/).
+A command-line tool for downloading and transferring Jeppesen databases aiming to be compatible with [Jeppesen Distribution Manager](https://ww2.jeppesen.com/data-solutions/jeppesen-distribution-manager/).
 
-It requires:
-- Jeppesen subscription
-- A GNS 430/530 data card programmer (USB ID `0e39:1250`)
-- A 16MB data card
+It requires a Jeppesen subscription, and currenty supports the following services:
+- NavData for Garmin GNS 400/500 Series
+  - Requires a Skybound data card programmer (USB ID `0e39:1250`)
+  - Requires a 16MB NavData WAAS card or a 4MB NavData non-WAAS card
+    - If you have an 8MB data card, please [file a bug](https://github.com/dimaryaz/jdmtool/issues/)!
+- NavData and Obstacles for Avidyne IFD 400 Series
 
-Currently, it has only been tested on Linux with GNS 430 and a Jeppesen NavData database.
+It is mainly tested on Linux, but should work on OS X and Windows.
 
 ## Installing
 
 You may want to create a Python virtual environment using e.g. [virtualenvwrapper](https://pypi.org/project/virtualenvwrapper/).
 
 Install the latest `jdmtool` release:
 
@@ -35,43 +37,47 @@
 
 Or install the latest code from GitHub:
 
 ```
 pip3 install "git+https://github.com/dimaryaz/jdmtool.git#egg=jdmtool"
 ```
 
-Make sure you have access to the USB device. On Linux, you should copy `udev/50-garmin.rules` to `/etc/udev/rules.d/`.
+To program Garmin data cards, make sure you have access to the USB device. On Linux, you should copy `udev/50-garmin.rules` to `/etc/udev/rules.d/` and possibly reload the rules.
 
 ## Basic Usage
 
 ### Log in
 
+You only need to run this once (unless you change your password).
+
 ```
 $ jdmtool login
 Username: test@example.com
 Password: 
 Logged in successfully
 ```
 
 ### Refresh the list of available downloads
 
+Run this every time you want to download updates.
+
 ```
 $ jdmtool refresh
 Downloading services...
 Downloading keychain...
 Success
 ```
 
 ### View available downloads
 
 ```
 $ jdmtool list
 ID  Name                                                                    Coverage              Version   Start Date  End Date    Downloaded
- 0  Garmin GNS 400/500 Series WAAS - NavData                                Americas              2303      2023-03-23  2023-04-20  Y         
- 1  Garmin GNS 400/500 Series WAAS - NavData                                Americas              2304      2023-04-20  2023-05-18  Y         
+ 0  Garmin GNS 400/500 Series WAAS - NavData                                Americas              2303      2023-03-23  2023-04-20            
+ 1  Garmin GNS 400/500 Series WAAS - NavData                                Americas              2304      2023-04-20  2023-05-18            
 ```
 
 ### View detailed info
 
 ```
 $ jdmtool info 0
 Aircraft Manufacturer:        LOCKHEED
@@ -107,28 +113,42 @@
 
 ```
 $ jdmtool download 0
 Downloading: 100%|█████████████████████████████████████████████████| 8.44M/8.44M [00:03<00:00, 2.15MB/s]
 Downloaded to /home/user/.local/share/jdmtool/downloads/dgrw72_2303_eceb0273.bin
 ```
 
-### Transfer the database to the data card
+### Transfer the database to the data card (GNS 400/500)
 
 ```
 $ jdmtool transfer 0
 Found device: Bus 001 Device 052: ID 0e39:1250
+Detected data card: 16MB WAAS
 Transfer /home/user/.local/share/jdmtool/downloads/dgrw72_2303_eceb0273.bin to the data card? (y/n) y
 Erasing the database: 100%|████████████████████████████████████████| 8.59M/8.59M [02:15<00:00, 63.1KB/s]
 Writing the database: 100%|████████████████████████████████████████| 8.59M/8.59M [04:14<00:00, 40.5KB/s]
 Verifying the database: 100%|██████████████████████████████████████| 8.59M/8.59M [01:32<00:00, 92.5KB/s]
 Writing new metadata: {2303~12345678}
 Done
 ```
 
-## Advanced Features
+### Transfer the database to the USB drive (Avidyne IFD 440)
+
+Note: the final database file will contain the FAT32 volume ID of the USB drive - which means, it requires an actual FAT32-formatted device, not any random directory.
+
+```
+$ jdmtool transfer 0 /run/media/user/USB/
+Transfer databases to /run/media/user/USB/? (y/n) y
+Found volume ID: 1234abcd
+Writing to /run/media/user/USB/navdata.dsf: 100%|██████████████████| 38.0M/38.0M [00:15<00:00, 2.49MB/s]
+Updating .jdm...
+Done
+```
+
+## Advanced Features (GNS 400/500)
 
 ### Check that the tool can detect the device and the data card:
 
 ```
 $ jdmtool detect
 Found device: Bus 001 Device 049: ID 0e39:1250
 Firmware version: 20071203
@@ -139,58 +159,64 @@
 
 ("Unknown identifier" likely contains the information about what type of card this is, but
 I don't have enough information to decode it.)
 
 
 ### Read the metadata (should contain the cycle and the service ID):
 
+JDM seems to only write it to 16MB cards. Not clear if it's actually used for anything.
+
 ```
 $ jdmtool read-metadata
 Found device: Bus 001 Device 045: ID 0e39:1250
+Detected data card: 16MB WAAS
 Database metadata: {2303~12345678}
 ```
 
 ### Write the metadata (should probably keep the same format):
 
+JDM seems to only write it to 16MB cards. Not clear if it's actually used for anything.
+
 ```
 $ jdmtool write-metadata '{2303~12345678}'
 Found device: Bus 001 Device 045: ID 0e39:1250
+Detected data card: 16MB WAAS
 Done
 ```
 
 ### Read the current database from the data card:
 
 ```
 $ jdmtool read-database db.bin
 Found device: Bus 001 Device 044: ID 0e39:1250
+Detected data card: 16MB WAAS
 Reading the database: 100%|████████████████████████████████████████| 8.59M/8.59M [01:33<00:00, 91.6KB/s]
 Truncating the file...
 Done
 ```
 
 You should now have the database in `db.bin`:
 
 ```
 $ file db.bin
 db.bin: DOS/MBR boot sector, code offset 0x3c+2, OEM-ID "GARMIN10", sectors/cluster 8, FAT  1, root entries 512, sectors 32768 (volumes <=32 MB), sectors/FAT 16, sectors/track 63, heads 255, hidden sectors 63, serial number 0x1102, label: "GARMIN AT  ", FAT (16 bit)
 ```
 
-### Write a new database to the data card:
+It may not match the original downloaded file exactly. There is no way to know the size of the database on the data card, so either `db.bin` or the original file will likely contain extra `\xFF` bytes at the end.
 
-This will do some sanity checks to make sure the file is in fact a Garmin database. If it rejects your file, please file a bug to let me know.
+### Write a new database to the data card:
 
 ```
 $ jdmtool write-database dgrw72_2303_eceb0273.bin
 Found device: Bus 001 Device 045: ID 0e39:1250
+Detected data card: 16MB WAAS
 Transfer dgrw72_2303_eceb0273.bin to the data card? (y/n) y
 Erasing the database: 100%|████████████████████████████████████████| 8.59M/8.59M [02:15<00:00, 63.1KB/s]
 Writing the database: 100%|████████████████████████████████████████| 8.59M/8.59M [04:14<00:00, 40.5KB/s]
 Verifying the database: 100%|██████████████████████████████████████| 8.59M/8.59M [01:32<00:00, 92.5KB/s]
 Done
 ```
 
-After it is done, you may want to run `jdmtool write-metadata '{...-...}'` to save the new cycle number in the metadata.
-
 
 ## Bugs
 
-This has only been tested with a single card reader and two cards, so chances are, it won't work correctly for others. Please file a bug if you run into problems.
+Please [file a bug](https://github.com/dimaryaz/jdmtool/issues/) if you run into problems, or if you have a device/service that is not currently supported.
```

