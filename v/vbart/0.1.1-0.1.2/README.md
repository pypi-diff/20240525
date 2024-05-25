# Comparing `tmp/vbart-0.1.1.tar.gz` & `tmp/vbart-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vbart-0.1.1.tar", max compression
+gzip compressed data, was "vbart-0.1.2.tar", max compression
```

## Comparing `vbart-0.1.1.tar` & `vbart-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rwxr-xr-x   0        0        0     1065 2024-03-17 19:15:15.000000 vbart-0.1.1/LICENSE
--rw-r--r--   0        0        0     3640 2024-03-23 11:14:03.426977 vbart-0.1.1/README.md
--rw-r--r--   0        0        0     1640 2024-03-23 11:44:34.398227 vbart-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       97 2024-03-17 22:26:34.000000 vbart-0.1.1/src/vbart/Dockerfile
--rw-r--r--   0        0        0        0 2024-03-17 19:10:53.000000 vbart-0.1.1/src/vbart/__init__.py
--rwxr-xr-x   0        0        0     2562 2024-03-23 11:44:35.694357 vbart-0.1.1/src/vbart/__main__.py
--rw-r--r--   0        0        0      903 2024-03-22 15:27:37.762008 vbart-0.1.1/src/vbart/backup.py
--rw-r--r--   0        0        0     1709 2024-03-22 12:43:23.874291 vbart-0.1.1/src/vbart/backups.py
--rw-r--r--   0        0        0     3328 2024-03-20 15:36:59.459037 vbart-0.1.1/src/vbart/classes.py
--rw-r--r--   0        0        0      332 2024-03-23 11:35:16.501382 vbart-0.1.1/src/vbart/constants.py
--rw-r--r--   0        0        0      290 2024-03-20 13:47:47.151305 vbart-0.1.1/src/vbart/null.py
--rw-r--r--   0        0        0       15 2024-03-19 21:20:21.831775 vbart-0.1.1/src/vbart/parsers/__init__.py
--rw-r--r--   0        0        0      634 2024-03-22 15:33:25.284295 vbart-0.1.1/src/vbart/parsers/backup_args.py
--rw-r--r--   0        0        0      958 2024-03-22 15:25:46.784134 vbart-0.1.1/src/vbart/parsers/backups_args.py
--rw-r--r--   0        0        0      818 2024-03-22 22:19:32.495283 vbart-0.1.1/src/vbart/parsers/refresh_args.py
--rw-r--r--   0        0        0      943 2024-03-20 20:12:43.759794 vbart-0.1.1/src/vbart/parsers/restore_args.py
--rw-r--r--   0        0        0        0 2024-03-20 00:40:14.711491 vbart-0.1.1/src/vbart/py.typed
--rw-r--r--   0        0        0     1427 2024-03-22 18:10:21.693090 vbart-0.1.1/src/vbart/refresh.py
--rw-r--r--   0        0        0     2110 2024-03-20 15:49:53.630691 vbart-0.1.1/src/vbart/restore.py
--rw-r--r--   0        0        0     3877 2024-03-20 19:28:11.500069 vbart-0.1.1/src/vbart/utilities.py
--rw-r--r--   0        0        0     4997 1970-01-01 00:00:00.000000 vbart-0.1.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1065 2024-03-20 22:26:02.499143 vbart-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3632 2024-05-25 10:57:57.869381 vbart-0.1.2/README.md
+-rw-r--r--   0        0        0     1640 2024-05-25 10:55:53.858227 vbart-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       97 2024-03-20 22:26:02.500947 vbart-0.1.2/src/vbart/Dockerfile
+-rw-r--r--   0        0        0        0 2024-03-20 22:26:02.500992 vbart-0.1.2/src/vbart/__init__.py
+-rwxr-xr-x   0        0        0     2562 2024-05-25 10:55:57.838738 vbart-0.1.2/src/vbart/__main__.py
+-rw-r--r--   0        0        0      903 2024-03-22 22:20:42.849779 vbart-0.1.2/src/vbart/backup.py
+-rw-r--r--   0        0        0     1709 2024-03-20 22:26:02.501353 vbart-0.1.2/src/vbart/backups.py
+-rw-r--r--   0        0        0     3328 2024-03-20 22:26:02.501465 vbart-0.1.2/src/vbart/classes.py
+-rw-r--r--   0        0        0      332 2024-03-23 11:49:54.681533 vbart-0.1.2/src/vbart/constants.py
+-rw-r--r--   0        0        0      290 2024-03-20 22:26:02.501680 vbart-0.1.2/src/vbart/null.py
+-rw-r--r--   0        0        0       15 2024-03-23 11:49:54.681651 vbart-0.1.2/src/vbart/parsers/__init__.py
+-rw-r--r--   0        0        0      634 2024-03-23 11:49:54.681887 vbart-0.1.2/src/vbart/parsers/backup_args.py
+-rw-r--r--   0        0        0      958 2024-03-23 11:49:54.682126 vbart-0.1.2/src/vbart/parsers/backups_args.py
+-rw-r--r--   0        0        0      818 2024-03-23 11:49:54.682782 vbart-0.1.2/src/vbart/parsers/refresh_args.py
+-rw-r--r--   0        0        0      943 2024-03-23 11:49:54.682885 vbart-0.1.2/src/vbart/parsers/restore_args.py
+-rw-r--r--   0        0        0        0 2024-03-20 22:26:02.501725 vbart-0.1.2/src/vbart/py.typed
+-rw-r--r--   0        0        0     1427 2024-03-22 22:20:42.849969 vbart-0.1.2/src/vbart/refresh.py
+-rw-r--r--   0        0        0     2110 2024-03-20 22:26:02.501976 vbart-0.1.2/src/vbart/restore.py
+-rw-r--r--   0        0        0     3877 2024-03-20 22:26:02.502094 vbart-0.1.2/src/vbart/utilities.py
+-rw-r--r--   0        0        0     4989 1970-01-01 00:00:00.000000 vbart-0.1.2/PKG-INFO
```

### Comparing `vbart-0.1.1/LICENSE` & `vbart-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vbart-0.1.1/README.md` & `vbart-0.1.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/vbart)
 ![GitHub repo size](https://img.shields.io/github/repo-size/geozeke/vbart)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/vbart)
 
 <br>
 
 <img
-src="https://drive.google.com/uc?export=view&id=1H04KVAA3ohH_dLXIrC0bXuJXDn3VutKc"
+src="https://lh3.googleusercontent.com/d/1H04KVAA3ohH_dLXIrC0bXuJXDn3VutKc"
 alt = "Dinobox logo" width="120"/>
 
 ## Volume Backup And Restoration Tool for Docker
 
 Why is backing up named docker volumes so hard? There's an
-[extension][def] for Docker Desktop, but I just want a simple, easy to
-use, command-line tool that allows me to backup and restore my named
-docker volumes. That's what vbart does.
+[extension][def] for Docker Desktop, but I just want a simple,
+easy-to-use command line tool that allows me to backup and restore my
+named docker volumes. That's what vbart does.
 
 With vbart you can:
 
 * Backup a single named volume.
 * Backup all active named volumes on your host.
 * Backup just the volumes you list in a separate file.
 * Restore a single backup to a named volume.
```

### Comparing `vbart-0.1.1/pyproject.toml` & `vbart-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vbart"
-version = "0.1.1"
+version = "0.1.2"
 description = "Volume Backup And Restoration Tool for Docker"
 authors = ["Peter Nardi <pete@nardi.com>"]
 maintainers = ["Peter Nardi <pete@nardi.com>"]
 homepage = "https://github.com/geozeke/vbart"
 readme = "README.md"
 packages = [{ include = "vbart", from = "src" }]
 include = ["LICENSE"]
```

### Comparing `vbart-0.1.1/src/vbart/__main__.py` & `vbart-0.1.2/src/vbart/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     if not (shutil.which("docker")):
         print("\nYou must have docker installed to use vbart.\n")
         sys.exit(1)
 
     msg = """Volume Backup And Restoration Tool (for docker). A tool to
     easily backup and restore named docker volumes. For help on any
     command below, use: vbart {command} -h"""
-    epi = "Version: 0.1.1"
+    epi = "Version: 0.1.2"
     parser = argparse.ArgumentParser(
         description=msg,
         epilog=epi,
     )
     subparsers = parser.add_subparsers(title="commands", dest="cmd")
 
     # Dynamically load argument subparsers.
```

### Comparing `vbart-0.1.1/src/vbart/backup.py` & `vbart-0.1.2/src/vbart/backup.py`

 * *Files identical despite different names*

### Comparing `vbart-0.1.1/src/vbart/backups.py` & `vbart-0.1.2/src/vbart/backups.py`

 * *Files identical despite different names*

### Comparing `vbart-0.1.1/src/vbart/classes.py` & `vbart-0.1.2/src/vbart/classes.py`

 * *Files identical despite different names*

### Comparing `vbart-0.1.1/src/vbart/parsers/backup_args.py` & `vbart-0.1.2/src/vbart/parsers/backup_args.py`

 * *Files identical despite different names*

### Comparing `vbart-0.1.1/src/vbart/parsers/backups_args.py` & `vbart-0.1.2/src/vbart/parsers/backups_args.py`

 * *Files identical despite different names*

### Comparing `vbart-0.1.1/src/vbart/parsers/refresh_args.py` & `vbart-0.1.2/src/vbart/parsers/refresh_args.py`

 * *Files identical despite different names*

### Comparing `vbart-0.1.1/src/vbart/parsers/restore_args.py` & `vbart-0.1.2/src/vbart/parsers/restore_args.py`

 * *Files identical despite different names*

### Comparing `vbart-0.1.1/src/vbart/refresh.py` & `vbart-0.1.2/src/vbart/refresh.py`

 * *Files identical despite different names*

### Comparing `vbart-0.1.1/src/vbart/restore.py` & `vbart-0.1.2/src/vbart/restore.py`

 * *Files identical despite different names*

### Comparing `vbart-0.1.1/src/vbart/utilities.py` & `vbart-0.1.2/src/vbart/utilities.py`

 * *Files identical despite different names*

### Comparing `vbart-0.1.1/PKG-INFO` & `vbart-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vbart
-Version: 0.1.1
+Version: 0.1.2
 Summary: Volume Backup And Restoration Tool for Docker
 Home-page: https://github.com/geozeke/vbart
 Keywords: archive,backup,compose,compress,compression,docker,restore,vbart,volume,volumes
 Author: Peter Nardi
 Author-email: pete@nardi.com
 Maintainer: Peter Nardi
 Maintainer-email: pete@nardi.com
@@ -40,23 +40,23 @@
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/vbart)
 ![GitHub repo size](https://img.shields.io/github/repo-size/geozeke/vbart)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/vbart)
 
 <br>
 
 <img
-src="https://drive.google.com/uc?export=view&id=1H04KVAA3ohH_dLXIrC0bXuJXDn3VutKc"
+src="https://lh3.googleusercontent.com/d/1H04KVAA3ohH_dLXIrC0bXuJXDn3VutKc"
 alt = "Dinobox logo" width="120"/>
 
 ## Volume Backup And Restoration Tool for Docker
 
 Why is backing up named docker volumes so hard? There's an
-[extension][def] for Docker Desktop, but I just want a simple, easy to
-use, command-line tool that allows me to backup and restore my named
-docker volumes. That's what vbart does.
+[extension][def] for Docker Desktop, but I just want a simple,
+easy-to-use command line tool that allows me to backup and restore my
+named docker volumes. That's what vbart does.
 
 With vbart you can:
 
 * Backup a single named volume.
 * Backup all active named volumes on your host.
 * Backup just the volumes you list in a separate file.
 * Restore a single backup to a named volume.
```

