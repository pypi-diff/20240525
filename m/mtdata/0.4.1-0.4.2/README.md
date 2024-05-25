# Comparing `tmp/mtdata-0.4.1.tar.gz` & `tmp/mtdata-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mtdata-0.4.1.tar", last modified: Fri Apr 26 04:42:17 2024, max compression
+gzip compressed data, was "mtdata-0.4.2.tar", last modified: Sat May 25 03:22:43 2024, max compression
```

## Comparing `mtdata-0.4.1.tar` & `mtdata-0.4.2.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxrwxr-x   0 tg        (1003) tg        (1003)        0 2024-04-26 04:42:17.142503 mtdata-0.4.1/
--rw-rw-r--   0 tg        (1003) tg        (1003)    11357 2024-03-05 03:25:13.000000 mtdata-0.4.1/LICENSE
--rw-rw-r--   0 tg        (1003) tg        (1003)       91 2024-03-05 03:25:13.000000 mtdata-0.4.1/MANIFEST.in
--rw-rw-r--   0 tg        (1003) tg        (1003)    19043 2024-04-26 04:42:17.138503 mtdata-0.4.1/PKG-INFO
--rw-rw-r--   0 tg        (1003) tg        (1003)    18137 2024-04-26 04:37:33.000000 mtdata-0.4.1/README.md
-drwxrwxr-x   0 tg        (1003) tg        (1003)        0 2024-04-26 04:42:17.122503 mtdata-0.4.1/mtdata/
--rw-rw-r--   0 tg        (1003) tg        (1003)      972 2024-04-26 04:37:33.000000 mtdata-0.4.1/mtdata/__init__.py
--rw-rw-r--   0 tg        (1003) tg        (1003)      341 2024-03-05 03:25:14.000000 mtdata-0.4.1/mtdata/__main__.py
--rw-rw-r--   0 tg        (1003) tg        (1003)     8726 2024-04-26 04:37:28.000000 mtdata-0.4.1/mtdata/cache.py
--rw-rw-r--   0 tg        (1003) tg        (1003)    24634 2024-04-26 04:37:28.000000 mtdata-0.4.1/mtdata/data.py
--rw-rw-r--   0 tg        (1003) tg        (1003)     7067 2024-03-05 03:25:14.000000 mtdata-0.4.1/mtdata/entry.py
-drwxrwxr-x   0 tg        (1003) tg        (1003)        0 2024-04-26 04:42:17.126503 mtdata-0.4.1/mtdata/index/
--rw-rw-r--   0 tg        (1003) tg        (1003)     8548 2024-03-05 03:25:14.000000 mtdata-0.4.1/mtdata/index/__init__.py
--rw-rw-r--   0 tg        (1003) tg        (1003)     2698 2024-03-05 03:25:14.000000 mtdata-0.4.1/mtdata/index/ai4bharat.py
--rw-rw-r--   0 tg        (1003) tg        (1003)      974 2024-03-05 03:25:14.000000 mtdata-0.4.1/mtdata/index/allenai_nllb.py
--rw-rw-r--   0 tg        (1003) tg        (1003)     2022 2024-03-05 03:25:14.000000 mtdata-0.4.1/mtdata/index/anuvaad.py
--rw-rw-r--   0 tg        (1003) tg        (1003)     1854 2024-03-05 03:25:14.000000 mtdata-0.4.1/mtdata/index/elrc_share.py
--rw-rw-r--   0 tg        (1003) tg        (1003)     2572 2024-03-05 03:25:14.000000 mtdata-0.4.1/mtdata/index/eu.py
--rw-rw-r--   0 tg        (1003) tg        (1003)     5181 2024-03-05 03:25:14.000000 mtdata-0.4.1/mtdata/index/flores.py
--rw-rw-r--   0 tg        (1003) tg        (1003)     1029 2024-03-05 03:25:14.000000 mtdata-0.4.1/mtdata/index/joshua_indian.py
--rw-rw-r--   0 tg        (1003) tg        (1003)     1606 2024-03-05 03:25:14.000000 mtdata-0.4.1/mtdata/index/leipzig.py
--rw-rw-r--   0 tg        (1003) tg        (1003)     6233 2024-03-05 03:25:14.000000 mtdata-0.4.1/mtdata/index/linguatools.py
--rw-rw-r--   0 tg        (1003) tg        (1003)     1556 2024-03-05 03:25:14.000000 mtdata-0.4.1/mtdata/index/neulab_tedtalks.py
-drwxrwxr-x   0 tg        (1003) tg        (1003)        0 2024-04-26 04:42:17.126503 mtdata-0.4.1/mtdata/index/opus/
--rw-rw-r--   0 tg        (1003) tg        (1003)       90 2024-03-05 03:25:14.000000 mtdata-0.4.1/mtdata/index/opus/__init__.py
--rw-rw-r--   0 tg        (1003) tg        (1003)     1213 2024-03-05 03:25:14.000000 mtdata-0.4.1/mtdata/index/opus/crawl_parse.py
--rw-rw-r--   0 tg        (1003) tg        (1003)   171105 2024-03-05 03:25:14.000000 mtdata-0.4.1/mtdata/index/opus/jw300.py
--rw-rw-r--   0 tg        (1003) tg        (1003)     2503 2024-03-05 03:25:14.000000 mtdata-0.4.1/mtdata/index/opus/opus100.py
--rw-rw-r--   0 tg        (1003) tg        (1003)     2457 2024-04-26 04:37:28.000000 mtdata-0.4.1/mtdata/index/opus/opus_index.py
--rw-rw-r--   0 tg        (1003) tg        (1003)     9441 2024-03-05 03:25:14.000000 mtdata-0.4.1/mtdata/index/other.py
--rw-rw-r--   0 tg        (1003) tg        (1003)     5316 2024-03-05 03:25:14.000000 mtdata-0.4.1/mtdata/index/paracrawl.py
--rw-rw-r--   0 tg        (1003) tg        (1003)    27995 2024-04-26 04:37:28.000000 mtdata-0.4.1/mtdata/index/statmt.py
--rw-rw-r--   0 tg        (1003) tg        (1003)     4114 2024-03-05 03:25:14.000000 mtdata-0.4.1/mtdata/index/tilde.py
--rw-rw-r--   0 tg        (1003) tg        (1003)      937 2024-03-05 03:25:14.000000 mtdata-0.4.1/mtdata/index/unitednations.py
--rw-rw-r--   0 tg        (1003) tg        (1003)    10566 2024-03-05 03:25:14.000000 mtdata-0.4.1/mtdata/index/wikimatrix.py
-drwxrwxr-x   0 tg        (1003) tg        (1003)        0 2024-04-26 04:42:17.130503 mtdata-0.4.1/mtdata/iso/
--rw-rw-r--   0 tg        (1003) tg        (1003)      148 2024-03-05 03:25:14.000000 mtdata-0.4.1/mtdata/iso/__init__.py
--rw-rw-r--   0 tg        (1003) tg        (1003)     1436 2024-03-05 03:25:14.000000 mtdata-0.4.1/mtdata/iso/__main__.py
--rw-rw-r--   0 tg        (1003) tg        (1003)   247313 2024-03-05 03:25:14.000000 mtdata-0.4.1/mtdata/iso/bcp47.json
--rw-rw-r--   0 tg        (1003) tg        (1003)    10188 2024-04-26 04:37:28.000000 mtdata-0.4.1/mtdata/iso/bcp47.py
--rw-rw-r--   0 tg        (1003) tg        (1003)      433 2024-03-05 03:25:14.000000 mtdata-0.4.1/mtdata/iso/custom.py
--rw-rw-r--   0 tg        (1003) tg        (1003)     1528 2024-03-05 03:25:14.000000 mtdata-0.4.1/mtdata/iso/iso639.py
--rw-rw-r--   0 tg        (1003) tg        (1003)     1769 2024-03-05 03:25:14.000000 mtdata-0.4.1/mtdata/iso/iso639_1.py
--rw-rw-r--   0 tg        (1003) tg        (1003)     9543 2024-03-05 03:25:14.000000 mtdata-0.4.1/mtdata/iso/iso639_2.py
--rw-rw-r--   0 tg        (1003) tg        (1003)   125322 2024-03-05 03:25:14.000000 mtdata-0.4.1/mtdata/iso/iso639_3.py
--rw-rw-r--   0 tg        (1003) tg        (1003)    16779 2024-04-26 04:37:28.000000 mtdata-0.4.1/mtdata/main.py
--rw-rw-r--   0 tg        (1003) tg        (1003)     4150 2024-03-05 03:25:14.000000 mtdata-0.4.1/mtdata/opus_xces.py
--rw-rw-r--   0 tg        (1003) tg        (1003)     5052 2024-03-05 03:25:14.000000 mtdata-0.4.1/mtdata/parser.py
--rw-rw-r--   0 tg        (1003) tg        (1003)     2318 2024-04-26 04:37:28.000000 mtdata-0.4.1/mtdata/pigz.py
-drwxrwxr-x   0 tg        (1003) tg        (1003)        0 2024-04-26 04:42:17.130503 mtdata-0.4.1/mtdata/recipe/
--rw-rw-r--   0 tg        (1003) tg        (1003)     3934 2024-04-26 04:37:28.000000 mtdata-0.4.1/mtdata/recipe/__init__.py
-drwxrwxr-x   0 tg        (1003) tg        (1003)        0 2024-04-26 04:42:17.138503 mtdata-0.4.1/mtdata/resource/
--rw-rw-r--   0 tg        (1003) tg        (1003)    40277 2024-03-05 03:25:14.000000 mtdata-0.4.1/mtdata/resource/allenai_nllb.json
--rw-rw-r--   0 tg        (1003) tg        (1003)    17310 2024-03-05 03:25:14.000000 mtdata-0.4.1/mtdata/resource/anuvaad.tsv
--rw-rw-r--   0 tg        (1003) tg        (1003)   674369 2024-03-05 03:25:14.000000 mtdata-0.4.1/mtdata/resource/elrc_share.tsv
--rw-rw-r--   0 tg        (1003) tg        (1003)   127368 2024-03-05 03:25:14.000000 mtdata-0.4.1/mtdata/resource/leipzig_de.txt
--rw-rw-r--   0 tg        (1003) tg        (1003)  3319201 2024-04-26 04:37:28.000000 mtdata-0.4.1/mtdata/resource/opus_index.tsv
--rw-rw-r--   0 tg        (1003) tg        (1003)     1375 2024-04-26 04:37:28.000000 mtdata-0.4.1/mtdata/resource/recipes.yml
--rw-rw-r--   0 tg        (1003) tg        (1003)    26753 2024-04-26 04:37:28.000000 mtdata-0.4.1/mtdata/resource/refs.bib
-drwxrwxr-x   0 tg        (1003) tg        (1003)        0 2024-04-26 04:42:17.138503 mtdata-0.4.1/mtdata/scripts/
--rwxrwxr-x   0 tg        (1003) tg        (1003)     7132 2024-03-05 03:25:14.000000 mtdata-0.4.1/mtdata/scripts/recipe_stats.py
--rw-rw-r--   0 tg        (1003) tg        (1003)     1278 2024-03-05 03:25:14.000000 mtdata-0.4.1/mtdata/scripts/tsv2xls.py
--rw-rw-r--   0 tg        (1003) tg        (1003)     3283 2024-04-26 04:37:28.000000 mtdata-0.4.1/mtdata/sgm.py
--rw-rw-r--   0 tg        (1003) tg        (1003)     4071 2024-03-05 03:25:14.000000 mtdata-0.4.1/mtdata/tmx.py
--rw-rw-r--   0 tg        (1003) tg        (1003)     8456 2024-04-26 04:37:28.000000 mtdata-0.4.1/mtdata/utils.py
-drwxrwxr-x   0 tg        (1003) tg        (1003)        0 2024-04-26 04:42:17.122503 mtdata-0.4.1/mtdata.egg-info/
--rw-rw-r--   0 tg        (1003) tg        (1003)    19043 2024-04-26 04:42:17.000000 mtdata-0.4.1/mtdata.egg-info/PKG-INFO
--rw-rw-r--   0 tg        (1003) tg        (1003)     1750 2024-04-26 04:42:17.000000 mtdata-0.4.1/mtdata.egg-info/SOURCES.txt
--rw-rw-r--   0 tg        (1003) tg        (1003)        1 2024-04-26 04:42:17.000000 mtdata-0.4.1/mtdata.egg-info/dependency_links.txt
--rw-rw-r--   0 tg        (1003) tg        (1003)      123 2024-04-26 04:42:17.000000 mtdata-0.4.1/mtdata.egg-info/entry_points.txt
--rw-rw-r--   0 tg        (1003) tg        (1003)        1 2024-04-26 04:42:17.000000 mtdata-0.4.1/mtdata.egg-info/not-zip-safe
--rw-rw-r--   0 tg        (1003) tg        (1003)       90 2024-04-26 04:42:17.000000 mtdata-0.4.1/mtdata.egg-info/requires.txt
--rw-rw-r--   0 tg        (1003) tg        (1003)        7 2024-04-26 04:42:17.000000 mtdata-0.4.1/mtdata.egg-info/top_level.txt
--rw-rw-r--   0 tg        (1003) tg        (1003)       38 2024-04-26 04:42:17.142503 mtdata-0.4.1/setup.cfg
--rw-rw-r--   0 tg        (1003) tg        (1003)     2209 2024-04-26 04:37:28.000000 mtdata-0.4.1/setup.py
-drwxrwxr-x   0 tg        (1003) tg        (1003)        0 2024-04-26 04:42:17.138503 mtdata-0.4.1/tests/
--rw-rw-r--   0 tg        (1003) tg        (1003)     4420 2024-04-26 04:37:28.000000 mtdata-0.4.1/tests/test_bcp47.py
--rw-rw-r--   0 tg        (1003) tg        (1003)     1222 2024-04-26 04:37:28.000000 mtdata-0.4.1/tests/test_cli.py
--rw-rw-r--   0 tg        (1003) tg        (1003)     1282 2024-04-26 04:37:28.000000 mtdata-0.4.1/tests/test_data_sort.py
--rw-rw-r--   0 tg        (1003) tg        (1003)     2355 2024-04-26 04:37:28.000000 mtdata-0.4.1/tests/test_dataset.py
--rw-rw-r--   0 tg        (1003) tg        (1003)     1063 2024-03-05 03:25:14.000000 mtdata-0.4.1/tests/test_entry.py
--rw-rw-r--   0 tg        (1003) tg        (1003)     1169 2024-03-05 03:25:14.000000 mtdata-0.4.1/tests/test_index.py
--rw-rw-r--   0 tg        (1003) tg        (1003)     1179 2024-03-05 03:25:14.000000 mtdata-0.4.1/tests/test_iso_lookup.py
--rw-rw-r--   0 tg        (1003) tg        (1003)     1135 2024-04-26 04:37:28.000000 mtdata-0.4.1/tests/test_pigz.py
--rw-rw-r--   0 tg        (1003) tg        (1003)      700 2024-04-26 03:09:47.000000 mtdata-0.4.1/tests/test_recipe.py
--rw-rw-r--   0 tg        (1003) tg        (1003)      698 2024-03-05 03:25:14.000000 mtdata-0.4.1/tests/test_stats.py
--rw-rw-r--   0 tg        (1003) tg        (1003)     1682 2024-03-05 03:25:14.000000 mtdata-0.4.1/tests/test_tmx.py
+drwxrwxr-x   0 tg        (1003) tg        (1003)        0 2024-05-25 03:22:42.995341 mtdata-0.4.2/
+-rw-rw-r--   0 tg        (1003) tg        (1003)    11357 2024-03-05 03:25:13.000000 mtdata-0.4.2/LICENSE
+-rw-rw-r--   0 tg        (1003) tg        (1003)       91 2024-03-05 03:25:13.000000 mtdata-0.4.2/MANIFEST.in
+-rw-r--r--   0 tg        (1003) tg        (1003)    19208 2024-05-25 03:22:42.995341 mtdata-0.4.2/PKG-INFO
+-rw-rw-r--   0 tg        (1003) tg        (1003)    18137 2024-04-26 04:37:33.000000 mtdata-0.4.2/README.md
+drwxrwxr-x   0 tg        (1003) tg        (1003)        0 2024-05-25 03:22:42.959341 mtdata-0.4.2/mtdata/
+-rw-rw-r--   0 tg        (1003) tg        (1003)      972 2024-05-25 03:21:48.000000 mtdata-0.4.2/mtdata/__init__.py
+-rw-rw-r--   0 tg        (1003) tg        (1003)      341 2024-03-05 03:25:14.000000 mtdata-0.4.2/mtdata/__main__.py
+-rw-rw-r--   0 tg        (1003) tg        (1003)     8726 2024-04-26 04:37:28.000000 mtdata-0.4.2/mtdata/cache.py
+-rw-rw-r--   0 tg        (1003) tg        (1003)    24634 2024-04-26 04:37:28.000000 mtdata-0.4.2/mtdata/data.py
+-rw-rw-r--   0 tg        (1003) tg        (1003)     7067 2024-03-05 03:25:14.000000 mtdata-0.4.2/mtdata/entry.py
+drwxrwxr-x   0 tg        (1003) tg        (1003)        0 2024-05-25 03:22:42.963341 mtdata-0.4.2/mtdata/index/
+-rw-rw-r--   0 tg        (1003) tg        (1003)     8548 2024-03-05 03:25:14.000000 mtdata-0.4.2/mtdata/index/__init__.py
+-rw-rw-r--   0 tg        (1003) tg        (1003)     2698 2024-03-05 03:25:14.000000 mtdata-0.4.2/mtdata/index/ai4bharat.py
+-rw-rw-r--   0 tg        (1003) tg        (1003)      974 2024-03-05 03:25:14.000000 mtdata-0.4.2/mtdata/index/allenai_nllb.py
+-rw-rw-r--   0 tg        (1003) tg        (1003)     2022 2024-03-05 03:25:14.000000 mtdata-0.4.2/mtdata/index/anuvaad.py
+-rw-rw-r--   0 tg        (1003) tg        (1003)     1854 2024-03-05 03:25:14.000000 mtdata-0.4.2/mtdata/index/elrc_share.py
+-rw-rw-r--   0 tg        (1003) tg        (1003)     2572 2024-03-05 03:25:14.000000 mtdata-0.4.2/mtdata/index/eu.py
+-rw-rw-r--   0 tg        (1003) tg        (1003)     5181 2024-03-05 03:25:14.000000 mtdata-0.4.2/mtdata/index/flores.py
+-rw-rw-r--   0 tg        (1003) tg        (1003)     1029 2024-03-05 03:25:14.000000 mtdata-0.4.2/mtdata/index/joshua_indian.py
+-rw-rw-r--   0 tg        (1003) tg        (1003)     1606 2024-03-05 03:25:14.000000 mtdata-0.4.2/mtdata/index/leipzig.py
+-rw-rw-r--   0 tg        (1003) tg        (1003)     6233 2024-03-05 03:25:14.000000 mtdata-0.4.2/mtdata/index/linguatools.py
+-rw-rw-r--   0 tg        (1003) tg        (1003)     1556 2024-03-05 03:25:14.000000 mtdata-0.4.2/mtdata/index/neulab_tedtalks.py
+drwxrwxr-x   0 tg        (1003) tg        (1003)        0 2024-05-25 03:22:42.967341 mtdata-0.4.2/mtdata/index/opus/
+-rw-rw-r--   0 tg        (1003) tg        (1003)       90 2024-03-05 03:25:14.000000 mtdata-0.4.2/mtdata/index/opus/__init__.py
+-rw-rw-r--   0 tg        (1003) tg        (1003)     1213 2024-03-05 03:25:14.000000 mtdata-0.4.2/mtdata/index/opus/crawl_parse.py
+-rw-rw-r--   0 tg        (1003) tg        (1003)   171105 2024-03-05 03:25:14.000000 mtdata-0.4.2/mtdata/index/opus/jw300.py
+-rw-rw-r--   0 tg        (1003) tg        (1003)     2503 2024-03-05 03:25:14.000000 mtdata-0.4.2/mtdata/index/opus/opus100.py
+-rw-rw-r--   0 tg        (1003) tg        (1003)     2457 2024-04-26 04:37:28.000000 mtdata-0.4.2/mtdata/index/opus/opus_index.py
+-rw-rw-r--   0 tg        (1003) tg        (1003)     9441 2024-03-05 03:25:14.000000 mtdata-0.4.2/mtdata/index/other.py
+-rw-rw-r--   0 tg        (1003) tg        (1003)     5773 2024-05-25 03:21:48.000000 mtdata-0.4.2/mtdata/index/paracrawl.py
+-rw-rw-r--   0 tg        (1003) tg        (1003)    27995 2024-04-26 04:37:28.000000 mtdata-0.4.2/mtdata/index/statmt.py
+-rw-rw-r--   0 tg        (1003) tg        (1003)     4114 2024-03-05 03:25:14.000000 mtdata-0.4.2/mtdata/index/tilde.py
+-rw-rw-r--   0 tg        (1003) tg        (1003)      937 2024-03-05 03:25:14.000000 mtdata-0.4.2/mtdata/index/unitednations.py
+-rw-rw-r--   0 tg        (1003) tg        (1003)    10566 2024-03-05 03:25:14.000000 mtdata-0.4.2/mtdata/index/wikimatrix.py
+drwxrwxr-x   0 tg        (1003) tg        (1003)        0 2024-05-25 03:22:42.967341 mtdata-0.4.2/mtdata/iso/
+-rw-rw-r--   0 tg        (1003) tg        (1003)      148 2024-03-05 03:25:14.000000 mtdata-0.4.2/mtdata/iso/__init__.py
+-rw-rw-r--   0 tg        (1003) tg        (1003)     1436 2024-03-05 03:25:14.000000 mtdata-0.4.2/mtdata/iso/__main__.py
+-rw-rw-r--   0 tg        (1003) tg        (1003)   247313 2024-03-05 03:25:14.000000 mtdata-0.4.2/mtdata/iso/bcp47.json
+-rw-rw-r--   0 tg        (1003) tg        (1003)    10188 2024-04-26 04:37:28.000000 mtdata-0.4.2/mtdata/iso/bcp47.py
+-rw-rw-r--   0 tg        (1003) tg        (1003)      433 2024-03-05 03:25:14.000000 mtdata-0.4.2/mtdata/iso/custom.py
+-rw-rw-r--   0 tg        (1003) tg        (1003)     1528 2024-03-05 03:25:14.000000 mtdata-0.4.2/mtdata/iso/iso639.py
+-rw-rw-r--   0 tg        (1003) tg        (1003)     1769 2024-03-05 03:25:14.000000 mtdata-0.4.2/mtdata/iso/iso639_1.py
+-rw-rw-r--   0 tg        (1003) tg        (1003)     9543 2024-03-05 03:25:14.000000 mtdata-0.4.2/mtdata/iso/iso639_2.py
+-rw-rw-r--   0 tg        (1003) tg        (1003)   125322 2024-03-05 03:25:14.000000 mtdata-0.4.2/mtdata/iso/iso639_3.py
+-rw-rw-r--   0 tg        (1003) tg        (1003)    16921 2024-05-25 03:21:48.000000 mtdata-0.4.2/mtdata/main.py
+-rw-rw-r--   0 tg        (1003) tg        (1003)     4150 2024-03-05 03:25:14.000000 mtdata-0.4.2/mtdata/opus_xces.py
+-rw-rw-r--   0 tg        (1003) tg        (1003)     5052 2024-03-05 03:25:14.000000 mtdata-0.4.2/mtdata/parser.py
+-rw-rw-r--   0 tg        (1003) tg        (1003)     2318 2024-04-26 04:37:28.000000 mtdata-0.4.2/mtdata/pigz.py
+drwxrwxr-x   0 tg        (1003) tg        (1003)        0 2024-05-25 03:22:42.967341 mtdata-0.4.2/mtdata/recipe/
+-rw-rw-r--   0 tg        (1003) tg        (1003)     3934 2024-04-26 04:37:28.000000 mtdata-0.4.2/mtdata/recipe/__init__.py
+drwxrwxr-x   0 tg        (1003) tg        (1003)        0 2024-05-25 03:22:42.991341 mtdata-0.4.2/mtdata/resource/
+-rw-rw-r--   0 tg        (1003) tg        (1003)    40277 2024-03-05 03:25:14.000000 mtdata-0.4.2/mtdata/resource/allenai_nllb.json
+-rw-rw-r--   0 tg        (1003) tg        (1003)    17310 2024-03-05 03:25:14.000000 mtdata-0.4.2/mtdata/resource/anuvaad.tsv
+-rw-rw-r--   0 tg        (1003) tg        (1003)   674369 2024-03-05 03:25:14.000000 mtdata-0.4.2/mtdata/resource/elrc_share.tsv
+-rw-rw-r--   0 tg        (1003) tg        (1003)   127368 2024-03-05 03:25:14.000000 mtdata-0.4.2/mtdata/resource/leipzig_de.txt
+-rw-rw-r--   0 tg        (1003) tg        (1003)  3319201 2024-04-26 04:37:28.000000 mtdata-0.4.2/mtdata/resource/opus_index.tsv
+-rw-rw-r--   0 tg        (1003) tg        (1003)     1375 2024-04-26 04:37:28.000000 mtdata-0.4.2/mtdata/resource/recipes.yml
+-rw-rw-r--   0 tg        (1003) tg        (1003)    27633 2024-05-25 03:21:48.000000 mtdata-0.4.2/mtdata/resource/refs.bib
+drwxrwxr-x   0 tg        (1003) tg        (1003)        0 2024-05-25 03:22:42.991341 mtdata-0.4.2/mtdata/scripts/
+-rwxrwxr-x   0 tg        (1003) tg        (1003)     7132 2024-03-05 03:25:14.000000 mtdata-0.4.2/mtdata/scripts/recipe_stats.py
+-rw-rw-r--   0 tg        (1003) tg        (1003)     1278 2024-03-05 03:25:14.000000 mtdata-0.4.2/mtdata/scripts/tsv2xls.py
+-rw-rw-r--   0 tg        (1003) tg        (1003)     3283 2024-04-26 04:37:28.000000 mtdata-0.4.2/mtdata/sgm.py
+-rw-rw-r--   0 tg        (1003) tg        (1003)     4071 2024-03-05 03:25:14.000000 mtdata-0.4.2/mtdata/tmx.py
+-rw-rw-r--   0 tg        (1003) tg        (1003)     8456 2024-04-26 04:37:28.000000 mtdata-0.4.2/mtdata/utils.py
+drwxrwxr-x   0 tg        (1003) tg        (1003)        0 2024-05-25 03:22:42.995341 mtdata-0.4.2/mtdata.egg-info/
+-rw-r--r--   0 tg        (1003) tg        (1003)    19208 2024-05-25 03:22:42.000000 mtdata-0.4.2/mtdata.egg-info/PKG-INFO
+-rw-rw-r--   0 tg        (1003) tg        (1003)     1750 2024-05-25 03:22:42.000000 mtdata-0.4.2/mtdata.egg-info/SOURCES.txt
+-rw-rw-r--   0 tg        (1003) tg        (1003)        1 2024-05-25 03:22:42.000000 mtdata-0.4.2/mtdata.egg-info/dependency_links.txt
+-rw-rw-r--   0 tg        (1003) tg        (1003)      123 2024-05-25 03:22:42.000000 mtdata-0.4.2/mtdata.egg-info/entry_points.txt
+-rw-rw-r--   0 tg        (1003) tg        (1003)        1 2024-05-25 03:22:42.000000 mtdata-0.4.2/mtdata.egg-info/not-zip-safe
+-rw-rw-r--   0 tg        (1003) tg        (1003)       90 2024-05-25 03:22:42.000000 mtdata-0.4.2/mtdata.egg-info/requires.txt
+-rw-rw-r--   0 tg        (1003) tg        (1003)        7 2024-05-25 03:22:42.000000 mtdata-0.4.2/mtdata.egg-info/top_level.txt
+-rw-rw-r--   0 tg        (1003) tg        (1003)       38 2024-05-25 03:22:42.995341 mtdata-0.4.2/setup.cfg
+-rw-rw-r--   0 tg        (1003) tg        (1003)     2209 2024-04-26 04:37:28.000000 mtdata-0.4.2/setup.py
+drwxrwxr-x   0 tg        (1003) tg        (1003)        0 2024-05-25 03:22:42.995341 mtdata-0.4.2/tests/
+-rw-rw-r--   0 tg        (1003) tg        (1003)     4420 2024-04-26 04:37:28.000000 mtdata-0.4.2/tests/test_bcp47.py
+-rw-rw-r--   0 tg        (1003) tg        (1003)     1222 2024-04-26 04:37:28.000000 mtdata-0.4.2/tests/test_cli.py
+-rw-rw-r--   0 tg        (1003) tg        (1003)     1282 2024-04-26 04:37:28.000000 mtdata-0.4.2/tests/test_data_sort.py
+-rw-rw-r--   0 tg        (1003) tg        (1003)     2355 2024-04-26 04:37:28.000000 mtdata-0.4.2/tests/test_dataset.py
+-rw-rw-r--   0 tg        (1003) tg        (1003)     1063 2024-03-05 03:25:14.000000 mtdata-0.4.2/tests/test_entry.py
+-rw-rw-r--   0 tg        (1003) tg        (1003)     1169 2024-03-05 03:25:14.000000 mtdata-0.4.2/tests/test_index.py
+-rw-rw-r--   0 tg        (1003) tg        (1003)     1179 2024-03-05 03:25:14.000000 mtdata-0.4.2/tests/test_iso_lookup.py
+-rw-rw-r--   0 tg        (1003) tg        (1003)     1135 2024-04-26 04:37:28.000000 mtdata-0.4.2/tests/test_pigz.py
+-rw-rw-r--   0 tg        (1003) tg        (1003)      700 2024-04-26 03:09:47.000000 mtdata-0.4.2/tests/test_recipe.py
+-rw-rw-r--   0 tg        (1003) tg        (1003)      698 2024-03-05 03:25:14.000000 mtdata-0.4.2/tests/test_stats.py
+-rw-rw-r--   0 tg        (1003) tg        (1003)     1682 2024-03-05 03:25:14.000000 mtdata-0.4.2/tests/test_tmx.py
```

### Comparing `mtdata-0.4.1/LICENSE` & `mtdata-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mtdata-0.4.1/PKG-INFO` & `mtdata-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mtdata
-Version: 0.4.1
+Version: 0.4.2
 Summary: mtdata is a tool to download datasets for machine translation
 Home-page: https://github.com/thammegowda/mtdata
 Download-URL: https://github.com/thammegowda/mtdata
 Author: Thamme Gowda
 Author-email: tgowdan@gmail.com
 Keywords: machine translation,datasets,NLP,natural language processing,computational linguistics
 Platform: any
@@ -16,14 +16,19 @@
 Classifier: Topic :: Text Processing :: Filters
 Classifier: Topic :: Text Processing :: Linguistic
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests==2.31.0
+Requires-Dist: enlighten==1.10.1
+Requires-Dist: portalocker==2.3.0
+Requires-Dist: pybtex==0.24.0
+Requires-Dist: ruamel.yaml>=0.17.10
 
 # MTData
 [![image](http://img.shields.io/pypi/v/mtdata.svg)](https://pypi.python.org/pypi/mtdata/)
 ![Travis (.com)](https://img.shields.io/travis/com/thammegowda/mtdata?style=plastic)
 
 MTData automates the collection and preparation of machine translation (MT) datasets.
 It provides CLI and python APIs, which can be used for preparing MT experiments.
```

### Comparing `mtdata-0.4.1/README.md` & `mtdata-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `mtdata-0.4.1/mtdata/__init__.py` & `mtdata-0.4.2/mtdata/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 #
 # Author: Thamme Gowda [tg (at) isi (dot) edu] 
 # Created: 4/4/20
 
 
-__version__ = '0.4.1'
+__version__ = '0.4.2'
 __description__ = 'mtdata is a tool to download datasets for machine translation'
 __author__ = 'Thamme Gowda'
 
 import logging as log
 from pathlib import Path
 import os
 import enlighten
```

### Comparing `mtdata-0.4.1/mtdata/cache.py` & `mtdata-0.4.2/mtdata/cache.py`

 * *Files identical despite different names*

### Comparing `mtdata-0.4.1/mtdata/data.py` & `mtdata-0.4.2/mtdata/data.py`

 * *Files identical despite different names*

### Comparing `mtdata-0.4.1/mtdata/entry.py` & `mtdata-0.4.2/mtdata/entry.py`

 * *Files identical despite different names*

### Comparing `mtdata-0.4.1/mtdata/index/__init__.py` & `mtdata-0.4.2/mtdata/index/__init__.py`

 * *Files identical despite different names*

### Comparing `mtdata-0.4.1/mtdata/index/ai4bharat.py` & `mtdata-0.4.2/mtdata/index/ai4bharat.py`

 * *Files identical despite different names*

### Comparing `mtdata-0.4.1/mtdata/index/allenai_nllb.py` & `mtdata-0.4.2/mtdata/index/allenai_nllb.py`

 * *Files identical despite different names*

### Comparing `mtdata-0.4.1/mtdata/index/anuvaad.py` & `mtdata-0.4.2/mtdata/index/anuvaad.py`

 * *Files identical despite different names*

### Comparing `mtdata-0.4.1/mtdata/index/elrc_share.py` & `mtdata-0.4.2/mtdata/index/elrc_share.py`

 * *Files identical despite different names*

### Comparing `mtdata-0.4.1/mtdata/index/eu.py` & `mtdata-0.4.2/mtdata/index/eu.py`

 * *Files identical despite different names*

### Comparing `mtdata-0.4.1/mtdata/index/flores.py` & `mtdata-0.4.2/mtdata/index/flores.py`

 * *Files identical despite different names*

### Comparing `mtdata-0.4.1/mtdata/index/joshua_indian.py` & `mtdata-0.4.2/mtdata/index/joshua_indian.py`

 * *Files identical despite different names*

### Comparing `mtdata-0.4.1/mtdata/index/leipzig.py` & `mtdata-0.4.2/mtdata/index/leipzig.py`

 * *Files identical despite different names*

### Comparing `mtdata-0.4.1/mtdata/index/linguatools.py` & `mtdata-0.4.2/mtdata/index/linguatools.py`

 * *Files identical despite different names*

### Comparing `mtdata-0.4.1/mtdata/index/neulab_tedtalks.py` & `mtdata-0.4.2/mtdata/index/neulab_tedtalks.py`

 * *Files identical despite different names*

### Comparing `mtdata-0.4.1/mtdata/index/opus/crawl_parse.py` & `mtdata-0.4.2/mtdata/index/opus/crawl_parse.py`

 * *Files identical despite different names*

### Comparing `mtdata-0.4.1/mtdata/index/opus/jw300.py` & `mtdata-0.4.2/mtdata/index/opus/jw300.py`

 * *Files identical despite different names*

### Comparing `mtdata-0.4.1/mtdata/index/opus/opus100.py` & `mtdata-0.4.2/mtdata/index/opus/opus100.py`

 * *Files identical despite different names*

### Comparing `mtdata-0.4.1/mtdata/index/opus/opus_index.py` & `mtdata-0.4.2/mtdata/index/opus/opus_index.py`

 * *Files identical despite different names*

### Comparing `mtdata-0.4.1/mtdata/index/other.py` & `mtdata-0.4.2/mtdata/index/other.py`

 * *Files identical despite different names*

### Comparing `mtdata-0.4.1/mtdata/index/paracrawl.py` & `mtdata-0.4.2/mtdata/index/paracrawl.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,20 +78,26 @@
         cite=cite, ext='tsv.gz'))
 
     index.add_entry(Entry(
         did=DatasetId(group=group_id, name=f'paracrawl', version='1_bonus', langs=('en', 'uk')),
         url=f'{URL_PREFIX}/bonus/en-uk-v1.txt.gz',
         cite=cite, ext='tsv.gz'))
 
-    # Japanese-English paracrawl (5.1) used by WMT20 and WMT21
+    # Japanese-English paracrawl (5.1) used by WMT20 ...
     for version, cols in [('2', (2, 3)), ('3', (3, 4))]:
         ent = Entry(did=DatasetId(group='KECL', name=f'paracrawl', version=version, langs=('eng', 'jpn')),
                     in_paths=['en-ja/en-ja.bicleaner05.txt'], in_ext='tsv', cols=cols, cite='',
                     url=f'http://www.kecl.ntt.co.jp/icl/lirg/jparacrawl/release/{version}.0/bitext/en-ja.tar.gz')
         index.add_entry(ent)
-        
-        # JParaCrawl Chinese-Japanese, only version 2 is available
-        if version == '2':
-            ent = Entry(did=DatasetId(group='KECL', name=f'paracrawl', version=version, langs=('zho', 'jpn')),
-                            in_paths=['zh-ja/zh-ja.bicleaner05.txt'], in_ext='tsv', cols=cols, cite='',
-                            url=f'http://www.kecl.ntt.co.jp/icl/lirg/jparacrawl/release/{version}.0/bitext/zh-ja.tar.gz')
-            index.add_entry(ent)
+
+    # JParaCrawl Chinese-Japanese, v2: cols=2,3
+    ent = Entry(did=DatasetId(group='KECL', name=f'paracrawl', version='2', langs=('zho', 'jpn')),
+                    in_paths=['zh-ja/zh-ja.bicleaner05.txt'], filename='jparacrawl-2.0-zh-ja.tar.gz',
+                    in_ext='tsv', cols=(2, 3), cite=('morishita-etal-2022-jparacrawl',),
+                    url=f'http://www.kecl.ntt.co.jp/icl/lirg/jparacrawl/release/zh/2.0/bitext/zh-ja.tar.gz')
+    index.add_entry(ent)
+    # v2wmt24: columns=(3, 4)
+    ent = Entry(did=DatasetId(group='KECL', name=f'paracrawl', version=f'2wmt24', langs=('zho', 'jpn')),
+                    in_paths=['zh-ja/zh-ja.crowdsourcing_b05l07.txt'], filename='jparacrawl-2.0-zh-ja.tar.gz',
+                    in_ext='tsv', cols=(3, 4), cite=('nagata2024japanesechinese',),
+                    url=f'http://www.kecl.ntt.co.jp/icl/lirg/jparacrawl/release/zh/2.0/bitext/zh-ja.tar.gz')
+    index.add_entry(ent)
```

### Comparing `mtdata-0.4.1/mtdata/index/statmt.py` & `mtdata-0.4.2/mtdata/index/statmt.py`

 * *Files identical despite different names*

### Comparing `mtdata-0.4.1/mtdata/index/tilde.py` & `mtdata-0.4.2/mtdata/index/tilde.py`

 * *Files identical despite different names*

### Comparing `mtdata-0.4.1/mtdata/index/unitednations.py` & `mtdata-0.4.2/mtdata/index/unitednations.py`

 * *Files identical despite different names*

### Comparing `mtdata-0.4.1/mtdata/index/wikimatrix.py` & `mtdata-0.4.2/mtdata/index/wikimatrix.py`

 * *Files identical despite different names*

### Comparing `mtdata-0.4.1/mtdata/iso/__main__.py` & `mtdata-0.4.2/mtdata/iso/__main__.py`

 * *Files identical despite different names*

### Comparing `mtdata-0.4.1/mtdata/iso/bcp47.json` & `mtdata-0.4.2/mtdata/iso/bcp47.json`

 * *Files identical despite different names*

### Comparing `mtdata-0.4.1/mtdata/iso/bcp47.py` & `mtdata-0.4.2/mtdata/iso/bcp47.py`

 * *Files identical despite different names*

### Comparing `mtdata-0.4.1/mtdata/iso/iso639.py` & `mtdata-0.4.2/mtdata/iso/iso639.py`

 * *Files identical despite different names*

### Comparing `mtdata-0.4.1/mtdata/iso/iso639_1.py` & `mtdata-0.4.2/mtdata/iso/iso639_1.py`

 * *Files identical despite different names*

### Comparing `mtdata-0.4.1/mtdata/iso/iso639_2.py` & `mtdata-0.4.2/mtdata/iso/iso639_2.py`

 * *Files identical despite different names*

### Comparing `mtdata-0.4.1/mtdata/iso/iso639_3.py` & `mtdata-0.4.2/mtdata/iso/iso639_3.py`

 * *Files identical despite different names*

### Comparing `mtdata-0.4.1/mtdata/main.py` & `mtdata-0.4.2/mtdata/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,16 @@
     from mtdata.data import INDEX, Cache, Parser
     assert did in INDEX
     entry = INDEX[did]
     cache = Cache(CACHE_DIR)
     path = cache.get_entry(entry)
     parser = Parser(path, ext=entry.in_ext or None, ent=entry)
     count = 0
-    for rec in parser.read_segs():
+    all_segs = parser.read_segs()
+    for rec in all_segs:
         if isinstance(rec, (list, tuple)):
             rec = (col.replace(delim, ' ').replace('\n', ' ') for col in rec)
             rec = delim.join(rec)
         print(rec)
         count += 1
     log.info(f'Total rows={count:,}')
 
@@ -319,14 +320,16 @@
         cached_index_file.rename(bak_file)
     if args.task == 'list':
         list_data(args.langs, args.names, not_names=args.not_names, full=args.full,
                   groups=args.groups, not_groups=args.not_groups, id_only=args.id)
     elif args.task == 'get':
         get_data(**vars(args))
     elif args.task == 'echo':
+        # disable progress bar for echo; it sometimes insert new lines in the output
+        pbar_man.enabled = False
         echo_data(did=args.dataset_id)
     elif args.task == 'list-recipe':
         list_recipes(id_only=args.id, format=args.format)
     elif args.task == 'get-recipe':
         get_recipe(**vars(args))
     elif args.task == 'stats':
         show_stats(*args.did, quick=args.quick)
```

### Comparing `mtdata-0.4.1/mtdata/opus_xces.py` & `mtdata-0.4.2/mtdata/opus_xces.py`

 * *Files identical despite different names*

### Comparing `mtdata-0.4.1/mtdata/parser.py` & `mtdata-0.4.2/mtdata/parser.py`

 * *Files identical despite different names*

### Comparing `mtdata-0.4.1/mtdata/pigz.py` & `mtdata-0.4.2/mtdata/pigz.py`

 * *Files identical despite different names*

### Comparing `mtdata-0.4.1/mtdata/recipe/__init__.py` & `mtdata-0.4.2/mtdata/recipe/__init__.py`

 * *Files identical despite different names*

### Comparing `mtdata-0.4.1/mtdata/resource/allenai_nllb.json` & `mtdata-0.4.2/mtdata/resource/allenai_nllb.json`

 * *Files identical despite different names*

### Comparing `mtdata-0.4.1/mtdata/resource/anuvaad.tsv` & `mtdata-0.4.2/mtdata/resource/anuvaad.tsv`

 * *Files identical despite different names*

### Comparing `mtdata-0.4.1/mtdata/resource/elrc_share.tsv` & `mtdata-0.4.2/mtdata/resource/elrc_share.tsv`

 * *Files identical despite different names*

### Comparing `mtdata-0.4.1/mtdata/resource/leipzig_de.txt` & `mtdata-0.4.2/mtdata/resource/leipzig_de.txt`

 * *Files identical despite different names*

### Comparing `mtdata-0.4.1/mtdata/resource/opus_index.tsv` & `mtdata-0.4.2/mtdata/resource/opus_index.tsv`

 * *Files identical despite different names*

### Comparing `mtdata-0.4.1/mtdata/resource/recipes.yml` & `mtdata-0.4.2/mtdata/resource/recipes.yml`

 * *Files identical despite different names*

### Comparing `mtdata-0.4.1/mtdata/resource/refs.bib` & `mtdata-0.4.2/mtdata/resource/refs.bib`

 * *Files 1% similar despite different names*

```diff
@@ -689,8 +689,34 @@
     booktitle = "Proceedings of the Eighth International Conference on Language Resources and Evaluation ({LREC}'12)",
     month = may,
     year = "2012",
     address = "Istanbul, Turkey",
     publisher = "European Language Resources Association (ELRA)",
     url = "http://www.lrec-conf.org/proceedings/lrec2012/pdf/327_Paper.pdf",
     pages = "759--765",
-}
+}
+
+%%% Japanese paracrawl
+@inproceedings{morishita-etal-2022-jparacrawl,
+    title = "{JP}ara{C}rawl v3.0: A Large-scale {E}nglish-{J}apanese Parallel Corpus",
+    author = "Morishita, Makoto  and
+      Chousa, Katsuki  and
+      Suzuki, Jun  and
+      Nagata, Masaaki",
+    booktitle = "Proceedings of the Thirteenth Language Resources and Evaluation Conference",
+    month = jun,
+    year = "2022",
+    address = "Marseille, France",
+    publisher = "European Language Resources Association",
+    url = "https://aclanthology.org/2022.lrec-1.721",
+    pages = "6704--6710",
+}
+
+
+@misc{nagata2024japanesechinese,
+    title={A Japanese-Chinese Parallel Corpus Using Crowdsourcing for Web Mining},
+    author={Masaaki Nagata and Makoto Morishita and Katsuki Chousa and Norihito Yasuda},
+    year={2024},
+    eprint={2405.09017},
+    archivePrefix={arXiv},
+    primaryClass={cs.CL},
+}
```

### Comparing `mtdata-0.4.1/mtdata/scripts/recipe_stats.py` & `mtdata-0.4.2/mtdata/scripts/recipe_stats.py`

 * *Files identical despite different names*

### Comparing `mtdata-0.4.1/mtdata/scripts/tsv2xls.py` & `mtdata-0.4.2/mtdata/scripts/tsv2xls.py`

 * *Files identical despite different names*

### Comparing `mtdata-0.4.1/mtdata/sgm.py` & `mtdata-0.4.2/mtdata/sgm.py`

 * *Files identical despite different names*

### Comparing `mtdata-0.4.1/mtdata/tmx.py` & `mtdata-0.4.2/mtdata/tmx.py`

 * *Files identical despite different names*

### Comparing `mtdata-0.4.1/mtdata/utils.py` & `mtdata-0.4.2/mtdata/utils.py`

 * *Files identical despite different names*

### Comparing `mtdata-0.4.1/mtdata.egg-info/PKG-INFO` & `mtdata-0.4.2/mtdata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mtdata
-Version: 0.4.1
+Version: 0.4.2
 Summary: mtdata is a tool to download datasets for machine translation
 Home-page: https://github.com/thammegowda/mtdata
 Download-URL: https://github.com/thammegowda/mtdata
 Author: Thamme Gowda
 Author-email: tgowdan@gmail.com
 Keywords: machine translation,datasets,NLP,natural language processing,computational linguistics
 Platform: any
@@ -16,14 +16,19 @@
 Classifier: Topic :: Text Processing :: Filters
 Classifier: Topic :: Text Processing :: Linguistic
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests==2.31.0
+Requires-Dist: enlighten==1.10.1
+Requires-Dist: portalocker==2.3.0
+Requires-Dist: pybtex==0.24.0
+Requires-Dist: ruamel.yaml>=0.17.10
 
 # MTData
 [![image](http://img.shields.io/pypi/v/mtdata.svg)](https://pypi.python.org/pypi/mtdata/)
 ![Travis (.com)](https://img.shields.io/travis/com/thammegowda/mtdata?style=plastic)
 
 MTData automates the collection and preparation of machine translation (MT) datasets.
 It provides CLI and python APIs, which can be used for preparing MT experiments.
```

### Comparing `mtdata-0.4.1/mtdata.egg-info/SOURCES.txt` & `mtdata-0.4.2/mtdata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mtdata-0.4.1/setup.py` & `mtdata-0.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `mtdata-0.4.1/tests/test_bcp47.py` & `mtdata-0.4.2/tests/test_bcp47.py`

 * *Files identical despite different names*

### Comparing `mtdata-0.4.1/tests/test_cli.py` & `mtdata-0.4.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `mtdata-0.4.1/tests/test_data_sort.py` & `mtdata-0.4.2/tests/test_data_sort.py`

 * *Files identical despite different names*

### Comparing `mtdata-0.4.1/tests/test_dataset.py` & `mtdata-0.4.2/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `mtdata-0.4.1/tests/test_entry.py` & `mtdata-0.4.2/tests/test_entry.py`

 * *Files identical despite different names*

### Comparing `mtdata-0.4.1/tests/test_index.py` & `mtdata-0.4.2/tests/test_index.py`

 * *Files identical despite different names*

### Comparing `mtdata-0.4.1/tests/test_iso_lookup.py` & `mtdata-0.4.2/tests/test_iso_lookup.py`

 * *Files identical despite different names*

### Comparing `mtdata-0.4.1/tests/test_pigz.py` & `mtdata-0.4.2/tests/test_pigz.py`

 * *Files identical despite different names*

### Comparing `mtdata-0.4.1/tests/test_recipe.py` & `mtdata-0.4.2/tests/test_recipe.py`

 * *Files identical despite different names*

### Comparing `mtdata-0.4.1/tests/test_stats.py` & `mtdata-0.4.2/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `mtdata-0.4.1/tests/test_tmx.py` & `mtdata-0.4.2/tests/test_tmx.py`

 * *Files identical despite different names*

