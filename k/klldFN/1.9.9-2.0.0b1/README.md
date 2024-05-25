# Comparing `tmp/klldFN-1.9.9.tar.gz` & `tmp/klldFN-2.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "klldFN-1.9.9.tar", last modified: Sat May 25 10:53:02 2024, max compression
+gzip compressed data, was "klldFN-2.0.0b1.tar", last modified: Sat May 18 16:01:32 2024, max compression
```

## Comparing `klldFN-1.9.9.tar` & `klldFN-2.0.0b1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-25 10:53:02.184429 klldFN-1.9.9/
--rw-r--r--   0 runner    (1000) runner    (1000)     1086 2024-05-25 10:53:02.184429 klldFN-1.9.9/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)       62 2024-05-25 10:49:24.000000 klldFN-1.9.9/README.md
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-25 10:53:02.180429 klldFN-1.9.9/klldFN/
--rw-r--r--   0 runner    (1000) runner    (1000)   134530 2024-05-25 10:52:16.000000 klldFN-1.9.9/klldFN/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-25 10:53:02.184429 klldFN-1.9.9/klldFN.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     1086 2024-05-25 10:53:01.000000 klldFN-1.9.9/klldFN.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      201 2024-05-25 10:53:01.000000 klldFN-1.9.9/klldFN.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-05-25 10:53:01.000000 klldFN-1.9.9/klldFN.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)      109 2024-05-25 10:53:01.000000 klldFN-1.9.9/klldFN.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        7 2024-05-25 10:53:01.000000 klldFN-1.9.9/klldFN.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)      494 2024-04-12 16:24:13.000000 klldFN-1.9.9/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-05-25 10:53:02.184429 klldFN-1.9.9/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)     1282 2024-05-25 10:50:48.000000 klldFN-1.9.9/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-18 16:01:32.433221 klldFN-2.0.0b1/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1052 2024-05-18 16:01:32.433221 klldFN-2.0.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)       64 2024-05-18 12:28:14.000000 klldFN-2.0.0b1/README.md
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-18 16:01:32.425220 klldFN-2.0.0b1/klldFN/
+-rw-r--r--   0 runner    (1000) runner    (1000)   134565 2024-05-18 13:15:51.000000 klldFN-2.0.0b1/klldFN/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-18 16:01:32.429221 klldFN-2.0.0b1/klldFN.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1052 2024-05-18 16:01:32.000000 klldFN-2.0.0b1/klldFN.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      201 2024-05-18 16:01:32.000000 klldFN-2.0.0b1/klldFN.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-05-18 16:01:32.000000 klldFN-2.0.0b1/klldFN.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)      102 2024-05-18 16:01:32.000000 klldFN-2.0.0b1/klldFN.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        7 2024-05-18 16:01:32.000000 klldFN-2.0.0b1/klldFN.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)      494 2024-04-12 16:24:13.000000 klldFN-2.0.0b1/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-05-18 16:01:32.433221 klldFN-2.0.0b1/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)     1248 2024-05-18 15:56:57.000000 klldFN-2.0.0b1/setup.py
```

### Comparing `klldFN-1.9.9/PKG-INFO` & `klldFN-2.0.0b1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: klldFN
-Version: 1.9.9
+Version: 2.0.0b1
 Summary: klldFN
-Home-page: https://github.com/klldtest/klldFN
+Home-page: https://klldfn.xyz
 Author: klld
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -23,13 +23,12 @@
 Requires-Dist: FortniteAPIAsync==0.1.6
 Requires-Dist: sanic==20.12.0
 Requires-Dist: requests
 Requires-Dist: rich
 Requires-Dist: aiohttp
 Requires-Dist: asyncio
 Requires-Dist: requests
-Requires-Dist: jinja2
 
-# klldFN 2.0.0
+# klldFN 2.0.0b1
 **pip install klldFN**
 
 **pip3 install klldFN**
```

### Comparing `klldFN-1.9.9/klldFN/__init__.py` & `klldFN-2.0.0b1/klldFN/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
                 TextColumn("[bold blue]{task.description}", justify="right"),
                 BarColumn(bar_width=None),
                 SpinnerColumn(spinner_name="clock", style="bright_yellow", speed=1.0),
                 TimeElapsedColumn(),
             )        
     task1 = None
     with progress:
-                task1 = progress.add_task("[bold green]Starting klldFN 2.0.0...", total=3)
+                task1 = progress.add_task("[bold green]Starting klldFN 2.0.0b1...", total=3)
                 await asyncio.sleep(2)
                 progress.update(task1, advance=2, description="[bold green]Checking and updating package...")
                 await check_and_update_package()
                 await asyncio.sleep(1)
                 progress.update(task1, advance=1, description="[bold green]Updating translations...")
                 await UpdateTranslations()
 
@@ -254,15 +254,15 @@
                         icon=configuration.read()['banner']['bannerName'],
                         color=configuration.read()['banner']['bannerColor'],
                         season_level=configuration.read()['banner']['level']),
                 partial(client.party.me.set_backpack, asset=configuration.read()['cosmetics']['backpack']),
                 partial(client.party.me.set_pickaxe, asset=configuration.read()['cosmetics']['pickaxe']),
             )
         except Exception as e:
-            error_klldfn = translations.read()["translations"]["error-klldfn"][get_Language]
+            error_klldfn = translations.read()["translations"]["error-klldfn"][f"{get_Language}"]
             print(error_klldfn, e)
 
 
     @client.event
     async def event_party_member_promote(old_leader: fortnitepy.PartyMember, new_leader: fortnitepy.PartyMember):
      if new_leader.id == client.user.id:
         try:
@@ -349,15 +349,15 @@
 
 
 
     @client.event
     async def event_party_member_join(member: fortnitepy.PartyMember) -> None:
         await set_crowns()
         #await edit_and_keep_client_member()
-        member_join = translations.read()["translations"]["member-join"][get_Language]
+        member_join = translations.read()["translations"]["member-join"][f"{get_Language}"]
         await member.party.send(member_join.format(member.display_name))
 
 
     @client.command(
     name="skin",
     aliases=[
         'outfit',
@@ -885,16 +885,16 @@
       <div class="row mt-4">
         <div class="col-lg-7 mb-lg-0 mb-4">
           <div class="card">
             <div class="card-body p-3">
               <div class="row">
                 <div class="col-lg-6">
                   <div class="d-flex flex-column h-100">
-                    <h5 class="font-weight-bolder">klldFN 2.0.0</h5>
-                    <p class="mb-5">Launch version 2.0.0</p>
+                    <h5 class="font-weight-bolder">klldFN 2.0.0b1</h5>
+                    <p class="mb-5">Available now with enhancements and fixes</p>
                     <!--
                     <a class="text-body text-sm font-weight-bold mb-0 icon-move-right mt-auto" href="javascript:;">
                       Read More
                       <i class="fas fa-arrow-right text-sm ms-1" aria-hidden="true"></i>
                     </a>
                   -->
                   </div>
```

### Comparing `klldFN-1.9.9/klldFN.egg-info/PKG-INFO` & `klldFN-2.0.0b1/klldFN.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: klldFN
-Version: 1.9.9
+Version: 2.0.0b1
 Summary: klldFN
-Home-page: https://github.com/klldtest/klldFN
+Home-page: https://klldfn.xyz
 Author: klld
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -23,13 +23,12 @@
 Requires-Dist: FortniteAPIAsync==0.1.6
 Requires-Dist: sanic==20.12.0
 Requires-Dist: requests
 Requires-Dist: rich
 Requires-Dist: aiohttp
 Requires-Dist: asyncio
 Requires-Dist: requests
-Requires-Dist: jinja2
 
-# klldFN 2.0.0
+# klldFN 2.0.0b1
 **pip install klldFN**
 
 **pip3 install klldFN**
```

### Comparing `klldFN-1.9.9/setup.py` & `klldFN-2.0.0b1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="klldFN",
-    version="1.9.9",
+    version="2.0.0b1",
     author="klld",
     description="klldFN",
     long_description=long_description,
     python_requires='>=3.8.0',
     long_description_content_type="text/markdown",
-    url="https://github.com/klldtest/klldFN",
+    url="https://klldfn.xyz",
     packages=setuptools.find_packages(),
     classifiers=[
           'License :: OSI Approved :: MIT License',
           'Intended Audience :: Developers',
           'Natural Language :: English',
           'Operating System :: OS Independent',
           'Programming Language :: Python :: 3.8',
@@ -32,11 +32,10 @@
           'fortnitepy-edit',
           'FortniteAPIAsync==0.1.6',
           'sanic==20.12.0',
           'requests',
           'rich',
           'aiohttp',
           'asyncio',
-          'requests',
-          'jinja2'
+          'requests'
       ],
 )
```

