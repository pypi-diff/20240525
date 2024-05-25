# Comparing `tmp/python_datapack-0.1.0.tar.gz` & `tmp/python_datapack-0.1.1.tar.gz`

## Comparing `python_datapack-0.1.0.tar` & `python_datapack-0.1.1.tar`

### file list

```diff
@@ -1,50 +1,51 @@
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 python_datapack-0.1.0/1_upgrades.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 python_datapack-0.1.0/2_build.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 python_datapack-0.1.0/3_upload.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 python_datapack-0.1.0/build_all_in_one.py
--rw-r--r--   0        0        0     8141 2020-02-02 00:00:00.000000 python_datapack-0.1.0/src/python_datapack/__init__.py
--rw-r--r--   0        0        0     2997 2020-02-02 00:00:00.000000 python_datapack-0.1.0/src/python_datapack/constants.py
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 python_datapack-0.1.0/src/python_datapack/enhance_config.py
--rw-r--r--   0        0        0     3874 2020-02-02 00:00:00.000000 python_datapack-0.1.0/src/python_datapack/finalyze.py
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 python_datapack-0.1.0/src/python_datapack/initialize.py
--rw-r--r--   0        0        0    10662 2020-02-02 00:00:00.000000 python_datapack-0.1.0/src/python_datapack/verify_database.py
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 python_datapack-0.1.0/src/python_datapack/datapack/basic_structure.py
--rw-r--r--   0        0        0    14581 2020-02-02 00:00:00.000000 python_datapack-0.1.0/src/python_datapack/datapack/custom_blocks.py
--rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 python_datapack-0.1.0/src/python_datapack/datapack/headers.py
--rw-r--r--   0        0        0     4134 2020-02-02 00:00:00.000000 python_datapack-0.1.0/src/python_datapack/datapack/lang.py
--rw-r--r--   0        0        0     6408 2020-02-02 00:00:00.000000 python_datapack-0.1.0/src/python_datapack/datapack/loading.py
--rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 python_datapack-0.1.0/src/python_datapack/datapack/loot_tables.py
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 python_datapack-0.1.0/src/python_datapack/datapack/main.py
--rw-r--r--   0        0        0     3942 2020-02-02 00:00:00.000000 python_datapack-0.1.0/src/python_datapack/datapack/recipes.py
--rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 python_datapack-0.1.0/src/python_datapack/manual/book_optimizer.py
--rw-r--r--   0        0        0    19193 2020-02-02 00:00:00.000000 python_datapack-0.1.0/src/python_datapack/manual/main.py
--rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 python_datapack-0.1.0/src/python_datapack/manual/shared_import.py
--rw-r--r--   0        0        0    25039 2020-02-02 00:00:00.000000 python_datapack-0.1.0/src/python_datapack/manual/utils.py
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 python_datapack-0.1.0/src/python_datapack/manual/assets/furnace.png
--rw-r--r--   0        0        0    42432 2020-02-02 00:00:00.000000 python_datapack-0.1.0/src/python_datapack/manual/assets/minecraft_font.ttf
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 python_datapack-0.1.0/src/python_datapack/manual/assets/none.png
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 python_datapack-0.1.0/src/python_datapack/manual/assets/none_release.png
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 python_datapack-0.1.0/src/python_datapack/manual/assets/shaped_2x2.png
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 python_datapack-0.1.0/src/python_datapack/manual/assets/shaped_3x3.png
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 python_datapack-0.1.0/src/python_datapack/manual/assets/simple_case_no_border.png
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 python_datapack-0.1.0/src/python_datapack/manual/assets/wiki_information.png
--rw-r--r--   0        0        0     3483 2020-02-02 00:00:00.000000 python_datapack-0.1.0/src/python_datapack/manual/assets/wiki_ingredient_of_craft.png
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 python_datapack-0.1.0/src/python_datapack/manual/assets/wiki_ingredient_of_craft_template.png
--rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 python_datapack-0.1.0/src/python_datapack/manual/assets/wiki_result_of_craft.png
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 python_datapack-0.1.0/src/python_datapack/resource_pack/check_unused_textures.py
--rw-r--r--   0        0        0     4497 2020-02-02 00:00:00.000000 python_datapack-0.1.0/src/python_datapack/resource_pack/item_models.py
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 python_datapack-0.1.0/src/python_datapack/resource_pack/main.py
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 python_datapack-0.1.0/src/python_datapack/resource_pack/sounds.py
--rw-r--r--   0        0        0     2787 2020-02-02 00:00:00.000000 python_datapack-0.1.0/src/python_datapack/resource_pack/vanilla_models.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 python_datapack-0.1.0/src/python_datapack/utils/cache.py
--rw-r--r--   0        0        0    28262 2020-02-02 00:00:00.000000 python_datapack-0.1.0/src/python_datapack/utils/database_helper.py
--rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 python_datapack-0.1.0/src/python_datapack/utils/ingredients.py
--rw-r--r--   0        0        0     4809 2020-02-02 00:00:00.000000 python_datapack-0.1.0/src/python_datapack/utils/io.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 python_datapack-0.1.0/src/python_datapack/utils/multiprocessing.py
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 python_datapack-0.1.0/src/python_datapack/utils/print.py
--rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 python_datapack-0.1.0/src/python_datapack/utils/weld.py
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 python_datapack-0.1.0/.gitignore
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 python_datapack-0.1.0/LICENSE
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 python_datapack-0.1.0/README.md
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 python_datapack-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 python_datapack-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 python_datapack-0.1.1/1_upgrades.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 python_datapack-0.1.1/2_build.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 python_datapack-0.1.1/3_upload.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 python_datapack-0.1.1/build_all_in_one.py
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 python_datapack-0.1.1/copy_in_local.py
+-rw-r--r--   0        0        0     8141 2020-02-02 00:00:00.000000 python_datapack-0.1.1/src/python_datapack/__init__.py
+-rw-r--r--   0        0        0     2997 2020-02-02 00:00:00.000000 python_datapack-0.1.1/src/python_datapack/constants.py
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 python_datapack-0.1.1/src/python_datapack/enhance_config.py
+-rw-r--r--   0        0        0     3874 2020-02-02 00:00:00.000000 python_datapack-0.1.1/src/python_datapack/finalyze.py
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 python_datapack-0.1.1/src/python_datapack/initialize.py
+-rw-r--r--   0        0        0    10662 2020-02-02 00:00:00.000000 python_datapack-0.1.1/src/python_datapack/verify_database.py
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 python_datapack-0.1.1/src/python_datapack/datapack/basic_structure.py
+-rw-r--r--   0        0        0    14581 2020-02-02 00:00:00.000000 python_datapack-0.1.1/src/python_datapack/datapack/custom_blocks.py
+-rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 python_datapack-0.1.1/src/python_datapack/datapack/headers.py
+-rw-r--r--   0        0        0     4134 2020-02-02 00:00:00.000000 python_datapack-0.1.1/src/python_datapack/datapack/lang.py
+-rw-r--r--   0        0        0     6408 2020-02-02 00:00:00.000000 python_datapack-0.1.1/src/python_datapack/datapack/loading.py
+-rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 python_datapack-0.1.1/src/python_datapack/datapack/loot_tables.py
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 python_datapack-0.1.1/src/python_datapack/datapack/main.py
+-rw-r--r--   0        0        0     3942 2020-02-02 00:00:00.000000 python_datapack-0.1.1/src/python_datapack/datapack/recipes.py
+-rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 python_datapack-0.1.1/src/python_datapack/manual/book_optimizer.py
+-rw-r--r--   0        0        0    19193 2020-02-02 00:00:00.000000 python_datapack-0.1.1/src/python_datapack/manual/main.py
+-rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 python_datapack-0.1.1/src/python_datapack/manual/shared_import.py
+-rw-r--r--   0        0        0    24334 2020-02-02 00:00:00.000000 python_datapack-0.1.1/src/python_datapack/manual/utils.py
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 python_datapack-0.1.1/src/python_datapack/manual/assets/furnace.png
+-rw-r--r--   0        0        0    42432 2020-02-02 00:00:00.000000 python_datapack-0.1.1/src/python_datapack/manual/assets/minecraft_font.ttf
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 python_datapack-0.1.1/src/python_datapack/manual/assets/none.png
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 python_datapack-0.1.1/src/python_datapack/manual/assets/none_release.png
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 python_datapack-0.1.1/src/python_datapack/manual/assets/shaped_2x2.png
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 python_datapack-0.1.1/src/python_datapack/manual/assets/shaped_3x3.png
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 python_datapack-0.1.1/src/python_datapack/manual/assets/simple_case_no_border.png
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 python_datapack-0.1.1/src/python_datapack/manual/assets/wiki_information.png
+-rw-r--r--   0        0        0     3483 2020-02-02 00:00:00.000000 python_datapack-0.1.1/src/python_datapack/manual/assets/wiki_ingredient_of_craft.png
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 python_datapack-0.1.1/src/python_datapack/manual/assets/wiki_ingredient_of_craft_template.png
+-rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 python_datapack-0.1.1/src/python_datapack/manual/assets/wiki_result_of_craft.png
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 python_datapack-0.1.1/src/python_datapack/resource_pack/check_unused_textures.py
+-rw-r--r--   0        0        0     4497 2020-02-02 00:00:00.000000 python_datapack-0.1.1/src/python_datapack/resource_pack/item_models.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 python_datapack-0.1.1/src/python_datapack/resource_pack/main.py
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 python_datapack-0.1.1/src/python_datapack/resource_pack/sounds.py
+-rw-r--r--   0        0        0     2787 2020-02-02 00:00:00.000000 python_datapack-0.1.1/src/python_datapack/resource_pack/vanilla_models.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 python_datapack-0.1.1/src/python_datapack/utils/cache.py
+-rw-r--r--   0        0        0    28262 2020-02-02 00:00:00.000000 python_datapack-0.1.1/src/python_datapack/utils/database_helper.py
+-rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 python_datapack-0.1.1/src/python_datapack/utils/ingredients.py
+-rw-r--r--   0        0        0     4911 2020-02-02 00:00:00.000000 python_datapack-0.1.1/src/python_datapack/utils/io.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 python_datapack-0.1.1/src/python_datapack/utils/multiprocessing.py
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 python_datapack-0.1.1/src/python_datapack/utils/print.py
+-rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 python_datapack-0.1.1/src/python_datapack/utils/weld.py
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 python_datapack-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 python_datapack-0.1.1/LICENSE
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 python_datapack-0.1.1/README.md
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 python_datapack-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 python_datapack-0.1.1/PKG-INFO
```

### Comparing `python_datapack-0.1.0/src/python_datapack/__init__.py` & `python_datapack-0.1.1/src/python_datapack/__init__.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.0/src/python_datapack/constants.py` & `python_datapack-0.1.1/src/python_datapack/constants.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.0/src/python_datapack/enhance_config.py` & `python_datapack-0.1.1/src/python_datapack/enhance_config.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.0/src/python_datapack/finalyze.py` & `python_datapack-0.1.1/src/python_datapack/finalyze.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.0/src/python_datapack/initialize.py` & `python_datapack-0.1.1/src/python_datapack/initialize.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.0/src/python_datapack/verify_database.py` & `python_datapack-0.1.1/src/python_datapack/verify_database.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.0/src/python_datapack/datapack/basic_structure.py` & `python_datapack-0.1.1/src/python_datapack/datapack/basic_structure.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.0/src/python_datapack/datapack/custom_blocks.py` & `python_datapack-0.1.1/src/python_datapack/datapack/custom_blocks.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.0/src/python_datapack/datapack/headers.py` & `python_datapack-0.1.1/src/python_datapack/datapack/headers.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.0/src/python_datapack/datapack/lang.py` & `python_datapack-0.1.1/src/python_datapack/datapack/lang.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.0/src/python_datapack/datapack/loading.py` & `python_datapack-0.1.1/src/python_datapack/datapack/loading.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.0/src/python_datapack/datapack/loot_tables.py` & `python_datapack-0.1.1/src/python_datapack/datapack/loot_tables.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.0/src/python_datapack/datapack/main.py` & `python_datapack-0.1.1/src/python_datapack/datapack/main.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.0/src/python_datapack/datapack/recipes.py` & `python_datapack-0.1.1/src/python_datapack/datapack/recipes.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.0/src/python_datapack/manual/book_optimizer.py` & `python_datapack-0.1.1/src/python_datapack/manual/book_optimizer.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.0/src/python_datapack/manual/main.py` & `python_datapack-0.1.1/src/python_datapack/manual/main.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.0/src/python_datapack/manual/shared_import.py` & `python_datapack-0.1.1/src/python_datapack/manual/shared_import.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.0/src/python_datapack/manual/utils.py` & `python_datapack-0.1.1/src/python_datapack/manual/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 # Imports & font textures
 from ..utils.io import *
 from ..utils.print import *
 from ..utils.cache import simple_cache
 from ..utils.ingredients import *
 from ..constants import *
 from .shared_import import *
+from pathlib import Path
 from PIL import Image, ImageDraw, ImageFont
+from model_resolver.cli import main as model_resolver_main
 import requests
 
 # Generate a border for a given Image
 def add_border(image: Image.Image, border_color: tuple, border_size: int, is_rectangle_shape: bool) -> Image.Image:
 	""" Add a border to every part of the image
 	Args:
 		image				(Image):	The image to add the border
@@ -83,64 +85,46 @@
 	draw.text(pos_2, str(count), (255, 255, 255), font = font)
 	return img
 
 # Generate iso renders for every item in the config['database']
 def generate_all_iso_renders(config: dict):
 	path = config['manual_path'] + "/items"
 	os.makedirs(f"{path}/{config['namespace']}", exist_ok = True)
+	for_model_resolver = {}
 	for item, data in config['database'].items():
 		
 		# If it's not a block, simply copy the texture
 		try:
 			if data["id"] == CUSTOM_BLOCK_VANILLA:
 				raise Exception()
 			if not os.path.exists(f"{path}/{config['namespace']}/{item}.png") or not config['cache_manual_assets']:
 				super_copy(f"{config['textures_folder']}/{item}.png", f"{path}/{config['namespace']}/{item}.png")
 		except:
-			# Else, render all the block textures and faces
-			try:
-				# Skip if item is already generated (to prevent launcher OpenGL for nothing)
-				if os.path.exists(f"{path}/{config['namespace']}/{item}.png") and config['cache_manual_assets']:
-					continue
-
-				# # Load front texture
-				# sides = ("_front", "_side", "_top", "_bottom", "")
-				# front_path = f"{config['textures_folder']}/{item}"
-				# for side in sides:
-				# 	if os.path.exists(f"{front_path}{side}.png"):
-				# 		front_path += side
-				# 		break
-				# front_texture = Image.open(front_path + ".png")
-				# side_texture = front_texture
-				# top_texture = front_texture
-
-				# # Try to load side
-				# side_path = f"{config['textures_folder']}/{item}_side.png"
-				# if os.path.exists(side_path):
-				# 	side_texture = Image.open(side_path)
-				
-				# # Try to load top texture
-				# top_path = f"{config['textures_folder']}/{item}_top.png"
-				# if os.path.exists(top_path):
-				# 	top_texture = Image.open(top_path)
-				
-				# # Make front texture 50% darker and side texture 25% darker
-				# front_texture = ImageEnhance.Brightness(front_texture).enhance(0.5)
-				# side_texture = ImageEnhance.Brightness(side_texture).enhance(0.75)
-
-				# # Render block and take a screenshot
-				# opengl.render_block(front_texture, side_texture, top_texture)
-				# opengl.take_screenshot(f"{path}/{config['namespace']}/{item}.png")
-				error("TODO")
-
-			except:
-				try:
-					super_copy(f"{config['textures_folder']}/{item}.png", f"{path}/{config['namespace']}/{item}.png")
-				except:
-					error(f"Failed to render iso for item '{item}', please add it manually to '{path}/{config['namespace']}/{item}.png'")
+			# Else, add the block to the model resolver list
+			# Skip if item is already generated (to prevent launcher OpenGL for nothing)
+			if os.path.exists(f"{path}/{config['namespace']}/{item}.png") and config['cache_manual_assets']:
+				continue
+
+			# Add to the model resolver queue
+			rp_path = f"{config['namespace']}:block/{item}"
+			dst_path = f"{path}/{config['namespace']}/{item}.png"
+			for_model_resolver[rp_path] = dst_path
+
+	# Launch model resolvers for remaining blocks
+	if len(for_model_resolver) > 0:
+		load_dir = Path(config['build_resource_pack'])
+		debug("Generating iso renders for %d items" % len(for_model_resolver))
+		model_resolver_main(
+			render_size = config['opengl_resolution'],
+			load_dir = load_dir,
+			output_dir = None,
+			use_cache = False,
+			minecraft_version = "latest",
+			__special_filter__ = for_model_resolver
+		)
 	debug("Generated iso renders for all items, or used cached renders")
 
 	## Copy every used vanilla items
 	# Get every used vanilla items
 	used_vanilla_items = set()
 	for item, data in config['database'].items():
 		all_crafts = []
```

### Comparing `python_datapack-0.1.0/src/python_datapack/manual/assets/furnace.png` & `python_datapack-0.1.1/src/python_datapack/manual/assets/furnace.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.0/src/python_datapack/manual/assets/minecraft_font.ttf` & `python_datapack-0.1.1/src/python_datapack/manual/assets/minecraft_font.ttf`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.0/src/python_datapack/manual/assets/shaped_2x2.png` & `python_datapack-0.1.1/src/python_datapack/manual/assets/shaped_2x2.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.0/src/python_datapack/manual/assets/shaped_3x3.png` & `python_datapack-0.1.1/src/python_datapack/manual/assets/shaped_3x3.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.0/src/python_datapack/manual/assets/simple_case_no_border.png` & `python_datapack-0.1.1/src/python_datapack/manual/assets/simple_case_no_border.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.0/src/python_datapack/manual/assets/wiki_information.png` & `python_datapack-0.1.1/src/python_datapack/manual/assets/wiki_information.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.0/src/python_datapack/manual/assets/wiki_ingredient_of_craft.png` & `python_datapack-0.1.1/src/python_datapack/manual/assets/wiki_ingredient_of_craft.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.0/src/python_datapack/manual/assets/wiki_ingredient_of_craft_template.png` & `python_datapack-0.1.1/src/python_datapack/manual/assets/wiki_ingredient_of_craft_template.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.0/src/python_datapack/manual/assets/wiki_result_of_craft.png` & `python_datapack-0.1.1/src/python_datapack/manual/assets/wiki_result_of_craft.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.0/src/python_datapack/resource_pack/check_unused_textures.py` & `python_datapack-0.1.1/src/python_datapack/resource_pack/check_unused_textures.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.0/src/python_datapack/resource_pack/item_models.py` & `python_datapack-0.1.1/src/python_datapack/resource_pack/item_models.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.0/src/python_datapack/resource_pack/sounds.py` & `python_datapack-0.1.1/src/python_datapack/resource_pack/sounds.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.0/src/python_datapack/resource_pack/vanilla_models.py` & `python_datapack-0.1.1/src/python_datapack/resource_pack/vanilla_models.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.0/src/python_datapack/utils/database_helper.py` & `python_datapack-0.1.1/src/python_datapack/utils/database_helper.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.0/src/python_datapack/utils/ingredients.py` & `python_datapack-0.1.1/src/python_datapack/utils/ingredients.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.0/src/python_datapack/utils/io.py` & `python_datapack-0.1.1/src/python_datapack/utils/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,16 +135,19 @@
 		old_content = json.loads(FILES_TO_WRITE[file_path])
 		FILES_TO_WRITE[file_path] = super_json_dump(super_merge_dict(old_content, dict_content))
 		return
 	
 	# Add the content to the file
 	FILES_TO_WRITE[file_path] += str(content)
 
-def write_all_files():
+def write_all_files(contains: str = ""):
+	contains = contains.replace("\\", "/")
 	for file_path, content in FILES_TO_WRITE.items():
+		if contains not in file_path:
+			continue
 
 		# Make sure the content ends with two break lines
 		if not content.endswith("\n\n"):
 			if content.endswith("\n"):
 				content += "\n"
 			else:
 				content += "\n\n"
```

### Comparing `python_datapack-0.1.0/src/python_datapack/utils/multiprocessing.py` & `python_datapack-0.1.1/src/python_datapack/utils/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.0/src/python_datapack/utils/print.py` & `python_datapack-0.1.1/src/python_datapack/utils/print.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.0/src/python_datapack/utils/weld.py` & `python_datapack-0.1.1/src/python_datapack/utils/weld.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.0/LICENSE` & `python_datapack-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.0/pyproject.toml` & `python_datapack-0.1.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
-requires = ["hatchling", "pillow", "smithed"]
+requires = ["hatchling", "pillow", "smithed", "model_resolver"]
 build-backend = "hatchling.build"
 
 [project]
 name = "python_datapack"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
 	{ name="Stoupy51", email="stoupy51@gmail.com" },
 ]
 description = "Python package to help generating advanced Minecraft datapack contents"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `python_datapack-0.1.0/PKG-INFO` & `python_datapack-0.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: python_datapack
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python package to help generating advanced Minecraft datapack contents
 Project-URL: Homepage, https://github.com/Stoupy51/python_datapack
 Project-URL: Issues, https://github.com/Stoupy51/python_datapack/issues
 Author-email: Stoupy51 <stoupy51@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

