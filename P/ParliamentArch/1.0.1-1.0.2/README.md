# Comparing `tmp/parliamentarch-1.0.1.tar.gz` & `tmp/parliamentarch-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parliamentarch-1.0.1.tar", last modified: Thu May 23 22:39:07 2024, max compression
+gzip compressed data, was "parliamentarch-1.0.2.tar", last modified: Sat May 25 13:13:48 2024, max compression
```

## Comparing `parliamentarch-1.0.1.tar` & `parliamentarch-1.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:39:07.085309 parliamentarch-1.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:39:07.081309 parliamentarch-1.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:39:07.081309 parliamentarch-1.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-23 22:39:02.000000 parliamentarch-1.0.1/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-23 22:39:02.000000 parliamentarch-1.0.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-23 22:39:02.000000 parliamentarch-1.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-05-23 22:39:02.000000 parliamentarch-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12947 2024-05-23 22:39:02.000000 parliamentarch-1.0.1/LISEZMOI.rst
--rw-r--r--   0 runner    (1001) docker     (127)    14346 2024-05-23 22:39:07.085309 parliamentarch-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12322 2024-05-23 22:39:02.000000 parliamentarch-1.0.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-23 22:39:02.000000 parliamentarch-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 22:39:07.085309 parliamentarch-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:39:07.081309 parliamentarch-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:39:07.085309 parliamentarch-1.0.1/src/ParliamentArch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14346 2024-05-23 22:39:07.000000 parliamentarch-1.0.1/src/ParliamentArch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-23 22:39:07.000000 parliamentarch-1.0.1/src/ParliamentArch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 22:39:07.000000 parliamentarch-1.0.1/src/ParliamentArch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-23 22:39:07.000000 parliamentarch-1.0.1/src/ParliamentArch.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:39:07.085309 parliamentarch-1.0.1/src/parliamentarch/
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-23 22:39:02.000000 parliamentarch-1.0.1/src/parliamentarch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-05-23 22:39:02.000000 parliamentarch-1.0.1/src/parliamentarch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-05-23 22:39:02.000000 parliamentarch-1.0.1/src/parliamentarch/_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     8869 2024-05-23 22:39:02.000000 parliamentarch-1.0.1/src/parliamentarch/geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     6378 2024-05-23 22:39:02.000000 parliamentarch-1.0.1/src/parliamentarch/svg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 13:13:48.492123 parliamentarch-1.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 13:13:48.488122 parliamentarch-1.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 13:13:48.488122 parliamentarch-1.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-25 13:13:38.000000 parliamentarch-1.0.2/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-25 13:13:38.000000 parliamentarch-1.0.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-25 13:13:38.000000 parliamentarch-1.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-05-25 13:13:38.000000 parliamentarch-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13023 2024-05-25 13:13:38.000000 parliamentarch-1.0.2/LISEZMOI.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    14438 2024-05-25 13:13:48.492123 parliamentarch-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12414 2024-05-25 13:13:38.000000 parliamentarch-1.0.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-25 13:13:38.000000 parliamentarch-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 13:13:48.492123 parliamentarch-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 13:13:48.488122 parliamentarch-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 13:13:48.492123 parliamentarch-1.0.2/src/ParliamentArch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14438 2024-05-25 13:13:48.000000 parliamentarch-1.0.2/src/ParliamentArch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-25 13:13:48.000000 parliamentarch-1.0.2/src/ParliamentArch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 13:13:48.000000 parliamentarch-1.0.2/src/ParliamentArch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-25 13:13:48.000000 parliamentarch-1.0.2/src/ParliamentArch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 13:13:48.492123 parliamentarch-1.0.2/src/parliamentarch/
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-25 13:13:38.000000 parliamentarch-1.0.2/src/parliamentarch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-05-25 13:13:38.000000 parliamentarch-1.0.2/src/parliamentarch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-05-25 13:13:38.000000 parliamentarch-1.0.2/src/parliamentarch/_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8869 2024-05-25 13:13:38.000000 parliamentarch-1.0.2/src/parliamentarch/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6378 2024-05-25 13:13:38.000000 parliamentarch-1.0.2/src/parliamentarch/svg.py
```

### Comparing `parliamentarch-1.0.1/.github/workflows/python-package.yml` & `parliamentarch-1.0.2/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `parliamentarch-1.0.1/.github/workflows/python-publish.yml` & `parliamentarch-1.0.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `parliamentarch-1.0.1/LICENSE` & `parliamentarch-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `parliamentarch-1.0.1/LISEZMOI.rst` & `parliamentarch-1.0.2/LISEZMOI.rst`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,16 @@
 ``write_svg_from_attribution(file, attrib, **kwargs)``
 
 Cette fonction écrit un fichier SVG représentant un hémicycle. Les paramètres
 sont les suivants :
 
 - ``file: str|io.TextIOBase`` : un fichier ouvert en mode texte, ou le chemin
   vers le fichier sur lequel écrire. Si un chemin est fourni, le fichier sera
-  créé si il n'existe pas, et sera écrasé sinon.
+  écrit sous l'encodage UTF-8, et il sera créé si il n'existe pas et sinon
+  réécrit.
 - ``attrib: dict[SeatData, int]`` : un dictionnaire d'objets SeatData
   s'appliquant à un ensemble de sièges présents dans l'hémicycle, vers le nombre
   de sièges auxquels l'objet s'applique. Typiquement, chaque objet correspond à
   un parti ou un groupe. L'ordre des clés a un sens, et les éléments seront
   disposés de gauche à droite dans l'hémicycle.
 - ``**kwargs`` : tous les paramètres optionnels acceptés par
   ``parliamentarch.geometry.get_seats_centers`` ou par
@@ -197,15 +198,16 @@
 ``write_svg(file, seat_centers, seat_actual_radius, *, canvas_size=175, margins=5., write_number_of_seats=True, font_size_factor=...)``
 
 Cette fonction écrit un fichier SVG représentant un hémicycle. Les paramètres
 sont les suivants :
 
 - ``file: str|io.TextIOBase`` : un fichier ouvert en mode texte, ou le chemin
   vers le fichier sur lequel écrire. Si un chemin est fourni, le fichier sera
-  créé si il n'existe pas, et sera écrasé sinon.
+  écrit sous l'encodage UTF-8, et il sera créé si il n'existe pas et sinon
+  réécrit.
 - ``seat_centers: dict[tuple[float, float], SeatData]`` : un dictionnaire des
   coordonnées (x, y) des centres des sièges vers des objets SeatData.
 - ``seat_actual_radius: float`` : le rayon des sièges, tel que renvoyé par
   ``get_seats_centers``.
 - ``canvas_size: float`` : la hauteur du rectangle 2:1 dans lequel l'hémicycle
   est inscrit.
 - ``margins: float|tuple[float, float]|tuple[float, float, float, float]`` : les
```

### Comparing `parliamentarch-1.0.1/PKG-INFO` & `parliamentarch-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ParliamentArch
-Version: 1.0.1
+Version: 1.0.2
 Summary: Generation of arch-styled parliamentary arches
 Author: Gouvernathor
 License: BSD 3-Clause License
         
         Copyright (c) 2024, Gouvernathor
         
         Redistribution and use in source and binary forms, with or without
@@ -119,16 +119,17 @@
 
 ``write_svg_from_attribution(file, attrib, **kwargs)``
 
 This function writes an SVG file representing a hemicycle. The parameters are as
 follows:
 
 - ``file: str|io.TextIOBase``: a file-like object open in text mode, or the path
-  to the file to write on. If a path is provided, the file will be created if it
-  doesn't exist, and otherwise overwritten.
+  to the file to write on. If a path is provided, the file will be written to in
+  UTF-8 encoding, and it will be created if it doesn't exist or overwritten if
+  it does.
 - ``attrib: dict[SeatData, int]``: a mapping from a SeatData object applying to
   a number of seats in the resulting hemicycle, to the number of seats each
   object applies to. Typically, each SeatData object corresponds to a group or
   party. The ordering of the keys matter, and the elements will be arranged from
   left to right in the hemicycle.
 - ``**kwargs``: all optional keyword parameters taken by
   ``parliamentarch.geometry.get_seats_centers`` or by
@@ -234,16 +235,17 @@
 
 ``write_svg(file, seat_centers, seat_actual_radius, *, canvas_size=175, margins=5., write_number_of_seats=True, font_size_factor=...)``
 
 This function writes an SVG file representing a hemicycle. The parameters are as
 follows:
 
 - ``file: str|io.TextIOBase``: a file-like object open in text mode, or the path
-  to the file to write on. If a path is provided, the file will be created if it
-  doesn't exist, and otherwise overwritten.
+  to the file to write on. If a path is provided, the file will be written to in
+  UTF-8 encoding, and it will be created if it doesn't exist or overwritten if
+  it does.
 - ``seat_centers: dict[tuple[float, float], SeatData]``: a mapping from the
   (x, y) coordinates of each seat's center to a SeatData object.
 - ``seat_actual_radius: float``: as output by ``get_seats_centers``.
 - ``canvas_size: float``: the height of the 2:1 rectangle in which the hemicycle
   will be drawn.
 - ``margins: float|tuple[float, float]|tuple[float, float, float, float]``:
   the margins around that rectangle. If four values are given, they are the
```

### Comparing `parliamentarch-1.0.1/README.rst` & `parliamentarch-1.0.2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -80,16 +80,17 @@
 
 ``write_svg_from_attribution(file, attrib, **kwargs)``
 
 This function writes an SVG file representing a hemicycle. The parameters are as
 follows:
 
 - ``file: str|io.TextIOBase``: a file-like object open in text mode, or the path
-  to the file to write on. If a path is provided, the file will be created if it
-  doesn't exist, and otherwise overwritten.
+  to the file to write on. If a path is provided, the file will be written to in
+  UTF-8 encoding, and it will be created if it doesn't exist or overwritten if
+  it does.
 - ``attrib: dict[SeatData, int]``: a mapping from a SeatData object applying to
   a number of seats in the resulting hemicycle, to the number of seats each
   object applies to. Typically, each SeatData object corresponds to a group or
   party. The ordering of the keys matter, and the elements will be arranged from
   left to right in the hemicycle.
 - ``**kwargs``: all optional keyword parameters taken by
   ``parliamentarch.geometry.get_seats_centers`` or by
@@ -195,16 +196,17 @@
 
 ``write_svg(file, seat_centers, seat_actual_radius, *, canvas_size=175, margins=5., write_number_of_seats=True, font_size_factor=...)``
 
 This function writes an SVG file representing a hemicycle. The parameters are as
 follows:
 
 - ``file: str|io.TextIOBase``: a file-like object open in text mode, or the path
-  to the file to write on. If a path is provided, the file will be created if it
-  doesn't exist, and otherwise overwritten.
+  to the file to write on. If a path is provided, the file will be written to in
+  UTF-8 encoding, and it will be created if it doesn't exist or overwritten if
+  it does.
 - ``seat_centers: dict[tuple[float, float], SeatData]``: a mapping from the
   (x, y) coordinates of each seat's center to a SeatData object.
 - ``seat_actual_radius: float``: as output by ``get_seats_centers``.
 - ``canvas_size: float``: the height of the 2:1 rectangle in which the hemicycle
   will be drawn.
 - ``margins: float|tuple[float, float]|tuple[float, float, float, float]``:
   the margins around that rectangle. If four values are given, they are the
```

### Comparing `parliamentarch-1.0.1/src/ParliamentArch.egg-info/PKG-INFO` & `parliamentarch-1.0.2/src/ParliamentArch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ParliamentArch
-Version: 1.0.1
+Version: 1.0.2
 Summary: Generation of arch-styled parliamentary arches
 Author: Gouvernathor
 License: BSD 3-Clause License
         
         Copyright (c) 2024, Gouvernathor
         
         Redistribution and use in source and binary forms, with or without
@@ -119,16 +119,17 @@
 
 ``write_svg_from_attribution(file, attrib, **kwargs)``
 
 This function writes an SVG file representing a hemicycle. The parameters are as
 follows:
 
 - ``file: str|io.TextIOBase``: a file-like object open in text mode, or the path
-  to the file to write on. If a path is provided, the file will be created if it
-  doesn't exist, and otherwise overwritten.
+  to the file to write on. If a path is provided, the file will be written to in
+  UTF-8 encoding, and it will be created if it doesn't exist or overwritten if
+  it does.
 - ``attrib: dict[SeatData, int]``: a mapping from a SeatData object applying to
   a number of seats in the resulting hemicycle, to the number of seats each
   object applies to. Typically, each SeatData object corresponds to a group or
   party. The ordering of the keys matter, and the elements will be arranged from
   left to right in the hemicycle.
 - ``**kwargs``: all optional keyword parameters taken by
   ``parliamentarch.geometry.get_seats_centers`` or by
@@ -234,16 +235,17 @@
 
 ``write_svg(file, seat_centers, seat_actual_radius, *, canvas_size=175, margins=5., write_number_of_seats=True, font_size_factor=...)``
 
 This function writes an SVG file representing a hemicycle. The parameters are as
 follows:
 
 - ``file: str|io.TextIOBase``: a file-like object open in text mode, or the path
-  to the file to write on. If a path is provided, the file will be created if it
-  doesn't exist, and otherwise overwritten.
+  to the file to write on. If a path is provided, the file will be written to in
+  UTF-8 encoding, and it will be created if it doesn't exist or overwritten if
+  it does.
 - ``seat_centers: dict[tuple[float, float], SeatData]``: a mapping from the
   (x, y) coordinates of each seat's center to a SeatData object.
 - ``seat_actual_radius: float``: as output by ``get_seats_centers``.
 - ``canvas_size: float``: the height of the 2:1 rectangle in which the hemicycle
   will be drawn.
 - ``margins: float|tuple[float, float]|tuple[float, float, float, float]``:
   the margins around that rectangle. If four values are given, they are the
```

### Comparing `parliamentarch-1.0.1/src/parliamentarch/__init__.py` & `parliamentarch-1.0.2/src/parliamentarch/__init__.py`

 * *Files identical despite different names*

### Comparing `parliamentarch-1.0.1/src/parliamentarch/__main__.py` & `parliamentarch-1.0.2/src/parliamentarch/__main__.py`

 * *Files identical despite different names*

### Comparing `parliamentarch-1.0.1/src/parliamentarch/_util.py` & `parliamentarch-1.0.2/src/parliamentarch/_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 _file_parameter = Parameter("file",
     Parameter.POSITIONAL_ONLY,
     annotation=str | TextIOBase)
 
 def write_from_get(get_func: Callable[..., str]) -> Callable[..., None]:
     def write_func(file, /, *args, **kwargs):
         if isinstance(file, str):
-            with open(file, "w") as f:
+            with open(file, "w", encoding="UTF-8") as f:
                 return write_func(f, *args, **kwargs)
         print(get_func(*args, **kwargs), file=file)
 
     get_sig = signature(get_func)
     write_sig = get_sig.replace(
         parameters=[_file_parameter] + list(get_sig.parameters.values()),
         return_annotation=None,
```

### Comparing `parliamentarch-1.0.1/src/parliamentarch/geometry.py` & `parliamentarch-1.0.2/src/parliamentarch/geometry.py`

 * *Files identical despite different names*

### Comparing `parliamentarch-1.0.1/src/parliamentarch/svg.py` & `parliamentarch-1.0.2/src/parliamentarch/svg.py`

 * *Files identical despite different names*

