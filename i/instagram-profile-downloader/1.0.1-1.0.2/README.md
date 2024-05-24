# Comparing `tmp/instagram_profile_downloader-1.0.1.tar.gz` & `tmp/instagram_profile_downloader-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "instagram_profile_downloader-1.0.1.tar", last modified: Fri May 24 19:17:22 2024, max compression
+gzip compressed data, was "instagram_profile_downloader-1.0.2.tar", last modified: Fri May 24 22:14:51 2024, max compression
```

## Comparing `instagram_profile_downloader-1.0.1.tar` & `instagram_profile_downloader-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 tadeasfort   (501) staff       (20)        0 2024-05-24 19:17:22.292236 instagram_profile_downloader-1.0.1/
--rw-r--r--   0 tadeasfort   (501) staff       (20)        0 2024-05-24 18:29:25.000000 instagram_profile_downloader-1.0.1/LICENSE
--rw-r--r--   0 tadeasfort   (501) staff       (20)     4319 2024-05-24 19:17:22.292006 instagram_profile_downloader-1.0.1/PKG-INFO
--rw-r--r--   0 tadeasfort   (501) staff       (20)     3623 2024-05-24 19:12:15.000000 instagram_profile_downloader-1.0.1/README.md
-drwxr-xr-x   0 tadeasfort   (501) staff       (20)        0 2024-05-24 19:17:22.290874 instagram_profile_downloader-1.0.1/instagram_profile_downloader/
--rw-r--r--   0 tadeasfort   (501) staff       (20)        0 2024-05-24 18:23:50.000000 instagram_profile_downloader-1.0.1/instagram_profile_downloader/__init__.py
--rw-r--r--   0 tadeasfort   (501) staff       (20)    12199 2024-05-24 18:27:37.000000 instagram_profile_downloader-1.0.1/instagram_profile_downloader/instagram_profile_downloader.py
-drwxr-xr-x   0 tadeasfort   (501) staff       (20)        0 2024-05-24 19:17:22.291746 instagram_profile_downloader-1.0.1/instagram_profile_downloader.egg-info/
--rw-r--r--   0 tadeasfort   (501) staff       (20)     4319 2024-05-24 19:17:22.000000 instagram_profile_downloader-1.0.1/instagram_profile_downloader.egg-info/PKG-INFO
--rw-r--r--   0 tadeasfort   (501) staff       (20)      442 2024-05-24 19:17:22.000000 instagram_profile_downloader-1.0.1/instagram_profile_downloader.egg-info/SOURCES.txt
--rw-r--r--   0 tadeasfort   (501) staff       (20)        1 2024-05-24 19:17:22.000000 instagram_profile_downloader-1.0.1/instagram_profile_downloader.egg-info/dependency_links.txt
--rw-r--r--   0 tadeasfort   (501) staff       (20)      112 2024-05-24 19:17:22.000000 instagram_profile_downloader-1.0.1/instagram_profile_downloader.egg-info/entry_points.txt
--rw-r--r--   0 tadeasfort   (501) staff       (20)       66 2024-05-24 19:17:22.000000 instagram_profile_downloader-1.0.1/instagram_profile_downloader.egg-info/requires.txt
--rw-r--r--   0 tadeasfort   (501) staff       (20)       29 2024-05-24 19:17:22.000000 instagram_profile_downloader-1.0.1/instagram_profile_downloader.egg-info/top_level.txt
--rw-r--r--   0 tadeasfort   (501) staff       (20)       38 2024-05-24 19:17:22.292270 instagram_profile_downloader-1.0.1/setup.cfg
--rw-r--r--   0 tadeasfort   (501) staff       (20)     1032 2024-05-24 19:17:03.000000 instagram_profile_downloader-1.0.1/setup.py
+drwxr-xr-x   0 tadeasfort   (501) staff       (20)        0 2024-05-24 22:14:51.674998 instagram_profile_downloader-1.0.2/
+-rw-r--r--   0 tadeasfort   (501) staff       (20)        0 2024-05-24 18:29:25.000000 instagram_profile_downloader-1.0.2/LICENSE
+-rw-r--r--   0 tadeasfort   (501) staff       (20)     4319 2024-05-24 22:14:51.674745 instagram_profile_downloader-1.0.2/PKG-INFO
+-rw-r--r--   0 tadeasfort   (501) staff       (20)     3623 2024-05-24 19:12:15.000000 instagram_profile_downloader-1.0.2/README.md
+drwxr-xr-x   0 tadeasfort   (501) staff       (20)        0 2024-05-24 22:14:51.673256 instagram_profile_downloader-1.0.2/instagram_profile_downloader/
+-rw-r--r--   0 tadeasfort   (501) staff       (20)        0 2024-05-24 18:23:50.000000 instagram_profile_downloader-1.0.2/instagram_profile_downloader/__init__.py
+-rw-r--r--   0 tadeasfort   (501) staff       (20)    12772 2024-05-24 22:13:57.000000 instagram_profile_downloader-1.0.2/instagram_profile_downloader/instagram_profile_downloader.py
+drwxr-xr-x   0 tadeasfort   (501) staff       (20)        0 2024-05-24 22:14:51.674458 instagram_profile_downloader-1.0.2/instagram_profile_downloader.egg-info/
+-rw-r--r--   0 tadeasfort   (501) staff       (20)     4319 2024-05-24 22:14:51.000000 instagram_profile_downloader-1.0.2/instagram_profile_downloader.egg-info/PKG-INFO
+-rw-r--r--   0 tadeasfort   (501) staff       (20)      442 2024-05-24 22:14:51.000000 instagram_profile_downloader-1.0.2/instagram_profile_downloader.egg-info/SOURCES.txt
+-rw-r--r--   0 tadeasfort   (501) staff       (20)        1 2024-05-24 22:14:51.000000 instagram_profile_downloader-1.0.2/instagram_profile_downloader.egg-info/dependency_links.txt
+-rw-r--r--   0 tadeasfort   (501) staff       (20)      112 2024-05-24 22:14:51.000000 instagram_profile_downloader-1.0.2/instagram_profile_downloader.egg-info/entry_points.txt
+-rw-r--r--   0 tadeasfort   (501) staff       (20)       66 2024-05-24 22:14:51.000000 instagram_profile_downloader-1.0.2/instagram_profile_downloader.egg-info/requires.txt
+-rw-r--r--   0 tadeasfort   (501) staff       (20)       29 2024-05-24 22:14:51.000000 instagram_profile_downloader-1.0.2/instagram_profile_downloader.egg-info/top_level.txt
+-rw-r--r--   0 tadeasfort   (501) staff       (20)       38 2024-05-24 22:14:51.675038 instagram_profile_downloader-1.0.2/setup.cfg
+-rw-r--r--   0 tadeasfort   (501) staff       (20)     1032 2024-05-24 22:14:36.000000 instagram_profile_downloader-1.0.2/setup.py
```

### Comparing `instagram_profile_downloader-1.0.1/PKG-INFO` & `instagram_profile_downloader-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: instagram_profile_downloader
-Version: 1.0.1
+Version: 1.0.2
 Summary: A tool to download all images and videos and story highlights from an Instagram profile.
 Home-page: https://github.com/tadeasf/instagram_profile_downloader
 Author: Tadeas Fort
 Author-email: taddy.fort@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `instagram_profile_downloader-1.0.1/README.md` & `instagram_profile_downloader-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `instagram_profile_downloader-1.0.1/instagram_profile_downloader/instagram_profile_downloader.py` & `instagram_profile_downloader-1.0.2/instagram_profile_downloader/instagram_profile_downloader.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,24 +7,35 @@
 from rich.progress import Progress, SpinnerColumn, BarColumn, TextColumn
 from rich.console import Console
 from rich.traceback import install
 from PIL import Image
 import cv2
 import tkinter as tk
 from tkinter import filedialog
+import yaml
 
 # Install rich traceback handler
 install()
 
 # Initialize rich console
 console = Console()
 
 # Configure loguru to log to a file
 logger.remove()
 
+CONFIG_PATH = os.path.expanduser("~/.config/instagram_profile_downloader/config.yml")
+
+
+def load_config():
+    """Load the configuration file."""
+    if os.path.exists(CONFIG_PATH):
+        with open(CONFIG_PATH, "r") as file:
+            return yaml.safe_load(file)
+    return {}
+
 
 def generate_log_filename(profile_name):
     # Create the filename from the name of the profile we are downloading + current date - DD/MM/YYYY
     return f"{profile_name}_{time.strftime('%d-%m-%Y')}.log"
 
 
 def format_size(size):
@@ -61,14 +72,16 @@
 @click.argument("profile_name", required=False)
 @click.option("--media-root", required=False, help="Base directory for media output.")
 @click.option("--no-highlights", is_flag=True, help="Do not download highlights.")
 @click.option("--no-posts", is_flag=True, help="Do not download posts.")
 @click.option("--user", required=False, help="Instagram username.")
 @click.option("--password", required=False, help="Instagram password.")
 def main(profile_name, media_root, no_highlights, no_posts, user, password):
+    config = load_config()
+
     if not profile_name:
         console.print(
             "[bold magenta]Please enter the Instagram profile name[/bold magenta]"
         )
         profile_name = click.prompt("", type=str)
         console.print(
             f"[green]Profile name set to:[/green] [bold]{profile_name}[/bold]"
@@ -118,14 +131,18 @@
         diagnose=True,
     )
 
     # Create an instance of Instaloader
     L = instaloader.Instaloader()
 
     if not no_highlights:
+        # Check if credentials are provided in the config file
+        user = user or config.get("username")
+        password = password or config.get("password")
+
         if not user or not password:
             console.print(
                 "[bold magenta]Please enter your Instagram credentials[/bold magenta]"
             )
             console.print("[bold cyan]Username:[/bold cyan]", end=" ")
             user = click.prompt("", type=str)
             console.print("[bold cyan]Password:[/bold cyan]", end=" ")
@@ -135,14 +152,15 @@
     def download_media(url, output_dir):
         try:
             # Ensure the output directory exists
             os.makedirs(output_dir, exist_ok=True)
 
             # Extract filename from URL
             filename = os.path.join(output_dir, url.split("?")[0].split("/")[-1])
+            short_filename = os.path.basename(filename)  # Get only the filename
 
             # Download the media
             response = requests.get(url, stream=True)
             if response.status_code == 200:
                 with open(filename, "wb") as f:
                     for chunk in response.iter_content(1024):
                         f.write(chunk)
@@ -151,27 +169,27 @@
                 file_size = os.path.getsize(filename)
                 formatted_size = format_size(file_size)
 
                 if filename.lower().endswith((".png", ".jpg", ".jpeg")):
                     with Image.open(filename) as img:
                         width, height = img.size
                     console.print(
-                        f"[cyan bold]Image downloaded:[/cyan bold] {filename} [magenta]({width}x{height}px, {formatted_size})[/magenta]"
+                        f"[cyan bold]Downloaded:[/cyan bold] {short_filename} [magenta]({width}x{height}px, {formatted_size})[/magenta]"
                     )
                 elif filename.lower().endswith((".mp4", ".avi", ".mov")):
                     cap = cv2.VideoCapture(filename)
                     fps = cap.get(cv2.CAP_PROP_FPS)
                     total_frames = int(cap.get(cv2.CAP_PROP_FRAME_COUNT))
                     duration = total_frames / fps
                     console.print(
-                        f"[cyan bold]Video downloaded:[/cyan bold] {filename} [magenta](FPS: {fps:.2f}, Duration: {duration:.2f}s, {formatted_size})[/magenta]"
+                        f"[cyan bold]Downloaded:[/cyan bold] {short_filename} [magenta](FPS: {fps:.2f}, Duration: {duration:.2f}s, {formatted_size})[/magenta]"
                     )
                 else:
                     console.print(
-                        f"[cyan bold]Downloaded:[/cyan bold] {filename} [magenta]({formatted_size})[/magenta]"
+                        f"[cyan bold]Downloaded:[/cyan bold] {short_filename} [magenta]({formatted_size})[/magenta]"
                     )
             else:
                 logger.error(f"Failed to download {url}: HTTP {response.status_code}")
                 console.print(
                     f"[red]Failed to download {url}: HTTP {response.status_code}[/red]"
                 )
         except Exception as e:
```

### Comparing `instagram_profile_downloader-1.0.1/instagram_profile_downloader.egg-info/PKG-INFO` & `instagram_profile_downloader-1.0.2/instagram_profile_downloader.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: instagram-profile-downloader
-Version: 1.0.1
+Version: 1.0.2
 Summary: A tool to download all images and videos and story highlights from an Instagram profile.
 Home-page: https://github.com/tadeasf/instagram_profile_downloader
 Author: Tadeas Fort
 Author-email: taddy.fort@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `instagram_profile_downloader-1.0.1/setup.py` & `instagram_profile_downloader-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="instagram_profile_downloader",
-    version="1.0.1",
+    version="1.0.2",
     author="Tadeas Fort",
     author_email="taddy.fort@gmail.com",
     description="A tool to download all images and videos and story highlights from an Instagram profile.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/tadeasf/instagram_profile_downloader",
     packages=find_packages(),
```

