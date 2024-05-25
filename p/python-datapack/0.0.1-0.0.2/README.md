# Comparing `tmp/python_datapack-0.0.1.tar.gz` & `tmp/python_datapack-0.0.2.tar.gz`

## Comparing `python_datapack-0.0.1.tar` & `python_datapack-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,50 @@
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 python_datapack-0.0.1/build_package copy.py
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 python_datapack-0.0.1/build_package.py
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 python_datapack-0.0.1/src/python_datapack/__init__.py
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 python_datapack-0.0.1/src/python_datapack/example.py
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 python_datapack-0.0.1/.gitignore
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 python_datapack-0.0.1/LICENSE
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 python_datapack-0.0.1/README.md
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 python_datapack-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 python_datapack-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 python_datapack-0.0.2/1_upgrades.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 python_datapack-0.0.2/2_build.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 python_datapack-0.0.2/3_upload.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 python_datapack-0.0.2/build_all_in_one.py
+-rw-r--r--   0        0        0     7996 2020-02-02 00:00:00.000000 python_datapack-0.0.2/src/python_datapack/__init__.py
+-rw-r--r--   0        0        0     2997 2020-02-02 00:00:00.000000 python_datapack-0.0.2/src/python_datapack/constants.py
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 python_datapack-0.0.2/src/python_datapack/enhance_config.py
+-rw-r--r--   0        0        0     3800 2020-02-02 00:00:00.000000 python_datapack-0.0.2/src/python_datapack/finalyze.py
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 python_datapack-0.0.2/src/python_datapack/initialize.py
+-rw-r--r--   0        0        0    10662 2020-02-02 00:00:00.000000 python_datapack-0.0.2/src/python_datapack/verify_database.py
+-rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 python_datapack-0.0.2/src/python_datapack/datapack/basic_structure.py
+-rw-r--r--   0        0        0    14654 2020-02-02 00:00:00.000000 python_datapack-0.0.2/src/python_datapack/datapack/custom_blocks.py
+-rw-r--r--   0        0        0     2988 2020-02-02 00:00:00.000000 python_datapack-0.0.2/src/python_datapack/datapack/headers.py
+-rw-r--r--   0        0        0     4134 2020-02-02 00:00:00.000000 python_datapack-0.0.2/src/python_datapack/datapack/lang.py
+-rw-r--r--   0        0        0     6449 2020-02-02 00:00:00.000000 python_datapack-0.0.2/src/python_datapack/datapack/loading.py
+-rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 python_datapack-0.0.2/src/python_datapack/datapack/loot_tables.py
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 python_datapack-0.0.2/src/python_datapack/datapack/main.py
+-rw-r--r--   0        0        0     3942 2020-02-02 00:00:00.000000 python_datapack-0.0.2/src/python_datapack/datapack/recipes.py
+-rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 python_datapack-0.0.2/src/python_datapack/manual/book_optimizer.py
+-rw-r--r--   0        0        0    19323 2020-02-02 00:00:00.000000 python_datapack-0.0.2/src/python_datapack/manual/main.py
+-rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 python_datapack-0.0.2/src/python_datapack/manual/shared_import.py
+-rw-r--r--   0        0        0    24998 2020-02-02 00:00:00.000000 python_datapack-0.0.2/src/python_datapack/manual/utils.py
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 python_datapack-0.0.2/src/python_datapack/manual/assets/furnace.png
+-rw-r--r--   0        0        0    42432 2020-02-02 00:00:00.000000 python_datapack-0.0.2/src/python_datapack/manual/assets/minecraft_font.ttf
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 python_datapack-0.0.2/src/python_datapack/manual/assets/none.png
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 python_datapack-0.0.2/src/python_datapack/manual/assets/none_release.png
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 python_datapack-0.0.2/src/python_datapack/manual/assets/shaped_2x2.png
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 python_datapack-0.0.2/src/python_datapack/manual/assets/shaped_3x3.png
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 python_datapack-0.0.2/src/python_datapack/manual/assets/simple_case_no_border.png
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 python_datapack-0.0.2/src/python_datapack/manual/assets/wiki_information.png
+-rw-r--r--   0        0        0     3483 2020-02-02 00:00:00.000000 python_datapack-0.0.2/src/python_datapack/manual/assets/wiki_ingredient_of_craft.png
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 python_datapack-0.0.2/src/python_datapack/manual/assets/wiki_ingredient_of_craft_template.png
+-rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 python_datapack-0.0.2/src/python_datapack/manual/assets/wiki_result_of_craft.png
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 python_datapack-0.0.2/src/python_datapack/resource_pack/check_unused_textures.py
+-rw-r--r--   0        0        0     4497 2020-02-02 00:00:00.000000 python_datapack-0.0.2/src/python_datapack/resource_pack/item_models.py
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 python_datapack-0.0.2/src/python_datapack/resource_pack/main.py
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 python_datapack-0.0.2/src/python_datapack/resource_pack/sounds.py
+-rw-r--r--   0        0        0     2787 2020-02-02 00:00:00.000000 python_datapack-0.0.2/src/python_datapack/resource_pack/vanilla_models.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 python_datapack-0.0.2/src/python_datapack/utils/cache.py
+-rw-r--r--   0        0        0    28192 2020-02-02 00:00:00.000000 python_datapack-0.0.2/src/python_datapack/utils/database_helper.py
+-rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 python_datapack-0.0.2/src/python_datapack/utils/ingredients.py
+-rw-r--r--   0        0        0     4809 2020-02-02 00:00:00.000000 python_datapack-0.0.2/src/python_datapack/utils/io.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 python_datapack-0.0.2/src/python_datapack/utils/multiprocessing.py
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 python_datapack-0.0.2/src/python_datapack/utils/print.py
+-rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 python_datapack-0.0.2/src/python_datapack/utils/weld.py
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 python_datapack-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 python_datapack-0.0.2/LICENSE
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 python_datapack-0.0.2/README.md
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 python_datapack-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 python_datapack-0.0.2/PKG-INFO
```

### Comparing `python_datapack-0.0.1/LICENSE` & `python_datapack-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python_datapack-0.0.1/pyproject.toml` & `python_datapack-0.0.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
-requires = ["hatchling", "pillow", "glfw", "smithed", "pygame"]
+requires = ["hatchling", "pillow", "smithed"]
 build-backend = "hatchling.build"
 
 [project]
 name = "python_datapack"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
 	{ name="Stoupy51", email="stoupy51@gmail.com" },
 ]
 description = "Python package to help generating advanced Minecraft datapack contents"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `python_datapack-0.0.1/PKG-INFO` & `python_datapack-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: python_datapack
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python package to help generating advanced Minecraft datapack contents
 Project-URL: Homepage, https://github.com/Stoupy51/python_datapack
 Project-URL: Issues, https://github.com/Stoupy51/python_datapack/issues
 Author-email: Stoupy51 <stoupy51@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

