# Comparing `tmp/python_datapack-0.0.3.tar.gz` & `tmp/python_datapack-0.0.4.tar.gz`

## Comparing `python_datapack-0.0.3.tar` & `python_datapack-0.0.4.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 python_datapack-0.0.3/1_upgrades.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 python_datapack-0.0.3/2_build.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 python_datapack-0.0.3/3_upload.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 python_datapack-0.0.3/build_all_in_one.py
--rw-r--r--   0        0        0     8074 2020-02-02 00:00:00.000000 python_datapack-0.0.3/src/python_datapack/__init__.py
--rw-r--r--   0        0        0     2997 2020-02-02 00:00:00.000000 python_datapack-0.0.3/src/python_datapack/constants.py
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 python_datapack-0.0.3/src/python_datapack/enhance_config.py
--rw-r--r--   0        0        0     3879 2020-02-02 00:00:00.000000 python_datapack-0.0.3/src/python_datapack/finalyze.py
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 python_datapack-0.0.3/src/python_datapack/initialize.py
--rw-r--r--   0        0        0    10662 2020-02-02 00:00:00.000000 python_datapack-0.0.3/src/python_datapack/verify_database.py
--rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 python_datapack-0.0.3/src/python_datapack/datapack/basic_structure.py
--rw-r--r--   0        0        0    14654 2020-02-02 00:00:00.000000 python_datapack-0.0.3/src/python_datapack/datapack/custom_blocks.py
--rw-r--r--   0        0        0     2988 2020-02-02 00:00:00.000000 python_datapack-0.0.3/src/python_datapack/datapack/headers.py
--rw-r--r--   0        0        0     4134 2020-02-02 00:00:00.000000 python_datapack-0.0.3/src/python_datapack/datapack/lang.py
--rw-r--r--   0        0        0     6449 2020-02-02 00:00:00.000000 python_datapack-0.0.3/src/python_datapack/datapack/loading.py
--rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 python_datapack-0.0.3/src/python_datapack/datapack/loot_tables.py
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 python_datapack-0.0.3/src/python_datapack/datapack/main.py
--rw-r--r--   0        0        0     3942 2020-02-02 00:00:00.000000 python_datapack-0.0.3/src/python_datapack/datapack/recipes.py
--rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 python_datapack-0.0.3/src/python_datapack/manual/book_optimizer.py
--rw-r--r--   0        0        0    19323 2020-02-02 00:00:00.000000 python_datapack-0.0.3/src/python_datapack/manual/main.py
--rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 python_datapack-0.0.3/src/python_datapack/manual/shared_import.py
--rw-r--r--   0        0        0    24998 2020-02-02 00:00:00.000000 python_datapack-0.0.3/src/python_datapack/manual/utils.py
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 python_datapack-0.0.3/src/python_datapack/manual/assets/furnace.png
--rw-r--r--   0        0        0    42432 2020-02-02 00:00:00.000000 python_datapack-0.0.3/src/python_datapack/manual/assets/minecraft_font.ttf
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 python_datapack-0.0.3/src/python_datapack/manual/assets/none.png
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 python_datapack-0.0.3/src/python_datapack/manual/assets/none_release.png
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 python_datapack-0.0.3/src/python_datapack/manual/assets/shaped_2x2.png
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 python_datapack-0.0.3/src/python_datapack/manual/assets/shaped_3x3.png
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 python_datapack-0.0.3/src/python_datapack/manual/assets/simple_case_no_border.png
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 python_datapack-0.0.3/src/python_datapack/manual/assets/wiki_information.png
--rw-r--r--   0        0        0     3483 2020-02-02 00:00:00.000000 python_datapack-0.0.3/src/python_datapack/manual/assets/wiki_ingredient_of_craft.png
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 python_datapack-0.0.3/src/python_datapack/manual/assets/wiki_ingredient_of_craft_template.png
--rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 python_datapack-0.0.3/src/python_datapack/manual/assets/wiki_result_of_craft.png
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 python_datapack-0.0.3/src/python_datapack/resource_pack/check_unused_textures.py
--rw-r--r--   0        0        0     4497 2020-02-02 00:00:00.000000 python_datapack-0.0.3/src/python_datapack/resource_pack/item_models.py
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 python_datapack-0.0.3/src/python_datapack/resource_pack/main.py
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 python_datapack-0.0.3/src/python_datapack/resource_pack/sounds.py
--rw-r--r--   0        0        0     2787 2020-02-02 00:00:00.000000 python_datapack-0.0.3/src/python_datapack/resource_pack/vanilla_models.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 python_datapack-0.0.3/src/python_datapack/utils/cache.py
--rw-r--r--   0        0        0    28192 2020-02-02 00:00:00.000000 python_datapack-0.0.3/src/python_datapack/utils/database_helper.py
--rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 python_datapack-0.0.3/src/python_datapack/utils/ingredients.py
--rw-r--r--   0        0        0     4809 2020-02-02 00:00:00.000000 python_datapack-0.0.3/src/python_datapack/utils/io.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 python_datapack-0.0.3/src/python_datapack/utils/multiprocessing.py
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 python_datapack-0.0.3/src/python_datapack/utils/print.py
--rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 python_datapack-0.0.3/src/python_datapack/utils/weld.py
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 python_datapack-0.0.3/.gitignore
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 python_datapack-0.0.3/LICENSE
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 python_datapack-0.0.3/README.md
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 python_datapack-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 python_datapack-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 python_datapack-0.0.4/1_upgrades.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 python_datapack-0.0.4/2_build.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 python_datapack-0.0.4/3_upload.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 python_datapack-0.0.4/build_all_in_one.py
+-rw-r--r--   0        0        0     8141 2020-02-02 00:00:00.000000 python_datapack-0.0.4/src/python_datapack/__init__.py
+-rw-r--r--   0        0        0     2997 2020-02-02 00:00:00.000000 python_datapack-0.0.4/src/python_datapack/constants.py
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 python_datapack-0.0.4/src/python_datapack/enhance_config.py
+-rw-r--r--   0        0        0     3879 2020-02-02 00:00:00.000000 python_datapack-0.0.4/src/python_datapack/finalyze.py
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 python_datapack-0.0.4/src/python_datapack/initialize.py
+-rw-r--r--   0        0        0    10662 2020-02-02 00:00:00.000000 python_datapack-0.0.4/src/python_datapack/verify_database.py
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 python_datapack-0.0.4/src/python_datapack/datapack/basic_structure.py
+-rw-r--r--   0        0        0    14581 2020-02-02 00:00:00.000000 python_datapack-0.0.4/src/python_datapack/datapack/custom_blocks.py
+-rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 python_datapack-0.0.4/src/python_datapack/datapack/headers.py
+-rw-r--r--   0        0        0     4134 2020-02-02 00:00:00.000000 python_datapack-0.0.4/src/python_datapack/datapack/lang.py
+-rw-r--r--   0        0        0     6408 2020-02-02 00:00:00.000000 python_datapack-0.0.4/src/python_datapack/datapack/loading.py
+-rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 python_datapack-0.0.4/src/python_datapack/datapack/loot_tables.py
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 python_datapack-0.0.4/src/python_datapack/datapack/main.py
+-rw-r--r--   0        0        0     3942 2020-02-02 00:00:00.000000 python_datapack-0.0.4/src/python_datapack/datapack/recipes.py
+-rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 python_datapack-0.0.4/src/python_datapack/manual/book_optimizer.py
+-rw-r--r--   0        0        0    19311 2020-02-02 00:00:00.000000 python_datapack-0.0.4/src/python_datapack/manual/main.py
+-rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 python_datapack-0.0.4/src/python_datapack/manual/shared_import.py
+-rw-r--r--   0        0        0    24998 2020-02-02 00:00:00.000000 python_datapack-0.0.4/src/python_datapack/manual/utils.py
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 python_datapack-0.0.4/src/python_datapack/manual/assets/furnace.png
+-rw-r--r--   0        0        0    42432 2020-02-02 00:00:00.000000 python_datapack-0.0.4/src/python_datapack/manual/assets/minecraft_font.ttf
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 python_datapack-0.0.4/src/python_datapack/manual/assets/none.png
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 python_datapack-0.0.4/src/python_datapack/manual/assets/none_release.png
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 python_datapack-0.0.4/src/python_datapack/manual/assets/shaped_2x2.png
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 python_datapack-0.0.4/src/python_datapack/manual/assets/shaped_3x3.png
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 python_datapack-0.0.4/src/python_datapack/manual/assets/simple_case_no_border.png
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 python_datapack-0.0.4/src/python_datapack/manual/assets/wiki_information.png
+-rw-r--r--   0        0        0     3483 2020-02-02 00:00:00.000000 python_datapack-0.0.4/src/python_datapack/manual/assets/wiki_ingredient_of_craft.png
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 python_datapack-0.0.4/src/python_datapack/manual/assets/wiki_ingredient_of_craft_template.png
+-rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 python_datapack-0.0.4/src/python_datapack/manual/assets/wiki_result_of_craft.png
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 python_datapack-0.0.4/src/python_datapack/resource_pack/check_unused_textures.py
+-rw-r--r--   0        0        0     4497 2020-02-02 00:00:00.000000 python_datapack-0.0.4/src/python_datapack/resource_pack/item_models.py
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 python_datapack-0.0.4/src/python_datapack/resource_pack/main.py
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 python_datapack-0.0.4/src/python_datapack/resource_pack/sounds.py
+-rw-r--r--   0        0        0     2787 2020-02-02 00:00:00.000000 python_datapack-0.0.4/src/python_datapack/resource_pack/vanilla_models.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 python_datapack-0.0.4/src/python_datapack/utils/cache.py
+-rw-r--r--   0        0        0    28262 2020-02-02 00:00:00.000000 python_datapack-0.0.4/src/python_datapack/utils/database_helper.py
+-rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 python_datapack-0.0.4/src/python_datapack/utils/ingredients.py
+-rw-r--r--   0        0        0     4809 2020-02-02 00:00:00.000000 python_datapack-0.0.4/src/python_datapack/utils/io.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 python_datapack-0.0.4/src/python_datapack/utils/multiprocessing.py
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 python_datapack-0.0.4/src/python_datapack/utils/print.py
+-rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 python_datapack-0.0.4/src/python_datapack/utils/weld.py
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 python_datapack-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 python_datapack-0.0.4/LICENSE
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 python_datapack-0.0.4/README.md
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 python_datapack-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 python_datapack-0.0.4/PKG-INFO
```

### Comparing `python_datapack-0.0.3/src/python_datapack/__init__.py` & `python_datapack-0.0.4/src/python_datapack/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,28 +13,28 @@
 from .manual.main import main as manual_main
 from .datapack.main import main as datapack_main
 from .finalyze import main as finalyze_main
 
 # Functions
 def basic_key_check(config: dict, key: str, value_type: type, hint: str, valid: bool) -> bool:
 	bool_return = valid
-	if not config.get(key):
-		bool_return = warning(f"Missing '{key}' key in config file\n" + hint)
-	elif type(config[key])!= value_type:
-		bool_return = warning(f"Invalid type for '{key}' key in config file, found {type(config[key])} instead of {value_type}\n" + hint)
+	if config.get(key, None) == None:
+		bool_return = warning(f"Missing '{key}' key in config file\n ({hint})")
+	elif not isinstance(config[key], value_type):
+		bool_return = warning(f"Invalid type for '{key}' key in config file, found {type(config[key])} instead of {value_type}\n ({hint})")
 	return bool_return
 
 def check_config_format(config: dict) -> bool:
 	valid = True
 	valid = basic_key_check(config, "merge_folder", str, "If a file exists in both merge and build folder, they will be merged. Otherwise, it's just copied.", valid)
 	valid = basic_key_check(config, "build_folder", str, "Folder where the final datapack and resource pack are built", valid)
 	valid = basic_key_check(config, "assets_folder", str, "Folder containing the all assets (textures, sounds, ...) for the datapack", valid)
 	valid = basic_key_check(config, "textures_folder", str, "Folder containing the textures for the datapack", valid)
 	valid = basic_key_check(config, "libs_folder", str, "The libraries are copied to the build destination, and merged with the datapack using Weld", valid)
-	valid = basic_key_check(config, "build_copy_destinations", tuple[str,str], "Can be empty paths if you don't want to copy the generated files", valid)
+	valid = basic_key_check(config, "build_copy_destinations", tuple, "Can be empty paths if you don't want to copy the generated files", valid)
 	valid = basic_key_check(config, "debug_mode", bool, "Shows up grids in manual", valid)
 	valid = basic_key_check(config, "database_debug", str, "Dump of the database for debugging purposes", valid)
 	valid = basic_key_check(config, "cmd_cache", str, "Cache of all items Custom Model Data", valid)
 	valid = basic_key_check(config, "enable_translations", bool, "Will convert all the text components to translate and generate a lang file (WARNING: The algorithm is pretty slow, so it's recommended to disable it when not needed)", valid)
 	valid = basic_key_check(config, "lang_file_debug", str, "Dump of the lang file for debugging purposes", valid)
 	valid = basic_key_check(config, "merge_libs", bool, "Make new zip of merged libraries with the datapack and resource pack using Smithed Weld", valid)
 	valid = basic_key_check(config, "author", str, "Author(s) name(s) displayed in pack.mcmeta, also used to add convention.debug tag to the players of the same name(s) <-- showing additionnal displays like datapack loading", valid)
@@ -42,33 +42,33 @@
 	valid = basic_key_check(config, "minecraft_version", str, "Text used when loading the datapack to warn the user when the data version is not right", valid)
 	valid = basic_key_check(config, "data_version", int, "Depending on MC version, given by /data get entity @p DataVersion to check if the datapack is not running in an older version of MC", valid)
 	valid = basic_key_check(config, "version", str, "Datapack version in the following mandatory format: major.minor.patch, ex: 1.0.0 or 1.21.615", valid)
 	valid = basic_key_check(config, "namespace", str, "Should be the same you use in the merge folder. Used to namespace functions, tags, etc.", valid)
 	valid = basic_key_check(config, "datapack_format", int, "Pack format version, see https://minecraft.wiki/w/Pack_format#List_of_data_pack_formats", valid)
 	valid = basic_key_check(config, "resource_pack_format", int, "Resource pack format version, see https://minecraft.wiki/w/Pack_format#List_of_resource_pack_formats", valid)
 	valid = basic_key_check(config, "description", str, "Pack description displayed in pack.mcmeta", valid)
-	valid = basic_key_check(config, "dependencies", dict[str, dict[str, list[int] | str]], "Automagically, the datapack will check for the presence of dependencies and their minimum required versions at runtime\nThe url is used when the dependency is not found to suggest where to get it\nThe version dict key contains the minimum required version of the dependency in [major, minor, patch] format\nThe main key is the dependency namespace to check for\nThe name can be whatever you want, it's just used in messages", valid)
-	valid = basic_key_check(config, "source_lore", list[dict], "Appended lore to any custom item, can be an empty string to disable", valid)
+	valid = basic_key_check(config, "dependencies", dict, "Automagically, the datapack will check for the presence of dependencies and their minimum required versions at runtime\nThe url is used when the dependency is not found to suggest where to get it\nThe version dict key contains the minimum required version of the dependency in [major, minor, patch] format\nThe main key is the dependency namespace to check for\nThe name can be whatever you want, it's just used in messages", valid)
+	valid = basic_key_check(config, "source_lore", list, "Appended lore to any custom item, can be an empty string to disable", valid)
 	has_manual = basic_key_check(config, "has_manual", bool, "Do the program generate a manual/guide? (WARNING: if an item is malformed in the database, the server log will be flooded on load by the manual hiding the malformed item)", True)
 	if has_manual == True:
 		valid = basic_key_check(config, "manual_path", str, "Cached manual assets", valid)
 		valid = basic_key_check(config, "cache_manual_assets", bool, "Caches the MC assets and the items renders for the manual (manual/items/*.png)", valid)
 		valid = basic_key_check(config, "cache_manual_pages", bool, "Caches the content of the manual and the images (manual/pages/*.png)", valid)
 		valid = basic_key_check(config, "manual_debug", str, "Dump of the manual for debugging purposes", valid)
 		valid = basic_key_check(config, "manual_name", str, "Name of the manual, used for the title of the book and first page", valid)
 		valid = basic_key_check(config, "max_items_per_row", int, "Max number of items per row in the manual, should not exceed 6", valid)
 		valid = basic_key_check(config, "max_rows_per_page", int, "Max number of rows per page in the manual, should not exceed 6", valid)
 		valid = basic_key_check(config, "opengl_resolution", int, "Resolution of the OpenGL renders used in the manual, best value is 64 <--- 64x64", valid)
-		valid = basic_key_check(config, "manual_first_page_text", list[dict], "Text for the first page of the manual", valid)
+		valid = basic_key_check(config, "manual_first_page_text", list, "Text for the first page of the manual", valid)
 	elif valid == True:
 		valid = has_manual
 	return valid == True
 
 
-def build_process(config: dict, setup_database: callable, setup_external_database: callable|None = None, user_code: callable|None = None):
+def build_process(config: dict, setup_database: callable, setup_external_database: callable = None, user_code: callable = None):
 	""" Main function of the datapack build process
 	Args:
 		config (dict): Configuration of the program, the program will check the config format with high precision
 		setup_database (callable): Function that will setup the database of the datapack items and blocks, again the program will check the format of the database
 		setup_external_database (callable|None): Function that will setup the external database (if you need an item in a craft), same format as first
 		user_code (callable|None): Function that will be called after the datapack has been generated, can be used to add custom code to generated some parts of the datapack
 	"""
@@ -88,14 +88,16 @@
 	info("Starting build process...")
 
 	# Initialize build process
 	initialize_main(config)
 
 	# Generate items/blocks database and verify the format
 	config["database"] = setup_database(config)
+	if config["database"] == None:
+		error("No database returned, when calling the setup_database function")
 	config["external_database"] = setup_external_database(config) if setup_external_database else {}
 	verify_database_main(config)
 
 	# Generate resource pack
 	resource_pack_main(config)
 
 	# Generate manual
```

### Comparing `python_datapack-0.0.3/src/python_datapack/constants.py` & `python_datapack-0.0.4/src/python_datapack/constants.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.3/src/python_datapack/enhance_config.py` & `python_datapack-0.0.4/src/python_datapack/enhance_config.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.3/src/python_datapack/finalyze.py` & `python_datapack-0.0.4/src/python_datapack/finalyze.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.3/src/python_datapack/initialize.py` & `python_datapack-0.0.4/src/python_datapack/initialize.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.3/src/python_datapack/verify_database.py` & `python_datapack-0.0.4/src/python_datapack/verify_database.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.3/src/python_datapack/datapack/basic_structure.py` & `python_datapack-0.0.4/src/python_datapack/datapack/basic_structure.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,37 +3,37 @@
 from ..utils.io import *
 from ..utils.print import *
 
 def main(config: dict):
 
 	# Tick structure, tick_2 and second_5 are "offsync" for a better load distribution
 	write_to_file(f"{config['datapack_functions']}/tick.mcfunction", f"""
-	# Timers
-	scoreboard players add #tick_2 {config['namespace']}.data 1
-	scoreboard players add #second {config['namespace']}.data 1
-	scoreboard players add #second_5 {config['namespace']}.data 1
-	scoreboard players add #minute {config['namespace']}.data 1
-	execute if score #tick_2 {config['namespace']}.data matches 3.. run function {config['namespace']}:tick_2
-	execute if score #second {config['namespace']}.data matches 20.. run function {config['namespace']}:second
-	execute if score #second_5 {config['namespace']}.data matches 90.. run function {config['namespace']}:second_5
-	execute if score #minute {config['namespace']}.data matches 1200.. run function {config['namespace']}:minute
-	""")
+# Timers
+scoreboard players add #tick_2 {config['namespace']}.data 1
+scoreboard players add #second {config['namespace']}.data 1
+scoreboard players add #second_5 {config['namespace']}.data 1
+scoreboard players add #minute {config['namespace']}.data 1
+execute if score #tick_2 {config['namespace']}.data matches 3.. run function {config['namespace']}:tick_2
+execute if score #second {config['namespace']}.data matches 20.. run function {config['namespace']}:second
+execute if score #second_5 {config['namespace']}.data matches 90.. run function {config['namespace']}:second_5
+execute if score #minute {config['namespace']}.data matches 1200.. run function {config['namespace']}:minute
+""")
 
 	# Write remaining files
 	write_to_file(f"{config['datapack_functions']}/tick_2.mcfunction", f"""
-	# Reset timer
-	scoreboard players set #tick_2 {config['namespace']}.data 1
-	""")
+# Reset timer
+scoreboard players set #tick_2 {config['namespace']}.data 1
+""")
 	write_to_file(f"{config['datapack_functions']}/second.mcfunction", f"""
-	# Reset timer
-	scoreboard players set #second {config['namespace']}.data 0
-	""")
+# Reset timer
+scoreboard players set #second {config['namespace']}.data 0
+""")
 	write_to_file(f"{config['datapack_functions']}/second_5.mcfunction", f"""
-	# Reset timer
-	scoreboard players set #second_5 {config['namespace']}.data -10
-	""")
+# Reset timer
+scoreboard players set #second_5 {config['namespace']}.data -10
+""")
 	write_to_file(f"{config['datapack_functions']}/minute.mcfunction", f"""
-	# Reset timer
-	scoreboard players set #minute {config['namespace']}.data 1
-	""")
+# Reset timer
+scoreboard players set #minute {config['namespace']}.data 1
+""")
```

### Comparing `python_datapack-0.0.3/src/python_datapack/datapack/custom_blocks.py` & `python_datapack-0.0.4/src/python_datapack/datapack/custom_blocks.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,43 +46,43 @@
 			write_to_file(f"{path}/place_main.mcfunction", content)
 
 			## Secondary function
 			unique_blocks.add(block)
 			block = block.replace(":","_")
 			custom_model_data = data["custom_model_data"]
 			content = f"""
-	# Add convention and utils tags, and the custom block tag
-	tag @s add global.ignore
-	tag @s add global.ignore.kill
-	tag @s add smithed.entity
-	tag @s add smithed.block
-	tag @s add {config['namespace']}.custom_block
-	tag @s add {config['namespace']}.{item}
-	tag @s add {config['namespace']}.vanilla.{block}
-
-	# Modify item display entity to match the custom block
-	item replace entity @s container.0 with deepslate[minecraft:custom_model_data={custom_model_data}]
-	data modify entity @s transformation.scale set value [1.002f,1.002f,1.002f]
-	data modify entity @s brightness set value {{block:15,sky:15}}
-
-	## Check if the block have rotation
-	# Furnace case
-	scoreboard players set #rotation {config['namespace']}.data 0
-	execute if score #rotation {config['namespace']}.data matches 0 store success score #rotation {config['namespace']}.data if block ~ ~ ~ furnace[facing=north] run data modify entity @s Rotation[0] set value 180.0f
-	execute if score #rotation {config['namespace']}.data matches 0 store success score #rotation {config['namespace']}.data if block ~ ~ ~ furnace[facing=east] run data modify entity @s Rotation[0] set value 270.0f
-	execute if score #rotation {config['namespace']}.data matches 0 store success score #rotation {config['namespace']}.data if block ~ ~ ~ furnace[facing=south] run data modify entity @s Rotation[0] set value 0.0f
-	execute if score #rotation {config['namespace']}.data matches 0 store success score #rotation {config['namespace']}.data if block ~ ~ ~ furnace[facing=west] run data modify entity @s Rotation[0] set value 90.0f
-	# Iron trapdoor case
-	execute if score #rotation {config['namespace']}.data matches 0 store success score #rotation {config['namespace']}.data if block ~ ~ ~ iron_trapdoor[facing=north] run data modify entity @s Rotation[0] set value 180.0f
-	execute if score #rotation {config['namespace']}.data matches 0 store success score #rotation {config['namespace']}.data if block ~ ~ ~ iron_trapdoor[facing=east] run data modify entity @s Rotation[0] set value 270.0f
-	execute if score #rotation {config['namespace']}.data matches 0 store success score #rotation {config['namespace']}.data if block ~ ~ ~ iron_trapdoor[facing=south] run data modify entity @s Rotation[0] set value 0.0f
-	execute if score #rotation {config['namespace']}.data matches 0 store success score #rotation {config['namespace']}.data if block ~ ~ ~ iron_trapdoor[facing=west] run data modify entity @s Rotation[0] set value 90.0f
-	# No more cases for now
+# Add convention and utils tags, and the custom block tag
+tag @s add global.ignore
+tag @s add global.ignore.kill
+tag @s add smithed.entity
+tag @s add smithed.block
+tag @s add {config['namespace']}.custom_block
+tag @s add {config['namespace']}.{item}
+tag @s add {config['namespace']}.vanilla.{block}
+
+# Modify item display entity to match the custom block
+item replace entity @s container.0 with deepslate[minecraft:custom_model_data={custom_model_data}]
+data modify entity @s transformation.scale set value [1.002f,1.002f,1.002f]
+data modify entity @s brightness set value {{block:15,sky:15}}
+
+## Check if the block have rotation
+# Furnace case
+scoreboard players set #rotation {config['namespace']}.data 0
+execute if score #rotation {config['namespace']}.data matches 0 store success score #rotation {config['namespace']}.data if block ~ ~ ~ furnace[facing=north] run data modify entity @s Rotation[0] set value 180.0f
+execute if score #rotation {config['namespace']}.data matches 0 store success score #rotation {config['namespace']}.data if block ~ ~ ~ furnace[facing=east] run data modify entity @s Rotation[0] set value 270.0f
+execute if score #rotation {config['namespace']}.data matches 0 store success score #rotation {config['namespace']}.data if block ~ ~ ~ furnace[facing=south] run data modify entity @s Rotation[0] set value 0.0f
+execute if score #rotation {config['namespace']}.data matches 0 store success score #rotation {config['namespace']}.data if block ~ ~ ~ furnace[facing=west] run data modify entity @s Rotation[0] set value 90.0f
+# Iron trapdoor case
+execute if score #rotation {config['namespace']}.data matches 0 store success score #rotation {config['namespace']}.data if block ~ ~ ~ iron_trapdoor[facing=north] run data modify entity @s Rotation[0] set value 180.0f
+execute if score #rotation {config['namespace']}.data matches 0 store success score #rotation {config['namespace']}.data if block ~ ~ ~ iron_trapdoor[facing=east] run data modify entity @s Rotation[0] set value 270.0f
+execute if score #rotation {config['namespace']}.data matches 0 store success score #rotation {config['namespace']}.data if block ~ ~ ~ iron_trapdoor[facing=south] run data modify entity @s Rotation[0] set value 0.0f
+execute if score #rotation {config['namespace']}.data matches 0 store success score #rotation {config['namespace']}.data if block ~ ~ ~ iron_trapdoor[facing=west] run data modify entity @s Rotation[0] set value 90.0f
+# No more cases for now
 
-	"""
+"""
 			# Add the commands on placement if any
 			if COMMANDS_ON_PLACEMENT in data:
 				if isinstance(data[COMMANDS_ON_PLACEMENT], list):
 					content += "\n".join(data[COMMANDS_ON_PLACEMENT]) + "\n"
 				else:
 					content += f"{data[COMMANDS_ON_PLACEMENT]}\n"
 				
@@ -137,66 +137,66 @@
 			block = data[VANILLA_BLOCK]
 			path = f"{config['datapack_functions']}/custom_blocks/{item}"
 			if isinstance(block, dict):
 				block = block["id"]
 			
 			# Destroy function
 			content = f"""
-	# Replace the item with the custom one
-	execute as @e[type=item,nbt={{Item:{{id:"{block}"}}}},limit=1,sort=nearest,distance=..1] run function {config['namespace']}:custom_blocks/{item}/replace_item
-	"""
+# Replace the item with the custom one
+execute as @e[type=item,nbt={{Item:{{id:"{block}"}}}},limit=1,sort=nearest,distance=..1] run function {config['namespace']}:custom_blocks/{item}/replace_item
+"""
 			# Add the commands on break if any
 			if COMMANDS_ON_BREAK in data:
 				if isinstance(data[COMMANDS_ON_BREAK], list):
 					content += "\n".join(data[COMMANDS_ON_BREAK]) + "\n"
 				else:
 					content += f"{data[COMMANDS_ON_BREAK]}\n"
 			write_to_file(f"{path}/destroy.mcfunction", content + "\n# Kill the custom block entity\nkill @s\n\n")
 
 			# Replace item function
 			if block != VANILLA_BLOCK_FOR_ORES:
 				content = f"""
-	data modify entity @s Item.components set from storage {config['namespace']}:items all.{item}.components
-	data modify entity @s Item.id set from storage {config['namespace']}:items all.{item}.id
-	"""
+data modify entity @s Item.components set from storage {config['namespace']}:items all.{item}.components
+data modify entity @s Item.id set from storage {config['namespace']}:items all.{item}.id
+"""
 				"""
-	# Replace the item by the ore if the player is holding a silk touch pickaxe
-	execute if score #is_silk_touch simplenergy.data matches 1 run data modify entity @e[type=item,nbt={Item:{id:"minecraft:polished_deepslate"}},limit=1,sort=nearest,distance=..1] Item set from storage simplenergy:main all.deepslate_simplunium_ore
+# Replace the item by the ore if the player is holding a silk touch pickaxe
+execute if score #is_silk_touch simplenergy.data matches 1 run data modify entity @e[type=item,nbt={Item:{id:"minecraft:polished_deepslate"}},limit=1,sort=nearest,distance=..1] Item set from storage simplenergy:main all.deepslate_simplunium_ore
 
-	# Replace the item by the raw form if the player is not holding a silk touch pickaxe
-	execute if score #is_silk_touch simplenergy.data matches 0 run data modify entity @e[type=item,nbt={Item:{id:"minecraft:polished_deepslate"}},limit=1,sort=nearest,distance=..1] Item set from storage simplenergy:main all.raw_simplunium
-	execute if score #is_silk_touch simplenergy.data matches 0 run scoreboard players operation #count simplenergy.data = #item_count simplenergy.data
-	execute if score #is_silk_touch simplenergy.data matches 0 store result score #temp simplenergy.data run data get entity @s UUID[1]
-	execute if score #is_silk_touch simplenergy.data matches 0 run scoreboard players operation #temp simplenergy.data %= #4 simplenergy.data
-	execute if score #is_silk_touch simplenergy.data matches 0 run scoreboard players add #temp simplenergy.data 1
-	execute if score #is_silk_touch simplenergy.data matches 0 run scoreboard players operation #count simplenergy.data *= #temp simplenergy.data
-	execute if score #is_silk_touch simplenergy.data matches 0 store result entity @e[type=item,nbt={Age:0s,Item:{tag:{simplenergy:{raw_simplunium:1b}}}},limit=1,sort=nearest,distance=..1] Item.Count byte 1 run scoreboard players get #count simplenergy.data
+# Replace the item by the raw form if the player is not holding a silk touch pickaxe
+execute if score #is_silk_touch simplenergy.data matches 0 run data modify entity @e[type=item,nbt={Item:{id:"minecraft:polished_deepslate"}},limit=1,sort=nearest,distance=..1] Item set from storage simplenergy:main all.raw_simplunium
+execute if score #is_silk_touch simplenergy.data matches 0 run scoreboard players operation #count simplenergy.data = #item_count simplenergy.data
+execute if score #is_silk_touch simplenergy.data matches 0 store result score #temp simplenergy.data run data get entity @s UUID[1]
+execute if score #is_silk_touch simplenergy.data matches 0 run scoreboard players operation #temp simplenergy.data %= #4 simplenergy.data
+execute if score #is_silk_touch simplenergy.data matches 0 run scoreboard players add #temp simplenergy.data 1
+execute if score #is_silk_touch simplenergy.data matches 0 run scoreboard players operation #count simplenergy.data *= #temp simplenergy.data
+execute if score #is_silk_touch simplenergy.data matches 0 store result entity @e[type=item,nbt={Age:0s,Item:{tag:{simplenergy:{raw_simplunium:1b}}}},limit=1,sort=nearest,distance=..1] Item.Count byte 1 run scoreboard players get #count simplenergy.data
 
-	# Remove the block
-	kill @s
+# Remove the block
+kill @s
 
-	"""
+"""
 			else:
 				no_silk_touch_drop = data[NO_SILK_TOUCH_DROP]
 				if ':' in no_silk_touch_drop:
-					silk_text = f'execute if score #is_silk_touch {config['namespace']}.data matches 0 run data modify entity @s Item.id set value "{no_silk_touch_drop}"'
+					silk_text = f'execute if score #is_silk_touch {config["namespace"]}.data matches 0 run data modify entity @s Item.id set value "{no_silk_touch_drop}"'
 				else:
 					silk_text = f"execute if score #is_silk_touch {config['namespace']}.data matches 0 run data modify entity @s Item.id set from storage {config['namespace']}:items all.{no_silk_touch_drop}.id"
 					silk_text += f"\nexecute if score #is_silk_touch {config['namespace']}.data matches 0 run data modify entity @s Item.components set from storage {config['namespace']}:items all.{no_silk_touch_drop}.components"
 				content = f"""
-	# If silk touch applied
-	execute if score #is_silk_touch {config['namespace']}.data matches 1 run data modify entity @s Item.id set from storage {config['namespace']}:items all.{item}.id
-	execute if score #is_silk_touch {config['namespace']}.data matches 1 run data modify entity @s Item.components set from storage {config['namespace']}:items all.{item}.components
-
-	# Else, no silk touch
-	{silk_text}
-
-	# Get item count in every case
-	execute store result entity @s Item.count byte 1 run scoreboard players get #item_count {config['namespace']}.data
-	"""
+# If silk touch applied
+execute if score #is_silk_touch {config['namespace']}.data matches 1 run data modify entity @s Item.id set from storage {config['namespace']}:items all.{item}.id
+execute if score #is_silk_touch {config['namespace']}.data matches 1 run data modify entity @s Item.components set from storage {config['namespace']}:items all.{item}.components
+
+# Else, no silk touch
+{silk_text}
+
+# Get item count in every case
+execute store result entity @s Item.count byte 1 run scoreboard players get #item_count {config['namespace']}.data
+"""
 			write_to_file(f"{path}/replace_item.mcfunction", content)
 
 
 	# Write the used_vanilla_blocks tag, the predicate to check the blocks with the tag and an advanced one
 	VANILLA_BLOCKS_TAG = "used_vanilla_blocks"
 	write_to_file(f"{config['build_datapack']}/data/{config['namespace']}/tags/block/{VANILLA_BLOCKS_TAG}.json", super_json_dump({"values": list(unique_blocks)}))
 	predicate = {"condition": "minecraft:location_check", "predicate": {"block": {"blocks": f"#{config['namespace']}:{VANILLA_BLOCKS_TAG}"}}}
@@ -206,40 +206,40 @@
 		block_underscore = block.replace(":","_")
 		predicate = {"condition": "minecraft:entity_properties", "entity": "this", "predicate": { "nbt": f"{{Tags:[\"iyc.vanilla.{block_underscore}\"]}}", "location": { "block": { "blocks": [block] }}}}
 		advanced_predicate["terms"].append(predicate)
 	write_to_file(f"{config['build_datapack']}/data/{config['namespace']}/predicate/advanced_check_vanilla_blocks.json", super_json_dump(advanced_predicate))
 
 	# Write a destroy check every 2 ticks, every second, and every 5 seconds
 	write_to_file(f"{config['datapack_functions']}/tick_2.mcfunction", f"""
-	# 2 ticks destroy detection
-	execute as @e[type=item_display,tag={config['namespace']}.custom_block,tag=!{config['namespace']}.vanilla.{VANILLA_BLOCK_FOR_ORES.replace(':', '_')},predicate=!{config['namespace']}:check_vanilla_blocks] at @s run function {config['namespace']}:custom_blocks/destroy
-	""")
+# 2 ticks destroy detection
+execute as @e[type=item_display,tag={config['namespace']}.custom_block,tag=!{config['namespace']}.vanilla.{VANILLA_BLOCK_FOR_ORES.replace(':', '_')},predicate=!{config['namespace']}:check_vanilla_blocks] at @s run function {config['namespace']}:custom_blocks/destroy
+""")
 	write_to_file(f"{config['datapack_functions']}/second.mcfunction", f"""
-	# 1 second break detection
-	execute as @e[type=item_display,tag={config['namespace']}.custom_block,tag=!{config['namespace']}.vanilla.{VANILLA_BLOCK_FOR_ORES.replace(':', '_')},predicate=!{config['namespace']}:advanced_check_vanilla_blocks] at @s run function {config['namespace']}:custom_blocks/destroy
-	""")
+# 1 second break detection
+execute as @e[type=item_display,tag={config['namespace']}.custom_block,tag=!{config['namespace']}.vanilla.{VANILLA_BLOCK_FOR_ORES.replace(':', '_')},predicate=!{config['namespace']}:advanced_check_vanilla_blocks] at @s run function {config['namespace']}:custom_blocks/destroy
+""")
 	write_to_file(f"{config['datapack_functions']}/second_5.mcfunction", f"""
-	# 5 seconds break detection
-	execute as @e[type=item_display,tag={config['namespace']}.custom_block,predicate=!{config['namespace']}:advanced_check_vanilla_blocks] at @s run function {config['namespace']}:custom_blocks/destroy
-	""")
+# 5 seconds break detection
+execute as @e[type=item_display,tag={config['namespace']}.custom_block,predicate=!{config['namespace']}:advanced_check_vanilla_blocks] at @s run function {config['namespace']}:custom_blocks/destroy
+""")
 
 
 
 	## Custom ores break detection
 	write_to_file(f"{config['build_datapack']}/data/common_signals/tags/function/signals/on_new_item.json", super_json_dump({"values": [f"{config['namespace']}:calls/common_signals/new_item"]}))
 	write_to_file(f"{config['datapack_functions']}/calls/common_signals/new_item.mcfunction", f"""
-	# If the item is from a custom ore, launch the on_ore_destroyed function
-	execute if data entity @s Item.components.\"minecraft:custom_data\".common_signals.temp at @s align xyz run function {config['namespace']}:calls/common_signals/on_ore_destroyed
-	""")
+# If the item is from a custom ore, launch the on_ore_destroyed function
+execute if data entity @s Item.components.\"minecraft:custom_data\".common_signals.temp at @s align xyz run function {config['namespace']}:calls/common_signals/on_ore_destroyed
+""")
 	write_to_file(f"{config['datapack_functions']}/calls/common_signals/on_ore_destroyed.mcfunction", f"""
-	# Get in a score the item count and if it is a silk touch
-	scoreboard players set #item_count {config['namespace']}.data 0
-	scoreboard players set #is_silk_touch {config['namespace']}.data 0
-	execute store result score #item_count {config['namespace']}.data run data get entity @s Item.count
-	execute store success score #is_silk_touch {config['namespace']}.data if data entity @s Item.components."minecraft:custom_data".common_signals.silk_touch
-
-	# Try to destroy the block
-	execute as @e[tag={config['namespace']}.custom_block,dx=0,dy=0,dz=0] at @s run function {config['namespace']}:custom_blocks/destroy
-	""")
+# Get in a score the item count and if it is a silk touch
+scoreboard players set #item_count {config['namespace']}.data 0
+scoreboard players set #is_silk_touch {config['namespace']}.data 0
+execute store result score #item_count {config['namespace']}.data run data get entity @s Item.count
+execute store success score #is_silk_touch {config['namespace']}.data if data entity @s Item.components."minecraft:custom_data".common_signals.silk_touch
+
+# Try to destroy the block
+execute as @e[tag={config['namespace']}.custom_block,dx=0,dy=0,dz=0] at @s run function {config['namespace']}:custom_blocks/destroy
+""")
 
 	info("All customs blocks are now placeable and destroyable!")
```

### Comparing `python_datapack-0.0.3/src/python_datapack/datapack/headers.py` & `python_datapack-0.0.4/src/python_datapack/datapack/headers.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,17 +74,17 @@
 		# Get file content
 		content = FILES_TO_WRITE[data["path"]]
 		if not content.startswith("\n"):
 			content = "\n" + content
 		
 		# Prepare header
 		header: str = f"""
-	#> {file}
-	#
-	# @within\t"""
+#> {file}
+#
+# @within\t"""
 
 		# Get all the calling function and join them with new lines
 		withins = "\n#\t\t\t".join(w.strip() for w in data["within"])
 		if data["within"]:
 			header += withins + "\n#\n"
 		else:
 			header += "???\n#\n"
```

### Comparing `python_datapack-0.0.3/src/python_datapack/datapack/lang.py` & `python_datapack-0.0.4/src/python_datapack/datapack/lang.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.3/src/python_datapack/datapack/loading.py` & `python_datapack-0.0.4/src/python_datapack/datapack/loading.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,74 +12,74 @@
 	calls = [{"id":f"#{namespace}:load", "required": False} for namespace in config['dependencies'].keys()]
 	write_to_file(f"{config['build_datapack']}/data/{config['namespace']}/tags/function/load/dependencies.json", super_json_dump({"values": calls}))
 	write_to_file(f"{config['build_datapack']}/data/minecraft/tags/function/tick.json", super_json_dump({"values": [f"{config['namespace']}:load/tick_verification"]}))
 
 
 	# Setup load main and secondary function
 	write_to_file(f"{config['datapack_functions']}/load/main.mcfunction", f"""
-	# Avoiding multiple executions of the same load function
-	execute unless score {config['datapack_name_simple']} load.status matches 1.. run function {config['namespace']}:load/secondary
+# Avoiding multiple executions of the same load function
+execute unless score {config['datapack_name_simple']} load.status matches 1.. run function {config['namespace']}:load/secondary
 
-	""")
+""")
 	major, minor, patch = config['version'].split(".")
 	authors = config['author'].split(" ")
 	convention_debug = "".join([f"tag {author} add convention.debug\n" for author in authors])
 	content = f"""
-	# {config['datapack_name']}
-	scoreboard objectives add {config['namespace']}.data dummy
-	scoreboard players set #{config['namespace']}.major load.status {major}
-	scoreboard players set #{config['namespace']}.minor load.status {minor}
-	scoreboard players set #{config['namespace']}.patch load.status {patch}
-	{convention_debug}
-
-	# Check dependencies and wait for a player to connect (to get server version)
-	function {config['namespace']}:load/check_dependencies
-	function {config['namespace']}:load/waiting_for_player
+# {config['datapack_name']}
+scoreboard objectives add {config['namespace']}.data dummy
+scoreboard players set #{config['namespace']}.major load.status {major}
+scoreboard players set #{config['namespace']}.minor load.status {minor}
+scoreboard players set #{config['namespace']}.patch load.status {patch}
+{convention_debug}
+
+# Check dependencies and wait for a player to connect (to get server version)
+function {config['namespace']}:load/check_dependencies
+function {config['namespace']}:load/waiting_for_player
 
-	"""
+"""
 	write_to_file(f"{config['datapack_functions']}/load/secondary.mcfunction", content)
 
 
 	# Check dependencies
 	checks = ""
 	for namespace, value in config['dependencies'].items():
 		major, minor, patch = value["version"]
 		checks += f"execute if score #dependency_error {config['namespace']}.data matches 0 unless score #{namespace}.major load.status matches {major}.. unless score #{namespace}.minor load.status matches {minor}.. unless score #{namespace}.patch load.status matches {patch}.. run scoreboard players set #dependency_error {config['namespace']}.data 1\n"
 	content = f"""
-	## Check if {config['datapack_name']} is loadable (dependencies)
-	scoreboard players set #dependency_error {config['namespace']}.data 0"""
+## Check if {config['datapack_name']} is loadable (dependencies)
+scoreboard players set #dependency_error {config['namespace']}.data 0"""
 	content += "\n" + checks + "\n"
 	write_to_file(f"{config['datapack_functions']}/load/check_dependencies.mcfunction", content)
 
 
 	# Waiting for player
 	decoder_checks = ""
 	for namespace, value in config['dependencies'].items():
 		major, minor, patch = value["version"]
 		name = value["name"]
 		url = value["url"]
-		decoder_checks += f'execute if score #dependency_error {config['namespace']}.data matches 1 unless score #{namespace}.major load.status matches {major}.. unless score #{namespace}.minor load.status matches {minor}.. unless score #{namespace}.patch load.status matches {patch}.. run tellraw @a {{"text":"- [{name}]","color":"gold","clickEvent":{{"action":"open_url","value":"{url}"}}}}\n'
+		decoder_checks += f'execute if score #dependency_error {config["namespace"]}.data matches 1 unless score #{namespace}.major load.status matches {major}.. unless score #{namespace}.minor load.status matches {minor}.. unless score #{namespace}.patch load.status matches {patch}.. run tellraw @a {{"text":"- [{name}]","color":"gold","clickEvent":{{"action":"open_url","value":"{url}"}}}}\n'
 	write_to_file(f"{config['datapack_functions']}/load/waiting_for_player.mcfunction", f"""
-	# Waiting for a player to get the game version, but stop function if no player found
-	execute unless entity @p run schedule function {config['namespace']}:load/waiting_for_player 1t replace
-	execute unless entity @p run return 0
-	execute store result score #game_version {config['namespace']}.data run data get entity @p DataVersion
-
-	# Check if the game version is supported
-	scoreboard players set #mcload_error {config['namespace']}.data 0
-	execute unless score #game_version {config['namespace']}.data matches {config['data_version']}.. run scoreboard players set #mcload_error {config['namespace']}.data 1
-
-	# Decode errors
-	execute if score #mcload_error {config['namespace']}.data matches 1 run tellraw @a {{"text":"{config['datapack_name']} Error: This version is made for Minecraft {config['minecraft_version']}+.","color":"red"}}
-	execute if score #dependency_error {config['namespace']}.data matches 1 run tellraw @a {{"text":"{config['datapack_name']} Error: Libraries are missing\\nplease download the right {config['datapack_name']} datapack\\nor download each of these libraries one by one:","color":"red"}}
-	{decoder_checks}
-	# Load {config['datapack_name']}
-	execute if score #game_version {config['namespace']}.data matches 1.. if score #mcload_error {config['namespace']}.data matches 0 if score #dependency_error {config['namespace']}.data matches 0 run function {config['namespace']}:load/confirm_load
+# Waiting for a player to get the game version, but stop function if no player found
+execute unless entity @p run schedule function {config['namespace']}:load/waiting_for_player 1t replace
+execute unless entity @p run return 0
+execute store result score #game_version {config['namespace']}.data run data get entity @p DataVersion
+
+# Check if the game version is supported
+scoreboard players set #mcload_error {config['namespace']}.data 0
+execute unless score #game_version {config['namespace']}.data matches {config['data_version']}.. run scoreboard players set #mcload_error {config['namespace']}.data 1
+
+# Decode errors
+execute if score #mcload_error {config['namespace']}.data matches 1 run tellraw @a {{"text":"{config['datapack_name']} Error: This version is made for Minecraft {config['minecraft_version']}+.","color":"red"}}
+execute if score #dependency_error {config['namespace']}.data matches 1 run tellraw @a {{"text":"{config['datapack_name']} Error: Libraries are missing\\nplease download the right {config['datapack_name']} datapack\\nor download each of these libraries one by one:","color":"red"}}
+{decoder_checks}
+# Load {config['datapack_name']}
+execute if score #game_version {config['namespace']}.data matches 1.. if score #mcload_error {config['namespace']}.data matches 0 if score #dependency_error {config['namespace']}.data matches 0 run function {config['namespace']}:load/confirm_load
 
-	""")
+""")
 
 
 	# Confirm load
 	items_storage = ""	# Storage representation of every item in the database
 	content = ""
 	for item, data in config['database'].items():
 		mc_data = {"id":"","count":1, "components":{"custom_model_data":-1}}
@@ -88,29 +88,29 @@
 				mc_data["components"][k] = v
 			elif k == "id":
 				mc_data[k] = v
 		items_storage += f"data modify storage {config['namespace']}:items all.{item} set value " + super_json_dump(mc_data, max_level = 0)
 		pass
 
 	write_to_file(f"{config['datapack_functions']}/load/confirm_load.mcfunction", f"""
-	tellraw @a[tag=convention.debug] {{"text":"[Loaded {config['datapack_name']} v{config['version']}]","color":"green"}}
+tellraw @a[tag=convention.debug] {{"text":"[Loaded {config['datapack_name']} v{config['version']}]","color":"green"}}
 
-	scoreboard objectives add {config['namespace']}.private dummy
-	scoreboard objectives add {config['namespace']}.right_click minecraft.used:minecraft.warped_fungus_on_a_stick
+scoreboard objectives add {config['namespace']}.private dummy
+scoreboard objectives add {config['namespace']}.right_click minecraft.used:minecraft.warped_fungus_on_a_stick
 
-	scoreboard players set #{config['namespace']}.loaded load.status 1
-	# "#second" starts at a random time for better load distribution
-	execute store result score #second {config['namespace']}.data run random value 1..19
-
-	# Items storage
-	data modify storage {config['namespace']}:items all set value {{}}
-	{items_storage}
-	""")
+scoreboard players set #{config['namespace']}.loaded load.status 1
+# "#second" starts at a random time for better load distribution
+execute store result score #second {config['namespace']}.data run random value 1..19
+
+# Items storage
+data modify storage {config['namespace']}:items all set value {{}}
+{items_storage}
+""")
 
 
 	# Tick verification
 	write_to_file(f"{config['datapack_functions']}/load/tick_verification.mcfunction", f"""
-	execute if score #{config['namespace']}.loaded load.status matches 1 run function {config['namespace']}:tick
+execute if score #{config['namespace']}.loaded load.status matches 1 run function {config['namespace']}:tick
 
-	""")
+""")
 	info("All loading functions and tags created")
```

### Comparing `python_datapack-0.0.3/src/python_datapack/datapack/loot_tables.py` & `python_datapack-0.0.4/src/python_datapack/datapack/loot_tables.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.3/src/python_datapack/datapack/main.py` & `python_datapack-0.0.4/src/python_datapack/datapack/main.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.3/src/python_datapack/datapack/recipes.py` & `python_datapack-0.0.4/src/python_datapack/datapack/recipes.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.3/src/python_datapack/manual/book_optimizer.py` & `python_datapack-0.0.4/src/python_datapack/manual/book_optimizer.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.3/src/python_datapack/manual/main.py` & `python_datapack-0.0.4/src/python_datapack/manual/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,20 +18,20 @@
 	MAX_ITEMS_PER_PAGE = config['max_items_per_row'] * config['max_rows_per_page'] # (for showing up all items in the categories pages)
 
 	# Calculate left padding for categories pages depending on config['max_items_per_row']: higher the value, lower the padding
 	LEFT_PADDING = 6 - config['max_items_per_row']
 
 	# Copy assets in the resource pack
 	if not config['debug_mode']:
-		super_copy(f"{MANUAL_ASSETS_PATH}/none_release.png", f"{config['build_resource_pack']}/assets/{config['namespace']}/textures/font/none.png")
+		super_copy(f"{TEMPLATES_PATH}/none_release.png", f"{config['build_resource_pack']}/assets/{config['namespace']}/textures/font/none.png")
 	else:
-		super_copy(f"{MANUAL_ASSETS_PATH}/none.png", f"{config['build_resource_pack']}/assets/{config['namespace']}/textures/font/none.png")
-	super_copy(f"{MANUAL_ASSETS_PATH}/wiki_information.png", f"{config['build_resource_pack']}/assets/{config['namespace']}/textures/font/wiki_information.png")
-	super_copy(f"{MANUAL_ASSETS_PATH}/wiki_result_of_craft.png", f"{config['build_resource_pack']}/assets/{config['namespace']}/textures/font/wiki_result_of_craft.png")
-	super_copy(f"{MANUAL_ASSETS_PATH}/wiki_ingredient_of_craft.png", f"{config['build_resource_pack']}/assets/{config['namespace']}/textures/font/wiki_ingredient_of_craft.png")
+		super_copy(f"{TEMPLATES_PATH}/none.png", f"{config['build_resource_pack']}/assets/{config['namespace']}/textures/font/none.png")
+	super_copy(f"{TEMPLATES_PATH}/wiki_information.png", f"{config['build_resource_pack']}/assets/{config['namespace']}/textures/font/wiki_information.png")
+	super_copy(f"{TEMPLATES_PATH}/wiki_result_of_craft.png", f"{config['build_resource_pack']}/assets/{config['namespace']}/textures/font/wiki_result_of_craft.png")
+	super_copy(f"{TEMPLATES_PATH}/wiki_ingredient_of_craft.png", f"{config['build_resource_pack']}/assets/{config['namespace']}/textures/font/wiki_ingredient_of_craft.png")
 
 
 	# If the manual cache is enabled and we have a cache file, load it
 	if config['cache_manual_pages'] and os.path.exists(config['manual_debug']):
 		with super_open(config['manual_debug'], "r") as f:
 			book_content = json.load(f)
 
@@ -403,14 +403,14 @@
 			"enchantment_glint_override": False,
 		}
 	}
 	config['database'].update(manual_database)
 
 	# Add the model to the resource pack
 	from ..resource_pack.item_models import handle_item
-	handle_item("manual", config['database']["manual"])
+	handle_item(config, "manual", config['database']["manual"])
 	vanilla_model = {"parent": "item/handheld","textures": {"layer0": "item/written_book"},"overrides": [{ "predicate": { "custom_model_data": manual_cmd}, "model": f"{config['namespace']}:item/manual" }]}
 	vanilla_model = super_json_dump(vanilla_model).replace('{"','{ "').replace('"}','" }').replace(',"', ', "')
 	write_to_file(f"{config['build_resource_pack']}/assets/minecraft/models/item/written_book.json", vanilla_model)
 
 	info(f"Added manual to the database")
```

### Comparing `python_datapack-0.0.3/src/python_datapack/manual/shared_import.py` & `python_datapack-0.0.4/src/python_datapack/manual/shared_import.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.3/src/python_datapack/manual/utils.py` & `python_datapack-0.0.4/src/python_datapack/manual/utils.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.3/src/python_datapack/manual/assets/furnace.png` & `python_datapack-0.0.4/src/python_datapack/manual/assets/furnace.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.3/src/python_datapack/manual/assets/minecraft_font.ttf` & `python_datapack-0.0.4/src/python_datapack/manual/assets/minecraft_font.ttf`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.3/src/python_datapack/manual/assets/shaped_2x2.png` & `python_datapack-0.0.4/src/python_datapack/manual/assets/shaped_2x2.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.3/src/python_datapack/manual/assets/shaped_3x3.png` & `python_datapack-0.0.4/src/python_datapack/manual/assets/shaped_3x3.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.3/src/python_datapack/manual/assets/simple_case_no_border.png` & `python_datapack-0.0.4/src/python_datapack/manual/assets/simple_case_no_border.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.3/src/python_datapack/manual/assets/wiki_information.png` & `python_datapack-0.0.4/src/python_datapack/manual/assets/wiki_information.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.3/src/python_datapack/manual/assets/wiki_ingredient_of_craft.png` & `python_datapack-0.0.4/src/python_datapack/manual/assets/wiki_ingredient_of_craft.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.3/src/python_datapack/manual/assets/wiki_ingredient_of_craft_template.png` & `python_datapack-0.0.4/src/python_datapack/manual/assets/wiki_ingredient_of_craft_template.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.3/src/python_datapack/manual/assets/wiki_result_of_craft.png` & `python_datapack-0.0.4/src/python_datapack/manual/assets/wiki_result_of_craft.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.3/src/python_datapack/resource_pack/check_unused_textures.py` & `python_datapack-0.0.4/src/python_datapack/resource_pack/check_unused_textures.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.3/src/python_datapack/resource_pack/item_models.py` & `python_datapack-0.0.4/src/python_datapack/resource_pack/item_models.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.3/src/python_datapack/resource_pack/sounds.py` & `python_datapack-0.0.4/src/python_datapack/resource_pack/sounds.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.3/src/python_datapack/resource_pack/vanilla_models.py` & `python_datapack-0.0.4/src/python_datapack/resource_pack/vanilla_models.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.3/src/python_datapack/utils/database_helper.py` & `python_datapack-0.0.4/src/python_datapack/utils/database_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,19 +110,19 @@
 		NOT_ON_TOOLS = ["generic.armor", "generic.armor_toughness"]
 		return {key: value for key, value in self.attributes.items() if key not in NOT_ON_TOOLS}
 	def get_armor_attributes(self) -> dict[str, float]:
 		NOT_ON_ARMOR = ["generic.attack_damage", "player.mining_efficiency"]
 		return {key: value for key, value in self.attributes.items() if key not in NOT_ON_ARMOR}
 
 # UUIDs utils
-def format_attributes(attributes: str, slot: str, config: dict = {}) -> list[dict]:
+def format_attributes(config: dict, attributes: str, slot: str, attr_config: dict = {}) -> list[dict]:
 	""" Returns generated attribute_modifiers key for an item (adds up attributes and config) """
 	# Get attributes from config
 	attribute_modifiers = []
-	for attribute_name, value in config.items():
+	for attribute_name, value in attr_config.items():
 		if attribute_name != "durability":
 			attribute_modifiers.append({"type": attribute_name, "amount": value, "operation": "add_value", "slot": slot, "id": f"{config['namespace']}:{attribute_name}.{slot}"})
 
 	# For each attribute, add it to the list if not in, else add the value
 	for attribute_name, value in attributes.items():
 		found = False
 		for attribute in attribute_modifiers:
@@ -251,15 +251,15 @@
 			database[armor][RESULT_OF_CRAFTING] = [{"type":"crafting_shaped","result_count":1,"category":"equipment","shape":["XXX","X X","X X"],"ingredients":{"X": main_ingredient}}]
 			gear_config = VanillaEquipments.LEGGINGS.value[equivalent_to]
 			database[armor]["max_damage"] = int(gear_config["durability"] * durability_factor)
 		elif gear == "boots":
 			database[armor][RESULT_OF_CRAFTING] = [{"type":"crafting_shaped","result_count":1,"category":"equipment","shape":["X X","X X"],"ingredients":{"X": main_ingredient}}]
 			gear_config = VanillaEquipments.BOOTS.value[equivalent_to]
 			database[armor]["max_damage"] = int(gear_config["durability"] * durability_factor)
-		database[armor]["attribute_modifiers"] = format_attributes(armor_attributes, SLOTS[gear], gear_config)
+		database[armor]["attribute_modifiers"] = format_attributes(config, armor_attributes, SLOTS[gear], gear_config)
 	
 	# Tools (sword, pickaxe, axe, shovel, hoe)
 	for gear in ["sword", "pickaxe", "axe", "shovel", "hoe"]:
 		tool = material_base + "_" + gear
 		if tool + ".png" not in config['textures_files']:
 			continue
 		if tool not in database:
@@ -286,29 +286,29 @@
 			gear_config = VanillaEquipments.SHOVEL.value[equivalent_to]
 			database[tool]["max_damage"] = int(gear_config["durability"] * durability_factor)
 			database[tool][RESULT_OF_CRAFTING] = [{"type":"crafting_shaped","result_count":1,"category":"equipment","shape":["X","S","S"],"ingredients": tools_ingr}]
 		elif gear == "hoe":
 			gear_config = VanillaEquipments.HOE.value[equivalent_to]
 			database[tool]["max_damage"] = int(gear_config["durability"] * durability_factor)
 			database[tool][RESULT_OF_CRAFTING] = [{"type":"crafting_shaped","result_count":1,"category":"equipment","shape":["XX"," S"," S"],"ingredients": tools_ingr}]
-		database[tool]["attribute_modifiers"] = format_attributes(tools_attributes, SLOTS[gear], gear_config)
+		database[tool]["attribute_modifiers"] = format_attributes(config, tools_attributes, SLOTS[gear], gear_config)
 	pass
 
 # Generate everything about these ores
-def generate_everything_about_these_ores(database: dict[str, dict], ores: dict[str, EquipmentsConfig|None]) -> dict[str, list[str]]:
+def generate_everything_about_these_ores(config: dict, database: dict[str, dict], ores: dict[str, EquipmentsConfig|None]) -> dict[str, list[str]]:
 	""" Uses function 'generate_everything_about_this_ore' for each ore in the ores dictionary.
 	Args:
 		database	(dict[str, dict]):	The database to apply the ores to.
 		ores		(dict[str, EquipmentsConfig|None]):	The ores to apply.
 	Returns:
 		dict[str, list[str]]:	The list of generated items for each ore.
 	"""
 	generated_items = {}
-	for material, config in ores.items():
-		generated_items[material] = generate_everything_about_this_ore(database, material, config)
+	for material, ore_config in ores.items():
+		generated_items[material] = generate_everything_about_this_ore(config, database, material, ore_config)
 	return generated_items
 
 
 
 # Custom records
 def generate_custom_records(config: dict, database: dict[str, dict], records: dict[str, tuple[str,float]], category: str|None = None) -> None:
 	""" Generate custom records by searching in config['assets_folder']/records/ for the files and copying them to the database and resource pack folder.
```

### Comparing `python_datapack-0.0.3/src/python_datapack/utils/ingredients.py` & `python_datapack-0.0.4/src/python_datapack/utils/ingredients.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.3/src/python_datapack/utils/io.py` & `python_datapack-0.0.4/src/python_datapack/utils/io.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.3/src/python_datapack/utils/multiprocessing.py` & `python_datapack-0.0.4/src/python_datapack/utils/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.3/src/python_datapack/utils/print.py` & `python_datapack-0.0.4/src/python_datapack/utils/print.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.3/src/python_datapack/utils/weld.py` & `python_datapack-0.0.4/src/python_datapack/utils/weld.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.3/LICENSE` & `python_datapack-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.3/pyproject.toml` & `python_datapack-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["hatchling", "pillow", "smithed"]
 build-backend = "hatchling.build"
 
 [project]
 name = "python_datapack"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
 	{ name="Stoupy51", email="stoupy51@gmail.com" },
 ]
 description = "Python package to help generating advanced Minecraft datapack contents"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `python_datapack-0.0.3/PKG-INFO` & `python_datapack-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: python_datapack
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python package to help generating advanced Minecraft datapack contents
 Project-URL: Homepage, https://github.com/Stoupy51/python_datapack
 Project-URL: Issues, https://github.com/Stoupy51/python_datapack/issues
 Author-email: Stoupy51 <stoupy51@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

