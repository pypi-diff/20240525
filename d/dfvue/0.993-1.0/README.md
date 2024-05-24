# Comparing `tmp/dfvue-0.993.tar.gz` & `tmp/dfvue-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfvue-0.993.tar", last modified: Thu Dec 14 17:19:19 2023, max compression
+gzip compressed data, was "dfvue-1.0.tar", last modified: Fri May 24 22:09:00 2024, max compression
```

## Comparing `dfvue-0.993.tar` & `dfvue-1.0.tar`

### file list

```diff
@@ -1,168 +1,169 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 17:19:19.970597 dfvue-0.993/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2023-12-14 17:18:36.000000 dfvue-0.993/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)       66 2023-12-14 17:18:36.000000 dfvue-0.993/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2023-12-14 17:18:36.000000 dfvue-0.993/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10509 2023-12-14 17:19:19.970597 dfvue-0.993/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8180 2023-12-14 17:18:36.000000 dfvue-0.993/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      614 2023-12-14 17:18:36.000000 dfvue-0.993/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2023-12-14 17:19:19.970597 dfvue-0.993/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 17:19:19.934597 dfvue-0.993/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 17:19:19.938597 dfvue-0.993/src/dfvue/
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4251 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-12-14 17:19:19.000000 dfvue-0.993/src/dfvue/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2505 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/dfvmain.py
--rw-r--r--   0 runner    (1001) docker     (127)    29041 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/dfvreadcsv.py
--rw-r--r--   0 runner    (1001) docker     (127)    30973 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/dfvscatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5568 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/dfvue.py
--rw-r--r--   0 runner    (1001) docker     (127)     5207 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/dfvutils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 17:19:19.938597 dfvue-0.993/src/dfvue/images/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/images/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    47992 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/images/dfvue_icon.ico
--rw-r--r--   0 runner    (1001) docker     (127)    47970 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/images/dfvue_icon.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      273 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/images/image2ico.sh
--rw-r--r--   0 runner    (1001) docker     (127)    21491 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/ncvwidgets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 17:19:19.938597 dfvue-0.993/src/dfvue/themes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 17:19:19.942597 dfvue-0.993/src/dfvue/themes/azure-2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)   418679 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/Dark screenshot.png
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)   418500 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/Light screenshot.png
--rw-r--r--   0 runner    (1001) docker     (127)     4621 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     3261 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/azure.tcl
--rw-r--r--   0 runner    (1001) docker     (127)    11829 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 17:19:19.942597 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 17:19:19.954597 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/dark/
--rw-r--r--   0 runner    (1001) docker     (127)      424 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/dark/box-accent.png
--rw-r--r--   0 runner    (1001) docker     (127)      330 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/dark/box-basic.png
--rw-r--r--   0 runner    (1001) docker     (127)      357 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/dark/box-hover.png
--rw-r--r--   0 runner    (1001) docker     (127)      405 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/dark/box-invalid.png
--rw-r--r--   0 runner    (1001) docker     (127)      346 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/dark/button-hover.png
--rw-r--r--   0 runner    (1001) docker     (127)      457 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/dark/card.png
--rw-r--r--   0 runner    (1001) docker     (127)      482 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/dark/check-accent.png
--rw-r--r--   0 runner    (1001) docker     (127)      423 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/dark/check-basic.png
--rw-r--r--   0 runner    (1001) docker     (127)      453 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/dark/check-hover.png
--rw-r--r--   0 runner    (1001) docker     (127)      346 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/dark/check-tri-accent.png
--rw-r--r--   0 runner    (1001) docker     (127)      310 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/dark/check-tri-basic.png
--rw-r--r--   0 runner    (1001) docker     (127)      326 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/dark/check-tri-hover.png
--rw-r--r--   0 runner    (1001) docker     (127)      484 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/dark/circle-accent.png
--rw-r--r--   0 runner    (1001) docker     (127)      437 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/dark/circle-basic.png
--rw-r--r--   0 runner    (1001) docker     (127)      470 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/dark/circle-hover.png
--rw-r--r--   0 runner    (1001) docker     (127)      242 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/dark/combo-button-basic.png
--rw-r--r--   0 runner    (1001) docker     (127)      248 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/dark/combo-button-focus.png
--rw-r--r--   0 runner    (1001) docker     (127)      297 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/dark/combo-button-hover.png
--rw-r--r--   0 runner    (1001) docker     (127)      234 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/dark/down-accent.png
--rw-r--r--   0 runner    (1001) docker     (127)      261 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/dark/down.png
--rw-r--r--   0 runner    (1001) docker     (127)      130 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/dark/empty.png
--rw-r--r--   0 runner    (1001) docker     (127)      154 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/dark/hor-accent.png
--rw-r--r--   0 runner    (1001) docker     (127)      156 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/dark/hor-basic.png
--rw-r--r--   0 runner    (1001) docker     (127)      154 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/dark/hor-hover.png
--rw-r--r--   0 runner    (1001) docker     (127)      410 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/dark/notebook.png
--rw-r--r--   0 runner    (1001) docker     (127)      677 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/dark/off-basic.png
--rw-r--r--   0 runner    (1001) docker     (127)      736 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/dark/on-accent.png
--rw-r--r--   0 runner    (1001) docker     (127)      668 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/dark/on-basic.png
--rw-r--r--   0 runner    (1001) docker     (127)      587 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/dark/outline-basic.png
--rw-r--r--   0 runner    (1001) docker     (127)      644 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/dark/outline-hover.png
--rw-r--r--   0 runner    (1001) docker     (127)      629 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/dark/radio-accent.png
--rw-r--r--   0 runner    (1001) docker     (127)      561 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/dark/radio-basic.png
--rw-r--r--   0 runner    (1001) docker     (127)      625 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/dark/radio-hover.png
--rw-r--r--   0 runner    (1001) docker     (127)      524 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/dark/radio-tri-accent.png
--rw-r--r--   0 runner    (1001) docker     (127)      505 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/dark/radio-tri-basic.png
--rw-r--r--   0 runner    (1001) docker     (127)      466 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/dark/radio-tri-hover.png
--rw-r--r--   0 runner    (1001) docker     (127)      289 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/dark/rect-accent-hover.png
--rw-r--r--   0 runner    (1001) docker     (127)      319 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/dark/rect-accent.png
--rw-r--r--   0 runner    (1001) docker     (127)      286 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/dark/rect-basic.png
--rw-r--r--   0 runner    (1001) docker     (127)      297 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/dark/rect-hover.png
--rw-r--r--   0 runner    (1001) docker     (127)      255 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/dark/right.png
--rw-r--r--   0 runner    (1001) docker     (127)      161 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/dark/scale-hor.png
--rw-r--r--   0 runner    (1001) docker     (127)      161 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/dark/scale-vert.png
--rw-r--r--   0 runner    (1001) docker     (127)      128 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/dark/separator.png
--rw-r--r--   0 runner    (1001) docker     (127)      477 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/dark/size.png
--rw-r--r--   0 runner    (1001) docker     (127)      249 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/dark/tab-basic.png
--rw-r--r--   0 runner    (1001) docker     (127)      234 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/dark/tab-disabled.png
--rw-r--r--   0 runner    (1001) docker     (127)      260 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/dark/tab-hover.png
--rw-r--r--   0 runner    (1001) docker     (127)      302 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/dark/tick-hor-accent.png
--rw-r--r--   0 runner    (1001) docker     (127)      267 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/dark/tick-hor-basic.png
--rw-r--r--   0 runner    (1001) docker     (127)      280 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/dark/tick-hor-hover.png
--rw-r--r--   0 runner    (1001) docker     (127)      295 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/dark/tick-vert-accent.png
--rw-r--r--   0 runner    (1001) docker     (127)      257 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/dark/tick-vert-basic.png
--rw-r--r--   0 runner    (1001) docker     (127)      277 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/dark/tick-vert-hover.png
--rw-r--r--   0 runner    (1001) docker     (127)      149 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/dark/tree-basic.png
--rw-r--r--   0 runner    (1001) docker     (127)      168 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/dark/tree-pressed.png
--rw-r--r--   0 runner    (1001) docker     (127)      242 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/dark/up-accent.png
--rw-r--r--   0 runner    (1001) docker     (127)      271 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/dark/up.png
--rw-r--r--   0 runner    (1001) docker     (127)      158 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/dark/vert-accent.png
--rw-r--r--   0 runner    (1001) docker     (127)      158 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/dark/vert-basic.png
--rw-r--r--   0 runner    (1001) docker     (127)      158 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/dark/vert-hover.png
--rw-r--r--   0 runner    (1001) docker     (127)    19367 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/dark.tcl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 17:19:19.966596 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/light/
--rw-r--r--   0 runner    (1001) docker     (127)      346 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/light/box-accent.png
--rw-r--r--   0 runner    (1001) docker     (127)      319 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/light/box-basic.png
--rw-r--r--   0 runner    (1001) docker     (127)      329 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/light/box-hover.png
--rw-r--r--   0 runner    (1001) docker     (127)      285 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/light/box-invalid.png
--rw-r--r--   0 runner    (1001) docker     (127)      326 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/light/button-hover.png
--rw-r--r--   0 runner    (1001) docker     (127)      444 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/light/card.png
--rw-r--r--   0 runner    (1001) docker     (127)      442 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/light/check-accent.png
--rw-r--r--   0 runner    (1001) docker     (127)      390 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/light/check-basic.png
--rw-r--r--   0 runner    (1001) docker     (127)      451 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/light/check-hover.png
--rw-r--r--   0 runner    (1001) docker     (127)      314 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/light/check-tri-accent.png
--rw-r--r--   0 runner    (1001) docker     (127)      281 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/light/check-tri-basic.png
--rw-r--r--   0 runner    (1001) docker     (127)      319 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/light/check-tri-hover.png
--rw-r--r--   0 runner    (1001) docker     (127)      440 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/light/circle-accent.png
--rw-r--r--   0 runner    (1001) docker     (127)      128 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/light/circle-basic.png
--rw-r--r--   0 runner    (1001) docker     (127)      429 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/light/circle-hover.png
--rw-r--r--   0 runner    (1001) docker     (127)      247 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/light/combo-button-basic.png
--rw-r--r--   0 runner    (1001) docker     (127)      254 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/light/combo-button-focus.png
--rw-r--r--   0 runner    (1001) docker     (127)      299 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/light/combo-button-hover.png
--rw-r--r--   0 runner    (1001) docker     (127)      234 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/light/down-accent.png
--rw-r--r--   0 runner    (1001) docker     (127)      271 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/light/down.png
--rw-r--r--   0 runner    (1001) docker     (127)      130 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/light/empty.png
--rw-r--r--   0 runner    (1001) docker     (127)      153 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/light/hor-accent.png
--rw-r--r--   0 runner    (1001) docker     (127)      157 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/light/hor-basic.png
--rw-r--r--   0 runner    (1001) docker     (127)      154 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/light/hor-hover.png
--rw-r--r--   0 runner    (1001) docker     (127)      389 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/light/notebook.png
--rw-r--r--   0 runner    (1001) docker     (127)      547 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/light/off-basic.png
--rw-r--r--   0 runner    (1001) docker     (127)      663 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/light/off-hover.png
--rw-r--r--   0 runner    (1001) docker     (127)      635 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/light/on-accent.png
--rw-r--r--   0 runner    (1001) docker     (127)      538 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/light/on-basic.png
--rw-r--r--   0 runner    (1001) docker     (127)      649 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/light/on-hover.png
--rw-r--r--   0 runner    (1001) docker     (127)      508 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/light/outline-basic.png
--rw-r--r--   0 runner    (1001) docker     (127)      598 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/light/outline-hover.png
--rw-r--r--   0 runner    (1001) docker     (127)      554 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/light/radio-accent.png
--rw-r--r--   0 runner    (1001) docker     (127)      482 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/light/radio-basic.png
--rw-r--r--   0 runner    (1001) docker     (127)      583 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/light/radio-hover.png
--rw-r--r--   0 runner    (1001) docker     (127)      471 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/light/radio-tri-accent.png
--rw-r--r--   0 runner    (1001) docker     (127)      400 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/light/radio-tri-basic.png
--rw-r--r--   0 runner    (1001) docker     (127)      465 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/light/radio-tri-hover.png
--rw-r--r--   0 runner    (1001) docker     (127)      283 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/light/rect-accent-hover.png
--rw-r--r--   0 runner    (1001) docker     (127)      292 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/light/rect-accent.png
--rw-r--r--   0 runner    (1001) docker     (127)      250 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/light/rect-basic.png
--rw-r--r--   0 runner    (1001) docker     (127)      294 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/light/rect-hover.png
--rw-r--r--   0 runner    (1001) docker     (127)      266 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/light/right.png
--rw-r--r--   0 runner    (1001) docker     (127)      161 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/light/scale-hor.png
--rw-r--r--   0 runner    (1001) docker     (127)      162 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/light/scale-vert.png
--rw-r--r--   0 runner    (1001) docker     (127)      128 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/light/separator.png
--rw-r--r--   0 runner    (1001) docker     (127)      471 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/light/size.png
--rw-r--r--   0 runner    (1001) docker     (127)      219 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/light/tab-basic.png
--rw-r--r--   0 runner    (1001) docker     (127)      220 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/light/tab-disabled.png
--rw-r--r--   0 runner    (1001) docker     (127)      263 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/light/tab-hover.png
--rw-r--r--   0 runner    (1001) docker     (127)      274 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/light/tick-hor-accent.png
--rw-r--r--   0 runner    (1001) docker     (127)      242 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/light/tick-hor-basic.png
--rw-r--r--   0 runner    (1001) docker     (127)      273 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/light/tick-hor-hover.png
--rw-r--r--   0 runner    (1001) docker     (127)      273 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/light/tick-vert-accent.png
--rw-r--r--   0 runner    (1001) docker     (127)      234 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/light/tick-vert-basic.png
--rw-r--r--   0 runner    (1001) docker     (127)      266 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/light/tick-vert-hover.png
--rw-r--r--   0 runner    (1001) docker     (127)      149 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/light/tree-basic.png
--rw-r--r--   0 runner    (1001) docker     (127)      169 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/light/tree-pressed.png
--rw-r--r--   0 runner    (1001) docker     (127)      242 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/light/up-accent.png
--rw-r--r--   0 runner    (1001) docker     (127)      270 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/light/up.png
--rw-r--r--   0 runner    (1001) docker     (127)      152 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/light/vert-accent.png
--rw-r--r--   0 runner    (1001) docker     (127)      158 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/light/vert-basic.png
--rw-r--r--   0 runner    (1001) docker     (127)      157 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/light/vert-hover.png
--rw-r--r--   0 runner    (1001) docker     (127)    19367 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/themes/azure-2.0/theme/light.tcl
--rw-r--r--   0 runner    (1001) docker     (127)     6675 2023-12-14 17:18:36.000000 dfvue-0.993/src/dfvue/tooltip.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 17:19:19.966596 dfvue-0.993/src/dfvue.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7601 2023-12-14 17:19:19.000000 dfvue-0.993/src/dfvue.egg-info/SOURCES.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 17:19:19.966596 dfvue-0.993/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-14 17:18:36.000000 dfvue-0.993/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:09:00.166042 dfvue-1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-24 22:08:22.000000 dfvue-1.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-24 22:08:22.000000 dfvue-1.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-24 22:08:22.000000 dfvue-1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16897 2024-05-24 22:09:00.166042 dfvue-1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14570 2024-05-24 22:08:22.000000 dfvue-1.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-24 22:08:22.000000 dfvue-1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-05-24 22:09:00.166042 dfvue-1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:09:00.138042 dfvue-1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:09:00.142042 dfvue-1.0/src/dfvue/
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-24 22:08:59.000000 dfvue-1.0/src/dfvue/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/dfvmain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29789 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/dfvreadcsv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31076 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/dfvscatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5568 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/dfvue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5207 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/dfvutils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:09:00.142042 dfvue-1.0/src/dfvue/images/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49635 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/images/dfvue_icon.exif.png
+-rw-r--r--   0 runner    (1001) docker     (127)    47992 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/images/dfvue_icon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    47970 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/images/dfvue_icon.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      273 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/images/image2ico.sh
+-rw-r--r--   0 runner    (1001) docker     (127)    21491 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/ncvwidgets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:09:00.142042 dfvue-1.0/src/dfvue/themes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:09:00.142042 dfvue-1.0/src/dfvue/themes/azure-2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)   418679 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/Dark screenshot.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)   418500 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/Light screenshot.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4621 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3261 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/azure.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)    11829 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:09:00.146042 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:09:00.154042 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/dark/
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/dark/box-accent.png
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/dark/box-basic.png
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/dark/box-hover.png
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/dark/box-invalid.png
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/dark/button-hover.png
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/dark/card.png
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/dark/check-accent.png
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/dark/check-basic.png
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/dark/check-hover.png
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/dark/check-tri-accent.png
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/dark/check-tri-basic.png
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/dark/check-tri-hover.png
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/dark/circle-accent.png
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/dark/circle-basic.png
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/dark/circle-hover.png
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/dark/combo-button-basic.png
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/dark/combo-button-focus.png
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/dark/combo-button-hover.png
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/dark/down-accent.png
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/dark/down.png
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/dark/empty.png
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/dark/hor-accent.png
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/dark/hor-basic.png
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/dark/hor-hover.png
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/dark/notebook.png
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/dark/off-basic.png
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/dark/on-accent.png
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/dark/on-basic.png
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/dark/outline-basic.png
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/dark/outline-hover.png
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/dark/radio-accent.png
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/dark/radio-basic.png
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/dark/radio-hover.png
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/dark/radio-tri-accent.png
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/dark/radio-tri-basic.png
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/dark/radio-tri-hover.png
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/dark/rect-accent-hover.png
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/dark/rect-accent.png
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/dark/rect-basic.png
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/dark/rect-hover.png
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/dark/right.png
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/dark/scale-hor.png
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/dark/scale-vert.png
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/dark/separator.png
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/dark/size.png
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/dark/tab-basic.png
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/dark/tab-disabled.png
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/dark/tab-hover.png
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/dark/tick-hor-accent.png
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/dark/tick-hor-basic.png
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/dark/tick-hor-hover.png
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/dark/tick-vert-accent.png
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/dark/tick-vert-basic.png
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/dark/tick-vert-hover.png
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/dark/tree-basic.png
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/dark/tree-pressed.png
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/dark/up-accent.png
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/dark/up.png
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/dark/vert-accent.png
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/dark/vert-basic.png
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/dark/vert-hover.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19367 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/dark.tcl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:09:00.166042 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/light/
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/light/box-accent.png
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/light/box-basic.png
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/light/box-hover.png
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/light/box-invalid.png
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/light/button-hover.png
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/light/card.png
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/light/check-accent.png
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/light/check-basic.png
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/light/check-hover.png
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/light/check-tri-accent.png
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/light/check-tri-basic.png
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/light/check-tri-hover.png
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/light/circle-accent.png
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/light/circle-basic.png
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/light/circle-hover.png
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/light/combo-button-basic.png
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/light/combo-button-focus.png
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/light/combo-button-hover.png
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/light/down-accent.png
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/light/down.png
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/light/empty.png
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/light/hor-accent.png
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/light/hor-basic.png
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/light/hor-hover.png
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/light/notebook.png
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/light/off-basic.png
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/light/off-hover.png
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/light/on-accent.png
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/light/on-basic.png
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/light/on-hover.png
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/light/outline-basic.png
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/light/outline-hover.png
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/light/radio-accent.png
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/light/radio-basic.png
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/light/radio-hover.png
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/light/radio-tri-accent.png
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/light/radio-tri-basic.png
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/light/radio-tri-hover.png
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/light/rect-accent-hover.png
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/light/rect-accent.png
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/light/rect-basic.png
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/light/rect-hover.png
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/light/right.png
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/light/scale-hor.png
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/light/scale-vert.png
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/light/separator.png
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/light/size.png
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/light/tab-basic.png
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/light/tab-disabled.png
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/light/tab-hover.png
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/light/tick-hor-accent.png
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/light/tick-hor-basic.png
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/light/tick-hor-hover.png
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/light/tick-vert-accent.png
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/light/tick-vert-basic.png
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/light/tick-vert-hover.png
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/light/tree-basic.png
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/light/tree-pressed.png
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/light/up-accent.png
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/light/up.png
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/light/vert-accent.png
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/light/vert-basic.png
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/light/vert-hover.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19367 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/themes/azure-2.0/theme/light.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)     6675 2024-05-24 22:08:22.000000 dfvue-1.0/src/dfvue/tooltip.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:09:00.166042 dfvue-1.0/src/dfvue.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7638 2024-05-24 22:09:00.000000 dfvue-1.0/src/dfvue.egg-info/SOURCES.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:09:00.166042 dfvue-1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 22:08:22.000000 dfvue-1.0/tests/__init__.py
```

### Comparing `dfvue-0.993/LICENSE` & `dfvue-1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dfvue-0.993/pyproject.toml` & `dfvue-1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dfvue-0.993/setup.cfg` & `dfvue-1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `dfvue-0.993/src/dfvue/__init__.py` & `dfvue-1.0/src/dfvue/__init__.py`

 * *Files identical despite different names*

### Comparing `dfvue-0.993/src/dfvue/__main__.py` & `dfvue-1.0/src/dfvue/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,31 +44,31 @@
     parser.add_argument('-s', '--sep', action='store', type=str,
                         default=sep, dest='sep',
                         metavar='separator', help=hstr)
     hstr = ('Column(s) to use as index, either given as column index'
             ' or string name.')
     parser.add_argument('-i', '--index_col', action='store', type=str,
                         default=index_col, dest='index_col',
-                        metavar='column(s)', help=hstr)
-    hstr = ('Line numbers to skip (0-indexed, must include comma,'
+                        metavar='columns', help=hstr)
+    hstr = ('Line number(s) to skip (0-indexed, must include comma,'
             ' e.g. "1," for skipping the second row) or\n'
             'number of lines to skip (int, without comma) at the start'
             ' of the file.')
     parser.add_argument('-k', '--skiprows', action='store', type=str,
                         default=skiprows, dest='skiprows',
-                        metavar='#rows', help=hstr)
-    hstr = ('boolean. If True -> try parsing the index.\n'
-            'list of int or names. e.g. If 1, 2, 3\n'
-            '    -> try parsing columns 1, 2, 3 each as a separate date'
+                        metavar='rows', help=hstr)
+    hstr = ('boolean, if True -> try parsing the index.\n'
+            'list of int or names, e.g. 1,2,3\n'
+            '    -> try parsing columns 1, 2, and 3 each as a separate date'
             ' column.\n'
-            'list of lists. e.g. If [1, 3]\n'
+            'list of lists, e.g. [1,3]\n'
             '    -> combine columns 1 and 3 and parse as a single date'
             ' column.\n'
-            'dict, e.g. "foo" : [1, 3]\n'
-            '    -> parse columns 1, 3 as date and call result')
+            'dict, e.g. "foo":[1,3]\n'
+            '    -> parse columns 1 and 3 as date and call result "foo"')
     parser.add_argument('-p', '--parse_dates', action='store', type=str,
                         default=parse_dates, dest='parse_dates',
                         metavar='bool/list/dict', help=hstr)
     hstr = ('Will parse dates according to this format.\n'
             'For example: "%%Y-%%m-%%d %%H:%%M%%S". See\n'
             'https://docs.python.org/3/library/datetime.html#strftime-and-strptime-behavior')
     parser.add_argument('-d', '--date_format', action='store', type=str,
```

### Comparing `dfvue-0.993/src/dfvue/dfvmain.py` & `dfvue-1.0/src/dfvue/dfvmain.py`

 * *Files identical despite different names*

### Comparing `dfvue-0.993/src/dfvue/dfvreadcsv.py` & `dfvue-1.0/src/dfvue/dfvreadcsv.py`

 * *Files 2% similar despite different names*

```diff
@@ -508,24 +508,39 @@
 
         # label for read_csv options
         opthead = ttk.Frame(self)
         opthead.pack(side='top', fill='x')
         optheadlabel1 = ttk.Label(opthead, text='Options for')
         optheadlabel1.pack(side='left')
         # https://stackoverflow.com/questions/1529847/how-to-change-the-foreground-or-background-colour-of-a-tkinter-button-on-mac-os/42591118#42591118
-        ttk.Style().configure('blue.TLabel', foreground='blue')
+        ttk.Style().configure('blue.TLabel', foreground='#0096FF')
         optheadlabel2 = ttk.Label(opthead, text='pandas.read_csv',
                                   style='blue.TLabel')
         optheadlabel2.pack(side='left')
         # https://stackoverflow.com/questions/3655449/underline-text-in-tkinter-label-widget
         font = tkfont.Font(optheadlabel2, optheadlabel2.cget("font"))
         font.configure(underline=True)
         optheadlabel2.configure(font=font)
         optheadlabel2.bind("<Button-1>",
-                           lambda e: callurl("https://pandas.pydata.org/docs/reference/api/pandas.read_csv.html"))
+                           lambda e:
+                           callurl("https://pandas.pydata.org/docs/reference/"
+                                   "api/pandas.read_csv.html"))
+        optheadlabel3 = ttk.Label(opthead, text='(date_format: see')
+        optheadlabel3.pack(side='left')
+        optheadlabel4 = ttk.Label(opthead, text='strftime',
+                                  style='blue.TLabel')
+        optheadlabel4.pack(side='left')
+        optheadlabel4.configure(font=font)
+        optheadlabel4.bind("<Button-1>",
+                           lambda e:
+                           callurl("https://docs.python.org/3/library/"
+                                   "datetime.html#"
+                                   "strftime-and-strptime-behavior"))
+        optheadlabel5 = ttk.Label(opthead, text=')')
+        optheadlabel5.pack(side='left', padx=0)
 
         # option fields
         self.opt = {}     # option
         self.optlbl = {}  # label
         self.opttip = {}  # tooltip
 
         # rows with pandas.read_csv options
```

### Comparing `dfvue-0.993/src/dfvue/dfvscatter.py` & `dfvue-1.0/src/dfvue/dfvscatter.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,16 +32,20 @@
 from .dfvutils import clone_dfvmain, format_coord_scatter, vardim2var
 from .ncvwidgets import add_checkbutton, add_combobox, add_entry
 from .ncvwidgets import add_tooltip
 from .dfvreadcsv import dfvReadcsv
 # import matplotlib
 # matplotlib.use('TkAgg')
 from matplotlib import pyplot as plt
-# plt.style.use('seaborn-v0_8-darkgrid')
-plt.style.use('seaborn-v0_8-dark')
+try:
+    # plt.style.use('seaborn-v0_8-darkgrid')
+    plt.style.use('seaborn-v0_8-dark')
+except OSError:
+    # plt.style.use('seaborn-darkgrid')
+    plt.style.use('seaborn-dark')
 # plt.style.use('fast')
 
 
 __all__ = ['dfvScatter']
 
 
 class dfvScatter(ttk.Frame):
```

### Comparing `dfvue-0.993/src/dfvue/dfvue.py` & `dfvue-1.0/src/dfvue/dfvue.py`

 * *Files identical despite different names*

### Comparing `dfvue-0.993/src/dfvue/dfvutils.py` & `dfvue-1.0/src/dfvue/dfvutils.py`

 * *Files identical despite different names*

### Comparing `dfvue-0.993/src/dfvue/images/dfvue_icon.ico` & `dfvue-1.0/src/dfvue/images/dfvue_icon.ico`

 * *Files identical despite different names*

### Comparing `dfvue-0.993/src/dfvue/images/dfvue_icon.png` & `dfvue-1.0/src/dfvue/images/dfvue_icon.png`

 * *Files identical despite different names*

### Comparing `dfvue-0.993/src/dfvue/ncvwidgets.py` & `dfvue-1.0/src/dfvue/ncvwidgets.py`

 * *Files identical despite different names*

### Comparing `dfvue-0.993/src/dfvue/themes/azure-2.0/.gitignore` & `dfvue-1.0/src/dfvue/themes/azure-2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dfvue-0.993/src/dfvue/themes/azure-2.0/Dark screenshot.png` & `dfvue-1.0/src/dfvue/themes/azure-2.0/Dark screenshot.png`

 * *Files identical despite different names*

### Comparing `dfvue-0.993/src/dfvue/themes/azure-2.0/LICENSE` & `dfvue-1.0/src/dfvue/themes/azure-2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dfvue-0.993/src/dfvue/themes/azure-2.0/Light screenshot.png` & `dfvue-1.0/src/dfvue/themes/azure-2.0/Light screenshot.png`

 * *Files identical despite different names*

### Comparing `dfvue-0.993/src/dfvue/themes/azure-2.0/README.md` & `dfvue-1.0/src/dfvue/themes/azure-2.0/README.md`

 * *Files identical despite different names*

### Comparing `dfvue-0.993/src/dfvue/themes/azure-2.0/azure.tcl` & `dfvue-1.0/src/dfvue/themes/azure-2.0/azure.tcl`

 * *Files identical despite different names*

### Comparing `dfvue-0.993/src/dfvue/themes/azure-2.0/example.py` & `dfvue-1.0/src/dfvue/themes/azure-2.0/example.py`

 * *Files identical despite different names*

### Comparing `dfvue-0.993/src/dfvue/themes/azure-2.0/theme/dark/off-basic.png` & `dfvue-1.0/src/dfvue/themes/azure-2.0/theme/dark/off-basic.png`

 * *Files identical despite different names*

### Comparing `dfvue-0.993/src/dfvue/themes/azure-2.0/theme/dark/on-accent.png` & `dfvue-1.0/src/dfvue/themes/azure-2.0/theme/dark/on-accent.png`

 * *Files identical despite different names*

### Comparing `dfvue-0.993/src/dfvue/themes/azure-2.0/theme/dark/on-basic.png` & `dfvue-1.0/src/dfvue/themes/azure-2.0/theme/dark/on-basic.png`

 * *Files identical despite different names*

### Comparing `dfvue-0.993/src/dfvue/themes/azure-2.0/theme/dark/outline-basic.png` & `dfvue-1.0/src/dfvue/themes/azure-2.0/theme/dark/outline-basic.png`

 * *Files identical despite different names*

### Comparing `dfvue-0.993/src/dfvue/themes/azure-2.0/theme/dark/outline-hover.png` & `dfvue-1.0/src/dfvue/themes/azure-2.0/theme/dark/outline-hover.png`

 * *Files identical despite different names*

### Comparing `dfvue-0.993/src/dfvue/themes/azure-2.0/theme/dark/radio-accent.png` & `dfvue-1.0/src/dfvue/themes/azure-2.0/theme/dark/radio-accent.png`

 * *Files identical despite different names*

### Comparing `dfvue-0.993/src/dfvue/themes/azure-2.0/theme/dark/radio-basic.png` & `dfvue-1.0/src/dfvue/themes/azure-2.0/theme/dark/radio-basic.png`

 * *Files identical despite different names*

### Comparing `dfvue-0.993/src/dfvue/themes/azure-2.0/theme/dark/radio-hover.png` & `dfvue-1.0/src/dfvue/themes/azure-2.0/theme/dark/radio-hover.png`

 * *Files identical despite different names*

### Comparing `dfvue-0.993/src/dfvue/themes/azure-2.0/theme/dark/radio-tri-accent.png` & `dfvue-1.0/src/dfvue/themes/azure-2.0/theme/dark/radio-tri-accent.png`

 * *Files identical despite different names*

### Comparing `dfvue-0.993/src/dfvue/themes/azure-2.0/theme/dark.tcl` & `dfvue-1.0/src/dfvue/themes/azure-2.0/theme/dark.tcl`

 * *Files identical despite different names*

### Comparing `dfvue-0.993/src/dfvue/themes/azure-2.0/theme/light/off-basic.png` & `dfvue-1.0/src/dfvue/themes/azure-2.0/theme/light/off-basic.png`

 * *Files identical despite different names*

### Comparing `dfvue-0.993/src/dfvue/themes/azure-2.0/theme/light/off-hover.png` & `dfvue-1.0/src/dfvue/themes/azure-2.0/theme/light/off-hover.png`

 * *Files identical despite different names*

### Comparing `dfvue-0.993/src/dfvue/themes/azure-2.0/theme/light/on-accent.png` & `dfvue-1.0/src/dfvue/themes/azure-2.0/theme/light/on-accent.png`

 * *Files identical despite different names*

### Comparing `dfvue-0.993/src/dfvue/themes/azure-2.0/theme/light/on-basic.png` & `dfvue-1.0/src/dfvue/themes/azure-2.0/theme/light/on-basic.png`

 * *Files identical despite different names*

### Comparing `dfvue-0.993/src/dfvue/themes/azure-2.0/theme/light/on-hover.png` & `dfvue-1.0/src/dfvue/themes/azure-2.0/theme/light/on-hover.png`

 * *Files identical despite different names*

### Comparing `dfvue-0.993/src/dfvue/themes/azure-2.0/theme/light/outline-hover.png` & `dfvue-1.0/src/dfvue/themes/azure-2.0/theme/light/outline-hover.png`

 * *Files identical despite different names*

### Comparing `dfvue-0.993/src/dfvue/themes/azure-2.0/theme/light/radio-accent.png` & `dfvue-1.0/src/dfvue/themes/azure-2.0/theme/light/radio-accent.png`

 * *Files identical despite different names*

### Comparing `dfvue-0.993/src/dfvue/themes/azure-2.0/theme/light/radio-hover.png` & `dfvue-1.0/src/dfvue/themes/azure-2.0/theme/light/radio-hover.png`

 * *Files identical despite different names*

### Comparing `dfvue-0.993/src/dfvue/themes/azure-2.0/theme/light.tcl` & `dfvue-1.0/src/dfvue/themes/azure-2.0/theme/light.tcl`

 * *Files identical despite different names*

### Comparing `dfvue-0.993/src/dfvue/tooltip.py` & `dfvue-1.0/src/dfvue/tooltip.py`

 * *Files identical despite different names*

### Comparing `dfvue-0.993/src/dfvue.egg-info/SOURCES.txt` & `dfvue-1.0/src/dfvue.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 src/dfvue/dfvreadcsv.py
 src/dfvue/dfvscatter.py
 src/dfvue/dfvue.py
 src/dfvue/dfvutils.py
 src/dfvue/ncvwidgets.py
 src/dfvue/tooltip.py
 src/dfvue/images/__init__.py
+src/dfvue/images/dfvue_icon.exif.png
 src/dfvue/images/dfvue_icon.ico
 src/dfvue/images/dfvue_icon.png
 src/dfvue/images/image2ico.sh
 src/dfvue/themes/__init__.py
 src/dfvue/themes/azure-2.0/.gitignore
 src/dfvue/themes/azure-2.0/Dark screenshot.png
 src/dfvue/themes/azure-2.0/LICENSE
```

