# Comparing `tmp/censusdis-1.1.7.tar.gz` & `tmp/censusdis-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "censusdis-1.1.7.tar", max compression
+gzip compressed data, was "censusdis-1.1.8.tar", max compression
```

## Comparing `censusdis-1.1.7.tar` & `censusdis-1.1.8.tar`

### file list

```diff
@@ -1,134 +1,134 @@
--rw-r--r--   0        0        0    19938 2023-05-29 16:16:27.244036 censusdis-1.1.7/LICENSE.md
--rw-r--r--   0        0        0     3717 2024-02-27 13:33:21.685281 censusdis-1.1.7/README.md
--rw-r--r--   0        0        0     6148 2023-12-17 16:06:26.749329 censusdis-1.1.7/censusdis/.DS_Store
--rw-r--r--   0        0        0      458 2024-02-15 00:31:57.583171 censusdis-1.1.7/censusdis/__init__.py
--rw-r--r--   0        0        0       92 2023-12-04 23:22:53.481176 censusdis-1.1.7/censusdis/cli/__init__.py
--rw-r--r--   0        0        0     5932 2023-12-05 20:25:11.495292 censusdis-1.1.7/censusdis/cli/cli.py
--rw-r--r--   0        0        0    34433 2024-01-24 14:31:26.141820 censusdis-1.1.7/censusdis/cli/yamlspec.py
--rw-r--r--   0        0        0     1129 2023-12-11 16:55:11.454323 censusdis-1.1.7/censusdis/counties/alabama.py
--rw-r--r--   0        0        0     1013 2023-12-11 16:55:11.455889 censusdis-1.1.7/censusdis/counties/alaska.py
--rw-r--r--   0        0        0      301 2023-12-11 16:55:11.456593 censusdis-1.1.7/censusdis/counties/arizona.py
--rw-r--r--   0        0        0     1261 2023-12-11 16:55:11.459042 censusdis-1.1.7/censusdis/counties/arkansas.py
--rw-r--r--   0        0        0     1029 2023-12-11 16:55:11.460975 censusdis-1.1.7/censusdis/counties/california.py
--rw-r--r--   0        0        0     1091 2023-12-11 16:55:11.463070 censusdis-1.1.7/censusdis/counties/colorado.py
--rw-r--r--   0        0        0     1115 2023-12-11 19:29:35.515569 censusdis-1.1.7/censusdis/counties/connecticut.py
--rw-r--r--   0        0        0      119 2023-12-11 16:55:11.463832 censusdis-1.1.7/censusdis/counties/delaware.py
--rw-r--r--   0        0        0      113 2023-12-11 16:55:11.464049 censusdis-1.1.7/censusdis/counties/district_of_columbia.py
--rw-r--r--   0        0        0     1140 2023-12-11 16:55:11.466050 censusdis-1.1.7/censusdis/counties/florida.py
--rw-r--r--   0        0        0     2539 2023-12-11 16:55:11.470438 censusdis-1.1.7/censusdis/counties/georgia.py
--rw-r--r--   0        0        0      145 2023-12-11 16:55:11.470786 censusdis-1.1.7/censusdis/counties/hawaii.py
--rw-r--r--   0        0        0      756 2023-12-11 16:55:11.472130 censusdis-1.1.7/censusdis/counties/idaho.py
--rw-r--r--   0        0        0     1670 2023-12-11 16:55:11.474786 censusdis-1.1.7/censusdis/counties/illinois.py
--rw-r--r--   0        0        0     1504 2023-12-11 16:55:11.477149 censusdis-1.1.7/censusdis/counties/indiana.py
--rw-r--r--   0        0        0     1627 2023-12-11 16:55:11.479639 censusdis-1.1.7/censusdis/counties/iowa.py
--rw-r--r--   0        0        0     1700 2023-12-11 16:55:11.482454 censusdis-1.1.7/censusdis/counties/kansas.py
--rw-r--r--   0        0        0     1943 2023-12-11 16:55:11.485657 censusdis-1.1.7/censusdis/counties/kentucky.py
--rw-r--r--   0        0        0     1227 2023-12-11 16:55:11.487208 censusdis-1.1.7/censusdis/counties/louisiana.py
--rw-r--r--   0        0        0      340 2023-12-11 16:55:11.487753 censusdis-1.1.7/censusdis/counties/maine.py
--rw-r--r--   0        0        0      492 2023-12-11 16:55:11.488448 censusdis-1.1.7/censusdis/counties/maryland.py
--rw-r--r--   0        0        0      312 2023-12-11 16:55:11.488933 censusdis-1.1.7/censusdis/counties/massachusetts.py
--rw-r--r--   0        0        0     1408 2023-12-11 16:55:11.490783 censusdis-1.1.7/censusdis/counties/michigan.py
--rw-r--r--   0        0        0     1472 2023-12-11 16:55:11.492725 censusdis-1.1.7/censusdis/counties/minnesota.py
--rw-r--r--   0        0        0     1388 2023-12-11 16:55:11.494560 censusdis-1.1.7/censusdis/counties/mississippi.py
--rw-r--r--   0        0        0     1876 2023-12-11 16:55:11.496943 censusdis-1.1.7/censusdis/counties/missouri.py
--rw-r--r--   0        0        0     1012 2023-12-11 16:55:11.498213 censusdis-1.1.7/censusdis/counties/montana.py
--rw-r--r--   0        0        0     1496 2023-12-11 16:55:11.500179 censusdis-1.1.7/censusdis/counties/nebraska.py
--rw-r--r--   0        0        0      339 2023-12-11 16:55:11.500687 censusdis-1.1.7/censusdis/counties/nevada.py
--rw-r--r--   0        0        0      248 2023-12-11 16:55:11.501047 censusdis-1.1.7/censusdis/counties/new_hampshire.py
--rw-r--r--   0        0        0      412 2023-12-11 16:55:11.501613 censusdis-1.1.7/censusdis/counties/new_jersey.py
--rw-r--r--   0        0        0      593 2023-12-11 16:55:11.502420 censusdis-1.1.7/censusdis/counties/new_mexico.py
--rw-r--r--   0        0        0     1083 2023-12-11 16:55:11.503743 censusdis-1.1.7/censusdis/counties/new_york.py
--rw-r--r--   0        0        0     1668 2023-12-11 16:55:11.505932 censusdis-1.1.7/censusdis/counties/north_carolina.py
--rw-r--r--   0        0        0      900 2023-12-11 16:55:11.507102 censusdis-1.1.7/censusdis/counties/north_dakota.py
--rw-r--r--   0        0        0     1446 2023-12-11 16:55:11.508907 censusdis-1.1.7/censusdis/counties/ohio.py
--rw-r--r--   0        0        0     1283 2023-12-11 16:55:11.510477 censusdis-1.1.7/censusdis/counties/oklahoma.py
--rw-r--r--   0        0        0      635 2023-12-11 16:55:11.511295 censusdis-1.1.7/censusdis/counties/oregon.py
--rw-r--r--   0        0        0     1168 2023-12-11 16:55:11.512672 censusdis-1.1.7/censusdis/counties/pennsylvania.py
--rw-r--r--   0        0        0     1381 2023-12-11 16:55:11.532504 censusdis-1.1.7/censusdis/counties/puerto_rico.py
--rw-r--r--   0        0        0      159 2023-12-11 16:55:11.512922 censusdis-1.1.7/censusdis/counties/rhode_island.py
--rw-r--r--   0        0        0      855 2023-12-11 16:55:11.514193 censusdis-1.1.7/censusdis/counties/south_carolina.py
--rw-r--r--   0        0        0     1104 2023-12-11 16:55:11.515784 censusdis-1.1.7/censusdis/counties/south_dakota.py
--rw-r--r--   0        0        0     1568 2023-12-11 16:55:11.517745 censusdis-1.1.7/censusdis/counties/tennessee.py
--rw-r--r--   0        0        0     4049 2023-12-11 16:55:11.522518 censusdis-1.1.7/censusdis/counties/texas.py
--rw-r--r--   0        0        0      506 2023-12-11 16:55:11.523238 censusdis-1.1.7/censusdis/counties/utah.py
--rw-r--r--   0        0        0      308 2023-12-11 16:55:11.523841 censusdis-1.1.7/censusdis/counties/vermont.py
--rw-r--r--   0        0        0     2603 2023-12-11 16:55:11.526648 censusdis-1.1.7/censusdis/counties/virginia.py
--rw-r--r--   0        0        0      705 2023-12-11 16:55:11.527561 censusdis-1.1.7/censusdis/counties/washington.py
--rw-r--r--   0        0        0      938 2023-12-11 16:55:11.528745 censusdis-1.1.7/censusdis/counties/west_virginia.py
--rw-r--r--   0        0        0     1219 2023-12-11 16:55:11.530242 censusdis-1.1.7/censusdis/counties/wisconsin.py
--rw-r--r--   0        0        0      439 2023-12-11 16:55:11.530847 censusdis-1.1.7/censusdis/counties/wyoming.py
--rw-r--r--   0        0        0     7109 2023-12-11 20:36:13.100154 censusdis-1.1.7/censusdis/csa.py
--rw-r--r--   0        0        0    50290 2024-03-23 17:38:35.323344 censusdis-1.1.7/censusdis/data.py
--rw-r--r--   0        0        0    30044 2024-05-21 22:00:31.394482 censusdis-1.1.7/censusdis/datasets.py
--rw-r--r--   0        0        0      332 2023-12-11 20:36:14.332200 censusdis-1.1.7/censusdis/division.py
--rw-r--r--   0        0        0    14425 2024-03-23 17:38:35.323871 censusdis-1.1.7/censusdis/geography.py
--rw-r--r--   0        0        0       98 2023-12-04 23:22:53.473814 censusdis-1.1.7/censusdis/impl/__init__.py
--rw-r--r--   0        0        0      160 2023-12-04 16:32:55.038743 censusdis-1.1.7/censusdis/impl/exceptions.py
--rw-r--r--   0        0        0     7671 2024-03-23 17:38:35.324199 censusdis-1.1.7/censusdis/impl/fetch.py
--rw-r--r--   0        0        0     5096 2024-01-26 21:46:43.129405 censusdis-1.1.7/censusdis/impl/geometry.py
--rw-r--r--   0        0        0    21273 2024-04-29 21:22:19.307664 censusdis-1.1.7/censusdis/impl/us_census_shapefiles.py
--rw-r--r--   0        0        0    23248 2024-04-29 21:22:19.307957 censusdis-1.1.7/censusdis/impl/varcache.py
--rw-r--r--   0        0        0       66 2023-12-04 23:22:53.483682 censusdis-1.1.7/censusdis/impl/varsource/__init__.py
--rw-r--r--   0        0        0     6682 2024-03-14 21:06:25.570849 censusdis-1.1.7/censusdis/impl/varsource/base.py
--rw-r--r--   0        0        0     5672 2024-03-14 21:06:25.571500 censusdis-1.1.7/censusdis/impl/varsource/censusapi.py
--rw-r--r--   0        0        0    40124 2024-03-23 17:38:35.324606 censusdis-1.1.7/censusdis/maps.py
--rw-r--r--   0        0        0    34128 2023-12-11 20:36:12.393854 censusdis-1.1.7/censusdis/msa_msa.py
--rw-r--r--   0        0        0    14558 2023-12-11 19:29:35.515941 censusdis-1.1.7/censusdis/places/alabama.py
--rw-r--r--   0        0        0     8790 2023-12-11 19:29:35.516183 censusdis-1.1.7/censusdis/places/alaska.py
--rw-r--r--   0        0        0    11861 2023-12-11 19:29:35.516445 censusdis-1.1.7/censusdis/places/arizona.py
--rw-r--r--   0        0        0    15048 2023-12-11 19:29:35.516764 censusdis-1.1.7/censusdis/places/arkansas.py
--rw-r--r--   0        0        0    41385 2023-12-11 19:29:35.517121 censusdis-1.1.7/censusdis/places/california.py
--rw-r--r--   0        0        0    11894 2023-12-11 19:29:35.517306 censusdis-1.1.7/censusdis/places/colorado.py
--rw-r--r--   0        0        0     5822 2023-12-11 19:29:35.517517 censusdis-1.1.7/censusdis/places/connecticut.py
--rw-r--r--   0        0        0     2047 2023-12-11 19:29:35.517640 censusdis-1.1.7/censusdis/places/delaware.py
--rw-r--r--   0        0        0      108 2023-12-11 19:29:35.517800 censusdis-1.1.7/censusdis/places/district_of_columbia.py
--rw-r--r--   0        0        0    25466 2023-12-11 19:29:35.518158 censusdis-1.1.7/censusdis/places/florida.py
--rw-r--r--   0        0        0    16652 2023-12-11 19:29:35.518343 censusdis-1.1.7/censusdis/places/georgia.py
--rw-r--r--   0        0        0     4060 2023-12-11 19:29:35.518467 censusdis-1.1.7/censusdis/places/hawaii.py
--rw-r--r--   0        0        0     5685 2023-12-11 19:29:35.518634 censusdis-1.1.7/censusdis/places/idaho.py
--rw-r--r--   0        0        0    38933 2023-12-11 19:29:35.519027 censusdis-1.1.7/censusdis/places/illinois.py
--rw-r--r--   0        0        0    23926 2023-12-11 19:29:35.519320 censusdis-1.1.7/censusdis/places/indiana.py
--rw-r--r--   0        0        0    24633 2023-12-11 19:29:35.519626 censusdis-1.1.7/censusdis/places/iowa.py
--rw-r--r--   0        0        0    17556 2023-12-11 19:29:35.519874 censusdis-1.1.7/censusdis/places/kansas.py
--rw-r--r--   0        0        0    14063 2023-12-11 19:29:35.520117 censusdis-1.1.7/censusdis/places/kentucky.py
--rw-r--r--   0        0        0    12119 2023-12-11 19:29:35.520465 censusdis-1.1.7/censusdis/places/louisiana.py
--rw-r--r--   0        0        0     3818 2023-12-11 19:29:35.520594 censusdis-1.1.7/censusdis/places/maine.py
--rw-r--r--   0        0        0    13853 2023-12-11 19:29:35.520760 censusdis-1.1.7/censusdis/places/maryland.py
--rw-r--r--   0        0        0     6351 2023-12-11 19:29:35.520935 censusdis-1.1.7/censusdis/places/massachusetts.py
--rw-r--r--   0        0        0    19186 2023-12-11 19:29:35.521108 censusdis-1.1.7/censusdis/places/michigan.py
--rw-r--r--   0        0        0    22227 2023-12-11 19:29:35.521432 censusdis-1.1.7/censusdis/places/minnesota.py
--rw-r--r--   0        0        0    10406 2023-12-11 19:29:35.521602 censusdis-1.1.7/censusdis/places/mississippi.py
--rw-r--r--   0        0        0    27499 2023-12-11 19:29:35.521942 censusdis-1.1.7/censusdis/places/missouri.py
--rw-r--r--   0        0        0    12297 2023-12-11 19:29:35.522122 censusdis-1.1.7/censusdis/places/montana.py
--rw-r--r--   0        0        0    14951 2023-12-11 19:29:35.522289 censusdis-1.1.7/censusdis/places/nebraska.py
--rw-r--r--   0        0        0     3341 2023-12-11 19:29:35.522400 censusdis-1.1.7/censusdis/places/nevada.py
--rw-r--r--   0        0        0     2504 2023-12-11 19:29:35.522517 censusdis-1.1.7/censusdis/places/new_hampshire.py
--rw-r--r--   0        0        0    19179 2023-12-11 19:29:35.522722 censusdis-1.1.7/censusdis/places/new_jersey.py
--rw-r--r--   0        0        0    13434 2023-12-11 19:29:35.522891 censusdis-1.1.7/censusdis/places/new_mexico.py
--rw-r--r--   0        0        0    34855 2023-12-11 19:29:35.523211 censusdis-1.1.7/censusdis/places/new_york.py
--rw-r--r--   0        0        0    19432 2023-12-11 19:29:35.523418 censusdis-1.1.7/censusdis/places/north_carolina.py
--rw-r--r--   0        0        0     9524 2023-12-11 19:29:35.523558 censusdis-1.1.7/censusdis/places/north_dakota.py
--rw-r--r--   0        0        0    34277 2023-12-11 19:29:35.523920 censusdis-1.1.7/censusdis/places/ohio.py
--rw-r--r--   0        0        0    19802 2023-12-11 19:29:35.524122 censusdis-1.1.7/censusdis/places/oklahoma.py
--rw-r--r--   0        0        0    10398 2023-12-11 19:29:35.524366 censusdis-1.1.7/censusdis/places/oregon.py
--rw-r--r--   0        0        0    51324 2023-12-11 19:29:35.524811 censusdis-1.1.7/censusdis/places/pennsylvania.py
--rw-r--r--   0        0        0     9391 2023-12-11 19:29:35.524961 censusdis-1.1.7/censusdis/places/puerto_rico.py
--rw-r--r--   0        0        0      985 2023-12-11 19:29:35.525076 censusdis-1.1.7/censusdis/places/rhode_island.py
--rw-r--r--   0        0        0    11708 2023-12-11 19:29:35.525311 censusdis-1.1.7/censusdis/places/south_carolina.py
--rw-r--r--   0        0        0    12094 2023-12-11 19:29:35.525524 censusdis-1.1.7/censusdis/places/south_dakota.py
--rw-r--r--   0        0        0    12647 2023-12-11 19:29:35.525795 censusdis-1.1.7/censusdis/places/tennessee.py
--rw-r--r--   0        0        0    46473 2023-12-11 19:29:35.526090 censusdis-1.1.7/censusdis/places/texas.py
--rw-r--r--   0        0        0     8246 2023-12-11 19:29:35.526224 censusdis-1.1.7/censusdis/places/utah.py
--rw-r--r--   0        0        0     4712 2023-12-11 19:29:35.526351 censusdis-1.1.7/censusdis/places/vermont.py
--rw-r--r--   0        0        0    17023 2023-12-11 19:29:35.526524 censusdis-1.1.7/censusdis/places/virginia.py
--rw-r--r--   0        0        0    15869 2023-12-11 19:29:35.526833 censusdis-1.1.7/censusdis/places/washington.py
--rw-r--r--   0        0        0    10717 2023-12-11 19:29:35.526982 censusdis-1.1.7/censusdis/places/west_virginia.py
--rw-r--r--   0        0        0    20957 2023-12-11 19:29:35.527184 censusdis-1.1.7/censusdis/places/wisconsin.py
--rw-r--r--   0        0        0     5030 2023-12-11 19:29:35.527313 censusdis-1.1.7/censusdis/places/wyoming.py
--rw-r--r--   0        0        0      140 2023-12-11 20:36:13.710754 censusdis-1.1.7/censusdis/region.py
--rw-r--r--   0        0        0       70 2023-12-04 22:25:55.364310 censusdis-1.1.7/censusdis/resources/__init__.py
--rw-r--r--   0        0        0    25951 2023-05-29 16:16:27.245353 censusdis-1.1.7/censusdis/resources/crs_bounds.geojson
--rw-r--r--   0        0        0     7192 2023-12-04 21:03:55.744421 censusdis-1.1.7/censusdis/states.py
--rw-r--r--   0        0        0     2399 2023-05-29 16:16:27.245539 censusdis-1.1.7/censusdis/values.py
--rw-r--r--   0        0        0     4300 2024-05-21 22:06:52.612247 censusdis-1.1.7/pyproject.toml
--rw-r--r--   0        0        0     5948 1970-01-01 00:00:00.000000 censusdis-1.1.7/PKG-INFO
+-rw-r--r--   0        0        0    19938 2023-05-29 16:16:27.244036 censusdis-1.1.8/LICENSE.md
+-rw-r--r--   0        0        0     3717 2024-02-27 13:33:21.685281 censusdis-1.1.8/README.md
+-rw-r--r--   0        0        0     6148 2023-12-17 16:06:26.749329 censusdis-1.1.8/censusdis/.DS_Store
+-rw-r--r--   0        0        0      458 2024-02-15 00:31:57.583171 censusdis-1.1.8/censusdis/__init__.py
+-rw-r--r--   0        0        0       92 2023-12-04 23:22:53.481176 censusdis-1.1.8/censusdis/cli/__init__.py
+-rw-r--r--   0        0        0     5932 2023-12-05 20:25:11.495292 censusdis-1.1.8/censusdis/cli/cli.py
+-rw-r--r--   0        0        0    34433 2024-01-24 14:31:26.141820 censusdis-1.1.8/censusdis/cli/yamlspec.py
+-rw-r--r--   0        0        0     1129 2023-12-11 16:55:11.454323 censusdis-1.1.8/censusdis/counties/alabama.py
+-rw-r--r--   0        0        0     1013 2023-12-11 16:55:11.455889 censusdis-1.1.8/censusdis/counties/alaska.py
+-rw-r--r--   0        0        0      301 2023-12-11 16:55:11.456593 censusdis-1.1.8/censusdis/counties/arizona.py
+-rw-r--r--   0        0        0     1261 2023-12-11 16:55:11.459042 censusdis-1.1.8/censusdis/counties/arkansas.py
+-rw-r--r--   0        0        0     1029 2023-12-11 16:55:11.460975 censusdis-1.1.8/censusdis/counties/california.py
+-rw-r--r--   0        0        0     1091 2023-12-11 16:55:11.463070 censusdis-1.1.8/censusdis/counties/colorado.py
+-rw-r--r--   0        0        0     1115 2023-12-11 19:29:35.515569 censusdis-1.1.8/censusdis/counties/connecticut.py
+-rw-r--r--   0        0        0      119 2023-12-11 16:55:11.463832 censusdis-1.1.8/censusdis/counties/delaware.py
+-rw-r--r--   0        0        0      113 2023-12-11 16:55:11.464049 censusdis-1.1.8/censusdis/counties/district_of_columbia.py
+-rw-r--r--   0        0        0     1140 2023-12-11 16:55:11.466050 censusdis-1.1.8/censusdis/counties/florida.py
+-rw-r--r--   0        0        0     2539 2023-12-11 16:55:11.470438 censusdis-1.1.8/censusdis/counties/georgia.py
+-rw-r--r--   0        0        0      145 2023-12-11 16:55:11.470786 censusdis-1.1.8/censusdis/counties/hawaii.py
+-rw-r--r--   0        0        0      756 2023-12-11 16:55:11.472130 censusdis-1.1.8/censusdis/counties/idaho.py
+-rw-r--r--   0        0        0     1670 2023-12-11 16:55:11.474786 censusdis-1.1.8/censusdis/counties/illinois.py
+-rw-r--r--   0        0        0     1504 2023-12-11 16:55:11.477149 censusdis-1.1.8/censusdis/counties/indiana.py
+-rw-r--r--   0        0        0     1627 2023-12-11 16:55:11.479639 censusdis-1.1.8/censusdis/counties/iowa.py
+-rw-r--r--   0        0        0     1700 2023-12-11 16:55:11.482454 censusdis-1.1.8/censusdis/counties/kansas.py
+-rw-r--r--   0        0        0     1943 2023-12-11 16:55:11.485657 censusdis-1.1.8/censusdis/counties/kentucky.py
+-rw-r--r--   0        0        0     1227 2023-12-11 16:55:11.487208 censusdis-1.1.8/censusdis/counties/louisiana.py
+-rw-r--r--   0        0        0      340 2023-12-11 16:55:11.487753 censusdis-1.1.8/censusdis/counties/maine.py
+-rw-r--r--   0        0        0      492 2023-12-11 16:55:11.488448 censusdis-1.1.8/censusdis/counties/maryland.py
+-rw-r--r--   0        0        0      312 2023-12-11 16:55:11.488933 censusdis-1.1.8/censusdis/counties/massachusetts.py
+-rw-r--r--   0        0        0     1408 2023-12-11 16:55:11.490783 censusdis-1.1.8/censusdis/counties/michigan.py
+-rw-r--r--   0        0        0     1472 2023-12-11 16:55:11.492725 censusdis-1.1.8/censusdis/counties/minnesota.py
+-rw-r--r--   0        0        0     1388 2023-12-11 16:55:11.494560 censusdis-1.1.8/censusdis/counties/mississippi.py
+-rw-r--r--   0        0        0     1876 2023-12-11 16:55:11.496943 censusdis-1.1.8/censusdis/counties/missouri.py
+-rw-r--r--   0        0        0     1012 2023-12-11 16:55:11.498213 censusdis-1.1.8/censusdis/counties/montana.py
+-rw-r--r--   0        0        0     1496 2023-12-11 16:55:11.500179 censusdis-1.1.8/censusdis/counties/nebraska.py
+-rw-r--r--   0        0        0      339 2023-12-11 16:55:11.500687 censusdis-1.1.8/censusdis/counties/nevada.py
+-rw-r--r--   0        0        0      248 2023-12-11 16:55:11.501047 censusdis-1.1.8/censusdis/counties/new_hampshire.py
+-rw-r--r--   0        0        0      412 2023-12-11 16:55:11.501613 censusdis-1.1.8/censusdis/counties/new_jersey.py
+-rw-r--r--   0        0        0      593 2023-12-11 16:55:11.502420 censusdis-1.1.8/censusdis/counties/new_mexico.py
+-rw-r--r--   0        0        0     1083 2023-12-11 16:55:11.503743 censusdis-1.1.8/censusdis/counties/new_york.py
+-rw-r--r--   0        0        0     1668 2023-12-11 16:55:11.505932 censusdis-1.1.8/censusdis/counties/north_carolina.py
+-rw-r--r--   0        0        0      900 2023-12-11 16:55:11.507102 censusdis-1.1.8/censusdis/counties/north_dakota.py
+-rw-r--r--   0        0        0     1446 2023-12-11 16:55:11.508907 censusdis-1.1.8/censusdis/counties/ohio.py
+-rw-r--r--   0        0        0     1283 2023-12-11 16:55:11.510477 censusdis-1.1.8/censusdis/counties/oklahoma.py
+-rw-r--r--   0        0        0      635 2023-12-11 16:55:11.511295 censusdis-1.1.8/censusdis/counties/oregon.py
+-rw-r--r--   0        0        0     1168 2023-12-11 16:55:11.512672 censusdis-1.1.8/censusdis/counties/pennsylvania.py
+-rw-r--r--   0        0        0     1381 2023-12-11 16:55:11.532504 censusdis-1.1.8/censusdis/counties/puerto_rico.py
+-rw-r--r--   0        0        0      159 2023-12-11 16:55:11.512922 censusdis-1.1.8/censusdis/counties/rhode_island.py
+-rw-r--r--   0        0        0      855 2023-12-11 16:55:11.514193 censusdis-1.1.8/censusdis/counties/south_carolina.py
+-rw-r--r--   0        0        0     1104 2023-12-11 16:55:11.515784 censusdis-1.1.8/censusdis/counties/south_dakota.py
+-rw-r--r--   0        0        0     1568 2023-12-11 16:55:11.517745 censusdis-1.1.8/censusdis/counties/tennessee.py
+-rw-r--r--   0        0        0     4049 2023-12-11 16:55:11.522518 censusdis-1.1.8/censusdis/counties/texas.py
+-rw-r--r--   0        0        0      506 2023-12-11 16:55:11.523238 censusdis-1.1.8/censusdis/counties/utah.py
+-rw-r--r--   0        0        0      308 2023-12-11 16:55:11.523841 censusdis-1.1.8/censusdis/counties/vermont.py
+-rw-r--r--   0        0        0     2603 2023-12-11 16:55:11.526648 censusdis-1.1.8/censusdis/counties/virginia.py
+-rw-r--r--   0        0        0      705 2023-12-11 16:55:11.527561 censusdis-1.1.8/censusdis/counties/washington.py
+-rw-r--r--   0        0        0      938 2023-12-11 16:55:11.528745 censusdis-1.1.8/censusdis/counties/west_virginia.py
+-rw-r--r--   0        0        0     1219 2023-12-11 16:55:11.530242 censusdis-1.1.8/censusdis/counties/wisconsin.py
+-rw-r--r--   0        0        0      439 2023-12-11 16:55:11.530847 censusdis-1.1.8/censusdis/counties/wyoming.py
+-rw-r--r--   0        0        0     7109 2023-12-11 20:36:13.100154 censusdis-1.1.8/censusdis/csa.py
+-rw-r--r--   0        0        0    50314 2024-05-24 21:20:46.668068 censusdis-1.1.8/censusdis/data.py
+-rw-r--r--   0        0        0    30145 2024-05-24 16:40:27.253797 censusdis-1.1.8/censusdis/datasets.py
+-rw-r--r--   0        0        0      332 2023-12-11 20:36:14.332200 censusdis-1.1.8/censusdis/division.py
+-rw-r--r--   0        0        0    14425 2024-03-23 17:38:35.323871 censusdis-1.1.8/censusdis/geography.py
+-rw-r--r--   0        0        0       98 2023-12-04 23:22:53.473814 censusdis-1.1.8/censusdis/impl/__init__.py
+-rw-r--r--   0        0        0      160 2023-12-04 16:32:55.038743 censusdis-1.1.8/censusdis/impl/exceptions.py
+-rw-r--r--   0        0        0     7671 2024-03-23 17:38:35.324199 censusdis-1.1.8/censusdis/impl/fetch.py
+-rw-r--r--   0        0        0     5096 2024-01-26 21:46:43.129405 censusdis-1.1.8/censusdis/impl/geometry.py
+-rw-r--r--   0        0        0    21273 2024-04-29 21:22:19.307664 censusdis-1.1.8/censusdis/impl/us_census_shapefiles.py
+-rw-r--r--   0        0        0    23248 2024-04-29 21:22:19.307957 censusdis-1.1.8/censusdis/impl/varcache.py
+-rw-r--r--   0        0        0       66 2023-12-04 23:22:53.483682 censusdis-1.1.8/censusdis/impl/varsource/__init__.py
+-rw-r--r--   0        0        0     6682 2024-03-14 21:06:25.570849 censusdis-1.1.8/censusdis/impl/varsource/base.py
+-rw-r--r--   0        0        0     5672 2024-03-14 21:06:25.571500 censusdis-1.1.8/censusdis/impl/varsource/censusapi.py
+-rw-r--r--   0        0        0    40124 2024-03-23 17:38:35.324606 censusdis-1.1.8/censusdis/maps.py
+-rw-r--r--   0        0        0    34128 2023-12-11 20:36:12.393854 censusdis-1.1.8/censusdis/msa_msa.py
+-rw-r--r--   0        0        0    14558 2023-12-11 19:29:35.515941 censusdis-1.1.8/censusdis/places/alabama.py
+-rw-r--r--   0        0        0     8790 2023-12-11 19:29:35.516183 censusdis-1.1.8/censusdis/places/alaska.py
+-rw-r--r--   0        0        0    11861 2023-12-11 19:29:35.516445 censusdis-1.1.8/censusdis/places/arizona.py
+-rw-r--r--   0        0        0    15048 2023-12-11 19:29:35.516764 censusdis-1.1.8/censusdis/places/arkansas.py
+-rw-r--r--   0        0        0    41385 2023-12-11 19:29:35.517121 censusdis-1.1.8/censusdis/places/california.py
+-rw-r--r--   0        0        0    11894 2023-12-11 19:29:35.517306 censusdis-1.1.8/censusdis/places/colorado.py
+-rw-r--r--   0        0        0     5822 2023-12-11 19:29:35.517517 censusdis-1.1.8/censusdis/places/connecticut.py
+-rw-r--r--   0        0        0     2047 2023-12-11 19:29:35.517640 censusdis-1.1.8/censusdis/places/delaware.py
+-rw-r--r--   0        0        0      108 2023-12-11 19:29:35.517800 censusdis-1.1.8/censusdis/places/district_of_columbia.py
+-rw-r--r--   0        0        0    25466 2023-12-11 19:29:35.518158 censusdis-1.1.8/censusdis/places/florida.py
+-rw-r--r--   0        0        0    16652 2023-12-11 19:29:35.518343 censusdis-1.1.8/censusdis/places/georgia.py
+-rw-r--r--   0        0        0     4060 2023-12-11 19:29:35.518467 censusdis-1.1.8/censusdis/places/hawaii.py
+-rw-r--r--   0        0        0     5685 2023-12-11 19:29:35.518634 censusdis-1.1.8/censusdis/places/idaho.py
+-rw-r--r--   0        0        0    38933 2023-12-11 19:29:35.519027 censusdis-1.1.8/censusdis/places/illinois.py
+-rw-r--r--   0        0        0    23926 2023-12-11 19:29:35.519320 censusdis-1.1.8/censusdis/places/indiana.py
+-rw-r--r--   0        0        0    24633 2023-12-11 19:29:35.519626 censusdis-1.1.8/censusdis/places/iowa.py
+-rw-r--r--   0        0        0    17556 2023-12-11 19:29:35.519874 censusdis-1.1.8/censusdis/places/kansas.py
+-rw-r--r--   0        0        0    14063 2023-12-11 19:29:35.520117 censusdis-1.1.8/censusdis/places/kentucky.py
+-rw-r--r--   0        0        0    12119 2023-12-11 19:29:35.520465 censusdis-1.1.8/censusdis/places/louisiana.py
+-rw-r--r--   0        0        0     3818 2023-12-11 19:29:35.520594 censusdis-1.1.8/censusdis/places/maine.py
+-rw-r--r--   0        0        0    13853 2023-12-11 19:29:35.520760 censusdis-1.1.8/censusdis/places/maryland.py
+-rw-r--r--   0        0        0     6351 2023-12-11 19:29:35.520935 censusdis-1.1.8/censusdis/places/massachusetts.py
+-rw-r--r--   0        0        0    19186 2023-12-11 19:29:35.521108 censusdis-1.1.8/censusdis/places/michigan.py
+-rw-r--r--   0        0        0    22227 2023-12-11 19:29:35.521432 censusdis-1.1.8/censusdis/places/minnesota.py
+-rw-r--r--   0        0        0    10406 2023-12-11 19:29:35.521602 censusdis-1.1.8/censusdis/places/mississippi.py
+-rw-r--r--   0        0        0    27499 2023-12-11 19:29:35.521942 censusdis-1.1.8/censusdis/places/missouri.py
+-rw-r--r--   0        0        0    12297 2023-12-11 19:29:35.522122 censusdis-1.1.8/censusdis/places/montana.py
+-rw-r--r--   0        0        0    14951 2023-12-11 19:29:35.522289 censusdis-1.1.8/censusdis/places/nebraska.py
+-rw-r--r--   0        0        0     3341 2023-12-11 19:29:35.522400 censusdis-1.1.8/censusdis/places/nevada.py
+-rw-r--r--   0        0        0     2504 2023-12-11 19:29:35.522517 censusdis-1.1.8/censusdis/places/new_hampshire.py
+-rw-r--r--   0        0        0    19179 2023-12-11 19:29:35.522722 censusdis-1.1.8/censusdis/places/new_jersey.py
+-rw-r--r--   0        0        0    13434 2023-12-11 19:29:35.522891 censusdis-1.1.8/censusdis/places/new_mexico.py
+-rw-r--r--   0        0        0    34855 2023-12-11 19:29:35.523211 censusdis-1.1.8/censusdis/places/new_york.py
+-rw-r--r--   0        0        0    19432 2023-12-11 19:29:35.523418 censusdis-1.1.8/censusdis/places/north_carolina.py
+-rw-r--r--   0        0        0     9524 2023-12-11 19:29:35.523558 censusdis-1.1.8/censusdis/places/north_dakota.py
+-rw-r--r--   0        0        0    34277 2023-12-11 19:29:35.523920 censusdis-1.1.8/censusdis/places/ohio.py
+-rw-r--r--   0        0        0    19802 2023-12-11 19:29:35.524122 censusdis-1.1.8/censusdis/places/oklahoma.py
+-rw-r--r--   0        0        0    10398 2023-12-11 19:29:35.524366 censusdis-1.1.8/censusdis/places/oregon.py
+-rw-r--r--   0        0        0    51324 2023-12-11 19:29:35.524811 censusdis-1.1.8/censusdis/places/pennsylvania.py
+-rw-r--r--   0        0        0     9391 2023-12-11 19:29:35.524961 censusdis-1.1.8/censusdis/places/puerto_rico.py
+-rw-r--r--   0        0        0      985 2023-12-11 19:29:35.525076 censusdis-1.1.8/censusdis/places/rhode_island.py
+-rw-r--r--   0        0        0    11708 2023-12-11 19:29:35.525311 censusdis-1.1.8/censusdis/places/south_carolina.py
+-rw-r--r--   0        0        0    12094 2023-12-11 19:29:35.525524 censusdis-1.1.8/censusdis/places/south_dakota.py
+-rw-r--r--   0        0        0    12647 2023-12-11 19:29:35.525795 censusdis-1.1.8/censusdis/places/tennessee.py
+-rw-r--r--   0        0        0    46473 2023-12-11 19:29:35.526090 censusdis-1.1.8/censusdis/places/texas.py
+-rw-r--r--   0        0        0     8246 2023-12-11 19:29:35.526224 censusdis-1.1.8/censusdis/places/utah.py
+-rw-r--r--   0        0        0     4712 2023-12-11 19:29:35.526351 censusdis-1.1.8/censusdis/places/vermont.py
+-rw-r--r--   0        0        0    17023 2023-12-11 19:29:35.526524 censusdis-1.1.8/censusdis/places/virginia.py
+-rw-r--r--   0        0        0    15869 2023-12-11 19:29:35.526833 censusdis-1.1.8/censusdis/places/washington.py
+-rw-r--r--   0        0        0    10717 2023-12-11 19:29:35.526982 censusdis-1.1.8/censusdis/places/west_virginia.py
+-rw-r--r--   0        0        0    20957 2023-12-11 19:29:35.527184 censusdis-1.1.8/censusdis/places/wisconsin.py
+-rw-r--r--   0        0        0     5030 2023-12-11 19:29:35.527313 censusdis-1.1.8/censusdis/places/wyoming.py
+-rw-r--r--   0        0        0      140 2023-12-11 20:36:13.710754 censusdis-1.1.8/censusdis/region.py
+-rw-r--r--   0        0        0       70 2023-12-04 22:25:55.364310 censusdis-1.1.8/censusdis/resources/__init__.py
+-rw-r--r--   0        0        0    25951 2023-05-29 16:16:27.245353 censusdis-1.1.8/censusdis/resources/crs_bounds.geojson
+-rw-r--r--   0        0        0     7192 2023-12-04 21:03:55.744421 censusdis-1.1.8/censusdis/states.py
+-rw-r--r--   0        0        0     2399 2023-05-29 16:16:27.245539 censusdis-1.1.8/censusdis/values.py
+-rw-r--r--   0        0        0     4300 2024-05-24 18:13:00.826390 censusdis-1.1.8/pyproject.toml
+-rw-r--r--   0        0        0     5948 1970-01-01 00:00:00.000000 censusdis-1.1.8/PKG-INFO
```

### Comparing `censusdis-1.1.7/LICENSE.md` & `censusdis-1.1.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/README.md` & `censusdis-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/.DS_Store` & `censusdis-1.1.8/censusdis/.DS_Store`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/cli/cli.py` & `censusdis-1.1.8/censusdis/cli/cli.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/cli/yamlspec.py` & `censusdis-1.1.8/censusdis/cli/yamlspec.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/counties/alabama.py` & `censusdis-1.1.8/censusdis/counties/alabama.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/counties/alaska.py` & `censusdis-1.1.8/censusdis/counties/alaska.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/counties/arkansas.py` & `censusdis-1.1.8/censusdis/counties/arkansas.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/counties/california.py` & `censusdis-1.1.8/censusdis/counties/california.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/counties/colorado.py` & `censusdis-1.1.8/censusdis/counties/colorado.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/counties/connecticut.py` & `censusdis-1.1.8/censusdis/counties/connecticut.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/counties/florida.py` & `censusdis-1.1.8/censusdis/counties/florida.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/counties/georgia.py` & `censusdis-1.1.8/censusdis/counties/georgia.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/counties/idaho.py` & `censusdis-1.1.8/censusdis/counties/idaho.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/counties/illinois.py` & `censusdis-1.1.8/censusdis/counties/illinois.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/counties/indiana.py` & `censusdis-1.1.8/censusdis/counties/indiana.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/counties/iowa.py` & `censusdis-1.1.8/censusdis/counties/iowa.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/counties/kansas.py` & `censusdis-1.1.8/censusdis/counties/kansas.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/counties/kentucky.py` & `censusdis-1.1.8/censusdis/counties/kentucky.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/counties/louisiana.py` & `censusdis-1.1.8/censusdis/counties/louisiana.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/counties/michigan.py` & `censusdis-1.1.8/censusdis/counties/michigan.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/counties/minnesota.py` & `censusdis-1.1.8/censusdis/counties/minnesota.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/counties/mississippi.py` & `censusdis-1.1.8/censusdis/counties/mississippi.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/counties/missouri.py` & `censusdis-1.1.8/censusdis/counties/missouri.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/counties/montana.py` & `censusdis-1.1.8/censusdis/counties/montana.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/counties/nebraska.py` & `censusdis-1.1.8/censusdis/counties/nebraska.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/counties/new_mexico.py` & `censusdis-1.1.8/censusdis/counties/new_mexico.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/counties/new_york.py` & `censusdis-1.1.8/censusdis/counties/new_york.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/counties/north_carolina.py` & `censusdis-1.1.8/censusdis/counties/north_carolina.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/counties/north_dakota.py` & `censusdis-1.1.8/censusdis/counties/north_dakota.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/counties/ohio.py` & `censusdis-1.1.8/censusdis/counties/ohio.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/counties/oklahoma.py` & `censusdis-1.1.8/censusdis/counties/oklahoma.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/counties/oregon.py` & `censusdis-1.1.8/censusdis/counties/oregon.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/counties/pennsylvania.py` & `censusdis-1.1.8/censusdis/counties/pennsylvania.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/counties/puerto_rico.py` & `censusdis-1.1.8/censusdis/counties/puerto_rico.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/counties/south_carolina.py` & `censusdis-1.1.8/censusdis/counties/south_carolina.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/counties/south_dakota.py` & `censusdis-1.1.8/censusdis/counties/south_dakota.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/counties/tennessee.py` & `censusdis-1.1.8/censusdis/counties/tennessee.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/counties/texas.py` & `censusdis-1.1.8/censusdis/counties/texas.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/counties/virginia.py` & `censusdis-1.1.8/censusdis/counties/virginia.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/counties/washington.py` & `censusdis-1.1.8/censusdis/counties/washington.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/counties/west_virginia.py` & `censusdis-1.1.8/censusdis/counties/west_virginia.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/counties/wisconsin.py` & `censusdis-1.1.8/censusdis/counties/wisconsin.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/csa.py` & `censusdis-1.1.8/censusdis/csa.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/data.py` & `censusdis-1.1.8/censusdis/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -644,15 +644,15 @@
     for variable in download_variables:
         # predicateType does not exist in some older data sets like acs/acs3
         # So in that case we just go with what we got in the JSON. But if we
         # have it try to set the type.
         if "predicateType" in variable_cache.get(dataset, vintage, variable):
             field_type = variable_cache.get(dataset, vintage, variable)["predicateType"]
 
-            if field_type == "int":
+            if field_type == "int" or field_type == "long":
                 if df_data[variable].isnull().any():
                     # Some Census data sets put in null in int fields.
                     # We have to go with a float to make this a NaN.
                     # Int has no representation for NaN or None.
                     df_data[variable] = df_data[variable].astype(float, errors="ignore")
                 else:
                     try:
```

### Comparing `censusdis-1.1.7/censusdis/datasets.py` & `censusdis-1.1.8/censusdis/datasets.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,14 +204,16 @@
 
 CPS_VOTING_NOV = "cps/voting/nov"
 
 CPS_WORKSCHED_MAY = "cps/worksched/may"
 
 CRE = "cre"
 
+CREPUERTORICO = "crepuertorico"
+
 DECENNIAL_AIAN = "dec/aian"
 
 DECENNIAL_AIANPROFILE = "dec/aianprofile"
 
 DECENNIAL_AS = "dec/as"
 
 DECENNIAL_ASYOE = "dec/asyoe"
@@ -710,14 +712,15 @@
     CPS_VETS_AUG: "http://api.census.gov/data/2023/cps/vets/aug",
     CPS_VETS_JUL: "http://api.census.gov/data/2010/cps/vets/jul",
     CPS_VETS_SEP: "http://api.census.gov/data/1999/cps/vets/sep",
     CPS_VOLUNTEER_SEP: "http://api.census.gov/data/2021/cps/volunteer/sep",
     CPS_VOTING_NOV: "http://api.census.gov/data/2022/cps/voting/nov",
     CPS_WORKSCHED_MAY: "http://api.census.gov/data/2004/cps/worksched/may",
     CRE: "http://api.census.gov/data/2022/cre",
+    CREPUERTORICO: "http://api.census.gov/data/2022/crepuertorico",
     DECENNIAL_AIAN: "http://api.census.gov/data/2010/dec/aian",
     DECENNIAL_AIANPROFILE: "http://api.census.gov/data/2000/dec/aianprofile",
     DECENNIAL_AS: "http://api.census.gov/data/2010/dec/as",
     DECENNIAL_ASYOE: "http://api.census.gov/data/2010/dec/asyoe",
     DECENNIAL_CD110H: "http://api.census.gov/data/2000/dec/cd110h",
     DECENNIAL_CD110HPROFILE: "http://api.census.gov/data/2000/dec/cd110hprofile",
     DECENNIAL_CD110S: "http://api.census.gov/data/2000/dec/cd110s",
```

### Comparing `censusdis-1.1.7/censusdis/geography.py` & `censusdis-1.1.8/censusdis/geography.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/impl/fetch.py` & `censusdis-1.1.8/censusdis/impl/fetch.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/impl/geometry.py` & `censusdis-1.1.8/censusdis/impl/geometry.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/impl/us_census_shapefiles.py` & `censusdis-1.1.8/censusdis/impl/us_census_shapefiles.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/impl/varcache.py` & `censusdis-1.1.8/censusdis/impl/varcache.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/impl/varsource/base.py` & `censusdis-1.1.8/censusdis/impl/varsource/base.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/impl/varsource/censusapi.py` & `censusdis-1.1.8/censusdis/impl/varsource/censusapi.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/maps.py` & `censusdis-1.1.8/censusdis/maps.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/msa_msa.py` & `censusdis-1.1.8/censusdis/msa_msa.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/places/alabama.py` & `censusdis-1.1.8/censusdis/places/alabama.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/places/alaska.py` & `censusdis-1.1.8/censusdis/places/alaska.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/places/arizona.py` & `censusdis-1.1.8/censusdis/places/arizona.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/places/arkansas.py` & `censusdis-1.1.8/censusdis/places/arkansas.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/places/california.py` & `censusdis-1.1.8/censusdis/places/california.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/places/colorado.py` & `censusdis-1.1.8/censusdis/places/colorado.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/places/connecticut.py` & `censusdis-1.1.8/censusdis/places/connecticut.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/places/delaware.py` & `censusdis-1.1.8/censusdis/places/delaware.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/places/florida.py` & `censusdis-1.1.8/censusdis/places/florida.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/places/georgia.py` & `censusdis-1.1.8/censusdis/places/georgia.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/places/hawaii.py` & `censusdis-1.1.8/censusdis/places/hawaii.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/places/idaho.py` & `censusdis-1.1.8/censusdis/places/idaho.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/places/illinois.py` & `censusdis-1.1.8/censusdis/places/illinois.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/places/indiana.py` & `censusdis-1.1.8/censusdis/places/indiana.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/places/iowa.py` & `censusdis-1.1.8/censusdis/places/iowa.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/places/kansas.py` & `censusdis-1.1.8/censusdis/places/kansas.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/places/kentucky.py` & `censusdis-1.1.8/censusdis/places/kentucky.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/places/louisiana.py` & `censusdis-1.1.8/censusdis/places/louisiana.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/places/maine.py` & `censusdis-1.1.8/censusdis/places/maine.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/places/maryland.py` & `censusdis-1.1.8/censusdis/places/maryland.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/places/massachusetts.py` & `censusdis-1.1.8/censusdis/places/massachusetts.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/places/michigan.py` & `censusdis-1.1.8/censusdis/places/michigan.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/places/minnesota.py` & `censusdis-1.1.8/censusdis/places/minnesota.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/places/mississippi.py` & `censusdis-1.1.8/censusdis/places/mississippi.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/places/missouri.py` & `censusdis-1.1.8/censusdis/places/missouri.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/places/montana.py` & `censusdis-1.1.8/censusdis/places/montana.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/places/nebraska.py` & `censusdis-1.1.8/censusdis/places/nebraska.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/places/nevada.py` & `censusdis-1.1.8/censusdis/places/nevada.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/places/new_hampshire.py` & `censusdis-1.1.8/censusdis/places/new_hampshire.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/places/new_jersey.py` & `censusdis-1.1.8/censusdis/places/new_jersey.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/places/new_mexico.py` & `censusdis-1.1.8/censusdis/places/new_mexico.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/places/new_york.py` & `censusdis-1.1.8/censusdis/places/new_york.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/places/north_carolina.py` & `censusdis-1.1.8/censusdis/places/north_carolina.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/places/north_dakota.py` & `censusdis-1.1.8/censusdis/places/north_dakota.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/places/ohio.py` & `censusdis-1.1.8/censusdis/places/ohio.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/places/oklahoma.py` & `censusdis-1.1.8/censusdis/places/oklahoma.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/places/oregon.py` & `censusdis-1.1.8/censusdis/places/oregon.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/places/pennsylvania.py` & `censusdis-1.1.8/censusdis/places/pennsylvania.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/places/puerto_rico.py` & `censusdis-1.1.8/censusdis/places/puerto_rico.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/places/rhode_island.py` & `censusdis-1.1.8/censusdis/places/rhode_island.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/places/south_carolina.py` & `censusdis-1.1.8/censusdis/places/south_carolina.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/places/south_dakota.py` & `censusdis-1.1.8/censusdis/places/south_dakota.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/places/tennessee.py` & `censusdis-1.1.8/censusdis/places/tennessee.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/places/texas.py` & `censusdis-1.1.8/censusdis/places/texas.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/places/utah.py` & `censusdis-1.1.8/censusdis/places/utah.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/places/vermont.py` & `censusdis-1.1.8/censusdis/places/vermont.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/places/virginia.py` & `censusdis-1.1.8/censusdis/places/virginia.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/places/washington.py` & `censusdis-1.1.8/censusdis/places/washington.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/places/west_virginia.py` & `censusdis-1.1.8/censusdis/places/west_virginia.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/places/wisconsin.py` & `censusdis-1.1.8/censusdis/places/wisconsin.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/places/wyoming.py` & `censusdis-1.1.8/censusdis/places/wyoming.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/resources/crs_bounds.geojson` & `censusdis-1.1.8/censusdis/resources/crs_bounds.geojson`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/states.py` & `censusdis-1.1.8/censusdis/states.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/censusdis/values.py` & `censusdis-1.1.8/censusdis/values.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.7/pyproject.toml` & `censusdis-1.1.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "censusdis"
-version = "1.1.7"
+version = "1.1.8"
 description = "US Census utilities for a variety of data loading, analysis, and mapping purposes."
 license = "HL3-CL-ECO-EXTR-FFD-LAW-MIL-SV"
 authors = ["Darren Vengroff"]
 readme = "README.md"
 repository = "https://github.com/vengroff/censusdis"
 keywords = ["census", "demographics"]
 classifiers = [
```

### Comparing `censusdis-1.1.7/PKG-INFO` & `censusdis-1.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: censusdis
-Version: 1.1.7
+Version: 1.1.8
 Summary: US Census utilities for a variety of data loading, analysis, and mapping purposes.
 Home-page: https://github.com/vengroff/censusdis
 License: HL3-CL-ECO-EXTR-FFD-LAW-MIL-SV
 Keywords: census,demographics
 Author: Darren Vengroff
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
```

