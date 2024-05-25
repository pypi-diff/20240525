# Comparing `tmp/Toisto-0.8.2.tar.gz` & `tmp/Toisto-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Toisto-0.8.2.tar", last modified: Sun Feb 19 18:22:55 2023, max compression
+gzip compressed data, was "Toisto-0.9.0.tar", last modified: Tue Mar 21 19:46:39 2023, max compression
```

## Comparing `Toisto-0.8.2.tar` & `Toisto-0.9.0.tar`

### file list

```diff
@@ -1,90 +1,91 @@
-drwxr-xr-x   0 fniessink   (501) staff       (20)        0 2023-02-19 18:22:55.882748 Toisto-0.8.2/
--rw-r--r--   0 fniessink   (501) staff       (20)    11357 2022-10-02 11:54:10.000000 Toisto-0.8.2/LICENSE
--rw-r--r--   0 fniessink   (501) staff       (20)     8343 2023-02-19 18:22:55.882396 Toisto-0.8.2/PKG-INFO
--rw-r--r--   0 fniessink   (501) staff       (20)     7334 2023-02-11 17:02:34.000000 Toisto-0.8.2/README.md
--rw-r--r--   0 fniessink   (501) staff       (20)     2210 2023-02-19 17:48:46.000000 Toisto-0.8.2/pyproject.toml
--rw-r--r--   0 fniessink   (501) staff       (20)       38 2023-02-19 18:22:55.882818 Toisto-0.8.2/setup.cfg
-drwxr-xr-x   0 fniessink   (501) staff       (20)        0 2023-02-19 18:22:55.843755 Toisto-0.8.2/src/
-drwxr-xr-x   0 fniessink   (501) staff       (20)        0 2023-02-19 18:22:55.845969 Toisto-0.8.2/src/Toisto.egg-info/
--rw-r--r--   0 fniessink   (501) staff       (20)     8343 2023-02-19 18:22:55.000000 Toisto-0.8.2/src/Toisto.egg-info/PKG-INFO
--rw-r--r--   0 fniessink   (501) staff       (20)     2210 2023-02-19 18:22:55.000000 Toisto-0.8.2/src/Toisto.egg-info/SOURCES.txt
--rw-r--r--   0 fniessink   (501) staff       (20)        1 2023-02-19 18:22:55.000000 Toisto-0.8.2/src/Toisto.egg-info/dependency_links.txt
--rw-r--r--   0 fniessink   (501) staff       (20)       43 2023-02-19 18:22:55.000000 Toisto-0.8.2/src/Toisto.egg-info/entry_points.txt
--rw-r--r--   0 fniessink   (501) staff       (20)      245 2023-02-19 18:22:55.000000 Toisto-0.8.2/src/Toisto.egg-info/requires.txt
--rw-r--r--   0 fniessink   (501) staff       (20)       24 2023-02-19 18:22:55.000000 Toisto-0.8.2/src/Toisto.egg-info/top_level.txt
-drwxr-xr-x   0 fniessink   (501) staff       (20)        0 2023-02-19 18:22:55.846195 Toisto-0.8.2/src/languages/
--rw-r--r--   0 fniessink   (501) staff       (20)   720189 2023-02-19 17:48:46.000000 Toisto-0.8.2/src/languages/iana-language-subtag-registry.txt
-drwxr-xr-x   0 fniessink   (501) staff       (20)        0 2023-02-19 18:22:55.848791 Toisto-0.8.2/src/toisto/
--rw-r--r--   0 fniessink   (501) staff       (20)        0 2022-10-05 17:24:02.000000 Toisto-0.8.2/src/toisto/__init__.py
--rw-r--r--   0 fniessink   (501) staff       (20)     1437 2023-02-18 20:20:36.000000 Toisto-0.8.2/src/toisto/app.py
-drwxr-xr-x   0 fniessink   (501) staff       (20)        0 2023-02-19 18:22:55.850131 Toisto-0.8.2/src/toisto/command/
--rw-r--r--   0 fniessink   (501) staff       (20)        0 2023-01-31 17:17:41.000000 Toisto-0.8.2/src/toisto/command/__init__.py
--rw-r--r--   0 fniessink   (501) staff       (20)     1945 2023-01-31 17:17:41.000000 Toisto-0.8.2/src/toisto/command/practice.py
--rw-r--r--   0 fniessink   (501) staff       (20)     2162 2023-02-19 17:48:46.000000 Toisto-0.8.2/src/toisto/command/show_progress.py
--rw-r--r--   0 fniessink   (501) staff       (20)     1727 2023-02-19 17:48:46.000000 Toisto-0.8.2/src/toisto/command/show_topics.py
--rw-r--r--   0 fniessink   (501) staff       (20)     1143 2023-02-19 17:48:46.000000 Toisto-0.8.2/src/toisto/metadata.py
-drwxr-xr-x   0 fniessink   (501) staff       (20)        0 2023-02-19 18:22:55.850409 Toisto-0.8.2/src/toisto/model/
--rw-r--r--   0 fniessink   (501) staff       (20)        0 2023-01-31 17:17:41.000000 Toisto-0.8.2/src/toisto/model/__init__.py
-drwxr-xr-x   0 fniessink   (501) staff       (20)        0 2023-02-19 18:22:55.867281 Toisto-0.8.2/src/toisto/model/language/
--rw-r--r--   0 fniessink   (501) staff       (20)       89 2023-02-19 17:48:46.000000 Toisto-0.8.2/src/toisto/model/language/__init__.py
--rw-r--r--   0 fniessink   (501) staff       (20)      947 2023-01-31 17:17:41.000000 Toisto-0.8.2/src/toisto/model/language/cefr.py
--rw-r--r--   0 fniessink   (501) staff       (20)     5161 2023-02-19 17:48:46.000000 Toisto-0.8.2/src/toisto/model/language/concept.py
--rw-r--r--   0 fniessink   (501) staff       (20)     5188 2023-02-19 17:48:46.000000 Toisto-0.8.2/src/toisto/model/language/concept_factory.py
--rw-r--r--   0 fniessink   (501) staff       (20)      678 2023-02-11 17:02:34.000000 Toisto-0.8.2/src/toisto/model/language/grammar.py
--rw-r--r--   0 fniessink   (501) staff       (20)      276 2023-02-19 17:48:46.000000 Toisto-0.8.2/src/toisto/model/language/iana_language_subtag_registry.py
--rw-r--r--   0 fniessink   (501) staff       (20)     1218 2023-01-31 17:17:41.000000 Toisto-0.8.2/src/toisto/model/language/label.py
-drwxr-xr-x   0 fniessink   (501) staff       (20)        0 2023-02-19 18:22:55.869710 Toisto-0.8.2/src/toisto/model/quiz/
--rw-r--r--   0 fniessink   (501) staff       (20)        0 2023-01-31 17:17:41.000000 Toisto-0.8.2/src/toisto/model/quiz/__init__.py
--rw-r--r--   0 fniessink   (501) staff       (20)      459 2023-01-15 18:30:50.000000 Toisto-0.8.2/src/toisto/model/quiz/match.py
--rw-r--r--   0 fniessink   (501) staff       (20)     4245 2023-02-18 17:38:39.000000 Toisto-0.8.2/src/toisto/model/quiz/progress.py
--rw-r--r--   0 fniessink   (501) staff       (20)     5721 2023-02-19 17:48:46.000000 Toisto-0.8.2/src/toisto/model/quiz/quiz.py
--rw-r--r--   0 fniessink   (501) staff       (20)     6257 2023-02-19 17:48:46.000000 Toisto-0.8.2/src/toisto/model/quiz/quiz_factory.py
--rw-r--r--   0 fniessink   (501) staff       (20)     2872 2023-02-18 17:38:39.000000 Toisto-0.8.2/src/toisto/model/quiz/retention.py
--rw-r--r--   0 fniessink   (501) staff       (20)      911 2023-02-18 17:38:39.000000 Toisto-0.8.2/src/toisto/model/quiz/topic.py
-drwxr-xr-x   0 fniessink   (501) staff       (20)        0 2023-02-19 18:22:55.871492 Toisto-0.8.2/src/toisto/persistence/
--rw-r--r--   0 fniessink   (501) staff       (20)        0 2023-01-31 17:17:41.000000 Toisto-0.8.2/src/toisto/persistence/__init__.py
--rw-r--r--   0 fniessink   (501) staff       (20)     4210 2023-02-19 17:48:46.000000 Toisto-0.8.2/src/toisto/persistence/config.py
--rw-r--r--   0 fniessink   (501) staff       (20)     1490 2023-02-19 17:48:46.000000 Toisto-0.8.2/src/toisto/persistence/iana_language_subtag_registry.py
--rw-r--r--   0 fniessink   (501) staff       (20)      741 2023-02-11 16:40:37.000000 Toisto-0.8.2/src/toisto/persistence/json_file.py
--rw-r--r--   0 fniessink   (501) staff       (20)     1137 2023-02-11 17:02:34.000000 Toisto-0.8.2/src/toisto/persistence/progress.py
--rw-r--r--   0 fniessink   (501) staff       (20)     1946 2023-02-19 17:48:46.000000 Toisto-0.8.2/src/toisto/persistence/topics.py
--rw-r--r--   0 fniessink   (501) staff       (20)      491 2023-02-11 17:02:34.000000 Toisto-0.8.2/src/toisto/tools.py
-drwxr-xr-x   0 fniessink   (501) staff       (20)        0 2023-02-19 18:22:55.873356 Toisto-0.8.2/src/toisto/ui/
--rw-r--r--   0 fniessink   (501) staff       (20)        0 2022-11-08 20:37:12.000000 Toisto-0.8.2/src/toisto/ui/__init__.py
--rw-r--r--   0 fniessink   (501) staff       (20)     5483 2023-02-19 17:48:46.000000 Toisto-0.8.2/src/toisto/ui/cli.py
--rw-r--r--   0 fniessink   (501) staff       (20)     1130 2023-01-31 17:17:41.000000 Toisto-0.8.2/src/toisto/ui/dictionary.py
--rw-r--r--   0 fniessink   (501) staff       (20)     1510 2023-01-31 17:17:41.000000 Toisto-0.8.2/src/toisto/ui/diff.py
--rw-r--r--   0 fniessink   (501) staff       (20)      732 2023-01-31 17:17:41.000000 Toisto-0.8.2/src/toisto/ui/format.py
--rw-r--r--   0 fniessink   (501) staff       (20)     1550 2023-01-31 17:17:41.000000 Toisto-0.8.2/src/toisto/ui/speech.py
--rw-r--r--   0 fniessink   (501) staff       (20)     3615 2023-02-18 17:38:39.000000 Toisto-0.8.2/src/toisto/ui/text.py
-drwxr-xr-x   0 fniessink   (501) staff       (20)        0 2023-02-19 18:22:55.882019 Toisto-0.8.2/src/topics/
--rw-r--r--   0 fniessink   (501) staff       (20)      153 2023-01-31 17:17:41.000000 Toisto-0.8.2/src/topics/adverbs.json
--rw-r--r--   0 fniessink   (501) staff       (20)     8392 2023-02-18 17:38:39.000000 Toisto-0.8.2/src/topics/animals.json
--rw-r--r--   0 fniessink   (501) staff       (20)    11594 2023-02-18 17:38:39.000000 Toisto-0.8.2/src/topics/auxiliary_verbs.json
--rw-r--r--   0 fniessink   (501) staff       (20)     7638 2023-02-18 17:38:39.000000 Toisto-0.8.2/src/topics/body.json
--rw-r--r--   0 fniessink   (501) staff       (20)    10590 2023-02-18 17:38:39.000000 Toisto-0.8.2/src/topics/city.json
--rw-r--r--   0 fniessink   (501) staff       (20)     6376 2023-02-18 17:38:39.000000 Toisto-0.8.2/src/topics/clothes.json
--rw-r--r--   0 fniessink   (501) staff       (20)     7098 2023-02-18 17:38:39.000000 Toisto-0.8.2/src/topics/colors.json
--rw-r--r--   0 fniessink   (501) staff       (20)     8848 2023-02-18 17:38:39.000000 Toisto-0.8.2/src/topics/counting.json
--rw-r--r--   0 fniessink   (501) staff       (20)     2589 2023-02-18 17:38:39.000000 Toisto-0.8.2/src/topics/countries.json
--rw-r--r--   0 fniessink   (501) staff       (20)     7325 2023-02-18 17:38:39.000000 Toisto-0.8.2/src/topics/days.json
--rw-r--r--   0 fniessink   (501) staff       (20)    17340 2023-02-11 17:02:34.000000 Toisto-0.8.2/src/topics/degrees_of_comparison.json
--rw-r--r--   0 fniessink   (501) staff       (20)    13101 2023-02-18 17:38:39.000000 Toisto-0.8.2/src/topics/family.json
--rw-r--r--   0 fniessink   (501) staff       (20)    15164 2023-02-18 17:38:39.000000 Toisto-0.8.2/src/topics/food.json
--rw-r--r--   0 fniessink   (501) staff       (20)     3952 2023-02-18 17:38:39.000000 Toisto-0.8.2/src/topics/furniture.json
--rw-r--r--   0 fniessink   (501) staff       (20)     4805 2023-02-18 17:38:39.000000 Toisto-0.8.2/src/topics/greetings.json
--rw-r--r--   0 fniessink   (501) staff       (20)     4224 2023-02-18 17:38:39.000000 Toisto-0.8.2/src/topics/health.json
--rw-r--r--   0 fniessink   (501) staff       (20)     5539 2023-02-18 17:38:39.000000 Toisto-0.8.2/src/topics/holidays.json
--rw-r--r--   0 fniessink   (501) staff       (20)     6949 2023-02-18 17:38:39.000000 Toisto-0.8.2/src/topics/house.json
--rw-r--r--   0 fniessink   (501) staff       (20)     4676 2023-02-18 17:38:39.000000 Toisto-0.8.2/src/topics/interrogative_pronouns.json
--rw-r--r--   0 fniessink   (501) staff       (20)     4469 2023-01-31 17:17:41.000000 Toisto-0.8.2/src/topics/languages.json
--rw-r--r--   0 fniessink   (501) staff       (20)     4621 2023-02-18 17:38:39.000000 Toisto-0.8.2/src/topics/months.json
--rw-r--r--   0 fniessink   (501) staff       (20)     8228 2023-02-18 17:38:39.000000 Toisto-0.8.2/src/topics/nature.json
--rw-r--r--   0 fniessink   (501) staff       (20)      382 2023-01-31 17:17:41.000000 Toisto-0.8.2/src/topics/objects.json
--rw-r--r--   0 fniessink   (501) staff       (20)     4876 2023-02-18 17:38:39.000000 Toisto-0.8.2/src/topics/possessive_adjectives.json
--rw-r--r--   0 fniessink   (501) staff       (20)     5751 2023-02-18 17:38:39.000000 Toisto-0.8.2/src/topics/seasons.json
--rw-r--r--   0 fniessink   (501) staff       (20)    23034 2023-02-18 17:38:39.000000 Toisto-0.8.2/src/topics/sentence_types.json
--rw-r--r--   0 fniessink   (501) staff       (20)    10023 2023-02-18 17:38:39.000000 Toisto-0.8.2/src/topics/time.json
--rw-r--r--   0 fniessink   (501) staff       (20)      376 2023-01-31 17:17:41.000000 Toisto-0.8.2/src/topics/transport.json
--rw-r--r--   0 fniessink   (501) staff       (20)    69731 2023-01-31 17:17:41.000000 Toisto-0.8.2/src/topics/verbs.json
--rw-r--r--   0 fniessink   (501) staff       (20)     6301 2023-02-18 17:38:39.000000 Toisto-0.8.2/src/topics/weather.json
+drwxr-xr-x   0 fniessink   (501) staff       (20)        0 2023-03-21 19:46:39.060768 Toisto-0.9.0/
+-rw-r--r--   0 fniessink   (501) staff       (20)    11357 2022-10-02 11:54:10.000000 Toisto-0.9.0/LICENSE
+-rw-r--r--   0 fniessink   (501) staff       (20)     8520 2023-03-21 19:46:39.058730 Toisto-0.9.0/PKG-INFO
+-rw-r--r--   0 fniessink   (501) staff       (20)     7511 2023-03-21 19:44:12.000000 Toisto-0.9.0/README.md
+-rw-r--r--   0 fniessink   (501) staff       (20)     2236 2023-03-21 19:44:12.000000 Toisto-0.9.0/pyproject.toml
+-rw-r--r--   0 fniessink   (501) staff       (20)       38 2023-03-21 19:46:39.060866 Toisto-0.9.0/setup.cfg
+drwxr-xr-x   0 fniessink   (501) staff       (20)        0 2023-03-21 19:46:39.028800 Toisto-0.9.0/src/
+drwxr-xr-x   0 fniessink   (501) staff       (20)        0 2023-03-21 19:46:39.034800 Toisto-0.9.0/src/Toisto.egg-info/
+-rw-r--r--   0 fniessink   (501) staff       (20)     8520 2023-03-21 19:46:39.000000 Toisto-0.9.0/src/Toisto.egg-info/PKG-INFO
+-rw-r--r--   0 fniessink   (501) staff       (20)     2234 2023-03-21 19:46:39.000000 Toisto-0.9.0/src/Toisto.egg-info/SOURCES.txt
+-rw-r--r--   0 fniessink   (501) staff       (20)        1 2023-03-21 19:46:39.000000 Toisto-0.9.0/src/Toisto.egg-info/dependency_links.txt
+-rw-r--r--   0 fniessink   (501) staff       (20)       43 2023-03-21 19:46:39.000000 Toisto-0.9.0/src/Toisto.egg-info/entry_points.txt
+-rw-r--r--   0 fniessink   (501) staff       (20)      262 2023-03-21 19:46:39.000000 Toisto-0.9.0/src/Toisto.egg-info/requires.txt
+-rw-r--r--   0 fniessink   (501) staff       (20)       24 2023-03-21 19:46:39.000000 Toisto-0.9.0/src/Toisto.egg-info/top_level.txt
+drwxr-xr-x   0 fniessink   (501) staff       (20)        0 2023-03-21 19:46:39.035114 Toisto-0.9.0/src/languages/
+-rw-r--r--   0 fniessink   (501) staff       (20)   720189 2023-03-03 20:45:55.000000 Toisto-0.9.0/src/languages/iana-language-subtag-registry.txt
+drwxr-xr-x   0 fniessink   (501) staff       (20)        0 2023-03-21 19:46:39.037984 Toisto-0.9.0/src/toisto/
+-rw-r--r--   0 fniessink   (501) staff       (20)        0 2022-10-05 17:24:02.000000 Toisto-0.9.0/src/toisto/__init__.py
+-rw-r--r--   0 fniessink   (501) staff       (20)     1459 2023-03-18 21:15:55.000000 Toisto-0.9.0/src/toisto/app.py
+drwxr-xr-x   0 fniessink   (501) staff       (20)        0 2023-03-21 19:46:39.039615 Toisto-0.9.0/src/toisto/command/
+-rw-r--r--   0 fniessink   (501) staff       (20)        0 2023-01-31 17:17:41.000000 Toisto-0.9.0/src/toisto/command/__init__.py
+-rw-r--r--   0 fniessink   (501) staff       (20)     2008 2023-03-18 16:40:34.000000 Toisto-0.9.0/src/toisto/command/practice.py
+-rw-r--r--   0 fniessink   (501) staff       (20)     2182 2023-03-18 16:28:21.000000 Toisto-0.9.0/src/toisto/command/show_progress.py
+-rw-r--r--   0 fniessink   (501) staff       (20)     1788 2023-03-03 20:45:55.000000 Toisto-0.9.0/src/toisto/command/show_topics.py
+-rw-r--r--   0 fniessink   (501) staff       (20)     1315 2023-03-18 21:15:55.000000 Toisto-0.9.0/src/toisto/metadata.py
+drwxr-xr-x   0 fniessink   (501) staff       (20)        0 2023-03-21 19:46:39.039935 Toisto-0.9.0/src/toisto/model/
+-rw-r--r--   0 fniessink   (501) staff       (20)        0 2023-01-31 17:17:41.000000 Toisto-0.9.0/src/toisto/model/__init__.py
+drwxr-xr-x   0 fniessink   (501) staff       (20)        0 2023-03-21 19:46:39.042043 Toisto-0.9.0/src/toisto/model/language/
+-rw-r--r--   0 fniessink   (501) staff       (20)       89 2023-03-03 20:45:55.000000 Toisto-0.9.0/src/toisto/model/language/__init__.py
+-rw-r--r--   0 fniessink   (501) staff       (20)      833 2023-03-03 20:45:55.000000 Toisto-0.9.0/src/toisto/model/language/cefr.py
+-rw-r--r--   0 fniessink   (501) staff       (20)     5242 2023-03-18 16:28:21.000000 Toisto-0.9.0/src/toisto/model/language/concept.py
+-rw-r--r--   0 fniessink   (501) staff       (20)     5529 2023-03-18 16:28:21.000000 Toisto-0.9.0/src/toisto/model/language/concept_factory.py
+-rw-r--r--   0 fniessink   (501) staff       (20)      737 2023-03-21 16:43:50.000000 Toisto-0.9.0/src/toisto/model/language/grammar.py
+-rw-r--r--   0 fniessink   (501) staff       (20)      276 2023-03-03 20:45:55.000000 Toisto-0.9.0/src/toisto/model/language/iana_language_subtag_registry.py
+-rw-r--r--   0 fniessink   (501) staff       (20)     1571 2023-03-03 20:45:55.000000 Toisto-0.9.0/src/toisto/model/language/label.py
+drwxr-xr-x   0 fniessink   (501) staff       (20)        0 2023-03-21 19:46:39.044191 Toisto-0.9.0/src/toisto/model/quiz/
+-rw-r--r--   0 fniessink   (501) staff       (20)        0 2023-01-31 17:17:41.000000 Toisto-0.9.0/src/toisto/model/quiz/__init__.py
+-rw-r--r--   0 fniessink   (501) staff       (20)      429 2023-03-14 21:00:14.000000 Toisto-0.9.0/src/toisto/model/quiz/match.py
+-rw-r--r--   0 fniessink   (501) staff       (20)     4529 2023-03-20 20:50:03.000000 Toisto-0.9.0/src/toisto/model/quiz/progress.py
+-rw-r--r--   0 fniessink   (501) staff       (20)     5693 2023-03-21 16:43:50.000000 Toisto-0.9.0/src/toisto/model/quiz/quiz.py
+-rw-r--r--   0 fniessink   (501) staff       (20)     6447 2023-03-21 16:43:50.000000 Toisto-0.9.0/src/toisto/model/quiz/quiz_factory.py
+-rw-r--r--   0 fniessink   (501) staff       (20)     2872 2023-03-18 16:27:46.000000 Toisto-0.9.0/src/toisto/model/quiz/retention.py
+-rw-r--r--   0 fniessink   (501) staff       (20)      925 2023-03-20 07:57:59.000000 Toisto-0.9.0/src/toisto/model/quiz/topic.py
+drwxr-xr-x   0 fniessink   (501) staff       (20)        0 2023-03-21 19:46:39.046053 Toisto-0.9.0/src/toisto/persistence/
+-rw-r--r--   0 fniessink   (501) staff       (20)        0 2023-01-31 17:17:41.000000 Toisto-0.9.0/src/toisto/persistence/__init__.py
+-rw-r--r--   0 fniessink   (501) staff       (20)     4210 2023-03-03 20:45:55.000000 Toisto-0.9.0/src/toisto/persistence/config.py
+-rw-r--r--   0 fniessink   (501) staff       (20)     1490 2023-03-03 20:45:55.000000 Toisto-0.9.0/src/toisto/persistence/iana_language_subtag_registry.py
+-rw-r--r--   0 fniessink   (501) staff       (20)      741 2023-02-11 16:40:37.000000 Toisto-0.9.0/src/toisto/persistence/json_file.py
+-rw-r--r--   0 fniessink   (501) staff       (20)     1378 2023-03-18 21:15:55.000000 Toisto-0.9.0/src/toisto/persistence/progress.py
+-rw-r--r--   0 fniessink   (501) staff       (20)     3594 2023-03-07 17:41:01.000000 Toisto-0.9.0/src/toisto/persistence/topics.py
+-rw-r--r--   0 fniessink   (501) staff       (20)      491 2023-02-11 17:02:34.000000 Toisto-0.9.0/src/toisto/tools.py
+drwxr-xr-x   0 fniessink   (501) staff       (20)        0 2023-03-21 19:46:39.047929 Toisto-0.9.0/src/toisto/ui/
+-rw-r--r--   0 fniessink   (501) staff       (20)        0 2022-11-08 20:37:12.000000 Toisto-0.9.0/src/toisto/ui/__init__.py
+-rw-r--r--   0 fniessink   (501) staff       (20)     5483 2023-03-03 20:45:55.000000 Toisto-0.9.0/src/toisto/ui/cli.py
+-rw-r--r--   0 fniessink   (501) staff       (20)     1133 2023-03-03 20:45:55.000000 Toisto-0.9.0/src/toisto/ui/dictionary.py
+-rw-r--r--   0 fniessink   (501) staff       (20)     1510 2023-01-31 17:17:41.000000 Toisto-0.9.0/src/toisto/ui/diff.py
+-rw-r--r--   0 fniessink   (501) staff       (20)      732 2023-01-31 17:17:41.000000 Toisto-0.9.0/src/toisto/ui/format.py
+-rw-r--r--   0 fniessink   (501) staff       (20)     1550 2023-03-02 21:58:47.000000 Toisto-0.9.0/src/toisto/ui/speech.py
+-rw-r--r--   0 fniessink   (501) staff       (20)     3615 2023-02-18 17:38:39.000000 Toisto-0.9.0/src/toisto/ui/text.py
+drwxr-xr-x   0 fniessink   (501) staff       (20)        0 2023-03-21 19:46:39.058124 Toisto-0.9.0/src/topics/
+-rw-r--r--   0 fniessink   (501) staff       (20)      153 2023-03-03 20:45:55.000000 Toisto-0.9.0/src/topics/adverbs.json
+-rw-r--r--   0 fniessink   (501) staff       (20)     8841 2023-03-18 16:28:21.000000 Toisto-0.9.0/src/topics/animals.json
+-rw-r--r--   0 fniessink   (501) staff       (20)    11769 2023-03-14 21:00:14.000000 Toisto-0.9.0/src/topics/auxiliary_verbs.json
+-rw-r--r--   0 fniessink   (501) staff       (20)     7638 2023-03-03 20:45:55.000000 Toisto-0.9.0/src/topics/body.json
+-rw-r--r--   0 fniessink   (501) staff       (20)    10904 2023-03-18 16:28:21.000000 Toisto-0.9.0/src/topics/city.json
+-rw-r--r--   0 fniessink   (501) staff       (20)     6453 2023-03-03 20:45:55.000000 Toisto-0.9.0/src/topics/clothes.json
+-rw-r--r--   0 fniessink   (501) staff       (20)     7147 2023-03-18 16:28:21.000000 Toisto-0.9.0/src/topics/colors.json
+-rw-r--r--   0 fniessink   (501) staff       (20)    10767 2023-03-14 21:00:14.000000 Toisto-0.9.0/src/topics/counting.json
+-rw-r--r--   0 fniessink   (501) staff       (20)     2489 2023-03-03 20:45:55.000000 Toisto-0.9.0/src/topics/countries.json
+-rw-r--r--   0 fniessink   (501) staff       (20)     8243 2023-03-14 21:00:14.000000 Toisto-0.9.0/src/topics/days.json
+-rw-r--r--   0 fniessink   (501) staff       (20)    17341 2023-03-18 16:28:21.000000 Toisto-0.9.0/src/topics/degrees_of_comparison.json
+-rw-r--r--   0 fniessink   (501) staff       (20)    15149 2023-03-21 16:43:50.000000 Toisto-0.9.0/src/topics/family.json
+-rw-r--r--   0 fniessink   (501) staff       (20)    15942 2023-03-18 16:28:21.000000 Toisto-0.9.0/src/topics/food.json
+-rw-r--r--   0 fniessink   (501) staff       (20)     4597 2023-03-14 21:00:14.000000 Toisto-0.9.0/src/topics/furniture.json
+-rw-r--r--   0 fniessink   (501) staff       (20)     1989 2023-03-14 21:00:14.000000 Toisto-0.9.0/src/topics/grammar.json
+-rw-r--r--   0 fniessink   (501) staff       (20)     4851 2023-03-14 21:00:14.000000 Toisto-0.9.0/src/topics/greetings.json
+-rw-r--r--   0 fniessink   (501) staff       (20)     4224 2023-03-03 20:45:55.000000 Toisto-0.9.0/src/topics/health.json
+-rw-r--r--   0 fniessink   (501) staff       (20)     5483 2023-03-20 07:57:59.000000 Toisto-0.9.0/src/topics/holidays.json
+-rw-r--r--   0 fniessink   (501) staff       (20)     6823 2023-03-14 21:00:14.000000 Toisto-0.9.0/src/topics/house.json
+-rw-r--r--   0 fniessink   (501) staff       (20)     4676 2023-02-18 17:38:39.000000 Toisto-0.9.0/src/topics/interrogative_pronouns.json
+-rw-r--r--   0 fniessink   (501) staff       (20)     4606 2023-03-14 21:00:14.000000 Toisto-0.9.0/src/topics/languages.json
+-rw-r--r--   0 fniessink   (501) staff       (20)     4632 2023-03-14 21:00:14.000000 Toisto-0.9.0/src/topics/months.json
+-rw-r--r--   0 fniessink   (501) staff       (20)    12544 2023-03-18 16:28:21.000000 Toisto-0.9.0/src/topics/nature.json
+-rw-r--r--   0 fniessink   (501) staff       (20)      769 2023-03-21 16:43:50.000000 Toisto-0.9.0/src/topics/objects.json
+-rw-r--r--   0 fniessink   (501) staff       (20)     4876 2023-03-03 20:45:55.000000 Toisto-0.9.0/src/topics/possessive_adjectives.json
+-rw-r--r--   0 fniessink   (501) staff       (20)     5856 2023-03-14 21:00:14.000000 Toisto-0.9.0/src/topics/seasons.json
+-rw-r--r--   0 fniessink   (501) staff       (20)    23192 2023-03-14 21:00:14.000000 Toisto-0.9.0/src/topics/sentence_types.json
+-rw-r--r--   0 fniessink   (501) staff       (20)    10053 2023-03-14 21:00:14.000000 Toisto-0.9.0/src/topics/time.json
+-rw-r--r--   0 fniessink   (501) staff       (20)     1241 2023-03-21 16:43:50.000000 Toisto-0.9.0/src/topics/transport.json
+-rw-r--r--   0 fniessink   (501) staff       (20)    73212 2023-03-18 16:28:21.000000 Toisto-0.9.0/src/topics/verbs.json
+-rw-r--r--   0 fniessink   (501) staff       (20)     6504 2023-03-14 21:00:14.000000 Toisto-0.9.0/src/topics/weather.json
```

### Comparing `Toisto-0.8.2/LICENSE` & `Toisto-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Toisto-0.8.2/PKG-INFO` & `Toisto-0.9.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Toisto
-Version: 0.8.2
+Version: 0.9.0
 Summary: Toisto is a command-line terminal app to practice languages.
 Author-email: Frank Niessink <frank@niessink.com>
 Project-URL: Homepage, https://github.com/fniessink/toisto
 Project-URL: Issue tracker, https://github.com/fniessink/toisto/issues
 Project-URL: Changelog, https://github.com/fniessink/toisto/blob/main/CHANGELOG.md
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
@@ -24,14 +24,16 @@
 
 # Toisto
 
 Command-line app to practice languages. *Toisto* is Finnish and means *reiteration, playback, repetition, reproduction*.
 
 Toisto is beta software at the moment. It comes with a limited set of words and phrases in Dutch, English, and Finnish.
 
+Heads up: as long as Toisto is in beta the progress file format may change occasionally, causing your progress to be lost.
+
 ## User guide
 
 ### Prerequisites
 
 Make sure you have these prequisities installed:
 
 - [Python 3.10 or newer](https://python.org).
@@ -93,15 +95,15 @@
 To prevent having to pass your language level as command-line argument each time you run Toisto, put the language levels you want to practice in Toisto's configuration file. Create a file `.toisto.cfg` in your home directory if it doesn't exist, add the `languages` section if it doesn't exist, and add the levels:
 
 ```ini
 [languages]
 levels = A1 A2 B1
 ```
 
-Note that not all words and phrases have a language level associated with them. This means that specifying `levels = A1 A2 B1 B2 C1 C2` will cause Toisto to load only words and phrases with a language level.
+Note that not all words and phrases have a language level associated with them. This means that specifying `levels = A1 A2 B1 B2 C1 C2` will cause Toisto to load only words and phrases with a known language level.
 
 #### How to configure a different mp3 player
 
 By default, Toisto uses `afplay` on MacOS, `mpg123` on Linux, and the PlaySound function on Windows to play mp3 files. You can configure Toisto to use a different mp3 player. Create a file `.toisto.cfg` in your home directory if it doesn't exist, add the `commands` section if it doesn't exist, and add the mp3 player:
 
 ```ini
 [commands]
@@ -112,15 +114,15 @@
 
 ### Example sessions
 
 ![gif](https://raw.githubusercontent.com/fniessink/toisto/main/docs/demo.gif)
 
 ```console
 $ toisto practice --target fi --source nl
- Welcome to Toisto v0.8.0!
+👋 Welcome to Toisto v0.9.0!
 
 Practice as many words and phrases as you like, for as long as you like.
 
 Toisto quizzes you on words and phrases repeatedly. Each time you answer
 a quiz correctly, Toisto will wait longer before repeating it. If you
 answer incorrectly, you get one additional attempt to give the correct
 answer. If the second attempt is not correct either, Toisto will reset
@@ -130,54 +132,54 @@
 ● To answer a quiz: type the answer, followed by Enter.
 ● To repeat the spoken text: type Enter without answer.
 ● To skip to the answer immediately: type ?, followed by Enter.
 ● To read more about an underlined word: keep ⌘ (the command key) pressed
   while clicking the word. Not all terminals may support this.
 ● To quit: type Ctrl-C or Ctrl-D.
 
-Translate into Finnish:
-Zij komt uit het Noorden
-> hän tuluu pohjoisesta
-⚠️  Incorrect. Please try again.
-> hän kuluu pohjoisesta
-❌ Incorrect. The correct answer is "Hän tulee pohjoisesta".
-
 Translate into Dutch:
-Pohjoisessa on kylmä
-> het is koud in het noorden
+musta
+> zwart
 ✅ Correct.
 
-Translate into Finnish:
-Zij komt uit het Noorden
-> hän tulee pohjoisesta
+Translate into Dutch:
+valkoinen
+> wit
 ✅ Correct.
-Another correct answer is "Hän on kotoisin pohjoisesta".
 
 Translate into Dutch:
-Hyvää yötä
-> Goedenavond
+keltainen
+> oranje
 ⚠️  Incorrect. Please try again.
-> Goedenacht
+> geel
 ✅ Correct.
-Another correct answer is "Welterusten".
+
+Translate into Finnish:
+oranje
+> oransi
+⚠️  Incorrect. Please try again.
+> oransie
+❌ Incorrect. The correct answer is "oranssi".
 ```
 
 ### How it works
 
 Toisto quizzes you repeatably on words and phrases in the language you want to practice, your target language. For each quiz, Toisto keeps track of how long you answer it correctly. When you answer a quiz correctly multiple times, Toisto will silence the quiz for a while. The longer the time you have answered the quiz correctly, the longer a quiz is silenced. This starts at a few minutes, but then increases rapidly when you keep answering correctly.
 
 At the moment, Toisto has the following types of quizzes:
 
-- Translate a word or phrase from your target language to your source language or the other way around. For example, if your native language is English and you're practicing Dutch, Toisto can ask you to give the English version of "Maandag" (which is, you guessed it, "Monday") or ask you to give the Dutch version of "Friday" (which is "Vrijdag").
+- Translate a word or phrase from your target language to your source language or the other way around. For example, if your native language is English and you're practicing Dutch, Toisto can ask you to give the English version of "maandag" (which is, you guessed it, "Monday") or ask you to give the Dutch version of "Friday" (which is "vrijdag").
 - Listen to a word or phrase from your target language and type what you hear. For example, if your target language is Finnish, Toisto may say "Tänään on maanantai" (Today is Monday) and that's then what you have to type.
-- Give a singular version of a plural, or a plural version of a singular. For example, what is the plural of "Talo" (meaning house in Finnish, and the answer is "Talot") or what is the singular of "Huizen" (meaning houses in Dutch, and the answer is "Huis").
-- Change the grammatical person from and to first person, second person, and third person. For example, when asked what the second person of "Ik eet" (meaning "I eat") is, the correct answer would be "Jij eet" ("You eat").
-- Change the tense of verbs from present to past tense or the other way around. For example, what is the past tense of "She walks" or what is the present tense version of "He painted".
-- Change the comparative degree of an adjective. For example, what is the superlative degree of "Aardig" (which means "Nice", and the answer would be "Aardigst").
-- Change the sentence type of declarative sentences into interrogative sentences and vice versa. For example, what is the interrogative form of "The car is black"? The answer would be "Is the car black?"
+- Give a singular version of a plural, or a plural version of a singular. For example, what is the plural of "talo" (meaning house in Finnish, and the answer is "talot") or what is the singular of "de huizen" (meaning the houses in Dutch, and the answer would be "het huis").
+- Give the diminutive form of a word. For example, what is the diminutive form of "het huis" in Dutch (meaning house in Dutch and the answer would be "het huisje").
+- Change the grammatical person from and to first person, second person, and third person. For example, when asked what the second person of "ik eet" (meaning "I eat") is, the correct answer would be "jij eet" ("you eat").
+- Change the tense of verbs from present to past tense or the other way around. For example, what is the past tense of "she walks" or what is the present tense version of "he painted".
+- Change the comparative degree of an adjective. For example, what is the superlative degree of "aardig" (which means "nice", and the answer would be "aardigst").
+- Give the antonym of adjectives. For example, what is the antonym of "good"? The answer of course being "bad".
+- Change the sentence type of declarative sentences into interrogative sentences and vice versa. For example, what is the interrogative form of "The car is black"? The answer would be "Is the car black?".
 
 When you stop the program (hit Ctrl-C or Ctrl-D), progress is saved in a file named `.toisto-progress.json` in your home folder.
 
 ## Further documentation
 
 - [More information](docs/background.md) on why Toisto exists and what the future plans are.
 - The [Toisto software documentation](docs/software.md) describes the inner workings of Toisto, including the format of the topic files.
```

### Comparing `Toisto-0.8.2/README.md` & `Toisto-0.9.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # Toisto
 
 Command-line app to practice languages. *Toisto* is Finnish and means *reiteration, playback, repetition, reproduction*.
 
 Toisto is beta software at the moment. It comes with a limited set of words and phrases in Dutch, English, and Finnish.
 
+Heads up: as long as Toisto is in beta the progress file format may change occasionally, causing your progress to be lost.
+
 ## User guide
 
 ### Prerequisites
 
 Make sure you have these prequisities installed:
 
 - [Python 3.10 or newer](https://python.org).
@@ -69,15 +71,15 @@
 To prevent having to pass your language level as command-line argument each time you run Toisto, put the language levels you want to practice in Toisto's configuration file. Create a file `.toisto.cfg` in your home directory if it doesn't exist, add the `languages` section if it doesn't exist, and add the levels:
 
 ```ini
 [languages]
 levels = A1 A2 B1
 ```
 
-Note that not all words and phrases have a language level associated with them. This means that specifying `levels = A1 A2 B1 B2 C1 C2` will cause Toisto to load only words and phrases with a language level.
+Note that not all words and phrases have a language level associated with them. This means that specifying `levels = A1 A2 B1 B2 C1 C2` will cause Toisto to load only words and phrases with a known language level.
 
 #### How to configure a different mp3 player
 
 By default, Toisto uses `afplay` on MacOS, `mpg123` on Linux, and the PlaySound function on Windows to play mp3 files. You can configure Toisto to use a different mp3 player. Create a file `.toisto.cfg` in your home directory if it doesn't exist, add the `commands` section if it doesn't exist, and add the mp3 player:
 
 ```ini
 [commands]
@@ -88,15 +90,15 @@
 
 ### Example sessions
 
 ![gif](https://raw.githubusercontent.com/fniessink/toisto/main/docs/demo.gif)
 
 ```console
 $ toisto practice --target fi --source nl
- Welcome to Toisto v0.8.0!
+👋 Welcome to Toisto v0.9.0!
 
 Practice as many words and phrases as you like, for as long as you like.
 
 Toisto quizzes you on words and phrases repeatedly. Each time you answer
 a quiz correctly, Toisto will wait longer before repeating it. If you
 answer incorrectly, you get one additional attempt to give the correct
 answer. If the second attempt is not correct either, Toisto will reset
@@ -106,54 +108,54 @@
 ● To answer a quiz: type the answer, followed by Enter.
 ● To repeat the spoken text: type Enter without answer.
 ● To skip to the answer immediately: type ?, followed by Enter.
 ● To read more about an underlined word: keep ⌘ (the command key) pressed
   while clicking the word. Not all terminals may support this.
 ● To quit: type Ctrl-C or Ctrl-D.
 
-Translate into Finnish:
-Zij komt uit het Noorden
-> hän tuluu pohjoisesta
-⚠️  Incorrect. Please try again.
-> hän kuluu pohjoisesta
-❌ Incorrect. The correct answer is "Hän tulee pohjoisesta".
-
 Translate into Dutch:
-Pohjoisessa on kylmä
-> het is koud in het noorden
+musta
+> zwart
 ✅ Correct.
 
-Translate into Finnish:
-Zij komt uit het Noorden
-> hän tulee pohjoisesta
+Translate into Dutch:
+valkoinen
+> wit
 ✅ Correct.
-Another correct answer is "Hän on kotoisin pohjoisesta".
 
 Translate into Dutch:
-Hyvää yötä
-> Goedenavond
+keltainen
+> oranje
 ⚠️  Incorrect. Please try again.
-> Goedenacht
+> geel
 ✅ Correct.
-Another correct answer is "Welterusten".
+
+Translate into Finnish:
+oranje
+> oransi
+⚠️  Incorrect. Please try again.
+> oransie
+❌ Incorrect. The correct answer is "oranssi".
 ```
 
 ### How it works
 
 Toisto quizzes you repeatably on words and phrases in the language you want to practice, your target language. For each quiz, Toisto keeps track of how long you answer it correctly. When you answer a quiz correctly multiple times, Toisto will silence the quiz for a while. The longer the time you have answered the quiz correctly, the longer a quiz is silenced. This starts at a few minutes, but then increases rapidly when you keep answering correctly.
 
 At the moment, Toisto has the following types of quizzes:
 
-- Translate a word or phrase from your target language to your source language or the other way around. For example, if your native language is English and you're practicing Dutch, Toisto can ask you to give the English version of "Maandag" (which is, you guessed it, "Monday") or ask you to give the Dutch version of "Friday" (which is "Vrijdag").
+- Translate a word or phrase from your target language to your source language or the other way around. For example, if your native language is English and you're practicing Dutch, Toisto can ask you to give the English version of "maandag" (which is, you guessed it, "Monday") or ask you to give the Dutch version of "Friday" (which is "vrijdag").
 - Listen to a word or phrase from your target language and type what you hear. For example, if your target language is Finnish, Toisto may say "Tänään on maanantai" (Today is Monday) and that's then what you have to type.
-- Give a singular version of a plural, or a plural version of a singular. For example, what is the plural of "Talo" (meaning house in Finnish, and the answer is "Talot") or what is the singular of "Huizen" (meaning houses in Dutch, and the answer is "Huis").
-- Change the grammatical person from and to first person, second person, and third person. For example, when asked what the second person of "Ik eet" (meaning "I eat") is, the correct answer would be "Jij eet" ("You eat").
-- Change the tense of verbs from present to past tense or the other way around. For example, what is the past tense of "She walks" or what is the present tense version of "He painted".
-- Change the comparative degree of an adjective. For example, what is the superlative degree of "Aardig" (which means "Nice", and the answer would be "Aardigst").
-- Change the sentence type of declarative sentences into interrogative sentences and vice versa. For example, what is the interrogative form of "The car is black"? The answer would be "Is the car black?"
+- Give a singular version of a plural, or a plural version of a singular. For example, what is the plural of "talo" (meaning house in Finnish, and the answer is "talot") or what is the singular of "de huizen" (meaning the houses in Dutch, and the answer would be "het huis").
+- Give the diminutive form of a word. For example, what is the diminutive form of "het huis" in Dutch (meaning house in Dutch and the answer would be "het huisje").
+- Change the grammatical person from and to first person, second person, and third person. For example, when asked what the second person of "ik eet" (meaning "I eat") is, the correct answer would be "jij eet" ("you eat").
+- Change the tense of verbs from present to past tense or the other way around. For example, what is the past tense of "she walks" or what is the present tense version of "he painted".
+- Change the comparative degree of an adjective. For example, what is the superlative degree of "aardig" (which means "nice", and the answer would be "aardigst").
+- Give the antonym of adjectives. For example, what is the antonym of "good"? The answer of course being "bad".
+- Change the sentence type of declarative sentences into interrogative sentences and vice versa. For example, what is the interrogative form of "The car is black"? The answer would be "Is the car black?".
 
 When you stop the program (hit Ctrl-C or Ctrl-D), progress is saved in a file named `.toisto-progress.json` in your home folder.
 
 ## Further documentation
 
 - [More information](docs/background.md) on why Toisto exists and what the future plans are.
 - The [Toisto software documentation](docs/software.md) describes the inner workings of Toisto, including the format of the topic files.
```

### Comparing `Toisto-0.8.2/pyproject.toml` & `Toisto-0.9.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "Toisto"
-version = "0.8.2"
+version = "0.9.0"
 authors = [
   { name="Frank Niessink", email="frank@niessink.com" },
 ]
 description = "Toisto is a command-line terminal app to practice languages."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -32,22 +32,23 @@
     "rich-argparse >= 1.0.0",
 ]
 
 [project.optional-dependencies]
 dev = [
     "black == 23.1.0",
     "build == 0.10.0",
-    "coverage == 7.1.0",
+    "coverage == 7.2.2",
     "green == 3.4.3",
-    "mypy == 1.0.0",
-    "pip == 23.0",
-    "ruff == 0.0.246",
+    "mypy == 1.1.1",
+    "pip == 23.0.1",
+    "ruff == 0.0.257",
     "twine == 4.0.2",
-    "types-playsound == 1.3.1.1",
-    "types-requests == 2.28.11.12"
+    "types-playsound == 1.3.1.2",
+    "types-requests == 2.28.11.15",
+    "vulture == 2.7.0"
 ]
 
 [project.scripts]
 toisto = "toisto.app:main"
 
 [project.urls]
 "Homepage" = "https://github.com/fniessink/toisto"
```

### Comparing `Toisto-0.8.2/src/Toisto.egg-info/PKG-INFO` & `Toisto-0.9.0/src/Toisto.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Toisto
-Version: 0.8.2
+Version: 0.9.0
 Summary: Toisto is a command-line terminal app to practice languages.
 Author-email: Frank Niessink <frank@niessink.com>
 Project-URL: Homepage, https://github.com/fniessink/toisto
 Project-URL: Issue tracker, https://github.com/fniessink/toisto/issues
 Project-URL: Changelog, https://github.com/fniessink/toisto/blob/main/CHANGELOG.md
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
@@ -24,14 +24,16 @@
 
 # Toisto
 
 Command-line app to practice languages. *Toisto* is Finnish and means *reiteration, playback, repetition, reproduction*.
 
 Toisto is beta software at the moment. It comes with a limited set of words and phrases in Dutch, English, and Finnish.
 
+Heads up: as long as Toisto is in beta the progress file format may change occasionally, causing your progress to be lost.
+
 ## User guide
 
 ### Prerequisites
 
 Make sure you have these prequisities installed:
 
 - [Python 3.10 or newer](https://python.org).
@@ -93,15 +95,15 @@
 To prevent having to pass your language level as command-line argument each time you run Toisto, put the language levels you want to practice in Toisto's configuration file. Create a file `.toisto.cfg` in your home directory if it doesn't exist, add the `languages` section if it doesn't exist, and add the levels:
 
 ```ini
 [languages]
 levels = A1 A2 B1
 ```
 
-Note that not all words and phrases have a language level associated with them. This means that specifying `levels = A1 A2 B1 B2 C1 C2` will cause Toisto to load only words and phrases with a language level.
+Note that not all words and phrases have a language level associated with them. This means that specifying `levels = A1 A2 B1 B2 C1 C2` will cause Toisto to load only words and phrases with a known language level.
 
 #### How to configure a different mp3 player
 
 By default, Toisto uses `afplay` on MacOS, `mpg123` on Linux, and the PlaySound function on Windows to play mp3 files. You can configure Toisto to use a different mp3 player. Create a file `.toisto.cfg` in your home directory if it doesn't exist, add the `commands` section if it doesn't exist, and add the mp3 player:
 
 ```ini
 [commands]
@@ -112,15 +114,15 @@
 
 ### Example sessions
 
 ![gif](https://raw.githubusercontent.com/fniessink/toisto/main/docs/demo.gif)
 
 ```console
 $ toisto practice --target fi --source nl
- Welcome to Toisto v0.8.0!
+👋 Welcome to Toisto v0.9.0!
 
 Practice as many words and phrases as you like, for as long as you like.
 
 Toisto quizzes you on words and phrases repeatedly. Each time you answer
 a quiz correctly, Toisto will wait longer before repeating it. If you
 answer incorrectly, you get one additional attempt to give the correct
 answer. If the second attempt is not correct either, Toisto will reset
@@ -130,54 +132,54 @@
 ● To answer a quiz: type the answer, followed by Enter.
 ● To repeat the spoken text: type Enter without answer.
 ● To skip to the answer immediately: type ?, followed by Enter.
 ● To read more about an underlined word: keep ⌘ (the command key) pressed
   while clicking the word. Not all terminals may support this.
 ● To quit: type Ctrl-C or Ctrl-D.
 
-Translate into Finnish:
-Zij komt uit het Noorden
-> hän tuluu pohjoisesta
-⚠️  Incorrect. Please try again.
-> hän kuluu pohjoisesta
-❌ Incorrect. The correct answer is "Hän tulee pohjoisesta".
-
 Translate into Dutch:
-Pohjoisessa on kylmä
-> het is koud in het noorden
+musta
+> zwart
 ✅ Correct.
 
-Translate into Finnish:
-Zij komt uit het Noorden
-> hän tulee pohjoisesta
+Translate into Dutch:
+valkoinen
+> wit
 ✅ Correct.
-Another correct answer is "Hän on kotoisin pohjoisesta".
 
 Translate into Dutch:
-Hyvää yötä
-> Goedenavond
+keltainen
+> oranje
 ⚠️  Incorrect. Please try again.
-> Goedenacht
+> geel
 ✅ Correct.
-Another correct answer is "Welterusten".
+
+Translate into Finnish:
+oranje
+> oransi
+⚠️  Incorrect. Please try again.
+> oransie
+❌ Incorrect. The correct answer is "oranssi".
 ```
 
 ### How it works
 
 Toisto quizzes you repeatably on words and phrases in the language you want to practice, your target language. For each quiz, Toisto keeps track of how long you answer it correctly. When you answer a quiz correctly multiple times, Toisto will silence the quiz for a while. The longer the time you have answered the quiz correctly, the longer a quiz is silenced. This starts at a few minutes, but then increases rapidly when you keep answering correctly.
 
 At the moment, Toisto has the following types of quizzes:
 
-- Translate a word or phrase from your target language to your source language or the other way around. For example, if your native language is English and you're practicing Dutch, Toisto can ask you to give the English version of "Maandag" (which is, you guessed it, "Monday") or ask you to give the Dutch version of "Friday" (which is "Vrijdag").
+- Translate a word or phrase from your target language to your source language or the other way around. For example, if your native language is English and you're practicing Dutch, Toisto can ask you to give the English version of "maandag" (which is, you guessed it, "Monday") or ask you to give the Dutch version of "Friday" (which is "vrijdag").
 - Listen to a word or phrase from your target language and type what you hear. For example, if your target language is Finnish, Toisto may say "Tänään on maanantai" (Today is Monday) and that's then what you have to type.
-- Give a singular version of a plural, or a plural version of a singular. For example, what is the plural of "Talo" (meaning house in Finnish, and the answer is "Talot") or what is the singular of "Huizen" (meaning houses in Dutch, and the answer is "Huis").
-- Change the grammatical person from and to first person, second person, and third person. For example, when asked what the second person of "Ik eet" (meaning "I eat") is, the correct answer would be "Jij eet" ("You eat").
-- Change the tense of verbs from present to past tense or the other way around. For example, what is the past tense of "She walks" or what is the present tense version of "He painted".
-- Change the comparative degree of an adjective. For example, what is the superlative degree of "Aardig" (which means "Nice", and the answer would be "Aardigst").
-- Change the sentence type of declarative sentences into interrogative sentences and vice versa. For example, what is the interrogative form of "The car is black"? The answer would be "Is the car black?"
+- Give a singular version of a plural, or a plural version of a singular. For example, what is the plural of "talo" (meaning house in Finnish, and the answer is "talot") or what is the singular of "de huizen" (meaning the houses in Dutch, and the answer would be "het huis").
+- Give the diminutive form of a word. For example, what is the diminutive form of "het huis" in Dutch (meaning house in Dutch and the answer would be "het huisje").
+- Change the grammatical person from and to first person, second person, and third person. For example, when asked what the second person of "ik eet" (meaning "I eat") is, the correct answer would be "jij eet" ("you eat").
+- Change the tense of verbs from present to past tense or the other way around. For example, what is the past tense of "she walks" or what is the present tense version of "he painted".
+- Change the comparative degree of an adjective. For example, what is the superlative degree of "aardig" (which means "nice", and the answer would be "aardigst").
+- Give the antonym of adjectives. For example, what is the antonym of "good"? The answer of course being "bad".
+- Change the sentence type of declarative sentences into interrogative sentences and vice versa. For example, what is the interrogative form of "The car is black"? The answer would be "Is the car black?".
 
 When you stop the program (hit Ctrl-C or Ctrl-D), progress is saved in a file named `.toisto-progress.json` in your home folder.
 
 ## Further documentation
 
 - [More information](docs/background.md) on why Toisto exists and what the future plans are.
 - The [Toisto software documentation](docs/software.md) describes the inner workings of Toisto, including the format of the topic files.
```

### Comparing `Toisto-0.8.2/src/Toisto.egg-info/SOURCES.txt` & `Toisto-0.9.0/src/Toisto.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -54,14 +54,15 @@
 src/topics/counting.json
 src/topics/countries.json
 src/topics/days.json
 src/topics/degrees_of_comparison.json
 src/topics/family.json
 src/topics/food.json
 src/topics/furniture.json
+src/topics/grammar.json
 src/topics/greetings.json
 src/topics/health.json
 src/topics/holidays.json
 src/topics/house.json
 src/topics/interrogative_pronouns.json
 src/topics/languages.json
 src/topics/months.json
```

### Comparing `Toisto-0.8.2/src/languages/iana-language-subtag-registry.txt` & `Toisto-0.9.0/src/languages/iana-language-subtag-registry.txt`

 * *Files identical despite different names*

### Comparing `Toisto-0.8.2/src/toisto/app.py` & `Toisto-0.9.0/src/toisto/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         args.target_language,
         args.source_language,
         args.levels,
         args.topic,
         args.topic_file,
         argument_parser,
     )
-    progress = load_progress(topics, argument_parser)
+    progress = load_progress(topics, args.target_language, argument_parser)
     if args.command == "practice":
         show_welcome(latest_version())
         practice(progress, config)
     elif args.command == "topics":
         show_topics(args.target_language, args.source_language, topics)
     else:
         show_progress(args.target_language, topics, progress, args.sort)
```

### Comparing `Toisto-0.8.2/src/toisto/command/practice.py` & `Toisto-0.9.0/src/toisto/command/practice.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Practice command."""
 
 from configparser import ConfigParser
+from typing import get_args
 
 from toisto.model.language.label import Label
 from toisto.model.quiz.progress import Progress
-from toisto.model.quiz.quiz import Quiz
+from toisto.model.quiz.quiz import ListenQuizType, Quiz
 from toisto.persistence.progress import save_progress
 from toisto.ui.dictionary import linkify
 from toisto.ui.speech import say
 from toisto.ui.text import DONE, TRY_AGAIN, console, feedback_correct, feedback_incorrect, instruction
 
 
 def do_quiz_attempt(quiz: Quiz, config: ConfigParser, attempt: int = 1) -> tuple[Label, bool]:
@@ -20,15 +21,15 @@
         print("\033[F", end="")  # noqa: T201  # Move cursor one line up
     return answer, quiz.is_correct(answer)
 
 
 def do_quiz(quiz: Quiz, progress: Progress, config: ConfigParser) -> None:
     """Do one quiz and update the progress."""
     console.print(instruction(quiz))
-    if "listen" not in quiz.quiz_types:
+    if quiz.quiz_types[0] not in get_args(ListenQuizType):
         console.print(linkify(quiz.question))
     answer, correct = do_quiz_attempt(quiz, config)
     if not correct and answer != "?":
         console.print(TRY_AGAIN)
         answer, correct = do_quiz_attempt(quiz, config, attempt=2)
     if correct:
         progress.increase_retention(quiz)
```

### Comparing `Toisto-0.8.2/src/toisto/command/show_progress.py` & `Toisto-0.9.0/src/toisto/command/show_progress.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,57 +1,53 @@
 """Command to show progress information."""
 
 from dataclasses import dataclass
 from datetime import datetime
 from typing import Literal
 
+from rich.console import JustifyMethod
 from rich.table import Table
 
 from toisto.model.language import Language
 from toisto.model.language.iana_language_subtag_registry import ALL_LANGUAGES
 from toisto.model.quiz.progress import Progress
 from toisto.model.quiz.quiz import Quiz
 from toisto.model.quiz.topic import Topics
 from toisto.ui.format import format_datetime, format_duration
 from toisto.ui.text import console
 
 SortColumn = Literal["attempts", "retention"]
 RETENTION_ATTRIBUTE = dict(attempts="count", retention="length")
 
 
-@dataclass
+@dataclass(frozen=True)
 class QuizSorter:
     """Class to provide a sort function to sort quizzes."""
 
     progress: Progress
     sort: SortColumn
 
     def get_sort_key(self, quiz: Quiz) -> str:
         """Return the retention attribute to sort by."""
         return getattr(self.progress.get_retention(quiz), RETENTION_ATTRIBUTE[self.sort])
 
 
 def show_progress(language: Language, topics: Topics, progress: Progress, sort: SortColumn = "attempts") -> None:
     """Show progress."""
     table = Table(title=f"Progress {ALL_LANGUAGES[language]}")
-    table.add_column("Quiz type")
-    table.add_column("Question")
-    table.add_column("From")
-    table.add_column("To")
-    table.add_column("Answer(s)")
-    table.add_column("Attempts", justify="right")
-    table.add_column("Retention")
-    table.add_column("Not quizzed until")
+    justify: dict[str, JustifyMethod] = dict(Attempts="right")
+    for column in ("Quiz type", "Question", "From", "To", "Answer(s)", "Attempts", "Retention", "Not quizzed until"):
+        table.add_column(column, justify=justify.get(column, "left"))
     sorted_quizzes = sorted(topics.quizzes, key=QuizSorter(progress, sort).get_sort_key, reverse=True)
     for quiz in sorted_quizzes:
         retention = progress.get_retention(quiz)
         skip = retention.skip_until
-        quiz_types = " and ".join(quiz.quiz_types)
+        quiz_types = " and ".join(quiz.quiz_types).capitalize()
         table.add_row(
-            quiz_types.capitalize(),
+            quiz_types,
             quiz.question,
             quiz.question_language,
             quiz.answer_language,
             "\n".join(quiz.answers),
             str(retention.count),
             format_duration(retention.length) if retention.length else "",
             format_datetime(skip) if skip and skip > datetime.now() else "",
```

### Comparing `Toisto-0.8.2/src/toisto/command/show_topics.py` & `Toisto-0.9.0/src/toisto/command/show_topics.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,18 +15,17 @@
     """Enumerate the labels."""
     return "\n".join(chain.from_iterable(label.spelling_alternatives for label in labels))
 
 
 def topic_table(target_language: Language, source_language: Language, topic: Topic) -> Table:
     """Show the concepts of the topic."""
     table = Table(title=f"Topic {topic.name}")
-    table.add_column(ALL_LANGUAGES[target_language])
-    table.add_column(ALL_LANGUAGES[source_language])
-    table.add_column("Grammatical categories")
-    table.add_column("Language level")
+    target_language_name, source_language_name = ALL_LANGUAGES[target_language], ALL_LANGUAGES[source_language]
+    for column in (target_language_name, source_language_name, "Grammatical categories", "Language level"):
+        table.add_column(column)
     for concept in topic.concepts:
         for leaf_concept in concept.leaf_concepts():
             target_labels = leaf_concept.labels(target_language)
             source_labels = leaf_concept.labels(source_language)
             if target_labels or source_labels:
                 table.add_row(
                     enumerate_labels(target_labels),
```

### Comparing `Toisto-0.8.2/src/toisto/model/language/cefr.py` & `Toisto-0.9.0/src/toisto/model/language/cefr.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,17 @@
-"""Common European Framework of Reference for Languages (CEFR)."""
+"""Common European Framework of Reference for Languages (CEFR).
+
+See https://www.coe.int/en/web/common-european-framework-reference-languages/level-descriptions
+
+Used sources for the language levels of words are:
+- EP: [English Vocabulary Profile Online - British English (en)](https://www.englishprofile.org/wordlists/evp")
+- KK: [Yle Kielikoulu Learning Profile (fi)]("https://kielikoulu.yle.fi/#/profile")
+- OD: [Oxford Advanced Learner's Dictionary online (en)]("https://www.oxfordlearnersdictionaries.com")
+"""
 
 from typing import Literal
 
-# Source: https://www.coe.int/en/web/common-european-framework-reference-languages/level-descriptions
+# The levels defined by the Common European Framework of Reference for Languages:
 CommonReferenceLevel = Literal["A1", "A2", "B1", "B2", "C1", "C2"]
 
 # Toisto uses different sources to assess the common reference level for concepts:
 CommonReferenceLevelSource = Literal["EP", "KK", "OD"]
-
-SOURCES: dict[CommonReferenceLevelSource, dict[Literal["name", "url", "language"], str]] = dict(
-    EP=dict(
-        name="English Vocabulary Profile Online - British English",
-        url="https://www.englishprofile.org/wordlists/evp",
-        language="en",
-    ),
-    KK=dict(name="Yle Kielikoulu Learning Profile", url="https://kielikoulu.yle.fi/#/profile", language="fi"),
-    OD=dict(
-        name="Oxford Advanced Learner's Dictionary online",
-        url="https://www.oxfordlearnersdictionaries.com",
-        language="en",
-    ),
-)
```

### Comparing `Toisto-0.8.2/src/toisto/model/language/concept.py` & `Toisto-0.9.0/src/toisto/model/language/concept.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 """Concept classes."""
 
 from __future__ import annotations
 
 from collections.abc import Iterable
 from dataclasses import dataclass, field
+from functools import cached_property
 from typing import ClassVar, NewType, cast, get_args
 
 from . import Language
 from .cefr import CommonReferenceLevel
 from .grammar import GrammaticalCategory
-from .label import Label, Labels
+from .label import Labels
 
 ConceptId = NewType("ConceptId", str)
 ConceptIds = tuple[ConceptId, ...]
 
 
-@dataclass
+@dataclass(frozen=True)
 class RelatedConcepts:
     """Class representing the relations of a concept with other concepts.
 
     Concepts can be composites, meaning they consists of subconcepts (called constituent concepts). For example, a noun
     concept may have a singular and plural form. These forms are represented as constituent concepts of the parent
     concept. The parent and constituent attributes keep track of these relations.
 
@@ -61,25 +62,26 @@
         return self._get_concepts(*concept_ids_of_roots)
 
     def _get_concepts(self, *concept_ids: ConceptId) -> Concepts:
         """Return the concepts with the given concept ids."""
         return tuple(Concept.instances[concept_id] for concept_id in concept_ids if concept_id in Concept.instances)
 
 
-@dataclass
+@dataclass(frozen=True)
 class Concept:
     """Class representing language concepts.
 
     A concept is either a composite or a leaf concept. Composite concepts have have two or more constituent concepts,
     representing different grammatical categories, for example singular and plural forms. Leaf concepts have labels
     in different languages.
     """
 
     concept_id: ConceptId
     _labels: dict[Language, Labels] = field(default_factory=dict)
+    _meanings: dict[Language, Labels] = field(default_factory=dict)
     level: CommonReferenceLevel | None = None
     related_concepts: RelatedConcepts = RelatedConcepts()
 
     instances: ClassVar[dict[ConceptId, Concept]] = {}
 
     def __post_init__(self) -> None:
         """Add the concept to the concept id -> concept mapping."""
@@ -89,15 +91,15 @@
         """Return the concept hash."""
         return hash(self.concept_id)
 
     def __getattr__(self, attribute: str) -> Concepts:
         """Forward properties to related concepts."""
         return getattr(self.related_concepts, attribute)
 
-    @property
+    @cached_property
     def base_concept(self) -> Concept:
         """Return the base concept of this concept."""
         return self.related_concepts.parent.base_concept if self.related_concepts.parent else self
 
     def leaf_concepts(self) -> Iterable[Concept]:
         """Return this concept's leaf concepts, or self if this concept is a leaf concept."""
         if self.constituents:
@@ -107,17 +109,16 @@
             yield self
 
     def labels(self, language: Language) -> Labels:
         """Return the labels for the language."""
         return self._labels.get(language, Labels())
 
     def meanings(self, language: Language) -> Labels:
-        """Return the meaning of the concept in the specified language."""
-        meaning = Label(self._labels.get(language, [""])[0])
-        return (meaning,) if meaning else ()
+        """Return the meanings of the concept in the specified language."""
+        return self._meanings.get(language, Labels())
 
     def grammatical_categories(self) -> tuple[GrammaticalCategory, ...]:
         """Return the grammatical categories of this concept."""
         keys = self.concept_id.split("/")
         return tuple(cast(GrammaticalCategory, key) for key in keys if key in get_args(GrammaticalCategory))
```

### Comparing `Toisto-0.8.2/src/toisto/model/language/concept_factory.py` & `Toisto-0.9.0/src/toisto/model/language/concept_factory.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing import Literal, Union, cast, get_args
 
 from . import Language
 from .cefr import CommonReferenceLevel, CommonReferenceLevelSource
 from .concept import Concept, ConceptId, ConceptIds, RelatedConcepts
 from .grammar import GrammaticalCategory
 from .iana_language_subtag_registry import ALL_LANGUAGES
-from .label import Labels, label_factory
+from .label import Labels, label_factory, meaning_factory
 
 CommonReferenceLevelDict = dict[CommonReferenceLevel, CommonReferenceLevelSource | list[CommonReferenceLevelSource]]
 ConceptIdListOrString = ConceptId | list[ConceptId]
 ConceptIdDictOrListOrString = dict[Language, ConceptIdListOrString] | ConceptIdListOrString
 MetaData = Literal["level", "antonym", "roots"]
 LeafConceptDict = dict[
     Language | MetaData,
@@ -23,33 +23,41 @@
 CompositeConceptDict = dict[
     GrammaticalCategory | MetaData,
     Union["CompositeConceptDict", LeafConceptDict, CommonReferenceLevelDict],
 ]
 ConceptDict = LeafConceptDict | CompositeConceptDict
 
 
-@dataclass
+@dataclass(frozen=True)
 class ConceptFactory:
     """Create concepts from the concept dict."""
 
     concept_id: ConceptId
     concept_dict: ConceptDict
 
     def create_concept(self, parent: ConceptId | None = None) -> Concept:
         """Create a concept from the concept_dict."""
-        return Concept(self.concept_id, self._labels(), self._level(), self._related_concepts(parent))
+        return Concept(self.concept_id, self._labels(), self._meanings(), self._level(), self._related_concepts(parent))
 
     def _labels(self) -> dict[Language, Labels]:
         """Return the concept labels."""
         return {
             cast(Language, key): label_factory(cast(str | list[str], value))
             for key, value in self.concept_dict.items()
             if key in ALL_LANGUAGES
         }
 
+    def _meanings(self) -> dict[Language, Labels]:
+        """Return the concept meanings."""
+        return {
+            cast(Language, key): meaning_factory(cast(str | list[str], value))
+            for key, value in self.concept_dict.items()
+            if key in ALL_LANGUAGES
+        }
+
     def _level(self) -> CommonReferenceLevel | None:
         """Determine the Common Reference Level for this concept.
 
         At the moment, just use the highest language level specified by the available sources.
         """
         concept_levels = [level for level in self._get_levels() if level in get_args(CommonReferenceLevel)]
         return max(concept_levels, default=None)
```

### Comparing `Toisto-0.8.2/src/toisto/model/language/grammar.py` & `Toisto-0.9.0/src/toisto/model/language/grammar.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,19 +2,21 @@
 
 from typing import Literal
 
 GrammaticalGender = Literal["female", "male", "neuter"]
 GrammaticalNumber = Literal["infinitive", "singular", "plural"]
 GrammaticalPerson = Literal["first person", "second person", "third person"]
 DegreeOfComparison = Literal["positive degree", "comparative degree", "superlative degree"]
+Diminutive = Literal["root", "diminutive"]
 Tense = Literal["present tense", "past tense"]
 SentenceForm = Literal["declarative", "interrogative"]
 GrammaticalPolarity = Literal["affirmative", "negative"]
 GrammaticalCategory = Literal[
     GrammaticalGender,
     GrammaticalNumber,
     GrammaticalPerson,
     DegreeOfComparison,
+    Diminutive,
     Tense,
     SentenceForm,
     GrammaticalPolarity,
 ]
```

### Comparing `Toisto-0.8.2/src/toisto/model/language/label.py` & `Toisto-0.9.0/src/toisto/model/language/label.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,37 +2,47 @@
 
 from __future__ import annotations
 
 
 class Label(str):
     """Class representing labels for concepts."""
 
+    HINT_SEP = ";"
+    SPELLING_ALTERNATIVES_SEP = "|"
+
     def __eq__(self, other: object) -> bool:
         """Ignore hints when determining equality."""
-        return self.split(";", maxsplit=1)[0] == str(other).split(";", maxsplit=1)[0]
+        return self.without_hint == Label(other).without_hint
 
     def __ne__(self, other: object) -> bool:
         """Return whether the labels are not equal."""
         return not self == other
 
-    def __hash__(self) -> int:
-        """Return the hash of the label, ignoring hints."""
-        return hash(self.split(";", maxsplit=1)[0])
-
     @property
     def spelling_alternatives(self) -> Labels:
         """Extract the spelling alternatives from the label."""
-        return tuple(self.__class__(label) for label in self.split(";", maxsplit=1)[0].split("|"))
+        return label_factory(self.without_hint.split(self.SPELLING_ALTERNATIVES_SEP))
 
     @property
     def hint(self) -> str:
         """Return the label hint, if any."""
-        return self.split(";")[1] if ";" in self else ""
+        return self.split(self.HINT_SEP)[1] if self.HINT_SEP in self else ""
+
+    @property
+    def without_hint(self) -> str:
+        """Return the label without the hint."""
+        return self.split(self.HINT_SEP)[0]
 
 
 Labels = tuple[Label, ...]
 
 
 def label_factory(string: str | list[str]) -> Labels:
     """Instantiate the labels from a string or list of strings."""
     labels = string if isinstance(string, list) else [string]
-    return tuple(Label(label) for label in labels)
+    return tuple(Label(label) for label in labels if not label.startswith("("))
+
+
+def meaning_factory(string: str | list[str]) -> Labels:
+    """Instantiate the meanings from a string or list of strings."""
+    meanings = string if isinstance(string, list) else [string]
+    return (Label(meanings[0].removeprefix("(").removesuffix(")")),) if meanings else Labels()
```

### Comparing `Toisto-0.8.2/src/toisto/model/quiz/progress.py` & `Toisto-0.9.0/src/toisto/model/quiz/progress.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,46 @@
 """Progress model class."""
 
 from collections import deque
 
+from toisto.model.language import Language
 from toisto.model.language.concept import Concept
 
 from .quiz import Quiz, Quizzes
 from .retention import Retention
 from .topic import Topics
 
+ProgressDict = dict[str, dict[str, str | int]]
+
 
 class Progress:
     """Keep track of progress on quizzes."""
 
-    def __init__(self, progress_dict: dict[str, dict[str, str | int]], topics: Topics) -> None:
+    def __init__(
+        self,
+        progress_dict: ProgressDict,
+        topics: Topics,
+        target_language: Language,
+        skip_concepts: int = 5,
+    ) -> None:
         self.__progress_dict = {key: Retention.from_dict(value) for key, value in progress_dict.items()}
         self.__topics = topics
-        self.__recent_concepts: deque[Concept] = deque(maxlen=2)  # Recent concepts to skip when selecting next quiz
+        self.target_language = target_language
+        self.__recent_concepts: deque[Concept] = deque(maxlen=skip_concepts)
         self.__quizzes_by_concept: dict[Concept, Quizzes] = {}
         for quiz in self.__topics.quizzes:
             self.__quizzes_by_concept.setdefault(quiz.concept.base_concept, set()).add(quiz)
 
     def increase_retention(self, quiz: Quiz) -> None:
         """Increase the retention of the quiz."""
-        self.__progress_dict.setdefault(str(quiz), Retention()).increase()
+        self.__progress_dict.setdefault(quiz.key, Retention()).increase()
 
     def reset_retention(self, quiz: Quiz) -> None:
         """Reset the retention of the quiz."""
-        self.__progress_dict.setdefault(str(quiz), Retention()).reset()
+        self.__progress_dict.setdefault(quiz.key, Retention()).reset()
 
     def next_quiz(self) -> Quiz | None:
         """Return the next quiz."""
         eligible_quizzes = {quiz for quiz in self.__topics.quizzes if self.__is_eligible(quiz)}
         quizzes_for_concepts_in_progress = {quiz for quiz in eligible_quizzes if self.__has_concept_in_progress(quiz)}
         quizzes_in_progress = {quiz for quiz in quizzes_for_concepts_in_progress if self.__in_progress(quiz)}
         for potential_quizzes in [quizzes_in_progress, quizzes_for_concepts_in_progress, eligible_quizzes]:
@@ -38,28 +48,28 @@
                 quiz = self.__sort_by_language_level(unblocked_quizzes)[0]
                 self.__recent_concepts.append(quiz.concept.base_concept)
                 return quiz
         return None
 
     def get_retention(self, quiz: Quiz) -> Retention:
         """Return the quiz retention."""
-        return self.__progress_dict.get(str(quiz), Retention())
+        return self.__progress_dict.get(quiz.key, Retention())
 
     def __is_eligible(self, quiz: Quiz) -> bool:
         """Return whether the quiz is not silenced and not the current quiz."""
         return quiz.concept.base_concept not in self.__recent_concepts and not self.get_retention(quiz).is_silenced()
 
     def __has_concept_in_progress(self, quiz: Quiz) -> bool:
         """Return whether the quiz's concept has been presented to the user before."""
         quizzes_for_same_concept = self.__quizzes_by_concept[quiz.concept.base_concept]
         return any(self.__in_progress(quiz_for_same_concept) for quiz_for_same_concept in quizzes_for_same_concept)
 
     def __in_progress(self, quiz: Quiz) -> bool:
         """Return whether the quiz has been presented to the user before."""
-        return str(quiz) in self.__progress_dict
+        return quiz.key in self.__progress_dict
 
     def __unblocked_quizzes(self, quizzes: Quizzes, eligible_quizzes: Quizzes) -> Quizzes:
         """Return the quizzes that are not blocked by other quizzes.
 
         Quiz A is blocked by quiz B if the concept of quiz A is a compound with a root that is quizzed by quiz B.
         """
         return {
@@ -67,18 +77,19 @@
             for quiz in quizzes
             if not self.__root_concepts_have_quizzes(quiz, eligible_quizzes)
             and not quiz.is_blocked_by(eligible_quizzes)
         }
 
     def __root_concepts_have_quizzes(self, quiz: Quiz, quizzes: Quizzes) -> bool:
         """Return whether the quiz's concept has root concepts that have quizzes."""
+        target_language = quiz.answer_language if "write" in quiz.quiz_types else quiz.question_language
         return any(
             other_quiz
-            for root in quiz.concept.related_concepts.roots(quiz.question_language)
-            for other_quiz in self.__quizzes_by_concept.get(root, set())
+            for root in quiz.concept.related_concepts.roots(target_language)
+            for other_quiz in self.__quizzes_by_concept.get(root.base_concept, set())
             if other_quiz != quiz and other_quiz in quizzes
         )
 
     def __sort_by_language_level(self, quizzes: Quizzes) -> list[Quiz]:
         """Sort the quizzes by the language level of the concept."""
         return sorted(quizzes, key=lambda quiz: str(quiz.concept.level))
```

### Comparing `Toisto-0.8.2/src/toisto/model/quiz/quiz.py` & `Toisto-0.9.0/src/toisto/model/quiz/quiz.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 """Quiz classes."""
 
 from __future__ import annotations
 
 from dataclasses import dataclass
 from functools import cached_property
 from itertools import chain
-from typing import Literal, cast
+from typing import Literal, cast, get_args
 
 from ..language import Language
 from ..language.concept import Concept
 from ..language.grammar import GrammaticalCategory
 from ..language.iana_language_subtag_registry import ALL_LANGUAGES
 from ..language.label import Label, Labels
 from .match import match
 
-QuizType = Literal[
-    "translate",
-    "listen",
-    "antonym",
+TranslationQuizType = Literal["read", "write"]
+ListenQuizType = Literal["listen"]
+SemanticQuizType = Literal["antonym"]
+GrammaticalQuizType = Literal[
     "pluralize",
     "singularize",
+    "diminutize",
     "masculinize",
     "feminize",
     "neuterize",
     "give positive degree",
     "give comparative degree",
     "give superlative degree",
     "give first person",
@@ -33,17 +34,19 @@
     "give present tense",
     "give past tense",
     "make declarative",
     "make interrogative",
     "affirm",
     "negate",
 ]
-GRAMMATICAL_QUIZ_TYPES: dict[GrammaticalCategory, QuizType] = {
+QuizType = Literal[TranslationQuizType, ListenQuizType, SemanticQuizType, GrammaticalQuizType]
+GRAMMATICAL_QUIZ_TYPES: dict[GrammaticalCategory, GrammaticalQuizType] = {
     "plural": "pluralize",
     "singular": "singularize",
+    "diminutive": "diminutize",
     "male": "masculinize",
     "female": "feminize",
     "neuter": "neuterize",
     "positive degree": "give positive degree",
     "comparative degree": "give comparative degree",
     "superlative degree": "give superlative degree",
     "first person": "give first person",
@@ -54,75 +57,54 @@
     "past tense": "give past tense",
     "declarative": "make declarative",
     "interrogative": "make interrogative",
     "affirmative": "affirm",
     "negative": "negate",
 }
 QUIZ_TYPE_GRAMMATICAL_CATEGORIES = {value: key for key, value in GRAMMATICAL_QUIZ_TYPES.items()}
-INSTRUCTIONS: dict[QuizType, str] = dict(
-    translate="Translate into",
+INSTRUCTIONS: dict[Literal[TranslationQuizType, ListenQuizType, SemanticQuizType], str] = dict(
+    read="Translate into",
+    write="Translate into",
     listen="Listen and write in",
     antonym="Give the [underline]antonym[/underline] in",
 )
 
 
-def instruction(*quiz_types: QuizType) -> str:
-    """Return the instruction text for the quiz types."""
-    if instruction_label := INSTRUCTIONS.get(quiz_types[0]):
-        return instruction_label
-    categories = " ".join(QUIZ_TYPE_GRAMMATICAL_CATEGORIES[quiz_type] for quiz_type in quiz_types)
-    return f"Give the [underline]{categories}[/underline] in"
-
-
 @dataclass(frozen=True)
 class Quiz:
     """Class representing a quiz."""
 
     concept: Concept
     question_language: Language
     answer_language: Language
     _question: Label
     _answers: Labels
-    quiz_types: tuple[QuizType, ...] = ("translate",)
+    quiz_types: tuple[QuizType, ...] = ("read",)
     blocked_by: tuple[Quiz, ...] = ()
     _meanings: Labels = Labels()
-    _hash: int = 0
-
-    def __post_init__(self) -> None:
-        """Initialize calculated attributes."""
-        # The dataclass is frozen, so some magic is needed to set the hash attribute.
-        super().__setattr__(
-            "_hash",
-            hash((self.question_language, self.answer_language, self.question, self.quiz_types)),
-        )
-
-    def __str__(self) -> str:
-        """Return a string version of the quiz that can be used as key in the progress dict."""
-        quiz_types = "+".join(self.quiz_types)
-        return f"{self.question_language}:{self.answer_language}:{self._question}:{quiz_types}"
 
     def __hash__(self) -> int:
         """Return a hash using the same attributes as used for testing equality."""
-        return self._hash
+        return hash(self.key)
 
     def __eq__(self, other: object) -> bool:
         """Return whether this quiz is equal to the other."""
-        if not isinstance(other, self.__class__):
-            return False
-        return (
-            self.question_language == other.question_language
-            and self.answer_language == other.answer_language
-            and self.question == other.question
-            and self.quiz_types == other.quiz_types
-        )
+        return self.key == other.key if isinstance(other, self.__class__) else False
 
     def __ne__(self, other: object) -> bool:
         """Return whether this quiz is not equal to the other."""
         return not self == other
 
+    @cached_property
+    def key(self) -> str:
+        """Return a string version of the quiz that can be used as key in the progress dict."""
+        concept_id = self.concept.base_concept.concept_id
+        quiz_types = "+".join(self.quiz_types)
+        return f"{concept_id}:{self.question_language}:{self.answer_language}:{self.question}:{quiz_types}"
+
     def is_correct(self, guess: Label) -> bool:
         """Return whether the guess is correct."""
         return match(guess, *self.answers)
 
     @cached_property
     def question(self) -> Label:
         """Return the first spelling alternative of the question."""
@@ -142,23 +124,31 @@
     @property
     def meanings(self) -> Labels:
         """Return the first spelling alternative of the meanings."""
         return Labels(meaning.spelling_alternatives[0] for meaning in self._meanings)
 
     def other_answers(self, guess: Label) -> Labels:
         """Return the answers not equal to the guess."""
-        if self.quiz_types == ("listen",):
+        if self.quiz_types[0] in get_args(ListenQuizType):
             return Labels()  # Other answers doesn't make sense if the user has to type what is spoken
         return tuple(answer for answer in self.answers if not match(guess, answer))
 
     def instruction(self) -> str:
         """Generate the quiz instruction."""
         hint = self._question.hint
-        hint = f" ({hint})" if self.question_language != self.answer_language and hint else ""
-        return f"{instruction(*self.quiz_types)} {ALL_LANGUAGES[self.answer_language]}{hint}"
+        hint_text = f" ({hint})" if self.question_language != self.answer_language and hint else ""
+        if self.quiz_types[0] in get_args(GrammaticalQuizType):
+            categories = " ".join(
+                QUIZ_TYPE_GRAMMATICAL_CATEGORIES[cast(GrammaticalQuizType, quiz_type)] for quiz_type in self.quiz_types
+            )
+            instruction_text = f"Give the [underline]{categories}[/underline] in"
+        else:
+            quiz_type = cast(Literal[TranslationQuizType, ListenQuizType, SemanticQuizType], self.quiz_types[0])
+            instruction_text = INSTRUCTIONS[quiz_type]
+        return f"{instruction_text} {ALL_LANGUAGES[self.answer_language]}{hint_text}"
 
     def is_blocked_by(self, quizzes: Quizzes) -> bool:
         """Return whether this quiz should come after any of the given quizzes."""
         return bool(set(self.blocked_by) & quizzes)
 
 
 Quizzes = set[Quiz]
```

### Comparing `Toisto-0.8.2/src/toisto/model/quiz/quiz_factory.py` & `Toisto-0.9.0/src/toisto/model/quiz/quiz_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from toisto.tools import zip_and_cycle
 
 from ..language import Language
 from ..language.concept import Concept
 from .quiz import GRAMMATICAL_QUIZ_TYPES, Quiz, QuizType, Quizzes
 
 
-@dataclass
+@dataclass(frozen=True)
 class QuizFactory:
     """Create quizzes for concepts."""
 
     target_language: Language
     source_language: Language
 
     def create_quizzes(self, *concepts: Concept) -> Quizzes:
@@ -51,19 +51,19 @@
         """Create translation quizzes for the concept."""
         target_language, source_language = self.target_language, self.source_language
         target_labels, source_labels = concept.labels(target_language), concept.labels(source_language)
         if not target_labels or not source_labels:
             return Quizzes()
         blocked_by = tuple(previous_quizzes)
         target_to_source = Quizzes(
-            Quiz(concept, target_language, source_language, target_label, source_labels, blocked_by=blocked_by)
+            Quiz(concept, target_language, source_language, target_label, source_labels, ("read",), blocked_by)
             for target_label in target_labels
         )
         source_to_target = Quizzes(
-            Quiz(concept, source_language, target_language, source_label, target_labels, blocked_by=blocked_by)
+            Quiz(concept, source_language, target_language, source_label, target_labels, ("write",), blocked_by)
             for source_label in source_labels
         )
         return target_to_source | source_to_target
 
     def listening_quizzes(self, concept: Concept, previous_quizzes: Quizzes) -> Quizzes:
         """Create listening quizzes for the concept."""
         target_language, source_language = self.target_language, self.source_language
@@ -77,54 +77,56 @@
 
     def grammatical_quizzes(self, concept: Concept, previous_quizzes: Quizzes) -> Quizzes:
         """Create grammatical quizzes for the concept."""
         target_language, source_language = self.target_language, self.source_language
         blocked_by = tuple(previous_quizzes)
         quizzes = Quizzes()
         for concept1, concept2 in paired_leaf_concepts(concept):
+            quiz_types = grammatical_quiz_types(concept1, concept2)
+            if not quiz_types:
+                continue
             labels1, labels2 = concept1.labels(target_language), concept2.labels(target_language)
             meanings = concept1.meanings(source_language) + concept2.meanings(source_language)
-            quiz_types = grammatical_quiz_types(concept1, concept2)
             quizzes |= Quizzes(
                 Quiz(concept, target_language, target_language, label1, (label2,), quiz_types, blocked_by, meanings)
                 for label1, label2 in zip(labels1, labels2, strict=False)
                 if label1 != label2
             )
         return quizzes
 
     def antonym_quizzes(self, concept: Concept, previous_quizzes: Quizzes) -> Quizzes:
         """Create antonym quizzes for the concept."""
         target_language, source_language = self.target_language, self.source_language
         labels = concept.labels(target_language)
-        blocked_by = tuple(previous_quizzes)
         quizzes = Quizzes()
         for antonym in concept.antonyms:
+            antonym_quizzes = self.translation_quizzes(antonym, Quizzes()) | self.listening_quizzes(antonym, Quizzes())
             antonym_labels = antonym.labels(target_language)
             meanings = concept.meanings(source_language) + antonym.meanings(source_language)
             quizzes |= Quizzes(
                 Quiz(
                     concept,
                     target_language,
                     target_language,
                     label,
                     antonym_labels,
                     ("antonym",),
-                    blocked_by,
+                    tuple(previous_quizzes | antonym_quizzes),
                     meanings,
                 )
                 for label in labels
             )
         return quizzes
 
 
 def grammatical_quiz_types(concept1: Concept, concept2: Concept) -> tuple[QuizType, ...]:
     """Return the quiz types to change the grammatical category of concept1 into that of concept2."""
     quiz_types = []
     for category1, category2 in zip_longest(concept1.grammatical_categories(), concept2.grammatical_categories()):
-        if category1 != category2 and category2 is not None:
+        if category1 != category2 and category2 in GRAMMATICAL_QUIZ_TYPES:
             quiz_types.append(GRAMMATICAL_QUIZ_TYPES[category2])
     return tuple(quiz_types)
 
 
 def paired_leaf_concepts(concept: Concept) -> Iterable[tuple[Concept, Concept]]:
     """Pair the leaf concepts from the constituent concepts."""
     for concept_group in zip_and_cycle(*[list(constituent.leaf_concepts()) for constituent in concept.constituents]):
```

### Comparing `Toisto-0.8.2/src/toisto/model/quiz/retention.py` & `Toisto-0.9.0/src/toisto/model/quiz/retention.py`

 * *Files identical despite different names*

### Comparing `Toisto-0.8.2/src/toisto/model/quiz/topic.py` & `Toisto-0.9.0/src/toisto/model/quiz/topic.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,19 +15,19 @@
     """Collection of quizzes for concepts centered around a topic."""
 
     name: str
     concepts: Concepts
     quizzes: Quizzes
 
     def __hash__(self) -> int:
-        """Return the hash of the file name."""
+        """Return the hash of the topic name."""
         return hash(self.name)
 
 
-@dataclass
+@dataclass(frozen=True)
 class Topics:
     """Collection of topics."""
 
     topics: set[Topic] = field(default_factory=set)
 
     @property
     def quizzes(self) -> Quizzes:
```

### Comparing `Toisto-0.8.2/src/toisto/persistence/config.py` & `Toisto-0.9.0/src/toisto/persistence/config.py`

 * *Files identical despite different names*

### Comparing `Toisto-0.8.2/src/toisto/persistence/iana_language_subtag_registry.py` & `Toisto-0.9.0/src/toisto/persistence/iana_language_subtag_registry.py`

 * *Files identical despite different names*

### Comparing `Toisto-0.8.2/src/toisto/persistence/json_file.py` & `Toisto-0.9.0/src/toisto/persistence/json_file.py`

 * *Files identical despite different names*

### Comparing `Toisto-0.8.2/src/toisto/ui/cli.py` & `Toisto-0.9.0/src/toisto/ui/cli.py`

 * *Files identical despite different names*

### Comparing `Toisto-0.8.2/src/toisto/ui/dictionary.py` & `Toisto-0.9.0/src/toisto/ui/dictionary.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,16 +10,16 @@
     return sep.join(f'"{linkify(text)}"' for text in texts)
 
 
 def linkify(text: str) -> str:
     """Return a version of the text where each word is turned into a link to a dictionary."""
     linkified_words = []
     for word in text.split():
-        prefix, word, postfix = split_punctuation(word)
-        linkified_words.append(f"{prefix}[link={DICTIONARY_URL}/{word.lower()}]{word}[/link]{postfix}")
+        prefix, infix, postfix = split_punctuation(word)
+        linkified_words.append(f"{prefix}[link={DICTIONARY_URL}/{infix.lower()}]{infix}[/link]{postfix}")
     return " ".join(linkified_words)
 
 
 def split_punctuation(text: str) -> tuple[str, str, str]:
     """Return a tuple of prefixed punctuation, the text without punctuation, and postfix punctuation."""
     stripped_text = text.strip(punctuation)
     stripped_text_start = text.find(stripped_text)
```

### Comparing `Toisto-0.8.2/src/toisto/ui/diff.py` & `Toisto-0.9.0/src/toisto/ui/diff.py`

 * *Files identical despite different names*

### Comparing `Toisto-0.8.2/src/toisto/ui/format.py` & `Toisto-0.9.0/src/toisto/ui/format.py`

 * *Files identical despite different names*

### Comparing `Toisto-0.8.2/src/toisto/ui/speech.py` & `Toisto-0.9.0/src/toisto/ui/speech.py`

 * *Files identical despite different names*

### Comparing `Toisto-0.8.2/src/toisto/ui/text.py` & `Toisto-0.9.0/src/toisto/ui/text.py`

 * *Files identical despite different names*

### Comparing `Toisto-0.8.2/src/topics/animals.json` & `Toisto-0.9.0/src/topics/animals.json`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8768939393939394%*

 * *Differences: {"'animal'": "{'singular': {'en': 'animal', 'fi': 'eläin', 'nl': 'het dier'}, 'plural': {'en': "*

 * *             "'animals', 'fi': 'eläimet', 'nl': 'de dieren'}}",*

 * * "'bear'": "{'singular': {'en': 'bear', 'fi': 'karhu', 'nl': 'de beer'}, 'plural': {'en': 'bears', "*

 * *           "'fi': 'karhut', 'nl': 'de beren'}}",*

 * * "'bird'": "{'singular': {'en': 'bird', 'fi': 'lintu', 'nl': 'de vogel'}, 'plural': {'en': "*

 * *           "'birds', 'fi': 'linnut', 'nl': 'de vogels'}}",*

 * * "'cat'": "{'singular': {'en': 'cat', 'fi': 'kiss […]*

```diff
@@ -4,411 +4,434 @@
             "A1": [
                 "EP",
                 "KK",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Animals",
-            "fi": "El\u00e4imet",
-            "nl": "De dieren"
+            "en": "animals",
+            "fi": "el\u00e4imet",
+            "nl": "de dieren"
         },
         "singular": {
-            "en": "Animal",
-            "fi": "El\u00e4in",
-            "nl": "Het dier"
+            "en": "animal",
+            "fi": "el\u00e4in",
+            "nl": "het dier"
         }
     },
     "bear": {
         "level": {
             "A2": "EP",
             "B2": "OD"
         },
         "plural": {
-            "en": "Bears",
-            "fi": "Karhut",
-            "nl": "De beren"
+            "en": "bears",
+            "fi": "karhut",
+            "nl": "de beren"
         },
         "singular": {
-            "en": "Bear",
-            "fi": "Karhu",
-            "nl": "De beer"
+            "en": "bear",
+            "fi": "karhu",
+            "nl": "de beer"
         }
     },
     "bird": {
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Birds",
-            "fi": "Linnut",
-            "nl": "De vogels"
+            "en": "birds",
+            "fi": "linnut",
+            "nl": "de vogels"
         },
         "singular": {
-            "en": "Bird",
-            "fi": "Lintu",
-            "nl": "De vogel"
+            "en": "bird",
+            "fi": "lintu",
+            "nl": "de vogel"
         }
     },
     "cat": {
         "level": {
             "A1": [
                 "EP",
                 "KK",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Cats",
-            "fi": "Kissat",
-            "nl": "De katten"
+            "en": "cats",
+            "fi": "kissat",
+            "nl": "de katten"
         },
         "singular": {
-            "en": "Cat",
-            "fi": "Kissa",
-            "nl": "De kat"
+            "en": "cat",
+            "fi": "kissa",
+            "nl": "de kat"
         }
     },
     "cow": {
         "level": {
             "A1": "OD"
         },
         "plural": {
-            "en": "Cows",
-            "fi": "Lehm\u00e4t",
-            "nl": "De koeien"
+            "en": "cows",
+            "fi": "lehm\u00e4t",
+            "nl": "de koeien"
         },
         "singular": {
-            "en": "Cow",
-            "fi": "Lehm\u00e4",
-            "nl": "De koe"
+            "en": "cow",
+            "fi": "lehm\u00e4",
+            "nl": "de koe"
         }
     },
     "crab": {
         "level": {
             "B2": [
                 "EP",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Crabs",
-            "fi": "Ravut",
-            "nl": "De krabben"
+            "en": "crabs",
+            "fi": "ravut",
+            "nl": "de krabben"
         },
         "singular": {
-            "en": "Crab",
-            "fi": "Rapu",
-            "nl": "De krab"
+            "en": "crab",
+            "fi": "rapu",
+            "nl": "de krab"
         }
     },
     "deer": {
         "level": {
             "B2": [
                 "EP",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Deer",
-            "fi": "Peurat",
-            "nl": "De herten"
+            "en": "deer",
+            "fi": "peurat",
+            "nl": "de herten"
         },
         "singular": {
-            "en": "Deer",
-            "fi": "Peura",
-            "nl": "Het hert"
+            "en": "deer",
+            "fi": "peura",
+            "nl": "het hert"
         }
     },
     "dog": {
         "level": {
             "A1": [
                 "EP",
                 "KK",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Dogs",
-            "fi": "Koirat",
-            "nl": "De honden"
+            "en": "dogs",
+            "fi": "koirat",
+            "nl": "de honden"
         },
         "singular": {
-            "en": "Dog",
-            "fi": "Koira",
-            "nl": "De hond"
+            "en": "dog",
+            "fi": "koira",
+            "nl": "de hond"
         }
     },
     "duck": {
         "level": {
             "A2": [
                 "EP",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Ducks",
-            "fi": "Ankat",
-            "nl": "De eenden"
+            "en": "ducks",
+            "fi": "ankat",
+            "nl": "de eenden"
         },
         "singular": {
-            "en": "Duck",
-            "fi": "Ankka",
-            "nl": "De eend"
+            "en": "duck",
+            "fi": "ankka",
+            "nl": "de eend"
         }
     },
     "elephant": {
         "level": {
             "A1": "OD",
             "A2": "EP"
         },
         "plural": {
-            "en": "Elephants",
+            "en": "elephants",
             "fi": [
-                "Elefantit",
-                "Norsut"
+                "elefantit",
+                "norsut"
             ],
-            "nl": "De olifanten"
+            "nl": "de olifanten"
         },
         "singular": {
-            "en": "Elephant",
+            "en": "elephant",
             "fi": [
-                "Elefantti",
-                "Norsu"
+                "elefantti",
+                "norsu"
             ],
-            "nl": "De olifant"
+            "nl": "de olifant"
         }
     },
     "goose": {
         "level": {
             "A2": "OD",
             "none": "EP"
         },
         "plural": {
-            "en": "Geese",
-            "fi": "Hanhet",
-            "nl": "De ganzen"
+            "en": "geese",
+            "fi": "hanhet",
+            "nl": "de ganzen"
         },
         "singular": {
-            "en": "Goose",
-            "fi": "Hanhi",
-            "nl": "De gans"
+            "en": "goose",
+            "fi": "hanhi",
+            "nl": "de gans"
         }
     },
     "horn": {
         "level": {
             "C1": [
                 "EP",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Horns",
-            "fi": "Sarvet",
-            "nl": "De hoorns"
+            "en": "horns",
+            "fi": "sarvet",
+            "nl": "de hoorns"
         },
         "singular": {
-            "en": "Horn",
-            "fi": "Sarvi",
-            "nl": "De hoorn"
+            "en": "horn",
+            "fi": "sarvi",
+            "nl": "de hoorn"
         }
     },
     "horse": {
         "level": {
             "A1": [
                 "EP",
                 "KK",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Horses",
-            "fi": "Hevoset",
-            "nl": "De paarden"
+            "en": "horses",
+            "fi": "hevoset",
+            "nl": "de paarden"
         },
         "singular": {
-            "en": "Horse",
-            "fi": "Hevonen",
-            "nl": "Het paard"
+            "en": "horse",
+            "fi": "hevonen",
+            "nl": "het paard"
         }
     },
     "mouse": {
         "level": {
             "A1": "OD",
             "A2": "EP"
         },
         "plural": {
-            "en": "Mice",
-            "fi": "Hiiret",
-            "nl": "De muizen"
+            "en": "mice",
+            "fi": "hiiret",
+            "nl": "de muizen"
         },
         "singular": {
-            "en": "Mouse",
-            "fi": "Hiiri",
-            "nl": "De muis"
+            "en": "mouse",
+            "fi": "hiiri",
+            "nl": "de muis"
         }
     },
     "pet": {
         "level": {
             "A1": "EP",
             "A2": "OD"
         },
         "plural": {
-            "en": "Pets",
+            "en": "pets",
             "fi": [
-                "Lemmikit",
-                "Kotiel\u00e4imet"
+                "lemmikit",
+                "kotiel\u00e4imet"
             ],
-            "nl": "De huisdieren"
+            "nl": "de huisdieren"
         },
         "roots": {
             "fi": [
                 "animal",
                 "home"
             ],
             "nl": [
                 "animal",
                 "house"
             ]
         },
         "singular": {
-            "en": "Pet",
+            "en": "pet",
             "fi": [
-                "Lemmikki",
-                "Kotiel\u00e4in"
+                "lemmikki",
+                "kotiel\u00e4in"
             ],
-            "nl": "Het huisdier"
+            "nl": "het huisdier"
         }
     },
     "pig": {
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Pigs",
+            "en": "pigs",
             "fi": [
-                "Possut",
-                "Siat"
+                "possut",
+                "siat"
             ],
-            "nl": "De varkens"
+            "nl": "de varkens"
         },
         "singular": {
-            "en": "Pig",
+            "en": "pig",
             "fi": [
-                "Possu",
-                "Sika"
+                "possu",
+                "sika"
             ],
-            "nl": "Het varken"
+            "nl": "het varken"
         }
     },
     "rabbit": {
         "level": {
             "A2": [
                 "EP",
                 "OD"
             ]
         },
         "plural": {
             "en": [
-                "Rabbits",
-                "Bunnies"
+                "rabbits",
+                "bunnies"
             ],
             "fi": [
-                "J\u00e4nikset",
-                "Puput"
+                "j\u00e4nikset",
+                "puput"
             ],
-            "nl": "De konijnen"
+            "nl": "de konijnen"
         },
         "singular": {
             "en": [
-                "Rabbit",
-                "Bunny"
+                "rabbit",
+                "bunny"
             ],
             "fi": [
-                "J\u00e4nis",
-                "Pupu"
+                "j\u00e4nis",
+                "pupu"
             ],
-            "nl": "Het konijn"
+            "nl": "het konijn"
+        }
+    },
+    "reindeer": {
+        "level": {
+            "B2": "OD",
+            "none": "EP"
+        },
+        "plural": {
+            "en": "reindeer;plural",
+            "fi": "porot",
+            "nl": "rendieren"
+        },
+        "roots": {
+            "en": "deer",
+            "nl": [
+                "to run",
+                "animal"
+            ]
+        },
+        "singular": {
+            "en": "reindeer;singular",
+            "fi": "poro",
+            "nl": "rendier"
         }
     },
     "rhino": {
         "level": {
             "C1": "OD",
             "none": "EP"
         },
         "plural": {
-            "en": "Rhinoceroses|Rhinos",
-            "fi": "Sarvikuonot",
-            "nl": "De neushoorns"
+            "en": "rhinoceroses|rhinos",
+            "fi": "sarvikuonot",
+            "nl": "de neushoorns"
         },
         "roots": {
             "fi": [
                 "horn"
             ],
             "nl": [
                 "horn",
                 "nose"
             ]
         },
         "singular": {
-            "en": "Rhinoceros|Rhino",
-            "fi": "Sarvikuono",
-            "nl": "De neushoorn"
+            "en": "rhinoceros|rhino",
+            "fi": "sarvikuono",
+            "nl": "de neushoorn"
         }
     },
     "sheep": {
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Sheep",
-            "fi": "Lampaat",
-            "nl": "De schapen"
+            "en": "sheep",
+            "fi": "lampaat",
+            "nl": "de schapen"
         },
         "singular": {
-            "en": "Sheep",
-            "fi": "Lammas",
-            "nl": "Het schaap"
+            "en": "sheep",
+            "fi": "lammas",
+            "nl": "het schaap"
         }
     },
     "spider": {
         "level": {
             "A2": "OD",
             "B1": "EP"
         },
         "plural": {
-            "en": "Spiders",
-            "fi": "H\u00e4m\u00e4h\u00e4kit",
-            "nl": "De spinnen"
+            "en": "spiders",
+            "fi": "h\u00e4m\u00e4h\u00e4kit",
+            "nl": "de spinnen"
         },
         "singular": {
-            "en": "Spider",
-            "fi": "H\u00e4m\u00e4h\u00e4kki",
-            "nl": "De spin"
+            "en": "spider",
+            "fi": "h\u00e4m\u00e4h\u00e4kki",
+            "nl": "de spin"
         }
     },
     "tail": {
         "level": {
             "B1": "OD",
             "B2": "EP"
         },
         "plural": {
-            "en": "Tails",
-            "fi": "H\u00e4nn\u00e4t",
-            "nl": "De staarten"
+            "en": "tails",
+            "fi": "h\u00e4nn\u00e4t",
+            "nl": "de staarten"
         },
         "singular": {
-            "en": "Tail",
-            "fi": "H\u00e4nt\u00e4",
-            "nl": "De staart"
+            "en": "tail",
+            "fi": "h\u00e4nt\u00e4",
+            "nl": "de staart"
         }
     }
 }
```

### Comparing `Toisto-0.8.2/src/topics/body.json` & `Toisto-0.9.0/src/topics/body.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.91875%*

 * *Differences: {"'arm'": "{'singular': {'en': 'arm', 'fi': 'käsivarsi', 'nl': 'de arm'}, 'plural': {'en': 'arms', "*

 * *          "'fi': 'käsivarret', 'nl': 'de armen'}}",*

 * * "'back'": "{'singular': {'en': 'back', 'fi': 'selkä', 'nl': 'de rug'}, 'plural': {'en': 'backs', "*

 * *           "'fi': 'selät', 'nl': 'de ruggen'}}",*

 * * "'belly'": "{'singular': {'en': 'belly', 'fi': ['maha', 'masu'], 'nl': 'de buik'}, 'plural': "*

 * *            "{'en': 'bellies', 'fi': ['mahat', 'masut'], 'nl': 'de buiken'}}",*

 * * "'body'": "{'singular': {'en': 'bo […]*

```diff
@@ -3,378 +3,378 @@
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Arms",
-            "fi": "K\u00e4sivarret",
-            "nl": "De armen"
+            "en": "arms",
+            "fi": "k\u00e4sivarret",
+            "nl": "de armen"
         },
         "roots": {
             "fi": "hand"
         },
         "singular": {
-            "en": "Arm",
-            "fi": "K\u00e4sivarsi",
-            "nl": "De arm"
+            "en": "arm",
+            "fi": "k\u00e4sivarsi",
+            "nl": "de arm"
         }
     },
     "back": {
         "level": {
             "A1": "OD",
             "A2": "EP"
         },
         "plural": {
-            "en": "Backs",
-            "fi": "Sel\u00e4t",
-            "nl": "De ruggen"
+            "en": "backs",
+            "fi": "sel\u00e4t",
+            "nl": "de ruggen"
         },
         "singular": {
-            "en": "Back",
-            "fi": "Selk\u00e4",
-            "nl": "De rug"
+            "en": "back",
+            "fi": "selk\u00e4",
+            "nl": "de rug"
         }
     },
     "belly": {
         "level": {
             "C2": "OD",
             "none": "EP"
         },
         "plural": {
-            "en": "Bellies",
+            "en": "bellies",
             "fi": [
-                "Mahat",
-                "Masut"
+                "mahat",
+                "masut"
             ],
-            "nl": "De buiken"
+            "nl": "de buiken"
         },
         "singular": {
-            "en": "Belly",
+            "en": "belly",
             "fi": [
-                "Maha",
-                "Masu"
+                "maha",
+                "masu"
             ],
-            "nl": "De buik"
+            "nl": "de buik"
         }
     },
     "body": {
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Bodies",
+            "en": "bodies",
             "fi": [
-                "Vartalot",
-                "Kehot"
+                "vartalot",
+                "kehot"
             ],
-            "nl": "De lichamen"
+            "nl": "de lichamen"
         },
         "singular": {
-            "en": "Body",
+            "en": "body",
             "fi": [
-                "Vartalo",
-                "Keho"
+                "vartalo",
+                "keho"
             ],
-            "nl": "Het lichaam"
+            "nl": "het lichaam"
         }
     },
     "ear": {
         "level": {
             "A1": [
                 "EP",
                 "KK",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Ears",
-            "fi": "Korvat",
-            "nl": "De oren"
+            "en": "ears",
+            "fi": "korvat",
+            "nl": "de oren"
         },
         "singular": {
-            "en": "Ear",
-            "fi": "Korva",
-            "nl": "Het oor"
+            "en": "ear",
+            "fi": "korva",
+            "nl": "het oor"
         }
     },
     "eye": {
         "level": {
             "A1": [
                 "EP",
                 "KK",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Eyes",
-            "fi": "Silm\u00e4t",
-            "nl": "De ogen"
+            "en": "eyes",
+            "fi": "silm\u00e4t",
+            "nl": "de ogen"
         },
         "singular": {
-            "en": "Eye",
-            "fi": "Silm\u00e4",
-            "nl": "Het oog"
+            "en": "eye",
+            "fi": "silm\u00e4",
+            "nl": "het oog"
         }
     },
     "finger": {
         "level": {
             "A1": "KK",
             "A2": [
                 "EP",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Fingers",
-            "fi": "Sormet",
-            "nl": "De vingers"
+            "en": "fingers",
+            "fi": "sormet",
+            "nl": "de vingers"
         },
         "singular": {
-            "en": "Finger",
-            "fi": "Sormi",
-            "nl": "De vinger"
+            "en": "finger",
+            "fi": "sormi",
+            "nl": "de vinger"
         }
     },
     "foot": {
         "level": {
             "A1": [
                 "EP",
                 "KK",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Feet",
-            "fi": "Jalat;lower part",
-            "nl": "De voeten"
+            "en": "feet",
+            "fi": "jalat;lower part",
+            "nl": "de voeten"
         },
         "singular": {
-            "en": "Foot",
-            "fi": "Jalka;lower part",
-            "nl": "De voet"
+            "en": "foot",
+            "fi": "jalka;lower part",
+            "nl": "de voet"
         }
     },
     "hair": {
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Hairs",
-            "fi": "Hiukset",
-            "nl": "De haren"
+            "en": "hairs",
+            "fi": "hiukset",
+            "nl": "de haren"
         },
         "singular": {
-            "en": "Hair",
-            "fi": "Hius",
+            "en": "hair",
+            "fi": "hius",
             "nl": [
-                "De haar",
-                "Het haar"
+                "de haar",
+                "het haar"
             ]
         }
     },
     "hand": {
         "level": {
             "A1": [
                 "EP",
                 "KK",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Hands",
-            "fi": "K\u00e4det",
-            "nl": "De handen"
+            "en": "hands",
+            "fi": "k\u00e4det",
+            "nl": "de handen"
         },
         "singular": {
-            "en": "Hand",
-            "fi": "K\u00e4si",
-            "nl": "De hand"
+            "en": "hand",
+            "fi": "k\u00e4si",
+            "nl": "de hand"
         }
     },
     "head": {
         "level": {
             "A1": [
                 "EP",
                 "KK",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Heads",
-            "fi": "P\u00e4\u00e4t",
-            "nl": "De hoofden"
+            "en": "heads",
+            "fi": "p\u00e4\u00e4t",
+            "nl": "de hoofden"
         },
         "singular": {
-            "en": "Head",
-            "fi": "P\u00e4\u00e4",
-            "nl": "Het hoofd"
+            "en": "head",
+            "fi": "p\u00e4\u00e4",
+            "nl": "het hoofd"
         }
     },
     "knee": {
         "level": {
             "A2": "OD",
             "B1": "EP"
         },
         "plural": {
-            "en": "Knees",
-            "fi": "Polvet",
-            "nl": "De knie\u00ebn"
+            "en": "knees",
+            "fi": "polvet",
+            "nl": "de knie\u00ebn"
         },
         "singular": {
-            "en": "Knee",
-            "fi": "Polvi",
-            "nl": "De knie"
+            "en": "knee",
+            "fi": "polvi",
+            "nl": "de knie"
         }
     },
     "leg": {
         "level": {
             "A1": [
                 "EP",
                 "KK",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Legs",
-            "fi": "Jalat;upper part",
-            "nl": "De benen"
+            "en": "legs",
+            "fi": "jalat;upper part",
+            "nl": "de benen"
         },
         "singular": {
-            "en": "Leg",
-            "fi": "Jalka;upper part",
-            "nl": "Het been"
+            "en": "leg",
+            "fi": "jalka;upper part",
+            "nl": "het been"
         }
     },
     "lip": {
         "level": {
             "B1": [
                 "EP",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Lips",
-            "fi": "Huulet",
-            "nl": "De lippen"
+            "en": "lips",
+            "fi": "huulet",
+            "nl": "de lippen"
         },
         "singular": {
-            "en": "Lip",
-            "fi": "Huuli",
-            "nl": "De lip"
+            "en": "lip",
+            "fi": "huuli",
+            "nl": "de lip"
         }
     },
     "mouth": {
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Mouths",
-            "fi": "Suut",
-            "nl": "De monden"
+            "en": "mouths",
+            "fi": "suut",
+            "nl": "de monden"
         },
         "singular": {
-            "en": "Mouth",
-            "fi": "Suu",
-            "nl": "De mond"
+            "en": "mouth",
+            "fi": "suu",
+            "nl": "de mond"
         }
     },
     "nose": {
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Noses",
-            "fi": "Nen\u00e4t",
-            "nl": "De neuzen"
+            "en": "noses",
+            "fi": "nen\u00e4t",
+            "nl": "de neuzen"
         },
         "singular": {
-            "en": "Nose",
-            "fi": "Nen\u00e4",
-            "nl": "De neus"
+            "en": "nose",
+            "fi": "nen\u00e4",
+            "nl": "de neus"
         }
     },
     "shoulder": {
         "level": {
             "A2": "OD",
             "B1": "EP"
         },
         "plural": {
-            "en": "Shoulders",
-            "fi": "Olkap\u00e4\u00e4t",
-            "nl": "De schouders"
+            "en": "shoulders",
+            "fi": "olkap\u00e4\u00e4t",
+            "nl": "de schouders"
         },
         "roots": {
             "fi": "head"
         },
         "singular": {
-            "en": "Shoulder",
-            "fi": "Olkap\u00e4\u00e4",
-            "nl": "De schouder"
+            "en": "shoulder",
+            "fi": "olkap\u00e4\u00e4",
+            "nl": "de schouder"
         }
     },
     "stomach": {
         "level": {
             "A2": [
                 "EP",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Stomachs",
-            "fi": "Vatsat",
-            "nl": "De magen"
+            "en": "stomachs",
+            "fi": "vatsat",
+            "nl": "de magen"
         },
         "singular": {
-            "en": "Stomach",
-            "fi": "Vatsa",
-            "nl": "De maag"
+            "en": "stomach",
+            "fi": "vatsa",
+            "nl": "de maag"
         }
     },
     "toe": {
         "level": {
             "A2": "EP",
             "B1": "OD"
         },
         "plural": {
-            "en": "Toes",
-            "fi": "Varpaat",
-            "nl": "De tenen"
+            "en": "toes",
+            "fi": "varpaat",
+            "nl": "de tenen"
         },
         "singular": {
-            "en": "Toe",
-            "fi": "Varvas",
-            "nl": "De teen"
+            "en": "toe",
+            "fi": "varvas",
+            "nl": "de teen"
         }
     },
     "tooth": {
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Teeth",
-            "fi": "Hampaat",
-            "nl": "De tanden"
+            "en": "teeth",
+            "fi": "hampaat",
+            "nl": "de tanden"
         },
         "singular": {
-            "en": "Tooth",
-            "fi": "Hammas",
-            "nl": "De tand"
+            "en": "tooth",
+            "fi": "hammas",
+            "nl": "de tand"
         }
     }
 }
```

### Comparing `Toisto-0.8.2/src/topics/city.json` & `Toisto-0.9.0/src/topics/food.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Differences: {'replace': "OrderedDict([('food', OrderedDict([('level', OrderedDict([('A1', ['EP', 'KK', "*

 * *            "'OD'])])), ('singular', OrderedDict([('en', 'food'), ('fi', 'ruoka'), ('nl', 'het "*

 * *            "voedsel')])), ('plural', OrderedDict([('en', 'foods'), ('fi', 'ruoat')]))])), "*

 * *            "('orange (fruit)', OrderedDict([('level', OrderedDict([('A1', ['EP', 'OD'])])), "*

 * *            "('roots', OrderedDict([('en', 'orange'), ('nl', 'apple')])), ('singular', "*

 * *            "OrderedDict([('en', 'orange'), ( […]*

```diff
@@ -1,493 +1,768 @@
 {
-    "I am in the office": {
-        "en": "I am in the office|I'm in the office",
-        "fi": "Min\u00e4 olen toimistolla|Olen toimistolla",
-        "nl": "Ik ben op kantoor",
-        "roots": [
-            "to be",
-            "office"
-        ]
-    },
-    "airport": {
+    "apple": {
         "level": {
-            "A1": "OD",
-            "A2": "EP"
+            "A1": [
+                "EP",
+                "OD"
+            ]
         },
         "plural": {
-            "en": "Airports",
-            "fi": "Lentokent\u00e4t",
-            "nl": "De vliegvelden"
+            "en": "apples",
+            "fi": "omenat",
+            "nl": "de appels"
         },
-        "roots": {
-            "en": "port"
+        "singular": {
+            "en": "apple",
+            "fi": "omena",
+            "nl": "de appel"
+        }
+    },
+    "banana": {
+        "level": {
+            "A1": [
+                "EP",
+                "OD"
+            ]
+        },
+        "plural": {
+            "en": "bananas",
+            "fi": "banaanit",
+            "nl": "de bananen"
         },
         "singular": {
-            "en": "Airport",
-            "fi": "Lentokentt\u00e4",
-            "nl": "Het vliegveld"
+            "en": "banana",
+            "fi": "banaani",
+            "nl": "de banaan"
         }
     },
-    "bridge": {
+    "bean": {
         "level": {
             "A2": [
                 "EP",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Bridges",
-            "fi": "Sillat",
-            "nl": "De bruggen"
+            "en": "beans",
+            "fi": "pavut",
+            "nl": "de bonen"
         },
         "singular": {
-            "en": "Bridge",
-            "fi": "Silta",
-            "nl": "De brug"
+            "en": "bean",
+            "fi": "papu",
+            "nl": "de boon"
         }
     },
-    "building": {
+    "bread": {
         "level": {
             "A1": [
-                "KK",
+                "EP",
                 "OD"
-            ],
-            "A2": "EP"
+            ]
         },
         "plural": {
-            "en": "Buildings",
-            "fi": "Rakennukset",
-            "nl": "De gebouwen"
+            "en": "breads",
+            "fi": "leiv\u00e4t",
+            "nl": "de broden"
         },
         "singular": {
-            "en": "Building",
-            "fi": "Rakennus",
-            "nl": "Het gebouw"
+            "en": "bread",
+            "fi": "leip\u00e4",
+            "nl": "het brood"
         }
     },
-    "capital": {
+    "cake": {
         "level": {
-            "A1": "OD",
-            "A2": "EP"
+            "A1": [
+                "EP",
+                "OD"
+            ]
         },
         "plural": {
-            "en": "Capitals",
-            "fi": "P\u00e4\u00e4kaupungit",
-            "nl": "De hoofdsteden"
+            "en": "cakes",
+            "fi": "kakut",
+            "nl": "de taarten"
         },
-        "roots": {
-            "fi": [
-                "city",
-                "head"
-            ],
-            "nl": [
-                "city",
-                "head"
+        "singular": {
+            "en": "cake",
+            "fi": "kakku",
+            "nl": "de taart"
+        }
+    },
+    "cauliflower": {
+        "level": {
+            "C1": "OD",
+            "none": "EP"
+        },
+        "plural": {
+            "en": "cauliflowers",
+            "fi": "kukkakaalit",
+            "nl": "de bloemkolen"
+        },
+        "roots": "flower",
+        "singular": {
+            "en": "cauliflower",
+            "fi": "kukkakaali",
+            "nl": "de bloemkool"
+        }
+    },
+    "cheese": {
+        "level": {
+            "A1": [
+                "EP",
+                "OD"
             ]
         },
+        "plural": {
+            "en": "cheeses",
+            "fi": "juustot",
+            "nl": "de kazen"
+        },
         "singular": {
-            "en": "Capital",
-            "fi": "P\u00e4\u00e4kaupunki",
-            "nl": "De hoofdstad"
+            "en": "cheese",
+            "fi": "juusto",
+            "nl": "de kaas"
         }
     },
-    "castle": {
+    "cherry": {
         "level": {
-            "A2": [
+            "B2": [
                 "EP",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Castles",
-            "fi": "Linnat",
-            "nl": "De kastelen"
+            "en": "cherries",
+            "fi": "kirsikat",
+            "nl": "de kersen"
+        },
+        "singular": {
+            "en": "cherry",
+            "fi": "kirsikka",
+            "nl": "de kers"
+        }
+    },
+    "chicken": {
+        "level": {
+            "A1": "OD",
+            "A2": "EP"
+        },
+        "plural": {
+            "en": "chickens",
+            "fi": "kanat",
+            "nl": "de kippen"
         },
         "singular": {
-            "en": "Castle",
-            "fi": "Linna",
-            "nl": "Het kasteel"
+            "en": "chicken",
+            "fi": "kana",
+            "nl": "de kip"
         }
     },
-    "centre": {
+    "coffee": {
         "level": {
             "A1": [
+                "EP",
                 "KK",
                 "OD"
-            ],
-            "A2": "EP"
+            ]
         },
         "plural": {
-            "en": "Centres",
-            "fi": "Keskustat",
-            "nl": "De centra"
+            "en": "coffees",
+            "fi": "kahvit",
+            "nl": "de koffies"
         },
         "singular": {
-            "en": "Centre",
-            "fi": "Keskusta",
-            "nl": "Het centrum"
+            "en": "coffee",
+            "fi": "kahvi",
+            "nl": "de koffie"
         }
     },
-    "church": {
+    "cookie": {
         "level": {
-            "A1": "KK",
-            "A2": [
+            "A2": "OD",
+            "none": "EP"
+        },
+        "plural": {
+            "en": "cookies",
+            "fi": "keksit",
+            "nl": "de koekjes"
+        },
+        "singular": {
+            "en": "cookie",
+            "fi": "keksi",
+            "nl": "het koekje"
+        }
+    },
+    "cream": {
+        "en": "cream",
+        "fi": "kerma",
+        "level": {
+            "A1": [
                 "EP",
                 "OD"
             ]
         },
+        "nl": "de room"
+    },
+    "dressing": {
+        "level": {
+            "C1": "OD",
+            "none": "EP"
+        },
         "plural": {
-            "en": "Churches",
-            "fi": "Kirkot",
-            "nl": "De kerken"
+            "en": "dressings",
+            "fi": "kastikkeet",
+            "nl": "de dressings"
         },
         "singular": {
-            "en": "Church",
-            "fi": "Kirkko",
-            "nl": "De kerk"
+            "en": "dressing",
+            "fi": "kastike",
+            "nl": "de dressing"
         }
     },
-    "city": {
+    "fish": {
         "level": {
             "A1": [
                 "EP",
                 "KK",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Cities",
-            "fi": "Kaupungit",
-            "nl": "De steden"
+            "en": [
+                "fish",
+                "fishes"
+            ],
+            "fi": "kalat",
+            "nl": "de vissen"
         },
         "singular": {
-            "en": "City",
-            "fi": "Kaupunki",
-            "nl": "De stad"
+            "en": "fish",
+            "fi": "kala",
+            "nl": "de vis"
         }
     },
-    "department store": {
+    "food": {
+        "level": {
+            "A1": [
+                "EP",
+                "KK",
+                "OD"
+            ]
+        },
+        "plural": {
+            "en": "foods",
+            "fi": "ruoat"
+        },
+        "singular": {
+            "en": "food",
+            "fi": "ruoka",
+            "nl": "het voedsel"
+        }
+    },
+    "garlic": {
         "level": {
             "A2": "EP",
             "B1": "OD"
         },
         "plural": {
-            "en": "Department stores",
-            "fi": "Tavaratalot",
-            "nl": "De warenhuizen"
+            "en": "garlics",
+            "fi": "valkosipulit",
+            "nl": "de knofloken"
+        },
+        "roots": {
+            "fi": [
+                "white",
+                "onion"
+            ]
+        },
+        "singular": {
+            "en": "garlic",
+            "fi": "valkosipuli",
+            "nl": "de knoflook"
+        }
+    },
+    "hotdog": {
+        "level": {
+            "A2": "OD",
+            "none": "EP"
+        },
+        "plural": {
+            "en": [
+                "hotdogs|hot dogs"
+            ],
+            "fi": "hotdogit",
+            "nl": "de hotdogs"
         },
         "roots": {
-            "en": "store",
-            "fi": "house",
-            "nl": "house"
+            "en": [
+                "hot",
+                "dog"
+            ]
         },
         "singular": {
-            "en": "Department store",
-            "fi": "Tavaratalo",
-            "nl": "Het warenhuis"
+            "en": [
+                "hotdog|hot dog"
+            ],
+            "fi": "hotdog",
+            "nl": "de hotdog"
         }
     },
-    "hospital": {
+    "ice cream": {
         "level": {
             "A1": [
                 "EP",
-                "KK",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Hospitals",
-            "fi": "Sairaalat",
-            "nl": "De ziekenhuizen"
+            "en": "ice creams",
+            "fi": "j\u00e4\u00e4tel\u00f6t",
+            "nl": "de ijsjes"
         },
         "roots": {
-            "nl": "house"
+            "en": [
+                "ice",
+                "cream"
+            ],
+            "fi": "ice",
+            "nl": "ice"
         },
         "singular": {
-            "en": "Hospital",
-            "fi": "Sairaala",
-            "nl": "Het ziekenhuis"
+            "en": "ice cream",
+            "fi": "j\u00e4\u00e4tel\u00f6",
+            "nl": "het ijsje|het ijs"
         }
     },
-    "hotel": {
+    "juice": {
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Hotels",
-            "fi": "Hotellit",
-            "nl": "De hotels"
+            "en": "juices",
+            "fi": "mehut",
+            "nl": "de sappen"
         },
         "singular": {
-            "en": "Hotel",
-            "fi": "Hotelli",
-            "nl": "Het hotel"
+            "en": "juice",
+            "fi": "mehu",
+            "nl": "het sap"
         }
     },
-    "library": {
+    "ketchup": {
         "level": {
-            "A1": "OD",
-            "A2": "EP"
+            "B2": "OD",
+            "none": "EP"
         },
         "plural": {
-            "en": "Libraries",
-            "fi": "Kirjastot",
-            "nl": "De bibliotheken"
+            "en": "ketchups",
+            "fi": "ketsupit"
         },
-        "roots": {
-            "fi": "book"
+        "singular": {
+            "en": "ketchup",
+            "fi": "ketsuppi",
+            "nl": "de ketchup"
+        }
+    },
+    "lemon": {
+        "level": {
+            "A2": [
+                "EP",
+                "OD"
+            ]
+        },
+        "plural": {
+            "en": "lemons",
+            "fi": "sitruunat",
+            "nl": "de citroenen"
         },
         "singular": {
-            "en": "Library",
-            "fi": "Kirjasto",
-            "nl": "De bibliotheek"
+            "en": "lemon",
+            "fi": "sitruuna",
+            "nl": "de citroen"
         }
     },
-    "mall": {
+    "meat": {
         "level": {
-            "B1": [
+            "A1": [
                 "EP",
                 "OD"
             ]
         },
         "plural": {
-            "en": [
-                "Malls",
-                "Shopping centers"
-            ],
-            "fi": [
-                "Kauppakeskukset",
-                "Ostoskeskukset"
-            ],
-            "nl": "De winkelcentra"
+            "en": "meats",
+            "fi": "lihat",
+            "nl": "de vlezen"
         },
-        "roots": {
-            "en": "centre",
-            "fi": [
-                "centre",
-                "store"
-            ],
-            "nl": [
-                "centre",
-                "store"
+        "singular": {
+            "en": "meat",
+            "fi": "liha",
+            "nl": "het vlees"
+        }
+    },
+    "milk": {
+        "level": {
+            "A1": [
+                "EP",
+                "OD"
             ]
         },
+        "plural": {
+            "en": "milks",
+            "fi": "maidot"
+        },
         "singular": {
-            "en": [
-                "Mall",
-                "Shopping center"
-            ],
-            "fi": [
-                "Kauppakeskus",
-                "Ostoskeskus"
-            ],
-            "nl": "Het winkelcentrum"
+            "en": "milk",
+            "fi": "maito",
+            "nl": "de melk"
         }
     },
-    "monument": {
+    "mushroom": {
         "level": {
-            "B1": "EP",
-            "B2": "OD"
+            "A2": [
+                "EP",
+                "OD"
+            ]
+        },
+        "plural": {
+            "en": "mushrooms",
+            "fi": "sienet",
+            "nl": "de paddenstoelen"
+        },
+        "roots": {
+            "nl": "chair"
+        },
+        "singular": {
+            "en": "mushroom",
+            "fi": "sieni",
+            "nl": "de paddenstoel"
+        }
+    },
+    "mustard": {
+        "level": {
+            "C1": "EP",
+            "C2": "OD"
         },
         "plural": {
-            "en": "Monuments",
-            "fi": "Monumentit",
-            "nl": "De monumenten"
+            "en": "mustards",
+            "fi": "sinapit",
+            "nl": "de mosterds"
         },
         "singular": {
-            "en": "Monument",
-            "fi": "Monumentti",
-            "nl": "Het monument"
+            "en": "mustard",
+            "fi": "sinappi",
+            "nl": "de mosterd"
         }
     },
-    "museum": {
+    "m\u00e4mmi": {
+        "plural": {
+            "en": "(traditional Finnish Easter desserts)",
+            "fi": "m\u00e4mmit",
+            "nl": "(traditionele Finse paasdesserts)"
+        },
+        "singular": {
+            "en": "(traditional Finnish Easter dessert)",
+            "fi": "m\u00e4mmi",
+            "nl": "(traditioneel Fins paasdessert)"
+        }
+    },
+    "nut": {
+        "level": {
+            "A2": "OD",
+            "B2": "EP"
+        },
+        "plural": {
+            "en": "nuts",
+            "fi": "p\u00e4hkin\u00e4t",
+            "nl": "de noten"
+        },
+        "singular": {
+            "en": "nut",
+            "fi": "p\u00e4hkin\u00e4",
+            "nl": "de noot"
+        }
+    },
+    "onion": {
+        "level": {
+            "A1": "OD",
+            "A2": "EP"
+        },
+        "plural": {
+            "en": "onions",
+            "fi": "sipulit",
+            "nl": "de uien"
+        },
+        "singular": {
+            "en": "onion",
+            "fi": "sipuli",
+            "nl": "de ui"
+        }
+    },
+    "orange (fruit)": {
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Museums",
-            "fi": "Museot",
-            "nl": "De musea"
+            "en": "oranges",
+            "fi": "appelsiinit",
+            "nl": "de sinaasappels"
+        },
+        "roots": {
+            "en": "orange",
+            "nl": "apple"
         },
         "singular": {
-            "en": "Museum",
-            "fi": "Museo",
-            "nl": "Het museum"
+            "en": "orange",
+            "fi": "appelsiini",
+            "nl": "de sinaasappel"
         }
     },
-    "office": {
+    "pear": {
+        "level": {
+            "A2": "EP",
+            "B1": "OD"
+        },
+        "plural": {
+            "en": "pears",
+            "fi": "p\u00e4\u00e4ryn\u00e4t",
+            "nl": "de peren"
+        },
+        "singular": {
+            "en": "pear",
+            "fi": "p\u00e4\u00e4ryn\u00e4",
+            "nl": "de peer"
+        }
+    },
+    "pepper": {
         "level": {
             "A1": "OD",
             "A2": "EP"
         },
         "plural": {
-            "en": "Offices",
-            "fi": "Toimistot",
-            "nl": "De kantoren"
+            "en": "peppers",
+            "fi": "pippurit",
+            "nl": "de pepers"
         },
         "singular": {
-            "en": "Office",
-            "fi": "Toimisto",
-            "nl": "Het kantoor"
+            "en": "pepper",
+            "fi": "pippuri",
+            "nl": "de peper"
         }
     },
-    "park": {
+    "potato": {
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Parks",
-            "fi": "Puistot",
-            "nl": "De parken"
+            "en": "potatoes",
+            "fi": "perunat",
+            "nl": "de aardappels"
+        },
+        "roots": {
+            "nl": "apple"
         },
         "singular": {
-            "en": "Park",
-            "fi": "Puisto",
-            "nl": "Het park"
+            "en": "potato",
+            "fi": "peruna",
+            "nl": "de aardappel"
         }
     },
-    "port": {
+    "salad": {
         "level": {
-            "B1": [
+            "A1": "OD",
+            "A2": "EP"
+        },
+        "plural": {
+            "en": "salads",
+            "fi": "salaatit",
+            "nl": "de salades"
+        },
+        "singular": {
+            "en": "salad",
+            "fi": "salaatti",
+            "nl": "de salade"
+        }
+    },
+    "salt": {
+        "level": {
+            "A1": [
                 "EP",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Ports",
-            "fi": "Satamat",
-            "nl": "De havens"
+            "en": "salts",
+            "fi": "suolat",
+            "nl": "de zouten"
         },
         "singular": {
-            "en": "Port",
-            "fi": "Satama",
-            "nl": "De haven"
+            "en": "salt",
+            "fi": "suola",
+            "nl": "het zout"
         }
     },
-    "square": {
+    "sandwich": {
         "level": {
-            "A2": [
+            "A1": [
                 "EP",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Squares",
-            "fi": "Aukiot",
-            "nl": "De pleinen"
+            "en": "sandwiches",
+            "fi": "voileiv\u00e4t",
+            "nl": "de boterhammen"
+        },
+        "roots": {
+            "fi": "bread"
         },
         "singular": {
-            "en": "Square",
-            "fi": "Aukio",
-            "nl": "Het plein"
+            "en": "sandwich",
+            "fi": "voileip\u00e4",
+            "nl": "de boterham"
         }
     },
-    "stadium": {
+    "sausage": {
         "level": {
             "A2": [
                 "EP",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Stadiums",
-            "fi": "Stadionit",
-            "nl": "De stadions"
+            "en": "sausages",
+            "fi": "makkarat",
+            "nl": "de worsten"
+        },
+        "singular": {
+            "en": "sausage",
+            "fi": "makkara",
+            "nl": "de worst"
+        }
+    },
+    "spice": {
+        "level": {
+            "B1": "EP",
+            "B2": "OD"
+        },
+        "plural": {
+            "en": "spices",
+            "fi": "mausteet",
+            "nl": "de kruiden"
         },
         "singular": {
-            "en": "Stadium",
-            "fi": "Stadion",
-            "nl": "Het stadion"
+            "en": "spice",
+            "fi": "mauste",
+            "nl": "het kruid"
         }
     },
-    "store": {
+    "steak": {
+        "level": {
+            "A2": "EP",
+            "B1": "OD"
+        },
+        "plural": {
+            "en": "steaks",
+            "fi": "pihvit",
+            "nl": "de steaks"
+        },
+        "singular": {
+            "en": "steak",
+            "fi": "pihvi",
+            "nl": "de steak"
+        }
+    },
+    "strawberry": {
         "level": {
-            "A1": "KK",
             "A2": "OD",
             "B1": "EP"
         },
         "plural": {
-            "en": "Stores",
-            "fi": "Kaupat",
-            "nl": "De winkels"
+            "en": "strawberries",
+            "fi": "mansikat",
+            "nl": "de aardbeien"
+        },
+        "singular": {
+            "en": "strawberry",
+            "fi": "mansikka",
+            "nl": "de aardbei"
+        }
+    },
+    "sugar": {
+        "level": {
+            "A1": [
+                "EP",
+                "OD"
+            ]
+        },
+        "plural": {
+            "en": "sugars",
+            "fi": "sokerit",
+            "nl": "de suikers"
+        },
+        "singular": {
+            "en": "sugar",
+            "fi": "sokeri",
+            "nl": "de suiker"
+        }
+    },
+    "tomato": {
+        "level": {
+            "A1": [
+                "EP",
+                "OD"
+            ]
+        },
+        "plural": {
+            "en": "tomatoes",
+            "fi": "tomaatit",
+            "nl": "de tomaten"
         },
         "singular": {
-            "en": "Store",
-            "fi": "Kauppa",
-            "nl": "De winkel"
+            "en": "tomato",
+            "fi": "tomaatti",
+            "nl": "de tomaat"
         }
     },
-    "street": {
+    "water": {
         "level": {
             "A1": [
                 "EP",
                 "KK",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Streets",
-            "fi": "Kadut",
-            "nl": "De straten"
-        },
-        "singular": {
-            "en": "Street",
-            "fi": "Katu",
-            "nl": "De straat"
-        }
-    },
-    "that building is a church": {
-        "en": "That building is a church",
-        "fi": "Tuo rakennus on kirkko",
-        "nl": "Dat gebouw is een kerk",
-        "roots": [
-            "to be",
-            "building",
-            "church"
-        ]
+            "en": "waters",
+            "fi": "vedet",
+            "nl": [
+                "de waters",
+                "de wateren"
+            ]
+        },
+        "singular": {
+            "en": "water",
+            "fi": "vesi",
+            "nl": "het water"
+        }
     },
-    "theater": {
+    "whipped cream": {
+        "en": "whipped cream",
+        "fi": "kermavaahto",
         "level": {
-            "B2": "OD",
+            "C1": "OD",
             "none": "EP"
         },
-        "plural": {
-            "en": "Theaters",
-            "fi": "Teatterit",
-            "nl": "De theaters"
-        },
-        "singular": {
-            "en": "Theater",
-            "fi": "Teatteri",
-            "nl": "Het theater"
-        }
-    },
-    "there is a christmas tree on the square": {
-        "en": "There is a Christmas tree on the square",
-        "fi": "Aukiolla on joulukuusi",
-        "nl": "Er staat een kerstboom op het plein",
-        "roots": [
-            "to be",
-            "square",
-            "christmas tree"
-        ]
-    },
-    "where is the library": {
-        "en": "Where is the library?",
-        "fi": "Miss\u00e4 on kirjasto?",
-        "nl": "Waar is de bibliotheek?",
-        "roots": [
-            "where",
-            "to be",
-            "library"
-        ]
+        "nl": "de slagroom",
+        "roots": "cream"
     }
 }
```

### Comparing `Toisto-0.8.2/src/topics/clothes.json` & `Toisto-0.9.0/src/topics/clothes.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9049278846153845%*

 * *Differences: {"'clothes'": "{'en': 'clothes', 'fi': 'vaatteet', 'nl': 'de kleren'}",*

 * * "'coat'": "{'singular': {'en': 'coat', 'fi': 'takki', 'nl': 'de jas'}, 'plural': {'en': 'coats', "*

 * *           "'fi': 'takit', 'nl': 'de jassen'}}",*

 * * "'dress'": "{'singular': {'en': 'dress', 'fi': 'mekko', 'nl': 'de jurk'}, 'plural': {'en': "*

 * *            "'dresses', 'fi': 'mekot', 'nl': 'de jurken'}}",*

 * * "'hat'": "{'singular': {'en': 'hat', 'fi': 'hattu', 'nl': 'de hoed'}, 'plural': {'en': 'hats', "*

 * *          "'fi': 'hatut', 'nl': 'de ho […]*

```diff
@@ -1,282 +1,284 @@
 {
     "clothes": {
-        "en": "Clothes",
-        "fi": "Vaatteet",
+        "en": "clothes",
+        "fi": "vaatteet",
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
-        "nl": "De kleren"
+        "nl": "de kleren"
     },
     "coat": {
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Coats",
-            "fi": "Takit",
-            "nl": "De jassen"
+            "en": "coats",
+            "fi": "takit",
+            "nl": "de jassen"
         },
         "singular": {
-            "en": "Coat",
-            "fi": "Takki",
-            "nl": "De jas"
+            "en": "coat",
+            "fi": "takki",
+            "nl": "de jas"
         }
     },
     "dress": {
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Dresses",
-            "fi": "Mekot",
-            "nl": "De jurken"
+            "en": "dresses",
+            "fi": "mekot",
+            "nl": "de jurken"
         },
         "singular": {
-            "en": "Dress",
-            "fi": "Mekko",
-            "nl": "De jurk"
+            "en": "dress",
+            "fi": "mekko",
+            "nl": "de jurk"
         }
     },
     "hat": {
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Hats",
-            "fi": "Hatut",
-            "nl": "De hoeden"
+            "en": "hats",
+            "fi": "hatut",
+            "nl": "de hoeden"
         },
         "singular": {
-            "en": "Hat",
-            "fi": "Hattu",
-            "nl": "De hoed"
+            "en": "hat",
+            "fi": "hattu",
+            "nl": "de hoed"
         }
     },
     "shirt": {
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Shirts",
-            "fi": "Paidat",
-            "nl": "De hemden"
+            "en": "shirts",
+            "fi": "paidat",
+            "nl": "de hemden"
         },
         "singular": {
-            "en": "Shirt",
-            "fi": "Paita",
-            "nl": "Het hemd"
+            "en": "shirt",
+            "fi": "paita",
+            "nl": "het hemd"
         }
     },
     "shoe": {
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Shoes",
-            "fi": "Keng\u00e4t",
-            "nl": "De schoenen"
+            "en": "shoes",
+            "fi": "keng\u00e4t",
+            "nl": "de schoenen"
         },
         "singular": {
-            "en": "Shoe",
-            "fi": "Kenk\u00e4",
-            "nl": "De schoen"
+            "en": "shoe",
+            "fi": "kenk\u00e4",
+            "nl": "de schoen"
         }
     },
     "skirt": {
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Skirts",
-            "fi": "Hameet",
-            "nl": "De rokken"
+            "en": "skirts",
+            "fi": "hameet",
+            "nl": "de rokken"
         },
         "singular": {
-            "en": "Skirt",
-            "fi": "Hame",
-            "nl": "De rok"
+            "en": "skirt",
+            "fi": "hame",
+            "nl": "de rok"
         }
     },
     "sock": {
         "level": {
             "A2": [
                 "EP",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Socks",
-            "fi": "Sukat",
-            "nl": "De sokken"
+            "en": "socks",
+            "fi": "sukat",
+            "nl": "de sokken"
         },
         "singular": {
-            "en": "Sock",
-            "fi": "Sukka",
-            "nl": "De sok"
+            "en": "sock",
+            "fi": "sukka",
+            "nl": "de sok"
         }
     },
     "suit": {
         "level": {
             "A2": [
                 "EP",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Suits",
-            "fi": "Puvut",
-            "nl": "De pakken"
+            "en": "suits",
+            "fi": "puvut",
+            "nl": "de pakken"
         },
         "singular": {
-            "en": "Suit",
-            "fi": "Puku",
-            "nl": "Het pak"
+            "en": "suit",
+            "fi": "puku",
+            "nl": "het pak"
         }
     },
     "sweater": {
         "level": {
             "A1": "OD",
             "A2": "EP"
         },
         "plural": {
-            "en": "Sweaters",
-            "fi": "Neulepaidat",
-            "nl": "De truien"
+            "en": "sweaters",
+            "fi": "neulepaidat",
+            "nl": "de truien"
         },
         "roots": {
             "fi": "shirt"
         },
         "singular": {
-            "en": "Sweater",
-            "fi": "Neulepaita",
-            "nl": "De trui"
+            "en": "sweater",
+            "fi": "neulepaita",
+            "nl": "de trui"
         }
     },
     "to dress": {
         "infinitive": {
             "en": [
-                "To dress",
-                "To get dressed"
+                "to dress",
+                "to get dressed"
             ],
-            "fi": "Pukeutua",
-            "nl": "Zich aankleden"
+            "fi": "pukeutua",
+            "nl": "zich aankleden"
         },
         "level": {
             "A1": "OD",
             "A2": "EP"
         },
         "plural": {
             "first person": {
                 "en": [
-                    "We dress",
-                    "We get dressed"
+                    "we dress",
+                    "we get dressed"
                 ],
-                "fi": "Me pukeudumme|Pukeudumme",
-                "nl": "Wij kleden ons aan|We kleden ons aan"
+                "fi": "me pukeudumme|pukeudumme",
+                "nl": "wij kleden ons aan|we kleden ons aan"
             },
             "second person": {
                 "en": [
-                    "You dress;plural",
-                    "You get dressed;plural"
+                    "you dress;plural",
+                    "you get dressed;plural"
                 ],
-                "fi": "Te pukeudutte|Pukeudutte",
-                "nl": "Jullie kleden je aan"
+                "fi": "te pukeudutte|pukeudutte",
+                "nl": "jullie kleden je aan"
             },
             "third person": {
                 "en": [
-                    "They dress",
-                    "They get dressed"
+                    "they dress",
+                    "they get dressed"
                 ],
-                "fi": "He pukeutuvat|Pukeutuvat",
-                "nl": "Zij kleden zich aan|Ze kleden zich aan"
+                "fi": "he pukeutuvat|pukeutuvat",
+                "nl": "zij kleden zich aan|ze kleden zich aan"
             }
         },
         "singular": {
             "first person": {
                 "en": [
                     "I dress",
                     "I get dressed"
                 ],
-                "fi": "Min\u00e4 pukeudun|Pukeudun",
-                "nl": "Ik kleed mij aan|Ik kleed me aan"
+                "fi": "min\u00e4 pukeudun|pukeudun",
+                "nl": "ik kleed mij aan|ik kleed me aan"
             },
             "second person": {
                 "en": [
-                    "You dress;singular",
-                    "You get dressed;singular"
+                    "you dress;singular",
+                    "you get dressed;singular"
                 ],
-                "fi": "Sin\u00e4 pukeudut|Pukeudut",
-                "nl": "Jij kleedt je aan"
+                "fi": "sin\u00e4 pukeudut|pukeudut",
+                "nl": "jij kleedt je aan"
             },
             "third person": {
                 "female": {
                     "en": [
-                        "She dresses",
-                        "She gets dressed"
+                        "she dresses",
+                        "she gets dressed"
                     ],
-                    "fi": "H\u00e4n pukeutuu;female",
-                    "nl": "Zij kleedt zich aan|Ze kleedt zich aan"
+                    "fi": "h\u00e4n pukeutuu;female",
+                    "nl": "zij kleedt zich aan|ze kleedt zich aan"
                 },
                 "male": {
                     "en": [
-                        "He dresses",
-                        "He gets dressed"
+                        "he dresses",
+                        "he gets dressed"
                     ],
-                    "fi": "H\u00e4n pukeutuu;male",
-                    "nl": "Hij kleedt zich aan"
+                    "fi": "h\u00e4n pukeutuu;male",
+                    "nl": "hij kleedt zich aan"
                 }
             }
         }
     },
     "trousers": {
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
         "plural": {
-            "nl": "De broeken"
+            "en": "(pairs of trousers)",
+            "fi": "(paria housut)",
+            "nl": "de broeken"
         },
         "singular": {
-            "en": "Trousers",
-            "fi": "Housut",
-            "nl": "De broek"
+            "en": "trousers",
+            "fi": "housut",
+            "nl": "de broek"
         }
     },
     "underwear": {
-        "en": "Underwear",
-        "fi": "Alusvaatteet",
+        "en": "underwear",
+        "fi": "alusvaatteet",
         "level": {
             "B1": [
                 "EP",
                 "OD"
             ]
         },
-        "nl": "Het ondergoed",
+        "nl": "het ondergoed",
         "roots": {
             "fi": "clothes"
         }
     }
 }
```

### Comparing `Toisto-0.8.2/src/topics/colors.json` & `Toisto-0.9.0/src/topics/colors.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8619318181818181%*

 * *Differences: {"'I read the red book'": "{'singular': {'en': 'I read the red book.;present tense', 'fi': 'Minä "*

 * *                          "luen punaisen kirjan.|Luen punaisen kirjan.', 'nl': 'Ik lees het rode "*

 * *                          "boek.'}, 'plural': {'en': 'I read the red books.;present tense', 'fi': "*

 * *                          "'Minä luen punaisia kirjoja.|Luen punaisia kirjoja.', 'nl': 'Ik lees de "*

 * *                          "rode boeken.'}}",*

 * * "'black'": "{'en': 'black', 'fi': 'musta', 'nl': 'zwart'}",*

 * * "'blue […]*

```diff
@@ -1,304 +1,304 @@
 {
     "I read the red book": {
         "plural": {
-            "en": "I read the red books;present tense",
-            "fi": "Min\u00e4 luen punaisia \u200b\u200bkirjoj|Luen punaisia \u200b\u200bkirjoja",
-            "nl": "Ik lees de rode boeken"
+            "en": "I read the red books.;present tense",
+            "fi": "Min\u00e4 luen punaisia kirjoja.|Luen punaisia kirjoja.",
+            "nl": "Ik lees de rode boeken."
         },
         "roots": [
             "to read",
             "red",
             "book"
         ],
         "singular": {
-            "en": "I read the red book;present tense",
-            "fi": "Min\u00e4 luen punaisen kirjan|Luen punaisen kirjan",
-            "nl": "Ik lees het rode boek"
+            "en": "I read the red book.;present tense",
+            "fi": "Min\u00e4 luen punaisen kirjan.|Luen punaisen kirjan.",
+            "nl": "Ik lees het rode boek."
         }
     },
     "black": {
         "antonym": "white",
-        "en": "Black",
-        "fi": "Musta",
+        "en": "black",
+        "fi": "musta",
         "level": {
             "A1": [
                 "EP",
                 "KK",
                 "OD"
             ]
         },
-        "nl": "Zwart"
+        "nl": "zwart"
     },
     "blue": {
-        "en": "Blue",
-        "fi": "Sininen",
+        "en": "blue",
+        "fi": "sininen",
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
-        "nl": "Blauw"
+        "nl": "blauw"
     },
     "brown": {
-        "en": "Brown",
-        "fi": "Ruskea",
+        "en": "brown",
+        "fi": "ruskea",
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
-        "nl": "Bruin"
+        "nl": "bruin"
     },
     "dark blue": {
-        "en": "Dark blue",
-        "fi": "Tummansininen",
+        "en": "dark blue",
+        "fi": "tummansininen",
         "level": {
             "A1": "OD",
             "A2": "EP"
         },
-        "nl": "Donkerblauw",
+        "nl": "donkerblauw",
         "roots": "blue"
     },
     "green": {
-        "en": "Green",
-        "fi": "Vihre\u00e4",
+        "en": "green",
+        "fi": "vihre\u00e4",
         "level": {
             "A1": [
                 "EP",
                 "KK",
                 "OD"
             ]
         },
-        "nl": "Groen"
+        "nl": "groen"
     },
     "grey": {
-        "en": "Grey|Gray",
-        "fi": "Harmaa",
+        "en": "grey|gray",
+        "fi": "harmaa",
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
-        "nl": "Grijs"
+        "nl": "grijs"
     },
     "i have a green table": {
         "plural": {
-            "en": "I have green tables",
-            "fi": "Minulla on vihreit\u00e4 p\u00f6yti\u00e4",
-            "nl": "Ik heb groene tafels"
+            "en": "I have green tables.",
+            "fi": "Minulla on vihreit\u00e4 p\u00f6yti\u00e4.",
+            "nl": "Ik heb groene tafels."
         },
         "roots": [
             "green",
             "to have",
             "table"
         ],
         "singular": {
-            "en": "I have a green table",
-            "fi": "Minulla on vihre\u00e4 p\u00f6yt\u00e4",
-            "nl": "Ik heb een groene tafel"
+            "en": "I have a green table.",
+            "fi": "Minulla on vihre\u00e4 p\u00f6yt\u00e4.",
+            "nl": "Ik heb een groene tafel."
         }
     },
     "i live in a purple house": {
         "plural": {
-            "en": "I live in purple houses",
-            "fi": "Min\u00e4 asun violeteissa taloissa|Asun violeteissa taloissa",
-            "nl": "Ik woon in paarse huizen"
+            "en": "I live in purple houses.",
+            "fi": "Min\u00e4 asun violeteissa taloissa.|Asun violeteissa taloissa.",
+            "nl": "Ik woon in paarse huizen."
         },
         "roots": [
             "to live",
             "purple",
             "house"
         ],
         "singular": {
-            "en": "I live in a purple house",
-            "fi": "Min\u00e4 asun violetissa talossa|Asun violetissa talossa",
-            "nl": "Ik woon in een paars huis"
+            "en": "I live in a purple house.",
+            "fi": "Min\u00e4 asun violetissa talossa.|Asun violetissa talossa.",
+            "nl": "Ik woon in een paars huis."
         }
     },
     "i sit on a green sofa": {
         "plural": {
-            "en": "I sit on green sofas",
-            "fi": "Min\u00e4 istun vihreill\u00e4 sohvilla|Istun vihreill\u00e4 sohvilla",
-            "nl": "Ik zit op groene sofa's"
+            "en": "I sit on green sofas.",
+            "fi": "Min\u00e4 istun vihreill\u00e4 sohvilla.|Istun vihreill\u00e4 sohvilla.",
+            "nl": "Ik zit op groene sofa's."
         },
         "roots": [
             "green",
             "sofa"
         ],
         "singular": {
-            "en": "I sit on a green sofa",
-            "fi": "Min\u00e4 istun vihre\u00e4ll\u00e4 sohvalla|Istun vihre\u00e4ll\u00e4 sohvalla",
-            "nl": "Ik zit op een groene sofa"
+            "en": "I sit on a green sofa.",
+            "fi": "Min\u00e4 istun vihre\u00e4ll\u00e4 sohvalla.|Istun vihre\u00e4ll\u00e4 sohvalla.",
+            "nl": "Ik zit op een groene sofa."
         }
     },
     "light blue": {
-        "en": "Light blue",
-        "fi": "Vaaleansininen",
+        "en": "light blue",
+        "fi": "vaaleansininen",
         "level": {
             "A1": "OD",
             "A2": "EP"
         },
-        "nl": "Lichtblauw",
+        "nl": "lichtblauw",
         "roots": "blue"
     },
     "orange": {
-        "en": "Orange",
-        "fi": "Oranssi",
+        "en": "orange",
+        "fi": "oranssi",
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
-        "nl": "Oranje"
+        "nl": "oranje"
     },
     "pink": {
-        "en": "Pink",
+        "en": "pink",
         "fi": [
-            "Vaaleanpunainen",
-            "Pinkki"
+            "vaaleanpunainen",
+            "pinkki"
         ],
         "level": {
             "A1": "OD",
             "A2": "EP"
         },
-        "nl": "Roze"
+        "nl": "roze"
     },
     "purple": {
-        "en": "Purple",
+        "en": "purple",
         "fi": [
-            "Liila",
-            "Violetti"
+            "liila",
+            "violetti"
         ],
         "level": {
             "A1": "OD",
             "A2": "EP"
         },
-        "nl": "Paars"
+        "nl": "paars"
     },
     "red": {
-        "en": "Red",
-        "fi": "Punainen",
+        "en": "red",
+        "fi": "punainen",
         "level": {
             "A1": [
                 "EP",
                 "KK",
                 "OD"
             ]
         },
-        "nl": "Rood"
+        "nl": "rood"
     },
     "the blue car is old": {
         "plural": {
-            "en": "The blue cars are old",
-            "fi": "Siniset autot ovat vanhoja",
-            "nl": "De blauwe auto's zijn oud"
+            "en": "The blue cars are old.",
+            "fi": "Siniset autot ovat vanhoja.",
+            "nl": "De blauwe auto's zijn oud."
         },
         "roots": [
             "blue",
             "car",
             "to be",
             "old"
         ],
         "singular": {
-            "en": "The blue car is old",
-            "fi": "Sininen auto on vanha",
-            "nl": "De blauwe auto is oud"
+            "en": "The blue car is old.",
+            "fi": "Sininen auto on vanha.",
+            "nl": "De blauwe auto is oud."
         }
     },
     "the car is blue": {
         "plural": {
-            "en": "The cars are blue",
-            "fi": "Autot ovat sinisi\u00e4",
-            "nl": "De auto's zijn blauw"
+            "en": "The cars are blue.",
+            "fi": "Autot ovat sinisi\u00e4.",
+            "nl": "De auto's zijn blauw."
         },
         "roots": [
             "car",
             "to be",
             "blue"
         ],
         "singular": {
-            "en": "The car is blue",
-            "fi": "Auto on sininen",
-            "nl": "De auto is blauw"
+            "en": "The car is blue.",
+            "fi": "Auto on sininen.",
+            "nl": "De auto is blauw."
         }
     },
     "the green table is mine": {
         "plural": {
-            "en": "The green tables are mine",
-            "fi": "Vihre\u00e4t p\u00f6yd\u00e4t ovat minun",
-            "nl": "De groene tafels zijn van mij"
+            "en": "The green tables are mine.",
+            "fi": "Vihre\u00e4t p\u00f6yd\u00e4t ovat minun.",
+            "nl": "De groene tafels zijn van mij."
         },
         "roots": [
             "green",
             "table",
             "to be"
         ],
         "singular": {
-            "en": "The green table is mine",
-            "fi": "Vihre\u00e4 p\u00f6yt\u00e4 on minun",
-            "nl": "De groene tafel is van mij"
+            "en": "The green table is mine.",
+            "fi": "Vihre\u00e4 p\u00f6yt\u00e4 on minun.",
+            "nl": "De groene tafel is van mij."
         }
     },
     "the house is white": {
         "plural": {
-            "en": "The houses are white",
-            "fi": "Talot on valkoisia",
-            "nl": "De huizen zijn wit"
+            "en": "The houses are white.",
+            "fi": "Talot on valkoisia.",
+            "nl": "De huizen zijn wit."
         },
         "roots": [
             "house",
             "to be",
             "white"
         ],
         "singular": {
-            "en": "The house is white",
-            "fi": "Talo on valkoinen",
-            "nl": "Het huis is wit"
+            "en": "The house is white.",
+            "fi": "Talo on valkoinen.",
+            "nl": "Het huis is wit."
         }
     },
     "the white house is big": {
         "plural": {
-            "en": "The white houses are big",
-            "fi": "Valkoiset talot ovat suuria",
-            "nl": "Het witte huis is groot"
+            "en": "The white houses are big.",
+            "fi": "Valkoiset talot ovat suuria.",
+            "nl": "Het witte huis is groot."
         },
         "roots": [
             "white",
             "house",
             "big"
         ],
         "singular": {
-            "en": "The white house is big",
-            "fi": "Valkoinen talo on suuri",
-            "nl": "Het witte huis is groot"
+            "en": "The white house is big.",
+            "fi": "Valkoinen talo on suuri.",
+            "nl": "Het witte huis is groot."
         }
     },
     "white": {
         "antonym": "black",
-        "en": "White",
-        "fi": "Valkoinen",
+        "en": "white",
+        "fi": "valkoinen",
         "level": {
             "A1": [
                 "EP",
                 "KK",
                 "OD"
             ]
         },
-        "nl": "Wit"
+        "nl": "wit"
     },
     "yellow": {
-        "en": "Yellow",
-        "fi": "Keltainen",
+        "en": "yellow",
+        "fi": "keltainen",
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
-        "nl": "Geel"
+        "nl": "geel"
     }
 }
```

### Comparing `Toisto-0.8.2/src/topics/counting.json` & `Toisto-0.9.0/src/topics/counting.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.700290697674419%*

 * *Differences: {"'1'": "{'en': 'one', 'fi': 'yksi', 'nl': 'één|een'}",*

 * * "'10'": "{'en': 'ten', 'fi': 'kymmenen', 'nl': 'tien'}",*

 * * "'100'": "{'en': 'hundred', 'fi': 'sata', 'nl': 'honderd'}",*

 * * "'1000'": "{'en': 'thousand', 'fi': 'tuhat', 'nl': 'duizend'}",*

 * * "'1000000'": "OrderedDict([('level', OrderedDict([('A1', 'OD'), ('A2', 'EP')])), ('en', "*

 * *              "'million'), ('fi', 'miljoona'), ('nl', 'miljoen')])",*

 * * "'1000000000'": "OrderedDict([('level', OrderedDict([('A2', 'OD'), ('B2', 'EP')])), ('en', "*

 * *                  […]*

```diff
@@ -1,484 +1,581 @@
 {
     "1": {
-        "en": "One",
-        "fi": "Yksi",
+        "en": "one",
+        "fi": "yksi",
         "level": {
             "A1": [
                 "EP",
                 "KK",
                 "OD"
             ]
         },
-        "nl": "E\u00e9n|\u00e9\u00e9n|Een"
+        "nl": "\u00e9\u00e9n|een"
     },
     "10": {
-        "en": "Ten",
-        "fi": "Kymmenen",
+        "en": "ten",
+        "fi": "kymmenen",
         "level": {
             "A1": [
                 "EP",
                 "KK",
                 "OD"
             ]
         },
-        "nl": "Tien"
+        "nl": "tien"
     },
     "100": {
-        "en": "Hundred",
-        "fi": "Sata",
+        "en": "hundred",
+        "fi": "sata",
         "level": {
             "A1": [
                 "KK",
                 "OD"
             ],
             "A2": "EP"
         },
-        "nl": "Honderd"
+        "nl": "honderd"
     },
     "1000": {
-        "en": "Thousand",
-        "fi": "Tuhat",
+        "en": "thousand",
+        "fi": "tuhat",
         "level": {
             "A1": [
                 "KK",
                 "OD"
             ],
             "A2": "EP"
         },
-        "nl": "Duizend"
+        "nl": "duizend"
+    },
+    "1000000": {
+        "en": "million",
+        "fi": "miljoona",
+        "level": {
+            "A1": "OD",
+            "A2": "EP"
+        },
+        "nl": "miljoen"
+    },
+    "1000000000": {
+        "en": "billion",
+        "fi": "miljardi",
+        "level": {
+            "A2": "OD",
+            "B2": "EP"
+        },
+        "nl": "miljard"
     },
     "11": {
-        "en": "Eleven",
-        "fi": "Yksitoista",
+        "en": "eleven",
+        "fi": "yksitoista",
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
-        "nl": "Elf",
+        "nl": "elf",
         "roots": [
             "1",
             "10"
         ]
     },
     "12": {
-        "en": "Twelve",
-        "fi": "Kaksitoista",
+        "en": "twelve",
+        "fi": "kaksitoista",
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
-        "nl": "Twaalf",
+        "nl": "twaalf",
         "roots": [
             "2",
             "10"
         ]
     },
     "13": {
-        "en": "Thirteen",
-        "fi": "Kolmetoista",
+        "en": "thirteen",
+        "fi": "kolmetoista",
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
-        "nl": "Dertien",
+        "nl": "dertien",
         "roots": [
             "3",
             "10"
         ]
     },
     "14": {
-        "en": "Fourteen",
-        "fi": "Nelj\u00e4toista",
+        "en": "fourteen",
+        "fi": "nelj\u00e4toista",
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
-        "nl": "Veertien",
+        "nl": "veertien",
         "roots": [
             "4",
             "10"
         ]
     },
     "15": {
-        "en": "Fifteen",
-        "fi": "Viisitoista",
+        "en": "fifteen",
+        "fi": "viisitoista",
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
-        "nl": "Vijftien",
+        "nl": "vijftien",
         "roots": [
             "5",
             "10"
         ]
     },
     "16": {
-        "en": "Sixteen",
-        "fi": "Kuusitoista",
+        "en": "sixteen",
+        "fi": "kuusitoista",
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
-        "nl": "Zestien",
+        "nl": "zestien",
         "roots": [
             "6",
             "10"
         ]
     },
     "17": {
-        "en": "Seventeen",
-        "fi": "Seitsem\u00e4ntoista",
+        "en": "seventeen",
+        "fi": "seitsem\u00e4ntoista",
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
-        "nl": "Zeventien",
+        "nl": "zeventien",
         "roots": [
             "7",
             "10"
         ]
     },
     "18": {
-        "en": "Eightteen",
-        "fi": "Kahdeksantoista",
+        "en": "eightteen",
+        "fi": "kahdeksantoista",
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
-        "nl": "Achttien",
+        "nl": "achttien",
         "roots": [
             "8",
             "10"
         ]
     },
     "19": {
-        "en": "Nineteen",
-        "fi": "Yhdeks\u00e4ntoista",
+        "en": "nineteen",
+        "fi": "yhdeks\u00e4ntoista",
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
-        "nl": "Negentien",
+        "nl": "negentien",
         "roots": [
             "9",
             "10"
         ]
     },
     "2": {
-        "en": "Two",
-        "fi": "Kaksi",
+        "en": "two",
+        "fi": "kaksi",
         "level": {
             "A1": [
                 "EP",
                 "KK",
                 "OD"
             ]
         },
-        "nl": "Twee"
+        "nl": "twee"
     },
     "20": {
-        "en": "Twenty",
-        "fi": "Kaksikymment\u00e4",
+        "en": "twenty",
+        "fi": "kaksikymment\u00e4",
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
-        "nl": "Twintig",
+        "nl": "twintig",
         "roots": [
             "2",
             "10"
         ]
     },
     "200": {
-        "en": "Two hundred",
-        "fi": "Kaksisataa",
+        "en": "two hundred",
+        "fi": "kaksisataa",
         "level": {
             "none": [
                 "EP",
                 "OD"
             ]
         },
-        "nl": "Tweehonderd",
+        "nl": "tweehonderd",
         "roots": [
             "2",
             "100"
         ]
     },
     "2000": {
-        "en": "Two thousand",
-        "fi": "Kaksituhatta",
+        "en": "two thousand",
+        "fi": "kaksituhatta",
         "level": {
             "none": [
                 "EP",
                 "OD"
             ]
         },
-        "nl": "Tweeduizend",
+        "nl": "tweeduizend",
         "roots": [
             "2",
             "1000"
         ]
     },
+    "2000000": {
+        "en": "two million",
+        "fi": "kaksi miljoonaa",
+        "level": {
+            "none": [
+                "EP",
+                "OD"
+            ]
+        },
+        "nl": "twee miljoen",
+        "roots": [
+            "2",
+            "1000000"
+        ]
+    },
     "21": {
-        "en": "Twenty-one",
-        "fi": "Kaksikymment\u00e4yksi",
+        "en": "twenty-one",
+        "fi": "kaksikymment\u00e4yksi",
         "level": {
             "none": [
                 "EP",
                 "OD"
             ]
         },
-        "nl": "Eenentwintig",
+        "nl": "eenentwintig",
         "roots": [
             "1",
             "20"
         ]
     },
     "22": {
-        "en": "Twenty-two",
-        "fi": "Kaksikymment\u00e4kaksi",
+        "en": "twenty-two",
+        "fi": "kaksikymment\u00e4kaksi",
         "level": {
             "none": [
                 "EP",
                 "OD"
             ]
         },
-        "nl": "Twee\u00ebntwintig",
+        "nl": "twee\u00ebntwintig",
         "roots": [
             "2",
             "20"
         ]
     },
     "23": {
-        "en": "Twenty-three",
-        "fi": "Kaksikymment\u00e4kolme",
+        "en": "twenty-three",
+        "fi": "kaksikymment\u00e4kolme",
         "level": {
             "none": [
                 "EP",
                 "OD"
             ]
         },
-        "nl": "Drie\u00ebntwintig",
+        "nl": "drie\u00ebntwintig",
         "roots": [
             "3",
             "20"
         ]
     },
     "24": {
-        "en": "Twenty-four",
-        "fi": "Kaksikymment\u00e4nelj\u00e4",
+        "en": "twenty-four",
+        "fi": "kaksikymment\u00e4nelj\u00e4",
         "level": {
             "none": [
                 "EP",
                 "OD"
             ]
         },
-        "nl": "Vierentwintig",
+        "nl": "vierentwintig",
         "roots": [
             "4",
             "20"
         ]
     },
     "3": {
-        "en": "Three",
-        "fi": "Kolme",
+        "en": "three",
+        "fi": "kolme",
         "level": {
             "A1": [
                 "EP",
                 "KK",
                 "OD"
             ]
         },
-        "nl": "Drie"
+        "nl": "drie"
     },
     "30": {
-        "en": "Thirty",
-        "fi": "Kolmekymment\u00e4",
+        "en": "thirty",
+        "fi": "kolmekymment\u00e4",
         "level": {
             "A1": "OD",
             "A2": "EP"
         },
-        "nl": "Dertig",
+        "nl": "dertig",
         "roots": [
             "3",
             "10"
         ]
     },
+    "300": {
+        "en": "three hundred",
+        "fi": "kolmesataa",
+        "level": {
+            "none": [
+                "EP",
+                "OD"
+            ]
+        },
+        "nl": "driehonderd",
+        "roots": [
+            "3",
+            "100"
+        ]
+    },
     "4": {
-        "en": "Four",
-        "fi": "Nelj\u00e4",
+        "en": "four",
+        "fi": "nelj\u00e4",
         "level": {
             "A1": [
                 "EP",
                 "KK",
                 "OD"
             ]
         },
-        "nl": "Vier"
+        "nl": "vier"
     },
     "40": {
-        "en": "Forty",
-        "fi": "Nelj\u00e4kymment\u00e4",
+        "en": "forty",
+        "fi": "nelj\u00e4kymment\u00e4",
         "level": {
             "A1": "OD",
             "A2": "EP"
         },
-        "nl": "Veertig",
+        "nl": "veertig",
         "roots": [
             "4",
             "10"
         ]
     },
     "5": {
-        "en": "Five",
-        "fi": "Viisi",
+        "en": "five",
+        "fi": "viisi",
         "level": {
             "A1": [
                 "EP",
                 "KK",
                 "OD"
             ]
         },
-        "nl": "Vijf"
+        "nl": "vijf"
     },
     "50": {
-        "en": "Fifty",
-        "fi": "Viisikymment\u00e4",
+        "en": "fifty",
+        "fi": "viisikymment\u00e4",
         "level": {
             "A1": "OD",
             "A2": "EP"
         },
-        "nl": "Vijftig",
+        "nl": "vijftig",
         "roots": [
             "5",
             "10"
         ]
     },
+    "500000": {
+        "en": "five hunderd thousand",
+        "fi": "viisisataatuhatta",
+        "level": {
+            "none": [
+                "EP",
+                "OD"
+            ]
+        },
+        "nl": "vijfhonderdduizend",
+        "roots": [
+            "5",
+            "100",
+            "1000"
+        ]
+    },
+    "5000000000": {
+        "en": "five billion",
+        "fi": "viisi miljardia",
+        "level": {
+            "node": [
+                "EP",
+                "OD"
+            ]
+        },
+        "nl": "vijf miljard",
+        "roots": [
+            "5",
+            "1000000000"
+        ]
+    },
     "6": {
-        "en": "Six",
-        "fi": "Kuusi",
+        "en": "six",
+        "fi": "kuusi",
         "level": {
             "A1": [
                 "EP",
                 "KK",
                 "OD"
             ]
         },
-        "nl": "Zes"
+        "nl": "zes"
     },
     "60": {
-        "en": "Sixty",
-        "fi": "Kuusikymment\u00e4",
+        "en": "sixty",
+        "fi": "kuusikymment\u00e4",
         "level": {
             "A1": "OD",
             "A2": "EP"
         },
-        "nl": "Zestig",
+        "nl": "zestig",
         "roots": [
             "6",
             "10"
         ]
     },
     "7": {
-        "en": "Seven",
-        "fi": "Seitsem\u00e4n",
+        "en": "seven",
+        "fi": "seitsem\u00e4n",
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
-        "nl": "Zeven"
+        "nl": "zeven"
     },
     "70": {
-        "en": "Seventy",
-        "fi": "Seitsem\u00e4nkymment\u00e4",
+        "en": "seventy",
+        "fi": "seitsem\u00e4nkymment\u00e4",
         "level": {
             "A1": "OD",
             "A2": "EP"
         },
-        "nl": "Zeventig",
+        "nl": "zeventig",
         "roots": [
             "7",
             "10"
         ]
     },
     "8": {
-        "en": "Eight",
-        "fi": "Kahdeksan",
+        "en": "eight",
+        "fi": "kahdeksan",
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
-        "nl": "Acht"
+        "nl": "acht"
     },
     "80": {
-        "en": "Eighty",
-        "fi": "Kahdeksankymment\u00e4",
+        "en": "eighty",
+        "fi": "kahdeksankymment\u00e4",
         "level": {
             "A1": "OD",
             "A2": "EP"
         },
-        "nl": "Tachtig",
+        "nl": "tachtig",
         "roots": [
             "8",
             "10"
         ]
     },
     "9": {
-        "en": "Nine",
-        "fi": "Yhdeks\u00e4n",
+        "en": "nine",
+        "fi": "yhdeks\u00e4n",
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
-        "nl": "Negen"
+        "nl": "negen"
     },
     "90": {
-        "en": "Ninety",
-        "fi": "Yhdeks\u00e4nkymment\u00e4",
+        "en": "ninety",
+        "fi": "yhdeks\u00e4nkymment\u00e4",
         "level": {
             "A1": "OD",
             "A2": "EP"
         },
-        "nl": "Negentig",
+        "nl": "negentig",
         "roots": [
             "9",
             "10"
         ]
     },
+    "number": {
+        "level": {
+            "A1": [
+                "EP",
+                "OD"
+            ]
+        },
+        "plural": {
+            "en": "numbers",
+            "fi": "numerot",
+            "nl": "de getallen"
+        },
+        "singular": {
+            "en": "number",
+            "fi": "numero",
+            "nl": "het getal"
+        }
+    },
     "to count": {
-        "en": "To count",
-        "fi": "Laskea",
+        "en": "to count",
+        "fi": "laskea",
         "level": {
             "A1": "KK",
             "A2": "OD",
             "B1": "EP"
         },
-        "nl": "Tellen"
+        "nl": "tellen"
     }
 }
```

### Comparing `Toisto-0.8.2/src/topics/countries.json` & `Toisto-0.9.0/src/topics/countries.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9328703703703702%*

 * *Differences: {"'china'": "{'fi': 'Kiina'}",*

 * * "'country'": "{'singular': {'en': 'country', 'fi': 'maa;geography', 'nl': 'het land'}, 'plural': "*

 * *              "{'en': 'countries', 'fi': 'maat;geography', 'nl': 'de landen'}}",*

 * * "'denmark'": "{'fi': 'Tanska'}",*

 * * "'england'": "{'fi': 'Englanti'}",*

 * * "'estland'": "{'fi': 'Viro'}",*

 * * "'finland'": "{'fi': 'Suomi'}",*

 * * "'france'": "{'fi': 'Ranska'}",*

 * * "'germany'": "{'fi': 'Saksa'}",*

 * * "'hungary'": "{'fi': 'Unkari'}",*

 * * "'iceland'": "{'fi': 'Islanti'}",*

 * * "'japan'": "{'fi': 'Japani'}" […]*

```diff
@@ -2,127 +2,127 @@
     "belgium": {
         "en": "Belgium",
         "fi": "Belgia",
         "nl": "Belgi\u00eb"
     },
     "china": {
         "en": "China",
-        "fi": "Kiina;country",
+        "fi": "Kiina",
         "nl": "China"
     },
     "country": {
         "level": {
             "A1": [
                 "EP",
                 "KK",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Countries",
-            "fi": "Maat",
-            "nl": "De landen"
+            "en": "countries",
+            "fi": "maat;geography",
+            "nl": "de landen"
         },
         "singular": {
-            "en": "Country",
-            "fi": "Maa",
-            "nl": "Het land"
+            "en": "country",
+            "fi": "maa;geography",
+            "nl": "het land"
         }
     },
     "denmark": {
         "en": "Denmark",
-        "fi": "Tanska;country",
+        "fi": "Tanska",
         "nl": "Denemarken"
     },
     "england": {
         "en": "England",
-        "fi": "Englanti;country",
+        "fi": "Englanti",
         "nl": "Engeland",
         "roots": {
             "nl": "country"
         }
     },
     "estland": {
         "en": "Estland",
-        "fi": "Viro;country",
+        "fi": "Viro",
         "nl": "Estland",
         "roots": {
             "nl": "country"
         }
     },
     "finland": {
         "en": "Finland",
-        "fi": "Suomi;country",
+        "fi": "Suomi",
         "nl": "Finland",
         "roots": {
             "nl": "country"
         }
     },
     "france": {
         "en": "France",
-        "fi": "Ranska;country",
+        "fi": "Ranska",
         "nl": "Frankrijk"
     },
     "germany": {
         "en": "Germany",
-        "fi": "Saksa;country",
+        "fi": "Saksa",
         "nl": "Duitsland",
         "roots": {
             "nl": "country"
         }
     },
     "hungary": {
         "en": "Hungary",
-        "fi": "Unkari;country",
+        "fi": "Unkari",
         "nl": "Hongarije"
     },
     "iceland": {
         "en": "Iceland",
-        "fi": "Islanti;country",
+        "fi": "Islanti",
         "nl": "IJsland",
         "roots": {
             "nl": "country"
         }
     },
     "japan": {
         "en": "Japan",
-        "fi": "Japani;country",
+        "fi": "Japani",
         "nl": "Japan"
     },
     "korea": {
         "en": "Korea",
-        "fi": "Korea;country",
+        "fi": "Korea",
         "nl": "Korea"
     },
     "netherlands": {
         "en": "The Netherlands",
         "fi": "Alankomaat",
         "nl": "Nederland",
         "roots": {
             "fi": "country",
             "nl": "country"
         }
     },
     "norway": {
         "en": "Norway",
-        "fi": "Norja;country",
+        "fi": "Norja",
         "nl": "Noorwegen"
     },
     "russia": {
         "en": "Russia",
-        "fi": "Ven\u00e4j\u00e4;country",
+        "fi": "Ven\u00e4j\u00e4",
         "nl": "Rusland",
         "roots": {
             "nl": "country"
         }
     },
     "spain": {
         "en": "Spain",
-        "fi": "Espanja;country",
+        "fi": "Espanja",
         "nl": "Spanje"
     },
     "sweden": {
         "en": "Sweden",
-        "fi": "Ruotsi;country",
+        "fi": "Ruotsi",
         "nl": "Zweden"
     }
 }
```

### Comparing `Toisto-0.8.2/src/topics/days.json` & `Toisto-0.9.0/src/topics/days.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7821666666666668%*

 * *Differences: {"'day'": "{'singular': {'en': 'day', 'fi': 'päivä', 'nl': 'de dag'}, 'plural': {'en': 'days', "*

 * *          "'fi': 'päivät', 'nl': 'de dagen'}}",*

 * * "'days of the week'": "{'en': 'days of the week', 'fi': 'viikonpäivät', 'nl': 'de dagen van de "*

 * *                       "week'}",*

 * * "'friday'": "{'singular': {'fi': 'perjantai', 'nl': 'vrijdag|de vrijdag'}, 'plural': {'fi': "*

 * *             "'perjantait', 'nl': 'de vrijdagen'}}",*

 * * "'good weekend'": "OrderedDict([('roots', OrderedDict([('en', ['good', 'weekend']), ('f […]*

```diff
@@ -4,233 +4,281 @@
             "A1": [
                 "EP",
                 "KK",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Days",
-            "fi": "P\u00e4iv\u00e4t",
-            "nl": "De dagen"
+            "en": "days",
+            "fi": "p\u00e4iv\u00e4t",
+            "nl": "de dagen"
         },
         "singular": {
-            "en": "Day",
-            "fi": "P\u00e4iv\u00e4",
-            "nl": "De dag"
+            "en": "day",
+            "fi": "p\u00e4iv\u00e4",
+            "nl": "de dag"
         }
     },
     "days of the week": {
-        "en": "Days of the week",
-        "fi": "Viikonp\u00e4iv\u00e4t",
-        "nl": "De dagen van de week",
+        "en": "days of the week",
+        "fi": "viikonp\u00e4iv\u00e4t",
+        "nl": "de dagen van de week",
         "roots": [
             "day",
             "week"
         ]
     },
     "friday": {
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
         "plural": {
             "en": "Fridays",
-            "fi": "Perjantait",
-            "nl": "De vrijdagen"
+            "fi": "perjantait",
+            "nl": "de vrijdagen"
         },
         "roots": {
             "en": "day",
             "nl": "day"
         },
         "singular": {
             "en": "Friday",
-            "fi": "Perjantai",
-            "nl": "Vrijdag|De vrijdag"
+            "fi": "perjantai",
+            "nl": "vrijdag|de vrijdag"
+        }
+    },
+    "good weekend": {
+        "en": "Good weekend!",
+        "fi": "Hauskaa viikonloppua!",
+        "nl": "Prettig weekend!",
+        "roots": {
+            "en": [
+                "good",
+                "weekend"
+            ],
+            "fi": "weekend",
+            "nl": "weekend"
         }
     },
     "last week": {
-        "en": "Last week",
-        "fi": "Viime viikolla",
+        "en": "last week",
+        "fi": "viime viikolla",
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
-        "nl": "Vorige week",
+        "nl": "vorige week",
         "roots": "week"
     },
     "monday": {
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
         "plural": {
             "en": "Mondays",
-            "fi": "Maanantait",
-            "nl": "De maandagen"
+            "fi": "maanantait",
+            "nl": "de maandagen"
         },
         "roots": {
             "en": "day",
             "nl": [
                 "moon",
                 "day"
             ]
         },
         "singular": {
             "en": "Monday",
-            "fi": "Maanantai",
-            "nl": "Maandag|De maandag"
+            "fi": "maanantai",
+            "nl": "maandag|de maandag"
         }
     },
     "next week": {
-        "en": "Next week",
-        "fi": "Ensi viikolla",
+        "en": "next week",
+        "fi": "ensi viikolla",
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
-        "nl": "Volgende week",
+        "nl": "volgende week",
         "roots": "week"
     },
     "on monday": {
-        "en": "On Monday",
-        "fi": "Maanantaina",
-        "nl": "Op maandag",
+        "en": "on Monday",
+        "fi": "maanantaina",
+        "nl": "op maandag",
         "roots": "monday"
     },
     "on wednesday": {
-        "en": "On Wednesday",
-        "fi": "Keskiviikkona",
-        "nl": "Op woensdag",
+        "en": "on Wednesday",
+        "fi": "keskiviikkona",
+        "nl": "op woensdag",
         "roots": "wednesday"
     },
     "saturday": {
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
         "plural": {
             "en": "Saturdays",
-            "fi": "Lauantait",
-            "nl": "De zaterdagen"
+            "fi": "lauantait",
+            "nl": "de zaterdagen"
         },
         "roots": {
             "en": "day",
             "nl": "day"
         },
         "singular": {
             "en": "Saturday",
-            "fi": "Lauantai",
-            "nl": "Zaterdag|De zaterdag"
+            "fi": "lauantai",
+            "nl": "zaterdag|de zaterdag"
         }
     },
     "sunday": {
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
         "plural": {
             "en": "Sundays",
-            "fi": "Sunnuntait",
-            "nl": "De zondagen"
+            "fi": "sunnuntait",
+            "nl": "de zondagen"
         },
         "roots": {
             "en": "day",
             "nl": "day"
         },
         "singular": {
             "en": "Sunday",
-            "fi": "Sunnuntai",
-            "nl": "Zondag|De zondag"
+            "fi": "sunnuntai",
+            "nl": "zondag|de zondag"
+        }
+    },
+    "the day after tomorrow": {
+        "en": "the day after tomorrow",
+        "fi": "ylihuomenna",
+        "level": {
+            "none": [
+                "EP",
+                "OD"
+            ]
+        },
+        "nl": "overmorgen",
+        "roots": {
+            "en": [
+                "day",
+                "tomorrow"
+            ],
+            "fi": "tomorrow",
+            "nl": "tomorrow"
+        }
+    },
+    "the day before yesterday": {
+        "en": "the day before yesterday",
+        "fi": "toissap\u00e4iv\u00e4n\u00e4",
+        "level": {
+            "none": [
+                "EP",
+                "OD"
+            ]
+        },
+        "nl": "eergisteren",
+        "roots": {
+            "en": "yesterday",
+            "fi": "day",
+            "nl": "yesterday"
         }
     },
     "this week": {
-        "en": "This week",
-        "fi": "T\u00e4ll\u00e4 viikolla",
+        "en": "this week",
+        "fi": "t\u00e4ll\u00e4 viikolla",
         "level": {
-            "EP": null,
-            "OD": "A1"
+            "A1": "OD",
+            "none": "EP"
         },
-        "nl": "Deze week",
+        "nl": "deze week",
         "roots": "week"
     },
     "thursday": {
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
         "plural": {
             "en": "Thursdays",
-            "fi": "Torstait",
-            "nl": "De donderdagen"
+            "fi": "torstait",
+            "nl": "de donderdagen"
         },
         "roots": {
             "en": "day",
             "nl": "day"
         },
         "singular": {
             "en": "Thursday",
-            "fi": "Torstai",
-            "nl": "Donderdag|De donderdag"
+            "fi": "torstai",
+            "nl": "donderdag|de donderdag"
         }
     },
     "today": {
-        "en": "Today",
-        "fi": "T\u00e4n\u00e4\u00e4n",
+        "en": "today",
+        "fi": "t\u00e4n\u00e4\u00e4n",
         "level": {
             "A1": [
                 "EP",
                 "KK",
                 "OD"
             ]
         },
-        "nl": "Vandaag",
+        "nl": "vandaag",
         "roots": {
             "en": "day"
         }
     },
     "today it is monday": {
-        "en": "Today it is Monday|Today it's Monday",
-        "fi": "T\u00e4n\u00e4\u00e4n on maanantai",
-        "nl": "Vandaag is het maandag",
+        "en": "Today it is Monday.|Today it's Monday.",
+        "fi": "T\u00e4n\u00e4\u00e4n on maanantai.",
+        "nl": "Vandaag is het maandag.",
         "roots": [
             "today",
             "to be",
             "monday"
         ]
     },
     "tomorrow": {
-        "en": "Tomorrow",
-        "fi": "Huomenna",
+        "en": "tomorrow",
+        "fi": "huomenna",
         "level": {
             "A1": [
                 "EP",
                 "KK",
                 "OD"
             ]
         },
-        "nl": "Morgen"
+        "nl": "morgen"
     },
     "tomorrow it is tuesday": {
-        "en": "Tomorrow it is Tuesday|Tomorrow it's Tuesday",
-        "fi": "Huomenna on tiistai",
-        "nl": "Morgen is het dinsdag",
+        "en": "Tomorrow it is Tuesday.|Tomorrow it's Tuesday.",
+        "fi": "Huomenna on tiistai.",
+        "nl": "Morgen is het dinsdag.",
         "roots": [
             "tomorrow",
             "to be",
             "tuesday"
         ]
     },
     "tuesday": {
@@ -238,107 +286,107 @@
             "A1": [
                 "EP",
                 "OD"
             ]
         },
         "plural": {
             "en": "Tuesdays",
-            "fi": "Tiistait",
-            "nl": "De dinsdagen"
+            "fi": "tiistait",
+            "nl": "de dinsdagen"
         },
         "roots": {
             "en": "day",
             "nl": "day"
         },
         "singular": {
             "en": "Tuesday",
-            "fi": "Tiistai",
-            "nl": "Dinsdag|De dinsdag"
+            "fi": "tiistai",
+            "nl": "dinsdag|de dinsdag"
         }
     },
     "wednesday": {
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
         "plural": {
             "en": "Wednesdays",
-            "fi": "Keskiviikot",
-            "nl": "De woensdagen"
+            "fi": "keskiviikot",
+            "nl": "de woensdagen"
         },
         "roots": {
             "en": "day",
             "fi": "week",
             "nl": "day"
         },
         "singular": {
             "en": "Wednesday",
-            "fi": "Keskiviikko",
-            "nl": "Woensdag|De woensdag"
+            "fi": "keskiviikko",
+            "nl": "woensdag|de woensdag"
         }
     },
     "week": {
         "level": {
             "A1": [
                 "EP",
                 "KK",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Weeks",
-            "fi": "Viikot",
-            "nl": "De weken"
+            "en": "weeks",
+            "fi": "viikot",
+            "nl": "de weken"
         },
         "singular": {
-            "en": "Week",
-            "fi": "Viikko",
-            "nl": "De week"
+            "en": "week",
+            "fi": "viikko",
+            "nl": "de week"
         }
     },
     "weekend": {
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Weekends",
-            "fi": "Viikonloput",
-            "nl": "De weekenden"
+            "en": "weekends",
+            "fi": "viikonloput",
+            "nl": "de weekenden"
         },
         "roots": "week",
         "singular": {
-            "en": "Weekend",
-            "fi": "Viikonloppu",
-            "nl": "Het weekend"
+            "en": "weekend",
+            "fi": "viikonloppu",
+            "nl": "het weekend"
         }
     },
     "what day is it today": {
         "en": "What day is it today?",
         "fi": "Mik\u00e4 p\u00e4iv\u00e4 t\u00e4n\u00e4\u00e4n on?|Mik\u00e4 p\u00e4iv\u00e4 on t\u00e4n\u00e4\u00e4n?",
         "nl": "Welke dag is het vandaag?",
         "roots": [
             "day",
             "to be",
             "today"
         ]
     },
     "yesterday": {
-        "en": "Yesterday",
-        "fi": "Eilen",
+        "en": "yesterday",
+        "fi": "eilen",
         "level": {
             "A1": [
                 "EP",
                 "KK",
                 "OD"
             ]
         },
-        "nl": "Gisteren",
+        "nl": "gisteren",
         "roots": {
             "en": "day"
         }
     }
 }
```

### Comparing `Toisto-0.8.2/src/topics/degrees_of_comparison.json` & `Toisto-0.9.0/src/topics/degrees_of_comparison.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9167968750000003%*

 * *Differences: {"'bad'": "{'positive degree': {'en': 'bad', 'fi': 'huono', 'nl': 'slecht'}, 'comparative degree': "*

 * *          "{'en': 'badder', 'fi': 'huonompi', 'nl': 'slechter'}, 'superlative degree': {'en': "*

 * *          "'baddest', 'fi': 'huonoin', 'nl': 'slechtst'}}",*

 * * "'beautiful'": "{'positive degree': {'en': 'beautiful', 'fi': 'kaunis', 'nl': 'mooi'}, "*

 * *                "'comparative degree': {'en': 'more beautiful', 'fi': 'kauniimpi', 'nl': "*

 * *                "'mooier'}, 'superlative degree': {'en': 'most beautiful', […]*

```diff
@@ -1,779 +1,779 @@
 {
     "bad": {
         "antonym": "good",
         "comparative degree": {
-            "en": "Badder",
-            "fi": "Huonompi",
-            "nl": "Slechter"
+            "en": "badder",
+            "fi": "huonompi",
+            "nl": "slechter"
         },
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
         "positive degree": {
-            "en": "Bad",
-            "fi": "Huono",
-            "nl": "Slecht"
+            "en": "bad",
+            "fi": "huono",
+            "nl": "slecht"
         },
         "superlative degree": {
-            "en": "Baddest",
-            "fi": "Huonoin",
-            "nl": "Slechtst"
+            "en": "baddest",
+            "fi": "huonoin",
+            "nl": "slechtst"
         }
     },
     "beautiful": {
         "comparative degree": {
-            "en": "More beautiful",
-            "fi": "Kauniimpi",
-            "nl": "Mooier"
+            "en": "more beautiful",
+            "fi": "kauniimpi",
+            "nl": "mooier"
         },
         "level": {
             "A1": [
                 "EP",
                 "KK",
                 "OD"
             ]
         },
         "positive degree": {
-            "en": "Beautiful",
-            "fi": "Kaunis",
-            "nl": "Mooi"
+            "en": "beautiful",
+            "fi": "kaunis",
+            "nl": "mooi"
         },
         "superlative degree": {
-            "en": "Most beautiful",
-            "fi": "Kaunein",
-            "nl": "Mooist"
+            "en": "most beautiful",
+            "fi": "kaunein",
+            "nl": "mooist"
         }
     },
     "big": {
         "antonym": "small",
         "comparative degree": {
-            "en": "Bigger",
+            "en": "bigger",
             "fi": [
-                "Isompi",
-                "Suurempi"
+                "isompi",
+                "suurempi"
             ],
-            "nl": "Groter"
+            "nl": "groter"
         },
         "level": {
             "A1": [
                 "EP",
                 "KK",
                 "OD"
             ]
         },
         "positive degree": {
-            "en": "Big",
+            "en": "big",
             "fi": [
-                "Iso",
-                "Suuri"
+                "iso",
+                "suuri"
             ],
-            "nl": "Groot"
+            "nl": "groot"
         },
         "superlative degree": {
-            "en": "Biggest",
+            "en": "biggest",
             "fi": [
-                "Isoin",
-                "Suurin"
+                "isoin",
+                "suurin"
             ],
-            "nl": "Grootst"
+            "nl": "grootst"
         }
     },
     "cheap": {
         "antonym": "expensive",
         "comparative degree": {
-            "en": "Cheaper",
-            "fi": "Halvempi",
-            "nl": "Goedkoper"
+            "en": "cheaper",
+            "fi": "halvempi",
+            "nl": "goedkoper"
         },
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
         "positive degree": {
-            "en": "Cheap",
-            "fi": "Halpa",
-            "nl": "Goedkoop"
+            "en": "cheap",
+            "fi": "halpa",
+            "nl": "goedkoop"
         },
         "superlative degree": {
-            "en": "Cheapest",
-            "fi": "Halvin",
-            "nl": "Goedkoopst"
+            "en": "cheapest",
+            "fi": "halvin",
+            "nl": "goedkoopst"
         }
     },
     "cold": {
         "antonym": "warm",
         "comparative degree": {
-            "en": "Colder",
-            "fi": "Kylmempi",
-            "nl": "Kouder"
+            "en": "colder",
+            "fi": "kylmempi",
+            "nl": "kouder"
         },
         "level": {
             "A1": [
                 "EP",
                 "KK",
                 "OD"
             ]
         },
         "positive degree": {
-            "en": "Cold",
-            "fi": "Kylm\u00e4",
-            "nl": "Koud"
+            "en": "cold",
+            "fi": "kylm\u00e4",
+            "nl": "koud"
         },
         "superlative degree": {
-            "en": "Coldest",
-            "fi": "Kylmin",
-            "nl": "Koudst"
+            "en": "coldest",
+            "fi": "kylmin",
+            "nl": "koudst"
         }
     },
     "cute": {
         "comparative degree": {
-            "en": "Cuter",
-            "fi": "S\u00f6p\u00f6mpi",
-            "nl": "Schattiger"
+            "en": "cuter",
+            "fi": "s\u00f6p\u00f6mpi",
+            "nl": "schattiger"
         },
         "level": {
             "B2": "OD",
             "none": "EP"
         },
         "positive degree": {
-            "en": "Cute",
-            "fi": "S\u00f6p\u00f6",
-            "nl": "Schattig"
+            "en": "cute",
+            "fi": "s\u00f6p\u00f6",
+            "nl": "schattig"
         },
         "superlative degree": {
-            "en": "Cutest",
-            "fi": "S\u00f6p\u00f6in",
-            "nl": "Schattigst"
+            "en": "cutest",
+            "fi": "s\u00f6p\u00f6in",
+            "nl": "schattigst"
         }
     },
     "dry": {
         "antonym": "wet",
         "comparative degree": {
-            "en": "Dryer",
-            "fi": "Kuivempi",
-            "nl": "Droger"
+            "en": "dryer",
+            "fi": "kuivempi",
+            "nl": "droger"
         },
         "level": {
             "A2": [
                 "EP",
                 "OD"
             ]
         },
         "positive degree": {
-            "en": "Dry",
-            "fi": "Kuiva",
-            "nl": "Droog"
+            "en": "dry",
+            "fi": "kuiva",
+            "nl": "droog"
         },
         "superlative degree": {
-            "en": "Dryest",
-            "fi": "Kuivin",
-            "nl": "Droogst"
+            "en": "dryest",
+            "fi": "kuivin",
+            "nl": "droogst"
         }
     },
     "easy": {
         "antonym": "hard",
         "comparative degree": {
-            "en": "Easier",
-            "fi": "Helpompi",
-            "nl": "Makkelijker"
+            "en": "easier",
+            "fi": "helpompi",
+            "nl": "makkelijker"
         },
         "level": {
             "A1": [
                 "EP",
                 "KK",
                 "OD"
             ]
         },
         "positive degree": {
-            "en": "Easy",
-            "fi": "Helppo",
-            "nl": "Makkelijk"
+            "en": "easy",
+            "fi": "helppo",
+            "nl": "makkelijk"
         },
         "superlative degree": {
-            "en": "Easiest",
-            "fi": "Helpoin",
-            "nl": "Makkelijkst"
+            "en": "easiest",
+            "fi": "helpoin",
+            "nl": "makkelijkst"
         }
     },
     "expensive": {
         "antonym": "cheap",
         "comparative degree": {
-            "en": "More expensive",
-            "fi": "Kalliimpi",
-            "nl": "Duurder"
+            "en": "more expensive",
+            "fi": "kalliimpi",
+            "nl": "duurder"
         },
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
         "positive degree": {
-            "en": "Expensive",
-            "fi": "Kallis",
-            "nl": "Duur"
+            "en": "expensive",
+            "fi": "kallis",
+            "nl": "duur"
         },
         "superlative degree": {
-            "en": "Most expensive",
-            "fi": "Kallein",
-            "nl": "Duurst"
+            "en": "most expensive",
+            "fi": "kallein",
+            "nl": "duurst"
         }
     },
     "fast": {
         "antonym": "slow",
         "comparative degree": {
-            "en": "Faster",
-            "fi": "Nopeampi",
-            "nl": "Sneller"
+            "en": "faster",
+            "fi": "nopeampi",
+            "nl": "sneller"
         },
         "level": {
             "A1": [
                 "EP",
                 "KK",
                 "OD"
             ]
         },
         "positive degree": {
-            "en": "Fast",
-            "fi": "Nopea",
-            "nl": "Snel"
+            "en": "fast",
+            "fi": "nopea",
+            "nl": "snel"
         },
         "superlative degree": {
-            "en": "Fastest",
-            "fi": "Nopein",
-            "nl": "Snelst"
+            "en": "fastest",
+            "fi": "nopein",
+            "nl": "snelst"
         }
     },
     "fresh": {
         "comparative degree": {
-            "en": "Fresher",
-            "fi": "Tuoreempi",
-            "nl": "Verser"
+            "en": "fresher",
+            "fi": "tuoreempi",
+            "nl": "verser"
         },
         "level": {
             "A2": [
                 "EP",
                 "OD"
             ]
         },
         "positive degree": {
-            "en": "Fresh",
-            "fi": "Tuore",
-            "nl": "Vers"
+            "en": "fresh",
+            "fi": "tuore",
+            "nl": "vers"
         },
         "superlative degree": {
-            "en": "Freshest",
-            "fi": "Tuorein",
-            "nl": "Verst"
+            "en": "freshest",
+            "fi": "tuorein",
+            "nl": "verst"
         }
     },
     "good": {
         "antonym": "bad",
         "comparative degree": {
-            "en": "Better",
-            "fi": "Parempi",
-            "nl": "Beter"
+            "en": "better",
+            "fi": "parempi",
+            "nl": "beter"
         },
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
         "positive degree": {
-            "en": "Good",
-            "fi": "Hyv\u00e4",
-            "nl": "Goed"
+            "en": "good",
+            "fi": "hyv\u00e4",
+            "nl": "goed"
         },
         "superlative degree": {
-            "en": "Best",
-            "fi": "Paras",
-            "nl": "Best"
+            "en": "best",
+            "fi": "paras",
+            "nl": "best"
         }
     },
     "happy": {
         "comparative degree": {
-            "en": "Happier",
-            "fi": "Onnellisempi",
-            "nl": "Gelukkiger"
+            "en": "happier",
+            "fi": "onnellisempi",
+            "nl": "gelukkiger"
         },
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
         "positive degree": {
-            "en": "Happy",
-            "fi": "Onnellinen",
-            "nl": "Gelukkig"
+            "en": "happy",
+            "fi": "onnellinen",
+            "nl": "gelukkig"
         },
         "superlative degree": {
-            "en": "Happiest",
-            "fi": "Onnellisin",
-            "nl": "Gelukkigst"
+            "en": "happiest",
+            "fi": "onnellisin",
+            "nl": "gelukkigst"
         }
     },
     "hard": {
         "antonym": "easy",
         "comparative degree": {
-            "en": "Harder",
-            "fi": "Vaikeampi",
-            "nl": "Moeilijker"
+            "en": "harder",
+            "fi": "vaikeampi",
+            "nl": "moeilijker"
         },
         "level": {
             "A1": [
                 "EP",
                 "KK",
                 "OD"
             ]
         },
         "positive degree": {
-            "en": "Hard",
-            "fi": "Vaikea",
-            "nl": "Moeilijk"
+            "en": "hard",
+            "fi": "vaikea",
+            "nl": "moeilijk"
         },
         "superlative degree": {
-            "en": "Hardest",
-            "fi": "Vaikein",
-            "nl": "Moeilijkst"
+            "en": "hardest",
+            "fi": "vaikein",
+            "nl": "moeilijkst"
         }
     },
     "honest": {
         "comparative degree": {
-            "en": "More honest",
-            "fi": "Rehellisempi",
-            "nl": "Eerlijker"
+            "en": "more honest",
+            "fi": "rehellisempi",
+            "nl": "eerlijker"
         },
         "level": {
             "B1": [
                 "EP",
                 "OD"
             ]
         },
         "positive degree": {
-            "en": "Honest",
-            "fi": "Rehellinen",
-            "nl": "Eerlijk"
+            "en": "honest",
+            "fi": "rehellinen",
+            "nl": "eerlijk"
         },
         "superlative degree": {
-            "en": "Most honest",
-            "fi": "Rehellisin",
-            "nl": "Eerlijkst"
+            "en": "most honest",
+            "fi": "rehellisin",
+            "nl": "eerlijkst"
         }
     },
     "hot": {
         "comparative degree": {
-            "en": "Hotter",
-            "fi": "Kuumempi",
-            "nl": "Heter"
+            "en": "hotter",
+            "fi": "kuumempi",
+            "nl": "heter"
         },
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
         "positive degree": {
-            "en": "Hot",
-            "fi": "Kuuma",
-            "nl": "Heet"
+            "en": "hot",
+            "fi": "kuuma",
+            "nl": "heet"
         },
         "superlative degree": {
-            "en": "Hottest",
-            "fi": "Kuumin",
-            "nl": "Heetst"
+            "en": "hottest",
+            "fi": "kuumin",
+            "nl": "heetst"
         }
     },
     "important": {
         "comparative degree": {
-            "en": "More important",
-            "fi": "T\u00e4rke\u00e4mpi",
-            "nl": "Belangrijker"
+            "en": "more important",
+            "fi": "t\u00e4rke\u00e4mpi",
+            "nl": "belangrijker"
         },
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
         "positive degree": {
-            "en": "Important",
-            "fi": "T\u00e4rke\u00e4",
-            "nl": "Belangrijk"
+            "en": "important",
+            "fi": "t\u00e4rke\u00e4",
+            "nl": "belangrijk"
         },
         "superlative degree": {
-            "en": "Most important",
-            "fi": "T\u00e4rkein",
-            "nl": "Belangrijkst"
+            "en": "most important",
+            "fi": "t\u00e4rkein",
+            "nl": "belangrijkst"
         }
     },
     "light (not heavy)": {
         "comparative degree": {
-            "en": "Lighter",
-            "fi": "Kevyempi",
-            "nl": "Lichter"
+            "en": "lighter",
+            "fi": "kevyempi",
+            "nl": "lichter"
         },
         "level": {
             "A1": "OD",
             "A2": "EP"
         },
         "positive degree": {
-            "en": "Light",
-            "fi": "Kevyt",
-            "nl": "Licht"
+            "en": "light",
+            "fi": "kevyt",
+            "nl": "licht"
         },
         "superlative degree": {
-            "en": "Lightest",
-            "fi": "Kevyin",
-            "nl": "Lichtst"
+            "en": "lightest",
+            "fi": "kevyin",
+            "nl": "lichtst"
         }
     },
     "long": {
         "antonym": "short",
         "comparative degree": {
-            "en": "Longer",
-            "fi": "Pidempi",
-            "nl": "Langer"
+            "en": "longer",
+            "fi": "pidempi",
+            "nl": "langer"
         },
         "level": {
             "A1": [
                 "EP",
                 "KK",
                 "OD"
             ]
         },
         "positive degree": {
-            "en": "Long",
-            "fi": "Pitk\u00e4",
-            "nl": "Lang"
+            "en": "long",
+            "fi": "pitk\u00e4",
+            "nl": "lang"
         },
         "superlative degree": {
-            "en": "Longest",
-            "fi": "Pisin",
-            "nl": "Langst"
+            "en": "longest",
+            "fi": "pisin",
+            "nl": "langst"
         }
     },
     "new": {
         "antonym": "old",
         "comparative degree": {
-            "en": "Newer",
-            "fi": "Uudempi",
-            "nl": "Nieuwer"
+            "en": "newer",
+            "fi": "uudempi",
+            "nl": "nieuwer"
         },
         "level": {
             "A1": [
                 "EP",
                 "KK",
                 "OD"
             ]
         },
         "positive degree": {
-            "en": "New",
-            "fi": "Uusi",
-            "nl": "Nieuw"
+            "en": "new",
+            "fi": "uusi",
+            "nl": "nieuw"
         },
         "superlative degree": {
-            "en": "Newest",
-            "fi": "Uusin",
-            "nl": "Nieuwst"
+            "en": "newest",
+            "fi": "uusin",
+            "nl": "nieuwst"
         }
     },
     "nice": {
         "comparative degree": {
-            "en": "Nicer",
+            "en": "nicer",
             "fi": [
-                "Kivampi|Kivempt",
-                "Mukavampi"
+                "kivampi|kivempt",
+                "mukavampi"
             ],
-            "nl": "Leuker"
+            "nl": "leuker"
         },
         "level": {
             "A1": [
                 "EP",
                 "KK",
                 "OD"
             ]
         },
         "positive degree": {
-            "en": "Nice",
+            "en": "nice",
             "fi": [
-                "Kiva",
-                "Mukava"
+                "kiva",
+                "mukava"
             ],
-            "nl": "Leuk"
+            "nl": "leuk"
         },
         "superlative degree": {
-            "en": "Nicest",
+            "en": "nicest",
             "fi": [
-                "Kivoin",
-                "Mukavin"
+                "kivoin",
+                "mukavin"
             ],
-            "nl": "Leukst"
+            "nl": "leukst"
         }
     },
     "old": {
         "antonym": "new",
         "comparative degree": {
-            "en": "Older",
-            "fi": "Vanhempi",
-            "nl": "Ouder"
+            "en": "older",
+            "fi": "vanhempi",
+            "nl": "ouder"
         },
         "level": {
             "A1": [
                 "EP",
                 "KK",
                 "OD"
             ]
         },
         "positive degree": {
-            "en": "Old",
-            "fi": "Vanha",
-            "nl": "Oud"
+            "en": "old",
+            "fi": "vanha",
+            "nl": "oud"
         },
         "superlative degree": {
-            "en": "Oldest",
-            "fi": "Vanhin",
-            "nl": "Oudst"
+            "en": "oldest",
+            "fi": "vanhin",
+            "nl": "oudst"
         }
     },
     "quiet": {
         "comparative degree": {
-            "en": "Quieter",
-            "fi": "Hiljaisempi",
-            "nl": "Stiller"
+            "en": "quieter",
+            "fi": "hiljaisempi",
+            "nl": "stiller"
         },
         "level": {
             "A1": "OD",
             "A2": "EP"
         },
         "positive degree": {
-            "en": "Quiet",
-            "fi": "Hiljainen",
-            "nl": "Stil"
+            "en": "quiet",
+            "fi": "hiljainen",
+            "nl": "stil"
         },
         "superlative degree": {
-            "en": "Quietest",
-            "fi": "Hiljaisin",
-            "nl": "Stilst"
+            "en": "quietest",
+            "fi": "hiljaisin",
+            "nl": "stilst"
         }
     },
     "round": {
         "comparative degree": {
-            "en": "Rounder",
-            "fi": "Py\u00f6re\u00e4mpi",
-            "nl": "Ronder"
+            "en": "rounder",
+            "fi": "py\u00f6re\u00e4mpi",
+            "nl": "ronder"
         },
         "level": {
             "A2": [
                 "EP",
                 "OD"
             ]
         },
         "positive degree": {
-            "en": "Round",
-            "fi": "Py\u00f6re\u00e4",
-            "nl": "Rond"
+            "en": "round",
+            "fi": "py\u00f6re\u00e4",
+            "nl": "rond"
         },
         "superlative degree": {
-            "en": "Roundest",
-            "fi": "Py\u00f6rein",
-            "nl": "Rondst"
+            "en": "roundest",
+            "fi": "py\u00f6rein",
+            "nl": "rondst"
         }
     },
     "short": {
         "antonym": "long",
         "comparative degree": {
-            "en": "Shorter",
-            "fi": "Lyhyempi",
-            "nl": "Korter"
+            "en": "shorter",
+            "fi": "lyhyempi",
+            "nl": "korter"
         },
         "level": {
             "A1": [
                 "EP",
                 "KK",
                 "OD"
             ]
         },
         "positive degree": {
-            "en": "Short",
-            "fi": "Lyhyt",
-            "nl": "Kort"
+            "en": "short",
+            "fi": "lyhyt",
+            "nl": "kort"
         },
         "superlative degree": {
-            "en": "Shortest",
-            "fi": "Lyhyin",
-            "nl": "Kortst"
+            "en": "shortest",
+            "fi": "lyhyin",
+            "nl": "kortst"
         }
     },
     "slow": {
         "antonym": "fast",
         "comparative degree": {
-            "en": "Slower",
-            "fi": "Hitaampi",
-            "nl": "Langzamer"
+            "en": "slower",
+            "fi": "hitaampi",
+            "nl": "langzamer"
         },
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
         "positive degree": {
-            "en": "Slow",
-            "fi": "Hidas",
-            "nl": "Langzaam"
+            "en": "slow",
+            "fi": "hidas",
+            "nl": "langzaam"
         },
         "superlative degree": {
-            "en": "Slowest",
-            "fi": "Hitain",
-            "nl": "Langzaamst"
+            "en": "slowest",
+            "fi": "hitain",
+            "nl": "langzaamst"
         }
     },
     "small": {
         "antonym": "big",
         "comparative degree": {
-            "en": "Smaller",
-            "fi": "Pienempi",
-            "nl": "Kleiner"
+            "en": "smaller",
+            "fi": "pienempi",
+            "nl": "kleiner"
         },
         "level": {
             "A1": [
                 "EP",
                 "KK",
                 "OD"
             ]
         },
         "positive degree": {
-            "en": "Small",
-            "fi": "Pieni",
-            "nl": "Klein"
+            "en": "small",
+            "fi": "pieni",
+            "nl": "klein"
         },
         "superlative degree": {
-            "en": "Smallest",
-            "fi": "Pienin",
-            "nl": "Kleinst"
+            "en": "smallest",
+            "fi": "pienin",
+            "nl": "kleinst"
         }
     },
     "strange": {
         "comparative degree": {
-            "en": "Stranger",
-            "fi": "Oudompi",
-            "nl": "Vreemder"
+            "en": "stranger",
+            "fi": "oudompi",
+            "nl": "vreemder"
         },
         "level": {
             "A1": "KK",
             "A2": [
                 "EP",
                 "OD"
             ]
         },
         "positive degree": {
-            "en": "Strange",
-            "fi": "Outo",
-            "nl": "Vreemd"
+            "en": "strange",
+            "fi": "outo",
+            "nl": "vreemd"
         },
         "superlative degree": {
-            "en": "Strangest",
-            "fi": "Oudoin",
-            "nl": "Vreemdst"
+            "en": "strangest",
+            "fi": "oudoin",
+            "nl": "vreemdst"
         }
     },
     "sweet": {
         "comparative degree": {
-            "en": "Sweter",
-            "fi": "Makeampi",
-            "nl": "Zoeter"
+            "en": "sweeter",
+            "fi": "makeampi",
+            "nl": "zoeter"
         },
         "level": {
             "A1": "EP",
             "A2": "OD"
         },
         "positive degree": {
-            "en": "Sweet",
-            "fi": "Makea",
-            "nl": "Zoet"
+            "en": "sweet",
+            "fi": "makea",
+            "nl": "zoet"
         },
         "superlative degree": {
-            "en": "Sweetest",
-            "fi": "Makein",
-            "nl": "Zoetst"
+            "en": "sweetest",
+            "fi": "makein",
+            "nl": "zoetst"
         }
     },
     "tasty": {
         "comparative degree": {
-            "en": "Tastier",
-            "fi": "Maukkaampi",
-            "nl": "Lekkerder"
+            "en": "tastier",
+            "fi": "maukkaampi",
+            "nl": "lekkerder"
         },
         "level": {
             "B1": [
                 "EP",
                 "OD"
             ]
         },
         "positive degree": {
-            "en": "Tasty",
-            "fi": "Maukas",
-            "nl": "Lekker"
+            "en": "tasty",
+            "fi": "maukas",
+            "nl": "lekker"
         },
         "superlative degree": {
-            "en": "Tastiest",
-            "fi": "Maukkain",
-            "nl": "Lekkerst"
+            "en": "tastiest",
+            "fi": "maukkain",
+            "nl": "lekkerst"
         }
     },
     "warm": {
         "antonym": "cold",
         "comparative degree": {
-            "en": "Warmer",
-            "fi": "L\u00e4mpim\u00e4mpi",
-            "nl": "Warmer"
+            "en": "warmer",
+            "fi": "l\u00e4mpim\u00e4mpi",
+            "nl": "warmer"
         },
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
         "positive degree": {
-            "en": "Warm",
-            "fi": "L\u00e4mmin",
-            "nl": "Warm"
+            "en": "warm",
+            "fi": "l\u00e4mmin",
+            "nl": "warm"
         },
         "superlative degree": {
-            "en": "Warmest",
-            "fi": "L\u00e4mpimin",
-            "nl": "Warmst"
+            "en": "warmest",
+            "fi": "l\u00e4mpimin",
+            "nl": "warmst"
         }
     },
     "wet": {
         "antonym": "dry",
         "comparative degree": {
-            "en": "Wetter",
-            "fi": "M\u00e4rempi",
-            "nl": "Natter"
+            "en": "wetter",
+            "fi": "m\u00e4rempi",
+            "nl": "natter"
         },
         "level": {
             "A2": [
                 "EP",
                 "OD"
             ]
         },
         "positive degree": {
-            "en": "Wet",
-            "fi": "M\u00e4rk\u00e4",
-            "nl": "Nat"
+            "en": "wet",
+            "fi": "m\u00e4rk\u00e4",
+            "nl": "nat"
         },
         "superlative degree": {
-            "en": "Wettest",
-            "fi": "M\u00e4rin",
-            "nl": "Natst"
+            "en": "wettest",
+            "fi": "m\u00e4rin",
+            "nl": "natst"
         }
     }
 }
```

### Comparing `Toisto-0.8.2/src/topics/family.json` & `Toisto-0.9.0/src/topics/family.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8529040404040403%*

 * *Differences: {"'I am an only child'": '{\'en\': "I am an only child.|I\'m an only child.", \'fi\': \'Olen ainoa '*

 * *                         "lapsi.|Minä olen ainoa lapsi.', 'nl': 'Ik ben enig kind.|Ik ben enigst "*

 * *                         "kind.'}",*

 * * "'I have no siblings'": "{'en': ['I have no siblings.', 'I have no brothers and sisters.'], 'fi': "*

 * *                         "['Minulla ei ole sisaruksia.', 'Minulla ei ole veljiä tai siskoja.'], "*

 * *                         "'nl': 'Ik heb geen broers en zussen.'}",*

 * * "'I have  […]*

```diff
@@ -1,325 +1,364 @@
 {
     "I am an only child": {
-        "en": "I am an only child|I'm an only child",
-        "fi": "Olen ainoa lapsi|Min\u00e4 olen ainoa lapsi",
-        "nl": "Ik ben enig kind|Ik ben enigst kind",
+        "en": "I am an only child.|I'm an only child.",
+        "fi": "Olen ainoa lapsi.|Min\u00e4 olen ainoa lapsi.",
+        "nl": "Ik ben enig kind.|Ik ben enigst kind.",
         "roots": [
             "to be",
             "child"
         ]
     },
     "I have no siblings": {
         "en": [
-            "I have no siblings",
-            "I have no brothers and sisters"
+            "I have no siblings.",
+            "I have no brothers and sisters."
         ],
         "fi": [
-            "Minulla ei ole sisaruksia",
-            "Minulla ei ole velji\u00e4 tai siskoja"
+            "Minulla ei ole sisaruksia.",
+            "Minulla ei ole velji\u00e4 tai siskoja."
         ],
-        "nl": "Ik heb geen broers en zussen",
+        "nl": "Ik heb geen broers en zussen.",
         "roots": [
             "to have",
             "sibling"
         ]
     },
     "I have x brothers and y sisters": {
-        "en": "I have two brothers and one sister",
-        "fi": "Minulla on kaksi velje\u00e4 ja yksi sisko",
-        "nl": "Ik heb twee broers en \u00e9\u00e9n zus|Ik heb twee broers en een zus",
+        "en": "I have two brothers and one sister.",
+        "fi": "Minulla on kaksi velje\u00e4 ja yksi sisko.",
+        "nl": "Ik heb twee broers en \u00e9\u00e9n zus|Ik heb twee broers en een zus.",
         "roots": [
             "to have",
             "2",
             "brother",
             "1",
             "sister"
         ]
     },
     "brother": {
+        "diminutive": {
+            "plural": {
+                "en": "(little brothers)",
+                "fi": "pikkuveljet",
+                "nl": "de broertjes"
+            },
+            "singular": {
+                "en": "(little brother)",
+                "fi": "pikkuveli",
+                "nl": "het broertje"
+            }
+        },
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
-        "plural": {
-            "en": "Brothers",
-            "fi": "Veljet",
-            "nl": "De broers"
-        },
-        "singular": {
-            "en": "Brother",
-            "fi": "Veli",
-            "nl": "De broer"
+        "root": {
+            "plural": {
+                "en": "brothers",
+                "fi": "veljet",
+                "nl": "de broers"
+            },
+            "singular": {
+                "en": "brother",
+                "fi": "veli",
+                "nl": "de broer"
+            }
         }
     },
     "child": {
+        "diminutive": {
+            "plural": {
+                "en": "(little children)",
+                "fi": "(pienet lapset)",
+                "nl": [
+                    "de kindjes",
+                    "de kindertjes"
+                ]
+            },
+            "singular": {
+                "en": "(little child)",
+                "fi": "(pieni lapsi)",
+                "nl": "het kindje"
+            }
+        },
         "level": {
             "A1": [
                 "EP",
                 "KK",
                 "OD"
             ]
         },
-        "plural": {
-            "en": "Children",
-            "fi": "Lapset",
-            "nl": "De kinderen"
-        },
-        "singular": {
-            "en": "Child",
-            "fi": "Lapsi",
-            "nl": "Het kind"
+        "root": {
+            "plural": {
+                "en": "children",
+                "fi": "lapset",
+                "nl": "de kinderen"
+            },
+            "singular": {
+                "en": "child",
+                "fi": "lapsi",
+                "nl": "het kind"
+            }
         }
     },
     "cousin": {
         "level": {
             "A1": "OD",
             "A2": "EP"
         },
         "plural": {
-            "en": "Cousins",
-            "fi": "Serkut",
-            "nl": [
-                "De neven",
-                "De nichten"
-            ]
+            "en": "cousins",
+            "fi": "serkut",
+            "nl": "(de neven en nichten)"
         },
         "singular": {
-            "en": "Cousin",
-            "fi": "Serkku",
-            "nl": [
-                "De neef",
-                "De nicht"
-            ]
+            "en": "cousin",
+            "fi": "serkku",
+            "nl": "(de neef of nicht)"
         }
     },
     "daughter": {
+        "diminutive": {
+            "plural": {
+                "en": "(little  daughters)",
+                "fi": "(pienet tyt\u00e4ret)",
+                "nl": "de dochtertjes"
+            },
+            "singular": {
+                "en": "(little  daughter)",
+                "fi": "(pieni tyt\u00e4r)",
+                "nl": "het dochtertje"
+            }
+        },
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
-        "plural": {
-            "en": "Daughters",
-            "fi": "Tytt\u00e4ret",
-            "nl": "De dochters"
-        },
-        "singular": {
-            "en": "Daughter",
-            "fi": "Tyt\u00e4r",
-            "nl": "De dochter"
+        "root": {
+            "plural": {
+                "en": "daughters",
+                "fi": "tytt\u00e4ret",
+                "nl": "de dochters"
+            },
+            "singular": {
+                "en": "daughter",
+                "fi": "tyt\u00e4r",
+                "nl": "de dochter"
+            }
         }
     },
     "divorced": {
-        "en": "Divorced",
-        "fi": "Eronnut",
+        "en": "divorced",
+        "fi": "eronnut",
         "level": {
             "A2": "OD",
             "B1": "EP"
         },
-        "nl": "Gescheiden"
+        "nl": "gescheiden"
     },
     "family": {
-        "en": "Family",
-        "fi": "Perhe",
+        "en": "family",
+        "fi": "perhe",
         "level": {
             "A1": [
                 "EP",
                 "KK",
                 "OD"
             ]
         },
-        "nl": "De familie"
+        "nl": "de familie"
     },
     "father": {
         "level": {
             "A1": [
                 "EP",
                 "KK",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Fathers",
-            "fi": "Is\u00e4t",
-            "nl": "De vaders"
+            "en": "fathers",
+            "fi": "is\u00e4t",
+            "nl": "de vaders"
         },
         "singular": {
-            "en": "Father",
-            "fi": "Is\u00e4",
-            "nl": "De vader"
+            "en": "father",
+            "fi": "is\u00e4",
+            "nl": "de vader"
         }
     },
     "father-in-law": {
         "level": {
             "B1": "OD",
             "B2": "EP"
         },
         "plural": {
-            "en": "Fathers-in-law",
-            "fi": "Appiukot",
-            "nl": "De schoonvaders"
+            "en": "fathers-in-law",
+            "fi": "appiukot",
+            "nl": "de schoonvaders"
         },
         "roots": "father",
         "singular": {
-            "en": "Father-in-law",
-            "fi": "Appiukko",
-            "nl": "De schoonvader"
+            "en": "father-in-law",
+            "fi": "appiukko",
+            "nl": "de schoonvader"
         }
     },
     "grandchild": {
         "level": {
             "A1": "OD",
             "A2": "EP"
         },
         "plural": {
-            "en": "Grandchildren",
-            "fi": "Lapsenlapset",
-            "nl": "De kleinkinderen"
+            "en": "grandchildren",
+            "fi": "lapsenlapset",
+            "nl": "de kleinkinderen"
         },
         "roots": {
             "en": "child",
             "fi": "child",
             "nl": [
                 "small",
                 "child"
             ]
         },
         "singular": {
-            "en": "Grandchild",
-            "fi": "Lapsenlapsi",
-            "nl": "Het kleinkind"
+            "en": "grandchild",
+            "fi": "lapsenlapsi",
+            "nl": "het kleinkind"
         }
     },
     "grandfather": {
         "level": {
             "A1": "OD",
             "A2": "EP"
         },
         "plural": {
-            "en": "Grandfathers",
-            "fi": "Isois\u00e4t",
-            "nl": "De grootvaders"
+            "en": "grandfathers",
+            "fi": "isois\u00e4t",
+            "nl": "de grootvaders"
         },
         "roots": {
             "en": "father",
             "fi": [
                 "big",
                 "father"
             ],
             "nl": [
                 "big",
                 "father"
             ]
         },
         "singular": {
-            "en": "Grandfather",
-            "fi": "Isois\u00e4",
-            "nl": "De grootvader"
+            "en": "grandfather",
+            "fi": "isois\u00e4",
+            "nl": "de grootvader"
         }
     },
     "grandma": {
         "level": {
             "A1": "OD",
             "A2": "EP"
         },
         "plural": {
-            "en": "Grandmas",
+            "en": "grandmas",
             "fi": [
-                "Mummot",
-                "Mummit"
+                "mummot",
+                "mummit"
             ],
-            "nl": "De oma's"
+            "nl": "de oma's"
         },
         "singular": {
-            "en": "Grandma",
+            "en": "grandma",
             "fi": [
-                "Mummo",
-                "Mummi"
+                "mummo",
+                "mummi"
             ],
-            "nl": "De oma"
+            "nl": "de oma"
         }
     },
     "grandmother": {
         "level": {
             "A1": "OD",
             "A2": "EP"
         },
         "plural": {
-            "en": "Grandmothers",
-            "fi": "Iso\u00e4idit",
-            "nl": "De grootmoeders"
+            "en": "grandmothers",
+            "fi": "iso\u00e4idit",
+            "nl": "de grootmoeders"
         },
         "roots": {
             "en": "mother",
             "fi": [
                 "big",
                 "mother"
             ],
             "nl": [
                 "big",
                 "mother"
             ]
         },
         "singular": {
-            "en": "Grandmother",
-            "fi": "Iso\u00e4iti",
-            "nl": "De grootmoeder"
+            "en": "grandmother",
+            "fi": "iso\u00e4iti",
+            "nl": "de grootmoeder"
         }
     },
     "grandpa": {
         "level": {
             "A1": "OD",
             "A2": "EP"
         },
         "plural": {
-            "en": "Grandpas",
+            "en": "grandpas",
             "fi": [
-                "Vaarit",
-                "Ukit"
+                "vaarit",
+                "ukit"
             ],
-            "nl": "De opa's"
+            "nl": "de opa's"
         },
         "singular": {
-            "en": "Grandpa",
+            "en": "grandpa",
             "fi": [
-                "Vaari",
-                "Ukki"
+                "vaari",
+                "ukki"
             ],
-            "nl": "De opa"
+            "nl": "de opa"
         }
     },
     "grandparent": {
         "level": {
             "A1": "OD",
             "A2": "EP"
         },
         "plural": {
-            "en": "Grandparents",
-            "fi": "Isovanhemmat",
-            "nl": "De grootouders"
+            "en": "grandparents",
+            "fi": "isovanhemmat",
+            "nl": "de grootouders"
         },
         "roots": {
             "en": "parent",
             "fi": [
                 "big",
                 "parent"
             ],
             "nl": [
                 "big",
                 "parent"
             ]
         },
         "singular": {
-            "en": "Grandparent",
-            "fi": "Isovanhempi",
-            "nl": "De grootouder"
+            "en": "grandparent",
+            "fi": "isovanhempi",
+            "nl": "de grootouder"
         }
     },
     "how many brothers and sisters do you have": {
         "en": "How many brothers and sisters do you have?",
         "fi": "Kuinka monta velje\u00e4 ja siskoa sinulla on?",
         "nl": "Hoeveel broers en zussen heb jij?|Hoeveel broers en zussen heb je?",
         "roots": [
@@ -334,237 +373,265 @@
             "A1": [
                 "EP",
                 "KK",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Husbands",
-            "fi": "Aviomiehet|Miehet",
-            "nl": "De echtgenoten"
+            "en": "husbands",
+            "fi": "aviomiehet|miehet",
+            "nl": "de echtgenoten"
         },
         "singular": {
-            "en": "Husband",
-            "fi": "Aviomies|Mies",
-            "nl": "De echtgenoot"
+            "en": "husband",
+            "fi": "aviomies|mies",
+            "nl": "de echtgenoot"
         }
     },
     "marriage": {
-        "en": "Marriage",
-        "fi": "Avioliitto",
+        "en": "marriage",
+        "fi": "avioliitto",
         "level": {
             "B1": [
                 "EP",
                 "OD"
             ]
         },
-        "nl": "Het huwelijk"
+        "nl": "het huwelijk"
     },
     "married": {
-        "en": "Married",
-        "fi": "Naimisissa",
+        "en": "married",
+        "fi": "naimisissa",
         "level": {
             "A1": "OD",
             "A2": "EP"
         },
-        "nl": "Getrouwd"
+        "nl": "getrouwd"
     },
     "mother": {
         "level": {
             "A1": [
                 "EP",
                 "KK",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Mothers",
-            "fi": "\u00c4idit",
-            "nl": "De moeders"
+            "en": "mothers",
+            "fi": "\u00e4idit",
+            "nl": "de moeders"
         },
         "singular": {
-            "en": "Mother",
-            "fi": "\u00c4iti",
-            "nl": "De moeder"
+            "en": "mother",
+            "fi": "\u00e4iti",
+            "nl": "de moeder"
         }
     },
     "mother-in-law": {
         "level": {
             "B1": "OD",
             "B2": "EP"
         },
         "plural": {
-            "en": "Mothers-in-law",
-            "fi": "Anopit",
-            "nl": "De schoonmoeders"
+            "en": "mothers-in-law",
+            "fi": "anopit",
+            "nl": "de schoonmoeders"
         },
         "roots": "mother",
         "singular": {
-            "en": "Mother-in-law",
-            "fi": "Anoppi",
-            "nl": "De schoonmoeder"
+            "en": "mother-in-law",
+            "fi": "anoppi",
+            "nl": "de schoonmoeder"
         }
     },
     "parent": {
         "level": {
             "A1": [
                 "EP",
                 "KK",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Parents",
-            "fi": "Vanhemmat",
-            "nl": "De ouders"
+            "en": "parents",
+            "fi": "vanhemmat",
+            "nl": "de ouders"
         },
         "roots": {
             "fi": "old",
             "nl": "old"
         },
         "singular": {
-            "en": "Parent",
-            "fi": "Vanhempi",
-            "nl": "De ouder"
+            "en": "parent",
+            "fi": "vanhempi;family",
+            "nl": "de ouder"
         }
     },
     "parent-in-law": {
         "level": {
             "B1": "OD",
             "none": "EP"
         },
         "plural": {
-            "en": "Parents-in-law",
-            "fi": "Appivanhemmat",
-            "nl": "De schoonouders"
+            "en": "parents-in-law",
+            "fi": "appivanhemmat",
+            "nl": "de schoonouders"
         },
         "roots": "parent",
         "singular": {
-            "en": "Parent-in-law",
-            "fi": "Appivanhempi",
-            "nl": "De schoonouder"
+            "en": "parent-in-law",
+            "fi": "appivanhempi",
+            "nl": "de schoonouder"
         }
     },
     "sibling": {
         "level": {
             "B2": "OD",
             "C2": "EP"
         },
         "plural": {
-            "en": "Siblings",
-            "fi": "Sisarukset",
-            "nl": "De broers of zussen|De zussen of broers"
+            "en": "siblings",
+            "fi": "sisarukset",
+            "nl": "(de broers en zussen)"
         },
         "roots": {
             "nl": [
                 "brother",
                 "sister"
             ]
         },
         "singular": {
-            "en": "Sibling",
-            "fi": "Sisarus",
-            "nl": "De broer of zus|De zus of broer"
+            "en": "sibling",
+            "fi": "sisarus",
+            "nl": "(de broer of zus)"
         }
     },
     "sister": {
+        "diminutive": {
+            "plural": {
+                "en": "(little sisters)",
+                "fi": "pikkusiskot",
+                "nl": "de zusjes"
+            },
+            "singular": {
+                "en": "(little sister)",
+                "fi": "pikkusisko",
+                "nl": "het zusje"
+            }
+        },
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
-        "plural": {
-            "en": "Sisters",
-            "fi": "Siskot",
-            "nl": "De zussen"
-        },
-        "singular": {
-            "en": "Sister",
-            "fi": "Sisko",
-            "nl": "De zus"
+        "root": {
+            "plural": {
+                "en": "sisters",
+                "fi": "siskot",
+                "nl": "de zussen"
+            },
+            "singular": {
+                "en": "sister",
+                "fi": "sisko",
+                "nl": "de zus"
+            }
         }
     },
     "son": {
+        "diminutive": {
+            "plural": {
+                "en": "(little sons)",
+                "fi": "(pienet pojat)",
+                "nl": "de zoontjes"
+            },
+            "singular": {
+                "en": "(little son)",
+                "fi": "(pieni poika)",
+                "nl": "het zoontje"
+            }
+        },
         "level": {
             "A1": [
                 "EP",
                 "KK",
                 "OD"
             ]
         },
-        "plural": {
-            "en": "Sons",
-            "fi": "Pojat",
-            "nl": "De zonen"
-        },
-        "singular": {
-            "en": "Son",
-            "fi": "Poika",
-            "nl": "De zoon"
+        "root": {
+            "plural": {
+                "en": "sons",
+                "fi": "pojat",
+                "nl": "de zonen"
+            },
+            "singular": {
+                "en": "son",
+                "fi": "poika",
+                "nl": "de zoon"
+            }
         }
     },
     "spouse": {
         "level": {
             "C1": "OD",
             "C2": "OD"
         },
         "plural": {
-            "en": "Spouses",
-            "fi": "Puolisot",
-            "nl": "De partners"
+            "en": "spouses",
+            "fi": "puolisot",
+            "nl": "de partners"
         },
         "singular": {
-            "en": "Spouse",
-            "fi": "Puoliso",
-            "nl": "De partner"
+            "en": "spouse",
+            "fi": "puoliso",
+            "nl": "de partner"
         }
     },
     "stepfather": {
         "level": {
             "B2": [
                 "EP",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Stepfathers",
-            "fi": "Is\u00e4puolet",
-            "nl": "De stiefvaders"
+            "en": "stepfathers",
+            "fi": "is\u00e4puolet",
+            "nl": "de stiefvaders"
         },
         "roots": "father",
         "singular": {
-            "en": "Stepfather",
-            "fi": "Is\u00e4puoli",
-            "nl": "De stiefvader"
+            "en": "stepfather",
+            "fi": "is\u00e4puoli",
+            "nl": "de stiefvader"
         }
     },
     "stepmother": {
         "level": {
             "B2": [
                 "EP",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Stepmothers",
-            "fi": "\u00c4itipuolet",
-            "nl": "De stiefmoeders"
+            "en": "stepmothers",
+            "fi": "\u00e4itipuolet",
+            "nl": "de stiefmoeders"
         },
         "roots": "mother",
         "singular": {
-            "en": "Stepmother",
-            "fi": "\u00c4itipuoli",
-            "nl": "De stiefmoeder"
+            "en": "stepmother",
+            "fi": "\u00e4itipuoli",
+            "nl": "de stiefmoeder"
         }
     },
     "they have x children and y grandchildren": {
-        "en": "They have three children and six grandchildren",
-        "fi": "Heill\u00e4 on kolme lasta ja kuusi lastenlasta",
-        "nl": "Zij hebben drie kinderen en zes kleinkinderen|Ze hebben drie kinderen en zes kleinkinderen",
+        "en": "They have three children and six grandchildren.",
+        "fi": "Heill\u00e4 on kolme lasta ja kuusi lastenlasta.",
+        "nl": "Zij hebben drie kinderen en zes kleinkinderen.|Ze hebben drie kinderen en zes kleinkinderen.",
         "roots": [
             "to have",
             "3",
             "child",
             "6",
             "grandchild"
         ]
@@ -574,18 +641,18 @@
             "A1": [
                 "EP",
                 "KK",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Wives",
-            "fi": "Vaimot",
-            "nl": "De echtgenotes"
+            "en": "wives",
+            "fi": "vaimot",
+            "nl": "de echtgenotes"
         },
         "singular": {
-            "en": "Wife",
-            "fi": "Vaimo",
-            "nl": "De echtgenote"
+            "en": "wife",
+            "fi": "vaimo",
+            "nl": "de echtgenote"
         }
     }
 }
```

### Comparing `Toisto-0.8.2/src/topics/furniture.json` & `Toisto-0.9.0/src/topics/languages.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Differences: {'replace': "OrderedDict([('language', OrderedDict([('level', OrderedDict([('A1', ['EP', 'KK', "*

 * *            "'OD'])])), ('singular', OrderedDict([('en', 'language'), ('fi', 'kieli'), ('nl', 'de "*

 * *            "taal')])), ('plural', OrderedDict([('en', 'languages'), ('fi', 'kielet'), ('nl', 'de "*

 * *            "talen')]))])), ('dialect', OrderedDict([('level', OrderedDict([('C1', 'OD'), ('C2', "*

 * *            "'EP')])), ('singular', OrderedDict([('en', 'dialect'), ('fi', 'murre'), ('nl', 'het "*

 * *            "dial […]*

```diff
@@ -1,190 +1,236 @@
 {
-    "bed": {
+    "I have a dutch accent": {
+        "en": "I have a Dutch accent.",
+        "fi": "Minulla on hollantilainen aksentti.",
+        "nl": "Ik heb een Nederlands accent.",
+        "roots": [
+            "to have",
+            "dutch",
+            "accent"
+        ]
+    },
+    "accent": {
         "level": {
-            "A1": [
-                "EP",
-                "OD"
-            ]
+            "C1": "OD",
+            "C2": "EP"
         },
         "plural": {
-            "en": "Beds",
-            "fi": "S\u00e4ngyt",
-            "nl": "De bedden"
+            "en": "accents",
+            "fi": "aksentit",
+            "nl": "de accenten"
         },
         "singular": {
-            "en": "Bed",
-            "fi": "S\u00e4nky",
-            "nl": "Het bed"
+            "en": "accent",
+            "fi": "aksentti",
+            "nl": "het accent"
         }
     },
-    "carpet": {
+    "chinese": {
+        "en": "Chinese",
+        "fi": "kiina",
         "level": {
-            "A2": [
+            "none": [
                 "EP",
                 "OD"
             ]
         },
-        "plural": {
-            "en": "Carpets",
-            "fi": "Matot",
-            "nl": "De tapijten"
-        },
-        "singular": {
-            "en": "Carpet",
-            "fi": "Matto",
-            "nl": "Het tapijt"
-        }
+        "nl": "Chinees"
     },
-    "chair": {
+    "danish": {
+        "en": "Danish",
+        "fi": "tanska",
         "level": {
-            "A1": [
+            "none": [
                 "EP",
                 "OD"
             ]
         },
+        "nl": "Deens"
+    },
+    "dialect": {
+        "level": {
+            "C1": "OD",
+            "C2": "EP"
+        },
         "plural": {
-            "en": "Chairs",
-            "fi": "Tuolit",
-            "nl": "De stoelen"
+            "en": "dialects",
+            "fi": "murteet",
+            "nl": "de dialecten"
         },
         "singular": {
-            "en": "Chair",
-            "fi": "Tuoli",
-            "nl": "De stoel"
+            "en": "dialect",
+            "fi": "murre",
+            "nl": "het dialect"
         }
     },
-    "curtain": {
+    "dutch": {
+        "en": "Dutch",
+        "fi": "hollanti",
         "level": {
-            "A2": "EP",
-            "B1": "OD"
+            "none": [
+                "EP",
+                "OD"
+            ]
         },
-        "plural": {
-            "en": "Curtains",
-            "fi": "Verhot",
-            "nl": "De gordijnen"
+        "nl": "Nederlands"
+    },
+    "english": {
+        "en": "English",
+        "fi": "englanti",
+        "level": {
+            "A1": "OD",
+            "C1": "EP"
         },
-        "singular": {
-            "en": "Curtain",
-            "fi": "Verho",
-            "nl": "Het gordijn"
-        }
+        "nl": "Engels"
     },
-    "desk": {
+    "estonian": {
+        "en": "Estonian",
+        "fi": "viro",
         "level": {
-            "A1": [
+            "none": [
                 "EP",
                 "OD"
             ]
         },
-        "plural": {
-            "en": "Desks",
-            "fi": [
-                "Ty\u00f6p\u00f6yd\u00e4t",
-                "Kirjoitusp\u00f6yd\u00e4t"
-            ],
-            "nl": "De bureaus"
-        },
-        "roots": {
-            "fi": [
-                "to write",
-                "table"
+        "nl": "Estisch"
+    },
+    "finnish": {
+        "en": "Finnish",
+        "fi": "suomi",
+        "level": {
+            "A1": "KK",
+            "none": [
+                "EP",
+                "OD"
             ]
         },
-        "singular": {
-            "en": "Desk",
-            "fi": [
-                "Ty\u00f6p\u00f6yt\u00e4",
-                "Kirjoitusp\u00f6yt\u00e4"
-            ],
-            "nl": "Het bureau"
-        }
+        "nl": "Fins"
     },
-    "lamp": {
+    "french": {
+        "en": "French",
+        "fi": "ranska",
         "level": {
-            "A2": [
+            "none": [
                 "EP",
                 "OD"
             ]
         },
-        "plural": {
-            "en": "Lamps",
-            "fi": "Lamput",
-            "nl": "De lampen"
+        "nl": "Frans"
+    },
+    "german": {
+        "en": "German",
+        "fi": "saksa",
+        "level": {
+            "none": [
+                "EP",
+                "OD"
+            ]
         },
-        "singular": {
-            "en": "Lamp",
-            "fi": "Lamppu",
-            "nl": "De lamp"
-        }
+        "nl": "Duits"
     },
-    "pillow": {
+    "hungarian": {
+        "en": "Hungarian",
+        "fi": "unkari",
         "level": {
-            "A2": "EP",
-            "none": "OD"
+            "none": [
+                "EP",
+                "OD"
+            ]
         },
-        "plural": {
-            "en": "Pillows",
-            "fi": "Tyynyt",
-            "nl": "De kussens"
+        "nl": "Hongaars"
+    },
+    "icelandic": {
+        "en": "Icelandic",
+        "fi": "islanti",
+        "level": {
+            "none": [
+                "EP",
+                "OD"
+            ]
         },
-        "singular": {
-            "en": "Pillow",
-            "fi": "Tyyny",
-            "nl": "Het kussen"
-        }
+        "nl": "IJslands"
     },
-    "sofa": {
+    "japanese": {
+        "en": "Japanese",
+        "fi": "japani",
         "level": {
-            "A1": "OD",
-            "A2": "EP"
+            "none": [
+                "EP",
+                "OD"
+            ]
         },
-        "plural": {
-            "en": "Sofas",
-            "fi": "Sohvat",
-            "nl": "De sofa's"
+        "nl": "Japans"
+    },
+    "korean": {
+        "en": "Korean",
+        "fi": "korea",
+        "level": {
+            "none": [
+                "EP",
+                "OD"
+            ]
         },
-        "singular": {
-            "en": "Sofa",
-            "fi": "Sohva",
-            "nl": "De sofa"
-        }
+        "nl": "Koreaans"
     },
-    "table": {
+    "language": {
         "level": {
             "A1": [
                 "EP",
                 "KK",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Tables",
-            "fi": "P\u00f6yd\u00e4t",
-            "nl": "De tafels"
+            "en": "languages",
+            "fi": "kielet",
+            "nl": "de talen"
         },
         "singular": {
-            "en": "Table",
-            "fi": "P\u00f6yt\u00e4",
-            "nl": "De tafel"
+            "en": "language",
+            "fi": "kieli",
+            "nl": "de taal"
         }
     },
-    "the cat is sleeping on the carpet": {
-        "en": "The cat is sleeping on the carpet",
-        "fi": "Kissa nukkuu matolla",
-        "nl": "De kat slaapt op het tapijt",
-        "roots": [
-            "cat",
-            "to sleep",
-            "carpet"
-        ]
+    "norwegian": {
+        "en": "Norwegian",
+        "fi": "norja",
+        "level": {
+            "none": [
+                "EP",
+                "OD"
+            ]
+        },
+        "nl": "Noors"
     },
-    "the door is locked": {
-        "en": "The door is locked",
-        "fi": "Ovi on lukossa",
-        "nl": "De deur is op slot",
-        "roots": [
-            "to be",
-            "door"
-        ]
+    "russian": {
+        "en": "Russian",
+        "fi": "ven\u00e4j\u00e4",
+        "level": {
+            "none": [
+                "EP",
+                "OD"
+            ]
+        },
+        "nl": "Russisch"
+    },
+    "spanish": {
+        "en": "Spanish",
+        "fi": "espanja",
+        "level": {
+            "A1": "EP",
+            "none": "OD"
+        },
+        "nl": "Spaans"
+    },
+    "swedish": {
+        "en": "Swedish",
+        "fi": "ruotsi",
+        "level": {
+            "none": [
+                "EP",
+                "OD"
+            ]
+        },
+        "nl": "Zweeds"
     }
 }
```

### Comparing `Toisto-0.8.2/src/topics/greetings.json` & `Toisto-0.9.0/src/topics/greetings.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.878921568627451%*

 * *Differences: {"'I am alice'": '{\'en\': "I am Alice.|I\'m Alice.", \'fi\': \'Minä olen Alice.\', \'nl\': \'Ik '*

 * *                 "ben Alice.'}",*

 * * "'bye'": "{'en': ['Bye!', 'Bye bye!'], 'fi': ['Hei hei!', 'Moi moi!'], 'nl': ['Doei!', 'Dag!', "*

 * *          "'Tot ziens!']}",*

 * * "'good afternoon'": "{'en': 'Good afternoon!', 'fi': ['Hyvää päivää!;afternoon', "*

 * *                     "'Päivää!;afternoon']}",*

 * * "'good day'": "{'en': 'Good day!', 'fi': ['Hyvää päivää!', 'Päivää!'], 'nl': 'Goedendag!'}",*

 * * "'good evening'": "{'en': 'Go […]*

```diff
@@ -1,41 +1,41 @@
 {
     "I am alice": {
-        "en": "I am Alice|I'm Alice",
-        "fi": "Min\u00e4 olen Alice",
-        "nl": "Ik ben Alice",
+        "en": "I am Alice.|I'm Alice.",
+        "fi": "Min\u00e4 olen Alice.",
+        "nl": "Ik ben Alice.",
         "roots": "to be"
     },
     "bye": {
         "en": [
-            "Bye",
-            "Bye bye"
+            "Bye!",
+            "Bye bye!"
         ],
         "fi": [
-            "Hei hei",
-            "Moi moi"
+            "Hei hei!",
+            "Moi moi!"
         ],
         "level": {
             "A1": [
                 "EP",
                 "KK",
                 "OD"
             ]
         },
         "nl": [
-            "Doei",
-            "Dag",
-            "Tot ziens"
+            "Doei!",
+            "Dag!",
+            "Tot ziens!"
         ]
     },
     "good afternoon": {
-        "en": "Good afternoon",
+        "en": "Good afternoon!",
         "fi": [
-            "Hyv\u00e4\u00e4 p\u00e4iv\u00e4\u00e4;afternoon",
-            "P\u00e4iv\u00e4\u00e4;afternoon"
+            "Hyv\u00e4\u00e4 p\u00e4iv\u00e4\u00e4!;afternoon",
+            "P\u00e4iv\u00e4\u00e4!;afternoon"
         ],
         "level": {
             "A1": "EP",
             "none": "OD"
         },
         "nl": "Goedemiddag",
         "roots": {
@@ -50,102 +50,102 @@
             "nl": [
                 "good",
                 "afternoon"
             ]
         }
     },
     "good day": {
-        "en": "Good day",
+        "en": "Good day!",
         "fi": [
-            "Hyv\u00e4\u00e4 p\u00e4iv\u00e4\u00e4",
-            "P\u00e4iv\u00e4\u00e4"
+            "Hyv\u00e4\u00e4 p\u00e4iv\u00e4\u00e4!",
+            "P\u00e4iv\u00e4\u00e4!"
         ],
         "level": {
             "none": [
                 "EP",
                 "OD"
             ]
         },
-        "nl": "Goedendag",
+        "nl": "Goedendag!",
         "roots": [
             "good",
             "day"
         ]
     },
     "good evening": {
-        "en": "Good evening",
+        "en": "Good evening!",
         "fi": [
-            "Hyv\u00e4\u00e4 iltaa",
-            "Iltaa"
+            "Hyv\u00e4\u00e4 iltaa!",
+            "Iltaa!"
         ],
         "level": {
             "A1": "EP",
             "none": "OD"
         },
-        "nl": "Goedenavond",
+        "nl": "Goedenavond!",
         "roots": [
             "good",
             "evening"
         ]
     },
     "good morning": {
-        "en": "Good morning",
+        "en": "Good morning!",
         "fi": [
-            "Hyv\u00e4\u00e4 huomenta",
-            "Huomenta"
+            "Hyv\u00e4\u00e4 huomenta!",
+            "Huomenta!"
         ],
         "level": {
             "A1": "EP",
             "none": "OD"
         },
-        "nl": "Goedemorgen",
+        "nl": "Goedemorgen!",
         "roots": [
             "good",
             "morning"
         ]
     },
     "good night": {
-        "en": "Good night",
-        "fi": "Hyv\u00e4\u00e4 y\u00f6t\u00e4",
+        "en": "Good night!",
+        "fi": "Hyv\u00e4\u00e4 y\u00f6t\u00e4!",
         "level": {
             "A1": "EP",
             "none": "OD"
         },
-        "nl": "Goedenacht",
+        "nl": "Goedenacht!",
         "roots": [
             "good",
             "night"
         ]
     },
     "hello": {
-        "en": "Hello",
-        "fi": "Terve",
+        "en": "Hello!",
+        "fi": "Terve!",
         "level": {
             "A1": [
                 "EP",
                 "KK",
                 "OD"
             ]
         },
-        "nl": "Hallo"
+        "nl": "Hallo!"
     },
     "hi": {
-        "en": "Hi",
+        "en": "Hi!",
         "fi": [
-            "Hei",
-            "Moi"
+            "Hei!",
+            "Moi!"
         ],
         "level": {
             "A1": [
                 "EP",
                 "KK",
                 "OD"
             ]
         },
-        "nl": "Hoi"
+        "nl": "Hoi!"
     },
     "how are you": {
         "en": "How are you?",
         "fi": [
             "Mit\u00e4 kuuluu?",
             "Miten menee?"
         ],
@@ -163,64 +163,64 @@
         "roots": [
             "how",
             "old",
             "to be"
         ]
     },
     "my name is bob": {
-        "en": "My name is Bob",
-        "fi": "Minun nimeni on Bob",
-        "nl": "Mijn naam is Bob",
+        "en": "My name is Bob.",
+        "fi": "Minun nimeni on Bob.",
+        "nl": "Mijn naam is Bob.",
         "roots": [
             "name",
             "to be"
         ]
     },
     "name": {
         "level": {
             "A1": [
                 "EP",
                 "KK",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Names",
-            "fi": "Nimet",
-            "nl": "De namen"
+            "en": "names",
+            "fi": "nimet",
+            "nl": "de namen"
         },
         "singular": {
-            "en": "Name",
-            "fi": "Nimi",
-            "nl": "De naam"
+            "en": "name",
+            "fi": "nimi",
+            "nl": "de naam"
         }
     },
     "sleep well": {
-        "en": "Sleep well",
-        "fi": "Nuku hyvin",
+        "en": "Sleep well!",
+        "fi": "Nuku hyvin!",
         "level": {
             "none": [
                 "EP",
                 "OD"
             ]
         },
         "nl": [
-            "Slaap lekker",
-            "Welterusten"
+            "Slaap lekker!",
+            "Welterusten!"
         ],
         "roots": "to sleep"
     },
     "welcome": {
-        "en": "Welcome",
-        "fi": "Tervetuloa",
+        "en": "Welcome!",
+        "fi": "Tervetuloa!",
         "level": {
             "A1": "OD",
             "A2": "EP"
         },
-        "nl": "Welkom"
+        "nl": "Welkom!"
     },
     "what is your name": {
         "en": "What is your name?",
         "fi": "Mik\u00e4 sinun nimesi on?",
         "nl": "Wat is jouw naam?|Wat is je naam?",
         "roots": [
             "what",
```

### Comparing `Toisto-0.8.2/src/topics/health.json` & `Toisto-0.9.0/src/topics/health.json`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8971153846153845%*

 * *Differences: {"'ache'": "{'singular': {'en': 'ache', 'fi': 'särky', 'nl': 'de pijn;dull'}, 'plural': {'en': "*

 * *           "'aches', 'fi': 'säryt', 'nl': 'de pijnen;dull'}}",*

 * * "'blood'": "{'singular': {'en': 'blood', 'fi': 'veri', 'nl': 'het bloed'}, 'plural': {'en': "*

 * *            "'bloods', 'fi': 'veret'}}",*

 * * "'care'": "{'en': 'care', 'fi': 'hoito', 'nl': 'de zorg'}",*

 * * "'disease'": "{'singular': {'en': 'disease', 'fi': 'sairaus', 'nl': 'de ziekte'}, 'plural': "*

 * *              "{'en': 'diseases', 'fi': 'sairaudet', 'nl': ' […]*

```diff
@@ -1,206 +1,206 @@
 {
     "ache": {
         "level": {
             "A2": "OD",
             "B1": "EP"
         },
         "plural": {
-            "en": "Aches",
-            "fi": "S\u00e4ryt",
-            "nl": "De pijnen;dull"
+            "en": "aches",
+            "fi": "s\u00e4ryt",
+            "nl": "de pijnen;dull"
         },
         "singular": {
-            "en": "Ache",
-            "fi": "S\u00e4rky",
-            "nl": "De pijn;dull"
+            "en": "ache",
+            "fi": "s\u00e4rky",
+            "nl": "de pijn;dull"
         }
     },
     "blood": {
         "level": {
             "A2": [
                 "EP",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Bloods",
-            "fi": "Veret"
+            "en": "bloods",
+            "fi": "veret"
         },
         "singular": {
-            "en": "Blood",
-            "fi": "Veri",
-            "nl": "Het bloed"
+            "en": "blood",
+            "fi": "veri",
+            "nl": "het bloed"
         }
     },
     "care": {
-        "en": "Care",
-        "fi": "Hoito",
+        "en": "care",
+        "fi": "hoito",
         "level": {
             "A2": "OD",
             "B2": "EP"
         },
-        "nl": "De zorg"
+        "nl": "de zorg"
     },
     "disease": {
         "level": {
             "A2": "OD",
             "B1": "EP"
         },
         "plural": {
-            "en": "Diseases",
-            "fi": "Sairaudet",
-            "nl": "De ziektes;De ziekten"
+            "en": "diseases",
+            "fi": "sairaudet",
+            "nl": "de ziektes|de ziekten"
         },
         "singular": {
-            "en": "Disease",
-            "fi": "Sairaus",
-            "nl": "De ziekte"
+            "en": "disease",
+            "fi": "sairaus",
+            "nl": "de ziekte"
         }
     },
     "fever": {
         "level": {
             "B1": "EP",
             "B2": "OD"
         },
         "plural": {
-            "en": "Fevers",
-            "fi": "Kuumeet",
-            "nl": "Koortsen"
+            "en": "fevers",
+            "fi": "kuumeet",
+            "nl": "koortsen"
         },
         "singular": {
-            "en": "Fever",
-            "fi": "Kuume",
-            "nl": "De koorts"
+            "en": "fever",
+            "fi": "kuume",
+            "nl": "de koorts"
         }
     },
     "flu": {
         "level": {
             "A2": "OD",
             "B1": "EP"
         },
         "plural": {
-            "en": "Flus",
-            "fi": "Flunssat",
-            "nl": "De griepen"
+            "en": "flus",
+            "fi": "flunssat",
+            "nl": "de griepen"
         },
         "singular": {
-            "en": "Flu",
-            "fi": "Flunssa",
-            "nl": "De griep"
+            "en": "flu",
+            "fi": "flunssa",
+            "nl": "de griep"
         }
     },
     "headache": {
         "level": {
             "A2": [
                 "EP",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Headaches",
-            "fi": "P\u00e4\u00e4ns\u00e4ryt",
-            "nl": "De hoofdpijnen"
+            "en": "headaches",
+            "fi": "p\u00e4\u00e4ns\u00e4ryt",
+            "nl": "de hoofdpijnen"
         },
         "roots": [
             "head",
             "ache"
         ],
         "singular": {
-            "en": "Headache",
-            "fi": "P\u00e4\u00e4ns\u00e4rky",
-            "nl": "De hoofdpijn"
+            "en": "headache",
+            "fi": "p\u00e4\u00e4ns\u00e4rky",
+            "nl": "de hoofdpijn"
         }
     },
     "health": {
-        "en": "Health",
-        "fi": "Terveys",
+        "en": "health",
+        "fi": "terveys",
         "level": {
             "A1": "OD",
             "A2": "EP"
         },
-        "nl": "De gezondheid"
+        "nl": "de gezondheid"
     },
     "health care": {
-        "en": "Health care",
-        "fi": "Terveydenhoito",
+        "en": "health care",
+        "fi": "terveydenhoito",
         "level": {
             "B2": "OD",
             "C1": "EP"
         },
-        "nl": "De gezondheidszorg",
+        "nl": "de gezondheidszorg",
         "roots": [
             "health",
             "care"
         ]
     },
     "medicine": {
         "level": {
             "A2": [
                 "EP",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Medicines",
-            "fi": "L\u00e4\u00e4kkeet",
-            "nl": "De medicijnen"
+            "en": "medicines",
+            "fi": "l\u00e4\u00e4kkeet",
+            "nl": "de medicijnen"
         },
         "singular": {
-            "en": "Medicine",
-            "fi": "L\u00e4\u00e4ke",
-            "nl": "Het medicijn"
+            "en": "medicine",
+            "fi": "l\u00e4\u00e4ke",
+            "nl": "het medicijn"
         }
     },
     "pain": {
         "level": {
             "A2": [
                 "EP",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Pains",
-            "fi": "Kivut",
-            "nl": "De pijnen;sharp"
+            "en": "pains",
+            "fi": "kivut",
+            "nl": "de pijnen;sharp"
         },
         "singular": {
-            "en": "Pain",
-            "fi": "Kipu",
-            "nl": "De pijn;sharp"
+            "en": "pain",
+            "fi": "kipu",
+            "nl": "de pijn;sharp"
         }
     },
     "patient": {
         "level": {
             "A2": "OD",
             "B1": "EP"
         },
         "plural": {
-            "en": "Patients",
-            "fi": "Potilaat",
-            "nl": "De pati\u00ebnten"
+            "en": "patients",
+            "fi": "potilaat",
+            "nl": "de pati\u00ebnten"
         },
         "singular": {
-            "en": "Patient",
-            "fi": "Potilas",
-            "nl": "De pati\u00ebnt"
+            "en": "patient",
+            "fi": "potilas",
+            "nl": "de pati\u00ebnt"
         }
     },
     "wound": {
         "level": {
             "B2": [
                 "EP",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Wounds",
-            "fi": "Haavat",
-            "nl": "De wonden"
+            "en": "wounds",
+            "fi": "haavat",
+            "nl": "de wonden"
         },
         "singular": {
-            "en": "Wound",
-            "fi": "Haava",
-            "nl": "De wond"
+            "en": "wound",
+            "fi": "haava",
+            "nl": "de wond"
         }
     }
 }
```

### Comparing `Toisto-0.8.2/src/topics/holidays.json` & `Toisto-0.9.0/src/topics/holidays.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9108082706766918%*

 * *Differences: {"'angel'": "{'en': 'angel', 'fi': 'enkeli', 'nl': 'de engel'}",*

 * * "'bauble'": "{'en': 'bauble', 'fi': 'joulukuusenpallo|joulupallo', 'nl': 'de kerstbal'}",*

 * * "'boxing day'": "{'nl': 'tweede kerstdag'}",*

 * * "'christmas day'": "{'nl': 'eerste kerstdag'}",*

 * * "'christmas eve'": "{'nl': 'kerstavond'}",*

 * * "'christmas tree'": "{'fi': 'joulukuusi', 'nl': 'de kerstboom'}",*

 * * "'elf'": "{'en': 'elf', 'fi': 'tonttu', 'nl': 'de elf'}",*

 * * "'finnish independence day'": "{'en': '(Finnish independence day, December 6th)', 'nl': '( […]*

```diff
@@ -1,23 +1,23 @@
 {
     "angel": {
-        "en": "Angel",
-        "fi": "Enkeli",
-        "nl": "De engel"
+        "en": "angel",
+        "fi": "enkeli",
+        "nl": "de engel"
     },
     "bauble": {
-        "en": "Bauble",
-        "fi": "Joulukuusenpallo|Joulupallo",
+        "en": "bauble",
+        "fi": "joulukuusenpallo|joulupallo",
         "level": {
             "none": [
                 "EP",
                 "OD"
             ]
         },
-        "nl": "De kerstbal",
+        "nl": "de kerstbal",
         "roots": {
             "fi": [
                 "christmas tree",
                 "christmas"
             ],
             "nl": "christmas"
         }
@@ -25,15 +25,15 @@
     "boxing day": {
         "en": "Boxing Day",
         "fi": "Tapaninp\u00e4iv\u00e4",
         "level": {
             "C1": "OD",
             "none": "EP"
         },
-        "nl": "Tweede kerstdag",
+        "nl": "tweede kerstdag",
         "roots": {
             "en": "day",
             "fi": "day",
             "nl": [
                 "christmas",
                 "day"
             ]
@@ -51,47 +51,47 @@
     "christmas day": {
         "en": "Christmas Day",
         "fi": "Joulup\u00e4iv\u00e4",
         "level": {
             "A1": "OD",
             "none": "EP"
         },
-        "nl": "Eerste kerstdag",
+        "nl": "eerste kerstdag",
         "roots": [
             "christmas",
             "day"
         ]
     },
     "christmas eve": {
         "en": "Christmas Eve",
         "fi": "Jouluaatto",
         "level": {
             "C1": "OD",
             "none": "EP"
         },
-        "nl": "Kerstavond",
+        "nl": "kerstavond",
         "roots": {
             "en": "christmas",
             "fi": "christmas",
             "nl": [
                 "christmas",
                 "evening"
             ]
         }
     },
     "christmas tree": {
         "en": "Christmas tree",
-        "fi": "Joulukuusi",
+        "fi": "joulukuusi",
         "level": {
             "none": [
                 "EP",
                 "OD"
             ]
         },
-        "nl": "De kerstboom",
+        "nl": "de kerstboom",
         "roots": [
             "christmas",
             "tree"
         ]
     },
     "easter": {
         "en": "Easter",
@@ -99,41 +99,43 @@
         "level": {
             "B1": "OD",
             "none": "EP"
         },
         "nl": "Pasen"
     },
     "elf": {
-        "en": "Elf",
-        "fi": "Tonttu",
+        "en": "elf",
+        "fi": "tonttu",
         "level": {
             "none": [
                 "EP",
                 "OD"
             ]
         },
-        "nl": "De elf"
+        "nl": "de elf"
     },
     "epiphany": {
         "en": "Epiphany",
         "fi": "Loppiainen",
         "level": {
             "C2": "OD",
             "none": "EP"
         },
         "nl": "Driekoningen"
     },
     "finnish independence day": {
+        "en": "(Finnish independence day, December 6th)",
         "fi": "Itsen\u00e4isyysp\u00e4iv\u00e4",
         "level": {
             "none": [
                 "EP",
                 "OD"
             ]
         },
+        "nl": "(Finse onafhankelijkheidsdag, 6 december)",
         "roots": "day"
     },
     "first of may": {
         "en": "First of May",
         "fi": "Vappu",
         "level": {
             "none": [
@@ -152,15 +154,15 @@
         "fi": "Hyv\u00e4\u00e4 uutta vuotta!",
         "level": {
             "none": [
                 "EP",
                 "OD"
             ]
         },
-        "nl": "Gelukkig nieuwjaar",
+        "nl": "Gelukkig nieuwjaar!",
         "roots": {
             "en": [
                 "happy",
                 "new year"
             ],
             "fi": [
                 "good",
@@ -170,31 +172,24 @@
             "nl": [
                 "happy",
                 "new year"
             ]
         }
     },
     "holiday": {
+        "en": "holiday",
+        "fi": "juhlap\u00e4iv\u00e4",
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
-        "plural": {
-            "en": "Holidays",
-            "fi": "Juhlap\u00e4iv\u00e4t",
-            "nl": "De feestdagen"
-        },
-        "roots": "day",
-        "singular": {
-            "en": "Holiday",
-            "fi": "Juhlap\u00e4iv\u00e4",
-            "nl": "De feestdag"
-        }
+        "nl": "de feestdag",
+        "roots": "day"
     },
     "merry christmas": {
         "en": "Merry Christmas!",
         "fi": "Hyv\u00e4\u00e4 joulua!",
         "level": {
             "none": [
                 "EP",
@@ -208,21 +203,21 @@
                 "good",
                 "christmas"
             ],
             "nl": "christmas"
         }
     },
     "midsummer": {
-        "en": "Midsummer",
-        "fi": "Juhannus",
+        "en": "midsummer",
+        "fi": "juhannus",
         "level": {
             "C1": "OD",
             "none": "EP"
         },
-        "nl": "Midzomer",
+        "nl": "midzomer",
         "roots": {
             "en": "summer",
             "nl": "summer"
         }
     },
     "new year": {
         "en": "New Year",
@@ -235,22 +230,22 @@
         "roots": [
             "new",
             "year"
         ]
     },
     "santa": {
         "en": "Santa Claus|Santa",
-        "fi": "Joulupukki",
+        "fi": "joulupukki",
         "level": {
             "none": [
                 "EP",
                 "OD"
             ]
         },
-        "nl": "De kerstman",
+        "nl": "de kerstman",
         "roots": {
             "fi": "christmas",
             "nl": "christmas"
         }
     },
     "valentine's day": {
         "en": "Valentine's Day",
```

### Comparing `Toisto-0.8.2/src/topics/house.json` & `Toisto-0.9.0/src/topics/house.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.82010582010582%*

 * *Differences: {"'apartment'": "{'singular': {'en': 'apartment', 'fi': 'asunto', 'nl': 'het appartement'}, "*

 * *                "'plural': {'en': 'apartments', 'fi': 'asunnot', 'nl': 'de appartementen'}}",*

 * * "'barbecue'": "{'singular': {'en': 'barbecue', 'fi': 'grilli', 'nl': 'de barbecue'}, 'plural': "*

 * *               "{'en': 'barbecues', 'fi': 'grillit', 'nl': 'de barbecues'}}",*

 * * "'basement'": "{'singular': {'en': 'basement', 'fi': 'kellari', 'nl': 'de kelder'}, 'plural': "*

 * *               "{'en': 'basements', 'fi': 'kellarit […]*

```diff
@@ -1,338 +1,338 @@
 {
     "apartment": {
         "level": {
             "A1": "OD",
             "A2": "EP"
         },
         "plural": {
-            "en": "Apartments",
-            "fi": "Asunnot",
-            "nl": "De appartementen"
+            "en": "apartments",
+            "fi": "asunnot",
+            "nl": "de appartementen"
         },
         "singular": {
-            "en": "Apartment",
-            "fi": "Asunto",
-            "nl": "Het appartement"
+            "en": "apartment",
+            "fi": "asunto",
+            "nl": "het appartement"
         }
     },
     "barbecue": {
         "level": {
             "A2": "EP",
             "B1": "OD"
         },
         "plural": {
-            "en": "Barbecues",
-            "fi": "Grillit",
-            "nl": "De barbecues"
+            "en": "barbecues",
+            "fi": "grillit",
+            "nl": "de barbecues"
         },
         "singular": {
-            "en": "Barbecue",
-            "fi": "Grilli",
-            "nl": "De barbecue"
+            "en": "barbecue",
+            "fi": "grilli",
+            "nl": "de barbecue"
         }
     },
     "basement": {
         "level": {
             "B2": [
                 "EP",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Basements",
-            "fi": "Kellarit",
-            "nl": "De kelders"
+            "en": "basements",
+            "fi": "kellarit",
+            "nl": "de kelders"
         },
         "singular": {
-            "en": "Basement",
-            "fi": "Kellari",
-            "nl": "De kelder"
+            "en": "basement",
+            "fi": "kellari",
+            "nl": "de kelder"
         }
     },
     "bathroom": {
+        "en": "bathroom",
+        "fi": "kylpyhuone",
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
-        "plural": {
-            "en": "Bathrooms",
-            "fi": "Kylpyhuoneet",
-            "nl": "De badkamers"
-        },
-        "roots": "room",
-        "singular": {
-            "en": "Bathroom",
-            "fi": "Kylpyhuone",
-            "nl": "De badkamer"
-        }
+        "nl": "de badkamer",
+        "roots": "room"
     },
     "bedroom": {
+        "en": "bedroom",
+        "fi": "makuuhuone",
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
-        "plural": {
-            "en": "Bedrooms",
-            "fi": "Makuuhuoneet",
-            "nl": "De slaapkamers"
-        },
+        "nl": "de slaapkamer",
         "roots": {
             "en": [
                 "room",
                 "bed"
             ],
             "fi": "room",
             "nl": [
                 "room",
                 "to sleep"
             ]
+        }
+    },
+    "dining room": {
+        "en": "dining room",
+        "fi": "ruokahuone",
+        "level": {
+            "A1": [
+                "EP",
+                "OD"
+            ]
         },
-        "singular": {
-            "en": "Bedroom",
-            "fi": "Makuuhuone",
-            "nl": "De slaapkamer"
+        "nl": "de eetkamer",
+        "roots": {
+            "en": [
+                "room"
+            ],
+            "fi": [
+                "food",
+                "root"
+            ],
+            "nl": [
+                "to eat",
+                "room"
+            ]
         }
     },
     "door": {
         "level": {
             "A1": [
                 "EP",
                 "KK",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Doors",
-            "fi": "Ovet",
-            "nl": "De deuren"
+            "en": "doors",
+            "fi": "ovet",
+            "nl": "de deuren"
         },
         "singular": {
-            "en": "Door",
-            "fi": "Ovi",
-            "nl": "De deur"
+            "en": "door",
+            "fi": "ovi",
+            "nl": "de deur"
         }
     },
     "floor": {
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Floors",
-            "fi": "Lattiat",
-            "nl": "De vloeren"
+            "en": "floors",
+            "fi": "lattiat",
+            "nl": "de vloeren"
         },
         "singular": {
-            "en": "Floor",
-            "fi": "Lattia",
-            "nl": "De vloer"
+            "en": "floor",
+            "fi": "lattia",
+            "nl": "de vloer"
         }
     },
     "garden": {
         "level": {
             "A1": [
                 "EP",
                 "KK",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Gardens",
-            "fi": "Pihat",
-            "nl": "De tuinen"
+            "en": "gardens",
+            "fi": "pihat",
+            "nl": "de tuinen"
         },
         "singular": {
-            "en": "Garden",
-            "fi": "Piha",
-            "nl": "De tuin"
+            "en": "garden",
+            "fi": "piha",
+            "nl": "de tuin"
         }
     },
     "home": {
         "level": {
             "A1": [
                 "EP",
                 "KK",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Homes",
-            "fi": "Kodit"
+            "en": "homes",
+            "fi": "kodit"
         },
         "singular": {
-            "en": "Home",
-            "fi": "Koti",
-            "nl": "Het thuis"
+            "en": "home",
+            "fi": "koti",
+            "nl": "het thuis"
         }
     },
     "house": {
         "level": {
             "A1": [
                 "EP",
                 "KK",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Houses",
-            "fi": "Talot",
-            "nl": "De huizen"
+            "en": "houses",
+            "fi": "talot",
+            "nl": "de huizen"
         },
         "singular": {
-            "en": "House",
-            "fi": "Talo",
-            "nl": "Het huis"
+            "en": "house",
+            "fi": "talo",
+            "nl": "het huis"
         }
     },
     "kitchen": {
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Kitchens",
-            "fi": "Keitti\u00f6t",
-            "nl": "De keukens"
+            "en": "kitchens",
+            "fi": "keitti\u00f6t",
+            "nl": "de keukens"
         },
         "singular": {
-            "en": "Kitchen",
-            "fi": "Keitti\u00f6",
-            "nl": "De keuken"
+            "en": "kitchen",
+            "fi": "keitti\u00f6",
+            "nl": "de keuken"
         }
     },
     "living room": {
+        "en": "living room",
+        "fi": "olohuone",
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
-        "plural": {
-            "en": "living rooms",
-            "fi": "Olohuoneet",
-            "nl": [
-                "De huiskamers",
-                "De woonkamers"
-            ]
-        },
+        "nl": [
+            "de huiskamer",
+            "de woonkamer"
+        ],
         "roots": {
             "en": [
                 "room",
                 "to live"
             ],
             "fi": "room",
             "nl": [
                 "house",
                 "room",
                 "to live"
             ]
-        },
-        "singular": {
-            "en": "Living room",
-            "fi": "Olohuone",
-            "nl": [
-                "De huiskamer",
-                "De woonkamer"
-            ]
         }
     },
     "room": {
         "level": {
             "A1": [
                 "EP",
                 "KK",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Rooms",
-            "fi": "Huoneet",
-            "nl": "De kamers"
+            "en": "rooms",
+            "fi": "huoneet",
+            "nl": "de kamers"
         },
         "singular": {
-            "en": "Room",
-            "fi": "Huone",
-            "nl": "De kamer"
+            "en": "room",
+            "fi": "huone",
+            "nl": "de kamer"
         }
     },
     "stairs": {
         "level": {
             "A2": [
                 "EP",
                 "OD"
             ]
         },
         "plural": {
-            "nl": "De trappen"
+            "nl": "de trappen"
         },
         "singular": {
-            "en": "Stairs",
+            "en": "stairs",
             "fi": [
-                "Portaat",
-                "Rappuset"
+                "portaat",
+                "rappuset"
             ],
-            "nl": "De trap"
+            "nl": "de trap"
         }
     },
     "veranda": {
         "level": {
             "C2": "OD",
             "none": "EP"
         },
         "plural": {
-            "en": "Verandas",
-            "fi": "Verannat",
-            "nl": "De veranda's"
+            "en": "verandas",
+            "fi": "verannat",
+            "nl": "de veranda's"
         },
         "singular": {
-            "en": "Veranda",
-            "fi": "Veranta",
-            "nl": "De veranda"
+            "en": "veranda",
+            "fi": "veranta",
+            "nl": "de veranda"
         }
     },
     "wall": {
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Walls",
-            "fi": "Sein\u00e4t",
-            "nl": "De muren"
+            "en": "walls",
+            "fi": "sein\u00e4t",
+            "nl": "de muren"
         },
         "singular": {
-            "en": "Wall",
-            "fi": "Sein\u00e4",
-            "nl": "De muur"
+            "en": "wall",
+            "fi": "sein\u00e4",
+            "nl": "de muur"
         }
     },
     "window": {
         "level": {
             "A1": [
                 "EP",
                 "KK",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Windows",
-            "fi": "Ikkunat",
-            "nl": "De ramen"
+            "en": "windows",
+            "fi": "ikkunat",
+            "nl": "de ramen"
         },
         "singular": {
-            "en": "Window",
-            "fi": "Ikkuna",
-            "nl": "Het raam"
+            "en": "window",
+            "fi": "ikkuna",
+            "nl": "het raam"
         }
     }
 }
```

### Comparing `Toisto-0.8.2/src/topics/interrogative_pronouns.json` & `Toisto-0.9.0/src/topics/interrogative_pronouns.json`

 * *Files identical despite different names*

### Comparing `Toisto-0.8.2/src/topics/months.json` & `Toisto-0.9.0/src/topics/months.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8877450980392159%*

 * *Differences: {"'april'": "{'fi': 'huhtikuu', 'nl': 'april'}",*

 * * "'august'": "{'fi': 'elokuu', 'nl': 'augustus'}",*

 * * "'december'": "{'fi': 'joulukuu', 'nl': 'december'}",*

 * * "'february'": "{'fi': 'helmikuu', 'nl': 'februari'}",*

 * * "'in april'": "{'en': 'In April.', 'fi': 'Huhtikuussa.', 'nl': 'In april.'}",*

 * * "'in january'": "{'en': 'In January.', 'fi': 'Tammikuussa.', 'nl': 'In januari.'}",*

 * * "'it is july'": '{\'en\': "It is July.|It\'s July.", \'fi\': [\'Nyt on heinäkuu.\', \'On '*

 * *                 "heinäkuu.'], 'nl': 'Het is j […]*

```diff
@@ -1,243 +1,243 @@
 {
     "april": {
         "en": "April",
-        "fi": "Huhtikuu",
+        "fi": "huhtikuu",
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
-        "nl": "April",
+        "nl": "april",
         "roots": {
             "fi": "moon"
         }
     },
     "august": {
         "en": "August",
-        "fi": "Elokuu",
+        "fi": "elokuu",
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
-        "nl": "Augustus",
+        "nl": "augustus",
         "roots": {
             "fi": "moon"
         }
     },
     "december": {
         "en": "December",
-        "fi": "Joulukuu",
+        "fi": "joulukuu",
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
-        "nl": "December",
+        "nl": "december",
         "roots": {
             "fi": [
                 "christmas",
                 "moon"
             ]
         }
     },
     "february": {
         "en": "February",
-        "fi": "Helmikuu",
+        "fi": "helmikuu",
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
-        "nl": "Februari",
+        "nl": "februari",
         "roots": {
             "fi": "moon"
         }
     },
     "in april": {
-        "en": "In April",
-        "fi": "Huhtikuussa",
-        "nl": "In april",
+        "en": "In April.",
+        "fi": "Huhtikuussa.",
+        "nl": "In april.",
         "roots": "april"
     },
     "in january": {
-        "en": "In January",
-        "fi": "Tammikuussa",
-        "nl": "In januari",
+        "en": "In January.",
+        "fi": "Tammikuussa.",
+        "nl": "In januari.",
         "roots": "january"
     },
     "it is july": {
-        "en": "It is July|It's July",
+        "en": "It is July.|It's July.",
         "fi": [
-            "Nyt on hein\u00e4kuu",
-            "On hein\u00e4kuu"
+            "Nyt on hein\u00e4kuu.",
+            "On hein\u00e4kuu."
         ],
-        "nl": "Het is juli",
+        "nl": "Het is juli.",
         "roots": [
             "july",
             "to be",
             "now"
         ]
     },
     "january": {
         "en": "January",
-        "fi": "Tammikuu",
+        "fi": "tammikuu",
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
-        "nl": "Januari",
+        "nl": "januari",
         "roots": {
             "fi": "moon"
         }
     },
     "july": {
         "en": "July",
-        "fi": "Hein\u00e4kuu",
+        "fi": "hein\u00e4kuu",
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
-        "nl": "Juli",
+        "nl": "juli",
         "roots": {
             "fi": "moon"
         }
     },
     "june": {
         "en": "June",
-        "fi": "Kes\u00e4kuu",
+        "fi": "kes\u00e4kuu",
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
-        "nl": "Juni",
+        "nl": "juni",
         "roots": {
             "fi": [
                 "summer",
                 "moon"
             ]
         }
     },
     "march": {
         "en": "March",
-        "fi": "Maaliskuu",
+        "fi": "maaliskuu",
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
-        "nl": "Maart",
+        "nl": "maart",
         "roots": {
             "fi": "moon"
         }
     },
     "may": {
         "en": "May",
-        "fi": "Toukokuu",
+        "fi": "toukokuu",
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
-        "nl": "Mei",
+        "nl": "mei",
         "roots": {
             "fi": "moon"
         }
     },
     "month": {
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Months",
-            "fi": "Kuukaudet",
-            "nl": "De maanden"
+            "en": "months",
+            "fi": "kuukaudet",
+            "nl": "de maanden"
         },
         "roots": {
             "fi": "moon",
             "nl": "moon"
         },
         "singular": {
-            "en": "Month",
-            "fi": "Kuukausi",
-            "nl": "De maand"
+            "en": "month",
+            "fi": "kuukausi",
+            "nl": "de maand"
         }
     },
     "moon": {
         "level": {
             "A2": [
                 "EP",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Moons",
-            "fi": "Kuut",
-            "nl": "De manen"
+            "en": "moons",
+            "fi": "kuut",
+            "nl": "de manen"
         },
         "singular": {
-            "en": "Moon",
-            "fi": "Kuu",
-            "nl": "De maan"
+            "en": "moon",
+            "fi": "kuu",
+            "nl": "de maan"
         }
     },
     "november": {
         "en": "November",
-        "fi": "Marraskuu",
+        "fi": "marraskuu",
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
-        "nl": "November",
+        "nl": "november",
         "roots": {
             "fi": "moon"
         }
     },
     "october": {
         "en": "October",
-        "fi": "Lokakuu",
+        "fi": "lokakuu",
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
-        "nl": "Oktober",
+        "nl": "oktober",
         "roots": {
             "fi": "moon"
         }
     },
     "september": {
         "en": "September",
-        "fi": "Syyskuu",
+        "fi": "syyskuu",
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
-        "nl": "September",
+        "nl": "september",
         "roots": {
             "fi": [
                 "autumn",
                 "moon"
             ]
         }
     }
```

### Comparing `Toisto-0.8.2/src/topics/nature.json` & `Toisto-0.9.0/src/topics/city.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Differences: {'replace': "OrderedDict([('city', OrderedDict([('level', OrderedDict([('A1', ['EP', 'KK', "*

 * *            "'OD'])])), ('singular', OrderedDict([('en', 'city'), ('fi', 'kaupunki'), ('nl', 'de "*

 * *            "stad')])), ('plural', OrderedDict([('en', 'cities'), ('fi', 'kaupungit'), ('nl', 'de "*

 * *            "steden')]))])), ('building', OrderedDict([('level', OrderedDict([('A1', ['KK', "*

 * *            "'OD']), ('A2', 'EP')])), ('singular', OrderedDict([('en', 'building'), ('fi', "*

 * *            "'rakennus'), ('nl',  […]*

```diff
@@ -1,392 +1,503 @@
 {
-    "beach": {
+    "I am in the office": {
+        "en": "I am in the office.|I'm in the office.",
+        "fi": "Min\u00e4 olen toimistolla.|Olen toimistolla.",
+        "nl": "Ik ben op kantoor.",
+        "roots": [
+            "to be",
+            "office"
+        ]
+    },
+    "airport": {
         "level": {
-            "A1": [
+            "A1": "OD",
+            "A2": "EP"
+        },
+        "plural": {
+            "en": "airports",
+            "fi": "lentokent\u00e4t",
+            "nl": "de vliegvelden"
+        },
+        "roots": {
+            "en": "port"
+        },
+        "singular": {
+            "en": "airport",
+            "fi": "lentokentt\u00e4",
+            "nl": "het vliegveld"
+        }
+    },
+    "bridge": {
+        "level": {
+            "A2": [
                 "EP",
-                "KK",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Beaches",
-            "fi": "Rannat",
-            "nl": "De stranden"
+            "en": "bridges",
+            "fi": "sillat",
+            "nl": "de bruggen"
         },
         "singular": {
-            "en": "Beach",
-            "fi": "Ranta",
-            "nl": "Het strand"
+            "en": "bridge",
+            "fi": "silta",
+            "nl": "de brug"
         }
     },
-    "coast": {
+    "building": {
         "level": {
-            "A2": "OD",
-            "B1": "EP"
+            "A1": [
+                "KK",
+                "OD"
+            ],
+            "A2": "EP"
         },
         "plural": {
-            "en": "Coasts",
-            "fi": "Rannikot",
-            "nl": "De kusten"
-        },
-        "roots": {
-            "fi": "beach"
+            "en": "buildings",
+            "fi": "rakennukset",
+            "nl": "de gebouwen"
         },
         "singular": {
-            "en": "Coast",
-            "fi": "Rannikko",
-            "nl": "De kust"
+            "en": "building",
+            "fi": "rakennus",
+            "nl": "het gebouw"
         }
     },
-    "continent": {
+    "capital": {
         "level": {
-            "A2": "OD",
-            "B1": "EP"
+            "A1": "OD",
+            "A2": "EP"
         },
         "plural": {
-            "en": "Continents",
-            "fi": "Maanosat",
-            "nl": "De continenten"
+            "en": "capitals",
+            "fi": "p\u00e4\u00e4kaupungit",
+            "nl": "de hoofdsteden"
         },
         "roots": {
-            "fi": "country"
+            "fi": [
+                "city",
+                "head"
+            ],
+            "nl": [
+                "city",
+                "head"
+            ]
         },
         "singular": {
-            "en": "Continent",
-            "fi": "Maanosa",
-            "nl": "Het continent"
+            "en": "capital",
+            "fi": "p\u00e4\u00e4kaupunki",
+            "nl": "de hoofdstad"
         }
     },
-    "desert": {
+    "castle": {
         "level": {
             "A2": [
                 "EP",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Deserts",
-            "fi": [
-                "Aavikot",
-                "Autiomaat"
+            "en": "castles",
+            "fi": "linnat",
+            "nl": "de kastelen"
+        },
+        "singular": {
+            "en": "castle",
+            "fi": "linna",
+            "nl": "het kasteel"
+        }
+    },
+    "centre": {
+        "level": {
+            "A1": [
+                "KK",
+                "OD"
             ],
-            "nl": "De woestijnen"
+            "A2": "EP"
         },
-        "roots": {
-            "fi": "country"
+        "plural": {
+            "en": "centres",
+            "fi": "keskustat",
+            "nl": "de centra"
         },
         "singular": {
-            "en": "Desert",
-            "fi": [
-                "Aavikko",
-                "Autiomaa"
-            ],
-            "nl": "De woestijn"
+            "en": "centre",
+            "fi": "keskusta",
+            "nl": "het centrum"
         }
     },
-    "east": {
-        "en": "East|The east",
-        "fi": "It\u00e4",
+    "church": {
         "level": {
-            "A1": "OD",
-            "A2": "EP"
+            "A1": "KK",
+            "A2": [
+                "EP",
+                "OD"
+            ]
         },
-        "nl": "Het oosten"
+        "plural": {
+            "en": "churches",
+            "fi": "kirkot",
+            "nl": "de kerken"
+        },
+        "singular": {
+            "en": "church",
+            "fi": "kirkko",
+            "nl": "de kerk"
+        }
     },
-    "flower": {
+    "city": {
         "level": {
             "A1": [
                 "EP",
+                "KK",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Flowers",
-            "fi": "Kukat",
-            "nl": "De bloemen"
+            "en": "cities",
+            "fi": "kaupungit",
+            "nl": "de steden"
         },
         "singular": {
-            "en": "Flower",
-            "fi": "Kukka",
-            "nl": "De bloem"
+            "en": "city",
+            "fi": "kaupunki",
+            "nl": "de stad"
         }
     },
-    "forest": {
+    "department store": {
         "level": {
-            "A1": "KK",
-            "A2": [
+            "A2": "EP",
+            "B1": "OD"
+        },
+        "plural": {
+            "en": "department stores",
+            "fi": "tavaratalot",
+            "nl": "de warenhuizen"
+        },
+        "roots": {
+            "en": "store",
+            "fi": "house",
+            "nl": "house"
+        },
+        "singular": {
+            "en": "department store",
+            "fi": "tavaratalo",
+            "nl": "het warenhuis"
+        }
+    },
+    "hospital": {
+        "level": {
+            "A1": [
                 "EP",
+                "KK",
                 "OD"
             ]
         },
         "plural": {
-            "en": [
-                "Forests",
-                "Woods"
-            ],
-            "fi": "Mets\u00e4t",
-            "nl": "De bossen"
+            "en": "hospitals",
+            "fi": "sairaalat",
+            "nl": "de ziekenhuizen"
+        },
+        "roots": {
+            "nl": "house"
         },
         "singular": {
-            "en": [
-                "Forest",
-                "Wood"
-            ],
-            "fi": "Mets\u00e4",
-            "nl": "Het bos"
+            "en": "hospital",
+            "fi": "sairaala",
+            "nl": "het ziekenhuis"
         }
     },
-    "hill": {
+    "hotel": {
         "level": {
-            "A2": [
+            "A1": [
                 "EP",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Hills",
-            "fi": [
-                "M\u00e4et",
-                "Kukkulat"
-            ],
-            "nl": "De heuvels"
+            "en": "hotels",
+            "fi": "hotellit",
+            "nl": "de hotels"
         },
         "singular": {
-            "en": "Hill",
-            "fi": [
-                "M\u00e4ki",
-                "Kukkula"
-            ],
-            "nl": "De heuvel"
+            "en": "hotel",
+            "fi": "hotelli",
+            "nl": "het hotel"
         }
     },
-    "island": {
+    "library": {
         "level": {
             "A1": "OD",
             "A2": "EP"
         },
         "plural": {
-            "en": "Islands",
-            "fi": "Saaret",
-            "nl": "De eilanden"
+            "en": "libraries",
+            "fi": "kirjastot",
+            "nl": "de bibliotheken"
+        },
+        "roots": {
+            "fi": "book"
         },
         "singular": {
-            "en": "Island",
-            "fi": "Saari",
-            "nl": "Het eiland"
+            "en": "library",
+            "fi": "kirjasto",
+            "nl": "de bibliotheek"
         }
     },
-    "it is cold in the north": {
-        "en": "It is cold in the North",
-        "fi": "Pohjoisessa on kylm\u00e4",
-        "nl": "Het is koud in het Noorden",
-        "roots": [
-            "to be",
-            "cold",
-            "north"
-        ]
-    },
-    "it is warm in the south": {
-        "en": "It is warm in the South",
-        "fi": "Etel\u00e4ss\u00e4 on l\u00e4mmin",
-        "nl": "Het is warm in het Zuiden",
-        "roots": [
-            "to be",
-            "warm",
-            "south"
-        ]
-    },
-    "lake": {
+    "mall": {
         "level": {
-            "A2": [
+            "B1": [
                 "EP",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Lakes",
-            "fi": "J\u00e4rvet",
-            "nl": "De meren"
+            "en": [
+                "malls",
+                "shopping centers"
+            ],
+            "fi": [
+                "kauppakeskukset",
+                "ostoskeskukset"
+            ],
+            "nl": "de winkelcentra"
+        },
+        "roots": {
+            "en": "centre",
+            "fi": [
+                "centre",
+                "store"
+            ],
+            "nl": [
+                "centre",
+                "store"
+            ]
         },
         "singular": {
-            "en": "Lake",
-            "fi": "J\u00e4rvi",
-            "nl": "Het meer"
+            "en": [
+                "mall",
+                "shopping center"
+            ],
+            "fi": [
+                "kauppakeskus",
+                "ostoskeskus"
+            ],
+            "nl": "het winkelcentrum"
         }
     },
-    "mountain": {
+    "monument": {
         "level": {
-            "A1": "OD",
-            "A2": "EP"
+            "B1": "EP",
+            "B2": "OD"
         },
         "plural": {
-            "en": "Mountains",
-            "fi": "Vuoret",
-            "nl": "De bergen"
+            "en": "monuments",
+            "fi": "monumentit",
+            "nl": "de monumenten"
         },
         "singular": {
-            "en": "Mountain",
-            "fi": "Vuori",
-            "nl": "De berg"
+            "en": "monument",
+            "fi": "monumentti",
+            "nl": "het monument"
         }
     },
-    "nature": {
-        "en": "Nature",
-        "fi": "Luonto",
+    "museum": {
         "level": {
-            "A1": "KK",
-            "A2": [
+            "A1": [
                 "EP",
                 "OD"
             ]
         },
-        "nl": "De natuur"
+        "plural": {
+            "en": "museums",
+            "fi": "museot",
+            "nl": "de musea"
+        },
+        "singular": {
+            "en": "museum",
+            "fi": "museo",
+            "nl": "het museum"
+        }
+    },
+    "my house is in this street": {
+        "en": "My house is in this street.",
+        "fi": "Minun taloni on t\u00e4ll\u00e4 kadulla.|Taloni on t\u00e4ll\u00e4 kadulla.",
+        "nl": "Mijn huis is in deze straat.",
+        "roots": [
+            "to be",
+            "house",
+            "street"
+        ]
     },
-    "north": {
-        "en": "North|The north",
-        "fi": "Pohjoinen",
+    "office": {
         "level": {
             "A1": "OD",
             "A2": "EP"
         },
-        "nl": "Het noorden"
+        "plural": {
+            "en": "offices",
+            "fi": "toimistot",
+            "nl": "de kantoren"
+        },
+        "singular": {
+            "en": "office",
+            "fi": "toimisto",
+            "nl": "het kantoor"
+        }
     },
-    "river": {
+    "park": {
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Rivers",
-            "fi": "Joet",
-            "nl": "De rivieren"
+            "en": "parks",
+            "fi": "puistot",
+            "nl": "de parken"
         },
         "singular": {
-            "en": "River",
-            "fi": "Joki",
-            "nl": "De rivier"
+            "en": "park",
+            "fi": "puisto",
+            "nl": "het park"
         }
     },
-    "sea": {
+    "port": {
         "level": {
-            "A1": [
+            "B1": [
                 "EP",
-                "KK",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Seas",
-            "fi": "Meret",
-            "nl": "De zee\u00ebn"
-        },
-        "singular": {
-            "en": "Sea",
-            "fi": "Meri",
-            "nl": "De zee"
-        }
-    },
-    "she is from the north": {
-        "en": "She is from the North",
-        "fi": [
-            "H\u00e4n tulee pohjoisesta;female",
-            "H\u00e4n on kotoisin pohjoisesta;female"
-        ],
-        "nl": "Zij komt uit het Noorden|Ze komt uit het Noorden",
-        "roots": [
-            "north",
-            "to come"
-        ]
+            "en": "ports",
+            "fi": "satamat",
+            "nl": "de havens"
+        },
+        "singular": {
+            "en": "port",
+            "fi": "satama",
+            "nl": "de haven"
+        }
     },
-    "south": {
-        "en": "South|The south",
-        "fi": "Etel\u00e4",
+    "square": {
         "level": {
-            "A1": "OD",
-            "A2": "EP"
+            "A2": [
+                "EP",
+                "OD"
+            ]
         },
-        "nl": "Het zuiden"
-    },
-    "the city is in the east": {
-        "en": "The city is in the East",
-        "fi": [
-            "Kaupunki on id\u00e4ss\u00e4",
-            "Kaupunki sijaitsee id\u00e4ss\u00e4"
-        ],
-        "nl": "De stad ligt in het Oosten",
-        "roots": [
-            "city",
-            "to be",
-            "east"
-        ]
-    },
-    "they live in the west": {
-        "en": "They live in the West",
-        "fi": "He asuvat l\u00e4nness\u00e4",
-        "nl": "Zij wonen in het Westen|Ze wonen in het Westen",
-        "roots": [
-            "west",
-            "to live"
-        ]
+        "plural": {
+            "en": "squares",
+            "fi": "aukiot",
+            "nl": "de pleinen"
+        },
+        "singular": {
+            "en": "square",
+            "fi": "aukio",
+            "nl": "het plein"
+        }
     },
-    "tree": {
+    "stadium": {
         "level": {
-            "A1": [
+            "A2": [
                 "EP",
-                "KK",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Trees",
-            "fi": "Puut",
-            "nl": "De bomen"
+            "en": "stadiums",
+            "fi": "stadionit",
+            "nl": "de stadions"
         },
         "singular": {
-            "en": "Tree",
-            "fi": "Puu",
-            "nl": "De boom"
+            "en": "stadium",
+            "fi": "stadion",
+            "nl": "het stadion"
         }
     },
-    "valley": {
+    "store": {
         "level": {
+            "A1": "KK",
             "A2": "OD",
             "B1": "EP"
         },
         "plural": {
-            "en": "Valleys",
-            "fi": "Laaksot",
-            "nl": "De valleien"
+            "en": "stores",
+            "fi": "kaupat",
+            "nl": "de winkels"
         },
         "singular": {
-            "en": "Valley",
-            "fi": "Laakso",
-            "nl": "De vallei"
+            "en": "store",
+            "fi": "kauppa",
+            "nl": "de winkel"
         }
     },
-    "west": {
-        "en": "West|The west",
-        "fi": "L\u00e4nsi",
-        "level": {
-            "A1": "OD",
-            "A2": "EP"
-        },
-        "nl": "Het westen"
-    },
-    "world": {
-        "en": "World",
-        "fi": "Maailma",
+    "street": {
         "level": {
             "A1": [
                 "EP",
                 "KK",
                 "OD"
             ]
         },
-        "nl": "De wereld",
-        "roots": {
-            "fi": "country"
+        "plural": {
+            "en": "streets",
+            "fi": "kadut",
+            "nl": "de straten"
+        },
+        "singular": {
+            "en": "street",
+            "fi": "katu",
+            "nl": "de straat"
+        }
+    },
+    "that building is a church": {
+        "en": "That building is a church.",
+        "fi": "Tuo rakennus on kirkko.",
+        "nl": "Dat gebouw is een kerk.",
+        "roots": [
+            "to be",
+            "building",
+            "church"
+        ]
+    },
+    "theater": {
+        "level": {
+            "B2": "OD",
+            "none": "EP"
+        },
+        "plural": {
+            "en": "theaters",
+            "fi": "teatterit",
+            "nl": "de theaters"
+        },
+        "singular": {
+            "en": "theater",
+            "fi": "teatteri",
+            "nl": "het theater"
         }
+    },
+    "there is a christmas tree on the square": {
+        "en": "There is a Christmas tree on the square.",
+        "fi": "Aukiolla on joulukuusi.",
+        "nl": "Er staat een kerstboom op het plein.",
+        "roots": [
+            "to be",
+            "square",
+            "christmas tree"
+        ]
+    },
+    "where is the library": {
+        "en": "Where is the library?",
+        "fi": "Miss\u00e4 on kirjasto?",
+        "nl": "Waar is de bibliotheek?",
+        "roots": [
+            "where",
+            "to be",
+            "library"
+        ]
     }
 }
```

### Comparing `Toisto-0.8.2/src/topics/possessive_adjectives.json` & `Toisto-0.9.0/src/topics/possessive_adjectives.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7788461538461539%*

 * *Differences: {"'her or his cat'": "OrderedDict([('roots', 'cat'), ('female', OrderedDict([('singular', "*

 * *                     "OrderedDict([('en', 'her cat'), ('fi', 'hänen kissansa;female singular'), "*

 * *                     "('nl', 'haar kat')])), ('plural', OrderedDict([('en', 'her cats'), ('fi', "*

 * *                     "'hänen kissansa;female plural'), ('nl', 'haar katten')]))])), ('male', "*

 * *                     "OrderedDict([('singular', OrderedDict([('en', 'his cat'), ('fi', 'hänen "*

 * *                     "kissansa;ma […]*

```diff
@@ -1,186 +1,186 @@
 {
-    "her or his house": {
+    "her or his cat": {
         "female": {
             "plural": {
-                "en": "Her houses",
-                "fi": "H\u00e4nen talonsa;female plural",
-                "nl": "Haar huizen"
+                "en": "her cats",
+                "fi": "h\u00e4nen kissansa;female plural",
+                "nl": "haar katten"
             },
             "singular": {
-                "en": "Her house",
-                "fi": "H\u00e4nen talonsa;female singular",
-                "nl": "Haar huis"
+                "en": "her cat",
+                "fi": "h\u00e4nen kissansa;female singular",
+                "nl": "haar kat"
             }
         },
         "male": {
             "plural": {
-                "en": "His houses",
-                "fi": "H\u00e4nen talonsa;male plural",
-                "nl": "Zijn huizen"
+                "en": "his cats",
+                "fi": "h\u00e4nen kissansa;male plural",
+                "nl": "zijn katten"
             },
             "singular": {
-                "en": "His house",
-                "fi": "H\u00e4nen talonsa;male singular",
-                "nl": "Zijn huis"
+                "en": "his cat",
+                "fi": "h\u00e4nen kissansa;male singular",
+                "nl": "zijn kat"
             }
         },
-        "roots": "house"
+        "roots": "cat"
     },
-    "hes or his cat": {
+    "her or his house": {
         "female": {
             "plural": {
-                "en": "Her cats",
-                "fi": "H\u00e4nen kissansa;female plural",
-                "nl": "Haar katten"
+                "en": "her houses",
+                "fi": "h\u00e4nen talonsa;female plural",
+                "nl": "haar huizen"
             },
             "singular": {
-                "en": "Her cat",
-                "fi": "H\u00e4nen kissansa;female singular",
-                "nl": "Haar kat"
+                "en": "her house",
+                "fi": "h\u00e4nen talonsa;female singular",
+                "nl": "haar huis"
             }
         },
         "male": {
             "plural": {
-                "en": "His cats",
-                "fi": "H\u00e4nen kissansa;male plural",
-                "nl": "Zijn katten"
+                "en": "his houses",
+                "fi": "h\u00e4nen talonsa;male plural",
+                "nl": "zijn huizen"
             },
             "singular": {
-                "en": "His cat",
-                "fi": "H\u00e4nen kissansa;male singular",
-                "nl": "Zijn kat"
+                "en": "his house",
+                "fi": "h\u00e4nen talonsa;male singular",
+                "nl": "zijn huis"
             }
         },
-        "roots": "cat"
+        "roots": "house"
     },
     "my cat": {
         "plural": {
-            "en": "My cats",
-            "fi": "Minun kissani;plural",
-            "nl": "Mijn katten"
+            "en": "my cats",
+            "fi": "minun kissani;plural",
+            "nl": "mijn katten"
         },
         "roots": "cat",
         "singular": {
-            "en": "My cat",
-            "fi": "Minun kissani;singular",
-            "nl": "Mijn kat"
+            "en": "my cat",
+            "fi": "minun kissani;singular",
+            "nl": "mijn kat"
         }
     },
     "my house": {
         "plural": {
-            "en": "My houses",
-            "fi": "Minun taloni;plural",
-            "nl": "Mijn huizen"
+            "en": "my houses",
+            "fi": "minun taloni;plural",
+            "nl": "mijn huizen"
         },
         "roots": "house",
         "singular": {
-            "en": "My house",
-            "fi": "Minun taloni;singular",
-            "nl": "Mijn huis"
+            "en": "my house",
+            "fi": "minun taloni;singular",
+            "nl": "mijn huis"
         }
     },
     "our cat": {
         "plural": {
-            "en": "Our cats",
-            "fi": "Meid\u00e4n kissamme;plural",
-            "nl": "Onze katten"
+            "en": "our cats",
+            "fi": "meid\u00e4n kissamme;plural",
+            "nl": "onze katten"
         },
         "roots": "cat",
         "singular": {
-            "en": "Our cat",
-            "fi": "Meid\u00e4n kissamme;singular",
-            "nl": "Onze kat"
+            "en": "our cat",
+            "fi": "meid\u00e4n kissamme;singular",
+            "nl": "onze kat"
         }
     },
     "our house": {
         "plural": {
-            "en": "Our houses",
-            "fi": "Meid\u00e4n talomme;plural",
-            "nl": "Onze huizen"
+            "en": "our houses",
+            "fi": "meid\u00e4n talomme;plural",
+            "nl": "onze huizen"
         },
         "roots": "house",
         "singular": {
-            "en": "Our house",
-            "fi": "Meid\u00e4n talomme;singular",
-            "nl": "Ons huis"
+            "en": "our house",
+            "fi": "meid\u00e4n talomme;singular",
+            "nl": "ons huis"
         }
     },
     "their cat": {
         "plural": {
-            "en": "Their cats",
-            "fi": "Heid\u00e4n kissansa;plural",
-            "nl": "Hun katten"
+            "en": "their cats",
+            "fi": "heid\u00e4n kissansa;plural",
+            "nl": "hun katten"
         },
         "roots": "cat",
         "singular": {
-            "en": "Their cat",
-            "fi": "Heid\u00e4n kissansa;singular",
-            "nl": "Hun kat"
+            "en": "their cat",
+            "fi": "heid\u00e4n kissansa;singular",
+            "nl": "hun kat"
         }
     },
     "their house": {
         "plural": {
-            "en": "Their houses",
-            "fi": "Heid\u00e4n talonsa;plural",
-            "nl": "Hun huizen"
+            "en": "their houses",
+            "fi": "heid\u00e4n talonsa;plural",
+            "nl": "hun huizen"
         },
         "roots": "house",
         "singular": {
-            "en": "Their house",
-            "fi": "Heid\u00e4n talonsa;singular",
-            "nl": "Hun huis"
+            "en": "their house",
+            "fi": "heid\u00e4n talonsa;singular",
+            "nl": "hun huis"
         }
     },
     "your (pl) cat": {
         "plural": {
-            "en": "Your cats;plural",
-            "fi": "Teid\u00e4n kissanne;plural",
-            "nl": "Jullie katten"
+            "en": "your cats;plural",
+            "fi": "teid\u00e4n kissanne;plural",
+            "nl": "jullie katten"
         },
         "roots": "cat",
         "singular": {
-            "en": "Yuur cat;plural",
-            "fi": "Teid\u00e4n kissanne;singular",
-            "nl": "Jullie kat"
+            "en": "your cat;plural",
+            "fi": "teid\u00e4n kissanne;singular",
+            "nl": "jullie kat"
         }
     },
     "your (pl) house": {
         "plural": {
-            "en": "Your houses;plural",
-            "fi": "Teid\u00e4n talonne;plural",
-            "nl": "Jullie huizen"
+            "en": "your houses;plural",
+            "fi": "teid\u00e4n talonne;plural",
+            "nl": "jullie huizen"
         },
         "roots": "house",
         "singular": {
-            "en": "Your house;plural",
-            "fi": "Teid\u00e4n talonne;singular",
-            "nl": "Jullie huis"
+            "en": "your house;plural",
+            "fi": "teid\u00e4n talonne;singular",
+            "nl": "jullie huis"
         }
     },
     "your cat": {
         "plural": {
-            "en": "Your cats;singular",
-            "fi": "Sinun kissasi;plural",
-            "nl": "Jouw katten"
+            "en": "your cats;singular",
+            "fi": "sinun kissasi;plural",
+            "nl": "jouw katten"
         },
         "roots": "cat",
         "singular": {
-            "en": "Your cat;singular",
-            "fi": "Sinun kissasi;singular",
-            "nl": "Jouw kat"
+            "en": "your cat;singular",
+            "fi": "sinun kissasi;singular",
+            "nl": "jouw kat"
         }
     },
     "your house": {
         "plural": {
-            "en": "Your houses;singular",
-            "fi": "Sinun talosi;plural",
-            "nl": "Jouw huizen"
+            "en": "your houses;singular",
+            "fi": "sinun talosi;plural",
+            "nl": "jouw huizen"
         },
         "roots": "house",
         "singular": {
-            "en": "Your house;singular",
-            "fi": "Sinun talosi;singular",
-            "nl": "Jouw huis"
+            "en": "your house;singular",
+            "fi": "sinun talosi;singular",
+            "nl": "jouw huis"
         }
     }
 }
```

### Comparing `Toisto-0.8.2/src/topics/seasons.json` & `Toisto-0.9.0/src/topics/seasons.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8373015873015874%*

 * *Differences: {"'autumn'": "{'singular': {'en': ['autumn', 'fall'], 'fi': 'syksy', 'nl': ['de herfst', 'het "*

 * *             "najaar']}, 'plural': {'en': ['autumns', 'falls'], 'fi': 'syksyt', 'nl': ['de "*

 * *             "herfsten', 'de najaren']}}",*

 * * "'dutch springs are wet'": "{'en': 'Dutch springs are wet.', 'fi': ['Hollannin keväät ovat "*

 * *                            "märkiä.', 'Alankomaiden keväät ovat märkiä.'], 'nl': ['Nederlandse "*

 * *                            "lentes zijn nat.', 'Nederlandse voorjaren zijn nat.']}",*

 * * " […]*

```diff
@@ -5,237 +5,243 @@
                 "KK",
                 "OD"
             ],
             "A2": "EP"
         },
         "plural": {
             "en": [
-                "Autumns",
-                "Falls"
+                "autumns",
+                "falls"
             ],
-            "fi": "Syksyt",
+            "fi": "syksyt",
             "nl": [
-                "De herfsten",
-                "De najaren"
+                "de herfsten",
+                "de najaren"
             ]
         },
         "singular": {
             "en": [
-                "Autumn",
-                "Fall"
+                "autumn",
+                "fall"
             ],
-            "fi": "Syksy",
+            "fi": "syksy",
             "nl": [
-                "De herfst",
-                "Het najaar"
+                "de herfst",
+                "het najaar"
             ]
         }
     },
     "dutch springs are wet": {
-        "en": "Dutch springs are wet",
+        "en": "Dutch springs are wet.",
         "fi": [
-            "Hollannin kev\u00e4\u00e4t ovat m\u00e4rki\u00e4",
-            "Alankomaiden kev\u00e4\u00e4t ovat m\u00e4rki\u00e4"
+            "Hollannin kev\u00e4\u00e4t ovat m\u00e4rki\u00e4.",
+            "Alankomaiden kev\u00e4\u00e4t ovat m\u00e4rki\u00e4."
         ],
         "nl": [
-            "Nederlandse lentes zijn nat",
-            "Nederlandse voorjaren zijn nat"
+            "Nederlandse lentes zijn nat.",
+            "Nederlandse voorjaren zijn nat."
         ],
         "roots": [
             "spring",
             "to be",
             "wet"
         ]
     },
     "finnish winters are cold": {
-        "en": "Finnish winters are cold",
-        "fi": "Suomen talvet ovat kylmi\u00e4",
-        "nl": "Finse winters zijn koud",
+        "en": "Finnish winters are cold.",
+        "fi": "Suomen talvet ovat kylmi\u00e4.",
+        "nl": "Finse winters zijn koud.",
         "roots": [
             "winter",
             "to be",
             "cold"
         ]
     },
     "in autumn": {
         "en": [
-            "In autumn",
-            "In fall"
+            "in autumn",
+            "in fall"
         ],
-        "fi": "Syksyll\u00e4",
+        "fi": "syksyll\u00e4",
         "nl": [
-            "In de herfst",
-            "In het najaar"
+            "in de herfst",
+            "in het najaar"
         ],
         "roots": "autumn"
     },
     "in spring": {
-        "en": "In spring",
-        "fi": "Kev\u00e4\u00e4ll\u00e4",
+        "en": "in spring",
+        "fi": "kev\u00e4\u00e4ll\u00e4",
         "nl": [
-            "In de lente",
-            "In het voorjaar"
+            "in de lente",
+            "in het voorjaar"
         ],
         "roots": "spring"
     },
     "in summer": {
-        "en": "In summer",
-        "fi": "Kes\u00e4ll\u00e4",
-        "nl": "In de zomer",
+        "en": "in summer",
+        "fi": "kes\u00e4ll\u00e4",
+        "nl": "in de zomer",
         "roots": "summer"
     },
     "in winter": {
-        "en": "In winter",
-        "fi": "Talvella",
-        "nl": "In de winter",
+        "en": "in winter",
+        "fi": "talvella",
+        "nl": "in de winter",
         "roots": "winter"
     },
     "last autumn": {
-        "en": "Last autumn",
-        "fi": "Viime syksyn\u00e4",
+        "en": [
+            "last autumn",
+            "last fall"
+        ],
+        "fi": "viime syksyn\u00e4",
         "nl": [
-            "Vorige herfst",
-            "Vorig najaar"
+            "vorige herfst",
+            "vorig najaar"
         ],
         "roots": "autumn"
     },
     "last spring": {
-        "en": "Last spring",
-        "fi": "Viime kev\u00e4\u00e4n\u00e4",
+        "en": "last spring",
+        "fi": "viime kev\u00e4\u00e4n\u00e4",
         "nl": [
-            "Vorige lente",
-            "Vorig voorjaar"
+            "vorige lente",
+            "vorig voorjaar"
         ],
         "roots": "spring"
     },
     "last summer": {
-        "en": "Last summer",
-        "fi": "Viime kes\u00e4n\u00e4",
-        "nl": "Vorige zomer",
+        "en": "last summer",
+        "fi": "viime kes\u00e4n\u00e4",
+        "nl": "vorige zomer",
         "roots": "summer"
     },
     "last winter": {
-        "en": "Last winter",
-        "fi": "Viime talvena",
-        "nl": "Vorige winter",
+        "en": "last winter",
+        "fi": "viime talvena",
+        "nl": "vorige winter",
         "roots": "winter"
     },
     "next autumn": {
-        "en": "Next autumn|Next fall",
-        "fi": "Ensi syksyn\u00e4",
+        "en": [
+            "next autumn",
+            "next fall"
+        ],
+        "fi": "ensi syksyn\u00e4",
         "nl": [
-            "Volgende herfst",
-            "Volgend najaar"
+            "volgende herfst",
+            "volgend najaar"
         ],
         "roots": "autumn"
     },
     "next spring": {
-        "en": "Next spring",
-        "fi": "Ensi kev\u00e4\u00e4n\u00e4",
+        "en": "next spring",
+        "fi": "ensi kev\u00e4\u00e4n\u00e4",
         "nl": [
-            "Volgende lente",
-            "Volgend voorjaar"
+            "volgende lente",
+            "volgend voorjaar"
         ],
         "roots": "spring"
     },
     "next summer": {
-        "en": "Next summer",
-        "fi": "Ensi kes\u00e4n\u00e4",
-        "nl": "Volgende zomer",
+        "en": "next summer",
+        "fi": "ensi kes\u00e4n\u00e4",
+        "nl": "volgende zomer",
         "roots": "summer"
     },
     "next winter": {
-        "en": "Next winter",
-        "fi": "Ensi talvena",
-        "nl": "Volgende winter",
+        "en": "next winter",
+        "fi": "ensi talvena",
+        "nl": "volgende winter",
         "roots": "winter"
     },
     "season": {
         "level": {
             "A2": "OD",
             "B1": "EP"
         },
         "plural": {
-            "en": "Seasons",
-            "fi": "Vuodenajat",
-            "nl": "De seizoenen"
+            "en": "seasons",
+            "fi": "vuodenajat",
+            "nl": "de seizoenen"
         },
         "singular": {
-            "en": "Season",
-            "fi": "Vuodenaika",
-            "nl": "Het seizoen"
+            "en": "season",
+            "fi": "vuodenaika",
+            "nl": "het seizoen"
         }
     },
     "spring": {
         "level": {
             "A1": [
                 "KK",
                 "OD"
             ],
             "A2": "EP"
         },
         "plural": {
-            "en": "Springs",
-            "fi": "Kev\u00e4\u00e4t",
+            "en": "springs",
+            "fi": "kev\u00e4\u00e4t",
             "nl": [
-                "De lentes",
-                "De voorjaren"
+                "de lentes",
+                "de voorjaren"
             ]
         },
         "singular": {
-            "en": "Spring",
-            "fi": "Kev\u00e4t",
+            "en": "spring",
+            "fi": "kev\u00e4t",
             "nl": [
-                "De lente",
-                "Het voorjaar"
+                "de lente",
+                "het voorjaar"
             ]
         }
     },
     "summer": {
         "level": {
             "A1": [
                 "EP",
                 "KK",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Summers",
-            "fi": "Kes\u00e4t",
-            "nl": "De zomers"
+            "en": "summers",
+            "fi": "kes\u00e4t",
+            "nl": "de zomers"
         },
         "singular": {
-            "en": "Summer",
-            "fi": "Kes\u00e4",
-            "nl": "De zomer"
+            "en": "summer",
+            "fi": "kes\u00e4",
+            "nl": "de zomer"
         }
     },
     "the dutch autumn is wet": {
         "en": [
-            "The Dutch autumn is wet",
-            "The Dutch fall is wet"
+            "The Dutch autumn is wet.",
+            "The Dutch fall is wet."
         ],
         "fi": [
-            "Hollannin syksy on m\u00e4rk\u00e4",
-            "Alankomaiden syksy on m\u00e4rk\u00e4"
+            "Hollannin syksy on m\u00e4rk\u00e4.",
+            "Alankomaiden syksy on m\u00e4rk\u00e4."
         ],
         "nl": [
-            "De Nederlandse herfst is nat",
-            "Het Nederlandse najaar is nat"
+            "De Nederlandse herfst is nat.",
+            "Het Nederlandse najaar is nat."
         ],
         "roots": [
             "autumn",
             "to be",
             "wet"
         ]
     },
     "the finnish winter is cold": {
-        "en": "The Finnish winter is cold",
-        "fi": "Suomen talvi on kylm\u00e4",
-        "nl": "De Finse winter is koud",
+        "en": "The Finnish winter is cold.",
+        "fi": "Suomen talvi on kylm\u00e4.",
+        "nl": "De Finse winter is koud.",
         "roots": [
             "winter",
             "to be",
             "cold"
         ]
     },
     "winter": {
@@ -243,18 +249,18 @@
             "A1": [
                 "EP",
                 "KK",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Winters",
-            "fi": "Talvet",
-            "nl": "De winters"
+            "en": "winters",
+            "fi": "talvet",
+            "nl": "de winters"
         },
         "singular": {
-            "en": "Winter",
-            "fi": "Talvi",
-            "nl": "De winter"
+            "en": "winter",
+            "fi": "talvi",
+            "nl": "de winter"
         }
     }
 }
```

### Comparing `Toisto-0.8.2/src/topics/sentence_types.json` & `Toisto-0.9.0/src/topics/sentence_types.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9962022569444444%*

 * *Differences: {"'the car is black'": "{'declarative': {'affirmative': {'present tense': {'singular': {'en': 'The "*

 * *                       "car is black.', 'fi': 'Auto on musta.', 'nl': 'De auto is zwart.'}, "*

 * *                       "'plural': {'en': 'The cars are black.', 'fi': 'Autot ovat mustia.', 'nl': "*

 * *                       '"De auto\'s zijn zwart."}}, \'past tense\': {\'singular\': {\'en\': \'The '*

 * *                       "car was black.', 'fi': 'Auto oli musta.', 'nl': 'De auto was zwart.'}, "*

 * *                     […]*

```diff
@@ -1,59 +1,59 @@
 {
     "the car is black": {
         "declarative": {
             "affirmative": {
                 "past tense": {
                     "plural": {
-                        "en": "The cars were black",
-                        "fi": "Autot olivat mustia",
-                        "nl": "De auto's waren zwart"
+                        "en": "The cars were black.",
+                        "fi": "Autot olivat mustia.",
+                        "nl": "De auto's waren zwart."
                     },
                     "singular": {
-                        "en": "The car was black",
-                        "fi": "Auto oli musta",
-                        "nl": "De auto was zwart"
+                        "en": "The car was black.",
+                        "fi": "Auto oli musta.",
+                        "nl": "De auto was zwart."
                     }
                 },
                 "present tense": {
                     "plural": {
-                        "en": "The cars are black",
-                        "fi": "Autot ovat mustia",
-                        "nl": "De auto's zijn zwart"
+                        "en": "The cars are black.",
+                        "fi": "Autot ovat mustia.",
+                        "nl": "De auto's zijn zwart."
                     },
                     "singular": {
-                        "en": "The car is black",
-                        "fi": "Auto on musta",
-                        "nl": "De auto is zwart"
+                        "en": "The car is black.",
+                        "fi": "Auto on musta.",
+                        "nl": "De auto is zwart."
                     }
                 }
             },
             "negative": {
                 "past tense": {
                     "plural": {
-                        "en": "The cars were not black|The cars weren't black",
-                        "fi": "Autot eiv\u00e4t olleet mustia",
-                        "nl": "De auto's waren niet zwart"
+                        "en": "The cars were not black.|The cars weren't black.",
+                        "fi": "Autot eiv\u00e4t olleet mustia.",
+                        "nl": "De auto's waren niet zwart."
                     },
                     "singular": {
-                        "en": "The car was not black|The car wasn't black",
-                        "fi": "Auto ei ollut musta",
-                        "nl": "De auto was niet zwart"
+                        "en": "The car was not black.|The car wasn't black.",
+                        "fi": "Auto ei ollut musta.",
+                        "nl": "De auto was niet zwart."
                     }
                 },
                 "present tense": {
                     "plural": {
-                        "en": "The cars are not black|The cars aren't black",
-                        "fi": "Autot eiv\u00e4t ole mustia",
-                        "nl": "De auto's zijn niet zwart"
+                        "en": "The cars are not black.|The cars aren't black.",
+                        "fi": "Autot eiv\u00e4t ole mustia.",
+                        "nl": "De auto's zijn niet zwart."
                     },
                     "singular": {
-                        "en": "The car is not black|The car isn't black",
-                        "fi": "Auto ei ole musta",
-                        "nl": "De auto is niet zwart"
+                        "en": "The car is not black.|The car isn't black.",
+                        "fi": "Auto ei ole musta.",
+                        "nl": "De auto is niet zwart."
                     }
                 }
             }
         },
         "interrogative": {
             "affirmative": {
                 "past tense": {
@@ -116,181 +116,181 @@
     },
     "to speak english": {
         "declarative": {
             "affirmative": {
                 "past tense": {
                     "plural": {
                         "first person": {
-                            "en": "We spoke English",
-                            "fi": "Me puhuimme englantia|Puhuimme englantia",
-                            "nl": "Wij spraken Engels|We spraken Engels"
+                            "en": "We spoke English.",
+                            "fi": "Me puhuimme englantia.|Puhuimme englantia.",
+                            "nl": "Wij spraken Engels.|We spraken Engels"
                         },
                         "second person": {
-                            "en": "You spoke English;plural",
-                            "fi": "Te puhuitte englantia|Puhuitte englantia",
-                            "nl": "Jullie spraken Engels"
+                            "en": "You spoke English.;plural",
+                            "fi": "Te puhuitte englantia.|Puhuitte englantia.",
+                            "nl": "Jullie spraken Engels."
                         },
                         "third person": {
-                            "en": "They spoke English",
-                            "fi": "He puhuivat englantia",
-                            "nl": "Zij spraken Engels|Ze spraken Engels"
+                            "en": "They spoke English.",
+                            "fi": "He puhuivat englantia.",
+                            "nl": "Zij spraken Engels.|Ze spraken Engels."
                         }
                     },
                     "singular": {
                         "first person": {
-                            "en": "I spoke English",
-                            "fi": "Min\u00e4 puhuin englantia|Puhuin englantia",
-                            "nl": "Ik sprak Engels"
+                            "en": "I spoke English.",
+                            "fi": "Min\u00e4 puhuin englantia.|Puhuin englantia.",
+                            "nl": "Ik sprak Engels."
                         },
                         "second person": {
-                            "en": "You spoke English;singular",
-                            "fi": "Sin\u00e4 puhuit englantia|Puhuit englantia",
-                            "nl": "Jij sprak Engels|Je sprak Engels"
+                            "en": "You spoke English.;singular",
+                            "fi": "Sin\u00e4 puhuit englantia.|Puhuit englantia.",
+                            "nl": "Jij sprak Engels.|Je sprak Engels."
                         },
                         "third person": {
                             "female": {
-                                "en": "She spoke English",
-                                "fi": "H\u00e4n puhui englantia;female",
-                                "nl": "Zij sprak Engels|Ze sprak Engels"
+                                "en": "She spoke English.",
+                                "fi": "H\u00e4n puhui englantia.;female",
+                                "nl": "Zij sprak Engels.|Ze sprak Engels."
                             },
                             "male": {
-                                "en": "He spoke English",
-                                "fi": "H\u00e4n puhui englantia;male",
-                                "nl": "Hij sprak Engels"
+                                "en": "He spoke English.",
+                                "fi": "H\u00e4n puhui englantia.;male",
+                                "nl": "Hij sprak Engels."
                             }
                         }
                     }
                 },
                 "present tense": {
                     "plural": {
                         "first person": {
-                            "en": "We speak English",
-                            "fi": "Me puhumme englantia|Puhumme englantia",
-                            "nl": "Wij spreken Engels|We spreken Engels"
+                            "en": "We speak English.",
+                            "fi": "Me puhumme englantia.|Puhumme englantia.",
+                            "nl": "Wij spreken Engels.|We spreken Engels."
                         },
                         "second person": {
-                            "en": "You speak English;plural",
-                            "fi": "Te puhutte englantia|Puhutte englantia",
-                            "nl": "Jullie spreken Engels"
+                            "en": "You speak English.;plural",
+                            "fi": "Te puhutte englantia.|Puhutte englantia.",
+                            "nl": "Jullie spreken Engels."
                         },
                         "third person": {
-                            "en": "They speak English",
-                            "fi": "He puhuvat englantia",
-                            "nl": "Zij spreken Engels|Ze spreken Engels"
+                            "en": "They speak English.",
+                            "fi": "He puhuvat englantia.",
+                            "nl": "Zij spreken Engels.|Ze spreken Engels."
                         }
                     },
                     "singular": {
                         "first person": {
-                            "en": "I speak English",
-                            "fi": "Min\u00e4 puhun englantia|Puhun englantia",
-                            "nl": "Ik spreek Engels"
+                            "en": "I speak English.",
+                            "fi": "Min\u00e4 puhun englantia.|Puhun englantia.",
+                            "nl": "Ik spreek Engels."
                         },
                         "second person": {
-                            "en": "You speak English;singular",
-                            "fi": "Sin\u00e4 puhut englantia|Puhut englantia",
-                            "nl": "Jij spreekt Engels|Je spreekt Engels"
+                            "en": "You speak English.;singular",
+                            "fi": "Sin\u00e4 puhut englantia.|Puhut englantia.",
+                            "nl": "Jij spreekt Engels.|Je spreekt Engels."
                         },
                         "third person": {
                             "female": {
-                                "en": "She speaks English",
-                                "fi": "H\u00e4n puhuu englantia;female",
-                                "nl": "Zij spreekt Engels|Ze spreekt Engels"
+                                "en": "She speaks English.",
+                                "fi": "H\u00e4n puhuu englantia.;female",
+                                "nl": "Zij spreekt Engels.|Ze spreekt Engels."
                             },
                             "male": {
-                                "en": "He speaks English",
-                                "fi": "H\u00e4n puhuu englantia;male",
-                                "nl": "Hij spreekt Engels"
+                                "en": "He speaks English.",
+                                "fi": "H\u00e4n puhuu englantia.;male",
+                                "nl": "Hij spreekt Engels."
                             }
                         }
                     }
                 }
             },
             "negative": {
                 "past tense": {
                     "plural": {
                         "first person": {
-                            "en": "We did not speak English|We didn't speak English",
-                            "fi": "Me emme puhuneet englantia|Emme puhuneet englantia",
-                            "nl": "Wij spraken geen Engels|We spraken geen Engels"
+                            "en": "We did not speak English.|We didn't speak English.",
+                            "fi": "Me emme puhuneet englantia.|Emme puhuneet englantia.",
+                            "nl": "Wij spraken geen Engels.|We spraken geen Engels."
                         },
                         "second person": {
-                            "en": "You did not speak English|You didn't speak English;plural",
-                            "fi": "Te ette puhuneet englantia|Ette puhuneet englantia",
-                            "nl": "Jullie spraken geen Engels"
+                            "en": "You did not speak English.|You didn't speak English.;plural",
+                            "fi": "Te ette puhuneet englantia.|Ette puhuneet englantia.",
+                            "nl": "Jullie spraken geen Engels."
                         },
                         "third person": {
-                            "en": "They did not speak English|They didn't speak English",
-                            "fi": "He eiv\u00e4t puhuneet englantia",
-                            "nl": "Zij spraken geen Engels|Ze spraken geen Engels"
+                            "en": "They did not speak English.|They didn't speak English.",
+                            "fi": "He eiv\u00e4t puhuneet englantia.",
+                            "nl": "Zij spraken geen Engels.|Ze spraken geen Engels."
                         }
                     },
                     "singular": {
                         "first person": {
-                            "en": "I did not speak English|I didn't speak English",
-                            "fi": "Min\u00e4 en puhunut englantia|En puhunut englantia",
-                            "nl": "Ik sprak geen Engels"
+                            "en": "I did not speak English.|I didn't speak English.",
+                            "fi": "Min\u00e4 en puhunut englantia.|En puhunut englantia.",
+                            "nl": "Ik sprak geen Engels."
                         },
                         "second person": {
-                            "en": "You did not speak English|You didn't speak English;singular",
-                            "fi": "Sin\u00e4 et puhunut englantia|Et puhunut englantia",
-                            "nl": "Jij sprak geen Engels|Je sprak geen Engels"
+                            "en": "You did not speak English.|You didn't speak English.;singular",
+                            "fi": "Sin\u00e4 et puhunut englantia.|Et puhunut englantia.",
+                            "nl": "Jij sprak geen Engels.|Je sprak geen Engels."
                         },
                         "third person": {
                             "female": {
-                                "en": "She did not speak English|She didn't speak English",
-                                "fi": "H\u00e4n ei puhunut englantia;female",
-                                "nl": "Zij sprak geen Engels|Ze sprak geen Engels"
+                                "en": "She did not speak English.|She didn't speak English.",
+                                "fi": "H\u00e4n ei puhunut englantia.;female",
+                                "nl": "Zij sprak geen Engels.|Ze sprak geen Engels."
                             },
                             "male": {
-                                "en": "He did not speak English|He didn't speak",
-                                "fi": "H\u00e4n ei puhunut englantia;male",
-                                "nl": "Hij sprak geen Engels"
+                                "en": "He did not speak English.|He didn't speak.",
+                                "fi": "H\u00e4n ei puhunut englantia.;male",
+                                "nl": "Hij sprak geen Engels."
                             }
                         }
                     }
                 },
                 "present tense": {
                     "plural": {
                         "first person": {
-                            "en": "We do not speak English|We don't speak English",
-                            "fi": "Me emme puhu englantia|Emme puhu englantia",
-                            "nl": "Wij spreken geen Engels|We spreken geen Engels"
+                            "en": "We do not speak English.|We don't speak English.",
+                            "fi": "Me emme puhu englantia.|Emme puhu englantia.",
+                            "nl": "Wij spreken geen Engels.|We spreken geen Engels."
                         },
                         "second person": {
-                            "en": "You do not speak EnglishYou don't speak English;plural",
-                            "fi": "Te ette puhu englantia|Ette puhu englantia",
-                            "nl": "Jullie spreken geen Engels"
+                            "en": "You do not speak English.|You don't speak English.;plural",
+                            "fi": "Te ette puhu englantia.|Ette puhu englantia.",
+                            "nl": "Jullie spreken geen Engels."
                         },
                         "third person": {
-                            "en": "They do not speak English|They don't speak English",
-                            "fi": "He eiv\u00e4t puhu englantia|Eiv\u00e4t puhu englantia",
-                            "nl": "Zij spreken geen Engels|Ze spreken geen Engels"
+                            "en": "They do not speak English.|They don't speak English.",
+                            "fi": "He eiv\u00e4t puhu englantia.|Eiv\u00e4t puhu englantia.",
+                            "nl": "Zij spreken geen Engels.|Ze spreken geen Engels."
                         }
                     },
                     "singular": {
                         "first person": {
-                            "en": "I do not speak English|I don't speak English",
-                            "fi": "Min\u00e4 en puhu englantia|En puhu englantia",
-                            "nl": "Ik spreek geen Engels"
+                            "en": "I do not speak English.|I don't speak English.",
+                            "fi": "Min\u00e4 en puhu englantia.|En puhu englantia.",
+                            "nl": "Ik spreek geen Engels."
                         },
                         "second person": {
-                            "en": "You do not speak English|You don't speak English;singular",
-                            "fi": "Sin\u00e4 et puhu englantia|Et puhu englantia",
-                            "nl": "Jij spreekt geen Engels|Je spreekt geen Engels"
+                            "en": "You do not speak English.|You don't speak English.;singular",
+                            "fi": "Sin\u00e4 et puhu englantia.|Et puhu englantia.",
+                            "nl": "Jij spreekt geen Engels.|Je spreekt geen Engels."
                         },
                         "third person": {
                             "female": {
-                                "en": "She does not speak English|She doesn't speak English",
-                                "fi": "H\u00e4n ei puhu englantia;female",
-                                "nl": "Zij spreekt geen Engels|Ze spreekt geen Engels"
+                                "en": "She does not speak English.|She doesn't speak English.",
+                                "fi": "H\u00e4n ei puhu englantia.;female",
+                                "nl": "Zij spreekt geen Engels.|Ze spreekt geen Engels."
                             },
                             "male": {
-                                "en": "He speaks English",
-                                "fi": "H\u00e4n ei puhu englantia;male",
-                                "nl": "Hij spreekt geen Engels"
+                                "en": "He speaks English.",
+                                "fi": "H\u00e4n ei puhu englantia.;male",
+                                "nl": "Hij spreekt geen Engels."
                             }
                         }
                     }
                 }
             }
         },
         "interrogative": {
```

### Comparing `Toisto-0.8.2/src/topics/time.json` & `Toisto-0.9.0/src/topics/time.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.892361111111111%*

 * *Differences: {"'afternoon'": "{'singular': {'en': 'afternoon', 'fi': 'iltapäivä', 'nl': 'de middag'}, 'plural': "*

 * *                "{'en': 'afternoons', 'fi': 'iltapäivät', 'nl': 'de middagen'}}",*

 * * "'century'": "{'singular': {'en': 'century', 'fi': 'vuosisata', 'nl': 'de eeuw'}, 'plural': "*

 * *              "{'en': 'centuries', 'fi': 'vuosisadat', 'nl': 'de eeuwen'}}",*

 * * "'clock'": "{'singular': {'en': 'clock', 'fi': 'kello', 'nl': 'de klok'}, 'plural': {'en': "*

 * *            "'clocks', 'fi': 'kelloja', 'nl': 'de klokken'}}",*

 * * […]*

```diff
@@ -3,146 +3,146 @@
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Afternoons",
-            "fi": "Iltap\u00e4iv\u00e4t",
-            "nl": "De middagen"
+            "en": "afternoons",
+            "fi": "iltap\u00e4iv\u00e4t",
+            "nl": "de middagen"
         },
         "roots": {
             "en": "noon",
             "fi": [
                 "evening",
                 "day"
             ],
             "nl": "day"
         },
         "singular": {
-            "en": "Afternoon",
-            "fi": "Iltap\u00e4iv\u00e4",
-            "nl": "De middag"
+            "en": "afternoon",
+            "fi": "iltap\u00e4iv\u00e4",
+            "nl": "de middag"
         }
     },
     "century": {
         "level": {
             "B1": "OD",
             "B2": "EP"
         },
         "plural": {
-            "en": "Centuries",
-            "fi": "Vuosisadat",
-            "nl": "De eeuwen"
+            "en": "centuries",
+            "fi": "vuosisadat",
+            "nl": "de eeuwen"
         },
         "roots": {
             "fi": [
                 "100",
                 "year"
             ]
         },
         "singular": {
-            "en": "Century",
-            "fi": "Vuosisata",
-            "nl": "De eeuw"
+            "en": "century",
+            "fi": "vuosisata",
+            "nl": "de eeuw"
         }
     },
     "clock": {
         "level": {
             "A1": [
                 "EP",
                 "KK",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Clocks",
-            "fi": "Kelloja",
-            "nl": "De klokken"
+            "en": "clocks",
+            "fi": "kelloja",
+            "nl": "de klokken"
         },
         "singular": {
-            "en": "Clock",
-            "fi": "Kello",
-            "nl": "De klok"
+            "en": "clock",
+            "fi": "kello",
+            "nl": "de klok"
         }
     },
     "decade": {
         "level": {
             "B1": "OD",
             "B2": "EP"
         },
         "plural": {
-            "en": "Decades",
-            "fi": "Vuosikymmenet",
-            "nl": "De decennia"
+            "en": "decades",
+            "fi": "vuosikymmenet",
+            "nl": "de decennia"
         },
         "roots": {
             "fi": [
                 "10",
                 "year"
             ]
         },
         "singular": {
-            "en": "Decade",
-            "fi": "Vuosikymmen",
-            "nl": "Het decennium"
+            "en": "decade",
+            "fi": "vuosikymmen",
+            "nl": "het decennium"
         }
     },
     "evening": {
         "level": {
             "A1": [
                 "EP",
                 "KK",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Evenings",
-            "fi": "Illat",
-            "nl": "De avonden"
+            "en": "evenings",
+            "fi": "illat",
+            "nl": "de avonden"
         },
         "singular": {
-            "en": "Evening",
-            "fi": "Ilta",
-            "nl": "De avond"
+            "en": "evening",
+            "fi": "ilta",
+            "nl": "de avond"
         }
     },
     "hour": {
         "level": {
             "A1": [
                 "EP",
                 "KK",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Hours",
-            "fi": "Tunnit",
-            "nl": "De uren"
+            "en": "hours",
+            "fi": "tunnit",
+            "nl": "de uren"
         },
         "singular": {
-            "en": "Hour",
-            "fi": "Tunti",
-            "nl": "Het uur"
+            "en": "hour",
+            "fi": "tunti",
+            "nl": "het uur"
         }
     },
     "how long does it take": {
         "en": "How long does it take?",
         "fi": [
             "Kauanko se kest\u00e4\u00e4?",
             "Kuinka kauan se kest\u00e4\u00e4?"
         ],
         "nl": "Hoe lang duurt het?",
         "roots": "how"
     },
     "it is 10:00": {
-        "en": "It is ten o'clock|It's ten o'clock",
-        "fi": "Kello on kymmenen",
-        "nl": "Het is tien uur",
+        "en": "It is ten o'clock.|It's ten o'clock.",
+        "fi": "Kello on kymmenen.",
+        "nl": "Het is tien uur.",
         "roots": {
             "en": [
                 "to be",
                 "10",
                 "clock"
             ],
             "fi": [
@@ -154,17 +154,17 @@
                 "to be",
                 "10",
                 "hour"
             ]
         }
     },
     "it is 2:30": {
-        "en": "It is half past two|It's half past two",
-        "fi": "Kello on puoli kolme",
-        "nl": "Het is half drie",
+        "en": "It is half past two.|It's half past two.",
+        "fi": "Kello on puoli kolme.",
+        "nl": "Het is half drie.",
         "roots": {
             "en": [
                 "to be",
                 "2",
                 "10"
             ],
             "fi": [
@@ -175,17 +175,17 @@
             "nl": [
                 "to be",
                 "3"
             ]
         }
     },
     "it is 3:15": {
-        "en": "It is a quarter past three|It's a quarter past three",
-        "fi": "Kello on vartin yli kolme",
-        "nl": "Het is kwart over drie",
+        "en": "It is a quarter past three.|It's a quarter past three.",
+        "fi": "Kello on vartin yli kolme.",
+        "nl": "Het is kwart over drie.",
         "roots": {
             "en": [
                 "to be",
                 "3"
             ],
             "fi": [
                 "to be",
@@ -195,17 +195,17 @@
             "nl": [
                 "to be",
                 "3"
             ]
         }
     },
     "it is 3:45": {
-        "en": "It is a quarter to four|It's a quarter to four",
-        "fi": "Kello on varttia vaille nelj\u00e4",
-        "nl": "Het is kwart voor vier",
+        "en": "It is a quarter to four.|It's a quarter to four.",
+        "fi": "Kello on varttia vaille nelj\u00e4.",
+        "nl": "Het is kwart voor vier.",
         "roots": {
             "en": [
                 "to be",
                 "4"
             ],
             "fi": [
                 "to be",
@@ -215,20 +215,20 @@
             "nl": [
                 "to be",
                 "4"
             ]
         }
     },
     "it is 6:20": {
-        "en": "It is twenty past six|It's twenty past six",
+        "en": "It is twenty past six.|It's twenty past six.",
         "fi": [
-            "Kello on kuusi kaksikymment\u00e4",
-            "Kello on kaksikymment\u00e4 yli kuusi"
+            "Kello on kuusi kaksikymment\u00e4.",
+            "Kello on kaksikymment\u00e4 yli kuusi."
         ],
-        "nl": "Het is tien voor half zeven",
+        "nl": "Het is tien voor half zeven.",
         "roots": {
             "en": [
                 "to be",
                 "6",
                 "20"
             ],
             "fi": [
@@ -241,20 +241,20 @@
                 "to be",
                 "10",
                 "7"
             ]
         }
     },
     "it is 6:40": {
-        "en": "It is twenty to seven|It's twenty to seven",
+        "en": "It is twenty to seven.|It's twenty to seven.",
         "fi": [
-            "Kello on kuusi nelj\u00e4kymment\u00e4",
-            "Kello on kahtakymment\u00e4 vaille seitsem\u00e4n"
+            "Kello on kuusi nelj\u00e4kymment\u00e4.",
+            "Kello on kahtakymment\u00e4 vaille seitsem\u00e4n."
         ],
-        "nl": "Het is tien over half zeven",
+        "nl": "Het is tien over half zeven.",
         "roots": {
             "en": [
                 "to be",
                 "7",
                 "20"
             ],
             "fi": [
@@ -269,17 +269,17 @@
                 "to be",
                 "10",
                 "7"
             ]
         }
     },
     "it takes one hour": {
-        "en": "It takes one hour",
-        "fi": "Se kest\u00e4\u00e4 tunnin",
-        "nl": "Het duurt \u00e9\u00e9n uur|Het duurt een uur",
+        "en": "It takes one hour.",
+        "fi": "Se kest\u00e4\u00e4 tunnin.",
+        "nl": "Het duurt \u00e9\u00e9n uur.|Het duurt een uur.",
         "roots": {
             "en": [
                 "1",
                 "hour"
             ],
             "fi": "hour",
             "nl": [
@@ -290,127 +290,127 @@
     },
     "midnight": {
         "level": {
             "A1": "OD",
             "A2": "EP"
         },
         "plural": {
-            "en": "Midnights",
-            "fi": "Keskiy\u00f6t",
-            "nl": "De middernachten"
+            "en": "midnights",
+            "fi": "keskiy\u00f6t",
+            "nl": "de middernachten"
         },
         "roots": "night",
         "singular": {
-            "en": "Midnight",
-            "fi": "Keskiy\u00f6",
-            "nl": "De middernacht"
+            "en": "midnight",
+            "fi": "keskiy\u00f6",
+            "nl": "de middernacht"
         }
     },
     "minute": {
         "level": {
             "A1": [
                 "EP",
                 "KK",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Minutes",
-            "fi": "Minuutit",
-            "nl": "De minuten"
+            "en": "minutes",
+            "fi": "minuutit",
+            "nl": "de minuten"
         },
         "singular": {
-            "en": "Minute",
-            "fi": "Minuutti",
-            "nl": "De minuut"
+            "en": "minute",
+            "fi": "minuutti",
+            "nl": "de minuut"
         }
     },
     "morning": {
         "level": {
             "A1": [
                 "EP",
                 "KK",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Mornings",
-            "fi": "Aamut",
-            "nl": "De ochtenden"
+            "en": "mornings",
+            "fi": "aamut",
+            "nl": "de ochtenden"
         },
         "singular": {
-            "en": "Morning",
-            "fi": "Aamu",
-            "nl": "De ochtend"
+            "en": "morning",
+            "fi": "aamu",
+            "nl": "de ochtend"
         }
     },
     "night": {
         "level": {
             "A1": [
                 "EP",
                 "KK",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Nights",
-            "fi": "Y\u00f6t",
-            "nl": "De nachten"
+            "en": "nights",
+            "fi": "y\u00f6t",
+            "nl": "de nachten"
         },
         "singular": {
-            "en": "Night",
-            "fi": "Y\u00f6",
-            "nl": "De nacht"
+            "en": "night",
+            "fi": "y\u00f6",
+            "nl": "de nacht"
         }
     },
     "noon": {
         "level": {
             "A2": "EP",
             "C1": "OD"
         },
         "plural": {
-            "fi": "Keskip\u00e4iv\u00e4t"
+            "fi": "keskip\u00e4iv\u00e4t"
         },
         "roots": {
             "fi": "day",
             "nl": [
                 "12",
                 "hour",
                 "afternoon"
             ]
         },
         "singular": {
-            "en": "Noon",
-            "fi": "Keskip\u00e4iv\u00e4",
-            "nl": "Twaalf uur 's middags"
+            "en": "noon",
+            "fi": "keskip\u00e4iv\u00e4",
+            "nl": "twaalf uur 's middags"
         }
     },
     "now": {
-        "en": "Now",
-        "fi": "Nyt",
+        "en": "now",
+        "fi": "nyt",
         "level": {
             "A1": [
                 "EP",
                 "KK",
                 "OD"
             ]
         },
-        "nl": "Nu"
+        "nl": "nu"
     },
     "time": {
-        "en": "Time",
-        "fi": "Aika",
+        "en": "time",
+        "fi": "aika",
         "level": {
             "A1": [
                 "EP",
                 "KK",
                 "OD"
             ]
         },
-        "nl": "De tijd"
+        "nl": "de tijd"
     },
     "what time": {
         "en": "What time?",
         "fi": "Mihin aikaan?",
         "nl": "Hoe laat?",
         "roots": {
             "en": [
@@ -452,18 +452,18 @@
             "A1": [
                 "EP",
                 "KK",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Years",
-            "fi": "Vuodet",
-            "nl": "De jaren"
+            "en": "years",
+            "fi": "vuodet",
+            "nl": "de jaren"
         },
         "singular": {
-            "en": "Year",
-            "fi": "Vuosi",
-            "nl": "Het jaar"
+            "en": "year",
+            "fi": "vuosi",
+            "nl": "het jaar"
         }
     }
 }
```

### Comparing `Toisto-0.8.2/src/topics/verbs.json` & `Toisto-0.9.0/src/topics/verbs.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9617472833076134%*

 * *Differences: {"'to be'": "{'declarative': {'affirmative': {'infinitive': {'en': 'to be', 'fi': 'olla', 'nl': "*

 * *            "'zijn'}, 'present tense': {'singular': {'first person': {'fi': 'minä olen|olen', "*

 * *            '\'nl\': \'ik ben\'}, \'second person\': {\'en\': "you are|you\'re;singular", \'fi\': '*

 * *            "'sinä olet|olet', 'nl': 'jij bent|je bent'}, 'third person': {'female': {'en': "*

 * *            '"she is|she\'s", \'fi\': \'hän on;female\', \'nl\': \'zij is|ze is\'}, \'male\': '*

 * *            '{\'en\': "he is […]*

```diff
@@ -1,405 +1,447 @@
 {
     "to be": {
         "declarative": {
             "affirmative": {
                 "infinitive": {
-                    "en": "To be",
-                    "fi": "Olla",
-                    "nl": "Zijn"
+                    "en": "to be",
+                    "fi": "olla",
+                    "nl": "zijn"
                 },
                 "past tense": {
                     "plural": {
                         "first person": {
-                            "en": "We were",
-                            "fi": "Me olimme|Olimme",
-                            "nl": "Wij waren|We waren"
+                            "en": "we were",
+                            "fi": "me olimme|olimme",
+                            "nl": "wij waren|we waren"
                         },
                         "second person": {
-                            "en": "You were;plural",
-                            "fi": "Te olitte|Olitte",
-                            "nl": "Jullie waren"
+                            "en": "you were;plural",
+                            "fi": "te olitte|olitte",
+                            "nl": "jullie waren"
                         },
                         "third person": {
-                            "en": "They were",
-                            "fi": "He olivat",
-                            "nl": "Zij waren|Ze waren"
+                            "en": "they were",
+                            "fi": "he olivat",
+                            "nl": "zij waren|ze waren"
                         }
                     },
                     "singular": {
                         "first person": {
                             "en": "I was",
-                            "fi": "Min\u00e4 olin|Olin",
-                            "nl": "Ik was"
+                            "fi": "min\u00e4 olin|olin",
+                            "nl": "ik was"
                         },
                         "second person": {
-                            "en": "You were;singular",
-                            "fi": "Sin\u00e4 olit|Olit",
-                            "nl": "Jij was|Je was"
+                            "en": "you were;singular",
+                            "fi": "sin\u00e4 olit|olit",
+                            "nl": "jij was|je was"
                         },
                         "third person": {
                             "female": {
-                                "en": "She was",
-                                "fi": "H\u00e4n oli;female",
-                                "nl": "Zij was|Ze was"
+                                "en": "she was",
+                                "fi": "h\u00e4n oli;female",
+                                "nl": "zij was|ze was"
                             },
                             "male": {
-                                "en": "He was",
-                                "fi": "H\u00e4n oli;male",
-                                "nl": "Hij was"
+                                "en": "he was",
+                                "fi": "h\u00e4n oli;male",
+                                "nl": "hij was"
                             }
                         }
                     }
                 },
                 "present tense": {
                     "plural": {
                         "first person": {
-                            "en": "We are|We're",
-                            "fi": "Me olemme|Olemme",
-                            "nl": "Wij zijn|We zijn"
+                            "en": "we are|we're",
+                            "fi": "me olemme|olemme",
+                            "nl": "wij zijn|we zijn"
                         },
                         "second person": {
-                            "en": "You are|You're;plural",
-                            "fi": "Te olette|Olette",
-                            "nl": "Jullie zijn"
+                            "en": "you are|you're;plural",
+                            "fi": "te olette|olette",
+                            "nl": "jullie zijn"
                         },
                         "third person": {
-                            "en": "They are|They're",
-                            "fi": "He ovat",
-                            "nl": "Zij zijn|Ze zijn"
+                            "en": "they are|they're",
+                            "fi": "he ovat",
+                            "nl": "zij zijn|ze zijn"
                         }
                     },
                     "singular": {
                         "first person": {
                             "en": "I am|I'm",
-                            "fi": "Min\u00e4 olen|Olen",
-                            "nl": "Ik ben"
+                            "fi": "min\u00e4 olen|olen",
+                            "nl": "ik ben"
                         },
                         "second person": {
-                            "en": "You are|You're;singular",
-                            "fi": "Sin\u00e4 olet|Olet",
-                            "nl": "Jij bent|Je bent"
+                            "en": "you are|you're;singular",
+                            "fi": "sin\u00e4 olet|olet",
+                            "nl": "jij bent|je bent"
                         },
                         "third person": {
                             "female": {
-                                "en": "She is|She's",
-                                "fi": "H\u00e4n on;female",
-                                "nl": "Zij is|Ze is"
+                                "en": "she is|she's",
+                                "fi": "h\u00e4n on;female",
+                                "nl": "zij is|ze is"
                             },
                             "male": {
-                                "en": "He is|He's",
-                                "fi": "H\u00e4n on;male",
-                                "nl": "Hij is"
+                                "en": "he is|he's",
+                                "fi": "h\u00e4n on;male",
+                                "nl": "hij is"
                             }
                         }
                     }
                 }
             },
             "negative": {
                 "past tense": {
                     "plural": {
                         "first person": {
-                            "en": "We were not|We weren't",
-                            "fi": "Me emme olleet|Emme olleet",
-                            "nl": "Wij waren niet|We waren niet"
+                            "en": "we were not|we weren't",
+                            "fi": "me emme olleet|emme olleet",
+                            "nl": [
+                                "wij waren niet|we waren niet",
+                                "wij waren geen|we waren geen"
+                            ]
                         },
                         "second person": {
-                            "en": "You were not|You weren't;plural",
-                            "fi": "Te ette olleet|Ette olleet",
-                            "nl": "Jullie waren niet"
+                            "en": "you were not|you weren't;plural",
+                            "fi": "te ette olleet|ette olleet",
+                            "nl": [
+                                "jullie waren niet",
+                                "jullie waren geen"
+                            ]
                         },
                         "third person": {
-                            "en": "They were not|They weren't",
-                            "fi": "He eiv\u00e4t olleet",
-                            "nl": "Zij waren niet|Ze waren niet"
+                            "en": "they were not|they weren't",
+                            "fi": "he eiv\u00e4t olleet",
+                            "nl": [
+                                "zij waren niet|ze waren niet",
+                                "zij waren geen|ze waren geen"
+                            ]
                         }
                     },
                     "singular": {
                         "first person": {
                             "en": "I was not|I wasn't",
-                            "fi": "Min\u00e4 en ollut|En ollut",
-                            "nl": "Ik was niet"
+                            "fi": "min\u00e4 en ollut|en ollut",
+                            "nl": [
+                                "ik was niet",
+                                "ik was geen"
+                            ]
                         },
                         "second person": {
-                            "en": "You were not|You weren't;singular",
-                            "fi": "Sin\u00e4 et ollut|Et ollut",
-                            "nl": "Jij was niet|Je was niet"
+                            "en": "you were not|you weren't;singular",
+                            "fi": "sin\u00e4 et ollut|et ollut",
+                            "nl": [
+                                "jij was niet|je was niet",
+                                "jij was geen|je was geen"
+                            ]
                         },
                         "third person": {
                             "female": {
-                                "en": "She was not|She wasn't",
-                                "fi": "H\u00e4n ei ollut;female",
-                                "nl": "Zij was niet|Ze was niet"
+                                "en": "she was not|she wasn't",
+                                "fi": "h\u00e4n ei ollut;female",
+                                "nl": [
+                                    "zij was niet|ze was niet",
+                                    "zij was geen|ze was geen"
+                                ]
                             },
                             "male": {
-                                "en": "He was not|He wasn't",
-                                "fi": "H\u00e4n ei ollut;male",
-                                "nl": "Hij was niet"
+                                "en": "he was not|he wasn't",
+                                "fi": "h\u00e4n ei ollut;male",
+                                "nl": [
+                                    "hij was niet",
+                                    "hij was geen"
+                                ]
                             }
                         }
                     }
                 },
                 "present tense": {
                     "plural": {
                         "first person": {
-                            "en": "We are not|We're not|We aren't",
-                            "fi": "Me emme ole|Emme ole",
-                            "nl": "Wij zijn niet|We zijn niet"
+                            "en": "we are not|we're not|we aren't",
+                            "fi": "me emme ole|emme ole",
+                            "nl": [
+                                "wij zijn niet|we zijn niet",
+                                "wij zijn geen|we zijn geen"
+                            ]
                         },
                         "second person": {
-                            "en": "You are not|You're not|You aren't;plural",
-                            "fi": "Te ette ole|Ette ole",
-                            "nl": "Jullie zijn niet"
+                            "en": "you are not|you're not|you aren't;plural",
+                            "fi": "te ette ole|ette ole",
+                            "nl": [
+                                "jullie zijn niet",
+                                "jullie zijn geen"
+                            ]
                         },
                         "third person": {
-                            "en": "They are not|They're not|They aren't",
-                            "fi": "He eiv\u00e4t ole",
-                            "nl": "Zij zijn nietl|Ze zijn nietl"
+                            "en": "they are not|they're not|they aren't",
+                            "fi": "he eiv\u00e4t ole",
+                            "nl": [
+                                "zij zijn nietl|ze zijn nietl",
+                                "zij zijn geen|ze zijn geen"
+                            ]
                         }
                     },
                     "singular": {
                         "first person": {
                             "en": "I am not|I'm not",
-                            "fi": "Min\u00e4 en ole|En ole",
-                            "nl": "Ik ben niet"
+                            "fi": "min\u00e4 en ole|en ole",
+                            "nl": [
+                                "ik ben niet",
+                                "ik ben geen"
+                            ]
                         },
                         "second person": {
-                            "en": "You are not|You're not;singular",
-                            "fi": "Sin\u00e4 et ole|Et ole",
-                            "nl": "Jij bent niet|Je bent niet"
+                            "en": "you are not|you're not;singular",
+                            "fi": "sin\u00e4 et ole|et ole",
+                            "nl": [
+                                "jij bent niet|je bent niet",
+                                "jij bent geen|je bent geen"
+                            ]
                         },
                         "third person": {
                             "female": {
-                                "en": "She is not|She's not|She isn't",
-                                "fi": "H\u00e4n ei ole;female",
-                                "nl": "Zij is niet|Ze is niet"
+                                "en": "she is not|she's not|she isn't",
+                                "fi": "h\u00e4n ei ole;female",
+                                "nl": [
+                                    "zij is niet|ze is niet",
+                                    "zij is geen|ze is geen"
+                                ]
                             },
                             "male": {
-                                "en": "He is not|He's not|He isn't",
-                                "fi": "H\u00e4n ei ole;male",
-                                "nl": "Hij is niet"
+                                "en": "he is not|he's not|he isn't",
+                                "fi": "h\u00e4n ei ole;male",
+                                "nl": [
+                                    "hij is niet",
+                                    "hij is geen"
+                                ]
                             }
                         }
                     }
                 }
             }
         },
         "interrogative": {
             "affirmative": {
                 "past tense": {
                     "plural": {
                         "first person": {
-                            "en": "Were we?",
-                            "fi": "Olimmeko me?|Olimmeko?",
-                            "nl": "Waren wij?|Waren we?"
+                            "en": "were we?",
+                            "fi": "olimmeko me?|olimmeko?",
+                            "nl": "waren wij?|waren we?"
                         },
                         "second person": {
-                            "en": "Were you?;plural",
-                            "fi": "Olitteko te?|Olitteko?",
-                            "nl": "Waren jullie?"
+                            "en": "were you?;plural",
+                            "fi": "olitteko te?|olitteko?",
+                            "nl": "waren jullie?"
                         },
                         "third person": {
-                            "en": "Were they?",
-                            "fi": "Olivatko he?",
-                            "nl": "Waren zij?|Waren ze?"
+                            "en": "were they?",
+                            "fi": "olivatko he?",
+                            "nl": "waren zij?|waren ze?"
                         }
                     },
                     "singular": {
                         "first person": {
-                            "en": "Was I?",
-                            "fi": "Olinko min\u00e4?|Olinko?",
-                            "nl": "Was ik?"
+                            "en": "was I?",
+                            "fi": "olinko min\u00e4?|olinko?",
+                            "nl": "was ik?"
                         },
                         "second person": {
-                            "en": "Were you?;singular",
-                            "fi": "Olitko sin\u00e4?|Olitko?",
-                            "nl": "Was jij?|Was je?"
+                            "en": "were you?;singular",
+                            "fi": "olitko sin\u00e4?|olitko?",
+                            "nl": "was jij?|was je?"
                         },
                         "third person": {
                             "female": {
-                                "en": "Was she?",
-                                "fi": "Oliko h\u00e4n?;female",
-                                "nl": "Was zij?|Was ze?"
+                                "en": "was she?",
+                                "fi": "oliko h\u00e4n?;female",
+                                "nl": "was zij?|was ze?"
                             },
                             "male": {
-                                "en": "Was he?",
-                                "fi": "Oliko h\u00e4n?;male",
-                                "nl": "Was hij?"
+                                "en": "was he?",
+                                "fi": "oliko h\u00e4n?;male",
+                                "nl": "was hij?"
                             }
                         }
                     }
                 },
                 "present tense": {
                     "plural": {
                         "first person": {
-                            "en": "Are we?",
-                            "fi": "Olemmeko me?|Olemmeko?",
-                            "nl": "Zijn wij?|Zijn we?"
+                            "en": "are we?",
+                            "fi": "olemmeko me?|olemmeko?",
+                            "nl": "zijn wij?|zijn we?"
                         },
                         "second person": {
-                            "en": "Are you?;plural",
-                            "fi": "Oletteko te?|Oletteko?",
-                            "nl": "Zijn jullie?"
+                            "en": "are you?;plural",
+                            "fi": "oletteko te?|oletteko?",
+                            "nl": "zijn jullie?"
                         },
                         "third person": {
-                            "en": "Are they?",
-                            "fi": "Ovatko he?",
-                            "nl": "Zijn zij?|Zijn ze?"
+                            "en": "are they?",
+                            "fi": "ovatko he?",
+                            "nl": "zijn zij?|zijn ze?"
                         }
                     },
                     "singular": {
                         "first person": {
-                            "en": "Am I?",
-                            "fi": "Olenko min\u00e4?|Olenko?",
-                            "nl": "Ben ik?"
+                            "en": "am I?",
+                            "fi": "olenko min\u00e4?|olenko?",
+                            "nl": "ben ik?"
                         },
                         "second person": {
-                            "en": "Are you?;singular",
-                            "fi": "Oletko sin\u00e4?|Oletko?",
-                            "nl": "Ben jij?|Ben je?"
+                            "en": "are you?;singular",
+                            "fi": "oletko sin\u00e4?|oletko?",
+                            "nl": "ben jij?|ben je?"
                         },
                         "third person": {
                             "female": {
-                                "en": "Is she?",
-                                "fi": "Onko h\u00e4n?;female",
-                                "nl": "Is zij?|Is ze?"
+                                "en": "is she?",
+                                "fi": "onko h\u00e4n?;female",
+                                "nl": "is zij?|is ze?"
                             },
                             "male": {
-                                "en": "Is he?",
-                                "fi": "Onko h\u00e4n?;male",
-                                "nl": "Is hij?"
+                                "en": "is he?",
+                                "fi": "onko h\u00e4n?;male",
+                                "nl": "is hij?"
                             }
                         }
                     }
                 }
             },
             "negative": {
                 "past tense": {
                     "plural": {
                         "first person": {
-                            "en": "Were we not?|Waren't we?",
-                            "fi": "Emmek\u00f6 me olleet?|Emmok\u00f6 olleet?",
+                            "en": "were we not?|weren't we?",
+                            "fi": "emmek\u00f6 me olleet?|emmok\u00f6 olleet?",
                             "nl": [
-                                "Waren wij niet?|Waren we niet?",
-                                "Waren we geen?|Waren we geen?"
+                                "waren wij niet?|waren we niet?",
+                                "waren we geen?|waren we geen?"
                             ]
                         },
                         "second person": {
-                            "en": "Were you not?|Weren't you?;plural",
-                            "fi": "Ettek\u00f6 te olleet?|Ettek\u00f6 olleet?",
+                            "en": "were you not?|weren't you?;plural",
+                            "fi": "ettek\u00f6 te olleet?|ettek\u00f6 olleet?",
                             "nl": [
-                                "Waren jullie niet?",
-                                "Waren jullie geen?"
+                                "waren jullie niet?",
+                                "waren jullie geen?"
                             ]
                         },
                         "third person": {
-                            "en": "Were they not?|Weren't they?",
-                            "fi": "Eiv\u00e4tk\u00f6 he olleet?",
+                            "en": "were they not?|weren't they?",
+                            "fi": "eiv\u00e4tk\u00f6 he olleet?",
                             "nl": [
-                                "Waren zij niet?|Waren ze niet?",
-                                "Waren zij geen?|Waren ze geen?"
+                                "waren zij niet?|waren ze niet?",
+                                "waren zij geen?|waren ze geen?"
                             ]
                         }
                     },
                     "singular": {
                         "first person": {
-                            "en": "Was I not?|Wasn't I",
-                            "fi": "Enk\u00f6 min\u00e4 ole?|Enk\u00f6 ole?",
+                            "en": "was I not?|wasn't I",
+                            "fi": "enk\u00f6 min\u00e4 ole?|enk\u00f6 ole?",
                             "nl": [
-                                "Was ik niet?",
-                                "Was ik geen?"
+                                "was ik niet?",
+                                "was ik geen?"
                             ]
                         },
                         "second person": {
-                            "en": "Were you not?|Weren't you?;singular",
-                            "fi": "Etk\u00f6 sin\u00e4 ollut?|Etk\u00f6 ollut?",
+                            "en": "were you not?|weren't you?;singular",
+                            "fi": "etk\u00f6 sin\u00e4 ollut?|etk\u00f6 ollut?",
                             "nl": [
-                                "Was jij niet?|Was je niet?",
-                                "Was jij geen?|Was je geen?"
+                                "was jij niet?|was je niet?",
+                                "was jij geen?|was je geen?"
                             ]
                         },
                         "third person": {
                             "female": {
-                                "en": "Was she not?|Wasn't she?",
-                                "fi": "Eik\u00f6 h\u00e4n ollut?;female",
+                                "en": "was she not?|wasn't she?",
+                                "fi": "eik\u00f6 H\u00c4n ollut?;female",
                                 "nl": [
-                                    "Was zij niet?|Was ze niet?",
-                                    "Was zij geen?|Was ze geen?"
+                                    "was zij niet?|was ze niet?",
+                                    "was zij geen?|was ze geen?"
                                 ]
                             },
                             "male": {
-                                "en": "Was he not?",
-                                "fi": "Eik\u00f6 h\u00e4n ollut?;male",
+                                "en": "was he not?",
+                                "fi": "eik\u00f6 h\u00e4n ollut?;male",
                                 "nl": [
-                                    "Was hij niet?",
-                                    "Was hij geen?"
+                                    "was hij niet?",
+                                    "was hij geen?"
                                 ]
                             }
                         }
                     }
                 },
                 "present tense": {
                     "plural": {
                         "first person": {
-                            "en": "Are we not?",
-                            "fi": "Emmek\u00f6 me ole?|Emmok\u00f6 ole?",
+                            "en": "are we not?",
+                            "fi": "emmek\u00f6 me ole?|emmok\u00f6 ole?",
                             "nl": [
-                                "Zijn wij niet?|Zijn we niet?",
-                                "Zijn we geen?|Zijn we geen?"
+                                "zijn wij niet?|zijn we niet?",
+                                "zijn we geen?|zijn we geen?"
                             ]
                         },
                         "second person": {
-                            "en": "Are you not?;plural",
-                            "fi": "Ettek\u00f6 te ole?|Ettek\u00f6 ole?",
+                            "en": "are you not?;plural",
+                            "fi": "ettek\u00f6 te ole?|ettek\u00f6 ole?",
                             "nl": [
-                                "Zijn jullie niet?",
-                                "Zijn jullie geen?"
+                                "zijn jullie niet?",
+                                "zijn jullie geen?"
                             ]
                         },
                         "third person": {
-                            "en": "Are they not?",
-                            "fi": "Eiv\u00e4tk\u00f6 he ole?",
+                            "en": "are they not?",
+                            "fi": "eiv\u00e4tk\u00f6 he ole?",
                             "nl": [
-                                "Zijn zij niet?|Zijn ze niet?",
-                                "Zijn zij geen?|Zijn ze geen?"
+                                "zijn zij niet?|zijn ze niet?",
+                                "zijn zij geen?|zijn ze geen?"
                             ]
                         }
                     },
                     "singular": {
                         "first person": {
-                            "en": "Am I not?",
-                            "fi": "Enk\u00f6 min\u00e4 ole?|Enk\u00f6 ole?",
+                            "en": "am I not?",
+                            "fi": "enk\u00f6 min\u00e4 ole?|enk\u00f6 ole?",
                             "nl": [
-                                "Ben ik niet?",
-                                "Ben ik geen?"
+                                "ben ik niet?",
+                                "ben ik geen?"
                             ]
                         },
                         "second person": {
-                            "en": "Are you not?;singular",
-                            "fi": "Etk\u00f6 sin\u00e4 ole?|Etk\u00f6 ole?",
+                            "en": "are you not?;singular",
+                            "fi": "etk\u00f6 sin\u00e4 ole?|etk\u00f6 ole?",
                             "nl": [
-                                "Ben jij niet?|Ben je niet?",
-                                "Ben jij geen?|Ben je geen?"
+                                "ben jij niet?|ben je niet?",
+                                "ben jij geen?|ben je geen?"
                             ]
                         },
                         "third person": {
                             "female": {
-                                "en": "Is she not?",
-                                "fi": "Eik\u00f6 h\u00e4n ole?;female",
+                                "en": "is she not?",
+                                "fi": "eik\u00f6 h\u00e4n ole?;female",
                                 "nl": [
-                                    "Is zij niet?|Is ze niet?",
-                                    "Is zij geen?|Is ze geen?"
+                                    "is zij niet?|is ze niet?",
+                                    "is zij geen?|is ze geen?"
                                 ]
                             },
                             "male": {
-                                "en": "Is he not?",
-                                "fi": "Eik\u00f6 h\u00e4n ole?;male",
+                                "en": "is he not?",
+                                "fi": "eik\u00f6 h\u00e4n ole?;male",
                                 "nl": [
-                                    "Is hij niet?",
-                                    "Is hij geen?"
+                                    "is hij niet?",
+                                    "is hij geen?"
                                 ]
                             }
                         }
                     }
                 }
             }
         },
@@ -409,750 +451,792 @@
                 "KK",
                 "OD"
             ]
         }
     },
     "to come": {
         "infinitive": {
-            "en": "To come",
-            "fi": "Tulla",
-            "nl": "Komen"
+            "en": "to come",
+            "fi": "tulla",
+            "nl": "komen"
         },
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
         "past tense": {
             "plural": {
                 "first person": {
-                    "en": "We came",
-                    "fi": "Me tulimme|Tulimme",
-                    "nl": "Wij kwamen|We kwamen"
+                    "en": "we came",
+                    "fi": "me tulimme|tulimme",
+                    "nl": "wij kwamen|we kwamen"
                 },
                 "second person": {
-                    "en": "You came;plural",
-                    "fi": "Te tulitte|Tulitte",
-                    "nl": "Jullie kwamen"
+                    "en": "you came;plural",
+                    "fi": "te tulitte|Tulitte",
+                    "nl": "jullie kwamen"
                 },
                 "third person": {
-                    "en": "They came",
-                    "fi": "He tulivat",
-                    "nl": "Zij kwamen|Ze kwamen"
+                    "en": "they came",
+                    "fi": "he tulivat",
+                    "nl": "zij kwamen|ze kwamen"
                 }
             },
             "singular": {
                 "first person": {
                     "en": "I came",
-                    "fi": "Min\u00e4 tulin|Tulin",
-                    "nl": "Ik kwam"
+                    "fi": "min\u00e4 tulin|tulin",
+                    "nl": "ik kwam"
                 },
                 "second person": {
-                    "en": "You came;singular",
-                    "fi": "Sin\u00e4 tulit|Tulit",
-                    "nl": "Jij kwam|Je kwam"
+                    "en": "you came;singular",
+                    "fi": "sin\u00e4 tulit|tulit",
+                    "nl": "jij kwam|je kwam"
                 },
                 "third person": {
                     "female": {
-                        "en": "She came",
-                        "fi": "H\u00e4n tuli;female",
-                        "nl": "Zij kwam|Ze kwam"
+                        "en": "she came",
+                        "fi": "h\u00e4n tuli;female",
+                        "nl": "zij kwam|ze kwam"
                     },
                     "male": {
-                        "en": "He came",
-                        "fi": "H\u00e4n tuli;male",
-                        "nl": "Hij kwam"
+                        "en": "he came",
+                        "fi": "h\u00e4n tuli;male",
+                        "nl": "hij kwam"
                     }
                 }
             }
         },
         "present tense": {
             "plural": {
                 "first person": {
-                    "en": "We come",
-                    "fi": "Me tulemme|Tulemme",
-                    "nl": "Wij komen|We komen"
+                    "en": "we come",
+                    "fi": "me tulemme|tulemme",
+                    "nl": "wij komen|we komen"
                 },
                 "second person": {
-                    "en": "You come;plural",
-                    "fi": "Te tulette|Tulette",
-                    "nl": "Jullie komen"
+                    "en": "you come;plural",
+                    "fi": "te tulette|tulette",
+                    "nl": "jullie komen"
                 },
                 "third person": {
-                    "en": "They come",
-                    "fi": "He tulevat",
-                    "nl": "Zij komen|Ze komen"
+                    "en": "they come",
+                    "fi": "he tulevat",
+                    "nl": "zij komen|ze Komen"
                 }
             },
             "singular": {
                 "first person": {
                     "en": "I come",
-                    "fi": "Min\u00e4 tulen|Tulen",
-                    "nl": "Ik kom"
+                    "fi": "min\u00e4 tulen|tulen",
+                    "nl": "ik kom"
                 },
                 "second person": {
-                    "en": "You come;singular",
-                    "fi": "Sin\u00e4 tulet|Tulet",
-                    "nl": "Jij komt|Je komt"
+                    "en": "you come;singular",
+                    "fi": "sin\u00e4 tulet|tulet",
+                    "nl": "jij komt|je komt"
                 },
                 "third person": {
                     "female": {
-                        "en": "She comes",
-                        "fi": "H\u00e4n tulee;female",
-                        "nl": "Zij komt|Ze komt"
+                        "en": "she comes",
+                        "fi": "h\u00e4n tulee;female",
+                        "nl": "zij komt|ze komt"
                     },
                     "male": {
-                        "en": "He comes",
-                        "fi": "H\u00e4n tulee;male",
-                        "nl": "Hij komt"
+                        "en": "he comes",
+                        "fi": "h\u00e4n tulee;male",
+                        "nl": "hij komt"
                     }
                 }
             }
         }
     },
     "to eat": {
         "infinitive": {
-            "en": "To eat",
-            "fi": "Sy\u00f6d\u00e4",
-            "nl": "Eten"
+            "en": "to eat",
+            "fi": "sy\u00f6d\u00e4",
+            "nl": "eten"
         },
         "level": {
             "A1": [
                 "EP",
                 "KK",
                 "OD"
             ]
         },
         "past tense": {
             "plural": {
                 "first person": {
-                    "en": "We ate",
-                    "fi": "Me s\u00f6imme|S\u00f6imme",
-                    "nl": "Wij aten|We aten"
+                    "en": "we ate",
+                    "fi": "me s\u00f6imme|s\u00f6imme",
+                    "nl": "wij aten|we aten"
                 },
                 "second person": {
-                    "en": "You ate;plural",
-                    "fi": "Te s\u00f6itte|S\u00f6itte",
-                    "nl": "Jullie aten"
+                    "en": "you ate;plural",
+                    "fi": "te s\u00f6itte|s\u00f6itte",
+                    "nl": "jullie aten"
                 },
                 "third person": {
-                    "en": "They ate",
-                    "fi": "He s\u00f6iv\u00e4t",
-                    "nl": "Zij aten|Ze aten"
+                    "en": "they ate",
+                    "fi": "he s\u00f6iv\u00e4t",
+                    "nl": "zij aten|ze aten"
                 }
             },
             "singular": {
                 "first person": {
                     "en": "I ate",
-                    "fi": "Min\u00e4 s\u00f6in|S\u00f6in",
-                    "nl": "Ik at"
+                    "fi": "min\u00e4 s\u00f6in|s\u00f6in",
+                    "nl": "ik at"
                 },
                 "second person": {
-                    "en": "You ate;singular",
-                    "fi": "Sin\u00e4 s\u00f6it|S\u00f6it",
-                    "nl": "Jij at|Je at"
+                    "en": "you ate;singular",
+                    "fi": "sin\u00e4 s\u00f6it|s\u00f6it",
+                    "nl": "jij at|je at"
                 },
                 "third person": {
                     "female": {
-                        "en": "She ate",
-                        "fi": "H\u00e4n s\u00f6i;female",
-                        "nl": "Zij at|Ze at"
+                        "en": "she ate",
+                        "fi": "h\u00e4n s\u00f6i;female",
+                        "nl": "zij at|ze at"
                     },
                     "male": {
-                        "en": "He ate",
-                        "fi": "H\u00e4n s\u00f6i;male",
-                        "nl": "Hij at"
+                        "en": "he ate",
+                        "fi": "h\u00e4n s\u00f6i;male",
+                        "nl": "hij at"
                     }
                 }
             }
         },
         "present tense": {
             "plural": {
                 "first person": {
-                    "en": "We eat",
-                    "fi": "Me sy\u00f6mme|Sy\u00f6mme",
-                    "nl": "Wij eten|We eten"
+                    "en": "we eat",
+                    "fi": "me sy\u00f6mme|sy\u00f6mme",
+                    "nl": "wij eten|we eten"
                 },
                 "second person": {
-                    "en": "You eat;plural",
-                    "fi": "Te sy\u00f6tte|Sy\u00f6tte",
-                    "nl": "Jullie eten"
+                    "en": "you eat;plural",
+                    "fi": "te sy\u00f6tte|sy\u00f6tte",
+                    "nl": "jullie eten"
                 },
                 "third person": {
-                    "en": "They eat",
-                    "fi": "He sy\u00f6v\u00e4t",
-                    "nl": "Zij eten|Ze eten"
+                    "en": "they eat",
+                    "fi": "he sy\u00f6v\u00e4t",
+                    "nl": "zij eten|ze eten"
                 }
             },
             "singular": {
                 "first person": {
                     "en": "I eat",
-                    "fi": "Min\u00e4 sy\u00f6n|Sy\u00f6n",
-                    "nl": "Ik eet"
+                    "fi": "min\u00e4 sy\u00f6n|sy\u00f6n",
+                    "nl": "ik eet"
                 },
                 "second person": {
-                    "en": "You eat;singular",
-                    "fi": "Sin\u00e4 sy\u00f6t|Sy\u00f6t",
-                    "nl": "Jij eet|Je eet"
+                    "en": "you eat;singular",
+                    "fi": "sin\u00e4 sy\u00f6t|sy\u00f6t",
+                    "nl": "jij eet|je eet"
                 },
                 "third person": {
                     "female": {
-                        "en": "She eats",
-                        "fi": "H\u00e4n sy\u00f6;female",
-                        "nl": "Zij eet|Ze eet"
+                        "en": "she eats",
+                        "fi": "h\u00e4n sy\u00f6;female",
+                        "nl": "zij eet|ze eet"
                     },
                     "male": {
-                        "en": "He eats",
-                        "fi": "H\u00e4n sy\u00f6;male",
-                        "nl": "Hij eet"
+                        "en": "he eats",
+                        "fi": "h\u00e4n sy\u00f6;male",
+                        "nl": "hij eet"
                     }
                 }
             }
         }
     },
     "to go": {
         "infinitive": {
-            "en": "To go",
-            "fi": "Menn\u00e4",
-            "nl": "Gaan"
+            "en": "to go",
+            "fi": "menn\u00e4",
+            "nl": "gaan"
         },
         "level": {
             "A1": [
                 "EP",
                 "KK",
                 "OD"
             ]
         },
         "past tense": {
             "plural": {
                 "first person": {
-                    "en": "We went",
-                    "fi": "Me menimme|Menimme",
-                    "nl": "Wij gingen|We gingen"
+                    "en": "we went",
+                    "fi": "me menimme|menimme",
+                    "nl": "wij gingen|we gingen"
                 },
                 "second person": {
-                    "en": "You went;plural",
-                    "fi": "Te menitte|Menitte",
-                    "nl": "Jullie gingen"
+                    "en": "you went;plural",
+                    "fi": "te menitte|menitte",
+                    "nl": "jullie gingen"
                 },
                 "third person": {
-                    "en": "They went",
-                    "fi": "He meniv\u00e4t",
-                    "nl": "Zij gingen|Ze gingen"
+                    "en": "they went",
+                    "fi": "he meniv\u00e4t",
+                    "nl": "zij gingen|ze gingen"
                 }
             },
             "singular": {
                 "first person": {
                     "en": "I went",
-                    "fi": "Min\u00e4 menin|Menin",
-                    "nl": "Ik ging"
+                    "fi": "min\u00e4 menin|menin",
+                    "nl": "ik ging"
                 },
                 "second person": {
-                    "en": "You went;singular",
-                    "fi": "Sin\u00e4 menit|Menit",
-                    "nl": "Jij ging|Je ging"
+                    "en": "you went;singular",
+                    "fi": "sin\u00e4 menit|menit",
+                    "nl": "jij ging|je ging"
                 },
                 "third person": {
                     "female": {
-                        "en": "She went",
-                        "fi": "H\u00e4n meni;female",
-                        "nl": "Zij ging|Ze ging"
+                        "en": "she went",
+                        "fi": "h\u00e4n meni;female",
+                        "nl": "zij ging|ze ging"
                     },
                     "male": {
-                        "en": "He went",
-                        "fi": "H\u00e4n meni;male",
-                        "nl": "Hij ging"
+                        "en": "he went",
+                        "fi": "h\u00e4n meni;male",
+                        "nl": "hij ging"
                     }
                 }
             }
         },
         "present tense": {
             "plural": {
                 "first person": {
-                    "en": "We go",
-                    "fi": "Me menemme|Menemme",
-                    "nl": "Wij gaan|We gaan"
+                    "en": "we go",
+                    "fi": "me menemme|menemme",
+                    "nl": "wij gaan|we gaan"
                 },
                 "second person": {
-                    "en": "You go;plural",
-                    "fi": "Te menette|Menette",
-                    "nl": "Jullie gaan"
+                    "en": "you go;plural",
+                    "fi": "te menette|menette",
+                    "nl": "jullie gaan"
                 },
                 "third person": {
-                    "en": "They go",
-                    "fi": "He menev\u00e4t",
-                    "nl": "Zij gaan|Ze gaan"
+                    "en": "they go",
+                    "fi": "he menev\u00e4t",
+                    "nl": "zij gaan|ze gaan"
                 }
             },
             "singular": {
                 "first person": {
                     "en": "I go",
-                    "fi": "Min\u00e4 menen|Menen",
-                    "nl": "Ik ga"
+                    "fi": "min\u00e4 menen|menen",
+                    "nl": "ik ga"
                 },
                 "second person": {
-                    "en": "You go;singular",
-                    "fi": "Sin\u00e4 menet|Menet",
-                    "nl": "Jij gaat|Je gaat"
+                    "en": "you go;singular",
+                    "fi": "sin\u00e4 menet|menet",
+                    "nl": "jij gaat|je gaat"
                 },
                 "third person": {
                     "female": {
-                        "en": "She goes",
-                        "fi": "H\u00e4n menee;female",
-                        "nl": "Zij gaat|Ze gaat"
+                        "en": "she goes",
+                        "fi": "h\u00e4n menee;female",
+                        "nl": "zij gaat|ze gaat"
                     },
                     "male": {
-                        "en": "He goes",
-                        "fi": "H\u00e4n menee;male",
-                        "nl": "Hij gaat"
+                        "en": "he goes",
+                        "fi": "h\u00e4n menee;male",
+                        "nl": "hij gaat"
                     }
                 }
             }
         }
     },
     "to have": {
         "declarative": {
             "affirmative": {
                 "infinitive": {
-                    "en": "To have",
-                    "fi": "Olla;omistaa",
-                    "nl": "Hebben"
+                    "en": "to have",
+                    "fi": "olla;omistaa",
+                    "nl": "hebben"
                 },
                 "past tense": {
                     "plural": {
                         "first person": {
-                            "en": "We had",
-                            "fi": "Meill\u00e4 oli",
-                            "nl": "Wij hadden|We hadden"
+                            "en": "we had",
+                            "fi": "meill\u00e4 oli",
+                            "nl": "wij hadden|we hadden"
                         },
                         "second person": {
-                            "en": "You had;plural",
-                            "fi": "Teill\u00e4 oli",
-                            "nl": "Jullie hadden"
+                            "en": "you had;plural",
+                            "fi": "teill\u00e4 oli",
+                            "nl": "jullie hadden"
                         },
                         "third person": {
-                            "en": "They had",
-                            "fi": "Heill\u00e4 oli",
-                            "nl": "Zij hadden|Ze hadden"
+                            "en": "they had",
+                            "fi": "heill\u00e4 oli",
+                            "nl": "zij hadden|ze hadden"
                         }
                     },
                     "singular": {
                         "first person": {
                             "en": "I had",
-                            "fi": "Minulla oli",
-                            "nl": "Ik had"
+                            "fi": "minulla oli",
+                            "nl": "ik had"
                         },
                         "second person": {
-                            "en": "You had;singular",
-                            "fi": "Sinulla oli",
-                            "nl": "Jij had|Je had"
+                            "en": "you had;singular",
+                            "fi": "sinulla oli",
+                            "nl": "jij had|je had"
                         },
                         "third person": {
                             "female": {
-                                "en": "She had",
-                                "fi": "H\u00e4nell\u00e4 oli;female",
-                                "nl": "Zij had|Ze had"
+                                "en": "she had",
+                                "fi": "h\u00e4nell\u00e4 oli;female",
+                                "nl": "zij had|ze had"
                             },
                             "male": {
-                                "en": "He had",
-                                "fi": "H\u00e4nell\u00e4 oli;male",
-                                "nl": "Hij had"
+                                "en": "he had",
+                                "fi": "h\u00e4nell\u00e4 oli;male",
+                                "nl": "hij had"
                             }
                         }
                     }
                 },
                 "present tense": {
                     "plural": {
                         "first person": {
-                            "en": "We have|We've",
-                            "fi": "Meill\u00e4 on",
-                            "nl": "Wij hebben|We hebben"
+                            "en": "we have|we've",
+                            "fi": "meill\u00e4 on",
+                            "nl": "wij hebben|we hebben"
                         },
                         "second person": {
-                            "en": "You have|You've;plural",
-                            "fi": "Teill\u00e4 on",
-                            "nl": "Jullie hebben"
+                            "en": "you have|you've;plural",
+                            "fi": "teill\u00e4 on",
+                            "nl": "jullie hebben"
                         },
                         "third person": {
-                            "en": "They have|They've",
-                            "fi": "Heill\u00e4 on",
-                            "nl": "Zij hebben|Ze hebben"
+                            "en": "they have|they've",
+                            "fi": "heill\u00e4 on",
+                            "nl": "zij hebben|ze hebben"
                         }
                     },
                     "singular": {
                         "first person": {
                             "en": "I have|I've",
-                            "fi": "Minulla on",
-                            "nl": "Ik heb"
+                            "fi": "minulla on",
+                            "nl": "ik heb"
                         },
                         "second person": {
-                            "en": "You have|You've;singular",
-                            "fi": "Sinulla on",
-                            "nl": "Jij hebt|Je hebt"
+                            "en": "you have|you've;singular",
+                            "fi": "sinulla on",
+                            "nl": "jij hebt|je hebt"
                         },
                         "third person": {
                             "female": {
-                                "en": "She has|She's",
-                                "fi": "H\u00e4nell\u00e4 on;female",
-                                "nl": "Zij heeft|Ze heeft"
+                                "en": "she has|she's",
+                                "fi": "h\u00e4nell\u00e4 on;female",
+                                "nl": "zij heeft|ze heeft"
                             },
                             "male": {
-                                "en": "He has|He's",
-                                "fi": "H\u00e4nell\u00e4 on;male",
-                                "nl": "Hij heeft"
+                                "en": "he has|he's",
+                                "fi": "h\u00e4nell\u00e4 on;male",
+                                "nl": "hij heeft"
                             }
                         }
                     }
                 }
             },
             "negative": {
                 "past tense": {
                     "plural": {
                         "first person": {
-                            "en": "We had not|We hadn't",
-                            "fi": "Meill\u00e4 ei ollut",
-                            "nl": "Wij hadden niet|We hadden niet"
+                            "en": "we had not|we hadn't",
+                            "fi": "meill\u00e4 ei ollut",
+                            "nl": [
+                                "wij hadden niet|we hadden niet",
+                                "wij hadden geen|we hadden geen"
+                            ]
                         },
                         "second person": {
-                            "en": "You had not|You hadn't;plural",
-                            "fi": "Teill\u00e4 ei ollut",
-                            "nl": "Jullie hadden niet"
+                            "en": "you had not|you hadn't;plural",
+                            "fi": "teill\u00e4 ei ollut",
+                            "nl": [
+                                "jullie hadden niet",
+                                "jullie hadden geen"
+                            ]
                         },
                         "third person": {
-                            "en": "They had not|They hadn't",
-                            "fi": "Heill\u00e4 ei ollut",
-                            "nl": "Zij hadden niet|Ze hadden niet"
+                            "en": "they had not|they hadn't",
+                            "fi": "heill\u00e4 ei ollut",
+                            "nl": [
+                                "zij hadden niet|ze hadden niet",
+                                "zij hadden geen|ze hadden geen"
+                            ]
                         }
                     },
                     "singular": {
                         "first person": {
                             "en": "I had not|I hadn't",
-                            "fi": "Minulla ei ollut",
-                            "nl": "Ik had niet"
+                            "fi": "minulla ei ollut",
+                            "nl": [
+                                "ik had niet",
+                                "ik had geen"
+                            ]
                         },
                         "second person": {
-                            "en": "You had not|You hadn't;singular",
-                            "fi": "Sinulla ei ollut",
-                            "nl": "Jij had niet|Je had niet"
+                            "en": "you had not|you hadn't;singular",
+                            "fi": "sinulla ei ollut",
+                            "nl": [
+                                "jij had niet|je had niet",
+                                "jij had geen|je had geen"
+                            ]
                         },
                         "third person": {
                             "female": {
-                                "en": "She had|She hadn't",
-                                "fi": "H\u00e4nell\u00e4 ei ollut;female",
-                                "nl": "Zij had niet|Ze had niet"
+                                "en": "she had|she hadn't",
+                                "fi": "h\u00e4nell\u00e4 ei ollut;female",
+                                "nl": [
+                                    "zij had niet|ze had niet",
+                                    "zij had geen|ze had geen"
+                                ]
                             },
                             "male": {
-                                "en": "He had not|He hadn't",
-                                "fi": "H\u00e4nell\u00e4 ei ollut;male",
-                                "nl": "Hij had niet"
+                                "en": "he had not|he hadn't",
+                                "fi": "h\u00e4nell\u00e4 ei ollut;male",
+                                "nl": [
+                                    "hij had niet",
+                                    "hij had geen"
+                                ]
                             }
                         }
                     }
                 },
                 "present tense": {
                     "plural": {
                         "first person": {
-                            "en": "We have not|We've not|We haven't",
-                            "fi": "Meill\u00e4 ei ole",
-                            "nl": "Wij hebben niet|We hebben niet"
+                            "en": "we have not|we've not|we haven't",
+                            "fi": "meill\u00e4 ei ole",
+                            "nl": [
+                                "wij hebben niet|we hebben niet",
+                                "wij hebben geen|we hebben geen"
+                            ]
                         },
                         "second person": {
-                            "en": "You have not|You've not|You haven't;plural",
-                            "fi": "Teill\u00e4 ei ole",
-                            "nl": "Jullie hebben niet"
+                            "en": "you have not|you've not|you haven't;plural",
+                            "fi": "teill\u00e4 ei ole",
+                            "nl": [
+                                "jullie hebben niet",
+                                "jullie hebben geen"
+                            ]
                         },
                         "third person": {
-                            "en": "They have not|They've not|They haven't",
-                            "fi": "Heill\u00e4 ei ole",
-                            "nl": "Zij hebben niet|Ze hebben niet"
+                            "en": "they have not|they've not|they haven't",
+                            "fi": "heill\u00e4 ei ole",
+                            "nl": [
+                                "zij hebben niet|ze hebben niet",
+                                "zij hebben geen|ze hebben geen"
+                            ]
                         }
                     },
                     "singular": {
                         "first person": {
                             "en": "I have not|I've not|I haven't",
-                            "fi": "Minulla ei ole",
-                            "nl": "Ik heb niet"
+                            "fi": "minulla ei ole",
+                            "nl": [
+                                "ik heb niet",
+                                "ik heb geen"
+                            ]
                         },
                         "second person": {
-                            "en": "You have not|You've not|You haven't;singular",
-                            "fi": "Sinulla ei ole",
-                            "nl": "Jij hebt nietl|Je hebt nietl"
+                            "en": "you have not|you've not|you haven't;singular",
+                            "fi": "sinulla ei ole",
+                            "nl": [
+                                "jij hebt nietl|je hebt niet",
+                                "jij hebt geen|je hebt geen"
+                            ]
                         },
                         "third person": {
                             "female": {
-                                "en": "She has not|She's not|She hasn't",
-                                "fi": "H\u00e4nell\u00e4 ei ole;female",
-                                "nl": "Zij heeft niet|Ze heeft niet"
+                                "en": "she has not|she's not|she hasn't",
+                                "fi": "h\u00e4nell\u00e4 ei ole;female",
+                                "nl": [
+                                    "zij heeft niet|ze heeft niet",
+                                    "zij heeft geen|ze heeft geen"
+                                ]
                             },
                             "male": {
-                                "en": "He has not|He's not|He hasn't",
-                                "fi": "H\u00e4nell\u00e4 ei ole;male",
-                                "nl": "Hij heeft niet"
+                                "en": "he has not|he's not|he hasn't",
+                                "fi": "h\u00e4nell\u00e4 ei ole;male",
+                                "nl": [
+                                    "hij heeft niet",
+                                    "hij heeft geen"
+                                ]
                             }
                         }
                     }
                 }
             }
         },
         "interrogative": {
             "affirmative": {
                 "past tense": {
                     "plural": {
                         "first person": {
-                            "en": "Did we have?",
-                            "fi": "Oliko meill\u00e4?",
-                            "nl": "Hadden wij?|Hadden we?"
+                            "en": "did we have?",
+                            "fi": "oliko meill\u00e4?",
+                            "nl": "hadden wij?|hadden we?"
                         },
                         "second person": {
-                            "en": "Did you have?;plural",
-                            "fi": "Oliko teill\u00e4?",
-                            "nl": "Hadden jullie?"
+                            "en": "did you have?;plural",
+                            "fi": "oliko teill\u00e4?",
+                            "nl": "hadden jullie?"
                         },
                         "third person": {
-                            "en": "Did they have?",
-                            "fi": "Oliko heill\u00e4?",
-                            "nl": "Hadden zij?|Hadden ze?"
+                            "en": "did they have?",
+                            "fi": "oliko heill\u00e4?",
+                            "nl": "hadden zij?|hadden ze?"
                         }
                     },
                     "singular": {
                         "first person": {
-                            "en": "Did I have?",
-                            "fi": "Oliko minulla?",
-                            "nl": "Had ik?"
+                            "en": "did I have?",
+                            "fi": "oliko minulla?",
+                            "nl": "had ik?"
                         },
                         "second person": {
-                            "en": "Did you have?;singular",
-                            "fi": "Oliko sinulla?",
-                            "nl": "Had jij?|Had je?"
+                            "en": "did you have?;singular",
+                            "fi": "oliko sinulla?",
+                            "nl": "had jij?|had je?"
                         },
                         "third person": {
                             "female": {
-                                "en": "Did she have?",
-                                "fi": "Oliko h\u00e4nell\u00e4?;female",
-                                "nl": "Had zij?|Had ze?"
+                                "en": "did she have?",
+                                "fi": "oliko h\u00e4nell\u00e4?;female",
+                                "nl": "had zij?|had ze?"
                             },
                             "male": {
-                                "en": "Did he have?",
-                                "fi": "Oliko h\u00e4nell\u00e4?;male",
-                                "nl": "Had hij?"
+                                "en": "did he have?",
+                                "fi": "oliko h\u00e4nell\u00e4?;male",
+                                "nl": "had hij?"
                             }
                         }
                     }
                 },
                 "present tense": {
                     "plural": {
                         "first person": {
                             "en": [
-                                "Have we got?",
-                                "Do we have?"
+                                "have we got?",
+                                "do we have?"
                             ],
-                            "fi": "Onko meill\u00e4?",
-                            "nl": "Hebben wij?|Hebben we?"
+                            "fi": "onko meill\u00e4?",
+                            "nl": "hebben wij?|hebben we?"
                         },
                         "second person": {
                             "en": [
-                                "Have you got?;plural",
-                                "Do you have?;plural"
+                                "have you got?;plural",
+                                "do you have?;plural"
                             ],
-                            "fi": "Onko teill\u00e4?",
-                            "nl": "Hebben jullie?"
+                            "fi": "onko teill\u00e4?",
+                            "nl": "hebben jullie?"
                         },
                         "third person": {
                             "en": [
-                                "Have they got?",
-                                "Do they have?"
+                                "have they got?",
+                                "do they have?"
                             ],
-                            "fi": "Onko heill\u00e4?",
-                            "nl": "Hebben zij?|Hebben ze?"
+                            "fi": "onko heill\u00e4?",
+                            "nl": "hebben zij?|hebben ze?"
                         }
                     },
                     "singular": {
                         "first person": {
                             "en": [
-                                "Have I got?",
-                                "Do I have?"
+                                "have I got?",
+                                "do I have?"
                             ],
-                            "fi": "Onko minulla?",
-                            "nl": "Heb ik?"
+                            "fi": "onko minulla?",
+                            "nl": "heb ik?"
                         },
                         "second person": {
                             "en": [
-                                "Have you got?|;singular",
-                                "Do you have?;singular"
+                                "have you got?;singular",
+                                "do you have?;singular"
                             ],
-                            "fi": "Onko sinulla?",
-                            "nl": "Heb jij?|Heb je?"
+                            "fi": "onko sinulla?",
+                            "nl": "heb jij?|heb je?"
                         },
                         "third person": {
                             "female": {
                                 "en": [
-                                    "Has she got?",
-                                    "Does she have?"
+                                    "has she got?",
+                                    "does she have?"
                                 ],
-                                "fi": "Onko h\u00e4nell\u00e4?;female",
-                                "nl": "Heeft zij?|Heeft ze?"
+                                "fi": "onko h\u00e4nell\u00e4?;female",
+                                "nl": "heeft zij?|heeft ze?"
                             },
                             "male": {
                                 "en": [
-                                    "Has he got?",
-                                    "Does he have?"
+                                    "has he got?",
+                                    "does he have?"
                                 ],
-                                "fi": "Onko h\u00e4nell\u00e4?;male",
-                                "nl": "Heeft hij?"
+                                "fi": "onko h\u00e4nell\u00e4?;male",
+                                "nl": "heeft hij?"
                             }
                         }
                     }
                 }
             },
             "negative": {
                 "past tense": {
                     "plural": {
                         "first person": {
-                            "en": "Did we not have?|Didn't we have?",
-                            "fi": "Eik\u00f6 meill\u00e4 ollut?",
+                            "en": "did we not have?|didn't we have?",
+                            "fi": "eik\u00f6 meill\u00e4 ollut?",
                             "nl": [
-                                "Hadden wij niet?|Hadden we niet?",
-                                "Hadden wij geen?|Hadden we heen?"
+                                "hadden wij niet?|hadden we niet?",
+                                "hadden wij geen?|hadden we geen?"
                             ]
                         },
                         "second person": {
-                            "en": "Did you not have?|Didn't you have?;plural",
-                            "fi": "Eik\u00f6 teill\u00e4 ollut?",
+                            "en": "did you not have?|didn't you have?;plural",
+                            "fi": "eik\u00f6 teill\u00e4 ollut?",
                             "nl": [
-                                "Hadden jullie niet?",
-                                "Hadden jullie geen?"
+                                "hadden jullie niet?",
+                                "hadden jullie geen?"
                             ]
                         },
                         "third person": {
-                            "en": "Did they not have?|Didn't they have?",
-                            "fi": "Eik\u00f6 heill\u00e4 ollut?",
+                            "en": "did they not have?|didn't they have?",
+                            "fi": "eik\u00f6 heill\u00e4 ollut?",
                             "nl": [
-                                "Hadden zij niet?|Hadden ze niet?",
-                                "Hadden zij geen?|Hadden ze geen?"
+                                "hadden zij niet?|hadden ze niet?",
+                                "hadden zij geen?|hadden ze geen?"
                             ]
                         }
                     },
                     "singular": {
                         "first person": {
-                            "en": "Did I not have?|Didn't I have?",
-                            "fi": "Eik\u00f6 minulla ollut?",
+                            "en": "did I not have?|didn't I have?",
+                            "fi": "eik\u00f6 minulla ollut?",
                             "nl": [
-                                "Had ik niet?",
-                                "Had ik geen?"
+                                "had ik niet?",
+                                "had ik geen?"
                             ]
                         },
                         "second person": {
-                            "en": "Did you not have?|Didn't you have?;singular",
-                            "fi": "Eik\u00f6 sinulla ollut",
+                            "en": "did you not have?|didn't you have?;singular",
+                            "fi": "eik\u00f6 sinulla ollut?",
                             "nl": [
-                                "Had jij niet?|Had je niet?",
-                                "Had jij geen?|Had je geen?"
+                                "had jij niet?|had je niet?",
+                                "had jij geen?|had je geen?"
                             ]
                         },
                         "third person": {
                             "female": {
-                                "en": "Did she not have?|Didn't she have?",
-                                "fi": "Eik\u00f6 h\u00e4nell\u00e4 ollut?;female",
+                                "en": "did she not have?|didn't she have?",
+                                "fi": "eik\u00f6 h\u00e4nell\u00e4 ollut?;female",
                                 "nl": [
-                                    "Had zij niet?|Had ze niet?",
-                                    "Hsd zij geen?|Had ze geen?"
+                                    "had zij niet?|had ze niet?",
+                                    "had zij geen?|had ze geen?"
                                 ]
                             },
                             "male": {
-                                "en": "Did he not have?|Didn't he have?",
-                                "fi": "Eik\u00f6 h\u00e4nell\u00e4 ollut?;male",
+                                "en": "did he not have?|didn't he have?",
+                                "fi": "eik\u00f6 h\u00e4nell\u00e4 ollut?;male",
                                 "nl": [
-                                    "Had hij niet?",
-                                    "Had hij geen?"
+                                    "had hij niet?",
+                                    "had hij geen?"
                                 ]
                             }
                         }
                     }
                 },
                 "present tense": {
                     "plural": {
                         "first person": {
                             "en": [
-                                "Have we not got?|Haven't we got?",
-                                "Do we not have?|Don't we have?"
+                                "have we not got?|haven't we got?",
+                                "do we not have?|don't we have?"
                             ],
-                            "fi": "Eik\u00f6 meill\u00e4 ole?",
+                            "fi": "eik\u00f6 meill\u00e4 ole?",
                             "nl": [
-                                "Hebben wij niet?|Hebben we niet?",
-                                "Hebben wij geen?|Hebben we geen?"
+                                "hebben wij niet?|hebben we niet?",
+                                "hebben wij geen?|hebben we geen?"
                             ]
                         },
                         "second person": {
                             "en": [
-                                "Have you not got?|Haven't you got;plural",
-                                "Do you not have?|Don't you have?;plural"
+                                "have you not got?|haven't you got;plural",
+                                "do you not have?|don't you have?;plural"
                             ],
-                            "fi": "Eik\u00f6 teill\u00e4 ole?",
+                            "fi": "eik\u00f6 teill\u00e4 ole?",
                             "nl": [
-                                "Hebben jullie niet?",
-                                "Hebben jullie geen?"
+                                "hebben jullie niet?",
+                                "hebben jullie geen?"
                             ]
                         },
                         "third person": {
                             "en": [
-                                "Have they not got?|Haven't they got",
-                                "Do they not have?|Don't they have?"
+                                "have they not got?|haven't they got",
+                                "do they not have?|don't they have?"
                             ],
-                            "fi": "Eik\u00f6 heill\u00e4 ole?",
+                            "fi": "eik\u00f6 heill\u00e4 ole?",
                             "nl": [
-                                "Hebben zij niet?|Hebben ze niet?",
-                                "Hebben zij geen?|Hebben ze geen?"
+                                "hebben zij niet?|hebben ze niet?",
+                                "hebben zij geen?|hebben ze geen?"
                             ]
                         }
                     },
                     "singular": {
                         "first person": {
                             "en": [
-                                "Have I not got?|Haven't I got?",
-                                "Do I not have?|Don't I have?"
+                                "have I not got?|haven't I got?",
+                                "do I not have?|don't I have?"
                             ],
-                            "fi": "Eik\u00f6 minulla ole?",
+                            "fi": "eik\u00f6 minulla ole?",
                             "nl": [
-                                "Heb ik niet?",
-                                "Heb ik geen?"
+                                "heb ik niet?",
+                                "heb ik geen?"
                             ]
                         },
                         "second person": {
                             "en": [
-                                "Have you not got?|Haven't you got;singular",
-                                "Do you not have?|Don't you have?;singular"
+                                "have you not got?|haven't you got;singular",
+                                "do you not have?|don't you have?;singular"
                             ],
-                            "fi": "Eik\u00f6 sinulla ole?",
+                            "fi": "eik\u00f6 sinulla ole?",
                             "nl": [
-                                "Heb jij niet?|Heb je niet?",
-                                "Heb jij geen?|Heb je geen?"
+                                "heb jij niet?|heb je niet?",
+                                "heb jij geen?|heb je geen?"
                             ]
                         },
                         "third person": {
                             "female": {
                                 "en": [
-                                    "Has she not got?|Hasn't she got?",
-                                    "Does she not have?|Doesn't she have?"
+                                    "has she not got?|hasn't she got?",
+                                    "does she not have?|doesn't she have?"
                                 ],
-                                "fi": "Eik\u00f6 h\u00e4nell\u00e4 ole;female",
+                                "fi": "eik\u00f6 h\u00e4nell\u00e4 ole;female",
                                 "nl": [
-                                    "Heeft zij niet?|Heeft ze niet?",
-                                    "Heeft zij geen?|Heeft ze geen?"
+                                    "heeft zij niet?|heeft ze niet?",
+                                    "heeft zij geen?|heeft ze geen?"
                                 ]
                             },
                             "male": {
                                 "en": [
-                                    "Has he not got?|Hasn't he got?",
-                                    "Does he not have?|Doesn't he have?"
+                                    "has he not got?|hasn't he got?",
+                                    "does he not have?|doesn't he have?"
                                 ],
-                                "fi": "H\u00e4nell\u00e4 ei ole;male",
+                                "fi": "h\u00e4nell\u00e4 ei ole;male",
                                 "nl": [
-                                    "Heeft hij niet?",
-                                    "Heeft hij geen?"
+                                    "heeft hij niet?",
+                                    "heeft hij geen?"
                                 ]
                             }
                         }
                     }
                 }
             }
         },
@@ -1161,704 +1245,704 @@
                 "EP",
                 "OD"
             ]
         }
     },
     "to live": {
         "infinitive": {
-            "en": "To live",
-            "fi": "Asua",
-            "nl": "Wonen"
+            "en": "to live",
+            "fi": "asua",
+            "nl": "wonen"
         },
         "level": {
             "A1": [
                 "EP",
                 "KK",
                 "OD"
             ]
         },
         "past tense": {
             "plural": {
                 "first person": {
-                    "en": "We lived",
-                    "fi": "Me asuimme|Asuimme",
-                    "nl": "Wij woonden|We woonden"
+                    "en": "we lived",
+                    "fi": "me asuimme|asuimme",
+                    "nl": "wij woonden|we woonden"
                 },
                 "second person": {
-                    "en": "You lived;plural",
-                    "fi": "Te asuitte|Asuitte",
-                    "nl": "Jullie woonden"
+                    "en": "you lived;plural",
+                    "fi": "te asuitte|asuitte",
+                    "nl": "jullie woonden"
                 },
                 "third person": {
-                    "en": "They lived",
-                    "fi": "He asuivat",
-                    "nl": "Zij woonden|Ze woonden"
+                    "en": "they lived",
+                    "fi": "he asuivat",
+                    "nl": "zij woonden|ze woonden"
                 }
             },
             "singular": {
                 "first person": {
                     "en": "I lived",
-                    "fi": "Min\u00e4 asuin|Asuin",
-                    "nl": "Ik woonde"
+                    "fi": "min\u00e4 asuin|asuin",
+                    "nl": "ik woonde"
                 },
                 "second person": {
-                    "en": "You lived;singular",
-                    "fi": "Sin\u00e4 asuit|Asuit",
-                    "nl": "Jij woonde|Je woonde"
+                    "en": "you lived;singular",
+                    "fi": "sin\u00e4 asuit|Asuit",
+                    "nl": "jij woonde|je woonde"
                 },
                 "third person": {
                     "female": {
-                        "en": "She lived",
-                        "fi": "H\u00e4n asui;female",
-                        "nl": "Zij woonde|Ze woonde"
+                        "en": "she lived",
+                        "fi": "h\u00e4n asui;female",
+                        "nl": "zij woonde|ze woonde"
                     },
                     "male": {
-                        "en": "He lived",
-                        "fi": "H\u00e4n asui;male",
-                        "nl": "Hij woonde"
+                        "en": "he lived",
+                        "fi": "h\u00e4n asui;male",
+                        "nl": "hij woonde"
                     }
                 }
             }
         },
         "present tense": {
             "plural": {
                 "first person": {
-                    "en": "We live",
-                    "fi": "Me asumme|Asumme",
-                    "nl": "Wij wonen|We wonen"
+                    "en": "we live",
+                    "fi": "me asumme|asumme",
+                    "nl": "wij wonen|we wonen"
                 },
                 "second person": {
-                    "en": "You live;plural",
-                    "fi": "Te asutte|Asutte",
-                    "nl": "Jullie wonen"
+                    "en": "you live;plural",
+                    "fi": "te asutte|asutte",
+                    "nl": "jullie wonen"
                 },
                 "third person": {
-                    "en": "They live",
-                    "fi": "He asuvat",
-                    "nl": "Zij wonen|Ze wonen"
+                    "en": "they live",
+                    "fi": "he asuvat",
+                    "nl": "zij wonen|ze wonen"
                 }
             },
             "singular": {
                 "first person": {
                     "en": "I live",
-                    "fi": "Min\u00e4 asun|Asun",
-                    "nl": "Ik woon"
+                    "fi": "min\u00e4 asun|asun",
+                    "nl": "ik woon"
                 },
                 "second person": {
-                    "en": "You live;singular",
-                    "fi": "Sin\u00e4 asut|Asut",
-                    "nl": "Jij woont|Je woont"
+                    "en": "you live;singular",
+                    "fi": "sin\u00e4 asut|asut",
+                    "nl": "jij woont|je woont"
                 },
                 "third person": {
                     "female": {
-                        "en": "She lives",
-                        "fi": "H\u00e4n asuu;female",
-                        "nl": "Zij woont|Ze woont"
+                        "en": "she lives",
+                        "fi": "h\u00e4n asuu;female",
+                        "nl": "zij woont|ze woont"
                     },
                     "male": {
-                        "en": "He lives",
-                        "fi": "H\u00e4n asuu;male",
-                        "nl": "Hij woont"
+                        "en": "he lives",
+                        "fi": "h\u00e4n asuu;male",
+                        "nl": "hij woont"
                     }
                 }
             }
         }
     },
     "to paint": {
         "infinitive": {
-            "en": "To paint",
-            "fi": "Maalata",
-            "nl": "Schilderen"
+            "en": "to paint",
+            "fi": "maalata",
+            "nl": "schilderen"
         },
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
         "past tense": {
             "plural": {
                 "first person": {
-                    "en": "We painted",
-                    "fi": "Me maalasimme|Maalasimme",
-                    "nl": "Wij schilderden|We schilderden"
+                    "en": "we painted",
+                    "fi": "me maalasimme|maalasimme",
+                    "nl": "wij schilderden|we schilderden"
                 },
                 "second person": {
-                    "en": "You painted;plural",
-                    "fi": "Te maalasitte|Maalasitte",
-                    "nl": "Jullie schilderden"
+                    "en": "you painted;plural",
+                    "fi": "te maalasitte|maalasitte",
+                    "nl": "jullie schilderden"
                 },
                 "third person": {
-                    "en": "They painted",
-                    "fi": "He maalasivat",
-                    "nl": "Zij schilderden|Ze schilderden"
+                    "en": "they painted",
+                    "fi": "he maalasivat",
+                    "nl": "zij schilderden|ze schilderden"
                 }
             },
             "singular": {
                 "first person": {
                     "en": "I painted",
-                    "fi": "Min\u00e4 maalasin|Maalasin",
-                    "nl": "Ik schilderde"
+                    "fi": "min\u00e4 maalasin|maalasin",
+                    "nl": "ik schilderde"
                 },
                 "second person": {
-                    "en": "You painted;singular",
-                    "fi": "Sin\u00e4 maalasit|Maalasit",
-                    "nl": "Jij schilderde|Je schilderde"
+                    "en": "you painted;singular",
+                    "fi": "sin\u00e4 maalasit|maalasit",
+                    "nl": "jij schilderde|je schilderde"
                 },
                 "third person": {
                     "female": {
-                        "en": "She painted",
-                        "fi": "H\u00e4n maalasi;female",
-                        "nl": "Zij schilderde|Ze schilderde"
+                        "en": "she painted",
+                        "fi": "h\u00e4n maalasi;female",
+                        "nl": "zij schilderde|ze schilderde"
                     },
                     "male": {
-                        "en": "He painted",
-                        "fi": "H\u00e4n maalasi;male",
-                        "nl": "Hij schilderde"
+                        "en": "he painted",
+                        "fi": "h\u00e4n maalasi;male",
+                        "nl": "hij schilderde"
                     }
                 }
             }
         },
         "present tense": {
             "plural": {
                 "first person": {
-                    "en": "We paint",
-                    "fi": "Me maalaamme|Maalaamme",
-                    "nl": "Wij schilderen|We schilderen"
+                    "en": "we paint",
+                    "fi": "me maalaamme|maalaamme",
+                    "nl": "wij schilderen|we schilderen"
                 },
                 "second person": {
-                    "en": "You paint;plural",
-                    "fi": "Te maalaatte|Maalaatte",
-                    "nl": "Jullie schilderen"
+                    "en": "you paint;plural",
+                    "fi": "te maalaatte|maalaatte",
+                    "nl": "jullie schilderen"
                 },
                 "third person": {
-                    "en": "They paint",
-                    "fi": "He maalaavat",
-                    "nl": "Zij schilderen|Ze schilderen"
+                    "en": "they paint",
+                    "fi": "he maalaavat",
+                    "nl": "zij schilderen|ze schilderen"
                 }
             },
             "singular": {
                 "first person": {
                     "en": "I paint",
-                    "fi": "Min\u00e4 maalaan|Maalaan",
-                    "nl": "Ik schilder"
+                    "fi": "min\u00e4 maalaan|maalaan",
+                    "nl": "ik schilder"
                 },
                 "second person": {
-                    "en": "You paint;singular",
-                    "fi": "Sin\u00e4 maalaat|Maalaat",
-                    "nl": "Jij schildert|Je schildert"
+                    "en": "you paint;singular",
+                    "fi": "sin\u00e4 maalaat|maalaat",
+                    "nl": "jij schildert|je schildert"
                 },
                 "third person": {
                     "female": {
-                        "en": "She paints",
-                        "fi": "H\u00e4n maalaa;female",
-                        "nl": "Zij schildert|Ze schildert"
+                        "en": "she paints",
+                        "fi": "h\u00e4n maalaa;female",
+                        "nl": "zij schildert|ze schildert"
                     },
                     "male": {
-                        "en": "He paints",
-                        "fi": "H\u00e4n maalaa;male",
-                        "nl": "Hij schildert"
+                        "en": "he paints",
+                        "fi": "h\u00e4n maalaa;male",
+                        "nl": "hij schildert"
                     }
                 }
             }
         }
     },
     "to read": {
         "infinitive": {
-            "en": "To read",
-            "fi": "Lukea",
-            "nl": "Lezen"
+            "en": "to read",
+            "fi": "lukea",
+            "nl": "lezen"
         },
         "level": {
             "A1": [
                 "EP",
                 "KK",
                 "OD"
             ]
         },
         "past tense": {
             "plural": {
                 "first person": {
-                    "en": "We read;past tense",
-                    "fi": "Me luimme|Luimme",
-                    "nl": "Wij lazen|We lazen"
+                    "en": "we read;past tense",
+                    "fi": "me luimme|luimme",
+                    "nl": "wij lazen|we lazen"
                 },
                 "second person": {
-                    "en": "You read;plural past tense",
-                    "fi": "Te luitte|Luitte",
-                    "nl": "Jullie lazen"
+                    "en": "you read;plural past tense",
+                    "fi": "te luitte|luitte",
+                    "nl": "jullie lazen"
                 },
                 "third person": {
-                    "en": "They read;past tense",
-                    "fi": "He lukivat",
-                    "nl": "Zij lazen|Ze lazen"
+                    "en": "they read;past tense",
+                    "fi": "he lukivat",
+                    "nl": "zij lazen|ze lazen"
                 }
             },
             "singular": {
                 "first person": {
                     "en": "I read;past tense",
-                    "fi": "Min\u00e4 luin|Luin",
-                    "nl": "Ik las"
+                    "fi": "min\u00e4 luin|luin",
+                    "nl": "ik las"
                 },
                 "second person": {
-                    "en": "You read;singular past tense",
-                    "fi": "Sin\u00e4 luit|Luit",
-                    "nl": "Jij las|Je las"
+                    "en": "you read;singular past tense",
+                    "fi": "sin\u00e4 luit|luit",
+                    "nl": "jij las|je las"
                 },
                 "third person": {
                     "female": {
-                        "en": "She read",
-                        "fi": "H\u00e4n luki;female",
-                        "nl": "Zij las|Ze las"
+                        "en": "she read",
+                        "fi": "h\u00e4n luki;female",
+                        "nl": "zij las|ze las"
                     },
                     "male": {
-                        "en": "He read",
-                        "fi": "H\u00e4n luki;male",
-                        "nl": "Hij las"
+                        "en": "he read",
+                        "fi": "h\u00e4n luki;male",
+                        "nl": "hij las"
                     }
                 }
             }
         },
         "present tense": {
             "plural": {
                 "first person": {
-                    "en": "We read;present tense",
-                    "fi": "Me luemme|Luemme",
-                    "nl": "Wij lezen|We lezen"
+                    "en": "we read;present tense",
+                    "fi": "me luemme|luemme",
+                    "nl": "wij lezen|we lezen"
                 },
                 "second person": {
-                    "en": "You read;plural present tense",
-                    "fi": "Te luette|Luette",
-                    "nl": "Jullie lezen"
+                    "en": "you read;plural present tense",
+                    "fi": "te luette|luette",
+                    "nl": "jullie lezen"
                 },
                 "third person": {
-                    "en": "They read;present tense",
-                    "fi": "He lukevat",
-                    "nl": "Zij lezen|Ze lezen"
+                    "en": "they read;present tense",
+                    "fi": "he lukevat",
+                    "nl": "zij lezen|ze lezen"
                 }
             },
             "singular": {
                 "first person": {
                     "en": "I read;present tense",
-                    "fi": "Min\u00e4 luen|Luen",
-                    "nl": "Ik lees"
+                    "fi": "min\u00e4 luen|luen",
+                    "nl": "ik lees"
                 },
                 "second person": {
-                    "en": "You read;singular present tense",
-                    "fi": "Sin\u00e4 luet|Luet",
-                    "nl": "Jij leest|Je leest"
+                    "en": "you read;singular present tense",
+                    "fi": "sin\u00e4 luet|luet",
+                    "nl": "jij leest|je leest"
                 },
                 "third person": {
                     "female": {
-                        "en": "She reads",
-                        "fi": "H\u00e4n lukee;female",
-                        "nl": "Zij leest|Ze leest"
+                        "en": "she reads",
+                        "fi": "h\u00e4n lukee;female",
+                        "nl": "zij leest|ze leest"
                     },
                     "male": {
-                        "en": "He reads",
-                        "fi": "H\u00e4n lukee;male",
-                        "nl": "Hij leest"
+                        "en": "he reads",
+                        "fi": "h\u00e4n lukee;male",
+                        "nl": "hij leest"
                     }
                 }
             }
         }
     },
     "to run": {
         "infinitive": {
-            "en": "To run",
-            "fi": "Juosta",
-            "nl": "Rennen"
+            "en": "to run",
+            "fi": "juosta",
+            "nl": "rennen"
         },
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
         "past tense": {
             "plural": {
                 "first person": {
-                    "en": "We ran",
-                    "fi": "Me juoksimme|Juoksimme",
-                    "nl": "Wij renden|We renden"
+                    "en": "we ran",
+                    "fi": "me juoksimme|juoksimme",
+                    "nl": "wij renden|we renden"
                 },
                 "second person": {
-                    "en": "You ran;plural",
-                    "fi": "Te juoksitte|Juoksitte",
-                    "nl": "Jullie renden"
+                    "en": "you ran;plural",
+                    "fi": "te juoksitte|juoksitte",
+                    "nl": "jullie renden"
                 },
                 "third person": {
-                    "en": "They ran",
-                    "fi": "He juoksivat",
-                    "nl": "Zij renden|Ze renden"
+                    "en": "they ran",
+                    "fi": "he juoksivat",
+                    "nl": "zij renden|ze renden"
                 }
             },
             "singular": {
                 "first person": {
                     "en": "I ran",
-                    "fi": "Min\u00e4 juoksin|Juoksin",
-                    "nl": "Ik rende"
+                    "fi": "min\u00e4 juoksin|juoksin",
+                    "nl": "ik rende"
                 },
                 "second person": {
-                    "en": "You ran;singular",
-                    "fi": "Sin\u00e4 juoksit|Juoksit",
-                    "nl": "Jij rende|Je rende"
+                    "en": "you ran;singular",
+                    "fi": "sin\u00e4 juoksit|juoksit",
+                    "nl": "jij rende|je rende"
                 },
                 "third person": {
                     "female": {
-                        "en": "She ran",
-                        "fi": "H\u00e4n juoksi;female",
-                        "nl": "Zij rende|Ze rende"
+                        "en": "she ran",
+                        "fi": "h\u00e4n juoksi;female",
+                        "nl": "zij rende|ze rende"
                     },
                     "male": {
-                        "en": "He ran",
-                        "fi": "H\u00e4n juoksi;male",
-                        "nl": "Hij rende"
+                        "en": "he ran",
+                        "fi": "h\u00e4n juoksi;male",
+                        "nl": "hij rende"
                     }
                 }
             }
         },
         "present tense": {
             "plural": {
                 "first person": {
-                    "en": "We run",
-                    "fi": "Me juoksemme|Juoksemme",
-                    "nl": "Wij rennen|We rennen"
+                    "en": "we run",
+                    "fi": "me juoksemme|juoksemme",
+                    "nl": "wij rennen|we rennen"
                 },
                 "second person": {
-                    "en": "You run;plural",
-                    "fi": "Te juoksette|Juoksette",
-                    "nl": "Jullie rennen"
+                    "en": "you run;plural",
+                    "fi": "te juoksette|juoksette",
+                    "nl": "jullie rennen"
                 },
                 "third person": {
-                    "en": "They run",
-                    "fi": "He juoksevat",
-                    "nl": "Zij rennen|Ze rennen"
+                    "en": "they run",
+                    "fi": "he juoksevat",
+                    "nl": "zij rennen|ze rennen"
                 }
             },
             "singular": {
                 "first person": {
                     "en": "I run",
-                    "fi": "Min\u00e4 juoksen|Juoksen",
-                    "nl": "Ik ren"
+                    "fi": "min\u00e4 juoksen|juoksen",
+                    "nl": "ik ren"
                 },
                 "second person": {
-                    "en": "You run;singular",
-                    "fi": "Sin\u00e4 juokset|Juokset",
-                    "nl": "Jij rent|Je rent"
+                    "en": "you run;singular",
+                    "fi": "sin\u00e4 juokset|juokset",
+                    "nl": "jij rent|je rent"
                 },
                 "third person": {
                     "female": {
-                        "en": "She runs",
-                        "fi": "H\u00e4n juoksee;female",
-                        "nl": "Zij rent|Ze rent"
+                        "en": "she runs",
+                        "fi": "h\u00e4n juoksee;female",
+                        "nl": "zij rent|ze rent"
                     },
                     "male": {
-                        "en": "He runs",
-                        "fi": "H\u00e4n juoksee;male",
-                        "nl": "Hij rent"
+                        "en": "he runs",
+                        "fi": "h\u00e4n juoksee;male",
+                        "nl": "hij rent"
                     }
                 }
             }
         }
     },
     "to sleep": {
         "infinitive": {
-            "en": "To sleep",
-            "fi": "Nukkua",
-            "nl": "Slapen"
+            "en": "to sleep",
+            "fi": "nukkua",
+            "nl": "slapen"
         },
         "level": {
             "A1": [
                 "EP",
                 "KK",
                 "OD"
             ]
         },
         "past tense": {
             "plural": {
                 "first person": {
-                    "en": "We slept",
-                    "fi": "Me nukuimme|Nukuimme",
-                    "nl": "Wij sliepen|We sliepen"
+                    "en": "we slept",
+                    "fi": "me nukuimme|nukuimme",
+                    "nl": "wij sliepen|we sliepen"
                 },
                 "second person": {
-                    "en": "You slept;plural",
-                    "fi": "Te nukuitte|Nukuitte",
-                    "nl": "Jullie sliepen"
+                    "en": "you slept;plural",
+                    "fi": "te nukuitte|nukuitte",
+                    "nl": "jullie sliepen"
                 },
                 "third person": {
-                    "en": "They slept",
-                    "fi": "He nukkuivat",
-                    "nl": "Zij sliepen|Ze sliepen"
+                    "en": "they slept",
+                    "fi": "he nukkuivat",
+                    "nl": "zij sliepen|ze sliepen"
                 }
             },
             "singular": {
                 "first person": {
                     "en": "I slept",
-                    "fi": "Min\u00e4 nukuin|Nukuin",
-                    "nl": "Ik sliep"
+                    "fi": "min\u00e4 nukuin|nukuin",
+                    "nl": "ik sliep"
                 },
                 "second person": {
-                    "en": "You slept;singular",
-                    "fi": "Sin\u00e4 nukuit|Nukuit",
-                    "nl": "Jij sliep|Je sliep"
+                    "en": "you slept;singular",
+                    "fi": "sin\u00e4 nukuit|nukuit",
+                    "nl": "jij sliep|je sliep"
                 },
                 "third person": {
                     "female": {
-                        "en": "She slept",
-                        "fi": "H\u00e4n nukkui;female",
-                        "nl": "Zij sliep|Ze sliep"
+                        "en": "she slept",
+                        "fi": "h\u00e4n nukkui;female",
+                        "nl": "zij sliep|ze sliep"
                     },
                     "male": {
-                        "en": "He slept",
-                        "fi": "H\u00e4n nukkui;male",
-                        "nl": "Hij sliep"
+                        "en": "he slept",
+                        "fi": "h\u00e4n nukkui;male",
+                        "nl": "hij sliep"
                     }
                 }
             }
         },
         "present tense": {
             "plural": {
                 "first person": {
-                    "en": "We sleep",
-                    "fi": "Me nukumme|Nukumme",
-                    "nl": "Wij slapen|We slapen"
+                    "en": "we sleep",
+                    "fi": "me nukumme|nukumme",
+                    "nl": "wij slapen|we slapen"
                 },
                 "second person": {
-                    "en": "You sleep;plural",
-                    "fi": "Te nukutte|Nukutte",
-                    "nl": "Jullie slapen"
+                    "en": "you sleep;plural",
+                    "fi": "te nukutte|nukutte",
+                    "nl": "jullie slapen"
                 },
                 "third person": {
-                    "en": "They sleep",
-                    "fi": "He nukkuvat",
-                    "nl": "Zij slapen|Ze slapen"
+                    "en": "they sleep",
+                    "fi": "he nukkuvat",
+                    "nl": "zij slapen|ze slapen"
                 }
             },
             "singular": {
                 "first person": {
                     "en": "I sleep",
-                    "fi": "Min\u00e4 nukun|Nukun",
-                    "nl": "Ik slaap"
+                    "fi": "min\u00e4 nukun|nukun",
+                    "nl": "ik slaap"
                 },
                 "second person": {
-                    "en": "You sleep;singular",
-                    "fi": "Sin\u00e4 nukut|Nukut",
-                    "nl": "Jij slaapt|Je slaapt"
+                    "en": "you sleep;singular",
+                    "fi": "sin\u00e4 nukut|nukut",
+                    "nl": "jij slaapt|je slaapt"
                 },
                 "third person": {
                     "female": {
-                        "en": "She sleeps",
-                        "fi": "H\u00e4n nukkuu;female",
-                        "nl": "Zij slaapt|Ze slaapt"
+                        "en": "she sleeps",
+                        "fi": "h\u00e4n nukkuu;female",
+                        "nl": "zij slaapt|ze slaapt"
                     },
                     "male": {
-                        "en": "He sleeps",
-                        "fi": "H\u00e4n nukkuu;male",
-                        "nl": "Hij slaapt"
+                        "en": "he sleeps",
+                        "fi": "h\u00e4n nukkuu;male",
+                        "nl": "hij slaapt"
                     }
                 }
             }
         }
     },
     "to walk": {
         "infinitive": {
-            "en": "To walk",
-            "fi": "K\u00e4vell\u00e4",
-            "nl": "Lopen"
+            "en": "to walk",
+            "fi": "k\u00e4vell\u00e4",
+            "nl": "lopen"
         },
         "level": {
             "A1": [
                 "EP",
                 "KK",
                 "OD"
             ]
         },
         "past tense": {
             "plural": {
                 "first person": {
-                    "en": "We walked",
-                    "fi": "Me k\u00e4velemme|K\u00e4velemme",
-                    "nl": "Wij liepen|We liepen"
+                    "en": "we walked",
+                    "fi": "me k\u00e4velimme|k\u00e4velimme",
+                    "nl": "wij liepen|we liepen"
                 },
                 "second person": {
-                    "en": "You walked;plural",
-                    "fi": "Te k\u00e4velette|K\u00e4velette",
-                    "nl": "Jullie liepen"
+                    "en": "you walked;plural",
+                    "fi": "te k\u00e4velitte|k\u00e4velitte",
+                    "nl": "jullie liepen"
                 },
                 "third person": {
-                    "en": "They walked",
-                    "fi": "He k\u00e4velev\u00e4t",
-                    "nl": "Zij liepen|Ze liepen"
+                    "en": "they walked",
+                    "fi": "he k\u00e4veliv\u00e4t",
+                    "nl": "zij liepen|ze liepen"
                 }
             },
             "singular": {
                 "first person": {
                     "en": "I walked",
-                    "fi": "Min\u00e4 k\u00e4velen|K\u00e4velen",
-                    "nl": "Ik liep"
+                    "fi": "min\u00e4 k\u00e4velin|k\u00e4velin",
+                    "nl": "ik liep"
                 },
                 "second person": {
-                    "en": "You walked;singular",
-                    "fi": "Sin\u00e4 k\u00e4velet|K\u00e4velet",
-                    "nl": "Jij liep|Je liep"
+                    "en": "you walked;singular",
+                    "fi": "sin\u00e4 k\u00e4velit|k\u00e4velit",
+                    "nl": "jij liep|je liep"
                 },
                 "third person": {
                     "female": {
-                        "en": "She walked",
-                        "fi": "H\u00e4n k\u00e4velee;female",
-                        "nl": "Zij liep|Ze liep"
+                        "en": "she walked",
+                        "fi": "h\u00e4n k\u00e4veli;female",
+                        "nl": "zij liep|ze liep"
                     },
                     "male": {
-                        "en": "He walked",
-                        "fi": "H\u00e4n k\u00e4velee;male",
-                        "nl": "Hij liep"
+                        "en": "he walked",
+                        "fi": "h\u00e4n k\u00e4veli;male",
+                        "nl": "hij liep"
                     }
                 }
             }
         },
         "present tense": {
             "plural": {
                 "first person": {
-                    "en": "We walk",
-                    "fi": "Me k\u00e4velemme|K\u00e4velemme",
-                    "nl": "Wij lopen|We lopen"
+                    "en": "we walk",
+                    "fi": "me k\u00e4velemme|k\u00e4velemme",
+                    "nl": "wij lopen|we lopen"
                 },
                 "second person": {
-                    "en": "You walk;plural",
-                    "fi": "Te k\u00e4velette|K\u00e4velette",
-                    "nl": "Jullie lopen"
+                    "en": "you walk;plural",
+                    "fi": "te k\u00e4velette|k\u00e4velette",
+                    "nl": "jullie lopen"
                 },
                 "third person": {
-                    "en": "They walk",
-                    "fi": "He k\u00e4velev\u00e4t",
-                    "nl": "Zij lopen|Ze lopen"
+                    "en": "they walk",
+                    "fi": "he k\u00e4velev\u00e4t",
+                    "nl": "zij lopen|ze lopen"
                 }
             },
             "singular": {
                 "first person": {
                     "en": "I walk",
-                    "fi": "Min\u00e4 k\u00e4velen|K\u00e4velen",
-                    "nl": "Ik loop"
+                    "fi": "min\u00e4 k\u00e4velen|k\u00e4velen",
+                    "nl": "ik loop"
                 },
                 "second person": {
-                    "en": "You walk;singular",
-                    "fi": "Sin\u00e4 k\u00e4velet|K\u00e4velet",
-                    "nl": "Jij loopt|Je loopt"
+                    "en": "you walk;singular",
+                    "fi": "sin\u00e4 k\u00e4velet|k\u00e4velet",
+                    "nl": "jij loopt|je loopt"
                 },
                 "third person": {
                     "female": {
-                        "en": "She walks",
-                        "fi": "H\u00e4n k\u00e4velee;female",
-                        "nl": "Zij loopt|Ze loopt"
+                        "en": "she walks",
+                        "fi": "h\u00e4n k\u00e4velee;female",
+                        "nl": "zij loopt|ze loopt"
                     },
                     "male": {
-                        "en": "He walks",
-                        "fi": "H\u00e4n k\u00e4velee;male",
-                        "nl": "Hij loopt"
+                        "en": "he walks",
+                        "fi": "h\u00e4n k\u00e4velee;male",
+                        "nl": "hij loopt"
                     }
                 }
             }
         }
     },
     "to write": {
         "infinitive": {
-            "en": "To write",
-            "fi": "Kirjoittaa",
-            "nl": "Schrijven"
+            "en": "to write",
+            "fi": "kirjoittaa",
+            "nl": "schrijven"
         },
         "level": {
             "A1": [
                 "EP",
                 "KK",
                 "OD"
             ]
         },
         "past tense": {
             "plural": {
                 "first person": {
-                    "en": "We wrote",
-                    "fi": "Me kirjoitimme|Kirjoitimme",
-                    "nl": "Wij schreven|We schreven"
+                    "en": "we wrote",
+                    "fi": "me kirjoitimme|kirjoitimme",
+                    "nl": "wij schreven|we schreven"
                 },
                 "second person": {
-                    "en": "You wrote;plural",
-                    "fi": "Te kirjoititte|Kirjoititte",
-                    "nl": "Jullie schreven"
+                    "en": "you wrote;plural",
+                    "fi": "te kirjoititte|kirjoititte",
+                    "nl": "jullie schreven"
                 },
                 "third person": {
-                    "en": "They wrote",
-                    "fi": "He kirjoittivat",
-                    "nl": "Zij schreven|Ze schreven"
+                    "en": "they wrote",
+                    "fi": "he kirjoittivat",
+                    "nl": "zij schreven|ze schreven"
                 }
             },
             "singular": {
                 "first person": {
                     "en": "I wrote",
-                    "fi": "Min\u00e4 kirjoitin|Kirjoitin",
-                    "nl": "Ik schreef"
+                    "fi": "min\u00e4 kirjoitin|kirjoitin",
+                    "nl": "ik schreef"
                 },
                 "second person": {
-                    "en": "You wrote;singular",
-                    "fi": "Sin\u00e4 kirjoitit|Kirjoitit",
-                    "nl": "Jij schreef|Je schreef"
+                    "en": "you wrote;singular",
+                    "fi": "sin\u00e4 kirjoitit|kirjoitit",
+                    "nl": "jij schreef|je schreef"
                 },
                 "third person": {
                     "female": {
-                        "en": "She wrote",
-                        "fi": "H\u00e4n kirjoitti;female",
-                        "nl": "Zij schreef|Ze schreef"
+                        "en": "she wrote",
+                        "fi": "h\u00e4n kirjoitti;female",
+                        "nl": "zij schreef|ze schreef"
                     },
                     "male": {
-                        "en": "He wrote",
-                        "fi": "H\u00e4n kirjoitti;male",
-                        "nl": "Hij schreef"
+                        "en": "he wrote",
+                        "fi": "h\u00e4n kirjoitti;male",
+                        "nl": "hij schreef"
                     }
                 }
             }
         },
         "present tense": {
             "plural": {
                 "first person": {
-                    "en": "We write",
-                    "fi": "Me kirjoitamme|Kirjoitamme",
-                    "nl": "Wij schrijven|We schrijven"
+                    "en": "we write",
+                    "fi": "me kirjoitamme|kirjoitamme",
+                    "nl": "wij schrijven|we schrijven"
                 },
                 "second person": {
-                    "en": "You write;plural",
-                    "fi": "Te kirjoitatte|Kirjoitatte",
-                    "nl": "Jullie schrijven"
+                    "en": "you write;plural",
+                    "fi": "te kirjoitatte|kirjoitatte",
+                    "nl": "jullie schrijven"
                 },
                 "third person": {
-                    "en": "They write",
-                    "fi": "He kirjoittavat",
-                    "nl": "Zij schrijven|Ze schrijven"
+                    "en": "they write",
+                    "fi": "he kirjoittavat",
+                    "nl": "zij schrijven|ze schrijven"
                 }
             },
             "singular": {
                 "first person": {
                     "en": "I write",
-                    "fi": "Min\u00e4 kirjoitan|Kirjoitan",
-                    "nl": "Ik schrijf"
+                    "fi": "min\u00e4 kirjoitan|kirjoitan",
+                    "nl": "ik schrijf"
                 },
                 "second person": {
-                    "en": "You write;singular",
-                    "fi": "Sin\u00e4 kirjoitat|Kirjoitat",
-                    "nl": "Jij schrijft|Je schrijft"
+                    "en": "you write;singular",
+                    "fi": "sin\u00e4 kirjoitat|kirjoitat",
+                    "nl": "jij schrijft|je schrijft"
                 },
                 "third person": {
                     "female": {
-                        "en": "She writes",
-                        "fi": "H\u00e4n kirjoittaa;female",
-                        "nl": "Zij schrijft|Ze schrijft"
+                        "en": "she writes",
+                        "fi": "h\u00e4n kirjoittaa;female",
+                        "nl": "zij schrijft|ze schrijft"
                     },
                     "male": {
-                        "en": "He writes",
-                        "fi": "H\u00e4n kirjoittaa;male",
-                        "nl": "Hij schrijft"
+                        "en": "he writes",
+                        "fi": "h\u00e4n kirjoittaa;male",
+                        "nl": "hij schrijft"
                     }
                 }
             }
         }
     }
 }
```

### Comparing `Toisto-0.8.2/src/topics/weather.json` & `Toisto-0.9.0/src/topics/weather.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8029320987654321%*

 * *Differences: {"'cloud'": "{'singular': {'en': 'cloud', 'fi': 'pilvi', 'nl': 'de wolk'}, 'plural': {'en': "*

 * *            "'clouds', 'fi': 'pilvet', 'nl': 'de wolken'}}",*

 * * "'cloudy'": "{'en': 'cloudy', 'fi': 'pilvinen', 'nl': 'bewolkt'}",*

 * * "'fog'": "{'en': 'fog', 'fi': 'sumu', 'nl': 'de mist'}",*

 * * "'foggy'": "{'en': 'foggy', 'fi': 'sumuinen', 'nl': 'mistig'}",*

 * * "'ice'": "OrderedDict([('level', OrderedDict([('A1', 'OD'), ('A2', 'EP')])), ('en', 'ice'), "*

 * *          "('fi', 'jää'), ('nl', 'het ijs')])",*

 * * "'it is cloudy'": '{\' […]*

```diff
@@ -3,51 +3,51 @@
         "level": {
             "A2": [
                 "EP",
                 "OD"
             ]
         },
         "plural": {
-            "en": "Clouds",
-            "fi": "Pilvet",
-            "nl": "De wolken"
+            "en": "clouds",
+            "fi": "pilvet",
+            "nl": "de wolken"
         },
         "singular": {
-            "en": "Cloud",
-            "fi": "Pilvi",
-            "nl": "De wolk"
+            "en": "cloud",
+            "fi": "pilvi",
+            "nl": "de wolk"
         }
     },
     "cloudy": {
-        "en": "Cloudy",
-        "fi": "Pilvinen",
+        "en": "cloudy",
+        "fi": "pilvinen",
         "level": {
             "A2": "EP",
             "B1": "OD"
         },
-        "nl": "Bewolkt",
+        "nl": "bewolkt",
         "roots": "cloud"
     },
     "fog": {
-        "en": "Fog",
-        "fi": "Sumu",
+        "en": "fog",
+        "fi": "sumu",
         "level": {
             "A2": "EP",
             "B2": "OD"
         },
-        "nl": "De mist"
+        "nl": "de mist"
     },
     "foggy": {
-        "en": "Foggy",
-        "fi": "Sumuinen",
+        "en": "foggy",
+        "fi": "sumuinen",
         "level": {
             "EP": "A2",
             "OD": "B2"
         },
-        "nl": "Mistig",
+        "nl": "mistig",
         "roots": "fog"
     },
     "how is the weather": {
         "en": "How is the weather?|How's the weather?",
         "fi": [
             "Millainen s\u00e4\u00e4 on?",
             "Mink\u00e4lainen s\u00e4\u00e4 on?"
@@ -67,242 +67,251 @@
             "nl": [
                 "how",
                 "to be",
                 "weather"
             ]
         }
     },
+    "ice": {
+        "en": "ice",
+        "fi": "j\u00e4\u00e4",
+        "level": {
+            "A1": "OD",
+            "A2": "EP"
+        },
+        "nl": "het ijs"
+    },
     "it is cloudy": {
-        "en": "It is cloudy|It's cloudy",
-        "fi": "On pilvist\u00e4",
-        "nl": "Het is bewolkt",
+        "en": "It is cloudy.|It's cloudy.",
+        "fi": "On pilvist\u00e4.",
+        "nl": "Het is bewolkt.",
         "roots": [
             "to be",
             "cloudy"
         ]
     },
     "it is foggy": {
-        "en": "It is foggy|It's foggy",
-        "fi": "On sumuista",
-        "nl": "Het is mistig",
+        "en": "It is foggy.|It's foggy.",
+        "fi": "On sumuista.",
+        "nl": "Het is mistig.",
         "roots": [
             "to be",
             "foggy"
         ]
     },
     "it is raining": {
-        "en": "It is raining|It's raining",
+        "en": "It is raining.|It's raining.",
         "fi": [
-            "Sataa vett\u00e4",
-            "Sataa"
+            "Sataa vett\u00e4.",
+            "Sataa."
         ],
-        "nl": "Het regent",
+        "nl": "Het regent.",
         "roots": {
             "en": [
                 "to be",
                 "rain"
             ],
             "fi": "rain",
             "nl": "rain"
         }
     },
     "it is rainy": {
-        "en": "It is rainy|It's rainy",
-        "fi": "On sateista",
-        "nl": "Het is regenachtig",
+        "en": "It is rainy.|It's rainy.",
+        "fi": "On sateista.",
+        "nl": "Het is regenachtig.",
         "roots": [
             "to be",
             "rainy"
         ]
     },
     "it is snowing": {
-        "en": "It is snowing|It's snowing",
-        "fi": "Sataa lunta",
-        "nl": "Het sneeuwt",
+        "en": "It is snowing.|It's snowing.",
+        "fi": "Sataa lunta.",
+        "nl": "Het sneeuwt.",
         "roots": {
             "en": [
                 "to be",
                 "snow"
             ],
             "fi": "snow",
             "nl": "snow"
         }
     },
     "it is stormy": {
-        "en": "It is stormy|It's stormy",
-        "fi": "On myrskyist\u00e4",
-        "nl": "Het is stormachtig",
+        "en": "It is stormy.|It's stormy.",
+        "fi": "On myrskyist\u00e4.",
+        "nl": "Het is stormachtig.",
         "roots": [
             "to be",
             "stormy"
         ]
     },
     "it is sunny": {
-        "en": "It is sunny|It's sunny",
-        "fi": "On aurinkoista",
-        "nl": "Het is zonnig",
+        "en": "It is sunny.|It's sunny.",
+        "fi": "On aurinkoista.",
+        "nl": "Het is zonnig.",
         "roots": [
             "to be",
             "sunny"
         ]
     },
     "it is windy": {
-        "en": "It is windy|It's windy",
-        "fi": "On tuulista",
-        "nl": "Het is winderig",
+        "en": "It is windy.|It's windy.",
+        "fi": "On tuulista.",
+        "nl": "Het is winderig.",
         "roots": [
             "to be",
             "windy"
         ]
     },
     "rain": {
-        "en": "Rain",
-        "fi": "Sade",
+        "en": "rain",
+        "fi": "sade",
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
-        "nl": "De regen"
+        "nl": "de regen"
     },
     "rainy": {
-        "en": "Rainy",
-        "fi": "Sateinen",
+        "en": "rainy",
+        "fi": "sateinen",
         "level": {
             "A2": "OD",
             "B1": "EP"
         },
-        "nl": "Regenachtig",
+        "nl": "regenachtig",
         "roots": "rain"
     },
     "snow": {
-        "en": "Snow",
-        "fi": "Lumi",
+        "en": "snow",
+        "fi": "lumi",
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
-        "nl": "De sneeuw"
+        "nl": "de sneeuw"
     },
     "snowy": {
-        "en": "Snowy",
-        "fi": "Luminen",
+        "en": "snowy",
+        "fi": "luminen",
         "level": {
             "A2": "OD",
             "none": "EP"
         },
-        "nl": "Besneeuwd",
+        "nl": "besneeuwd",
         "roots": "snow"
     },
     "storm": {
-        "en": "Storm",
-        "fi": "Myrsky",
+        "en": "storm",
+        "fi": "myrsky",
         "level": {
             "A2": [
                 "EP",
                 "OD"
             ]
         },
-        "nl": "De storm"
+        "nl": "de storm"
     },
     "stormy": {
-        "en": "Stormy",
-        "fi": "Myrskyinen",
+        "en": "stormy",
+        "fi": "myrskyinen",
         "level": {
             "B2": [
                 "EP",
                 "OD"
             ]
         },
-        "nl": "Stormachtig",
+        "nl": "stormachtig",
         "roots": "storm"
     },
     "sun": {
-        "en": "Sun",
-        "fi": "Aurinko",
+        "en": "sun",
+        "fi": "aurinko",
         "level": {
             "A1": [
                 "EP",
                 "KK",
                 "OD"
             ]
         },
-        "nl": "De zon"
+        "nl": "de zon"
     },
     "sunny": {
-        "en": "Sunny",
-        "fi": "Aurinkoinen",
+        "en": "sunny",
+        "fi": "aurinkoinen",
         "level": {
             "A1": "OD",
             "A2": "EP"
         },
-        "nl": "Zonnig",
+        "nl": "zonnig",
         "roots": "sun"
     },
     "there is a thunderstorm": {
-        "en": "There is a thunderstorm|There's a thunderstorm",
+        "en": "There is a thunderstorm.|There's a thunderstorm.",
         "fi": [
-            "Ukkostaa",
-            "On ukonilma"
+            "Ukkostaa.",
+            "On ukonilma."
         ],
-        "nl": "Het onweert",
+        "nl": "Het onweert.",
         "roots": {
             "en": [
                 "to be",
                 "storm",
                 "thunder"
             ],
             "fi": [
                 "to be",
                 "thunder"
             ],
             "nl": "to be"
         }
     },
     "thunder": {
-        "en": "Thunder",
-        "fi": "Ukkonen",
+        "en": "thunder",
+        "fi": "ukkonen",
         "level": {
             "B1": "EP",
             "C1": "OD"
         },
-        "nl": "De donder"
+        "nl": "de donder"
     },
     "weather": {
-        "en": "Weather",
-        "fi": "S\u00e4\u00e4",
+        "en": "weather",
+        "fi": "s\u00e4\u00e4",
         "level": {
             "A1": [
                 "EP",
                 "OD"
             ]
         },
-        "nl": "Het weer"
+        "nl": "het weer"
     },
     "wind": {
-        "en": "Wind",
-        "fi": "Tuuli",
+        "en": "wind",
+        "fi": "tuuli",
         "level": {
             "A1": [
                 "EP",
                 "KK"
             ],
             "A2": "OD"
         },
-        "nl": "De wind"
+        "nl": "de wind"
     },
     "windy": {
-        "en": "Windy",
-        "fi": "Tuulinen",
+        "en": "windy",
+        "fi": "tuulinen",
         "level": {
             "A2": [
                 "EP",
                 "OD"
             ]
         },
-        "nl": "Winderig",
+        "nl": "winderig",
         "roots": "wind"
     }
 }
```

