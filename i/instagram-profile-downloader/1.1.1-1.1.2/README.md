# Comparing `tmp/instagram_profile_downloader-1.1.1.tar.gz` & `tmp/instagram_profile_downloader-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "instagram_profile_downloader-1.1.1.tar", last modified: Fri May 24 23:48:48 2024, max compression
+gzip compressed data, was "instagram_profile_downloader-1.1.2.tar", last modified: Sat May 25 00:45:33 2024, max compression
```

## Comparing `instagram_profile_downloader-1.1.1.tar` & `instagram_profile_downloader-1.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:48:48.026512 instagram_profile_downloader-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 23:48:40.000000 instagram_profile_downloader-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4391 2024-05-24 23:48:48.026512 instagram_profile_downloader-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-05-24 23:48:40.000000 instagram_profile_downloader-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:48:48.022512 instagram_profile_downloader-1.1.1/instagram_profile_downloader/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 23:48:40.000000 instagram_profile_downloader-1.1.1/instagram_profile_downloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12768 2024-05-24 23:48:40.000000 instagram_profile_downloader-1.1.1/instagram_profile_downloader/instagram_profile_downloader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:48:48.026512 instagram_profile_downloader-1.1.1/instagram_profile_downloader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4391 2024-05-24 23:48:47.000000 instagram_profile_downloader-1.1.1/instagram_profile_downloader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-24 23:48:47.000000 instagram_profile_downloader-1.1.1/instagram_profile_downloader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 23:48:47.000000 instagram_profile_downloader-1.1.1/instagram_profile_downloader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-24 23:48:47.000000 instagram_profile_downloader-1.1.1/instagram_profile_downloader.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-24 23:48:47.000000 instagram_profile_downloader-1.1.1/instagram_profile_downloader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-24 23:48:47.000000 instagram_profile_downloader-1.1.1/instagram_profile_downloader.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 23:48:48.026512 instagram_profile_downloader-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-24 23:48:40.000000 instagram_profile_downloader-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 00:45:33.517681 instagram_profile_downloader-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 00:45:22.000000 instagram_profile_downloader-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4391 2024-05-25 00:45:33.517681 instagram_profile_downloader-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-05-25 00:45:22.000000 instagram_profile_downloader-1.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 00:45:33.513681 instagram_profile_downloader-1.1.2/instagram_profile_downloader/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 00:45:22.000000 instagram_profile_downloader-1.1.2/instagram_profile_downloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12833 2024-05-25 00:45:22.000000 instagram_profile_downloader-1.1.2/instagram_profile_downloader/instagram_profile_downloader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 00:45:33.517681 instagram_profile_downloader-1.1.2/instagram_profile_downloader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4391 2024-05-25 00:45:33.000000 instagram_profile_downloader-1.1.2/instagram_profile_downloader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-25 00:45:33.000000 instagram_profile_downloader-1.1.2/instagram_profile_downloader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 00:45:33.000000 instagram_profile_downloader-1.1.2/instagram_profile_downloader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-25 00:45:33.000000 instagram_profile_downloader-1.1.2/instagram_profile_downloader.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-25 00:45:33.000000 instagram_profile_downloader-1.1.2/instagram_profile_downloader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-25 00:45:33.000000 instagram_profile_downloader-1.1.2/instagram_profile_downloader.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 00:45:33.517681 instagram_profile_downloader-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-25 00:45:22.000000 instagram_profile_downloader-1.1.2/setup.py
```

### Comparing `instagram_profile_downloader-1.1.1/PKG-INFO` & `instagram_profile_downloader-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: instagram_profile_downloader
-Version: 1.1.1
+Version: 1.1.2
 Summary: A tool to download all images and videos and story highlights from an Instagram profile.
 Home-page: https://github.com/tadeasf/instagram_profile_downloader
 Author: Tadeas Fort
 Author-email: taddy.fort@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `instagram_profile_downloader-1.1.1/README.md` & `instagram_profile_downloader-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `instagram_profile_downloader-1.1.1/instagram_profile_downloader/instagram_profile_downloader.py` & `instagram_profile_downloader-1.1.2/instagram_profile_downloader/instagram_profile_downloader.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,14 +74,15 @@
 @click.option("--no-highlights", is_flag=True, help="Do not download highlights.")
 @click.option("--no-posts", is_flag=True, help="Do not download posts.")
 @click.option("--user", required=False, help="Instagram username.")
 @click.option("--password", required=False, help="Instagram password.")
 def main(profile_names, media_root, no_highlights, no_posts, user, password):
     config = load_config()
 
+    profile_names = profile_names or config.get("profile_names")
     if not profile_names:
         console.print(
             "[bold magenta]Please enter the Instagram profile names separated by commas[/bold magenta]"
         )
         profile_names = click.prompt("", type=str)
 
     profile_names = [name.strip() for name in profile_names.split(",")]
```

### Comparing `instagram_profile_downloader-1.1.1/instagram_profile_downloader.egg-info/PKG-INFO` & `instagram_profile_downloader-1.1.2/instagram_profile_downloader.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: instagram_profile_downloader
-Version: 1.1.1
+Version: 1.1.2
 Summary: A tool to download all images and videos and story highlights from an Instagram profile.
 Home-page: https://github.com/tadeasf/instagram_profile_downloader
 Author: Tadeas Fort
 Author-email: taddy.fort@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `instagram_profile_downloader-1.1.1/setup.py` & `instagram_profile_downloader-1.1.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="instagram_profile_downloader",
-    version="1.1.1",
+    version="1.1.2",
     author="Tadeas Fort",
     author_email="taddy.fort@gmail.com",
     description="A tool to download all images and videos and story highlights from an Instagram profile.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/tadeasf/instagram_profile_downloader",
     packages=find_packages(),
```

