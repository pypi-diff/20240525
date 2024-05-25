# Comparing `tmp/pih-plb_db-0.20.4.tar.gz` & `tmp/pih-plb_db-0.20.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-plb_db-0.20.4.tar", last modified: Fri May 24 15:21:52 2024, max compression
+gzip compressed data, was "pih-plb_db-0.20.5.tar", last modified: Sat May 25 15:28:55 2024, max compression
```

## Comparing `pih-plb_db-0.20.4.tar` & `pih-plb_db-0.20.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 15:21:52.334277 pih-plb_db-0.20.4/
--rw-rw-rw-   0        0        0      282 2024-05-24 15:21:52.303030 pih-plb_db-0.20.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-24 15:21:51.957191 pih-plb_db-0.20.4/PolibaseDatabaseService/
--rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-plb_db-0.20.4/PolibaseDatabaseService/__init__.py
--rw-rw-rw-   0        0        0      158 2024-02-15 00:09:03.000000 pih-plb_db-0.20.4/PolibaseDatabaseService/__main__.py
--rw-rw-rw-   0        0        0    12167 2024-05-24 15:21:21.000000 pih-plb_db-0.20.4/PolibaseDatabaseService/api.py
--rw-rw-rw-   0        0        0     1082 2024-05-24 15:21:34.000000 pih-plb_db-0.20.4/PolibaseDatabaseService/const.py
--rw-rw-rw-   0        0        0     1135 2024-04-22 03:09:08.000000 pih-plb_db-0.20.4/PolibaseDatabaseService/service.py
-drwxrwxrwx   0        0        0        0 2024-05-24 15:21:52.256157 pih-plb_db-0.20.4/pih_plb_db.egg-info/
--rw-rw-rw-   0        0        0      282 2024-05-24 15:21:51.000000 pih-plb_db-0.20.4/pih_plb_db.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      376 2024-05-24 15:21:51.000000 pih-plb_db-0.20.4/pih_plb_db.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 15:21:51.000000 pih-plb_db-0.20.4/pih_plb_db.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2024-05-24 15:21:51.000000 pih-plb_db-0.20.4/pih_plb_db.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        5 2024-05-24 15:21:51.000000 pih-plb_db-0.20.4/pih_plb_db.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2024-05-24 15:21:51.000000 pih-plb_db-0.20.4/pih_plb_db.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-24 15:21:52.334277 pih-plb_db-0.20.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-25 15:28:56.094345 pih-plb_db-0.20.5/
+-rw-rw-rw-   0        0        0      282 2024-05-25 15:28:56.078698 pih-plb_db-0.20.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-25 15:28:55.640160 pih-plb_db-0.20.5/PolibaseDatabaseService/
+-rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-plb_db-0.20.5/PolibaseDatabaseService/__init__.py
+-rw-rw-rw-   0        0        0      158 2024-02-15 00:09:03.000000 pih-plb_db-0.20.5/PolibaseDatabaseService/__main__.py
+-rw-rw-rw-   0        0        0    11976 2024-05-25 15:24:27.000000 pih-plb_db-0.20.5/PolibaseDatabaseService/api.py
+-rw-rw-rw-   0        0        0     1081 2024-05-25 15:24:24.000000 pih-plb_db-0.20.5/PolibaseDatabaseService/const.py
+-rw-rw-rw-   0        0        0     1135 2024-04-22 03:09:08.000000 pih-plb_db-0.20.5/PolibaseDatabaseService/service.py
+drwxrwxrwx   0        0        0        0 2024-05-25 15:28:56.031824 pih-plb_db-0.20.5/pih_plb_db.egg-info/
+-rw-rw-rw-   0        0        0      282 2024-05-25 15:28:55.000000 pih-plb_db-0.20.5/pih_plb_db.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      376 2024-05-25 15:28:55.000000 pih-plb_db-0.20.5/pih_plb_db.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 15:28:55.000000 pih-plb_db-0.20.5/pih_plb_db.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2024-05-25 15:28:55.000000 pih-plb_db-0.20.5/pih_plb_db.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        5 2024-05-25 15:28:55.000000 pih-plb_db-0.20.5/pih_plb_db.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2024-05-25 15:28:55.000000 pih-plb_db-0.20.5/pih_plb_db.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-25 15:28:56.109948 pih-plb_db-0.20.5/setup.cfg
```

### Comparing `pih-plb_db-0.20.4/PolibaseDatabaseService/api.py` & `pih-plb_db-0.20.5/PolibaseDatabaseService/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,28 +19,26 @@
             (POLIBASE_NAME, DATABASE_DUMP.FILE_NAME)
         )
         nas_polibase_database_dump_folder_name: str = A.PTH.join(
             POLIBASE_NAME, DATABASE_DUMP.FILE_NAME
         )
         polibase_folder_path: str = A.PTH.join(
             j((MOUNT_POINT.POLIBASE, A.CT.SPLITTER)),
-            "\\",
+            os.sep,
             local_polibase_database_dump_folder_name,
         )
 
         if test:
             file_name = TEST_NAME
         else:
             if n(file_name):
                 file_name = A.D.now_to_string(A.CT_P.DB_DATETIME_FORMAT)
 
-        dump_file_name_result: str = DATABASE_DUMP.RESULT_FILE_NAME
-
-        dump_file_name_result = A.PTH.add_extension(
-            dump_file_name_result, DATABASE_DUMP.FILE_EXTENSION
+        dump_file_name_result: str = A.PTH.add_extension(
+            DATABASE_DUMP.RESULT_FILE_NAME, DATABASE_DUMP.FILE_EXTENSION
         )
         file_database_dump_name_out: str = A.PTH.add_extension(
             file_name, DATABASE_DUMP.FILE_EXTENSION
         )
         if test:
             polibase_folder_path_src: str = polibase_folder_path
             polibase_folder_path = A.PTH.for_windows(
@@ -158,21 +156,22 @@
                 )
             )
             os.system(nas_create_connection_command)
             os.system(polibase2_create_connection_command)
 
         # step 3
         A.E.backup_notify_about_polibase_creation_archived_db_dumb_start()
-        archive_creation_parameters: str = A.S.get(
+        archive_creation_parameters: str | None = A.S.get(
             A.CT_S.POLIBASE_DB_DUMP_ARCHIVE_CREATION_PARAMETERS
         )
         password_parameter: str = j(
             (
                 "-p",
-                esc(A.D_V_E.value("POLIBASE_DATABASE_ARCHIVE_PASSWORD")),
+                "1"
+                #esc(A.D_V_E.value("POLIBASE_DATABASE_ARCHIVE_PASSWORD")),
             )
         )
         compression_level: int | None = A.S.get(
             A.CT_S.POLIBASE_DB_DUMP_ARCHIVE_COMPRESSION_LEVEL
         )
         A.L.debug_bot(
             js(
@@ -189,17 +188,15 @@
                                                 j(("a -t", ARCHIVE_TYPE)),
                                                 (
                                                     None
                                                     if n(compression_level)
                                                     else j(
                                                         (
                                                             "-mx",
-                                                            A.S.get(
-                                                                A.CT_S.POLIBASE_DB_DUMP_ARCHIVE_COMPRESSION_LEVEL
-                                                            ),
+                                                            compression_level,
                                                         )
                                                     )
                                                 ),
                                                 password_parameter,
                                             )
                                         )
                                     )
@@ -256,15 +253,15 @@
                                     PRECONNECTED_MOUNT_POINT.POLIBASE2
                                     if USE_PRECONNECTED_DISKS
                                     else MOUNT_POINT.POLIBASE2
                                 ),
                                 A.CT.SPLITTER,
                             )
                         ),
-                        "\\",
+                        os.sep,
                         dump_file_name_result,
                     )
                 ),
             )
         )
         polibase_file_rename_command: str = js(
             (
@@ -277,15 +274,15 @@
                                     PRECONNECTED_MOUNT_POINT.POLIBASE2
                                     if USE_PRECONNECTED_DISKS
                                     else MOUNT_POINT.POLIBASE2
                                 ),
                                 A.CT.SPLITTER,
                             )
                         ),
-                        "\\",
+                        os.sep,
                         file_database_dump_name_out,
                     )
                 ),
                 dump_file_name_result,
             )
         )
```

### Comparing `pih-plb_db-0.20.4/PolibaseDatabaseService/const.py` & `pih-plb_db-0.20.5/PolibaseDatabaseService/const.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,26 +4,26 @@
 from pih.consts import CONST
 from pih.collections.service import ServiceDescription
 
 NAME: str = "PolibaseDatabase"
 
 HOST = A.CT_H.POLIBASE
 
-VERSION: str = "0.20.4"
+VERSION: str = "0.20.5"
 
 
 SD: ServiceDescription = ServiceDescription(
     name=NAME,
     host=HOST.NAME,
     description="Polibase database service",
     commands=("create_polibase_database_backup",),
     version=VERSION,
     use_standalone=True,
     standalone_name="plb_db",
-    host_changeable=False,
+    host_changeable=True,
     run_from_system_account=True,
     python_executable_path=CONST.UNKNOWN_VALUE,
 )
 
 TEST_NAME: str = "test"
 STUB_DIRECTORY_NAME: str = "stub"
 #
```

### Comparing `pih-plb_db-0.20.4/PolibaseDatabaseService/service.py` & `pih-plb_db-0.20.5/PolibaseDatabaseService/service.py`

 * *Files identical despite different names*

