# Comparing `tmp/soundbook-0.0.1.tar.gz` & `tmp/soundbook-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soundbook-0.0.1.tar", last modified: Fri May 17 04:23:51 2024, max compression
+gzip compressed data, was "soundbook-0.0.2.tar", last modified: Sat May 25 05:54:51 2024, max compression
```

## Comparing `soundbook-0.0.1.tar` & `soundbook-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 04:23:51.867999 soundbook-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-17 04:23:47.000000 soundbook-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-05-17 04:23:51.867999 soundbook-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-05-17 04:23:47.000000 soundbook-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 04:23:51.867999 soundbook-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-17 04:23:47.000000 soundbook-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 04:23:51.863999 soundbook-0.0.1/soundbook/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-17 04:23:47.000000 soundbook-0.0.1/soundbook/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 04:23:51.867999 soundbook-0.0.1/soundbook/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 04:23:47.000000 soundbook-0.0.1/soundbook/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-17 04:23:47.000000 soundbook-0.0.1/soundbook/core/handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-17 04:23:47.000000 soundbook-0.0.1/soundbook/core/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 04:23:51.867999 soundbook-0.0.1/soundbook/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 04:23:47.000000 soundbook-0.0.1/soundbook/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-17 04:23:47.000000 soundbook-0.0.1/soundbook/modules/get_book.py
--rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-05-17 04:23:47.000000 soundbook-0.0.1/soundbook/modules/get_url.py
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-17 04:23:47.000000 soundbook-0.0.1/soundbook/soundbook.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 04:23:51.867999 soundbook-0.0.1/soundbook.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-05-17 04:23:51.000000 soundbook-0.0.1/soundbook.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-17 04:23:51.000000 soundbook-0.0.1/soundbook.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 04:23:51.000000 soundbook-0.0.1/soundbook.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-17 04:23:51.000000 soundbook-0.0.1/soundbook.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-17 04:23:51.000000 soundbook-0.0.1/soundbook.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-17 04:23:51.000000 soundbook-0.0.1/soundbook.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 05:54:51.027759 soundbook-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-25 05:54:47.000000 soundbook-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-05-25 05:54:51.027759 soundbook-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-25 05:54:47.000000 soundbook-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 05:54:51.027759 soundbook-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-25 05:54:47.000000 soundbook-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 05:54:51.027759 soundbook-0.0.2/soundbook/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-25 05:54:47.000000 soundbook-0.0.2/soundbook/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 05:54:51.027759 soundbook-0.0.2/soundbook/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 05:54:47.000000 soundbook-0.0.2/soundbook/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-25 05:54:47.000000 soundbook-0.0.2/soundbook/core/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-25 05:54:47.000000 soundbook-0.0.2/soundbook/core/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 05:54:51.027759 soundbook-0.0.2/soundbook/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 05:54:47.000000 soundbook-0.0.2/soundbook/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-25 05:54:47.000000 soundbook-0.0.2/soundbook/modules/get_book.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-05-25 05:54:47.000000 soundbook-0.0.2/soundbook/modules/get_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-25 05:54:47.000000 soundbook-0.0.2/soundbook/soundbook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 05:54:51.027759 soundbook-0.0.2/soundbook.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-05-25 05:54:51.000000 soundbook-0.0.2/soundbook.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-25 05:54:51.000000 soundbook-0.0.2/soundbook.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 05:54:51.000000 soundbook-0.0.2/soundbook.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-25 05:54:51.000000 soundbook-0.0.2/soundbook.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-25 05:54:51.000000 soundbook-0.0.2/soundbook.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-25 05:54:51.000000 soundbook-0.0.2/soundbook.egg-info/top_level.txt
```

### Comparing `soundbook-0.0.1/LICENSE` & `soundbook-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `soundbook-0.0.1/PKG-INFO` & `soundbook-0.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soundbook
-Version: 0.0.1
+Version: 0.0.2
 Summary: search, download, and merge audiobooks
 Home-page: https://erfansamandarian.com/soundbook
 Author: Erfan Samandarian
 Author-email: mail@erfansamandarian.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -61,27 +61,33 @@
 
 ### by url 
 
 ```
 soundbook --url "https://<website>.com/<book>/"
 ```
 
+### by url 
+
+```
+soundbook --url "https://<website>.com/<book>/" --title "book title" --author "book author"
+```
+
 ### example
 
 ```
 soundbook --url "https://appaudiobooks.com/the-fountainhead-audiobook/"
 ```
 
 do not pirate, pirating is bad, paying money for dead people's ip is good, believe in the system, the system is always right
 
 ### by search
 
 <b>coming soon</b>
 
-requests.json() not working for these shitty websites
+requests.json() not working for these websites
 
 i get 403 when i try to connect, even with the correct headers
 
 anyone know how to do it? if so, submit a pull request
 
 ## contemplation / todo
```

### Comparing `soundbook-0.0.1/README.md` & `soundbook-0.0.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -42,34 +42,40 @@
 
 ### by url 
 
 ```
 soundbook --url "https://<website>.com/<book>/"
 ```
 
+### by url 
+
+```
+soundbook --url "https://<website>.com/<book>/" --title "book title" --author "book author"
+```
+
 ### example
 
 ```
 soundbook --url "https://appaudiobooks.com/the-fountainhead-audiobook/"
 ```
 
 do not pirate, pirating is bad, paying money for dead people's ip is good, believe in the system, the system is always right
 
 ### by search
 
 <b>coming soon</b>
 
-requests.json() not working for these shitty websites
+requests.json() not working for these websites
 
 i get 403 when i try to connect, even with the correct headers
 
 anyone know how to do it? if so, submit a pull request
 
 ## contemplation / todo
 
 what is fountainhead about? is it worth reading / listening to
 
 is making a gui worth it?
 
 need to make ffmpeg work on systems other than m-series mac
 
-what happens if the book doesn't have a cover image?
+what happens if the book doesn't have a cover image?
```

### Comparing `soundbook-0.0.1/setup.py` & `soundbook-0.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,13 +9,13 @@
     description="search, download, and merge audiobooks",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Erfan Samandarian",
     author_email="mail@erfansamandarian.com",
     url="https://erfansamandarian.com/soundbook",
     license="MIT",
-    version="0.0.1",
+    version="0.0.2",
     packages=find_packages(),
     install_requires=["setuptools", "ffmpeg", "mutagen", "eyed3", "pillow", "requests", "sox", "yt_dlp"],
     py_modules=["soundbook"],
     entry_points={"console_scripts": ["soundbook=soundbook:main"]},
 )
```

### Comparing `soundbook-0.0.1/soundbook/modules/get_url.py` & `soundbook-0.0.2/soundbook/modules/get_url.py`

 * *Files 15% similar despite different names*

```diff
@@ -64,31 +64,35 @@
             im = Image.open(BytesIO(pic))
             title = tags.get("TIT2").text[0] if tags.get("TIT2") else "unknown"
             title = title.replace("-", "/")
             cover_image_path = os.path.join(dir_path, f"{title}_cover.jpg")
             im.save(cover_image_path)
 
 
-def add_cover_image(directory, title):
+def add_cover_image(directory, title, book_title, book_author):
     title = title + ".m4b"
     dir_path = f"downloads/{directory}"
     full_path_to_file = os.path.join(dir_path, title)
     image_files = glob.glob(os.path.join(dir_path, "*.jpg"))
     if image_files:
         cover_img = image_files[0]
         if os.path.isfile(cover_img):
             audio = MP4(full_path_to_file)
             cover_image = open(cover_img, "rb").read()
             audio["covr"] = [MP4Cover(cover_image)]
+            if book_title is not None:
+                audio["\xa9nam"] = [book_title]
+            if book_author is not None:
+                audio["\xa9ART"] = [book_author]
             audio.save()
             os.remove(cover_img)
         else:
             print(f"Cover image {cover_img} not found")
 
 
-def get_url(url):
+def get_url(url, book_title, book_author):
     directory = get_title(url)
     make_folder(directory)
     title = extract_audio(url, directory)
     get_cover_image(directory)
     merge_audio(directory)
-    add_cover_image(directory, title)
+    add_cover_image(directory, title, book_title, book_author)
```

### Comparing `soundbook-0.0.1/soundbook.egg-info/PKG-INFO` & `soundbook-0.0.2/soundbook.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soundbook
-Version: 0.0.1
+Version: 0.0.2
 Summary: search, download, and merge audiobooks
 Home-page: https://erfansamandarian.com/soundbook
 Author: Erfan Samandarian
 Author-email: mail@erfansamandarian.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -61,27 +61,33 @@
 
 ### by url 
 
 ```
 soundbook --url "https://<website>.com/<book>/"
 ```
 
+### by url 
+
+```
+soundbook --url "https://<website>.com/<book>/" --title "book title" --author "book author"
+```
+
 ### example
 
 ```
 soundbook --url "https://appaudiobooks.com/the-fountainhead-audiobook/"
 ```
 
 do not pirate, pirating is bad, paying money for dead people's ip is good, believe in the system, the system is always right
 
 ### by search
 
 <b>coming soon</b>
 
-requests.json() not working for these shitty websites
+requests.json() not working for these websites
 
 i get 403 when i try to connect, even with the correct headers
 
 anyone know how to do it? if so, submit a pull request
 
 ## contemplation / todo
```

