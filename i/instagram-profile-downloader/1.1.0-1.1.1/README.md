# Comparing `tmp/instagram_profile_downloader-1.1.0.tar.gz` & `tmp/instagram_profile_downloader-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "instagram_profile_downloader-1.1.0.tar", last modified: Fri May 24 23:35:38 2024, max compression
+gzip compressed data, was "instagram_profile_downloader-1.1.1.tar", last modified: Fri May 24 23:48:48 2024, max compression
```

## Comparing `instagram_profile_downloader-1.1.0.tar` & `instagram_profile_downloader-1.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:35:38.910374 instagram_profile_downloader-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 23:35:30.000000 instagram_profile_downloader-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4391 2024-05-24 23:35:38.906374 instagram_profile_downloader-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-05-24 23:35:30.000000 instagram_profile_downloader-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:35:38.906374 instagram_profile_downloader-1.1.0/instagram_profile_downloader/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 23:35:30.000000 instagram_profile_downloader-1.1.0/instagram_profile_downloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14942 2024-05-24 23:35:30.000000 instagram_profile_downloader-1.1.0/instagram_profile_downloader/instagram_profile_downloader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:35:38.906374 instagram_profile_downloader-1.1.0/instagram_profile_downloader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4391 2024-05-24 23:35:38.000000 instagram_profile_downloader-1.1.0/instagram_profile_downloader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-24 23:35:38.000000 instagram_profile_downloader-1.1.0/instagram_profile_downloader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 23:35:38.000000 instagram_profile_downloader-1.1.0/instagram_profile_downloader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-24 23:35:38.000000 instagram_profile_downloader-1.1.0/instagram_profile_downloader.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-24 23:35:38.000000 instagram_profile_downloader-1.1.0/instagram_profile_downloader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-24 23:35:38.000000 instagram_profile_downloader-1.1.0/instagram_profile_downloader.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 23:35:38.910374 instagram_profile_downloader-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-24 23:35:30.000000 instagram_profile_downloader-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:48:48.026512 instagram_profile_downloader-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 23:48:40.000000 instagram_profile_downloader-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4391 2024-05-24 23:48:48.026512 instagram_profile_downloader-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-05-24 23:48:40.000000 instagram_profile_downloader-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:48:48.022512 instagram_profile_downloader-1.1.1/instagram_profile_downloader/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 23:48:40.000000 instagram_profile_downloader-1.1.1/instagram_profile_downloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12768 2024-05-24 23:48:40.000000 instagram_profile_downloader-1.1.1/instagram_profile_downloader/instagram_profile_downloader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:48:48.026512 instagram_profile_downloader-1.1.1/instagram_profile_downloader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4391 2024-05-24 23:48:47.000000 instagram_profile_downloader-1.1.1/instagram_profile_downloader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-24 23:48:47.000000 instagram_profile_downloader-1.1.1/instagram_profile_downloader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 23:48:47.000000 instagram_profile_downloader-1.1.1/instagram_profile_downloader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-24 23:48:47.000000 instagram_profile_downloader-1.1.1/instagram_profile_downloader.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-24 23:48:47.000000 instagram_profile_downloader-1.1.1/instagram_profile_downloader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-24 23:48:47.000000 instagram_profile_downloader-1.1.1/instagram_profile_downloader.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 23:48:48.026512 instagram_profile_downloader-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-24 23:48:40.000000 instagram_profile_downloader-1.1.1/setup.py
```

### Comparing `instagram_profile_downloader-1.1.0/PKG-INFO` & `instagram_profile_downloader-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: instagram_profile_downloader
-Version: 1.1.0
+Version: 1.1.1
 Summary: A tool to download all images and videos and story highlights from an Instagram profile.
 Home-page: https://github.com/tadeasf/instagram_profile_downloader
 Author: Tadeas Fort
 Author-email: taddy.fort@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `instagram_profile_downloader-1.1.0/README.md` & `instagram_profile_downloader-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `instagram_profile_downloader-1.1.0/instagram_profile_downloader/instagram_profile_downloader.py` & `instagram_profile_downloader-1.1.1/instagram_profile_downloader/instagram_profile_downloader.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import os
 import time
+import requests
 import instaloader
 import rich_click as click
 from loguru import logger
 from rich.progress import Progress, SpinnerColumn, BarColumn, TextColumn
 from rich.console import Console
 from rich.traceback import install
 from PIL import Image
 import cv2
 import tkinter as tk
 from tkinter import filedialog
 import yaml
-import asyncio
-from aiohttp import ClientSession
 
 # Install rich traceback handler
 install()
 
 # Initialize rich console
 console = Console()
 
@@ -83,14 +82,15 @@
         console.print(
             "[bold magenta]Please enter the Instagram profile names separated by commas[/bold magenta]"
         )
         profile_names = click.prompt("", type=str)
 
     profile_names = [name.strip() for name in profile_names.split(",")]
 
+    # instead of this: console.print(f"[green]Profile names set to:[/green] [bold]{profile_names}[/bold]") i would like to get multiple lines of console output -> one line per profile name
     for profile_name in profile_names:
         console.print(
             f"[green]Profile name set to:[/green] [bold]{profile_name}[/bold]"
         )
 
     media_root = media_root or config.get("download_directory")
     if not media_root:
@@ -109,67 +109,62 @@
         console.print("[bold cyan]Password:[/bold cyan]", end=" ")
         password = click.prompt("", type=str, hide_input=True)
 
     # Create an instance of Instaloader
     L = instaloader.Instaloader()
     L.login(user, password)
 
-    async def download_media(
-        url, output_dir, session: ClientSession, semaphore: asyncio.Semaphore
-    ):
-        async with semaphore:
-            try:
-                # Ensure the output directory exists
-                os.makedirs(output_dir, exist_ok=True)
-
-                # Extract filename from URL
-                filename = os.path.join(output_dir, url.split("?")[0].split("/")[-1])
-                short_filename = os.path.basename(filename)  # Get only the filename
-
-                # Download the media
-                async with session.get(url) as response:
-                    if response.status == 200:
-                        with open(filename, "wb") as f:
-                            async for chunk in response.content.iter_chunked(1024):
-                                f.write(chunk)
-                        logger.info(f"Downloaded {url} to {filename}")
-
-                        file_size = os.path.getsize(filename)
-                        formatted_size = format_size(file_size)
-
-                        if filename.lower().endswith((".png", ".jpg", ".jpeg")):
-                            with Image.open(filename) as img:
-                                width, height = img.size
-                            console.print(
-                                f"[cyan bold]Downloaded:[/cyan bold] {short_filename} [magenta]({width}x{height}px, {formatted_size})[/magenta]"
-                            )
-                        elif filename.lower().endswith((".mp4", ".avi", ".mov")):
-                            cap = cv2.VideoCapture(filename)
-                            fps = cap.get(cv2.CAP_PROP_FPS)
-                            total_frames = int(cap.get(cv2.CAP_PROP_FRAME_COUNT))
-                            duration = total_frames / fps
-                            console.print(
-                                f"[cyan bold]Downloaded:[/cyan bold] {short_filename} [magenta](FPS: {fps:.2f}, Duration: {duration:.2f}s, {formatted_size})[/magenta]"
-                            )
-                        else:
-                            console.print(
-                                f"[cyan bold]Downloaded:[/cyan bold] {short_filename} [magenta]({formatted_size})[/magenta]"
-                            )
-                    else:
-                        logger.error(
-                            f"Failed to download {url}: HTTP {response.status}"
-                        )
-                        console.print(
-                            f"[red]Failed to download {url}: HTTP {response.status}[/red]"
-                        )
-            except Exception as e:
-                logger.error(f"Failed to download {url}: {e}")
-                console.print(f"[red]Failed to download {url}: {e}[/red]")
+    def download_media(url, output_dir):
+        try:
+            # Ensure the output directory exists
+            os.makedirs(output_dir, exist_ok=True)
+
+            # Extract filename from URL
+            filename = os.path.join(output_dir, url.split("?")[0].split("/")[-1])
+            short_filename = os.path.basename(filename)  # Get only the filename
+
+            # Download the media
+            response = requests.get(url, stream=True)
+            if response.status_code == 200:
+                with open(filename, "wb") as f:
+                    for chunk in response.iter_content(1024):
+                        f.write(chunk)
+                logger.info(f"Downloaded {url} to {filename}")
+
+                file_size = os.path.getsize(filename)
+                formatted_size = format_size(file_size)
+
+                if filename.lower().endswith((".png", ".jpg", ".jpeg")):
+                    with Image.open(filename) as img:
+                        width, height = img.size
+                    console.print(
+                        f"[cyan bold]Downloaded:[/cyan bold] {short_filename} [magenta]({width}x{height}px, {formatted_size})[/magenta]"
+                    )
+                elif filename.lower().endswith((".mp4", ".avi", ".mov")):
+                    cap = cv2.VideoCapture(filename)
+                    fps = cap.get(cv2.CAP_PROP_FPS)
+                    total_frames = int(cap.get(cv2.CAP_PROP_FRAME_COUNT))
+                    duration = total_frames / fps
+                    console.print(
+                        f"[cyan bold]Downloaded:[/cyan bold] {short_filename} [magenta](FPS: {fps:.2f}, Duration: {duration:.2f}s, {formatted_size})[/magenta]"
+                    )
+                else:
+                    console.print(
+                        f"[cyan bold]Downloaded:[/cyan bold] {short_filename} [magenta]({formatted_size})[/magenta]"
+                    )
+            else:
+                logger.error(f"Failed to download {url}: HTTP {response.status_code}")
+                console.print(
+                    f"[red]Failed to download {url}: HTTP {response.status_code}[/red]"
+                )
+        except Exception as e:
+            logger.error(f"Failed to download {url}: {e}")
+            console.print(f"[red]Failed to download {url}: {e}[/red]")
 
-    async def get_profile_media(profile_name, progress):
+    def get_profile_media(profile_name):
         try:
             # Define directories based on the profile name
             base_dir = os.path.join(media_root, f"{profile_name}_media")
             log_dir = os.path.join(base_dir, "logs")
             media_dir = base_dir
 
             # Ensure the directories exist
@@ -218,133 +213,91 @@
                 total_highlights = 0
 
             logger.info(f"Total posts: {total_posts}")
             logger.info(f"Total highlights: {total_highlights}")
             console.print(f"[blue]Total posts: {total_posts}[/blue]")
             console.print(f"[blue]Total highlights: {total_highlights}[/blue]")
 
-            async with ClientSession() as session:
-                semaphore = asyncio.Semaphore(4)  # Limiting to 4 concurrent downloads
-                tasks = []
-                if not no_posts:
+            if not no_posts:
+                # Download posts with progress bar
+                with Progress(
+                    SpinnerColumn(),
+                    BarColumn(),
+                    "[progress.percentage]{task.percentage:>3.1f}%",
+                    TextColumn("{task.description}"),
+                    console=console,
+                ) as progress:
                     post_task = progress.add_task(
-                        f"Downloading posts for {profile_name}...", total=total_posts
+                        "Downloading posts...", total=total_posts
                     )
 
                     for post in profile.get_posts():
                         try:
                             if post.typename == "GraphImage":
                                 logger.info(f"Downloading image: {post.url}")
-                                tasks.append(
-                                    download_media(
-                                        post.url, media_dir, session, semaphore
-                                    )
-                                )
+                                download_media(post.url, media_dir)
                             elif post.typename == "GraphVideo":
                                 logger.info(f"Downloading video: {post.video_url}")
-                                tasks.append(
-                                    download_media(
-                                        post.video_url, media_dir, session, semaphore
-                                    )
-                                )
+                                download_media(post.video_url, media_dir)
                             elif post.typename == "GraphSidecar":
                                 for sidecar in post.get_sidecar_nodes():
                                     if sidecar.is_video:
                                         logger.info(
                                             f"Downloading sidecar video: {sidecar.video_url}"
                                         )
-                                        tasks.append(
-                                            download_media(
-                                                sidecar.video_url,
-                                                media_dir,
-                                                session,
-                                                semaphore,
-                                            )
-                                        )
+                                        download_media(sidecar.video_url, media_dir)
                                     else:
                                         logger.info(
                                             f"Downloading sidecar image: {sidecar.display_url}"
                                         )
-                                        tasks.append(
-                                            download_media(
-                                                sidecar.display_url,
-                                                media_dir,
-                                                session,
-                                                semaphore,
-                                            )
-                                        )
+                                        download_media(sidecar.display_url, media_dir)
                             # Implement rate limiting
-                            await asyncio.sleep(0.2)
+                            time.sleep(0.2)
                         except Exception as e:
                             logger.error(f"Error processing post: {e}")
                             console.print(f"[red]Error processing post: {e}[/red]")
                         progress.update(post_task, advance=1)
 
-                    await asyncio.gather(*tasks, return_exceptions=True)
-
-                if not no_highlights:
+            if not no_highlights:
+                # Download highlights and their stories with spinners
+                with Progress(
+                    SpinnerColumn(), TextColumn("{task.description}"), console=console
+                ) as progress:
                     for highlight in highlights:
                         highlight_title = (
                             f"[bold magenta]{highlight.title}[/bold magenta]"
                         )
                         highlight_task = progress.add_task(
-                            f"Downloading highlight {highlight_title}",
-                            total=len(highlight.get_items()),
+                            f"Downloading highlight {highlight_title}"
                         )
 
                         for item in highlight.get_items():
                             try:
                                 if item.is_video:
                                     logger.info(
                                         f"Downloading highlight video: {item.video_url}"
                                     )
-                                    tasks.append(
-                                        download_media(
-                                            item.video_url,
-                                            media_dir,
-                                            session,
-                                            semaphore,
-                                        )
-                                    )
+                                    download_media(item.video_url, media_dir)
                                 else:
                                     logger.info(
                                         f"Downloading highlight image: {item.url}"
                                     )
-                                    tasks.append(
-                                        download_media(
-                                            item.url, media_dir, session, semaphore
-                                        )
-                                    )
+                                    download_media(item.url, media_dir)
                                 # Implement rate limiting
-                                await asyncio.sleep(0.2)
+                                time.sleep(0.2)
                             except Exception as e:
                                 logger.error(f"Error processing highlight item: {e}")
                                 console.print(
                                     f"[red]Error processing highlight item: {e}[/red]"
                                 )
-                            progress.update(highlight_task, advance=1)
-
-                    await asyncio.gather(*tasks, return_exceptions=True)
+                        progress.update(highlight_task, completed=1)
 
         except Exception as e:
             logger.error(f"Error fetching profile {profile_name}: {e}")
             console.print(f"[red]Error fetching profile {profile_name}: {e}[/red]")
 
-    async def main_async():
-        with Progress(
-            SpinnerColumn(),
-            BarColumn(),
-            "[progress.percentage]{task.percentage:>3.1f}%",
-            TextColumn("{task.description}"),
-            console=console,
-        ) as progress:
-            tasks = [
-                get_profile_media(profile_name, progress)
-                for profile_name in profile_names
-            ]
-            await asyncio.gather(*tasks)
-
-    asyncio.run(main_async())
+    for profile_name in profile_names:
+        get_profile_media(profile_name)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `instagram_profile_downloader-1.1.0/instagram_profile_downloader.egg-info/PKG-INFO` & `instagram_profile_downloader-1.1.1/instagram_profile_downloader.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: instagram_profile_downloader
-Version: 1.1.0
+Version: 1.1.1
 Summary: A tool to download all images and videos and story highlights from an Instagram profile.
 Home-page: https://github.com/tadeasf/instagram_profile_downloader
 Author: Tadeas Fort
 Author-email: taddy.fort@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `instagram_profile_downloader-1.1.0/setup.py` & `instagram_profile_downloader-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="instagram_profile_downloader",
-    version="1.1.0",
+    version="1.1.1",
     author="Tadeas Fort",
     author_email="taddy.fort@gmail.com",
     description="A tool to download all images and videos and story highlights from an Instagram profile.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/tadeasf/instagram_profile_downloader",
     packages=find_packages(),
```

