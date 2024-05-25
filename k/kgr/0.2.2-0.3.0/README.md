# Comparing `tmp/kgr-0.2.2.tar.gz` & `tmp/kgr-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kgr-0.2.2.tar", last modified: Thu May 23 21:28:51 2024, max compression
+gzip compressed data, was "kgr-0.3.0.tar", last modified: Sat May 25 16:26:20 2024, max compression
```

## Comparing `kgr-0.2.2.tar` & `kgr-0.3.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1071 2024-04-13 20:46:37.220586 kgr-0.2.2/LICENSE
--rw-r--r--   0        0        0       73 2024-04-13 20:46:37.220754 kgr-0.2.2/README.md
--rw-r--r--   0        0        0      876 2024-05-23 21:28:51.835186 kgr-0.2.2/pyproject.toml
--rw-r--r--   0        0        0       94 2024-05-13 11:07:57.892389 kgr-0.2.2/src/kgr/__init__.py
--rw-r--r--   0        0        0      645 2024-05-13 15:45:03.297572 kgr-0.2.2/src/kgr/__main__.py
--rw-r--r--   0        0        0     3210 2024-05-23 21:24:15.791694 kgr-0.2.2/src/kgr/convert.py
--rw-r--r--   0        0        0     3396 2024-05-23 19:50:12.189075 kgr-0.2.2/src/kgr/geocode.py
--rw-r--r--   0        0        0     1302 2024-05-13 15:42:53.776396 kgr-0.2.2/src/kgr/lib.py
--rw-r--r--   0        0        0     2781 2024-05-13 15:46:54.378388 kgr-0.2.2/src/kgr/prepare.py
--rw-r--r--   0        0        0     2042 1970-01-01 00:00:00.000000 kgr-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-04-13 20:46:37.220586 kgr-0.3.0/LICENSE
+-rw-r--r--   0        0        0     4833 2024-05-25 16:18:56.951691 kgr-0.3.0/README.md
+-rw-r--r--   0        0        0      905 2024-05-25 16:26:20.423607 kgr-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       94 2024-05-13 11:07:57.892389 kgr-0.3.0/src/kgr/__init__.py
+-rw-r--r--   0        0        0      638 2024-05-25 12:02:03.622507 kgr-0.3.0/src/kgr/__main__.py
+-rw-r--r--   0        0        0     3210 2024-05-25 16:10:04.054117 kgr-0.3.0/src/kgr/convert.py
+-rw-r--r--   0        0        0     3396 2024-05-23 19:50:12.189075 kgr-0.3.0/src/kgr/geocode.py
+-rw-r--r--   0        0        0     1302 2024-05-13 15:42:53.776396 kgr-0.3.0/src/kgr/lib.py
+-rw-r--r--   0        0        0     2781 2024-05-13 15:46:54.378388 kgr-0.3.0/src/kgr/prepare.py
+-rw-r--r--   0        0        0     6836 1970-01-01 00:00:00.000000 kgr-0.3.0/PKG-INFO
```

### Comparing `kgr-0.2.2/LICENSE` & `kgr-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kgr-0.2.2/pyproject.toml` & `kgr-0.3.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [project]
 name = "kgr"
-version = "0.2.2"
+version = "0.3.0"
 dependencies = [
     "requests",
     "geopy",
     "bs4",
 ]
 authors = [
     { name = "Dmitry Luschan", email = "dluschan@gmail.com" },
@@ -18,19 +18,20 @@
 maintainers = [
     { name = "Dmitry Luschan", email = "dluschan@gmail.com" },
 ]
 description = "Miltitool for convert data from https://memopzk.org to Google Maps"
 readme = "README.md"
 keywords = []
 classifiers = [
-    "Development Status :: 3 - Alpha",
+    "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
     "Topic :: Utilities",
+    "Environment :: Console",
 ]
 
 [project.license]
 file = "LICENSE"
 
 [project.urls]
 Homepage = "https://github.com/dluschan/kgr"
```

### Comparing `kgr-0.2.2/src/kgr/convert.py` & `kgr-0.3.0/src/kgr/convert.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 	name_tag = Document().createElement("name")
 	name_tag.appendChild(Document().createTextNode(row["ФИО"]))
 	placemark_tag.appendChild(name_tag)
 
 	p_tag = Document().createElement("p")
 	p_tag.appendChild(Document().createTextNode(row["description"] + src_name))
 	description_tag = Document().createElement("description")
-	if "img_src" in row.keys():
+	if "img_src" in row and row["img_src"]:
 		img_tag = Document().createElement("img")
 		img_tag.setAttribute("src", row["img_src"])
 		img_tag.setAttribute("alt", f"""Фотография: {row["ФИО"]}""")
 		description_tag.appendChild(Document().createCDATASection(img_tag.toprettyxml() + p_tag.toprettyxml()))
 	else:
 		description_tag.appendChild(Document().createCDATASection(p_tag.toprettyxml()))
 
@@ -57,15 +57,15 @@
 	root.appendChild(doc_tag)
 	return root
 
 
 def convert(args: Namespace) -> None:
 	"""Convert a datafile from CSV to KML format.
 	
-	The source file must contain columns "ФИО", "description", [img_src]", "lon", and "lat"."""
+	The source file must contain columns "ФИО", "description", "lon", and "lat"."""
 	if args.output is None:
 		args.output = args.input.with_suffix(".kml")
 	if args.suffix is None:
 		args.suffix = ""
 	else:
 		args.suffix = " " + args.suffix.strip()
 	if args.layout is None:
```

### Comparing `kgr-0.2.2/src/kgr/geocode.py` & `kgr-0.3.0/src/kgr/geocode.py`

 * *Files identical despite different names*

### Comparing `kgr-0.2.2/src/kgr/lib.py` & `kgr-0.3.0/src/kgr/lib.py`

 * *Files identical despite different names*

### Comparing `kgr-0.2.2/src/kgr/prepare.py` & `kgr-0.3.0/src/kgr/prepare.py`

 * *Files identical despite different names*

