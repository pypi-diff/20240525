# Comparing `tmp/python_datapack-0.0.4.tar.gz` & `tmp/python_datapack-0.1.0.tar.gz`

## Comparing `python_datapack-0.0.4.tar` & `python_datapack-0.1.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 python_datapack-0.0.4/1_upgrades.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 python_datapack-0.0.4/2_build.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 python_datapack-0.0.4/3_upload.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 python_datapack-0.0.4/build_all_in_one.py
--rw-r--r--   0        0        0     8141 2020-02-02 00:00:00.000000 python_datapack-0.0.4/src/python_datapack/__init__.py
--rw-r--r--   0        0        0     2997 2020-02-02 00:00:00.000000 python_datapack-0.0.4/src/python_datapack/constants.py
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 python_datapack-0.0.4/src/python_datapack/enhance_config.py
--rw-r--r--   0        0        0     3879 2020-02-02 00:00:00.000000 python_datapack-0.0.4/src/python_datapack/finalyze.py
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 python_datapack-0.0.4/src/python_datapack/initialize.py
--rw-r--r--   0        0        0    10662 2020-02-02 00:00:00.000000 python_datapack-0.0.4/src/python_datapack/verify_database.py
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 python_datapack-0.0.4/src/python_datapack/datapack/basic_structure.py
--rw-r--r--   0        0        0    14581 2020-02-02 00:00:00.000000 python_datapack-0.0.4/src/python_datapack/datapack/custom_blocks.py
--rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 python_datapack-0.0.4/src/python_datapack/datapack/headers.py
--rw-r--r--   0        0        0     4134 2020-02-02 00:00:00.000000 python_datapack-0.0.4/src/python_datapack/datapack/lang.py
--rw-r--r--   0        0        0     6408 2020-02-02 00:00:00.000000 python_datapack-0.0.4/src/python_datapack/datapack/loading.py
--rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 python_datapack-0.0.4/src/python_datapack/datapack/loot_tables.py
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 python_datapack-0.0.4/src/python_datapack/datapack/main.py
--rw-r--r--   0        0        0     3942 2020-02-02 00:00:00.000000 python_datapack-0.0.4/src/python_datapack/datapack/recipes.py
--rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 python_datapack-0.0.4/src/python_datapack/manual/book_optimizer.py
--rw-r--r--   0        0        0    19311 2020-02-02 00:00:00.000000 python_datapack-0.0.4/src/python_datapack/manual/main.py
--rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 python_datapack-0.0.4/src/python_datapack/manual/shared_import.py
--rw-r--r--   0        0        0    24998 2020-02-02 00:00:00.000000 python_datapack-0.0.4/src/python_datapack/manual/utils.py
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 python_datapack-0.0.4/src/python_datapack/manual/assets/furnace.png
--rw-r--r--   0        0        0    42432 2020-02-02 00:00:00.000000 python_datapack-0.0.4/src/python_datapack/manual/assets/minecraft_font.ttf
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 python_datapack-0.0.4/src/python_datapack/manual/assets/none.png
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 python_datapack-0.0.4/src/python_datapack/manual/assets/none_release.png
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 python_datapack-0.0.4/src/python_datapack/manual/assets/shaped_2x2.png
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 python_datapack-0.0.4/src/python_datapack/manual/assets/shaped_3x3.png
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 python_datapack-0.0.4/src/python_datapack/manual/assets/simple_case_no_border.png
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 python_datapack-0.0.4/src/python_datapack/manual/assets/wiki_information.png
--rw-r--r--   0        0        0     3483 2020-02-02 00:00:00.000000 python_datapack-0.0.4/src/python_datapack/manual/assets/wiki_ingredient_of_craft.png
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 python_datapack-0.0.4/src/python_datapack/manual/assets/wiki_ingredient_of_craft_template.png
--rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 python_datapack-0.0.4/src/python_datapack/manual/assets/wiki_result_of_craft.png
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 python_datapack-0.0.4/src/python_datapack/resource_pack/check_unused_textures.py
--rw-r--r--   0        0        0     4497 2020-02-02 00:00:00.000000 python_datapack-0.0.4/src/python_datapack/resource_pack/item_models.py
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 python_datapack-0.0.4/src/python_datapack/resource_pack/main.py
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 python_datapack-0.0.4/src/python_datapack/resource_pack/sounds.py
--rw-r--r--   0        0        0     2787 2020-02-02 00:00:00.000000 python_datapack-0.0.4/src/python_datapack/resource_pack/vanilla_models.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 python_datapack-0.0.4/src/python_datapack/utils/cache.py
--rw-r--r--   0        0        0    28262 2020-02-02 00:00:00.000000 python_datapack-0.0.4/src/python_datapack/utils/database_helper.py
--rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 python_datapack-0.0.4/src/python_datapack/utils/ingredients.py
--rw-r--r--   0        0        0     4809 2020-02-02 00:00:00.000000 python_datapack-0.0.4/src/python_datapack/utils/io.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 python_datapack-0.0.4/src/python_datapack/utils/multiprocessing.py
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 python_datapack-0.0.4/src/python_datapack/utils/print.py
--rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 python_datapack-0.0.4/src/python_datapack/utils/weld.py
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 python_datapack-0.0.4/.gitignore
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 python_datapack-0.0.4/LICENSE
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 python_datapack-0.0.4/README.md
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 python_datapack-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 python_datapack-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 python_datapack-0.1.0/1_upgrades.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 python_datapack-0.1.0/2_build.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 python_datapack-0.1.0/3_upload.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 python_datapack-0.1.0/build_all_in_one.py
+-rw-r--r--   0        0        0     8141 2020-02-02 00:00:00.000000 python_datapack-0.1.0/src/python_datapack/__init__.py
+-rw-r--r--   0        0        0     2997 2020-02-02 00:00:00.000000 python_datapack-0.1.0/src/python_datapack/constants.py
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 python_datapack-0.1.0/src/python_datapack/enhance_config.py
+-rw-r--r--   0        0        0     3874 2020-02-02 00:00:00.000000 python_datapack-0.1.0/src/python_datapack/finalyze.py
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 python_datapack-0.1.0/src/python_datapack/initialize.py
+-rw-r--r--   0        0        0    10662 2020-02-02 00:00:00.000000 python_datapack-0.1.0/src/python_datapack/verify_database.py
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 python_datapack-0.1.0/src/python_datapack/datapack/basic_structure.py
+-rw-r--r--   0        0        0    14581 2020-02-02 00:00:00.000000 python_datapack-0.1.0/src/python_datapack/datapack/custom_blocks.py
+-rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 python_datapack-0.1.0/src/python_datapack/datapack/headers.py
+-rw-r--r--   0        0        0     4134 2020-02-02 00:00:00.000000 python_datapack-0.1.0/src/python_datapack/datapack/lang.py
+-rw-r--r--   0        0        0     6408 2020-02-02 00:00:00.000000 python_datapack-0.1.0/src/python_datapack/datapack/loading.py
+-rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 python_datapack-0.1.0/src/python_datapack/datapack/loot_tables.py
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 python_datapack-0.1.0/src/python_datapack/datapack/main.py
+-rw-r--r--   0        0        0     3942 2020-02-02 00:00:00.000000 python_datapack-0.1.0/src/python_datapack/datapack/recipes.py
+-rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 python_datapack-0.1.0/src/python_datapack/manual/book_optimizer.py
+-rw-r--r--   0        0        0    19193 2020-02-02 00:00:00.000000 python_datapack-0.1.0/src/python_datapack/manual/main.py
+-rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 python_datapack-0.1.0/src/python_datapack/manual/shared_import.py
+-rw-r--r--   0        0        0    25039 2020-02-02 00:00:00.000000 python_datapack-0.1.0/src/python_datapack/manual/utils.py
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 python_datapack-0.1.0/src/python_datapack/manual/assets/furnace.png
+-rw-r--r--   0        0        0    42432 2020-02-02 00:00:00.000000 python_datapack-0.1.0/src/python_datapack/manual/assets/minecraft_font.ttf
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 python_datapack-0.1.0/src/python_datapack/manual/assets/none.png
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 python_datapack-0.1.0/src/python_datapack/manual/assets/none_release.png
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 python_datapack-0.1.0/src/python_datapack/manual/assets/shaped_2x2.png
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 python_datapack-0.1.0/src/python_datapack/manual/assets/shaped_3x3.png
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 python_datapack-0.1.0/src/python_datapack/manual/assets/simple_case_no_border.png
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 python_datapack-0.1.0/src/python_datapack/manual/assets/wiki_information.png
+-rw-r--r--   0        0        0     3483 2020-02-02 00:00:00.000000 python_datapack-0.1.0/src/python_datapack/manual/assets/wiki_ingredient_of_craft.png
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 python_datapack-0.1.0/src/python_datapack/manual/assets/wiki_ingredient_of_craft_template.png
+-rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 python_datapack-0.1.0/src/python_datapack/manual/assets/wiki_result_of_craft.png
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 python_datapack-0.1.0/src/python_datapack/resource_pack/check_unused_textures.py
+-rw-r--r--   0        0        0     4497 2020-02-02 00:00:00.000000 python_datapack-0.1.0/src/python_datapack/resource_pack/item_models.py
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 python_datapack-0.1.0/src/python_datapack/resource_pack/main.py
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 python_datapack-0.1.0/src/python_datapack/resource_pack/sounds.py
+-rw-r--r--   0        0        0     2787 2020-02-02 00:00:00.000000 python_datapack-0.1.0/src/python_datapack/resource_pack/vanilla_models.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 python_datapack-0.1.0/src/python_datapack/utils/cache.py
+-rw-r--r--   0        0        0    28262 2020-02-02 00:00:00.000000 python_datapack-0.1.0/src/python_datapack/utils/database_helper.py
+-rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 python_datapack-0.1.0/src/python_datapack/utils/ingredients.py
+-rw-r--r--   0        0        0     4809 2020-02-02 00:00:00.000000 python_datapack-0.1.0/src/python_datapack/utils/io.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 python_datapack-0.1.0/src/python_datapack/utils/multiprocessing.py
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 python_datapack-0.1.0/src/python_datapack/utils/print.py
+-rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 python_datapack-0.1.0/src/python_datapack/utils/weld.py
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 python_datapack-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 python_datapack-0.1.0/LICENSE
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 python_datapack-0.1.0/README.md
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 python_datapack-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 python_datapack-0.1.0/PKG-INFO
```

### Comparing `python_datapack-0.0.4/src/python_datapack/__init__.py` & `python_datapack-0.1.0/src/python_datapack/__init__.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.4/src/python_datapack/constants.py` & `python_datapack-0.1.0/src/python_datapack/constants.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.4/src/python_datapack/enhance_config.py` & `python_datapack-0.1.0/src/python_datapack/enhance_config.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.4/src/python_datapack/finalyze.py` & `python_datapack-0.1.0/src/python_datapack/finalyze.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from .utils.print import *
 from .utils.weld import weld_datapack, weld_resource_pack
 from .datapack.lang import main as lang_main
 from .datapack.headers import main as headers_main
 from .resource_pack.check_unused_textures import main as check_unused_textures_main
 import shutil
 
-def main(config: dict, user_code: callable|None):
+def main(config: dict, user_code: callable):
 
 	# For every file in the merge folder, copy it to the build folder (with append content)
 	print()
 	for root, _, files in os.walk(config['merge_folder']):
 		for file in files:
 			merge_path = f"{root}/{file}".replace("\\", "/")
 			build_path = merge_path.replace(config['merge_folder'], config['build_folder'])
```

### Comparing `python_datapack-0.0.4/src/python_datapack/initialize.py` & `python_datapack-0.1.0/src/python_datapack/initialize.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.4/src/python_datapack/verify_database.py` & `python_datapack-0.1.0/src/python_datapack/verify_database.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.4/src/python_datapack/datapack/basic_structure.py` & `python_datapack-0.1.0/src/python_datapack/datapack/basic_structure.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.4/src/python_datapack/datapack/custom_blocks.py` & `python_datapack-0.1.0/src/python_datapack/datapack/custom_blocks.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.4/src/python_datapack/datapack/headers.py` & `python_datapack-0.1.0/src/python_datapack/datapack/headers.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.4/src/python_datapack/datapack/lang.py` & `python_datapack-0.1.0/src/python_datapack/datapack/lang.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.4/src/python_datapack/datapack/loading.py` & `python_datapack-0.1.0/src/python_datapack/datapack/loading.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.4/src/python_datapack/datapack/loot_tables.py` & `python_datapack-0.1.0/src/python_datapack/datapack/loot_tables.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.4/src/python_datapack/datapack/main.py` & `python_datapack-0.1.0/src/python_datapack/datapack/main.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.4/src/python_datapack/datapack/recipes.py` & `python_datapack-0.1.0/src/python_datapack/datapack/recipes.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.4/src/python_datapack/manual/book_optimizer.py` & `python_datapack-0.1.0/src/python_datapack/manual/book_optimizer.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.4/src/python_datapack/manual/main.py` & `python_datapack-0.1.0/src/python_datapack/manual/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 
 # Imports
 from ..utils.io import *
 from ..utils.print import *
 from .utils import *
+from .shared_import import *
 from .book_optimizer import *
 from ..constants import *
 
 def main(config: dict):
 
 	# Prework
 	os.makedirs(f"{config['manual_path']}/font/page", exist_ok=True)
@@ -87,15 +88,15 @@
 		for item, data in sorted_database_on_category:
 			i += 1
 			manual_pages.append({"number": i, "name": item, "raw_data": data, "type": "item"})
 
 		# Encode pages
 		book_content = []
 		os.makedirs(f"{config['manual_path']}/font/category", exist_ok=True)
-		simple_case = Image.open(f"{MANUAL_ASSETS_PATH}/simple_case_no_border.png")	# Load the simple case image for later use in categories pages
+		simple_case = Image.open(f"{TEMPLATES_PATH}/simple_case_no_border.png")	# Load the simple case image for later use in categories pages
 		for page in manual_pages:
 			content = []
 			number = page["number"]
 			page_font = get_page_font(number)
 			name = str(page["name"])
 			raw_data = page["raw_data"]
 			titled = name.replace("_", " ").title() + "\n"
@@ -322,17 +323,14 @@
 		# If remaining items in the line, add them
 		if len(line) > 0:
 			line[-1]["text"] += "\n"
 			line[0]["text"] = SMALL_NONE_FONT * LEFT_PADDING + line[0]["text"]
 			content += line * 2
 		
 		# Add the 2 pixels border
-		BORDER_COLOR = 0xB64E2F
-		BORDER_SIZE = 2
-		BORDER_COLOR = (BORDER_COLOR >> 16) & 0xFF, (BORDER_COLOR >> 8) & 0xFF, BORDER_COLOR & 0xFF, 255
 		is_rectangle_shape = len(raw_data) % config['max_items_per_row'] == 0
 		page_image = add_border(page_image, BORDER_COLOR, BORDER_SIZE, is_rectangle_shape)
 		
 		# Save the image and add the page to the book
 		page_image.save(f"{config['manual_path']}/font/category/{file_name}.png")
 		book_content.insert(0, content)
```

### Comparing `python_datapack-0.0.4/src/python_datapack/manual/shared_import.py` & `python_datapack-0.1.0/src/python_datapack/manual/shared_import.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 
 # Constants
 SQUARE_SIZE = 32
 MANUAL_ASSETS_PATH = os.path.dirname(os.path.realpath(__file__)).replace("\\","/") + "/"
 TEMPLATES_PATH = MANUAL_ASSETS_PATH + "assets"
 FONT_FILE = "manual"
 BORDER_COLOR = 0xB64E2F
-BORDER_SIZE = 2
 BORDER_COLOR = (BORDER_COLOR >> 16) & 0xFF, (BORDER_COLOR >> 8) & 0xFF, BORDER_COLOR & 0xFF, 255
+BORDER_SIZE = 2
 NONE_FONT = get_font(0x0000)
 MEDIUM_NONE_FONT = get_font(0x0001)
 SMALL_NONE_FONT = get_font(0x0002)
 VERY_SMALL_NONE_FONT = get_font(0x0003)
 WIKI_NONE_FONT = get_font(0x0004)
 WIKI_INFO_FONT = get_font(0x0005)
 WIKI_RESULT_OF_CRAFT_FONT = get_font(0x0006)
```

### Comparing `python_datapack-0.0.4/src/python_datapack/manual/utils.py` & `python_datapack-0.1.0/src/python_datapack/manual/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,18 +65,20 @@
 		count (int): The count to show
 	Returns:
 		Image: The image with the count
 	"""
 	# Create the image
 	img = Image.new("RGBA", (32, 32), (0, 0, 0, 0))
 	draw = ImageDraw.Draw(img)
-	font = ImageFont.truetype(f"{TEMPLATES_PATH}/minecraft_font.ttf", size = 16)
+	font_size = 16
+	font = ImageFont.truetype(f"{TEMPLATES_PATH}/minecraft_font.ttf", size = font_size)
 
 	# Calculate text size and positions of the two texts
-	text_width, text_height = draw.textsize(str(count), font = font)
+	text_width = draw.textlength(str(count), font = font)
+	text_height = font_size
 	pos_1 = (32-text_width), (32-text_height)
 	pos_2 = (30-text_width), (30-text_height)
 	
 	# Draw the count
 	draw.text(pos_1, str(count), (50, 50, 50), font = font)
 	draw.text(pos_2, str(count), (255, 255, 255), font = font)
 	return img
@@ -439,15 +441,15 @@
 
 	# Convert shapeless crafting to shaped crafting
 	if craft_type == "crafting_shapeless":
 		craft = convert_shapeless_to_shaped(craft)
 		craft_type = "crafting_shaped"
 	
 	# Generate the image for the page
-	generate_page_font(name, page_font, craft)
+	generate_page_font(config, name, page_font, craft)
 
 	# Get result component
 	result_component = get_item_component(config, name)
 	if result_component.get("clickEvent"):
 		del result_component["clickEvent"]	# Remove clickEvent for result item (as we already are on the page)
 
 	# If the craft is shaped
@@ -608,15 +610,15 @@
 
 			# Load texture and resize it
 			item_texture = Image.open(texture_path)
 			item_texture = item_texture.resize((42, 42), Image.NEAREST)
 			item_texture = item_texture.convert("RGBA")
 
 			# Load the template and paste the texture on it
-			template = Image.open(f"{MANUAL_ASSETS_PATH}/wiki_ingredient_of_craft_template.png")
+			template = Image.open(f"{TEMPLATES_PATH}/wiki_ingredient_of_craft_template.png")
 			template.paste(item_texture, (11, 11), item_texture)
 			
 			# Save the result
 			template.save(dest_path)
 
 		# Prepare provider
 		font = get_next_font()
```

### Comparing `python_datapack-0.0.4/src/python_datapack/manual/assets/furnace.png` & `python_datapack-0.1.0/src/python_datapack/manual/assets/furnace.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.4/src/python_datapack/manual/assets/minecraft_font.ttf` & `python_datapack-0.1.0/src/python_datapack/manual/assets/minecraft_font.ttf`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.4/src/python_datapack/manual/assets/shaped_2x2.png` & `python_datapack-0.1.0/src/python_datapack/manual/assets/shaped_2x2.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.4/src/python_datapack/manual/assets/shaped_3x3.png` & `python_datapack-0.1.0/src/python_datapack/manual/assets/shaped_3x3.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.4/src/python_datapack/manual/assets/simple_case_no_border.png` & `python_datapack-0.1.0/src/python_datapack/manual/assets/simple_case_no_border.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.4/src/python_datapack/manual/assets/wiki_information.png` & `python_datapack-0.1.0/src/python_datapack/manual/assets/wiki_information.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.4/src/python_datapack/manual/assets/wiki_ingredient_of_craft.png` & `python_datapack-0.1.0/src/python_datapack/manual/assets/wiki_ingredient_of_craft.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.4/src/python_datapack/manual/assets/wiki_ingredient_of_craft_template.png` & `python_datapack-0.1.0/src/python_datapack/manual/assets/wiki_ingredient_of_craft_template.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.4/src/python_datapack/manual/assets/wiki_result_of_craft.png` & `python_datapack-0.1.0/src/python_datapack/manual/assets/wiki_result_of_craft.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.4/src/python_datapack/resource_pack/check_unused_textures.py` & `python_datapack-0.1.0/src/python_datapack/resource_pack/check_unused_textures.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.4/src/python_datapack/resource_pack/item_models.py` & `python_datapack-0.1.0/src/python_datapack/resource_pack/item_models.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.4/src/python_datapack/resource_pack/sounds.py` & `python_datapack-0.1.0/src/python_datapack/resource_pack/sounds.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.4/src/python_datapack/resource_pack/vanilla_models.py` & `python_datapack-0.1.0/src/python_datapack/resource_pack/vanilla_models.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.4/src/python_datapack/utils/database_helper.py` & `python_datapack-0.1.0/src/python_datapack/utils/database_helper.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.4/src/python_datapack/utils/ingredients.py` & `python_datapack-0.1.0/src/python_datapack/utils/ingredients.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.4/src/python_datapack/utils/io.py` & `python_datapack-0.1.0/src/python_datapack/utils/io.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.4/src/python_datapack/utils/multiprocessing.py` & `python_datapack-0.1.0/src/python_datapack/utils/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.4/src/python_datapack/utils/print.py` & `python_datapack-0.1.0/src/python_datapack/utils/print.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.4/src/python_datapack/utils/weld.py` & `python_datapack-0.1.0/src/python_datapack/utils/weld.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.4/LICENSE` & `python_datapack-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.4/pyproject.toml` & `python_datapack-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["hatchling", "pillow", "smithed"]
 build-backend = "hatchling.build"
 
 [project]
 name = "python_datapack"
-version = "0.0.4"
+version = "0.1.0"
 authors = [
 	{ name="Stoupy51", email="stoupy51@gmail.com" },
 ]
 description = "Python package to help generating advanced Minecraft datapack contents"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `python_datapack-0.0.4/PKG-INFO` & `python_datapack-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: python_datapack
-Version: 0.0.4
+Version: 0.1.0
 Summary: Python package to help generating advanced Minecraft datapack contents
 Project-URL: Homepage, https://github.com/Stoupy51/python_datapack
 Project-URL: Issues, https://github.com/Stoupy51/python_datapack/issues
 Author-email: Stoupy51 <stoupy51@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

