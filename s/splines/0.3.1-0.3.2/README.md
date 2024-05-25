# Comparing `tmp/splines-0.3.1.tar.gz` & `tmp/splines-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splines-0.3.1.tar", last modified: Thu Oct 19 17:27:55 2023, max compression
+gzip compressed data, was "splines-0.3.2.tar", last modified: Sat May 25 18:11:35 2024, max compression
```

## Comparing `splines-0.3.1.tar` & `splines-0.3.2.tar`

### file list

```diff
@@ -1,107 +1,84 @@
-drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2023-10-19 17:27:55.309205 splines-0.3.1/
-drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2023-10-19 17:27:55.269205 splines-0.3.1/.binder/
--rw-r--r--   0 mg        (1000) mg        (1000)      327 2023-03-12 15:36:42.000000 splines-0.3.1/.binder/README
--rw-r--r--   0 mg        (1000) mg        (1000)        0 2021-08-22 13:40:33.000000 splines-0.3.1/.binder/apt.txt
--rwxr-xr-x   0 mg        (1000) mg        (1000)       44 2021-08-22 13:40:33.000000 splines-0.3.1/.binder/postBuild
--rw-r--r--   0 mg        (1000) mg        (1000)       31 2022-11-24 21:30:17.000000 splines-0.3.1/.binder/requirements.txt
--rw-r--r--   0 mg        (1000) mg        (1000)      304 2018-07-09 18:17:30.000000 splines-0.3.1/.editorconfig
-drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2023-10-19 17:27:55.261205 splines-0.3.1/.github/
-drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2023-10-19 17:27:55.273205 splines-0.3.1/.github/workflows/
--rw-r--r--   0 mg        (1000) mg        (1000)     1708 2023-02-06 21:59:15.000000 splines-0.3.1/.github/workflows/docs.yml
--rw-r--r--   0 mg        (1000) mg        (1000)      863 2023-02-06 21:59:15.000000 splines-0.3.1/.github/workflows/tests.yml
--rw-r--r--   0 mg        (1000) mg        (1000)      100 2021-08-22 13:40:33.000000 splines-0.3.1/.gitignore
--rw-r--r--   0 mg        (1000) mg        (1000)      195 2023-10-19 17:08:49.000000 splines-0.3.1/.readthedocs.yml
--rw-r--r--   0 mg        (1000) mg        (1000)     1063 2023-03-12 15:36:42.000000 splines-0.3.1/LICENSE
--rw-r--r--   0 mg        (1000) mg        (1000)      163 2018-07-09 19:06:29.000000 splines-0.3.1/MANIFEST.in
--rw-r--r--   0 mg        (1000) mg        (1000)     1490 2023-10-19 17:27:55.309205 splines-0.3.1/PKG-INFO
--rw-r--r--   0 mg        (1000) mg        (1000)      629 2023-03-12 15:36:42.000000 splines-0.3.1/README.rst
--rwxr-xr-x   0 mg        (1000) mg        (1000)      281 2021-12-23 13:54:01.000000 splines-0.3.1/autobuild.sh
-drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2023-10-19 17:27:55.277205 splines-0.3.1/doc/
-drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2023-10-19 17:27:55.277205 splines-0.3.1/doc/_templates/
-drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2023-10-19 17:27:55.277205 splines-0.3.1/doc/_templates/autosummary/
--rw-r--r--   0 mg        (1000) mg        (1000)     1249 2023-05-24 20:38:31.000000 splines-0.3.1/doc/_templates/autosummary/module.rst
--rw-r--r--   0 mg        (1000) mg        (1000)      897 2023-01-08 18:29:13.000000 splines-0.3.1/doc/_templates/layout.html
--rw-r--r--   0 mg        (1000) mg        (1000)     5724 2023-10-19 17:08:49.000000 splines-0.3.1/doc/conf.py
-drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2023-10-19 17:27:55.297205 splines-0.3.1/doc/euclidean/
--rw-r--r--   0 mg        (1000) mg        (1000)     2362 2022-11-24 21:33:06.000000 splines-0.3.1/doc/euclidean/barry_goldman.py
--rw-r--r--   0 mg        (1000) mg        (1000)    28393 2023-06-27 20:56:30.000000 splines-0.3.1/doc/euclidean/bezier-de-casteljau.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)     6458 2023-05-24 20:38:31.000000 splines-0.3.1/doc/euclidean/bezier-non-uniform.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)     4297 2023-05-24 20:38:31.000000 splines-0.3.1/doc/euclidean/bezier-properties.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)     2076 2023-05-24 20:38:31.000000 splines-0.3.1/doc/euclidean/bezier.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)     1715 2021-09-29 20:01:14.000000 splines-0.3.1/doc/euclidean/casteljau.py
--rw-r--r--   0 mg        (1000) mg        (1000)    30816 2023-06-27 20:56:30.000000 splines-0.3.1/doc/euclidean/catmull-rom-barry-goldman.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)    23378 2023-06-27 20:56:30.000000 splines-0.3.1/doc/euclidean/catmull-rom-non-uniform.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)    25504 2023-06-27 20:56:30.000000 splines-0.3.1/doc/euclidean/catmull-rom-properties.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)    25787 2023-06-27 20:56:30.000000 splines-0.3.1/doc/euclidean/catmull-rom-uniform.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)     2113 2023-05-24 20:38:31.000000 splines-0.3.1/doc/euclidean/catmull-rom.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)     3735 2022-11-24 21:33:06.000000 splines-0.3.1/doc/euclidean/catmull_rom.py
--rw-r--r--   0 mg        (1000) mg        (1000)    17191 2023-05-24 20:38:31.000000 splines-0.3.1/doc/euclidean/end-conditions-natural.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)     1977 2023-10-19 17:08:49.000000 splines-0.3.1/doc/euclidean/end-conditions.rst
--rw-r--r--   0 mg        (1000) mg        (1000)     5734 2023-05-24 20:38:31.000000 splines-0.3.1/doc/euclidean/helper.py
--rw-r--r--   0 mg        (1000) mg        (1000)    17290 2023-06-27 20:56:30.000000 splines-0.3.1/doc/euclidean/hermite-non-uniform.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)     8746 2023-05-24 20:38:31.000000 splines-0.3.1/doc/euclidean/hermite-properties.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)    21534 2023-06-27 20:56:30.000000 splines-0.3.1/doc/euclidean/hermite-uniform.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)     1721 2021-08-22 13:40:33.000000 splines-0.3.1/doc/euclidean/hermite.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)     2397 2023-05-24 20:39:09.000000 splines-0.3.1/doc/euclidean/index.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)    13944 2023-05-24 20:38:31.000000 splines-0.3.1/doc/euclidean/kochanek-bartels-non-uniform.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)     6292 2023-05-24 20:38:31.000000 splines-0.3.1/doc/euclidean/kochanek-bartels-properties.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)    15000 2023-05-24 20:38:31.000000 splines-0.3.1/doc/euclidean/kochanek-bartels-uniform.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)     1568 2023-05-24 20:38:31.000000 splines-0.3.1/doc/euclidean/kochanek-bartels.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)     1335 2023-05-24 20:38:31.000000 splines-0.3.1/doc/euclidean/kochanek_bartels.py
--rw-r--r--   0 mg        (1000) mg        (1000)    20703 2023-05-24 20:39:09.000000 splines-0.3.1/doc/euclidean/lagrange.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)       36 2023-01-08 18:29:13.000000 splines-0.3.1/doc/euclidean/matplotlibrc
--rw-r--r--   0 mg        (1000) mg        (1000)     7526 2023-05-24 20:38:31.000000 splines-0.3.1/doc/euclidean/natural-non-uniform.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)     5080 2023-06-27 20:56:30.000000 splines-0.3.1/doc/euclidean/natural-properties.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)    14614 2023-06-27 20:56:30.000000 splines-0.3.1/doc/euclidean/natural-uniform.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)     1776 2022-11-24 21:33:06.000000 splines-0.3.1/doc/euclidean/natural.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)    32062 2023-05-24 20:38:31.000000 splines-0.3.1/doc/euclidean/piecewise-monotone.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)     8416 2023-06-27 20:56:30.000000 splines-0.3.1/doc/euclidean/polynomials.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)    11610 2023-06-27 20:56:30.000000 splines-0.3.1/doc/euclidean/quadrangle.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)    10260 2023-05-24 20:38:31.000000 splines-0.3.1/doc/euclidean/re-parameterization.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)    11703 2023-05-24 20:38:31.000000 splines-0.3.1/doc/euclidean/splines.rst
--rw-r--r--   0 mg        (1000) mg        (1000)     7149 2023-01-08 18:29:13.000000 splines-0.3.1/doc/euclidean/utility.py
--rw-r--r--   0 mg        (1000) mg        (1000)     1818 2021-08-22 13:40:33.000000 splines-0.3.1/doc/favicon.svg
--rw-r--r--   0 mg        (1000) mg        (1000)     1288 2023-03-12 15:36:42.000000 splines-0.3.1/doc/how-to-navigate.rst
--rw-r--r--   0 mg        (1000) mg        (1000)     1951 2023-03-12 15:36:42.000000 splines-0.3.1/doc/index.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)     3526 2023-05-24 20:39:09.000000 splines-0.3.1/doc/intro.rst
--rw-r--r--   0 mg        (1000) mg        (1000)       36 2023-01-08 18:29:13.000000 splines-0.3.1/doc/matplotlibrc
-drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2023-10-19 17:27:55.297205 splines-0.3.1/doc/python-module/
--rw-r--r--   0 mg        (1000) mg        (1000)      505 2023-05-18 10:39:00.000000 splines-0.3.1/doc/python-module/splines.quaternion.rst
--rw-r--r--   0 mg        (1000) mg        (1000)      406 2023-05-18 10:39:00.000000 splines-0.3.1/doc/python-module/splines.rst
--rw-r--r--   0 mg        (1000) mg        (1000)      110 2023-05-18 10:25:47.000000 splines-0.3.1/doc/python-module.rst
--rw-r--r--   0 mg        (1000) mg        (1000)     6954 2023-06-27 20:56:30.000000 splines-0.3.1/doc/references.bib
--rw-r--r--   0 mg        (1000) mg        (1000)      229 2023-03-12 15:36:42.000000 splines-0.3.1/doc/references.rst
--rw-r--r--   0 mg        (1000) mg        (1000)      226 2023-06-27 20:56:30.000000 splines-0.3.1/doc/requirements.txt
-drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2023-10-19 17:27:55.301205 splines-0.3.1/doc/rotation/
--rw-r--r--   0 mg        (1000) mg        (1000)    10830 2023-05-24 20:38:31.000000 splines-0.3.1/doc/rotation/barry-goldman.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)    13521 2023-05-24 20:38:31.000000 splines-0.3.1/doc/rotation/catmull-rom-non-uniform.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)    25605 2023-06-27 20:56:30.000000 splines-0.3.1/doc/rotation/catmull-rom-uniform.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)    14119 2023-05-24 20:38:31.000000 splines-0.3.1/doc/rotation/cumulative-form.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)     9181 2023-05-24 20:38:31.000000 splines-0.3.1/doc/rotation/de-casteljau.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)     5683 2023-05-24 20:38:31.000000 splines-0.3.1/doc/rotation/end-conditions-natural.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)     9613 2023-01-08 18:29:13.000000 splines-0.3.1/doc/rotation/helper.py
--rw-r--r--   0 mg        (1000) mg        (1000)     2611 2023-05-24 20:38:31.000000 splines-0.3.1/doc/rotation/index.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)    11334 2023-05-24 20:38:31.000000 splines-0.3.1/doc/rotation/kochanek-bartels.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)       36 2023-01-08 18:29:13.000000 splines-0.3.1/doc/rotation/matplotlibrc
--rw-r--r--   0 mg        (1000) mg        (1000)    10747 2023-05-24 20:38:31.000000 splines-0.3.1/doc/rotation/naive-4d-interpolation.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)     4503 2023-05-24 20:38:31.000000 splines-0.3.1/doc/rotation/naive-euler-angles-interpolation.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)    20730 2023-05-24 20:38:31.000000 splines-0.3.1/doc/rotation/quaternions.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)    17234 2023-05-24 20:38:31.000000 splines-0.3.1/doc/rotation/slerp.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)    16544 2023-06-27 20:56:30.000000 splines-0.3.1/doc/rotation/squad.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)      100 2023-02-06 21:59:15.000000 splines-0.3.1/pyproject.toml
--rw-r--r--   0 mg        (1000) mg        (1000)       38 2023-10-19 17:27:55.309205 splines-0.3.1/setup.cfg
--rw-r--r--   0 mg        (1000) mg        (1000)     1336 2023-02-06 21:59:15.000000 splines-0.3.1/setup.py
-drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2023-10-19 17:27:55.265205 splines-0.3.1/src/
-drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2023-10-19 17:27:55.305205 splines-0.3.1/src/splines/
--rw-r--r--   0 mg        (1000) mg        (1000)    33247 2023-10-19 17:08:49.000000 splines-0.3.1/src/splines/__init__.py
--rw-r--r--   0 mg        (1000) mg        (1000)    25850 2023-06-27 20:56:30.000000 splines-0.3.1/src/splines/quaternion.py
-drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2023-10-19 17:27:55.305205 splines-0.3.1/src/splines.egg-info/
--rw-r--r--   0 mg        (1000) mg        (1000)     1490 2023-10-19 17:27:55.000000 splines-0.3.1/src/splines.egg-info/PKG-INFO
--rw-r--r--   0 mg        (1000) mg        (1000)     2675 2023-10-19 17:27:55.000000 splines-0.3.1/src/splines.egg-info/SOURCES.txt
--rw-r--r--   0 mg        (1000) mg        (1000)        1 2023-10-19 17:27:55.000000 splines-0.3.1/src/splines.egg-info/dependency_links.txt
--rw-r--r--   0 mg        (1000) mg        (1000)        6 2023-10-19 17:27:55.000000 splines-0.3.1/src/splines.egg-info/requires.txt
--rw-r--r--   0 mg        (1000) mg        (1000)        8 2023-10-19 17:27:55.000000 splines-0.3.1/src/splines.egg-info/top_level.txt
--rw-r--r--   0 mg        (1000) mg        (1000)        1 2020-06-17 15:26:29.000000 splines-0.3.1/src/splines.egg-info/zip-safe
-drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2023-10-19 17:27:55.305205 splines-0.3.1/tests/
--rw-r--r--   0 mg        (1000) mg        (1000)        7 2018-09-15 15:50:44.000000 splines-0.3.1/tests/requirements.txt
--rw-r--r--   0 mg        (1000) mg        (1000)      250 2018-09-15 15:50:44.000000 splines-0.3.1/tests/test_catmullrom.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 18:11:35.234851 splines-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-25 18:11:31.000000 splines-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-25 18:11:31.000000 splines-0.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-05-25 18:11:35.234851 splines-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-25 18:11:31.000000 splines-0.3.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 18:11:35.226852 splines-0.3.2/doc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 18:11:35.222852 splines-0.3.2/doc/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 18:11:35.226852 splines-0.3.2/doc/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-25 18:11:31.000000 splines-0.3.2/doc/_templates/autosummary/module.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5992 2024-05-25 18:11:31.000000 splines-0.3.2/doc/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 18:11:35.230852 splines-0.3.2/doc/euclidean/
+-rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-05-25 18:11:31.000000 splines-0.3.2/doc/euclidean/barry_goldman.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28170 2024-05-25 18:11:31.000000 splines-0.3.2/doc/euclidean/bezier-de-casteljau.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6458 2024-05-25 18:11:31.000000 splines-0.3.2/doc/euclidean/bezier-non-uniform.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-05-25 18:11:31.000000 splines-0.3.2/doc/euclidean/bezier-properties.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-05-25 18:11:31.000000 splines-0.3.2/doc/euclidean/bezier.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-05-25 18:11:31.000000 splines-0.3.2/doc/euclidean/casteljau.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30816 2024-05-25 18:11:31.000000 splines-0.3.2/doc/euclidean/catmull-rom-barry-goldman.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    23378 2024-05-25 18:11:31.000000 splines-0.3.2/doc/euclidean/catmull-rom-non-uniform.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    25504 2024-05-25 18:11:31.000000 splines-0.3.2/doc/euclidean/catmull-rom-properties.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    25787 2024-05-25 18:11:31.000000 splines-0.3.2/doc/euclidean/catmull-rom-uniform.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-05-25 18:11:31.000000 splines-0.3.2/doc/euclidean/catmull-rom.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-05-25 18:11:31.000000 splines-0.3.2/doc/euclidean/catmull_rom.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17191 2024-05-25 18:11:31.000000 splines-0.3.2/doc/euclidean/end-conditions-natural.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-05-25 18:11:31.000000 splines-0.3.2/doc/euclidean/end-conditions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6032 2024-05-25 18:11:31.000000 splines-0.3.2/doc/euclidean/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17290 2024-05-25 18:11:31.000000 splines-0.3.2/doc/euclidean/hermite-non-uniform.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     8746 2024-05-25 18:11:31.000000 splines-0.3.2/doc/euclidean/hermite-properties.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    21440 2024-05-25 18:11:31.000000 splines-0.3.2/doc/euclidean/hermite-uniform.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-05-25 18:11:31.000000 splines-0.3.2/doc/euclidean/hermite.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-05-25 18:11:31.000000 splines-0.3.2/doc/euclidean/index.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    13928 2024-05-25 18:11:31.000000 splines-0.3.2/doc/euclidean/kochanek-bartels-non-uniform.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6292 2024-05-25 18:11:31.000000 splines-0.3.2/doc/euclidean/kochanek-bartels-properties.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    15000 2024-05-25 18:11:31.000000 splines-0.3.2/doc/euclidean/kochanek-bartels-uniform.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-05-25 18:11:31.000000 splines-0.3.2/doc/euclidean/kochanek-bartels.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-25 18:11:31.000000 splines-0.3.2/doc/euclidean/kochanek_bartels.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20703 2024-05-25 18:11:31.000000 splines-0.3.2/doc/euclidean/lagrange.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     7526 2024-05-25 18:11:31.000000 splines-0.3.2/doc/euclidean/natural-non-uniform.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5080 2024-05-25 18:11:31.000000 splines-0.3.2/doc/euclidean/natural-properties.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    14614 2024-05-25 18:11:31.000000 splines-0.3.2/doc/euclidean/natural-uniform.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-25 18:11:31.000000 splines-0.3.2/doc/euclidean/natural.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    32062 2024-05-25 18:11:31.000000 splines-0.3.2/doc/euclidean/piecewise-monotone.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     8416 2024-05-25 18:11:31.000000 splines-0.3.2/doc/euclidean/polynomials.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    11610 2024-05-25 18:11:31.000000 splines-0.3.2/doc/euclidean/quadrangle.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    10260 2024-05-25 18:11:31.000000 splines-0.3.2/doc/euclidean/re-parameterization.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    11703 2024-05-25 18:11:31.000000 splines-0.3.2/doc/euclidean/splines.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7149 2024-05-25 18:11:31.000000 splines-0.3.2/doc/euclidean/utility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-05-25 18:11:31.000000 splines-0.3.2/doc/how-to-navigate.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-05-25 18:11:31.000000 splines-0.3.2/doc/index.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-05-25 18:11:31.000000 splines-0.3.2/doc/intro.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-25 18:11:31.000000 splines-0.3.2/doc/python-module.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-25 18:11:31.000000 splines-0.3.2/doc/references.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-25 18:11:31.000000 splines-0.3.2/doc/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 18:11:35.234851 splines-0.3.2/doc/rotation/
+-rw-r--r--   0 runner    (1001) docker     (127)    10830 2024-05-25 18:11:31.000000 splines-0.3.2/doc/rotation/barry-goldman.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    13521 2024-05-25 18:11:31.000000 splines-0.3.2/doc/rotation/catmull-rom-non-uniform.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    25605 2024-05-25 18:11:31.000000 splines-0.3.2/doc/rotation/catmull-rom-uniform.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    14119 2024-05-25 18:11:31.000000 splines-0.3.2/doc/rotation/cumulative-form.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9181 2024-05-25 18:11:31.000000 splines-0.3.2/doc/rotation/de-casteljau.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5683 2024-05-25 18:11:31.000000 splines-0.3.2/doc/rotation/end-conditions-natural.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9613 2024-05-25 18:11:31.000000 splines-0.3.2/doc/rotation/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-05-25 18:11:31.000000 splines-0.3.2/doc/rotation/index.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    11334 2024-05-25 18:11:31.000000 splines-0.3.2/doc/rotation/kochanek-bartels.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    10747 2024-05-25 18:11:31.000000 splines-0.3.2/doc/rotation/naive-4d-interpolation.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-05-25 18:11:31.000000 splines-0.3.2/doc/rotation/naive-euler-angles-interpolation.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    20730 2024-05-25 18:11:31.000000 splines-0.3.2/doc/rotation/quaternions.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    17234 2024-05-25 18:11:31.000000 splines-0.3.2/doc/rotation/slerp.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    16544 2024-05-25 18:11:31.000000 splines-0.3.2/doc/rotation/squad.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-25 18:11:31.000000 splines-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 18:11:35.234851 splines-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-25 18:11:31.000000 splines-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 18:11:35.222852 splines-0.3.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 18:11:35.234851 splines-0.3.2/src/splines/
+-rw-r--r--   0 runner    (1001) docker     (127)    33322 2024-05-25 18:11:31.000000 splines-0.3.2/src/splines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25850 2024-05-25 18:11:31.000000 splines-0.3.2/src/splines/quaternion.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 18:11:35.234851 splines-0.3.2/src/splines.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-05-25 18:11:35.000000 splines-0.3.2/src/splines.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-05-25 18:11:35.000000 splines-0.3.2/src/splines.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 18:11:35.000000 splines-0.3.2/src/splines.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-25 18:11:35.000000 splines-0.3.2/src/splines.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-25 18:11:35.000000 splines-0.3.2/src/splines.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 18:11:35.000000 splines-0.3.2/src/splines.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 18:11:35.234851 splines-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-25 18:11:31.000000 splines-0.3.2/tests/test_catmullrom.py
```

### Comparing `splines-0.3.1/LICENSE` & `splines-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `splines-0.3.1/PKG-INFO` & `splines-0.3.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splines
-Version: 0.3.1
+Version: 0.3.2
 Summary: Splines in Euclidean Space and Beyond
 Home-page: https://splines.readthedocs.io/
 Author: Matthias Geier
 Author-email: Matthias.Geier@gmail.com
 License: MIT
 Project-URL: Documentation, https://splines.readthedocs.io/
 Project-URL: Source Code, https://github.com/AudioSceneDescriptionFormat/splines/
@@ -35,10 +35,12 @@
 
 Documentation notebooks on Binder
     https://mybinder.org/v2/gh/AudioSceneDescriptionFormat/splines/master?labpath=doc/index.ipynb
 
 Source code repository (and issue tracker)
     https://github.com/AudioSceneDescriptionFormat/splines
 
+DOI
+    https://doi.org/10.5281/zenodo.4568902
+
 License
     MIT -- see the file ``LICENSE`` for details.
-
```

### Comparing `splines-0.3.1/README.rst` & `splines-0.3.2/README.rst`

 * *Files 15% similar despite different names*

```diff
@@ -12,10 +12,12 @@
 
 Documentation notebooks on Binder
     https://mybinder.org/v2/gh/AudioSceneDescriptionFormat/splines/master?labpath=doc/index.ipynb
 
 Source code repository (and issue tracker)
     https://github.com/AudioSceneDescriptionFormat/splines
 
+DOI
+    https://doi.org/10.5281/zenodo.4568902
+
 License
     MIT -- see the file ``LICENSE`` for details.
-
```

### Comparing `splines-0.3.1/doc/_templates/autosummary/module.rst` & `splines-0.3.2/doc/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `splines-0.3.1/doc/conf.py` & `splines-0.3.2/doc/conf.py`

 * *Files 7% similar despite different names*

```diff
@@ -40,14 +40,19 @@
 linkcheck_ignore = [
     # Anchors with line numbers don't seem to work with linkcheck builder
     'https://github.com/scipy/scipy/blob/',
     # The idea of DOIs is that they are kept valid, so why check them at all?
     'https://doi.org/',
     # This causes timeout errors during linkcheck:
     'https://chm.secure.nonprofitsoapbox.com/donate',
+    # [SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed:
+    # unable to get local issuer certificate
+    'https://www.computerhistory.org/collections/catalog/102724883',
+    # 403 Client Error: Forbidden for url:
+    'https://stackoverflow.com/a/23980479/',
 ]
 
 nbsphinx_execute_arguments = [
     "--InlineBackend.figure_formats={'svg', 'pdf'}",
 ]
```

### Comparing `splines-0.3.1/doc/euclidean/barry_goldman.py` & `splines-0.3.2/doc/euclidean/barry_goldman.py`

 * *Files identical despite different names*

### Comparing `splines-0.3.1/doc/euclidean/bezier-de-casteljau.ipynb` & `splines-0.3.2/doc/euclidean/bezier-de-casteljau.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9976342520703934%*

 * *Differences: {"'cells'": "{5: {'source': {insert: [(1, 'from helper import plot_basis, plot_vertices_2d')], "*

 * *            "delete: [1]}}, 9: {'source': {insert: [(5, '    plot_vertices_2d(points, "*

 * *            "ax=ax)\\n')], delete: [12, 11, 10, 9, 8, 7, 6, 5]}}}",*

 * * "'metadata'": "{'language_info': {'version': '3.11.8'}}"}*

```diff
@@ -58,15 +58,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from utility import NamedExpression, NamedMatrix\n",
-                "from helper import plot_basis"
+                "from helper import plot_basis, plot_vertices_2d"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Let's prepare a few symbols for later use ..."
@@ -95,22 +95,15 @@
             "outputs": [],
             "source": [
                 "def plot_curve(func, points, dots=30, ax=None):\n",
                 "    if ax is None:\n",
                 "        ax = plt.gca()\n",
                 "    times = np.linspace(0, 1, dots)\n",
                 "    ax.plot(*func(points, times).T, '.')\n",
-                "    ax.plot(\n",
-                "        *np.asarray(points).T,\n",
-                "        color='lightgrey',\n",
-                "        linestyle=':',\n",
-                "        marker='x',\n",
-                "        markeredgecolor='black',\n",
-                "    )\n",
-                "    ax.scatter(*np.asarray(points).T, marker='x', c='black')\n",
+                "    plot_vertices_2d(points, ax=ax)\n",
                 "    ax.set_title(func.__name__ + ' B\u00e9zier curve')\n",
                 "    ax.axis('equal')"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
@@ -1193,13 +1186,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.2"
+            "version": "3.11.8"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `splines-0.3.1/doc/euclidean/bezier-non-uniform.ipynb` & `splines-0.3.2/doc/euclidean/bezier-non-uniform.ipynb`

 * *Files identical despite different names*

### Comparing `splines-0.3.1/doc/euclidean/bezier-properties.ipynb` & `splines-0.3.2/doc/euclidean/bezier-properties.ipynb`

 * *Files identical despite different names*

### Comparing `splines-0.3.1/doc/euclidean/bezier.ipynb` & `splines-0.3.2/doc/euclidean/bezier.ipynb`

 * *Files identical despite different names*

### Comparing `splines-0.3.1/doc/euclidean/casteljau.py` & `splines-0.3.2/doc/euclidean/casteljau.py`

 * *Files 10% similar despite different names*

```diff
@@ -51,12 +51,19 @@
     partial_curve = []
 
     def animation_func(t):
         ax.clear()
         if partial_curve:
             ax.plot(*np.asarray(partial_curve).T, '.', c='lightgrey')
         point = plot_casteljau(points, t, ax=ax)
-        ax.scatter(*np.asarray(points).T, marker='x', c='black')
+        ax.plot(
+            *np.asarray(points).T,
+            linestyle='',
+            marker='h',
+            markersize=10,
+            markeredgecolor='black',
+            markerfacecolor='none',
+        )
         partial_curve.append(point)
 
     times = np.linspace(0, 1, frames)
     return FuncAnimation(ax.figure, animation_func, frames=times, **kwargs)
```

### Comparing `splines-0.3.1/doc/euclidean/catmull-rom-barry-goldman.ipynb` & `splines-0.3.2/doc/euclidean/catmull-rom-barry-goldman.ipynb`

 * *Files identical despite different names*

### Comparing `splines-0.3.1/doc/euclidean/catmull-rom-non-uniform.ipynb` & `splines-0.3.2/doc/euclidean/catmull-rom-non-uniform.ipynb`

 * *Files identical despite different names*

### Comparing `splines-0.3.1/doc/euclidean/catmull-rom-properties.ipynb` & `splines-0.3.2/doc/euclidean/catmull-rom-properties.ipynb`

 * *Files identical despite different names*

### Comparing `splines-0.3.1/doc/euclidean/catmull-rom-uniform.ipynb` & `splines-0.3.2/doc/euclidean/catmull-rom-uniform.ipynb`

 * *Files identical despite different names*

### Comparing `splines-0.3.1/doc/euclidean/catmull-rom.ipynb` & `splines-0.3.2/doc/euclidean/catmull-rom.ipynb`

 * *Files identical despite different names*

### Comparing `splines-0.3.1/doc/euclidean/catmull_rom.py` & `splines-0.3.2/doc/euclidean/catmull_rom.py`

 * *Files identical despite different names*

### Comparing `splines-0.3.1/doc/euclidean/end-conditions-natural.ipynb` & `splines-0.3.2/doc/euclidean/end-conditions-natural.ipynb`

 * *Files identical despite different names*

### Comparing `splines-0.3.1/doc/euclidean/end-conditions.rst` & `splines-0.3.2/doc/euclidean/end-conditions.rst`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 There are many ways to provide this missing information,
 here we will mention only a few of them.
 
 clamped
     This means providing a fixed tangent (i.e. first derivative)
     at the beginning and end of a cubic spline.
-    For higher degree splines, additional derivatives have to be be specified.
+    For higher degree splines, additional derivatives have to be specified.
 
 natural
     For a cubic spline, this means setting the second derivative
     at the beginning and end of the spline to zero
     and calculating the first derivative from that constraint,
     see :doc:`end-conditions-natural`.
```

### Comparing `splines-0.3.1/doc/euclidean/helper.py` & `splines-0.3.2/doc/euclidean/helper.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,29 +58,39 @@
     for i in range(len(vertices) - 1):
         plot_tangent_2d(tangents[2 * i], vertices[i], color=color, **kwargs)
         plot_tangent_2d(
             tangents[2 * i + 1], vertices[i + 1], color=color, outgoing=False,
             **kwargs)
 
 
+def plot_vertices_2d(vertices, *, markeredgecolor='black', chords=True,
+                     ax=None):
+    if ax is None:
+        ax = _plt.gca()
+    ax.plot(
+        *_np.asarray(vertices).T,
+        color='lightgrey',
+        linestyle=(':' if chords else ''),
+        marker='h',
+        markersize=10,
+        markeredgecolor=markeredgecolor,
+        markerfacecolor='none',
+    )
+    ax.axis('equal')
+
+
 def plot_spline_2d(spline, dots_per_second=15, marker='.', linestyle='',
                    chords=True, ax=None, **kwargs):
     """Plot a two-dimensional spline."""
     if ax is None:
         ax = _plt.gca()
     total_duration = spline.grid[-1] - spline.grid[0]
     dots = int(total_duration * dots_per_second) + 1
     times = spline.grid[0] + _np.arange(dots) / dots_per_second
-    ax.plot(
-        *spline.evaluate(spline.grid).T,
-        color='lightgrey',
-        linestyle=(':' if chords else ''),
-        marker='x',
-        markeredgecolor='black',
-    )
+    plot_vertices_2d(spline.evaluate(spline.grid), chords=chords, ax=ax)
     ax.plot(
         *spline.evaluate(times).T,
         marker=marker,
         linestyle=linestyle,
         **kwargs)
     ax.axis('equal')
```

### Comparing `splines-0.3.1/doc/euclidean/hermite-non-uniform.ipynb` & `splines-0.3.2/doc/euclidean/hermite-non-uniform.ipynb`

 * *Files identical despite different names*

### Comparing `splines-0.3.1/doc/euclidean/hermite-properties.ipynb` & `splines-0.3.2/doc/euclidean/hermite-properties.ipynb`

 * *Files identical despite different names*

### Comparing `splines-0.3.1/doc/euclidean/hermite-uniform.ipynb` & `splines-0.3.2/doc/euclidean/hermite-uniform.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9959049823633157%*

 * *Differences: {"'cells'": "{49: {'source': {insert: [(0, 'import matplotlib.pyplot as plt\\n')]}}, 51: "*

 * *            "{'source': ['from helper import plot_spline_2d, plot_tangents_2d, "*

 * *            'plot_vertices_2d\']}, 79: {\'source\': {insert: [(2, "plot_vertices_2d(points, '*

 * *            'chords=False, markeredgecolor=\'purple\')\\n"), (4, '*

 * *            '"plt.annotate(r\'$\\\\quad\\\\tilde{\\\\bf{x}}_1$\', points[2]);")], delete: [4, '*

 * *            '2]}}, delete: [79]}',*

 * * "'metadata'": "{'language_info': {'version': '3 […]*

```diff
@@ -522,14 +522,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
+                "import matplotlib.pyplot as plt\n",
                 "import numpy as np"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -540,15 +541,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from helper import plot_spline_2d, plot_tangents_2d"
+                "from helper import plot_spline_2d, plot_tangents_2d, plot_vertices_2d"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -842,28 +843,19 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "import matplotlib.pyplot as plt"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
                 "plot_spline_2d(s, chords=False)\n",
                 "plot_tangents_2d(tangents, vertices)\n",
-                "plt.scatter(*points.T, marker='X', color='black')\n",
+                "plot_vertices_2d(points, chords=False, markeredgecolor='purple')\n",
                 "plt.annotate(r'$\\quad\\tilde{\\bf{x}}_0$', points[1])\n",
-                "plt.annotate(r'$\\tilde{\\bf{x}}_1\\quad$', points[2], ha='right');"
+                "plt.annotate(r'$\\quad\\tilde{\\bf{x}}_1$', points[2]);"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
@@ -875,13 +867,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.2"
+            "version": "3.11.8"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `splines-0.3.1/doc/euclidean/hermite.ipynb` & `splines-0.3.2/doc/euclidean/hermite.ipynb`

 * *Files identical despite different names*

### Comparing `splines-0.3.1/doc/euclidean/index.ipynb` & `splines-0.3.2/doc/euclidean/index.ipynb`

 * *Files identical despite different names*

### Comparing `splines-0.3.1/doc/euclidean/kochanek-bartels-non-uniform.ipynb` & `splines-0.3.2/doc/euclidean/kochanek-bartels-non-uniform.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9787894214703425%*

 * *Differences: {"'cells'": "{17: {'source': {insert: [(1, 'plot_vertices_2d(vertices1, chords=False)')], delete: "*

 * *            "[2, 1]}}, 25: {'source': {insert: [(0, '... and plot it for direct comparison\\n')], "*

 * *            "delete: [0]}}, insert: [(8, OrderedDict([('cell_type', 'markdown'), ('metadata', "*

 * *            'OrderedDict()), (\'source\', ["Let\'s import some helper functions from '*

 * *            '[helper.py](helper.py):"])])), (9, OrderedDict([(\'cell_type\', \'code\'), '*

 * *            "('execution_count', None), […]*

```diff
@@ -129,14 +129,30 @@
                 "import matplotlib.pyplot as plt"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
+                "Let's import some helper functions from [helper.py](helper.py):"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "from helper import plot_vertices_2d, plot_spline_2d"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
                 "We'll need the Hermite basis matrix\n",
                 "that we derived in the\n",
                 "[notebook about uniform Hermite splines](hermite-uniform.ipynb#Basis-Matrix)\n",
                 "and which is also shown by\n",
                 "<cite data-cite-t=\"kochanek1984tcb\">Kochanek and Bartels (1984)</cite>\n",
                 "in equation 2:"
             ]
@@ -237,16 +253,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "plt.scatter(*pseudo_catmull_rom(vertices1, inbetweens1).T, marker='.')\n",
-                "plt.scatter(*np.array(vertices1).T, marker='x', color='k')\n",
-                "plt.axis('equal');"
+                "plot_vertices_2d(vertices1, chords=False)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "This doesn't look too bad,\n",
@@ -309,31 +324,15 @@
                 "cr_spline1 = CatmullRom(vertices1, times1, endconditions='closed')"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "... and with a helper function from [helper.py](helper.py) ..."
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "from helper import plot_spline_2d"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "... we can plot it for direct comparison\n",
+                "... and plot it for direct comparison\n",
                 "with the one suggested by Kochanek and Bartels:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
@@ -481,27 +480,27 @@
                 "These equations are used in the implementation of the class\n",
                 "[splines.KochanekBartels](../python-module/splines.rst#splines.KochanekBartels)."
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3",
+            "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.9"
+            "version": "3.11.8"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `splines-0.3.1/doc/euclidean/kochanek-bartels-properties.ipynb` & `splines-0.3.2/doc/euclidean/kochanek-bartels-properties.ipynb`

 * *Files identical despite different names*

### Comparing `splines-0.3.1/doc/euclidean/kochanek-bartels-uniform.ipynb` & `splines-0.3.2/doc/euclidean/kochanek-bartels-uniform.ipynb`

 * *Files identical despite different names*

### Comparing `splines-0.3.1/doc/euclidean/kochanek-bartels.ipynb` & `splines-0.3.2/doc/euclidean/kochanek-bartels.ipynb`

 * *Files identical despite different names*

### Comparing `splines-0.3.1/doc/euclidean/kochanek_bartels.py` & `splines-0.3.2/doc/euclidean/kochanek_bartels.py`

 * *Files identical despite different names*

### Comparing `splines-0.3.1/doc/euclidean/lagrange.ipynb` & `splines-0.3.2/doc/euclidean/lagrange.ipynb`

 * *Files identical despite different names*

### Comparing `splines-0.3.1/doc/euclidean/natural-non-uniform.ipynb` & `splines-0.3.2/doc/euclidean/natural-non-uniform.ipynb`

 * *Files identical despite different names*

### Comparing `splines-0.3.1/doc/euclidean/natural-properties.ipynb` & `splines-0.3.2/doc/euclidean/natural-properties.ipynb`

 * *Files identical despite different names*

### Comparing `splines-0.3.1/doc/euclidean/natural-uniform.ipynb` & `splines-0.3.2/doc/euclidean/natural-uniform.ipynb`

 * *Files identical despite different names*

### Comparing `splines-0.3.1/doc/euclidean/natural.ipynb` & `splines-0.3.2/doc/euclidean/natural.ipynb`

 * *Files identical despite different names*

### Comparing `splines-0.3.1/doc/euclidean/piecewise-monotone.ipynb` & `splines-0.3.2/doc/euclidean/piecewise-monotone.ipynb`

 * *Files identical despite different names*

### Comparing `splines-0.3.1/doc/euclidean/polynomials.ipynb` & `splines-0.3.2/doc/euclidean/polynomials.ipynb`

 * *Files identical despite different names*

### Comparing `splines-0.3.1/doc/euclidean/quadrangle.ipynb` & `splines-0.3.2/doc/euclidean/quadrangle.ipynb`

 * *Files identical despite different names*

### Comparing `splines-0.3.1/doc/euclidean/re-parameterization.ipynb` & `splines-0.3.2/doc/euclidean/re-parameterization.ipynb`

 * *Files identical despite different names*

### Comparing `splines-0.3.1/doc/euclidean/splines.rst` & `splines-0.3.2/doc/euclidean/splines.rst`

 * *Files identical despite different names*

### Comparing `splines-0.3.1/doc/euclidean/utility.py` & `splines-0.3.2/doc/euclidean/utility.py`

 * *Files identical despite different names*

### Comparing `splines-0.3.1/doc/how-to-navigate.rst` & `splines-0.3.2/doc/how-to-navigate.rst`

 * *Files identical despite different names*

### Comparing `splines-0.3.1/doc/index.ipynb` & `splines-0.3.2/doc/index.ipynb`

 * *Files identical despite different names*

### Comparing `splines-0.3.1/doc/intro.rst` & `splines-0.3.2/doc/intro.rst`

 * *Files identical despite different names*

### Comparing `splines-0.3.1/doc/rotation/barry-goldman.ipynb` & `splines-0.3.2/doc/rotation/barry-goldman.ipynb`

 * *Files identical despite different names*

### Comparing `splines-0.3.1/doc/rotation/catmull-rom-non-uniform.ipynb` & `splines-0.3.2/doc/rotation/catmull-rom-non-uniform.ipynb`

 * *Files identical despite different names*

### Comparing `splines-0.3.1/doc/rotation/catmull-rom-uniform.ipynb` & `splines-0.3.2/doc/rotation/catmull-rom-uniform.ipynb`

 * *Files identical despite different names*

### Comparing `splines-0.3.1/doc/rotation/cumulative-form.ipynb` & `splines-0.3.2/doc/rotation/cumulative-form.ipynb`

 * *Files identical despite different names*

### Comparing `splines-0.3.1/doc/rotation/de-casteljau.ipynb` & `splines-0.3.2/doc/rotation/de-casteljau.ipynb`

 * *Files identical despite different names*

### Comparing `splines-0.3.1/doc/rotation/end-conditions-natural.ipynb` & `splines-0.3.2/doc/rotation/end-conditions-natural.ipynb`

 * *Files identical despite different names*

### Comparing `splines-0.3.1/doc/rotation/helper.py` & `splines-0.3.2/doc/rotation/helper.py`

 * *Files identical despite different names*

### Comparing `splines-0.3.1/doc/rotation/index.ipynb` & `splines-0.3.2/doc/rotation/index.ipynb`

 * *Files identical despite different names*

### Comparing `splines-0.3.1/doc/rotation/kochanek-bartels.ipynb` & `splines-0.3.2/doc/rotation/kochanek-bartels.ipynb`

 * *Files identical despite different names*

### Comparing `splines-0.3.1/doc/rotation/naive-4d-interpolation.ipynb` & `splines-0.3.2/doc/rotation/naive-4d-interpolation.ipynb`

 * *Files identical despite different names*

### Comparing `splines-0.3.1/doc/rotation/naive-euler-angles-interpolation.ipynb` & `splines-0.3.2/doc/rotation/naive-euler-angles-interpolation.ipynb`

 * *Files identical despite different names*

### Comparing `splines-0.3.1/doc/rotation/quaternions.ipynb` & `splines-0.3.2/doc/rotation/quaternions.ipynb`

 * *Files identical despite different names*

### Comparing `splines-0.3.1/doc/rotation/slerp.ipynb` & `splines-0.3.2/doc/rotation/slerp.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999379036264282%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(0, 'The [Wikipedia article for "*

 * *            "Slerp](https://en.wikipedia.org/wiki/Slerp#Quaternion_slerp)\\n')], delete: [0]}}}"}*

```diff
@@ -36,15 +36,15 @@
                 "to $1$ (where the expression simplifies to $q_2$)."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "The [Wikipedia article for Slerp](https://en.wikipedia.org/wiki/Slerp#Quaternion_Slerp)\n",
+                "The [Wikipedia article for Slerp](https://en.wikipedia.org/wiki/Slerp#Quaternion_slerp)\n",
                 "provides four equivalent ways to describe the same thing:\n",
                 "\n",
                 "\\begin{align*}\n",
                 "\\operatorname{Slerp}(q_0, q_1; t)\n",
                 "& = q_0 \\, \\left({q_0}^{-1} q_1\\right)^t \\\\\n",
                 "& = q_1 \\, \\left({q_1}^{-1} q_0\\right)^{1-t} \\\\\n",
                 "& = \\left(q_0 {q_1}^{-1}\\right)^{1-t} \\, q_1 \\\\\n",
```

### Comparing `splines-0.3.1/doc/rotation/squad.ipynb` & `splines-0.3.2/doc/rotation/squad.ipynb`

 * *Files identical despite different names*

### Comparing `splines-0.3.1/setup.py` & `splines-0.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `splines-0.3.1/src/splines/__init__.py` & `splines-0.3.2/src/splines/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from bisect import bisect_right as _bisect_right, bisect_left as _bisect_left
 from itertools import accumulate as _accumulate
 from math import factorial as _factorial
 
 import numpy as _np
 
 
-__version__ = '0.3.1'
+__version__ = '0.3.2'
 
 
 class Monomial:
     """Piecewise polynomial curve, see __init__()."""
 
     def __init__(self, segments, grid=None):
         r"""Piecewise polynomial curve using monomial basis.
@@ -515,14 +515,28 @@
             tangents = _np.concatenate([tangents, tangents[:1]])
         # Duplicate inner tangents (incoming and outgoing are the same):
         tangents = _np.concatenate(
             [tangents[i:i + 2] for i in range(len(tangents) - 1)])
         CubicHermite.__init__(self, vertices, tangents, grid)
 
 
+def _monotonous_slope(slope, left, right):
+    """Manipulate the slope to preserve monotonicity.
+
+    See Dougherty et al. (1989), eq. (4.2)
+
+    """
+    if left * right <= 0:
+        return 0
+    elif right > 0:
+        return min(max(0, slope), 3 * min(abs(left), abs(right)))
+    else:
+        return max(min(0, slope), -3 * min(abs(left), abs(right)))
+
+
 def _monotone_end_condition(inner_slope, secant_slope):
     """
 
     Return the "outer" (i.e. first or last) slope given the "inner"
     (i.e. second or penultimate) slope and the secant slope of the
     first or last segment.
 
@@ -581,56 +595,44 @@
 
         if closed:
             second_value = values[1:2]
             values = _np.concatenate([values, second_value])
             first_interval = grid[1] - grid[0]
             grid = list(grid) + [grid[-1] + first_interval]
 
-        def fix_slope(slope, left, right):
-            """Manipulate the slope to preserve monotonicity.
-
-            See Dougherty et al. (1989), eq. (4.2)
-
-            """
-            if left * right <= 0:
-                return 0
-            elif right > 0:
-                return min(max(0, slope), 3 * min(abs(left), abs(right)))
-            else:
-                return max(min(0, slope), -3 * min(abs(left), abs(right)))
-
         final_slopes = []
         for xs, ts, slope in zip(zip(values, values[1:], values[2:]),
                                  zip(grid, grid[1:], grid[2:]),
                                  slopes[1:]):
             x_1, x0, x1 = xs
             t_1, t0, t1 = ts
             left = (x0 - x_1) / (t0 - t_1)
             right = (x1 - x0) / (t1 - t0)
             if slope is None:
                 # NB: This has to be defined on the parent class:
                 slope = self._calculate_tangent(xs, ts)
-                slope = fix_slope(slope, left, right)
+                slope = _monotonous_slope(slope, left, right)
             else:
-                if slope != fix_slope(slope, left, right):
+                if slope != _monotonous_slope(slope, left, right):
                     raise ValueError(f'Slope too steep: {slope}')
             final_slopes.append(slope)  # incoming
             final_slopes.append(slope)  # outgoing
 
         if closed:
             # Move last outgoing slope to front:
             final_slopes = final_slopes[-1:] + final_slopes[:-1]
             values = values[:-1]
             grid = grid[:-1]
         elif not final_slopes:
             secant_slope = (values[1] - values[0]) / (grid[1] - grid[0])
             one, two = slopes
 
             def check_slope(slope):
-                if slope != fix_slope(slope, secant_slope, secant_slope):
+                if slope != _monotonous_slope(
+                        slope, secant_slope, secant_slope):
                     raise ValueError(f'Slope too steep or wrong sign: {slope}')
 
             if one is None:
                 if two is None:
                     final_slopes = [secant_slope] * 2
                 else:
                     check_slope(two)
@@ -649,15 +651,16 @@
                     final_slopes = [one, two]
         else:
 
             def end_slope(outer, inner, secant_slope):
                 if outer is None:
                     outer = _monotone_end_condition(inner, secant_slope)
                 else:
-                    if outer != fix_slope(outer, secant_slope, secant_slope):
+                    if outer != _monotonous_slope(
+                            outer, secant_slope, secant_slope):
                         raise ValueError(
                             f'Slope too steep or wrong sign: {outer}')
                 return outer
 
             final_slopes.insert(
                 0, end_slope(slopes[0], final_slopes[0],
                              (values[1] - values[0]) / (grid[1] - grid[0])))
@@ -690,24 +693,25 @@
         grid = _check_grid(grid, alpha, values)
         if cyclic:
             if slopes is None:
                 slopes = [None] * len(values)
             if (slopes[0], slopes[-1]) != (None, None):
                 raise ValueError(
                     'If "cyclic", the first and last slope must be None')
-            temp_values = (
-                values[-2],
-                values[-1],
-                values[-1] + (values[1] - values[0]))
-            temp_grid = (
-                grid[-2],
-                grid[-1],
-                grid[-1] + (grid[1] - grid[0]))
-            temp_spline = PiecewiseMonotoneCubic(temp_values, grid=temp_grid)
-            cyclic_slope = temp_spline.evaluate(temp_grid[1], 1)
+            x_1 = values[-2]
+            x0 = values[-1]
+            x1 = values[-1] + (values[1] - values[0])
+            t_1 = grid[-2]
+            t0 = grid[-1]
+            t1 = grid[-1] + (grid[1] - grid[0])
+            left = (x0 - x_1) / (t0 - t_1)
+            right = (x1 - x0) / (t1 - t0)
+            cyclic_slope = self._calculate_tangent(
+                (x_1, x0, x1), (t_1, t0, t1))
+            cyclic_slope = _monotonous_slope(cyclic_slope, left, right)
             slopes[0] = cyclic_slope
             slopes[-1] = cyclic_slope
 
         # NB: "alpha" has already been applied, we don't have to pass it on:
         PiecewiseMonotoneCubic.__init__(self, values, grid, slopes, **kwargs)
         diffs = _np.diff(values)
         if not (all(diffs >= 0) or all(diffs <= 0)):
```

### Comparing `splines-0.3.1/src/splines/quaternion.py` & `splines-0.3.2/src/splines/quaternion.py`

 * *Files identical despite different names*

### Comparing `splines-0.3.1/src/splines.egg-info/PKG-INFO` & `splines-0.3.2/src/splines.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splines
-Version: 0.3.1
+Version: 0.3.2
 Summary: Splines in Euclidean Space and Beyond
 Home-page: https://splines.readthedocs.io/
 Author: Matthias Geier
 Author-email: Matthias.Geier@gmail.com
 License: MIT
 Project-URL: Documentation, https://splines.readthedocs.io/
 Project-URL: Source Code, https://github.com/AudioSceneDescriptionFormat/splines/
@@ -35,10 +35,12 @@
 
 Documentation notebooks on Binder
     https://mybinder.org/v2/gh/AudioSceneDescriptionFormat/splines/master?labpath=doc/index.ipynb
 
 Source code repository (and issue tracker)
     https://github.com/AudioSceneDescriptionFormat/splines
 
+DOI
+    https://doi.org/10.5281/zenodo.4568902
+
 License
     MIT -- see the file ``LICENSE`` for details.
-
```

