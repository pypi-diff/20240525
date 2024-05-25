# Comparing `tmp/Orange3-WorldHappiness-0.1.8.tar.gz` & `tmp/Orange3-WorldHappiness-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Orange3-WorldHappiness-0.1.8.tar", last modified: Fri Aug 26 14:10:07 2022, max compression
+gzip compressed data, was "dist\Orange3-WorldHappiness-0.1.9.tar", last modified: Wed Nov 23 08:48:43 2022, max compression
```

## Comparing `Orange3-WorldHappiness-0.1.8.tar` & `Orange3-WorldHappiness-0.1.9.tar`

### file list

```diff
@@ -1,94 +1,96 @@
-drwxrwxrwx   0        0        0        0 2022-08-26 14:10:07.401840 Orange3-WorldHappiness-0.1.8/
--rw-rw-rw-   0        0        0    35147 2022-03-14 14:01:52.000000 Orange3-WorldHappiness-0.1.8/LICENSE.txt
--rw-rw-rw-   0        0        0      233 2022-03-14 13:00:44.000000 Orange3-WorldHappiness-0.1.8/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2022-08-26 14:10:07.333778 Orange3-WorldHappiness-0.1.8/Orange3_WorldHappiness.egg-info/
--rw-rw-rw-   0        0        0     1013 2022-08-26 14:10:07.000000 Orange3-WorldHappiness-0.1.8/Orange3_WorldHappiness.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3265 2022-08-26 14:10:07.000000 Orange3-WorldHappiness-0.1.8/Orange3_WorldHappiness.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-26 14:10:07.000000 Orange3-WorldHappiness-0.1.8/Orange3_WorldHappiness.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      232 2022-08-26 14:10:07.000000 Orange3-WorldHappiness-0.1.8/Orange3_WorldHappiness.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2022-08-26 14:10:07.000000 Orange3-WorldHappiness-0.1.8/Orange3_WorldHappiness.egg-info/namespace_packages.txt
--rw-rw-rw-   0        0        0        2 2022-08-26 14:10:06.000000 Orange3-WorldHappiness-0.1.8/Orange3_WorldHappiness.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       46 2022-08-26 14:10:07.000000 Orange3-WorldHappiness-0.1.8/Orange3_WorldHappiness.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2022-08-26 14:10:07.000000 Orange3-WorldHappiness-0.1.8/Orange3_WorldHappiness.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1013 2022-08-26 14:10:07.401840 Orange3-WorldHappiness-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0      992 2022-03-14 12:40:12.000000 Orange3-WorldHappiness-0.1.8/README.md
--rw-rw-rw-   0        0        0      334 2022-03-18 11:05:57.000000 Orange3-WorldHappiness-0.1.8/README.pypi
-drwxrwxrwx   0        0        0        0 2022-08-26 14:10:07.339783 Orange3-WorldHappiness-0.1.8/doc/
--rw-rw-rw-   0        0        0     6981 2022-03-14 12:26:00.000000 Orange3-WorldHappiness-0.1.8/doc/Makefile
-drwxrwxrwx   0        0        0        0 2022-08-26 14:10:07.305753 Orange3-WorldHappiness-0.1.8/doc/_build/
-drwxrwxrwx   0        0        0        0 2022-08-26 14:10:07.346789 Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/
--rw-rw-rw-   0        0        0      234 2022-07-06 07:21:33.000000 Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/.buildinfo
--rw-rw-rw-   0        0        0      684 2022-07-06 07:21:33.000000 Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/Orange3ImageAnalyticsdoc.hhc
--rw-rw-rw-   0        0        0       13 2022-07-06 07:21:33.000000 Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/Orange3ImageAnalyticsdoc.hhk
--rw-rw-rw-   0        0        0     1570 2022-07-06 07:21:33.000000 Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/Orange3ImageAnalyticsdoc.hhp
--rw-rw-rw-   0        0        0      165 2022-03-14 12:00:34.000000 Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/Orange3ImageAnalyticsdoc.stp
-drwxrwxrwx   0        0        0        0 2022-08-26 14:10:07.347790 Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/_images/
--rw-rw-rw-   0        0        0    94987 2022-03-18 11:32:19.000000 Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/_images/socioeconomic-indices.png
-drwxrwxrwx   0        0        0        0 2022-08-26 14:10:07.361803 Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/_static/
--rw-rw-rw-   0        0        0    15597 2022-07-06 07:21:32.000000 Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/_static/basic.css
-drwxrwxrwx   0        0        0        0 2022-08-26 14:10:07.363805 Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/_static/css/
--rw-rw-rw-   0        0        0     3275 2022-03-14 12:29:53.000000 Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/_static/css/badge_only.css
-drwxrwxrwx   0        0        0        0 2022-08-26 14:10:07.384824 Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/_static/css/fonts/
--rw-rw-rw-   0        0        0    87624 2022-03-14 12:29:53.000000 Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/_static/css/fonts/Roboto-Slab-Bold.woff
--rw-rw-rw-   0        0        0    67312 2022-03-14 12:29:53.000000 Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/_static/css/fonts/Roboto-Slab-Bold.woff2
--rw-rw-rw-   0        0        0    86288 2022-03-14 12:29:53.000000 Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/_static/css/fonts/Roboto-Slab-Regular.woff
--rw-rw-rw-   0        0        0    66444 2022-03-14 12:29:53.000000 Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/_static/css/fonts/Roboto-Slab-Regular.woff2
--rw-rw-rw-   0        0        0   165742 2022-03-14 12:29:53.000000 Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/_static/css/fonts/fontawesome-webfont.eot
--rw-rw-rw-   0        0        0   444379 2022-03-14 12:29:53.000000 Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/_static/css/fonts/fontawesome-webfont.svg
--rw-rw-rw-   0        0        0   165548 2022-03-14 12:29:53.000000 Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/_static/css/fonts/fontawesome-webfont.ttf
--rw-rw-rw-   0        0        0    98024 2022-03-14 12:29:53.000000 Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/_static/css/fonts/fontawesome-webfont.woff
--rw-rw-rw-   0        0        0    77160 2022-03-14 12:29:53.000000 Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/_static/css/fonts/fontawesome-webfont.woff2
--rw-rw-rw-   0        0        0   323344 2022-03-14 12:29:53.000000 Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/_static/css/fonts/lato-bold-italic.woff
--rw-rw-rw-   0        0        0   193308 2022-03-14 12:29:53.000000 Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/_static/css/fonts/lato-bold-italic.woff2
--rw-rw-rw-   0        0        0   309728 2022-03-14 12:29:53.000000 Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/_static/css/fonts/lato-bold.woff
--rw-rw-rw-   0        0        0   184912 2022-03-14 12:29:53.000000 Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/_static/css/fonts/lato-bold.woff2
--rw-rw-rw-   0        0        0   328412 2022-03-14 12:29:53.000000 Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/_static/css/fonts/lato-normal-italic.woff
--rw-rw-rw-   0        0        0   195704 2022-03-14 12:29:53.000000 Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/_static/css/fonts/lato-normal-italic.woff2
--rw-rw-rw-   0        0        0   309192 2022-03-14 12:29:53.000000 Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/_static/css/fonts/lato-normal.woff
--rw-rw-rw-   0        0        0   182708 2022-03-14 12:29:53.000000 Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/_static/css/fonts/lato-normal.woff2
--rw-rw-rw-   0        0        0   129674 2022-03-14 12:29:53.000000 Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/_static/css/theme.css
--rw-rw-rw-   0        0        0      549 2022-03-14 12:28:03.000000 Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/_static/custom.css
--rw-rw-rw-   0        0        0     9758 2022-03-14 12:00:37.000000 Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/_static/doctools.js
--rw-rw-rw-   0        0        0      365 2022-07-06 07:21:32.000000 Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/_static/documentation_options.js
--rw-rw-rw-   0        0        0      286 2022-03-14 12:00:37.000000 Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/_static/file.png
--rw-rw-rw-   0        0        0   287630 2022-03-14 12:00:37.000000 Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/_static/jquery-3.5.1.js
--rw-rw-rw-   0        0        0    89476 2022-03-14 12:00:37.000000 Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/_static/jquery.js
-drwxrwxrwx   0        0        0        0 2022-08-26 14:10:07.388828 Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/_static/js/
--rw-rw-rw-   0        0        0      934 2022-03-14 12:29:53.000000 Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/_static/js/badge_only.js
--rw-rw-rw-   0        0        0     4370 2022-03-14 12:29:53.000000 Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/_static/js/html5shiv-printshiv.min.js
--rw-rw-rw-   0        0        0     2734 2022-03-14 12:29:53.000000 Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/_static/js/html5shiv.min.js
--rw-rw-rw-   0        0        0     5023 2022-03-14 12:29:53.000000 Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/_static/js/theme.js
--rw-rw-rw-   0        0        0      339 2022-07-06 07:21:32.000000 Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/_static/language_data.js
--rw-rw-rw-   0        0        0       90 2022-03-14 12:00:37.000000 Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/_static/minus.png
--rw-rw-rw-   0        0        0       90 2022-03-14 12:00:37.000000 Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/_static/plus.png
--rw-rw-rw-   0        0        0     4919 2022-07-06 07:21:32.000000 Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/_static/pygments.css
--rw-rw-rw-   0        0        0    16793 2022-03-14 12:00:37.000000 Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/_static/searchtools.js
--rw-rw-rw-   0        0        0    68420 2022-03-14 12:00:37.000000 Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/_static/underscore-1.13.1.js
--rw-rw-rw-   0        0        0    19530 2022-03-14 12:00:37.000000 Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/_static/underscore.js
--rw-rw-rw-   0        0        0     3000 2022-07-06 07:21:32.000000 Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/genindex.html
--rw-rw-rw-   0        0        0     4313 2022-07-06 07:21:32.000000 Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/index.html
-drwxrwxrwx   0        0        0        0 2022-08-26 14:10:07.389829 Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/widgets/
--rw-rw-rw-   0        0        0     5209 2022-07-06 07:21:32.000000 Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/widgets/socioeconomicindices.html
--rw-rw-rw-   0        0        0     9246 2022-03-14 12:27:02.000000 Orange3-WorldHappiness-0.1.8/doc/conf.py
--rw-rw-rw-   0        0        0      291 2022-03-14 12:20:15.000000 Orange3-WorldHappiness-0.1.8/doc/index.rst
--rwxrwxrwx   0        0        0     6721 2022-03-14 12:25:42.000000 Orange3-WorldHappiness-0.1.8/doc/make.bat
-drwxrwxrwx   0        0        0        0 2022-08-26 14:10:07.390830 Orange3-WorldHappiness-0.1.8/doc/widgets/
-drwxrwxrwx   0        0        0        0 2022-08-26 14:10:07.391831 Orange3-WorldHappiness-0.1.8/doc/widgets/images/
--rw-rw-rw-   0        0        0    94987 2022-03-18 11:32:19.000000 Orange3-WorldHappiness-0.1.8/doc/widgets/images/socioeconomic-indices.png
--rw-rw-rw-   0        0        0     1248 2022-03-18 17:36:35.000000 Orange3-WorldHappiness-0.1.8/doc/widgets/socioeconomicindices.md
--rw-rw-rw-   0        0        0      353 2022-03-14 12:15:28.000000 Orange3-WorldHappiness-0.1.8/doc/widgets.json
-drwxrwxrwx   0        0        0        0 2022-08-26 14:10:07.393833 Orange3-WorldHappiness-0.1.8/orangecontrib/
--rw-rw-rw-   0        0        0      167 2022-03-14 10:43:14.000000 Orange3-WorldHappiness-0.1.8/orangecontrib/__init__.py
-drwxrwxrwx   0        0        0        0 2022-08-26 14:10:07.394833 Orange3-WorldHappiness-0.1.8/orangecontrib/worldhappiness/
--rw-rw-rw-   0        0        0        0 2022-03-14 10:43:14.000000 Orange3-WorldHappiness-0.1.8/orangecontrib/worldhappiness/__init__.py
-drwxrwxrwx   0        0        0        0 2022-08-26 14:10:07.396836 Orange3-WorldHappiness-0.1.8/orangecontrib/worldhappiness/whstudy/
--rw-rw-rw-   0        0        0     5656 2022-08-08 14:09:29.000000 Orange3-WorldHappiness-0.1.8/orangecontrib/worldhappiness/whstudy/__init__.py
--rw-rw-rw-   0        0        0    18839 2022-08-08 14:18:51.000000 Orange3-WorldHappiness-0.1.8/orangecontrib/worldhappiness/whstudy/world_data_api.py
-drwxrwxrwx   0        0        0        0 2022-08-26 14:10:07.398837 Orange3-WorldHappiness-0.1.8/orangecontrib/worldhappiness/widgets/
--rw-rw-rw-   0        0        0     1101 2022-03-14 12:40:28.000000 Orange3-WorldHappiness-0.1.8/orangecontrib/worldhappiness/widgets/__init__.py
-drwxrwxrwx   0        0        0        0 2022-08-26 14:10:07.400839 Orange3-WorldHappiness-0.1.8/orangecontrib/worldhappiness/widgets/icons/
--rw-rw-rw-   0        0        0      631 2022-03-18 08:43:41.000000 Orange3-WorldHappiness-0.1.8/orangecontrib/worldhappiness/widgets/icons/category.svg
--rw-rw-rw-   0        0        0      793 2022-03-18 08:43:41.000000 Orange3-WorldHappiness-0.1.8/orangecontrib/worldhappiness/widgets/icons/socioeconomicindices.svg
--rw-rw-rw-   0        0        0    27056 2022-08-26 14:08:01.000000 Orange3-WorldHappiness-0.1.8/orangecontrib/worldhappiness/widgets/owwhstudy.py
--rw-rw-rw-   0        0        0       42 2022-08-26 14:10:07.402840 Orange3-WorldHappiness-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     2834 2022-08-26 14:09:01.000000 Orange3-WorldHappiness-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2022-11-23 08:48:43.932042 Orange3-WorldHappiness-0.1.9/
+-rw-rw-rw-   0        0        0    35821 2022-03-25 08:44:41.000000 Orange3-WorldHappiness-0.1.9/LICENSE.txt
+-rw-rw-rw-   0        0        0      233 2022-03-25 08:44:41.000000 Orange3-WorldHappiness-0.1.9/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2022-11-23 08:48:43.814167 Orange3-WorldHappiness-0.1.9/Orange3_WorldHappiness.egg-info/
+-rw-rw-rw-   0        0        0     1104 2022-11-23 08:48:43.000000 Orange3-WorldHappiness-0.1.9/Orange3_WorldHappiness.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3381 2022-11-23 08:48:43.000000 Orange3-WorldHappiness-0.1.9/Orange3_WorldHappiness.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-11-23 08:48:43.000000 Orange3-WorldHappiness-0.1.9/Orange3_WorldHappiness.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      233 2022-11-23 08:48:43.000000 Orange3-WorldHappiness-0.1.9/Orange3_WorldHappiness.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2022-11-23 08:48:43.000000 Orange3-WorldHappiness-0.1.9/Orange3_WorldHappiness.egg-info/namespace_packages.txt
+-rw-rw-rw-   0        0        0        2 2022-03-25 08:52:48.000000 Orange3-WorldHappiness-0.1.9/Orange3_WorldHappiness.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       46 2022-11-23 08:48:43.000000 Orange3-WorldHappiness-0.1.9/Orange3_WorldHappiness.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2022-11-23 08:48:43.000000 Orange3-WorldHappiness-0.1.9/Orange3_WorldHappiness.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1104 2022-11-23 08:48:43.931044 Orange3-WorldHappiness-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0      992 2022-03-25 08:44:41.000000 Orange3-WorldHappiness-0.1.9/README.md
+-rw-rw-rw-   0        0        0      334 2022-03-25 08:44:41.000000 Orange3-WorldHappiness-0.1.9/README.pypi
+drwxrwxrwx   0        0        0        0 2022-11-23 08:48:43.822181 Orange3-WorldHappiness-0.1.9/doc/
+-rw-rw-rw-   0        0        0     6981 2022-03-25 08:44:41.000000 Orange3-WorldHappiness-0.1.9/doc/Makefile
+drwxrwxrwx   0        0        0        0 2022-11-23 08:48:43.784329 Orange3-WorldHappiness-0.1.9/doc/_build/
+drwxrwxrwx   0        0        0        0 2022-11-23 08:48:43.834992 Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/
+-rw-rw-rw-   0        0        0      234 2022-11-23 08:47:30.000000 Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/.buildinfo
+-rw-rw-rw-   0        0        0      684 2022-11-23 08:47:30.000000 Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/Orange3ImageAnalyticsdoc.hhc
+-rw-rw-rw-   0        0        0       13 2022-11-23 08:47:30.000000 Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/Orange3ImageAnalyticsdoc.hhk
+-rw-rw-rw-   0        0        0     1570 2022-11-23 08:47:30.000000 Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/Orange3ImageAnalyticsdoc.hhp
+-rw-rw-rw-   0        0        0      165 2022-11-23 08:45:32.000000 Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/Orange3ImageAnalyticsdoc.stp
+drwxrwxrwx   0        0        0        0 2022-11-23 08:48:43.838563 Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/_images/
+-rw-rw-rw-   0        0        0    94987 2022-03-25 08:44:41.000000 Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/_images/socioeconomic-indices.png
+drwxrwxrwx   0        0        0        0 2022-11-23 08:48:43.866936 Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/_static/
+-rw-rw-rw-   0        0        0     4418 2022-11-23 08:45:35.000000 Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/_static/_sphinx_javascript_frameworks_compat.js
+-rw-rw-rw-   0        0        0    15519 2022-11-23 08:47:30.000000 Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/_static/basic.css
+drwxrwxrwx   0        0        0        0 2022-11-23 08:48:43.870924 Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/_static/css/
+-rw-rw-rw-   0        0        0     3229 2022-11-23 08:47:23.000000 Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/_static/css/badge_only.css
+drwxrwxrwx   0        0        0        0 2022-11-23 08:48:43.903466 Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/_static/css/fonts/
+-rw-rw-rw-   0        0        0    87624 2022-11-23 08:47:23.000000 Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/_static/css/fonts/Roboto-Slab-Bold.woff
+-rw-rw-rw-   0        0        0    67312 2022-11-23 08:47:23.000000 Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/_static/css/fonts/Roboto-Slab-Bold.woff2
+-rw-rw-rw-   0        0        0    86288 2022-11-23 08:47:23.000000 Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/_static/css/fonts/Roboto-Slab-Regular.woff
+-rw-rw-rw-   0        0        0    66444 2022-11-23 08:47:23.000000 Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/_static/css/fonts/Roboto-Slab-Regular.woff2
+-rw-rw-rw-   0        0        0   165742 2022-11-23 08:47:23.000000 Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/_static/css/fonts/fontawesome-webfont.eot
+-rw-rw-rw-   0        0        0   444379 2022-11-23 08:47:23.000000 Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/_static/css/fonts/fontawesome-webfont.svg
+-rw-rw-rw-   0        0        0   165548 2022-11-23 08:47:23.000000 Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/_static/css/fonts/fontawesome-webfont.ttf
+-rw-rw-rw-   0        0        0    98024 2022-11-23 08:47:23.000000 Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/_static/css/fonts/fontawesome-webfont.woff
+-rw-rw-rw-   0        0        0    77160 2022-11-23 08:47:23.000000 Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/_static/css/fonts/fontawesome-webfont.woff2
+-rw-rw-rw-   0        0        0   323344 2022-11-23 08:47:23.000000 Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/_static/css/fonts/lato-bold-italic.woff
+-rw-rw-rw-   0        0        0   193308 2022-11-23 08:47:23.000000 Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/_static/css/fonts/lato-bold-italic.woff2
+-rw-rw-rw-   0        0        0   309728 2022-11-23 08:47:23.000000 Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/_static/css/fonts/lato-bold.woff
+-rw-rw-rw-   0        0        0   184912 2022-11-23 08:47:23.000000 Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/_static/css/fonts/lato-bold.woff2
+-rw-rw-rw-   0        0        0   328412 2022-11-23 08:47:23.000000 Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/_static/css/fonts/lato-normal-italic.woff
+-rw-rw-rw-   0        0        0   195704 2022-11-23 08:47:23.000000 Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/_static/css/fonts/lato-normal-italic.woff2
+-rw-rw-rw-   0        0        0   309192 2022-11-23 08:47:23.000000 Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/_static/css/fonts/lato-normal.woff
+-rw-rw-rw-   0        0        0   182708 2022-11-23 08:47:23.000000 Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/_static/css/fonts/lato-normal.woff2
+-rw-rw-rw-   0        0        0   131657 2022-11-23 08:47:23.000000 Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/_static/css/theme.css
+-rw-rw-rw-   0        0        0      549 2022-03-25 08:44:41.000000 Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/_static/custom.css
+-rw-rw-rw-   0        0        0     4472 2022-11-23 08:45:35.000000 Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/_static/doctools.js
+-rw-rw-rw-   0        0        0      432 2022-11-23 08:47:30.000000 Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/_static/documentation_options.js
+-rw-rw-rw-   0        0        0      286 2022-11-23 08:45:35.000000 Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/_static/file.png
+-rw-rw-rw-   0        0        0   288580 2022-11-23 08:45:35.000000 Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/_static/jquery-3.6.0.js
+-rw-rw-rw-   0        0        0    89501 2022-11-23 08:45:35.000000 Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/_static/jquery.js
+drwxrwxrwx   0        0        0        0 2022-11-23 08:48:43.910279 Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/_static/js/
+-rw-rw-rw-   0        0        0      934 2022-11-23 08:47:23.000000 Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/_static/js/badge_only.js
+-rw-rw-rw-   0        0        0     4370 2022-11-23 08:47:23.000000 Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/_static/js/html5shiv-printshiv.min.js
+-rw-rw-rw-   0        0        0     2734 2022-11-23 08:47:23.000000 Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/_static/js/html5shiv.min.js
+-rw-rw-rw-   0        0        0     5023 2022-11-23 08:47:23.000000 Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/_static/js/theme.js
+-rw-rw-rw-   0        0        0      339 2022-11-23 08:47:30.000000 Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/_static/language_data.js
+-rw-rw-rw-   0        0        0       90 2022-11-23 08:45:35.000000 Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/_static/minus.png
+-rw-rw-rw-   0        0        0       90 2022-11-23 08:45:35.000000 Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/_static/plus.png
+-rw-rw-rw-   0        0        0     4919 2022-11-23 08:47:30.000000 Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/_static/pygments.css
+-rw-rw-rw-   0        0        0    18215 2022-11-23 08:45:35.000000 Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/_static/searchtools.js
+-rw-rw-rw-   0        0        0     4712 2022-11-23 08:45:35.000000 Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/_static/sphinx_highlight.js
+-rw-rw-rw-   0        0        0    68420 2022-11-23 08:45:35.000000 Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/_static/underscore-1.13.1.js
+-rw-rw-rw-   0        0        0    19530 2022-11-23 08:45:35.000000 Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/_static/underscore.js
+-rw-rw-rw-   0        0        0     3023 2022-11-23 08:47:30.000000 Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/genindex.html
+-rw-rw-rw-   0        0        0     4336 2022-11-23 08:47:30.000000 Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/index.html
+drwxrwxrwx   0        0        0        0 2022-11-23 08:48:43.911280 Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/widgets/
+-rw-rw-rw-   0        0        0     5232 2022-11-23 08:47:30.000000 Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/widgets/socioeconomicindices.html
+-rw-rw-rw-   0        0        0     9246 2022-03-25 08:44:41.000000 Orange3-WorldHappiness-0.1.9/doc/conf.py
+-rw-rw-rw-   0        0        0      291 2022-03-25 08:44:41.000000 Orange3-WorldHappiness-0.1.9/doc/index.rst
+-rwxrwxrwx   0        0        0     6721 2022-03-25 08:44:41.000000 Orange3-WorldHappiness-0.1.9/doc/make.bat
+drwxrwxrwx   0        0        0        0 2022-11-23 08:48:43.912278 Orange3-WorldHappiness-0.1.9/doc/widgets/
+drwxrwxrwx   0        0        0        0 2022-11-23 08:48:43.914271 Orange3-WorldHappiness-0.1.9/doc/widgets/images/
+-rw-rw-rw-   0        0        0    94987 2022-03-25 08:44:41.000000 Orange3-WorldHappiness-0.1.9/doc/widgets/images/socioeconomic-indices.png
+-rw-rw-rw-   0        0        0     1248 2022-03-25 08:44:41.000000 Orange3-WorldHappiness-0.1.9/doc/widgets/socioeconomicindices.md
+-rw-rw-rw-   0        0        0      353 2022-03-25 08:44:41.000000 Orange3-WorldHappiness-0.1.9/doc/widgets.json
+drwxrwxrwx   0        0        0        0 2022-11-23 08:48:43.916647 Orange3-WorldHappiness-0.1.9/orangecontrib/
+-rw-rw-rw-   0        0        0      167 2022-03-25 08:44:41.000000 Orange3-WorldHappiness-0.1.9/orangecontrib/__init__.py
+drwxrwxrwx   0        0        0        0 2022-11-23 08:48:43.917675 Orange3-WorldHappiness-0.1.9/orangecontrib/worldhappiness/
+-rw-rw-rw-   0        0        0        0 2022-03-25 08:44:41.000000 Orange3-WorldHappiness-0.1.9/orangecontrib/worldhappiness/__init__.py
+drwxrwxrwx   0        0        0        0 2022-11-23 08:48:43.921070 Orange3-WorldHappiness-0.1.9/orangecontrib/worldhappiness/whstudy/
+-rw-rw-rw-   0        0        0     5656 2022-11-23 08:31:50.000000 Orange3-WorldHappiness-0.1.9/orangecontrib/worldhappiness/whstudy/__init__.py
+-rw-rw-rw-   0        0        0    18839 2022-11-23 08:31:50.000000 Orange3-WorldHappiness-0.1.9/orangecontrib/worldhappiness/whstudy/world_data_api.py
+drwxrwxrwx   0        0        0        0 2022-11-23 08:48:43.925061 Orange3-WorldHappiness-0.1.9/orangecontrib/worldhappiness/widgets/
+-rw-rw-rw-   0        0        0     1101 2022-03-25 08:44:41.000000 Orange3-WorldHappiness-0.1.9/orangecontrib/worldhappiness/widgets/__init__.py
+drwxrwxrwx   0        0        0        0 2022-11-23 08:48:43.929049 Orange3-WorldHappiness-0.1.9/orangecontrib/worldhappiness/widgets/icons/
+-rw-rw-rw-   0        0        0      631 2022-03-25 08:44:41.000000 Orange3-WorldHappiness-0.1.9/orangecontrib/worldhappiness/widgets/icons/category.svg
+-rw-rw-rw-   0        0        0      793 2022-03-25 08:44:41.000000 Orange3-WorldHappiness-0.1.9/orangecontrib/worldhappiness/widgets/icons/socioeconomicindices.svg
+-rw-rw-rw-   0        0        0    28741 2022-11-23 08:35:49.000000 Orange3-WorldHappiness-0.1.9/orangecontrib/worldhappiness/widgets/owwhstudy.py
+-rw-rw-rw-   0        0        0       42 2022-11-23 08:48:43.932042 Orange3-WorldHappiness-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     2834 2022-11-23 08:41:00.000000 Orange3-WorldHappiness-0.1.9/setup.py
```

### Comparing `Orange3-WorldHappiness-0.1.8/LICENSE.txt` & `Orange3-WorldHappiness-0.1.9/LICENSE.txt`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,674 +1,674 @@
-                    GNU GENERAL PUBLIC LICENSE
-                       Version 3, 29 June 2007
-
- Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
- Everyone is permitted to copy and distribute verbatim copies
- of this license document, but changing it is not allowed.
-
-                            Preamble
-
-  The GNU General Public License is a free, copyleft license for
-software and other kinds of works.
-
-  The licenses for most software and other practical works are designed
-to take away your freedom to share and change the works.  By contrast,
-the GNU General Public License is intended to guarantee your freedom to
-share and change all versions of a program--to make sure it remains free
-software for all its users.  We, the Free Software Foundation, use the
-GNU General Public License for most of our software; it applies also to
-any other work released this way by its authors.  You can apply it to
-your programs, too.
-
-  When we speak of free software, we are referring to freedom, not
-price.  Our General Public Licenses are designed to make sure that you
-have the freedom to distribute copies of free software (and charge for
-them if you wish), that you receive source code or can get it if you
-want it, that you can change the software or use pieces of it in new
-free programs, and that you know you can do these things.
-
-  To protect your rights, we need to prevent others from denying you
-these rights or asking you to surrender the rights.  Therefore, you have
-certain responsibilities if you distribute copies of the software, or if
-you modify it: responsibilities to respect the freedom of others.
-
-  For example, if you distribute copies of such a program, whether
-gratis or for a fee, you must pass on to the recipients the same
-freedoms that you received.  You must make sure that they, too, receive
-or can get the source code.  And you must show them these terms so they
-know their rights.
-
-  Developers that use the GNU GPL protect your rights with two steps:
-(1) assert copyright on the software, and (2) offer you this License
-giving you legal permission to copy, distribute and/or modify it.
-
-  For the developers' and authors' protection, the GPL clearly explains
-that there is no warranty for this free software.  For both users' and
-authors' sake, the GPL requires that modified versions be marked as
-changed, so that their problems will not be attributed erroneously to
-authors of previous versions.
-
-  Some devices are designed to deny users access to install or run
-modified versions of the software inside them, although the manufacturer
-can do so.  This is fundamentally incompatible with the aim of
-protecting users' freedom to change the software.  The systematic
-pattern of such abuse occurs in the area of products for individuals to
-use, which is precisely where it is most unacceptable.  Therefore, we
-have designed this version of the GPL to prohibit the practice for those
-products.  If such problems arise substantially in other domains, we
-stand ready to extend this provision to those domains in future versions
-of the GPL, as needed to protect the freedom of users.
-
-  Finally, every program is threatened constantly by software patents.
-States should not allow patents to restrict development and use of
-software on general-purpose computers, but in those that do, we wish to
-avoid the special danger that patents applied to a free program could
-make it effectively proprietary.  To prevent this, the GPL assures that
-patents cannot be used to render the program non-free.
-
-  The precise terms and conditions for copying, distribution and
-modification follow.
-
-                       TERMS AND CONDITIONS
-
-  0. Definitions.
-
-  "This License" refers to version 3 of the GNU General Public License.
-
-  "Copyright" also means copyright-like laws that apply to other kinds of
-works, such as semiconductor masks.
-
-  "The Program" refers to any copyrightable work licensed under this
-License.  Each licensee is addressed as "you".  "Licensees" and
-"recipients" may be individuals or organizations.
-
-  To "modify" a work means to copy from or adapt all or part of the work
-in a fashion requiring copyright permission, other than the making of an
-exact copy.  The resulting work is called a "modified version" of the
-earlier work or a work "based on" the earlier work.
-
-  A "covered work" means either the unmodified Program or a work based
-on the Program.
-
-  To "propagate" a work means to do anything with it that, without
-permission, would make you directly or secondarily liable for
-infringement under applicable copyright law, except executing it on a
-computer or modifying a private copy.  Propagation includes copying,
-distribution (with or without modification), making available to the
-public, and in some countries other activities as well.
-
-  To "convey" a work means any kind of propagation that enables other
-parties to make or receive copies.  Mere interaction with a user through
-a computer network, with no transfer of a copy, is not conveying.
-
-  An interactive user interface displays "Appropriate Legal Notices"
-to the extent that it includes a convenient and prominently visible
-feature that (1) displays an appropriate copyright notice, and (2)
-tells the user that there is no warranty for the work (except to the
-extent that warranties are provided), that licensees may convey the
-work under this License, and how to view a copy of this License.  If
-the interface presents a list of user commands or options, such as a
-menu, a prominent item in the list meets this criterion.
-
-  1. Source Code.
-
-  The "source code" for a work means the preferred form of the work
-for making modifications to it.  "Object code" means any non-source
-form of a work.
-
-  A "Standard Interface" means an interface that either is an official
-standard defined by a recognized standards body, or, in the case of
-interfaces specified for a particular programming language, one that
-is widely used among developers working in that language.
-
-  The "System Libraries" of an executable work include anything, other
-than the work as a whole, that (a) is included in the normal form of
-packaging a Major Component, but which is not part of that Major
-Component, and (b) serves only to enable use of the work with that
-Major Component, or to implement a Standard Interface for which an
-implementation is available to the public in source code form.  A
-"Major Component", in this context, means a major essential component
-(kernel, window system, and so on) of the specific operating system
-(if any) on which the executable work runs, or a compiler used to
-produce the work, or an object code interpreter used to run it.
-
-  The "Corresponding Source" for a work in object code form means all
-the source code needed to generate, install, and (for an executable
-work) run the object code and to modify the work, including scripts to
-control those activities.  However, it does not include the work's
-System Libraries, or general-purpose tools or generally available free
-programs which are used unmodified in performing those activities but
-which are not part of the work.  For example, Corresponding Source
-includes interface definition files associated with source files for
-the work, and the source code for shared libraries and dynamically
-linked subprograms that the work is specifically designed to require,
-such as by intimate data communication or control flow between those
-subprograms and other parts of the work.
-
-  The Corresponding Source need not include anything that users
-can regenerate automatically from other parts of the Corresponding
-Source.
-
-  The Corresponding Source for a work in source code form is that
-same work.
-
-  2. Basic Permissions.
-
-  All rights granted under this License are granted for the term of
-copyright on the Program, and are irrevocable provided the stated
-conditions are met.  This License explicitly affirms your unlimited
-permission to run the unmodified Program.  The output from running a
-covered work is covered by this License only if the output, given its
-content, constitutes a covered work.  This License acknowledges your
-rights of fair use or other equivalent, as provided by copyright law.
-
-  You may make, run and propagate covered works that you do not
-convey, without conditions so long as your license otherwise remains
-in force.  You may convey covered works to others for the sole purpose
-of having them make modifications exclusively for you, or provide you
-with facilities for running those works, provided that you comply with
-the terms of this License in conveying all material for which you do
-not control copyright.  Those thus making or running the covered works
-for you must do so exclusively on your behalf, under your direction
-and control, on terms that prohibit them from making any copies of
-your copyrighted material outside their relationship with you.
-
-  Conveying under any other circumstances is permitted solely under
-the conditions stated below.  Sublicensing is not allowed; section 10
-makes it unnecessary.
-
-  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-
-  No covered work shall be deemed part of an effective technological
-measure under any applicable law fulfilling obligations under article
-11 of the WIPO copyright treaty adopted on 20 December 1996, or
-similar laws prohibiting or restricting circumvention of such
-measures.
-
-  When you convey a covered work, you waive any legal power to forbid
-circumvention of technological measures to the extent such circumvention
-is effected by exercising rights under this License with respect to
-the covered work, and you disclaim any intention to limit operation or
-modification of the work as a means of enforcing, against the work's
-users, your or third parties' legal rights to forbid circumvention of
-technological measures.
-
-  4. Conveying Verbatim Copies.
-
-  You may convey verbatim copies of the Program's source code as you
-receive it, in any medium, provided that you conspicuously and
-appropriately publish on each copy an appropriate copyright notice;
-keep intact all notices stating that this License and any
-non-permissive terms added in accord with section 7 apply to the code;
-keep intact all notices of the absence of any warranty; and give all
-recipients a copy of this License along with the Program.
-
-  You may charge any price or no price for each copy that you convey,
-and you may offer support or warranty protection for a fee.
-
-  5. Conveying Modified Source Versions.
-
-  You may convey a work based on the Program, or the modifications to
-produce it from the Program, in the form of source code under the
-terms of section 4, provided that you also meet all of these conditions:
-
-    a) The work must carry prominent notices stating that you modified
-    it, and giving a relevant date.
-
-    b) The work must carry prominent notices stating that it is
-    released under this License and any conditions added under section
-    7.  This requirement modifies the requirement in section 4 to
-    "keep intact all notices".
-
-    c) You must license the entire work, as a whole, under this
-    License to anyone who comes into possession of a copy.  This
-    License will therefore apply, along with any applicable section 7
-    additional terms, to the whole of the work, and all its parts,
-    regardless of how they are packaged.  This License gives no
-    permission to license the work in any other way, but it does not
-    invalidate such permission if you have separately received it.
-
-    d) If the work has interactive user interfaces, each must display
-    Appropriate Legal Notices; however, if the Program has interactive
-    interfaces that do not display Appropriate Legal Notices, your
-    work need not make them do so.
-
-  A compilation of a covered work with other separate and independent
-works, which are not by their nature extensions of the covered work,
-and which are not combined with it such as to form a larger program,
-in or on a volume of a storage or distribution medium, is called an
-"aggregate" if the compilation and its resulting copyright are not
-used to limit the access or legal rights of the compilation's users
-beyond what the individual works permit.  Inclusion of a covered work
-in an aggregate does not cause this License to apply to the other
-parts of the aggregate.
-
-  6. Conveying Non-Source Forms.
-
-  You may convey a covered work in object code form under the terms
-of sections 4 and 5, provided that you also convey the
-machine-readable Corresponding Source under the terms of this License,
-in one of these ways:
-
-    a) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by the
-    Corresponding Source fixed on a durable physical medium
-    customarily used for software interchange.
-
-    b) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by a
-    written offer, valid for at least three years and valid for as
-    long as you offer spare parts or customer support for that product
-    model, to give anyone who possesses the object code either (1) a
-    copy of the Corresponding Source for all the software in the
-    product that is covered by this License, on a durable physical
-    medium customarily used for software interchange, for a price no
-    more than your reasonable cost of physically performing this
-    conveying of source, or (2) access to copy the
-    Corresponding Source from a network server at no charge.
-
-    c) Convey individual copies of the object code with a copy of the
-    written offer to provide the Corresponding Source.  This
-    alternative is allowed only occasionally and noncommercially, and
-    only if you received the object code with such an offer, in accord
-    with subsection 6b.
-
-    d) Convey the object code by offering access from a designated
-    place (gratis or for a charge), and offer equivalent access to the
-    Corresponding Source in the same way through the same place at no
-    further charge.  You need not require recipients to copy the
-    Corresponding Source along with the object code.  If the place to
-    copy the object code is a network server, the Corresponding Source
-    may be on a different server (operated by you or a third party)
-    that supports equivalent copying facilities, provided you maintain
-    clear directions next to the object code saying where to find the
-    Corresponding Source.  Regardless of what server hosts the
-    Corresponding Source, you remain obligated to ensure that it is
-    available for as long as needed to satisfy these requirements.
-
-    e) Convey the object code using peer-to-peer transmission, provided
-    you inform other peers where the object code and Corresponding
-    Source of the work are being offered to the general public at no
-    charge under subsection 6d.
-
-  A separable portion of the object code, whose source code is excluded
-from the Corresponding Source as a System Library, need not be
-included in conveying the object code work.
-
-  A "User Product" is either (1) a "consumer product", which means any
-tangible personal property which is normally used for personal, family,
-or household purposes, or (2) anything designed or sold for incorporation
-into a dwelling.  In determining whether a product is a consumer product,
-doubtful cases shall be resolved in favor of coverage.  For a particular
-product received by a particular user, "normally used" refers to a
-typical or common use of that class of product, regardless of the status
-of the particular user or of the way in which the particular user
-actually uses, or expects or is expected to use, the product.  A product
-is a consumer product regardless of whether the product has substantial
-commercial, industrial or non-consumer uses, unless such uses represent
-the only significant mode of use of the product.
-
-  "Installation Information" for a User Product means any methods,
-procedures, authorization keys, or other information required to install
-and execute modified versions of a covered work in that User Product from
-a modified version of its Corresponding Source.  The information must
-suffice to ensure that the continued functioning of the modified object
-code is in no case prevented or interfered with solely because
-modification has been made.
-
-  If you convey an object code work under this section in, or with, or
-specifically for use in, a User Product, and the conveying occurs as
-part of a transaction in which the right of possession and use of the
-User Product is transferred to the recipient in perpetuity or for a
-fixed term (regardless of how the transaction is characterized), the
-Corresponding Source conveyed under this section must be accompanied
-by the Installation Information.  But this requirement does not apply
-if neither you nor any third party retains the ability to install
-modified object code on the User Product (for example, the work has
-been installed in ROM).
-
-  The requirement to provide Installation Information does not include a
-requirement to continue to provide support service, warranty, or updates
-for a work that has been modified or installed by the recipient, or for
-the User Product in which it has been modified or installed.  Access to a
-network may be denied when the modification itself materially and
-adversely affects the operation of the network or violates the rules and
-protocols for communication across the network.
-
-  Corresponding Source conveyed, and Installation Information provided,
-in accord with this section must be in a format that is publicly
-documented (and with an implementation available to the public in
-source code form), and must require no special password or key for
-unpacking, reading or copying.
-
-  7. Additional Terms.
-
-  "Additional permissions" are terms that supplement the terms of this
-License by making exceptions from one or more of its conditions.
-Additional permissions that are applicable to the entire Program shall
-be treated as though they were included in this License, to the extent
-that they are valid under applicable law.  If additional permissions
-apply only to part of the Program, that part may be used separately
-under those permissions, but the entire Program remains governed by
-this License without regard to the additional permissions.
-
-  When you convey a copy of a covered work, you may at your option
-remove any additional permissions from that copy, or from any part of
-it.  (Additional permissions may be written to require their own
-removal in certain cases when you modify the work.)  You may place
-additional permissions on material, added by you to a covered work,
-for which you have or can give appropriate copyright permission.
-
-  Notwithstanding any other provision of this License, for material you
-add to a covered work, you may (if authorized by the copyright holders of
-that material) supplement the terms of this License with terms:
-
-    a) Disclaiming warranty or limiting liability differently from the
-    terms of sections 15 and 16 of this License; or
-
-    b) Requiring preservation of specified reasonable legal notices or
-    author attributions in that material or in the Appropriate Legal
-    Notices displayed by works containing it; or
-
-    c) Prohibiting misrepresentation of the origin of that material, or
-    requiring that modified versions of such material be marked in
-    reasonable ways as different from the original version; or
-
-    d) Limiting the use for publicity purposes of names of licensors or
-    authors of the material; or
-
-    e) Declining to grant rights under trademark law for use of some
-    trade names, trademarks, or service marks; or
-
-    f) Requiring indemnification of licensors and authors of that
-    material by anyone who conveys the material (or modified versions of
-    it) with contractual assumptions of liability to the recipient, for
-    any liability that these contractual assumptions directly impose on
-    those licensors and authors.
-
-  All other non-permissive additional terms are considered "further
-restrictions" within the meaning of section 10.  If the Program as you
-received it, or any part of it, contains a notice stating that it is
-governed by this License along with a term that is a further
-restriction, you may remove that term.  If a license document contains
-a further restriction but permits relicensing or conveying under this
-License, you may add to a covered work material governed by the terms
-of that license document, provided that the further restriction does
-not survive such relicensing or conveying.
-
-  If you add terms to a covered work in accord with this section, you
-must place, in the relevant source files, a statement of the
-additional terms that apply to those files, or a notice indicating
-where to find the applicable terms.
-
-  Additional terms, permissive or non-permissive, may be stated in the
-form of a separately written license, or stated as exceptions;
-the above requirements apply either way.
-
-  8. Termination.
-
-  You may not propagate or modify a covered work except as expressly
-provided under this License.  Any attempt otherwise to propagate or
-modify it is void, and will automatically terminate your rights under
-this License (including any patent licenses granted under the third
-paragraph of section 11).
-
-  However, if you cease all violation of this License, then your
-license from a particular copyright holder is reinstated (a)
-provisionally, unless and until the copyright holder explicitly and
-finally terminates your license, and (b) permanently, if the copyright
-holder fails to notify you of the violation by some reasonable means
-prior to 60 days after the cessation.
-
-  Moreover, your license from a particular copyright holder is
-reinstated permanently if the copyright holder notifies you of the
-violation by some reasonable means, this is the first time you have
-received notice of violation of this License (for any work) from that
-copyright holder, and you cure the violation prior to 30 days after
-your receipt of the notice.
-
-  Termination of your rights under this section does not terminate the
-licenses of parties who have received copies or rights from you under
-this License.  If your rights have been terminated and not permanently
-reinstated, you do not qualify to receive new licenses for the same
-material under section 10.
-
-  9. Acceptance Not Required for Having Copies.
-
-  You are not required to accept this License in order to receive or
-run a copy of the Program.  Ancillary propagation of a covered work
-occurring solely as a consequence of using peer-to-peer transmission
-to receive a copy likewise does not require acceptance.  However,
-nothing other than this License grants you permission to propagate or
-modify any covered work.  These actions infringe copyright if you do
-not accept this License.  Therefore, by modifying or propagating a
-covered work, you indicate your acceptance of this License to do so.
-
-  10. Automatic Licensing of Downstream Recipients.
-
-  Each time you convey a covered work, the recipient automatically
-receives a license from the original licensors, to run, modify and
-propagate that work, subject to this License.  You are not responsible
-for enforcing compliance by third parties with this License.
-
-  An "entity transaction" is a transaction transferring control of an
-organization, or substantially all assets of one, or subdividing an
-organization, or merging organizations.  If propagation of a covered
-work results from an entity transaction, each party to that
-transaction who receives a copy of the work also receives whatever
-licenses to the work the party's predecessor in interest had or could
-give under the previous paragraph, plus a right to possession of the
-Corresponding Source of the work from the predecessor in interest, if
-the predecessor has it or can get it with reasonable efforts.
-
-  You may not impose any further restrictions on the exercise of the
-rights granted or affirmed under this License.  For example, you may
-not impose a license fee, royalty, or other charge for exercise of
-rights granted under this License, and you may not initiate litigation
-(including a cross-claim or counterclaim in a lawsuit) alleging that
-any patent claim is infringed by making, using, selling, offering for
-sale, or importing the Program or any portion of it.
-
-  11. Patents.
-
-  A "contributor" is a copyright holder who authorizes use under this
-License of the Program or a work on which the Program is based.  The
-work thus licensed is called the contributor's "contributor version".
-
-  A contributor's "essential patent claims" are all patent claims
-owned or controlled by the contributor, whether already acquired or
-hereafter acquired, that would be infringed by some manner, permitted
-by this License, of making, using, or selling its contributor version,
-but do not include claims that would be infringed only as a
-consequence of further modification of the contributor version.  For
-purposes of this definition, "control" includes the right to grant
-patent sublicenses in a manner consistent with the requirements of
-this License.
-
-  Each contributor grants you a non-exclusive, worldwide, royalty-free
-patent license under the contributor's essential patent claims, to
-make, use, sell, offer for sale, import and otherwise run, modify and
-propagate the contents of its contributor version.
-
-  In the following three paragraphs, a "patent license" is any express
-agreement or commitment, however denominated, not to enforce a patent
-(such as an express permission to practice a patent or covenant not to
-sue for patent infringement).  To "grant" such a patent license to a
-party means to make such an agreement or commitment not to enforce a
-patent against the party.
-
-  If you convey a covered work, knowingly relying on a patent license,
-and the Corresponding Source of the work is not available for anyone
-to copy, free of charge and under the terms of this License, through a
-publicly available network server or other readily accessible means,
-then you must either (1) cause the Corresponding Source to be so
-available, or (2) arrange to deprive yourself of the benefit of the
-patent license for this particular work, or (3) arrange, in a manner
-consistent with the requirements of this License, to extend the patent
-license to downstream recipients.  "Knowingly relying" means you have
-actual knowledge that, but for the patent license, your conveying the
-covered work in a country, or your recipient's use of the covered work
-in a country, would infringe one or more identifiable patents in that
-country that you have reason to believe are valid.
-
-  If, pursuant to or in connection with a single transaction or
-arrangement, you convey, or propagate by procuring conveyance of, a
-covered work, and grant a patent license to some of the parties
-receiving the covered work authorizing them to use, propagate, modify
-or convey a specific copy of the covered work, then the patent license
-you grant is automatically extended to all recipients of the covered
-work and works based on it.
-
-  A patent license is "discriminatory" if it does not include within
-the scope of its coverage, prohibits the exercise of, or is
-conditioned on the non-exercise of one or more of the rights that are
-specifically granted under this License.  You may not convey a covered
-work if you are a party to an arrangement with a third party that is
-in the business of distributing software, under which you make payment
-to the third party based on the extent of your activity of conveying
-the work, and under which the third party grants, to any of the
-parties who would receive the covered work from you, a discriminatory
-patent license (a) in connection with copies of the covered work
-conveyed by you (or copies made from those copies), or (b) primarily
-for and in connection with specific products or compilations that
-contain the covered work, unless you entered into that arrangement,
-or that patent license was granted, prior to 28 March 2007.
-
-  Nothing in this License shall be construed as excluding or limiting
-any implied license or other defenses to infringement that may
-otherwise be available to you under applicable patent law.
-
-  12. No Surrender of Others' Freedom.
-
-  If conditions are imposed on you (whether by court order, agreement or
-otherwise) that contradict the conditions of this License, they do not
-excuse you from the conditions of this License.  If you cannot convey a
-covered work so as to satisfy simultaneously your obligations under this
-License and any other pertinent obligations, then as a consequence you may
-not convey it at all.  For example, if you agree to terms that obligate you
-to collect a royalty for further conveying from those to whom you convey
-the Program, the only way you could satisfy both those terms and this
-License would be to refrain entirely from conveying the Program.
-
-  13. Use with the GNU Affero General Public License.
-
-  Notwithstanding any other provision of this License, you have
-permission to link or combine any covered work with a work licensed
-under version 3 of the GNU Affero General Public License into a single
-combined work, and to convey the resulting work.  The terms of this
-License will continue to apply to the part which is the covered work,
-but the special requirements of the GNU Affero General Public License,
-section 13, concerning interaction through a network will apply to the
-combination as such.
-
-  14. Revised Versions of this License.
-
-  The Free Software Foundation may publish revised and/or new versions of
-the GNU General Public License from time to time.  Such new versions will
-be similar in spirit to the present version, but may differ in detail to
-address new problems or concerns.
-
-  Each version is given a distinguishing version number.  If the
-Program specifies that a certain numbered version of the GNU General
-Public License "or any later version" applies to it, you have the
-option of following the terms and conditions either of that numbered
-version or of any later version published by the Free Software
-Foundation.  If the Program does not specify a version number of the
-GNU General Public License, you may choose any version ever published
-by the Free Software Foundation.
-
-  If the Program specifies that a proxy can decide which future
-versions of the GNU General Public License can be used, that proxy's
-public statement of acceptance of a version permanently authorizes you
-to choose that version for the Program.
-
-  Later license versions may give you additional or different
-permissions.  However, no additional obligations are imposed on any
-author or copyright holder as a result of your choosing to follow a
-later version.
-
-  15. Disclaimer of Warranty.
-
-  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
-OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
-THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
-IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-
-  16. Limitation of Liability.
-
-  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
-THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
-USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
-DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
-PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
-EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
-SUCH DAMAGES.
-
-  17. Interpretation of Sections 15 and 16.
-
-  If the disclaimer of warranty and limitation of liability provided
-above cannot be given local legal effect according to their terms,
-reviewing courts shall apply local law that most closely approximates
-an absolute waiver of all civil liability in connection with the
-Program, unless a warranty or assumption of liability accompanies a
-copy of the Program in return for a fee.
-
-                     END OF TERMS AND CONDITIONS
-
-            How to Apply These Terms to Your New Programs
-
-  If you develop a new program, and you want it to be of the greatest
-possible use to the public, the best way to achieve this is to make it
-free software which everyone can redistribute and change under these terms.
-
-  To do so, attach the following notices to the program.  It is safest
-to attach them to the start of each source file to most effectively
-state the exclusion of warranty; and each file should have at least
-the "copyright" line and a pointer to where the full notice is found.
-
-    <one line to give the program's name and a brief idea of what it does.>
-    Copyright (C) <year>  <name of author>
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <http://www.gnu.org/licenses/>.
-
-Also add information on how to contact you by electronic and paper mail.
-
-  If the program does terminal interaction, make it output a short
-notice like this when it starts in an interactive mode:
-
-    <program>  Copyright (C) <year>  <name of author>
-    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
-    This is free software, and you are welcome to redistribute it
-    under certain conditions; type `show c' for details.
-
-The hypothetical commands `show w' and `show c' should show the appropriate
-parts of the General Public License.  Of course, your program's commands
-might be different; for a GUI interface, you would use an "about box".
-
-  You should also get your employer (if you work as a programmer) or school,
-if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU GPL, see
-<http://www.gnu.org/licenses/>.
-
-  The GNU General Public License does not permit incorporating your program
-into proprietary programs.  If your program is a subroutine library, you
-may consider it more useful to permit linking proprietary applications with
-the library.  If this is what you want to do, use the GNU Lesser General
-Public License instead of this License.  But first, please read
-<http://www.gnu.org/philosophy/why-not-lgpl.html>.
+                    GNU GENERAL PUBLIC LICENSE
+                       Version 3, 29 June 2007
+
+ Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
+ Everyone is permitted to copy and distribute verbatim copies
+ of this license document, but changing it is not allowed.
+
+                            Preamble
+
+  The GNU General Public License is a free, copyleft license for
+software and other kinds of works.
+
+  The licenses for most software and other practical works are designed
+to take away your freedom to share and change the works.  By contrast,
+the GNU General Public License is intended to guarantee your freedom to
+share and change all versions of a program--to make sure it remains free
+software for all its users.  We, the Free Software Foundation, use the
+GNU General Public License for most of our software; it applies also to
+any other work released this way by its authors.  You can apply it to
+your programs, too.
+
+  When we speak of free software, we are referring to freedom, not
+price.  Our General Public Licenses are designed to make sure that you
+have the freedom to distribute copies of free software (and charge for
+them if you wish), that you receive source code or can get it if you
+want it, that you can change the software or use pieces of it in new
+free programs, and that you know you can do these things.
+
+  To protect your rights, we need to prevent others from denying you
+these rights or asking you to surrender the rights.  Therefore, you have
+certain responsibilities if you distribute copies of the software, or if
+you modify it: responsibilities to respect the freedom of others.
+
+  For example, if you distribute copies of such a program, whether
+gratis or for a fee, you must pass on to the recipients the same
+freedoms that you received.  You must make sure that they, too, receive
+or can get the source code.  And you must show them these terms so they
+know their rights.
+
+  Developers that use the GNU GPL protect your rights with two steps:
+(1) assert copyright on the software, and (2) offer you this License
+giving you legal permission to copy, distribute and/or modify it.
+
+  For the developers' and authors' protection, the GPL clearly explains
+that there is no warranty for this free software.  For both users' and
+authors' sake, the GPL requires that modified versions be marked as
+changed, so that their problems will not be attributed erroneously to
+authors of previous versions.
+
+  Some devices are designed to deny users access to install or run
+modified versions of the software inside them, although the manufacturer
+can do so.  This is fundamentally incompatible with the aim of
+protecting users' freedom to change the software.  The systematic
+pattern of such abuse occurs in the area of products for individuals to
+use, which is precisely where it is most unacceptable.  Therefore, we
+have designed this version of the GPL to prohibit the practice for those
+products.  If such problems arise substantially in other domains, we
+stand ready to extend this provision to those domains in future versions
+of the GPL, as needed to protect the freedom of users.
+
+  Finally, every program is threatened constantly by software patents.
+States should not allow patents to restrict development and use of
+software on general-purpose computers, but in those that do, we wish to
+avoid the special danger that patents applied to a free program could
+make it effectively proprietary.  To prevent this, the GPL assures that
+patents cannot be used to render the program non-free.
+
+  The precise terms and conditions for copying, distribution and
+modification follow.
+
+                       TERMS AND CONDITIONS
+
+  0. Definitions.
+
+  "This License" refers to version 3 of the GNU General Public License.
+
+  "Copyright" also means copyright-like laws that apply to other kinds of
+works, such as semiconductor masks.
+
+  "The Program" refers to any copyrightable work licensed under this
+License.  Each licensee is addressed as "you".  "Licensees" and
+"recipients" may be individuals or organizations.
+
+  To "modify" a work means to copy from or adapt all or part of the work
+in a fashion requiring copyright permission, other than the making of an
+exact copy.  The resulting work is called a "modified version" of the
+earlier work or a work "based on" the earlier work.
+
+  A "covered work" means either the unmodified Program or a work based
+on the Program.
+
+  To "propagate" a work means to do anything with it that, without
+permission, would make you directly or secondarily liable for
+infringement under applicable copyright law, except executing it on a
+computer or modifying a private copy.  Propagation includes copying,
+distribution (with or without modification), making available to the
+public, and in some countries other activities as well.
+
+  To "convey" a work means any kind of propagation that enables other
+parties to make or receive copies.  Mere interaction with a user through
+a computer network, with no transfer of a copy, is not conveying.
+
+  An interactive user interface displays "Appropriate Legal Notices"
+to the extent that it includes a convenient and prominently visible
+feature that (1) displays an appropriate copyright notice, and (2)
+tells the user that there is no warranty for the work (except to the
+extent that warranties are provided), that licensees may convey the
+work under this License, and how to view a copy of this License.  If
+the interface presents a list of user commands or options, such as a
+menu, a prominent item in the list meets this criterion.
+
+  1. Source Code.
+
+  The "source code" for a work means the preferred form of the work
+for making modifications to it.  "Object code" means any non-source
+form of a work.
+
+  A "Standard Interface" means an interface that either is an official
+standard defined by a recognized standards body, or, in the case of
+interfaces specified for a particular programming language, one that
+is widely used among developers working in that language.
+
+  The "System Libraries" of an executable work include anything, other
+than the work as a whole, that (a) is included in the normal form of
+packaging a Major Component, but which is not part of that Major
+Component, and (b) serves only to enable use of the work with that
+Major Component, or to implement a Standard Interface for which an
+implementation is available to the public in source code form.  A
+"Major Component", in this context, means a major essential component
+(kernel, window system, and so on) of the specific operating system
+(if any) on which the executable work runs, or a compiler used to
+produce the work, or an object code interpreter used to run it.
+
+  The "Corresponding Source" for a work in object code form means all
+the source code needed to generate, install, and (for an executable
+work) run the object code and to modify the work, including scripts to
+control those activities.  However, it does not include the work's
+System Libraries, or general-purpose tools or generally available free
+programs which are used unmodified in performing those activities but
+which are not part of the work.  For example, Corresponding Source
+includes interface definition files associated with source files for
+the work, and the source code for shared libraries and dynamically
+linked subprograms that the work is specifically designed to require,
+such as by intimate data communication or control flow between those
+subprograms and other parts of the work.
+
+  The Corresponding Source need not include anything that users
+can regenerate automatically from other parts of the Corresponding
+Source.
+
+  The Corresponding Source for a work in source code form is that
+same work.
+
+  2. Basic Permissions.
+
+  All rights granted under this License are granted for the term of
+copyright on the Program, and are irrevocable provided the stated
+conditions are met.  This License explicitly affirms your unlimited
+permission to run the unmodified Program.  The output from running a
+covered work is covered by this License only if the output, given its
+content, constitutes a covered work.  This License acknowledges your
+rights of fair use or other equivalent, as provided by copyright law.
+
+  You may make, run and propagate covered works that you do not
+convey, without conditions so long as your license otherwise remains
+in force.  You may convey covered works to others for the sole purpose
+of having them make modifications exclusively for you, or provide you
+with facilities for running those works, provided that you comply with
+the terms of this License in conveying all material for which you do
+not control copyright.  Those thus making or running the covered works
+for you must do so exclusively on your behalf, under your direction
+and control, on terms that prohibit them from making any copies of
+your copyrighted material outside their relationship with you.
+
+  Conveying under any other circumstances is permitted solely under
+the conditions stated below.  Sublicensing is not allowed; section 10
+makes it unnecessary.
+
+  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+
+  No covered work shall be deemed part of an effective technological
+measure under any applicable law fulfilling obligations under article
+11 of the WIPO copyright treaty adopted on 20 December 1996, or
+similar laws prohibiting or restricting circumvention of such
+measures.
+
+  When you convey a covered work, you waive any legal power to forbid
+circumvention of technological measures to the extent such circumvention
+is effected by exercising rights under this License with respect to
+the covered work, and you disclaim any intention to limit operation or
+modification of the work as a means of enforcing, against the work's
+users, your or third parties' legal rights to forbid circumvention of
+technological measures.
+
+  4. Conveying Verbatim Copies.
+
+  You may convey verbatim copies of the Program's source code as you
+receive it, in any medium, provided that you conspicuously and
+appropriately publish on each copy an appropriate copyright notice;
+keep intact all notices stating that this License and any
+non-permissive terms added in accord with section 7 apply to the code;
+keep intact all notices of the absence of any warranty; and give all
+recipients a copy of this License along with the Program.
+
+  You may charge any price or no price for each copy that you convey,
+and you may offer support or warranty protection for a fee.
+
+  5. Conveying Modified Source Versions.
+
+  You may convey a work based on the Program, or the modifications to
+produce it from the Program, in the form of source code under the
+terms of section 4, provided that you also meet all of these conditions:
+
+    a) The work must carry prominent notices stating that you modified
+    it, and giving a relevant date.
+
+    b) The work must carry prominent notices stating that it is
+    released under this License and any conditions added under section
+    7.  This requirement modifies the requirement in section 4 to
+    "keep intact all notices".
+
+    c) You must license the entire work, as a whole, under this
+    License to anyone who comes into possession of a copy.  This
+    License will therefore apply, along with any applicable section 7
+    additional terms, to the whole of the work, and all its parts,
+    regardless of how they are packaged.  This License gives no
+    permission to license the work in any other way, but it does not
+    invalidate such permission if you have separately received it.
+
+    d) If the work has interactive user interfaces, each must display
+    Appropriate Legal Notices; however, if the Program has interactive
+    interfaces that do not display Appropriate Legal Notices, your
+    work need not make them do so.
+
+  A compilation of a covered work with other separate and independent
+works, which are not by their nature extensions of the covered work,
+and which are not combined with it such as to form a larger program,
+in or on a volume of a storage or distribution medium, is called an
+"aggregate" if the compilation and its resulting copyright are not
+used to limit the access or legal rights of the compilation's users
+beyond what the individual works permit.  Inclusion of a covered work
+in an aggregate does not cause this License to apply to the other
+parts of the aggregate.
+
+  6. Conveying Non-Source Forms.
+
+  You may convey a covered work in object code form under the terms
+of sections 4 and 5, provided that you also convey the
+machine-readable Corresponding Source under the terms of this License,
+in one of these ways:
+
+    a) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by the
+    Corresponding Source fixed on a durable physical medium
+    customarily used for software interchange.
+
+    b) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by a
+    written offer, valid for at least three years and valid for as
+    long as you offer spare parts or customer support for that product
+    model, to give anyone who possesses the object code either (1) a
+    copy of the Corresponding Source for all the software in the
+    product that is covered by this License, on a durable physical
+    medium customarily used for software interchange, for a price no
+    more than your reasonable cost of physically performing this
+    conveying of source, or (2) access to copy the
+    Corresponding Source from a network server at no charge.
+
+    c) Convey individual copies of the object code with a copy of the
+    written offer to provide the Corresponding Source.  This
+    alternative is allowed only occasionally and noncommercially, and
+    only if you received the object code with such an offer, in accord
+    with subsection 6b.
+
+    d) Convey the object code by offering access from a designated
+    place (gratis or for a charge), and offer equivalent access to the
+    Corresponding Source in the same way through the same place at no
+    further charge.  You need not require recipients to copy the
+    Corresponding Source along with the object code.  If the place to
+    copy the object code is a network server, the Corresponding Source
+    may be on a different server (operated by you or a third party)
+    that supports equivalent copying facilities, provided you maintain
+    clear directions next to the object code saying where to find the
+    Corresponding Source.  Regardless of what server hosts the
+    Corresponding Source, you remain obligated to ensure that it is
+    available for as long as needed to satisfy these requirements.
+
+    e) Convey the object code using peer-to-peer transmission, provided
+    you inform other peers where the object code and Corresponding
+    Source of the work are being offered to the general public at no
+    charge under subsection 6d.
+
+  A separable portion of the object code, whose source code is excluded
+from the Corresponding Source as a System Library, need not be
+included in conveying the object code work.
+
+  A "User Product" is either (1) a "consumer product", which means any
+tangible personal property which is normally used for personal, family,
+or household purposes, or (2) anything designed or sold for incorporation
+into a dwelling.  In determining whether a product is a consumer product,
+doubtful cases shall be resolved in favor of coverage.  For a particular
+product received by a particular user, "normally used" refers to a
+typical or common use of that class of product, regardless of the status
+of the particular user or of the way in which the particular user
+actually uses, or expects or is expected to use, the product.  A product
+is a consumer product regardless of whether the product has substantial
+commercial, industrial or non-consumer uses, unless such uses represent
+the only significant mode of use of the product.
+
+  "Installation Information" for a User Product means any methods,
+procedures, authorization keys, or other information required to install
+and execute modified versions of a covered work in that User Product from
+a modified version of its Corresponding Source.  The information must
+suffice to ensure that the continued functioning of the modified object
+code is in no case prevented or interfered with solely because
+modification has been made.
+
+  If you convey an object code work under this section in, or with, or
+specifically for use in, a User Product, and the conveying occurs as
+part of a transaction in which the right of possession and use of the
+User Product is transferred to the recipient in perpetuity or for a
+fixed term (regardless of how the transaction is characterized), the
+Corresponding Source conveyed under this section must be accompanied
+by the Installation Information.  But this requirement does not apply
+if neither you nor any third party retains the ability to install
+modified object code on the User Product (for example, the work has
+been installed in ROM).
+
+  The requirement to provide Installation Information does not include a
+requirement to continue to provide support service, warranty, or updates
+for a work that has been modified or installed by the recipient, or for
+the User Product in which it has been modified or installed.  Access to a
+network may be denied when the modification itself materially and
+adversely affects the operation of the network or violates the rules and
+protocols for communication across the network.
+
+  Corresponding Source conveyed, and Installation Information provided,
+in accord with this section must be in a format that is publicly
+documented (and with an implementation available to the public in
+source code form), and must require no special password or key for
+unpacking, reading or copying.
+
+  7. Additional Terms.
+
+  "Additional permissions" are terms that supplement the terms of this
+License by making exceptions from one or more of its conditions.
+Additional permissions that are applicable to the entire Program shall
+be treated as though they were included in this License, to the extent
+that they are valid under applicable law.  If additional permissions
+apply only to part of the Program, that part may be used separately
+under those permissions, but the entire Program remains governed by
+this License without regard to the additional permissions.
+
+  When you convey a copy of a covered work, you may at your option
+remove any additional permissions from that copy, or from any part of
+it.  (Additional permissions may be written to require their own
+removal in certain cases when you modify the work.)  You may place
+additional permissions on material, added by you to a covered work,
+for which you have or can give appropriate copyright permission.
+
+  Notwithstanding any other provision of this License, for material you
+add to a covered work, you may (if authorized by the copyright holders of
+that material) supplement the terms of this License with terms:
+
+    a) Disclaiming warranty or limiting liability differently from the
+    terms of sections 15 and 16 of this License; or
+
+    b) Requiring preservation of specified reasonable legal notices or
+    author attributions in that material or in the Appropriate Legal
+    Notices displayed by works containing it; or
+
+    c) Prohibiting misrepresentation of the origin of that material, or
+    requiring that modified versions of such material be marked in
+    reasonable ways as different from the original version; or
+
+    d) Limiting the use for publicity purposes of names of licensors or
+    authors of the material; or
+
+    e) Declining to grant rights under trademark law for use of some
+    trade names, trademarks, or service marks; or
+
+    f) Requiring indemnification of licensors and authors of that
+    material by anyone who conveys the material (or modified versions of
+    it) with contractual assumptions of liability to the recipient, for
+    any liability that these contractual assumptions directly impose on
+    those licensors and authors.
+
+  All other non-permissive additional terms are considered "further
+restrictions" within the meaning of section 10.  If the Program as you
+received it, or any part of it, contains a notice stating that it is
+governed by this License along with a term that is a further
+restriction, you may remove that term.  If a license document contains
+a further restriction but permits relicensing or conveying under this
+License, you may add to a covered work material governed by the terms
+of that license document, provided that the further restriction does
+not survive such relicensing or conveying.
+
+  If you add terms to a covered work in accord with this section, you
+must place, in the relevant source files, a statement of the
+additional terms that apply to those files, or a notice indicating
+where to find the applicable terms.
+
+  Additional terms, permissive or non-permissive, may be stated in the
+form of a separately written license, or stated as exceptions;
+the above requirements apply either way.
+
+  8. Termination.
+
+  You may not propagate or modify a covered work except as expressly
+provided under this License.  Any attempt otherwise to propagate or
+modify it is void, and will automatically terminate your rights under
+this License (including any patent licenses granted under the third
+paragraph of section 11).
+
+  However, if you cease all violation of this License, then your
+license from a particular copyright holder is reinstated (a)
+provisionally, unless and until the copyright holder explicitly and
+finally terminates your license, and (b) permanently, if the copyright
+holder fails to notify you of the violation by some reasonable means
+prior to 60 days after the cessation.
+
+  Moreover, your license from a particular copyright holder is
+reinstated permanently if the copyright holder notifies you of the
+violation by some reasonable means, this is the first time you have
+received notice of violation of this License (for any work) from that
+copyright holder, and you cure the violation prior to 30 days after
+your receipt of the notice.
+
+  Termination of your rights under this section does not terminate the
+licenses of parties who have received copies or rights from you under
+this License.  If your rights have been terminated and not permanently
+reinstated, you do not qualify to receive new licenses for the same
+material under section 10.
+
+  9. Acceptance Not Required for Having Copies.
+
+  You are not required to accept this License in order to receive or
+run a copy of the Program.  Ancillary propagation of a covered work
+occurring solely as a consequence of using peer-to-peer transmission
+to receive a copy likewise does not require acceptance.  However,
+nothing other than this License grants you permission to propagate or
+modify any covered work.  These actions infringe copyright if you do
+not accept this License.  Therefore, by modifying or propagating a
+covered work, you indicate your acceptance of this License to do so.
+
+  10. Automatic Licensing of Downstream Recipients.
+
+  Each time you convey a covered work, the recipient automatically
+receives a license from the original licensors, to run, modify and
+propagate that work, subject to this License.  You are not responsible
+for enforcing compliance by third parties with this License.
+
+  An "entity transaction" is a transaction transferring control of an
+organization, or substantially all assets of one, or subdividing an
+organization, or merging organizations.  If propagation of a covered
+work results from an entity transaction, each party to that
+transaction who receives a copy of the work also receives whatever
+licenses to the work the party's predecessor in interest had or could
+give under the previous paragraph, plus a right to possession of the
+Corresponding Source of the work from the predecessor in interest, if
+the predecessor has it or can get it with reasonable efforts.
+
+  You may not impose any further restrictions on the exercise of the
+rights granted or affirmed under this License.  For example, you may
+not impose a license fee, royalty, or other charge for exercise of
+rights granted under this License, and you may not initiate litigation
+(including a cross-claim or counterclaim in a lawsuit) alleging that
+any patent claim is infringed by making, using, selling, offering for
+sale, or importing the Program or any portion of it.
+
+  11. Patents.
+
+  A "contributor" is a copyright holder who authorizes use under this
+License of the Program or a work on which the Program is based.  The
+work thus licensed is called the contributor's "contributor version".
+
+  A contributor's "essential patent claims" are all patent claims
+owned or controlled by the contributor, whether already acquired or
+hereafter acquired, that would be infringed by some manner, permitted
+by this License, of making, using, or selling its contributor version,
+but do not include claims that would be infringed only as a
+consequence of further modification of the contributor version.  For
+purposes of this definition, "control" includes the right to grant
+patent sublicenses in a manner consistent with the requirements of
+this License.
+
+  Each contributor grants you a non-exclusive, worldwide, royalty-free
+patent license under the contributor's essential patent claims, to
+make, use, sell, offer for sale, import and otherwise run, modify and
+propagate the contents of its contributor version.
+
+  In the following three paragraphs, a "patent license" is any express
+agreement or commitment, however denominated, not to enforce a patent
+(such as an express permission to practice a patent or covenant not to
+sue for patent infringement).  To "grant" such a patent license to a
+party means to make such an agreement or commitment not to enforce a
+patent against the party.
+
+  If you convey a covered work, knowingly relying on a patent license,
+and the Corresponding Source of the work is not available for anyone
+to copy, free of charge and under the terms of this License, through a
+publicly available network server or other readily accessible means,
+then you must either (1) cause the Corresponding Source to be so
+available, or (2) arrange to deprive yourself of the benefit of the
+patent license for this particular work, or (3) arrange, in a manner
+consistent with the requirements of this License, to extend the patent
+license to downstream recipients.  "Knowingly relying" means you have
+actual knowledge that, but for the patent license, your conveying the
+covered work in a country, or your recipient's use of the covered work
+in a country, would infringe one or more identifiable patents in that
+country that you have reason to believe are valid.
+
+  If, pursuant to or in connection with a single transaction or
+arrangement, you convey, or propagate by procuring conveyance of, a
+covered work, and grant a patent license to some of the parties
+receiving the covered work authorizing them to use, propagate, modify
+or convey a specific copy of the covered work, then the patent license
+you grant is automatically extended to all recipients of the covered
+work and works based on it.
+
+  A patent license is "discriminatory" if it does not include within
+the scope of its coverage, prohibits the exercise of, or is
+conditioned on the non-exercise of one or more of the rights that are
+specifically granted under this License.  You may not convey a covered
+work if you are a party to an arrangement with a third party that is
+in the business of distributing software, under which you make payment
+to the third party based on the extent of your activity of conveying
+the work, and under which the third party grants, to any of the
+parties who would receive the covered work from you, a discriminatory
+patent license (a) in connection with copies of the covered work
+conveyed by you (or copies made from those copies), or (b) primarily
+for and in connection with specific products or compilations that
+contain the covered work, unless you entered into that arrangement,
+or that patent license was granted, prior to 28 March 2007.
+
+  Nothing in this License shall be construed as excluding or limiting
+any implied license or other defenses to infringement that may
+otherwise be available to you under applicable patent law.
+
+  12. No Surrender of Others' Freedom.
+
+  If conditions are imposed on you (whether by court order, agreement or
+otherwise) that contradict the conditions of this License, they do not
+excuse you from the conditions of this License.  If you cannot convey a
+covered work so as to satisfy simultaneously your obligations under this
+License and any other pertinent obligations, then as a consequence you may
+not convey it at all.  For example, if you agree to terms that obligate you
+to collect a royalty for further conveying from those to whom you convey
+the Program, the only way you could satisfy both those terms and this
+License would be to refrain entirely from conveying the Program.
+
+  13. Use with the GNU Affero General Public License.
+
+  Notwithstanding any other provision of this License, you have
+permission to link or combine any covered work with a work licensed
+under version 3 of the GNU Affero General Public License into a single
+combined work, and to convey the resulting work.  The terms of this
+License will continue to apply to the part which is the covered work,
+but the special requirements of the GNU Affero General Public License,
+section 13, concerning interaction through a network will apply to the
+combination as such.
+
+  14. Revised Versions of this License.
+
+  The Free Software Foundation may publish revised and/or new versions of
+the GNU General Public License from time to time.  Such new versions will
+be similar in spirit to the present version, but may differ in detail to
+address new problems or concerns.
+
+  Each version is given a distinguishing version number.  If the
+Program specifies that a certain numbered version of the GNU General
+Public License "or any later version" applies to it, you have the
+option of following the terms and conditions either of that numbered
+version or of any later version published by the Free Software
+Foundation.  If the Program does not specify a version number of the
+GNU General Public License, you may choose any version ever published
+by the Free Software Foundation.
+
+  If the Program specifies that a proxy can decide which future
+versions of the GNU General Public License can be used, that proxy's
+public statement of acceptance of a version permanently authorizes you
+to choose that version for the Program.
+
+  Later license versions may give you additional or different
+permissions.  However, no additional obligations are imposed on any
+author or copyright holder as a result of your choosing to follow a
+later version.
+
+  15. Disclaimer of Warranty.
+
+  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
+APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
+HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
+OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
+THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
+IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
+ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+
+  16. Limitation of Liability.
+
+  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
+THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
+GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
+USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
+DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
+PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
+EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
+SUCH DAMAGES.
+
+  17. Interpretation of Sections 15 and 16.
+
+  If the disclaimer of warranty and limitation of liability provided
+above cannot be given local legal effect according to their terms,
+reviewing courts shall apply local law that most closely approximates
+an absolute waiver of all civil liability in connection with the
+Program, unless a warranty or assumption of liability accompanies a
+copy of the Program in return for a fee.
+
+                     END OF TERMS AND CONDITIONS
+
+            How to Apply These Terms to Your New Programs
+
+  If you develop a new program, and you want it to be of the greatest
+possible use to the public, the best way to achieve this is to make it
+free software which everyone can redistribute and change under these terms.
+
+  To do so, attach the following notices to the program.  It is safest
+to attach them to the start of each source file to most effectively
+state the exclusion of warranty; and each file should have at least
+the "copyright" line and a pointer to where the full notice is found.
+
+    <one line to give the program's name and a brief idea of what it does.>
+    Copyright (C) <year>  <name of author>
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
+Also add information on how to contact you by electronic and paper mail.
+
+  If the program does terminal interaction, make it output a short
+notice like this when it starts in an interactive mode:
+
+    <program>  Copyright (C) <year>  <name of author>
+    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
+    This is free software, and you are welcome to redistribute it
+    under certain conditions; type `show c' for details.
+
+The hypothetical commands `show w' and `show c' should show the appropriate
+parts of the General Public License.  Of course, your program's commands
+might be different; for a GUI interface, you would use an "about box".
+
+  You should also get your employer (if you work as a programmer) or school,
+if any, to sign a "copyright disclaimer" for the program, if necessary.
+For more information on this, and how to apply and follow the GNU GPL, see
+<http://www.gnu.org/licenses/>.
+
+  The GNU General Public License does not permit incorporating your program
+into proprietary programs.  If your program is a subroutine library, you
+may consider it more useful to permit linking proprietary applications with
+the library.  If this is what you want to do, use the GNU Lesser General
+Public License instead of this License.  But first, please read
+<http://www.gnu.org/philosophy/why-not-lgpl.html>.
```

### Comparing `Orange3-WorldHappiness-0.1.8/Orange3_WorldHappiness.egg-info/PKG-INFO` & `Orange3-WorldHappiness-0.1.9/Orange3_WorldHappiness.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: Orange3-WorldHappiness
-Version: 0.1.8
+Version: 0.1.9
 Summary: Orange3 add-on for retrieving socioeconomic data
 Home-page: http://orange.biolab.si/download
 Author: Bioinformatics Laboratory, FRI UL
 Author-email: contact@orange.biolab.si
 License: GPL3+
+Description: Orange3 World Happiness
+        =======================
+        
+        Enables downloading of socioeconomic data in Orange3 from
+        a remote mongo database filled with indicators from various
+        economic databases.
+        
+        Features
+        --------
+        #### World Happiness data
+        * download and use socioeconomic data
+        * filter based on region, year, country, organization
 Keywords: orange3 add-on,orange3-world-happiness
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-Orange3 World Happiness
-=======================
-
-Enables downloading of socioeconomic data in Orange3 from
-a remote mongo database filled with indicators from various
-economic databases.
-
-Features
---------
-#### World Happiness data
-* download and use socioeconomic data
-* filter based on region, year, country, organization
```

### Comparing `Orange3-WorldHappiness-0.1.8/Orange3_WorldHappiness.egg-info/SOURCES.txt` & `Orange3-WorldHappiness-0.1.9/Orange3_WorldHappiness.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -20,26 +20,28 @@
 doc/_build/htmlhelp/Orange3ImageAnalyticsdoc.hhc
 doc/_build/htmlhelp/Orange3ImageAnalyticsdoc.hhk
 doc/_build/htmlhelp/Orange3ImageAnalyticsdoc.hhp
 doc/_build/htmlhelp/Orange3ImageAnalyticsdoc.stp
 doc/_build/htmlhelp/genindex.html
 doc/_build/htmlhelp/index.html
 doc/_build/htmlhelp/_images/socioeconomic-indices.png
+doc/_build/htmlhelp/_static/_sphinx_javascript_frameworks_compat.js
 doc/_build/htmlhelp/_static/basic.css
 doc/_build/htmlhelp/_static/custom.css
 doc/_build/htmlhelp/_static/doctools.js
 doc/_build/htmlhelp/_static/documentation_options.js
 doc/_build/htmlhelp/_static/file.png
-doc/_build/htmlhelp/_static/jquery-3.5.1.js
+doc/_build/htmlhelp/_static/jquery-3.6.0.js
 doc/_build/htmlhelp/_static/jquery.js
 doc/_build/htmlhelp/_static/language_data.js
 doc/_build/htmlhelp/_static/minus.png
 doc/_build/htmlhelp/_static/plus.png
 doc/_build/htmlhelp/_static/pygments.css
 doc/_build/htmlhelp/_static/searchtools.js
+doc/_build/htmlhelp/_static/sphinx_highlight.js
 doc/_build/htmlhelp/_static/underscore-1.13.1.js
 doc/_build/htmlhelp/_static/underscore.js
 doc/_build/htmlhelp/_static/css/badge_only.css
 doc/_build/htmlhelp/_static/css/theme.css
 doc/_build/htmlhelp/_static/css/fonts/Roboto-Slab-Bold.woff
 doc/_build/htmlhelp/_static/css/fonts/Roboto-Slab-Bold.woff2
 doc/_build/htmlhelp/_static/css/fonts/Roboto-Slab-Regular.woff
```

### Comparing `Orange3-WorldHappiness-0.1.8/PKG-INFO` & `Orange3-WorldHappiness-0.1.9/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: Orange3-WorldHappiness
-Version: 0.1.8
+Version: 0.1.9
 Summary: Orange3 add-on for retrieving socioeconomic data
 Home-page: http://orange.biolab.si/download
 Author: Bioinformatics Laboratory, FRI UL
 Author-email: contact@orange.biolab.si
 License: GPL3+
+Description: Orange3 World Happiness
+        =======================
+        
+        Enables downloading of socioeconomic data in Orange3 from
+        a remote mongo database filled with indicators from various
+        economic databases.
+        
+        Features
+        --------
+        #### World Happiness data
+        * download and use socioeconomic data
+        * filter based on region, year, country, organization
 Keywords: orange3 add-on,orange3-world-happiness
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-Orange3 World Happiness
-=======================
-
-Enables downloading of socioeconomic data in Orange3 from
-a remote mongo database filled with indicators from various
-economic databases.
-
-Features
---------
-#### World Happiness data
-* download and use socioeconomic data
-* filter based on region, year, country, organization
```

### Comparing `Orange3-WorldHappiness-0.1.8/README.md` & `Orange3-WorldHappiness-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `Orange3-WorldHappiness-0.1.8/doc/Makefile` & `Orange3-WorldHappiness-0.1.9/doc/Makefile`

 * *Files identical despite different names*

### Comparing `Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/Orange3ImageAnalyticsdoc.hhc` & `Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/Orange3ImageAnalyticsdoc.hhc`

 * *Files identical despite different names*

### Comparing `Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/Orange3ImageAnalyticsdoc.hhp` & `Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/Orange3ImageAnalyticsdoc.hhp`

 * *Files identical despite different names*

### Comparing `Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/_images/socioeconomic-indices.png` & `Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/_images/socioeconomic-indices.png`

 * *Files identical despite different names*

### Comparing `Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/_static/basic.css` & `Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/_static/basic.css`

 * *Files 1% similar despite different names*

```diff
@@ -218,39 +218,39 @@
     padding: 2px;
     border-collapse: collapse;
 }
 
 /* -- general body styles --------------------------------------------------- */
 
 div.body {
-    min-width: 450px;
+    min-width: 360px;
     max-width: 800px;
 }
 
 div.body p, div.body dd, div.body li, div.body blockquote {
     -moz-hyphens: auto;
     -ms-hyphens: auto;
     -webkit-hyphens: auto;
     hyphens: auto;
 }
 
 a.headerlink {
     visibility: hidden;
 }
-
 a.brackets:before,
 span.brackets > a:before{
     content: "[";
 }
 
 a.brackets:after,
 span.brackets > a:after {
     content: "]";
 }
 
+
 h1:hover > a.headerlink,
 h2:hover > a.headerlink,
 h3:hover > a.headerlink,
 h4:hover > a.headerlink,
 h5:hover > a.headerlink,
 h6:hover > a.headerlink,
 dt:hover > a.headerlink,
@@ -330,21 +330,19 @@
     clear: right;
     overflow-x: auto;
 }
 
 p.sidebar-title {
     font-weight: bold;
 }
-
 div.admonition, div.topic, blockquote {
     clear: left;
 }
 
 /* -- topics ---------------------------------------------------------------- */
-
 div.topic {
     border: 1px solid #ccc;
     padding: 7px;
     margin: 10px 0 10px 0;
 }
 
 p.topic-title {
@@ -424,18 +422,14 @@
     padding: 1px 8px 1px 5px;
     border-top: 0;
     border-left: 0;
     border-right: 0;
     border-bottom: 1px solid #aaa;
 }
 
-table.footnote td, table.footnote th {
-    border: 0 !important;
-}
-
 th {
     text-align: left;
     padding-right: 5px;
 }
 
 table.citation {
     border-left: solid 1px gray;
@@ -610,15 +604,14 @@
     margin-top: 0;
 }
 
 ol.simple p,
 ul.simple p {
     margin-bottom: 0;
 }
-
 dl.footnote > dt,
 dl.citation > dt {
     float: left;
     margin-right: 0.5em;
 }
 
 dl.footnote > dd,
@@ -639,19 +632,19 @@
 
 dl.field-list > dt {
     font-weight: bold;
     word-break: break-word;
     padding-left: 0.5em;
     padding-right: 5px;
 }
-
 dl.field-list > dt:after {
     content: ":";
 }
 
+
 dl.field-list > dd {
     padding-left: 0.5em;
     margin-top: 0em;
     margin-left: 0em;
     margin-bottom: 0em;
 }
```

### Comparing `Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/_static/css/badge_only.css` & `Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/_static/css/badge_only.css`

 * *Files 1% similar despite different names*

```diff
@@ -1 +1 @@
-.fa:before{-webkit-font-smoothing:antialiased}.clearfix{*zoom:1}.clearfix:after,.clearfix:before{display:table;content:""}.clearfix:after{clear:both}@font-face{font-family:FontAwesome;font-style:normal;font-weight:400;src:url(fonts/fontawesome-webfont.eot?674f50d287a8c48dc19ba404d20fe713?#iefix) format("embedded-opentype"),url(fonts/fontawesome-webfont.woff2?af7ae505a9eed503f8b8e6982036873e) format("woff2"),url(fonts/fontawesome-webfont.woff?fee66e712a8a08eef5805a46892932ad) format("woff"),url(fonts/fontawesome-webfont.ttf?b06871f281fee6b241d60582ae9369b9) format("truetype"),url(fonts/fontawesome-webfont.svg?912ec66d7572ff821749319396470bde#FontAwesome) format("svg")}.fa:before{font-family:FontAwesome;font-style:normal;font-weight:400;line-height:1}.fa:before,a .fa{text-decoration:inherit}.fa:before,a .fa,li .fa{display:inline-block}li .fa-large:before{width:1.875em}ul.fas{list-style-type:none;margin-left:2em;text-indent:-.8em}ul.fas li .fa{width:.8em}ul.fas li .fa-large:before{vertical-align:baseline}.fa-book:before,.icon-book:before{content:"\f02d"}.fa-caret-down:before,.icon-caret-down:before{content:"\f0d7"}.fa-caret-up:before,.icon-caret-up:before{content:"\f0d8"}.fa-caret-left:before,.icon-caret-left:before{content:"\f0d9"}.fa-caret-right:before,.icon-caret-right:before{content:"\f0da"}.rst-versions{position:fixed;bottom:0;left:0;width:300px;color:#fcfcfc;background:#1f1d1d;font-family:Lato,proxima-nova,Helvetica Neue,Arial,sans-serif;z-index:400}.rst-versions a{color:#2980b9;text-decoration:none}.rst-versions .rst-badge-small{display:none}.rst-versions .rst-current-version{padding:12px;background-color:#272525;display:block;text-align:right;font-size:90%;cursor:pointer;color:#27ae60}.rst-versions .rst-current-version:after{clear:both;content:"";display:block}.rst-versions .rst-current-version .fa{color:#fcfcfc}.rst-versions .rst-current-version .fa-book,.rst-versions .rst-current-version .icon-book{float:left}.rst-versions .rst-current-version.rst-out-of-date{background-color:#e74c3c;color:#fff}.rst-versions .rst-current-version.rst-active-old-version{background-color:#f1c40f;color:#000}.rst-versions.shift-up{height:auto;max-height:100%;overflow-y:scroll}.rst-versions.shift-up .rst-other-versions{display:block}.rst-versions .rst-other-versions{font-size:90%;padding:12px;color:grey;display:none}.rst-versions .rst-other-versions hr{display:block;height:1px;border:0;margin:20px 0;padding:0;border-top:1px solid #413d3d}.rst-versions .rst-other-versions dd{display:inline-block;margin:0}.rst-versions .rst-other-versions dd a{display:inline-block;padding:6px;color:#fcfcfc}.rst-versions.rst-badge{width:auto;bottom:20px;right:20px;left:auto;border:none;max-width:300px;max-height:90%}.rst-versions.rst-badge .fa-book,.rst-versions.rst-badge .icon-book{float:none;line-height:30px}.rst-versions.rst-badge.shift-up .rst-current-version{text-align:right}.rst-versions.rst-badge.shift-up .rst-current-version .fa-book,.rst-versions.rst-badge.shift-up .rst-current-version .icon-book{float:left}.rst-versions.rst-badge>.rst-current-version{width:auto;height:30px;line-height:30px;padding:0 6px;display:block;text-align:center}@media screen and (max-width:768px){.rst-versions{width:85%;display:none}.rst-versions.shift{display:block}}
+.clearfix{*zoom:1}.clearfix:after,.clearfix:before{display:table;content:""}.clearfix:after{clear:both}@font-face{font-family:FontAwesome;font-style:normal;font-weight:400;src:url(fonts/fontawesome-webfont.eot?674f50d287a8c48dc19ba404d20fe713?#iefix) format("embedded-opentype"),url(fonts/fontawesome-webfont.woff2?af7ae505a9eed503f8b8e6982036873e) format("woff2"),url(fonts/fontawesome-webfont.woff?fee66e712a8a08eef5805a46892932ad) format("woff"),url(fonts/fontawesome-webfont.ttf?b06871f281fee6b241d60582ae9369b9) format("truetype"),url(fonts/fontawesome-webfont.svg?912ec66d7572ff821749319396470bde#FontAwesome) format("svg")}.fa:before{font-family:FontAwesome;font-style:normal;font-weight:400;line-height:1}.fa:before,a .fa{text-decoration:inherit}.fa:before,a .fa,li .fa{display:inline-block}li .fa-large:before{width:1.875em}ul.fas{list-style-type:none;margin-left:2em;text-indent:-.8em}ul.fas li .fa{width:.8em}ul.fas li .fa-large:before{vertical-align:baseline}.fa-book:before,.icon-book:before{content:"\f02d"}.fa-caret-down:before,.icon-caret-down:before{content:"\f0d7"}.fa-caret-up:before,.icon-caret-up:before{content:"\f0d8"}.fa-caret-left:before,.icon-caret-left:before{content:"\f0d9"}.fa-caret-right:before,.icon-caret-right:before{content:"\f0da"}.rst-versions{position:fixed;bottom:0;left:0;width:300px;color:#fcfcfc;background:#1f1d1d;font-family:Lato,proxima-nova,Helvetica Neue,Arial,sans-serif;z-index:400}.rst-versions a{color:#2980b9;text-decoration:none}.rst-versions .rst-badge-small{display:none}.rst-versions .rst-current-version{padding:12px;background-color:#272525;display:block;text-align:right;font-size:90%;cursor:pointer;color:#27ae60}.rst-versions .rst-current-version:after{clear:both;content:"";display:block}.rst-versions .rst-current-version .fa{color:#fcfcfc}.rst-versions .rst-current-version .fa-book,.rst-versions .rst-current-version .icon-book{float:left}.rst-versions .rst-current-version.rst-out-of-date{background-color:#e74c3c;color:#fff}.rst-versions .rst-current-version.rst-active-old-version{background-color:#f1c40f;color:#000}.rst-versions.shift-up{height:auto;max-height:100%;overflow-y:scroll}.rst-versions.shift-up .rst-other-versions{display:block}.rst-versions .rst-other-versions{font-size:90%;padding:12px;color:grey;display:none}.rst-versions .rst-other-versions hr{display:block;height:1px;border:0;margin:20px 0;padding:0;border-top:1px solid #413d3d}.rst-versions .rst-other-versions dd{display:inline-block;margin:0}.rst-versions .rst-other-versions dd a{display:inline-block;padding:6px;color:#fcfcfc}.rst-versions.rst-badge{width:auto;bottom:20px;right:20px;left:auto;border:none;max-width:300px;max-height:90%}.rst-versions.rst-badge .fa-book,.rst-versions.rst-badge .icon-book{float:none;line-height:30px}.rst-versions.rst-badge.shift-up .rst-current-version{text-align:right}.rst-versions.rst-badge.shift-up .rst-current-version .fa-book,.rst-versions.rst-badge.shift-up .rst-current-version .icon-book{float:left}.rst-versions.rst-badge>.rst-current-version{width:auto;height:30px;line-height:30px;padding:0 6px;display:block;text-align:center}@media screen and (max-width:768px){.rst-versions{width:85%;display:none}.rst-versions.shift{display:block}}
```

### Comparing `Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/_static/css/fonts/Roboto-Slab-Bold.woff` & `Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/_static/css/fonts/Roboto-Slab-Bold.woff`

 * *Files identical despite different names*

### Comparing `Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/_static/css/fonts/Roboto-Slab-Bold.woff2` & `Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/_static/css/fonts/Roboto-Slab-Bold.woff2`

 * *Files identical despite different names*

### Comparing `Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/_static/css/fonts/Roboto-Slab-Regular.woff` & `Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/_static/css/fonts/Roboto-Slab-Regular.woff`

 * *Files identical despite different names*

### Comparing `Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/_static/css/fonts/Roboto-Slab-Regular.woff2` & `Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/_static/css/fonts/Roboto-Slab-Regular.woff2`

 * *Files identical despite different names*

### Comparing `Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/_static/css/fonts/fontawesome-webfont.eot` & `Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/_static/css/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/_static/css/fonts/fontawesome-webfont.svg` & `Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/_static/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/_static/css/fonts/fontawesome-webfont.ttf` & `Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/_static/css/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/_static/css/fonts/fontawesome-webfont.woff` & `Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/_static/css/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/_static/css/fonts/fontawesome-webfont.woff2` & `Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/_static/css/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/_static/css/fonts/lato-bold-italic.woff` & `Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/_static/css/fonts/lato-bold-italic.woff`

 * *Files identical despite different names*

### Comparing `Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/_static/css/fonts/lato-bold-italic.woff2` & `Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/_static/css/fonts/lato-bold-italic.woff2`

 * *Files identical despite different names*

### Comparing `Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/_static/css/fonts/lato-bold.woff` & `Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/_static/css/fonts/lato-bold.woff`

 * *Files identical despite different names*

### Comparing `Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/_static/css/fonts/lato-bold.woff2` & `Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/_static/css/fonts/lato-bold.woff2`

 * *Files identical despite different names*

### Comparing `Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/_static/css/fonts/lato-normal-italic.woff` & `Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/_static/css/fonts/lato-normal-italic.woff`

 * *Files identical despite different names*

### Comparing `Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/_static/css/fonts/lato-normal-italic.woff2` & `Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/_static/css/fonts/lato-normal-italic.woff2`

 * *Files identical despite different names*

### Comparing `Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/_static/css/fonts/lato-normal.woff` & `Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/_static/css/fonts/lato-normal.woff`

 * *Files identical despite different names*

### Comparing `Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/_static/css/fonts/lato-normal.woff2` & `Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/_static/css/fonts/lato-normal.woff2`

 * *Files identical despite different names*

### Comparing `Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/_static/css/theme.css` & `Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/_static/css/theme.css`

 * *Files 1% similar despite different names*

```diff
@@ -1,4 +1,4 @@
-html{box-sizing:border-box}*,:after,:before{box-sizing:inherit}article,aside,details,figcaption,figure,footer,header,hgroup,nav,section{display:block}audio,canvas,video{display:inline-block;*display:inline;*zoom:1}[hidden],audio:not([controls]){display:none}*{-webkit-box-sizing:border-box;-moz-box-sizing:border-box;box-sizing:border-box}html{font-size:100%;-webkit-text-size-adjust:100%;-ms-text-size-adjust:100%}body{margin:0}a:active,a:hover{outline:0}abbr[title]{border-bottom:1px dotted}b,strong{font-weight:700}blockquote{margin:0}dfn{font-style:italic}ins{background:#ff9;text-decoration:none}ins,mark{color:#000}mark{background:#ff0;font-style:italic;font-weight:700}.rst-content code,.rst-content tt,code,kbd,pre,samp{font-family:monospace,serif;_font-family:courier new,monospace;font-size:1em}pre{white-space:pre}q{quotes:none}q:after,q:before{content:"";content:none}small{font-size:85%}sub,sup{font-size:75%;line-height:0;position:relative;vertical-align:baseline}sup{top:-.5em}sub{bottom:-.25em}dl,ol,ul{margin:0;padding:0;list-style:none;list-style-image:none}li{list-style:none}dd{margin:0}img{border:0;-ms-interpolation-mode:bicubic;vertical-align:middle;max-width:100%}svg:not(:root){overflow:hidden}figure,form{margin:0}label{cursor:pointer}button,input,select,textarea{font-size:100%;margin:0;vertical-align:baseline;*vertical-align:middle}button,input{line-height:normal}button,input[type=button],input[type=reset],input[type=submit]{cursor:pointer;-webkit-appearance:button;*overflow:visible}button[disabled],input[disabled]{cursor:default}input[type=search]{-webkit-appearance:textfield;-moz-box-sizing:content-box;-webkit-box-sizing:content-box;box-sizing:content-box}textarea{resize:vertical}table{border-collapse:collapse;border-spacing:0}td{vertical-align:top}.chromeframe{margin:.2em 0;background:#ccc;color:#000;padding:.2em 0}.ir{display:block;border:0;text-indent:-999em;overflow:hidden;background-color:transparent;background-repeat:no-repeat;text-align:left;direction:ltr;*line-height:0}.ir br{display:none}.hidden{display:none!important;visibility:hidden}.visuallyhidden{border:0;clip:rect(0 0 0 0);height:1px;margin:-1px;overflow:hidden;padding:0;position:absolute;width:1px}.visuallyhidden.focusable:active,.visuallyhidden.focusable:focus{clip:auto;height:auto;margin:0;overflow:visible;position:static;width:auto}.invisible{visibility:hidden}.relative{position:relative}big,small{font-size:100%}@media print{body,html,section{background:none!important}*{box-shadow:none!important;text-shadow:none!important;filter:none!important;-ms-filter:none!important}a,a:visited{text-decoration:underline}.ir a:after,a[href^="#"]:after,a[href^="javascript:"]:after{content:""}blockquote,pre{page-break-inside:avoid}thead{display:table-header-group}img,tr{page-break-inside:avoid}img{max-width:100%!important}@page{margin:.5cm}.rst-content .toctree-wrapper>p.caption,h2,h3,p{orphans:3;widows:3}.rst-content .toctree-wrapper>p.caption,h2,h3{page-break-after:avoid}}.btn,.fa:before,.icon:before,.rst-content .admonition,.rst-content .admonition-title:before,.rst-content .admonition-todo,.rst-content .attention,.rst-content .caution,.rst-content .code-block-caption .headerlink:before,.rst-content .danger,.rst-content .eqno .headerlink:before,.rst-content .error,.rst-content .hint,.rst-content .important,.rst-content .note,.rst-content .seealso,.rst-content .tip,.rst-content .warning,.rst-content code.download span:first-child:before,.rst-content dl dt .headerlink:before,.rst-content h1 .headerlink:before,.rst-content h2 .headerlink:before,.rst-content h3 .headerlink:before,.rst-content h4 .headerlink:before,.rst-content h5 .headerlink:before,.rst-content h6 .headerlink:before,.rst-content p.caption .headerlink:before,.rst-content p .headerlink:before,.rst-content table>caption .headerlink:before,.rst-content tt.download span:first-child:before,.wy-alert,.wy-dropdown .caret:before,.wy-inline-validate.wy-inline-validate-danger .wy-input-context:before,.wy-inline-validate.wy-inline-validate-info .wy-input-context:before,.wy-inline-validate.wy-inline-validate-success .wy-input-context:before,.wy-inline-validate.wy-inline-validate-warning .wy-input-context:before,.wy-menu-vertical li.current>a,.wy-menu-vertical li.current>a button.toctree-expand:before,.wy-menu-vertical li.on a,.wy-menu-vertical li.on a button.toctree-expand:before,.wy-menu-vertical li button.toctree-expand:before,.wy-nav-top a,.wy-side-nav-search .wy-dropdown>a,.wy-side-nav-search>a,input[type=color],input[type=date],input[type=datetime-local],input[type=datetime],input[type=email],input[type=month],input[type=number],input[type=password],input[type=search],input[type=tel],input[type=text],input[type=time],input[type=url],input[type=week],select,textarea{-webkit-font-smoothing:antialiased}.clearfix{*zoom:1}.clearfix:after,.clearfix:before{display:table;content:""}.clearfix:after{clear:both}/*!
+html{box-sizing:border-box}*,:after,:before{box-sizing:inherit}article,aside,details,figcaption,figure,footer,header,hgroup,nav,section{display:block}audio,canvas,video{display:inline-block;*display:inline;*zoom:1}[hidden],audio:not([controls]){display:none}*{-webkit-box-sizing:border-box;-moz-box-sizing:border-box;box-sizing:border-box}html{font-size:100%;-webkit-text-size-adjust:100%;-ms-text-size-adjust:100%}body{margin:0}a:active,a:hover{outline:0}abbr[title]{border-bottom:1px dotted}b,strong{font-weight:700}blockquote{margin:0}dfn{font-style:italic}ins{background:#ff9;text-decoration:none}ins,mark{color:#000}mark{background:#ff0;font-style:italic;font-weight:700}.rst-content code,.rst-content tt,code,kbd,pre,samp{font-family:monospace,serif;_font-family:courier new,monospace;font-size:1em}pre{white-space:pre}q{quotes:none}q:after,q:before{content:"";content:none}small{font-size:85%}sub,sup{font-size:75%;line-height:0;position:relative;vertical-align:baseline}sup{top:-.5em}sub{bottom:-.25em}dl,ol,ul{margin:0;padding:0;list-style:none;list-style-image:none}li{list-style:none}dd{margin:0}img{border:0;-ms-interpolation-mode:bicubic;vertical-align:middle;max-width:100%}svg:not(:root){overflow:hidden}figure,form{margin:0}label{cursor:pointer}button,input,select,textarea{font-size:100%;margin:0;vertical-align:baseline;*vertical-align:middle}button,input{line-height:normal}button,input[type=button],input[type=reset],input[type=submit]{cursor:pointer;-webkit-appearance:button;*overflow:visible}button[disabled],input[disabled]{cursor:default}input[type=search]{-webkit-appearance:textfield;-moz-box-sizing:content-box;-webkit-box-sizing:content-box;box-sizing:content-box}textarea{resize:vertical}table{border-collapse:collapse;border-spacing:0}td{vertical-align:top}.chromeframe{margin:.2em 0;background:#ccc;color:#000;padding:.2em 0}.ir{display:block;border:0;text-indent:-999em;overflow:hidden;background-color:transparent;background-repeat:no-repeat;text-align:left;direction:ltr;*line-height:0}.ir br{display:none}.hidden{display:none!important;visibility:hidden}.visuallyhidden{border:0;clip:rect(0 0 0 0);height:1px;margin:-1px;overflow:hidden;padding:0;position:absolute;width:1px}.visuallyhidden.focusable:active,.visuallyhidden.focusable:focus{clip:auto;height:auto;margin:0;overflow:visible;position:static;width:auto}.invisible{visibility:hidden}.relative{position:relative}big,small{font-size:100%}@media print{body,html,section{background:none!important}*{box-shadow:none!important;text-shadow:none!important;filter:none!important;-ms-filter:none!important}a,a:visited{text-decoration:underline}.ir a:after,a[href^="#"]:after,a[href^="javascript:"]:after{content:""}blockquote,pre{page-break-inside:avoid}thead{display:table-header-group}img,tr{page-break-inside:avoid}img{max-width:100%!important}@page{margin:.5cm}.rst-content .toctree-wrapper>p.caption,h2,h3,p{orphans:3;widows:3}.rst-content .toctree-wrapper>p.caption,h2,h3{page-break-after:avoid}}.btn,.fa:before,.icon:before,.rst-content .admonition,.rst-content .admonition-title:before,.rst-content .admonition-todo,.rst-content .attention,.rst-content .caution,.rst-content .code-block-caption .headerlink:before,.rst-content .danger,.rst-content .eqno .headerlink:before,.rst-content .error,.rst-content .hint,.rst-content .important,.rst-content .note,.rst-content .seealso,.rst-content .tip,.rst-content .warning,.rst-content code.download span:first-child:before,.rst-content dl dt .headerlink:before,.rst-content h1 .headerlink:before,.rst-content h2 .headerlink:before,.rst-content h3 .headerlink:before,.rst-content h4 .headerlink:before,.rst-content h5 .headerlink:before,.rst-content h6 .headerlink:before,.rst-content p.caption .headerlink:before,.rst-content p .headerlink:before,.rst-content table>caption .headerlink:before,.rst-content tt.download span:first-child:before,.wy-alert,.wy-dropdown .caret:before,.wy-inline-validate.wy-inline-validate-danger .wy-input-context:before,.wy-inline-validate.wy-inline-validate-info .wy-input-context:before,.wy-inline-validate.wy-inline-validate-success .wy-input-context:before,.wy-inline-validate.wy-inline-validate-warning .wy-input-context:before,.wy-menu-vertical li.current>a button.toctree-expand:before,.wy-menu-vertical li.on a button.toctree-expand:before,.wy-menu-vertical li button.toctree-expand:before,input[type=color],input[type=date],input[type=datetime-local],input[type=datetime],input[type=email],input[type=month],input[type=number],input[type=password],input[type=search],input[type=tel],input[type=text],input[type=time],input[type=url],input[type=week],select,textarea{-webkit-font-smoothing:antialiased}.clearfix{*zoom:1}.clearfix:after,.clearfix:before{display:table;content:""}.clearfix:after{clear:both}/*!
  *  Font Awesome 4.7.0 by @davegandy - http://fontawesome.io - @fontawesome
  *  License - http://fontawesome.io/license (Font: SIL OFL 1.1, CSS: MIT License)
- */@font-face{font-family:FontAwesome;src:url(fonts/fontawesome-webfont.eot?674f50d287a8c48dc19ba404d20fe713);src:url(fonts/fontawesome-webfont.eot?674f50d287a8c48dc19ba404d20fe713?#iefix&v=4.7.0) format("embedded-opentype"),url(fonts/fontawesome-webfont.woff2?af7ae505a9eed503f8b8e6982036873e) format("woff2"),url(fonts/fontawesome-webfont.woff?fee66e712a8a08eef5805a46892932ad) format("woff"),url(fonts/fontawesome-webfont.ttf?b06871f281fee6b241d60582ae9369b9) format("truetype"),url(fonts/fontawesome-webfont.svg?912ec66d7572ff821749319396470bde#fontawesomeregular) format("svg");font-weight:400;font-style:normal}.fa,.icon,.rst-content .admonition-title,.rst-content .code-block-caption .headerlink,.rst-content .eqno .headerlink,.rst-content code.download span:first-child,.rst-content dl dt .headerlink,.rst-content h1 .headerlink,.rst-content h2 .headerlink,.rst-content h3 .headerlink,.rst-content h4 .headerlink,.rst-content h5 .headerlink,.rst-content h6 .headerlink,.rst-content p.caption .headerlink,.rst-content p .headerlink,.rst-content table>caption .headerlink,.rst-content tt.download span:first-child,.wy-menu-vertical li.current>a button.toctree-expand,.wy-menu-vertical li.on a button.toctree-expand,.wy-menu-vertical li button.toctree-expand{display:inline-block;font:normal normal normal 14px/1 FontAwesome;font-size:inherit;text-rendering:auto;-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale}.fa-lg{font-size:1.33333em;line-height:.75em;vertical-align:-15%}.fa-2x{font-size:2em}.fa-3x{font-size:3em}.fa-4x{font-size:4em}.fa-5x{font-size:5em}.fa-fw{width:1.28571em;text-align:center}.fa-ul{padding-left:0;margin-left:2.14286em;list-style-type:none}.fa-ul>li{position:relative}.fa-li{position:absolute;left:-2.14286em;width:2.14286em;top:.14286em;text-align:center}.fa-li.fa-lg{left:-1.85714em}.fa-border{padding:.2em .25em .15em;border:.08em solid #eee;border-radius:.1em}.fa-pull-left{float:left}.fa-pull-right{float:right}.fa-pull-left.icon,.fa.fa-pull-left,.rst-content .code-block-caption .fa-pull-left.headerlink,.rst-content .eqno .fa-pull-left.headerlink,.rst-content .fa-pull-left.admonition-title,.rst-content code.download span.fa-pull-left:first-child,.rst-content dl dt .fa-pull-left.headerlink,.rst-content h1 .fa-pull-left.headerlink,.rst-content h2 .fa-pull-left.headerlink,.rst-content h3 .fa-pull-left.headerlink,.rst-content h4 .fa-pull-left.headerlink,.rst-content h5 .fa-pull-left.headerlink,.rst-content h6 .fa-pull-left.headerlink,.rst-content p .fa-pull-left.headerlink,.rst-content table>caption .fa-pull-left.headerlink,.rst-content tt.download span.fa-pull-left:first-child,.wy-menu-vertical li.current>a button.fa-pull-left.toctree-expand,.wy-menu-vertical li.on a button.fa-pull-left.toctree-expand,.wy-menu-vertical li button.fa-pull-left.toctree-expand{margin-right:.3em}.fa-pull-right.icon,.fa.fa-pull-right,.rst-content .code-block-caption .fa-pull-right.headerlink,.rst-content .eqno .fa-pull-right.headerlink,.rst-content .fa-pull-right.admonition-title,.rst-content code.download span.fa-pull-right:first-child,.rst-content dl dt .fa-pull-right.headerlink,.rst-content h1 .fa-pull-right.headerlink,.rst-content h2 .fa-pull-right.headerlink,.rst-content h3 .fa-pull-right.headerlink,.rst-content h4 .fa-pull-right.headerlink,.rst-content h5 .fa-pull-right.headerlink,.rst-content h6 .fa-pull-right.headerlink,.rst-content p .fa-pull-right.headerlink,.rst-content table>caption .fa-pull-right.headerlink,.rst-content tt.download span.fa-pull-right:first-child,.wy-menu-vertical li.current>a button.fa-pull-right.toctree-expand,.wy-menu-vertical li.on a button.fa-pull-right.toctree-expand,.wy-menu-vertical li button.fa-pull-right.toctree-expand{margin-left:.3em}.pull-right{float:right}.pull-left{float:left}.fa.pull-left,.pull-left.icon,.rst-content .code-block-caption .pull-left.headerlink,.rst-content .eqno .pull-left.headerlink,.rst-content .pull-left.admonition-title,.rst-content code.download span.pull-left:first-child,.rst-content dl dt .pull-left.headerlink,.rst-content h1 .pull-left.headerlink,.rst-content h2 .pull-left.headerlink,.rst-content h3 .pull-left.headerlink,.rst-content h4 .pull-left.headerlink,.rst-content h5 .pull-left.headerlink,.rst-content h6 .pull-left.headerlink,.rst-content p .pull-left.headerlink,.rst-content table>caption .pull-left.headerlink,.rst-content tt.download span.pull-left:first-child,.wy-menu-vertical li.current>a button.pull-left.toctree-expand,.wy-menu-vertical li.on a button.pull-left.toctree-expand,.wy-menu-vertical li button.pull-left.toctree-expand{margin-right:.3em}.fa.pull-right,.pull-right.icon,.rst-content .code-block-caption .pull-right.headerlink,.rst-content .eqno .pull-right.headerlink,.rst-content .pull-right.admonition-title,.rst-content code.download span.pull-right:first-child,.rst-content dl dt .pull-right.headerlink,.rst-content h1 .pull-right.headerlink,.rst-content h2 .pull-right.headerlink,.rst-content h3 .pull-right.headerlink,.rst-content h4 .pull-right.headerlink,.rst-content h5 .pull-right.headerlink,.rst-content h6 .pull-right.headerlink,.rst-content p .pull-right.headerlink,.rst-content table>caption .pull-right.headerlink,.rst-content tt.download span.pull-right:first-child,.wy-menu-vertical li.current>a button.pull-right.toctree-expand,.wy-menu-vertical li.on a button.pull-right.toctree-expand,.wy-menu-vertical li button.pull-right.toctree-expand{margin-left:.3em}.fa-spin{-webkit-animation:fa-spin 2s linear infinite;animation:fa-spin 2s linear infinite}.fa-pulse{-webkit-animation:fa-spin 1s steps(8) infinite;animation:fa-spin 1s steps(8) infinite}@-webkit-keyframes fa-spin{0%{-webkit-transform:rotate(0deg);transform:rotate(0deg)}to{-webkit-transform:rotate(359deg);transform:rotate(359deg)}}@keyframes fa-spin{0%{-webkit-transform:rotate(0deg);transform:rotate(0deg)}to{-webkit-transform:rotate(359deg);transform:rotate(359deg)}}.fa-rotate-90{-ms-filter:"progid:DXImageTransform.Microsoft.BasicImage(rotation=1)";-webkit-transform:rotate(90deg);-ms-transform:rotate(90deg);transform:rotate(90deg)}.fa-rotate-180{-ms-filter:"progid:DXImageTransform.Microsoft.BasicImage(rotation=2)";-webkit-transform:rotate(180deg);-ms-transform:rotate(180deg);transform:rotate(180deg)}.fa-rotate-270{-ms-filter:"progid:DXImageTransform.Microsoft.BasicImage(rotation=3)";-webkit-transform:rotate(270deg);-ms-transform:rotate(270deg);transform:rotate(270deg)}.fa-flip-horizontal{-ms-filter:"progid:DXImageTransform.Microsoft.BasicImage(rotation=0, mirror=1)";-webkit-transform:scaleX(-1);-ms-transform:scaleX(-1);transform:scaleX(-1)}.fa-flip-vertical{-ms-filter:"progid:DXImageTransform.Microsoft.BasicImage(rotation=2, mirror=1)";-webkit-transform:scaleY(-1);-ms-transform:scaleY(-1);transform:scaleY(-1)}:root .fa-flip-horizontal,:root .fa-flip-vertical,:root .fa-rotate-90,:root .fa-rotate-180,:root .fa-rotate-270{filter:none}.fa-stack{position:relative;display:inline-block;width:2em;height:2em;line-height:2em;vertical-align:middle}.fa-stack-1x,.fa-stack-2x{position:absolute;left:0;width:100%;text-align:center}.fa-stack-1x{line-height:inherit}.fa-stack-2x{font-size:2em}.fa-inverse{color:#fff}.fa-glass:before{content:""}.fa-music:before{content:""}.fa-search:before,.icon-search:before{content:""}.fa-envelope-o:before{content:""}.fa-heart:before{content:""}.fa-star:before{content:""}.fa-star-o:before{content:""}.fa-user:before{content:""}.fa-film:before{content:""}.fa-th-large:before{content:""}.fa-th:before{content:""}.fa-th-list:before{content:""}.fa-check:before{content:""}.fa-close:before,.fa-remove:before,.fa-times:before{content:""}.fa-search-plus:before{content:""}.fa-search-minus:before{content:""}.fa-power-off:before{content:""}.fa-signal:before{content:""}.fa-cog:before,.fa-gear:before{content:""}.fa-trash-o:before{content:""}.fa-home:before,.icon-home:before{content:""}.fa-file-o:before{content:""}.fa-clock-o:before{content:""}.fa-road:before{content:""}.fa-download:before,.rst-content code.download span:first-child:before,.rst-content tt.download span:first-child:before{content:""}.fa-arrow-circle-o-down:before{content:""}.fa-arrow-circle-o-up:before{content:""}.fa-inbox:before{content:""}.fa-play-circle-o:before{content:""}.fa-repeat:before,.fa-rotate-right:before{content:""}.fa-refresh:before{content:""}.fa-list-alt:before{content:""}.fa-lock:before{content:""}.fa-flag:before{content:""}.fa-headphones:before{content:""}.fa-volume-off:before{content:""}.fa-volume-down:before{content:""}.fa-volume-up:before{content:""}.fa-qrcode:before{content:""}.fa-barcode:before{content:""}.fa-tag:before{content:""}.fa-tags:before{content:""}.fa-book:before,.icon-book:before{content:""}.fa-bookmark:before{content:""}.fa-print:before{content:""}.fa-camera:before{content:""}.fa-font:before{content:""}.fa-bold:before{content:""}.fa-italic:before{content:""}.fa-text-height:before{content:""}.fa-text-width:before{content:""}.fa-align-left:before{content:""}.fa-align-center:before{content:""}.fa-align-right:before{content:""}.fa-align-justify:before{content:""}.fa-list:before{content:""}.fa-dedent:before,.fa-outdent:before{content:""}.fa-indent:before{content:""}.fa-video-camera:before{content:""}.fa-image:before,.fa-photo:before,.fa-picture-o:before{content:""}.fa-pencil:before{content:""}.fa-map-marker:before{content:""}.fa-adjust:before{content:""}.fa-tint:before{content:""}.fa-edit:before,.fa-pencil-square-o:before{content:""}.fa-share-square-o:before{content:""}.fa-check-square-o:before{content:""}.fa-arrows:before{content:""}.fa-step-backward:before{content:""}.fa-fast-backward:before{content:""}.fa-backward:before{content:""}.fa-play:before{content:""}.fa-pause:before{content:""}.fa-stop:before{content:""}.fa-forward:before{content:""}.fa-fast-forward:before{content:""}.fa-step-forward:before{content:""}.fa-eject:before{content:""}.fa-chevron-left:before{content:""}.fa-chevron-right:before{content:""}.fa-plus-circle:before{content:""}.fa-minus-circle:before{content:""}.fa-times-circle:before,.wy-inline-validate.wy-inline-validate-danger .wy-input-context:before{content:""}.fa-check-circle:before,.wy-inline-validate.wy-inline-validate-success .wy-input-context:before{content:""}.fa-question-circle:before{content:""}.fa-info-circle:before{content:""}.fa-crosshairs:before{content:""}.fa-times-circle-o:before{content:""}.fa-check-circle-o:before{content:""}.fa-ban:before{content:""}.fa-arrow-left:before{content:""}.fa-arrow-right:before{content:""}.fa-arrow-up:before{content:""}.fa-arrow-down:before{content:""}.fa-mail-forward:before,.fa-share:before{content:""}.fa-expand:before{content:""}.fa-compress:before{content:""}.fa-plus:before{content:""}.fa-minus:before{content:""}.fa-asterisk:before{content:""}.fa-exclamation-circle:before,.rst-content .admonition-title:before,.wy-inline-validate.wy-inline-validate-info .wy-input-context:before,.wy-inline-validate.wy-inline-validate-warning .wy-input-context:before{content:""}.fa-gift:before{content:""}.fa-leaf:before{content:""}.fa-fire:before,.icon-fire:before{content:""}.fa-eye:before{content:""}.fa-eye-slash:before{content:""}.fa-exclamation-triangle:before,.fa-warning:before{content:""}.fa-plane:before{content:""}.fa-calendar:before{content:""}.fa-random:before{content:""}.fa-comment:before{content:""}.fa-magnet:before{content:""}.fa-chevron-up:before{content:""}.fa-chevron-down:before{content:""}.fa-retweet:before{content:""}.fa-shopping-cart:before{content:""}.fa-folder:before{content:""}.fa-folder-open:before{content:""}.fa-arrows-v:before{content:""}.fa-arrows-h:before{content:""}.fa-bar-chart-o:before,.fa-bar-chart:before{content:""}.fa-twitter-square:before{content:""}.fa-facebook-square:before{content:""}.fa-camera-retro:before{content:""}.fa-key:before{content:""}.fa-cogs:before,.fa-gears:before{content:""}.fa-comments:before{content:""}.fa-thumbs-o-up:before{content:""}.fa-thumbs-o-down:before{content:""}.fa-star-half:before{content:""}.fa-heart-o:before{content:""}.fa-sign-out:before{content:""}.fa-linkedin-square:before{content:""}.fa-thumb-tack:before{content:""}.fa-external-link:before{content:""}.fa-sign-in:before{content:""}.fa-trophy:before{content:""}.fa-github-square:before{content:""}.fa-upload:before{content:""}.fa-lemon-o:before{content:""}.fa-phone:before{content:""}.fa-square-o:before{content:""}.fa-bookmark-o:before{content:""}.fa-phone-square:before{content:""}.fa-twitter:before{content:""}.fa-facebook-f:before,.fa-facebook:before{content:""}.fa-github:before,.icon-github:before{content:""}.fa-unlock:before{content:""}.fa-credit-card:before{content:""}.fa-feed:before,.fa-rss:before{content:""}.fa-hdd-o:before{content:""}.fa-bullhorn:before{content:""}.fa-bell:before{content:""}.fa-certificate:before{content:""}.fa-hand-o-right:before{content:""}.fa-hand-o-left:before{content:""}.fa-hand-o-up:before{content:""}.fa-hand-o-down:before{content:""}.fa-arrow-circle-left:before,.icon-circle-arrow-left:before{content:""}.fa-arrow-circle-right:before,.icon-circle-arrow-right:before{content:""}.fa-arrow-circle-up:before{content:""}.fa-arrow-circle-down:before{content:""}.fa-globe:before{content:""}.fa-wrench:before{content:""}.fa-tasks:before{content:""}.fa-filter:before{content:""}.fa-briefcase:before{content:""}.fa-arrows-alt:before{content:""}.fa-group:before,.fa-users:before{content:""}.fa-chain:before,.fa-link:before,.icon-link:before{content:""}.fa-cloud:before{content:""}.fa-flask:before{content:""}.fa-cut:before,.fa-scissors:before{content:""}.fa-copy:before,.fa-files-o:before{content:""}.fa-paperclip:before{content:""}.fa-floppy-o:before,.fa-save:before{content:""}.fa-square:before{content:""}.fa-bars:before,.fa-navicon:before,.fa-reorder:before{content:""}.fa-list-ul:before{content:""}.fa-list-ol:before{content:""}.fa-strikethrough:before{content:""}.fa-underline:before{content:""}.fa-table:before{content:""}.fa-magic:before{content:""}.fa-truck:before{content:""}.fa-pinterest:before{content:""}.fa-pinterest-square:before{content:""}.fa-google-plus-square:before{content:""}.fa-google-plus:before{content:""}.fa-money:before{content:""}.fa-caret-down:before,.icon-caret-down:before,.wy-dropdown .caret:before{content:""}.fa-caret-up:before{content:""}.fa-caret-left:before{content:""}.fa-caret-right:before{content:""}.fa-columns:before{content:""}.fa-sort:before,.fa-unsorted:before{content:""}.fa-sort-desc:before,.fa-sort-down:before{content:""}.fa-sort-asc:before,.fa-sort-up:before{content:""}.fa-envelope:before{content:""}.fa-linkedin:before{content:""}.fa-rotate-left:before,.fa-undo:before{content:""}.fa-gavel:before,.fa-legal:before{content:""}.fa-dashboard:before,.fa-tachometer:before{content:""}.fa-comment-o:before{content:""}.fa-comments-o:before{content:""}.fa-bolt:before,.fa-flash:before{content:""}.fa-sitemap:before{content:""}.fa-umbrella:before{content:""}.fa-clipboard:before,.fa-paste:before{content:""}.fa-lightbulb-o:before{content:""}.fa-exchange:before{content:""}.fa-cloud-download:before{content:""}.fa-cloud-upload:before{content:""}.fa-user-md:before{content:""}.fa-stethoscope:before{content:""}.fa-suitcase:before{content:""}.fa-bell-o:before{content:""}.fa-coffee:before{content:""}.fa-cutlery:before{content:""}.fa-file-text-o:before{content:""}.fa-building-o:before{content:""}.fa-hospital-o:before{content:""}.fa-ambulance:before{content:""}.fa-medkit:before{content:""}.fa-fighter-jet:before{content:""}.fa-beer:before{content:""}.fa-h-square:before{content:""}.fa-plus-square:before{content:""}.fa-angle-double-left:before{content:""}.fa-angle-double-right:before{content:""}.fa-angle-double-up:before{content:""}.fa-angle-double-down:before{content:""}.fa-angle-left:before{content:""}.fa-angle-right:before{content:""}.fa-angle-up:before{content:""}.fa-angle-down:before{content:""}.fa-desktop:before{content:""}.fa-laptop:before{content:""}.fa-tablet:before{content:""}.fa-mobile-phone:before,.fa-mobile:before{content:""}.fa-circle-o:before{content:""}.fa-quote-left:before{content:""}.fa-quote-right:before{content:""}.fa-spinner:before{content:""}.fa-circle:before{content:""}.fa-mail-reply:before,.fa-reply:before{content:""}.fa-github-alt:before{content:""}.fa-folder-o:before{content:""}.fa-folder-open-o:before{content:""}.fa-smile-o:before{content:""}.fa-frown-o:before{content:""}.fa-meh-o:before{content:""}.fa-gamepad:before{content:""}.fa-keyboard-o:before{content:""}.fa-flag-o:before{content:""}.fa-flag-checkered:before{content:""}.fa-terminal:before{content:""}.fa-code:before{content:""}.fa-mail-reply-all:before,.fa-reply-all:before{content:""}.fa-star-half-empty:before,.fa-star-half-full:before,.fa-star-half-o:before{content:""}.fa-location-arrow:before{content:""}.fa-crop:before{content:""}.fa-code-fork:before{content:""}.fa-chain-broken:before,.fa-unlink:before{content:""}.fa-question:before{content:""}.fa-info:before{content:""}.fa-exclamation:before{content:""}.fa-superscript:before{content:""}.fa-subscript:before{content:""}.fa-eraser:before{content:""}.fa-puzzle-piece:before{content:""}.fa-microphone:before{content:""}.fa-microphone-slash:before{content:""}.fa-shield:before{content:""}.fa-calendar-o:before{content:""}.fa-fire-extinguisher:before{content:""}.fa-rocket:before{content:""}.fa-maxcdn:before{content:""}.fa-chevron-circle-left:before{content:""}.fa-chevron-circle-right:before{content:""}.fa-chevron-circle-up:before{content:""}.fa-chevron-circle-down:before{content:""}.fa-html5:before{content:""}.fa-css3:before{content:""}.fa-anchor:before{content:""}.fa-unlock-alt:before{content:""}.fa-bullseye:before{content:""}.fa-ellipsis-h:before{content:""}.fa-ellipsis-v:before{content:""}.fa-rss-square:before{content:""}.fa-play-circle:before{content:""}.fa-ticket:before{content:""}.fa-minus-square:before{content:""}.fa-minus-square-o:before,.wy-menu-vertical li.current>a button.toctree-expand:before,.wy-menu-vertical li.on a button.toctree-expand:before{content:""}.fa-level-up:before{content:""}.fa-level-down:before{content:""}.fa-check-square:before{content:""}.fa-pencil-square:before{content:""}.fa-external-link-square:before{content:""}.fa-share-square:before{content:""}.fa-compass:before{content:""}.fa-caret-square-o-down:before,.fa-toggle-down:before{content:""}.fa-caret-square-o-up:before,.fa-toggle-up:before{content:""}.fa-caret-square-o-right:before,.fa-toggle-right:before{content:""}.fa-eur:before,.fa-euro:before{content:""}.fa-gbp:before{content:""}.fa-dollar:before,.fa-usd:before{content:""}.fa-inr:before,.fa-rupee:before{content:""}.fa-cny:before,.fa-jpy:before,.fa-rmb:before,.fa-yen:before{content:""}.fa-rouble:before,.fa-rub:before,.fa-ruble:before{content:""}.fa-krw:before,.fa-won:before{content:""}.fa-bitcoin:before,.fa-btc:before{content:""}.fa-file:before{content:""}.fa-file-text:before{content:""}.fa-sort-alpha-asc:before{content:""}.fa-sort-alpha-desc:before{content:""}.fa-sort-amount-asc:before{content:""}.fa-sort-amount-desc:before{content:""}.fa-sort-numeric-asc:before{content:""}.fa-sort-numeric-desc:before{content:""}.fa-thumbs-up:before{content:""}.fa-thumbs-down:before{content:""}.fa-youtube-square:before{content:""}.fa-youtube:before{content:""}.fa-xing:before{content:""}.fa-xing-square:before{content:""}.fa-youtube-play:before{content:""}.fa-dropbox:before{content:""}.fa-stack-overflow:before{content:""}.fa-instagram:before{content:""}.fa-flickr:before{content:""}.fa-adn:before{content:""}.fa-bitbucket:before,.icon-bitbucket:before{content:""}.fa-bitbucket-square:before{content:""}.fa-tumblr:before{content:""}.fa-tumblr-square:before{content:""}.fa-long-arrow-down:before{content:""}.fa-long-arrow-up:before{content:""}.fa-long-arrow-left:before{content:""}.fa-long-arrow-right:before{content:""}.fa-apple:before{content:""}.fa-windows:before{content:""}.fa-android:before{content:""}.fa-linux:before{content:""}.fa-dribbble:before{content:""}.fa-skype:before{content:""}.fa-foursquare:before{content:""}.fa-trello:before{content:""}.fa-female:before{content:""}.fa-male:before{content:""}.fa-gittip:before,.fa-gratipay:before{content:""}.fa-sun-o:before{content:""}.fa-moon-o:before{content:""}.fa-archive:before{content:""}.fa-bug:before{content:""}.fa-vk:before{content:""}.fa-weibo:before{content:""}.fa-renren:before{content:""}.fa-pagelines:before{content:""}.fa-stack-exchange:before{content:""}.fa-arrow-circle-o-right:before{content:""}.fa-arrow-circle-o-left:before{content:""}.fa-caret-square-o-left:before,.fa-toggle-left:before{content:""}.fa-dot-circle-o:before{content:""}.fa-wheelchair:before{content:""}.fa-vimeo-square:before{content:""}.fa-try:before,.fa-turkish-lira:before{content:""}.fa-plus-square-o:before,.wy-menu-vertical li button.toctree-expand:before{content:""}.fa-space-shuttle:before{content:""}.fa-slack:before{content:""}.fa-envelope-square:before{content:""}.fa-wordpress:before{content:""}.fa-openid:before{content:""}.fa-bank:before,.fa-institution:before,.fa-university:before{content:""}.fa-graduation-cap:before,.fa-mortar-board:before{content:""}.fa-yahoo:before{content:""}.fa-google:before{content:""}.fa-reddit:before{content:""}.fa-reddit-square:before{content:""}.fa-stumbleupon-circle:before{content:""}.fa-stumbleupon:before{content:""}.fa-delicious:before{content:""}.fa-digg:before{content:""}.fa-pied-piper-pp:before{content:""}.fa-pied-piper-alt:before{content:""}.fa-drupal:before{content:""}.fa-joomla:before{content:""}.fa-language:before{content:""}.fa-fax:before{content:""}.fa-building:before{content:""}.fa-child:before{content:""}.fa-paw:before{content:""}.fa-spoon:before{content:""}.fa-cube:before{content:""}.fa-cubes:before{content:""}.fa-behance:before{content:""}.fa-behance-square:before{content:""}.fa-steam:before{content:""}.fa-steam-square:before{content:""}.fa-recycle:before{content:""}.fa-automobile:before,.fa-car:before{content:""}.fa-cab:before,.fa-taxi:before{content:""}.fa-tree:before{content:""}.fa-spotify:before{content:""}.fa-deviantart:before{content:""}.fa-soundcloud:before{content:""}.fa-database:before{content:""}.fa-file-pdf-o:before{content:""}.fa-file-word-o:before{content:""}.fa-file-excel-o:before{content:""}.fa-file-powerpoint-o:before{content:""}.fa-file-image-o:before,.fa-file-photo-o:before,.fa-file-picture-o:before{content:""}.fa-file-archive-o:before,.fa-file-zip-o:before{content:""}.fa-file-audio-o:before,.fa-file-sound-o:before{content:""}.fa-file-movie-o:before,.fa-file-video-o:before{content:""}.fa-file-code-o:before{content:""}.fa-vine:before{content:""}.fa-codepen:before{content:""}.fa-jsfiddle:before{content:""}.fa-life-bouy:before,.fa-life-buoy:before,.fa-life-ring:before,.fa-life-saver:before,.fa-support:before{content:""}.fa-circle-o-notch:before{content:""}.fa-ra:before,.fa-rebel:before,.fa-resistance:before{content:""}.fa-empire:before,.fa-ge:before{content:""}.fa-git-square:before{content:""}.fa-git:before{content:""}.fa-hacker-news:before,.fa-y-combinator-square:before,.fa-yc-square:before{content:""}.fa-tencent-weibo:before{content:""}.fa-qq:before{content:""}.fa-wechat:before,.fa-weixin:before{content:""}.fa-paper-plane:before,.fa-send:before{content:""}.fa-paper-plane-o:before,.fa-send-o:before{content:""}.fa-history:before{content:""}.fa-circle-thin:before{content:""}.fa-header:before{content:""}.fa-paragraph:before{content:""}.fa-sliders:before{content:""}.fa-share-alt:before{content:""}.fa-share-alt-square:before{content:""}.fa-bomb:before{content:""}.fa-futbol-o:before,.fa-soccer-ball-o:before{content:""}.fa-tty:before{content:""}.fa-binoculars:before{content:""}.fa-plug:before{content:""}.fa-slideshare:before{content:""}.fa-twitch:before{content:""}.fa-yelp:before{content:""}.fa-newspaper-o:before{content:""}.fa-wifi:before{content:""}.fa-calculator:before{content:""}.fa-paypal:before{content:""}.fa-google-wallet:before{content:""}.fa-cc-visa:before{content:""}.fa-cc-mastercard:before{content:""}.fa-cc-discover:before{content:""}.fa-cc-amex:before{content:""}.fa-cc-paypal:before{content:""}.fa-cc-stripe:before{content:""}.fa-bell-slash:before{content:""}.fa-bell-slash-o:before{content:""}.fa-trash:before{content:""}.fa-copyright:before{content:""}.fa-at:before{content:""}.fa-eyedropper:before{content:""}.fa-paint-brush:before{content:""}.fa-birthday-cake:before{content:""}.fa-area-chart:before{content:""}.fa-pie-chart:before{content:""}.fa-line-chart:before{content:""}.fa-lastfm:before{content:""}.fa-lastfm-square:before{content:""}.fa-toggle-off:before{content:""}.fa-toggle-on:before{content:""}.fa-bicycle:before{content:""}.fa-bus:before{content:""}.fa-ioxhost:before{content:""}.fa-angellist:before{content:""}.fa-cc:before{content:""}.fa-ils:before,.fa-shekel:before,.fa-sheqel:before{content:""}.fa-meanpath:before{content:""}.fa-buysellads:before{content:""}.fa-connectdevelop:before{content:""}.fa-dashcube:before{content:""}.fa-forumbee:before{content:""}.fa-leanpub:before{content:""}.fa-sellsy:before{content:""}.fa-shirtsinbulk:before{content:""}.fa-simplybuilt:before{content:""}.fa-skyatlas:before{content:""}.fa-cart-plus:before{content:""}.fa-cart-arrow-down:before{content:""}.fa-diamond:before{content:""}.fa-ship:before{content:""}.fa-user-secret:before{content:""}.fa-motorcycle:before{content:""}.fa-street-view:before{content:""}.fa-heartbeat:before{content:""}.fa-venus:before{content:""}.fa-mars:before{content:""}.fa-mercury:before{content:""}.fa-intersex:before,.fa-transgender:before{content:""}.fa-transgender-alt:before{content:""}.fa-venus-double:before{content:""}.fa-mars-double:before{content:""}.fa-venus-mars:before{content:""}.fa-mars-stroke:before{content:""}.fa-mars-stroke-v:before{content:""}.fa-mars-stroke-h:before{content:""}.fa-neuter:before{content:""}.fa-genderless:before{content:""}.fa-facebook-official:before{content:""}.fa-pinterest-p:before{content:""}.fa-whatsapp:before{content:""}.fa-server:before{content:""}.fa-user-plus:before{content:""}.fa-user-times:before{content:""}.fa-bed:before,.fa-hotel:before{content:""}.fa-viacoin:before{content:""}.fa-train:before{content:""}.fa-subway:before{content:""}.fa-medium:before{content:""}.fa-y-combinator:before,.fa-yc:before{content:""}.fa-optin-monster:before{content:""}.fa-opencart:before{content:""}.fa-expeditedssl:before{content:""}.fa-battery-4:before,.fa-battery-full:before,.fa-battery:before{content:""}.fa-battery-3:before,.fa-battery-three-quarters:before{content:""}.fa-battery-2:before,.fa-battery-half:before{content:""}.fa-battery-1:before,.fa-battery-quarter:before{content:""}.fa-battery-0:before,.fa-battery-empty:before{content:""}.fa-mouse-pointer:before{content:""}.fa-i-cursor:before{content:""}.fa-object-group:before{content:""}.fa-object-ungroup:before{content:""}.fa-sticky-note:before{content:""}.fa-sticky-note-o:before{content:""}.fa-cc-jcb:before{content:""}.fa-cc-diners-club:before{content:""}.fa-clone:before{content:""}.fa-balance-scale:before{content:""}.fa-hourglass-o:before{content:""}.fa-hourglass-1:before,.fa-hourglass-start:before{content:""}.fa-hourglass-2:before,.fa-hourglass-half:before{content:""}.fa-hourglass-3:before,.fa-hourglass-end:before{content:""}.fa-hourglass:before{content:""}.fa-hand-grab-o:before,.fa-hand-rock-o:before{content:""}.fa-hand-paper-o:before,.fa-hand-stop-o:before{content:""}.fa-hand-scissors-o:before{content:""}.fa-hand-lizard-o:before{content:""}.fa-hand-spock-o:before{content:""}.fa-hand-pointer-o:before{content:""}.fa-hand-peace-o:before{content:""}.fa-trademark:before{content:""}.fa-registered:before{content:""}.fa-creative-commons:before{content:""}.fa-gg:before{content:""}.fa-gg-circle:before{content:""}.fa-tripadvisor:before{content:""}.fa-odnoklassniki:before{content:""}.fa-odnoklassniki-square:before{content:""}.fa-get-pocket:before{content:""}.fa-wikipedia-w:before{content:""}.fa-safari:before{content:""}.fa-chrome:before{content:""}.fa-firefox:before{content:""}.fa-opera:before{content:""}.fa-internet-explorer:before{content:""}.fa-television:before,.fa-tv:before{content:""}.fa-contao:before{content:""}.fa-500px:before{content:""}.fa-amazon:before{content:""}.fa-calendar-plus-o:before{content:""}.fa-calendar-minus-o:before{content:""}.fa-calendar-times-o:before{content:""}.fa-calendar-check-o:before{content:""}.fa-industry:before{content:""}.fa-map-pin:before{content:""}.fa-map-signs:before{content:""}.fa-map-o:before{content:""}.fa-map:before{content:""}.fa-commenting:before{content:""}.fa-commenting-o:before{content:""}.fa-houzz:before{content:""}.fa-vimeo:before{content:""}.fa-black-tie:before{content:""}.fa-fonticons:before{content:""}.fa-reddit-alien:before{content:""}.fa-edge:before{content:""}.fa-credit-card-alt:before{content:""}.fa-codiepie:before{content:""}.fa-modx:before{content:""}.fa-fort-awesome:before{content:""}.fa-usb:before{content:""}.fa-product-hunt:before{content:""}.fa-mixcloud:before{content:""}.fa-scribd:before{content:""}.fa-pause-circle:before{content:""}.fa-pause-circle-o:before{content:""}.fa-stop-circle:before{content:""}.fa-stop-circle-o:before{content:""}.fa-shopping-bag:before{content:""}.fa-shopping-basket:before{content:""}.fa-hashtag:before{content:""}.fa-bluetooth:before{content:""}.fa-bluetooth-b:before{content:""}.fa-percent:before{content:""}.fa-gitlab:before,.icon-gitlab:before{content:""}.fa-wpbeginner:before{content:""}.fa-wpforms:before{content:""}.fa-envira:before{content:""}.fa-universal-access:before{content:""}.fa-wheelchair-alt:before{content:""}.fa-question-circle-o:before{content:""}.fa-blind:before{content:""}.fa-audio-description:before{content:""}.fa-volume-control-phone:before{content:""}.fa-braille:before{content:""}.fa-assistive-listening-systems:before{content:""}.fa-american-sign-language-interpreting:before,.fa-asl-interpreting:before{content:""}.fa-deaf:before,.fa-deafness:before,.fa-hard-of-hearing:before{content:""}.fa-glide:before{content:""}.fa-glide-g:before{content:""}.fa-sign-language:before,.fa-signing:before{content:""}.fa-low-vision:before{content:""}.fa-viadeo:before{content:""}.fa-viadeo-square:before{content:""}.fa-snapchat:before{content:""}.fa-snapchat-ghost:before{content:""}.fa-snapchat-square:before{content:""}.fa-pied-piper:before{content:""}.fa-first-order:before{content:""}.fa-yoast:before{content:""}.fa-themeisle:before{content:""}.fa-google-plus-circle:before,.fa-google-plus-official:before{content:""}.fa-fa:before,.fa-font-awesome:before{content:""}.fa-handshake-o:before{content:""}.fa-envelope-open:before{content:""}.fa-envelope-open-o:before{content:""}.fa-linode:before{content:""}.fa-address-book:before{content:""}.fa-address-book-o:before{content:""}.fa-address-card:before,.fa-vcard:before{content:""}.fa-address-card-o:before,.fa-vcard-o:before{content:""}.fa-user-circle:before{content:""}.fa-user-circle-o:before{content:""}.fa-user-o:before{content:""}.fa-id-badge:before{content:""}.fa-drivers-license:before,.fa-id-card:before{content:""}.fa-drivers-license-o:before,.fa-id-card-o:before{content:""}.fa-quora:before{content:""}.fa-free-code-camp:before{content:""}.fa-telegram:before{content:""}.fa-thermometer-4:before,.fa-thermometer-full:before,.fa-thermometer:before{content:""}.fa-thermometer-3:before,.fa-thermometer-three-quarters:before{content:""}.fa-thermometer-2:before,.fa-thermometer-half:before{content:""}.fa-thermometer-1:before,.fa-thermometer-quarter:before{content:""}.fa-thermometer-0:before,.fa-thermometer-empty:before{content:""}.fa-shower:before{content:""}.fa-bath:before,.fa-bathtub:before,.fa-s15:before{content:""}.fa-podcast:before{content:""}.fa-window-maximize:before{content:""}.fa-window-minimize:before{content:""}.fa-window-restore:before{content:""}.fa-times-rectangle:before,.fa-window-close:before{content:""}.fa-times-rectangle-o:before,.fa-window-close-o:before{content:""}.fa-bandcamp:before{content:""}.fa-grav:before{content:""}.fa-etsy:before{content:""}.fa-imdb:before{content:""}.fa-ravelry:before{content:""}.fa-eercast:before{content:""}.fa-microchip:before{content:""}.fa-snowflake-o:before{content:""}.fa-superpowers:before{content:""}.fa-wpexplorer:before{content:""}.fa-meetup:before{content:""}.sr-only{position:absolute;width:1px;height:1px;padding:0;margin:-1px;overflow:hidden;clip:rect(0,0,0,0);border:0}.sr-only-focusable:active,.sr-only-focusable:focus{position:static;width:auto;height:auto;margin:0;overflow:visible;clip:auto}.fa,.icon,.rst-content .admonition-title,.rst-content .code-block-caption .headerlink,.rst-content .eqno .headerlink,.rst-content code.download span:first-child,.rst-content dl dt .headerlink,.rst-content h1 .headerlink,.rst-content h2 .headerlink,.rst-content h3 .headerlink,.rst-content h4 .headerlink,.rst-content h5 .headerlink,.rst-content h6 .headerlink,.rst-content p.caption .headerlink,.rst-content p .headerlink,.rst-content table>caption .headerlink,.rst-content tt.download span:first-child,.wy-dropdown .caret,.wy-inline-validate.wy-inline-validate-danger .wy-input-context,.wy-inline-validate.wy-inline-validate-info .wy-input-context,.wy-inline-validate.wy-inline-validate-success .wy-input-context,.wy-inline-validate.wy-inline-validate-warning .wy-input-context,.wy-menu-vertical li.current>a button.toctree-expand,.wy-menu-vertical li.on a button.toctree-expand,.wy-menu-vertical li button.toctree-expand{font-family:inherit}.fa:before,.icon:before,.rst-content .admonition-title:before,.rst-content .code-block-caption .headerlink:before,.rst-content .eqno .headerlink:before,.rst-content code.download span:first-child:before,.rst-content dl dt .headerlink:before,.rst-content h1 .headerlink:before,.rst-content h2 .headerlink:before,.rst-content h3 .headerlink:before,.rst-content h4 .headerlink:before,.rst-content h5 .headerlink:before,.rst-content h6 .headerlink:before,.rst-content p.caption .headerlink:before,.rst-content p .headerlink:before,.rst-content table>caption .headerlink:before,.rst-content tt.download span:first-child:before,.wy-dropdown .caret:before,.wy-inline-validate.wy-inline-validate-danger .wy-input-context:before,.wy-inline-validate.wy-inline-validate-info .wy-input-context:before,.wy-inline-validate.wy-inline-validate-success .wy-input-context:before,.wy-inline-validate.wy-inline-validate-warning .wy-input-context:before,.wy-menu-vertical li.current>a button.toctree-expand:before,.wy-menu-vertical li.on a button.toctree-expand:before,.wy-menu-vertical li button.toctree-expand:before{font-family:FontAwesome;display:inline-block;font-style:normal;font-weight:400;line-height:1;text-decoration:inherit}.rst-content .code-block-caption a .headerlink,.rst-content .eqno a .headerlink,.rst-content a .admonition-title,.rst-content code.download a span:first-child,.rst-content dl dt a .headerlink,.rst-content h1 a .headerlink,.rst-content h2 a .headerlink,.rst-content h3 a .headerlink,.rst-content h4 a .headerlink,.rst-content h5 a .headerlink,.rst-content h6 a .headerlink,.rst-content p.caption a .headerlink,.rst-content p a .headerlink,.rst-content table>caption a .headerlink,.rst-content tt.download a span:first-child,.wy-menu-vertical li.current>a button.toctree-expand,.wy-menu-vertical li.on a button.toctree-expand,.wy-menu-vertical li a button.toctree-expand,a .fa,a .icon,a .rst-content .admonition-title,a .rst-content .code-block-caption .headerlink,a .rst-content .eqno .headerlink,a .rst-content code.download span:first-child,a .rst-content dl dt .headerlink,a .rst-content h1 .headerlink,a .rst-content h2 .headerlink,a .rst-content h3 .headerlink,a .rst-content h4 .headerlink,a .rst-content h5 .headerlink,a .rst-content h6 .headerlink,a .rst-content p.caption .headerlink,a .rst-content p .headerlink,a .rst-content table>caption .headerlink,a .rst-content tt.download span:first-child,a .wy-menu-vertical li button.toctree-expand{display:inline-block;text-decoration:inherit}.btn .fa,.btn .icon,.btn .rst-content .admonition-title,.btn .rst-content .code-block-caption .headerlink,.btn .rst-content .eqno .headerlink,.btn .rst-content code.download span:first-child,.btn .rst-content dl dt .headerlink,.btn .rst-content h1 .headerlink,.btn .rst-content h2 .headerlink,.btn .rst-content h3 .headerlink,.btn .rst-content h4 .headerlink,.btn .rst-content h5 .headerlink,.btn .rst-content h6 .headerlink,.btn .rst-content p .headerlink,.btn .rst-content table>caption .headerlink,.btn .rst-content tt.download span:first-child,.btn .wy-menu-vertical li.current>a button.toctree-expand,.btn .wy-menu-vertical li.on a button.toctree-expand,.btn .wy-menu-vertical li button.toctree-expand,.nav .fa,.nav .icon,.nav .rst-content .admonition-title,.nav .rst-content .code-block-caption .headerlink,.nav .rst-content .eqno .headerlink,.nav .rst-content code.download span:first-child,.nav .rst-content dl dt .headerlink,.nav .rst-content h1 .headerlink,.nav .rst-content h2 .headerlink,.nav .rst-content h3 .headerlink,.nav .rst-content h4 .headerlink,.nav .rst-content h5 .headerlink,.nav .rst-content h6 .headerlink,.nav .rst-content p .headerlink,.nav .rst-content table>caption .headerlink,.nav .rst-content tt.download span:first-child,.nav .wy-menu-vertical li.current>a button.toctree-expand,.nav .wy-menu-vertical li.on a button.toctree-expand,.nav .wy-menu-vertical li button.toctree-expand,.rst-content .btn .admonition-title,.rst-content .code-block-caption .btn .headerlink,.rst-content .code-block-caption .nav .headerlink,.rst-content .eqno .btn .headerlink,.rst-content .eqno .nav .headerlink,.rst-content .nav .admonition-title,.rst-content code.download .btn span:first-child,.rst-content code.download .nav span:first-child,.rst-content dl dt .btn .headerlink,.rst-content dl dt .nav .headerlink,.rst-content h1 .btn .headerlink,.rst-content h1 .nav .headerlink,.rst-content h2 .btn .headerlink,.rst-content h2 .nav .headerlink,.rst-content h3 .btn .headerlink,.rst-content h3 .nav .headerlink,.rst-content h4 .btn .headerlink,.rst-content h4 .nav .headerlink,.rst-content h5 .btn .headerlink,.rst-content h5 .nav .headerlink,.rst-content h6 .btn .headerlink,.rst-content h6 .nav .headerlink,.rst-content p .btn .headerlink,.rst-content p .nav .headerlink,.rst-content table>caption .btn .headerlink,.rst-content table>caption .nav .headerlink,.rst-content tt.download .btn span:first-child,.rst-content tt.download .nav span:first-child,.wy-menu-vertical li .btn button.toctree-expand,.wy-menu-vertical li.current>a .btn button.toctree-expand,.wy-menu-vertical li.current>a .nav button.toctree-expand,.wy-menu-vertical li .nav button.toctree-expand,.wy-menu-vertical li.on a .btn button.toctree-expand,.wy-menu-vertical li.on a .nav button.toctree-expand{display:inline}.btn .fa-large.icon,.btn .fa.fa-large,.btn .rst-content .code-block-caption .fa-large.headerlink,.btn .rst-content .eqno .fa-large.headerlink,.btn .rst-content .fa-large.admonition-title,.btn .rst-content code.download span.fa-large:first-child,.btn .rst-content dl dt .fa-large.headerlink,.btn .rst-content h1 .fa-large.headerlink,.btn .rst-content h2 .fa-large.headerlink,.btn .rst-content h3 .fa-large.headerlink,.btn .rst-content h4 .fa-large.headerlink,.btn .rst-content h5 .fa-large.headerlink,.btn .rst-content h6 .fa-large.headerlink,.btn .rst-content p .fa-large.headerlink,.btn .rst-content table>caption .fa-large.headerlink,.btn .rst-content tt.download span.fa-large:first-child,.btn .wy-menu-vertical li button.fa-large.toctree-expand,.nav .fa-large.icon,.nav .fa.fa-large,.nav .rst-content .code-block-caption .fa-large.headerlink,.nav .rst-content .eqno .fa-large.headerlink,.nav .rst-content .fa-large.admonition-title,.nav .rst-content code.download span.fa-large:first-child,.nav .rst-content dl dt .fa-large.headerlink,.nav .rst-content h1 .fa-large.headerlink,.nav .rst-content h2 .fa-large.headerlink,.nav .rst-content h3 .fa-large.headerlink,.nav .rst-content h4 .fa-large.headerlink,.nav .rst-content h5 .fa-large.headerlink,.nav .rst-content h6 .fa-large.headerlink,.nav .rst-content p .fa-large.headerlink,.nav .rst-content table>caption .fa-large.headerlink,.nav .rst-content tt.download span.fa-large:first-child,.nav .wy-menu-vertical li button.fa-large.toctree-expand,.rst-content .btn .fa-large.admonition-title,.rst-content .code-block-caption .btn .fa-large.headerlink,.rst-content .code-block-caption .nav .fa-large.headerlink,.rst-content .eqno .btn .fa-large.headerlink,.rst-content .eqno .nav .fa-large.headerlink,.rst-content .nav .fa-large.admonition-title,.rst-content code.download .btn span.fa-large:first-child,.rst-content code.download .nav span.fa-large:first-child,.rst-content dl dt .btn .fa-large.headerlink,.rst-content dl dt .nav .fa-large.headerlink,.rst-content h1 .btn .fa-large.headerlink,.rst-content h1 .nav .fa-large.headerlink,.rst-content h2 .btn .fa-large.headerlink,.rst-content h2 .nav .fa-large.headerlink,.rst-content h3 .btn .fa-large.headerlink,.rst-content h3 .nav .fa-large.headerlink,.rst-content h4 .btn .fa-large.headerlink,.rst-content h4 .nav .fa-large.headerlink,.rst-content h5 .btn .fa-large.headerlink,.rst-content h5 .nav .fa-large.headerlink,.rst-content h6 .btn .fa-large.headerlink,.rst-content h6 .nav .fa-large.headerlink,.rst-content p .btn .fa-large.headerlink,.rst-content p .nav .fa-large.headerlink,.rst-content table>caption .btn .fa-large.headerlink,.rst-content table>caption .nav .fa-large.headerlink,.rst-content tt.download .btn span.fa-large:first-child,.rst-content tt.download .nav span.fa-large:first-child,.wy-menu-vertical li .btn button.fa-large.toctree-expand,.wy-menu-vertical li .nav button.fa-large.toctree-expand{line-height:.9em}.btn .fa-spin.icon,.btn .fa.fa-spin,.btn .rst-content .code-block-caption .fa-spin.headerlink,.btn .rst-content .eqno .fa-spin.headerlink,.btn .rst-content .fa-spin.admonition-title,.btn .rst-content code.download span.fa-spin:first-child,.btn .rst-content dl dt .fa-spin.headerlink,.btn .rst-content h1 .fa-spin.headerlink,.btn .rst-content h2 .fa-spin.headerlink,.btn .rst-content h3 .fa-spin.headerlink,.btn .rst-content h4 .fa-spin.headerlink,.btn .rst-content h5 .fa-spin.headerlink,.btn .rst-content h6 .fa-spin.headerlink,.btn .rst-content p .fa-spin.headerlink,.btn .rst-content table>caption .fa-spin.headerlink,.btn .rst-content tt.download span.fa-spin:first-child,.btn .wy-menu-vertical li button.fa-spin.toctree-expand,.nav .fa-spin.icon,.nav .fa.fa-spin,.nav .rst-content .code-block-caption .fa-spin.headerlink,.nav .rst-content .eqno .fa-spin.headerlink,.nav .rst-content .fa-spin.admonition-title,.nav .rst-content code.download span.fa-spin:first-child,.nav .rst-content dl dt .fa-spin.headerlink,.nav .rst-content h1 .fa-spin.headerlink,.nav .rst-content h2 .fa-spin.headerlink,.nav .rst-content h3 .fa-spin.headerlink,.nav .rst-content h4 .fa-spin.headerlink,.nav .rst-content h5 .fa-spin.headerlink,.nav .rst-content h6 .fa-spin.headerlink,.nav .rst-content p .fa-spin.headerlink,.nav .rst-content table>caption .fa-spin.headerlink,.nav .rst-content tt.download span.fa-spin:first-child,.nav .wy-menu-vertical li button.fa-spin.toctree-expand,.rst-content .btn .fa-spin.admonition-title,.rst-content .code-block-caption .btn .fa-spin.headerlink,.rst-content .code-block-caption .nav .fa-spin.headerlink,.rst-content .eqno .btn .fa-spin.headerlink,.rst-content .eqno .nav .fa-spin.headerlink,.rst-content .nav .fa-spin.admonition-title,.rst-content code.download .btn span.fa-spin:first-child,.rst-content code.download .nav span.fa-spin:first-child,.rst-content dl dt .btn .fa-spin.headerlink,.rst-content dl dt .nav .fa-spin.headerlink,.rst-content h1 .btn .fa-spin.headerlink,.rst-content h1 .nav .fa-spin.headerlink,.rst-content h2 .btn .fa-spin.headerlink,.rst-content h2 .nav .fa-spin.headerlink,.rst-content h3 .btn .fa-spin.headerlink,.rst-content h3 .nav .fa-spin.headerlink,.rst-content h4 .btn .fa-spin.headerlink,.rst-content h4 .nav .fa-spin.headerlink,.rst-content h5 .btn .fa-spin.headerlink,.rst-content h5 .nav .fa-spin.headerlink,.rst-content h6 .btn .fa-spin.headerlink,.rst-content h6 .nav .fa-spin.headerlink,.rst-content p .btn .fa-spin.headerlink,.rst-content p .nav .fa-spin.headerlink,.rst-content table>caption .btn .fa-spin.headerlink,.rst-content table>caption .nav .fa-spin.headerlink,.rst-content tt.download .btn span.fa-spin:first-child,.rst-content tt.download .nav span.fa-spin:first-child,.wy-menu-vertical li .btn button.fa-spin.toctree-expand,.wy-menu-vertical li .nav button.fa-spin.toctree-expand{display:inline-block}.btn.fa:before,.btn.icon:before,.rst-content .btn.admonition-title:before,.rst-content .code-block-caption .btn.headerlink:before,.rst-content .eqno .btn.headerlink:before,.rst-content code.download span.btn:first-child:before,.rst-content dl dt .btn.headerlink:before,.rst-content h1 .btn.headerlink:before,.rst-content h2 .btn.headerlink:before,.rst-content h3 .btn.headerlink:before,.rst-content h4 .btn.headerlink:before,.rst-content h5 .btn.headerlink:before,.rst-content h6 .btn.headerlink:before,.rst-content p .btn.headerlink:before,.rst-content table>caption .btn.headerlink:before,.rst-content tt.download span.btn:first-child:before,.wy-menu-vertical li button.btn.toctree-expand:before{opacity:.5;-webkit-transition:opacity .05s ease-in;-moz-transition:opacity .05s ease-in;transition:opacity .05s ease-in}.btn.fa:hover:before,.btn.icon:hover:before,.rst-content .btn.admonition-title:hover:before,.rst-content .code-block-caption .btn.headerlink:hover:before,.rst-content .eqno .btn.headerlink:hover:before,.rst-content code.download span.btn:first-child:hover:before,.rst-content dl dt .btn.headerlink:hover:before,.rst-content h1 .btn.headerlink:hover:before,.rst-content h2 .btn.headerlink:hover:before,.rst-content h3 .btn.headerlink:hover:before,.rst-content h4 .btn.headerlink:hover:before,.rst-content h5 .btn.headerlink:hover:before,.rst-content h6 .btn.headerlink:hover:before,.rst-content p .btn.headerlink:hover:before,.rst-content table>caption .btn.headerlink:hover:before,.rst-content tt.download span.btn:first-child:hover:before,.wy-menu-vertical li button.btn.toctree-expand:hover:before{opacity:1}.btn-mini .fa:before,.btn-mini .icon:before,.btn-mini .rst-content .admonition-title:before,.btn-mini .rst-content .code-block-caption .headerlink:before,.btn-mini .rst-content .eqno .headerlink:before,.btn-mini .rst-content code.download span:first-child:before,.btn-mini .rst-content dl dt .headerlink:before,.btn-mini .rst-content h1 .headerlink:before,.btn-mini .rst-content h2 .headerlink:before,.btn-mini .rst-content h3 .headerlink:before,.btn-mini .rst-content h4 .headerlink:before,.btn-mini .rst-content h5 .headerlink:before,.btn-mini .rst-content h6 .headerlink:before,.btn-mini .rst-content p .headerlink:before,.btn-mini .rst-content table>caption .headerlink:before,.btn-mini .rst-content tt.download span:first-child:before,.btn-mini .wy-menu-vertical li button.toctree-expand:before,.rst-content .btn-mini .admonition-title:before,.rst-content .code-block-caption .btn-mini .headerlink:before,.rst-content .eqno .btn-mini .headerlink:before,.rst-content code.download .btn-mini span:first-child:before,.rst-content dl dt .btn-mini .headerlink:before,.rst-content h1 .btn-mini .headerlink:before,.rst-content h2 .btn-mini .headerlink:before,.rst-content h3 .btn-mini .headerlink:before,.rst-content h4 .btn-mini .headerlink:before,.rst-content h5 .btn-mini .headerlink:before,.rst-content h6 .btn-mini .headerlink:before,.rst-content p .btn-mini .headerlink:before,.rst-content table>caption .btn-mini .headerlink:before,.rst-content tt.download .btn-mini span:first-child:before,.wy-menu-vertical li .btn-mini button.toctree-expand:before{font-size:14px;vertical-align:-15%}.rst-content .admonition,.rst-content .admonition-todo,.rst-content .attention,.rst-content .caution,.rst-content .danger,.rst-content .error,.rst-content .hint,.rst-content .important,.rst-content .note,.rst-content .seealso,.rst-content .tip,.rst-content .warning,.wy-alert{padding:12px;line-height:24px;margin-bottom:24px;background:#e7f2fa}.rst-content .admonition-title,.wy-alert-title{font-weight:700;display:block;color:#fff;background:#6ab0de;padding:6px 12px;margin:-12px -12px 12px}.rst-content .danger,.rst-content .error,.rst-content .wy-alert-danger.admonition,.rst-content .wy-alert-danger.admonition-todo,.rst-content .wy-alert-danger.attention,.rst-content .wy-alert-danger.caution,.rst-content .wy-alert-danger.hint,.rst-content .wy-alert-danger.important,.rst-content .wy-alert-danger.note,.rst-content .wy-alert-danger.seealso,.rst-content .wy-alert-danger.tip,.rst-content .wy-alert-danger.warning,.wy-alert.wy-alert-danger{background:#fdf3f2}.rst-content .danger .admonition-title,.rst-content .danger .wy-alert-title,.rst-content .error .admonition-title,.rst-content .error .wy-alert-title,.rst-content .wy-alert-danger.admonition-todo .admonition-title,.rst-content .wy-alert-danger.admonition-todo .wy-alert-title,.rst-content .wy-alert-danger.admonition .admonition-title,.rst-content .wy-alert-danger.admonition .wy-alert-title,.rst-content .wy-alert-danger.attention .admonition-title,.rst-content .wy-alert-danger.attention .wy-alert-title,.rst-content .wy-alert-danger.caution .admonition-title,.rst-content .wy-alert-danger.caution .wy-alert-title,.rst-content .wy-alert-danger.hint .admonition-title,.rst-content .wy-alert-danger.hint .wy-alert-title,.rst-content .wy-alert-danger.important .admonition-title,.rst-content .wy-alert-danger.important .wy-alert-title,.rst-content .wy-alert-danger.note .admonition-title,.rst-content .wy-alert-danger.note .wy-alert-title,.rst-content .wy-alert-danger.seealso .admonition-title,.rst-content .wy-alert-danger.seealso .wy-alert-title,.rst-content .wy-alert-danger.tip .admonition-title,.rst-content .wy-alert-danger.tip .wy-alert-title,.rst-content .wy-alert-danger.warning .admonition-title,.rst-content .wy-alert-danger.warning .wy-alert-title,.rst-content .wy-alert.wy-alert-danger .admonition-title,.wy-alert.wy-alert-danger .rst-content .admonition-title,.wy-alert.wy-alert-danger .wy-alert-title{background:#f29f97}.rst-content .admonition-todo,.rst-content .attention,.rst-content .caution,.rst-content .warning,.rst-content .wy-alert-warning.admonition,.rst-content .wy-alert-warning.danger,.rst-content .wy-alert-warning.error,.rst-content .wy-alert-warning.hint,.rst-content .wy-alert-warning.important,.rst-content .wy-alert-warning.note,.rst-content .wy-alert-warning.seealso,.rst-content .wy-alert-warning.tip,.wy-alert.wy-alert-warning{background:#ffedcc}.rst-content .admonition-todo .admonition-title,.rst-content .admonition-todo .wy-alert-title,.rst-content .attention .admonition-title,.rst-content .attention .wy-alert-title,.rst-content .caution .admonition-title,.rst-content .caution .wy-alert-title,.rst-content .warning .admonition-title,.rst-content .warning .wy-alert-title,.rst-content .wy-alert-warning.admonition .admonition-title,.rst-content .wy-alert-warning.admonition .wy-alert-title,.rst-content .wy-alert-warning.danger .admonition-title,.rst-content .wy-alert-warning.danger .wy-alert-title,.rst-content .wy-alert-warning.error .admonition-title,.rst-content .wy-alert-warning.error .wy-alert-title,.rst-content .wy-alert-warning.hint .admonition-title,.rst-content .wy-alert-warning.hint .wy-alert-title,.rst-content .wy-alert-warning.important .admonition-title,.rst-content .wy-alert-warning.important .wy-alert-title,.rst-content .wy-alert-warning.note .admonition-title,.rst-content .wy-alert-warning.note .wy-alert-title,.rst-content .wy-alert-warning.seealso .admonition-title,.rst-content .wy-alert-warning.seealso .wy-alert-title,.rst-content .wy-alert-warning.tip .admonition-title,.rst-content .wy-alert-warning.tip .wy-alert-title,.rst-content .wy-alert.wy-alert-warning .admonition-title,.wy-alert.wy-alert-warning .rst-content .admonition-title,.wy-alert.wy-alert-warning .wy-alert-title{background:#f0b37e}.rst-content .note,.rst-content .seealso,.rst-content .wy-alert-info.admonition,.rst-content .wy-alert-info.admonition-todo,.rst-content .wy-alert-info.attention,.rst-content .wy-alert-info.caution,.rst-content .wy-alert-info.danger,.rst-content .wy-alert-info.error,.rst-content .wy-alert-info.hint,.rst-content .wy-alert-info.important,.rst-content .wy-alert-info.tip,.rst-content .wy-alert-info.warning,.wy-alert.wy-alert-info{background:#e7f2fa}.rst-content .note .admonition-title,.rst-content .note .wy-alert-title,.rst-content .seealso .admonition-title,.rst-content .seealso .wy-alert-title,.rst-content .wy-alert-info.admonition-todo .admonition-title,.rst-content .wy-alert-info.admonition-todo .wy-alert-title,.rst-content .wy-alert-info.admonition .admonition-title,.rst-content .wy-alert-info.admonition .wy-alert-title,.rst-content .wy-alert-info.attention .admonition-title,.rst-content .wy-alert-info.attention .wy-alert-title,.rst-content .wy-alert-info.caution .admonition-title,.rst-content .wy-alert-info.caution .wy-alert-title,.rst-content .wy-alert-info.danger .admonition-title,.rst-content .wy-alert-info.danger .wy-alert-title,.rst-content .wy-alert-info.error .admonition-title,.rst-content .wy-alert-info.error .wy-alert-title,.rst-content .wy-alert-info.hint .admonition-title,.rst-content .wy-alert-info.hint .wy-alert-title,.rst-content .wy-alert-info.important .admonition-title,.rst-content .wy-alert-info.important .wy-alert-title,.rst-content .wy-alert-info.tip .admonition-title,.rst-content .wy-alert-info.tip .wy-alert-title,.rst-content .wy-alert-info.warning .admonition-title,.rst-content .wy-alert-info.warning .wy-alert-title,.rst-content .wy-alert.wy-alert-info .admonition-title,.wy-alert.wy-alert-info .rst-content .admonition-title,.wy-alert.wy-alert-info .wy-alert-title{background:#6ab0de}.rst-content .hint,.rst-content .important,.rst-content .tip,.rst-content .wy-alert-success.admonition,.rst-content .wy-alert-success.admonition-todo,.rst-content .wy-alert-success.attention,.rst-content .wy-alert-success.caution,.rst-content .wy-alert-success.danger,.rst-content .wy-alert-success.error,.rst-content .wy-alert-success.note,.rst-content .wy-alert-success.seealso,.rst-content .wy-alert-success.warning,.wy-alert.wy-alert-success{background:#dbfaf4}.rst-content .hint .admonition-title,.rst-content .hint .wy-alert-title,.rst-content .important .admonition-title,.rst-content .important .wy-alert-title,.rst-content .tip .admonition-title,.rst-content .tip .wy-alert-title,.rst-content .wy-alert-success.admonition-todo .admonition-title,.rst-content .wy-alert-success.admonition-todo .wy-alert-title,.rst-content .wy-alert-success.admonition .admonition-title,.rst-content .wy-alert-success.admonition .wy-alert-title,.rst-content .wy-alert-success.attention .admonition-title,.rst-content .wy-alert-success.attention .wy-alert-title,.rst-content .wy-alert-success.caution .admonition-title,.rst-content .wy-alert-success.caution .wy-alert-title,.rst-content .wy-alert-success.danger .admonition-title,.rst-content .wy-alert-success.danger .wy-alert-title,.rst-content .wy-alert-success.error .admonition-title,.rst-content .wy-alert-success.error .wy-alert-title,.rst-content .wy-alert-success.note .admonition-title,.rst-content .wy-alert-success.note .wy-alert-title,.rst-content .wy-alert-success.seealso .admonition-title,.rst-content .wy-alert-success.seealso .wy-alert-title,.rst-content .wy-alert-success.warning .admonition-title,.rst-content .wy-alert-success.warning .wy-alert-title,.rst-content .wy-alert.wy-alert-success .admonition-title,.wy-alert.wy-alert-success .rst-content .admonition-title,.wy-alert.wy-alert-success .wy-alert-title{background:#1abc9c}.rst-content .wy-alert-neutral.admonition,.rst-content .wy-alert-neutral.admonition-todo,.rst-content .wy-alert-neutral.attention,.rst-content .wy-alert-neutral.caution,.rst-content .wy-alert-neutral.danger,.rst-content .wy-alert-neutral.error,.rst-content .wy-alert-neutral.hint,.rst-content .wy-alert-neutral.important,.rst-content .wy-alert-neutral.note,.rst-content .wy-alert-neutral.seealso,.rst-content .wy-alert-neutral.tip,.rst-content .wy-alert-neutral.warning,.wy-alert.wy-alert-neutral{background:#f3f6f6}.rst-content .wy-alert-neutral.admonition-todo .admonition-title,.rst-content .wy-alert-neutral.admonition-todo .wy-alert-title,.rst-content .wy-alert-neutral.admonition .admonition-title,.rst-content .wy-alert-neutral.admonition .wy-alert-title,.rst-content .wy-alert-neutral.attention .admonition-title,.rst-content .wy-alert-neutral.attention .wy-alert-title,.rst-content .wy-alert-neutral.caution .admonition-title,.rst-content .wy-alert-neutral.caution .wy-alert-title,.rst-content .wy-alert-neutral.danger .admonition-title,.rst-content .wy-alert-neutral.danger .wy-alert-title,.rst-content .wy-alert-neutral.error .admonition-title,.rst-content .wy-alert-neutral.error .wy-alert-title,.rst-content .wy-alert-neutral.hint .admonition-title,.rst-content .wy-alert-neutral.hint .wy-alert-title,.rst-content .wy-alert-neutral.important .admonition-title,.rst-content .wy-alert-neutral.important .wy-alert-title,.rst-content .wy-alert-neutral.note .admonition-title,.rst-content .wy-alert-neutral.note .wy-alert-title,.rst-content .wy-alert-neutral.seealso .admonition-title,.rst-content .wy-alert-neutral.seealso .wy-alert-title,.rst-content .wy-alert-neutral.tip .admonition-title,.rst-content .wy-alert-neutral.tip .wy-alert-title,.rst-content .wy-alert-neutral.warning .admonition-title,.rst-content .wy-alert-neutral.warning .wy-alert-title,.rst-content .wy-alert.wy-alert-neutral .admonition-title,.wy-alert.wy-alert-neutral .rst-content .admonition-title,.wy-alert.wy-alert-neutral .wy-alert-title{color:#404040;background:#e1e4e5}.rst-content .wy-alert-neutral.admonition-todo a,.rst-content .wy-alert-neutral.admonition a,.rst-content .wy-alert-neutral.attention a,.rst-content .wy-alert-neutral.caution a,.rst-content .wy-alert-neutral.danger a,.rst-content .wy-alert-neutral.error a,.rst-content .wy-alert-neutral.hint a,.rst-content .wy-alert-neutral.important a,.rst-content .wy-alert-neutral.note a,.rst-content .wy-alert-neutral.seealso a,.rst-content .wy-alert-neutral.tip a,.rst-content .wy-alert-neutral.warning a,.wy-alert.wy-alert-neutral a{color:#2980b9}.rst-content .admonition-todo p:last-child,.rst-content .admonition p:last-child,.rst-content .attention p:last-child,.rst-content .caution p:last-child,.rst-content .danger p:last-child,.rst-content .error p:last-child,.rst-content .hint p:last-child,.rst-content .important p:last-child,.rst-content .note p:last-child,.rst-content .seealso p:last-child,.rst-content .tip p:last-child,.rst-content .warning p:last-child,.wy-alert p:last-child{margin-bottom:0}.wy-tray-container{position:fixed;bottom:0;left:0;z-index:600}.wy-tray-container li{display:block;width:300px;background:transparent;color:#fff;text-align:center;box-shadow:0 5px 5px 0 rgba(0,0,0,.1);padding:0 24px;min-width:20%;opacity:0;height:0;line-height:56px;overflow:hidden;-webkit-transition:all .3s ease-in;-moz-transition:all .3s ease-in;transition:all .3s ease-in}.wy-tray-container li.wy-tray-item-success{background:#27ae60}.wy-tray-container li.wy-tray-item-info{background:#2980b9}.wy-tray-container li.wy-tray-item-warning{background:#e67e22}.wy-tray-container li.wy-tray-item-danger{background:#e74c3c}.wy-tray-container li.on{opacity:1;height:56px}@media screen and (max-width:768px){.wy-tray-container{bottom:auto;top:0;width:100%}.wy-tray-container li{width:100%}}button{font-size:100%;margin:0;vertical-align:baseline;*vertical-align:middle;cursor:pointer;line-height:normal;-webkit-appearance:button;*overflow:visible}button::-moz-focus-inner,input::-moz-focus-inner{border:0;padding:0}button[disabled]{cursor:default}.btn{display:inline-block;border-radius:2px;line-height:normal;white-space:nowrap;text-align:center;cursor:pointer;font-size:100%;padding:6px 12px 8px;color:#fff;border:1px solid rgba(0,0,0,.1);background-color:#27ae60;text-decoration:none;font-weight:400;font-family:Lato,proxima-nova,Helvetica Neue,Arial,sans-serif;box-shadow:inset 0 1px 2px -1px hsla(0,0%,100%,.5),inset 0 -2px 0 0 rgba(0,0,0,.1);outline-none:false;vertical-align:middle;*display:inline;zoom:1;-webkit-user-drag:none;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;-webkit-transition:all .1s linear;-moz-transition:all .1s linear;transition:all .1s linear}.btn-hover{background:#2e8ece;color:#fff}.btn:hover{background:#2cc36b;color:#fff}.btn:focus{background:#2cc36b;outline:0}.btn:active{box-shadow:inset 0 -1px 0 0 rgba(0,0,0,.05),inset 0 2px 0 0 rgba(0,0,0,.1);padding:8px 12px 6px}.btn:visited{color:#fff}.btn-disabled,.btn-disabled:active,.btn-disabled:focus,.btn-disabled:hover,.btn:disabled{background-image:none;filter:progid:DXImageTransform.Microsoft.gradient(enabled = false);filter:alpha(opacity=40);opacity:.4;cursor:not-allowed;box-shadow:none}.btn::-moz-focus-inner{padding:0;border:0}.btn-small{font-size:80%}.btn-info{background-color:#2980b9!important}.btn-info:hover{background-color:#2e8ece!important}.btn-neutral{background-color:#f3f6f6!important;color:#404040!important}.btn-neutral:hover{background-color:#e5ebeb!important;color:#404040}.btn-neutral:visited{color:#404040!important}.btn-success{background-color:#27ae60!important}.btn-success:hover{background-color:#295!important}.btn-danger{background-color:#e74c3c!important}.btn-danger:hover{background-color:#ea6153!important}.btn-warning{background-color:#e67e22!important}.btn-warning:hover{background-color:#e98b39!important}.btn-invert{background-color:#222}.btn-invert:hover{background-color:#2f2f2f!important}.btn-link{background-color:transparent!important;color:#2980b9;box-shadow:none;border-color:transparent!important}.btn-link:active,.btn-link:hover{background-color:transparent!important;color:#409ad5!important;box-shadow:none}.btn-link:visited{color:#9b59b6}.wy-btn-group .btn,.wy-control .btn{vertical-align:middle}.wy-btn-group{margin-bottom:24px;*zoom:1}.wy-btn-group:after,.wy-btn-group:before{display:table;content:""}.wy-btn-group:after{clear:both}.wy-dropdown{position:relative;display:inline-block}.wy-dropdown-active .wy-dropdown-menu{display:block}.wy-dropdown-menu{position:absolute;left:0;display:none;float:left;top:100%;min-width:100%;background:#fcfcfc;z-index:100;border:1px solid #cfd7dd;box-shadow:0 2px 2px 0 rgba(0,0,0,.1);padding:12px}.wy-dropdown-menu>dd>a{display:block;clear:both;color:#404040;white-space:nowrap;font-size:90%;padding:0 12px;cursor:pointer}.wy-dropdown-menu>dd>a:hover{background:#2980b9;color:#fff}.wy-dropdown-menu>dd.divider{border-top:1px solid #cfd7dd;margin:6px 0}.wy-dropdown-menu>dd.search{padding-bottom:12px}.wy-dropdown-menu>dd.search input[type=search]{width:100%}.wy-dropdown-menu>dd.call-to-action{background:#e3e3e3;text-transform:uppercase;font-weight:500;font-size:80%}.wy-dropdown-menu>dd.call-to-action:hover{background:#e3e3e3}.wy-dropdown-menu>dd.call-to-action .btn{color:#fff}.wy-dropdown.wy-dropdown-up .wy-dropdown-menu{bottom:100%;top:auto;left:auto;right:0}.wy-dropdown.wy-dropdown-bubble .wy-dropdown-menu{background:#fcfcfc;margin-top:2px}.wy-dropdown.wy-dropdown-bubble .wy-dropdown-menu a{padding:6px 12px}.wy-dropdown.wy-dropdown-bubble .wy-dropdown-menu a:hover{background:#2980b9;color:#fff}.wy-dropdown.wy-dropdown-left .wy-dropdown-menu{right:0;left:auto;text-align:right}.wy-dropdown-arrow:before{content:" ";border-bottom:5px solid #f5f5f5;border-left:5px solid transparent;border-right:5px solid transparent;position:absolute;display:block;top:-4px;left:50%;margin-left:-3px}.wy-dropdown-arrow.wy-dropdown-arrow-left:before{left:11px}.wy-form-stacked select{display:block}.wy-form-aligned .wy-help-inline,.wy-form-aligned input,.wy-form-aligned label,.wy-form-aligned select,.wy-form-aligned textarea{display:inline-block;*display:inline;*zoom:1;vertical-align:middle}.wy-form-aligned .wy-control-group>label{display:inline-block;vertical-align:middle;width:10em;margin:6px 12px 0 0;float:left}.wy-form-aligned .wy-control{float:left}.wy-form-aligned .wy-control label{display:block}.wy-form-aligned .wy-control select{margin-top:6px}fieldset{margin:0}fieldset,legend{border:0;padding:0}legend{width:100%;white-space:normal;margin-bottom:24px;font-size:150%;*margin-left:-7px}label,legend{display:block}label{margin:0 0 .3125em;color:#333;font-size:90%}input,select,textarea{font-size:100%;margin:0;vertical-align:baseline;*vertical-align:middle}.wy-control-group{margin-bottom:24px;max-width:1200px;margin-left:auto;margin-right:auto;*zoom:1}.wy-control-group:after,.wy-control-group:before{display:table;content:""}.wy-control-group:after{clear:both}.wy-control-group.wy-control-group-required>label:after{content:" *";color:#e74c3c}.wy-control-group .wy-form-full,.wy-control-group .wy-form-halves,.wy-control-group .wy-form-thirds{padding-bottom:12px}.wy-control-group .wy-form-full input[type=color],.wy-control-group .wy-form-full input[type=date],.wy-control-group .wy-form-full input[type=datetime-local],.wy-control-group .wy-form-full input[type=datetime],.wy-control-group .wy-form-full input[type=email],.wy-control-group .wy-form-full input[type=month],.wy-control-group .wy-form-full input[type=number],.wy-control-group .wy-form-full input[type=password],.wy-control-group .wy-form-full input[type=search],.wy-control-group .wy-form-full input[type=tel],.wy-control-group .wy-form-full input[type=text],.wy-control-group .wy-form-full input[type=time],.wy-control-group .wy-form-full input[type=url],.wy-control-group .wy-form-full input[type=week],.wy-control-group .wy-form-full select,.wy-control-group .wy-form-halves input[type=color],.wy-control-group .wy-form-halves input[type=date],.wy-control-group .wy-form-halves input[type=datetime-local],.wy-control-group .wy-form-halves input[type=datetime],.wy-control-group .wy-form-halves input[type=email],.wy-control-group .wy-form-halves input[type=month],.wy-control-group .wy-form-halves input[type=number],.wy-control-group .wy-form-halves input[type=password],.wy-control-group .wy-form-halves input[type=search],.wy-control-group .wy-form-halves input[type=tel],.wy-control-group .wy-form-halves input[type=text],.wy-control-group .wy-form-halves input[type=time],.wy-control-group .wy-form-halves input[type=url],.wy-control-group .wy-form-halves input[type=week],.wy-control-group .wy-form-halves select,.wy-control-group .wy-form-thirds input[type=color],.wy-control-group .wy-form-thirds input[type=date],.wy-control-group .wy-form-thirds input[type=datetime-local],.wy-control-group .wy-form-thirds input[type=datetime],.wy-control-group .wy-form-thirds input[type=email],.wy-control-group .wy-form-thirds input[type=month],.wy-control-group .wy-form-thirds input[type=number],.wy-control-group .wy-form-thirds input[type=password],.wy-control-group .wy-form-thirds input[type=search],.wy-control-group .wy-form-thirds input[type=tel],.wy-control-group .wy-form-thirds input[type=text],.wy-control-group .wy-form-thirds input[type=time],.wy-control-group .wy-form-thirds input[type=url],.wy-control-group .wy-form-thirds input[type=week],.wy-control-group .wy-form-thirds select{width:100%}.wy-control-group .wy-form-full{float:left;display:block;width:100%;margin-right:0}.wy-control-group .wy-form-full:last-child{margin-right:0}.wy-control-group .wy-form-halves{float:left;display:block;margin-right:2.35765%;width:48.82117%}.wy-control-group .wy-form-halves:last-child,.wy-control-group .wy-form-halves:nth-of-type(2n){margin-right:0}.wy-control-group .wy-form-halves:nth-of-type(odd){clear:left}.wy-control-group .wy-form-thirds{float:left;display:block;margin-right:2.35765%;width:31.76157%}.wy-control-group .wy-form-thirds:last-child,.wy-control-group .wy-form-thirds:nth-of-type(3n){margin-right:0}.wy-control-group .wy-form-thirds:nth-of-type(3n+1){clear:left}.wy-control-group.wy-control-group-no-input .wy-control,.wy-control-no-input{margin:6px 0 0;font-size:90%}.wy-control-no-input{display:inline-block}.wy-control-group.fluid-input input[type=color],.wy-control-group.fluid-input input[type=date],.wy-control-group.fluid-input input[type=datetime-local],.wy-control-group.fluid-input input[type=datetime],.wy-control-group.fluid-input input[type=email],.wy-control-group.fluid-input input[type=month],.wy-control-group.fluid-input input[type=number],.wy-control-group.fluid-input input[type=password],.wy-control-group.fluid-input input[type=search],.wy-control-group.fluid-input input[type=tel],.wy-control-group.fluid-input input[type=text],.wy-control-group.fluid-input input[type=time],.wy-control-group.fluid-input input[type=url],.wy-control-group.fluid-input input[type=week]{width:100%}.wy-form-message-inline{padding-left:.3em;color:#666;font-size:90%}.wy-form-message{display:block;color:#999;font-size:70%;margin-top:.3125em;font-style:italic}.wy-form-message p{font-size:inherit;font-style:italic;margin-bottom:6px}.wy-form-message p:last-child{margin-bottom:0}input{line-height:normal}input[type=button],input[type=reset],input[type=submit]{-webkit-appearance:button;cursor:pointer;font-family:Lato,proxima-nova,Helvetica Neue,Arial,sans-serif;*overflow:visible}input[type=color],input[type=date],input[type=datetime-local],input[type=datetime],input[type=email],input[type=month],input[type=number],input[type=password],input[type=search],input[type=tel],input[type=text],input[type=time],input[type=url],input[type=week]{-webkit-appearance:none;padding:6px;display:inline-block;border:1px solid #ccc;font-size:80%;font-family:Lato,proxima-nova,Helvetica Neue,Arial,sans-serif;box-shadow:inset 0 1px 3px #ddd;border-radius:0;-webkit-transition:border .3s linear;-moz-transition:border .3s linear;transition:border .3s linear}input[type=datetime-local]{padding:.34375em .625em}input[disabled]{cursor:default}input[type=checkbox],input[type=radio]{padding:0;margin-right:.3125em;*height:13px;*width:13px}input[type=checkbox],input[type=radio],input[type=search]{-webkit-box-sizing:border-box;-moz-box-sizing:border-box;box-sizing:border-box}input[type=search]::-webkit-search-cancel-button,input[type=search]::-webkit-search-decoration{-webkit-appearance:none}input[type=color]:focus,input[type=date]:focus,input[type=datetime-local]:focus,input[type=datetime]:focus,input[type=email]:focus,input[type=month]:focus,input[type=number]:focus,input[type=password]:focus,input[type=search]:focus,input[type=tel]:focus,input[type=text]:focus,input[type=time]:focus,input[type=url]:focus,input[type=week]:focus{outline:0;outline:thin dotted\9;border-color:#333}input.no-focus:focus{border-color:#ccc!important}input[type=checkbox]:focus,input[type=file]:focus,input[type=radio]:focus{outline:thin dotted #333;outline:1px auto #129fea}input[type=color][disabled],input[type=date][disabled],input[type=datetime-local][disabled],input[type=datetime][disabled],input[type=email][disabled],input[type=month][disabled],input[type=number][disabled],input[type=password][disabled],input[type=search][disabled],input[type=tel][disabled],input[type=text][disabled],input[type=time][disabled],input[type=url][disabled],input[type=week][disabled]{cursor:not-allowed;background-color:#fafafa}input:focus:invalid,select:focus:invalid,textarea:focus:invalid{color:#e74c3c;border:1px solid #e74c3c}input:focus:invalid:focus,select:focus:invalid:focus,textarea:focus:invalid:focus{border-color:#e74c3c}input[type=checkbox]:focus:invalid:focus,input[type=file]:focus:invalid:focus,input[type=radio]:focus:invalid:focus{outline-color:#e74c3c}input.wy-input-large{padding:12px;font-size:100%}textarea{overflow:auto;vertical-align:top;width:100%;font-family:Lato,proxima-nova,Helvetica Neue,Arial,sans-serif}select,textarea{padding:.5em .625em;display:inline-block;border:1px solid #ccc;font-size:80%;box-shadow:inset 0 1px 3px #ddd;-webkit-transition:border .3s linear;-moz-transition:border .3s linear;transition:border .3s linear}select{border:1px solid #ccc;background-color:#fff}select[multiple]{height:auto}select:focus,textarea:focus{outline:0}input[readonly],select[disabled],select[readonly],textarea[disabled],textarea[readonly]{cursor:not-allowed;background-color:#fafafa}input[type=checkbox][disabled],input[type=radio][disabled]{cursor:not-allowed}.wy-checkbox,.wy-radio{margin:6px 0;color:#404040;display:block}.wy-checkbox input,.wy-radio input{vertical-align:baseline}.wy-form-message-inline{display:inline-block;*display:inline;*zoom:1;vertical-align:middle}.wy-input-prefix,.wy-input-suffix{white-space:nowrap;padding:6px}.wy-input-prefix .wy-input-context,.wy-input-suffix .wy-input-context{line-height:27px;padding:0 8px;display:inline-block;font-size:80%;background-color:#f3f6f6;border:1px solid #ccc;color:#999}.wy-input-suffix .wy-input-context{border-left:0}.wy-input-prefix .wy-input-context{border-right:0}.wy-switch{position:relative;display:block;height:24px;margin-top:12px;cursor:pointer}.wy-switch:before{left:0;top:0;width:36px;height:12px;background:#ccc}.wy-switch:after,.wy-switch:before{position:absolute;content:"";display:block;border-radius:4px;-webkit-transition:all .2s ease-in-out;-moz-transition:all .2s ease-in-out;transition:all .2s ease-in-out}.wy-switch:after{width:18px;height:18px;background:#999;left:-3px;top:-3px}.wy-switch span{position:absolute;left:48px;display:block;font-size:12px;color:#ccc;line-height:1}.wy-switch.active:before{background:#1e8449}.wy-switch.active:after{left:24px;background:#27ae60}.wy-switch.disabled{cursor:not-allowed;opacity:.8}.wy-control-group.wy-control-group-error .wy-form-message,.wy-control-group.wy-control-group-error>label{color:#e74c3c}.wy-control-group.wy-control-group-error input[type=color],.wy-control-group.wy-control-group-error input[type=date],.wy-control-group.wy-control-group-error input[type=datetime-local],.wy-control-group.wy-control-group-error input[type=datetime],.wy-control-group.wy-control-group-error input[type=email],.wy-control-group.wy-control-group-error input[type=month],.wy-control-group.wy-control-group-error input[type=number],.wy-control-group.wy-control-group-error input[type=password],.wy-control-group.wy-control-group-error input[type=search],.wy-control-group.wy-control-group-error input[type=tel],.wy-control-group.wy-control-group-error input[type=text],.wy-control-group.wy-control-group-error input[type=time],.wy-control-group.wy-control-group-error input[type=url],.wy-control-group.wy-control-group-error input[type=week],.wy-control-group.wy-control-group-error textarea{border:1px solid #e74c3c}.wy-inline-validate{white-space:nowrap}.wy-inline-validate .wy-input-context{padding:.5em .625em;display:inline-block;font-size:80%}.wy-inline-validate.wy-inline-validate-success .wy-input-context{color:#27ae60}.wy-inline-validate.wy-inline-validate-danger .wy-input-context{color:#e74c3c}.wy-inline-validate.wy-inline-validate-warning .wy-input-context{color:#e67e22}.wy-inline-validate.wy-inline-validate-info .wy-input-context{color:#2980b9}.rotate-90{-webkit-transform:rotate(90deg);-moz-transform:rotate(90deg);-ms-transform:rotate(90deg);-o-transform:rotate(90deg);transform:rotate(90deg)}.rotate-180{-webkit-transform:rotate(180deg);-moz-transform:rotate(180deg);-ms-transform:rotate(180deg);-o-transform:rotate(180deg);transform:rotate(180deg)}.rotate-270{-webkit-transform:rotate(270deg);-moz-transform:rotate(270deg);-ms-transform:rotate(270deg);-o-transform:rotate(270deg);transform:rotate(270deg)}.mirror{-webkit-transform:scaleX(-1);-moz-transform:scaleX(-1);-ms-transform:scaleX(-1);-o-transform:scaleX(-1);transform:scaleX(-1)}.mirror.rotate-90{-webkit-transform:scaleX(-1) rotate(90deg);-moz-transform:scaleX(-1) rotate(90deg);-ms-transform:scaleX(-1) rotate(90deg);-o-transform:scaleX(-1) rotate(90deg);transform:scaleX(-1) rotate(90deg)}.mirror.rotate-180{-webkit-transform:scaleX(-1) rotate(180deg);-moz-transform:scaleX(-1) rotate(180deg);-ms-transform:scaleX(-1) rotate(180deg);-o-transform:scaleX(-1) rotate(180deg);transform:scaleX(-1) rotate(180deg)}.mirror.rotate-270{-webkit-transform:scaleX(-1) rotate(270deg);-moz-transform:scaleX(-1) rotate(270deg);-ms-transform:scaleX(-1) rotate(270deg);-o-transform:scaleX(-1) rotate(270deg);transform:scaleX(-1) rotate(270deg)}@media only screen and (max-width:480px){.wy-form button[type=submit]{margin:.7em 0 0}.wy-form input[type=color],.wy-form input[type=date],.wy-form input[type=datetime-local],.wy-form input[type=datetime],.wy-form input[type=email],.wy-form input[type=month],.wy-form input[type=number],.wy-form input[type=password],.wy-form input[type=search],.wy-form input[type=tel],.wy-form input[type=text],.wy-form input[type=time],.wy-form input[type=url],.wy-form input[type=week],.wy-form label{margin-bottom:.3em;display:block}.wy-form input[type=color],.wy-form input[type=date],.wy-form input[type=datetime-local],.wy-form input[type=datetime],.wy-form input[type=email],.wy-form input[type=month],.wy-form input[type=number],.wy-form input[type=password],.wy-form input[type=search],.wy-form input[type=tel],.wy-form input[type=time],.wy-form input[type=url],.wy-form input[type=week]{margin-bottom:0}.wy-form-aligned .wy-control-group label{margin-bottom:.3em;text-align:left;display:block;width:100%}.wy-form-aligned .wy-control{margin:1.5em 0 0}.wy-form-message,.wy-form-message-inline,.wy-form .wy-help-inline{display:block;font-size:80%;padding:6px 0}}@media screen and (max-width:768px){.tablet-hide{display:none}}@media screen and (max-width:480px){.mobile-hide{display:none}}.float-left{float:left}.float-right{float:right}.full-width{width:100%}.rst-content table.docutils,.rst-content table.field-list,.wy-table{border-collapse:collapse;border-spacing:0;empty-cells:show;margin-bottom:24px}.rst-content table.docutils caption,.rst-content table.field-list caption,.wy-table caption{color:#000;font:italic 85%/1 arial,sans-serif;padding:1em 0;text-align:center}.rst-content table.docutils td,.rst-content table.docutils th,.rst-content table.field-list td,.rst-content table.field-list th,.wy-table td,.wy-table th{font-size:90%;margin:0;overflow:visible;padding:8px 16px}.rst-content table.docutils td:first-child,.rst-content table.docutils th:first-child,.rst-content table.field-list td:first-child,.rst-content table.field-list th:first-child,.wy-table td:first-child,.wy-table th:first-child{border-left-width:0}.rst-content table.docutils thead,.rst-content table.field-list thead,.wy-table thead{color:#000;text-align:left;vertical-align:bottom;white-space:nowrap}.rst-content table.docutils thead th,.rst-content table.field-list thead th,.wy-table thead th{font-weight:700;border-bottom:2px solid #e1e4e5}.rst-content table.docutils td,.rst-content table.field-list td,.wy-table td{background-color:transparent;vertical-align:middle}.rst-content table.docutils td p,.rst-content table.field-list td p,.wy-table td p{line-height:18px}.rst-content table.docutils td p:last-child,.rst-content table.field-list td p:last-child,.wy-table td p:last-child{margin-bottom:0}.rst-content table.docutils .wy-table-cell-min,.rst-content table.field-list .wy-table-cell-min,.wy-table .wy-table-cell-min{width:1%;padding-right:0}.rst-content table.docutils .wy-table-cell-min input[type=checkbox],.rst-content table.field-list .wy-table-cell-min input[type=checkbox],.wy-table .wy-table-cell-min input[type=checkbox]{margin:0}.wy-table-secondary{color:grey;font-size:90%}.wy-table-tertiary{color:grey;font-size:80%}.rst-content table.docutils:not(.field-list) tr:nth-child(2n-1) td,.wy-table-backed,.wy-table-odd td,.wy-table-striped tr:nth-child(2n-1) td{background-color:#f3f6f6}.rst-content table.docutils,.wy-table-bordered-all{border:1px solid #e1e4e5}.rst-content table.docutils td,.wy-table-bordered-all td{border-bottom:1px solid #e1e4e5;border-left:1px solid #e1e4e5}.rst-content table.docutils tbody>tr:last-child td,.wy-table-bordered-all tbody>tr:last-child td{border-bottom-width:0}.wy-table-bordered{border:1px solid #e1e4e5}.wy-table-bordered-rows td{border-bottom:1px solid #e1e4e5}.wy-table-bordered-rows tbody>tr:last-child td{border-bottom-width:0}.wy-table-horizontal td,.wy-table-horizontal th{border-width:0 0 1px;border-bottom:1px solid #e1e4e5}.wy-table-horizontal tbody>tr:last-child td{border-bottom-width:0}.wy-table-responsive{margin-bottom:24px;max-width:100%;overflow:auto}.wy-table-responsive table{margin-bottom:0!important}.wy-table-responsive table td,.wy-table-responsive table th{white-space:nowrap}a{color:#2980b9;text-decoration:none;cursor:pointer}a:hover{color:#3091d1}a:visited{color:#9b59b6}html{height:100%}body,html{overflow-x:hidden}body{font-family:Lato,proxima-nova,Helvetica Neue,Arial,sans-serif;font-weight:400;color:#404040;min-height:100%;background:#edf0f2}.wy-text-left{text-align:left}.wy-text-center{text-align:center}.wy-text-right{text-align:right}.wy-text-large{font-size:120%}.wy-text-normal{font-size:100%}.wy-text-small,small{font-size:80%}.wy-text-strike{text-decoration:line-through}.wy-text-warning{color:#e67e22!important}a.wy-text-warning:hover{color:#eb9950!important}.wy-text-info{color:#2980b9!important}a.wy-text-info:hover{color:#409ad5!important}.wy-text-success{color:#27ae60!important}a.wy-text-success:hover{color:#36d278!important}.wy-text-danger{color:#e74c3c!important}a.wy-text-danger:hover{color:#ed7669!important}.wy-text-neutral{color:#404040!important}a.wy-text-neutral:hover{color:#595959!important}.rst-content .toctree-wrapper>p.caption,h1,h2,h3,h4,h5,h6,legend{margin-top:0;font-weight:700;font-family:Roboto Slab,ff-tisa-web-pro,Georgia,Arial,sans-serif}p{line-height:24px;font-size:16px;margin:0 0 24px}h1{font-size:175%}.rst-content .toctree-wrapper>p.caption,h2{font-size:150%}h3{font-size:125%}h4{font-size:115%}h5{font-size:110%}h6{font-size:100%}hr{display:block;height:1px;border:0;border-top:1px solid #e1e4e5;margin:24px 0;padding:0}.rst-content code,.rst-content tt,code{white-space:nowrap;max-width:100%;background:#fff;border:1px solid #e1e4e5;font-size:75%;padding:0 5px;font-family:SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,Courier,monospace;color:#e74c3c;overflow-x:auto}.rst-content tt.code-large,code.code-large{font-size:90%}.rst-content .section ul,.rst-content .toctree-wrapper ul,.rst-content section ul,.wy-plain-list-disc,article ul{list-style:disc;line-height:24px;margin-bottom:24px}.rst-content .section ul li,.rst-content .toctree-wrapper ul li,.rst-content section ul li,.wy-plain-list-disc li,article ul li{list-style:disc;margin-left:24px}.rst-content .section ul li p:last-child,.rst-content .section ul li ul,.rst-content .toctree-wrapper ul li p:last-child,.rst-content .toctree-wrapper ul li ul,.rst-content section ul li p:last-child,.rst-content section ul li ul,.wy-plain-list-disc li p:last-child,.wy-plain-list-disc li ul,article ul li p:last-child,article ul li ul{margin-bottom:0}.rst-content .section ul li li,.rst-content .toctree-wrapper ul li li,.rst-content section ul li li,.wy-plain-list-disc li li,article ul li li{list-style:circle}.rst-content .section ul li li li,.rst-content .toctree-wrapper ul li li li,.rst-content section ul li li li,.wy-plain-list-disc li li li,article ul li li li{list-style:square}.rst-content .section ul li ol li,.rst-content .toctree-wrapper ul li ol li,.rst-content section ul li ol li,.wy-plain-list-disc li ol li,article ul li ol li{list-style:decimal}.rst-content .section ol,.rst-content .section ol.arabic,.rst-content .toctree-wrapper ol,.rst-content .toctree-wrapper ol.arabic,.rst-content section ol,.rst-content section ol.arabic,.wy-plain-list-decimal,article ol{list-style:decimal;line-height:24px;margin-bottom:24px}.rst-content .section ol.arabic li,.rst-content .section ol li,.rst-content .toctree-wrapper ol.arabic li,.rst-content .toctree-wrapper ol li,.rst-content section ol.arabic li,.rst-content section ol li,.wy-plain-list-decimal li,article ol li{list-style:decimal;margin-left:24px}.rst-content .section ol.arabic li ul,.rst-content .section ol li p:last-child,.rst-content .section ol li ul,.rst-content .toctree-wrapper ol.arabic li ul,.rst-content .toctree-wrapper ol li p:last-child,.rst-content .toctree-wrapper ol li ul,.rst-content section ol.arabic li ul,.rst-content section ol li p:last-child,.rst-content section ol li ul,.wy-plain-list-decimal li p:last-child,.wy-plain-list-decimal li ul,article ol li p:last-child,article ol li ul{margin-bottom:0}.rst-content .section ol.arabic li ul li,.rst-content .section ol li ul li,.rst-content .toctree-wrapper ol.arabic li ul li,.rst-content .toctree-wrapper ol li ul li,.rst-content section ol.arabic li ul li,.rst-content section ol li ul li,.wy-plain-list-decimal li ul li,article ol li ul li{list-style:disc}.wy-breadcrumbs{*zoom:1}.wy-breadcrumbs:after,.wy-breadcrumbs:before{display:table;content:""}.wy-breadcrumbs:after{clear:both}.wy-breadcrumbs li{display:inline-block}.wy-breadcrumbs li.wy-breadcrumbs-aside{float:right}.wy-breadcrumbs li a{display:inline-block;padding:5px}.wy-breadcrumbs li a:first-child{padding-left:0}.rst-content .wy-breadcrumbs li tt,.wy-breadcrumbs li .rst-content tt,.wy-breadcrumbs li code{padding:5px;border:none;background:none}.rst-content .wy-breadcrumbs li tt.literal,.wy-breadcrumbs li .rst-content tt.literal,.wy-breadcrumbs li code.literal{color:#404040}.wy-breadcrumbs-extra{margin-bottom:0;color:#b3b3b3;font-size:80%;display:inline-block}@media screen and (max-width:480px){.wy-breadcrumbs-extra,.wy-breadcrumbs li.wy-breadcrumbs-aside{display:none}}@media print{.wy-breadcrumbs li.wy-breadcrumbs-aside{display:none}}html{font-size:16px}.wy-affix{position:fixed;top:1.618em}.wy-menu a:hover{text-decoration:none}.wy-menu-horiz{*zoom:1}.wy-menu-horiz:after,.wy-menu-horiz:before{display:table;content:""}.wy-menu-horiz:after{clear:both}.wy-menu-horiz li,.wy-menu-horiz ul{display:inline-block}.wy-menu-horiz li:hover{background:hsla(0,0%,100%,.1)}.wy-menu-horiz li.divide-left{border-left:1px solid #404040}.wy-menu-horiz li.divide-right{border-right:1px solid #404040}.wy-menu-horiz a{height:32px;display:inline-block;line-height:32px;padding:0 16px}.wy-menu-vertical{width:300px}.wy-menu-vertical header,.wy-menu-vertical p.caption{color:#55a5d9;height:32px;line-height:32px;padding:0 1.618em;margin:12px 0 0;display:block;font-weight:700;text-transform:uppercase;font-size:85%;white-space:nowrap}.wy-menu-vertical ul{margin-bottom:0}.wy-menu-vertical li.divide-top{border-top:1px solid #404040}.wy-menu-vertical li.divide-bottom{border-bottom:1px solid #404040}.wy-menu-vertical li.current{background:#e3e3e3}.wy-menu-vertical li.current a{color:grey;border-right:1px solid #c9c9c9;padding:.4045em 2.427em}.wy-menu-vertical li.current a:hover{background:#d6d6d6}.rst-content .wy-menu-vertical li tt,.wy-menu-vertical li .rst-content tt,.wy-menu-vertical li code{border:none;background:inherit;color:inherit;padding-left:0;padding-right:0}.wy-menu-vertical li button.toctree-expand{display:block;float:left;margin-left:-1.2em;line-height:18px;color:#4d4d4d;border:none;background:none;padding:0}.wy-menu-vertical li.current>a,.wy-menu-vertical li.on a{color:#404040;font-weight:700;position:relative;background:#fcfcfc;border:none;padding:.4045em 1.618em}.wy-menu-vertical li.current>a:hover,.wy-menu-vertical li.on a:hover{background:#fcfcfc}.wy-menu-vertical li.current>a:hover button.toctree-expand,.wy-menu-vertical li.on a:hover button.toctree-expand{color:grey}.wy-menu-vertical li.current>a button.toctree-expand,.wy-menu-vertical li.on a button.toctree-expand{display:block;line-height:18px;color:#333}.wy-menu-vertical li.toctree-l1.current>a{border-bottom:1px solid #c9c9c9;border-top:1px solid #c9c9c9}.wy-menu-vertical .toctree-l1.current .toctree-l2>ul,.wy-menu-vertical .toctree-l2.current .toctree-l3>ul,.wy-menu-vertical .toctree-l3.current .toctree-l4>ul,.wy-menu-vertical .toctree-l4.current .toctree-l5>ul,.wy-menu-vertical .toctree-l5.current .toctree-l6>ul,.wy-menu-vertical .toctree-l6.current .toctree-l7>ul,.wy-menu-vertical .toctree-l7.current .toctree-l8>ul,.wy-menu-vertical .toctree-l8.current .toctree-l9>ul,.wy-menu-vertical .toctree-l9.current .toctree-l10>ul,.wy-menu-vertical .toctree-l10.current .toctree-l11>ul{display:none}.wy-menu-vertical .toctree-l1.current .current.toctree-l2>ul,.wy-menu-vertical .toctree-l2.current .current.toctree-l3>ul,.wy-menu-vertical .toctree-l3.current .current.toctree-l4>ul,.wy-menu-vertical .toctree-l4.current .current.toctree-l5>ul,.wy-menu-vertical .toctree-l5.current .current.toctree-l6>ul,.wy-menu-vertical .toctree-l6.current .current.toctree-l7>ul,.wy-menu-vertical .toctree-l7.current .current.toctree-l8>ul,.wy-menu-vertical .toctree-l8.current .current.toctree-l9>ul,.wy-menu-vertical .toctree-l9.current .current.toctree-l10>ul,.wy-menu-vertical .toctree-l10.current .current.toctree-l11>ul{display:block}.wy-menu-vertical li.toctree-l3,.wy-menu-vertical li.toctree-l4{font-size:.9em}.wy-menu-vertical li.toctree-l2 a,.wy-menu-vertical li.toctree-l3 a,.wy-menu-vertical li.toctree-l4 a,.wy-menu-vertical li.toctree-l5 a,.wy-menu-vertical li.toctree-l6 a,.wy-menu-vertical li.toctree-l7 a,.wy-menu-vertical li.toctree-l8 a,.wy-menu-vertical li.toctree-l9 a,.wy-menu-vertical li.toctree-l10 a{color:#404040}.wy-menu-vertical li.toctree-l2 a:hover button.toctree-expand,.wy-menu-vertical li.toctree-l3 a:hover button.toctree-expand,.wy-menu-vertical li.toctree-l4 a:hover button.toctree-expand,.wy-menu-vertical li.toctree-l5 a:hover button.toctree-expand,.wy-menu-vertical li.toctree-l6 a:hover button.toctree-expand,.wy-menu-vertical li.toctree-l7 a:hover button.toctree-expand,.wy-menu-vertical li.toctree-l8 a:hover button.toctree-expand,.wy-menu-vertical li.toctree-l9 a:hover button.toctree-expand,.wy-menu-vertical li.toctree-l10 a:hover button.toctree-expand{color:grey}.wy-menu-vertical li.toctree-l2.current li.toctree-l3>a,.wy-menu-vertical li.toctree-l3.current li.toctree-l4>a,.wy-menu-vertical li.toctree-l4.current li.toctree-l5>a,.wy-menu-vertical li.toctree-l5.current li.toctree-l6>a,.wy-menu-vertical li.toctree-l6.current li.toctree-l7>a,.wy-menu-vertical li.toctree-l7.current li.toctree-l8>a,.wy-menu-vertical li.toctree-l8.current li.toctree-l9>a,.wy-menu-vertical li.toctree-l9.current li.toctree-l10>a,.wy-menu-vertical li.toctree-l10.current li.toctree-l11>a{display:block}.wy-menu-vertical li.toctree-l2.current>a{padding:.4045em 2.427em}.wy-menu-vertical li.toctree-l2.current li.toctree-l3>a{padding:.4045em 1.618em .4045em 4.045em}.wy-menu-vertical li.toctree-l3.current>a{padding:.4045em 4.045em}.wy-menu-vertical li.toctree-l3.current li.toctree-l4>a{padding:.4045em 1.618em .4045em 5.663em}.wy-menu-vertical li.toctree-l4.current>a{padding:.4045em 5.663em}.wy-menu-vertical li.toctree-l4.current li.toctree-l5>a{padding:.4045em 1.618em .4045em 7.281em}.wy-menu-vertical li.toctree-l5.current>a{padding:.4045em 7.281em}.wy-menu-vertical li.toctree-l5.current li.toctree-l6>a{padding:.4045em 1.618em .4045em 8.899em}.wy-menu-vertical li.toctree-l6.current>a{padding:.4045em 8.899em}.wy-menu-vertical li.toctree-l6.current li.toctree-l7>a{padding:.4045em 1.618em .4045em 10.517em}.wy-menu-vertical li.toctree-l7.current>a{padding:.4045em 10.517em}.wy-menu-vertical li.toctree-l7.current li.toctree-l8>a{padding:.4045em 1.618em .4045em 12.135em}.wy-menu-vertical li.toctree-l8.current>a{padding:.4045em 12.135em}.wy-menu-vertical li.toctree-l8.current li.toctree-l9>a{padding:.4045em 1.618em .4045em 13.753em}.wy-menu-vertical li.toctree-l9.current>a{padding:.4045em 13.753em}.wy-menu-vertical li.toctree-l9.current li.toctree-l10>a{padding:.4045em 1.618em .4045em 15.371em}.wy-menu-vertical li.toctree-l10.current>a{padding:.4045em 15.371em}.wy-menu-vertical li.toctree-l10.current li.toctree-l11>a{padding:.4045em 1.618em .4045em 16.989em}.wy-menu-vertical li.toctree-l2.current>a,.wy-menu-vertical li.toctree-l2.current li.toctree-l3>a{background:#c9c9c9}.wy-menu-vertical li.toctree-l2 button.toctree-expand{color:#a3a3a3}.wy-menu-vertical li.toctree-l3.current>a,.wy-menu-vertical li.toctree-l3.current li.toctree-l4>a{background:#bdbdbd}.wy-menu-vertical li.toctree-l3 button.toctree-expand{color:#969696}.wy-menu-vertical li.current ul{display:block}.wy-menu-vertical li ul{margin-bottom:0;display:none}.wy-menu-vertical li ul li a{margin-bottom:0;color:#d9d9d9;font-weight:400}.wy-menu-vertical a{line-height:18px;padding:.4045em 1.618em;display:block;position:relative;font-size:90%;color:#d9d9d9}.wy-menu-vertical a:hover{background-color:#4e4a4a;cursor:pointer}.wy-menu-vertical a:hover button.toctree-expand{color:#d9d9d9}.wy-menu-vertical a:active{background-color:#2980b9;cursor:pointer;color:#fff}.wy-menu-vertical a:active button.toctree-expand{color:#fff}.wy-side-nav-search{display:block;width:300px;padding:.809em;margin-bottom:.809em;z-index:200;background-color:#2980b9;text-align:center;color:#fcfcfc}.wy-side-nav-search input[type=text]{width:100%;border-radius:50px;padding:6px 12px;border-color:#2472a4}.wy-side-nav-search img{display:block;margin:auto auto .809em;height:45px;width:45px;background-color:#2980b9;padding:5px;border-radius:100%}.wy-side-nav-search .wy-dropdown>a,.wy-side-nav-search>a{color:#fcfcfc;font-size:100%;font-weight:700;display:inline-block;padding:4px 6px;margin-bottom:.809em;max-width:100%}.wy-side-nav-search .wy-dropdown>a:hover,.wy-side-nav-search>a:hover{background:hsla(0,0%,100%,.1)}.wy-side-nav-search .wy-dropdown>a img.logo,.wy-side-nav-search>a img.logo{display:block;margin:0 auto;height:auto;width:auto;border-radius:0;max-width:100%;background:transparent}.wy-side-nav-search .wy-dropdown>a.icon img.logo,.wy-side-nav-search>a.icon img.logo{margin-top:.85em}.wy-side-nav-search>div.version{margin-top:-.4045em;margin-bottom:.809em;font-weight:400;color:hsla(0,0%,100%,.3)}.wy-nav .wy-menu-vertical header{color:#2980b9}.wy-nav .wy-menu-vertical a{color:#b3b3b3}.wy-nav .wy-menu-vertical a:hover{background-color:#2980b9;color:#fff}[data-menu-wrap]{-webkit-transition:all .2s ease-in;-moz-transition:all .2s ease-in;transition:all .2s ease-in;position:absolute;opacity:1;width:100%;opacity:0}[data-menu-wrap].move-center{left:0;right:auto;opacity:1}[data-menu-wrap].move-left{right:auto;left:-100%;opacity:0}[data-menu-wrap].move-right{right:-100%;left:auto;opacity:0}.wy-body-for-nav{background:#fcfcfc}.wy-grid-for-nav{position:absolute;width:100%;height:100%}.wy-nav-side{position:fixed;top:0;bottom:0;left:0;padding-bottom:2em;width:300px;overflow-x:hidden;overflow-y:hidden;min-height:100%;color:#9b9b9b;background:#343131;z-index:200}.wy-side-scroll{width:320px;position:relative;overflow-x:hidden;overflow-y:scroll;height:100%}.wy-nav-top{display:none;background:#2980b9;color:#fff;padding:.4045em .809em;position:relative;line-height:50px;text-align:center;font-size:100%;*zoom:1}.wy-nav-top:after,.wy-nav-top:before{display:table;content:""}.wy-nav-top:after{clear:both}.wy-nav-top a{color:#fff;font-weight:700}.wy-nav-top img{margin-right:12px;height:45px;width:45px;background-color:#2980b9;padding:5px;border-radius:100%}.wy-nav-top i{font-size:30px;float:left;cursor:pointer;padding-top:inherit}.wy-nav-content-wrap{margin-left:300px;background:#fcfcfc;min-height:100%}.wy-nav-content{padding:1.618em 3.236em;height:100%;max-width:800px;margin:auto}.wy-body-mask{position:fixed;width:100%;height:100%;background:rgba(0,0,0,.2);display:none;z-index:499}.wy-body-mask.on{display:block}footer{color:grey}footer p{margin-bottom:12px}.rst-content footer span.commit tt,footer span.commit .rst-content tt,footer span.commit code{padding:0;font-family:SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,Courier,monospace;font-size:1em;background:none;border:none;color:grey}.rst-footer-buttons{*zoom:1}.rst-footer-buttons:after,.rst-footer-buttons:before{width:100%;display:table;content:""}.rst-footer-buttons:after{clear:both}.rst-breadcrumbs-buttons{margin-top:12px;*zoom:1}.rst-breadcrumbs-buttons:after,.rst-breadcrumbs-buttons:before{display:table;content:""}.rst-breadcrumbs-buttons:after{clear:both}#search-results .search li{margin-bottom:24px;border-bottom:1px solid #e1e4e5;padding-bottom:24px}#search-results .search li:first-child{border-top:1px solid #e1e4e5;padding-top:24px}#search-results .search li a{font-size:120%;margin-bottom:12px;display:inline-block}#search-results .context{color:grey;font-size:90%}.genindextable li>ul{margin-left:24px}@media screen and (max-width:768px){.wy-body-for-nav{background:#fcfcfc}.wy-nav-top{display:block}.wy-nav-side{left:-300px}.wy-nav-side.shift{width:85%;left:0}.wy-menu.wy-menu-vertical,.wy-side-nav-search,.wy-side-scroll{width:auto}.wy-nav-content-wrap{margin-left:0}.wy-nav-content-wrap .wy-nav-content{padding:1.618em}.wy-nav-content-wrap.shift{position:fixed;min-width:100%;left:85%;top:0;height:100%;overflow:hidden}}@media screen and (min-width:1100px){.wy-nav-content-wrap{background:rgba(0,0,0,.05)}.wy-nav-content{margin:0;background:#fcfcfc}}@media print{.rst-versions,.wy-nav-side,footer{display:none}.wy-nav-content-wrap{margin-left:0}}.rst-versions{position:fixed;bottom:0;left:0;width:300px;color:#fcfcfc;background:#1f1d1d;font-family:Lato,proxima-nova,Helvetica Neue,Arial,sans-serif;z-index:400}.rst-versions a{color:#2980b9;text-decoration:none}.rst-versions .rst-badge-small{display:none}.rst-versions .rst-current-version{padding:12px;background-color:#272525;display:block;text-align:right;font-size:90%;cursor:pointer;color:#27ae60;*zoom:1}.rst-versions .rst-current-version:after,.rst-versions .rst-current-version:before{display:table;content:""}.rst-versions .rst-current-version:after{clear:both}.rst-content .code-block-caption .rst-versions .rst-current-version .headerlink,.rst-content .eqno .rst-versions .rst-current-version .headerlink,.rst-content .rst-versions .rst-current-version .admonition-title,.rst-content code.download .rst-versions .rst-current-version span:first-child,.rst-content dl dt .rst-versions .rst-current-version .headerlink,.rst-content h1 .rst-versions .rst-current-version .headerlink,.rst-content h2 .rst-versions .rst-current-version .headerlink,.rst-content h3 .rst-versions .rst-current-version .headerlink,.rst-content h4 .rst-versions .rst-current-version .headerlink,.rst-content h5 .rst-versions .rst-current-version .headerlink,.rst-content h6 .rst-versions .rst-current-version .headerlink,.rst-content p .rst-versions .rst-current-version .headerlink,.rst-content table>caption .rst-versions .rst-current-version .headerlink,.rst-content tt.download .rst-versions .rst-current-version span:first-child,.rst-versions .rst-current-version .fa,.rst-versions .rst-current-version .icon,.rst-versions .rst-current-version .rst-content .admonition-title,.rst-versions .rst-current-version .rst-content .code-block-caption .headerlink,.rst-versions .rst-current-version .rst-content .eqno .headerlink,.rst-versions .rst-current-version .rst-content code.download span:first-child,.rst-versions .rst-current-version .rst-content dl dt .headerlink,.rst-versions .rst-current-version .rst-content h1 .headerlink,.rst-versions .rst-current-version .rst-content h2 .headerlink,.rst-versions .rst-current-version .rst-content h3 .headerlink,.rst-versions .rst-current-version .rst-content h4 .headerlink,.rst-versions .rst-current-version .rst-content h5 .headerlink,.rst-versions .rst-current-version .rst-content h6 .headerlink,.rst-versions .rst-current-version .rst-content p .headerlink,.rst-versions .rst-current-version .rst-content table>caption .headerlink,.rst-versions .rst-current-version .rst-content tt.download span:first-child,.rst-versions .rst-current-version .wy-menu-vertical li button.toctree-expand,.wy-menu-vertical li .rst-versions .rst-current-version button.toctree-expand{color:#fcfcfc}.rst-versions .rst-current-version .fa-book,.rst-versions .rst-current-version .icon-book{float:left}.rst-versions .rst-current-version.rst-out-of-date{background-color:#e74c3c;color:#fff}.rst-versions .rst-current-version.rst-active-old-version{background-color:#f1c40f;color:#000}.rst-versions.shift-up{height:auto;max-height:100%;overflow-y:scroll}.rst-versions.shift-up .rst-other-versions{display:block}.rst-versions .rst-other-versions{font-size:90%;padding:12px;color:grey;display:none}.rst-versions .rst-other-versions hr{display:block;height:1px;border:0;margin:20px 0;padding:0;border-top:1px solid #413d3d}.rst-versions .rst-other-versions dd{display:inline-block;margin:0}.rst-versions .rst-other-versions dd a{display:inline-block;padding:6px;color:#fcfcfc}.rst-versions.rst-badge{width:auto;bottom:20px;right:20px;left:auto;border:none;max-width:300px;max-height:90%}.rst-versions.rst-badge .fa-book,.rst-versions.rst-badge .icon-book{float:none;line-height:30px}.rst-versions.rst-badge.shift-up .rst-current-version{text-align:right}.rst-versions.rst-badge.shift-up .rst-current-version .fa-book,.rst-versions.rst-badge.shift-up .rst-current-version .icon-book{float:left}.rst-versions.rst-badge>.rst-current-version{width:auto;height:30px;line-height:30px;padding:0 6px;display:block;text-align:center}@media screen and (max-width:768px){.rst-versions{width:85%;display:none}.rst-versions.shift{display:block}}.rst-content .toctree-wrapper>p.caption,.rst-content h1,.rst-content h2,.rst-content h3,.rst-content h4,.rst-content h5,.rst-content h6{margin-bottom:24px}.rst-content img{max-width:100%;height:auto}.rst-content div.figure,.rst-content figure{margin-bottom:24px}.rst-content div.figure .caption-text,.rst-content figure .caption-text{font-style:italic}.rst-content div.figure p:last-child.caption,.rst-content figure p:last-child.caption{margin-bottom:0}.rst-content div.figure.align-center,.rst-content figure.align-center{text-align:center}.rst-content .section>a>img,.rst-content .section>img,.rst-content section>a>img,.rst-content section>img{margin-bottom:24px}.rst-content abbr[title]{text-decoration:none}.rst-content.style-external-links a.reference.external:after{font-family:FontAwesome;content:"\f08e";color:#b3b3b3;vertical-align:super;font-size:60%;margin:0 .2em}.rst-content blockquote{margin-left:24px;line-height:24px;margin-bottom:24px}.rst-content pre.literal-block{white-space:pre;margin:0;padding:12px;font-family:SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,Courier,monospace;display:block;overflow:auto}.rst-content div[class^=highlight],.rst-content pre.literal-block{border:1px solid #e1e4e5;overflow-x:auto;margin:1px 0 24px}.rst-content div[class^=highlight] div[class^=highlight],.rst-content pre.literal-block div[class^=highlight]{padding:0;border:none;margin:0}.rst-content div[class^=highlight] td.code{width:100%}.rst-content .linenodiv pre{border-right:1px solid #e6e9ea;margin:0;padding:12px;font-family:SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,Courier,monospace;user-select:none;pointer-events:none}.rst-content div[class^=highlight] pre{white-space:pre;margin:0;padding:12px;display:block;overflow:auto}.rst-content div[class^=highlight] pre .hll{display:block;margin:0 -12px;padding:0 12px}.rst-content .linenodiv pre,.rst-content div[class^=highlight] pre,.rst-content pre.literal-block{font-family:SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,Courier,monospace;font-size:12px;line-height:1.4}.rst-content div.highlight .gp,.rst-content div.highlight span.linenos{user-select:none;pointer-events:none}.rst-content div.highlight span.linenos{display:inline-block;padding-left:0;padding-right:12px;margin-right:12px;border-right:1px solid #e6e9ea}.rst-content .code-block-caption{font-style:italic;font-size:85%;line-height:1;padding:1em 0;text-align:center}@media print{.rst-content .codeblock,.rst-content div[class^=highlight],.rst-content div[class^=highlight] pre{white-space:pre-wrap}}.rst-content .admonition,.rst-content .admonition-todo,.rst-content .attention,.rst-content .caution,.rst-content .danger,.rst-content .error,.rst-content .hint,.rst-content .important,.rst-content .note,.rst-content .seealso,.rst-content .tip,.rst-content .warning{clear:both}.rst-content .admonition-todo .last,.rst-content .admonition-todo>:last-child,.rst-content .admonition .last,.rst-content .admonition>:last-child,.rst-content .attention .last,.rst-content .attention>:last-child,.rst-content .caution .last,.rst-content .caution>:last-child,.rst-content .danger .last,.rst-content .danger>:last-child,.rst-content .error .last,.rst-content .error>:last-child,.rst-content .hint .last,.rst-content .hint>:last-child,.rst-content .important .last,.rst-content .important>:last-child,.rst-content .note .last,.rst-content .note>:last-child,.rst-content .seealso .last,.rst-content .seealso>:last-child,.rst-content .tip .last,.rst-content .tip>:last-child,.rst-content .warning .last,.rst-content .warning>:last-child{margin-bottom:0}.rst-content .admonition-title:before{margin-right:4px}.rst-content .admonition table{border-color:rgba(0,0,0,.1)}.rst-content .admonition table td,.rst-content .admonition table th{background:transparent!important;border-color:rgba(0,0,0,.1)!important}.rst-content .section ol.loweralpha,.rst-content .section ol.loweralpha>li,.rst-content .toctree-wrapper ol.loweralpha,.rst-content .toctree-wrapper ol.loweralpha>li,.rst-content section ol.loweralpha,.rst-content section ol.loweralpha>li{list-style:lower-alpha}.rst-content .section ol.upperalpha,.rst-content .section ol.upperalpha>li,.rst-content .toctree-wrapper ol.upperalpha,.rst-content .toctree-wrapper ol.upperalpha>li,.rst-content section ol.upperalpha,.rst-content section ol.upperalpha>li{list-style:upper-alpha}.rst-content .section ol li>*,.rst-content .section ul li>*,.rst-content .toctree-wrapper ol li>*,.rst-content .toctree-wrapper ul li>*,.rst-content section ol li>*,.rst-content section ul li>*{margin-top:12px;margin-bottom:12px}.rst-content .section ol li>:first-child,.rst-content .section ul li>:first-child,.rst-content .toctree-wrapper ol li>:first-child,.rst-content .toctree-wrapper ul li>:first-child,.rst-content section ol li>:first-child,.rst-content section ul li>:first-child{margin-top:0}.rst-content .section ol li>p,.rst-content .section ol li>p:last-child,.rst-content .section ul li>p,.rst-content .section ul li>p:last-child,.rst-content .toctree-wrapper ol li>p,.rst-content .toctree-wrapper ol li>p:last-child,.rst-content .toctree-wrapper ul li>p,.rst-content .toctree-wrapper ul li>p:last-child,.rst-content section ol li>p,.rst-content section ol li>p:last-child,.rst-content section ul li>p,.rst-content section ul li>p:last-child{margin-bottom:12px}.rst-content .section ol li>p:only-child,.rst-content .section ol li>p:only-child:last-child,.rst-content .section ul li>p:only-child,.rst-content .section ul li>p:only-child:last-child,.rst-content .toctree-wrapper ol li>p:only-child,.rst-content .toctree-wrapper ol li>p:only-child:last-child,.rst-content .toctree-wrapper ul li>p:only-child,.rst-content .toctree-wrapper ul li>p:only-child:last-child,.rst-content section ol li>p:only-child,.rst-content section ol li>p:only-child:last-child,.rst-content section ul li>p:only-child,.rst-content section ul li>p:only-child:last-child{margin-bottom:0}.rst-content .section ol li>ol,.rst-content .section ol li>ul,.rst-content .section ul li>ol,.rst-content .section ul li>ul,.rst-content .toctree-wrapper ol li>ol,.rst-content .toctree-wrapper ol li>ul,.rst-content .toctree-wrapper ul li>ol,.rst-content .toctree-wrapper ul li>ul,.rst-content section ol li>ol,.rst-content section ol li>ul,.rst-content section ul li>ol,.rst-content section ul li>ul{margin-bottom:12px}.rst-content .section ol.simple li>*,.rst-content .section ol.simple li ol,.rst-content .section ol.simple li ul,.rst-content .section ul.simple li>*,.rst-content .section ul.simple li ol,.rst-content .section ul.simple li ul,.rst-content .toctree-wrapper ol.simple li>*,.rst-content .toctree-wrapper ol.simple li ol,.rst-content .toctree-wrapper ol.simple li ul,.rst-content .toctree-wrapper ul.simple li>*,.rst-content .toctree-wrapper ul.simple li ol,.rst-content .toctree-wrapper ul.simple li ul,.rst-content section ol.simple li>*,.rst-content section ol.simple li ol,.rst-content section ol.simple li ul,.rst-content section ul.simple li>*,.rst-content section ul.simple li ol,.rst-content section ul.simple li ul{margin-top:0;margin-bottom:0}.rst-content .line-block{margin-left:0;margin-bottom:24px;line-height:24px}.rst-content .line-block .line-block{margin-left:24px;margin-bottom:0}.rst-content .topic-title{font-weight:700;margin-bottom:12px}.rst-content .toc-backref{color:#404040}.rst-content .align-right{float:right;margin:0 0 24px 24px}.rst-content .align-left{float:left;margin:0 24px 24px 0}.rst-content .align-center{margin:auto}.rst-content .align-center:not(table){display:block}.rst-content .code-block-caption .headerlink,.rst-content .eqno .headerlink,.rst-content .toctree-wrapper>p.caption .headerlink,.rst-content dl dt .headerlink,.rst-content h1 .headerlink,.rst-content h2 .headerlink,.rst-content h3 .headerlink,.rst-content h4 .headerlink,.rst-content h5 .headerlink,.rst-content h6 .headerlink,.rst-content p.caption .headerlink,.rst-content p .headerlink,.rst-content table>caption .headerlink{opacity:0;font-size:14px;font-family:FontAwesome;margin-left:.5em}.rst-content .code-block-caption .headerlink:focus,.rst-content .code-block-caption:hover .headerlink,.rst-content .eqno .headerlink:focus,.rst-content .eqno:hover .headerlink,.rst-content .toctree-wrapper>p.caption .headerlink:focus,.rst-content .toctree-wrapper>p.caption:hover .headerlink,.rst-content dl dt .headerlink:focus,.rst-content dl dt:hover .headerlink,.rst-content h1 .headerlink:focus,.rst-content h1:hover .headerlink,.rst-content h2 .headerlink:focus,.rst-content h2:hover .headerlink,.rst-content h3 .headerlink:focus,.rst-content h3:hover .headerlink,.rst-content h4 .headerlink:focus,.rst-content h4:hover .headerlink,.rst-content h5 .headerlink:focus,.rst-content h5:hover .headerlink,.rst-content h6 .headerlink:focus,.rst-content h6:hover .headerlink,.rst-content p.caption .headerlink:focus,.rst-content p.caption:hover .headerlink,.rst-content p .headerlink:focus,.rst-content p:hover .headerlink,.rst-content table>caption .headerlink:focus,.rst-content table>caption:hover .headerlink{opacity:1}.rst-content .btn:focus{outline:2px solid}.rst-content table>caption .headerlink:after{font-size:12px}.rst-content .centered{text-align:center}.rst-content .sidebar{float:right;width:40%;display:block;margin:0 0 24px 24px;padding:24px;background:#f3f6f6;border:1px solid #e1e4e5}.rst-content .sidebar dl,.rst-content .sidebar p,.rst-content .sidebar ul{font-size:90%}.rst-content .sidebar .last,.rst-content .sidebar>:last-child{margin-bottom:0}.rst-content .sidebar .sidebar-title{display:block;font-family:Roboto Slab,ff-tisa-web-pro,Georgia,Arial,sans-serif;font-weight:700;background:#e1e4e5;padding:6px 12px;margin:-24px -24px 24px;font-size:100%}.rst-content .highlighted{background:#f1c40f;box-shadow:0 0 0 2px #f1c40f;display:inline;font-weight:700}.rst-content .citation-reference,.rst-content .footnote-reference{vertical-align:baseline;position:relative;top:-.4em;line-height:0;font-size:90%}.rst-content .hlist{width:100%}.rst-content dl dt span.classifier:before{content:" : "}.rst-content dl dt span.classifier-delimiter{display:none!important}html.writer-html4 .rst-content table.docutils.citation,html.writer-html4 .rst-content table.docutils.footnote{background:none;border:none}html.writer-html4 .rst-content table.docutils.citation td,html.writer-html4 .rst-content table.docutils.citation tr,html.writer-html4 .rst-content table.docutils.footnote td,html.writer-html4 .rst-content table.docutils.footnote tr{border:none;background-color:transparent!important;white-space:normal}html.writer-html4 .rst-content table.docutils.citation td.label,html.writer-html4 .rst-content table.docutils.footnote td.label{padding-left:0;padding-right:0;vertical-align:top}html.writer-html5 .rst-content dl.field-list,html.writer-html5 .rst-content dl.footnote{display:grid;grid-template-columns:max-content auto}html.writer-html5 .rst-content dl.field-list>dt,html.writer-html5 .rst-content dl.footnote>dt{padding-left:1rem}html.writer-html5 .rst-content dl.field-list>dt:after,html.writer-html5 .rst-content dl.footnote>dt:after{content:":"}html.writer-html5 .rst-content dl.field-list>dd,html.writer-html5 .rst-content dl.field-list>dt,html.writer-html5 .rst-content dl.footnote>dd,html.writer-html5 .rst-content dl.footnote>dt{margin-bottom:0}html.writer-html5 .rst-content dl.footnote{font-size:.9rem}html.writer-html5 .rst-content dl.footnote>dt{margin:0 .5rem .5rem 0;line-height:1.2rem;word-break:break-all;font-weight:400}html.writer-html5 .rst-content dl.footnote>dt>span.brackets{margin-right:.5rem}html.writer-html5 .rst-content dl.footnote>dt>span.brackets:before{content:"["}html.writer-html5 .rst-content dl.footnote>dt>span.brackets:after{content:"]"}html.writer-html5 .rst-content dl.footnote>dt>span.fn-backref{font-style:italic}html.writer-html5 .rst-content dl.footnote>dd{margin:0 0 .5rem;line-height:1.2rem}html.writer-html5 .rst-content dl.footnote>dd p,html.writer-html5 .rst-content dl.option-list kbd{font-size:.9rem}.rst-content table.docutils.footnote,html.writer-html4 .rst-content table.docutils.citation,html.writer-html5 .rst-content dl.footnote{color:grey}.rst-content table.docutils.footnote code,.rst-content table.docutils.footnote tt,html.writer-html4 .rst-content table.docutils.citation code,html.writer-html4 .rst-content table.docutils.citation tt,html.writer-html5 .rst-content dl.footnote code,html.writer-html5 .rst-content dl.footnote tt{color:#555}.rst-content .wy-table-responsive.citation,.rst-content .wy-table-responsive.footnote{margin-bottom:0}.rst-content .wy-table-responsive.citation+:not(.citation),.rst-content .wy-table-responsive.footnote+:not(.footnote){margin-top:24px}.rst-content .wy-table-responsive.citation:last-child,.rst-content .wy-table-responsive.footnote:last-child{margin-bottom:24px}.rst-content table.docutils th{border-color:#e1e4e5}html.writer-html5 .rst-content table.docutils th{border:1px solid #e1e4e5}html.writer-html5 .rst-content table.docutils td>p,html.writer-html5 .rst-content table.docutils th>p{line-height:1rem;margin-bottom:0;font-size:.9rem}.rst-content table.docutils td .last,.rst-content table.docutils td .last>:last-child{margin-bottom:0}.rst-content table.field-list,.rst-content table.field-list td{border:none}.rst-content table.field-list td p{font-size:inherit;line-height:inherit}.rst-content table.field-list td>strong{display:inline-block}.rst-content table.field-list .field-name{padding-right:10px;text-align:left;white-space:nowrap}.rst-content table.field-list .field-body{text-align:left}.rst-content code,.rst-content tt{color:#000;font-family:SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,Courier,monospace;padding:2px 5px}.rst-content code big,.rst-content code em,.rst-content tt big,.rst-content tt em{font-size:100%!important;line-height:normal}.rst-content code.literal,.rst-content tt.literal{color:#e74c3c;white-space:normal}.rst-content code.xref,.rst-content tt.xref,a .rst-content code,a .rst-content tt{font-weight:700;color:#404040}.rst-content kbd,.rst-content pre,.rst-content samp{font-family:SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,Courier,monospace}.rst-content a code,.rst-content a tt{color:#2980b9}.rst-content dl{margin-bottom:24px}.rst-content dl dt{font-weight:700;margin-bottom:12px}.rst-content dl ol,.rst-content dl p,.rst-content dl table,.rst-content dl ul{margin-bottom:12px}.rst-content dl dd{margin:0 0 12px 24px;line-height:24px}html.writer-html4 .rst-content dl:not(.docutils),html.writer-html5 .rst-content dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.glossary):not(.simple){margin-bottom:24px}html.writer-html4 .rst-content dl:not(.docutils)>dt,html.writer-html5 .rst-content dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.glossary):not(.simple)>dt{display:table;margin:6px 0;font-size:90%;line-height:normal;background:#e7f2fa;color:#2980b9;border-top:3px solid #6ab0de;padding:6px;position:relative}html.writer-html4 .rst-content dl:not(.docutils)>dt:before,html.writer-html5 .rst-content dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.glossary):not(.simple)>dt:before{color:#6ab0de}html.writer-html4 .rst-content dl:not(.docutils)>dt .headerlink,html.writer-html5 .rst-content dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.glossary):not(.simple)>dt .headerlink{color:#404040;font-size:100%!important}html.writer-html4 .rst-content dl:not(.docutils) dl:not(.field-list)>dt,html.writer-html5 .rst-content dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.glossary):not(.simple) dl:not(.field-list)>dt{margin-bottom:6px;border:none;border-left:3px solid #ccc;background:#f0f0f0;color:#555}html.writer-html4 .rst-content dl:not(.docutils) dl:not(.field-list)>dt .headerlink,html.writer-html5 .rst-content dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.glossary):not(.simple) dl:not(.field-list)>dt .headerlink{color:#404040;font-size:100%!important}html.writer-html4 .rst-content dl:not(.docutils)>dt:first-child,html.writer-html5 .rst-content dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.glossary):not(.simple)>dt:first-child{margin-top:0}html.writer-html4 .rst-content dl:not(.docutils) code.descclassname,html.writer-html4 .rst-content dl:not(.docutils) code.descname,html.writer-html4 .rst-content dl:not(.docutils) tt.descclassname,html.writer-html4 .rst-content dl:not(.docutils) tt.descname,html.writer-html5 .rst-content dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.glossary):not(.simple) code.descclassname,html.writer-html5 .rst-content dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.glossary):not(.simple) code.descname,html.writer-html5 .rst-content dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.glossary):not(.simple) tt.descclassname,html.writer-html5 .rst-content dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.glossary):not(.simple) tt.descname{background-color:transparent;border:none;padding:0;font-size:100%!important}html.writer-html4 .rst-content dl:not(.docutils) code.descname,html.writer-html4 .rst-content dl:not(.docutils) tt.descname,html.writer-html5 .rst-content dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.glossary):not(.simple) code.descname,html.writer-html5 .rst-content dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.glossary):not(.simple) tt.descname{font-weight:700}html.writer-html4 .rst-content dl:not(.docutils) .optional,html.writer-html5 .rst-content dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.glossary):not(.simple) .optional{display:inline-block;padding:0 4px;color:#000;font-weight:700}html.writer-html4 .rst-content dl:not(.docutils) .property,html.writer-html5 .rst-content dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.glossary):not(.simple) .property{display:inline-block;padding-right:8px;max-width:100%}html.writer-html4 .rst-content dl:not(.docutils) .k,html.writer-html5 .rst-content dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.glossary):not(.simple) .k{font-style:italic}html.writer-html4 .rst-content dl:not(.docutils) .descclassname,html.writer-html4 .rst-content dl:not(.docutils) .descname,html.writer-html4 .rst-content dl:not(.docutils) .sig-name,html.writer-html5 .rst-content dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.glossary):not(.simple) .descclassname,html.writer-html5 .rst-content dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.glossary):not(.simple) .descname,html.writer-html5 .rst-content dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.glossary):not(.simple) .sig-name{font-family:SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,Courier,monospace;color:#000}.rst-content .viewcode-back,.rst-content .viewcode-link{display:inline-block;color:#27ae60;font-size:80%;padding-left:24px}.rst-content .viewcode-back{display:block;float:right}.rst-content p.rubric{margin-bottom:12px;font-weight:700}.rst-content code.download,.rst-content tt.download{background:inherit;padding:inherit;font-weight:400;font-family:inherit;font-size:inherit;color:inherit;border:inherit;white-space:inherit}.rst-content code.download span:first-child,.rst-content tt.download span:first-child{-webkit-font-smoothing:subpixel-antialiased}.rst-content code.download span:first-child:before,.rst-content tt.download span:first-child:before{margin-right:4px}.rst-content .guilabel{border:1px solid #7fbbe3;background:#e7f2fa;font-size:80%;font-weight:700;border-radius:4px;padding:2.4px 6px;margin:auto 2px}.rst-content .versionmodified{font-style:italic}@media screen and (max-width:480px){.rst-content .sidebar{width:100%}}span[id*=MathJax-Span]{color:#404040}.math{text-align:center}@font-face{font-family:Lato;src:url(fonts/lato-normal.woff2?bd03a2cc277bbbc338d464e679fe9942) format("woff2"),url(fonts/lato-normal.woff?27bd77b9162d388cb8d4c4217c7c5e2a) format("woff");font-weight:400;font-style:normal;font-display:block}@font-face{font-family:Lato;src:url(fonts/lato-bold.woff2?cccb897485813c7c256901dbca54ecf2) format("woff2"),url(fonts/lato-bold.woff?d878b6c29b10beca227e9eef4246111b) format("woff");font-weight:700;font-style:normal;font-display:block}@font-face{font-family:Lato;src:url(fonts/lato-bold-italic.woff2?0b6bb6725576b072c5d0b02ecdd1900d) format("woff2"),url(fonts/lato-bold-italic.woff?9c7e4e9eb485b4a121c760e61bc3707c) format("woff");font-weight:700;font-style:italic;font-display:block}@font-face{font-family:Lato;src:url(fonts/lato-normal-italic.woff2?4eb103b4d12be57cb1d040ed5e162e9d) format("woff2"),url(fonts/lato-normal-italic.woff?f28f2d6482446544ef1ea1ccc6dd5892) format("woff");font-weight:400;font-style:italic;font-display:block}@font-face{font-family:Roboto Slab;font-style:normal;font-weight:400;src:url(fonts/Roboto-Slab-Regular.woff2?7abf5b8d04d26a2cafea937019bca958) format("woff2"),url(fonts/Roboto-Slab-Regular.woff?c1be9284088d487c5e3ff0a10a92e58c) format("woff");font-display:block}@font-face{font-family:Roboto Slab;font-style:normal;font-weight:700;src:url(fonts/Roboto-Slab-Bold.woff2?9984f4a9bda09be08e83f2506954adbe) format("woff2"),url(fonts/Roboto-Slab-Bold.woff?bed5564a116b05148e3b3bea6fb1162a) format("woff");font-display:block}
+ */@font-face{font-family:FontAwesome;src:url(fonts/fontawesome-webfont.eot?674f50d287a8c48dc19ba404d20fe713);src:url(fonts/fontawesome-webfont.eot?674f50d287a8c48dc19ba404d20fe713?#iefix&v=4.7.0) format("embedded-opentype"),url(fonts/fontawesome-webfont.woff2?af7ae505a9eed503f8b8e6982036873e) format("woff2"),url(fonts/fontawesome-webfont.woff?fee66e712a8a08eef5805a46892932ad) format("woff"),url(fonts/fontawesome-webfont.ttf?b06871f281fee6b241d60582ae9369b9) format("truetype"),url(fonts/fontawesome-webfont.svg?912ec66d7572ff821749319396470bde#fontawesomeregular) format("svg");font-weight:400;font-style:normal}.fa,.icon,.rst-content .admonition-title,.rst-content .code-block-caption .headerlink,.rst-content .eqno .headerlink,.rst-content code.download span:first-child,.rst-content dl dt .headerlink,.rst-content h1 .headerlink,.rst-content h2 .headerlink,.rst-content h3 .headerlink,.rst-content h4 .headerlink,.rst-content h5 .headerlink,.rst-content h6 .headerlink,.rst-content p.caption .headerlink,.rst-content p .headerlink,.rst-content table>caption .headerlink,.rst-content tt.download span:first-child,.wy-menu-vertical li.current>a button.toctree-expand,.wy-menu-vertical li.on a button.toctree-expand,.wy-menu-vertical li button.toctree-expand{display:inline-block;font:normal normal normal 14px/1 FontAwesome;font-size:inherit;text-rendering:auto;-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale}.fa-lg{font-size:1.33333em;line-height:.75em;vertical-align:-15%}.fa-2x{font-size:2em}.fa-3x{font-size:3em}.fa-4x{font-size:4em}.fa-5x{font-size:5em}.fa-fw{width:1.28571em;text-align:center}.fa-ul{padding-left:0;margin-left:2.14286em;list-style-type:none}.fa-ul>li{position:relative}.fa-li{position:absolute;left:-2.14286em;width:2.14286em;top:.14286em;text-align:center}.fa-li.fa-lg{left:-1.85714em}.fa-border{padding:.2em .25em .15em;border:.08em solid #eee;border-radius:.1em}.fa-pull-left{float:left}.fa-pull-right{float:right}.fa-pull-left.icon,.fa.fa-pull-left,.rst-content .code-block-caption .fa-pull-left.headerlink,.rst-content .eqno .fa-pull-left.headerlink,.rst-content .fa-pull-left.admonition-title,.rst-content code.download span.fa-pull-left:first-child,.rst-content dl dt .fa-pull-left.headerlink,.rst-content h1 .fa-pull-left.headerlink,.rst-content h2 .fa-pull-left.headerlink,.rst-content h3 .fa-pull-left.headerlink,.rst-content h4 .fa-pull-left.headerlink,.rst-content h5 .fa-pull-left.headerlink,.rst-content h6 .fa-pull-left.headerlink,.rst-content p .fa-pull-left.headerlink,.rst-content table>caption .fa-pull-left.headerlink,.rst-content tt.download span.fa-pull-left:first-child,.wy-menu-vertical li.current>a button.fa-pull-left.toctree-expand,.wy-menu-vertical li.on a button.fa-pull-left.toctree-expand,.wy-menu-vertical li button.fa-pull-left.toctree-expand{margin-right:.3em}.fa-pull-right.icon,.fa.fa-pull-right,.rst-content .code-block-caption .fa-pull-right.headerlink,.rst-content .eqno .fa-pull-right.headerlink,.rst-content .fa-pull-right.admonition-title,.rst-content code.download span.fa-pull-right:first-child,.rst-content dl dt .fa-pull-right.headerlink,.rst-content h1 .fa-pull-right.headerlink,.rst-content h2 .fa-pull-right.headerlink,.rst-content h3 .fa-pull-right.headerlink,.rst-content h4 .fa-pull-right.headerlink,.rst-content h5 .fa-pull-right.headerlink,.rst-content h6 .fa-pull-right.headerlink,.rst-content p .fa-pull-right.headerlink,.rst-content table>caption .fa-pull-right.headerlink,.rst-content tt.download span.fa-pull-right:first-child,.wy-menu-vertical li.current>a button.fa-pull-right.toctree-expand,.wy-menu-vertical li.on a button.fa-pull-right.toctree-expand,.wy-menu-vertical li button.fa-pull-right.toctree-expand{margin-left:.3em}.pull-right{float:right}.pull-left{float:left}.fa.pull-left,.pull-left.icon,.rst-content .code-block-caption .pull-left.headerlink,.rst-content .eqno .pull-left.headerlink,.rst-content .pull-left.admonition-title,.rst-content code.download span.pull-left:first-child,.rst-content dl dt .pull-left.headerlink,.rst-content h1 .pull-left.headerlink,.rst-content h2 .pull-left.headerlink,.rst-content h3 .pull-left.headerlink,.rst-content h4 .pull-left.headerlink,.rst-content h5 .pull-left.headerlink,.rst-content h6 .pull-left.headerlink,.rst-content p .pull-left.headerlink,.rst-content table>caption .pull-left.headerlink,.rst-content tt.download span.pull-left:first-child,.wy-menu-vertical li.current>a button.pull-left.toctree-expand,.wy-menu-vertical li.on a button.pull-left.toctree-expand,.wy-menu-vertical li button.pull-left.toctree-expand{margin-right:.3em}.fa.pull-right,.pull-right.icon,.rst-content .code-block-caption .pull-right.headerlink,.rst-content .eqno .pull-right.headerlink,.rst-content .pull-right.admonition-title,.rst-content code.download span.pull-right:first-child,.rst-content dl dt .pull-right.headerlink,.rst-content h1 .pull-right.headerlink,.rst-content h2 .pull-right.headerlink,.rst-content h3 .pull-right.headerlink,.rst-content h4 .pull-right.headerlink,.rst-content h5 .pull-right.headerlink,.rst-content h6 .pull-right.headerlink,.rst-content p .pull-right.headerlink,.rst-content table>caption .pull-right.headerlink,.rst-content tt.download span.pull-right:first-child,.wy-menu-vertical li.current>a button.pull-right.toctree-expand,.wy-menu-vertical li.on a button.pull-right.toctree-expand,.wy-menu-vertical li button.pull-right.toctree-expand{margin-left:.3em}.fa-spin{-webkit-animation:fa-spin 2s linear infinite;animation:fa-spin 2s linear infinite}.fa-pulse{-webkit-animation:fa-spin 1s steps(8) infinite;animation:fa-spin 1s steps(8) infinite}@-webkit-keyframes fa-spin{0%{-webkit-transform:rotate(0deg);transform:rotate(0deg)}to{-webkit-transform:rotate(359deg);transform:rotate(359deg)}}@keyframes fa-spin{0%{-webkit-transform:rotate(0deg);transform:rotate(0deg)}to{-webkit-transform:rotate(359deg);transform:rotate(359deg)}}.fa-rotate-90{-ms-filter:"progid:DXImageTransform.Microsoft.BasicImage(rotation=1)";-webkit-transform:rotate(90deg);-ms-transform:rotate(90deg);transform:rotate(90deg)}.fa-rotate-180{-ms-filter:"progid:DXImageTransform.Microsoft.BasicImage(rotation=2)";-webkit-transform:rotate(180deg);-ms-transform:rotate(180deg);transform:rotate(180deg)}.fa-rotate-270{-ms-filter:"progid:DXImageTransform.Microsoft.BasicImage(rotation=3)";-webkit-transform:rotate(270deg);-ms-transform:rotate(270deg);transform:rotate(270deg)}.fa-flip-horizontal{-ms-filter:"progid:DXImageTransform.Microsoft.BasicImage(rotation=0, mirror=1)";-webkit-transform:scaleX(-1);-ms-transform:scaleX(-1);transform:scaleX(-1)}.fa-flip-vertical{-ms-filter:"progid:DXImageTransform.Microsoft.BasicImage(rotation=2, mirror=1)";-webkit-transform:scaleY(-1);-ms-transform:scaleY(-1);transform:scaleY(-1)}:root .fa-flip-horizontal,:root .fa-flip-vertical,:root .fa-rotate-90,:root .fa-rotate-180,:root .fa-rotate-270{filter:none}.fa-stack{position:relative;display:inline-block;width:2em;height:2em;line-height:2em;vertical-align:middle}.fa-stack-1x,.fa-stack-2x{position:absolute;left:0;width:100%;text-align:center}.fa-stack-1x{line-height:inherit}.fa-stack-2x{font-size:2em}.fa-inverse{color:#fff}.fa-glass:before{content:""}.fa-music:before{content:""}.fa-search:before,.icon-search:before{content:""}.fa-envelope-o:before{content:""}.fa-heart:before{content:""}.fa-star:before{content:""}.fa-star-o:before{content:""}.fa-user:before{content:""}.fa-film:before{content:""}.fa-th-large:before{content:""}.fa-th:before{content:""}.fa-th-list:before{content:""}.fa-check:before{content:""}.fa-close:before,.fa-remove:before,.fa-times:before{content:""}.fa-search-plus:before{content:""}.fa-search-minus:before{content:""}.fa-power-off:before{content:""}.fa-signal:before{content:""}.fa-cog:before,.fa-gear:before{content:""}.fa-trash-o:before{content:""}.fa-home:before,.icon-home:before{content:""}.fa-file-o:before{content:""}.fa-clock-o:before{content:""}.fa-road:before{content:""}.fa-download:before,.rst-content code.download span:first-child:before,.rst-content tt.download span:first-child:before{content:""}.fa-arrow-circle-o-down:before{content:""}.fa-arrow-circle-o-up:before{content:""}.fa-inbox:before{content:""}.fa-play-circle-o:before{content:""}.fa-repeat:before,.fa-rotate-right:before{content:""}.fa-refresh:before{content:""}.fa-list-alt:before{content:""}.fa-lock:before{content:""}.fa-flag:before{content:""}.fa-headphones:before{content:""}.fa-volume-off:before{content:""}.fa-volume-down:before{content:""}.fa-volume-up:before{content:""}.fa-qrcode:before{content:""}.fa-barcode:before{content:""}.fa-tag:before{content:""}.fa-tags:before{content:""}.fa-book:before,.icon-book:before{content:""}.fa-bookmark:before{content:""}.fa-print:before{content:""}.fa-camera:before{content:""}.fa-font:before{content:""}.fa-bold:before{content:""}.fa-italic:before{content:""}.fa-text-height:before{content:""}.fa-text-width:before{content:""}.fa-align-left:before{content:""}.fa-align-center:before{content:""}.fa-align-right:before{content:""}.fa-align-justify:before{content:""}.fa-list:before{content:""}.fa-dedent:before,.fa-outdent:before{content:""}.fa-indent:before{content:""}.fa-video-camera:before{content:""}.fa-image:before,.fa-photo:before,.fa-picture-o:before{content:""}.fa-pencil:before{content:""}.fa-map-marker:before{content:""}.fa-adjust:before{content:""}.fa-tint:before{content:""}.fa-edit:before,.fa-pencil-square-o:before{content:""}.fa-share-square-o:before{content:""}.fa-check-square-o:before{content:""}.fa-arrows:before{content:""}.fa-step-backward:before{content:""}.fa-fast-backward:before{content:""}.fa-backward:before{content:""}.fa-play:before{content:""}.fa-pause:before{content:""}.fa-stop:before{content:""}.fa-forward:before{content:""}.fa-fast-forward:before{content:""}.fa-step-forward:before{content:""}.fa-eject:before{content:""}.fa-chevron-left:before{content:""}.fa-chevron-right:before{content:""}.fa-plus-circle:before{content:""}.fa-minus-circle:before{content:""}.fa-times-circle:before,.wy-inline-validate.wy-inline-validate-danger .wy-input-context:before{content:""}.fa-check-circle:before,.wy-inline-validate.wy-inline-validate-success .wy-input-context:before{content:""}.fa-question-circle:before{content:""}.fa-info-circle:before{content:""}.fa-crosshairs:before{content:""}.fa-times-circle-o:before{content:""}.fa-check-circle-o:before{content:""}.fa-ban:before{content:""}.fa-arrow-left:before{content:""}.fa-arrow-right:before{content:""}.fa-arrow-up:before{content:""}.fa-arrow-down:before{content:""}.fa-mail-forward:before,.fa-share:before{content:""}.fa-expand:before{content:""}.fa-compress:before{content:""}.fa-plus:before{content:""}.fa-minus:before{content:""}.fa-asterisk:before{content:""}.fa-exclamation-circle:before,.rst-content .admonition-title:before,.wy-inline-validate.wy-inline-validate-info .wy-input-context:before,.wy-inline-validate.wy-inline-validate-warning .wy-input-context:before{content:""}.fa-gift:before{content:""}.fa-leaf:before{content:""}.fa-fire:before,.icon-fire:before{content:""}.fa-eye:before{content:""}.fa-eye-slash:before{content:""}.fa-exclamation-triangle:before,.fa-warning:before{content:""}.fa-plane:before{content:""}.fa-calendar:before{content:""}.fa-random:before{content:""}.fa-comment:before{content:""}.fa-magnet:before{content:""}.fa-chevron-up:before{content:""}.fa-chevron-down:before{content:""}.fa-retweet:before{content:""}.fa-shopping-cart:before{content:""}.fa-folder:before{content:""}.fa-folder-open:before{content:""}.fa-arrows-v:before{content:""}.fa-arrows-h:before{content:""}.fa-bar-chart-o:before,.fa-bar-chart:before{content:""}.fa-twitter-square:before{content:""}.fa-facebook-square:before{content:""}.fa-camera-retro:before{content:""}.fa-key:before{content:""}.fa-cogs:before,.fa-gears:before{content:""}.fa-comments:before{content:""}.fa-thumbs-o-up:before{content:""}.fa-thumbs-o-down:before{content:""}.fa-star-half:before{content:""}.fa-heart-o:before{content:""}.fa-sign-out:before{content:""}.fa-linkedin-square:before{content:""}.fa-thumb-tack:before{content:""}.fa-external-link:before{content:""}.fa-sign-in:before{content:""}.fa-trophy:before{content:""}.fa-github-square:before{content:""}.fa-upload:before{content:""}.fa-lemon-o:before{content:""}.fa-phone:before{content:""}.fa-square-o:before{content:""}.fa-bookmark-o:before{content:""}.fa-phone-square:before{content:""}.fa-twitter:before{content:""}.fa-facebook-f:before,.fa-facebook:before{content:""}.fa-github:before,.icon-github:before{content:""}.fa-unlock:before{content:""}.fa-credit-card:before{content:""}.fa-feed:before,.fa-rss:before{content:""}.fa-hdd-o:before{content:""}.fa-bullhorn:before{content:""}.fa-bell:before{content:""}.fa-certificate:before{content:""}.fa-hand-o-right:before{content:""}.fa-hand-o-left:before{content:""}.fa-hand-o-up:before{content:""}.fa-hand-o-down:before{content:""}.fa-arrow-circle-left:before,.icon-circle-arrow-left:before{content:""}.fa-arrow-circle-right:before,.icon-circle-arrow-right:before{content:""}.fa-arrow-circle-up:before{content:""}.fa-arrow-circle-down:before{content:""}.fa-globe:before{content:""}.fa-wrench:before{content:""}.fa-tasks:before{content:""}.fa-filter:before{content:""}.fa-briefcase:before{content:""}.fa-arrows-alt:before{content:""}.fa-group:before,.fa-users:before{content:""}.fa-chain:before,.fa-link:before,.icon-link:before{content:""}.fa-cloud:before{content:""}.fa-flask:before{content:""}.fa-cut:before,.fa-scissors:before{content:""}.fa-copy:before,.fa-files-o:before{content:""}.fa-paperclip:before{content:""}.fa-floppy-o:before,.fa-save:before{content:""}.fa-square:before{content:""}.fa-bars:before,.fa-navicon:before,.fa-reorder:before{content:""}.fa-list-ul:before{content:""}.fa-list-ol:before{content:""}.fa-strikethrough:before{content:""}.fa-underline:before{content:""}.fa-table:before{content:""}.fa-magic:before{content:""}.fa-truck:before{content:""}.fa-pinterest:before{content:""}.fa-pinterest-square:before{content:""}.fa-google-plus-square:before{content:""}.fa-google-plus:before{content:""}.fa-money:before{content:""}.fa-caret-down:before,.icon-caret-down:before,.wy-dropdown .caret:before{content:""}.fa-caret-up:before{content:""}.fa-caret-left:before{content:""}.fa-caret-right:before{content:""}.fa-columns:before{content:""}.fa-sort:before,.fa-unsorted:before{content:""}.fa-sort-desc:before,.fa-sort-down:before{content:""}.fa-sort-asc:before,.fa-sort-up:before{content:""}.fa-envelope:before{content:""}.fa-linkedin:before{content:""}.fa-rotate-left:before,.fa-undo:before{content:""}.fa-gavel:before,.fa-legal:before{content:""}.fa-dashboard:before,.fa-tachometer:before{content:""}.fa-comment-o:before{content:""}.fa-comments-o:before{content:""}.fa-bolt:before,.fa-flash:before{content:""}.fa-sitemap:before{content:""}.fa-umbrella:before{content:""}.fa-clipboard:before,.fa-paste:before{content:""}.fa-lightbulb-o:before{content:""}.fa-exchange:before{content:""}.fa-cloud-download:before{content:""}.fa-cloud-upload:before{content:""}.fa-user-md:before{content:""}.fa-stethoscope:before{content:""}.fa-suitcase:before{content:""}.fa-bell-o:before{content:""}.fa-coffee:before{content:""}.fa-cutlery:before{content:""}.fa-file-text-o:before{content:""}.fa-building-o:before{content:""}.fa-hospital-o:before{content:""}.fa-ambulance:before{content:""}.fa-medkit:before{content:""}.fa-fighter-jet:before{content:""}.fa-beer:before{content:""}.fa-h-square:before{content:""}.fa-plus-square:before{content:""}.fa-angle-double-left:before{content:""}.fa-angle-double-right:before{content:""}.fa-angle-double-up:before{content:""}.fa-angle-double-down:before{content:""}.fa-angle-left:before{content:""}.fa-angle-right:before{content:""}.fa-angle-up:before{content:""}.fa-angle-down:before{content:""}.fa-desktop:before{content:""}.fa-laptop:before{content:""}.fa-tablet:before{content:""}.fa-mobile-phone:before,.fa-mobile:before{content:""}.fa-circle-o:before{content:""}.fa-quote-left:before{content:""}.fa-quote-right:before{content:""}.fa-spinner:before{content:""}.fa-circle:before{content:""}.fa-mail-reply:before,.fa-reply:before{content:""}.fa-github-alt:before{content:""}.fa-folder-o:before{content:""}.fa-folder-open-o:before{content:""}.fa-smile-o:before{content:""}.fa-frown-o:before{content:""}.fa-meh-o:before{content:""}.fa-gamepad:before{content:""}.fa-keyboard-o:before{content:""}.fa-flag-o:before{content:""}.fa-flag-checkered:before{content:""}.fa-terminal:before{content:""}.fa-code:before{content:""}.fa-mail-reply-all:before,.fa-reply-all:before{content:""}.fa-star-half-empty:before,.fa-star-half-full:before,.fa-star-half-o:before{content:""}.fa-location-arrow:before{content:""}.fa-crop:before{content:""}.fa-code-fork:before{content:""}.fa-chain-broken:before,.fa-unlink:before{content:""}.fa-question:before{content:""}.fa-info:before{content:""}.fa-exclamation:before{content:""}.fa-superscript:before{content:""}.fa-subscript:before{content:""}.fa-eraser:before{content:""}.fa-puzzle-piece:before{content:""}.fa-microphone:before{content:""}.fa-microphone-slash:before{content:""}.fa-shield:before{content:""}.fa-calendar-o:before{content:""}.fa-fire-extinguisher:before{content:""}.fa-rocket:before{content:""}.fa-maxcdn:before{content:""}.fa-chevron-circle-left:before{content:""}.fa-chevron-circle-right:before{content:""}.fa-chevron-circle-up:before{content:""}.fa-chevron-circle-down:before{content:""}.fa-html5:before{content:""}.fa-css3:before{content:""}.fa-anchor:before{content:""}.fa-unlock-alt:before{content:""}.fa-bullseye:before{content:""}.fa-ellipsis-h:before{content:""}.fa-ellipsis-v:before{content:""}.fa-rss-square:before{content:""}.fa-play-circle:before{content:""}.fa-ticket:before{content:""}.fa-minus-square:before{content:""}.fa-minus-square-o:before,.wy-menu-vertical li.current>a button.toctree-expand:before,.wy-menu-vertical li.on a button.toctree-expand:before{content:""}.fa-level-up:before{content:""}.fa-level-down:before{content:""}.fa-check-square:before{content:""}.fa-pencil-square:before{content:""}.fa-external-link-square:before{content:""}.fa-share-square:before{content:""}.fa-compass:before{content:""}.fa-caret-square-o-down:before,.fa-toggle-down:before{content:""}.fa-caret-square-o-up:before,.fa-toggle-up:before{content:""}.fa-caret-square-o-right:before,.fa-toggle-right:before{content:""}.fa-eur:before,.fa-euro:before{content:""}.fa-gbp:before{content:""}.fa-dollar:before,.fa-usd:before{content:""}.fa-inr:before,.fa-rupee:before{content:""}.fa-cny:before,.fa-jpy:before,.fa-rmb:before,.fa-yen:before{content:""}.fa-rouble:before,.fa-rub:before,.fa-ruble:before{content:""}.fa-krw:before,.fa-won:before{content:""}.fa-bitcoin:before,.fa-btc:before{content:""}.fa-file:before{content:""}.fa-file-text:before{content:""}.fa-sort-alpha-asc:before{content:""}.fa-sort-alpha-desc:before{content:""}.fa-sort-amount-asc:before{content:""}.fa-sort-amount-desc:before{content:""}.fa-sort-numeric-asc:before{content:""}.fa-sort-numeric-desc:before{content:""}.fa-thumbs-up:before{content:""}.fa-thumbs-down:before{content:""}.fa-youtube-square:before{content:""}.fa-youtube:before{content:""}.fa-xing:before{content:""}.fa-xing-square:before{content:""}.fa-youtube-play:before{content:""}.fa-dropbox:before{content:""}.fa-stack-overflow:before{content:""}.fa-instagram:before{content:""}.fa-flickr:before{content:""}.fa-adn:before{content:""}.fa-bitbucket:before,.icon-bitbucket:before{content:""}.fa-bitbucket-square:before{content:""}.fa-tumblr:before{content:""}.fa-tumblr-square:before{content:""}.fa-long-arrow-down:before{content:""}.fa-long-arrow-up:before{content:""}.fa-long-arrow-left:before{content:""}.fa-long-arrow-right:before{content:""}.fa-apple:before{content:""}.fa-windows:before{content:""}.fa-android:before{content:""}.fa-linux:before{content:""}.fa-dribbble:before{content:""}.fa-skype:before{content:""}.fa-foursquare:before{content:""}.fa-trello:before{content:""}.fa-female:before{content:""}.fa-male:before{content:""}.fa-gittip:before,.fa-gratipay:before{content:""}.fa-sun-o:before{content:""}.fa-moon-o:before{content:""}.fa-archive:before{content:""}.fa-bug:before{content:""}.fa-vk:before{content:""}.fa-weibo:before{content:""}.fa-renren:before{content:""}.fa-pagelines:before{content:""}.fa-stack-exchange:before{content:""}.fa-arrow-circle-o-right:before{content:""}.fa-arrow-circle-o-left:before{content:""}.fa-caret-square-o-left:before,.fa-toggle-left:before{content:""}.fa-dot-circle-o:before{content:""}.fa-wheelchair:before{content:""}.fa-vimeo-square:before{content:""}.fa-try:before,.fa-turkish-lira:before{content:""}.fa-plus-square-o:before,.wy-menu-vertical li button.toctree-expand:before{content:""}.fa-space-shuttle:before{content:""}.fa-slack:before{content:""}.fa-envelope-square:before{content:""}.fa-wordpress:before{content:""}.fa-openid:before{content:""}.fa-bank:before,.fa-institution:before,.fa-university:before{content:""}.fa-graduation-cap:before,.fa-mortar-board:before{content:""}.fa-yahoo:before{content:""}.fa-google:before{content:""}.fa-reddit:before{content:""}.fa-reddit-square:before{content:""}.fa-stumbleupon-circle:before{content:""}.fa-stumbleupon:before{content:""}.fa-delicious:before{content:""}.fa-digg:before{content:""}.fa-pied-piper-pp:before{content:""}.fa-pied-piper-alt:before{content:""}.fa-drupal:before{content:""}.fa-joomla:before{content:""}.fa-language:before{content:""}.fa-fax:before{content:""}.fa-building:before{content:""}.fa-child:before{content:""}.fa-paw:before{content:""}.fa-spoon:before{content:""}.fa-cube:before{content:""}.fa-cubes:before{content:""}.fa-behance:before{content:""}.fa-behance-square:before{content:""}.fa-steam:before{content:""}.fa-steam-square:before{content:""}.fa-recycle:before{content:""}.fa-automobile:before,.fa-car:before{content:""}.fa-cab:before,.fa-taxi:before{content:""}.fa-tree:before{content:""}.fa-spotify:before{content:""}.fa-deviantart:before{content:""}.fa-soundcloud:before{content:""}.fa-database:before{content:""}.fa-file-pdf-o:before{content:""}.fa-file-word-o:before{content:""}.fa-file-excel-o:before{content:""}.fa-file-powerpoint-o:before{content:""}.fa-file-image-o:before,.fa-file-photo-o:before,.fa-file-picture-o:before{content:""}.fa-file-archive-o:before,.fa-file-zip-o:before{content:""}.fa-file-audio-o:before,.fa-file-sound-o:before{content:""}.fa-file-movie-o:before,.fa-file-video-o:before{content:""}.fa-file-code-o:before{content:""}.fa-vine:before{content:""}.fa-codepen:before{content:""}.fa-jsfiddle:before{content:""}.fa-life-bouy:before,.fa-life-buoy:before,.fa-life-ring:before,.fa-life-saver:before,.fa-support:before{content:""}.fa-circle-o-notch:before{content:""}.fa-ra:before,.fa-rebel:before,.fa-resistance:before{content:""}.fa-empire:before,.fa-ge:before{content:""}.fa-git-square:before{content:""}.fa-git:before{content:""}.fa-hacker-news:before,.fa-y-combinator-square:before,.fa-yc-square:before{content:""}.fa-tencent-weibo:before{content:""}.fa-qq:before{content:""}.fa-wechat:before,.fa-weixin:before{content:""}.fa-paper-plane:before,.fa-send:before{content:""}.fa-paper-plane-o:before,.fa-send-o:before{content:""}.fa-history:before{content:""}.fa-circle-thin:before{content:""}.fa-header:before{content:""}.fa-paragraph:before{content:""}.fa-sliders:before{content:""}.fa-share-alt:before{content:""}.fa-share-alt-square:before{content:""}.fa-bomb:before{content:""}.fa-futbol-o:before,.fa-soccer-ball-o:before{content:""}.fa-tty:before{content:""}.fa-binoculars:before{content:""}.fa-plug:before{content:""}.fa-slideshare:before{content:""}.fa-twitch:before{content:""}.fa-yelp:before{content:""}.fa-newspaper-o:before{content:""}.fa-wifi:before{content:""}.fa-calculator:before{content:""}.fa-paypal:before{content:""}.fa-google-wallet:before{content:""}.fa-cc-visa:before{content:""}.fa-cc-mastercard:before{content:""}.fa-cc-discover:before{content:""}.fa-cc-amex:before{content:""}.fa-cc-paypal:before{content:""}.fa-cc-stripe:before{content:""}.fa-bell-slash:before{content:""}.fa-bell-slash-o:before{content:""}.fa-trash:before{content:""}.fa-copyright:before{content:""}.fa-at:before{content:""}.fa-eyedropper:before{content:""}.fa-paint-brush:before{content:""}.fa-birthday-cake:before{content:""}.fa-area-chart:before{content:""}.fa-pie-chart:before{content:""}.fa-line-chart:before{content:""}.fa-lastfm:before{content:""}.fa-lastfm-square:before{content:""}.fa-toggle-off:before{content:""}.fa-toggle-on:before{content:""}.fa-bicycle:before{content:""}.fa-bus:before{content:""}.fa-ioxhost:before{content:""}.fa-angellist:before{content:""}.fa-cc:before{content:""}.fa-ils:before,.fa-shekel:before,.fa-sheqel:before{content:""}.fa-meanpath:before{content:""}.fa-buysellads:before{content:""}.fa-connectdevelop:before{content:""}.fa-dashcube:before{content:""}.fa-forumbee:before{content:""}.fa-leanpub:before{content:""}.fa-sellsy:before{content:""}.fa-shirtsinbulk:before{content:""}.fa-simplybuilt:before{content:""}.fa-skyatlas:before{content:""}.fa-cart-plus:before{content:""}.fa-cart-arrow-down:before{content:""}.fa-diamond:before{content:""}.fa-ship:before{content:""}.fa-user-secret:before{content:""}.fa-motorcycle:before{content:""}.fa-street-view:before{content:""}.fa-heartbeat:before{content:""}.fa-venus:before{content:""}.fa-mars:before{content:""}.fa-mercury:before{content:""}.fa-intersex:before,.fa-transgender:before{content:""}.fa-transgender-alt:before{content:""}.fa-venus-double:before{content:""}.fa-mars-double:before{content:""}.fa-venus-mars:before{content:""}.fa-mars-stroke:before{content:""}.fa-mars-stroke-v:before{content:""}.fa-mars-stroke-h:before{content:""}.fa-neuter:before{content:""}.fa-genderless:before{content:""}.fa-facebook-official:before{content:""}.fa-pinterest-p:before{content:""}.fa-whatsapp:before{content:""}.fa-server:before{content:""}.fa-user-plus:before{content:""}.fa-user-times:before{content:""}.fa-bed:before,.fa-hotel:before{content:""}.fa-viacoin:before{content:""}.fa-train:before{content:""}.fa-subway:before{content:""}.fa-medium:before{content:""}.fa-y-combinator:before,.fa-yc:before{content:""}.fa-optin-monster:before{content:""}.fa-opencart:before{content:""}.fa-expeditedssl:before{content:""}.fa-battery-4:before,.fa-battery-full:before,.fa-battery:before{content:""}.fa-battery-3:before,.fa-battery-three-quarters:before{content:""}.fa-battery-2:before,.fa-battery-half:before{content:""}.fa-battery-1:before,.fa-battery-quarter:before{content:""}.fa-battery-0:before,.fa-battery-empty:before{content:""}.fa-mouse-pointer:before{content:""}.fa-i-cursor:before{content:""}.fa-object-group:before{content:""}.fa-object-ungroup:before{content:""}.fa-sticky-note:before{content:""}.fa-sticky-note-o:before{content:""}.fa-cc-jcb:before{content:""}.fa-cc-diners-club:before{content:""}.fa-clone:before{content:""}.fa-balance-scale:before{content:""}.fa-hourglass-o:before{content:""}.fa-hourglass-1:before,.fa-hourglass-start:before{content:""}.fa-hourglass-2:before,.fa-hourglass-half:before{content:""}.fa-hourglass-3:before,.fa-hourglass-end:before{content:""}.fa-hourglass:before{content:""}.fa-hand-grab-o:before,.fa-hand-rock-o:before{content:""}.fa-hand-paper-o:before,.fa-hand-stop-o:before{content:""}.fa-hand-scissors-o:before{content:""}.fa-hand-lizard-o:before{content:""}.fa-hand-spock-o:before{content:""}.fa-hand-pointer-o:before{content:""}.fa-hand-peace-o:before{content:""}.fa-trademark:before{content:""}.fa-registered:before{content:""}.fa-creative-commons:before{content:""}.fa-gg:before{content:""}.fa-gg-circle:before{content:""}.fa-tripadvisor:before{content:""}.fa-odnoklassniki:before{content:""}.fa-odnoklassniki-square:before{content:""}.fa-get-pocket:before{content:""}.fa-wikipedia-w:before{content:""}.fa-safari:before{content:""}.fa-chrome:before{content:""}.fa-firefox:before{content:""}.fa-opera:before{content:""}.fa-internet-explorer:before{content:""}.fa-television:before,.fa-tv:before{content:""}.fa-contao:before{content:""}.fa-500px:before{content:""}.fa-amazon:before{content:""}.fa-calendar-plus-o:before{content:""}.fa-calendar-minus-o:before{content:""}.fa-calendar-times-o:before{content:""}.fa-calendar-check-o:before{content:""}.fa-industry:before{content:""}.fa-map-pin:before{content:""}.fa-map-signs:before{content:""}.fa-map-o:before{content:""}.fa-map:before{content:""}.fa-commenting:before{content:""}.fa-commenting-o:before{content:""}.fa-houzz:before{content:""}.fa-vimeo:before{content:""}.fa-black-tie:before{content:""}.fa-fonticons:before{content:""}.fa-reddit-alien:before{content:""}.fa-edge:before{content:""}.fa-credit-card-alt:before{content:""}.fa-codiepie:before{content:""}.fa-modx:before{content:""}.fa-fort-awesome:before{content:""}.fa-usb:before{content:""}.fa-product-hunt:before{content:""}.fa-mixcloud:before{content:""}.fa-scribd:before{content:""}.fa-pause-circle:before{content:""}.fa-pause-circle-o:before{content:""}.fa-stop-circle:before{content:""}.fa-stop-circle-o:before{content:""}.fa-shopping-bag:before{content:""}.fa-shopping-basket:before{content:""}.fa-hashtag:before{content:""}.fa-bluetooth:before{content:""}.fa-bluetooth-b:before{content:""}.fa-percent:before{content:""}.fa-gitlab:before,.icon-gitlab:before{content:""}.fa-wpbeginner:before{content:""}.fa-wpforms:before{content:""}.fa-envira:before{content:""}.fa-universal-access:before{content:""}.fa-wheelchair-alt:before{content:""}.fa-question-circle-o:before{content:""}.fa-blind:before{content:""}.fa-audio-description:before{content:""}.fa-volume-control-phone:before{content:""}.fa-braille:before{content:""}.fa-assistive-listening-systems:before{content:""}.fa-american-sign-language-interpreting:before,.fa-asl-interpreting:before{content:""}.fa-deaf:before,.fa-deafness:before,.fa-hard-of-hearing:before{content:""}.fa-glide:before{content:""}.fa-glide-g:before{content:""}.fa-sign-language:before,.fa-signing:before{content:""}.fa-low-vision:before{content:""}.fa-viadeo:before{content:""}.fa-viadeo-square:before{content:""}.fa-snapchat:before{content:""}.fa-snapchat-ghost:before{content:""}.fa-snapchat-square:before{content:""}.fa-pied-piper:before{content:""}.fa-first-order:before{content:""}.fa-yoast:before{content:""}.fa-themeisle:before{content:""}.fa-google-plus-circle:before,.fa-google-plus-official:before{content:""}.fa-fa:before,.fa-font-awesome:before{content:""}.fa-handshake-o:before{content:""}.fa-envelope-open:before{content:""}.fa-envelope-open-o:before{content:""}.fa-linode:before{content:""}.fa-address-book:before{content:""}.fa-address-book-o:before{content:""}.fa-address-card:before,.fa-vcard:before{content:""}.fa-address-card-o:before,.fa-vcard-o:before{content:""}.fa-user-circle:before{content:""}.fa-user-circle-o:before{content:""}.fa-user-o:before{content:""}.fa-id-badge:before{content:""}.fa-drivers-license:before,.fa-id-card:before{content:""}.fa-drivers-license-o:before,.fa-id-card-o:before{content:""}.fa-quora:before{content:""}.fa-free-code-camp:before{content:""}.fa-telegram:before{content:""}.fa-thermometer-4:before,.fa-thermometer-full:before,.fa-thermometer:before{content:""}.fa-thermometer-3:before,.fa-thermometer-three-quarters:before{content:""}.fa-thermometer-2:before,.fa-thermometer-half:before{content:""}.fa-thermometer-1:before,.fa-thermometer-quarter:before{content:""}.fa-thermometer-0:before,.fa-thermometer-empty:before{content:""}.fa-shower:before{content:""}.fa-bath:before,.fa-bathtub:before,.fa-s15:before{content:""}.fa-podcast:before{content:""}.fa-window-maximize:before{content:""}.fa-window-minimize:before{content:""}.fa-window-restore:before{content:""}.fa-times-rectangle:before,.fa-window-close:before{content:""}.fa-times-rectangle-o:before,.fa-window-close-o:before{content:""}.fa-bandcamp:before{content:""}.fa-grav:before{content:""}.fa-etsy:before{content:""}.fa-imdb:before{content:""}.fa-ravelry:before{content:""}.fa-eercast:before{content:""}.fa-microchip:before{content:""}.fa-snowflake-o:before{content:""}.fa-superpowers:before{content:""}.fa-wpexplorer:before{content:""}.fa-meetup:before{content:""}.sr-only{position:absolute;width:1px;height:1px;padding:0;margin:-1px;overflow:hidden;clip:rect(0,0,0,0);border:0}.sr-only-focusable:active,.sr-only-focusable:focus{position:static;width:auto;height:auto;margin:0;overflow:visible;clip:auto}.fa,.icon,.rst-content .admonition-title,.rst-content .code-block-caption .headerlink,.rst-content .eqno .headerlink,.rst-content code.download span:first-child,.rst-content dl dt .headerlink,.rst-content h1 .headerlink,.rst-content h2 .headerlink,.rst-content h3 .headerlink,.rst-content h4 .headerlink,.rst-content h5 .headerlink,.rst-content h6 .headerlink,.rst-content p.caption .headerlink,.rst-content p .headerlink,.rst-content table>caption .headerlink,.rst-content tt.download span:first-child,.wy-dropdown .caret,.wy-inline-validate.wy-inline-validate-danger .wy-input-context,.wy-inline-validate.wy-inline-validate-info .wy-input-context,.wy-inline-validate.wy-inline-validate-success .wy-input-context,.wy-inline-validate.wy-inline-validate-warning .wy-input-context,.wy-menu-vertical li.current>a button.toctree-expand,.wy-menu-vertical li.on a button.toctree-expand,.wy-menu-vertical li button.toctree-expand{font-family:inherit}.fa:before,.icon:before,.rst-content .admonition-title:before,.rst-content .code-block-caption .headerlink:before,.rst-content .eqno .headerlink:before,.rst-content code.download span:first-child:before,.rst-content dl dt .headerlink:before,.rst-content h1 .headerlink:before,.rst-content h2 .headerlink:before,.rst-content h3 .headerlink:before,.rst-content h4 .headerlink:before,.rst-content h5 .headerlink:before,.rst-content h6 .headerlink:before,.rst-content p.caption .headerlink:before,.rst-content p .headerlink:before,.rst-content table>caption .headerlink:before,.rst-content tt.download span:first-child:before,.wy-dropdown .caret:before,.wy-inline-validate.wy-inline-validate-danger .wy-input-context:before,.wy-inline-validate.wy-inline-validate-info .wy-input-context:before,.wy-inline-validate.wy-inline-validate-success .wy-input-context:before,.wy-inline-validate.wy-inline-validate-warning .wy-input-context:before,.wy-menu-vertical li.current>a button.toctree-expand:before,.wy-menu-vertical li.on a button.toctree-expand:before,.wy-menu-vertical li button.toctree-expand:before{font-family:FontAwesome;display:inline-block;font-style:normal;font-weight:400;line-height:1;text-decoration:inherit}.rst-content .code-block-caption a .headerlink,.rst-content .eqno a .headerlink,.rst-content a .admonition-title,.rst-content code.download a span:first-child,.rst-content dl dt a .headerlink,.rst-content h1 a .headerlink,.rst-content h2 a .headerlink,.rst-content h3 a .headerlink,.rst-content h4 a .headerlink,.rst-content h5 a .headerlink,.rst-content h6 a .headerlink,.rst-content p.caption a .headerlink,.rst-content p a .headerlink,.rst-content table>caption a .headerlink,.rst-content tt.download a span:first-child,.wy-menu-vertical li.current>a button.toctree-expand,.wy-menu-vertical li.on a button.toctree-expand,.wy-menu-vertical li a button.toctree-expand,a .fa,a .icon,a .rst-content .admonition-title,a .rst-content .code-block-caption .headerlink,a .rst-content .eqno .headerlink,a .rst-content code.download span:first-child,a .rst-content dl dt .headerlink,a .rst-content h1 .headerlink,a .rst-content h2 .headerlink,a .rst-content h3 .headerlink,a .rst-content h4 .headerlink,a .rst-content h5 .headerlink,a .rst-content h6 .headerlink,a .rst-content p.caption .headerlink,a .rst-content p .headerlink,a .rst-content table>caption .headerlink,a .rst-content tt.download span:first-child,a .wy-menu-vertical li button.toctree-expand{display:inline-block;text-decoration:inherit}.btn .fa,.btn .icon,.btn .rst-content .admonition-title,.btn .rst-content .code-block-caption .headerlink,.btn .rst-content .eqno .headerlink,.btn .rst-content code.download span:first-child,.btn .rst-content dl dt .headerlink,.btn .rst-content h1 .headerlink,.btn .rst-content h2 .headerlink,.btn .rst-content h3 .headerlink,.btn .rst-content h4 .headerlink,.btn .rst-content h5 .headerlink,.btn .rst-content h6 .headerlink,.btn .rst-content p .headerlink,.btn .rst-content table>caption .headerlink,.btn .rst-content tt.download span:first-child,.btn .wy-menu-vertical li.current>a button.toctree-expand,.btn .wy-menu-vertical li.on a button.toctree-expand,.btn .wy-menu-vertical li button.toctree-expand,.nav .fa,.nav .icon,.nav .rst-content .admonition-title,.nav .rst-content .code-block-caption .headerlink,.nav .rst-content .eqno .headerlink,.nav .rst-content code.download span:first-child,.nav .rst-content dl dt .headerlink,.nav .rst-content h1 .headerlink,.nav .rst-content h2 .headerlink,.nav .rst-content h3 .headerlink,.nav .rst-content h4 .headerlink,.nav .rst-content h5 .headerlink,.nav .rst-content h6 .headerlink,.nav .rst-content p .headerlink,.nav .rst-content table>caption .headerlink,.nav .rst-content tt.download span:first-child,.nav .wy-menu-vertical li.current>a button.toctree-expand,.nav .wy-menu-vertical li.on a button.toctree-expand,.nav .wy-menu-vertical li button.toctree-expand,.rst-content .btn .admonition-title,.rst-content .code-block-caption .btn .headerlink,.rst-content .code-block-caption .nav .headerlink,.rst-content .eqno .btn .headerlink,.rst-content .eqno .nav .headerlink,.rst-content .nav .admonition-title,.rst-content code.download .btn span:first-child,.rst-content code.download .nav span:first-child,.rst-content dl dt .btn .headerlink,.rst-content dl dt .nav .headerlink,.rst-content h1 .btn .headerlink,.rst-content h1 .nav .headerlink,.rst-content h2 .btn .headerlink,.rst-content h2 .nav .headerlink,.rst-content h3 .btn .headerlink,.rst-content h3 .nav .headerlink,.rst-content h4 .btn .headerlink,.rst-content h4 .nav .headerlink,.rst-content h5 .btn .headerlink,.rst-content h5 .nav .headerlink,.rst-content h6 .btn .headerlink,.rst-content h6 .nav .headerlink,.rst-content p .btn .headerlink,.rst-content p .nav .headerlink,.rst-content table>caption .btn .headerlink,.rst-content table>caption .nav .headerlink,.rst-content tt.download .btn span:first-child,.rst-content tt.download .nav span:first-child,.wy-menu-vertical li .btn button.toctree-expand,.wy-menu-vertical li.current>a .btn button.toctree-expand,.wy-menu-vertical li.current>a .nav button.toctree-expand,.wy-menu-vertical li .nav button.toctree-expand,.wy-menu-vertical li.on a .btn button.toctree-expand,.wy-menu-vertical li.on a .nav button.toctree-expand{display:inline}.btn .fa-large.icon,.btn .fa.fa-large,.btn .rst-content .code-block-caption .fa-large.headerlink,.btn .rst-content .eqno .fa-large.headerlink,.btn .rst-content .fa-large.admonition-title,.btn .rst-content code.download span.fa-large:first-child,.btn .rst-content dl dt .fa-large.headerlink,.btn .rst-content h1 .fa-large.headerlink,.btn .rst-content h2 .fa-large.headerlink,.btn .rst-content h3 .fa-large.headerlink,.btn .rst-content h4 .fa-large.headerlink,.btn .rst-content h5 .fa-large.headerlink,.btn .rst-content h6 .fa-large.headerlink,.btn .rst-content p .fa-large.headerlink,.btn .rst-content table>caption .fa-large.headerlink,.btn .rst-content tt.download span.fa-large:first-child,.btn .wy-menu-vertical li button.fa-large.toctree-expand,.nav .fa-large.icon,.nav .fa.fa-large,.nav .rst-content .code-block-caption .fa-large.headerlink,.nav .rst-content .eqno .fa-large.headerlink,.nav .rst-content .fa-large.admonition-title,.nav .rst-content code.download span.fa-large:first-child,.nav .rst-content dl dt .fa-large.headerlink,.nav .rst-content h1 .fa-large.headerlink,.nav .rst-content h2 .fa-large.headerlink,.nav .rst-content h3 .fa-large.headerlink,.nav .rst-content h4 .fa-large.headerlink,.nav .rst-content h5 .fa-large.headerlink,.nav .rst-content h6 .fa-large.headerlink,.nav .rst-content p .fa-large.headerlink,.nav .rst-content table>caption .fa-large.headerlink,.nav .rst-content tt.download span.fa-large:first-child,.nav .wy-menu-vertical li button.fa-large.toctree-expand,.rst-content .btn .fa-large.admonition-title,.rst-content .code-block-caption .btn .fa-large.headerlink,.rst-content .code-block-caption .nav .fa-large.headerlink,.rst-content .eqno .btn .fa-large.headerlink,.rst-content .eqno .nav .fa-large.headerlink,.rst-content .nav .fa-large.admonition-title,.rst-content code.download .btn span.fa-large:first-child,.rst-content code.download .nav span.fa-large:first-child,.rst-content dl dt .btn .fa-large.headerlink,.rst-content dl dt .nav .fa-large.headerlink,.rst-content h1 .btn .fa-large.headerlink,.rst-content h1 .nav .fa-large.headerlink,.rst-content h2 .btn .fa-large.headerlink,.rst-content h2 .nav .fa-large.headerlink,.rst-content h3 .btn .fa-large.headerlink,.rst-content h3 .nav .fa-large.headerlink,.rst-content h4 .btn .fa-large.headerlink,.rst-content h4 .nav .fa-large.headerlink,.rst-content h5 .btn .fa-large.headerlink,.rst-content h5 .nav .fa-large.headerlink,.rst-content h6 .btn .fa-large.headerlink,.rst-content h6 .nav .fa-large.headerlink,.rst-content p .btn .fa-large.headerlink,.rst-content p .nav .fa-large.headerlink,.rst-content table>caption .btn .fa-large.headerlink,.rst-content table>caption .nav .fa-large.headerlink,.rst-content tt.download .btn span.fa-large:first-child,.rst-content tt.download .nav span.fa-large:first-child,.wy-menu-vertical li .btn button.fa-large.toctree-expand,.wy-menu-vertical li .nav button.fa-large.toctree-expand{line-height:.9em}.btn .fa-spin.icon,.btn .fa.fa-spin,.btn .rst-content .code-block-caption .fa-spin.headerlink,.btn .rst-content .eqno .fa-spin.headerlink,.btn .rst-content .fa-spin.admonition-title,.btn .rst-content code.download span.fa-spin:first-child,.btn .rst-content dl dt .fa-spin.headerlink,.btn .rst-content h1 .fa-spin.headerlink,.btn .rst-content h2 .fa-spin.headerlink,.btn .rst-content h3 .fa-spin.headerlink,.btn .rst-content h4 .fa-spin.headerlink,.btn .rst-content h5 .fa-spin.headerlink,.btn .rst-content h6 .fa-spin.headerlink,.btn .rst-content p .fa-spin.headerlink,.btn .rst-content table>caption .fa-spin.headerlink,.btn .rst-content tt.download span.fa-spin:first-child,.btn .wy-menu-vertical li button.fa-spin.toctree-expand,.nav .fa-spin.icon,.nav .fa.fa-spin,.nav .rst-content .code-block-caption .fa-spin.headerlink,.nav .rst-content .eqno .fa-spin.headerlink,.nav .rst-content .fa-spin.admonition-title,.nav .rst-content code.download span.fa-spin:first-child,.nav .rst-content dl dt .fa-spin.headerlink,.nav .rst-content h1 .fa-spin.headerlink,.nav .rst-content h2 .fa-spin.headerlink,.nav .rst-content h3 .fa-spin.headerlink,.nav .rst-content h4 .fa-spin.headerlink,.nav .rst-content h5 .fa-spin.headerlink,.nav .rst-content h6 .fa-spin.headerlink,.nav .rst-content p .fa-spin.headerlink,.nav .rst-content table>caption .fa-spin.headerlink,.nav .rst-content tt.download span.fa-spin:first-child,.nav .wy-menu-vertical li button.fa-spin.toctree-expand,.rst-content .btn .fa-spin.admonition-title,.rst-content .code-block-caption .btn .fa-spin.headerlink,.rst-content .code-block-caption .nav .fa-spin.headerlink,.rst-content .eqno .btn .fa-spin.headerlink,.rst-content .eqno .nav .fa-spin.headerlink,.rst-content .nav .fa-spin.admonition-title,.rst-content code.download .btn span.fa-spin:first-child,.rst-content code.download .nav span.fa-spin:first-child,.rst-content dl dt .btn .fa-spin.headerlink,.rst-content dl dt .nav .fa-spin.headerlink,.rst-content h1 .btn .fa-spin.headerlink,.rst-content h1 .nav .fa-spin.headerlink,.rst-content h2 .btn .fa-spin.headerlink,.rst-content h2 .nav .fa-spin.headerlink,.rst-content h3 .btn .fa-spin.headerlink,.rst-content h3 .nav .fa-spin.headerlink,.rst-content h4 .btn .fa-spin.headerlink,.rst-content h4 .nav .fa-spin.headerlink,.rst-content h5 .btn .fa-spin.headerlink,.rst-content h5 .nav .fa-spin.headerlink,.rst-content h6 .btn .fa-spin.headerlink,.rst-content h6 .nav .fa-spin.headerlink,.rst-content p .btn .fa-spin.headerlink,.rst-content p .nav .fa-spin.headerlink,.rst-content table>caption .btn .fa-spin.headerlink,.rst-content table>caption .nav .fa-spin.headerlink,.rst-content tt.download .btn span.fa-spin:first-child,.rst-content tt.download .nav span.fa-spin:first-child,.wy-menu-vertical li .btn button.fa-spin.toctree-expand,.wy-menu-vertical li .nav button.fa-spin.toctree-expand{display:inline-block}.btn.fa:before,.btn.icon:before,.rst-content .btn.admonition-title:before,.rst-content .code-block-caption .btn.headerlink:before,.rst-content .eqno .btn.headerlink:before,.rst-content code.download span.btn:first-child:before,.rst-content dl dt .btn.headerlink:before,.rst-content h1 .btn.headerlink:before,.rst-content h2 .btn.headerlink:before,.rst-content h3 .btn.headerlink:before,.rst-content h4 .btn.headerlink:before,.rst-content h5 .btn.headerlink:before,.rst-content h6 .btn.headerlink:before,.rst-content p .btn.headerlink:before,.rst-content table>caption .btn.headerlink:before,.rst-content tt.download span.btn:first-child:before,.wy-menu-vertical li button.btn.toctree-expand:before{opacity:.5;-webkit-transition:opacity .05s ease-in;-moz-transition:opacity .05s ease-in;transition:opacity .05s ease-in}.btn.fa:hover:before,.btn.icon:hover:before,.rst-content .btn.admonition-title:hover:before,.rst-content .code-block-caption .btn.headerlink:hover:before,.rst-content .eqno .btn.headerlink:hover:before,.rst-content code.download span.btn:first-child:hover:before,.rst-content dl dt .btn.headerlink:hover:before,.rst-content h1 .btn.headerlink:hover:before,.rst-content h2 .btn.headerlink:hover:before,.rst-content h3 .btn.headerlink:hover:before,.rst-content h4 .btn.headerlink:hover:before,.rst-content h5 .btn.headerlink:hover:before,.rst-content h6 .btn.headerlink:hover:before,.rst-content p .btn.headerlink:hover:before,.rst-content table>caption .btn.headerlink:hover:before,.rst-content tt.download span.btn:first-child:hover:before,.wy-menu-vertical li button.btn.toctree-expand:hover:before{opacity:1}.btn-mini .fa:before,.btn-mini .icon:before,.btn-mini .rst-content .admonition-title:before,.btn-mini .rst-content .code-block-caption .headerlink:before,.btn-mini .rst-content .eqno .headerlink:before,.btn-mini .rst-content code.download span:first-child:before,.btn-mini .rst-content dl dt .headerlink:before,.btn-mini .rst-content h1 .headerlink:before,.btn-mini .rst-content h2 .headerlink:before,.btn-mini .rst-content h3 .headerlink:before,.btn-mini .rst-content h4 .headerlink:before,.btn-mini .rst-content h5 .headerlink:before,.btn-mini .rst-content h6 .headerlink:before,.btn-mini .rst-content p .headerlink:before,.btn-mini .rst-content table>caption .headerlink:before,.btn-mini .rst-content tt.download span:first-child:before,.btn-mini .wy-menu-vertical li button.toctree-expand:before,.rst-content .btn-mini .admonition-title:before,.rst-content .code-block-caption .btn-mini .headerlink:before,.rst-content .eqno .btn-mini .headerlink:before,.rst-content code.download .btn-mini span:first-child:before,.rst-content dl dt .btn-mini .headerlink:before,.rst-content h1 .btn-mini .headerlink:before,.rst-content h2 .btn-mini .headerlink:before,.rst-content h3 .btn-mini .headerlink:before,.rst-content h4 .btn-mini .headerlink:before,.rst-content h5 .btn-mini .headerlink:before,.rst-content h6 .btn-mini .headerlink:before,.rst-content p .btn-mini .headerlink:before,.rst-content table>caption .btn-mini .headerlink:before,.rst-content tt.download .btn-mini span:first-child:before,.wy-menu-vertical li .btn-mini button.toctree-expand:before{font-size:14px;vertical-align:-15%}.rst-content .admonition,.rst-content .admonition-todo,.rst-content .attention,.rst-content .caution,.rst-content .danger,.rst-content .error,.rst-content .hint,.rst-content .important,.rst-content .note,.rst-content .seealso,.rst-content .tip,.rst-content .warning,.wy-alert{padding:12px;line-height:24px;margin-bottom:24px;background:#e7f2fa}.rst-content .admonition-title,.wy-alert-title{font-weight:700;display:block;color:#fff;background:#6ab0de;padding:6px 12px;margin:-12px -12px 12px}.rst-content .danger,.rst-content .error,.rst-content .wy-alert-danger.admonition,.rst-content .wy-alert-danger.admonition-todo,.rst-content .wy-alert-danger.attention,.rst-content .wy-alert-danger.caution,.rst-content .wy-alert-danger.hint,.rst-content .wy-alert-danger.important,.rst-content .wy-alert-danger.note,.rst-content .wy-alert-danger.seealso,.rst-content .wy-alert-danger.tip,.rst-content .wy-alert-danger.warning,.wy-alert.wy-alert-danger{background:#fdf3f2}.rst-content .danger .admonition-title,.rst-content .danger .wy-alert-title,.rst-content .error .admonition-title,.rst-content .error .wy-alert-title,.rst-content .wy-alert-danger.admonition-todo .admonition-title,.rst-content .wy-alert-danger.admonition-todo .wy-alert-title,.rst-content .wy-alert-danger.admonition .admonition-title,.rst-content .wy-alert-danger.admonition .wy-alert-title,.rst-content .wy-alert-danger.attention .admonition-title,.rst-content .wy-alert-danger.attention .wy-alert-title,.rst-content .wy-alert-danger.caution .admonition-title,.rst-content .wy-alert-danger.caution .wy-alert-title,.rst-content .wy-alert-danger.hint .admonition-title,.rst-content .wy-alert-danger.hint .wy-alert-title,.rst-content .wy-alert-danger.important .admonition-title,.rst-content .wy-alert-danger.important .wy-alert-title,.rst-content .wy-alert-danger.note .admonition-title,.rst-content .wy-alert-danger.note .wy-alert-title,.rst-content .wy-alert-danger.seealso .admonition-title,.rst-content .wy-alert-danger.seealso .wy-alert-title,.rst-content .wy-alert-danger.tip .admonition-title,.rst-content .wy-alert-danger.tip .wy-alert-title,.rst-content .wy-alert-danger.warning .admonition-title,.rst-content .wy-alert-danger.warning .wy-alert-title,.rst-content .wy-alert.wy-alert-danger .admonition-title,.wy-alert.wy-alert-danger .rst-content .admonition-title,.wy-alert.wy-alert-danger .wy-alert-title{background:#f29f97}.rst-content .admonition-todo,.rst-content .attention,.rst-content .caution,.rst-content .warning,.rst-content .wy-alert-warning.admonition,.rst-content .wy-alert-warning.danger,.rst-content .wy-alert-warning.error,.rst-content .wy-alert-warning.hint,.rst-content .wy-alert-warning.important,.rst-content .wy-alert-warning.note,.rst-content .wy-alert-warning.seealso,.rst-content .wy-alert-warning.tip,.wy-alert.wy-alert-warning{background:#ffedcc}.rst-content .admonition-todo .admonition-title,.rst-content .admonition-todo .wy-alert-title,.rst-content .attention .admonition-title,.rst-content .attention .wy-alert-title,.rst-content .caution .admonition-title,.rst-content .caution .wy-alert-title,.rst-content .warning .admonition-title,.rst-content .warning .wy-alert-title,.rst-content .wy-alert-warning.admonition .admonition-title,.rst-content .wy-alert-warning.admonition .wy-alert-title,.rst-content .wy-alert-warning.danger .admonition-title,.rst-content .wy-alert-warning.danger .wy-alert-title,.rst-content .wy-alert-warning.error .admonition-title,.rst-content .wy-alert-warning.error .wy-alert-title,.rst-content .wy-alert-warning.hint .admonition-title,.rst-content .wy-alert-warning.hint .wy-alert-title,.rst-content .wy-alert-warning.important .admonition-title,.rst-content .wy-alert-warning.important .wy-alert-title,.rst-content .wy-alert-warning.note .admonition-title,.rst-content .wy-alert-warning.note .wy-alert-title,.rst-content .wy-alert-warning.seealso .admonition-title,.rst-content .wy-alert-warning.seealso .wy-alert-title,.rst-content .wy-alert-warning.tip .admonition-title,.rst-content .wy-alert-warning.tip .wy-alert-title,.rst-content .wy-alert.wy-alert-warning .admonition-title,.wy-alert.wy-alert-warning .rst-content .admonition-title,.wy-alert.wy-alert-warning .wy-alert-title{background:#f0b37e}.rst-content .note,.rst-content .seealso,.rst-content .wy-alert-info.admonition,.rst-content .wy-alert-info.admonition-todo,.rst-content .wy-alert-info.attention,.rst-content .wy-alert-info.caution,.rst-content .wy-alert-info.danger,.rst-content .wy-alert-info.error,.rst-content .wy-alert-info.hint,.rst-content .wy-alert-info.important,.rst-content .wy-alert-info.tip,.rst-content .wy-alert-info.warning,.wy-alert.wy-alert-info{background:#e7f2fa}.rst-content .note .admonition-title,.rst-content .note .wy-alert-title,.rst-content .seealso .admonition-title,.rst-content .seealso .wy-alert-title,.rst-content .wy-alert-info.admonition-todo .admonition-title,.rst-content .wy-alert-info.admonition-todo .wy-alert-title,.rst-content .wy-alert-info.admonition .admonition-title,.rst-content .wy-alert-info.admonition .wy-alert-title,.rst-content .wy-alert-info.attention .admonition-title,.rst-content .wy-alert-info.attention .wy-alert-title,.rst-content .wy-alert-info.caution .admonition-title,.rst-content .wy-alert-info.caution .wy-alert-title,.rst-content .wy-alert-info.danger .admonition-title,.rst-content .wy-alert-info.danger .wy-alert-title,.rst-content .wy-alert-info.error .admonition-title,.rst-content .wy-alert-info.error .wy-alert-title,.rst-content .wy-alert-info.hint .admonition-title,.rst-content .wy-alert-info.hint .wy-alert-title,.rst-content .wy-alert-info.important .admonition-title,.rst-content .wy-alert-info.important .wy-alert-title,.rst-content .wy-alert-info.tip .admonition-title,.rst-content .wy-alert-info.tip .wy-alert-title,.rst-content .wy-alert-info.warning .admonition-title,.rst-content .wy-alert-info.warning .wy-alert-title,.rst-content .wy-alert.wy-alert-info .admonition-title,.wy-alert.wy-alert-info .rst-content .admonition-title,.wy-alert.wy-alert-info .wy-alert-title{background:#6ab0de}.rst-content .hint,.rst-content .important,.rst-content .tip,.rst-content .wy-alert-success.admonition,.rst-content .wy-alert-success.admonition-todo,.rst-content .wy-alert-success.attention,.rst-content .wy-alert-success.caution,.rst-content .wy-alert-success.danger,.rst-content .wy-alert-success.error,.rst-content .wy-alert-success.note,.rst-content .wy-alert-success.seealso,.rst-content .wy-alert-success.warning,.wy-alert.wy-alert-success{background:#dbfaf4}.rst-content .hint .admonition-title,.rst-content .hint .wy-alert-title,.rst-content .important .admonition-title,.rst-content .important .wy-alert-title,.rst-content .tip .admonition-title,.rst-content .tip .wy-alert-title,.rst-content .wy-alert-success.admonition-todo .admonition-title,.rst-content .wy-alert-success.admonition-todo .wy-alert-title,.rst-content .wy-alert-success.admonition .admonition-title,.rst-content .wy-alert-success.admonition .wy-alert-title,.rst-content .wy-alert-success.attention .admonition-title,.rst-content .wy-alert-success.attention .wy-alert-title,.rst-content .wy-alert-success.caution .admonition-title,.rst-content .wy-alert-success.caution .wy-alert-title,.rst-content .wy-alert-success.danger .admonition-title,.rst-content .wy-alert-success.danger .wy-alert-title,.rst-content .wy-alert-success.error .admonition-title,.rst-content .wy-alert-success.error .wy-alert-title,.rst-content .wy-alert-success.note .admonition-title,.rst-content .wy-alert-success.note .wy-alert-title,.rst-content .wy-alert-success.seealso .admonition-title,.rst-content .wy-alert-success.seealso .wy-alert-title,.rst-content .wy-alert-success.warning .admonition-title,.rst-content .wy-alert-success.warning .wy-alert-title,.rst-content .wy-alert.wy-alert-success .admonition-title,.wy-alert.wy-alert-success .rst-content .admonition-title,.wy-alert.wy-alert-success .wy-alert-title{background:#1abc9c}.rst-content .wy-alert-neutral.admonition,.rst-content .wy-alert-neutral.admonition-todo,.rst-content .wy-alert-neutral.attention,.rst-content .wy-alert-neutral.caution,.rst-content .wy-alert-neutral.danger,.rst-content .wy-alert-neutral.error,.rst-content .wy-alert-neutral.hint,.rst-content .wy-alert-neutral.important,.rst-content .wy-alert-neutral.note,.rst-content .wy-alert-neutral.seealso,.rst-content .wy-alert-neutral.tip,.rst-content .wy-alert-neutral.warning,.wy-alert.wy-alert-neutral{background:#f3f6f6}.rst-content .wy-alert-neutral.admonition-todo .admonition-title,.rst-content .wy-alert-neutral.admonition-todo .wy-alert-title,.rst-content .wy-alert-neutral.admonition .admonition-title,.rst-content .wy-alert-neutral.admonition .wy-alert-title,.rst-content .wy-alert-neutral.attention .admonition-title,.rst-content .wy-alert-neutral.attention .wy-alert-title,.rst-content .wy-alert-neutral.caution .admonition-title,.rst-content .wy-alert-neutral.caution .wy-alert-title,.rst-content .wy-alert-neutral.danger .admonition-title,.rst-content .wy-alert-neutral.danger .wy-alert-title,.rst-content .wy-alert-neutral.error .admonition-title,.rst-content .wy-alert-neutral.error .wy-alert-title,.rst-content .wy-alert-neutral.hint .admonition-title,.rst-content .wy-alert-neutral.hint .wy-alert-title,.rst-content .wy-alert-neutral.important .admonition-title,.rst-content .wy-alert-neutral.important .wy-alert-title,.rst-content .wy-alert-neutral.note .admonition-title,.rst-content .wy-alert-neutral.note .wy-alert-title,.rst-content .wy-alert-neutral.seealso .admonition-title,.rst-content .wy-alert-neutral.seealso .wy-alert-title,.rst-content .wy-alert-neutral.tip .admonition-title,.rst-content .wy-alert-neutral.tip .wy-alert-title,.rst-content .wy-alert-neutral.warning .admonition-title,.rst-content .wy-alert-neutral.warning .wy-alert-title,.rst-content .wy-alert.wy-alert-neutral .admonition-title,.wy-alert.wy-alert-neutral .rst-content .admonition-title,.wy-alert.wy-alert-neutral .wy-alert-title{color:#404040;background:#e1e4e5}.rst-content .wy-alert-neutral.admonition-todo a,.rst-content .wy-alert-neutral.admonition a,.rst-content .wy-alert-neutral.attention a,.rst-content .wy-alert-neutral.caution a,.rst-content .wy-alert-neutral.danger a,.rst-content .wy-alert-neutral.error a,.rst-content .wy-alert-neutral.hint a,.rst-content .wy-alert-neutral.important a,.rst-content .wy-alert-neutral.note a,.rst-content .wy-alert-neutral.seealso a,.rst-content .wy-alert-neutral.tip a,.rst-content .wy-alert-neutral.warning a,.wy-alert.wy-alert-neutral a{color:#2980b9}.rst-content .admonition-todo p:last-child,.rst-content .admonition p:last-child,.rst-content .attention p:last-child,.rst-content .caution p:last-child,.rst-content .danger p:last-child,.rst-content .error p:last-child,.rst-content .hint p:last-child,.rst-content .important p:last-child,.rst-content .note p:last-child,.rst-content .seealso p:last-child,.rst-content .tip p:last-child,.rst-content .warning p:last-child,.wy-alert p:last-child{margin-bottom:0}.wy-tray-container{position:fixed;bottom:0;left:0;z-index:600}.wy-tray-container li{display:block;width:300px;background:transparent;color:#fff;text-align:center;box-shadow:0 5px 5px 0 rgba(0,0,0,.1);padding:0 24px;min-width:20%;opacity:0;height:0;line-height:56px;overflow:hidden;-webkit-transition:all .3s ease-in;-moz-transition:all .3s ease-in;transition:all .3s ease-in}.wy-tray-container li.wy-tray-item-success{background:#27ae60}.wy-tray-container li.wy-tray-item-info{background:#2980b9}.wy-tray-container li.wy-tray-item-warning{background:#e67e22}.wy-tray-container li.wy-tray-item-danger{background:#e74c3c}.wy-tray-container li.on{opacity:1;height:56px}@media screen and (max-width:768px){.wy-tray-container{bottom:auto;top:0;width:100%}.wy-tray-container li{width:100%}}button{font-size:100%;margin:0;vertical-align:baseline;*vertical-align:middle;cursor:pointer;line-height:normal;-webkit-appearance:button;*overflow:visible}button::-moz-focus-inner,input::-moz-focus-inner{border:0;padding:0}button[disabled]{cursor:default}.btn{display:inline-block;border-radius:2px;line-height:normal;white-space:nowrap;text-align:center;cursor:pointer;font-size:100%;padding:6px 12px 8px;color:#fff;border:1px solid rgba(0,0,0,.1);background-color:#27ae60;text-decoration:none;font-weight:400;font-family:Lato,proxima-nova,Helvetica Neue,Arial,sans-serif;box-shadow:inset 0 1px 2px -1px hsla(0,0%,100%,.5),inset 0 -2px 0 0 rgba(0,0,0,.1);outline-none:false;vertical-align:middle;*display:inline;zoom:1;-webkit-user-drag:none;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;-webkit-transition:all .1s linear;-moz-transition:all .1s linear;transition:all .1s linear}.btn-hover{background:#2e8ece;color:#fff}.btn:hover{background:#2cc36b;color:#fff}.btn:focus{background:#2cc36b;outline:0}.btn:active{box-shadow:inset 0 -1px 0 0 rgba(0,0,0,.05),inset 0 2px 0 0 rgba(0,0,0,.1);padding:8px 12px 6px}.btn:visited{color:#fff}.btn-disabled,.btn-disabled:active,.btn-disabled:focus,.btn-disabled:hover,.btn:disabled{background-image:none;filter:progid:DXImageTransform.Microsoft.gradient(enabled = false);filter:alpha(opacity=40);opacity:.4;cursor:not-allowed;box-shadow:none}.btn::-moz-focus-inner{padding:0;border:0}.btn-small{font-size:80%}.btn-info{background-color:#2980b9!important}.btn-info:hover{background-color:#2e8ece!important}.btn-neutral{background-color:#f3f6f6!important;color:#404040!important}.btn-neutral:hover{background-color:#e5ebeb!important;color:#404040}.btn-neutral:visited{color:#404040!important}.btn-success{background-color:#27ae60!important}.btn-success:hover{background-color:#295!important}.btn-danger{background-color:#e74c3c!important}.btn-danger:hover{background-color:#ea6153!important}.btn-warning{background-color:#e67e22!important}.btn-warning:hover{background-color:#e98b39!important}.btn-invert{background-color:#222}.btn-invert:hover{background-color:#2f2f2f!important}.btn-link{background-color:transparent!important;color:#2980b9;box-shadow:none;border-color:transparent!important}.btn-link:active,.btn-link:hover{background-color:transparent!important;color:#409ad5!important;box-shadow:none}.btn-link:visited{color:#9b59b6}.wy-btn-group .btn,.wy-control .btn{vertical-align:middle}.wy-btn-group{margin-bottom:24px;*zoom:1}.wy-btn-group:after,.wy-btn-group:before{display:table;content:""}.wy-btn-group:after{clear:both}.wy-dropdown{position:relative;display:inline-block}.wy-dropdown-active .wy-dropdown-menu{display:block}.wy-dropdown-menu{position:absolute;left:0;display:none;float:left;top:100%;min-width:100%;background:#fcfcfc;z-index:100;border:1px solid #cfd7dd;box-shadow:0 2px 2px 0 rgba(0,0,0,.1);padding:12px}.wy-dropdown-menu>dd>a{display:block;clear:both;color:#404040;white-space:nowrap;font-size:90%;padding:0 12px;cursor:pointer}.wy-dropdown-menu>dd>a:hover{background:#2980b9;color:#fff}.wy-dropdown-menu>dd.divider{border-top:1px solid #cfd7dd;margin:6px 0}.wy-dropdown-menu>dd.search{padding-bottom:12px}.wy-dropdown-menu>dd.search input[type=search]{width:100%}.wy-dropdown-menu>dd.call-to-action{background:#e3e3e3;text-transform:uppercase;font-weight:500;font-size:80%}.wy-dropdown-menu>dd.call-to-action:hover{background:#e3e3e3}.wy-dropdown-menu>dd.call-to-action .btn{color:#fff}.wy-dropdown.wy-dropdown-up .wy-dropdown-menu{bottom:100%;top:auto;left:auto;right:0}.wy-dropdown.wy-dropdown-bubble .wy-dropdown-menu{background:#fcfcfc;margin-top:2px}.wy-dropdown.wy-dropdown-bubble .wy-dropdown-menu a{padding:6px 12px}.wy-dropdown.wy-dropdown-bubble .wy-dropdown-menu a:hover{background:#2980b9;color:#fff}.wy-dropdown.wy-dropdown-left .wy-dropdown-menu{right:0;left:auto;text-align:right}.wy-dropdown-arrow:before{content:" ";border-bottom:5px solid #f5f5f5;border-left:5px solid transparent;border-right:5px solid transparent;position:absolute;display:block;top:-4px;left:50%;margin-left:-3px}.wy-dropdown-arrow.wy-dropdown-arrow-left:before{left:11px}.wy-form-stacked select{display:block}.wy-form-aligned .wy-help-inline,.wy-form-aligned input,.wy-form-aligned label,.wy-form-aligned select,.wy-form-aligned textarea{display:inline-block;*display:inline;*zoom:1;vertical-align:middle}.wy-form-aligned .wy-control-group>label{display:inline-block;vertical-align:middle;width:10em;margin:6px 12px 0 0;float:left}.wy-form-aligned .wy-control{float:left}.wy-form-aligned .wy-control label{display:block}.wy-form-aligned .wy-control select{margin-top:6px}fieldset{margin:0}fieldset,legend{border:0;padding:0}legend{width:100%;white-space:normal;margin-bottom:24px;font-size:150%;*margin-left:-7px}label,legend{display:block}label{margin:0 0 .3125em;color:#333;font-size:90%}input,select,textarea{font-size:100%;margin:0;vertical-align:baseline;*vertical-align:middle}.wy-control-group{margin-bottom:24px;max-width:1200px;margin-left:auto;margin-right:auto;*zoom:1}.wy-control-group:after,.wy-control-group:before{display:table;content:""}.wy-control-group:after{clear:both}.wy-control-group.wy-control-group-required>label:after{content:" *";color:#e74c3c}.wy-control-group .wy-form-full,.wy-control-group .wy-form-halves,.wy-control-group .wy-form-thirds{padding-bottom:12px}.wy-control-group .wy-form-full input[type=color],.wy-control-group .wy-form-full input[type=date],.wy-control-group .wy-form-full input[type=datetime-local],.wy-control-group .wy-form-full input[type=datetime],.wy-control-group .wy-form-full input[type=email],.wy-control-group .wy-form-full input[type=month],.wy-control-group .wy-form-full input[type=number],.wy-control-group .wy-form-full input[type=password],.wy-control-group .wy-form-full input[type=search],.wy-control-group .wy-form-full input[type=tel],.wy-control-group .wy-form-full input[type=text],.wy-control-group .wy-form-full input[type=time],.wy-control-group .wy-form-full input[type=url],.wy-control-group .wy-form-full input[type=week],.wy-control-group .wy-form-full select,.wy-control-group .wy-form-halves input[type=color],.wy-control-group .wy-form-halves input[type=date],.wy-control-group .wy-form-halves input[type=datetime-local],.wy-control-group .wy-form-halves input[type=datetime],.wy-control-group .wy-form-halves input[type=email],.wy-control-group .wy-form-halves input[type=month],.wy-control-group .wy-form-halves input[type=number],.wy-control-group .wy-form-halves input[type=password],.wy-control-group .wy-form-halves input[type=search],.wy-control-group .wy-form-halves input[type=tel],.wy-control-group .wy-form-halves input[type=text],.wy-control-group .wy-form-halves input[type=time],.wy-control-group .wy-form-halves input[type=url],.wy-control-group .wy-form-halves input[type=week],.wy-control-group .wy-form-halves select,.wy-control-group .wy-form-thirds input[type=color],.wy-control-group .wy-form-thirds input[type=date],.wy-control-group .wy-form-thirds input[type=datetime-local],.wy-control-group .wy-form-thirds input[type=datetime],.wy-control-group .wy-form-thirds input[type=email],.wy-control-group .wy-form-thirds input[type=month],.wy-control-group .wy-form-thirds input[type=number],.wy-control-group .wy-form-thirds input[type=password],.wy-control-group .wy-form-thirds input[type=search],.wy-control-group .wy-form-thirds input[type=tel],.wy-control-group .wy-form-thirds input[type=text],.wy-control-group .wy-form-thirds input[type=time],.wy-control-group .wy-form-thirds input[type=url],.wy-control-group .wy-form-thirds input[type=week],.wy-control-group .wy-form-thirds select{width:100%}.wy-control-group .wy-form-full{float:left;display:block;width:100%;margin-right:0}.wy-control-group .wy-form-full:last-child{margin-right:0}.wy-control-group .wy-form-halves{float:left;display:block;margin-right:2.35765%;width:48.82117%}.wy-control-group .wy-form-halves:last-child,.wy-control-group .wy-form-halves:nth-of-type(2n){margin-right:0}.wy-control-group .wy-form-halves:nth-of-type(odd){clear:left}.wy-control-group .wy-form-thirds{float:left;display:block;margin-right:2.35765%;width:31.76157%}.wy-control-group .wy-form-thirds:last-child,.wy-control-group .wy-form-thirds:nth-of-type(3n){margin-right:0}.wy-control-group .wy-form-thirds:nth-of-type(3n+1){clear:left}.wy-control-group.wy-control-group-no-input .wy-control,.wy-control-no-input{margin:6px 0 0;font-size:90%}.wy-control-no-input{display:inline-block}.wy-control-group.fluid-input input[type=color],.wy-control-group.fluid-input input[type=date],.wy-control-group.fluid-input input[type=datetime-local],.wy-control-group.fluid-input input[type=datetime],.wy-control-group.fluid-input input[type=email],.wy-control-group.fluid-input input[type=month],.wy-control-group.fluid-input input[type=number],.wy-control-group.fluid-input input[type=password],.wy-control-group.fluid-input input[type=search],.wy-control-group.fluid-input input[type=tel],.wy-control-group.fluid-input input[type=text],.wy-control-group.fluid-input input[type=time],.wy-control-group.fluid-input input[type=url],.wy-control-group.fluid-input input[type=week]{width:100%}.wy-form-message-inline{padding-left:.3em;color:#666;font-size:90%}.wy-form-message{display:block;color:#999;font-size:70%;margin-top:.3125em;font-style:italic}.wy-form-message p{font-size:inherit;font-style:italic;margin-bottom:6px}.wy-form-message p:last-child{margin-bottom:0}input{line-height:normal}input[type=button],input[type=reset],input[type=submit]{-webkit-appearance:button;cursor:pointer;font-family:Lato,proxima-nova,Helvetica Neue,Arial,sans-serif;*overflow:visible}input[type=color],input[type=date],input[type=datetime-local],input[type=datetime],input[type=email],input[type=month],input[type=number],input[type=password],input[type=search],input[type=tel],input[type=text],input[type=time],input[type=url],input[type=week]{-webkit-appearance:none;padding:6px;display:inline-block;border:1px solid #ccc;font-size:80%;font-family:Lato,proxima-nova,Helvetica Neue,Arial,sans-serif;box-shadow:inset 0 1px 3px #ddd;border-radius:0;-webkit-transition:border .3s linear;-moz-transition:border .3s linear;transition:border .3s linear}input[type=datetime-local]{padding:.34375em .625em}input[disabled]{cursor:default}input[type=checkbox],input[type=radio]{padding:0;margin-right:.3125em;*height:13px;*width:13px}input[type=checkbox],input[type=radio],input[type=search]{-webkit-box-sizing:border-box;-moz-box-sizing:border-box;box-sizing:border-box}input[type=search]::-webkit-search-cancel-button,input[type=search]::-webkit-search-decoration{-webkit-appearance:none}input[type=color]:focus,input[type=date]:focus,input[type=datetime-local]:focus,input[type=datetime]:focus,input[type=email]:focus,input[type=month]:focus,input[type=number]:focus,input[type=password]:focus,input[type=search]:focus,input[type=tel]:focus,input[type=text]:focus,input[type=time]:focus,input[type=url]:focus,input[type=week]:focus{outline:0;outline:thin dotted\9;border-color:#333}input.no-focus:focus{border-color:#ccc!important}input[type=checkbox]:focus,input[type=file]:focus,input[type=radio]:focus{outline:thin dotted #333;outline:1px auto #129fea}input[type=color][disabled],input[type=date][disabled],input[type=datetime-local][disabled],input[type=datetime][disabled],input[type=email][disabled],input[type=month][disabled],input[type=number][disabled],input[type=password][disabled],input[type=search][disabled],input[type=tel][disabled],input[type=text][disabled],input[type=time][disabled],input[type=url][disabled],input[type=week][disabled]{cursor:not-allowed;background-color:#fafafa}input:focus:invalid,select:focus:invalid,textarea:focus:invalid{color:#e74c3c;border:1px solid #e74c3c}input:focus:invalid:focus,select:focus:invalid:focus,textarea:focus:invalid:focus{border-color:#e74c3c}input[type=checkbox]:focus:invalid:focus,input[type=file]:focus:invalid:focus,input[type=radio]:focus:invalid:focus{outline-color:#e74c3c}input.wy-input-large{padding:12px;font-size:100%}textarea{overflow:auto;vertical-align:top;width:100%;font-family:Lato,proxima-nova,Helvetica Neue,Arial,sans-serif}select,textarea{padding:.5em .625em;display:inline-block;border:1px solid #ccc;font-size:80%;box-shadow:inset 0 1px 3px #ddd;-webkit-transition:border .3s linear;-moz-transition:border .3s linear;transition:border .3s linear}select{border:1px solid #ccc;background-color:#fff}select[multiple]{height:auto}select:focus,textarea:focus{outline:0}input[readonly],select[disabled],select[readonly],textarea[disabled],textarea[readonly]{cursor:not-allowed;background-color:#fafafa}input[type=checkbox][disabled],input[type=radio][disabled]{cursor:not-allowed}.wy-checkbox,.wy-radio{margin:6px 0;color:#404040;display:block}.wy-checkbox input,.wy-radio input{vertical-align:baseline}.wy-form-message-inline{display:inline-block;*display:inline;*zoom:1;vertical-align:middle}.wy-input-prefix,.wy-input-suffix{white-space:nowrap;padding:6px}.wy-input-prefix .wy-input-context,.wy-input-suffix .wy-input-context{line-height:27px;padding:0 8px;display:inline-block;font-size:80%;background-color:#f3f6f6;border:1px solid #ccc;color:#999}.wy-input-suffix .wy-input-context{border-left:0}.wy-input-prefix .wy-input-context{border-right:0}.wy-switch{position:relative;display:block;height:24px;margin-top:12px;cursor:pointer}.wy-switch:before{left:0;top:0;width:36px;height:12px;background:#ccc}.wy-switch:after,.wy-switch:before{position:absolute;content:"";display:block;border-radius:4px;-webkit-transition:all .2s ease-in-out;-moz-transition:all .2s ease-in-out;transition:all .2s ease-in-out}.wy-switch:after{width:18px;height:18px;background:#999;left:-3px;top:-3px}.wy-switch span{position:absolute;left:48px;display:block;font-size:12px;color:#ccc;line-height:1}.wy-switch.active:before{background:#1e8449}.wy-switch.active:after{left:24px;background:#27ae60}.wy-switch.disabled{cursor:not-allowed;opacity:.8}.wy-control-group.wy-control-group-error .wy-form-message,.wy-control-group.wy-control-group-error>label{color:#e74c3c}.wy-control-group.wy-control-group-error input[type=color],.wy-control-group.wy-control-group-error input[type=date],.wy-control-group.wy-control-group-error input[type=datetime-local],.wy-control-group.wy-control-group-error input[type=datetime],.wy-control-group.wy-control-group-error input[type=email],.wy-control-group.wy-control-group-error input[type=month],.wy-control-group.wy-control-group-error input[type=number],.wy-control-group.wy-control-group-error input[type=password],.wy-control-group.wy-control-group-error input[type=search],.wy-control-group.wy-control-group-error input[type=tel],.wy-control-group.wy-control-group-error input[type=text],.wy-control-group.wy-control-group-error input[type=time],.wy-control-group.wy-control-group-error input[type=url],.wy-control-group.wy-control-group-error input[type=week],.wy-control-group.wy-control-group-error textarea{border:1px solid #e74c3c}.wy-inline-validate{white-space:nowrap}.wy-inline-validate .wy-input-context{padding:.5em .625em;display:inline-block;font-size:80%}.wy-inline-validate.wy-inline-validate-success .wy-input-context{color:#27ae60}.wy-inline-validate.wy-inline-validate-danger .wy-input-context{color:#e74c3c}.wy-inline-validate.wy-inline-validate-warning .wy-input-context{color:#e67e22}.wy-inline-validate.wy-inline-validate-info .wy-input-context{color:#2980b9}.rotate-90{-webkit-transform:rotate(90deg);-moz-transform:rotate(90deg);-ms-transform:rotate(90deg);-o-transform:rotate(90deg);transform:rotate(90deg)}.rotate-180{-webkit-transform:rotate(180deg);-moz-transform:rotate(180deg);-ms-transform:rotate(180deg);-o-transform:rotate(180deg);transform:rotate(180deg)}.rotate-270{-webkit-transform:rotate(270deg);-moz-transform:rotate(270deg);-ms-transform:rotate(270deg);-o-transform:rotate(270deg);transform:rotate(270deg)}.mirror{-webkit-transform:scaleX(-1);-moz-transform:scaleX(-1);-ms-transform:scaleX(-1);-o-transform:scaleX(-1);transform:scaleX(-1)}.mirror.rotate-90{-webkit-transform:scaleX(-1) rotate(90deg);-moz-transform:scaleX(-1) rotate(90deg);-ms-transform:scaleX(-1) rotate(90deg);-o-transform:scaleX(-1) rotate(90deg);transform:scaleX(-1) rotate(90deg)}.mirror.rotate-180{-webkit-transform:scaleX(-1) rotate(180deg);-moz-transform:scaleX(-1) rotate(180deg);-ms-transform:scaleX(-1) rotate(180deg);-o-transform:scaleX(-1) rotate(180deg);transform:scaleX(-1) rotate(180deg)}.mirror.rotate-270{-webkit-transform:scaleX(-1) rotate(270deg);-moz-transform:scaleX(-1) rotate(270deg);-ms-transform:scaleX(-1) rotate(270deg);-o-transform:scaleX(-1) rotate(270deg);transform:scaleX(-1) rotate(270deg)}@media only screen and (max-width:480px){.wy-form button[type=submit]{margin:.7em 0 0}.wy-form input[type=color],.wy-form input[type=date],.wy-form input[type=datetime-local],.wy-form input[type=datetime],.wy-form input[type=email],.wy-form input[type=month],.wy-form input[type=number],.wy-form input[type=password],.wy-form input[type=search],.wy-form input[type=tel],.wy-form input[type=text],.wy-form input[type=time],.wy-form input[type=url],.wy-form input[type=week],.wy-form label{margin-bottom:.3em;display:block}.wy-form input[type=color],.wy-form input[type=date],.wy-form input[type=datetime-local],.wy-form input[type=datetime],.wy-form input[type=email],.wy-form input[type=month],.wy-form input[type=number],.wy-form input[type=password],.wy-form input[type=search],.wy-form input[type=tel],.wy-form input[type=time],.wy-form input[type=url],.wy-form input[type=week]{margin-bottom:0}.wy-form-aligned .wy-control-group label{margin-bottom:.3em;text-align:left;display:block;width:100%}.wy-form-aligned .wy-control{margin:1.5em 0 0}.wy-form-message,.wy-form-message-inline,.wy-form .wy-help-inline{display:block;font-size:80%;padding:6px 0}}@media screen and (max-width:768px){.tablet-hide{display:none}}@media screen and (max-width:480px){.mobile-hide{display:none}}.float-left{float:left}.float-right{float:right}.full-width{width:100%}.rst-content table.docutils,.rst-content table.field-list,.wy-table{border-collapse:collapse;border-spacing:0;empty-cells:show;margin-bottom:24px}.rst-content table.docutils caption,.rst-content table.field-list caption,.wy-table caption{color:#000;font:italic 85%/1 arial,sans-serif;padding:1em 0;text-align:center}.rst-content table.docutils td,.rst-content table.docutils th,.rst-content table.field-list td,.rst-content table.field-list th,.wy-table td,.wy-table th{font-size:90%;margin:0;overflow:visible;padding:8px 16px}.rst-content table.docutils td:first-child,.rst-content table.docutils th:first-child,.rst-content table.field-list td:first-child,.rst-content table.field-list th:first-child,.wy-table td:first-child,.wy-table th:first-child{border-left-width:0}.rst-content table.docutils thead,.rst-content table.field-list thead,.wy-table thead{color:#000;text-align:left;vertical-align:bottom;white-space:nowrap}.rst-content table.docutils thead th,.rst-content table.field-list thead th,.wy-table thead th{font-weight:700;border-bottom:2px solid #e1e4e5}.rst-content table.docutils td,.rst-content table.field-list td,.wy-table td{background-color:transparent;vertical-align:middle}.rst-content table.docutils td p,.rst-content table.field-list td p,.wy-table td p{line-height:18px}.rst-content table.docutils td p:last-child,.rst-content table.field-list td p:last-child,.wy-table td p:last-child{margin-bottom:0}.rst-content table.docutils .wy-table-cell-min,.rst-content table.field-list .wy-table-cell-min,.wy-table .wy-table-cell-min{width:1%;padding-right:0}.rst-content table.docutils .wy-table-cell-min input[type=checkbox],.rst-content table.field-list .wy-table-cell-min input[type=checkbox],.wy-table .wy-table-cell-min input[type=checkbox]{margin:0}.wy-table-secondary{color:grey;font-size:90%}.wy-table-tertiary{color:grey;font-size:80%}.rst-content table.docutils:not(.field-list) tr:nth-child(2n-1) td,.wy-table-backed,.wy-table-odd td,.wy-table-striped tr:nth-child(2n-1) td{background-color:#f3f6f6}.rst-content table.docutils,.wy-table-bordered-all{border:1px solid #e1e4e5}.rst-content table.docutils td,.wy-table-bordered-all td{border-bottom:1px solid #e1e4e5;border-left:1px solid #e1e4e5}.rst-content table.docutils tbody>tr:last-child td,.wy-table-bordered-all tbody>tr:last-child td{border-bottom-width:0}.wy-table-bordered{border:1px solid #e1e4e5}.wy-table-bordered-rows td{border-bottom:1px solid #e1e4e5}.wy-table-bordered-rows tbody>tr:last-child td{border-bottom-width:0}.wy-table-horizontal td,.wy-table-horizontal th{border-width:0 0 1px;border-bottom:1px solid #e1e4e5}.wy-table-horizontal tbody>tr:last-child td{border-bottom-width:0}.wy-table-responsive{margin-bottom:24px;max-width:100%;overflow:auto}.wy-table-responsive table{margin-bottom:0!important}.wy-table-responsive table td,.wy-table-responsive table th{white-space:nowrap}a{color:#2980b9;text-decoration:none;cursor:pointer}a:hover{color:#3091d1}a:visited{color:#9b59b6}html{height:100%}body,html{overflow-x:hidden}body{font-family:Lato,proxima-nova,Helvetica Neue,Arial,sans-serif;font-weight:400;color:#404040;min-height:100%;background:#edf0f2}.wy-text-left{text-align:left}.wy-text-center{text-align:center}.wy-text-right{text-align:right}.wy-text-large{font-size:120%}.wy-text-normal{font-size:100%}.wy-text-small,small{font-size:80%}.wy-text-strike{text-decoration:line-through}.wy-text-warning{color:#e67e22!important}a.wy-text-warning:hover{color:#eb9950!important}.wy-text-info{color:#2980b9!important}a.wy-text-info:hover{color:#409ad5!important}.wy-text-success{color:#27ae60!important}a.wy-text-success:hover{color:#36d278!important}.wy-text-danger{color:#e74c3c!important}a.wy-text-danger:hover{color:#ed7669!important}.wy-text-neutral{color:#404040!important}a.wy-text-neutral:hover{color:#595959!important}.rst-content .toctree-wrapper>p.caption,h1,h2,h3,h4,h5,h6,legend{margin-top:0;font-weight:700;font-family:Roboto Slab,ff-tisa-web-pro,Georgia,Arial,sans-serif}p{line-height:24px;font-size:16px;margin:0 0 24px}h1{font-size:175%}.rst-content .toctree-wrapper>p.caption,h2{font-size:150%}h3{font-size:125%}h4{font-size:115%}h5{font-size:110%}h6{font-size:100%}hr{display:block;height:1px;border:0;border-top:1px solid #e1e4e5;margin:24px 0;padding:0}.rst-content code,.rst-content tt,code{white-space:nowrap;max-width:100%;background:#fff;border:1px solid #e1e4e5;font-size:75%;padding:0 5px;font-family:SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,Courier,monospace;color:#e74c3c;overflow-x:auto}.rst-content tt.code-large,code.code-large{font-size:90%}.rst-content .section ul,.rst-content .toctree-wrapper ul,.rst-content section ul,.wy-plain-list-disc,article ul{list-style:disc;line-height:24px;margin-bottom:24px}.rst-content .section ul li,.rst-content .toctree-wrapper ul li,.rst-content section ul li,.wy-plain-list-disc li,article ul li{list-style:disc;margin-left:24px}.rst-content .section ul li p:last-child,.rst-content .section ul li ul,.rst-content .toctree-wrapper ul li p:last-child,.rst-content .toctree-wrapper ul li ul,.rst-content section ul li p:last-child,.rst-content section ul li ul,.wy-plain-list-disc li p:last-child,.wy-plain-list-disc li ul,article ul li p:last-child,article ul li ul{margin-bottom:0}.rst-content .section ul li li,.rst-content .toctree-wrapper ul li li,.rst-content section ul li li,.wy-plain-list-disc li li,article ul li li{list-style:circle}.rst-content .section ul li li li,.rst-content .toctree-wrapper ul li li li,.rst-content section ul li li li,.wy-plain-list-disc li li li,article ul li li li{list-style:square}.rst-content .section ul li ol li,.rst-content .toctree-wrapper ul li ol li,.rst-content section ul li ol li,.wy-plain-list-disc li ol li,article ul li ol li{list-style:decimal}.rst-content .section ol,.rst-content .section ol.arabic,.rst-content .toctree-wrapper ol,.rst-content .toctree-wrapper ol.arabic,.rst-content section ol,.rst-content section ol.arabic,.wy-plain-list-decimal,article ol{list-style:decimal;line-height:24px;margin-bottom:24px}.rst-content .section ol.arabic li,.rst-content .section ol li,.rst-content .toctree-wrapper ol.arabic li,.rst-content .toctree-wrapper ol li,.rst-content section ol.arabic li,.rst-content section ol li,.wy-plain-list-decimal li,article ol li{list-style:decimal;margin-left:24px}.rst-content .section ol.arabic li ul,.rst-content .section ol li p:last-child,.rst-content .section ol li ul,.rst-content .toctree-wrapper ol.arabic li ul,.rst-content .toctree-wrapper ol li p:last-child,.rst-content .toctree-wrapper ol li ul,.rst-content section ol.arabic li ul,.rst-content section ol li p:last-child,.rst-content section ol li ul,.wy-plain-list-decimal li p:last-child,.wy-plain-list-decimal li ul,article ol li p:last-child,article ol li ul{margin-bottom:0}.rst-content .section ol.arabic li ul li,.rst-content .section ol li ul li,.rst-content .toctree-wrapper ol.arabic li ul li,.rst-content .toctree-wrapper ol li ul li,.rst-content section ol.arabic li ul li,.rst-content section ol li ul li,.wy-plain-list-decimal li ul li,article ol li ul li{list-style:disc}.wy-breadcrumbs{*zoom:1}.wy-breadcrumbs:after,.wy-breadcrumbs:before{display:table;content:""}.wy-breadcrumbs:after{clear:both}.wy-breadcrumbs>li{display:inline-block;padding-top:5px}.wy-breadcrumbs>li.wy-breadcrumbs-aside{float:right}.rst-content .wy-breadcrumbs>li code,.rst-content .wy-breadcrumbs>li tt,.wy-breadcrumbs>li .rst-content tt,.wy-breadcrumbs>li code{all:inherit;color:inherit}.breadcrumb-item:before{content:"/";color:#bbb;font-size:13px;padding:0 6px 0 3px}.wy-breadcrumbs-extra{margin-bottom:0;color:#b3b3b3;font-size:80%;display:inline-block}@media screen and (max-width:480px){.wy-breadcrumbs-extra,.wy-breadcrumbs li.wy-breadcrumbs-aside{display:none}}@media print{.wy-breadcrumbs li.wy-breadcrumbs-aside{display:none}}html{font-size:16px}.wy-affix{position:fixed;top:1.618em}.wy-menu a:hover{text-decoration:none}.wy-menu-horiz{*zoom:1}.wy-menu-horiz:after,.wy-menu-horiz:before{display:table;content:""}.wy-menu-horiz:after{clear:both}.wy-menu-horiz li,.wy-menu-horiz ul{display:inline-block}.wy-menu-horiz li:hover{background:hsla(0,0%,100%,.1)}.wy-menu-horiz li.divide-left{border-left:1px solid #404040}.wy-menu-horiz li.divide-right{border-right:1px solid #404040}.wy-menu-horiz a{height:32px;display:inline-block;line-height:32px;padding:0 16px}.wy-menu-vertical{width:300px}.wy-menu-vertical header,.wy-menu-vertical p.caption{color:#55a5d9;height:32px;line-height:32px;padding:0 1.618em;margin:12px 0 0;display:block;font-weight:700;text-transform:uppercase;font-size:85%;white-space:nowrap}.wy-menu-vertical ul{margin-bottom:0}.wy-menu-vertical li.divide-top{border-top:1px solid #404040}.wy-menu-vertical li.divide-bottom{border-bottom:1px solid #404040}.wy-menu-vertical li.current{background:#e3e3e3}.wy-menu-vertical li.current a{color:grey;border-right:1px solid #c9c9c9;padding:.4045em 2.427em}.wy-menu-vertical li.current a:hover{background:#d6d6d6}.rst-content .wy-menu-vertical li tt,.wy-menu-vertical li .rst-content tt,.wy-menu-vertical li code{border:none;background:inherit;color:inherit;padding-left:0;padding-right:0}.wy-menu-vertical li button.toctree-expand{display:block;float:left;margin-left:-1.2em;line-height:18px;color:#4d4d4d;border:none;background:none;padding:0}.wy-menu-vertical li.current>a,.wy-menu-vertical li.on a{color:#404040;font-weight:700;position:relative;background:#fcfcfc;border:none;padding:.4045em 1.618em}.wy-menu-vertical li.current>a:hover,.wy-menu-vertical li.on a:hover{background:#fcfcfc}.wy-menu-vertical li.current>a:hover button.toctree-expand,.wy-menu-vertical li.on a:hover button.toctree-expand{color:grey}.wy-menu-vertical li.current>a button.toctree-expand,.wy-menu-vertical li.on a button.toctree-expand{display:block;line-height:18px;color:#333}.wy-menu-vertical li.toctree-l1.current>a{border-bottom:1px solid #c9c9c9;border-top:1px solid #c9c9c9}.wy-menu-vertical .toctree-l1.current .toctree-l2>ul,.wy-menu-vertical .toctree-l2.current .toctree-l3>ul,.wy-menu-vertical .toctree-l3.current .toctree-l4>ul,.wy-menu-vertical .toctree-l4.current .toctree-l5>ul,.wy-menu-vertical .toctree-l5.current .toctree-l6>ul,.wy-menu-vertical .toctree-l6.current .toctree-l7>ul,.wy-menu-vertical .toctree-l7.current .toctree-l8>ul,.wy-menu-vertical .toctree-l8.current .toctree-l9>ul,.wy-menu-vertical .toctree-l9.current .toctree-l10>ul,.wy-menu-vertical .toctree-l10.current .toctree-l11>ul{display:none}.wy-menu-vertical .toctree-l1.current .current.toctree-l2>ul,.wy-menu-vertical .toctree-l2.current .current.toctree-l3>ul,.wy-menu-vertical .toctree-l3.current .current.toctree-l4>ul,.wy-menu-vertical .toctree-l4.current .current.toctree-l5>ul,.wy-menu-vertical .toctree-l5.current .current.toctree-l6>ul,.wy-menu-vertical .toctree-l6.current .current.toctree-l7>ul,.wy-menu-vertical .toctree-l7.current .current.toctree-l8>ul,.wy-menu-vertical .toctree-l8.current .current.toctree-l9>ul,.wy-menu-vertical .toctree-l9.current .current.toctree-l10>ul,.wy-menu-vertical .toctree-l10.current .current.toctree-l11>ul{display:block}.wy-menu-vertical li.toctree-l3,.wy-menu-vertical li.toctree-l4{font-size:.9em}.wy-menu-vertical li.toctree-l2 a,.wy-menu-vertical li.toctree-l3 a,.wy-menu-vertical li.toctree-l4 a,.wy-menu-vertical li.toctree-l5 a,.wy-menu-vertical li.toctree-l6 a,.wy-menu-vertical li.toctree-l7 a,.wy-menu-vertical li.toctree-l8 a,.wy-menu-vertical li.toctree-l9 a,.wy-menu-vertical li.toctree-l10 a{color:#404040}.wy-menu-vertical li.toctree-l2 a:hover button.toctree-expand,.wy-menu-vertical li.toctree-l3 a:hover button.toctree-expand,.wy-menu-vertical li.toctree-l4 a:hover button.toctree-expand,.wy-menu-vertical li.toctree-l5 a:hover button.toctree-expand,.wy-menu-vertical li.toctree-l6 a:hover button.toctree-expand,.wy-menu-vertical li.toctree-l7 a:hover button.toctree-expand,.wy-menu-vertical li.toctree-l8 a:hover button.toctree-expand,.wy-menu-vertical li.toctree-l9 a:hover button.toctree-expand,.wy-menu-vertical li.toctree-l10 a:hover button.toctree-expand{color:grey}.wy-menu-vertical li.toctree-l2.current li.toctree-l3>a,.wy-menu-vertical li.toctree-l3.current li.toctree-l4>a,.wy-menu-vertical li.toctree-l4.current li.toctree-l5>a,.wy-menu-vertical li.toctree-l5.current li.toctree-l6>a,.wy-menu-vertical li.toctree-l6.current li.toctree-l7>a,.wy-menu-vertical li.toctree-l7.current li.toctree-l8>a,.wy-menu-vertical li.toctree-l8.current li.toctree-l9>a,.wy-menu-vertical li.toctree-l9.current li.toctree-l10>a,.wy-menu-vertical li.toctree-l10.current li.toctree-l11>a{display:block}.wy-menu-vertical li.toctree-l2.current>a{padding:.4045em 2.427em}.wy-menu-vertical li.toctree-l2.current li.toctree-l3>a{padding:.4045em 1.618em .4045em 4.045em}.wy-menu-vertical li.toctree-l3.current>a{padding:.4045em 4.045em}.wy-menu-vertical li.toctree-l3.current li.toctree-l4>a{padding:.4045em 1.618em .4045em 5.663em}.wy-menu-vertical li.toctree-l4.current>a{padding:.4045em 5.663em}.wy-menu-vertical li.toctree-l4.current li.toctree-l5>a{padding:.4045em 1.618em .4045em 7.281em}.wy-menu-vertical li.toctree-l5.current>a{padding:.4045em 7.281em}.wy-menu-vertical li.toctree-l5.current li.toctree-l6>a{padding:.4045em 1.618em .4045em 8.899em}.wy-menu-vertical li.toctree-l6.current>a{padding:.4045em 8.899em}.wy-menu-vertical li.toctree-l6.current li.toctree-l7>a{padding:.4045em 1.618em .4045em 10.517em}.wy-menu-vertical li.toctree-l7.current>a{padding:.4045em 10.517em}.wy-menu-vertical li.toctree-l7.current li.toctree-l8>a{padding:.4045em 1.618em .4045em 12.135em}.wy-menu-vertical li.toctree-l8.current>a{padding:.4045em 12.135em}.wy-menu-vertical li.toctree-l8.current li.toctree-l9>a{padding:.4045em 1.618em .4045em 13.753em}.wy-menu-vertical li.toctree-l9.current>a{padding:.4045em 13.753em}.wy-menu-vertical li.toctree-l9.current li.toctree-l10>a{padding:.4045em 1.618em .4045em 15.371em}.wy-menu-vertical li.toctree-l10.current>a{padding:.4045em 15.371em}.wy-menu-vertical li.toctree-l10.current li.toctree-l11>a{padding:.4045em 1.618em .4045em 16.989em}.wy-menu-vertical li.toctree-l2.current>a,.wy-menu-vertical li.toctree-l2.current li.toctree-l3>a{background:#c9c9c9}.wy-menu-vertical li.toctree-l2 button.toctree-expand{color:#a3a3a3}.wy-menu-vertical li.toctree-l3.current>a,.wy-menu-vertical li.toctree-l3.current li.toctree-l4>a{background:#bdbdbd}.wy-menu-vertical li.toctree-l3 button.toctree-expand{color:#969696}.wy-menu-vertical li.current ul{display:block}.wy-menu-vertical li ul{margin-bottom:0;display:none}.wy-menu-vertical li ul li a{margin-bottom:0;color:#d9d9d9;font-weight:400}.wy-menu-vertical a{line-height:18px;padding:.4045em 1.618em;display:block;position:relative;font-size:90%;color:#d9d9d9}.wy-menu-vertical a:hover{background-color:#4e4a4a;cursor:pointer}.wy-menu-vertical a:hover button.toctree-expand{color:#d9d9d9}.wy-menu-vertical a:active{background-color:#2980b9;cursor:pointer;color:#fff}.wy-menu-vertical a:active button.toctree-expand{color:#fff}.wy-side-nav-search{display:block;width:300px;padding:.809em;margin-bottom:.809em;z-index:200;background-color:#2980b9;text-align:center;color:#fcfcfc}.wy-side-nav-search input[type=text]{width:100%;border-radius:50px;padding:6px 12px;border-color:#2472a4}.wy-side-nav-search img{display:block;margin:auto auto .809em;height:45px;width:45px;background-color:#2980b9;padding:5px;border-radius:100%}.wy-side-nav-search .wy-dropdown>a,.wy-side-nav-search>a{color:#fcfcfc;font-size:100%;font-weight:700;display:inline-block;padding:4px 6px;margin-bottom:.809em;max-width:100%}.wy-side-nav-search .wy-dropdown>a:hover,.wy-side-nav-search>a:hover{background:hsla(0,0%,100%,.1)}.wy-side-nav-search .wy-dropdown>a img.logo,.wy-side-nav-search>a img.logo{display:block;margin:0 auto;height:auto;width:auto;border-radius:0;max-width:100%;background:transparent}.wy-side-nav-search .wy-dropdown>a.icon img.logo,.wy-side-nav-search>a.icon img.logo{margin-top:.85em}.wy-side-nav-search>div.version{margin-top:-.4045em;margin-bottom:.809em;font-weight:400;color:hsla(0,0%,100%,.3)}.wy-nav .wy-menu-vertical header{color:#2980b9}.wy-nav .wy-menu-vertical a{color:#b3b3b3}.wy-nav .wy-menu-vertical a:hover{background-color:#2980b9;color:#fff}[data-menu-wrap]{-webkit-transition:all .2s ease-in;-moz-transition:all .2s ease-in;transition:all .2s ease-in;position:absolute;opacity:1;width:100%;opacity:0}[data-menu-wrap].move-center{left:0;right:auto;opacity:1}[data-menu-wrap].move-left{right:auto;left:-100%;opacity:0}[data-menu-wrap].move-right{right:-100%;left:auto;opacity:0}.wy-body-for-nav{background:#fcfcfc}.wy-grid-for-nav{position:absolute;width:100%;height:100%}.wy-nav-side{position:fixed;top:0;bottom:0;left:0;padding-bottom:2em;width:300px;overflow-x:hidden;overflow-y:hidden;min-height:100%;color:#9b9b9b;background:#343131;z-index:200}.wy-side-scroll{width:320px;position:relative;overflow-x:hidden;overflow-y:scroll;height:100%}.wy-nav-top{display:none;background:#2980b9;color:#fff;padding:.4045em .809em;position:relative;line-height:50px;text-align:center;font-size:100%;*zoom:1}.wy-nav-top:after,.wy-nav-top:before{display:table;content:""}.wy-nav-top:after{clear:both}.wy-nav-top a{color:#fff;font-weight:700}.wy-nav-top img{margin-right:12px;height:45px;width:45px;background-color:#2980b9;padding:5px;border-radius:100%}.wy-nav-top i{font-size:30px;float:left;cursor:pointer;padding-top:inherit}.wy-nav-content-wrap{margin-left:300px;background:#fcfcfc;min-height:100%}.wy-nav-content{padding:1.618em 3.236em;height:100%;max-width:800px;margin:auto}.wy-body-mask{position:fixed;width:100%;height:100%;background:rgba(0,0,0,.2);display:none;z-index:499}.wy-body-mask.on{display:block}footer{color:grey}footer p{margin-bottom:12px}.rst-content footer span.commit tt,footer span.commit .rst-content tt,footer span.commit code{padding:0;font-family:SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,Courier,monospace;font-size:1em;background:none;border:none;color:grey}.rst-footer-buttons{*zoom:1}.rst-footer-buttons:after,.rst-footer-buttons:before{width:100%;display:table;content:""}.rst-footer-buttons:after{clear:both}.rst-breadcrumbs-buttons{margin-top:12px;*zoom:1}.rst-breadcrumbs-buttons:after,.rst-breadcrumbs-buttons:before{display:table;content:""}.rst-breadcrumbs-buttons:after{clear:both}#search-results .search li{margin-bottom:24px;border-bottom:1px solid #e1e4e5;padding-bottom:24px}#search-results .search li:first-child{border-top:1px solid #e1e4e5;padding-top:24px}#search-results .search li a{font-size:120%;margin-bottom:12px;display:inline-block}#search-results .context{color:grey;font-size:90%}.genindextable li>ul{margin-left:24px}@media screen and (max-width:768px){.wy-body-for-nav{background:#fcfcfc}.wy-nav-top{display:block}.wy-nav-side{left:-300px}.wy-nav-side.shift{width:85%;left:0}.wy-menu.wy-menu-vertical,.wy-side-nav-search,.wy-side-scroll{width:auto}.wy-nav-content-wrap{margin-left:0}.wy-nav-content-wrap .wy-nav-content{padding:1.618em}.wy-nav-content-wrap.shift{position:fixed;min-width:100%;left:85%;top:0;height:100%;overflow:hidden}}@media screen and (min-width:1100px){.wy-nav-content-wrap{background:rgba(0,0,0,.05)}.wy-nav-content{margin:0;background:#fcfcfc}}@media print{.rst-versions,.wy-nav-side,footer{display:none}.wy-nav-content-wrap{margin-left:0}}.rst-versions{position:fixed;bottom:0;left:0;width:300px;color:#fcfcfc;background:#1f1d1d;font-family:Lato,proxima-nova,Helvetica Neue,Arial,sans-serif;z-index:400}.rst-versions a{color:#2980b9;text-decoration:none}.rst-versions .rst-badge-small{display:none}.rst-versions .rst-current-version{padding:12px;background-color:#272525;display:block;text-align:right;font-size:90%;cursor:pointer;color:#27ae60;*zoom:1}.rst-versions .rst-current-version:after,.rst-versions .rst-current-version:before{display:table;content:""}.rst-versions .rst-current-version:after{clear:both}.rst-content .code-block-caption .rst-versions .rst-current-version .headerlink,.rst-content .eqno .rst-versions .rst-current-version .headerlink,.rst-content .rst-versions .rst-current-version .admonition-title,.rst-content code.download .rst-versions .rst-current-version span:first-child,.rst-content dl dt .rst-versions .rst-current-version .headerlink,.rst-content h1 .rst-versions .rst-current-version .headerlink,.rst-content h2 .rst-versions .rst-current-version .headerlink,.rst-content h3 .rst-versions .rst-current-version .headerlink,.rst-content h4 .rst-versions .rst-current-version .headerlink,.rst-content h5 .rst-versions .rst-current-version .headerlink,.rst-content h6 .rst-versions .rst-current-version .headerlink,.rst-content p .rst-versions .rst-current-version .headerlink,.rst-content table>caption .rst-versions .rst-current-version .headerlink,.rst-content tt.download .rst-versions .rst-current-version span:first-child,.rst-versions .rst-current-version .fa,.rst-versions .rst-current-version .icon,.rst-versions .rst-current-version .rst-content .admonition-title,.rst-versions .rst-current-version .rst-content .code-block-caption .headerlink,.rst-versions .rst-current-version .rst-content .eqno .headerlink,.rst-versions .rst-current-version .rst-content code.download span:first-child,.rst-versions .rst-current-version .rst-content dl dt .headerlink,.rst-versions .rst-current-version .rst-content h1 .headerlink,.rst-versions .rst-current-version .rst-content h2 .headerlink,.rst-versions .rst-current-version .rst-content h3 .headerlink,.rst-versions .rst-current-version .rst-content h4 .headerlink,.rst-versions .rst-current-version .rst-content h5 .headerlink,.rst-versions .rst-current-version .rst-content h6 .headerlink,.rst-versions .rst-current-version .rst-content p .headerlink,.rst-versions .rst-current-version .rst-content table>caption .headerlink,.rst-versions .rst-current-version .rst-content tt.download span:first-child,.rst-versions .rst-current-version .wy-menu-vertical li button.toctree-expand,.wy-menu-vertical li .rst-versions .rst-current-version button.toctree-expand{color:#fcfcfc}.rst-versions .rst-current-version .fa-book,.rst-versions .rst-current-version .icon-book{float:left}.rst-versions .rst-current-version.rst-out-of-date{background-color:#e74c3c;color:#fff}.rst-versions .rst-current-version.rst-active-old-version{background-color:#f1c40f;color:#000}.rst-versions.shift-up{height:auto;max-height:100%;overflow-y:scroll}.rst-versions.shift-up .rst-other-versions{display:block}.rst-versions .rst-other-versions{font-size:90%;padding:12px;color:grey;display:none}.rst-versions .rst-other-versions hr{display:block;height:1px;border:0;margin:20px 0;padding:0;border-top:1px solid #413d3d}.rst-versions .rst-other-versions dd{display:inline-block;margin:0}.rst-versions .rst-other-versions dd a{display:inline-block;padding:6px;color:#fcfcfc}.rst-versions.rst-badge{width:auto;bottom:20px;right:20px;left:auto;border:none;max-width:300px;max-height:90%}.rst-versions.rst-badge .fa-book,.rst-versions.rst-badge .icon-book{float:none;line-height:30px}.rst-versions.rst-badge.shift-up .rst-current-version{text-align:right}.rst-versions.rst-badge.shift-up .rst-current-version .fa-book,.rst-versions.rst-badge.shift-up .rst-current-version .icon-book{float:left}.rst-versions.rst-badge>.rst-current-version{width:auto;height:30px;line-height:30px;padding:0 6px;display:block;text-align:center}@media screen and (max-width:768px){.rst-versions{width:85%;display:none}.rst-versions.shift{display:block}}.rst-content .toctree-wrapper>p.caption,.rst-content h1,.rst-content h2,.rst-content h3,.rst-content h4,.rst-content h5,.rst-content h6{margin-bottom:24px}.rst-content img{max-width:100%;height:auto}.rst-content div.figure,.rst-content figure{margin-bottom:24px}.rst-content div.figure .caption-text,.rst-content figure .caption-text{font-style:italic}.rst-content div.figure p:last-child.caption,.rst-content figure p:last-child.caption{margin-bottom:0}.rst-content div.figure.align-center,.rst-content figure.align-center{text-align:center}.rst-content .section>a>img,.rst-content .section>img,.rst-content section>a>img,.rst-content section>img{margin-bottom:24px}.rst-content abbr[title]{text-decoration:none}.rst-content.style-external-links a.reference.external:after{font-family:FontAwesome;content:"\f08e";color:#b3b3b3;vertical-align:super;font-size:60%;margin:0 .2em}.rst-content blockquote{margin-left:24px;line-height:24px;margin-bottom:24px}.rst-content pre.literal-block{white-space:pre;margin:0;padding:12px;font-family:SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,Courier,monospace;display:block;overflow:auto}.rst-content div[class^=highlight],.rst-content pre.literal-block{border:1px solid #e1e4e5;overflow-x:auto;margin:1px 0 24px}.rst-content div[class^=highlight] div[class^=highlight],.rst-content pre.literal-block div[class^=highlight]{padding:0;border:none;margin:0}.rst-content div[class^=highlight] td.code{width:100%}.rst-content .linenodiv pre{border-right:1px solid #e6e9ea;margin:0;padding:12px;font-family:SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,Courier,monospace;user-select:none;pointer-events:none}.rst-content div[class^=highlight] pre{white-space:pre;margin:0;padding:12px;display:block;overflow:auto}.rst-content div[class^=highlight] pre .hll{display:block;margin:0 -12px;padding:0 12px}.rst-content .linenodiv pre,.rst-content div[class^=highlight] pre,.rst-content pre.literal-block{font-family:SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,Courier,monospace;font-size:12px;line-height:1.4}.rst-content div.highlight .gp,.rst-content div.highlight span.linenos{user-select:none;pointer-events:none}.rst-content div.highlight span.linenos{display:inline-block;padding-left:0;padding-right:12px;margin-right:12px;border-right:1px solid #e6e9ea}.rst-content .code-block-caption{font-style:italic;font-size:85%;line-height:1;padding:1em 0;text-align:center}@media print{.rst-content .codeblock,.rst-content div[class^=highlight],.rst-content div[class^=highlight] pre{white-space:pre-wrap}}.rst-content .admonition,.rst-content .admonition-todo,.rst-content .attention,.rst-content .caution,.rst-content .danger,.rst-content .error,.rst-content .hint,.rst-content .important,.rst-content .note,.rst-content .seealso,.rst-content .tip,.rst-content .warning{clear:both}.rst-content .admonition-todo .last,.rst-content .admonition-todo>:last-child,.rst-content .admonition .last,.rst-content .admonition>:last-child,.rst-content .attention .last,.rst-content .attention>:last-child,.rst-content .caution .last,.rst-content .caution>:last-child,.rst-content .danger .last,.rst-content .danger>:last-child,.rst-content .error .last,.rst-content .error>:last-child,.rst-content .hint .last,.rst-content .hint>:last-child,.rst-content .important .last,.rst-content .important>:last-child,.rst-content .note .last,.rst-content .note>:last-child,.rst-content .seealso .last,.rst-content .seealso>:last-child,.rst-content .tip .last,.rst-content .tip>:last-child,.rst-content .warning .last,.rst-content .warning>:last-child{margin-bottom:0}.rst-content .admonition-title:before{margin-right:4px}.rst-content .admonition table{border-color:rgba(0,0,0,.1)}.rst-content .admonition table td,.rst-content .admonition table th{background:transparent!important;border-color:rgba(0,0,0,.1)!important}.rst-content .section ol.loweralpha,.rst-content .section ol.loweralpha>li,.rst-content .toctree-wrapper ol.loweralpha,.rst-content .toctree-wrapper ol.loweralpha>li,.rst-content section ol.loweralpha,.rst-content section ol.loweralpha>li{list-style:lower-alpha}.rst-content .section ol.upperalpha,.rst-content .section ol.upperalpha>li,.rst-content .toctree-wrapper ol.upperalpha,.rst-content .toctree-wrapper ol.upperalpha>li,.rst-content section ol.upperalpha,.rst-content section ol.upperalpha>li{list-style:upper-alpha}.rst-content .section ol li>*,.rst-content .section ul li>*,.rst-content .toctree-wrapper ol li>*,.rst-content .toctree-wrapper ul li>*,.rst-content section ol li>*,.rst-content section ul li>*{margin-top:12px;margin-bottom:12px}.rst-content .section ol li>:first-child,.rst-content .section ul li>:first-child,.rst-content .toctree-wrapper ol li>:first-child,.rst-content .toctree-wrapper ul li>:first-child,.rst-content section ol li>:first-child,.rst-content section ul li>:first-child{margin-top:0}.rst-content .section ol li>p,.rst-content .section ol li>p:last-child,.rst-content .section ul li>p,.rst-content .section ul li>p:last-child,.rst-content .toctree-wrapper ol li>p,.rst-content .toctree-wrapper ol li>p:last-child,.rst-content .toctree-wrapper ul li>p,.rst-content .toctree-wrapper ul li>p:last-child,.rst-content section ol li>p,.rst-content section ol li>p:last-child,.rst-content section ul li>p,.rst-content section ul li>p:last-child{margin-bottom:12px}.rst-content .section ol li>p:only-child,.rst-content .section ol li>p:only-child:last-child,.rst-content .section ul li>p:only-child,.rst-content .section ul li>p:only-child:last-child,.rst-content .toctree-wrapper ol li>p:only-child,.rst-content .toctree-wrapper ol li>p:only-child:last-child,.rst-content .toctree-wrapper ul li>p:only-child,.rst-content .toctree-wrapper ul li>p:only-child:last-child,.rst-content section ol li>p:only-child,.rst-content section ol li>p:only-child:last-child,.rst-content section ul li>p:only-child,.rst-content section ul li>p:only-child:last-child{margin-bottom:0}.rst-content .section ol li>ol,.rst-content .section ol li>ul,.rst-content .section ul li>ol,.rst-content .section ul li>ul,.rst-content .toctree-wrapper ol li>ol,.rst-content .toctree-wrapper ol li>ul,.rst-content .toctree-wrapper ul li>ol,.rst-content .toctree-wrapper ul li>ul,.rst-content section ol li>ol,.rst-content section ol li>ul,.rst-content section ul li>ol,.rst-content section ul li>ul{margin-bottom:12px}.rst-content .section ol.simple li>*,.rst-content .section ol.simple li ol,.rst-content .section ol.simple li ul,.rst-content .section ul.simple li>*,.rst-content .section ul.simple li ol,.rst-content .section ul.simple li ul,.rst-content .toctree-wrapper ol.simple li>*,.rst-content .toctree-wrapper ol.simple li ol,.rst-content .toctree-wrapper ol.simple li ul,.rst-content .toctree-wrapper ul.simple li>*,.rst-content .toctree-wrapper ul.simple li ol,.rst-content .toctree-wrapper ul.simple li ul,.rst-content section ol.simple li>*,.rst-content section ol.simple li ol,.rst-content section ol.simple li ul,.rst-content section ul.simple li>*,.rst-content section ul.simple li ol,.rst-content section ul.simple li ul{margin-top:0;margin-bottom:0}.rst-content .line-block{margin-left:0;margin-bottom:24px;line-height:24px}.rst-content .line-block .line-block{margin-left:24px;margin-bottom:0}.rst-content .topic-title{font-weight:700;margin-bottom:12px}.rst-content .toc-backref{color:#404040}.rst-content .align-right{float:right;margin:0 0 24px 24px}.rst-content .align-left{float:left;margin:0 24px 24px 0}.rst-content .align-center{margin:auto}.rst-content .align-center:not(table){display:block}.rst-content .code-block-caption .headerlink,.rst-content .eqno .headerlink,.rst-content .toctree-wrapper>p.caption .headerlink,.rst-content dl dt .headerlink,.rst-content h1 .headerlink,.rst-content h2 .headerlink,.rst-content h3 .headerlink,.rst-content h4 .headerlink,.rst-content h5 .headerlink,.rst-content h6 .headerlink,.rst-content p.caption .headerlink,.rst-content p .headerlink,.rst-content table>caption .headerlink{opacity:0;font-size:14px;font-family:FontAwesome;margin-left:.5em}.rst-content .code-block-caption .headerlink:focus,.rst-content .code-block-caption:hover .headerlink,.rst-content .eqno .headerlink:focus,.rst-content .eqno:hover .headerlink,.rst-content .toctree-wrapper>p.caption .headerlink:focus,.rst-content .toctree-wrapper>p.caption:hover .headerlink,.rst-content dl dt .headerlink:focus,.rst-content dl dt:hover .headerlink,.rst-content h1 .headerlink:focus,.rst-content h1:hover .headerlink,.rst-content h2 .headerlink:focus,.rst-content h2:hover .headerlink,.rst-content h3 .headerlink:focus,.rst-content h3:hover .headerlink,.rst-content h4 .headerlink:focus,.rst-content h4:hover .headerlink,.rst-content h5 .headerlink:focus,.rst-content h5:hover .headerlink,.rst-content h6 .headerlink:focus,.rst-content h6:hover .headerlink,.rst-content p.caption .headerlink:focus,.rst-content p.caption:hover .headerlink,.rst-content p .headerlink:focus,.rst-content p:hover .headerlink,.rst-content table>caption .headerlink:focus,.rst-content table>caption:hover .headerlink{opacity:1}.rst-content p a{overflow-wrap:anywhere}.rst-content .wy-table td p,.rst-content .wy-table td ul,.rst-content .wy-table th p,.rst-content .wy-table th ul,.rst-content table.docutils td p,.rst-content table.docutils td ul,.rst-content table.docutils th p,.rst-content table.docutils th ul,.rst-content table.field-list td p,.rst-content table.field-list td ul,.rst-content table.field-list th p,.rst-content table.field-list th ul{font-size:inherit}.rst-content .btn:focus{outline:2px solid}.rst-content table>caption .headerlink:after{font-size:12px}.rst-content .centered{text-align:center}.rst-content .sidebar{float:right;width:40%;display:block;margin:0 0 24px 24px;padding:24px;background:#f3f6f6;border:1px solid #e1e4e5}.rst-content .sidebar dl,.rst-content .sidebar p,.rst-content .sidebar ul{font-size:90%}.rst-content .sidebar .last,.rst-content .sidebar>:last-child{margin-bottom:0}.rst-content .sidebar .sidebar-title{display:block;font-family:Roboto Slab,ff-tisa-web-pro,Georgia,Arial,sans-serif;font-weight:700;background:#e1e4e5;padding:6px 12px;margin:-24px -24px 24px;font-size:100%}.rst-content .highlighted{background:#f1c40f;box-shadow:0 0 0 2px #f1c40f;display:inline;font-weight:700}.rst-content .citation-reference,.rst-content .footnote-reference{vertical-align:baseline;position:relative;top:-.4em;line-height:0;font-size:90%}.rst-content .hlist{width:100%}.rst-content dl dt span.classifier:before{content:" : "}.rst-content dl dt span.classifier-delimiter{display:none!important}html.writer-html4 .rst-content table.docutils.citation,html.writer-html4 .rst-content table.docutils.footnote{background:none;border:none}html.writer-html4 .rst-content table.docutils.citation td,html.writer-html4 .rst-content table.docutils.citation tr,html.writer-html4 .rst-content table.docutils.footnote td,html.writer-html4 .rst-content table.docutils.footnote tr{border:none;background-color:transparent!important;white-space:normal}html.writer-html4 .rst-content table.docutils.citation td.label,html.writer-html4 .rst-content table.docutils.footnote td.label{padding-left:0;padding-right:0;vertical-align:top}html.writer-html5 .rst-content dl.citation,html.writer-html5 .rst-content dl.field-list,html.writer-html5 .rst-content dl.footnote{display:grid;grid-template-columns:max-content auto}html.writer-html5 .rst-content dl.citation>dt,html.writer-html5 .rst-content dl.field-list>dt,html.writer-html5 .rst-content dl.footnote>dt{padding-left:1rem}html.writer-html5 .rst-content dl.citation>dt:after,html.writer-html5 .rst-content dl.field-list>dt:after,html.writer-html5 .rst-content dl.footnote>dt:after{content:":"}html.writer-html5 .rst-content dl.citation>dd,html.writer-html5 .rst-content dl.citation>dt,html.writer-html5 .rst-content dl.field-list>dd,html.writer-html5 .rst-content dl.field-list>dt,html.writer-html5 .rst-content dl.footnote>dd,html.writer-html5 .rst-content dl.footnote>dt{margin-bottom:0}html.writer-html5 .rst-content dl.citation,html.writer-html5 .rst-content dl.footnote{font-size:.9rem}html.writer-html5 .rst-content dl.citation>dt,html.writer-html5 .rst-content dl.footnote>dt{margin:0 .5rem .5rem 0;line-height:1.2rem;word-break:break-all;font-weight:400}html.writer-html5 .rst-content dl.citation>dt>span.brackets,html.writer-html5 .rst-content dl.footnote>dt>span.brackets{margin-right:.5rem}html.writer-html5 .rst-content dl.citation>dt>span.brackets:before,html.writer-html5 .rst-content dl.footnote>dt>span.brackets:before{content:"["}html.writer-html5 .rst-content dl.citation>dt>span.brackets:after,html.writer-html5 .rst-content dl.footnote>dt>span.brackets:after{content:"]"}html.writer-html5 .rst-content dl.citation>dt>span.fn-backref,html.writer-html5 .rst-content dl.footnote>dt>span.fn-backref{font-style:italic}html.writer-html5 .rst-content dl.citation>dd,html.writer-html5 .rst-content dl.footnote>dd{margin:0 0 .5rem;line-height:1.2rem}html.writer-html5 .rst-content dl.citation>dd p,html.writer-html5 .rst-content dl.footnote>dd p,html.writer-html5 .rst-content dl.option-list kbd{font-size:.9rem}.rst-content dl.citation,.rst-content table.docutils.footnote,html.writer-html4 .rst-content table.docutils.citation,html.writer-html5 .rst-content dl.footnote{color:grey}.rst-content dl.citation code,.rst-content dl.citation tt,.rst-content table.docutils.footnote code,.rst-content table.docutils.footnote tt,html.writer-html4 .rst-content table.docutils.citation code,html.writer-html4 .rst-content table.docutils.citation tt,html.writer-html5 .rst-content dl.footnote code,html.writer-html5 .rst-content dl.footnote tt{color:#555}.rst-content .wy-table-responsive.citation,.rst-content .wy-table-responsive.footnote{margin-bottom:0}.rst-content .wy-table-responsive.citation+:not(.citation),.rst-content .wy-table-responsive.footnote+:not(.footnote){margin-top:24px}.rst-content .wy-table-responsive.citation:last-child,.rst-content .wy-table-responsive.footnote:last-child{margin-bottom:24px}.rst-content table.docutils th{border-color:#e1e4e5}html.writer-html5 .rst-content table.docutils th{border:1px solid #e1e4e5}html.writer-html5 .rst-content table.docutils td>p,html.writer-html5 .rst-content table.docutils th>p{line-height:1rem;margin-bottom:0;font-size:.9rem}.rst-content table.docutils td .last,.rst-content table.docutils td .last>:last-child{margin-bottom:0}.rst-content table.field-list,.rst-content table.field-list td{border:none}.rst-content table.field-list td p{line-height:inherit}.rst-content table.field-list td>strong{display:inline-block}.rst-content table.field-list .field-name{padding-right:10px;text-align:left;white-space:nowrap}.rst-content table.field-list .field-body{text-align:left}.rst-content code,.rst-content tt{color:#000;font-family:SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,Courier,monospace;padding:2px 5px}.rst-content code big,.rst-content code em,.rst-content tt big,.rst-content tt em{font-size:100%!important;line-height:normal}.rst-content code.literal,.rst-content tt.literal{color:#e74c3c;white-space:normal}.rst-content code.xref,.rst-content tt.xref,a .rst-content code,a .rst-content tt{font-weight:700;color:#404040;overflow-wrap:normal}.rst-content kbd,.rst-content pre,.rst-content samp{font-family:SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,Courier,monospace}.rst-content a code,.rst-content a tt{color:#2980b9}.rst-content dl{margin-bottom:24px}.rst-content dl dt{font-weight:700;margin-bottom:12px}.rst-content dl ol,.rst-content dl p,.rst-content dl table,.rst-content dl ul{margin-bottom:12px}.rst-content dl dd{margin:0 0 12px 24px;line-height:24px}.rst-content dl dd>ol:last-child,.rst-content dl dd>p:last-child,.rst-content dl dd>table:last-child,.rst-content dl dd>ul:last-child{margin-bottom:0}html.writer-html4 .rst-content dl:not(.docutils),html.writer-html5 .rst-content dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.citation):not(.glossary):not(.simple){margin-bottom:24px}html.writer-html4 .rst-content dl:not(.docutils)>dt,html.writer-html5 .rst-content dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.citation):not(.glossary):not(.simple)>dt{display:table;margin:6px 0;font-size:90%;line-height:normal;background:#e7f2fa;color:#2980b9;border-top:3px solid #6ab0de;padding:6px;position:relative}html.writer-html4 .rst-content dl:not(.docutils)>dt:before,html.writer-html5 .rst-content dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.citation):not(.glossary):not(.simple)>dt:before{color:#6ab0de}html.writer-html4 .rst-content dl:not(.docutils)>dt .headerlink,html.writer-html5 .rst-content dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.citation):not(.glossary):not(.simple)>dt .headerlink{color:#404040;font-size:100%!important}html.writer-html4 .rst-content dl:not(.docutils) dl:not(.option-list):not(.field-list):not(.footnote):not(.citation):not(.glossary):not(.simple)>dt,html.writer-html5 .rst-content dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.citation):not(.glossary):not(.simple) dl:not(.option-list):not(.field-list):not(.footnote):not(.citation):not(.glossary):not(.simple)>dt{margin-bottom:6px;border:none;border-left:3px solid #ccc;background:#f0f0f0;color:#555}html.writer-html4 .rst-content dl:not(.docutils) dl:not(.option-list):not(.field-list):not(.footnote):not(.citation):not(.glossary):not(.simple)>dt .headerlink,html.writer-html5 .rst-content dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.citation):not(.glossary):not(.simple) dl:not(.option-list):not(.field-list):not(.footnote):not(.citation):not(.glossary):not(.simple)>dt .headerlink{color:#404040;font-size:100%!important}html.writer-html4 .rst-content dl:not(.docutils)>dt:first-child,html.writer-html5 .rst-content dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.citation):not(.glossary):not(.simple)>dt:first-child{margin-top:0}html.writer-html4 .rst-content dl:not(.docutils) code.descclassname,html.writer-html4 .rst-content dl:not(.docutils) code.descname,html.writer-html4 .rst-content dl:not(.docutils) tt.descclassname,html.writer-html4 .rst-content dl:not(.docutils) tt.descname,html.writer-html5 .rst-content dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.citation):not(.glossary):not(.simple) code.descclassname,html.writer-html5 .rst-content dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.citation):not(.glossary):not(.simple) code.descname,html.writer-html5 .rst-content dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.citation):not(.glossary):not(.simple) tt.descclassname,html.writer-html5 .rst-content dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.citation):not(.glossary):not(.simple) tt.descname{background-color:transparent;border:none;padding:0;font-size:100%!important}html.writer-html4 .rst-content dl:not(.docutils) code.descname,html.writer-html4 .rst-content dl:not(.docutils) tt.descname,html.writer-html5 .rst-content dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.citation):not(.glossary):not(.simple) code.descname,html.writer-html5 .rst-content dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.citation):not(.glossary):not(.simple) tt.descname{font-weight:700}html.writer-html4 .rst-content dl:not(.docutils) .optional,html.writer-html5 .rst-content dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.citation):not(.glossary):not(.simple) .optional{display:inline-block;padding:0 4px;color:#000;font-weight:700}html.writer-html4 .rst-content dl:not(.docutils) .property,html.writer-html5 .rst-content dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.citation):not(.glossary):not(.simple) .property{display:inline-block;padding-right:8px;max-width:100%}html.writer-html4 .rst-content dl:not(.docutils) .k,html.writer-html5 .rst-content dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.citation):not(.glossary):not(.simple) .k{font-style:italic}html.writer-html4 .rst-content dl:not(.docutils) .descclassname,html.writer-html4 .rst-content dl:not(.docutils) .descname,html.writer-html4 .rst-content dl:not(.docutils) .sig-name,html.writer-html5 .rst-content dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.citation):not(.glossary):not(.simple) .descclassname,html.writer-html5 .rst-content dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.citation):not(.glossary):not(.simple) .descname,html.writer-html5 .rst-content dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.citation):not(.glossary):not(.simple) .sig-name{font-family:SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,Courier,monospace;color:#000}.rst-content .viewcode-back,.rst-content .viewcode-link{display:inline-block;color:#27ae60;font-size:80%;padding-left:24px}.rst-content .viewcode-back{display:block;float:right}.rst-content p.rubric{margin-bottom:12px;font-weight:700}.rst-content code.download,.rst-content tt.download{background:inherit;padding:inherit;font-weight:400;font-family:inherit;font-size:inherit;color:inherit;border:inherit;white-space:inherit}.rst-content code.download span:first-child,.rst-content tt.download span:first-child{-webkit-font-smoothing:subpixel-antialiased}.rst-content code.download span:first-child:before,.rst-content tt.download span:first-child:before{margin-right:4px}.rst-content .guilabel{border:1px solid #7fbbe3;background:#e7f2fa;font-size:80%;font-weight:700;border-radius:4px;padding:2.4px 6px;margin:auto 2px}.rst-content :not(dl.option-list)>:not(dt):not(kbd):not(.kbd)>.kbd,.rst-content :not(dl.option-list)>:not(dt):not(kbd):not(.kbd)>kbd{color:inherit;font-size:80%;background-color:#fff;border:1px solid #a6a6a6;border-radius:4px;box-shadow:0 2px grey;padding:2.4px 6px;margin:auto 0}.rst-content .versionmodified{font-style:italic}@media screen and (max-width:480px){.rst-content .sidebar{width:100%}}span[id*=MathJax-Span]{color:#404040}.math{text-align:center}@font-face{font-family:Lato;src:url(fonts/lato-normal.woff2?bd03a2cc277bbbc338d464e679fe9942) format("woff2"),url(fonts/lato-normal.woff?27bd77b9162d388cb8d4c4217c7c5e2a) format("woff");font-weight:400;font-style:normal;font-display:block}@font-face{font-family:Lato;src:url(fonts/lato-bold.woff2?cccb897485813c7c256901dbca54ecf2) format("woff2"),url(fonts/lato-bold.woff?d878b6c29b10beca227e9eef4246111b) format("woff");font-weight:700;font-style:normal;font-display:block}@font-face{font-family:Lato;src:url(fonts/lato-bold-italic.woff2?0b6bb6725576b072c5d0b02ecdd1900d) format("woff2"),url(fonts/lato-bold-italic.woff?9c7e4e9eb485b4a121c760e61bc3707c) format("woff");font-weight:700;font-style:italic;font-display:block}@font-face{font-family:Lato;src:url(fonts/lato-normal-italic.woff2?4eb103b4d12be57cb1d040ed5e162e9d) format("woff2"),url(fonts/lato-normal-italic.woff?f28f2d6482446544ef1ea1ccc6dd5892) format("woff");font-weight:400;font-style:italic;font-display:block}@font-face{font-family:Roboto Slab;font-style:normal;font-weight:400;src:url(fonts/Roboto-Slab-Regular.woff2?7abf5b8d04d26a2cafea937019bca958) format("woff2"),url(fonts/Roboto-Slab-Regular.woff?c1be9284088d487c5e3ff0a10a92e58c) format("woff");font-display:block}@font-face{font-family:Roboto Slab;font-style:normal;font-weight:700;src:url(fonts/Roboto-Slab-Bold.woff2?9984f4a9bda09be08e83f2506954adbe) format("woff2"),url(fonts/Roboto-Slab-Bold.woff?bed5564a116b05148e3b3bea6fb1162a) format("woff");font-display:block}
```

### Comparing `Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/_static/custom.css` & `Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/_static/custom.css`

 * *Files identical despite different names*

### Comparing `Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/_static/jquery-3.5.1.js` & `Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/_static/jquery-3.6.0.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,19 +1,19 @@
 /*!
- * jQuery JavaScript Library v3.5.1
+ * jQuery JavaScript Library v3.6.0
  * https://jquery.com/
  *
  * Includes Sizzle.js
  * https://sizzlejs.com/
  *
- * Copyright JS Foundation and other contributors
+ * Copyright OpenJS Foundation and other contributors
  * Released under the MIT license
  * https://jquery.org/license
  *
- * Date: 2020-05-04T22:49Z
+ * Date: 2021-03-02T17:08Z
  */
 (function(global, factory) {
 
     "use strict";
 
     if (typeof module === "object" && typeof module.exports === "object") {
 
@@ -76,15 +76,19 @@
 
     var isFunction = function isFunction(obj) {
 
         // Support: Chrome <=57, Firefox <=52
         // In some browsers, typeof returns "function" for HTML <object> elements
         // (i.e., `typeof document.createElement( "object" ) === "function"`).
         // We don't want to classify *any* DOM node as a function.
-        return typeof obj === "function" && typeof obj.nodeType !== "number";
+        // Support: QtWeb <=3.8.5, WebKit <=534.34, wkhtmltopdf tool <=0.12.5
+        // Plus for old WebKit, typeof returns "function" for HTML collections
+        // (e.g., `typeof document.getElementsByTagName("div") === "function"`). (gh-4756)
+        return typeof obj === "function" && typeof obj.nodeType !== "number" &&
+            typeof obj.item !== "function";
     };
 
 
     var isWindow = function isWindow(obj) {
         return obj != null && obj === obj.window;
     };
 
@@ -143,15 +147,15 @@
     /* global Symbol */
     // Defining this global in .eslintrc.json would create a danger of using the global
     // unguarded in another place, it seems safer to define global only for this module
 
 
 
     var
-        version = "3.5.1",
+        version = "3.6.0",
 
         // Define a local copy of jQuery
         jQuery = function(selector, context) {
 
             // The jQuery object is actually just the init constructor 'enhanced'
             // Need init if jQuery is called (just allow error to be thrown if not included)
             return new jQuery.fn.init(selector, context);
@@ -515,22 +519,22 @@
         }
 
         return type === "array" || length === 0 ||
             typeof length === "number" && length > 0 && (length - 1) in obj;
     }
     var Sizzle =
         /*!
-         * Sizzle CSS Selector Engine v2.3.5
+         * Sizzle CSS Selector Engine v2.3.6
          * https://sizzlejs.com/
          *
          * Copyright JS Foundation and other contributors
          * Released under the MIT license
          * https://js.foundation/
          *
-         * Date: 2020-03-14
+         * Date: 2021-02-16
          */
         (function(window) {
             var i,
                 support,
                 Expr,
                 getText,
                 isXML,
@@ -1108,16 +1112,16 @@
 
             /**
              * Detects XML nodes
              * @param {Element|Object} elem An element or a document
              * @returns {Boolean} True iff elem is a non-HTML XML node
              */
             isXML = Sizzle.isXML = function(elem) {
-                var namespace = elem.namespaceURI,
-                    docElem = (elem.ownerDocument || elem).documentElement;
+                var namespace = elem && elem.namespaceURI,
+                    docElem = elem && (elem.ownerDocument || elem).documentElement;
 
                 // Support: IE <=8
                 // Assume HTML when documentElement doesn't yet exist, such as inside loading iframes
                 // https://bugs.jquery.com/ticket/4833
                 return !rhtml.test(namespace || docElem && docElem.nodeName || "HTML");
             };
 
@@ -3048,15 +3052,15 @@
 
 
 
     function nodeName(elem, name) {
 
         return elem.nodeName && elem.nodeName.toLowerCase() === name.toLowerCase();
 
-    };
+    }
     var rsingleTag = (/^<([a-z][^\/\0>:\x20\t\r\n\f]*)[\x20\t\r\n\f]*\/?>(?:<\/\1>|)$/i);
 
 
 
     // Implement the identical functionality for filter and not
     function winnow(elements, qualifier, not) {
         if (isFunction(qualifier)) {
@@ -4024,47 +4028,47 @@
                 // count of unprocessed arguments
                 i = remaining,
 
                 // subordinate fulfillment data
                 resolveContexts = Array(i),
                 resolveValues = slice.call(arguments),
 
-                // the master Deferred
-                master = jQuery.Deferred(),
+                // the primary Deferred
+                primary = jQuery.Deferred(),
 
                 // subordinate callback factory
                 updateFunc = function(i) {
                     return function(value) {
                         resolveContexts[i] = this;
                         resolveValues[i] = arguments.length > 1 ? slice.call(arguments) : value;
                         if (!(--remaining)) {
-                            master.resolveWith(resolveContexts, resolveValues);
+                            primary.resolveWith(resolveContexts, resolveValues);
                         }
                     };
                 };
 
             // Single- and empty arguments are adopted like Promise.resolve
             if (remaining <= 1) {
-                adoptValue(singleValue, master.done(updateFunc(i)).resolve, master.reject,
+                adoptValue(singleValue, primary.done(updateFunc(i)).resolve, primary.reject,
                     !remaining);
 
                 // Use .then() to unwrap secondary thenables (cf. gh-3000)
-                if (master.state() === "pending" ||
+                if (primary.state() === "pending" ||
                     isFunction(resolveValues[i] && resolveValues[i].then)) {
 
-                    return master.then();
+                    return primary.then();
                 }
             }
 
             // Multiple arguments are aggregated like Promise.all array elements
             while (i--) {
-                adoptValue(resolveValues[i], updateFunc(i), master.reject);
+                adoptValue(resolveValues[i], updateFunc(i), primary.reject);
             }
 
-            return master.promise();
+            return primary.promise();
         }
     });
 
 
     // These usually indicate a programmer mistake during development,
     // warn about them ASAP rather than swallowing them by default.
     var rerrorNames = /^(Eval|Internal|Range|Reference|Syntax|Type|URI)Error$/;
@@ -5117,18 +5121,15 @@
             }
         }
 
         return fragment;
     }
 
 
-    var
-        rkeyEvent = /^key/,
-        rmouseEvent = /^(?:mouse|pointer|contextmenu|drag|drop)|click/,
-        rtypenamespace = /^([^.]*)(?:\.(.+)|)/;
+    var rtypenamespace = /^([^.]*)(?:\.(.+)|)/;
 
     function returnTrue() {
         return true;
     }
 
     function returnFalse() {
         return false;
@@ -5689,15 +5690,21 @@
                             result = {};
                         }
                         if (saved !== result) {
 
                             // Cancel the outer synthetic event
                             event.stopImmediatePropagation();
                             event.preventDefault();
-                            return result.value;
+
+                            // Support: Chrome 86+
+                            // In Chrome, if an element having a focusout handler is blurred by
+                            // clicking outside of it, it invokes the handler synchronously. If
+                            // that handler calls `.remove()` on the element, the data is cleared,
+                            // leaving `result` undefined. We need to guard against this.
+                            return result && result.value;
                         }
 
                         // If this is an inner synthetic event for an event with a bubbling surrogate
                         // (focus or blur), assume that the surrogate already propagated from triggering the
                         // native event and prevent that from happening again here.
                         // This technically gets the ordering wrong w.r.t. to `.trigger()` (in which the
                         // bubbling surrogate propagates *after* the non-bubbling base), but that seems
@@ -5854,42 +5861,15 @@
         pointerId: true,
         pointerType: true,
         screenX: true,
         screenY: true,
         targetTouches: true,
         toElement: true,
         touches: true,
-
-        which: function(event) {
-            var button = event.button;
-
-            // Add which for key events
-            if (event.which == null && rkeyEvent.test(event.type)) {
-                return event.charCode != null ? event.charCode : event.keyCode;
-            }
-
-            // Add which for click: 1 === left; 2 === middle; 3 === right
-            if (!event.which && button !== undefined && rmouseEvent.test(event.type)) {
-                if (button & 1) {
-                    return 1;
-                }
-
-                if (button & 2) {
-                    return 3;
-                }
-
-                if (button & 4) {
-                    return 2;
-                }
-
-                return 0;
-            }
-
-            return event.which;
-        }
+        which: true
     }, jQuery.event.addProp);
 
     jQuery.each({
         focus: "focusin",
         blur: "focusout"
     }, function(type, delegateType) {
         jQuery.event.special[type] = {
@@ -5910,14 +5890,20 @@
                 // Force setup before trigger
                 leverageNative(this, type);
 
                 // Return non-false to allow normal event-path propagation
                 return true;
             },
 
+            // Suppress native focus or blur as it's already being fired
+            // in leverageNative.
+            _default: function() {
+                return true;
+            },
+
             delegateType: delegateType
         };
     });
 
     // Create mouseenter/leave events using mouseover/out and event-time checks
     // so that event delegation works in jQuery.
     // Do the same for pointerenter/pointerleave and pointerover/pointerout
@@ -6581,32 +6567,51 @@
             },
 
             // Support: IE 9 - 11+, Edge 15 - 18+
             // IE/Edge misreport `getComputedStyle` of table rows with width/height
             // set in CSS while `offset*` properties report correct values.
             // Behavior in IE 9 is more subtle than in newer versions & it passes
             // some versions of this test; make sure not to make it pass there!
+            //
+            // Support: Firefox 70+
+            // Only Firefox includes border widths
+            // in computed dimensions. (gh-4529)
             reliableTrDimensions: function() {
                 var table, tr, trChild, trStyle;
                 if (reliableTrDimensionsVal == null) {
                     table = document.createElement("table");
                     tr = document.createElement("tr");
                     trChild = document.createElement("div");
 
-                    table.style.cssText = "position:absolute;left:-11111px";
+                    table.style.cssText = "position:absolute;left:-11111px;border-collapse:separate";
+                    tr.style.cssText = "border:1px solid";
+
+                    // Support: Chrome 86+
+                    // Height set through cssText does not get applied.
+                    // Computed height then comes back as 0.
                     tr.style.height = "1px";
                     trChild.style.height = "9px";
 
+                    // Support: Android 8 Chrome 86+
+                    // In our bodyBackground.html iframe,
+                    // display for all div elements is set to "inline",
+                    // which causes a problem only in Android 8 Chrome 86.
+                    // Ensuring the div is display: block
+                    // gets around this issue.
+                    trChild.style.display = "block";
+
                     documentElement
                         .appendChild(table)
                         .appendChild(tr)
                         .appendChild(trChild);
 
                     trStyle = window.getComputedStyle(tr);
-                    reliableTrDimensionsVal = parseInt(trStyle.height) > 3;
+                    reliableTrDimensionsVal = (parseInt(trStyle.height, 10) +
+                        parseInt(trStyle.borderTopWidth, 10) +
+                        parseInt(trStyle.borderBottomWidth, 10)) === tr.offsetHeight;
 
                     documentElement.removeChild(table);
                 }
                 return reliableTrDimensionsVal;
             }
         });
     })();
@@ -7813,14 +7818,15 @@
                     var anim = Animation(this, jQuery.extend({}, prop), optall);
 
                     // Empty animations, or finishing resolves immediately
                     if (empty || dataPriv.get(this, "finish")) {
                         anim.stop(true);
                     }
                 };
+
             doAnimation.finish = doAnimation;
 
             return empty || optall.queue === false ?
                 this.each(doAnimation) :
                 this.queue(optall.queue, doAnimation);
         },
         stop: function(type, clearQueue, gotoEnd) {
@@ -8764,17 +8770,15 @@
             while ((cur = eventPath[i++]) && !event.isPropagationStopped()) {
                 lastElement = cur;
                 event.type = i > 1 ?
                     bubbleType :
                     special.bindType || type;
 
                 // jQuery handler
-                handle = (
-                        dataPriv.get(cur, "events") || Object.create(null)
-                    )[event.type] &&
+                handle = (dataPriv.get(cur, "events") || Object.create(null))[event.type] &&
                     dataPriv.get(cur, "handle");
                 if (handle) {
                     handle.apply(cur, data);
                 }
 
                 // Native handler
                 handle = ontype && cur[ontype];
@@ -8917,29 +8921,34 @@
 
     var rquery = (/\?/);
 
 
 
     // Cross-browser xml parsing
     jQuery.parseXML = function(data) {
-        var xml;
+        var xml, parserErrorElem;
         if (!data || typeof data !== "string") {
             return null;
         }
 
         // Support: IE 9 - 11 only
         // IE throws on parseFromString with invalid input.
         try {
             xml = (new window.DOMParser()).parseFromString(data, "text/xml");
-        } catch (e) {
-            xml = undefined;
-        }
+        } catch (e) {}
 
-        if (!xml || xml.getElementsByTagName("parsererror").length) {
-            jQuery.error("Invalid XML: " + data);
+        parserErrorElem = xml && xml.getElementsByTagName("parsererror")[0];
+        if (!xml || parserErrorElem) {
+            jQuery.error("Invalid XML: " + (
+                parserErrorElem ?
+                jQuery.map(parserErrorElem.childNodes, function(el) {
+                    return el.textContent;
+                }).join("\n") :
+                data
+            ));
         }
         return xml;
     };
 
 
     var
         rbracket = /\[\]$/,
@@ -9029,47 +9038,45 @@
     jQuery.fn.extend({
         serialize: function() {
             return jQuery.param(this.serializeArray());
         },
         serializeArray: function() {
             return this.map(function() {
 
-                    // Can add propHook for "elements" to filter or add form elements
-                    var elements = jQuery.prop(this, "elements");
-                    return elements ? jQuery.makeArray(elements) : this;
-                })
-                .filter(function() {
-                    var type = this.type;
-
-                    // Use .is( ":disabled" ) so that fieldset[disabled] works
-                    return this.name && !jQuery(this).is(":disabled") &&
-                        rsubmittable.test(this.nodeName) && !rsubmitterTypes.test(type) &&
-                        (this.checked || !rcheckableType.test(type));
-                })
-                .map(function(_i, elem) {
-                    var val = jQuery(this).val();
+                // Can add propHook for "elements" to filter or add form elements
+                var elements = jQuery.prop(this, "elements");
+                return elements ? jQuery.makeArray(elements) : this;
+            }).filter(function() {
+                var type = this.type;
+
+                // Use .is( ":disabled" ) so that fieldset[disabled] works
+                return this.name && !jQuery(this).is(":disabled") &&
+                    rsubmittable.test(this.nodeName) && !rsubmitterTypes.test(type) &&
+                    (this.checked || !rcheckableType.test(type));
+            }).map(function(_i, elem) {
+                var val = jQuery(this).val();
 
-                    if (val == null) {
-                        return null;
-                    }
+                if (val == null) {
+                    return null;
+                }
 
-                    if (Array.isArray(val)) {
-                        return jQuery.map(val, function(val) {
-                            return {
-                                name: elem.name,
-                                value: val.replace(rCRLF, "\r\n")
-                            };
-                        });
-                    }
+                if (Array.isArray(val)) {
+                    return jQuery.map(val, function(val) {
+                        return {
+                            name: elem.name,
+                            value: val.replace(rCRLF, "\r\n")
+                        };
+                    });
+                }
 
-                    return {
-                        name: elem.name,
-                        value: val.replace(rCRLF, "\r\n")
-                    };
-                }).get();
+                return {
+                    name: elem.name,
+                    value: val.replace(rCRLF, "\r\n")
+                };
+            }).get();
         }
     });
 
 
     var
         r20 = /%20/g,
         rhash = /#.*$/,
@@ -9100,14 +9107,15 @@
         transports = {},
 
         // Avoid comment-prolog char sequence (#10098); must appease lint and evade compression
         allTypes = "*/".concat("*"),
 
         // Anchor tag for parsing the document origin
         originAnchor = document.createElement("a");
+
     originAnchor.href = location.href;
 
     // Base "constructor" for jQuery.ajaxPrefilter and jQuery.ajaxTransport
     function addToPrefiltersOrTransports(structure) {
 
         // dataTypeExpression is optional and defaults to "*"
         return function(dataTypeExpression, func) {
@@ -9797,16 +9805,18 @@
                 isSuccess = status >= 200 && status < 300 || status === 304;
 
                 // Get response data
                 if (responses) {
                     response = ajaxHandleResponses(s, jqXHR, responses);
                 }
 
-                // Use a noop converter for missing script
-                if (!isSuccess && jQuery.inArray("script", s.dataTypes) > -1) {
+                // Use a noop converter for missing script but not if jsonp
+                if (!isSuccess &&
+                    jQuery.inArray("script", s.dataTypes) > -1 &&
+                    jQuery.inArray("json", s.dataTypes) < 0) {
                     s.converters["text script"] = function() {};
                 }
 
                 // Convert no matter what (that way responseXXX fields are always set)
                 response = ajaxConvert(s, response, jqXHR, isSuccess);
 
                 // If successful, handle type chaining
@@ -10541,20 +10551,14 @@
                 props.left = (options.left - curOffset.left) + curLeft;
             }
 
             if ("using" in options) {
                 options.using.call(elem, props);
 
             } else {
-                if (typeof props.top === "number") {
-                    props.top += "px";
-                }
-                if (typeof props.left === "number") {
-                    props.left += "px";
-                }
                 curElem.css(props);
             }
         }
     };
 
     jQuery.fn.extend({
 
@@ -10728,59 +10732,58 @@
 
     // Create innerHeight, innerWidth, height, width, outerHeight and outerWidth methods
     jQuery.each({
         Height: "height",
         Width: "width"
     }, function(name, type) {
         jQuery.each({
-                padding: "inner" + name,
-                content: type,
-                "": "outer" + name
-            },
-            function(defaultExtra, funcName) {
-
-                // Margin is only for outerHeight, outerWidth
-                jQuery.fn[funcName] = function(margin, value) {
-                    var chainable = arguments.length && (defaultExtra || typeof margin !== "boolean"),
-                        extra = defaultExtra || (margin === true || value === true ? "margin" : "border");
-
-                    return access(this, function(elem, type, value) {
-                        var doc;
-
-                        if (isWindow(elem)) {
-
-                            // $( window ).outerWidth/Height return w/h including scrollbars (gh-1729)
-                            return funcName.indexOf("outer") === 0 ?
-                                elem["inner" + name] :
-                                elem.document.documentElement["client" + name];
-                        }
-
-                        // Get document width or height
-                        if (elem.nodeType === 9) {
-                            doc = elem.documentElement;
-
-                            // Either scroll[Width/Height] or offset[Width/Height] or client[Width/Height],
-                            // whichever is greatest
-                            return Math.max(
-                                elem.body["scroll" + name], doc["scroll" + name],
-                                elem.body["offset" + name], doc["offset" + name],
-                                doc["client" + name]
-                            );
-                        }
+            padding: "inner" + name,
+            content: type,
+            "": "outer" + name
+        }, function(defaultExtra, funcName) {
+
+            // Margin is only for outerHeight, outerWidth
+            jQuery.fn[funcName] = function(margin, value) {
+                var chainable = arguments.length && (defaultExtra || typeof margin !== "boolean"),
+                    extra = defaultExtra || (margin === true || value === true ? "margin" : "border");
+
+                return access(this, function(elem, type, value) {
+                    var doc;
+
+                    if (isWindow(elem)) {
+
+                        // $( window ).outerWidth/Height return w/h including scrollbars (gh-1729)
+                        return funcName.indexOf("outer") === 0 ?
+                            elem["inner" + name] :
+                            elem.document.documentElement["client" + name];
+                    }
+
+                    // Get document width or height
+                    if (elem.nodeType === 9) {
+                        doc = elem.documentElement;
+
+                        // Either scroll[Width/Height] or offset[Width/Height] or client[Width/Height],
+                        // whichever is greatest
+                        return Math.max(
+                            elem.body["scroll" + name], doc["scroll" + name],
+                            elem.body["offset" + name], doc["offset" + name],
+                            doc["client" + name]
+                        );
+                    }
 
-                        return value === undefined ?
+                    return value === undefined ?
 
-                            // Get width or height on the element, requesting but not forcing parseFloat
-                            jQuery.css(elem, type, extra) :
+                        // Get width or height on the element, requesting but not forcing parseFloat
+                        jQuery.css(elem, type, extra) :
 
-                            // Set width or height on the element
-                            jQuery.style(elem, type, value, extra);
-                    }, type, chainable ? margin : undefined, chainable);
-                };
-            });
+                        // Set width or height on the element
+                        jQuery.style(elem, type, value, extra);
+                }, type, chainable ? margin : undefined, chainable);
+            };
+        });
     });
 
 
     jQuery.each([
         "ajaxStart",
         "ajaxStop",
         "ajaxComplete",
@@ -10817,26 +10820,28 @@
         },
 
         hover: function(fnOver, fnOut) {
             return this.mouseenter(fnOver).mouseleave(fnOut || fnOver);
         }
     });
 
-    jQuery.each(("blur focus focusin focusout resize scroll click dblclick " +
+    jQuery.each(
+        ("blur focus focusin focusout resize scroll click dblclick " +
             "mousedown mouseup mousemove mouseover mouseout mouseenter mouseleave " +
             "change select submit keydown keypress keyup contextmenu").split(" "),
         function(_i, name) {
 
             // Handle event binding
             jQuery.fn[name] = function(data, fn) {
                 return arguments.length > 0 ?
                     this.on(name, null, data, fn) :
                     this.trigger(name);
             };
-        });
+        }
+    );
 
 
 
 
     // Support: Android <=4.0 only
     // Make sure we trim BOM and NBSP
     var rtrim = /^[\s\uFEFF\xA0]+|[\s\uFEFF\xA0]+$/g;
```

### Comparing `Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/_static/jquery.js` & `Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/_static/jquery.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! jQuery v3.5.1 | (c) JS Foundation and other contributors | jquery.org/license */ ! function(e, t) {
+/*! jQuery v3.6.0 | (c) OpenJS Foundation and other contributors | jquery.org/license */ ! function(e, t) {
     "use strict";
     "object" == typeof module && "object" == typeof module.exports ? module.exports = e.document ? t(e, !0) : function(e) {
         if (!e.document) throw new Error("jQuery requires a window with a document");
         return t(e)
     } : t(e)
 }("undefined" != typeof window ? window : this, function(C, e) {
     "use strict";
@@ -19,15 +19,15 @@
         n = {},
         o = n.toString,
         v = n.hasOwnProperty,
         a = v.toString,
         l = a.call(Object),
         y = {},
         m = function(e) {
-            return "function" == typeof e && "number" != typeof e.nodeType
+            return "function" == typeof e && "number" != typeof e.nodeType && "function" != typeof e.item
         },
         x = function(e) {
             return null != e && e === e.window
         },
         E = C.document,
         c = {
             type: !0,
@@ -42,15 +42,15 @@
             for (r in c)(i = t[r] || t.getAttribute && t.getAttribute(r)) && o.setAttribute(r, i);
         n.head.appendChild(o).parentNode.removeChild(o)
     }
 
     function w(e) {
         return null == e ? e + "" : "object" == typeof e || "function" == typeof e ? n[o.call(e)] || "object" : typeof e
     }
-    var f = "3.5.1",
+    var f = "3.6.0",
         S = function(e, t) {
             return new S.fn.init(e, t)
         };
 
     function p(e) {
         var t = !!e && "length" in e && e.length,
             n = w(e);
@@ -182,18 +182,18 @@
             p = n.document,
             k = 0,
             r = 0,
             m = ue(),
             x = ue(),
             A = ue(),
             N = ue(),
-            D = function(e, t) {
+            j = function(e, t) {
                 return e === t && (l = !0), 0
             },
-            j = {}.hasOwnProperty,
+            D = {}.hasOwnProperty,
             t = [],
             q = t.pop,
             L = t.push,
             H = t.push,
             O = t.slice,
             P = function(e, t) {
                 for (var n = 0, r = e.length; n < r; n++)
@@ -360,16 +360,16 @@
             })
         }
 
         function ye(e) {
             return e && "undefined" != typeof e.getElementsByTagName && e
         }
         for (e in d = se.support = {}, i = se.isXML = function(e) {
-                var t = e.namespaceURI,
-                    n = (e.ownerDocument || e).documentElement;
+                var t = e && e.namespaceURI,
+                    n = e && (e.ownerDocument || e).documentElement;
                 return !Y.test(t || n && n.nodeName || "HTML")
             }, T = se.setDocument = function(e) {
                 var t, n, r = e ? e.ownerDocument || e : p;
                 return r != C && 9 === r.nodeType && r.documentElement && (a = (C = r).documentElement, E = !i(C), p != C && (n = C.defaultView) && n.top !== n && (n.addEventListener ? n.addEventListener("unload", oe, !1) : n.attachEvent && n.attachEvent("onunload", oe)), d.scope = ce(function(e) {
                     return a.appendChild(e).appendChild(C.createElement("div")), "undefined" != typeof e.querySelectorAll && !e.querySelectorAll(":scope fieldset div").length
                 }), d.attributes = ce(function(e) {
                     return e.className = "i", !e.getAttribute("className")
@@ -431,15 +431,15 @@
                         r = t && t.parentNode;
                     return e === r || !(!r || 1 !== r.nodeType || !(n.contains ? n.contains(r) : e.compareDocumentPosition && 16 & e.compareDocumentPosition(r)))
                 } : function(e, t) {
                     if (t)
                         while (t = t.parentNode)
                             if (t === e) return !0;
                     return !1
-                }, D = t ? function(e, t) {
+                }, j = t ? function(e, t) {
                     if (e === t) return l = !0, 0;
                     var n = !e.compareDocumentPosition - !t.compareDocumentPosition;
                     return n || (1 & (n = (e.ownerDocument || e) == (t.ownerDocument || t) ? e.compareDocumentPosition(t) : 1) || !d.sortDetached && t.compareDocumentPosition(e) === n ? e == C || e.ownerDocument == p && y(p, e) ? -1 : t == C || t.ownerDocument == p && y(p, t) ? 1 : u ? P(u, e) - P(u, t) : 0 : 4 & n ? -1 : 1)
                 } : function(e, t) {
                     if (e === t) return l = !0, 0;
                     var n, r = 0,
                         i = e.parentNode,
@@ -466,25 +466,25 @@
                 }
                 return 0 < se(t, C, null, [e]).length
             }, se.contains = function(e, t) {
                 return (e.ownerDocument || e) != C && T(e), y(e, t)
             }, se.attr = function(e, t) {
                 (e.ownerDocument || e) != C && T(e);
                 var n = b.attrHandle[t.toLowerCase()],
-                    r = n && j.call(b.attrHandle, t.toLowerCase()) ? n(e, t, !E) : void 0;
+                    r = n && D.call(b.attrHandle, t.toLowerCase()) ? n(e, t, !E) : void 0;
                 return void 0 !== r ? r : d.attributes || !E ? e.getAttribute(t) : (r = e.getAttributeNode(t)) && r.specified ? r.value : null
             }, se.escape = function(e) {
                 return (e + "").replace(re, ie)
             }, se.error = function(e) {
                 throw new Error("Syntax error, unrecognized expression: " + e)
             }, se.uniqueSort = function(e) {
                 var t, n = [],
                     r = 0,
                     i = 0;
-                if (l = !d.detectDuplicates, u = !d.sortStable && e.slice(0), e.sort(D), l) {
+                if (l = !d.detectDuplicates, u = !d.sortStable && e.slice(0), e.sort(j), l) {
                     while (t = e[i++]) t === e[i] && (r = n.push(i));
                     while (r--) e.splice(n[r], 1)
                 }
                 return u = null, e
             }, o = se.getText = function(e) {
                 var t, n = "",
                     r = 0,
@@ -880,15 +880,15 @@
                     if ((u = b.find[s]) && (r = u(a.matches[0].replace(te, ne), ee.test(o[0].type) && ye(t.parentNode) || t))) {
                         if (o.splice(i, 1), !(e = r.length && xe(o))) return H.apply(n, r), n;
                         break
                     }
                 }
             }
             return (l || f(e, c))(r, t, !E, n, !t || ee.test(e) && ye(t.parentNode) || t), n
-        }, d.sortStable = S.split("").sort(D).join("") === S, d.detectDuplicates = !!l, T(), d.sortDetached = ce(function(e) {
+        }, d.sortStable = S.split("").sort(j).join("") === S, d.detectDuplicates = !!l, T(), d.sortDetached = ce(function(e) {
             return 1 & e.compareDocumentPosition(C.createElement("fieldset"))
         }), ce(function(e) {
             return e.innerHTML = "<a href='#'></a>", "#" === e.firstChild.getAttribute("href")
         }) || fe("type|href|height|width", function(e, t, n) {
             if (!n) return e.getAttribute(t, "type" === t.toLowerCase() ? 1 : 2)
         }), d.attributes && ce(function(e) {
             return e.innerHTML = "<input/>", e.firstChild.setAttribute("value", ""), "" === e.firstChild.getAttribute("value")
@@ -918,15 +918,15 @@
         k = S.expr.match.needsContext;
 
     function A(e, t) {
         return e.nodeName && e.nodeName.toLowerCase() === t.toLowerCase()
     }
     var N = /^<([a-z][^\/\0>:\x20\t\r\n\f]*)[\x20\t\r\n\f]*\/?>(?:<\/\1>|)$/i;
 
-    function D(e, n, r) {
+    function j(e, n, r) {
         return m(n) ? S.grep(e, function(e, t) {
             return !!n.call(e, t, e) !== r
         }) : n.nodeType ? S.grep(e, function(e) {
             return e === n !== r
         }) : "string" != typeof n ? S.grep(e, function(e) {
             return -1 < i.call(n, e) !== r
         }) : S.filter(n, e, r)
@@ -944,38 +944,38 @@
                 for (t = 0; t < r; t++)
                     if (S.contains(i[t], this)) return !0
             }));
             for (n = this.pushStack([]), t = 0; t < r; t++) S.find(e, i[t], n);
             return 1 < r ? S.uniqueSort(n) : n
         },
         filter: function(e) {
-            return this.pushStack(D(this, e || [], !1))
+            return this.pushStack(j(this, e || [], !1))
         },
         not: function(e) {
-            return this.pushStack(D(this, e || [], !0))
+            return this.pushStack(j(this, e || [], !0))
         },
         is: function(e) {
-            return !!D(this, "string" == typeof e && k.test(e) ? S(e) : e || [], !1).length
+            return !!j(this, "string" == typeof e && k.test(e) ? S(e) : e || [], !1).length
         }
     });
-    var j, q = /^(?:\s*(<[\w\W]+>)[^>]*|#([\w-]+))$/;
+    var D, q = /^(?:\s*(<[\w\W]+>)[^>]*|#([\w-]+))$/;
     (S.fn.init = function(e, t, n) {
         var r, i;
         if (!e) return this;
-        if (n = n || j, "string" == typeof e) {
+        if (n = n || D, "string" == typeof e) {
             if (!(r = "<" === e[0] && ">" === e[e.length - 1] && 3 <= e.length ? [null, e, null] : q.exec(e)) || !r[1] && t) return !t || t.jquery ? (t || n).find(e) : this.constructor(t).find(e);
             if (r[1]) {
                 if (t = t instanceof S ? t[0] : t, S.merge(this, S.parseHTML(r[1], t && t.nodeType ? t.ownerDocument || t : E, !0)), N.test(r[1]) && S.isPlainObject(t))
                     for (r in t) m(this[r]) ? this[r](t[r]) : this.attr(r, t[r]);
                 return this
             }
             return (i = E.getElementById(r[2])) && (this[0] = i, this.length = 1), this
         }
         return e.nodeType ? (this[0] = e, this.length = 1, this) : m(e) ? void 0 !== n.ready ? n.ready(e) : e(S) : S.makeArray(e, this)
-    }).prototype = S.fn, j = S(E);
+    }).prototype = S.fn, D = S(E);
     var L = /^(?:parents|prev(?:Until|All))/,
         H = {
             children: !0,
             contents: !0,
             next: !0,
             prev: !0
         };
@@ -1514,72 +1514,70 @@
             if (r && -1 < S.inArray(o, r)) i && i.push(o);
             else if (l = ie(o), a = ve(f.appendChild(o), "script"), l && ye(a), n) {
             c = 0;
             while (o = a[c++]) he.test(o.type || "") && n.push(o)
         }
         return f
     }
-    var be = /^key/,
-        we = /^(?:mouse|pointer|contextmenu|drag|drop)|click/,
-        Te = /^([^.]*)(?:\.(.+)|)/;
+    var be = /^([^.]*)(?:\.(.+)|)/;
 
-    function Ce() {
+    function we() {
         return !0
     }
 
-    function Ee() {
+    function Te() {
         return !1
     }
 
-    function Se(e, t) {
+    function Ce(e, t) {
         return e === function() {
             try {
                 return E.activeElement
             } catch (e) {}
         }() == ("focus" === t)
     }
 
-    function ke(e, t, n, r, i, o) {
+    function Ee(e, t, n, r, i, o) {
         var a, s;
         if ("object" == typeof t) {
-            for (s in "string" != typeof n && (r = r || n, n = void 0), t) ke(e, s, n, r, t[s], o);
+            for (s in "string" != typeof n && (r = r || n, n = void 0), t) Ee(e, s, n, r, t[s], o);
             return e
         }
-        if (null == r && null == i ? (i = n, r = n = void 0) : null == i && ("string" == typeof n ? (i = r, r = void 0) : (i = r, r = n, n = void 0)), !1 === i) i = Ee;
+        if (null == r && null == i ? (i = n, r = n = void 0) : null == i && ("string" == typeof n ? (i = r, r = void 0) : (i = r, r = n, n = void 0)), !1 === i) i = Te;
         else if (!i) return e;
         return 1 === o && (a = i, (i = function(e) {
             return S().off(e), a.apply(this, arguments)
         }).guid = a.guid || (a.guid = S.guid++)), e.each(function() {
             S.event.add(this, t, i, r, n)
         })
     }
 
-    function Ae(e, i, o) {
+    function Se(e, i, o) {
         o ? (Y.set(e, i, !1), S.event.add(e, i, {
             namespace: !1,
             handler: function(e) {
                 var t, n, r = Y.get(this, i);
                 if (1 & e.isTrigger && this[i]) {
                     if (r.length)(S.event.special[i] || {}).delegateType && e.stopPropagation();
-                    else if (r = s.call(arguments), Y.set(this, i, r), t = o(this, i), this[i](), r !== (n = Y.get(this, i)) || t ? Y.set(this, i, !1) : n = {}, r !== n) return e.stopImmediatePropagation(), e.preventDefault(), n.value
+                    else if (r = s.call(arguments), Y.set(this, i, r), t = o(this, i), this[i](), r !== (n = Y.get(this, i)) || t ? Y.set(this, i, !1) : n = {}, r !== n) return e.stopImmediatePropagation(), e.preventDefault(), n && n.value
                 } else r.length && (Y.set(this, i, {
                     value: S.event.trigger(S.extend(r[0], S.Event.prototype), r.slice(1), this)
                 }), e.stopImmediatePropagation())
             }
-        })) : void 0 === Y.get(e, i) && S.event.add(e, i, Ce)
+        })) : void 0 === Y.get(e, i) && S.event.add(e, i, we)
     }
     S.event = {
         global: {},
         add: function(t, e, n, r, i) {
             var o, a, s, u, l, c, f, p, d, h, g, v = Y.get(t);
             if (V(t)) {
                 n.handler && (n = (o = n).handler, i = o.selector), i && S.find.matchesSelector(re, i), n.guid || (n.guid = S.guid++), (u = v.events) || (u = v.events = Object.create(null)), (a = v.handle) || (a = v.handle = function(e) {
                     return "undefined" != typeof S && S.event.triggered !== e.type ? S.event.dispatch.apply(t, arguments) : void 0
                 }), l = (e = (e || "").match(P) || [""]).length;
-                while (l--) d = g = (s = Te.exec(e[l]) || [])[1], h = (s[2] || "").split(".").sort(), d && (f = S.event.special[d] || {}, d = (i ? f.delegateType : f.bindType) || d, f = S.event.special[d] || {}, c = S.extend({
+                while (l--) d = g = (s = be.exec(e[l]) || [])[1], h = (s[2] || "").split(".").sort(), d && (f = S.event.special[d] || {}, d = (i ? f.delegateType : f.bindType) || d, f = S.event.special[d] || {}, c = S.extend({
                     type: d,
                     origType: g,
                     data: r,
                     handler: n,
                     guid: n.guid,
                     selector: i,
                     needsContext: i && S.expr.match.needsContext.test(i),
@@ -1588,15 +1586,15 @@
             }
         },
         remove: function(e, t, n, r, i) {
             var o, a, s, u, l, c, f, p, d, h, g, v = Y.hasData(e) && Y.get(e);
             if (v && (u = v.events)) {
                 l = (t = (t || "").match(P) || [""]).length;
                 while (l--)
-                    if (d = g = (s = Te.exec(t[l]) || [])[1], h = (s[2] || "").split(".").sort(), d) {
+                    if (d = g = (s = be.exec(t[l]) || [])[1], h = (s[2] || "").split(".").sort(), d) {
                         f = S.event.special[d] || {}, p = u[d = (r ? f.delegateType : f.bindType) || d] || [], s = s[2] && new RegExp("(^|\\.)" + h.join("\\.(?:.*\\.|)") + "(\\.|$)"), a = o = p.length;
                         while (o--) c = p[o], !i && g !== c.origType || n && n.guid !== c.guid || s && !s.test(c.namespace) || r && r !== c.selector && ("**" !== r || !c.selector) || (p.splice(o, 1), c.selector && p.delegateCount--, f.remove && f.remove.call(e, c));
                         a && !p.length && (f.teardown && !1 !== f.teardown.call(e, h, v.handle) || S.removeEvent(e, d, v.handle), delete u[d])
                     } else
                         for (d in u) S.event.remove(e, d + t[l], n, r, !0);
                 S.isEmptyObject(u) && Y.remove(e, "handle events")
             }
@@ -1658,19 +1656,19 @@
         special: {
             load: {
                 noBubble: !0
             },
             click: {
                 setup: function(e) {
                     var t = this || e;
-                    return pe.test(t.type) && t.click && A(t, "input") && Ae(t, "click", Ce), !1
+                    return pe.test(t.type) && t.click && A(t, "input") && Se(t, "click", we), !1
                 },
                 trigger: function(e) {
                     var t = this || e;
-                    return pe.test(t.type) && t.click && A(t, "input") && Ae(t, "click"), !0
+                    return pe.test(t.type) && t.click && A(t, "input") && Se(t, "click"), !0
                 },
                 _default: function(e) {
                     var t = e.target;
                     return pe.test(t.type) && t.click && A(t, "input") && Y.get(t, "click") || A(t, "a")
                 }
             },
             beforeunload: {
@@ -1679,32 +1677,32 @@
                 }
             }
         }
     }, S.removeEvent = function(e, t, n) {
         e.removeEventListener && e.removeEventListener(t, n)
     }, S.Event = function(e, t) {
         if (!(this instanceof S.Event)) return new S.Event(e, t);
-        e && e.type ? (this.originalEvent = e, this.type = e.type, this.isDefaultPrevented = e.defaultPrevented || void 0 === e.defaultPrevented && !1 === e.returnValue ? Ce : Ee, this.target = e.target && 3 === e.target.nodeType ? e.target.parentNode : e.target, this.currentTarget = e.currentTarget, this.relatedTarget = e.relatedTarget) : this.type = e, t && S.extend(this, t), this.timeStamp = e && e.timeStamp || Date.now(), this[S.expando] = !0
+        e && e.type ? (this.originalEvent = e, this.type = e.type, this.isDefaultPrevented = e.defaultPrevented || void 0 === e.defaultPrevented && !1 === e.returnValue ? we : Te, this.target = e.target && 3 === e.target.nodeType ? e.target.parentNode : e.target, this.currentTarget = e.currentTarget, this.relatedTarget = e.relatedTarget) : this.type = e, t && S.extend(this, t), this.timeStamp = e && e.timeStamp || Date.now(), this[S.expando] = !0
     }, S.Event.prototype = {
         constructor: S.Event,
-        isDefaultPrevented: Ee,
-        isPropagationStopped: Ee,
-        isImmediatePropagationStopped: Ee,
+        isDefaultPrevented: Te,
+        isPropagationStopped: Te,
+        isImmediatePropagationStopped: Te,
         isSimulated: !1,
         preventDefault: function() {
             var e = this.originalEvent;
-            this.isDefaultPrevented = Ce, e && !this.isSimulated && e.preventDefault()
+            this.isDefaultPrevented = we, e && !this.isSimulated && e.preventDefault()
         },
         stopPropagation: function() {
             var e = this.originalEvent;
-            this.isPropagationStopped = Ce, e && !this.isSimulated && e.stopPropagation()
+            this.isPropagationStopped = we, e && !this.isSimulated && e.stopPropagation()
         },
         stopImmediatePropagation: function() {
             var e = this.originalEvent;
-            this.isImmediatePropagationStopped = Ce, e && !this.isSimulated && e.stopImmediatePropagation(), this.stopPropagation()
+            this.isImmediatePropagationStopped = we, e && !this.isSimulated && e.stopImmediatePropagation(), this.stopPropagation()
         }
     }, S.each({
         altKey: !0,
         bubbles: !0,
         cancelable: !0,
         changedTouches: !0,
         ctrlKey: !0,
@@ -1729,28 +1727,28 @@
         pointerId: !0,
         pointerType: !0,
         screenX: !0,
         screenY: !0,
         targetTouches: !0,
         toElement: !0,
         touches: !0,
-        which: function(e) {
-            var t = e.button;
-            return null == e.which && be.test(e.type) ? null != e.charCode ? e.charCode : e.keyCode : !e.which && void 0 !== t && we.test(e.type) ? 1 & t ? 1 : 2 & t ? 3 : 4 & t ? 2 : 0 : e.which
-        }
+        which: !0
     }, S.event.addProp), S.each({
         focus: "focusin",
         blur: "focusout"
     }, function(e, t) {
         S.event.special[e] = {
             setup: function() {
-                return Ae(this, e, Se), !1
+                return Se(this, e, Ce), !1
             },
             trigger: function() {
-                return Ae(this, e), !0
+                return Se(this, e), !0
+            },
+            _default: function() {
+                return !0
             },
             delegateType: t
         }
     }), S.each({
         mouseenter: "mouseover",
         mouseleave: "mouseout",
         pointerenter: "pointerover",
@@ -1763,95 +1761,95 @@
                 var t, n = e.relatedTarget,
                     r = e.handleObj;
                 return n && (n === this || S.contains(this, n)) || (e.type = r.origType, t = r.handler.apply(this, arguments), e.type = i), t
             }
         }
     }), S.fn.extend({
         on: function(e, t, n, r) {
-            return ke(this, e, t, n, r)
+            return Ee(this, e, t, n, r)
         },
         one: function(e, t, n, r) {
-            return ke(this, e, t, n, r, 1)
+            return Ee(this, e, t, n, r, 1)
         },
         off: function(e, t, n) {
             var r, i;
             if (e && e.preventDefault && e.handleObj) return r = e.handleObj, S(e.delegateTarget).off(r.namespace ? r.origType + "." + r.namespace : r.origType, r.selector, r.handler), this;
             if ("object" == typeof e) {
                 for (i in e) this.off(i, t, e[i]);
                 return this
             }
-            return !1 !== t && "function" != typeof t || (n = t, t = void 0), !1 === n && (n = Ee), this.each(function() {
+            return !1 !== t && "function" != typeof t || (n = t, t = void 0), !1 === n && (n = Te), this.each(function() {
                 S.event.remove(this, e, n, t)
             })
         }
     });
-    var Ne = /<script|<style|<link/i,
-        De = /checked\s*(?:[^=]|=\s*.checked.)/i,
-        je = /^\s*<!(?:\[CDATA\[|--)|(?:\]\]|--)>\s*$/g;
+    var ke = /<script|<style|<link/i,
+        Ae = /checked\s*(?:[^=]|=\s*.checked.)/i,
+        Ne = /^\s*<!(?:\[CDATA\[|--)|(?:\]\]|--)>\s*$/g;
 
-    function qe(e, t) {
+    function je(e, t) {
         return A(e, "table") && A(11 !== t.nodeType ? t : t.firstChild, "tr") && S(e).children("tbody")[0] || e
     }
 
-    function Le(e) {
+    function De(e) {
         return e.type = (null !== e.getAttribute("type")) + "/" + e.type, e
     }
 
-    function He(e) {
+    function qe(e) {
         return "true/" === (e.type || "").slice(0, 5) ? e.type = e.type.slice(5) : e.removeAttribute("type"), e
     }
 
-    function Oe(e, t) {
+    function Le(e, t) {
         var n, r, i, o, a, s;
         if (1 === t.nodeType) {
             if (Y.hasData(e) && (s = Y.get(e).events))
                 for (i in Y.remove(t, "handle events"), s)
                     for (n = 0, r = s[i].length; n < r; n++) S.event.add(t, i, s[i][n]);
             Q.hasData(e) && (o = Q.access(e), a = S.extend({}, o), Q.set(t, a))
         }
     }
 
-    function Pe(n, r, i, o) {
+    function He(n, r, i, o) {
         r = g(r);
         var e, t, a, s, u, l, c = 0,
             f = n.length,
             p = f - 1,
             d = r[0],
             h = m(d);
-        if (h || 1 < f && "string" == typeof d && !y.checkClone && De.test(d)) return n.each(function(e) {
+        if (h || 1 < f && "string" == typeof d && !y.checkClone && Ae.test(d)) return n.each(function(e) {
             var t = n.eq(e);
-            h && (r[0] = d.call(this, e, t.html())), Pe(t, r, i, o)
+            h && (r[0] = d.call(this, e, t.html())), He(t, r, i, o)
         });
         if (f && (t = (e = xe(r, n[0].ownerDocument, !1, n, o)).firstChild, 1 === e.childNodes.length && (e = t), t || o)) {
-            for (s = (a = S.map(ve(e, "script"), Le)).length; c < f; c++) u = e, c !== p && (u = S.clone(u, !0, !0), s && S.merge(a, ve(u, "script"))), i.call(n[c], u, c);
+            for (s = (a = S.map(ve(e, "script"), De)).length; c < f; c++) u = e, c !== p && (u = S.clone(u, !0, !0), s && S.merge(a, ve(u, "script"))), i.call(n[c], u, c);
             if (s)
-                for (l = a[a.length - 1].ownerDocument, S.map(a, He), c = 0; c < s; c++) u = a[c], he.test(u.type || "") && !Y.access(u, "globalEval") && S.contains(l, u) && (u.src && "module" !== (u.type || "").toLowerCase() ? S._evalUrl && !u.noModule && S._evalUrl(u.src, {
+                for (l = a[a.length - 1].ownerDocument, S.map(a, qe), c = 0; c < s; c++) u = a[c], he.test(u.type || "") && !Y.access(u, "globalEval") && S.contains(l, u) && (u.src && "module" !== (u.type || "").toLowerCase() ? S._evalUrl && !u.noModule && S._evalUrl(u.src, {
                     nonce: u.nonce || u.getAttribute("nonce")
-                }, l) : b(u.textContent.replace(je, ""), u, l))
+                }, l) : b(u.textContent.replace(Ne, ""), u, l))
         }
         return n
     }
 
-    function Re(e, t, n) {
+    function Oe(e, t, n) {
         for (var r, i = t ? S.filter(t, e) : e, o = 0; null != (r = i[o]); o++) n || 1 !== r.nodeType || S.cleanData(ve(r)), r.parentNode && (n && ie(r) && ye(ve(r, "script")), r.parentNode.removeChild(r));
         return e
     }
     S.extend({
         htmlPrefilter: function(e) {
             return e
         },
         clone: function(e, t, n) {
             var r, i, o, a, s, u, l, c = e.cloneNode(!0),
                 f = ie(e);
             if (!(y.noCloneChecked || 1 !== e.nodeType && 11 !== e.nodeType || S.isXMLDoc(e)))
                 for (a = ve(c), r = 0, i = (o = ve(e)).length; r < i; r++) s = o[r], u = a[r], void 0, "input" === (l = u.nodeName.toLowerCase()) && pe.test(s.type) ? u.checked = s.checked : "input" !== l && "textarea" !== l || (u.defaultValue = s.defaultValue);
             if (t)
                 if (n)
-                    for (o = o || ve(e), a = a || ve(c), r = 0, i = o.length; r < i; r++) Oe(o[r], a[r]);
-                else Oe(e, c);
+                    for (o = o || ve(e), a = a || ve(c), r = 0, i = o.length; r < i; r++) Le(o[r], a[r]);
+                else Le(e, c);
             return 0 < (a = ve(c, "script")).length && ye(a, !f && ve(e, "script")), c
         },
         cleanData: function(e) {
             for (var t, n, r, i = S.event.special, o = 0; void 0 !== (n = e[o]); o++)
                 if (V(n)) {
                     if (t = n[Y.expando]) {
                         if (t.events)
@@ -1859,46 +1857,46 @@
                         n[Y.expando] = void 0
                     }
                     n[Q.expando] && (n[Q.expando] = void 0)
                 }
         }
     }), S.fn.extend({
         detach: function(e) {
-            return Re(this, e, !0)
+            return Oe(this, e, !0)
         },
         remove: function(e) {
-            return Re(this, e)
+            return Oe(this, e)
         },
         text: function(e) {
             return $(this, function(e) {
                 return void 0 === e ? S.text(this) : this.empty().each(function() {
                     1 !== this.nodeType && 11 !== this.nodeType && 9 !== this.nodeType || (this.textContent = e)
                 })
             }, null, e, arguments.length)
         },
         append: function() {
-            return Pe(this, arguments, function(e) {
-                1 !== this.nodeType && 11 !== this.nodeType && 9 !== this.nodeType || qe(this, e).appendChild(e)
+            return He(this, arguments, function(e) {
+                1 !== this.nodeType && 11 !== this.nodeType && 9 !== this.nodeType || je(this, e).appendChild(e)
             })
         },
         prepend: function() {
-            return Pe(this, arguments, function(e) {
+            return He(this, arguments, function(e) {
                 if (1 === this.nodeType || 11 === this.nodeType || 9 === this.nodeType) {
-                    var t = qe(this, e);
+                    var t = je(this, e);
                     t.insertBefore(e, t.firstChild)
                 }
             })
         },
         before: function() {
-            return Pe(this, arguments, function(e) {
+            return He(this, arguments, function(e) {
                 this.parentNode && this.parentNode.insertBefore(e, this)
             })
         },
         after: function() {
-            return Pe(this, arguments, function(e) {
+            return He(this, arguments, function(e) {
                 this.parentNode && this.parentNode.insertBefore(e, this.nextSibling)
             })
         },
         empty: function() {
             for (var e, t = 0; null != (e = this[t]); t++) 1 === e.nodeType && (S.cleanData(ve(e, !1)), e.textContent = "");
             return this
         },
@@ -1909,27 +1907,27 @@
         },
         html: function(e) {
             return $(this, function(e) {
                 var t = this[0] || {},
                     n = 0,
                     r = this.length;
                 if (void 0 === e && 1 === t.nodeType) return t.innerHTML;
-                if ("string" == typeof e && !Ne.test(e) && !ge[(de.exec(e) || ["", ""])[1].toLowerCase()]) {
+                if ("string" == typeof e && !ke.test(e) && !ge[(de.exec(e) || ["", ""])[1].toLowerCase()]) {
                     e = S.htmlPrefilter(e);
                     try {
                         for (; n < r; n++) 1 === (t = this[n] || {}).nodeType && (S.cleanData(ve(t, !1)), t.innerHTML = e);
                         t = 0
                     } catch (e) {}
                 }
                 t && this.empty().append(e)
             }, null, e, arguments.length)
         },
         replaceWith: function() {
             var n = [];
-            return Pe(this, arguments, function(e) {
+            return He(this, arguments, function(e) {
                 var t = this.parentNode;
                 S.inArray(this, n) < 0 && (S.cleanData(ve(this)), t && t.replaceChild(e, this))
             }, n)
         }
     }), S.each({
         appendTo: "append",
         prependTo: "prepend",
@@ -1938,33 +1936,33 @@
         replaceAll: "replaceWith"
     }, function(e, a) {
         S.fn[e] = function(e) {
             for (var t, n = [], r = S(e), i = r.length - 1, o = 0; o <= i; o++) t = o === i ? this : this.clone(!0), S(r[o])[a](t), u.apply(n, t.get());
             return this.pushStack(n)
         }
     });
-    var Me = new RegExp("^(" + ee + ")(?!px)[a-z%]+$", "i"),
-        Ie = function(e) {
+    var Pe = new RegExp("^(" + ee + ")(?!px)[a-z%]+$", "i"),
+        Re = function(e) {
             var t = e.ownerDocument.defaultView;
             return t && t.opener || (t = C), t.getComputedStyle(e)
         },
-        We = function(e, t, n) {
+        Me = function(e, t, n) {
             var r, i, o = {};
             for (i in t) o[i] = e.style[i], e.style[i] = t[i];
             for (i in r = n.call(e), t) e.style[i] = o[i];
             return r
         },
-        Fe = new RegExp(ne.join("|"), "i");
+        Ie = new RegExp(ne.join("|"), "i");
 
-    function Be(e, t, n) {
+    function We(e, t, n) {
         var r, i, o, a, s = e.style;
-        return (n = n || Ie(e)) && ("" !== (a = n.getPropertyValue(t) || n[t]) || ie(e) || (a = S.style(e, t)), !y.pixelBoxStyles() && Me.test(a) && Fe.test(t) && (r = s.width, i = s.minWidth, o = s.maxWidth, s.minWidth = s.maxWidth = s.width = a, a = n.width, s.width = r, s.minWidth = i, s.maxWidth = o)), void 0 !== a ? a + "" : a
+        return (n = n || Re(e)) && ("" !== (a = n.getPropertyValue(t) || n[t]) || ie(e) || (a = S.style(e, t)), !y.pixelBoxStyles() && Pe.test(a) && Ie.test(t) && (r = s.width, i = s.minWidth, o = s.maxWidth, s.minWidth = s.maxWidth = s.width = a, a = n.width, s.width = r, s.minWidth = i, s.maxWidth = o)), void 0 !== a ? a + "" : a
     }
 
-    function $e(e, t) {
+    function Fe(e, t) {
         return {
             get: function() {
                 if (!e()) return (this.get = t).apply(this, arguments);
                 delete this.get
             }
         }
     }! function() {
@@ -1995,79 +1993,79 @@
                 return e(), s
             },
             scrollboxSize: function() {
                 return e(), i
             },
             reliableTrDimensions: function() {
                 var e, t, n, r;
-                return null == a && (e = E.createElement("table"), t = E.createElement("tr"), n = E.createElement("div"), e.style.cssText = "position:absolute;left:-11111px", t.style.height = "1px", n.style.height = "9px", re.appendChild(e).appendChild(t).appendChild(n), r = C.getComputedStyle(t), a = 3 < parseInt(r.height), re.removeChild(e)), a
+                return null == a && (e = E.createElement("table"), t = E.createElement("tr"), n = E.createElement("div"), e.style.cssText = "position:absolute;left:-11111px;border-collapse:separate", t.style.cssText = "border:1px solid", t.style.height = "1px", n.style.height = "9px", n.style.display = "block", re.appendChild(e).appendChild(t).appendChild(n), r = C.getComputedStyle(t), a = parseInt(r.height, 10) + parseInt(r.borderTopWidth, 10) + parseInt(r.borderBottomWidth, 10) === t.offsetHeight, re.removeChild(e)), a
             }
         }))
     }();
-    var _e = ["Webkit", "Moz", "ms"],
-        ze = E.createElement("div").style,
-        Ue = {};
-
-    function Xe(e) {
-        var t = S.cssProps[e] || Ue[e];
-        return t || (e in ze ? e : Ue[e] = function(e) {
+    var Be = ["Webkit", "Moz", "ms"],
+        $e = E.createElement("div").style,
+        _e = {};
+
+    function ze(e) {
+        var t = S.cssProps[e] || _e[e];
+        return t || (e in $e ? e : _e[e] = function(e) {
             var t = e[0].toUpperCase() + e.slice(1),
-                n = _e.length;
+                n = Be.length;
             while (n--)
-                if ((e = _e[n] + t) in ze) return e
+                if ((e = Be[n] + t) in $e) return e
         }(e) || e)
     }
-    var Ve = /^(none|table(?!-c[ea]).+)/,
-        Ge = /^--/,
-        Ye = {
+    var Ue = /^(none|table(?!-c[ea]).+)/,
+        Xe = /^--/,
+        Ve = {
             position: "absolute",
             visibility: "hidden",
             display: "block"
         },
-        Qe = {
+        Ge = {
             letterSpacing: "0",
             fontWeight: "400"
         };
 
-    function Je(e, t, n) {
+    function Ye(e, t, n) {
         var r = te.exec(t);
         return r ? Math.max(0, r[2] - (n || 0)) + (r[3] || "px") : t
     }
 
-    function Ke(e, t, n, r, i, o) {
+    function Qe(e, t, n, r, i, o) {
         var a = "width" === t ? 1 : 0,
             s = 0,
             u = 0;
         if (n === (r ? "border" : "content")) return 0;
         for (; a < 4; a += 2) "margin" === n && (u += S.css(e, n + ne[a], !0, i)), r ? ("content" === n && (u -= S.css(e, "padding" + ne[a], !0, i)), "margin" !== n && (u -= S.css(e, "border" + ne[a] + "Width", !0, i))) : (u += S.css(e, "padding" + ne[a], !0, i), "padding" !== n ? u += S.css(e, "border" + ne[a] + "Width", !0, i) : s += S.css(e, "border" + ne[a] + "Width", !0, i));
         return !r && 0 <= o && (u += Math.max(0, Math.ceil(e["offset" + t[0].toUpperCase() + t.slice(1)] - o - u - s - .5)) || 0), u
     }
 
-    function Ze(e, t, n) {
-        var r = Ie(e),
+    function Je(e, t, n) {
+        var r = Re(e),
             i = (!y.boxSizingReliable() || n) && "border-box" === S.css(e, "boxSizing", !1, r),
             o = i,
-            a = Be(e, t, r),
+            a = We(e, t, r),
             s = "offset" + t[0].toUpperCase() + t.slice(1);
-        if (Me.test(a)) {
+        if (Pe.test(a)) {
             if (!n) return a;
             a = "auto"
         }
-        return (!y.boxSizingReliable() && i || !y.reliableTrDimensions() && A(e, "tr") || "auto" === a || !parseFloat(a) && "inline" === S.css(e, "display", !1, r)) && e.getClientRects().length && (i = "border-box" === S.css(e, "boxSizing", !1, r), (o = s in e) && (a = e[s])), (a = parseFloat(a) || 0) + Ke(e, t, n || (i ? "border" : "content"), o, r, a) + "px"
+        return (!y.boxSizingReliable() && i || !y.reliableTrDimensions() && A(e, "tr") || "auto" === a || !parseFloat(a) && "inline" === S.css(e, "display", !1, r)) && e.getClientRects().length && (i = "border-box" === S.css(e, "boxSizing", !1, r), (o = s in e) && (a = e[s])), (a = parseFloat(a) || 0) + Qe(e, t, n || (i ? "border" : "content"), o, r, a) + "px"
     }
 
-    function et(e, t, n, r, i) {
-        return new et.prototype.init(e, t, n, r, i)
+    function Ke(e, t, n, r, i) {
+        return new Ke.prototype.init(e, t, n, r, i)
     }
     S.extend({
         cssHooks: {
             opacity: {
                 get: function(e, t) {
                     if (t) {
-                        var n = Be(e, "opacity");
+                        var n = We(e, "opacity");
                         return "" === n ? "1" : n
                     }
                 }
             }
         },
         cssNumber: {
             animationIterationCount: !0,
@@ -2091,152 +2089,152 @@
             zIndex: !0,
             zoom: !0
         },
         cssProps: {},
         style: function(e, t, n, r) {
             if (e && 3 !== e.nodeType && 8 !== e.nodeType && e.style) {
                 var i, o, a, s = X(t),
-                    u = Ge.test(t),
+                    u = Xe.test(t),
                     l = e.style;
-                if (u || (t = Xe(s)), a = S.cssHooks[t] || S.cssHooks[s], void 0 === n) return a && "get" in a && void 0 !== (i = a.get(e, !1, r)) ? i : l[t];
+                if (u || (t = ze(s)), a = S.cssHooks[t] || S.cssHooks[s], void 0 === n) return a && "get" in a && void 0 !== (i = a.get(e, !1, r)) ? i : l[t];
                 "string" === (o = typeof n) && (i = te.exec(n)) && i[1] && (n = se(e, t, i), o = "number"), null != n && n == n && ("number" !== o || u || (n += i && i[3] || (S.cssNumber[s] ? "" : "px")), y.clearCloneStyle || "" !== n || 0 !== t.indexOf("background") || (l[t] = "inherit"), a && "set" in a && void 0 === (n = a.set(e, n, r)) || (u ? l.setProperty(t, n) : l[t] = n))
             }
         },
         css: function(e, t, n, r) {
             var i, o, a, s = X(t);
-            return Ge.test(t) || (t = Xe(s)), (a = S.cssHooks[t] || S.cssHooks[s]) && "get" in a && (i = a.get(e, !0, n)), void 0 === i && (i = Be(e, t, r)), "normal" === i && t in Qe && (i = Qe[t]), "" === n || n ? (o = parseFloat(i), !0 === n || isFinite(o) ? o || 0 : i) : i
+            return Xe.test(t) || (t = ze(s)), (a = S.cssHooks[t] || S.cssHooks[s]) && "get" in a && (i = a.get(e, !0, n)), void 0 === i && (i = We(e, t, r)), "normal" === i && t in Ge && (i = Ge[t]), "" === n || n ? (o = parseFloat(i), !0 === n || isFinite(o) ? o || 0 : i) : i
         }
     }), S.each(["height", "width"], function(e, u) {
         S.cssHooks[u] = {
             get: function(e, t, n) {
-                if (t) return !Ve.test(S.css(e, "display")) || e.getClientRects().length && e.getBoundingClientRect().width ? Ze(e, u, n) : We(e, Ye, function() {
-                    return Ze(e, u, n)
+                if (t) return !Ue.test(S.css(e, "display")) || e.getClientRects().length && e.getBoundingClientRect().width ? Je(e, u, n) : Me(e, Ve, function() {
+                    return Je(e, u, n)
                 })
             },
             set: function(e, t, n) {
-                var r, i = Ie(e),
+                var r, i = Re(e),
                     o = !y.scrollboxSize() && "absolute" === i.position,
                     a = (o || n) && "border-box" === S.css(e, "boxSizing", !1, i),
-                    s = n ? Ke(e, u, n, a, i) : 0;
-                return a && o && (s -= Math.ceil(e["offset" + u[0].toUpperCase() + u.slice(1)] - parseFloat(i[u]) - Ke(e, u, "border", !1, i) - .5)), s && (r = te.exec(t)) && "px" !== (r[3] || "px") && (e.style[u] = t, t = S.css(e, u)), Je(0, t, s)
+                    s = n ? Qe(e, u, n, a, i) : 0;
+                return a && o && (s -= Math.ceil(e["offset" + u[0].toUpperCase() + u.slice(1)] - parseFloat(i[u]) - Qe(e, u, "border", !1, i) - .5)), s && (r = te.exec(t)) && "px" !== (r[3] || "px") && (e.style[u] = t, t = S.css(e, u)), Ye(0, t, s)
             }
         }
-    }), S.cssHooks.marginLeft = $e(y.reliableMarginLeft, function(e, t) {
-        if (t) return (parseFloat(Be(e, "marginLeft")) || e.getBoundingClientRect().left - We(e, {
+    }), S.cssHooks.marginLeft = Fe(y.reliableMarginLeft, function(e, t) {
+        if (t) return (parseFloat(We(e, "marginLeft")) || e.getBoundingClientRect().left - Me(e, {
             marginLeft: 0
         }, function() {
             return e.getBoundingClientRect().left
         })) + "px"
     }), S.each({
         margin: "",
         padding: "",
         border: "Width"
     }, function(i, o) {
         S.cssHooks[i + o] = {
             expand: function(e) {
                 for (var t = 0, n = {}, r = "string" == typeof e ? e.split(" ") : [e]; t < 4; t++) n[i + ne[t] + o] = r[t] || r[t - 2] || r[0];
                 return n
             }
-        }, "margin" !== i && (S.cssHooks[i + o].set = Je)
+        }, "margin" !== i && (S.cssHooks[i + o].set = Ye)
     }), S.fn.extend({
         css: function(e, t) {
             return $(this, function(e, t, n) {
                 var r, i, o = {},
                     a = 0;
                 if (Array.isArray(t)) {
-                    for (r = Ie(e), i = t.length; a < i; a++) o[t[a]] = S.css(e, t[a], !1, r);
+                    for (r = Re(e), i = t.length; a < i; a++) o[t[a]] = S.css(e, t[a], !1, r);
                     return o
                 }
                 return void 0 !== n ? S.style(e, t, n) : S.css(e, t)
             }, e, t, 1 < arguments.length)
         }
-    }), ((S.Tween = et).prototype = {
-        constructor: et,
+    }), ((S.Tween = Ke).prototype = {
+        constructor: Ke,
         init: function(e, t, n, r, i, o) {
             this.elem = e, this.prop = n, this.easing = i || S.easing._default, this.options = t, this.start = this.now = this.cur(), this.end = r, this.unit = o || (S.cssNumber[n] ? "" : "px")
         },
         cur: function() {
-            var e = et.propHooks[this.prop];
-            return e && e.get ? e.get(this) : et.propHooks._default.get(this)
+            var e = Ke.propHooks[this.prop];
+            return e && e.get ? e.get(this) : Ke.propHooks._default.get(this)
         },
         run: function(e) {
-            var t, n = et.propHooks[this.prop];
-            return this.options.duration ? this.pos = t = S.easing[this.easing](e, this.options.duration * e, 0, 1, this.options.duration) : this.pos = t = e, this.now = (this.end - this.start) * t + this.start, this.options.step && this.options.step.call(this.elem, this.now, this), n && n.set ? n.set(this) : et.propHooks._default.set(this), this
+            var t, n = Ke.propHooks[this.prop];
+            return this.options.duration ? this.pos = t = S.easing[this.easing](e, this.options.duration * e, 0, 1, this.options.duration) : this.pos = t = e, this.now = (this.end - this.start) * t + this.start, this.options.step && this.options.step.call(this.elem, this.now, this), n && n.set ? n.set(this) : Ke.propHooks._default.set(this), this
         }
-    }).init.prototype = et.prototype, (et.propHooks = {
+    }).init.prototype = Ke.prototype, (Ke.propHooks = {
         _default: {
             get: function(e) {
                 var t;
                 return 1 !== e.elem.nodeType || null != e.elem[e.prop] && null == e.elem.style[e.prop] ? e.elem[e.prop] : (t = S.css(e.elem, e.prop, "")) && "auto" !== t ? t : 0
             },
             set: function(e) {
-                S.fx.step[e.prop] ? S.fx.step[e.prop](e) : 1 !== e.elem.nodeType || !S.cssHooks[e.prop] && null == e.elem.style[Xe(e.prop)] ? e.elem[e.prop] = e.now : S.style(e.elem, e.prop, e.now + e.unit)
+                S.fx.step[e.prop] ? S.fx.step[e.prop](e) : 1 !== e.elem.nodeType || !S.cssHooks[e.prop] && null == e.elem.style[ze(e.prop)] ? e.elem[e.prop] = e.now : S.style(e.elem, e.prop, e.now + e.unit)
             }
         }
-    }).scrollTop = et.propHooks.scrollLeft = {
+    }).scrollTop = Ke.propHooks.scrollLeft = {
         set: function(e) {
             e.elem.nodeType && e.elem.parentNode && (e.elem[e.prop] = e.now)
         }
     }, S.easing = {
         linear: function(e) {
             return e
         },
         swing: function(e) {
             return .5 - Math.cos(e * Math.PI) / 2
         },
         _default: "swing"
-    }, S.fx = et.prototype.init, S.fx.step = {};
-    var tt, nt, rt, it, ot = /^(?:toggle|show|hide)$/,
-        at = /queueHooks$/;
+    }, S.fx = Ke.prototype.init, S.fx.step = {};
+    var Ze, et, tt, nt, rt = /^(?:toggle|show|hide)$/,
+        it = /queueHooks$/;
 
-    function st() {
-        nt && (!1 === E.hidden && C.requestAnimationFrame ? C.requestAnimationFrame(st) : C.setTimeout(st, S.fx.interval), S.fx.tick())
+    function ot() {
+        et && (!1 === E.hidden && C.requestAnimationFrame ? C.requestAnimationFrame(ot) : C.setTimeout(ot, S.fx.interval), S.fx.tick())
     }
 
-    function ut() {
+    function at() {
         return C.setTimeout(function() {
-            tt = void 0
-        }), tt = Date.now()
+            Ze = void 0
+        }), Ze = Date.now()
     }
 
-    function lt(e, t) {
+    function st(e, t) {
         var n, r = 0,
             i = {
                 height: e
             };
         for (t = t ? 1 : 0; r < 4; r += 2 - t) i["margin" + (n = ne[r])] = i["padding" + n] = e;
         return t && (i.opacity = i.width = e), i
     }
 
-    function ct(e, t, n) {
-        for (var r, i = (ft.tweeners[t] || []).concat(ft.tweeners["*"]), o = 0, a = i.length; o < a; o++)
+    function ut(e, t, n) {
+        for (var r, i = (lt.tweeners[t] || []).concat(lt.tweeners["*"]), o = 0, a = i.length; o < a; o++)
             if (r = i[o].call(n, t, e)) return r
     }
 
-    function ft(o, e, t) {
+    function lt(o, e, t) {
         var n, a, r = 0,
-            i = ft.prefilters.length,
+            i = lt.prefilters.length,
             s = S.Deferred().always(function() {
                 delete u.elem
             }),
             u = function() {
                 if (a) return !1;
-                for (var e = tt || ut(), t = Math.max(0, l.startTime + l.duration - e), n = 1 - (t / l.duration || 0), r = 0, i = l.tweens.length; r < i; r++) l.tweens[r].run(n);
+                for (var e = Ze || at(), t = Math.max(0, l.startTime + l.duration - e), n = 1 - (t / l.duration || 0), r = 0, i = l.tweens.length; r < i; r++) l.tweens[r].run(n);
                 return s.notifyWith(o, [l, n, t]), n < 1 && i ? t : (i || s.notifyWith(o, [l, 1, 0]), s.resolveWith(o, [l]), !1)
             },
             l = s.promise({
                 elem: o,
                 props: S.extend({}, e),
                 opts: S.extend(!0, {
                     specialEasing: {},
                     easing: S.easing._default
                 }, t),
                 originalProperties: e,
                 originalOptions: t,
-                startTime: tt || ut(),
+                startTime: Ze || at(),
                 duration: t.duration,
                 tweens: [],
                 createTween: function(e, t) {
                     var n = S.Tween(o, l.opts, e, t, l.opts.specialEasing[e] || l.opts.easing);
                     return l.tweens.push(n), n
                 },
                 stop: function(e) {
@@ -2251,31 +2249,31 @@
         for (! function(e, t) {
                 var n, r, i, o, a;
                 for (n in e)
                     if (i = t[r = X(n)], o = e[n], Array.isArray(o) && (i = o[1], o = e[n] = o[0]), n !== r && (e[r] = o, delete e[n]), (a = S.cssHooks[r]) && "expand" in a)
                         for (n in o = a.expand(o), delete e[r], o) n in e || (e[n] = o[n], t[n] = i);
                     else t[r] = i
             }(c, l.opts.specialEasing); r < i; r++)
-            if (n = ft.prefilters[r].call(l, o, c, l.opts)) return m(n.stop) && (S._queueHooks(l.elem, l.opts.queue).stop = n.stop.bind(n)), n;
-        return S.map(c, ct, l), m(l.opts.start) && l.opts.start.call(o, l), l.progress(l.opts.progress).done(l.opts.done, l.opts.complete).fail(l.opts.fail).always(l.opts.always), S.fx.timer(S.extend(u, {
+            if (n = lt.prefilters[r].call(l, o, c, l.opts)) return m(n.stop) && (S._queueHooks(l.elem, l.opts.queue).stop = n.stop.bind(n)), n;
+        return S.map(c, ut, l), m(l.opts.start) && l.opts.start.call(o, l), l.progress(l.opts.progress).done(l.opts.done, l.opts.complete).fail(l.opts.fail).always(l.opts.always), S.fx.timer(S.extend(u, {
             elem: o,
             anim: l,
             queue: l.opts.queue
         })), l
     }
-    S.Animation = S.extend(ft, {
+    S.Animation = S.extend(lt, {
         tweeners: {
             "*": [function(e, t) {
                 var n = this.createTween(e, t);
                 return se(n.elem, e, te.exec(t), n), n
             }]
         },
         tweener: function(e, t) {
             m(e) ? (t = e, e = ["*"]) : e = e.match(P);
-            for (var n, r = 0, i = e.length; r < i; r++) n = e[r], ft.tweeners[n] = ft.tweeners[n] || [], ft.tweeners[n].unshift(t)
+            for (var n, r = 0, i = e.length; r < i; r++) n = e[r], lt.tweeners[n] = lt.tweeners[n] || [], lt.tweeners[n].unshift(t)
         },
         prefilters: [function(e, t, n) {
             var r, i, o, a, s, u, l, c, f = "width" in t || "height" in t,
                 p = this,
                 d = {},
                 h = e.style,
                 g = e.nodeType && ae(e),
@@ -2283,33 +2281,33 @@
             for (r in n.queue || (null == (a = S._queueHooks(e, "fx")).unqueued && (a.unqueued = 0, s = a.empty.fire, a.empty.fire = function() {
                     a.unqueued || s()
                 }), a.unqueued++, p.always(function() {
                     p.always(function() {
                         a.unqueued--, S.queue(e, "fx").length || a.empty.fire()
                     })
                 })), t)
-                if (i = t[r], ot.test(i)) {
+                if (i = t[r], rt.test(i)) {
                     if (delete t[r], o = o || "toggle" === i, i === (g ? "hide" : "show")) {
                         if ("show" !== i || !v || void 0 === v[r]) continue;
                         g = !0
                     }
                     d[r] = v && v[r] || S.style(e, r)
                 } if ((u = !S.isEmptyObject(t)) || !S.isEmptyObject(d))
                 for (r in f && 1 === e.nodeType && (n.overflow = [h.overflow, h.overflowX, h.overflowY], null == (l = v && v.display) && (l = Y.get(e, "display")), "none" === (c = S.css(e, "display")) && (l ? c = l : (le([e], !0), l = e.style.display || l, c = S.css(e, "display"), le([e]))), ("inline" === c || "inline-block" === c && null != l) && "none" === S.css(e, "float") && (u || (p.done(function() {
                         h.display = l
                     }), null == l && (c = h.display, l = "none" === c ? "" : c)), h.display = "inline-block")), n.overflow && (h.overflow = "hidden", p.always(function() {
                         h.overflow = n.overflow[0], h.overflowX = n.overflow[1], h.overflowY = n.overflow[2]
                     })), u = !1, d) u || (v ? "hidden" in v && (g = v.hidden) : v = Y.access(e, "fxshow", {
                     display: l
                 }), o && (v.hidden = !g), g && le([e], !0), p.done(function() {
                     for (r in g || le([e]), Y.remove(e, "fxshow"), d) S.style(e, r, d[r])
-                })), u = ct(g ? v[r] : 0, r, p), r in v || (v[r] = u.start, g && (u.end = u.start, u.start = 0))
+                })), u = ut(g ? v[r] : 0, r, p), r in v || (v[r] = u.start, g && (u.end = u.start, u.start = 0))
         }],
         prefilter: function(e, t) {
-            t ? ft.prefilters.unshift(e) : ft.prefilters.push(e)
+            t ? lt.prefilters.unshift(e) : lt.prefilters.push(e)
         }
     }), S.speed = function(e, t, n) {
         var r = e && "object" == typeof e ? S.extend({}, e) : {
             complete: n || !n && t || m(e) && e,
             duration: e,
             easing: n && t || t && !m(t) && t
         };
@@ -2322,15 +2320,15 @@
                 opacity: t
             }, e, n, r)
         },
         animate: function(t, e, n, r) {
             var i = S.isEmptyObject(t),
                 o = S.speed(e, n, r),
                 a = function() {
-                    var e = ft(this, S.extend({}, t), o);
+                    var e = lt(this, S.extend({}, t), o);
                     (i || Y.get(this, "finish")) && e.stop(!0)
                 };
             return a.finish = a, i || !1 === o.queue ? this.each(a) : this.queue(o.queue, a)
         },
         stop: function(i, e, o) {
             var a = function(e) {
                 var t = e.stop;
@@ -2339,15 +2337,15 @@
             return "string" != typeof i && (o = e, e = i, i = void 0), e && this.queue(i || "fx", []), this.each(function() {
                 var e = !0,
                     t = null != i && i + "queueHooks",
                     n = S.timers,
                     r = Y.get(this);
                 if (t) r[t] && r[t].stop && a(r[t]);
                 else
-                    for (t in r) r[t] && r[t].stop && at.test(t) && a(r[t]);
+                    for (t in r) r[t] && r[t].stop && it.test(t) && a(r[t]);
                 for (t = n.length; t--;) n[t].elem !== this || null != i && n[t].queue !== i || (n[t].anim.stop(o), e = !1, n.splice(t, 1));
                 !e && o || S.dequeue(this, i)
             })
         },
         finish: function(a) {
             return !1 !== a && (a = a || "fx"), this.each(function() {
                 var e, t = Y.get(this),
@@ -2359,20 +2357,20 @@
                 for (e = 0; e < o; e++) n[e] && n[e].finish && n[e].finish.call(this);
                 delete t.finish
             })
         }
     }), S.each(["toggle", "show", "hide"], function(e, r) {
         var i = S.fn[r];
         S.fn[r] = function(e, t, n) {
-            return null == e || "boolean" == typeof e ? i.apply(this, arguments) : this.animate(lt(r, !0), e, t, n)
+            return null == e || "boolean" == typeof e ? i.apply(this, arguments) : this.animate(st(r, !0), e, t, n)
         }
     }), S.each({
-        slideDown: lt("show"),
-        slideUp: lt("hide"),
-        slideToggle: lt("toggle"),
+        slideDown: st("show"),
+        slideUp: st("hide"),
+        slideToggle: st("toggle"),
         fadeIn: {
             opacity: "show"
         },
         fadeOut: {
             opacity: "hide"
         },
         fadeToggle: {
@@ -2381,48 +2379,48 @@
     }, function(e, r) {
         S.fn[e] = function(e, t, n) {
             return this.animate(r, e, t, n)
         }
     }), S.timers = [], S.fx.tick = function() {
         var e, t = 0,
             n = S.timers;
-        for (tt = Date.now(); t < n.length; t++)(e = n[t])() || n[t] !== e || n.splice(t--, 1);
-        n.length || S.fx.stop(), tt = void 0
+        for (Ze = Date.now(); t < n.length; t++)(e = n[t])() || n[t] !== e || n.splice(t--, 1);
+        n.length || S.fx.stop(), Ze = void 0
     }, S.fx.timer = function(e) {
         S.timers.push(e), S.fx.start()
     }, S.fx.interval = 13, S.fx.start = function() {
-        nt || (nt = !0, st())
+        et || (et = !0, ot())
     }, S.fx.stop = function() {
-        nt = null
+        et = null
     }, S.fx.speeds = {
         slow: 600,
         fast: 200,
         _default: 400
     }, S.fn.delay = function(r, e) {
         return r = S.fx && S.fx.speeds[r] || r, e = e || "fx", this.queue(e, function(e, t) {
             var n = C.setTimeout(e, r);
             t.stop = function() {
                 C.clearTimeout(n)
             }
         })
-    }, rt = E.createElement("input"), it = E.createElement("select").appendChild(E.createElement("option")), rt.type = "checkbox", y.checkOn = "" !== rt.value, y.optSelected = it.selected, (rt = E.createElement("input")).value = "t", rt.type = "radio", y.radioValue = "t" === rt.value;
-    var pt, dt = S.expr.attrHandle;
+    }, tt = E.createElement("input"), nt = E.createElement("select").appendChild(E.createElement("option")), tt.type = "checkbox", y.checkOn = "" !== tt.value, y.optSelected = nt.selected, (tt = E.createElement("input")).value = "t", tt.type = "radio", y.radioValue = "t" === tt.value;
+    var ct, ft = S.expr.attrHandle;
     S.fn.extend({
         attr: function(e, t) {
             return $(this, S.attr, e, t, 1 < arguments.length)
         },
         removeAttr: function(e) {
             return this.each(function() {
                 S.removeAttr(this, e)
             })
         }
     }), S.extend({
         attr: function(e, t, n) {
             var r, i, o = e.nodeType;
-            if (3 !== o && 8 !== o && 2 !== o) return "undefined" == typeof e.getAttribute ? S.prop(e, t, n) : (1 === o && S.isXMLDoc(e) || (i = S.attrHooks[t.toLowerCase()] || (S.expr.match.bool.test(t) ? pt : void 0)), void 0 !== n ? null === n ? void S.removeAttr(e, t) : i && "set" in i && void 0 !== (r = i.set(e, n, t)) ? r : (e.setAttribute(t, n + ""), n) : i && "get" in i && null !== (r = i.get(e, t)) ? r : null == (r = S.find.attr(e, t)) ? void 0 : r)
+            if (3 !== o && 8 !== o && 2 !== o) return "undefined" == typeof e.getAttribute ? S.prop(e, t, n) : (1 === o && S.isXMLDoc(e) || (i = S.attrHooks[t.toLowerCase()] || (S.expr.match.bool.test(t) ? ct : void 0)), void 0 !== n ? null === n ? void S.removeAttr(e, t) : i && "set" in i && void 0 !== (r = i.set(e, n, t)) ? r : (e.setAttribute(t, n + ""), n) : i && "get" in i && null !== (r = i.get(e, t)) ? r : null == (r = S.find.attr(e, t)) ? void 0 : r)
         },
         attrHooks: {
             type: {
                 set: function(e, t) {
                     if (!y.radioValue && "radio" === t && A(e, "input")) {
                         var n = e.value;
                         return e.setAttribute("type", t), n && (e.value = n), t
@@ -2432,37 +2430,37 @@
         },
         removeAttr: function(e, t) {
             var n, r = 0,
                 i = t && t.match(P);
             if (i && 1 === e.nodeType)
                 while (n = i[r++]) e.removeAttribute(n)
         }
-    }), pt = {
+    }), ct = {
         set: function(e, t, n) {
             return !1 === t ? S.removeAttr(e, n) : e.setAttribute(n, n), n
         }
     }, S.each(S.expr.match.bool.source.match(/\w+/g), function(e, t) {
-        var a = dt[t] || S.find.attr;
-        dt[t] = function(e, t, n) {
+        var a = ft[t] || S.find.attr;
+        ft[t] = function(e, t, n) {
             var r, i, o = t.toLowerCase();
-            return n || (i = dt[o], dt[o] = r, r = null != a(e, t, n) ? o : null, dt[o] = i), r
+            return n || (i = ft[o], ft[o] = r, r = null != a(e, t, n) ? o : null, ft[o] = i), r
         }
     });
-    var ht = /^(?:input|select|textarea|button)$/i,
-        gt = /^(?:a|area)$/i;
+    var pt = /^(?:input|select|textarea|button)$/i,
+        dt = /^(?:a|area)$/i;
 
-    function vt(e) {
+    function ht(e) {
         return (e.match(P) || []).join(" ")
     }
 
-    function yt(e) {
+    function gt(e) {
         return e.getAttribute && e.getAttribute("class") || ""
     }
 
-    function mt(e) {
+    function vt(e) {
         return Array.isArray(e) ? e : "string" == typeof e && e.match(P) || []
     }
     S.fn.extend({
         prop: function(e, t) {
             return $(this, S.prop, e, t, 1 < arguments.length)
         },
         removeProp: function(e) {
@@ -2475,15 +2473,15 @@
             var r, i, o = e.nodeType;
             if (3 !== o && 8 !== o && 2 !== o) return 1 === o && S.isXMLDoc(e) || (t = S.propFix[t] || t, i = S.propHooks[t]), void 0 !== n ? i && "set" in i && void 0 !== (r = i.set(e, n, t)) ? r : e[t] = n : i && "get" in i && null !== (r = i.get(e, t)) ? r : e[t]
         },
         propHooks: {
             tabIndex: {
                 get: function(e) {
                     var t = S.find.attr(e, "tabindex");
-                    return t ? parseInt(t, 10) : ht.test(e.nodeName) || gt.test(e.nodeName) && e.href ? 0 : -1
+                    return t ? parseInt(t, 10) : pt.test(e.nodeName) || dt.test(e.nodeName) && e.href ? 0 : -1
                 }
             }
         },
         propFix: {
             "for": "htmlFor",
             "class": "className"
         }
@@ -2498,77 +2496,77 @@
         }
     }), S.each(["tabIndex", "readOnly", "maxLength", "cellSpacing", "cellPadding", "rowSpan", "colSpan", "useMap", "frameBorder", "contentEditable"], function() {
         S.propFix[this.toLowerCase()] = this
     }), S.fn.extend({
         addClass: function(t) {
             var e, n, r, i, o, a, s, u = 0;
             if (m(t)) return this.each(function(e) {
-                S(this).addClass(t.call(this, e, yt(this)))
+                S(this).addClass(t.call(this, e, gt(this)))
             });
-            if ((e = mt(t)).length)
+            if ((e = vt(t)).length)
                 while (n = this[u++])
-                    if (i = yt(n), r = 1 === n.nodeType && " " + vt(i) + " ") {
+                    if (i = gt(n), r = 1 === n.nodeType && " " + ht(i) + " ") {
                         a = 0;
                         while (o = e[a++]) r.indexOf(" " + o + " ") < 0 && (r += o + " ");
-                        i !== (s = vt(r)) && n.setAttribute("class", s)
+                        i !== (s = ht(r)) && n.setAttribute("class", s)
                     } return this
         },
         removeClass: function(t) {
             var e, n, r, i, o, a, s, u = 0;
             if (m(t)) return this.each(function(e) {
-                S(this).removeClass(t.call(this, e, yt(this)))
+                S(this).removeClass(t.call(this, e, gt(this)))
             });
             if (!arguments.length) return this.attr("class", "");
-            if ((e = mt(t)).length)
+            if ((e = vt(t)).length)
                 while (n = this[u++])
-                    if (i = yt(n), r = 1 === n.nodeType && " " + vt(i) + " ") {
+                    if (i = gt(n), r = 1 === n.nodeType && " " + ht(i) + " ") {
                         a = 0;
                         while (o = e[a++])
                             while (-1 < r.indexOf(" " + o + " ")) r = r.replace(" " + o + " ", " ");
-                        i !== (s = vt(r)) && n.setAttribute("class", s)
+                        i !== (s = ht(r)) && n.setAttribute("class", s)
                     } return this
         },
         toggleClass: function(i, t) {
             var o = typeof i,
                 a = "string" === o || Array.isArray(i);
             return "boolean" == typeof t && a ? t ? this.addClass(i) : this.removeClass(i) : m(i) ? this.each(function(e) {
-                S(this).toggleClass(i.call(this, e, yt(this), t), t)
+                S(this).toggleClass(i.call(this, e, gt(this), t), t)
             }) : this.each(function() {
                 var e, t, n, r;
                 if (a) {
-                    t = 0, n = S(this), r = mt(i);
+                    t = 0, n = S(this), r = vt(i);
                     while (e = r[t++]) n.hasClass(e) ? n.removeClass(e) : n.addClass(e)
-                } else void 0 !== i && "boolean" !== o || ((e = yt(this)) && Y.set(this, "__className__", e), this.setAttribute && this.setAttribute("class", e || !1 === i ? "" : Y.get(this, "__className__") || ""))
+                } else void 0 !== i && "boolean" !== o || ((e = gt(this)) && Y.set(this, "__className__", e), this.setAttribute && this.setAttribute("class", e || !1 === i ? "" : Y.get(this, "__className__") || ""))
             })
         },
         hasClass: function(e) {
             var t, n, r = 0;
             t = " " + e + " ";
             while (n = this[r++])
-                if (1 === n.nodeType && -1 < (" " + vt(yt(n)) + " ").indexOf(t)) return !0;
+                if (1 === n.nodeType && -1 < (" " + ht(gt(n)) + " ").indexOf(t)) return !0;
             return !1
         }
     });
-    var xt = /\r/g;
+    var yt = /\r/g;
     S.fn.extend({
         val: function(n) {
             var r, e, i, t = this[0];
             return arguments.length ? (i = m(n), this.each(function(e) {
                 var t;
                 1 === this.nodeType && (null == (t = i ? n.call(this, e, S(this).val()) : n) ? t = "" : "number" == typeof t ? t += "" : Array.isArray(t) && (t = S.map(t, function(e) {
                     return null == e ? "" : e + ""
                 })), (r = S.valHooks[this.type] || S.valHooks[this.nodeName.toLowerCase()]) && "set" in r && void 0 !== r.set(this, t, "value") || (this.value = t))
-            })) : t ? (r = S.valHooks[t.type] || S.valHooks[t.nodeName.toLowerCase()]) && "get" in r && void 0 !== (e = r.get(t, "value")) ? e : "string" == typeof(e = t.value) ? e.replace(xt, "") : null == e ? "" : e : void 0
+            })) : t ? (r = S.valHooks[t.type] || S.valHooks[t.nodeName.toLowerCase()]) && "get" in r && void 0 !== (e = r.get(t, "value")) ? e : "string" == typeof(e = t.value) ? e.replace(yt, "") : null == e ? "" : e : void 0
         }
     }), S.extend({
         valHooks: {
             option: {
                 get: function(e) {
                     var t = S.find.attr(e, "value");
-                    return null != t ? t : vt(S.text(e))
+                    return null != t ? t : ht(S.text(e))
                 }
             },
             select: {
                 get: function(e) {
                     var t, n, r, i = e.options,
                         o = e.selectedIndex,
                         a = "select-one" === e.type,
@@ -2594,31 +2592,31 @@
             set: function(e, t) {
                 if (Array.isArray(t)) return e.checked = -1 < S.inArray(S(e).val(), t)
             }
         }, y.checkOn || (S.valHooks[this].get = function(e) {
             return null === e.getAttribute("value") ? "on" : e.value
         })
     }), y.focusin = "onfocusin" in C;
-    var bt = /^(?:focusinfocus|focusoutblur)$/,
-        wt = function(e) {
+    var mt = /^(?:focusinfocus|focusoutblur)$/,
+        xt = function(e) {
             e.stopPropagation()
         };
     S.extend(S.event, {
         trigger: function(e, t, n, r) {
             var i, o, a, s, u, l, c, f, p = [n || E],
                 d = v.call(e, "type") ? e.type : e,
                 h = v.call(e, "namespace") ? e.namespace.split(".") : [];
-            if (o = f = a = n = n || E, 3 !== n.nodeType && 8 !== n.nodeType && !bt.test(d + S.event.triggered) && (-1 < d.indexOf(".") && (d = (h = d.split(".")).shift(), h.sort()), u = d.indexOf(":") < 0 && "on" + d, (e = e[S.expando] ? e : new S.Event(d, "object" == typeof e && e)).isTrigger = r ? 2 : 3, e.namespace = h.join("."), e.rnamespace = e.namespace ? new RegExp("(^|\\.)" + h.join("\\.(?:.*\\.|)") + "(\\.|$)") : null, e.result = void 0, e.target || (e.target = n), t = null == t ? [e] : S.makeArray(t, [e]), c = S.event.special[d] || {}, r || !c.trigger || !1 !== c.trigger.apply(n, t))) {
+            if (o = f = a = n = n || E, 3 !== n.nodeType && 8 !== n.nodeType && !mt.test(d + S.event.triggered) && (-1 < d.indexOf(".") && (d = (h = d.split(".")).shift(), h.sort()), u = d.indexOf(":") < 0 && "on" + d, (e = e[S.expando] ? e : new S.Event(d, "object" == typeof e && e)).isTrigger = r ? 2 : 3, e.namespace = h.join("."), e.rnamespace = e.namespace ? new RegExp("(^|\\.)" + h.join("\\.(?:.*\\.|)") + "(\\.|$)") : null, e.result = void 0, e.target || (e.target = n), t = null == t ? [e] : S.makeArray(t, [e]), c = S.event.special[d] || {}, r || !c.trigger || !1 !== c.trigger.apply(n, t))) {
                 if (!r && !c.noBubble && !x(n)) {
-                    for (s = c.delegateType || d, bt.test(s + d) || (o = o.parentNode); o; o = o.parentNode) p.push(o), a = o;
+                    for (s = c.delegateType || d, mt.test(s + d) || (o = o.parentNode); o; o = o.parentNode) p.push(o), a = o;
                     a === (n.ownerDocument || E) && p.push(a.defaultView || a.parentWindow || C)
                 }
                 i = 0;
                 while ((o = p[i++]) && !e.isPropagationStopped()) f = o, e.type = 1 < i ? s : c.bindType || d, (l = (Y.get(o, "events") || Object.create(null))[e.type] && Y.get(o, "handle")) && l.apply(o, t), (l = u && o[u]) && l.apply && V(o) && (e.result = l.apply(o, t), !1 === e.result && e.preventDefault());
-                return e.type = d, r || e.isDefaultPrevented() || c._default && !1 !== c._default.apply(p.pop(), t) || !V(n) || u && m(n[d]) && !x(n) && ((a = n[u]) && (n[u] = null), S.event.triggered = d, e.isPropagationStopped() && f.addEventListener(d, wt), n[d](), e.isPropagationStopped() && f.removeEventListener(d, wt), S.event.triggered = void 0, a && (n[u] = a)), e.result
+                return e.type = d, r || e.isDefaultPrevented() || c._default && !1 !== c._default.apply(p.pop(), t) || !V(n) || u && m(n[d]) && !x(n) && ((a = n[u]) && (n[u] = null), S.event.triggered = d, e.isPropagationStopped() && f.addEventListener(d, xt), n[d](), e.isPropagationStopped() && f.removeEventListener(d, xt), S.event.triggered = void 0, a && (n[u] = a)), e.result
             }
         },
         simulate: function(e, t, n) {
             var r = S.extend(new S.Event, n, {
                 type: e,
                 isSimulated: !0
             });
@@ -2650,135 +2648,135 @@
             teardown: function() {
                 var e = this.ownerDocument || this.document || this,
                     t = Y.access(e, r) - 1;
                 t ? Y.access(e, r, t) : (e.removeEventListener(n, i, !0), Y.remove(e, r))
             }
         }
     });
-    var Tt = C.location,
-        Ct = {
+    var bt = C.location,
+        wt = {
             guid: Date.now()
         },
-        Et = /\?/;
+        Tt = /\?/;
     S.parseXML = function(e) {
-        var t;
+        var t, n;
         if (!e || "string" != typeof e) return null;
         try {
             t = (new C.DOMParser).parseFromString(e, "text/xml")
-        } catch (e) {
-            t = void 0
-        }
-        return t && !t.getElementsByTagName("parsererror").length || S.error("Invalid XML: " + e), t
+        } catch (e) {}
+        return n = t && t.getElementsByTagName("parsererror")[0], t && !n || S.error("Invalid XML: " + (n ? S.map(n.childNodes, function(e) {
+            return e.textContent
+        }).join("\n") : e)), t
     };
-    var St = /\[\]$/,
-        kt = /\r?\n/g,
-        At = /^(?:submit|button|image|reset|file)$/i,
-        Nt = /^(?:input|select|textarea|keygen)/i;
+    var Ct = /\[\]$/,
+        Et = /\r?\n/g,
+        St = /^(?:submit|button|image|reset|file)$/i,
+        kt = /^(?:input|select|textarea|keygen)/i;
 
-    function Dt(n, e, r, i) {
+    function At(n, e, r, i) {
         var t;
         if (Array.isArray(e)) S.each(e, function(e, t) {
-            r || St.test(n) ? i(n, t) : Dt(n + "[" + ("object" == typeof t && null != t ? e : "") + "]", t, r, i)
+            r || Ct.test(n) ? i(n, t) : At(n + "[" + ("object" == typeof t && null != t ? e : "") + "]", t, r, i)
         });
         else if (r || "object" !== w(e)) i(n, e);
         else
-            for (t in e) Dt(n + "[" + t + "]", e[t], r, i)
+            for (t in e) At(n + "[" + t + "]", e[t], r, i)
     }
     S.param = function(e, t) {
         var n, r = [],
             i = function(e, t) {
                 var n = m(t) ? t() : t;
                 r[r.length] = encodeURIComponent(e) + "=" + encodeURIComponent(null == n ? "" : n)
             };
         if (null == e) return "";
         if (Array.isArray(e) || e.jquery && !S.isPlainObject(e)) S.each(e, function() {
             i(this.name, this.value)
         });
         else
-            for (n in e) Dt(n, e[n], t, i);
+            for (n in e) At(n, e[n], t, i);
         return r.join("&")
     }, S.fn.extend({
         serialize: function() {
             return S.param(this.serializeArray())
         },
         serializeArray: function() {
             return this.map(function() {
                 var e = S.prop(this, "elements");
                 return e ? S.makeArray(e) : this
             }).filter(function() {
                 var e = this.type;
-                return this.name && !S(this).is(":disabled") && Nt.test(this.nodeName) && !At.test(e) && (this.checked || !pe.test(e))
+                return this.name && !S(this).is(":disabled") && kt.test(this.nodeName) && !St.test(e) && (this.checked || !pe.test(e))
             }).map(function(e, t) {
                 var n = S(this).val();
                 return null == n ? null : Array.isArray(n) ? S.map(n, function(e) {
                     return {
                         name: t.name,
-                        value: e.replace(kt, "\r\n")
+                        value: e.replace(Et, "\r\n")
                     }
                 }) : {
                     name: t.name,
-                    value: n.replace(kt, "\r\n")
+                    value: n.replace(Et, "\r\n")
                 }
             }).get()
         }
     });
-    var jt = /%20/g,
-        qt = /#.*$/,
-        Lt = /([?&])_=[^&]*/,
-        Ht = /^(.*?):[ \t]*([^\r\n]*)$/gm,
-        Ot = /^(?:GET|HEAD)$/,
-        Pt = /^\/\//,
-        Rt = {},
-        Mt = {},
-        It = "*/".concat("*"),
-        Wt = E.createElement("a");
+    var Nt = /%20/g,
+        jt = /#.*$/,
+        Dt = /([?&])_=[^&]*/,
+        qt = /^(.*?):[ \t]*([^\r\n]*)$/gm,
+        Lt = /^(?:GET|HEAD)$/,
+        Ht = /^\/\//,
+        Ot = {},
+        Pt = {},
+        Rt = "*/".concat("*"),
+        Mt = E.createElement("a");
 
-    function Ft(o) {
+    function It(o) {
         return function(e, t) {
             "string" != typeof e && (t = e, e = "*");
             var n, r = 0,
                 i = e.toLowerCase().match(P) || [];
             if (m(t))
                 while (n = i[r++]) "+" === n[0] ? (n = n.slice(1) || "*", (o[n] = o[n] || []).unshift(t)) : (o[n] = o[n] || []).push(t)
         }
     }
 
-    function Bt(t, i, o, a) {
+    function Wt(t, i, o, a) {
         var s = {},
-            u = t === Mt;
+            u = t === Pt;
 
         function l(e) {
             var r;
             return s[e] = !0, S.each(t[e] || [], function(e, t) {
                 var n = t(i, o, a);
                 return "string" != typeof n || u || s[n] ? u ? !(r = n) : void 0 : (i.dataTypes.unshift(n), l(n), !1)
             }), r
         }
         return l(i.dataTypes[0]) || !s["*"] && l("*")
     }
 
-    function $t(e, t) {
+    function Ft(e, t) {
         var n, r, i = S.ajaxSettings.flatOptions || {};
         for (n in t) void 0 !== t[n] && ((i[n] ? e : r || (r = {}))[n] = t[n]);
         return r && S.extend(!0, e, r), e
     }
-    Wt.href = Tt.href, S.extend({
+    Mt.href = bt.href, S.extend({
         active: 0,
         lastModified: {},
         etag: {},
         ajaxSettings: {
-            url: Tt.href,
+            url: bt.href,
             type: "GET",
-            isLocal: /^(?:about|app|app-storage|.+-extension|file|res|widget):$/.test(Tt.protocol),
+            isLocal: /^(?:about|app|app-storage|.+-extension|file|res|widget):$/.test(bt.protocol),
             global: !0,
             processData: !0,
             async: !0,
             contentType: "application/x-www-form-urlencoded; charset=UTF-8",
             accepts: {
-                "*": It,
+                "*": Rt,
                 text: "text/plain",
                 html: "text/html",
                 xml: "application/xml, text/xml",
                 json: "application/json, text/javascript"
             },
             contents: {
                 xml: /\bxml\b/,
@@ -2798,18 +2796,18 @@
             },
             flatOptions: {
                 url: !0,
                 context: !0
             }
         },
         ajaxSetup: function(e, t) {
-            return t ? $t($t(e, S.ajaxSettings), t) : $t(S.ajaxSettings, e)
+            return t ? Ft(Ft(e, S.ajaxSettings), t) : Ft(S.ajaxSettings, e)
         },
-        ajaxPrefilter: Ft(Rt),
-        ajaxTransport: Ft(Mt),
+        ajaxPrefilter: It(Ot),
+        ajaxTransport: It(Pt),
         ajax: function(e, t) {
             "object" == typeof e && (t = e, e = void 0), t = t || {};
             var c, f, p, n, d, r, h, g, i, o, v = S.ajaxSetup({}, t),
                 y = v.context || v,
                 m = v.context && (y.nodeType || y.jquery) ? S(y) : S.event,
                 x = S.Deferred(),
                 b = S.Callbacks("once memory"),
@@ -2820,15 +2818,15 @@
                 T = {
                     readyState: 0,
                     getResponseHeader: function(e) {
                         var t;
                         if (h) {
                             if (!n) {
                                 n = {};
-                                while (t = Ht.exec(p)) n[t[1].toLowerCase() + " "] = (n[t[1].toLowerCase() + " "] || []).concat(t[2])
+                                while (t = qt.exec(p)) n[t[1].toLowerCase() + " "] = (n[t[1].toLowerCase() + " "] || []).concat(t[2])
                             }
                             t = n[e.toLowerCase() + " "]
                         }
                         return null == t ? null : t.join(", ")
                     },
                     getAllResponseHeaders: function() {
                         return h ? p : null
@@ -2848,26 +2846,26 @@
                         return this
                     },
                     abort: function(e) {
                         var t = e || u;
                         return c && c.abort(t), l(0, t), this
                     }
                 };
-            if (x.promise(T), v.url = ((e || v.url || Tt.href) + "").replace(Pt, Tt.protocol + "//"), v.type = t.method || t.type || v.method || v.type, v.dataTypes = (v.dataType || "*").toLowerCase().match(P) || [""], null == v.crossDomain) {
+            if (x.promise(T), v.url = ((e || v.url || bt.href) + "").replace(Ht, bt.protocol + "//"), v.type = t.method || t.type || v.method || v.type, v.dataTypes = (v.dataType || "*").toLowerCase().match(P) || [""], null == v.crossDomain) {
                 r = E.createElement("a");
                 try {
-                    r.href = v.url, r.href = r.href, v.crossDomain = Wt.protocol + "//" + Wt.host != r.protocol + "//" + r.host
+                    r.href = v.url, r.href = r.href, v.crossDomain = Mt.protocol + "//" + Mt.host != r.protocol + "//" + r.host
                 } catch (e) {
                     v.crossDomain = !0
                 }
             }
-            if (v.data && v.processData && "string" != typeof v.data && (v.data = S.param(v.data, v.traditional)), Bt(Rt, v, t, T), h) return T;
-            for (i in (g = S.event && v.global) && 0 == S.active++ && S.event.trigger("ajaxStart"), v.type = v.type.toUpperCase(), v.hasContent = !Ot.test(v.type), f = v.url.replace(qt, ""), v.hasContent ? v.data && v.processData && 0 === (v.contentType || "").indexOf("application/x-www-form-urlencoded") && (v.data = v.data.replace(jt, "+")) : (o = v.url.slice(f.length), v.data && (v.processData || "string" == typeof v.data) && (f += (Et.test(f) ? "&" : "?") + v.data, delete v.data), !1 === v.cache && (f = f.replace(Lt, "$1"), o = (Et.test(f) ? "&" : "?") + "_=" + Ct.guid++ + o), v.url = f + o), v.ifModified && (S.lastModified[f] && T.setRequestHeader("If-Modified-Since", S.lastModified[f]), S.etag[f] && T.setRequestHeader("If-None-Match", S.etag[f])), (v.data && v.hasContent && !1 !== v.contentType || t.contentType) && T.setRequestHeader("Content-Type", v.contentType), T.setRequestHeader("Accept", v.dataTypes[0] && v.accepts[v.dataTypes[0]] ? v.accepts[v.dataTypes[0]] + ("*" !== v.dataTypes[0] ? ", " + It + "; q=0.01" : "") : v.accepts["*"]), v.headers) T.setRequestHeader(i, v.headers[i]);
+            if (v.data && v.processData && "string" != typeof v.data && (v.data = S.param(v.data, v.traditional)), Wt(Ot, v, t, T), h) return T;
+            for (i in (g = S.event && v.global) && 0 == S.active++ && S.event.trigger("ajaxStart"), v.type = v.type.toUpperCase(), v.hasContent = !Lt.test(v.type), f = v.url.replace(jt, ""), v.hasContent ? v.data && v.processData && 0 === (v.contentType || "").indexOf("application/x-www-form-urlencoded") && (v.data = v.data.replace(Nt, "+")) : (o = v.url.slice(f.length), v.data && (v.processData || "string" == typeof v.data) && (f += (Tt.test(f) ? "&" : "?") + v.data, delete v.data), !1 === v.cache && (f = f.replace(Dt, "$1"), o = (Tt.test(f) ? "&" : "?") + "_=" + wt.guid++ + o), v.url = f + o), v.ifModified && (S.lastModified[f] && T.setRequestHeader("If-Modified-Since", S.lastModified[f]), S.etag[f] && T.setRequestHeader("If-None-Match", S.etag[f])), (v.data && v.hasContent && !1 !== v.contentType || t.contentType) && T.setRequestHeader("Content-Type", v.contentType), T.setRequestHeader("Accept", v.dataTypes[0] && v.accepts[v.dataTypes[0]] ? v.accepts[v.dataTypes[0]] + ("*" !== v.dataTypes[0] ? ", " + Rt + "; q=0.01" : "") : v.accepts["*"]), v.headers) T.setRequestHeader(i, v.headers[i]);
             if (v.beforeSend && (!1 === v.beforeSend.call(y, T, v) || h)) return T.abort();
-            if (u = "abort", b.add(v.complete), T.done(v.success), T.fail(v.error), c = Bt(Mt, v, t, T)) {
+            if (u = "abort", b.add(v.complete), T.done(v.success), T.fail(v.error), c = Wt(Pt, v, t, T)) {
                 if (T.readyState = 1, g && m.trigger("ajaxSend", [T, v]), h) return T;
                 v.async && 0 < v.timeout && (d = C.setTimeout(function() {
                     T.abort("timeout")
                 }, v.timeout));
                 try {
                     h = !1, c.send(a, l)
                 } catch (e) {
@@ -2895,15 +2893,15 @@
                                 break
                             }
                             a || (a = i)
                         }
                         o = o || a
                     }
                     if (o) return o !== u[0] && u.unshift(o), n[o]
-                }(v, T, n)), !i && -1 < S.inArray("script", v.dataTypes) && (v.converters["text script"] = function() {}), s = function(e, t, n, r) {
+                }(v, T, n)), !i && -1 < S.inArray("script", v.dataTypes) && S.inArray("json", v.dataTypes) < 0 && (v.converters["text script"] = function() {}), s = function(e, t, n, r) {
                     var i, o, a, s, u, l = {},
                         c = e.dataTypes.slice();
                     if (c[1])
                         for (a in e.converters) l[a.toLowerCase()] = e.converters[a];
                     o = c.shift();
                     while (o)
                         if (e.responseFields[o] && (n[e.responseFields[o]] = t), !u && r && e.dataFilter && (t = e.dataFilter(t, e.dataType)), u = o, o = c.shift())
@@ -3001,30 +2999,30 @@
     }, S.expr.pseudos.visible = function(e) {
         return !!(e.offsetWidth || e.offsetHeight || e.getClientRects().length)
     }, S.ajaxSettings.xhr = function() {
         try {
             return new C.XMLHttpRequest
         } catch (e) {}
     };
-    var _t = {
+    var Bt = {
             0: 200,
             1223: 204
         },
-        zt = S.ajaxSettings.xhr();
-    y.cors = !!zt && "withCredentials" in zt, y.ajax = zt = !!zt, S.ajaxTransport(function(i) {
+        $t = S.ajaxSettings.xhr();
+    y.cors = !!$t && "withCredentials" in $t, y.ajax = $t = !!$t, S.ajaxTransport(function(i) {
         var o, a;
-        if (y.cors || zt && !i.crossDomain) return {
+        if (y.cors || $t && !i.crossDomain) return {
             send: function(e, t) {
                 var n, r = i.xhr();
                 if (r.open(i.type, i.url, i.async, i.username, i.password), i.xhrFields)
                     for (n in i.xhrFields) r[n] = i.xhrFields[n];
                 for (n in i.mimeType && r.overrideMimeType && r.overrideMimeType(i.mimeType), i.crossDomain || e["X-Requested-With"] || (e["X-Requested-With"] = "XMLHttpRequest"), e) r.setRequestHeader(n, e[n]);
                 o = function(e) {
                     return function() {
-                        o && (o = a = r.onload = r.onerror = r.onabort = r.ontimeout = r.onreadystatechange = null, "abort" === e ? r.abort() : "error" === e ? "number" != typeof r.status ? t(0, "error") : t(r.status, r.statusText) : t(_t[r.status] || r.status, r.statusText, "text" !== (r.responseType || "text") || "string" != typeof r.responseText ? {
+                        o && (o = a = r.onload = r.onerror = r.onabort = r.ontimeout = r.onreadystatechange = null, "abort" === e ? r.abort() : "error" === e ? "number" != typeof r.status ? t(0, "error") : t(r.status, r.statusText) : t(Bt[r.status] || r.status, r.statusText, "text" !== (r.responseType || "text") || "string" != typeof r.responseText ? {
                             binary: r.response
                         } : {
                             text: r.responseText
                         }, r.getAllResponseHeaders()))
                     }
                 }, r.onload = o(), a = r.onerror = r.ontimeout = o("error"), void 0 !== r.onabort ? r.onabort = a : r.onreadystatechange = function() {
                     4 === r.readyState && C.setTimeout(function() {
@@ -3069,38 +3067,38 @@
                 }), E.head.appendChild(r[0])
             },
             abort: function() {
                 i && i()
             }
         }
     });
-    var Ut, Xt = [],
-        Vt = /(=)\?(?=&|$)|\?\?/;
+    var _t, zt = [],
+        Ut = /(=)\?(?=&|$)|\?\?/;
     S.ajaxSetup({
         jsonp: "callback",
         jsonpCallback: function() {
-            var e = Xt.pop() || S.expando + "_" + Ct.guid++;
+            var e = zt.pop() || S.expando + "_" + wt.guid++;
             return this[e] = !0, e
         }
     }), S.ajaxPrefilter("json jsonp", function(e, t, n) {
-        var r, i, o, a = !1 !== e.jsonp && (Vt.test(e.url) ? "url" : "string" == typeof e.data && 0 === (e.contentType || "").indexOf("application/x-www-form-urlencoded") && Vt.test(e.data) && "data");
-        if (a || "jsonp" === e.dataTypes[0]) return r = e.jsonpCallback = m(e.jsonpCallback) ? e.jsonpCallback() : e.jsonpCallback, a ? e[a] = e[a].replace(Vt, "$1" + r) : !1 !== e.jsonp && (e.url += (Et.test(e.url) ? "&" : "?") + e.jsonp + "=" + r), e.converters["script json"] = function() {
+        var r, i, o, a = !1 !== e.jsonp && (Ut.test(e.url) ? "url" : "string" == typeof e.data && 0 === (e.contentType || "").indexOf("application/x-www-form-urlencoded") && Ut.test(e.data) && "data");
+        if (a || "jsonp" === e.dataTypes[0]) return r = e.jsonpCallback = m(e.jsonpCallback) ? e.jsonpCallback() : e.jsonpCallback, a ? e[a] = e[a].replace(Ut, "$1" + r) : !1 !== e.jsonp && (e.url += (Tt.test(e.url) ? "&" : "?") + e.jsonp + "=" + r), e.converters["script json"] = function() {
             return o || S.error(r + " was not called"), o[0]
         }, e.dataTypes[0] = "json", i = C[r], C[r] = function() {
             o = arguments
         }, n.always(function() {
-            void 0 === i ? S(C).removeProp(r) : C[r] = i, e[r] && (e.jsonpCallback = t.jsonpCallback, Xt.push(r)), o && m(i) && i(o[0]), o = i = void 0
+            void 0 === i ? S(C).removeProp(r) : C[r] = i, e[r] && (e.jsonpCallback = t.jsonpCallback, zt.push(r)), o && m(i) && i(o[0]), o = i = void 0
         }), "script"
-    }), y.createHTMLDocument = ((Ut = E.implementation.createHTMLDocument("").body).innerHTML = "<form></form><form></form>", 2 === Ut.childNodes.length), S.parseHTML = function(e, t, n) {
+    }), y.createHTMLDocument = ((_t = E.implementation.createHTMLDocument("").body).innerHTML = "<form></form><form></form>", 2 === _t.childNodes.length), S.parseHTML = function(e, t, n) {
         return "string" != typeof e ? [] : ("boolean" == typeof t && (n = t, t = !1), t || (y.createHTMLDocument ? ((r = (t = E.implementation.createHTMLDocument("")).createElement("base")).href = E.location.href, t.head.appendChild(r)) : t = E), o = !n && [], (i = N.exec(e)) ? [t.createElement(i[1])] : (i = xe([e], t, o), o && o.length && S(o).remove(), S.merge([], i.childNodes)));
         var r, i, o
     }, S.fn.load = function(e, t, n) {
         var r, i, o, a = this,
             s = e.indexOf(" ");
-        return -1 < s && (r = vt(e.slice(s)), e = e.slice(0, s)), m(t) ? (n = t, t = void 0) : t && "object" == typeof t && (i = "POST"), 0 < a.length && S.ajax({
+        return -1 < s && (r = ht(e.slice(s)), e = e.slice(0, s)), m(t) ? (n = t, t = void 0) : t && "object" == typeof t && (i = "POST"), 0 < a.length && S.ajax({
             url: e,
             type: i || "GET",
             dataType: "html",
             data: t
         }).done(function(e) {
             o = arguments, a.html(r ? S("<div>").append(S.parseHTML(e)).find(r) : e)
         }).always(n && function(e, t) {
@@ -3113,15 +3111,15 @@
             return t === e.elem
         }).length
     }, S.offset = {
         setOffset: function(e, t, n) {
             var r, i, o, a, s, u, l = S.css(e, "position"),
                 c = S(e),
                 f = {};
-            "static" === l && (e.style.position = "relative"), s = c.offset(), o = S.css(e, "top"), u = S.css(e, "left"), ("absolute" === l || "fixed" === l) && -1 < (o + u).indexOf("auto") ? (a = (r = c.position()).top, i = r.left) : (a = parseFloat(o) || 0, i = parseFloat(u) || 0), m(t) && (t = t.call(e, n, S.extend({}, s))), null != t.top && (f.top = t.top - s.top + a), null != t.left && (f.left = t.left - s.left + i), "using" in t ? t.using.call(e, f) : ("number" == typeof f.top && (f.top += "px"), "number" == typeof f.left && (f.left += "px"), c.css(f))
+            "static" === l && (e.style.position = "relative"), s = c.offset(), o = S.css(e, "top"), u = S.css(e, "left"), ("absolute" === l || "fixed" === l) && -1 < (o + u).indexOf("auto") ? (a = (r = c.position()).top, i = r.left) : (a = parseFloat(o) || 0, i = parseFloat(u) || 0), m(t) && (t = t.call(e, n, S.extend({}, s))), null != t.top && (f.top = t.top - s.top + a), null != t.left && (f.left = t.left - s.left + i), "using" in t ? t.using.call(e, f) : c.css(f)
         }
     }, S.fn.extend({
         offset: function(t) {
             if (arguments.length) return void 0 === t ? this : this.each(function(e) {
                 S.offset.setOffset(this, t, e)
             });
             var e, n, r = this[0];
@@ -3168,16 +3166,16 @@
             return $(this, function(e, t, n) {
                 var r;
                 if (x(e) ? r = e : 9 === e.nodeType && (r = e.defaultView), void 0 === n) return r ? r[i] : e[t];
                 r ? r.scrollTo(o ? r.pageXOffset : n, o ? n : r.pageYOffset) : e[t] = n
             }, t, e, arguments.length)
         }
     }), S.each(["top", "left"], function(e, n) {
-        S.cssHooks[n] = $e(y.pixelPosition, function(e, t) {
-            if (t) return t = Be(e, n), Me.test(t) ? S(e).position()[n] + "px" : t
+        S.cssHooks[n] = Fe(y.pixelPosition, function(e, t) {
+            if (t) return t = We(e, n), Pe.test(t) ? S(e).position()[n] + "px" : t
         })
     }), S.each({
         Height: "height",
         Width: "width"
     }, function(a, s) {
         S.each({
             padding: "inner" + a,
@@ -3214,29 +3212,29 @@
             return this.mouseenter(e).mouseleave(t || e)
         }
     }), S.each("blur focus focusin focusout resize scroll click dblclick mousedown mouseup mousemove mouseover mouseout mouseenter mouseleave change select submit keydown keypress keyup contextmenu".split(" "), function(e, n) {
         S.fn[n] = function(e, t) {
             return 0 < arguments.length ? this.on(n, null, e, t) : this.trigger(n)
         }
     });
-    var Gt = /^[\s\uFEFF\xA0]+|[\s\uFEFF\xA0]+$/g;
+    var Xt = /^[\s\uFEFF\xA0]+|[\s\uFEFF\xA0]+$/g;
     S.proxy = function(e, t) {
         var n, r, i;
         if ("string" == typeof t && (n = e[t], t = e, e = n), m(e)) return r = s.call(arguments, 2), (i = function() {
             return e.apply(t || this, r.concat(s.call(arguments)))
         }).guid = e.guid = e.guid || S.guid++, i
     }, S.holdReady = function(e) {
         e ? S.readyWait++ : S.ready(!0)
     }, S.isArray = Array.isArray, S.parseJSON = JSON.parse, S.nodeName = A, S.isFunction = m, S.isWindow = x, S.camelCase = X, S.type = w, S.now = Date.now, S.isNumeric = function(e) {
         var t = S.type(e);
         return ("number" === t || "string" === t) && !isNaN(e - parseFloat(e))
     }, S.trim = function(e) {
-        return null == e ? "" : (e + "").replace(Gt, "")
+        return null == e ? "" : (e + "").replace(Xt, "")
     }, "function" == typeof define && define.amd && define("jquery", [], function() {
         return S
     });
-    var Yt = C.jQuery,
-        Qt = C.$;
+    var Vt = C.jQuery,
+        Gt = C.$;
     return S.noConflict = function(e) {
-        return C.$ === S && (C.$ = Qt), e && C.jQuery === S && (C.jQuery = Yt), S
+        return C.$ === S && (C.$ = Gt), e && C.jQuery === S && (C.jQuery = Vt), S
     }, "undefined" == typeof e && (C.jQuery = C.$ = S), S
 });
```

### Comparing `Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/_static/js/badge_only.js` & `Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/_static/js/badge_only.js`

 * *Files identical despite different names*

### Comparing `Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/_static/js/html5shiv-printshiv.min.js` & `Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/_static/js/html5shiv-printshiv.min.js`

 * *Files identical despite different names*

### Comparing `Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/_static/js/html5shiv.min.js` & `Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/_static/js/html5shiv.min.js`

 * *Files identical despite different names*

### Comparing `Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/_static/js/theme.js` & `Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/_static/js/theme.js`

 * *Files identical despite different names*

### Comparing `Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/_static/pygments.css` & `Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/_static/searchtools.js` & `Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/_static/searchtools.js`

 * *Files 22% similar despite different names*

#### js-beautify {}

```diff
@@ -4,551 +4,574 @@
  *
  * Sphinx JavaScript utilities for the full-text search.
  *
  * :copyright: Copyright 2007-2022 by the Sphinx team, see AUTHORS.
  * :license: BSD, see LICENSE for details.
  *
  */
+"use strict";
 
-if (!Scorer) {
-    /**
-     * Simple result scoring code.
-     */
+/**
+ * Simple result scoring code.
+ */
+if (typeof Scorer === "undefined") {
     var Scorer = {
         // Implement the following function to further tweak the score for each result
-        // The function takes a result array [filename, title, anchor, descr, score]
+        // The function takes a result array [docname, title, anchor, descr, score, filename]
         // and returns the new score.
         /*
-        score: function(result) {
-          return result[4];
+        score: result => {
+          const [docname, title, anchor, descr, score, filename] = result
+          return score
         },
         */
 
         // query matches the full name of an object
         objNameMatch: 11,
         // or matches in the last dotted part of the object name
         objPartialMatch: 6,
         // Additive scores depending on the priority of the object
         objPrio: {
             0: 15, // used to be importantResults
             1: 5, // used to be objectResults
-            2: -5
-        }, // used to be unimportantResults
+            2: -5, // used to be unimportantResults
+        },
         //  Used when the priority is not in the mapping.
         objPrioDefault: 0,
 
         // query found in title
         title: 15,
         partialTitle: 7,
         // query found in terms
         term: 5,
-        partialTerm: 2
+        partialTerm: 2,
     };
 }
 
-if (!splitQuery) {
-    function splitQuery(query) {
-        return query.split(/\s+/);
+const _removeChildren = (element) => {
+    while (element && element.lastChild) element.removeChild(element.lastChild);
+};
+
+/**
+ * See https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions#escaping
+ */
+const _escapeRegExp = (string) =>
+    string.replace(/[.*+\-?^${}()|[\]\\]/g, "\\$&"); // $& means the whole matched string
+
+const _displayItem = (item, searchTerms) => {
+    const docBuilder = DOCUMENTATION_OPTIONS.BUILDER;
+    const docUrlRoot = DOCUMENTATION_OPTIONS.URL_ROOT;
+    const docFileSuffix = DOCUMENTATION_OPTIONS.FILE_SUFFIX;
+    const docLinkSuffix = DOCUMENTATION_OPTIONS.LINK_SUFFIX;
+    const showSearchSummary = DOCUMENTATION_OPTIONS.SHOW_SEARCH_SUMMARY;
+
+    const [docName, title, anchor, descr, score, _filename] = item;
+
+    let listItem = document.createElement("li");
+    let requestUrl;
+    let linkUrl;
+    if (docBuilder === "dirhtml") {
+        // dirhtml builder
+        let dirname = docName + "/";
+        if (dirname.match(/\/index\/$/))
+            dirname = dirname.substring(0, dirname.length - 6);
+        else if (dirname === "index/") dirname = "";
+        requestUrl = docUrlRoot + dirname;
+        linkUrl = requestUrl;
+    } else {
+        // normal html builders
+        requestUrl = docUrlRoot + docName + docFileSuffix;
+        linkUrl = docName + docLinkSuffix;
+    }
+    let linkEl = listItem.appendChild(document.createElement("a"));
+    linkEl.href = linkUrl + anchor;
+    linkEl.dataset.score = score;
+    linkEl.innerHTML = title;
+    if (descr)
+        listItem.appendChild(document.createElement("span")).innerHTML =
+        " (" + descr + ")";
+    else if (showSearchSummary)
+        fetch(requestUrl)
+        .then((responseData) => responseData.text())
+        .then((data) => {
+            if (data)
+                listItem.appendChild(
+                    Search.makeSearchSummary(data, searchTerms)
+                );
+        });
+    Search.output.appendChild(listItem);
+};
+const _finishSearch = (resultCount) => {
+    Search.stopPulse();
+    Search.title.innerText = _("Search Results");
+    if (!resultCount)
+        Search.status.innerText = Documentation.gettext(
+            "Your search did not match any documents. Please make sure that all words are spelled correctly and that you've selected enough categories."
+        );
+    else
+        Search.status.innerText = _(
+            `Search finished, found ${resultCount} page(s) matching the search query.`
+        );
+};
+const _displayNextItem = (
+    results,
+    resultCount,
+    searchTerms
+) => {
+    // results left, load the summary and display it
+    // this is intended to be dynamic (don't sub resultsCount)
+    if (results.length) {
+        _displayItem(results.pop(), searchTerms);
+        setTimeout(
+            () => _displayNextItem(results, resultCount, searchTerms),
+            5
+        );
     }
+    // search finished, update title and status message
+    else _finishSearch(resultCount);
+};
+
+/**
+ * Default splitQuery function. Can be overridden in ``sphinx.search`` with a
+ * custom function per language.
+ *
+ * The regular expression works by splitting the string on consecutive characters
+ * that are not Unicode letters, numbers, underscores, or emoji characters.
+ * This is the same as ``\W+`` in Python, preserving the surrogate pair area.
+ */
+if (typeof splitQuery === "undefined") {
+    var splitQuery = (query) => query
+        .split(/[^\p{Letter}\p{Number}_\p{Emoji_Presentation}]+/gu)
+        .filter(term => term) // remove remaining empty strings
 }
 
 /**
  * Search Module
  */
-var Search = {
-
+const Search = {
     _index: null,
     _queued_query: null,
     _pulse_status: -1,
 
-    htmlToText: function(htmlString) {
-        var virtualDocument = document.implementation.createHTMLDocument('virtual');
-        var htmlElement = $(htmlString, virtualDocument);
-        htmlElement.find('.headerlink').remove();
-        docContent = htmlElement.find('[role=main]')[0];
-        if (docContent === undefined) {
-            console.warn("Content block not found. Sphinx search tries to obtain it " +
-                "via '[role=main]'. Could you check your theme or template.");
-            return "";
-        }
-        return docContent.textContent || docContent.innerText;
+    htmlToText: (htmlString) => {
+        const htmlElement = new DOMParser().parseFromString(htmlString, 'text/html');
+        htmlElement.querySelectorAll(".headerlink").forEach((el) => {
+            el.remove()
+        });
+        const docContent = htmlElement.querySelector('[role="main"]');
+        if (docContent !== undefined) return docContent.textContent;
+        console.warn(
+            "Content block not found. Sphinx search tries to obtain it via '[role=main]'. Could you check your theme or template."
+        );
+        return "";
     },
 
-    init: function() {
-        var params = $.getQueryParameters();
-        if (params.q) {
-            var query = params.q[0];
-            $('input[name="q"]')[0].value = query;
-            this.performSearch(query);
-        }
+    init: () => {
+        const query = new URLSearchParams(window.location.search).get("q");
+        document
+            .querySelectorAll('input[name="q"]')
+            .forEach((el) => (el.value = query));
+        if (query) Search.performSearch(query);
     },
 
-    loadIndex: function(url) {
-        $.ajax({
-            type: "GET",
-            url: url,
-            data: null,
-            dataType: "script",
-            cache: true,
-            complete: function(jqxhr, textstatus) {
-                if (textstatus != "success") {
-                    document.getElementById("searchindexloader").src = url;
-                }
-            }
-        });
-    },
+    loadIndex: (url) =>
+        (document.body.appendChild(document.createElement("script")).src = url),
 
-    setIndex: function(index) {
-        var q;
-        this._index = index;
-        if ((q = this._queued_query) !== null) {
-            this._queued_query = null;
-            Search.query(q);
+    setIndex: (index) => {
+        Search._index = index;
+        if (Search._queued_query !== null) {
+            const query = Search._queued_query;
+            Search._queued_query = null;
+            Search.query(query);
         }
     },
 
-    hasIndex: function() {
-        return this._index !== null;
-    },
+    hasIndex: () => Search._index !== null,
 
-    deferQuery: function(query) {
-        this._queued_query = query;
-    },
+    deferQuery: (query) => (Search._queued_query = query),
 
-    stopPulse: function() {
-        this._pulse_status = 0;
-    },
+    stopPulse: () => (Search._pulse_status = -1),
 
-    startPulse: function() {
-        if (this._pulse_status >= 0)
-            return;
+    startPulse: () => {
+        if (Search._pulse_status >= 0) return;
 
-        function pulse() {
-            var i;
+        const pulse = () => {
             Search._pulse_status = (Search._pulse_status + 1) % 4;
-            var dotString = '';
-            for (i = 0; i < Search._pulse_status; i++)
-                dotString += '.';
-            Search.dots.text(dotString);
-            if (Search._pulse_status > -1)
-                window.setTimeout(pulse, 500);
-        }
+            Search.dots.innerText = ".".repeat(Search._pulse_status);
+            if (Search._pulse_status >= 0) window.setTimeout(pulse, 500);
+        };
         pulse();
     },
 
     /**
      * perform a search for something (or wait until index is loaded)
      */
-    performSearch: function(query) {
+    performSearch: (query) => {
         // create the required interface elements
-        this.out = $('#search-results');
-        this.title = $('<h2>' + _('Searching') + '</h2>').appendTo(this.out);
-        this.dots = $('<span></span>').appendTo(this.title);
-        this.status = $('<p class="search-summary">&nbsp;</p>').appendTo(this.out);
-        this.output = $('<ul class="search"/>').appendTo(this.out);
-
-        $('#search-progress').text(_('Preparing search...'));
-        this.startPulse();
+        const searchText = document.createElement("h2");
+        searchText.textContent = _("Searching");
+        const searchSummary = document.createElement("p");
+        searchSummary.classList.add("search-summary");
+        searchSummary.innerText = "";
+        const searchList = document.createElement("ul");
+        searchList.classList.add("search");
+
+        const out = document.getElementById("search-results");
+        Search.title = out.appendChild(searchText);
+        Search.dots = Search.title.appendChild(document.createElement("span"));
+        Search.status = out.appendChild(searchSummary);
+        Search.output = out.appendChild(searchList);
+
+        const searchProgress = document.getElementById("search-progress");
+        // Some themes don't use the search progress node
+        if (searchProgress) {
+            searchProgress.innerText = _("Preparing search...");
+        }
+        Search.startPulse();
 
         // index already loaded, the browser was quick!
-        if (this.hasIndex())
-            this.query(query);
-        else
-            this.deferQuery(query);
+        if (Search.hasIndex()) Search.query(query);
+        else Search.deferQuery(query);
     },
 
     /**
      * execute search (requires search index to be loaded)
      */
-    query: function(query) {
-        var i;
+    query: (query) => {
+        const filenames = Search._index.filenames;
+        const docNames = Search._index.docnames;
+        const titles = Search._index.titles;
+        const allTitles = Search._index.alltitles;
+        const indexEntries = Search._index.indexentries;
+
+        // stem the search terms and add them to the correct list
+        const stemmer = new Stemmer();
+        const searchTerms = new Set();
+        const excludedTerms = new Set();
+        const highlightTerms = new Set();
+        const objectTerms = new Set(splitQuery(query.toLowerCase().trim()));
+        splitQuery(query.trim()).forEach((queryTerm) => {
+            const queryTermLower = queryTerm.toLowerCase();
 
-        // stem the searchterms and add them to the correct list
-        var stemmer = new Stemmer();
-        var searchterms = [];
-        var excluded = [];
-        var hlterms = [];
-        var tmp = splitQuery(query);
-        var objectterms = [];
-        for (i = 0; i < tmp.length; i++) {
-            if (tmp[i] !== "") {
-                objectterms.push(tmp[i].toLowerCase());
-            }
+            // maybe skip this "word"
+            // stopwords array is from language_data.js
+            if (
+                stopwords.indexOf(queryTermLower) !== -1 ||
+                queryTerm.match(/^\d+$/)
+            )
+                return;
 
-            if ($u.indexOf(stopwords, tmp[i].toLowerCase()) != -1 || tmp[i] === "") {
-                // skip this "word"
-                continue;
-            }
             // stem the word
-            var word = stemmer.stemWord(tmp[i].toLowerCase());
-            // prevent stemmer from cutting word smaller than two chars
-            if (word.length < 3 && tmp[i].length >= 3) {
-                word = tmp[i];
-            }
-            var toAppend;
+            let word = stemmer.stemWord(queryTermLower);
             // select the correct list
-            if (word[0] == '-') {
-                toAppend = excluded;
-                word = word.substr(1);
-            } else {
-                toAppend = searchterms;
-                hlterms.push(tmp[i].toLowerCase());
+            if (word[0] === "-") excludedTerms.add(word.substr(1));
+            else {
+                searchTerms.add(word);
+                highlightTerms.add(queryTermLower);
             }
-            // only add if not already in the list
-            if (!$u.contains(toAppend, word))
-                toAppend.push(word);
-        }
-        var highlightstring = '?highlight=' + $.urlencode(hlterms.join(" "));
+        });
 
-        // console.debug('SEARCH: searching for:');
-        // console.info('required: ', searchterms);
-        // console.info('excluded: ', excluded);
+        if (SPHINX_HIGHLIGHT_ENABLED) { // set in sphinx_highlight.js
+            localStorage.setItem("sphinx_highlight_terms", [...highlightTerms].join(" "))
+        }
 
-        // prepare search
-        var terms = this._index.terms;
-        var titleterms = this._index.titleterms;
+        // console.debug("SEARCH: searching for:");
+        // console.info("required: ", [...searchTerms]);
+        // console.info("excluded: ", [...excludedTerms]);
+
+        // array of [docname, title, anchor, descr, score, filename]
+        let results = [];
+        _removeChildren(document.getElementById("search-progress"));
+
+        const queryLower = query.toLowerCase();
+        for (const [title, foundTitles] of Object.entries(allTitles)) {
+            if (title.toLowerCase().includes(queryLower) && (queryLower.length >= title.length / 2)) {
+                for (const [file, id] of foundTitles) {
+                    let score = Math.round(100 * queryLower.length / title.length)
+                    results.push([
+                        docNames[file],
+                        titles[file] !== title ? `${titles[file]} > ${title}` : title,
+                        id !== null ? "#" + id : "",
+                        null,
+                        score,
+                        filenames[file],
+                    ]);
+                }
+            }
+        }
 
-        // array of [filename, title, anchor, descr, score]
-        var results = [];
-        $('#search-progress').empty();
+        // search for explicit entries in index directives
+        for (const [entry, foundEntries] of Object.entries(indexEntries)) {
+            if (entry.includes(queryLower) && (queryLower.length >= entry.length / 2)) {
+                for (const [file, id] of foundEntries) {
+                    let score = Math.round(100 * queryLower.length / entry.length)
+                    results.push([
+                        docNames[file],
+                        titles[file],
+                        id ? "#" + id : "",
+                        null,
+                        score,
+                        filenames[file],
+                    ]);
+                }
+            }
+        }
 
         // lookup as object
-        for (i = 0; i < objectterms.length; i++) {
-            var others = [].concat(objectterms.slice(0, i),
-                objectterms.slice(i + 1, objectterms.length));
-            results = results.concat(this.performObjectSearch(objectterms[i], others));
-        }
+        objectTerms.forEach((term) =>
+            results.push(...Search.performObjectSearch(term, objectTerms))
+        );
 
         // lookup as search terms in fulltext
-        results = results.concat(this.performTermsSearch(searchterms, excluded, terms, titleterms));
+        results.push(...Search.performTermsSearch(searchTerms, excludedTerms));
 
         // let the scorer override scores with a custom scoring function
-        if (Scorer.score) {
-            for (i = 0; i < results.length; i++)
-                results[i][4] = Scorer.score(results[i]);
-        }
+        if (Scorer.score) results.forEach((item) => (item[4] = Scorer.score(item)));
 
         // now sort the results by score (in opposite order of appearance, since the
         // display function below uses pop() to retrieve items) and then
         // alphabetically
-        results.sort(function(a, b) {
-            var left = a[4];
-            var right = b[4];
-            if (left > right) {
-                return 1;
-            } else if (left < right) {
-                return -1;
-            } else {
+        results.sort((a, b) => {
+            const leftScore = a[4];
+            const rightScore = b[4];
+            if (leftScore === rightScore) {
                 // same score: sort alphabetically
-                left = a[1].toLowerCase();
-                right = b[1].toLowerCase();
-                return (left > right) ? -1 : ((left < right) ? 1 : 0);
+                const leftTitle = a[1].toLowerCase();
+                const rightTitle = b[1].toLowerCase();
+                if (leftTitle === rightTitle) return 0;
+                return leftTitle > rightTitle ? -1 : 1; // inverted is intentional
             }
+            return leftScore > rightScore ? 1 : -1;
         });
 
+        // remove duplicate search results
+        // note the reversing of results, so that in the case of duplicates, the highest-scoring entry is kept
+        let seen = new Set();
+        results = results.reverse().reduce((acc, result) => {
+            let resultStr = result.slice(0, 4).concat([result[5]]).map(v => String(v)).join(',');
+            if (!seen.has(resultStr)) {
+                acc.push(result);
+                seen.add(resultStr);
+            }
+            return acc;
+        }, []);
+
+        results = results.reverse();
+
         // for debugging
         //Search.lastresults = results.slice();  // a copy
-        //console.info('search results:', Search.lastresults);
+        // console.info("search results:", Search.lastresults);
 
         // print the results
-        var resultCount = results.length;
-
-        function displayNextItem() {
-            // results left, load the summary and display it
-            if (results.length) {
-                var item = results.pop();
-                var listItem = $('<li></li>');
-                var requestUrl = "";
-                var linkUrl = "";
-                if (DOCUMENTATION_OPTIONS.BUILDER === 'dirhtml') {
-                    // dirhtml builder
-                    var dirname = item[0] + '/';
-                    if (dirname.match(/\/index\/$/)) {
-                        dirname = dirname.substring(0, dirname.length - 6);
-                    } else if (dirname == 'index/') {
-                        dirname = '';
-                    }
-                    requestUrl = DOCUMENTATION_OPTIONS.URL_ROOT + dirname;
-                    linkUrl = requestUrl;
-
-                } else {
-                    // normal html builders
-                    requestUrl = DOCUMENTATION_OPTIONS.URL_ROOT + item[0] + DOCUMENTATION_OPTIONS.FILE_SUFFIX;
-                    linkUrl = item[0] + DOCUMENTATION_OPTIONS.LINK_SUFFIX;
-                }
-                listItem.append($('<a/>').attr('href',
-                    linkUrl +
-                    highlightstring + item[2]).html(item[1]));
-                if (item[3]) {
-                    listItem.append($('<span> (' + item[3] + ')</span>'));
-                    Search.output.append(listItem);
-                    setTimeout(function() {
-                        displayNextItem();
-                    }, 5);
-                } else if (DOCUMENTATION_OPTIONS.HAS_SOURCE) {
-                    $.ajax({
-                        url: requestUrl,
-                        dataType: "text",
-                        complete: function(jqxhr, textstatus) {
-                            var data = jqxhr.responseText;
-                            if (data !== '' && data !== undefined) {
-                                var summary = Search.makeSearchSummary(data, searchterms, hlterms);
-                                if (summary) {
-                                    listItem.append(summary);
-                                }
-                            }
-                            Search.output.append(listItem);
-                            setTimeout(function() {
-                                displayNextItem();
-                            }, 5);
-                        }
-                    });
-                } else {
-                    // no source available, just display title
-                    Search.output.append(listItem);
-                    setTimeout(function() {
-                        displayNextItem();
-                    }, 5);
-                }
-            }
-            // search finished, update title and status message
-            else {
-                Search.stopPulse();
-                Search.title.text(_('Search Results'));
-                if (!resultCount)
-                    Search.status.text(_('Your search did not match any documents. Please make sure that all words are spelled correctly and that you\'ve selected enough categories.'));
-                else
-                    Search.status.text(_('Search finished, found %s page(s) matching the search query.').replace('%s', resultCount));
-                Search.status.fadeIn(500);
-            }
-        }
-        displayNextItem();
+        _displayNextItem(results, results.length, searchTerms);
     },
 
     /**
      * search for object names
      */
-    performObjectSearch: function(object, otherterms) {
-        var filenames = this._index.filenames;
-        var docnames = this._index.docnames;
-        var objects = this._index.objects;
-        var objnames = this._index.objnames;
-        var titles = this._index.titles;
-
-        var i;
-        var results = [];
-
-        for (var prefix in objects) {
-            for (var iMatch = 0; iMatch != objects[prefix].length; ++iMatch) {
-                var match = objects[prefix][iMatch];
-                var name = match[4];
-                var fullname = (prefix ? prefix + '.' : '') + name;
-                var fullnameLower = fullname.toLowerCase()
-                if (fullnameLower.indexOf(object) > -1) {
-                    var score = 0;
-                    var parts = fullnameLower.split('.');
-                    // check for different match types: exact matches of full name or
-                    // "last name" (i.e. last dotted part)
-                    if (fullnameLower == object || parts[parts.length - 1] == object) {
-                        score += Scorer.objNameMatch;
-                        // matches in last name
-                    } else if (parts[parts.length - 1].indexOf(object) > -1) {
-                        score += Scorer.objPartialMatch;
-                    }
-                    var objname = objnames[match[1]][2];
-                    var title = titles[match[0]];
-                    // If more than one term searched for, we require other words to be
-                    // found in the name/title/description
-                    if (otherterms.length > 0) {
-                        var haystack = (prefix + ' ' + name + ' ' +
-                            objname + ' ' + title).toLowerCase();
-                        var allfound = true;
-                        for (i = 0; i < otherterms.length; i++) {
-                            if (haystack.indexOf(otherterms[i]) == -1) {
-                                allfound = false;
-                                break;
-                            }
-                        }
-                        if (!allfound) {
-                            continue;
-                        }
-                    }
-                    var descr = objname + _(', in ') + title;
-
-                    var anchor = match[3];
-                    if (anchor === '')
-                        anchor = fullname;
-                    else if (anchor == '-')
-                        anchor = objnames[match[1]][1] + '-' + fullname;
-                    // add custom score for some objects according to scorer
-                    if (Scorer.objPrio.hasOwnProperty(match[2])) {
-                        score += Scorer.objPrio[match[2]];
-                    } else {
-                        score += Scorer.objPrioDefault;
-                    }
-                    results.push([docnames[match[0]], fullname, '#' + anchor, descr, score, filenames[match[0]]]);
-                }
-            }
-        }
-
+    performObjectSearch: (object, objectTerms) => {
+        const filenames = Search._index.filenames;
+        const docNames = Search._index.docnames;
+        const objects = Search._index.objects;
+        const objNames = Search._index.objnames;
+        const titles = Search._index.titles;
+
+        const results = [];
+
+        const objectSearchCallback = (prefix, match) => {
+            const name = match[4]
+            const fullname = (prefix ? prefix + "." : "") + name;
+            const fullnameLower = fullname.toLowerCase();
+            if (fullnameLower.indexOf(object) < 0) return;
+
+            let score = 0;
+            const parts = fullnameLower.split(".");
+
+            // check for different match types: exact matches of full name or
+            // "last name" (i.e. last dotted part)
+            if (fullnameLower === object || parts.slice(-1)[0] === object)
+                score += Scorer.objNameMatch;
+            else if (parts.slice(-1)[0].indexOf(object) > -1)
+                score += Scorer.objPartialMatch; // matches in last name
+
+            const objName = objNames[match[1]][2];
+            const title = titles[match[0]];
+
+            // If more than one term searched for, we require other words to be
+            // found in the name/title/description
+            const otherTerms = new Set(objectTerms);
+            otherTerms.delete(object);
+            if (otherTerms.size > 0) {
+                const haystack = `${prefix} ${name} ${objName} ${title}`.toLowerCase();
+                if (
+                    [...otherTerms].some((otherTerm) => haystack.indexOf(otherTerm) < 0)
+                )
+                    return;
+            }
+
+            let anchor = match[3];
+            if (anchor === "") anchor = fullname;
+            else if (anchor === "-") anchor = objNames[match[1]][1] + "-" + fullname;
+
+            const descr = objName + _(", in ") + title;
+
+            // add custom score for some objects according to scorer
+            if (Scorer.objPrio.hasOwnProperty(match[2]))
+                score += Scorer.objPrio[match[2]];
+            else score += Scorer.objPrioDefault;
+
+            results.push([
+                docNames[match[0]],
+                fullname,
+                "#" + anchor,
+                descr,
+                score,
+                filenames[match[0]],
+            ]);
+        };
+        Object.keys(objects).forEach((prefix) =>
+            objects[prefix].forEach((array) =>
+                objectSearchCallback(prefix, array)
+            )
+        );
         return results;
     },
 
     /**
-     * See https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions
-     */
-    escapeRegExp: function(string) {
-        return string.replace(/[.*+\-?^${}()|[\]\\]/g, '\\$&'); // $& means the whole matched string
-    },
-
-    /**
      * search for full-text terms in the index
      */
-    performTermsSearch: function(searchterms, excluded, terms, titleterms) {
-        var docnames = this._index.docnames;
-        var filenames = this._index.filenames;
-        var titles = this._index.titles;
-
-        var i, j, file;
-        var fileMap = {};
-        var scoreMap = {};
-        var results = [];
+    performTermsSearch: (searchTerms, excludedTerms) => {
+        // prepare search
+        const terms = Search._index.terms;
+        const titleTerms = Search._index.titleterms;
+        const filenames = Search._index.filenames;
+        const docNames = Search._index.docnames;
+        const titles = Search._index.titles;
+
+        const scoreMap = new Map();
+        const fileMap = new Map();
 
         // perform the search on the required terms
-        for (i = 0; i < searchterms.length; i++) {
-            var word = searchterms[i];
-            var files = [];
-            var _o = [{
+        searchTerms.forEach((word) => {
+            const files = [];
+            const arr = [{
                 files: terms[word],
                 score: Scorer.term
             }, {
-                files: titleterms[word],
+                files: titleTerms[word],
                 score: Scorer.title
-            }];
+            }, ];
             // add support for partial matches
             if (word.length > 2) {
-                var word_regex = this.escapeRegExp(word);
-                for (var w in terms) {
-                    if (w.match(word_regex) && !terms[word]) {
-                        _o.push({
-                            files: terms[w],
+                const escapedWord = _escapeRegExp(word);
+                Object.keys(terms).forEach((term) => {
+                    if (term.match(escapedWord) && !terms[word])
+                        arr.push({
+                            files: terms[term],
                             score: Scorer.partialTerm
-                        })
-                    }
-                }
-                for (var w in titleterms) {
-                    if (w.match(word_regex) && !titleterms[word]) {
-                        _o.push({
-                            files: titleterms[w],
+                        });
+                });
+                Object.keys(titleTerms).forEach((term) => {
+                    if (term.match(escapedWord) && !titleTerms[word])
+                        arr.push({
+                            files: titleTerms[word],
                             score: Scorer.partialTitle
-                        })
-                    }
-                }
+                        });
+                });
             }
 
             // no match but word was a required one
-            if ($u.every(_o, function(o) {
-                    return o.files === undefined;
-                })) {
-                break;
-            }
+            if (arr.every((record) => record.files === undefined)) return;
+
             // found search word in contents
-            $u.each(_o, function(o) {
-                var _files = o.files;
-                if (_files === undefined)
-                    return
-
-                if (_files.length === undefined)
-                    _files = [_files];
-                files = files.concat(_files);
-
-                // set score for the word in each file to Scorer.term
-                for (j = 0; j < _files.length; j++) {
-                    file = _files[j];
-                    if (!(file in scoreMap))
-                        scoreMap[file] = {};
-                    scoreMap[file][word] = o.score;
-                }
+            arr.forEach((record) => {
+                if (record.files === undefined) return;
+
+                let recordFiles = record.files;
+                if (recordFiles.length === undefined) recordFiles = [recordFiles];
+                files.push(...recordFiles);
+
+                // set score for the word in each file
+                recordFiles.forEach((file) => {
+                    if (!scoreMap.has(file)) scoreMap.set(file, {});
+                    scoreMap.get(file)[word] = record.score;
+                });
             });
 
             // create the mapping
-            for (j = 0; j < files.length; j++) {
-                file = files[j];
-                if (file in fileMap && fileMap[file].indexOf(word) === -1)
-                    fileMap[file].push(word);
-                else
-                    fileMap[file] = [word];
-            }
-        }
+            files.forEach((file) => {
+                if (fileMap.has(file) && fileMap.get(file).indexOf(word) === -1)
+                    fileMap.get(file).push(word);
+                else fileMap.set(file, [word]);
+            });
+        });
 
         // now check if the files don't contain excluded terms
-        for (file in fileMap) {
-            var valid = true;
-
+        const results = [];
+        for (const [file, wordList] of fileMap) {
             // check if all requirements are matched
-            var filteredTermCount = // as search terms with length < 3 are discarded: ignore
-                searchterms.filter(function(term) {
-                    return term.length > 2
-                }).length
+
+            // as search terms with length < 3 are discarded
+            const filteredTermCount = [...searchTerms].filter(
+                (term) => term.length > 2
+            ).length;
             if (
-                fileMap[file].length != searchterms.length &&
-                fileMap[file].length != filteredTermCount
-            ) continue;
+                wordList.length !== searchTerms.size &&
+                wordList.length !== filteredTermCount
+            )
+                continue;
 
             // ensure that none of the excluded terms is in the search result
-            for (i = 0; i < excluded.length; i++) {
-                if (terms[excluded[i]] == file ||
-                    titleterms[excluded[i]] == file ||
-                    $u.contains(terms[excluded[i]] || [], file) ||
-                    $u.contains(titleterms[excluded[i]] || [], file)) {
-                    valid = false;
-                    break;
-                }
-            }
+            if (
+                [...excludedTerms].some(
+                    (term) =>
+                    terms[term] === file ||
+                    titleTerms[term] === file ||
+                    (terms[term] || []).includes(file) ||
+                    (titleTerms[term] || []).includes(file)
+                )
+            )
+                break;
 
-            // if we have still a valid result we can add it to the result list
-            if (valid) {
-                // select one (max) score for the file.
-                // for better ranking, we should calculate ranking by using words statistics like basic tf-idf...
-                var score = $u.max($u.map(fileMap[file], function(w) {
-                    return scoreMap[file][w]
-                }));
-                results.push([docnames[file], titles[file], '', null, score, filenames[file]]);
-            }
+            // select one (max) score for the file.
+            const score = Math.max(...wordList.map((w) => scoreMap.get(file)[w]));
+            // add result to the result list
+            results.push([
+                docNames[file],
+                titles[file],
+                "",
+                null,
+                score,
+                filenames[file],
+            ]);
         }
         return results;
     },
 
     /**
      * helper function to return a node containing the
      * search summary for a given text. keywords is a list
-     * of stemmed words, hlwords is the list of normal, unstemmed
-     * words. the first one is used to find the occurrence, the
-     * latter for highlighting it.
+     * of stemmed words.
      */
-    makeSearchSummary: function(htmlText, keywords, hlwords) {
-        var text = Search.htmlToText(htmlText);
-        if (text == "") {
-            return null;
-        }
-        var textLower = text.toLowerCase();
-        var start = 0;
-        $.each(keywords, function() {
-            var i = textLower.indexOf(this.toLowerCase());
-            if (i > -1)
-                start = i;
-        });
-        start = Math.max(start - 120, 0);
-        var excerpt = ((start > 0) ? '...' : '') +
-            $.trim(text.substr(start, 240)) +
-            ((start + 240 - text.length) ? '...' : '');
-        var rv = $('<p class="context"></p>').text(excerpt);
-        $.each(hlwords, function() {
-            rv = rv.highlightText(this, 'highlighted');
-        });
-        return rv;
-    }
+    makeSearchSummary: (htmlText, keywords) => {
+        const text = Search.htmlToText(htmlText);
+        if (text === "") return null;
+
+        const textLower = text.toLowerCase();
+        const actualStartPosition = [...keywords]
+            .map((k) => textLower.indexOf(k.toLowerCase()))
+            .filter((i) => i > -1)
+            .slice(-1)[0];
+        const startWithContext = Math.max(actualStartPosition - 120, 0);
+
+        const top = startWithContext === 0 ? "" : "...";
+        const tail = startWithContext + 240 < text.length ? "..." : "";
+
+        let summary = document.createElement("p");
+        summary.classList.add("context");
+        summary.textContent = top + text.substr(startWithContext, 240).trim() + tail;
+
+        return summary;
+    },
 };
 
-$(document).ready(function() {
-    Search.init();
-});
+_ready(Search.init);
```

### Comparing `Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/_static/underscore-1.13.1.js` & `Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/_static/underscore-1.13.1.js`

 * *Files identical despite different names*

### Comparing `Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/_static/underscore.js` & `Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/genindex.html` & `Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/genindex.html`

 * *Files 1% similar despite different names*

```diff
@@ -41,16 +41,16 @@
           <a href="index.html">Orange3 World Happiness</a>
       </nav>
 
       <div class="wy-nav-content">
         <div class="rst-content">
           <div role="navigation" aria-label="Page navigation">
   <ul class="wy-breadcrumbs">
-      <li><a href="index.html" class="icon icon-home"></a> &raquo;</li>
-      <li>Index</li>
+      <li><a href="index.html" class="icon icon-home"></a></li>
+      <li class="breadcrumb-item active">Index</li>
       <li class="wy-breadcrumbs-aside">
       </li>
   </ul>
   <hr/>
 </div>
           <div role="main" class="document" itemscope="itemscope" itemtype="http://schema.org/Article">
            <div itemprop="articleBody">
```

#### html2text {}

```diff
@@ -1,12 +1,11 @@
 _O_r_a_n_g_e_3_ _W_o_r_l_d_ _H_a_p_p_i_n_e_s_s
 [q                   ]
     * _S_o_c_i_o_e_c_o_n_o_m_i_c_ _I_n_d_i_c_e_s
 _O_r_a_n_g_e_3_ _W_o_r_l_d_ _H_a_p_p_i_n_e_s_s
-    * »
     * Index
 ===============================================================================
 ************ IInnddeexx ************
 ===============================================================================
 © Copyright 2022, Laboratory of Bioinformatics, Faculty of Computer Science,
 University of Ljubljana.
 Built with _S_p_h_i_n_x using a _t_h_e_m_e provided by _R_e_a_d_ _t_h_e_ _D_o_c_s.
```

### Comparing `Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/index.html` & `Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -42,16 +42,16 @@
           <a href="#">Orange3 World Happiness</a>
       </nav>
 
       <div class="wy-nav-content">
         <div class="rst-content">
           <div role="navigation" aria-label="Page navigation">
   <ul class="wy-breadcrumbs">
-      <li><a href="#" class="icon icon-home"></a> &raquo;</li>
-      <li>Welcome to Orange3 World Happiness documentation!</li>
+      <li><a href="#" class="icon icon-home"></a></li>
+      <li class="breadcrumb-item active">Welcome to Orange3 World Happiness documentation!</li>
       <li class="wy-breadcrumbs-aside">
             <a href="_sources/index.rst.txt" rel="nofollow"> View page source</a>
       </li>
   </ul>
   <hr/>
 </div>
           <div role="main" class="document" itemscope="itemscope" itemtype="http://schema.org/Article">
```

#### html2text {}

```diff
@@ -1,12 +1,11 @@
 _O_r_a_n_g_e_3_ _W_o_r_l_d_ _H_a_p_p_i_n_e_s_s
 [q                   ]
     * _S_o_c_i_o_e_c_o_n_o_m_i_c_ _I_n_d_i_c_e_s
 _O_r_a_n_g_e_3_ _W_o_r_l_d_ _H_a_p_p_i_n_e_s_s
-    * »
     * Welcome to Orange3 World Happiness documentation!
     * _V_i_e_w_ _p_a_g_e_ _s_o_u_r_c_e
 ===============================================================================
 ************ WWeellccoommee ttoo OOrraannggee33 WWoorrlldd HHaappppiinneessss ddooccuummeennttaattiioonn!! ************
 ********** WWiiddggeettss **********
     * _S_o_c_i_o_e_c_o_n_o_m_i_c_ _I_n_d_i_c_e_s
 ************ IInnddiicceess aanndd ttaabblleess ************
```

### Comparing `Orange3-WorldHappiness-0.1.8/doc/_build/htmlhelp/widgets/socioeconomicindices.html` & `Orange3-WorldHappiness-0.1.9/doc/_build/htmlhelp/widgets/socioeconomicindices.html`

 * *Files 1% similar despite different names*

```diff
@@ -42,16 +42,16 @@
           <a href="../index.html">Orange3 World Happiness</a>
       </nav>
 
       <div class="wy-nav-content">
         <div class="rst-content">
           <div role="navigation" aria-label="Page navigation">
   <ul class="wy-breadcrumbs">
-      <li><a href="../index.html" class="icon icon-home"></a> &raquo;</li>
-      <li>Socioeconomic Indices</li>
+      <li><a href="../index.html" class="icon icon-home"></a></li>
+      <li class="breadcrumb-item active">Socioeconomic Indices</li>
       <li class="wy-breadcrumbs-aside">
             <a href="../_sources/widgets/socioeconomicindices.md.txt" rel="nofollow"> View page source</a>
       </li>
   </ul>
   <hr/>
 </div>
           <div role="main" class="document" itemscope="itemscope" itemtype="http://schema.org/Article">
```

#### html2text {}

```diff
@@ -1,12 +1,11 @@
 _O_r_a_n_g_e_3_ _W_o_r_l_d_ _H_a_p_p_i_n_e_s_s
 [q                   ]
     * _S_o_c_i_o_e_c_o_n_o_m_i_c_ _I_n_d_i_c_e_s
 _O_r_a_n_g_e_3_ _W_o_r_l_d_ _H_a_p_p_i_n_e_s_s
-    * »
     * Socioeconomic Indices
     * _V_i_e_w_ _p_a_g_e_ _s_o_u_r_c_e
 ===============================================================================
 ************ SSoocciiooeeccoonnoommiicc IInnddiicceess ************
 Downloads socioeconomic data from remote Mongo database.
 OOuuttppuuttss:
     * Data: Dataset containing filtered selected socioeconomic data.
```

### Comparing `Orange3-WorldHappiness-0.1.8/doc/conf.py` & `Orange3-WorldHappiness-0.1.9/doc/conf.py`

 * *Files identical despite different names*

### Comparing `Orange3-WorldHappiness-0.1.8/doc/make.bat` & `Orange3-WorldHappiness-0.1.9/doc/make.bat`

 * *Files identical despite different names*

### Comparing `Orange3-WorldHappiness-0.1.8/doc/widgets/images/socioeconomic-indices.png` & `Orange3-WorldHappiness-0.1.9/doc/widgets/images/socioeconomic-indices.png`

 * *Files identical despite different names*

### Comparing `Orange3-WorldHappiness-0.1.8/doc/widgets/socioeconomicindices.md` & `Orange3-WorldHappiness-0.1.9/doc/widgets/socioeconomicindices.md`

 * *Files identical despite different names*

### Comparing `Orange3-WorldHappiness-0.1.8/orangecontrib/worldhappiness/whstudy/__init__.py` & `Orange3-WorldHappiness-0.1.9/orangecontrib/worldhappiness/whstudy/__init__.py`

 * *Files identical despite different names*

### Comparing `Orange3-WorldHappiness-0.1.8/orangecontrib/worldhappiness/whstudy/world_data_api.py` & `Orange3-WorldHappiness-0.1.9/orangecontrib/worldhappiness/whstudy/world_data_api.py`

 * *Files identical despite different names*

### Comparing `Orange3-WorldHappiness-0.1.8/orangecontrib/worldhappiness/widgets/__init__.py` & `Orange3-WorldHappiness-0.1.9/orangecontrib/worldhappiness/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `Orange3-WorldHappiness-0.1.8/orangecontrib/worldhappiness/widgets/icons/category.svg` & `Orange3-WorldHappiness-0.1.9/orangecontrib/worldhappiness/widgets/icons/category.svg`

 * *Files identical despite different names*

### Comparing `Orange3-WorldHappiness-0.1.8/orangecontrib/worldhappiness/widgets/icons/socioeconomicindices.svg` & `Orange3-WorldHappiness-0.1.9/orangecontrib/worldhappiness/widgets/icons/socioeconomicindices.svg`

 * *Files identical despite different names*

### Comparing `Orange3-WorldHappiness-0.1.8/orangecontrib/worldhappiness/widgets/owwhstudy.py` & `Orange3-WorldHappiness-0.1.9/orangecontrib/worldhappiness/widgets/owwhstudy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-import re
 from typing import Any, Set, Optional
-from functools import partial
 
 from AnyQt.QtCore import Qt, Signal, QSortFilterProxyModel, QItemSelection, QItemSelectionModel, \
-    QTimer, QModelIndex, QMimeData
+    QModelIndex, QMimeData
 from AnyQt.QtWidgets import QLineEdit, \
-    QTableView, QListView, QTreeWidget, QTreeWidgetItem, QAbstractItemView, QCheckBox, QSplitter, QVBoxLayout
-from AnyQt.QtGui import QDrag
+    QTableView, QListView, QTreeWidget, QTreeWidgetItem, QAbstractItemView, QCheckBox, QSplitter, QVBoxLayout, \
+    QApplication
+from AnyQt.QtGui import QDrag, QClipboard
 
 from Orange.widgets.settings import Setting
 from Orange.widgets.utils.concurrent import ConcurrentWidgetMixin, TaskState
 from Orange.widgets.utils.itemmodels import PyTableModel
 from Orange.widgets.utils.listfilter import (
     slices, delslice
 )
+from Orange.widgets.utils.tableview import table_selection_to_mime_data
 from Orange.widgets.widget import OWWidget, Output, Input
 from Orange.widgets import gui
 
 from orangecontrib.worldhappiness.whstudy import *
 
 MONGO_HANDLE = WorldIndicators('main', 'biolab')
 EXP_NAMES = ['Topic', 'General Subject', 'Specific subject', 'Extension', 'Extension', 'Extension']
@@ -195,15 +195,14 @@
         event.accept()
         return True
 
     def keyPressEvent(self, event):
         super().keyPressEvent(event)
         self.keyPressed.emit(event.key())
 
-
 class IndicatorTableModel(PyTableModel):
     """
     A Indicator table item model specialized for Drag and Drop.
     """
     MIME_TYPE = "application/x-Orange-IndicatorTableItemModelData"
 
     def __init__(self, *args, placeholder=None, **kwargs):
@@ -354,15 +353,15 @@
 
     agg_method: int = Setting(AggregationMethods.MEAN)
     indicator_freq: float = Setting(60)
     country_freq: float = Setting(90)
     selected_years: List = Setting([])
     selected_indicators: List = Setting([])
     selected_countries: Set = Setting(set({}))
-    auto_apply: bool = Setting(True)
+    auto_apply: bool = Setting(False)
     splitter_state: bytes = Setting(b'')
 
     class Inputs:
         indicators = Input("Indicators", Table)
 
     class Outputs:
         world_data = Output("World data", Table)
@@ -435,16 +434,16 @@
         self.country_tree.itemChanged.connect(self.country_checked)
         self.country_tree.itemClicked.connect(self.__on_dummy_change)
 
         bbox = gui.vBox(controls_box)
         gui.auto_send(bbox, self, "auto_apply")
 
         splitter = QSplitter(orientation=Qt.Vertical)
-        available_box = gui.widgetBox(splitter, "Available Indicators")
-        selected_box = gui.widgetBox(splitter, "Selected Indicators")
+        self.available_box = gui.widgetBox(splitter, f"Available Indicators")
+        self.selected_box = gui.widgetBox(splitter, f"Selected Indicators")
 
         self.__indicator_filter_line_edit = QLineEdit(placeholderText="Filter ...")
 
         self.__indicator_relative_checkbox = QCheckBox("Relative Only", self)
         self.__indicator_relative_checkbox.setToolTip("Toggle filtering only relative indicators.")
         self.__indicator_relative_checkbox.setChecked(False)
         self.__indicator_relative_checkbox.stateChanged.connect(
@@ -458,45 +457,49 @@
             self.__on_indicator_relative_changed
         )
 
         self.__indicator_and_button = gui.button(box, self, "Any", width=50, callback=self.__on_indicator_filter_changed)
         self.__indicator_and_button.adjustSize()
         self.__indicator_and_button.setToolTip("Toggle filtering indicators that include all words.")
 
-        filters_row = gui.hBox(available_box)
+        filters_row = gui.hBox(self.available_box)
         filters_row.layout().addWidget(self.__indicator_filter_line_edit)
         filters_row.layout().addWidget(self.__indicator_and_button)
         filters_row.layout().addWidget(self.__indicator_relative_checkbox)
         filters_row.layout().addWidget(self.__indicator_sparse_checkbox)
-        available_box.layout().addWidget(filters_row)
+        self.available_box.layout().addWidget(filters_row)
 
         def dropcompleted(action):
             if action == Qt.MoveAction:
                 self.fix_redraw()
                 self.commit.deferred()
 
         self.available_indices_model = IndicatorTableModel()
         self.available_indices_view = IndicatorTableView()
         proxy = IndicatorFilterProxyModel()
         proxy.setFilterKeyColumn(-1)
         proxy.setFilterCaseSensitivity(Qt.CaseSensitivity.CaseInsensitive)
         self.__indicator_filter_line_edit.textChanged.connect(proxy.set_filter_string)
+        self.__indicator_filter_line_edit.textChanged.connect(self.fix_redraw)
         self.available_indices_view.setModel(proxy)
         self.available_indices_view.model().setSourceModel(self.available_indices_model)
         self.available_indices_view.dragDropActionDidComplete.connect(dropcompleted)
-        available_box.layout().addWidget(self.available_indices_view)
+        self.available_indices_view.selectionModel().selectionChanged.connect(self.fix_redraw)
+        self.available_box.layout().addWidget(self.available_indices_view)
 
         self.selected_indices_model = IndicatorTableModel()
         self.selected_indices_view = IndicatorTableView()
         self.selected_indices_view.setModel(self.selected_indices_model)
+        self.selected_indices_view.selectionModel().selectionChanged.connect(self.fix_redraw)
+
         self.selected_indices_model.rowsInserted.connect(self.__on_dummy_change)
         self.selected_indices_model.rowsRemoved.connect(self.__on_dummy_change)
         self.selected_indices_view.dragDropActionDidComplete.connect(dropcompleted)
         self.selected_indices_view.keyPressed.connect(self.__on_indicator_delete)
-        selected_box.layout().addWidget(self.selected_indices_view)
+        self.selected_box.layout().addWidget(self.selected_indices_view)
 
         splitter.setSizes([300, 200])
         splitter.splitterMoved.connect(
             lambda:
             setattr(self, "splitter_state", bytes(splitter.saveState()))
         )
         self.mainArea.layout().addWidget(splitter)
@@ -509,22 +512,35 @@
 
         # Hide all collumns used in hover and etc.
         for i in range(3, self.available_indices_view.model().columnCount()):
             self.available_indices_view.setColumnHidden(i, True)
         for i in range(3, self.selected_indices_view.model().columnCount()):
             self.selected_indices_view.setColumnHidden(i, True)
 
+        self.available_box.setTitle(f'Available Indicators     '
+                                    f'{self.available_indices_view.model().rowCount()} / '
+                                    f'{self.available_indices_model.rowCount()} displayed | '
+                                    f'{int(len(self.available_indices_view.selectedIndexes())/3)} chosen')
+        self.selected_box.setTitle(f'Selected Indicators     '
+                                   f'{self.selected_indices_view.model().rowCount()} displayed | '
+                                   f'{int(len(self.selected_indices_view.selectedIndexes())/3)} chosen')
+
     def initial_indices_update(self):
         used = self.selected_indicators
         self.available_indices_model[:] = [index for index in self.indicator_features
                                            if index not in used]
         self.selected_indices_model[:] = self.selected_indicators
 
         self.selected_years = self.selected_years if len(self.selected_years) > 0 else list(range(10))
         self.fix_redraw()
+
+        # If big querry make sure auto apply is False
+        if len(used) > 50 or len(self.selected_countries) > 10 or len(self.selected_years) > 10:
+            self.auto_apply = False
+
         self.commit.deferred()
 
     def __on_indicator_filter_changed(self):
         model = self.available_indices_view.model()
         model.set_and_filter()
         self.__indicator_and_button.setText("All" if model.and_filter else "Any")
         self._select_indicator_rows()
@@ -569,14 +585,25 @@
 
     def on_done(self, result: Any):
         self.Outputs.world_data.send(result)
 
     def on_partial_result(self, result: Any) -> None:
         pass
 
+    def copy_to_clipboard(self):
+        self.copyRow()
+
+    def copyRow(self):
+        mime_available = table_selection_to_mime_data(self.available_indices_view)
+        mime_selected = table_selection_to_mime_data(self.selected_indices_view)
+        if mime_available.text():
+            QApplication.clipboard().setMimeData(mime_available, QClipboard.Clipboard)
+        elif mime_selected.text():
+            QApplication.clipboard().setMimeData(mime_selected, QClipboard.Clipboard)
+
     @Inputs.indicators
     def set_inputs(self, inputs: Optional[Table]):
         if inputs is not None and inputs.domain is not None:
             input_indicators = []
             for col in inputs.domain:
                 if isinstance(col, ContinuousVariable) and not re.match(r'\d+-.*', col.name):
                     indicator = [ind for ind in self.indicator_features if ind[1] == col.name]
```

### Comparing `Orange3-WorldHappiness-0.1.8/setup.py` & `Orange3-WorldHappiness-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup, find_packages
 
 with io.open('README.pypi', 'r', encoding='utf-8') as f:
     ABOUT = f.read()
 
 NAME = "Orange3-WorldHappiness"
 
-VERSION = "0.1.8"
+VERSION = "0.1.9"
 
 AUTHOR = 'Bioinformatics Laboratory, FRI UL'
 AUTHOR_EMAIL = 'contact@orange.biolab.si'
 
 URL = 'http://orange.biolab.si/download'
 DESCRIPTION = "Orange3 add-on for retrieving socioeconomic data"
 LONG_DESCRIPTION = ABOUT
```

