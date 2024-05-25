# Comparing `tmp/articraft-2.4.1.tar.gz` & `tmp/articraft-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "articraft-2.4.1.tar", last modified: Thu May 23 04:20:14 2024, max compression
+gzip compressed data, was "articraft-2.5.1.tar", last modified: Sat May 25 01:18:41 2024, max compression
```

## Comparing `articraft-2.4.1.tar` & `articraft-2.5.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-23 04:20:14.867571 articraft-2.4.1/
--rw-r--r--   0 kamangir   (502) staff       (20)     7048 2023-01-11 05:01:32.000000 articraft-2.4.1/LICENSE
--rw-r--r--   0 kamangir   (502) staff       (20)       24 2024-05-21 06:03:51.000000 articraft-2.4.1/MANIFEST.in
--rw-r--r--   0 kamangir   (502) staff       (20)     3596 2024-05-23 04:20:14.867223 articraft-2.4.1/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)     2682 2024-05-23 04:20:01.000000 articraft-2.4.1/README.md
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-23 04:20:14.863765 articraft-2.4.1/articraft/
--rw-r--r--   0 kamangir   (502) staff       (20)      100 2024-05-23 04:20:09.000000 articraft-2.4.1/articraft/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      252 2024-05-23 04:15:46.000000 articraft-2.4.1/articraft/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)       90 2024-05-23 04:15:48.000000 articraft-2.4.1/articraft/logger.py
--rw-r--r--   0 kamangir   (502) staff       (20)       17 2023-01-11 05:01:32.000000 articraft-2.4.1/articraft/urls.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-23 04:20:14.866724 articraft-2.4.1/articraft.egg-info/
--rw-r--r--   0 kamangir   (502) staff       (20)     3596 2024-05-23 04:20:14.000000 articraft-2.4.1/articraft.egg-info/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)      316 2024-05-23 04:20:14.000000 articraft-2.4.1/articraft.egg-info/SOURCES.txt
--rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-23 04:20:14.000000 articraft-2.4.1/articraft.egg-info/dependency_links.txt
--rw-r--r--   0 kamangir   (502) staff       (20)      156 2024-05-23 04:20:14.000000 articraft-2.4.1/articraft.egg-info/requires.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       10 2024-05-23 04:20:14.000000 articraft-2.4.1/articraft.egg-info/top_level.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       81 2024-05-21 06:03:51.000000 articraft-2.4.1/pyproject.toml
--rw-r--r--   0 kamangir   (502) staff       (20)      156 2024-05-21 06:04:42.000000 articraft-2.4.1/requirements.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-23 04:20:14.867703 articraft-2.4.1/setup.cfg
--rw-r--r--   0 kamangir   (502) staff       (20)      223 2024-05-23 04:15:33.000000 articraft-2.4.1/setup.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-25 01:18:41.753457 articraft-2.5.1/
+-rw-r--r--   0 kamangir   (502) staff       (20)     7048 2023-01-11 05:01:32.000000 articraft-2.5.1/LICENSE
+-rw-r--r--   0 kamangir   (502) staff       (20)       24 2024-05-21 06:03:51.000000 articraft-2.5.1/MANIFEST.in
+-rw-r--r--   0 kamangir   (502) staff       (20)     3670 2024-05-25 01:18:41.752547 articraft-2.5.1/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)     2756 2024-05-25 01:18:21.000000 articraft-2.5.1/README.md
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-25 01:18:41.746607 articraft-2.5.1/articraft/
+-rw-r--r--   0 kamangir   (502) staff       (20)      100 2024-05-25 01:18:33.000000 articraft-2.5.1/articraft/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      252 2024-05-23 04:15:46.000000 articraft-2.5.1/articraft/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       90 2024-05-23 04:15:48.000000 articraft-2.5.1/articraft/logger.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       17 2023-01-11 05:01:32.000000 articraft-2.5.1/articraft/urls.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-25 01:18:41.751518 articraft-2.5.1/articraft.egg-info/
+-rw-r--r--   0 kamangir   (502) staff       (20)     3670 2024-05-25 01:18:41.000000 articraft-2.5.1/articraft.egg-info/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)      316 2024-05-25 01:18:41.000000 articraft-2.5.1/articraft.egg-info/SOURCES.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-25 01:18:41.000000 articraft-2.5.1/articraft.egg-info/dependency_links.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)      156 2024-05-25 01:18:41.000000 articraft-2.5.1/articraft.egg-info/requires.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       10 2024-05-25 01:18:41.000000 articraft-2.5.1/articraft.egg-info/top_level.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       81 2024-05-21 06:03:51.000000 articraft-2.5.1/pyproject.toml
+-rw-r--r--   0 kamangir   (502) staff       (20)      156 2024-05-21 06:04:42.000000 articraft-2.5.1/requirements.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-25 01:18:41.753681 articraft-2.5.1/setup.cfg
+-rw-r--r--   0 kamangir   (502) staff       (20)      223 2024-05-23 04:15:33.000000 articraft-2.5.1/setup.py
```

### Comparing `articraft-2.4.1/LICENSE` & `articraft-2.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `articraft-2.4.1/PKG-INFO` & `articraft-2.5.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: articraft
-Version: 2.4.1
+Version: 2.5.1
 Summary: 🎨 tools for ai artists.
 Home-page: https://github.com/kamangir/aiart
 Author: Arash Abadpour (Kamangir)
 Author-email: arash@kamangir.net
 License: Public Domain
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Unix Shell
@@ -27,56 +27,56 @@
 Requires-Dist: pytest
 Requires-Dist: python-dotenv[cli]
 Requires-Dist: requests
 Requires-Dist: tqdm
 
 # aiart (articraft)
 
-🎨 `aiart` is an interface to [OpenAI](https://github.com/kamangir/openai_cli), [DALL-E](https://github.com/kamangir/openai_cli/blob/main/.abcli/DALLE.sh), and [Stable Diffusion](https://github.com/kamangir/blue-stability). AiArt can ingest [text and poetry](https://github.com/kamangir/aiart/blob/main/aiart/html/functions.py) from [allpoetry.com](https://allpoetry.com/), [medium](https://medium.com/), and [poetryfoundation.org](https://www.poetryfoundation.org/).
+🎨 `aiart` is an interface to [OpenAI commands](https://github.com/kamangir/openai-commands), [DALL-E](https://github.com/kamangir/openai-commands/blob/main/.abcli/DALLE.sh), and [Stable Diffusion](https://github.com/kamangir/blue-stability). AiArt can ingest [text and poetry](https://github.com/kamangir/aiart/blob/main/aiart/html/functions.py) from [allpoetry.com](https://allpoetry.com/), [medium](https://medium.com/), and [poetryfoundation.org](https://www.poetryfoundation.org/).
 
 🔷 [APIs](https://raw.githubusercontent.com/kamangir/aiart/main/APIs.yaml) 🔷
 
 ```bash
 abcli_quote <message>
  . urllib.parse.quote(<message>).
 abcli_unquote <message>
  . urllib.parse.unquote(<message>).
 aiart generate image \
-	[app=blue_stability|openai_cli,~dryrun,height=<576>,~sign,~tag,width=<768>] \
+	[app=blue_stability|openai_commands,~dryrun,height=<576>,~sign,~tag,width=<768>] \
 	[<image>] [<previous-image>] \
 	["<prompt>"] \
 	[-]
  . <prompt> -[<previous-image>]-> <image>.png.
 aiart generate video \
-	[app=blue_stability|openai_cli,~dryrun,frame_count=16,marker=PART,~publish,~render,resize_to=1280x1024,~sign,slice_by=words|sentences,~upload,url] \
+	[app=blue_stability|openai_commands,~dryrun,frame_count=16,marker=PART,~publish,~render,resize_to=1280x1024,~sign,slice_by=words|sentences,~upload,url] \
 	<filename.txt|url> \
 	[-]
  . <filename.txt>|url -> video.mp4
 aiart generate validate \
-	[app=blue_stability|openai_cli,dryrun,what=all|image|video]
+	[app=blue_stability|openai_commands,dryrun,what=all|image|video]
  . validate aiart.
 aiart html ingest_url \
 	<url> \
 	[--fake_agent 1] \
 	[--verbose 1]
  . ingest <url>.
 aiart publish \
-	[generator=blue_stability|DALL-E|openai_cli]
+	[generator=blue_stability|DALL-E|openai_commands]
  . publish 2024-05-22-07-37-34-67918.
 aiart transform \
 	[count=<1>,~dryrun,extension=jpg,~sign,~tag,~upload] \
 	[<object-name>] \
 	["<prompt>"] \
 	[-]
  . <object-name> -<prompt>-> 2024-05-22-07-37-34-67918.
 ```
 
-| [Stable Diffusion](https://github.com/kamangir/blue-stability)                                   | [OpenAI](https://github.com/kamangir/openai_cli)                                             |
-| ------------------------------------------------------------------------------------------------ | -------------------------------------------------------------------------------------------- |
-| ![image](https://raw.githubusercontent.com/kamangir/blue-stability/main/assets/carrot.png?raw=1) | ![image](https://raw.githubusercontent.com/kamangir/openai_cli/main/assets/carrot.png?raw=1) |
-| ![image](https://raw.githubusercontent.com/kamangir/blue-stability/main/assets/minds.gif?raw=1)  | ![image](https://raw.githubusercontent.com/kamangir/openai_cli/main/assets/minds.gif?raw=1)  |
-
-| [DALL-E](https://github.com/kamangir/openai_cli/blob/main/.abcli/DALLE.sh)        |
-| --------------------------------------------------------------------------------- |
-| ![image](https://github.com/kamangir/openai_cli/raw/main/assets/DALL-E.png?raw=1) |
+| [Stable Diffusion](https://github.com/kamangir/blue-stability)                                   | [OpenAI commands](https://github.com/kamangir/openai-commands)                                    |
+| ------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------- |
+| ![image](https://raw.githubusercontent.com/kamangir/blue-stability/main/assets/carrot.png?raw=1) | ![image](https://raw.githubusercontent.com/kamangir/openai-commands/main/assets/carrot.png?raw=1) |
+| ![image](https://raw.githubusercontent.com/kamangir/blue-stability/main/assets/minds.gif?raw=1)  | ![image](https://raw.githubusercontent.com/kamangir/openai-commands/main/assets/minds.gif?raw=1)  |
+
+| [DALL-E](https://github.com/kamangir/openai-commands/blob/main/.abcli/DALLE.sh)        |
+| -------------------------------------------------------------------------------------- |
+| ![image](https://github.com/kamangir/openai-commands/raw/main/assets/DALL-E.png?raw=1) |
 
 an [`awesome-bash-cli`](https://github.com/kamangir/awesome-bash-cli) (`abcli`) plugin.
```

### Comparing `articraft-2.4.1/README.md` & `articraft-2.5.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,51 +1,51 @@
 # aiart (articraft)
 
-🎨 `aiart` is an interface to [OpenAI](https://github.com/kamangir/openai_cli), [DALL-E](https://github.com/kamangir/openai_cli/blob/main/.abcli/DALLE.sh), and [Stable Diffusion](https://github.com/kamangir/blue-stability). AiArt can ingest [text and poetry](https://github.com/kamangir/aiart/blob/main/aiart/html/functions.py) from [allpoetry.com](https://allpoetry.com/), [medium](https://medium.com/), and [poetryfoundation.org](https://www.poetryfoundation.org/).
+🎨 `aiart` is an interface to [OpenAI commands](https://github.com/kamangir/openai-commands), [DALL-E](https://github.com/kamangir/openai-commands/blob/main/.abcli/DALLE.sh), and [Stable Diffusion](https://github.com/kamangir/blue-stability). AiArt can ingest [text and poetry](https://github.com/kamangir/aiart/blob/main/aiart/html/functions.py) from [allpoetry.com](https://allpoetry.com/), [medium](https://medium.com/), and [poetryfoundation.org](https://www.poetryfoundation.org/).
 
 🔷 [APIs](./APIs.yaml) 🔷
 
 ```bash
 abcli_quote <message>
  . urllib.parse.quote(<message>).
 abcli_unquote <message>
  . urllib.parse.unquote(<message>).
 aiart generate image \
-	[app=blue_stability|openai_cli,~dryrun,height=<576>,~sign,~tag,width=<768>] \
+	[app=blue_stability|openai_commands,~dryrun,height=<576>,~sign,~tag,width=<768>] \
 	[<image>] [<previous-image>] \
 	["<prompt>"] \
 	[-]
  . <prompt> -[<previous-image>]-> <image>.png.
 aiart generate video \
-	[app=blue_stability|openai_cli,~dryrun,frame_count=16,marker=PART,~publish,~render,resize_to=1280x1024,~sign,slice_by=words|sentences,~upload,url] \
+	[app=blue_stability|openai_commands,~dryrun,frame_count=16,marker=PART,~publish,~render,resize_to=1280x1024,~sign,slice_by=words|sentences,~upload,url] \
 	<filename.txt|url> \
 	[-]
  . <filename.txt>|url -> video.mp4
 aiart generate validate \
-	[app=blue_stability|openai_cli,dryrun,what=all|image|video]
+	[app=blue_stability|openai_commands,dryrun,what=all|image|video]
  . validate aiart.
 aiart html ingest_url \
 	<url> \
 	[--fake_agent 1] \
 	[--verbose 1]
  . ingest <url>.
 aiart publish \
-	[generator=blue_stability|DALL-E|openai_cli]
+	[generator=blue_stability|DALL-E|openai_commands]
  . publish 2024-05-22-07-37-34-67918.
 aiart transform \
 	[count=<1>,~dryrun,extension=jpg,~sign,~tag,~upload] \
 	[<object-name>] \
 	["<prompt>"] \
 	[-]
  . <object-name> -<prompt>-> 2024-05-22-07-37-34-67918.
 ```
 
-| [Stable Diffusion](https://github.com/kamangir/blue-stability)                                   | [OpenAI](https://github.com/kamangir/openai_cli)                                             |
-| ------------------------------------------------------------------------------------------------ | -------------------------------------------------------------------------------------------- |
-| ![image](https://raw.githubusercontent.com/kamangir/blue-stability/main/assets/carrot.png?raw=1) | ![image](https://raw.githubusercontent.com/kamangir/openai_cli/main/assets/carrot.png?raw=1) |
-| ![image](https://raw.githubusercontent.com/kamangir/blue-stability/main/assets/minds.gif?raw=1)  | ![image](https://raw.githubusercontent.com/kamangir/openai_cli/main/assets/minds.gif?raw=1)  |
-
-| [DALL-E](https://github.com/kamangir/openai_cli/blob/main/.abcli/DALLE.sh)        |
-| --------------------------------------------------------------------------------- |
-| ![image](https://github.com/kamangir/openai_cli/raw/main/assets/DALL-E.png?raw=1) |
+| [Stable Diffusion](https://github.com/kamangir/blue-stability)                                   | [OpenAI commands](https://github.com/kamangir/openai-commands)                                    |
+| ------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------- |
+| ![image](https://raw.githubusercontent.com/kamangir/blue-stability/main/assets/carrot.png?raw=1) | ![image](https://raw.githubusercontent.com/kamangir/openai-commands/main/assets/carrot.png?raw=1) |
+| ![image](https://raw.githubusercontent.com/kamangir/blue-stability/main/assets/minds.gif?raw=1)  | ![image](https://raw.githubusercontent.com/kamangir/openai-commands/main/assets/minds.gif?raw=1)  |
+
+| [DALL-E](https://github.com/kamangir/openai-commands/blob/main/.abcli/DALLE.sh)        |
+| -------------------------------------------------------------------------------------- |
+| ![image](https://github.com/kamangir/openai-commands/raw/main/assets/DALL-E.png?raw=1) |
 
 an [`awesome-bash-cli`](https://github.com/kamangir/awesome-bash-cli) (`abcli`) plugin.
```

### Comparing `articraft-2.4.1/articraft.egg-info/PKG-INFO` & `articraft-2.5.1/articraft.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: articraft
-Version: 2.4.1
+Version: 2.5.1
 Summary: 🎨 tools for ai artists.
 Home-page: https://github.com/kamangir/aiart
 Author: Arash Abadpour (Kamangir)
 Author-email: arash@kamangir.net
 License: Public Domain
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Unix Shell
@@ -27,56 +27,56 @@
 Requires-Dist: pytest
 Requires-Dist: python-dotenv[cli]
 Requires-Dist: requests
 Requires-Dist: tqdm
 
 # aiart (articraft)
 
-🎨 `aiart` is an interface to [OpenAI](https://github.com/kamangir/openai_cli), [DALL-E](https://github.com/kamangir/openai_cli/blob/main/.abcli/DALLE.sh), and [Stable Diffusion](https://github.com/kamangir/blue-stability). AiArt can ingest [text and poetry](https://github.com/kamangir/aiart/blob/main/aiart/html/functions.py) from [allpoetry.com](https://allpoetry.com/), [medium](https://medium.com/), and [poetryfoundation.org](https://www.poetryfoundation.org/).
+🎨 `aiart` is an interface to [OpenAI commands](https://github.com/kamangir/openai-commands), [DALL-E](https://github.com/kamangir/openai-commands/blob/main/.abcli/DALLE.sh), and [Stable Diffusion](https://github.com/kamangir/blue-stability). AiArt can ingest [text and poetry](https://github.com/kamangir/aiart/blob/main/aiart/html/functions.py) from [allpoetry.com](https://allpoetry.com/), [medium](https://medium.com/), and [poetryfoundation.org](https://www.poetryfoundation.org/).
 
 🔷 [APIs](https://raw.githubusercontent.com/kamangir/aiart/main/APIs.yaml) 🔷
 
 ```bash
 abcli_quote <message>
  . urllib.parse.quote(<message>).
 abcli_unquote <message>
  . urllib.parse.unquote(<message>).
 aiart generate image \
-	[app=blue_stability|openai_cli,~dryrun,height=<576>,~sign,~tag,width=<768>] \
+	[app=blue_stability|openai_commands,~dryrun,height=<576>,~sign,~tag,width=<768>] \
 	[<image>] [<previous-image>] \
 	["<prompt>"] \
 	[-]
  . <prompt> -[<previous-image>]-> <image>.png.
 aiart generate video \
-	[app=blue_stability|openai_cli,~dryrun,frame_count=16,marker=PART,~publish,~render,resize_to=1280x1024,~sign,slice_by=words|sentences,~upload,url] \
+	[app=blue_stability|openai_commands,~dryrun,frame_count=16,marker=PART,~publish,~render,resize_to=1280x1024,~sign,slice_by=words|sentences,~upload,url] \
 	<filename.txt|url> \
 	[-]
  . <filename.txt>|url -> video.mp4
 aiart generate validate \
-	[app=blue_stability|openai_cli,dryrun,what=all|image|video]
+	[app=blue_stability|openai_commands,dryrun,what=all|image|video]
  . validate aiart.
 aiart html ingest_url \
 	<url> \
 	[--fake_agent 1] \
 	[--verbose 1]
  . ingest <url>.
 aiart publish \
-	[generator=blue_stability|DALL-E|openai_cli]
+	[generator=blue_stability|DALL-E|openai_commands]
  . publish 2024-05-22-07-37-34-67918.
 aiart transform \
 	[count=<1>,~dryrun,extension=jpg,~sign,~tag,~upload] \
 	[<object-name>] \
 	["<prompt>"] \
 	[-]
  . <object-name> -<prompt>-> 2024-05-22-07-37-34-67918.
 ```
 
-| [Stable Diffusion](https://github.com/kamangir/blue-stability)                                   | [OpenAI](https://github.com/kamangir/openai_cli)                                             |
-| ------------------------------------------------------------------------------------------------ | -------------------------------------------------------------------------------------------- |
-| ![image](https://raw.githubusercontent.com/kamangir/blue-stability/main/assets/carrot.png?raw=1) | ![image](https://raw.githubusercontent.com/kamangir/openai_cli/main/assets/carrot.png?raw=1) |
-| ![image](https://raw.githubusercontent.com/kamangir/blue-stability/main/assets/minds.gif?raw=1)  | ![image](https://raw.githubusercontent.com/kamangir/openai_cli/main/assets/minds.gif?raw=1)  |
-
-| [DALL-E](https://github.com/kamangir/openai_cli/blob/main/.abcli/DALLE.sh)        |
-| --------------------------------------------------------------------------------- |
-| ![image](https://github.com/kamangir/openai_cli/raw/main/assets/DALL-E.png?raw=1) |
+| [Stable Diffusion](https://github.com/kamangir/blue-stability)                                   | [OpenAI commands](https://github.com/kamangir/openai-commands)                                    |
+| ------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------- |
+| ![image](https://raw.githubusercontent.com/kamangir/blue-stability/main/assets/carrot.png?raw=1) | ![image](https://raw.githubusercontent.com/kamangir/openai-commands/main/assets/carrot.png?raw=1) |
+| ![image](https://raw.githubusercontent.com/kamangir/blue-stability/main/assets/minds.gif?raw=1)  | ![image](https://raw.githubusercontent.com/kamangir/openai-commands/main/assets/minds.gif?raw=1)  |
+
+| [DALL-E](https://github.com/kamangir/openai-commands/blob/main/.abcli/DALLE.sh)        |
+| -------------------------------------------------------------------------------------- |
+| ![image](https://github.com/kamangir/openai-commands/raw/main/assets/DALL-E.png?raw=1) |
 
 an [`awesome-bash-cli`](https://github.com/kamangir/awesome-bash-cli) (`abcli`) plugin.
```

