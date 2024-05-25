# Comparing `tmp/anipy_cli-3.0.5.tar.gz` & `tmp/anipy_cli-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anipy_cli-3.0.5.tar", max compression
+gzip compressed data, was "anipy_cli-3.1.0.tar", max compression
```

## Comparing `anipy_cli-3.0.5.tar` & `anipy_cli-3.1.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1974 2024-05-19 09:41:00.160333 anipy_cli-3.0.5/README.md
--rw-r--r--   0        0        0      855 2024-05-19 09:41:00.160333 anipy_cli-3.0.5/pyproject.toml
--rw-r--r--   0        0        0       48 2024-05-19 09:41:00.160333 anipy_cli-3.0.5/src/anipy_cli/__init__.py
--rw-r--r--   0        0        0     5299 2024-05-19 09:41:00.160333 anipy_cli-3.0.5/src/anipy_cli/arg_parser.py
--rw-r--r--   0        0        0     1922 2024-05-19 09:41:00.160333 anipy_cli-3.0.5/src/anipy_cli/cli.py
--rw-r--r--   0        0        0      411 2024-05-19 09:41:00.164333 anipy_cli-3.0.5/src/anipy_cli/clis/__init__.py
--rw-r--r--   0        0        0      609 2024-05-19 09:41:00.164333 anipy_cli-3.0.5/src/anipy_cli/clis/base_cli.py
--rw-r--r--   0        0        0     2281 2024-05-19 09:41:00.164333 anipy_cli-3.0.5/src/anipy_cli/clis/binge_cli.py
--rw-r--r--   0        0        0     2815 2024-05-19 09:41:00.164333 anipy_cli-3.0.5/src/anipy_cli/clis/default_cli.py
--rw-r--r--   0        0        0     3197 2024-05-19 09:41:00.164333 anipy_cli-3.0.5/src/anipy_cli/clis/download_cli.py
--rw-r--r--   0        0        0     2675 2024-05-19 09:41:00.164333 anipy_cli-3.0.5/src/anipy_cli/clis/history_cli.py
--rw-r--r--   0        0        0     2258 2024-05-19 09:41:00.164333 anipy_cli-3.0.5/src/anipy_cli/clis/mal_cli.py
--rw-r--r--   0        0        0      616 2024-05-19 09:41:00.164333 anipy_cli-3.0.5/src/anipy_cli/clis/seasonal_cli.py
--rw-r--r--   0        0        0      916 2024-05-19 09:41:00.164333 anipy_cli-3.0.5/src/anipy_cli/colors.py
--rw-r--r--   0        0        0    15404 2024-05-19 09:41:00.164333 anipy_cli-3.0.5/src/anipy_cli/config.py
--rw-r--r--   0        0        0     1160 2024-05-19 09:41:00.164333 anipy_cli-3.0.5/src/anipy_cli/discord.py
--rw-r--r--   0        0        0     6981 2024-05-19 09:41:00.164333 anipy_cli-3.0.5/src/anipy_cli/mal_proxy.py
--rw-r--r--   0        0        0      185 2024-05-19 09:41:00.164333 anipy_cli-3.0.5/src/anipy_cli/menus/__init__.py
--rw-r--r--   0        0        0     1140 2024-05-19 09:41:00.164333 anipy_cli-3.0.5/src/anipy_cli/menus/base_menu.py
--rw-r--r--   0        0        0    24077 2024-05-19 09:41:00.164333 anipy_cli-3.0.5/src/anipy_cli/menus/mal_menu.py
--rw-r--r--   0        0        0     6179 2024-05-19 09:41:00.164333 anipy_cli-3.0.5/src/anipy_cli/menus/menu.py
--rw-r--r--   0        0        0     9097 2024-05-19 09:41:00.164333 anipy_cli-3.0.5/src/anipy_cli/menus/seasonal_menu.py
--rw-r--r--   0        0        0     7119 2024-05-19 09:41:00.164333 anipy_cli-3.0.5/src/anipy_cli/prompts.py
--rw-r--r--   0        0        0     7684 2024-05-19 09:41:00.164333 anipy_cli-3.0.5/src/anipy_cli/util.py
--rw-r--r--   0        0        0     3084 1970-01-01 00:00:00.000000 anipy_cli-3.0.5/PKG-INFO
+-rw-r--r--   0        0        0     2308 2024-05-25 15:11:01.412294 anipy_cli-3.1.0/README.md
+-rw-r--r--   0        0        0      855 2024-05-25 15:11:59.031561 anipy_cli-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0       48 2024-05-25 15:11:59.038561 anipy_cli-3.1.0/src/anipy_cli/__init__.py
+-rw-r--r--   0        0        0     5299 2024-05-16 13:57:50.981018 anipy_cli-3.1.0/src/anipy_cli/arg_parser.py
+-rw-r--r--   0        0        0     1922 2024-05-16 13:57:50.981018 anipy_cli-3.1.0/src/anipy_cli/cli.py
+-rw-r--r--   0        0        0      411 2024-05-16 13:57:50.981018 anipy_cli-3.1.0/src/anipy_cli/clis/__init__.py
+-rw-r--r--   0        0        0      609 2024-05-16 13:57:50.981018 anipy_cli-3.1.0/src/anipy_cli/clis/base_cli.py
+-rw-r--r--   0        0        0     2281 2024-05-16 13:57:50.982018 anipy_cli-3.1.0/src/anipy_cli/clis/binge_cli.py
+-rw-r--r--   0        0        0     2815 2024-05-16 13:57:50.982018 anipy_cli-3.1.0/src/anipy_cli/clis/default_cli.py
+-rw-r--r--   0        0        0     3197 2024-05-16 13:57:50.982018 anipy_cli-3.1.0/src/anipy_cli/clis/download_cli.py
+-rw-r--r--   0        0        0     2675 2024-05-16 13:57:50.982018 anipy_cli-3.1.0/src/anipy_cli/clis/history_cli.py
+-rw-r--r--   0        0        0     2258 2024-05-16 13:57:50.982018 anipy_cli-3.1.0/src/anipy_cli/clis/mal_cli.py
+-rw-r--r--   0        0        0      616 2024-05-16 13:57:50.982018 anipy_cli-3.1.0/src/anipy_cli/clis/seasonal_cli.py
+-rw-r--r--   0        0        0      916 2024-05-16 13:57:50.982018 anipy_cli-3.1.0/src/anipy_cli/colors.py
+-rw-r--r--   0        0        0    15422 2024-05-25 14:53:26.203390 anipy_cli-3.1.0/src/anipy_cli/config.py
+-rw-r--r--   0        0        0     1160 2024-05-16 13:57:50.982018 anipy_cli-3.1.0/src/anipy_cli/discord.py
+-rw-r--r--   0        0        0     6981 2024-05-16 13:57:50.982018 anipy_cli-3.1.0/src/anipy_cli/mal_proxy.py
+-rw-r--r--   0        0        0      185 2024-05-16 13:57:50.982018 anipy_cli-3.1.0/src/anipy_cli/menus/__init__.py
+-rw-r--r--   0        0        0     1140 2024-05-16 13:57:50.982018 anipy_cli-3.1.0/src/anipy_cli/menus/base_menu.py
+-rw-r--r--   0        0        0    24077 2024-05-16 13:57:50.983018 anipy_cli-3.1.0/src/anipy_cli/menus/mal_menu.py
+-rw-r--r--   0        0        0     6179 2024-05-16 13:57:50.983018 anipy_cli-3.1.0/src/anipy_cli/menus/menu.py
+-rw-r--r--   0        0        0     9097 2024-05-16 13:57:50.983018 anipy_cli-3.1.0/src/anipy_cli/menus/seasonal_menu.py
+-rw-r--r--   0        0        0     7229 2024-05-25 14:53:26.203390 anipy_cli-3.1.0/src/anipy_cli/prompts.py
+-rw-r--r--   0        0        0     7684 2024-05-25 14:04:15.858789 anipy_cli-3.1.0/src/anipy_cli/util.py
+-rw-r--r--   0        0        0     3418 1970-01-01 00:00:00.000000 anipy_cli-3.1.0/PKG-INFO
```

### Comparing `anipy_cli-3.0.5/README.md` & `anipy_cli-3.1.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 # ANIPY-CLI
 **Anime from the comfort of your Terminal**
 
 <p align="center"><img src="https://github.com/sdaqo/anipy-cli/assets/63876564/1dafa5fb-4273-4dc1-a7ab-2664dd668fc9" /> </p>
 
-https://user-images.githubusercontent.com/63876564/162056019-ed0e7a60-78f6-4a2c-bc73-9be5dc2a4f07.mp4
-
-
 ## What even is this?
 A Little tool written in python to watch and download anime from the terminal (the better way to watch anime)
 This project's main aim is to create a enjoyable anime watching and downloading experience, directly in the terminal - your favorite place.
 
 Since the version 3 rewrite this project is split into api and frontend this makes it easy to integrate this into your project!
 
 ## You are just here for the client?
+<a href="https://pypi.org/project/anipy-cli/"><img alt="PyPI - Version" src="https://img.shields.io/pypi/v/anipy-cli?style=for-the-badge&logo=pypi&label=anipy-cli"></a>
+
 As one wise man once said:
 > I DONT GIVE A FUCK ABOUT THE FUCKING CODE! i just want to download this stupid fucking application and use it.
 >
 > WHY IS THERE CODE??? MAKE A FUCKING .EXE FILE AND GIVE IT TO ME. these dumbfucks think that everyone is a developer and understands code. well i am not and i don't understand it. I only know to download and install applications. SO WHY THE FUCK IS THERE CODE? make an EXE file and give it to me. STUPID FUCKING SMELLY NERDS
 
 <sub>Please do not take this seriously this is some stupid copypasta</sub>
 
 We do not have a .exe but we have pipx: `pipx install anipy-cli`
 
 Check out [Getting Started - CLI](https://sdaqo.github.io/anipy-cli/getting-started-cli) for better instructions and advice!
 
 ## You want to use the api for your project?
+<a href="https://pypi.org/project/anipy-api/"><img alt="PyPI - Version" src="https://img.shields.io/pypi/v/anipy-api?style=for-the-badge&logo=pypi&label=anipy-api"></a>
+
 Feel free to - please check out [Getting Started - API](https://sdaqo.github.io/anipy-cli/getting-started-api) for instructions
 
 
 ## :heart: Credits! 
 
 #### Heavily inspired by https://github.com/pystardust/ani-cli/
 
 #### All contributors for contributing
 
 <a href="https://github.com/sdaqo/anipy-cli/graphs/contributors">
     <img src="https://contrib.rocks/image?repo=sdaqo/anipy-cli" alt="anipy-cli contributors" title="anipy-cli contributors" width="800"/>
 </a>
+
+If you want to contribute as well check out this: https://sdaqo.github.io/anipy-cli/contributing
```

#### html2text {}

```diff
@@ -1,24 +1,24 @@
 # ANIPY-CLI **Anime from the comfort of your Terminal**
  [https://github.com/sdaqo/anipy-cli/assets/63876564/1dafa5fb-4273-4dc1-a7ab-
                                  2664dd668fc9]
-https://user-images.githubusercontent.com/63876564/162056019-ed0e7a60-78f6-
-4a2c-bc73-9be5dc2a4f07.mp4 ## What even is this? A Little tool written in
-python to watch and download anime from the terminal (the better way to watch
-anime) This project's main aim is to create a enjoyable anime watching and
-downloading experience, directly in the terminal - your favorite place. Since
-the version 3 rewrite this project is split into api and frontend this makes it
-easy to integrate this into your project! ## You are just here for the client?
-As one wise man once said: > I DONT GIVE A FUCK ABOUT THE FUCKING CODE! i just
-want to download this stupid fucking application and use it. > > WHY IS THERE
-CODE??? MAKE A FUCKING .EXE FILE AND GIVE IT TO ME. these dumbfucks think that
-everyone is a developer and understands code. well i am not and i don't
-understand it. I only know to download and install applications. SO WHY THE
-FUCK IS THERE CODE? make an EXE file and give it to me. STUPID FUCKING SMELLY
-NERDS Please do not take this seriously this is some stupid copypasta We do not
-have a .exe but we have pipx: `pipx install anipy-cli` Check out [Getting
-Started - CLI](https://sdaqo.github.io/anipy-cli/getting-started-cli) for
-better instructions and advice! ## You want to use the api for your project?
-Feel free to - please check out [Getting Started - API](https://
-sdaqo.github.io/anipy-cli/getting-started-api) for instructions ## :heart:
-Credits! #### Heavily inspired by https://github.com/pystardust/ani-cli/ ####
-All contributors for contributing_[_a_n_i_p_y_-_c_l_i_ _c_o_n_t_r_i_b_u_t_o_r_s_]
+## What even is this? A Little tool written in python to watch and download
+anime from the terminal (the better way to watch anime) This project's main aim
+is to create a enjoyable anime watching and downloading experience, directly in
+the terminal - your favorite place. Since the version 3 rewrite this project is
+split into api and frontend this makes it easy to integrate this into your
+project! ## You are just here for the client? _[_P_y_P_I_ _-_ _V_e_r_s_i_o_n_]As one wise man
+once said: > I DONT GIVE A FUCK ABOUT THE FUCKING CODE! i just want to download
+this stupid fucking application and use it. > > WHY IS THERE CODE??? MAKE A
+FUCKING .EXE FILE AND GIVE IT TO ME. these dumbfucks think that everyone is a
+developer and understands code. well i am not and i don't understand it. I only
+know to download and install applications. SO WHY THE FUCK IS THERE CODE? make
+an EXE file and give it to me. STUPID FUCKING SMELLY NERDS Please do not take
+this seriously this is some stupid copypasta We do not have a .exe but we have
+pipx: `pipx install anipy-cli` Check out [Getting Started - CLI](https://
+sdaqo.github.io/anipy-cli/getting-started-cli) for better instructions and
+advice! ## You want to use the api for your project? _[_P_y_P_I_ _-_ _V_e_r_s_i_o_n_]Feel free
+to - please check out [Getting Started - API](https://sdaqo.github.io/anipy-
+cli/getting-started-api) for instructions ## :heart: Credits! #### Heavily
+inspired by https://github.com/pystardust/ani-cli/ #### All contributors for
+contributing _[_a_n_i_p_y_-_c_l_i_ _c_o_n_t_r_i_b_u_t_o_r_s_]If you want to contribute as well check
+out this: https://sdaqo.github.io/anipy-cli/contributing
```

### Comparing `anipy_cli-3.0.5/pyproject.toml` & `anipy_cli-3.1.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "anipy-cli"
-version = "3.0.5"
+version = "3.1.0"
 description = "Watch and Download anime from the comfort of your Terminal"
 authors = ["sdaqo <sdaqo.dev@protonmail.com>"]
 license = "GPL-3.0"
 repository = "https://github.com/sdaqo/anipy-cli"
 homepage = "https://sdaqo.github.io/anipy-cli"
 documentation = "https://sdaqo.github.io/anipy-cli/getting-started-cli"
 keywords = ["anime", "cli"]
@@ -15,16 +15,16 @@
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pyyaml = "^6.0.1"
 yaspin = "^3.0.2"
 inquirerpy = "^0.3.4"
 appdirs = "^1.4.4"
-anipy-api = "^3.0.3"
 pypresence = "^4.3.0"
+anipy-api = "^3.1.0"
 
 [tool.poetry.scripts]
 anipy-cli = "anipy_cli.cli:run_cli"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/sdaqo/anipy-cli/issues"
```

### Comparing `anipy_cli-3.0.5/src/anipy_cli/arg_parser.py` & `anipy_cli-3.1.0/src/anipy_cli/arg_parser.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.0.5/src/anipy_cli/cli.py` & `anipy_cli-3.1.0/src/anipy_cli/cli.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.0.5/src/anipy_cli/clis/base_cli.py` & `anipy_cli-3.1.0/src/anipy_cli/clis/base_cli.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.0.5/src/anipy_cli/clis/binge_cli.py` & `anipy_cli-3.1.0/src/anipy_cli/clis/binge_cli.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.0.5/src/anipy_cli/clis/default_cli.py` & `anipy_cli-3.1.0/src/anipy_cli/clis/default_cli.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.0.5/src/anipy_cli/clis/download_cli.py` & `anipy_cli-3.1.0/src/anipy_cli/clis/download_cli.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.0.5/src/anipy_cli/clis/history_cli.py` & `anipy_cli-3.1.0/src/anipy_cli/clis/history_cli.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.0.5/src/anipy_cli/clis/mal_cli.py` & `anipy_cli-3.1.0/src/anipy_cli/clis/mal_cli.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.0.5/src/anipy_cli/clis/seasonal_cli.py` & `anipy_cli-3.1.0/src/anipy_cli/clis/seasonal_cli.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.0.5/src/anipy_cli/colors.py` & `anipy_cli-3.1.0/src/anipy_cli/colors.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.0.5/src/anipy_cli/config.py` & `anipy_cli-3.1.0/src/anipy_cli/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -68,31 +68,31 @@
         in different parts of the program. Configurable areas are as follows:
         default (and history), download (-D), seasonal (-S), binge (-B) and mal
         (-M) The example will show you how it is done! Please note that for seasonal
         search always the first provider that supports it is used.
 
         For an updated list of providers look here: https://sdaqo.github.io/anipy-cli/availabilty
 
-        Supported providers (as of $version): gogoanime
+        Supported providers (as of $version): gogoanime, yugenanime
 
         Examples:
             providers:
                 default: ["provider1"] # used in default mode and for the history
                 download: ["provider2"]
                 seasonal: ["provider3"]
                 binge: ["provider4"]
                 mal: ["provider2", "provider3"]
         """
         defaults = {
-            "default": ["gogoanime"],
-            "download": ["gogoanime"],
-            "history": ["gogoanime"],
-            "seasonal": ["gogoanime"],
-            "binge": ["gogoanime"],
-            "mal": ["gogoanime"],
+            "default": ["yugenanime"],
+            "download": ["yugenanime"],
+            "history": ["yugenanime"],
+            "seasonal": ["yugenanime"],
+            "binge": ["yugenanime"],
+            "mal": ["yugenanime"],
         }
 
         value = self._get_value("providers", defaults, dict)
 
         # Merge Dicts
         defaults.update(value)
         return defaults
```

### Comparing `anipy_cli-3.0.5/src/anipy_cli/discord.py` & `anipy_cli-3.1.0/src/anipy_cli/discord.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.0.5/src/anipy_cli/mal_proxy.py` & `anipy_cli-3.1.0/src/anipy_cli/mal_proxy.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.0.5/src/anipy_cli/menus/base_menu.py` & `anipy_cli-3.1.0/src/anipy_cli/menus/base_menu.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.0.5/src/anipy_cli/menus/mal_menu.py` & `anipy_cli-3.1.0/src/anipy_cli/menus/mal_menu.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.0.5/src/anipy_cli/menus/menu.py` & `anipy_cli-3.1.0/src/anipy_cli/menus/menu.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.0.5/src/anipy_cli/menus/seasonal_menu.py` & `anipy_cli-3.1.0/src/anipy_cli/menus/seasonal_menu.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.0.5/src/anipy_cli/prompts.py` & `anipy_cli-3.1.0/src/anipy_cli/prompts.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,15 +69,20 @@
         error("no search results")
         # Do not prompt for season again
         return search_show_prompt(mode, skip_season_search=True)
 
     anime = inquirer.fuzzy(  # type: ignore
         message="Select Show:",
         choices=results,
-        long_instruction="\nS = Anime is available in sub\nD = Anime is available in dub\nTo skip this prompt press ctrl+z",
+        long_instruction=(
+            "\nS = Anime is available in sub\n"
+            "D = Anime is available in dub\n"
+            "First two letters indicate the provider\n"
+            "To skip this prompt press ctrl+z"
+        ),
         mandatory=False,
     ).execute()
 
     return anime
 
 
 def season_search_prompt(provider: "BaseProvider") -> Optional["Anime"]:
```

### Comparing `anipy_cli-3.0.5/src/anipy_cli/util.py` & `anipy_cli-3.1.0/src/anipy_cli/util.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.0.5/PKG-INFO` & `anipy_cli-3.1.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: anipy-cli
-Version: 3.0.5
+Version: 3.1.0
 Summary: Watch and Download anime from the comfort of your Terminal
 Home-page: https://sdaqo.github.io/anipy-cli
 License: GPL-3.0
 Keywords: anime,cli
 Author: sdaqo
 Author-email: sdaqo.dev@protonmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: anipy-api (>=3.0.3,<4.0.0)
+Requires-Dist: anipy-api (>=3.1.0,<4.0.0)
 Requires-Dist: appdirs (>=1.4.4,<2.0.0)
 Requires-Dist: inquirerpy (>=0.3.4,<0.4.0)
 Requires-Dist: pypresence (>=4.3.0,<5.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: yaspin (>=3.0.2,<4.0.0)
 Project-URL: Bug Tracker, https://github.com/sdaqo/anipy-cli/issues
 Project-URL: Documentation, https://sdaqo.github.io/anipy-cli/getting-started-cli
@@ -26,42 +26,45 @@
 Description-Content-Type: text/markdown
 
 # ANIPY-CLI
 **Anime from the comfort of your Terminal**
 
 <p align="center"><img src="https://github.com/sdaqo/anipy-cli/assets/63876564/1dafa5fb-4273-4dc1-a7ab-2664dd668fc9" /> </p>
 
-https://user-images.githubusercontent.com/63876564/162056019-ed0e7a60-78f6-4a2c-bc73-9be5dc2a4f07.mp4
-
-
 ## What even is this?
 A Little tool written in python to watch and download anime from the terminal (the better way to watch anime)
 This project's main aim is to create a enjoyable anime watching and downloading experience, directly in the terminal - your favorite place.
 
 Since the version 3 rewrite this project is split into api and frontend this makes it easy to integrate this into your project!
 
 ## You are just here for the client?
+<a href="https://pypi.org/project/anipy-cli/"><img alt="PyPI - Version" src="https://img.shields.io/pypi/v/anipy-cli?style=for-the-badge&logo=pypi&label=anipy-cli"></a>
+
 As one wise man once said:
 > I DONT GIVE A FUCK ABOUT THE FUCKING CODE! i just want to download this stupid fucking application and use it.
 >
 > WHY IS THERE CODE??? MAKE A FUCKING .EXE FILE AND GIVE IT TO ME. these dumbfucks think that everyone is a developer and understands code. well i am not and i don't understand it. I only know to download and install applications. SO WHY THE FUCK IS THERE CODE? make an EXE file and give it to me. STUPID FUCKING SMELLY NERDS
 
 <sub>Please do not take this seriously this is some stupid copypasta</sub>
 
 We do not have a .exe but we have pipx: `pipx install anipy-cli`
 
 Check out [Getting Started - CLI](https://sdaqo.github.io/anipy-cli/getting-started-cli) for better instructions and advice!
 
 ## You want to use the api for your project?
+<a href="https://pypi.org/project/anipy-api/"><img alt="PyPI - Version" src="https://img.shields.io/pypi/v/anipy-api?style=for-the-badge&logo=pypi&label=anipy-api"></a>
+
 Feel free to - please check out [Getting Started - API](https://sdaqo.github.io/anipy-cli/getting-started-api) for instructions
 
 
 ## :heart: Credits! 
 
 #### Heavily inspired by https://github.com/pystardust/ani-cli/
 
 #### All contributors for contributing
 
 <a href="https://github.com/sdaqo/anipy-cli/graphs/contributors">
     <img src="https://contrib.rocks/image?repo=sdaqo/anipy-cli" alt="anipy-cli contributors" title="anipy-cli contributors" width="800"/>
 </a>
 
+If you want to contribute as well check out this: https://sdaqo.github.io/anipy-cli/contributing
+
```

#### html2text {}

```diff
@@ -1,39 +1,39 @@
-Metadata-Version: 2.1 Name: anipy-cli Version: 3.0.5 Summary: Watch and
+Metadata-Version: 2.1 Name: anipy-cli Version: 3.1.0 Summary: Watch and
 Download anime from the comfort of your Terminal Home-page: https://
 sdaqo.github.io/anipy-cli License: GPL-3.0 Keywords: anime,cli Author: sdaqo
 Author-email: sdaqo.dev@protonmail.com Requires-Python: >=3.9,<4.0 Classifier:
 License :: OSI Approved :: GNU General Public License v3 (GPLv3) Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
-Python :: 3.12 Requires-Dist: anipy-api (>=3.0.3,<4.0.0) Requires-Dist: appdirs
+Python :: 3.12 Requires-Dist: anipy-api (>=3.1.0,<4.0.0) Requires-Dist: appdirs
 (>=1.4.4,<2.0.0) Requires-Dist: inquirerpy (>=0.3.4,<0.4.0) Requires-Dist:
 pypresence (>=4.3.0,<5.0.0) Requires-Dist: pyyaml (>=6.0.1,<7.0.0) Requires-
 Dist: yaspin (>=3.0.2,<4.0.0) Project-URL: Bug Tracker, https://github.com/
 sdaqo/anipy-cli/issues Project-URL: Documentation, https://sdaqo.github.io/
 anipy-cli/getting-started-cli Project-URL: Repository, https://github.com/
 sdaqo/anipy-cli Description-Content-Type: text/markdown # ANIPY-CLI **Anime
 from the comfort of your Terminal**
  [https://github.com/sdaqo/anipy-cli/assets/63876564/1dafa5fb-4273-4dc1-a7ab-
                                  2664dd668fc9]
-https://user-images.githubusercontent.com/63876564/162056019-ed0e7a60-78f6-
-4a2c-bc73-9be5dc2a4f07.mp4 ## What even is this? A Little tool written in
-python to watch and download anime from the terminal (the better way to watch
-anime) This project's main aim is to create a enjoyable anime watching and
-downloading experience, directly in the terminal - your favorite place. Since
-the version 3 rewrite this project is split into api and frontend this makes it
-easy to integrate this into your project! ## You are just here for the client?
-As one wise man once said: > I DONT GIVE A FUCK ABOUT THE FUCKING CODE! i just
-want to download this stupid fucking application and use it. > > WHY IS THERE
-CODE??? MAKE A FUCKING .EXE FILE AND GIVE IT TO ME. these dumbfucks think that
-everyone is a developer and understands code. well i am not and i don't
-understand it. I only know to download and install applications. SO WHY THE
-FUCK IS THERE CODE? make an EXE file and give it to me. STUPID FUCKING SMELLY
-NERDS Please do not take this seriously this is some stupid copypasta We do not
-have a .exe but we have pipx: `pipx install anipy-cli` Check out [Getting
-Started - CLI](https://sdaqo.github.io/anipy-cli/getting-started-cli) for
-better instructions and advice! ## You want to use the api for your project?
-Feel free to - please check out [Getting Started - API](https://
-sdaqo.github.io/anipy-cli/getting-started-api) for instructions ## :heart:
-Credits! #### Heavily inspired by https://github.com/pystardust/ani-cli/ ####
-All contributors for contributing_[_a_n_i_p_y_-_c_l_i_ _c_o_n_t_r_i_b_u_t_o_r_s_]
+## What even is this? A Little tool written in python to watch and download
+anime from the terminal (the better way to watch anime) This project's main aim
+is to create a enjoyable anime watching and downloading experience, directly in
+the terminal - your favorite place. Since the version 3 rewrite this project is
+split into api and frontend this makes it easy to integrate this into your
+project! ## You are just here for the client? _[_P_y_P_I_ _-_ _V_e_r_s_i_o_n_]As one wise man
+once said: > I DONT GIVE A FUCK ABOUT THE FUCKING CODE! i just want to download
+this stupid fucking application and use it. > > WHY IS THERE CODE??? MAKE A
+FUCKING .EXE FILE AND GIVE IT TO ME. these dumbfucks think that everyone is a
+developer and understands code. well i am not and i don't understand it. I only
+know to download and install applications. SO WHY THE FUCK IS THERE CODE? make
+an EXE file and give it to me. STUPID FUCKING SMELLY NERDS Please do not take
+this seriously this is some stupid copypasta We do not have a .exe but we have
+pipx: `pipx install anipy-cli` Check out [Getting Started - CLI](https://
+sdaqo.github.io/anipy-cli/getting-started-cli) for better instructions and
+advice! ## You want to use the api for your project? _[_P_y_P_I_ _-_ _V_e_r_s_i_o_n_]Feel free
+to - please check out [Getting Started - API](https://sdaqo.github.io/anipy-
+cli/getting-started-api) for instructions ## :heart: Credits! #### Heavily
+inspired by https://github.com/pystardust/ani-cli/ #### All contributors for
+contributing _[_a_n_i_p_y_-_c_l_i_ _c_o_n_t_r_i_b_u_t_o_r_s_]If you want to contribute as well check
+out this: https://sdaqo.github.io/anipy-cli/contributing
```

