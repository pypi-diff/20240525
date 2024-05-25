# Comparing `tmp/honeybee-idaice-0.4.8.tar.gz` & `tmp/honeybee-idaice-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/honeybee-idaice-0.4.8.tar", last modified: Sat Mar 16 01:11:02 2024, max compression
+gzip compressed data, was "dist/honeybee-idaice-0.4.9.tar", last modified: Sat May 25 18:21:53 2024, max compression
```

## Comparing `honeybee-idaice-0.4.8.tar` & `honeybee-idaice-0.4.9.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 01:11:02.000000 honeybee-idaice-0.4.8/
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-03-16 01:10:07.000000 honeybee-idaice-0.4.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-03-16 01:10:07.000000 honeybee-idaice-0.4.8/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-03-16 01:10:07.000000 honeybee-idaice-0.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-03-16 01:10:07.000000 honeybee-idaice-0.4.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-03-16 01:11:02.000000 honeybee-idaice-0.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-03-16 01:10:07.000000 honeybee-idaice-0.4.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-03-16 01:10:07.000000 honeybee-idaice-0.4.8/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 01:11:02.000000 honeybee-idaice-0.4.8/honeybee_idaice/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-03-16 01:10:07.000000 honeybee-idaice-0.4.8/honeybee_idaice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-16 01:10:07.000000 honeybee-idaice-0.4.8/honeybee_idaice/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-03-16 01:10:07.000000 honeybee-idaice-0.4.8/honeybee_idaice/_extend_honeybee.py
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-03-16 01:10:07.000000 honeybee-idaice-0.4.8/honeybee_idaice/archive.py
--rw-r--r--   0 runner    (1001) docker     (127)    18631 2024-03-16 01:10:07.000000 honeybee-idaice-0.4.8/honeybee_idaice/bldgbody.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 01:11:02.000000 honeybee-idaice-0.4.8/honeybee_idaice/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-03-16 01:10:07.000000 honeybee-idaice-0.4.8/honeybee_idaice/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4059 2024-03-16 01:10:07.000000 honeybee-idaice-0.4.8/honeybee_idaice/cli/translate.py
--rw-r--r--   0 runner    (1001) docker     (127)     5997 2024-03-16 01:10:07.000000 honeybee-idaice-0.4.8/honeybee_idaice/face.py
--rw-r--r--   0 runner    (1001) docker     (127)     5350 2024-03-16 01:10:07.000000 honeybee-idaice-0.4.8/honeybee_idaice/shade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 01:11:02.000000 honeybee-idaice-0.4.8/honeybee_idaice/templates/
--rw-r--r--   0 runner    (1001) docker     (127)    10761 2024-03-16 01:10:07.000000 honeybee-idaice-0.4.8/honeybee_idaice/templates/ahu.idc
--rw-r--r--   0 runner    (1001) docker     (127)     6144 2024-03-16 01:10:07.000000 honeybee-idaice-0.4.8/honeybee_idaice/templates/ahu.idm
--rw-r--r--   0 runner    (1001) docker     (127)    20327 2024-03-16 01:10:07.000000 honeybee-idaice-0.4.8/honeybee_idaice/templates/building.idm
--rw-r--r--   0 runner    (1001) docker     (127)    13552 2024-03-16 01:10:07.000000 honeybee-idaice-0.4.8/honeybee_idaice/templates/plant.idc
--rw-r--r--   0 runner    (1001) docker     (127)     7678 2024-03-16 01:10:07.000000 honeybee-idaice-0.4.8/honeybee_idaice/templates/plant.idm
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-03-16 01:10:07.000000 honeybee-idaice-0.4.8/honeybee_idaice/templates/room.idm
--rw-r--r--   0 runner    (1001) docker     (127)    22439 2024-03-16 01:10:07.000000 honeybee-idaice-0.4.8/honeybee_idaice/writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-03-16 01:10:07.000000 honeybee-idaice-0.4.8/honeybee_idaice/writer_obj.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 01:11:02.000000 honeybee-idaice-0.4.8/honeybee_idaice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-03-16 01:11:02.000000 honeybee-idaice-0.4.8/honeybee_idaice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-03-16 01:11:02.000000 honeybee-idaice-0.4.8/honeybee_idaice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-16 01:11:02.000000 honeybee-idaice-0.4.8/honeybee_idaice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-16 01:11:02.000000 honeybee-idaice-0.4.8/honeybee_idaice.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-16 01:11:02.000000 honeybee-idaice-0.4.8/honeybee_idaice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-16 01:11:02.000000 honeybee-idaice-0.4.8/honeybee_idaice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-16 01:10:07.000000 honeybee-idaice-0.4.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-03-16 01:11:02.000000 honeybee-idaice-0.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-03-16 01:10:07.000000 honeybee-idaice-0.4.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 18:21:53.000000 honeybee-idaice-0.4.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-25 18:20:19.000000 honeybee-idaice-0.4.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-25 18:20:19.000000 honeybee-idaice-0.4.9/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-25 18:20:19.000000 honeybee-idaice-0.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-25 18:20:19.000000 honeybee-idaice-0.4.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-25 18:21:53.000000 honeybee-idaice-0.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-25 18:20:19.000000 honeybee-idaice-0.4.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-25 18:20:19.000000 honeybee-idaice-0.4.9/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 18:21:53.000000 honeybee-idaice-0.4.9/honeybee_idaice/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-25 18:20:19.000000 honeybee-idaice-0.4.9/honeybee_idaice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-25 18:20:19.000000 honeybee-idaice-0.4.9/honeybee_idaice/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-25 18:20:19.000000 honeybee-idaice-0.4.9/honeybee_idaice/_extend_honeybee.py
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-25 18:20:19.000000 honeybee-idaice-0.4.9/honeybee_idaice/archive.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18631 2024-05-25 18:20:19.000000 honeybee-idaice-0.4.9/honeybee_idaice/bldgbody.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 18:21:53.000000 honeybee-idaice-0.4.9/honeybee_idaice/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-25 18:20:19.000000 honeybee-idaice-0.4.9/honeybee_idaice/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4059 2024-05-25 18:20:19.000000 honeybee-idaice-0.4.9/honeybee_idaice/cli/translate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6878 2024-05-25 18:20:19.000000 honeybee-idaice-0.4.9/honeybee_idaice/face.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5350 2024-05-25 18:20:19.000000 honeybee-idaice-0.4.9/honeybee_idaice/shade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 18:21:53.000000 honeybee-idaice-0.4.9/honeybee_idaice/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)    10761 2024-05-25 18:20:19.000000 honeybee-idaice-0.4.9/honeybee_idaice/templates/ahu.idc
+-rw-r--r--   0 runner    (1001) docker     (127)     6144 2024-05-25 18:20:19.000000 honeybee-idaice-0.4.9/honeybee_idaice/templates/ahu.idm
+-rw-r--r--   0 runner    (1001) docker     (127)    20327 2024-05-25 18:20:19.000000 honeybee-idaice-0.4.9/honeybee_idaice/templates/building.idm
+-rw-r--r--   0 runner    (1001) docker     (127)    13552 2024-05-25 18:20:19.000000 honeybee-idaice-0.4.9/honeybee_idaice/templates/plant.idc
+-rw-r--r--   0 runner    (1001) docker     (127)     7678 2024-05-25 18:20:19.000000 honeybee-idaice-0.4.9/honeybee_idaice/templates/plant.idm
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-25 18:20:19.000000 honeybee-idaice-0.4.9/honeybee_idaice/templates/room.idm
+-rw-r--r--   0 runner    (1001) docker     (127)    23061 2024-05-25 18:20:19.000000 honeybee-idaice-0.4.9/honeybee_idaice/writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-05-25 18:20:19.000000 honeybee-idaice-0.4.9/honeybee_idaice/writer_obj.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 18:21:53.000000 honeybee-idaice-0.4.9/honeybee_idaice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-25 18:21:52.000000 honeybee-idaice-0.4.9/honeybee_idaice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-25 18:21:52.000000 honeybee-idaice-0.4.9/honeybee_idaice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 18:21:52.000000 honeybee-idaice-0.4.9/honeybee_idaice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-25 18:21:52.000000 honeybee-idaice-0.4.9/honeybee_idaice.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-25 18:21:52.000000 honeybee-idaice-0.4.9/honeybee_idaice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-25 18:21:52.000000 honeybee-idaice-0.4.9/honeybee_idaice.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-25 18:20:19.000000 honeybee-idaice-0.4.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-25 18:21:53.000000 honeybee-idaice-0.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-25 18:20:19.000000 honeybee-idaice-0.4.9/setup.py
```

### Comparing `honeybee-idaice-0.4.8/LICENSE` & `honeybee-idaice-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.4.8/PKG-INFO` & `honeybee-idaice-0.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honeybee-idaice
-Version: 0.4.8
+Version: 0.4.9
 Summary: Honeybee extension for translating HBJSON files to IDA-ICE IDM.
 Home-page: https://github.com/ladybug-tools/honeybee-idaice
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
```

### Comparing `honeybee-idaice-0.4.8/README.md` & `honeybee-idaice-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.4.8/honeybee_idaice/archive.py` & `honeybee-idaice-0.4.9/honeybee_idaice/archive.py`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.4.8/honeybee_idaice/bldgbody.py` & `honeybee-idaice-0.4.9/honeybee_idaice/bldgbody.py`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.4.8/honeybee_idaice/cli/translate.py` & `honeybee-idaice-0.4.9/honeybee_idaice/cli/translate.py`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.4.8/honeybee_idaice/face.py` & `honeybee-idaice-0.4.9/honeybee_idaice/face.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,42 +1,55 @@
 import math
 from typing import Union
 
-from honeybee.model import Face, Aperture, Door
+from ladybug_geometry.geometry2d import Point2D
 from ladybug_geometry.geometry3d import Point3D, Vector3D, Plane
+from honeybee.model import Face, Aperture, Door
 
 
 def opening_to_idm(
         opening: Union[Aperture, Door], ref_plane: Plane,
-        is_aperture=True, decimal_places: int = 3) -> str:
+        is_aperture=True, decimal_places: int = 3, angle_tolerance: float = 1.0) -> str:
     """Translate a HBJSON aperture or Door to an IDM Window.
 
     Args:
         opening: A Honeybee Aperture or Door to be translated to IDM.
         ref_plane: A ladybug-geometry Plane object for the reference Plane
             of the parent geometry. This plane should be pointing inwards
             towards the Room volume.
         is_aperture: A boolean to note whether the opening is an Aperture or a
             Door. (Default: True).
         decimal_places: An integer for the number of decimal places to which
             coordinate values will be rounded. (Default: 3).
+        angle_tolerance: The max angle in degrees that opening normal can differ
+            from the World Z before the opening is treated as being in the
+            World XY plane. (Default: 1).
     """
     # get the name
     name = opening.identifier
 
-    # IDA-ICE looks to apertures from inside the room
-    opening = opening.geometry.flip()
-
-    # get the rectangle in the reference plane
-    apt_llc = opening.lower_left_corner
-    apt_urc = opening.upper_right_corner
-    min_2d = ref_plane.xyz_to_xy(apt_llc)
-    max_2d = ref_plane.xyz_to_xy(apt_urc)
-    height = round(max_2d.y - min_2d.y, decimal_places)
-    width = round(max_2d.x - min_2d.x, decimal_places)
+    # if the aperture is horizontal, use the world XY
+    ang_tol = math.radians(angle_tolerance)
+    vertical = Vector3D(0, 0, 1)
+    vert_ang = ref_plane.n.angle(vertical)
+    if vert_ang <= ang_tol or vert_ang >= math.pi - ang_tol:
+        min_2d = Point2D(opening.min.x - ref_plane.o.x, opening.min.y - ref_plane.o.y)
+        max_2d = Point2D(opening.max.x - ref_plane.o.x, opening.max.y - ref_plane.o.y)
+        height = round(max_2d.y - min_2d.y, decimal_places)
+        width = round(max_2d.x - min_2d.x, decimal_places)
+    else:
+        # IDA-ICE looks to apertures from inside the room
+        opening = opening.geometry.flip()
+        # get the rectangle in the reference plane
+        apt_llc = opening.lower_left_corner
+        apt_urc = opening.upper_right_corner
+        min_2d = ref_plane.xyz_to_xy(apt_llc)
+        max_2d = ref_plane.xyz_to_xy(apt_urc)
+        height = round(max_2d.y - min_2d.y, decimal_places)
+        width = round(max_2d.x - min_2d.x, decimal_places)
 
     if is_aperture:
         opening_idm = f'\n ((CE-WINDOW :N "{name}" :T WINDOW)\n' \
             f'  (:PAR :N X :V {round(min_2d.x, decimal_places)})\n' \
             f'  (:PAR :N Y :V {round(min_2d.y, decimal_places)})\n' \
             f'  (:PAR :N DX :V {width})\n' \
             f'  (:PAR :N DY :V {height}))'
@@ -144,13 +157,14 @@
     rel_plane = parent.plane
 
     # use the XY plane if the Face is perfectly horizontal
     ang_tol = math.radians(angle_tolerance)
     vertical = Vector3D(0, 0, 1)
     vert_ang = rel_plane.n.angle(vertical)
     if vert_ang <= ang_tol or vert_ang >= math.pi - ang_tol:
+        parent_llc = parent.min
         proj_x = Vector3D(1, 0, 0)
     else:
         proj_y = Vector3D(0, 0, 1).project(rel_plane.n)
         proj_x = proj_y.rotate(rel_plane.n, math.pi / -2)
 
     return Plane(rel_plane.n, parent_llc, proj_x)
```

### Comparing `honeybee-idaice-0.4.8/honeybee_idaice/shade.py` & `honeybee-idaice-0.4.9/honeybee_idaice/shade.py`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.4.8/honeybee_idaice/templates/ahu.idc` & `honeybee-idaice-0.4.9/honeybee_idaice/templates/ahu.idc`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.4.8/honeybee_idaice/templates/ahu.idm` & `honeybee-idaice-0.4.9/honeybee_idaice/templates/ahu.idm`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.4.8/honeybee_idaice/templates/building.idm` & `honeybee-idaice-0.4.9/honeybee_idaice/templates/building.idm`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.4.8/honeybee_idaice/templates/plant.idc` & `honeybee-idaice-0.4.9/honeybee_idaice/templates/plant.idc`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.4.8/honeybee_idaice/templates/plant.idm` & `honeybee-idaice-0.4.9/honeybee_idaice/templates/plant.idm`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.4.8/honeybee_idaice/templates/room.idm` & `honeybee-idaice-0.4.9/honeybee_idaice/templates/room.idm`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.4.8/honeybee_idaice/writer.py` & `honeybee-idaice-0.4.9/honeybee_idaice/writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Write an idm file from a HBJSON file."""
 import math
 import pathlib
 import shutil
 from typing import List, Tuple
 
 from ladybug_geometry.bounding import bounding_box
-from ladybug_geometry.geometry3d import Point3D, Face3D
+from ladybug_geometry.geometry3d import Vector3D, Point3D, Plane, Face3D
 from honeybee.model import Model, Room
 from honeybee.facetype import RoofCeiling, Wall, Floor, AirBoundary, get_type_from_normal
 
 from .archive import zip_folder_to_idm
 from .bldgbody import section_to_idm, MAX_FLOOR_ELEVATION_DIFFERENCE, \
     IDA_ICE_BUILDING_BODY_TOL
 from .shade import shades_to_idm
@@ -89,21 +89,25 @@
         vc = sum(len(c) for c in contours)
         contours_formatted = ' '.join(str(len(c)) for c in contours)
         vertices_idm = ' '.join(
             f'({round(v.x - origin.x, dpl)} {round(v.y - origin.y, dpl)} {round(v.z - origin.z, dpl)})'
             for vv in contours for v in vv
         )
 
-        # add apertures
-        ref_plane = face_reference_plane(face, angle_tolerance) \
-            if face.has_sub_faces else None
+        # add apertures and doors
         windows = ['']
-        for aperture in face.apertures:
-            windows.append(opening_to_idm(aperture, ref_plane, decimal_places=dpl))
-
+        if face.has_sub_faces:
+            if angle_tolerance < face.tilt < 180 - angle_tolerance:
+                ref_plane = face_reference_plane(face, angle_tolerance)
+            else:
+                ref_plane = Plane(n=Vector3D(0, 0, 1), o=origin, x=Vector3D(1, 0, 0))
+            for aperture in face.apertures:
+                op_str = opening_to_idm(aperture, ref_plane, decimal_places=dpl,
+                                        angle_tolerance=angle_tolerance)
+                windows.append(op_str)
         windows = ''.join(windows)
 
         cp = f' ((ENCLOSING-ELEMENT :N "{name}" :T CEILING-PART :INDEX {-1001 - fc})\n' \
             '  ((AGGREGATE :N GEOMETRY)\n' \
             f'   (:PAR :N CORNERS :DIM ({vc} 3) :SP ({vc} 3) :V #2A({vertices_idm}))\n' \
             f'   (:PAR :N CONTOURS :V ({contours_formatted}))\n' \
             f'   (:PAR :N SLOPE :V {round(face.altitude + 90, 2)})){windows})'
@@ -150,16 +154,15 @@
 
     # derive the origin and the lighting point from the largest floor Face3D
     if len(hz_bounds) != 1:
         hz_bounds.sort(key=lambda x: x.area, reverse=True)
     horiz_boundary = hz_bounds[0]
     if horiz_boundary.normal.z <= 0:  # ensure upward-facing Face3D
         horiz_boundary = horiz_boundary.flip()
-    ordered_vertices = horiz_boundary.lower_left_counter_clockwise_vertices
-    origin = ordered_vertices[0]
+    origin = horiz_boundary.min
     if horiz_boundary.is_convex:
         pole = horiz_boundary.center
     else:  # use a 1 cm tolerance for pole that will not be time consuming to compute
         pole = horiz_boundary.pole_of_inaccessibility(0.01)
 
     # relative coordinates of the pole
     rp = pole - origin
@@ -258,40 +261,45 @@
         else:
             # TODO: support air boundaries
             walls.append(face)
 
     return walls, ceilings, floors
 
 
-def _is_room_extruded(room: Room, angle_tolerance: float) -> Tuple:
+def _is_room_extruded(room: Room, tolerance: float, angle_tolerance: float) -> Tuple:
     """Check if the room geometry is an extrusion in Z direction.
 
     Args:
         room: A honeybee Room.
+        tolerance: The minimum difference between coordinate values at which point
+            vertices are considered distinct.
         angle_tolerance: The max angle difference in degrees that the normals of
             Faces are allowed to differ from vertical/horizontal for the Room
             to not be considered extruded.
     """
-    f_h = 0
-    c_h = 0
+    f_hs = []
+    c_hs = []
     for face in room.faces:
         type_ = face.type
         if isinstance(type_, Wall):
             if abs(face.altitude) > angle_tolerance:
                 return False, -1
         elif isinstance(type_, RoofCeiling):
             if abs(90 - face.altitude) > angle_tolerance:
                 return False, -1
-            c_h = face.vertices[0].z
+            c_hs.append(face.vertices[0].z)
         elif isinstance(type_, Floor):
             if abs(face.altitude + 90) > angle_tolerance:
                 return False, -1
-            f_h = face.vertices[0].z
+            f_hs.append(face.vertices[0].z)
 
-    return True, round(c_h - f_h, 2)
+    if len(f_hs) != 0 and len(c_hs) != 0 and max(c_hs) - min(c_hs) < tolerance and \
+            max(f_hs) - min(f_hs) < tolerance:
+        return True, round(room.max.z - room.min.z, 2)
+    return False, -1
 
 
 def prepare_model(model: Model, max_int_wall_thickness: float = 0.45) -> Model:
     """Perform a number of model edits to prepare it for translation to IDM.
 
     * Check room display names and ensure they are unique
     * Mark rooms as extruded and non-extruded
@@ -324,15 +332,15 @@
                 room.display_name = \
                     f'{room.display_name}_{room_names[original_name]}'
                 room_names[original_name] += 1
             else:
                 room_names[room.display_name] = 1
             # add markers for whether the Room is extruded or not
             is_extruded, floor_to_ceiling_height = \
-                _is_room_extruded(room, model.angle_tolerance)
+                _is_room_extruded(room, model.tolerance, model.angle_tolerance)
             room.user_data = {
                 '_idm_is_extruded': is_extruded,
                 '_idm_flr_ceil_height': floor_to_ceiling_height
             }
             # add markers so adjacent interior Apertures and Doors are not duplicated
             for face in room.faces:
                 # remove AirBoundaries until we learn how to support them
@@ -459,15 +467,17 @@
 
     __here__ = pathlib.Path(__file__).parent
     templates_folder = __here__.joinpath('templates')
 
     # create building file that includes building bodies and a reference to the rooms
     with bldg_file.open('w', encoding='UTF-8') as bldg:
         header = ';IDA 4.80002 Data UTF-8\n' \
-            f'(DOCUMENT-HEADER :TYPE BUILDING :N "{bldg_name}" :MS 4 :CK ((RECENT (WINDEF . "Double Clear Air (WIN7)"))) :PARENT ICE :APP (ICE :VER 4.802))\n'
+            '(DOCUMENT-HEADER :TYPE BUILDING :N "{}" :MS 4 :CK ' \
+            '((RECENT (WINDEF . "Double Clear Air (WIN7)"))) ' \
+            ':PARENT ICE :APP (ICE :VER 4.802))\n'.format(bldg_name)
         bldg.write(header)
         # add template values
         bldg_template = templates_folder.joinpath('building.idm')
         for line in bldg_template.open('r'):
             bldg.write(line)
 
         # create a building sections/bodies for the building
```

### Comparing `honeybee-idaice-0.4.8/honeybee_idaice/writer_obj.py` & `honeybee-idaice-0.4.9/honeybee_idaice/writer_obj.py`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.4.8/honeybee_idaice.egg-info/PKG-INFO` & `honeybee-idaice-0.4.9/honeybee_idaice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honeybee-idaice
-Version: 0.4.8
+Version: 0.4.9
 Summary: Honeybee extension for translating HBJSON files to IDA-ICE IDM.
 Home-page: https://github.com/ladybug-tools/honeybee-idaice
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
```

### Comparing `honeybee-idaice-0.4.8/honeybee_idaice.egg-info/SOURCES.txt` & `honeybee-idaice-0.4.9/honeybee_idaice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.4.8/setup.py` & `honeybee-idaice-0.4.9/setup.py`

 * *Files identical despite different names*

