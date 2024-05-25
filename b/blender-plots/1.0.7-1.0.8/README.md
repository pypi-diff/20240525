# Comparing `tmp/blender-plots-1.0.7.tar.gz` & `tmp/blender-plots-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blender-plots-1.0.7.tar", last modified: Thu May 23 12:51:37 2024, max compression
+gzip compressed data, was "blender-plots-1.0.8.tar", last modified: Sat May 25 10:12:48 2024, max compression
```

## Comparing `blender-plots-1.0.7.tar` & `blender-plots-1.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 linus     (1000) linus     (1000)        0 2024-05-23 12:51:37.806628 blender-plots-1.0.7/
--rw-rw-r--   0 linus     (1000) linus     (1000)    35149 2023-08-26 09:18:57.000000 blender-plots-1.0.7/LICENSE
--rw-rw-r--   0 linus     (1000) linus     (1000)      268 2024-05-23 12:51:37.806628 blender-plots-1.0.7/PKG-INFO
--rw-rw-r--   0 linus     (1000) linus     (1000)    12333 2024-02-10 13:48:12.000000 blender-plots-1.0.7/README.md
-drwxrwxr-x   0 linus     (1000) linus     (1000)        0 2024-05-23 12:51:37.806628 blender-plots-1.0.7/blender_plots/
--rw-rw-r--   0 linus     (1000) linus     (1000)      216 2024-05-06 16:17:21.000000 blender-plots-1.0.7/blender_plots/__init__.py
--rw-rw-r--   0 linus     (1000) linus     (1000)     5645 2024-02-02 20:12:46.000000 blender-plots-1.0.7/blender_plots/arrows.py
--rw-rw-r--   0 linus     (1000) linus     (1000)    10320 2024-05-23 12:50:22.000000 blender-plots-1.0.7/blender_plots/blender_utils.py
--rw-rw-r--   0 linus     (1000) linus     (1000)     2269 2024-05-06 16:34:56.000000 blender-plots-1.0.7/blender_plots/marker_utils.py
--rw-rw-r--   0 linus     (1000) linus     (1000)     5453 2024-05-06 15:17:02.000000 blender-plots-1.0.7/blender_plots/plots_base.py
--rw-rw-r--   0 linus     (1000) linus     (1000)     9484 2024-05-06 15:54:55.000000 blender-plots-1.0.7/blender_plots/scatter.py
--rw-rw-r--   0 linus     (1000) linus     (1000)     3133 2023-12-05 22:14:57.000000 blender-plots-1.0.7/blender_plots/surface.py
-drwxrwxr-x   0 linus     (1000) linus     (1000)        0 2024-05-23 12:51:37.806628 blender-plots-1.0.7/blender_plots.egg-info/
--rw-r--r--   0 linus     (1000) linus     (1000)      268 2024-05-23 12:51:37.000000 blender-plots-1.0.7/blender_plots.egg-info/PKG-INFO
--rw-rw-r--   0 linus     (1000) linus     (1000)      363 2024-05-23 12:51:37.000000 blender-plots-1.0.7/blender_plots.egg-info/SOURCES.txt
--rw-rw-r--   0 linus     (1000) linus     (1000)        1 2024-05-23 12:51:37.000000 blender-plots-1.0.7/blender_plots.egg-info/dependency_links.txt
--rw-rw-r--   0 linus     (1000) linus     (1000)       14 2024-05-23 12:51:37.000000 blender-plots-1.0.7/blender_plots.egg-info/top_level.txt
--rw-rw-r--   0 linus     (1000) linus     (1000)       38 2024-05-23 12:51:37.806628 blender-plots-1.0.7/setup.cfg
--rw-rw-r--   0 linus     (1000) linus     (1000)      283 2024-05-23 12:50:41.000000 blender-plots-1.0.7/setup.py
+drwxrwxr-x   0 linus     (1000) linus     (1000)        0 2024-05-25 10:12:48.570567 blender-plots-1.0.8/
+-rw-rw-r--   0 linus     (1000) linus     (1000)    35149 2023-08-26 09:18:57.000000 blender-plots-1.0.8/LICENSE
+-rw-rw-r--   0 linus     (1000) linus     (1000)      268 2024-05-25 10:12:48.570567 blender-plots-1.0.8/PKG-INFO
+-rw-rw-r--   0 linus     (1000) linus     (1000)    12333 2024-02-10 13:48:12.000000 blender-plots-1.0.8/README.md
+drwxrwxr-x   0 linus     (1000) linus     (1000)        0 2024-05-25 10:12:48.570567 blender-plots-1.0.8/blender_plots/
+-rw-rw-r--   0 linus     (1000) linus     (1000)      216 2024-05-06 16:17:21.000000 blender-plots-1.0.8/blender_plots/__init__.py
+-rw-rw-r--   0 linus     (1000) linus     (1000)     5645 2024-02-02 20:12:46.000000 blender-plots-1.0.8/blender_plots/arrows.py
+-rw-rw-r--   0 linus     (1000) linus     (1000)    10429 2024-05-25 10:11:17.000000 blender-plots-1.0.8/blender_plots/blender_utils.py
+-rw-rw-r--   0 linus     (1000) linus     (1000)     2269 2024-05-06 16:34:56.000000 blender-plots-1.0.8/blender_plots/marker_utils.py
+-rw-rw-r--   0 linus     (1000) linus     (1000)     5453 2024-05-06 15:17:02.000000 blender-plots-1.0.8/blender_plots/plots_base.py
+-rw-rw-r--   0 linus     (1000) linus     (1000)     9484 2024-05-06 15:54:55.000000 blender-plots-1.0.8/blender_plots/scatter.py
+-rw-rw-r--   0 linus     (1000) linus     (1000)     3133 2023-12-05 22:14:57.000000 blender-plots-1.0.8/blender_plots/surface.py
+drwxrwxr-x   0 linus     (1000) linus     (1000)        0 2024-05-25 10:12:48.570567 blender-plots-1.0.8/blender_plots.egg-info/
+-rw-r--r--   0 linus     (1000) linus     (1000)      268 2024-05-25 10:12:48.000000 blender-plots-1.0.8/blender_plots.egg-info/PKG-INFO
+-rw-rw-r--   0 linus     (1000) linus     (1000)      363 2024-05-25 10:12:48.000000 blender-plots-1.0.8/blender_plots.egg-info/SOURCES.txt
+-rw-rw-r--   0 linus     (1000) linus     (1000)        1 2024-05-25 10:12:48.000000 blender-plots-1.0.8/blender_plots.egg-info/dependency_links.txt
+-rw-rw-r--   0 linus     (1000) linus     (1000)       14 2024-05-25 10:12:48.000000 blender-plots-1.0.8/blender_plots.egg-info/top_level.txt
+-rw-rw-r--   0 linus     (1000) linus     (1000)       38 2024-05-25 10:12:48.570567 blender-plots-1.0.8/setup.cfg
+-rw-rw-r--   0 linus     (1000) linus     (1000)      283 2024-05-25 10:11:27.000000 blender-plots-1.0.8/setup.py
```

### Comparing `blender-plots-1.0.7/LICENSE` & `blender-plots-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `blender-plots-1.0.7/README.md` & `blender-plots-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `blender-plots-1.0.7/blender_plots/arrows.py` & `blender-plots-1.0.8/blender_plots/arrows.py`

 * *Files identical despite different names*

### Comparing `blender-plots-1.0.7/blender_plots/blender_utils.py` & `blender-plots-1.0.8/blender_plots/blender_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from dataclasses import dataclass
-import numpy as np
 
 import bpy
+import numpy as np
 
 
 @dataclass
 class Constants:
     MARKER_COLOR = "marker_color"
     FRAME_INDEX = "frame_index"
     ARROWS = "arrows"
@@ -176,19 +176,23 @@
     mesh.attributes[Constants.MARKER_COLOR].data.foreach_set("color", color.reshape(-1))
 
 
 def get_vertex_color_material():
     """Create a material that obtains its color from the marker_color attribute"""
     material = bpy.data.materials.new("color")
     material.use_nodes = True
+    bsdf = material.node_tree.nodes.get("Principled BSDF")
+
     color_node = material.node_tree.nodes.new("ShaderNodeAttribute")
     color_node.attribute_name = Constants.MARKER_COLOR
 
-    material.node_tree.links.new(color_node.outputs["Color"],
-                                 material.node_tree.nodes["Principled BSDF"].inputs["Base Color"])
+    material.node_tree.links.new(color_node.outputs["Color"], bsdf.inputs["Base Color"])
+    material.node_tree.links.new(color_node.outputs["Alpha"], bsdf.inputs["Alpha"])
+
+    material.blend_method = "BLEND"
     return material
 
 def add_mesh_color(mesh, color):
     """Add uniform color to mesh."""
     if len(color) == 3:
         color = (*color, 1)
     material = bpy.data.materials.new("color")
```

### Comparing `blender-plots-1.0.7/blender_plots/marker_utils.py` & `blender-plots-1.0.8/blender_plots/marker_utils.py`

 * *Files identical despite different names*

### Comparing `blender-plots-1.0.7/blender_plots/plots_base.py` & `blender-plots-1.0.8/blender_plots/plots_base.py`

 * *Files identical despite different names*

### Comparing `blender-plots-1.0.7/blender_plots/scatter.py` & `blender-plots-1.0.8/blender_plots/scatter.py`

 * *Files identical despite different names*

### Comparing `blender-plots-1.0.7/blender_plots/surface.py` & `blender-plots-1.0.8/blender_plots/surface.py`

 * *Files identical despite different names*

