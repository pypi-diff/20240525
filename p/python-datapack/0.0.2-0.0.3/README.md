# Comparing `tmp/python_datapack-0.0.2.tar.gz` & `tmp/python_datapack-0.0.3.tar.gz`

## Comparing `python_datapack-0.0.2.tar` & `python_datapack-0.0.3.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 python_datapack-0.0.2/1_upgrades.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 python_datapack-0.0.2/2_build.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 python_datapack-0.0.2/3_upload.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 python_datapack-0.0.2/build_all_in_one.py
--rw-r--r--   0        0        0     7996 2020-02-02 00:00:00.000000 python_datapack-0.0.2/src/python_datapack/__init__.py
--rw-r--r--   0        0        0     2997 2020-02-02 00:00:00.000000 python_datapack-0.0.2/src/python_datapack/constants.py
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 python_datapack-0.0.2/src/python_datapack/enhance_config.py
--rw-r--r--   0        0        0     3800 2020-02-02 00:00:00.000000 python_datapack-0.0.2/src/python_datapack/finalyze.py
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 python_datapack-0.0.2/src/python_datapack/initialize.py
--rw-r--r--   0        0        0    10662 2020-02-02 00:00:00.000000 python_datapack-0.0.2/src/python_datapack/verify_database.py
--rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 python_datapack-0.0.2/src/python_datapack/datapack/basic_structure.py
--rw-r--r--   0        0        0    14654 2020-02-02 00:00:00.000000 python_datapack-0.0.2/src/python_datapack/datapack/custom_blocks.py
--rw-r--r--   0        0        0     2988 2020-02-02 00:00:00.000000 python_datapack-0.0.2/src/python_datapack/datapack/headers.py
--rw-r--r--   0        0        0     4134 2020-02-02 00:00:00.000000 python_datapack-0.0.2/src/python_datapack/datapack/lang.py
--rw-r--r--   0        0        0     6449 2020-02-02 00:00:00.000000 python_datapack-0.0.2/src/python_datapack/datapack/loading.py
--rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 python_datapack-0.0.2/src/python_datapack/datapack/loot_tables.py
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 python_datapack-0.0.2/src/python_datapack/datapack/main.py
--rw-r--r--   0        0        0     3942 2020-02-02 00:00:00.000000 python_datapack-0.0.2/src/python_datapack/datapack/recipes.py
--rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 python_datapack-0.0.2/src/python_datapack/manual/book_optimizer.py
--rw-r--r--   0        0        0    19323 2020-02-02 00:00:00.000000 python_datapack-0.0.2/src/python_datapack/manual/main.py
--rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 python_datapack-0.0.2/src/python_datapack/manual/shared_import.py
--rw-r--r--   0        0        0    24998 2020-02-02 00:00:00.000000 python_datapack-0.0.2/src/python_datapack/manual/utils.py
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 python_datapack-0.0.2/src/python_datapack/manual/assets/furnace.png
--rw-r--r--   0        0        0    42432 2020-02-02 00:00:00.000000 python_datapack-0.0.2/src/python_datapack/manual/assets/minecraft_font.ttf
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 python_datapack-0.0.2/src/python_datapack/manual/assets/none.png
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 python_datapack-0.0.2/src/python_datapack/manual/assets/none_release.png
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 python_datapack-0.0.2/src/python_datapack/manual/assets/shaped_2x2.png
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 python_datapack-0.0.2/src/python_datapack/manual/assets/shaped_3x3.png
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 python_datapack-0.0.2/src/python_datapack/manual/assets/simple_case_no_border.png
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 python_datapack-0.0.2/src/python_datapack/manual/assets/wiki_information.png
--rw-r--r--   0        0        0     3483 2020-02-02 00:00:00.000000 python_datapack-0.0.2/src/python_datapack/manual/assets/wiki_ingredient_of_craft.png
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 python_datapack-0.0.2/src/python_datapack/manual/assets/wiki_ingredient_of_craft_template.png
--rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 python_datapack-0.0.2/src/python_datapack/manual/assets/wiki_result_of_craft.png
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 python_datapack-0.0.2/src/python_datapack/resource_pack/check_unused_textures.py
--rw-r--r--   0        0        0     4497 2020-02-02 00:00:00.000000 python_datapack-0.0.2/src/python_datapack/resource_pack/item_models.py
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 python_datapack-0.0.2/src/python_datapack/resource_pack/main.py
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 python_datapack-0.0.2/src/python_datapack/resource_pack/sounds.py
--rw-r--r--   0        0        0     2787 2020-02-02 00:00:00.000000 python_datapack-0.0.2/src/python_datapack/resource_pack/vanilla_models.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 python_datapack-0.0.2/src/python_datapack/utils/cache.py
--rw-r--r--   0        0        0    28192 2020-02-02 00:00:00.000000 python_datapack-0.0.2/src/python_datapack/utils/database_helper.py
--rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 python_datapack-0.0.2/src/python_datapack/utils/ingredients.py
--rw-r--r--   0        0        0     4809 2020-02-02 00:00:00.000000 python_datapack-0.0.2/src/python_datapack/utils/io.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 python_datapack-0.0.2/src/python_datapack/utils/multiprocessing.py
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 python_datapack-0.0.2/src/python_datapack/utils/print.py
--rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 python_datapack-0.0.2/src/python_datapack/utils/weld.py
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 python_datapack-0.0.2/.gitignore
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 python_datapack-0.0.2/LICENSE
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 python_datapack-0.0.2/README.md
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 python_datapack-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 python_datapack-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 python_datapack-0.0.3/1_upgrades.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 python_datapack-0.0.3/2_build.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 python_datapack-0.0.3/3_upload.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 python_datapack-0.0.3/build_all_in_one.py
+-rw-r--r--   0        0        0     8074 2020-02-02 00:00:00.000000 python_datapack-0.0.3/src/python_datapack/__init__.py
+-rw-r--r--   0        0        0     2997 2020-02-02 00:00:00.000000 python_datapack-0.0.3/src/python_datapack/constants.py
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 python_datapack-0.0.3/src/python_datapack/enhance_config.py
+-rw-r--r--   0        0        0     3879 2020-02-02 00:00:00.000000 python_datapack-0.0.3/src/python_datapack/finalyze.py
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 python_datapack-0.0.3/src/python_datapack/initialize.py
+-rw-r--r--   0        0        0    10662 2020-02-02 00:00:00.000000 python_datapack-0.0.3/src/python_datapack/verify_database.py
+-rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 python_datapack-0.0.3/src/python_datapack/datapack/basic_structure.py
+-rw-r--r--   0        0        0    14654 2020-02-02 00:00:00.000000 python_datapack-0.0.3/src/python_datapack/datapack/custom_blocks.py
+-rw-r--r--   0        0        0     2988 2020-02-02 00:00:00.000000 python_datapack-0.0.3/src/python_datapack/datapack/headers.py
+-rw-r--r--   0        0        0     4134 2020-02-02 00:00:00.000000 python_datapack-0.0.3/src/python_datapack/datapack/lang.py
+-rw-r--r--   0        0        0     6449 2020-02-02 00:00:00.000000 python_datapack-0.0.3/src/python_datapack/datapack/loading.py
+-rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 python_datapack-0.0.3/src/python_datapack/datapack/loot_tables.py
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 python_datapack-0.0.3/src/python_datapack/datapack/main.py
+-rw-r--r--   0        0        0     3942 2020-02-02 00:00:00.000000 python_datapack-0.0.3/src/python_datapack/datapack/recipes.py
+-rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 python_datapack-0.0.3/src/python_datapack/manual/book_optimizer.py
+-rw-r--r--   0        0        0    19323 2020-02-02 00:00:00.000000 python_datapack-0.0.3/src/python_datapack/manual/main.py
+-rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 python_datapack-0.0.3/src/python_datapack/manual/shared_import.py
+-rw-r--r--   0        0        0    24998 2020-02-02 00:00:00.000000 python_datapack-0.0.3/src/python_datapack/manual/utils.py
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 python_datapack-0.0.3/src/python_datapack/manual/assets/furnace.png
+-rw-r--r--   0        0        0    42432 2020-02-02 00:00:00.000000 python_datapack-0.0.3/src/python_datapack/manual/assets/minecraft_font.ttf
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 python_datapack-0.0.3/src/python_datapack/manual/assets/none.png
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 python_datapack-0.0.3/src/python_datapack/manual/assets/none_release.png
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 python_datapack-0.0.3/src/python_datapack/manual/assets/shaped_2x2.png
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 python_datapack-0.0.3/src/python_datapack/manual/assets/shaped_3x3.png
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 python_datapack-0.0.3/src/python_datapack/manual/assets/simple_case_no_border.png
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 python_datapack-0.0.3/src/python_datapack/manual/assets/wiki_information.png
+-rw-r--r--   0        0        0     3483 2020-02-02 00:00:00.000000 python_datapack-0.0.3/src/python_datapack/manual/assets/wiki_ingredient_of_craft.png
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 python_datapack-0.0.3/src/python_datapack/manual/assets/wiki_ingredient_of_craft_template.png
+-rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 python_datapack-0.0.3/src/python_datapack/manual/assets/wiki_result_of_craft.png
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 python_datapack-0.0.3/src/python_datapack/resource_pack/check_unused_textures.py
+-rw-r--r--   0        0        0     4497 2020-02-02 00:00:00.000000 python_datapack-0.0.3/src/python_datapack/resource_pack/item_models.py
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 python_datapack-0.0.3/src/python_datapack/resource_pack/main.py
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 python_datapack-0.0.3/src/python_datapack/resource_pack/sounds.py
+-rw-r--r--   0        0        0     2787 2020-02-02 00:00:00.000000 python_datapack-0.0.3/src/python_datapack/resource_pack/vanilla_models.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 python_datapack-0.0.3/src/python_datapack/utils/cache.py
+-rw-r--r--   0        0        0    28192 2020-02-02 00:00:00.000000 python_datapack-0.0.3/src/python_datapack/utils/database_helper.py
+-rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 python_datapack-0.0.3/src/python_datapack/utils/ingredients.py
+-rw-r--r--   0        0        0     4809 2020-02-02 00:00:00.000000 python_datapack-0.0.3/src/python_datapack/utils/io.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 python_datapack-0.0.3/src/python_datapack/utils/multiprocessing.py
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 python_datapack-0.0.3/src/python_datapack/utils/print.py
+-rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 python_datapack-0.0.3/src/python_datapack/utils/weld.py
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 python_datapack-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 python_datapack-0.0.3/LICENSE
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 python_datapack-0.0.3/README.md
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 python_datapack-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 python_datapack-0.0.3/PKG-INFO
```

### Comparing `python_datapack-0.0.2/src/python_datapack/__init__.py` & `python_datapack-0.0.3/src/python_datapack/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from .initialize import main as initialize_main
 from .verify_database import main as verify_database_main
 from .resource_pack.main import main as resource_pack_main
 from .manual.main import main as manual_main
 from .datapack.main import main as datapack_main
 from .finalyze import main as finalyze_main
 
+# Functions
 def basic_key_check(config: dict, key: str, value_type: type, hint: str, valid: bool) -> bool:
 	bool_return = valid
 	if not config.get(key):
 		bool_return = warning(f"Missing '{key}' key in config file\n" + hint)
 	elif type(config[key])!= value_type:
 		bool_return = warning(f"Invalid type for '{key}' key in config file, found {type(config[key])} instead of {value_type}\n" + hint)
 	return bool_return
@@ -67,14 +68,16 @@
 	""" Main function of the datapack build process
 	Args:
 		config (dict): Configuration of the program, the program will check the config format with high precision
 		setup_database (callable): Function that will setup the database of the datapack items and blocks, again the program will check the format of the database
 		setup_external_database (callable|None): Function that will setup the external database (if you need an item in a craft), same format as first
 		user_code (callable|None): Function that will be called after the datapack has been generated, can be used to add custom code to generated some parts of the datapack
 	"""
+	os.environ['PYGAME_HIDE_SUPPORT_PROMPT'] = "hide"
+
 	# Check config format
 	valid = check_config_format(config)
 	if not valid:
 		error("Invalid config format, please check the documentation")
 	
 	# Enhance config dict
 	config = enhance_config_main(config)
@@ -99,13 +102,13 @@
 	if config["has_manual"]:
 		manual_main(config)
 	
 	# Generate datapack
 	datapack_main(config)
 
 	# Finalyze build process
-	finalyze_main(config)
+	finalyze_main(config, user_code)
 
 	# Total time
 	total_time = time.time() - START_TIME
 	info(f"Build finished in {total_time:.3f} seconds")
```

### Comparing `python_datapack-0.0.2/src/python_datapack/constants.py` & `python_datapack-0.0.3/src/python_datapack/constants.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.2/src/python_datapack/enhance_config.py` & `python_datapack-0.0.3/src/python_datapack/enhance_config.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.2/src/python_datapack/finalyze.py` & `python_datapack-0.0.3/src/python_datapack/finalyze.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from .utils.print import *
 from .utils.weld import weld_datapack, weld_resource_pack
 from .datapack.lang import main as lang_main
 from .datapack.headers import main as headers_main
 from .resource_pack.check_unused_textures import main as check_unused_textures_main
 import shutil
 
-def main(config: dict):
+def main(config: dict, user_code: callable|None):
 
 	# For every file in the merge folder, copy it to the build folder (with append content)
 	print()
 	for root, _, files in os.walk(config['merge_folder']):
 		for file in files:
 			merge_path = f"{root}/{file}".replace("\\", "/")
 			build_path = merge_path.replace(config['merge_folder'], config['build_folder'])
@@ -40,14 +40,18 @@
 						write_to_file(build_path, f.read())
 				
 				# Else, just copy the file, such as pack.mcmeta, pack.png, ...
 				else:
 					super_copy(merge_path, build_path)
 	info(f"All content in the '{config['merge_folder']}' folder copied to '{config['build_folder']}'")
 
+	# Run user code
+	if user_code:
+		user_code(config)
+
 	# Generate lang file
 	if config['enable_translations']:
 		lang_main(config)
 
 	# Add a small header for each .mcfunction file
 	headers_main(config)
```

### Comparing `python_datapack-0.0.2/src/python_datapack/initialize.py` & `python_datapack-0.0.3/src/python_datapack/initialize.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.2/src/python_datapack/verify_database.py` & `python_datapack-0.0.3/src/python_datapack/verify_database.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.2/src/python_datapack/datapack/basic_structure.py` & `python_datapack-0.0.3/src/python_datapack/datapack/basic_structure.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.2/src/python_datapack/datapack/custom_blocks.py` & `python_datapack-0.0.3/src/python_datapack/datapack/custom_blocks.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.2/src/python_datapack/datapack/headers.py` & `python_datapack-0.0.3/src/python_datapack/datapack/headers.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.2/src/python_datapack/datapack/lang.py` & `python_datapack-0.0.3/src/python_datapack/datapack/lang.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.2/src/python_datapack/datapack/loading.py` & `python_datapack-0.0.3/src/python_datapack/datapack/loading.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.2/src/python_datapack/datapack/loot_tables.py` & `python_datapack-0.0.3/src/python_datapack/datapack/loot_tables.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.2/src/python_datapack/datapack/main.py` & `python_datapack-0.0.3/src/python_datapack/datapack/main.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.2/src/python_datapack/datapack/recipes.py` & `python_datapack-0.0.3/src/python_datapack/datapack/recipes.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.2/src/python_datapack/manual/book_optimizer.py` & `python_datapack-0.0.3/src/python_datapack/manual/book_optimizer.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.2/src/python_datapack/manual/main.py` & `python_datapack-0.0.3/src/python_datapack/manual/main.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.2/src/python_datapack/manual/shared_import.py` & `python_datapack-0.0.3/src/python_datapack/manual/shared_import.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 	global next_craft_font
 	next_craft_font += 1
 	return get_font(next_craft_font)
 
 
 # Constants
 SQUARE_SIZE = 32
-MANUAL_ASSETS_PATH = os.path.dirname(os.path.abspath(__file__)).replace("\\","/") + "/"
+MANUAL_ASSETS_PATH = os.path.dirname(os.path.realpath(__file__)).replace("\\","/") + "/"
 TEMPLATES_PATH = MANUAL_ASSETS_PATH + "assets"
 FONT_FILE = "manual"
 BORDER_COLOR = 0xB64E2F
 BORDER_SIZE = 2
 BORDER_COLOR = (BORDER_COLOR >> 16) & 0xFF, (BORDER_COLOR >> 8) & 0xFF, BORDER_COLOR & 0xFF, 255
 NONE_FONT = get_font(0x0000)
 MEDIUM_NONE_FONT = get_font(0x0001)
```

### Comparing `python_datapack-0.0.2/src/python_datapack/manual/utils.py` & `python_datapack-0.0.3/src/python_datapack/manual/utils.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.2/src/python_datapack/manual/assets/furnace.png` & `python_datapack-0.0.3/src/python_datapack/manual/assets/furnace.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.2/src/python_datapack/manual/assets/minecraft_font.ttf` & `python_datapack-0.0.3/src/python_datapack/manual/assets/minecraft_font.ttf`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.2/src/python_datapack/manual/assets/shaped_2x2.png` & `python_datapack-0.0.3/src/python_datapack/manual/assets/shaped_2x2.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.2/src/python_datapack/manual/assets/shaped_3x3.png` & `python_datapack-0.0.3/src/python_datapack/manual/assets/shaped_3x3.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.2/src/python_datapack/manual/assets/simple_case_no_border.png` & `python_datapack-0.0.3/src/python_datapack/manual/assets/simple_case_no_border.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.2/src/python_datapack/manual/assets/wiki_information.png` & `python_datapack-0.0.3/src/python_datapack/manual/assets/wiki_information.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.2/src/python_datapack/manual/assets/wiki_ingredient_of_craft.png` & `python_datapack-0.0.3/src/python_datapack/manual/assets/wiki_ingredient_of_craft.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.2/src/python_datapack/manual/assets/wiki_ingredient_of_craft_template.png` & `python_datapack-0.0.3/src/python_datapack/manual/assets/wiki_ingredient_of_craft_template.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.2/src/python_datapack/manual/assets/wiki_result_of_craft.png` & `python_datapack-0.0.3/src/python_datapack/manual/assets/wiki_result_of_craft.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.2/src/python_datapack/resource_pack/check_unused_textures.py` & `python_datapack-0.0.3/src/python_datapack/resource_pack/check_unused_textures.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.2/src/python_datapack/resource_pack/item_models.py` & `python_datapack-0.0.3/src/python_datapack/resource_pack/item_models.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.2/src/python_datapack/resource_pack/sounds.py` & `python_datapack-0.0.3/src/python_datapack/resource_pack/sounds.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.2/src/python_datapack/resource_pack/vanilla_models.py` & `python_datapack-0.0.3/src/python_datapack/resource_pack/vanilla_models.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.2/src/python_datapack/utils/database_helper.py` & `python_datapack-0.0.3/src/python_datapack/utils/database_helper.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.2/src/python_datapack/utils/ingredients.py` & `python_datapack-0.0.3/src/python_datapack/utils/ingredients.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.2/src/python_datapack/utils/io.py` & `python_datapack-0.0.3/src/python_datapack/utils/io.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.2/src/python_datapack/utils/multiprocessing.py` & `python_datapack-0.0.3/src/python_datapack/utils/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.2/src/python_datapack/utils/print.py` & `python_datapack-0.0.3/src/python_datapack/utils/print.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.2/src/python_datapack/utils/weld.py` & `python_datapack-0.0.3/src/python_datapack/utils/weld.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.2/LICENSE` & `python_datapack-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.2/pyproject.toml` & `python_datapack-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["hatchling", "pillow", "smithed"]
 build-backend = "hatchling.build"
 
 [project]
 name = "python_datapack"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
 	{ name="Stoupy51", email="stoupy51@gmail.com" },
 ]
 description = "Python package to help generating advanced Minecraft datapack contents"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `python_datapack-0.0.2/PKG-INFO` & `python_datapack-0.0.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: python_datapack
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python package to help generating advanced Minecraft datapack contents
 Project-URL: Homepage, https://github.com/Stoupy51/python_datapack
 Project-URL: Issues, https://github.com/Stoupy51/python_datapack/issues
 Author-email: Stoupy51 <stoupy51@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

