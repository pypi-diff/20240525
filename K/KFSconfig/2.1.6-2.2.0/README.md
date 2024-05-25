# Comparing `tmp/kfsconfig-2.1.6.tar.gz` & `tmp/kfsconfig-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kfsconfig-2.1.6.tar", max compression
+gzip compressed data, was "kfsconfig-2.2.0.tar", max compression
```

## Comparing `kfsconfig-2.1.6.tar` & `kfsconfig-2.2.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0    17060 2024-05-12 11:27:16.921288 kfsconfig-2.1.6/KFSconfig/KFSconfig.py
--rw-r--r--   0        0        0      514 2024-05-12 11:27:16.921288 kfsconfig-2.1.6/pyproject.toml
--rw-r--r--   0        0        0      668 2024-05-12 11:27:16.921288 kfsconfig-2.1.6/readme.md
--rw-r--r--   0        0        0     1185 1970-01-01 00:00:00.000000 kfsconfig-2.1.6/PKG-INFO
+-rw-r--r--   0        0        0    18513 2024-05-25 17:23:30.335016 kfsconfig-2.2.0/KFSconfig/KFSconfig.py
+-rw-r--r--   0        0        0      514 2024-05-25 17:23:30.335016 kfsconfig-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0      668 2024-05-25 17:23:30.335016 kfsconfig-2.2.0/readme.md
+-rw-r--r--   0        0        0     1185 1970-01-01 00:00:00.000000 kfsconfig-2.2.0/PKG-INFO
```

### Comparing `kfsconfig-2.1.6/KFSconfig/KFSconfig.py` & `kfsconfig-2.2.0/KFSconfig/KFSconfig.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,84 +25,89 @@
     - ValueError: user input is not in input_allowed and tries_max has been exhausted
     """
 
     input_allowed_matched: str  # entry from inputs_allowed that matched user input
     logger: logging.Logger      # logger
     try_current: int=0          # try current
     user_input: str             # user input
-    
+
 
     if 1<=len(logging.getLogger("").handlers):  # if root logger defined handlers:
         logger=logging.getLogger("")            # also use root logger to match formats defined outside KFS
     else:                                       # if no root logger defined:
         logger=KFSlog.setup_logging("KFS")      # use KFS default format
 
 
     while try_current!=tries_max:   # as long as tries not exhausted: prompt for input
         try_current+=1              # increment try_current
         logger.info(prompt)         # prompt user for input
         user_input=input()          # get user input
-        
+
         if user_input in inputs_allowed:                                                                                                # try to find match case-sensitive and prefer that
             input_allowed_matched=user_input
             break
         elif match_case_sensitive==False and user_input.casefold() in [input_allowed.casefold() for input_allowed in inputs_allowed]:   # if no match case-sensitive found and match case-insensitive allowed: fallback to try to find match case-insensitive
             input_allowed_matched=next(input_allowed for input_allowed in inputs_allowed if input_allowed.casefold()==user_input.casefold())
             break
-            
+
         if try_current!=tries_max:  # if no match and not last try: try again
             logger.warning(f"Input \"{user_input}\" is invalid. Trying again...")
             continue
         else:                       # if no match and last try: error
             logger.error(f"Input \"{user_input}\" is invalid. Giving up.")
             raise ValueError(f"Error in {force_input.__name__}{inspect.signature(force_input)}: Input \"{user_input}\" is invalid. Giving up.")
-        
+
     return input_allowed_matched
 
 
 def load_config(env: bool=True, config_filepaths: list[str]|None=["./.env", "./config/config.json"], config_default: dict[str, typing.Any]={}, setting_None_ok: bool=False) -> dict[str, typing.Any]:
     """
     Tries to load config with the name of the config_default's keys. Multiple sources can be used and will be prioritised accordingly:
     1. if env is True: passed environemental variables from os.environ
     2. if config_filepath is not None: config from file at filepath with decreasing priority
+    
     If any setting is still None after all sources have been tried and setting_None_ok is false, it is considered undefined and a ValueError is raised.
     If any setting is undefined and none of the enabled filepaths exist, creation of a default config file at the highest priority filepath will be offered using config_default's values.
+    Depending on the file extension, the loaded data is stored differently, either using the whole dictionary or only using key "content". See argument config_default for details, same rules apply.
 
     Arguments:
-    - config_default: defaults to use for creation of a default config file, unformatted file formats like .txt require key "content"
+    - config_default: defaults to use for creation of a default config file, depending on file extension interpreted differently:
+        - .env: whole dictionary is used
+        - .json: whole dictionary is used unless only key "content" is present, then only its value is used. This makes it possible to support other top level json data types than dict.
+        - default: only key "content"'s raw value is used, all other keys are ignored
     - env: use passed environmental variables from os.environ?
     - config_filepath: filepath to config files or None if unused, formats depending on file extension, unformatted formats like .txt save raw string content from file in key "content"
     - setting_None_ok: allow settings to be None or require to be set?
 
     Returns:
     - config: loaded config, same keys as config_default
 
     Raises:
     - KeyError: config_default is missing key "content" while trying to save raw string content
     - ValueError: After going through all enabled sources, a setting is still None and setting_None_ok is false.
     """
 
     config: dict[str, typing.Any]={key: None for key in config_default.keys()}  # loaded config, initialised empty with same keys as config_default
     sources_loaded: list[str]=[]                                                # sources loaded successfully
-    
+
 
     if 1<=len(logging.getLogger("").handlers):  # if root logger defined handlers:
         logger=logging.getLogger("")            # also use root logger to match formats defined outside KFS
     else:                                       # if no root logger defined:
         logger=KFSlog.setup_logging("KFS")      # use KFS default format
 
     if env==False and (config_filepaths==None or len(config_filepaths)==0): # if no source enabled: error
         logger.error(f"No config source is enabled. Loading config is impossible.")
         raise ValueError(f"Error in {load_config.__name__}{inspect.signature(load_config)}: No config source is enabled. Loading config is impossible.")
 
 
     if env==True:
         config.update({k: v for k, v in _load_env().items() if k in config.keys() and config[k]==None}) # update config with environmental variables, only overwrite if key already exists and value is None
         sources_loaded.append("environmental variables")                                                # log success
-    
+
     if config_filepaths!=None and len(config_filepaths)!=0:
         for config_filepath in config_filepaths:
             try:
                 config.update({k: v for k, v in _load_config_file(config_filepath).items() if k in config.keys() and config[k]==None})  # update config with config file, only overwrite if key already exists and value is None
             except (FileNotFoundError, IsADirectoryError, OSError):                                                                     # if fails: ignore source
                 pass
             else:
@@ -110,15 +115,15 @@
     if 1<=len(sources_loaded):  # if source loaded: log
         logger.info(f"Loaded config from: {", ".join(sources_loaded)}")
     logger.debug(config)
 
 
     if any(v==None for v in config.values())==True and setting_None_ok==False:                                                                                  # if any setting is still None and not allowed to be None: error
         logger.error(f"After going through all enabled sources, settings {[k for k, v in config.items() if v==None]} are still None and setting_None_ok is false.")
-        
+
         if config_filepaths!=None and 1<=len(config_filepaths) and all([os.path.exists(config_filepath)==False for config_filepath in config_filepaths])==True: # if a file source is enabled and no files at set filepaths exist: offer creation of default config file at highest priority filepath using config_default's values
             match force_input(f"Would you like to create a default \"{config_filepaths[0]}\"? (y/n)"):
                 case "y":
                     try:
                         _create_default_file(config_filepaths[0], config_default)                                                                               # create default config file at highest priority filepath using config_default's values
                     except OSError:                                                                                                                             # if creating fails: error, if file already exists error because it should have been checked before
                         pass
@@ -191,29 +196,31 @@
     try:
         with open(config_filepath, "rt", encoding="utf8") as config_file:                                                                                                               # read file
             match os.path.basename(config_filepath).rsplit(".", 1)[-1]:                                                                                                                 # parse file content
                 case "env":
                     config={line.strip(" ").split("=")[0]: line.strip(" ").split("=")[1] for line in config_file.readlines() if "=" in line and line.strip(" ").startswith("#")==False} # parse env
                 case "json":
                     config=json.loads(config_file.read())                                                                                                                               # parse json
+                    if type(config)!=dict:                                                                                                                                              # if json is not dict:
+                        config={"content": config}                                                                                                                                      # wrap in dict to match other formats
                 case "token" | "txt":
                     config={"content": config_file.read()}                                                                                                                              # parse raw string
                 case _:
                     defaulted=True                                                                                                                                                      # defaulted to forwarding raw string content
                     config={"content": config_file.read()}                                                                                                                              # parse raw string
     except OSError as e:                                                                                                                                                                # write to log, then forward exception
         logger.warning(f"\rLoading \"{config_filepath}\" failed with {KFSfstr.full_class_name(e)}. Source will be skipped.")
         raise
     else:
         if defaulted==False:
             logger.debug(f"\rLoaded \"{config_filepath}\".")
         else:                   # if defaulted to forwarding raw string content: warn
             logger.warning(f"\rLoaded \"{config_filepath}\", but custom behaviour for file extension \"{os.path.basename(config_filepath).rsplit(".", 1)[-1]}\" is not implemented. Defaulted to forwarding content unchanged into key \"content\".")
         logger.debug(config)
-    
+
     return config
 
 
 def _create_default_file(config_filepath: str, config_default: dict[str, typing.Any]) -> None:
     """
     Creates a default config file at the specified filepath using config_default.
 
@@ -234,37 +241,40 @@
         logger=logging.getLogger("")            # also use root logger to match formats defined outside KFS
     else:                                       # if no root logger defined:
         logger=KFSlog.setup_logging("KFS")      # use KFS default format
 
     if os.path.exists(config_filepath)==True:   # if config filepath already exists: error
         logger.error(f"Creating \"{config_filepath}\" is not possible, because it already exists.")
         raise FileExistsError(f"Error in {load_config.__name__}{inspect.signature(load_config)}: Creating \"{config_filepath}\" is not possible, because it already exists.")
-    
-    
+
+
     logger.info(f"Creating default \"{config_filepath}\"...")
     try:
         if os.path.dirname(config_filepath)!="":
-            os.makedirs(os.path.dirname(config_filepath), exist_ok=True)    # create directories
-        with open(config_filepath, "wt", encoding="utf8") as config_file:   # create file
-            match os.path.basename(config_filepath).rsplit(".", 1)[-1]:     # fill with default content
+            os.makedirs(os.path.dirname(config_filepath), exist_ok=True)                    # create directories
+        with open(config_filepath, "wt", encoding="utf8") as config_file:                   # create file
+            match os.path.basename(config_filepath).rsplit(".", 1)[-1]:                     # fill with default content
                 case "env":
                     config_file.write("\n".join([f"{k}={v}" for k, v in config_default.items()]))
                 case "json":
-                    config_file.write(json.dumps(config_default, indent=4))
+                    if list(config_default.keys())==["content"]:                            # if only key is "content":
+                        config_file.write(json.dumps(config_default["content"], indent=4))  # unwrap content, save that as json, for top level data type support other than dict
+                    else:                                                                   # if normal json:
+                        config_file.write(json.dumps(config_default, indent=4))             # save normally as json
                 case "token" | "txt":
                     config_file.write(config_default["content"])
                 case _:
-                    defaulted=True                                          # defaulted to forwarding raw string content
+                    defaulted=True                                                          # defaulted to forwarding raw string content
                     config_file.write(config_default["content"])
     except KeyError:
         logger.error(f"\rCreating default \"{config_filepath}\" failed, because config_default is missing key \"content\".")
         raise
     except OSError as e:
         logger.error(f"\rCreating default \"{config_filepath}\" failed with {KFSfstr.full_class_name(e)}.")
         raise
     else:
         if defaulted==False:
             logger.info(f"\rCreated default \"{config_filepath}\".")
-        else:                   # if defaulted to forwarding raw string content: warn
+        else:                                                                               #  if defaulted to forwarding raw string content: warn
             logger.warning(f"Created default \"{config_filepath}\", but custom behaviour for file extension \"{os.path.basename(config_filepath).rsplit(".", 1)[-1]}\" is not implemented. Defaulted to forwarding content unchanged from key \"content\".")
 
     return
```

### Comparing `kfsconfig-2.1.6/pyproject.toml` & `kfsconfig-2.2.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 authors     = ["9FS <pray4spam@googlemail.com>"]
 description = ""
 license     = "MIT"
 name        = "KFSconfig"
 packages    = [{ include = "KFSconfig" }]
 readme      = "readme.md"
 repository  = "https://github.com/9-FS/2023-09-20-KFSconfig"
-version     = "2.1.6"
+version     = "2.2.0"
 
 [tool.poetry.dependencies]
 kfslog = "^2.0.0"
 python = "^3.12.0"
 
 [tool.poetry.group.dev.dependencies]
 hypothesis = "^6.0.0"
```

### Comparing `kfsconfig-2.1.6/readme.md` & `kfsconfig-2.2.0/readme.md`

 * *Files identical despite different names*

### Comparing `kfsconfig-2.1.6/PKG-INFO` & `kfsconfig-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KFSconfig
-Version: 2.1.6
+Version: 2.2.0
 Summary: 
 Home-page: https://github.com/9-FS/2023-09-20-KFSconfig
 License: MIT
 Author: 9FS
 Author-email: pray4spam@googlemail.com
 Requires-Python: >=3.12.0,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

