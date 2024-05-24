# Comparing `tmp/instagram_profile_downloader-1.0.2.tar.gz` & `tmp/instagram_profile_downloader-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "instagram_profile_downloader-1.0.2.tar", last modified: Fri May 24 22:14:51 2024, max compression
+gzip compressed data, was "instagram_profile_downloader-1.0.3.tar", last modified: Fri May 24 22:19:24 2024, max compression
```

## Comparing `instagram_profile_downloader-1.0.2.tar` & `instagram_profile_downloader-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 tadeasfort   (501) staff       (20)        0 2024-05-24 22:14:51.674998 instagram_profile_downloader-1.0.2/
--rw-r--r--   0 tadeasfort   (501) staff       (20)        0 2024-05-24 18:29:25.000000 instagram_profile_downloader-1.0.2/LICENSE
--rw-r--r--   0 tadeasfort   (501) staff       (20)     4319 2024-05-24 22:14:51.674745 instagram_profile_downloader-1.0.2/PKG-INFO
--rw-r--r--   0 tadeasfort   (501) staff       (20)     3623 2024-05-24 19:12:15.000000 instagram_profile_downloader-1.0.2/README.md
-drwxr-xr-x   0 tadeasfort   (501) staff       (20)        0 2024-05-24 22:14:51.673256 instagram_profile_downloader-1.0.2/instagram_profile_downloader/
--rw-r--r--   0 tadeasfort   (501) staff       (20)        0 2024-05-24 18:23:50.000000 instagram_profile_downloader-1.0.2/instagram_profile_downloader/__init__.py
--rw-r--r--   0 tadeasfort   (501) staff       (20)    12772 2024-05-24 22:13:57.000000 instagram_profile_downloader-1.0.2/instagram_profile_downloader/instagram_profile_downloader.py
-drwxr-xr-x   0 tadeasfort   (501) staff       (20)        0 2024-05-24 22:14:51.674458 instagram_profile_downloader-1.0.2/instagram_profile_downloader.egg-info/
--rw-r--r--   0 tadeasfort   (501) staff       (20)     4319 2024-05-24 22:14:51.000000 instagram_profile_downloader-1.0.2/instagram_profile_downloader.egg-info/PKG-INFO
--rw-r--r--   0 tadeasfort   (501) staff       (20)      442 2024-05-24 22:14:51.000000 instagram_profile_downloader-1.0.2/instagram_profile_downloader.egg-info/SOURCES.txt
--rw-r--r--   0 tadeasfort   (501) staff       (20)        1 2024-05-24 22:14:51.000000 instagram_profile_downloader-1.0.2/instagram_profile_downloader.egg-info/dependency_links.txt
--rw-r--r--   0 tadeasfort   (501) staff       (20)      112 2024-05-24 22:14:51.000000 instagram_profile_downloader-1.0.2/instagram_profile_downloader.egg-info/entry_points.txt
--rw-r--r--   0 tadeasfort   (501) staff       (20)       66 2024-05-24 22:14:51.000000 instagram_profile_downloader-1.0.2/instagram_profile_downloader.egg-info/requires.txt
--rw-r--r--   0 tadeasfort   (501) staff       (20)       29 2024-05-24 22:14:51.000000 instagram_profile_downloader-1.0.2/instagram_profile_downloader.egg-info/top_level.txt
--rw-r--r--   0 tadeasfort   (501) staff       (20)       38 2024-05-24 22:14:51.675038 instagram_profile_downloader-1.0.2/setup.cfg
--rw-r--r--   0 tadeasfort   (501) staff       (20)     1032 2024-05-24 22:14:36.000000 instagram_profile_downloader-1.0.2/setup.py
+drwxr-xr-x   0 tadeasfort   (501) staff       (20)        0 2024-05-24 22:19:24.584147 instagram_profile_downloader-1.0.3/
+-rw-r--r--   0 tadeasfort   (501) staff       (20)        0 2024-05-24 18:29:25.000000 instagram_profile_downloader-1.0.3/LICENSE
+-rw-r--r--   0 tadeasfort   (501) staff       (20)     4319 2024-05-24 22:19:24.583866 instagram_profile_downloader-1.0.3/PKG-INFO
+-rw-r--r--   0 tadeasfort   (501) staff       (20)     3623 2024-05-24 19:12:15.000000 instagram_profile_downloader-1.0.3/README.md
+drwxr-xr-x   0 tadeasfort   (501) staff       (20)        0 2024-05-24 22:19:24.581972 instagram_profile_downloader-1.0.3/instagram_profile_downloader/
+-rw-r--r--   0 tadeasfort   (501) staff       (20)        0 2024-05-24 18:23:50.000000 instagram_profile_downloader-1.0.3/instagram_profile_downloader/__init__.py
+-rw-r--r--   0 tadeasfort   (501) staff       (20)    12836 2024-05-24 22:17:54.000000 instagram_profile_downloader-1.0.3/instagram_profile_downloader/instagram_profile_downloader.py
+drwxr-xr-x   0 tadeasfort   (501) staff       (20)        0 2024-05-24 22:19:24.583551 instagram_profile_downloader-1.0.3/instagram_profile_downloader.egg-info/
+-rw-r--r--   0 tadeasfort   (501) staff       (20)     4319 2024-05-24 22:19:24.000000 instagram_profile_downloader-1.0.3/instagram_profile_downloader.egg-info/PKG-INFO
+-rw-r--r--   0 tadeasfort   (501) staff       (20)      442 2024-05-24 22:19:24.000000 instagram_profile_downloader-1.0.3/instagram_profile_downloader.egg-info/SOURCES.txt
+-rw-r--r--   0 tadeasfort   (501) staff       (20)        1 2024-05-24 22:19:24.000000 instagram_profile_downloader-1.0.3/instagram_profile_downloader.egg-info/dependency_links.txt
+-rw-r--r--   0 tadeasfort   (501) staff       (20)      112 2024-05-24 22:19:24.000000 instagram_profile_downloader-1.0.3/instagram_profile_downloader.egg-info/entry_points.txt
+-rw-r--r--   0 tadeasfort   (501) staff       (20)       66 2024-05-24 22:19:24.000000 instagram_profile_downloader-1.0.3/instagram_profile_downloader.egg-info/requires.txt
+-rw-r--r--   0 tadeasfort   (501) staff       (20)       29 2024-05-24 22:19:24.000000 instagram_profile_downloader-1.0.3/instagram_profile_downloader.egg-info/top_level.txt
+-rw-r--r--   0 tadeasfort   (501) staff       (20)       38 2024-05-24 22:19:24.584188 instagram_profile_downloader-1.0.3/setup.cfg
+-rw-r--r--   0 tadeasfort   (501) staff       (20)     1032 2024-05-24 22:19:14.000000 instagram_profile_downloader-1.0.3/setup.py
```

### Comparing `instagram_profile_downloader-1.0.2/PKG-INFO` & `instagram_profile_downloader-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: instagram_profile_downloader
-Version: 1.0.2
+Version: 1.0.3
 Summary: A tool to download all images and videos and story highlights from an Instagram profile.
 Home-page: https://github.com/tadeasf/instagram_profile_downloader
 Author: Tadeas Fort
 Author-email: taddy.fort@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `instagram_profile_downloader-1.0.2/README.md` & `instagram_profile_downloader-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `instagram_profile_downloader-1.0.2/instagram_profile_downloader/instagram_profile_downloader.py` & `instagram_profile_downloader-1.0.3/instagram_profile_downloader/instagram_profile_downloader.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,14 +83,15 @@
             "[bold magenta]Please enter the Instagram profile name[/bold magenta]"
         )
         profile_name = click.prompt("", type=str)
         console.print(
             f"[green]Profile name set to:[/green] [bold]{profile_name}[/bold]"
         )
 
+    media_root = media_root or config.get("download_directory")
     if not media_root:
         media_root = select_input_directory()
 
     # Define directories based on the profile name
     base_dir = os.path.join(media_root, f"{profile_name}_media")
     log_dir = os.path.join(base_dir, "logs")
     media_dir = base_dir
```

### Comparing `instagram_profile_downloader-1.0.2/instagram_profile_downloader.egg-info/PKG-INFO` & `instagram_profile_downloader-1.0.3/instagram_profile_downloader.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: instagram-profile-downloader
-Version: 1.0.2
+Version: 1.0.3
 Summary: A tool to download all images and videos and story highlights from an Instagram profile.
 Home-page: https://github.com/tadeasf/instagram_profile_downloader
 Author: Tadeas Fort
 Author-email: taddy.fort@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `instagram_profile_downloader-1.0.2/setup.py` & `instagram_profile_downloader-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="instagram_profile_downloader",
-    version="1.0.2",
+    version="1.0.3",
     author="Tadeas Fort",
     author_email="taddy.fort@gmail.com",
     description="A tool to download all images and videos and story highlights from an Instagram profile.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/tadeasf/instagram_profile_downloader",
     packages=find_packages(),
```

