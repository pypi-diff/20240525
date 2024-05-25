# Comparing `tmp/raimad-0.1.1.tar.gz` & `tmp/raimad-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raimad-0.1.1.tar", last modified: Fri May 24 18:14:07 2024, max compression
+gzip compressed data, was "raimad-0.1.2.tar", last modified: Fri May 24 18:15:10 2024, max compression
```

## Comparing `raimad-0.1.1.tar` & `raimad-0.1.2.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 maybetree  (1000) maybetree  (1000)        0 2024-05-24 18:14:07.675185 raimad-0.1.1/
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)    34893 2024-05-24 18:04:10.000000 raimad-0.1.1/LICENSE.md
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)    41373 2024-05-24 18:14:07.675185 raimad-0.1.1/PKG-INFO
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)      764 2024-05-24 18:04:10.000000 raimad-0.1.1/README.md
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)      742 2024-05-24 18:13:29.000000 raimad-0.1.1/pyproject.toml
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)      439 2024-05-24 18:14:07.676185 raimad-0.1.1/setup.cfg
-drwxr-xr-x   0 maybetree  (1000) maybetree  (1000)        0 2024-05-24 18:14:07.663184 raimad-0.1.1/src/
-drwxr-xr-x   0 maybetree  (1000) maybetree  (1000)        0 2024-05-24 18:14:07.670184 raimad-0.1.1/src/raimad/
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)     1775 2024-05-24 18:04:10.000000 raimad-0.1.1/src/raimad/__init__.py
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)     2921 2024-05-24 18:04:10.000000 raimad-0.1.1/src/raimad/affine.py
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)     7448 2024-05-24 18:04:10.000000 raimad-0.1.1/src/raimad/ansec.py
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)    14928 2024-05-24 18:04:10.000000 raimad-0.1.1/src/raimad/bbox.py
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)     1985 2024-05-24 18:04:10.000000 raimad-0.1.1/src/raimad/boundpoint.py
-drwxr-xr-x   0 maybetree  (1000) maybetree  (1000)        0 2024-05-24 18:14:07.671184 raimad-0.1.1/src/raimad/checker/
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)        1 2024-05-24 18:04:10.000000 raimad-0.1.1/src/raimad/checker/__init__.py
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)     4559 2024-05-24 18:04:10.000000 raimad-0.1.1/src/raimad/checker/checker.py
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)     1580 2024-05-24 18:04:10.000000 raimad-0.1.1/src/raimad/checker/violations.py
-drwxr-xr-x   0 maybetree  (1000) maybetree  (1000)        0 2024-05-24 18:14:07.672185 raimad-0.1.1/src/raimad/cif/
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)       29 2024-05-24 18:04:10.000000 raimad-0.1.1/src/raimad/cif/__init__.py
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)     1987 2024-05-24 18:04:10.000000 raimad-0.1.1/src/raimad/cif/noreuse.py
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)      730 2024-05-24 18:04:10.000000 raimad-0.1.1/src/raimad/circle.py
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)     6569 2024-05-24 18:04:10.000000 raimad-0.1.1/src/raimad/compo.py
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)     1668 2024-05-24 18:04:10.000000 raimad-0.1.1/src/raimad/custompoly.py
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)      221 2024-05-24 18:04:10.000000 raimad-0.1.1/src/raimad/debug.py
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)     2499 2024-05-24 18:04:10.000000 raimad-0.1.1/src/raimad/dictlist.py
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)      615 2024-05-24 18:04:10.000000 raimad-0.1.1/src/raimad/docparse.py
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)      972 2024-05-24 18:04:10.000000 raimad-0.1.1/src/raimad/empty.py
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)      605 2024-05-24 18:04:10.000000 raimad-0.1.1/src/raimad/err.py
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)     5535 2024-05-24 18:04:10.000000 raimad-0.1.1/src/raimad/fortunes.py
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)      773 2024-05-24 18:04:10.000000 raimad-0.1.1/src/raimad/graphviz.py
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)     3654 2024-05-24 18:04:10.000000 raimad-0.1.1/src/raimad/helpers.py
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)     3126 2024-05-24 18:04:10.000000 raimad-0.1.1/src/raimad/iters.py
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)      141 2024-05-24 18:04:10.000000 raimad-0.1.1/src/raimad/layer.py
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)      141 2024-05-24 18:04:10.000000 raimad-0.1.1/src/raimad/mark.py
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)      985 2024-05-24 18:04:10.000000 raimad-0.1.1/src/raimad/option.py
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)      444 2024-05-24 18:04:10.000000 raimad-0.1.1/src/raimad/partial.py
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)     8843 2024-05-24 18:04:10.000000 raimad-0.1.1/src/raimad/proxy.py
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)      746 2024-05-24 18:04:10.000000 raimad-0.1.1/src/raimad/rectwh.py
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)      824 2024-05-24 18:04:10.000000 raimad-0.1.1/src/raimad/rectwire.py
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)     1937 2024-05-24 18:04:10.000000 raimad-0.1.1/src/raimad/snowman.py
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)     1959 2024-05-24 18:04:10.000000 raimad-0.1.1/src/raimad/string_import.py
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)      892 2024-05-24 18:04:10.000000 raimad-0.1.1/src/raimad/svg.py
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)     5136 2024-05-24 18:04:10.000000 raimad-0.1.1/src/raimad/transform.py
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)      914 2024-05-24 18:04:10.000000 raimad-0.1.1/src/raimad/typing.py
-drwxr-xr-x   0 maybetree  (1000) maybetree  (1000)        0 2024-05-24 18:14:07.675185 raimad-0.1.1/src/raimad.egg-info/
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)    41373 2024-05-24 18:14:07.000000 raimad-0.1.1/src/raimad.egg-info/PKG-INFO
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)     1365 2024-05-24 18:14:07.000000 raimad-0.1.1/src/raimad.egg-info/SOURCES.txt
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)        1 2024-05-24 18:14:07.000000 raimad-0.1.1/src/raimad.egg-info/dependency_links.txt
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)       62 2024-05-24 18:14:07.000000 raimad-0.1.1/src/raimad.egg-info/entry_points.txt
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)        6 2024-05-24 18:14:07.000000 raimad-0.1.1/src/raimad.egg-info/requires.txt
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)        7 2024-05-24 18:14:07.000000 raimad-0.1.1/src/raimad.egg-info/top_level.txt
-drwxr-xr-x   0 maybetree  (1000) maybetree  (1000)        0 2024-05-24 18:14:07.674185 raimad-0.1.1/tests/
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)     8008 2024-05-24 18:04:10.000000 raimad-0.1.1/tests/test_bbox.py
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)     2200 2024-05-24 18:04:10.000000 raimad-0.1.1/tests/test_check_marks.py
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)     1512 2024-05-24 18:04:10.000000 raimad-0.1.1/tests/test_cif_noreuse.py
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)     1725 2024-05-24 18:04:10.000000 raimad-0.1.1/tests/test_compo.py
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)     2815 2024-05-24 18:04:10.000000 raimad-0.1.1/tests/test_compoclass_introspect.py
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)      739 2024-05-24 18:04:10.000000 raimad-0.1.1/tests/test_custom_base.py
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)     7003 2024-05-24 18:04:10.000000 raimad-0.1.1/tests/test_geoms_equal_mixin.py
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)     2398 2024-05-24 18:04:10.000000 raimad-0.1.1/tests/test_helpers.py
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)     4064 2024-05-24 18:04:10.000000 raimad-0.1.1/tests/test_lmap.py
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)     4398 2024-05-24 18:04:10.000000 raimad-0.1.1/tests/test_marks.py
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)     2179 2024-05-24 18:04:10.000000 raimad-0.1.1/tests/test_named_subcompos.py
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)     4268 2024-05-24 18:04:10.000000 raimad-0.1.1/tests/test_polys.py
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)      505 2024-05-24 18:04:10.000000 raimad-0.1.1/tests/test_snowman.py
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)     2743 2024-05-24 18:04:10.000000 raimad-0.1.1/tests/test_transform.py
+drwxr-xr-x   0 maybetree  (1000) maybetree  (1000)        0 2024-05-24 18:15:10.265048 raimad-0.1.2/
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)    34893 2024-05-24 18:04:10.000000 raimad-0.1.2/LICENSE.md
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)    41375 2024-05-24 18:15:10.265048 raimad-0.1.2/PKG-INFO
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)      764 2024-05-24 18:04:10.000000 raimad-0.1.2/README.md
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)      741 2024-05-24 18:14:44.000000 raimad-0.1.2/pyproject.toml
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)      439 2024-05-24 18:15:10.265048 raimad-0.1.2/setup.cfg
+drwxr-xr-x   0 maybetree  (1000) maybetree  (1000)        0 2024-05-24 18:15:10.253046 raimad-0.1.2/src/
+drwxr-xr-x   0 maybetree  (1000) maybetree  (1000)        0 2024-05-24 18:15:10.259047 raimad-0.1.2/src/raimad/
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)     1775 2024-05-24 18:04:10.000000 raimad-0.1.2/src/raimad/__init__.py
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)     2921 2024-05-24 18:04:10.000000 raimad-0.1.2/src/raimad/affine.py
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)     7448 2024-05-24 18:04:10.000000 raimad-0.1.2/src/raimad/ansec.py
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)    14928 2024-05-24 18:04:10.000000 raimad-0.1.2/src/raimad/bbox.py
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)     1985 2024-05-24 18:04:10.000000 raimad-0.1.2/src/raimad/boundpoint.py
+drwxr-xr-x   0 maybetree  (1000) maybetree  (1000)        0 2024-05-24 18:15:10.261047 raimad-0.1.2/src/raimad/checker/
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)        1 2024-05-24 18:04:10.000000 raimad-0.1.2/src/raimad/checker/__init__.py
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)     4559 2024-05-24 18:04:10.000000 raimad-0.1.2/src/raimad/checker/checker.py
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)     1580 2024-05-24 18:04:10.000000 raimad-0.1.2/src/raimad/checker/violations.py
+drwxr-xr-x   0 maybetree  (1000) maybetree  (1000)        0 2024-05-24 18:15:10.261047 raimad-0.1.2/src/raimad/cif/
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)       29 2024-05-24 18:04:10.000000 raimad-0.1.2/src/raimad/cif/__init__.py
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)     1987 2024-05-24 18:04:10.000000 raimad-0.1.2/src/raimad/cif/noreuse.py
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)      730 2024-05-24 18:04:10.000000 raimad-0.1.2/src/raimad/circle.py
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)     6569 2024-05-24 18:04:10.000000 raimad-0.1.2/src/raimad/compo.py
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)     1668 2024-05-24 18:04:10.000000 raimad-0.1.2/src/raimad/custompoly.py
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)      221 2024-05-24 18:04:10.000000 raimad-0.1.2/src/raimad/debug.py
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)     2499 2024-05-24 18:04:10.000000 raimad-0.1.2/src/raimad/dictlist.py
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)      615 2024-05-24 18:04:10.000000 raimad-0.1.2/src/raimad/docparse.py
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)      972 2024-05-24 18:04:10.000000 raimad-0.1.2/src/raimad/empty.py
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)      605 2024-05-24 18:04:10.000000 raimad-0.1.2/src/raimad/err.py
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)     5535 2024-05-24 18:04:10.000000 raimad-0.1.2/src/raimad/fortunes.py
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)      773 2024-05-24 18:04:10.000000 raimad-0.1.2/src/raimad/graphviz.py
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)     3654 2024-05-24 18:04:10.000000 raimad-0.1.2/src/raimad/helpers.py
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)     3126 2024-05-24 18:04:10.000000 raimad-0.1.2/src/raimad/iters.py
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)      141 2024-05-24 18:04:10.000000 raimad-0.1.2/src/raimad/layer.py
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)      141 2024-05-24 18:04:10.000000 raimad-0.1.2/src/raimad/mark.py
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)      985 2024-05-24 18:04:10.000000 raimad-0.1.2/src/raimad/option.py
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)      444 2024-05-24 18:04:10.000000 raimad-0.1.2/src/raimad/partial.py
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)     8843 2024-05-24 18:04:10.000000 raimad-0.1.2/src/raimad/proxy.py
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)      746 2024-05-24 18:04:10.000000 raimad-0.1.2/src/raimad/rectwh.py
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)      824 2024-05-24 18:04:10.000000 raimad-0.1.2/src/raimad/rectwire.py
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)     1937 2024-05-24 18:04:10.000000 raimad-0.1.2/src/raimad/snowman.py
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)     1959 2024-05-24 18:04:10.000000 raimad-0.1.2/src/raimad/string_import.py
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)      892 2024-05-24 18:04:10.000000 raimad-0.1.2/src/raimad/svg.py
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)     5136 2024-05-24 18:04:10.000000 raimad-0.1.2/src/raimad/transform.py
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)      914 2024-05-24 18:04:10.000000 raimad-0.1.2/src/raimad/typing.py
+drwxr-xr-x   0 maybetree  (1000) maybetree  (1000)        0 2024-05-24 18:15:10.264048 raimad-0.1.2/src/raimad.egg-info/
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)    41375 2024-05-24 18:15:10.000000 raimad-0.1.2/src/raimad.egg-info/PKG-INFO
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)     1365 2024-05-24 18:15:10.000000 raimad-0.1.2/src/raimad.egg-info/SOURCES.txt
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)        1 2024-05-24 18:15:10.000000 raimad-0.1.2/src/raimad.egg-info/dependency_links.txt
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)       62 2024-05-24 18:15:10.000000 raimad-0.1.2/src/raimad.egg-info/entry_points.txt
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)        6 2024-05-24 18:15:10.000000 raimad-0.1.2/src/raimad.egg-info/requires.txt
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)        7 2024-05-24 18:15:10.000000 raimad-0.1.2/src/raimad.egg-info/top_level.txt
+drwxr-xr-x   0 maybetree  (1000) maybetree  (1000)        0 2024-05-24 18:15:10.264048 raimad-0.1.2/tests/
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)     8008 2024-05-24 18:04:10.000000 raimad-0.1.2/tests/test_bbox.py
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)     2200 2024-05-24 18:04:10.000000 raimad-0.1.2/tests/test_check_marks.py
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)     1512 2024-05-24 18:04:10.000000 raimad-0.1.2/tests/test_cif_noreuse.py
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)     1725 2024-05-24 18:04:10.000000 raimad-0.1.2/tests/test_compo.py
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)     2815 2024-05-24 18:04:10.000000 raimad-0.1.2/tests/test_compoclass_introspect.py
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)      739 2024-05-24 18:04:10.000000 raimad-0.1.2/tests/test_custom_base.py
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)     7003 2024-05-24 18:04:10.000000 raimad-0.1.2/tests/test_geoms_equal_mixin.py
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)     2398 2024-05-24 18:04:10.000000 raimad-0.1.2/tests/test_helpers.py
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)     4064 2024-05-24 18:04:10.000000 raimad-0.1.2/tests/test_lmap.py
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)     4398 2024-05-24 18:04:10.000000 raimad-0.1.2/tests/test_marks.py
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)     2179 2024-05-24 18:04:10.000000 raimad-0.1.2/tests/test_named_subcompos.py
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)     4268 2024-05-24 18:04:10.000000 raimad-0.1.2/tests/test_polys.py
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)      505 2024-05-24 18:04:10.000000 raimad-0.1.2/tests/test_snowman.py
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)     2743 2024-05-24 18:04:10.000000 raimad-0.1.2/tests/test_transform.py
```

### Comparing `raimad-0.1.1/LICENSE.md` & `raimad-0.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `raimad-0.1.1/PKG-INFO` & `raimad-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: raimad
-Version: 0.1.1
-Summary: RAIMAD Astronomical Instrument MAsk Design
+Version: 0.1.2
+Summary: RAIMAD Astronomical Instrument MAsk Designer
 Author-email: maybetree <maybetree48@gmail.com>
 License: # GNU GENERAL PUBLIC LICENSE
         
         Version 3, 29 June 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc.
         <https://fsf.org/>
```

### Comparing `raimad-0.1.1/README.md` & `raimad-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `raimad-0.1.1/pyproject.toml` & `raimad-0.1.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -4,18 +4,16 @@
 # At least, when giving `setuptools` without a version,
 # I get an error that it can't find module `distutils`
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "raimad"
-version = "0.1.1"
-description = """\
-RAIMAD Astronomical Instrument MAsk Design
-"""
+version = "0.1.2"
+description = """RAIMAD Astronomical Instrument MAsk Designer"""
 authors = [
 	{name = "maybetree", email = "maybetree48@gmail.com"}
 	]
 license = { file = "LICENSE.md" }
 readme = "README.md"
 classifiers = [
 	'Programming Language :: Python :: 3',
```

### Comparing `raimad-0.1.1/src/raimad/__init__.py` & `raimad-0.1.2/src/raimad/__init__.py`

 * *Files identical despite different names*

### Comparing `raimad-0.1.1/src/raimad/affine.py` & `raimad-0.1.2/src/raimad/affine.py`

 * *Files identical despite different names*

### Comparing `raimad-0.1.1/src/raimad/ansec.py` & `raimad-0.1.2/src/raimad/ansec.py`

 * *Files identical despite different names*

### Comparing `raimad-0.1.1/src/raimad/bbox.py` & `raimad-0.1.2/src/raimad/bbox.py`

 * *Files identical despite different names*

### Comparing `raimad-0.1.1/src/raimad/boundpoint.py` & `raimad-0.1.2/src/raimad/boundpoint.py`

 * *Files identical despite different names*

### Comparing `raimad-0.1.1/src/raimad/checker/checker.py` & `raimad-0.1.2/src/raimad/checker/checker.py`

 * *Files identical despite different names*

### Comparing `raimad-0.1.1/src/raimad/checker/violations.py` & `raimad-0.1.2/src/raimad/checker/violations.py`

 * *Files identical despite different names*

### Comparing `raimad-0.1.1/src/raimad/cif/noreuse.py` & `raimad-0.1.2/src/raimad/cif/noreuse.py`

 * *Files identical despite different names*

### Comparing `raimad-0.1.1/src/raimad/circle.py` & `raimad-0.1.2/src/raimad/circle.py`

 * *Files identical despite different names*

### Comparing `raimad-0.1.1/src/raimad/compo.py` & `raimad-0.1.2/src/raimad/compo.py`

 * *Files identical despite different names*

### Comparing `raimad-0.1.1/src/raimad/custompoly.py` & `raimad-0.1.2/src/raimad/custompoly.py`

 * *Files identical despite different names*

### Comparing `raimad-0.1.1/src/raimad/dictlist.py` & `raimad-0.1.2/src/raimad/dictlist.py`

 * *Files identical despite different names*

### Comparing `raimad-0.1.1/src/raimad/docparse.py` & `raimad-0.1.2/src/raimad/docparse.py`

 * *Files identical despite different names*

### Comparing `raimad-0.1.1/src/raimad/empty.py` & `raimad-0.1.2/src/raimad/empty.py`

 * *Files identical despite different names*

### Comparing `raimad-0.1.1/src/raimad/err.py` & `raimad-0.1.2/src/raimad/err.py`

 * *Files identical despite different names*

### Comparing `raimad-0.1.1/src/raimad/fortunes.py` & `raimad-0.1.2/src/raimad/fortunes.py`

 * *Files identical despite different names*

### Comparing `raimad-0.1.1/src/raimad/graphviz.py` & `raimad-0.1.2/src/raimad/graphviz.py`

 * *Files identical despite different names*

### Comparing `raimad-0.1.1/src/raimad/helpers.py` & `raimad-0.1.2/src/raimad/helpers.py`

 * *Files identical despite different names*

### Comparing `raimad-0.1.1/src/raimad/iters.py` & `raimad-0.1.2/src/raimad/iters.py`

 * *Files identical despite different names*

### Comparing `raimad-0.1.1/src/raimad/option.py` & `raimad-0.1.2/src/raimad/option.py`

 * *Files identical despite different names*

### Comparing `raimad-0.1.1/src/raimad/proxy.py` & `raimad-0.1.2/src/raimad/proxy.py`

 * *Files identical despite different names*

### Comparing `raimad-0.1.1/src/raimad/rectwh.py` & `raimad-0.1.2/src/raimad/rectwh.py`

 * *Files identical despite different names*

### Comparing `raimad-0.1.1/src/raimad/rectwire.py` & `raimad-0.1.2/src/raimad/rectwire.py`

 * *Files identical despite different names*

### Comparing `raimad-0.1.1/src/raimad/snowman.py` & `raimad-0.1.2/src/raimad/snowman.py`

 * *Files identical despite different names*

### Comparing `raimad-0.1.1/src/raimad/string_import.py` & `raimad-0.1.2/src/raimad/string_import.py`

 * *Files identical despite different names*

### Comparing `raimad-0.1.1/src/raimad/svg.py` & `raimad-0.1.2/src/raimad/svg.py`

 * *Files identical despite different names*

### Comparing `raimad-0.1.1/src/raimad/transform.py` & `raimad-0.1.2/src/raimad/transform.py`

 * *Files identical despite different names*

### Comparing `raimad-0.1.1/src/raimad/typing.py` & `raimad-0.1.2/src/raimad/typing.py`

 * *Files identical despite different names*

### Comparing `raimad-0.1.1/src/raimad.egg-info/PKG-INFO` & `raimad-0.1.2/src/raimad.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: raimad
-Version: 0.1.1
-Summary: RAIMAD Astronomical Instrument MAsk Design
+Version: 0.1.2
+Summary: RAIMAD Astronomical Instrument MAsk Designer
 Author-email: maybetree <maybetree48@gmail.com>
 License: # GNU GENERAL PUBLIC LICENSE
         
         Version 3, 29 June 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc.
         <https://fsf.org/>
```

### Comparing `raimad-0.1.1/src/raimad.egg-info/SOURCES.txt` & `raimad-0.1.2/src/raimad.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `raimad-0.1.1/tests/test_bbox.py` & `raimad-0.1.2/tests/test_bbox.py`

 * *Files identical despite different names*

### Comparing `raimad-0.1.1/tests/test_check_marks.py` & `raimad-0.1.2/tests/test_check_marks.py`

 * *Files identical despite different names*

### Comparing `raimad-0.1.1/tests/test_cif_noreuse.py` & `raimad-0.1.2/tests/test_cif_noreuse.py`

 * *Files identical despite different names*

### Comparing `raimad-0.1.1/tests/test_compo.py` & `raimad-0.1.2/tests/test_compo.py`

 * *Files identical despite different names*

### Comparing `raimad-0.1.1/tests/test_compoclass_introspect.py` & `raimad-0.1.2/tests/test_compoclass_introspect.py`

 * *Files identical despite different names*

### Comparing `raimad-0.1.1/tests/test_custom_base.py` & `raimad-0.1.2/tests/test_custom_base.py`

 * *Files identical despite different names*

### Comparing `raimad-0.1.1/tests/test_geoms_equal_mixin.py` & `raimad-0.1.2/tests/test_geoms_equal_mixin.py`

 * *Files identical despite different names*

### Comparing `raimad-0.1.1/tests/test_helpers.py` & `raimad-0.1.2/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `raimad-0.1.1/tests/test_lmap.py` & `raimad-0.1.2/tests/test_lmap.py`

 * *Files identical despite different names*

### Comparing `raimad-0.1.1/tests/test_marks.py` & `raimad-0.1.2/tests/test_marks.py`

 * *Files identical despite different names*

### Comparing `raimad-0.1.1/tests/test_named_subcompos.py` & `raimad-0.1.2/tests/test_named_subcompos.py`

 * *Files identical despite different names*

### Comparing `raimad-0.1.1/tests/test_polys.py` & `raimad-0.1.2/tests/test_polys.py`

 * *Files identical despite different names*

### Comparing `raimad-0.1.1/tests/test_transform.py` & `raimad-0.1.2/tests/test_transform.py`

 * *Files identical despite different names*

