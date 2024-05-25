# Comparing `tmp/ingredient_slicer-1.0.2.tar.gz` & `tmp/ingredient_slicer-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ingredient_slicer-1.0.2.tar", last modified: Sat May 18 16:16:52 2024, max compression
+gzip compressed data, was "ingredient_slicer-1.0.3.tar", last modified: Sat May 25 16:29:22 2024, max compression
```

## Comparing `ingredient_slicer-1.0.2.tar` & `ingredient_slicer-1.0.3.tar`

### file list

```diff
@@ -1,69 +1,70 @@
-drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-05-18 16:16:52.129885 ingredient_slicer-1.0.2/
-drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-05-18 16:16:52.116373 ingredient_slicer-1.0.2/.github/
-drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-05-18 16:16:52.118044 ingredient_slicer-1.0.2/.github/workflows/
--rw-r--r--   0 anguswatters   (501) staff       (20)     3289 2024-05-07 12:28:17.000000 ingredient_slicer-1.0.2/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 anguswatters   (501) staff       (20)      782 2024-03-23 22:54:24.000000 ingredient_slicer-1.0.2/.github/workflows/run-unit-tests.yml
--rw-r--r--   0 anguswatters   (501) staff       (20)     3118 2024-03-17 16:59:19.000000 ingredient_slicer-1.0.2/.gitignore
--rw-r--r--   0 anguswatters   (501) staff       (20)     1075 2024-03-17 16:52:34.000000 ingredient_slicer-1.0.2/LICENSE
--rw-r--r--   0 anguswatters   (501) staff       (20)     3362 2024-05-18 16:16:52.129584 ingredient_slicer-1.0.2/PKG-INFO
--rw-r--r--   0 anguswatters   (501) staff       (20)     2389 2024-04-08 22:17:24.000000 ingredient_slicer-1.0.2/README.md
-drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-05-18 16:16:52.119927 ingredient_slicer-1.0.2/ingredient_slicer/
--rw-r--r--   0 anguswatters   (501) staff       (20)     1725 2024-05-18 16:16:43.000000 ingredient_slicer-1.0.2/ingredient_slicer/__init__.py
--rw-r--r--   0 anguswatters   (501) staff       (20)   156564 2024-05-18 16:16:01.000000 ingredient_slicer-1.0.2/ingredient_slicer/_constants.py
--rw-r--r--   0 anguswatters   (501) staff       (20)   102582 2024-05-06 17:09:54.000000 ingredient_slicer-1.0.2/ingredient_slicer/_ingredient_slicer.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    91104 2024-04-18 00:53:53.000000 ingredient_slicer-1.0.2/ingredient_slicer/_regex_patterns.py
--rw-r--r--   0 anguswatters   (501) staff       (20)   106410 2024-05-18 16:16:27.000000 ingredient_slicer-1.0.2/ingredient_slicer/_utils.py
-drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-05-18 16:16:52.128925 ingredient_slicer-1.0.2/ingredient_slicer.egg-info/
--rw-r--r--   0 anguswatters   (501) staff       (20)     3362 2024-05-18 16:16:52.000000 ingredient_slicer-1.0.2/ingredient_slicer.egg-info/PKG-INFO
--rw-r--r--   0 anguswatters   (501) staff       (20)     2108 2024-05-18 16:16:52.000000 ingredient_slicer-1.0.2/ingredient_slicer.egg-info/SOURCES.txt
--rw-r--r--   0 anguswatters   (501) staff       (20)        1 2024-05-18 16:16:52.000000 ingredient_slicer-1.0.2/ingredient_slicer.egg-info/dependency_links.txt
--rw-r--r--   0 anguswatters   (501) staff       (20)       38 2024-05-18 16:16:52.000000 ingredient_slicer-1.0.2/ingredient_slicer.egg-info/requires.txt
--rw-r--r--   0 anguswatters   (501) staff       (20)       18 2024-05-18 16:16:52.000000 ingredient_slicer-1.0.2/ingredient_slicer.egg-info/top_level.txt
--rw-r--r--   0 anguswatters   (501) staff       (20)     1124 2024-05-18 16:16:39.000000 ingredient_slicer-1.0.2/pyproject.toml
--rw-r--r--   0 anguswatters   (501) staff       (20)       38 2024-05-18 16:16:52.129940 ingredient_slicer-1.0.2/setup.cfg
-drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-05-18 16:16:52.128670 ingredient_slicer-1.0.2/tests/
--rw-r--r--   0 anguswatters   (501) staff       (20)        0 2024-04-06 13:59:44.000000 ingredient_slicer-1.0.2/tests/__init__.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     2402 2024-04-06 15:22:11.000000 ingredient_slicer-1.0.2/tests/test_avg_ranges.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     5566 2024-04-10 14:53:42.000000 ingredient_slicer-1.0.2/tests/test_casual_ingredients.py
--rw-r--r--   0 anguswatters   (501) staff       (20)        0 2024-04-06 15:22:03.000000 ingredient_slicer-1.0.2/tests/test_clean_hyphen_padded_substrings.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     5502 2024-04-06 15:27:00.000000 ingredient_slicer-1.0.2/tests/test_convert_fractions_to_decimals.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     2145 2024-04-06 15:27:01.000000 ingredient_slicer-1.0.2/tests/test_convert_volumes_to_milliliters.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     1182 2024-03-29 21:19:57.000000 ingredient_slicer-1.0.2/tests/test_duplicate_unit_ranges.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     8507 2024-03-29 21:18:52.000000 ingredient_slicer-1.0.2/tests/test_extract_dimensions.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     3541 2024-03-29 21:19:50.000000 ingredient_slicer-1.0.2/tests/test_extract_quantities_utils.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     3711 2024-03-29 21:19:48.000000 ingredient_slicer-1.0.2/tests/test_find_and_remove.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     2842 2024-03-29 21:19:52.000000 ingredient_slicer-1.0.2/tests/test_find_and_remove_hyphen_substrings.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     3352 2024-04-06 13:59:33.000000 ingredient_slicer-1.0.2/tests/test_fraction_str_to_decimal.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    26160 2024-05-06 14:16:39.000000 ingredient_slicer-1.0.2/tests/test_get_gram_weight.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     2496 2024-05-06 15:32:33.000000 ingredient_slicer-1.0.2/tests/test_get_single_item_gram_weight.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    20386 2024-04-10 16:18:22.000000 ingredient_slicer-1.0.2/tests/test_ingredient_slicer.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     3428 2024-04-08 13:04:03.000000 ingredient_slicer-1.0.2/tests/test_ingredient_slicer_dimensions.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     4718 2024-04-10 14:52:58.000000 ingredient_slicer-1.0.2/tests/test_ingredient_slicer_fraction_conversions.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     1903 2024-05-06 17:14:21.000000 ingredient_slicer-1.0.2/tests/test_ingredient_slicer_gram_weights.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     1515 2024-04-10 14:52:56.000000 ingredient_slicer-1.0.2/tests/test_ingredient_slicer_parenthesis.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     7502 2024-04-10 14:52:56.000000 ingredient_slicer-1.0.2/tests/test_ingredient_slicer_x_separators.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     4178 2024-04-10 14:52:54.000000 ingredient_slicer-1.0.2/tests/test_is_approximate_quantity_only_parenthesis.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     2965 2024-04-10 14:52:54.000000 ingredient_slicer-1.0.2/tests/test_make_int_or_float_str.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     2169 2024-04-06 15:26:57.000000 ingredient_slicer-1.0.2/tests/test_merge_misleading_ranges.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    14464 2024-03-29 21:19:43.000000 ingredient_slicer-1.0.2/tests/test_merge_numbers.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    43982 2024-04-06 14:42:17.000000 ingredient_slicer-1.0.2/tests/test_number_ranges.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    56318 2024-03-29 21:19:45.000000 ingredient_slicer-1.0.2/tests/test_number_ranges_separated_by_words.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     5652 2024-04-06 13:59:36.000000 ingredient_slicer-1.0.2/tests/test_numbers_with_inch_symbols.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    15368 2024-03-29 21:19:20.000000 ingredient_slicer-1.0.2/tests/test_parenthesis.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    11036 2024-04-10 14:53:13.000000 ingredient_slicer-1.0.2/tests/test_parenthesis_utils.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     2512 2024-03-29 21:19:22.000000 ingredient_slicer-1.0.2/tests/test_percentages.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     3547 2024-03-29 21:19:26.000000 ingredient_slicer-1.0.2/tests/test_prefixed_number_words_regex.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     5013 2024-03-29 21:19:28.000000 ingredient_slicer-1.0.2/tests/test_prep_words.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     5261 2024-03-29 21:19:25.000000 ingredient_slicer-1.0.2/tests/test_quantity_range_regex.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    27045 2024-04-06 13:59:38.000000 ingredient_slicer-1.0.2/tests/test_quantity_units_regex.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     3571 2024-04-06 13:31:28.000000 ingredient_slicer-1.0.2/tests/test_remove_repeat_units_in_ranges.py
--rw-r--r--   0 anguswatters   (501) staff       (20)      633 2024-03-29 21:19:14.000000 ingredient_slicer-1.0.2/tests/test_remove_x_separators.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     6384 2024-03-29 21:19:12.000000 ingredient_slicer-1.0.2/tests/test_replace_a_or_an_quantities.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     6869 2024-03-29 21:19:08.000000 ingredient_slicer-1.0.2/tests/test_separate_dimensions.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     1808 2024-03-29 21:19:42.000000 ingredient_slicer-1.0.2/tests/test_size_modifiers.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     8974 2024-03-29 21:19:39.000000 ingredient_slicer-1.0.2/tests/test_spaced_numbers.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     5838 2024-03-29 21:19:40.000000 ingredient_slicer-1.0.2/tests/test_unit_regex.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    16676 2024-04-06 15:22:15.000000 ingredient_slicer-1.0.2/tests/test_wild_ingredients.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     8022 2024-04-06 15:22:14.000000 ingredient_slicer-1.0.2/tests/test_word_fractions.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     7167 2024-03-29 21:19:33.000000 ingredient_slicer-1.0.2/tests/test_word_numbers.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     1337 2024-04-06 14:42:17.000000 ingredient_slicer-1.0.2/tests/test_x_after_number_regex.py
+drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-05-25 16:29:22.499187 ingredient_slicer-1.0.3/
+drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-05-25 16:29:22.485881 ingredient_slicer-1.0.3/.github/
+drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-05-25 16:29:22.487074 ingredient_slicer-1.0.3/.github/workflows/
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3289 2024-05-07 12:28:17.000000 ingredient_slicer-1.0.3/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 anguswatters   (501) staff       (20)      782 2024-03-23 22:54:24.000000 ingredient_slicer-1.0.3/.github/workflows/run-unit-tests.yml
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3118 2024-03-17 16:59:19.000000 ingredient_slicer-1.0.3/.gitignore
+-rw-r--r--   0 anguswatters   (501) staff       (20)     1075 2024-03-17 16:52:34.000000 ingredient_slicer-1.0.3/LICENSE
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3362 2024-05-25 16:29:22.498879 ingredient_slicer-1.0.3/PKG-INFO
+-rw-r--r--   0 anguswatters   (501) staff       (20)     2389 2024-04-08 22:17:24.000000 ingredient_slicer-1.0.3/README.md
+drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-05-25 16:29:22.488133 ingredient_slicer-1.0.3/ingredient_slicer/
+-rw-r--r--   0 anguswatters   (501) staff       (20)     1725 2024-05-25 13:54:14.000000 ingredient_slicer-1.0.3/ingredient_slicer/__init__.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)   160805 2024-05-25 15:17:43.000000 ingredient_slicer-1.0.3/ingredient_slicer/_constants.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)   103245 2024-05-25 16:20:12.000000 ingredient_slicer-1.0.3/ingredient_slicer/_ingredient_slicer.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    91510 2024-05-25 15:48:42.000000 ingredient_slicer-1.0.3/ingredient_slicer/_regex_patterns.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)   108927 2024-05-25 16:27:13.000000 ingredient_slicer-1.0.3/ingredient_slicer/_utils.py
+drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-05-25 16:29:22.498208 ingredient_slicer-1.0.3/ingredient_slicer.egg-info/
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3362 2024-05-25 16:29:22.000000 ingredient_slicer-1.0.3/ingredient_slicer.egg-info/PKG-INFO
+-rw-r--r--   0 anguswatters   (501) staff       (20)     2156 2024-05-25 16:29:22.000000 ingredient_slicer-1.0.3/ingredient_slicer.egg-info/SOURCES.txt
+-rw-r--r--   0 anguswatters   (501) staff       (20)        1 2024-05-25 16:29:22.000000 ingredient_slicer-1.0.3/ingredient_slicer.egg-info/dependency_links.txt
+-rw-r--r--   0 anguswatters   (501) staff       (20)       38 2024-05-25 16:29:22.000000 ingredient_slicer-1.0.3/ingredient_slicer.egg-info/requires.txt
+-rw-r--r--   0 anguswatters   (501) staff       (20)       18 2024-05-25 16:29:22.000000 ingredient_slicer-1.0.3/ingredient_slicer.egg-info/top_level.txt
+-rw-r--r--   0 anguswatters   (501) staff       (20)     1124 2024-05-25 16:29:11.000000 ingredient_slicer-1.0.3/pyproject.toml
+-rw-r--r--   0 anguswatters   (501) staff       (20)       38 2024-05-25 16:29:22.499246 ingredient_slicer-1.0.3/setup.cfg
+drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-05-25 16:29:22.497952 ingredient_slicer-1.0.3/tests/
+-rw-r--r--   0 anguswatters   (501) staff       (20)        0 2024-04-06 13:59:44.000000 ingredient_slicer-1.0.3/tests/__init__.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     2402 2024-04-06 15:22:11.000000 ingredient_slicer-1.0.3/tests/test_avg_ranges.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     5566 2024-04-10 14:53:42.000000 ingredient_slicer-1.0.3/tests/test_casual_ingredients.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)        0 2024-04-06 15:22:03.000000 ingredient_slicer-1.0.3/tests/test_clean_hyphen_padded_substrings.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     5502 2024-04-06 15:27:00.000000 ingredient_slicer-1.0.3/tests/test_convert_fractions_to_decimals.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     2145 2024-04-06 15:27:01.000000 ingredient_slicer-1.0.3/tests/test_convert_volumes_to_milliliters.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     1182 2024-03-29 21:19:57.000000 ingredient_slicer-1.0.3/tests/test_duplicate_unit_ranges.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     8507 2024-03-29 21:18:52.000000 ingredient_slicer-1.0.3/tests/test_extract_dimensions.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3541 2024-03-29 21:19:50.000000 ingredient_slicer-1.0.3/tests/test_extract_quantities_utils.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3711 2024-03-29 21:19:48.000000 ingredient_slicer-1.0.3/tests/test_find_and_remove.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     2842 2024-03-29 21:19:52.000000 ingredient_slicer-1.0.3/tests/test_find_and_remove_hyphen_substrings.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3352 2024-04-06 13:59:33.000000 ingredient_slicer-1.0.3/tests/test_fraction_str_to_decimal.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    26160 2024-05-06 14:16:39.000000 ingredient_slicer-1.0.3/tests/test_get_gram_weight.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     2496 2024-05-06 15:32:33.000000 ingredient_slicer-1.0.3/tests/test_get_single_item_gram_weight.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    20386 2024-04-10 16:18:22.000000 ingredient_slicer-1.0.3/tests/test_ingredient_slicer.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3428 2024-04-08 13:04:03.000000 ingredient_slicer-1.0.3/tests/test_ingredient_slicer_dimensions.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     4771 2024-05-25 16:28:38.000000 ingredient_slicer-1.0.3/tests/test_ingredient_slicer_edge_case_foods.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     4899 2024-05-25 15:50:27.000000 ingredient_slicer-1.0.3/tests/test_ingredient_slicer_fraction_conversions.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     1903 2024-05-06 17:14:21.000000 ingredient_slicer-1.0.3/tests/test_ingredient_slicer_gram_weights.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     1515 2024-04-10 14:52:56.000000 ingredient_slicer-1.0.3/tests/test_ingredient_slicer_parenthesis.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     7502 2024-04-10 14:52:56.000000 ingredient_slicer-1.0.3/tests/test_ingredient_slicer_x_separators.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     4178 2024-04-10 14:52:54.000000 ingredient_slicer-1.0.3/tests/test_is_approximate_quantity_only_parenthesis.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     2965 2024-04-10 14:52:54.000000 ingredient_slicer-1.0.3/tests/test_make_int_or_float_str.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     2169 2024-04-06 15:26:57.000000 ingredient_slicer-1.0.3/tests/test_merge_misleading_ranges.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    14464 2024-03-29 21:19:43.000000 ingredient_slicer-1.0.3/tests/test_merge_numbers.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    45639 2024-05-25 15:12:12.000000 ingredient_slicer-1.0.3/tests/test_number_ranges.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    56318 2024-03-29 21:19:45.000000 ingredient_slicer-1.0.3/tests/test_number_ranges_separated_by_words.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     5652 2024-04-06 13:59:36.000000 ingredient_slicer-1.0.3/tests/test_numbers_with_inch_symbols.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    15368 2024-03-29 21:19:20.000000 ingredient_slicer-1.0.3/tests/test_parenthesis.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    11036 2024-04-10 14:53:13.000000 ingredient_slicer-1.0.3/tests/test_parenthesis_utils.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     2512 2024-03-29 21:19:22.000000 ingredient_slicer-1.0.3/tests/test_percentages.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3547 2024-03-29 21:19:26.000000 ingredient_slicer-1.0.3/tests/test_prefixed_number_words_regex.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     5013 2024-03-29 21:19:28.000000 ingredient_slicer-1.0.3/tests/test_prep_words.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     5261 2024-03-29 21:19:25.000000 ingredient_slicer-1.0.3/tests/test_quantity_range_regex.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    27045 2024-04-06 13:59:38.000000 ingredient_slicer-1.0.3/tests/test_quantity_units_regex.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3571 2024-04-06 13:31:28.000000 ingredient_slicer-1.0.3/tests/test_remove_repeat_units_in_ranges.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)      633 2024-03-29 21:19:14.000000 ingredient_slicer-1.0.3/tests/test_remove_x_separators.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     6384 2024-03-29 21:19:12.000000 ingredient_slicer-1.0.3/tests/test_replace_a_or_an_quantities.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     6869 2024-03-29 21:19:08.000000 ingredient_slicer-1.0.3/tests/test_separate_dimensions.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     1808 2024-03-29 21:19:42.000000 ingredient_slicer-1.0.3/tests/test_size_modifiers.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     8974 2024-03-29 21:19:39.000000 ingredient_slicer-1.0.3/tests/test_spaced_numbers.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     5838 2024-03-29 21:19:40.000000 ingredient_slicer-1.0.3/tests/test_unit_regex.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    16676 2024-04-06 15:22:15.000000 ingredient_slicer-1.0.3/tests/test_wild_ingredients.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     8022 2024-04-06 15:22:14.000000 ingredient_slicer-1.0.3/tests/test_word_fractions.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     7167 2024-03-29 21:19:33.000000 ingredient_slicer-1.0.3/tests/test_word_numbers.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     1337 2024-04-06 14:42:17.000000 ingredient_slicer-1.0.3/tests/test_x_after_number_regex.py
```

### Comparing `ingredient_slicer-1.0.2/.github/workflows/publish-to-pypi.yml` & `ingredient_slicer-1.0.3/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.2/.github/workflows/run-unit-tests.yml` & `ingredient_slicer-1.0.3/.github/workflows/run-unit-tests.yml`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.2/.gitignore` & `ingredient_slicer-1.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.2/LICENSE` & `ingredient_slicer-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.2/PKG-INFO` & `ingredient_slicer-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ingredient_slicer
-Version: 1.0.2
+Version: 1.0.3
 Summary: Parses unstructured recipe ingredient text into standardized quantities, units, and foods
 Author-email: Angus Watters <anguswatters@gmail.com>
 License: MIT License
 Keywords: ingredient,parser,recipe,text processing,food,cooking,grocery,shopping
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ingredient_slicer-1.0.2/README.md` & `ingredient_slicer-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.2/ingredient_slicer/__init__.py` & `ingredient_slicer-1.0.3/ingredient_slicer/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # __init__.py
 
-__version__ = "1.0.2"
+__version__ = "1.0.3"
 
 from ._ingredient_slicer import IngredientSlicer
 
 from ._constants import UNITS, WEIGHT_UNITS, VOLUME_UNITS, DIMENSION_UNITS, \
     CASUAL_UNITS, CASUAL_QUANTITIES, PREP_WORDS, \
     FOOD_CATALOG, FOOD_CATEGORIES, FOOD_DENSITY_BY_GROUP, \
     PRIMARY_CATEGORIES, SECONDARY_CATEGORIES, \
```

### Comparing `ingredient_slicer-1.0.2/ingredient_slicer/_constants.py` & `ingredient_slicer-1.0.3/ingredient_slicer/_constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -1185,42 +1185,42 @@
             "venison loins": ("meat_and_meat_products", "venison"),
             "venison tenderloin": ("meat_and_meat_products", "venison"),
             "venison tenderloins": ("meat_and_meat_products", "venison"),
             "venison shoulder": ("meat_and_meat_products", "venison"),
             "venison shoulders": ("meat_and_meat_products", "venison"),
 
             # -------------------------------------------------------------------------------------------------------
-            # ----- Meat substitutes, classified as misc. ("miscellaneous_foods") -----
+            # ----- Meat substitutes, classified as misc. ("legumes") -----
             # -------------------------------------------------------------------------------------------------------
 
             # TODO: Meat substitutes (not sure how to handle this as it relates to density groups)
-            "tofu": ("miscellaneous_foods", "meat substitute"),
-            "tofus": ("miscellaneous_foods", "meat substitute"),
-            "tofu block": ("miscellaneous_foods", "meat substitute"),
-            "tofu blocks": ("miscellaneous_foods", "meat substitute"),
-            "tofu burger": ("miscellaneous_foods", "meat substitute"),
-            "tofu burgers": ("miscellaneous_foods", "meat substitute"),
-            "tofu bacon": ("miscellaneous_foods", "meat substitute"),
-            "tempeh": ("miscellaneous_foods", "meat substitute"),
-            "seitan": ("miscellaneous_foods", "meat substitute"),
-            "soy protein": ("miscellaneous_foods", "meat substitute"),
-            "soy protein powder": ("miscellaneous_foods", "meat substitute"),
-            "soy protein isolate": ("miscellaneous_foods", "meat substitute"),
-            "pea protein": ("miscellaneous_foods", "meat substitute"),
-            "tofurkey": ("miscellaneous_foods", "meat substitute"),
-            "tofurkey sausage": ("miscellaneous_foods", "meat substitute"),
-            "tofurkey sausages": ("miscellaneous_foods", "meat substitute"),
-            "impossible burger": ("miscellaneous_foods", "meat substitute"),
-            "impossible burgers": ("miscellaneous_foods", "meat substitute"),
-            "impossible meat": ("miscellaneous_foods", "meat substitute"),
-            "impossible meats": ("miscellaneous_foods", "meat substitute"),
-            "impossible sausage": ("miscellaneous_foods", "meat substitute"),
-            "impossible sausages": ("miscellaneous_foods", "meat substitute"),
-            "beyond burger": ("miscellaneous_foods", "meat substitute"),
-            "beyond burgers": ("miscellaneous_foods", "meat substitute"),
+            "tofu": ("legumes", "meat substitute"),
+            "tofus": ("legumes", "meat substitute"),
+            "tofu block": ("legumes", "meat substitute"),
+            "tofu blocks": ("legumes", "meat substitute"),
+            "tofu burger": ("legumes", "meat substitute"),
+            "tofu burgers": ("legumes", "meat substitute"),
+            "tofu bacon": ("legumes", "meat substitute"),
+            "tempeh": ("legumes", "meat substitute"),
+            "seitan": ("legumes", "meat substitute"),
+            "soy protein": ("legumes", "meat substitute"),
+            "soy protein powder": ("legumes", "meat substitute"),
+            "soy protein isolate": ("legumes", "meat substitute"),
+            "pea protein": ("legumes", "meat substitute"),
+            "tofurkey": ("legumes", "meat substitute"),
+            "tofurkey sausage": ("legumes", "meat substitute"),
+            "tofurkey sausages": ("legumes", "meat substitute"),
+            "impossible burger": ("legumes", "meat substitute"),
+            "impossible burgers": ("legumes", "meat substitute"),
+            "impossible meat": ("legumes", "meat substitute"),
+            "impossible meats": ("legumes", "meat substitute"),
+            "impossible sausage": ("legumes", "meat substitute"),
+            "impossible sausages": ("legumes", "meat substitute"),
+            "beyond burger": ("legumes", "meat substitute"),
+            "beyond burgers": ("legumes", "meat substitute"),
 
             # -------------------------------------------------------------------------------------------------------
             # ----- Fish & Fish products ("fish_and_fish_products") -----
             # -------------------------------------------------------------------------------------------------------
 
             # SEAFOOD
             "salmon": ("fish_and_fish_products", "fish"),
@@ -1385,17 +1385,17 @@
             "lowfat cottage cheese": ("dairy_products", "cheese"),
             "yogurt": ("dairy_products", "yogurt"),
             "nonfat yogurt": ("dairy_products", "yogurt"),
             "lowfat yogurt": ("dairy_products", "yogurt"),
             "greek yogurt": ("dairy_products", "yogurt"),
             "nonfat greek yogurt": ("dairy_products", "yogurt"),
             "lowfat greek yogurt": ("dairy_products", "yogurt"),
-            "sour cream": ("dairy_products", "miscellaneous_foods"),
-            "light sour cream": ("dairy_products", "miscellaneous_foods"),
-            "heavy cream": ("dairy_products", "miscellaneous_foods"),
+            "sour cream": ("dairy_products", "sour cream"),
+            "light sour cream": ("dairy_products", "sour cream"),
+            "heavy cream": ("dairy_products", "cream"),
             "ice cream": ("dairy_products", "ice cream"),
             "vanilla ice cream": ("dairy_products", "ice cream"),
             "chocolate ice cream": ("dairy_products", "ice cream"),
 
             # -------------------------------------------------------------------------------------------------------
             # ----- GRAINS ("cereal_and_cereal_products") -----
             # -------------------------------------------------------------------------------------------------------
@@ -1535,60 +1535,60 @@
             "cornstarch": ("cereal_and_cereal_products", "flour"),
             "corn starch": ("cereal_and_cereal_products", "flour"),
             "cornmeal": ("cereal_and_cereal_products", "flour"),
             "corn meal": ("cereal_and_cereal_products", "flour"),
             "oat flour": ("cereal_and_cereal_products", "flour"),
             "oat bran": ("cereal_and_cereal_products", "flour"),
             "almond flour": ("cereal_and_cereal_products", "flour"),
-            "cake": ("cereal_and_cereal_products", "miscellaneous_foods"),
+            # "cake": ("cereal_and_cereal_products", "flour"), # TODO: moved to baked_goods
             "cake mix": ("cereal_and_cereal_products", "flour"),
-            "dough": ("cereal_and_cereal_products", "miscellaneous_foods"),
-            "dough mix": ("cereal_and_cereal_products", "miscellaneous_foods"),
+            "dough": ("cereal_and_cereal_products", "flour"),
+            "dough mix": ("cereal_and_cereal_products", "flour"),
             "toast": ("cereal_and_cereal_products", "bread"),
             "toasts" : ("cereal_and_cereal_products", "bread"),
             "toasts bread": ("cereal_and_cereal_products", "bread"),
             "toasted bread": ("cereal_and_cereal_products", "bread"),
-            "cracker" : ("cereal_and_cereal_products", "miscellaneous_foods"),
-            "crackers" : ("cereal_and_cereal_products", "miscellaneous_foods"),
+            "cracker" : ("cereal_and_cereal_products", "cracker"),
+            "crackers" : ("cereal_and_cereal_products", "cracker"),
             # -------------------------------------------------------------------------------------------------------
             # ----- Nuts and Seeds ("nuts_and_seeds") -----
             # -------------------------------------------------------------------------------------------------------
 
             # NUTS
-            "almond": ("nuts_and_seeds", "miscellaneous_foods"),
-            "almonds": ("nuts_and_seeds", "miscellaneous_foods"),
-            "roasted almond": ("nuts_and_seeds", "miscellaneous_foods"),
-            "roasted almonds": ("nuts_and_seeds", "miscellaneous_foods"),
-            "peanut": ("nuts_and_seeds", "miscellaneous_foods"),
-            "peanuts": ("nuts_and_seeds", "miscellaneous_foods"),
-            "roasted peanut": ("nuts_and_seeds", "miscellaneous_foods"),
-            "roasted peanuts": ("nuts_and_seeds", "miscellaneous_foods"),
-            "unsalted peanut": ("nuts_and_seeds", "miscellaneous_foods"),
-            "unsalted peanuts": ("nuts_and_seeds", "miscellaneous_foods"),
-            "salted peanut": ("nuts_and_seeds", "miscellaneous_foods"),
-            "salted peanuts": ("nuts_and_seeds", "miscellaneous_foods"),
-            "cashew": ("nuts_and_seeds", "miscellaneous_foods"),
-            "cashews": ("nuts_and_seeds", "miscellaneous_foods"),
-            "pisatchio": ("nuts_and_seeds", "miscellaneous_foods"),
-            "pistachios": ("nuts_and_seeds", "miscellaneous_foods"),
-            "macadamia": ("nuts_and_seeds", "miscellaneous_foods"),
-            "macadamia nut": ("nuts_and_seeds", "miscellaneous_foods"),
-            "macadamia nuts": ("nuts_and_seeds", "miscellaneous_foods"),
-            "hazelnut": ("nuts_and_seeds", "miscellaneous_foods"),
-            "hazelnuts": ("nuts_and_seeds", "miscellaneous_foods"),
-            "chestnut": ("nuts_and_seeds", "miscellaneous_foods"),
-            "chestnuts": ("nuts_and_seeds", "miscellaneous_foods"),
-            "pine nut": ("nuts_and_seeds", "miscellaneous_foods"),
-            "pine nuts": ("nuts_and_seeds", "miscellaneous_foods"),
-            "brazil nut": ("nuts_and_seeds", "miscellaneous_foods"),
-            "brazil nuts": ("nuts_and_seeds", "miscellaneous_foods"),
-            "walnut": ("nuts_and_seeds", "miscellaneous_foods"),
-            "walnuts": ("nuts_and_seeds", "miscellaneous_foods"),
-            "pecan": ("nuts_and_seeds", "miscellaneous_foods"),
-            "pecans": ("nuts_and_seeds", "miscellaneous_foods"),
+            "almond": ("nuts_and_seeds", "nut"),
+            "almonds": ("nuts_and_seeds", "nut"),
+            "roasted almond": ("nuts_and_seeds", "nut"),
+            "roasted almonds": ("nuts_and_seeds", "nut"),
+            "peanut": ("nuts_and_seeds", "nut"),
+            "peanuts": ("nuts_and_seeds", "nut"),
+            "roasted peanut": ("nuts_and_seeds", "nut"),
+            "roasted peanuts": ("nuts_and_seeds", "nut"),
+            "unsalted peanut": ("nuts_and_seeds", "nut"),
+            "unsalted peanuts": ("nuts_and_seeds", "nut"),
+            "salted peanut": ("nuts_and_seeds", "nut"),
+            "salted peanuts": ("nuts_and_seeds", "nut"),
+            "cashew": ("nuts_and_seeds", "nut"),
+            "cashews": ("nuts_and_seeds", "nut"),
+            "pisatchio": ("nuts_and_seeds", "nut"),
+            "pistachios": ("nuts_and_seeds", "nut"),
+            "macadamia": ("nuts_and_seeds", "nut"),
+            "macadamia nut": ("nuts_and_seeds", "nut"),
+            "macadamia nuts": ("nuts_and_seeds", "nut"),
+            "hazelnut": ("nuts_and_seeds", "nut"),
+            "hazelnuts": ("nuts_and_seeds", "nut"),
+            "chestnut": ("nuts_and_seeds", "nut"),
+            "chestnuts": ("nuts_and_seeds", "nut"),
+            "pine nut": ("nuts_and_seeds", "nut"),
+            "pine nuts": ("nuts_and_seeds", "nut"),
+            "brazil nut": ("nuts_and_seeds", "nut"),
+            "brazil nuts": ("nuts_and_seeds", "nut"),
+            "walnut": ("nuts_and_seeds", "nut"),
+            "walnuts": ("nuts_and_seeds", "nut"),
+            "pecan": ("nuts_and_seeds", "nut"),
+            "pecans": ("nuts_and_seeds", "nut"),
             "peanut butter": ("nuts_and_seeds", "nut butter"),
             "almond butter": ("nuts_and_seeds", "nut butter"),
             "cashew butter": ("nuts_and_seeds", "nut butter"),
             "pumpkin seed": ("nuts_and_seeds", "seed"),
             "pumpkin seeds": ("nuts_and_seeds", "seed"),
             "sunflower seed": ("nuts_and_seeds", "seed"),
             "sunflower seeds": ("nuts_and_seeds", "seed"),
@@ -1596,66 +1596,66 @@
             "sesame seeds": ("nuts_and_seeds", "seed"),
 
             # -------------------------------------------------------------------------------------------------------
             # ----- Oils ("oils") -----
             # -------------------------------------------------------------------------------------------------------
 
             # OILS
-            "vegetable oil": ("oils", "vegetable-based"),
-            "sesame oil": ("oils", "seed-based"),
-            "sunflower oil": ("oils", "seed-based"),
-            "canola oil": ("oils", "seed-based"),
-            "olive oil": ("oils", "vegetable-based"),
-            "coconut oil": ("oils", "vegetable-based"),
-            "avocado oil": ("oils", "vegetable-based"),
-            "extra virgin olive oil": ("oils", "vegetable-based"),
-            "peanut oil": ("oils", "seed-based"),
-            "truffle oil": ("oils", "vegetable-based"),
-            "chili oil": ("oils", "vegetable-based"),
-            "salmon oil": ("oils", "animal-based"),
-            "wild alaskan salmon oil": ("oils", "animal-based"),
-            "cod liver oil": ("oils", "animal-based"),
-            "omega-3 oil": ("oils", "animal-based"),
-            "fish oil": ("oils", "animal-based"),
-            "omega-3 fish oil": ("oils", "animal-based"),
+            "vegetable oil": ("oils", "vegetable_based"),
+            "sesame oil": ("oils", "seed_based"),
+            "sunflower oil": ("oils", "seed_based"),
+            "canola oil": ("oils", "seed_based"),
+            "olive oil": ("oils", "vegetable_based"),
+            "coconut oil": ("oils", "vegetable_based"),
+            "avocado oil": ("oils", "vegetable_based"),
+            "extra virgin olive oil": ("oils", "vegetable_based"),
+            "peanut oil": ("oils", "seed_based"),
+            "truffle oil": ("oils", "vegetable_based"),
+            "chili oil": ("oils", "vegetable_based"),
+            "salmon oil": ("oils", "animal_based"),
+            "wild alaskan salmon oil": ("oils", "animal_based"),
+            "cod liver oil": ("oils", "animal_based"),
+            "omega-3 oil": ("oils", "animal_based"),
+            "fish oil": ("oils", "animal_based"),
+            "omega-3 fish oil": ("oils", "animal_based"),
             "cooking spray": ("oils", "cooking spray"),
 
             # -------------------------------------------------------------------------------------------------------
             # ----- Fats ("fats_and_other") -----
             # -------------------------------------------------------------------------------------------------------
 
-            "lard": ("fats_and_other", "animal-based"),
-            "duck fat": ("fats_and_other", "animal-based"),
-            "goose fat": ("fats_and_other", "animal-based"),
-            "tallow": ("fats_and_other", "animal-based"),
-            "beef tallow": ("fats_and_other", "animal-based"),
-            "chicken fat": ("fats_and_other", "animal-based"),
-            "ghee": ("fats_and_other", "animal-based"),
-            "suet": ("fats_and_other", "animal-based"),
-            "grass-fed ghee": ("fats_and_other", "animal-based"),
-            "grassfed ghee": ("fats_and_other", "animal-based"),
-            "grass fed ghee": ("fats_and_other", "animal-based"),
-            "mayonnaise": ("fats_and_other", "condiment/sauce"),
-            "light mayonnaise": ("fats_and_other", "condiment/sauce"),
-            "lowfat mayonnaise": ("fats_and_other", "condiment/sauce"),
-            "low-fat mayonnaise": ("fats_and_other", "condiment/sauce"),
-            "low fat mayonnaise": ("fats_and_other", "condiment/sauce"),
-            "fat-free mayonnaise": ("fats_and_other", "condiment/sauce"),
-            "fat free mayonnaise": ("fats_and_other", "condiment/sauce"),
-            "mayo": ("fats_and_other", "condiment/sauce"),
-            "light mayo": ("fats_and_other", "condiment/sauce"),
-            "lowfat mayo": ("fats_and_other", "condiment/sauce"),
-            "low-fat mayo": ("fats_and_other", "condiment/sauce"),
-            "low fat mayo": ("fats_and_other", "condiment/sauce"),
-            "fat-free mayo": ("fats_and_other", "condiment/sauce"),
-            "fat free mayo": ("fats_and_other", "condiment/sauce"),
-            "miracle whip": ("fats_and_other", "condiment/sauce"),
-            "miracle whip light": ("fats_and_other", "condiment/sauce"),
-            "miracle whip fat-free": ("fats_and_other", "condiment/sauce"),
-            "miracle whip lowfat": ("fats_and_other", "condiment/sauce"),
+            "lard": ("fats_and_other", "animal_based"),
+            "duck fat": ("fats_and_other", "animal_based"),
+            "goose fat": ("fats_and_other", "animal_based"),
+            "tallow": ("fats_and_other", "animal_based"),
+            "beef tallow": ("fats_and_other", "animal_based"),
+            "chicken fat": ("fats_and_other", "animal_based"),
+            "ghee": ("fats_and_other", "animal_based"),
+            "suet": ("fats_and_other", "animal_based"),
+            "grass-fed ghee": ("fats_and_other", "animal_based"),
+            "grassfed ghee": ("fats_and_other", "animal_based"),
+            "grass fed ghee": ("fats_and_other", "animal_based"),
+            "mayonnaise": ("fats_and_other", "condiment_sauce"),
+            "light mayonnaise": ("fats_and_other", "condiment_sauce"),
+            "lowfat mayonnaise": ("fats_and_other", "condiment_sauce"),
+            "low-fat mayonnaise": ("fats_and_other", "condiment_sauce"),
+            "low fat mayonnaise": ("fats_and_other", "condiment_sauce"),
+            "fat-free mayonnaise": ("fats_and_other", "condiment_sauce"),
+            "fat free mayonnaise": ("fats_and_other", "condiment_sauce"),
+            "mayo": ("fats_and_other", "condiment_sauce"),
+            "light mayo": ("fats_and_other", "condiment_sauce"),
+            "lowfat mayo": ("fats_and_other", "condiment_sauce"),
+            "low-fat mayo": ("fats_and_other", "condiment_sauce"),
+            "low fat mayo": ("fats_and_other", "condiment_sauce"),
+            "fat-free mayo": ("fats_and_other", "condiment_sauce"),
+            "fat free mayo": ("fats_and_other", "condiment_sauce"),
+            "miracle whip": ("fats_and_other", "condiment_sauce"),
+            "miracle whip light": ("fats_and_other", "condiment_sauce"),
+            "miracle whip fat-free": ("fats_and_other", "condiment_sauce"),
+            "miracle whip lowfat": ("fats_and_other", "condiment_sauce"),
 
             # -------------------------------------------------------------------------------------------------------
             # ----- Herbs & Spices ("herbes_and_spices") -----
             # -------------------------------------------------------------------------------------------------------
 
             # SPICES
             "salt": ("herbes_and_spices", "salt"),
@@ -1670,38 +1670,38 @@
             "garlic salt": ("herbes_and_spices", "salt"),
             "onion salt": ("herbes_and_spices", "salt"),
             "cinnamon": ("herbes_and_spices", "bark"),
             "cinnamon stick": ("herbes_and_spices", "bark"),
             "cinnamon sticks": ("herbes_and_spices", "bark"),
             "cinnamon powder": ("herbes_and_spices", "bark"),
             "ground cinnamon": ("herbes_and_spices", "bark"),
-            "cumin": ("herbes_and_spices", "miscellaneous_foods"),
-            "coriander": ("herbes_and_spices", "miscellaneous_foods"),
-            "paprika": ("herbes_and_spices", "miscellaneous_foods"),
-            "cayenne": ("herbes_and_spices", "miscellaneous_foods"),
-            "chili powder": ("herbes_and_spices", "miscellaneous_foods"),
-            "curry powder": ("herbes_and_spices", "miscellaneous_foods"),
-            "turmeric": ("herbes_and_spices", "miscellaneous_foods"),
+            "cumin": ("herbes_and_spices", "spice"),
+            "coriander": ("herbes_and_spices", "spice"),
+            "paprika": ("herbes_and_spices", "spice"),
+            "cayenne": ("herbes_and_spices", "spice"),
+            "chili powder": ("herbes_and_spices", "spice"),
+            "curry powder": ("herbes_and_spices", "spice"),
+            "turmeric": ("herbes_and_spices", "spice"),
             "ginger": ("herbes_and_spices", "herb"),
-            "nutmeg": ("herbes_and_spices", "miscellaneous_foods"),
-            "cloves": ("herbes_and_spices", "miscellaneous_foods"),
-            "allspice": ("herbes_and_spices", "miscellaneous_foods"),
-            "cardamom": ("herbes_and_spices", "miscellaneous_foods"),
+            "nutmeg": ("herbes_and_spices", "spice"),
+            "cloves": ("herbes_and_spices", "spice"),
+            "allspice": ("herbes_and_spices", "spice"),
+            "cardamom": ("herbes_and_spices", "spice"),
             "oregano": ("herbes_and_spices", "herb"),
             "thyme": ("herbes_and_spices", "herb"),
             "rosemary": ("herbes_and_spices", "herb"),
             "sage": ("herbes_and_spices", "herb"),
             "basil": ("herbes_and_spices", "herb"),
             "mint": ("herbes_and_spices", "herb"),
             "parsley": ("herbes_and_spices", "herb"),
             "cilantro": ("herbes_and_spices", "herb"),
             "dill": ("herbes_and_spices", "herb"),
             "tarragon": ("herbes_and_spices", "herb"),
-            "garlic powder": ("herbes_and_spices", "miscellaneous_foods"),
-            "onion powder": ("herbes_and_spices", "miscellaneous_foods"),
+            "garlic powder": ("herbes_and_spices", "spice"),
+            "onion powder": ("herbes_and_spices", "spice"),
             "cayenne pepper": ("herbes_and_spices", "pepper"),
             "lemon pepper": ("herbes_and_spices", "pepper"),
             "fresh tarragon": ("herbes_and_spices", "herb"),
             "pepper": ("herbes_and_spices", "pepper"),
             "ground pepper": ("herbes_and_spices", "pepper"),
             "black pepper": ("herbes_and_spices", "pepper"),
             "ground black pepper": ("herbes_and_spices", "pepper"),
@@ -1764,42 +1764,42 @@
             "peaches": ("fruits", "stone"),
             "plum": ("fruits", "stone"),
             "plums": ("fruits", "stone"),
             "apricot": ("fruits", "stone"),
             "apricots": ("fruits", "stone"),
             "cherry": ("fruits", "stone"),
             "cherries": ("fruits", "stone"),
-            "fig": ("fruits", "miscellaneous_foods"),
-            "figs": ("fruits", "miscellaneous_foods"),
-            "date": ("fruits", "miscellaneous_foods"),
-            "dates": ("fruits", "miscellaneous_foods"),
-            "pomegranate": ("fruits", "miscellaneous_foods"),
-            "pomegranates": ("fruits", "miscellaneous_foods"),
-            "coconut": ("fruits", "miscellaneous_foods"),
-            "coconuts": ("fruits", "miscellaneous_foods"),
-            "passion fruit": ("fruits", "miscellaneous_foods"),
-            "passion fruits": ("fruits", "miscellaneous_foods"),
-            "dragon fruit": ("fruits", "miscellaneous_foods"),
-            "dragon fruits": ("fruits", "miscellaneous_foods"),
-            "guava": ("fruits", "miscellaneous_foods"),
-            "guavas": ("fruits", "miscellaneous_foods"),
-            "star fruit": ("fruits", "miscellaneous_foods"),
-            "star fruits": ("fruits", "miscellaneous_foods"),
-            "lychee": ("fruits", "miscellaneous_foods"),
-            "lychees": ("fruits", "miscellaneous_foods"),
-            "persimmon": ("fruits", "miscellaneous_foods"),
-            "persimmons": ("fruits", "miscellaneous_foods"),
+            "fig": ("fruits", "fig"),
+            "figs": ("fruits", "fig"),
+            "date": ("fruits", "date"),
+            "dates": ("fruits", "date"),
+            "pomegranate": ("fruits", "tropical"),
+            "pomegranates": ("fruits", "tropical"),
+            "coconut": ("fruits", "tropical"),
+            "coconuts": ("fruits", "tropical"),
+            "passion fruit": ("fruits", "tropical"),
+            "passion fruits": ("fruits", "tropical"),
+            "dragon fruit": ("fruits", "tropical"),
+            "dragon fruits": ("fruits", "tropical"),
+            "guava": ("fruits", "tropical"),
+            "guavas": ("fruits", "tropical"),
+            "star fruit": ("fruits", "tropical"),
+            "star fruits": ("fruits", "tropical"),
+            "lychee": ("fruits", "tropical"),
+            "lychees": ("fruits", "tropical"),
+            "persimmon": ("fruits", "berry"),
+            "persimmons": ("fruits", "berry"),
             "papaya": ("fruits", "tropical"),
             "papayas": ("fruits", "tropical"),
             "cranberry": ("fruits", "berry"),
             "cranberries": ("fruits", "berry"),
-            "raisin": ("fruits", "miscellaneous_foods"),
-            "raisins": ("fruits", "miscellaneous_foods"),
-            "prune": ("fruits", "miscellaneous_foods"),
-            "prunes": ("fruits", "miscellaneous_foods"),
+            "raisin": ("fruits", "grape"),
+            "raisins": ("fruits", "grape"),
+            "prune": ("fruits", "drupe"),
+            "prunes": ("fruits", "drupe"),
             "currant": ("fruits", "berry"),
             "currants": ("fruits", "berry"),
             "elderberry": ("fruits", "berry"),
             "elderberries": ("fruits", "berry"),
             "goji berry": ("fruits", "berry"),
             "goji berries": ("fruits", "berry"),
             "acai": ("fruits", "berry"),
@@ -1942,60 +1942,61 @@
 
             # -------------------------------------------------------------------------------------------------------
             # ----- Misc foods, condiments, sauces ("miscellaneous_foods") -----
             # -------------------------------------------------------------------------------------------------------
 
             # miscellaneous_foods 
             # CONDIMENTS/SAUCES
-            "vinegar": ("miscellaneous_foods", "vinegar"),
-            "white wine vinegar": ("miscellaneous_foods", "vinegar"),
-            "balsamic vinegar": ("miscellaneous_foods", "vinegar"),
-            "red wine vinegar": ("miscellaneous_foods", "vinegar"),
-            "apple cider vinegar": ("miscellaneous_foods", "vinegar"),
-            "distilled vinegar": ("miscellaneous_foods", "vinegar"),
-            "rice vinegar": ("miscellaneous_foods", "vinegar"),
-            "white vinegar": ("miscellaneous_foods", "vinegar"),
-            "fish sauce": ("miscellaneous_foods", "condiment/sauce"),
-            "ketchup": ("miscellaneous_foods", "condiment/sauce"),
-            "reduced-sugar ketchup": ("miscellaneous_foods", "condiment/sauce"),
-            "reduced sugar ketchup": ("miscellaneous_foods", "condiment/sauce"),
-            "low-sugar ketchup": ("miscellaneous_foods", "condiment/sauce"),
-            "low sugar ketchup": ("miscellaneous_foods", "condiment/sauce"),
-            "sugar-free ketchup": ("miscellaneous_foods", "condiment/sauce"),
-            "sugar free ketchup": ("miscellaneous_foods", "condiment/sauce"),
-            "low-sodium ketchup": ("miscellaneous_foods", "condiment/sauce"),
-            "low sodium ketchup": ("miscellaneous_foods", "condiment/sauce"),
-            "sodium-free ketchup": ("miscellaneous_foods", "condiment/sauce"),
-            "sodium free ketchup": ("miscellaneous_foods", "condiment/sauce"),
-            "relish": ("miscellaneous_foods", "condiment/sauce"),
-            "mustard": ("miscellaneous_foods", "condiment/sauce"),
-            "dijon mustard": ("miscellaneous_foods", "condiment/sauce"),
-            "yellow mustard": ("miscellaneous_foods", "condiment/sauce"),
-            "honey mustard": ("miscellaneous_foods", "condiment/sauce"),
-            "soy sauce": ("miscellaneous_foods", "condiment/sauce"),
-            "BBQ sauce": ("miscellaneous_foods", "condiment/sauce"),
-            "bbq sauce": ("miscellaneous_foods", "condiment/sauce"),
-            "barbecue sauce": ("miscellaneous_foods", "condiment/sauce"),
-            "hot sauce": ("miscellaneous_foods", "condiment/sauce"),
-            "sriracha": ("miscellaneous_foods", "condiment/sauce"),
-            "salsa": ("miscellaneous_foods", "condiment/sauce"),
+            "vinegar": ("sauces_and_gravies", "vinegar"),
+            "white wine vinegar": ("sauces_and_gravies", "vinegar"),
+            "balsamic vinegar": ("sauces_and_gravies", "vinegar"),
+            "red wine vinegar": ("sauces_and_gravies", "vinegar"),
+            "apple cider vinegar": ("sauces_and_gravies", "vinegar"),
+            "distilled vinegar": ("sauces_and_gravies", "vinegar"),
+            "rice vinegar": ("sauces_and_gravies", "vinegar"),
+            "white vinegar": ("sauces_and_gravies", "vinegar"),
+            "fish sauce": ("sauces_and_gravies", "condiment_sauce"),
+            "ketchup": ("sauces_and_gravies", "condiment_sauce"),
+            "reduced-sugar ketchup": ("sauces_and_gravies", "condiment_sauce"),
+            "reduced sugar ketchup": ("sauces_and_gravies", "condiment_sauce"),
+            "low-sugar ketchup": ("sauces_and_gravies", "condiment_sauce"),
+            "low sugar ketchup": ("sauces_and_gravies", "condiment_sauce"),
+            "sugar-free ketchup": ("sauces_and_gravies", "condiment_sauce"),
+            "sugar free ketchup": ("sauces_and_gravies", "condiment_sauce"),
+            "low-sodium ketchup": ("sauces_and_gravies", "condiment_sauce"),
+            "low sodium ketchup": ("sauces_and_gravies", "condiment_sauce"),
+            "sodium-free ketchup": ("sauces_and_gravies", "condiment_sauce"),
+            "sodium free ketchup": ("sauces_and_gravies", "condiment_sauce"),
+            "relish": ("sauces_and_gravies", "condiment_sauce"),
+            "mustard": ("sauces_and_gravies", "condiment_sauce"),
+            "dijon mustard": ("sauces_and_gravies", "condiment_sauce"),
+            "yellow mustard": ("sauces_and_gravies", "condiment_sauce"),
+            "honey mustard": ("sauces_and_gravies", "condiment_sauce"),
+            "soy sauce": ("sauces_and_gravies", "condiment_sauce"),
+            "BBQ sauce": ("sauces_and_gravies", "condiment_sauce"),
+            "bbq sauce": ("sauces_and_gravies", "condiment_sauce"),
+            "barbecue sauce": ("sauces_and_gravies", "condiment_sauce"),
+            "hot sauce": ("sauces_and_gravies", "condiment_sauce"),
+            "sriracha": ("sauces_and_gravies", "condiment_sauce"),
+            "salsa": ("sauces_and_gravies", "condiment_sauce"),
             
             # Salad dressing 
-            "ranch": ("miscellaneous_foods", "salad dressing"),
-            "ranch dressing": ("miscellaneous_foods", "salad dressing"),
-            "caesar dressing": ("miscellaneous_foods", "salad dressing"),
-            "thousand island dressing": ("miscellaneous_foods", "salad dressing"),
-            "blue cheese dressing": ("miscellaneous_foods", "salad dressing"),
-            "italian dressing": ("miscellaneous_foods", "salad dressing"),
-            "vinaigrette": ("miscellaneous_foods", "salad dressing"),
-            "vinaigrette dressing": ("miscellaneous_foods", "salad dressing"),
-            "sesame dressing": ("miscellaneous_foods", "salad dressing"),
-            "honey mustard dressing": ("miscellaneous_foods", "salad dressing"),
-            "balsamic dressing": ("miscellaneous_foods", "salad dressing"),
-            "balsamic vinaigrette": ("miscellaneous_foods", "salad dressing"),
+            "ranch": ("fats_and_other", "salad dressing"),
+            "ranch dressing": ("fats_and_other", "salad dressing"),
+            "caesar dressing": ("fats_and_other", "salad dressing"),
+            "thousand island dressing": ("fats_and_other", "salad dressing"),
+            "blue cheese dressing": ("fats_and_other", "salad dressing"),
+            "italian dressing": ("fats_and_other", "salad dressing"),
+            "vinaigrette": ("fats_and_other", "salad dressing"),
+            "vinaigrette dressing": ("fats_and_other", "salad dressing"),
+            "sesame dressing": ("fats_and_other", "salad dressing"),
+            "honey mustard dressing": ("fats_and_other", "salad dressing"),
+            "balsamic dressing": ("fats_and_other", "salad dressing"),
+            "balsamic vinaigrette": ("fats_and_other", "salad dressing"),
+
             # -------------------------------------------------------------------------------------------------------
             # ----- Sweets, sugars ("sweets") -----
             # -------------------------------------------------------------------------------------------------------
 
             # SWEETENERS
             "sugar": ("sweets", "sugar"),
             "brown sugar": ("sweets", "sugar"),
@@ -2023,20 +2024,25 @@
             "sorbitol": ("sweets", "sugar alcohol"),
             "maltitol": ("sweets", "sugar alcohol"),
             "chocolate chips": ("sweets", "chocolate"),
             "chocolate": ("sweets", "chocolate"),
             "white chocolate": ("sweets", "chocolate"),
             "dark chocolate": ("sweets", "chocolate"),
             "milk chocolate": ("sweets", "chocolate"),
+            "baking chocolate": ("sweets", "chocolate"),
             "cocoa": ("sweets", "chocolate"),
             "ladyfinger": ("sweets", "cookie"),
             "ladysfingers": ("sweets", "cookie"),
             "ladyfingers": ("sweets", "cookie"),
 
-            # SYRUPS
+
+            # -------------------------------------------------------------------------------------------------------
+            # ----- SYRUPS ("syrups") -----
+            # -------------------------------------------------------------------------------------------------------
+
             "corn syrup": ("syrups", "syrup"),
             "high fructose corn syrup": ("syrups", "syrup"),
             "honey": ("syrups", "honey"),
             "organic honey": ("syrups", "honey"),
             "maple syrup": ("syrups", "syrup"),
             "maple sugar": ("syrups", "sugar"),
             "agave": ("syrups", "nectar"),
@@ -2084,47 +2090,135 @@
             "strawberry marmalade" : ("syrups", "syrup"),
             "blueberry marmalade" : ("syrups", "syrup"),
             "blackberry marmalade" : ("syrups", "syrup"),
             "peach marmalade" : ("syrups", "syrup"),
             "raspberry marmalade" : ("syrups", "syrup"),
             "fruit preserves" : ("syrups", "syrup"),
 
+            # -------------------------------------------------------------------------------------------------------
+            # ----- SNACKS ("snacks") -----
+            # -------------------------------------------------------------------------------------------------------
             # SNACKS
-            "potato chip": ("snacks", "miscellaneous_foods"),
-            "potato chips": ("snacks", "miscellaneous_foods"),
-            "puff chip": ("snacks", "miscellaneous_foods"),
-            "puff chips": ("snacks", "miscellaneous_foods"),
-            "tortilla chip": ("snacks", "miscellaneous_foods"),
-            "tortilla chips": ("snacks", "miscellaneous_foods"),
-            "corn chip": ("snacks", "miscellaneous_foods"),
-            "corn chips": ("snacks", "miscellaneous_foods"),
-            "wonton" : ("snacks", "miscellaneous_foods"),
-            "wontons" : ("snacks", "miscellaneous_foods"),
-            "wonton chip": ("snacks", "miscellaneous_foods"),
-            "wonton chips": ("snacks", "miscellaneous_foods"),
-            "pretzel stick": ("snacks", "miscellaneous_foods"),
-            "pretzel sticks": ("snacks", "miscellaneous_foods"),
-            "pretzel": ("snacks", "miscellaneous_foods"),
-            "pretzels": ("snacks", "miscellaneous_foods"),
-            "popcorn": ("snacks", "miscellaneous_foods"),
-            "popcorn kernel": ("snacks", "miscellaneous_foods"),
-            "popcorn kernels": ("snacks", "miscellaneous_foods"),
+            "potato chip": ("snacks", "chip"),
+            "potato chips": ("snacks", "chip"),
+            "puff chip": ("snacks", "chip"),
+            "puff chips": ("snacks", "chip"),
+            "tortilla chip": ("snacks", "chip"),
+            "tortilla chips": ("snacks", "chip"),
+            "corn chip": ("snacks", "chip"),
+            "corn chips": ("snacks", "chip"),
+            "wonton" : ("snacks", "chip"),
+            "wontons" : ("snacks", "chip"),
+            "wonton chip": ("snacks", "chip"),
+            "wonton chips": ("snacks", "chip"),
+            "pretzel stick": ("snacks", "chip"),
+            "pretzel sticks": ("snacks", "chip"),
+            "pretzel": ("snacks", "chip"),
+            "pretzels": ("snacks", "chip"),
+            "popcorn": ("snacks", "chip"),
+            "popcorn kernel": ("snacks", "chip"),
+            "popcorn kernels": ("snacks", "chip"),
 
+            # -------------------------------------------------------------------------------------------------------
+            # ----- Mixed dishes ("mixed_dishes") -----
+            # -------------------------------------------------------------------------------------------------------
+            
             # Mixed dishes
-            "pizza": ("mixed_dishes", "miscellaneous_foods"),
+            "pizza": ("mixed_dishes", "mixed_dish"),
 
-            # Miscllaneous foods (baking)
-            "baking sheets": ("miscellaneous_foods", "baking"),
-            "baking powder": ("miscellaneous_foods", "baking"),
-            "baking soda": ("miscellaneous_foods", "baking"),
-            "yeast": ("miscellaneous_foods", "baking"),
-            "baking yeast": ("miscellaneous_foods", "baking"),
-            "active dry yeast": ("miscellaneous_foods", "baking"),
-            "instant yeast": ("miscellaneous_foods", "baking"),
-            "baking chocolate": ("miscellaneous_foods", "baking")
+            # -------------------------------------------------------------------------------------------------------
+            # ----- Baked goods ("baked_goods") -----
+            # -------------------------------------------------------------------------------------------------------
+            
+            # Baked goods
+            "muffin" : ("baked_goods", "pastry"),
+            "muffins" : ("baked_goods", "pastry"),
+            "croissant" : ("baked_goods", "pastry"),
+            "croissants" : ("baked_goods", "pastry"),
+            "almond croissant" : ("baked_goods", "pastry"),
+            "almond croissants" : ("baked_goods", "pastry"),
+            "chocolate croissant" : ("baked_goods", "pastry"),
+            "chocolate croissants" : ("baked_goods", "pastry"),
+            "bear claw" : ("baked_goods", "pastry"),
+            "bear claws" : ("baked_goods", "pastry"),
+            "cinnamon roll" : ("baked_goods", "pastry"),
+            "cinnamon rolls" : ("baked_goods", "pastry"),
+            "cinammon bun" : ("baked_goods", "pastry"),
+            "cinammon buns" : ("baked_goods", "pastry"),
+            "danish" : ("baked_goods", "pastry"),
+            "danishes" : ("baked_goods", "pastry"),
+            "scone" : ("baked_goods", "pastry"),
+            "scones" : ("baked_goods", "pastry"),
+            "donut" : ("baked_goods", "pastry"),
+            "donuts" : ("baked_goods", "pastry"),
+            "donut hole" : ("baked_goods", "pastry"),
+            "donut holes" : ("baked_goods", "pastry"),
+            "doughnut" : ("baked_goods", "pastry"),
+            "doughnuts" : ("baked_goods", "pastry"),
+            "doughnut hole" : ("baked_goods", "pastry"),
+            "doughnut holes" : ("baked_goods", "pastry"),
+
+            "cookie" : ("baked_goods", "cookie"),
+            "cookies" : ("baked_goods", "cookie"),
+            "molasses cookie" : ("baked_goods", "cookie"),
+            "molasses cookies" : ("baked_goods", "cookie"),
+            "chocolate chip cookie" : ("baked_goods", "cookie"),
+            "chocolate chip cookies" : ("baked_goods", "cookie"),
+            "sugar cookie" : ("baked_goods", "cookie"),
+            "sugar cookies" : ("baked_goods", "cookie"),
+            "oatmeal cookie" : ("baked_goods", "cookie"),
+            "oatmeal cookies" : ("baked_goods", "cookie"),
+            "peanut butter cookie" : ("baked_goods", "cookie"),
+            "peanut butter cookies" : ("baked_goods", "cookie"),
+            "snickerdoodle" : ("baked_goods", "cookie"),
+            "snickerdoodles" : ("baked_goods", "cookie"),
+            "gingerbread cookie" : ("baked_goods", "cookie"),
+            "gingerbread cookies" : ("baked_goods", "cookie"),
+            "shortbread cookie" : ("baked_goods", "cookie"),
+            "shortbread cookies" : ("baked_goods", "cookie"),
+            "macaroon" : ("baked_goods", "cookie"),
+            "macaroons" : ("baked_goods", "cookie"),
+            "macaron" : ("baked_goods", "cookie"),
+            "macarons" : ("baked_goods", "cookie"),
+            "biscotti" : ("baked_goods", "cookie"),
+            "biscottis" : ("baked_goods", "cookie"),
+            "oatmeal raisin cookie" : ("baked_goods", "cookie"),
+            "oatmeal raisin cookies" : ("baked_goods", "cookie"),
+            "peanut butter chocolate chip cookie" : ("baked_goods", "cookie"),
+            "peanut butter chocolate chip cookies" : ("baked_goods", "cookie"),
+            "peanut butter oatmeal cookie" : ("baked_goods", "cookie"),
+            "peanut butter oatmeal cookies" : ("baked_goods", "cookie"),
+            "peanut butter oatmeal chocolate chip cookie" : ("baked_goods", "cookie"),
+            "peanut butter oatmeal chocolate chip cookies" : ("baked_goods", "cookie"),
+            "brownie" : ("baked_goods", "brownie"),
+            "brownies" : ("baked_goods", "brownie"),
+            "blondie" : ("baked_goods", "brownie"),
+            "blondies" : ("baked_goods", "brownie"),
+
+            "cake" : ("baked_goods", "cake"),
+            "pound cake" : ("baked_goods", "cake"),
+            "pound cakes" : ("baked_goods", "cake"),
+            "angel food cake" : ("baked_goods", "cake"),
+            "angel food cakes" : ("baked_goods", "cake"),
+            "bundt cake" : ("baked_goods", "cake"),
+            "bundt cakes" : ("baked_goods", "cake"),
+            "cupcake" : ("baked_goods", "cake"),
+            "cupcakes" : ("baked_goods", "cake"),
+            "birthday cake" : ("baked_goods", "cake"),
+            "birthday cakes" : ("baked_goods", "cake"),
+            "sheet cake" : ("baked_goods", "cake"),
+            "sheet cakes" : ("baked_goods", "cake"),
+
+            "baking sheets": ("baked_goods", "baking"), # TODO: why? 
+            "baking powder": ("baked_goods", "baking"),
+            "baking soda": ("baked_goods", "baking"),
+            "yeast": ("baked_goods", "baking"),
+            "baking yeast": ("baked_goods", "baking"),
+            "active dry yeast": ("baked_goods", "baking"),
+            "instant yeast": ("baked_goods", "baking")
             }
 # -----------------------------------------------------------------------------------------------------
 # ---- Map of all of the subcategories in each primary category in the FOOD_CATALOG ----
 # -----------------------------------------------------------------------------------------------------
 
 # From the FOOD_CATALOG, generate new food categories dictionary with the major categories as keys and the minor categories as tuple values
 FOOD_CATEGORIES = {}
@@ -2196,32 +2290,41 @@
 FOOD_DENSITY_BY_GROUP = {
     "water" : {   # NOTE: manually added this category to use a default
        "category": "water",
        "density_g_per_ml": 1.0,
        "min_density_g_per_ml": 1.0,
        "max_density_g_per_ml": 1.0
        },
-    "syrups" : {   # NOTE: manually added this category for syrups which are not in the Density Database categories
+     "syrups" : {   # NOTE: manually added this category for syrups which are not in the Density Database categories
        "category": "syrups",
        "density_g_per_ml": 1.2,
        "min_density_g_per_ml": 1.2,
        "max_density_g_per_ml": 1.2
        },
-   "beverages_non_alcoholic_including_soft_drinks_and_juices" : {
+    "beverages_non_alcoholic_including_soft_drinks_and_juices" : {
        "category": "beverages_non_alcoholic_including_soft_drinks_and_juices",
        "density_g_per_ml": 1.0419,
         "min_density_g_per_ml": 0.916,
         "max_density_g_per_ml": 1.2372
        },
-    "miscellaneous_foods": {
-        "category": "miscellaneous_foods",
+       # TODO: Just commented this out, the categories here should be a 1:1 mapping with 
+       # TODO: the FOOD_CATALOG (i.e. all of these categories should be represented in the FOOD_CATALOG)
+    # "miscellaneous_foods": {
+    #     "category": "miscellaneous_foods",
+    #     "density_g_per_ml": 1.0379,
+    #     "min_density_g_per_ml": 0.26,
+    #     "max_density_g_per_ml": 2.2
+    # },
+    "sauces_and_gravies": {
+        "category": "sauces_and_gravies",
         "density_g_per_ml": 1.0379,
         "min_density_g_per_ml": 0.26,
         "max_density_g_per_ml": 2.2
     },
+    
     "soups": {
         "category": "soups",
         "density_g_per_ml": 1.0321,
         "min_density_g_per_ml": 0.99,
         "max_density_g_per_ml": 1.09
     },
     "wine_and_cider": {
@@ -2316,14 +2419,20 @@
     },
     "cereal_and_cereal_products": {
         "category": "cereal_and_cereal_products",
         "density_g_per_ml": 0.5781,
         "min_density_g_per_ml": 0.35,
         "max_density_g_per_ml": 1.07
     },
+    "baked_goods": {
+        "category": "baked_goods",
+        "density_g_per_ml": 0.5781,
+        "min_density_g_per_ml": 0.35,
+        "max_density_g_per_ml": 1.07
+    },
     "herbes_and_spices": {
         "category": "herbes_and_spices",
         "density_g_per_ml": 0.5062,
         "min_density_g_per_ml": 0.29,
         "max_density_g_per_ml": 0.77
     },
     "fruits": {
```

### Comparing `ingredient_slicer-1.0.2/ingredient_slicer/_ingredient_slicer.py` & `ingredient_slicer-1.0.3/ingredient_slicer/_ingredient_slicer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1547,14 +1547,30 @@
         """
 
         # print(f"Best effort extraction of food words from: {ingredient}") if self.debug else None
 
         # Apply _utils._remove_parenthesis_from_str() to remove parenthesis content
         ingredient = _utils._remove_parenthesis_from_str(ingredient)
 
+        # check for obscure/tricky edge case foods and if found, return them as the food (i.e. half-and-half, etc.)
+        edge_food = _utils._extract_edge_case_foods(ingredient)
+        if edge_food:
+            # edge_food = re.sub(r'[^\w\s]', '', edge_food)
+            # edge_food = re.sub(r'\s+', ' ', edge_food).strip()
+            return edge_food
+        # ingredient = "1/2 half and-half"
+
+        # half_and_half_match = HALF_AND_HALF_PATTERN.search(ingredient)
+
+        # if half_and_half_match:
+        #     half_and_half_match.group()
+
+        # HALF_AND_HALF_PATTERN.findall(ingredient)
+        # HALF_AND_HALF_PATTERN.search(ingredient).group()
+
         # regular expressions to find and remove from the ingredient
         # NOTE: important to remove "parenthesis" first and "stop words" last to.
         # Parenthesis can contain other patterns and they need to be dealt with first (i.e. "(about 8 oz)" contains a number and a unit)
         patterns_map = {
             # "parenthesis" : _regex_patterns.SPLIT_BY_PARENTHESIS, # NOTE: testing this removal
             "units" : _regex_patterns.UNITS_PATTERN,
             "numbers" : _regex_patterns.ALL_NUMBERS,
```

### Comparing `ingredient_slicer-1.0.2/ingredient_slicer/_regex_patterns.py` & `ingredient_slicer-1.0.3/ingredient_slicer/_regex_patterns.py`

 * *Files 0% similar despite different names*

```diff
@@ -459,14 +459,21 @@
 # create a map containg regexs for matching a number followed by a "%", "percent", or "pct" string
 # NUMBER_WITH_DIMENSIONS_SYMBOLS_MAP = {}
     
 NUMBER_WITH_INCH_SYMBOL_MAP = {}
 for inch_symbol in ["\"", "”"]:
     NUMBER_WITH_INCH_SYMBOL_MAP[inch_symbol] = re.compile(r'(?:\d*\.\d+|\d+\s*/\s*\d+|\d+)\s*' + inch_symbol + r'')
 
+# -----------------------------------------------------------------------------
+# --------------------------- Specific Edge case foods -----------------------------
+# Find foods that are specifically tricky to parse:
+# "half-n-half"
+# -----------------------------------------------------------------------------
+HALF_AND_HALF_PATTERN = re.compile(r'half[\s-]{0,5}(and|n|&)[\s-]{0,5}half', re.IGNORECASE)
+
 # # -----------------------------------------------------------------------------
 # # ---------------------------- OLD IngredientTools class... ---------------------------------
 # # -----------------------------------------------------------------------------
 # # --------------------------- Class to store all regex patterns -----------------------
 # # A class to hold all regex patterns used in the recipe parser (version 2)
 # # - Each pattern is stored as a class attribute and the class 
 # # - IngredientTools class has a single method that applies ALL of the
```

### Comparing `ingredient_slicer-1.0.2/ingredient_slicer/_utils.py` & `ingredient_slicer-1.0.3/ingredient_slicer/_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,15 +204,74 @@
         decimal_str = f"-{_make_int_or_float_str(str(decimal_value))}" if is_negative else _make_int_or_float_str(str(decimal_value))
 
         # return _make_int_or_float_str(str(round(float(Fraction(numerator, denominator)), 3)))
         return decimal_str
 
 # -----------------------------------------------------------------------------------------------
 # -----------------------------------------------------------------------------------------------
+# TODO: Write unit tests
+# TODO: Move EDGE_CASE_FOOD_PATTERNS to the _regex_patterns.py file
+# TODO: Possibly add move foods to the EDGE_CASE_FOOD_PATTERNS dictionary
+def _extract_edge_case_foods(ingredient: str) -> str:
+        """
+        Find and extract any edge case like foods from an ingredient string (i.e. "half and half").
+        Args:
+            ingredient (str): The ingredient string to parse.
+        Returns:
+            str: The extracted food, otherwise None
+        """
 
+        # ingredient = "0.43 tablespoon half and half cream"
+        # ingredient = "1/2 half and-half"
+        
+        EDGE_CASE_FOOD_PATTERNS = {
+            "HALF_AND_HALF_PATTERN" : _regex_patterns.HALF_AND_HALF_PATTERN
+        }
+
+        food_matches = []
+        
+        for key in EDGE_CASE_FOOD_PATTERNS:
+            edge_pattern = EDGE_CASE_FOOD_PATTERNS[key]
+            edge_pattern_match = edge_pattern.search(ingredient)
+
+            if edge_pattern_match:
+                food = edge_pattern_match.group()
+                end_index = edge_pattern_match.end()
+                # TODO: Super hacky way to handle the "HALF_AND_HALF_PATTERN" edge case and add the word "creamer" to the food
+                if key == "HALF_AND_HALF_PATTERN":
+                    creamer_words = [i for i in ingredient[end_index:].split() if i in ["cream", "creams",
+                                                                                        "creamer", "creamers"]]
+                    if creamer_words:
+                        food = f"{food} {creamer_words[0]}"
+                        # food = " ".join([food] + creamer_words[0])
+                food_matches.append((food))
+                # food_matches.append((edge_pattern_match.group(), key, edge_pattern_match.end()))
+
+        food = " ".join(food_matches).strip()
+
+        # Remove extra white spaces and non-alphanumeric characters
+        food = re.sub(r'[^\w\s]', '', food)
+        food = re.sub(r'\s+', ' ', food).strip()
+
+        # TODO: super hacky way of dealing with missing ampersands from the "half & half" food
+        if food in ["half half", "halfnhalf", "halfn half", "half nhalf", "halfhalf"]:
+            food = "half and half"
+
+        food = food if food else None
+        return food
+
+# ingredient = "1/2 half and-half"
+
+# half_and_half_match = HALF_AND_HALF_PATTERN.search(ingredient)
+
+# if half_and_half_match:
+#     half_and_half_match.group()
+
+# HALF_AND_HALF_PATTERN.findall(ingredient)
+# HALF_AND_HALF_PATTERN.search(ingredient).group()
 # -----------------------------------------------------------------------------------------------
 # ---- Convert ALL fractions in a string to their decimal equivalent ----
 # -----------------------------------------------------------------------------------------------
 
 # TODO: Replace the _convert_fractions_to_decimals function defined in the IngredientSlicer class with this version
 # NOTE: This is the NEW implementation of _convert_fractions_to_decimals and specifically deals with each fraction type
 # NOTE: in a specific order and with a specific regex pattern to ensure the most accurate conversion
```

### Comparing `ingredient_slicer-1.0.2/ingredient_slicer.egg-info/PKG-INFO` & `ingredient_slicer-1.0.3/ingredient_slicer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ingredient_slicer
-Version: 1.0.2
+Version: 1.0.3
 Summary: Parses unstructured recipe ingredient text into standardized quantities, units, and foods
 Author-email: Angus Watters <anguswatters@gmail.com>
 License: MIT License
 Keywords: ingredient,parser,recipe,text processing,food,cooking,grocery,shopping
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ingredient_slicer-1.0.2/ingredient_slicer.egg-info/SOURCES.txt` & `ingredient_slicer-1.0.3/ingredient_slicer.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 tests/test_find_and_remove.py
 tests/test_find_and_remove_hyphen_substrings.py
 tests/test_fraction_str_to_decimal.py
 tests/test_get_gram_weight.py
 tests/test_get_single_item_gram_weight.py
 tests/test_ingredient_slicer.py
 tests/test_ingredient_slicer_dimensions.py
+tests/test_ingredient_slicer_edge_case_foods.py
 tests/test_ingredient_slicer_fraction_conversions.py
 tests/test_ingredient_slicer_gram_weights.py
 tests/test_ingredient_slicer_parenthesis.py
 tests/test_ingredient_slicer_x_separators.py
 tests/test_is_approximate_quantity_only_parenthesis.py
 tests/test_make_int_or_float_str.py
 tests/test_merge_misleading_ranges.py
```

### Comparing `ingredient_slicer-1.0.2/pyproject.toml` & `ingredient_slicer-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 requires = ["setuptools", "setuptools-scm"]
 
 [project]
 name = "ingredient_slicer"
 authors = [
   {name = "Angus Watters", email = "anguswatters@gmail.com"},
 ]
-version = "1.0.2"
+version = "1.0.3"
 description = "Parses unstructured recipe ingredient text into standardized quantities, units, and foods"
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Operating System :: Microsoft :: Windows",
   "Operating System :: Unix",
```

### Comparing `ingredient_slicer-1.0.2/tests/test_avg_ranges.py` & `ingredient_slicer-1.0.3/tests/test_avg_ranges.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.2/tests/test_casual_ingredients.py` & `ingredient_slicer-1.0.3/tests/test_casual_ingredients.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.2/tests/test_convert_fractions_to_decimals.py` & `ingredient_slicer-1.0.3/tests/test_convert_fractions_to_decimals.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.2/tests/test_convert_volumes_to_milliliters.py` & `ingredient_slicer-1.0.3/tests/test_convert_volumes_to_milliliters.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.2/tests/test_duplicate_unit_ranges.py` & `ingredient_slicer-1.0.3/tests/test_duplicate_unit_ranges.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.2/tests/test_extract_dimensions.py` & `ingredient_slicer-1.0.3/tests/test_extract_dimensions.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.2/tests/test_extract_quantities_utils.py` & `ingredient_slicer-1.0.3/tests/test_extract_quantities_utils.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.2/tests/test_find_and_remove.py` & `ingredient_slicer-1.0.3/tests/test_find_and_remove.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.2/tests/test_find_and_remove_hyphen_substrings.py` & `ingredient_slicer-1.0.3/tests/test_find_and_remove_hyphen_substrings.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.2/tests/test_fraction_str_to_decimal.py` & `ingredient_slicer-1.0.3/tests/test_fraction_str_to_decimal.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.2/tests/test_get_gram_weight.py` & `ingredient_slicer-1.0.3/tests/test_get_gram_weight.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.2/tests/test_get_single_item_gram_weight.py` & `ingredient_slicer-1.0.3/tests/test_get_single_item_gram_weight.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.2/tests/test_ingredient_slicer.py` & `ingredient_slicer-1.0.3/tests/test_ingredient_slicer.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.2/tests/test_ingredient_slicer_dimensions.py` & `ingredient_slicer-1.0.3/tests/test_ingredient_slicer_dimensions.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.2/tests/test_ingredient_slicer_fraction_conversions.py` & `ingredient_slicer-1.0.3/tests/test_ingredient_slicer_fraction_conversions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,23 @@
 # "4/0.48 Bites"
 
 # pytest library
 import pytest
 
 import re
 
-from ingredient_slicer import IngredientSlicer
+from ingredient_slicer import IngredientSlicer, _constants
+
+# subcats = [i[1] for i in _constants.FOOD_CATEGORIES.items()]
+
+# subcat_list = []
+
+# for subcat in subcats:
+#     for cat in subcat:
+#         subcat_list.append(cat)
 
 # -------------------------------------------------------------------------------
 # -------------------------------------------------------------------------------
 # ---- Test the fraction conversion outputs of the IngredientSlicer ----
 # -------------------------------------------------------------------------------
 
 def test_whole_number_numerartor_with_whole_number_denominator():
```

### Comparing `ingredient_slicer-1.0.2/tests/test_ingredient_slicer_gram_weights.py` & `ingredient_slicer-1.0.3/tests/test_ingredient_slicer_gram_weights.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.2/tests/test_ingredient_slicer_parenthesis.py` & `ingredient_slicer-1.0.3/tests/test_ingredient_slicer_parenthesis.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.2/tests/test_ingredient_slicer_x_separators.py` & `ingredient_slicer-1.0.3/tests/test_ingredient_slicer_x_separators.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.2/tests/test_is_approximate_quantity_only_parenthesis.py` & `ingredient_slicer-1.0.3/tests/test_is_approximate_quantity_only_parenthesis.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.2/tests/test_make_int_or_float_str.py` & `ingredient_slicer-1.0.3/tests/test_make_int_or_float_str.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.2/tests/test_merge_misleading_ranges.py` & `ingredient_slicer-1.0.3/tests/test_merge_misleading_ranges.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.2/tests/test_merge_numbers.py` & `ingredient_slicer-1.0.3/tests/test_merge_numbers.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.2/tests/test_number_ranges.py` & `ingredient_slicer-1.0.3/tests/test_number_ranges.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,49 @@
 import pytest
 
 import re
 
 # from fractions import Fraction
 
 from ingredient_slicer import IngredientSlicer, _utils
+# from ingredient_slicer import _constants
 
+# _constants.SECONDARY_CATEGORIES
+# categories_to_ignore = [
+#                     # TODO: misc_changes
+#                     "miscellaneous_foods", 
+#                     "baked_goods",
+#                     "mixed_dishes", 
+#                     "beverages_non_alcoholic_including_soft_drinks_and_juices",
+#                     "tea_cacao_coffee_and_drinking_powders",
+#                     "wine_and_cider", 
+#                     "beer",
+#                     "spirits_and_liqueurs",
+#                     "snacks",
+#                     "water"
+#                     ]
+
+# secondary_categories_to_ignore = [_constants.FOOD_CATEGORIES[i] for i in _constants.FOOD_CATEGORIES if i in categories_to_ignore]
+# secondary_categories_to_ignore = [item for category in categories_to_ignore for item in _constants.FOOD_CATEGORIES.get(category, [])]
+# [i for i in _constants.SECONDARY_CATEGORIES if i not in secondary_categories_to_ignore]
+# [item for sublist in _constants.FOOD_CATEGORIES[i] for item in sublist for i in _constants.FOOD_CATEGORIES if i in categories_to_ignore]
+
+# categories_to_ignore = [
+#                     # TODO: misc_changes
+#                     "miscellaneous_foods", 
+#                     "baked_goods",
+#                     "mixed_dishes", 
+#                     "beverages_non_alcoholic_including_soft_drinks_and_juices",
+#                     "tea_cacao_coffee_and_drinking_powders",
+#                     "wine_and_cider", 
+#                     "beer",
+#                     "spirits_and_liqueurs",
+#                     "snacks",
+#                     "water"
+#                     ]
 # -------------------------------------------------------------------------------
 # ---- Simple number ranges (whole numbers/decimals to whole numbers/decimals) ----
 # -------------------------------------------------------------------------------
 
 def test_simple_number_range_1():
     slicer = IngredientSlicer("1-2 cups of sugar", debug = True)
     # slicer.parse()
@@ -210,14 +244,15 @@
     assert parsed['prep'] == []
     assert parsed['food'] == 'sugar'
     assert parsed['size_modifiers'] == []
 
 def test_average_from_two_whole_numbers_2():
     parse = IngredientSlicer("1-   8 tbsp of thickened cream")
     # parse.parse()
+
     parsed = parse.to_json()
     assert parsed["standardized_ingredient"] == '4.5 tbsp of thickened cream'
     assert parsed['quantity'] == "4.5"
     assert parsed['unit'] == 'tbsp'
     assert parsed['standardized_unit'] == 'tablespoon'
     
     assert parsed['secondary_quantity'] == None
```

### Comparing `ingredient_slicer-1.0.2/tests/test_number_ranges_separated_by_words.py` & `ingredient_slicer-1.0.3/tests/test_number_ranges_separated_by_words.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.2/tests/test_numbers_with_inch_symbols.py` & `ingredient_slicer-1.0.3/tests/test_numbers_with_inch_symbols.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.2/tests/test_parenthesis.py` & `ingredient_slicer-1.0.3/tests/test_parenthesis.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.2/tests/test_parenthesis_utils.py` & `ingredient_slicer-1.0.3/tests/test_parenthesis_utils.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.2/tests/test_percentages.py` & `ingredient_slicer-1.0.3/tests/test_percentages.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.2/tests/test_prefixed_number_words_regex.py` & `ingredient_slicer-1.0.3/tests/test_prefixed_number_words_regex.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.2/tests/test_prep_words.py` & `ingredient_slicer-1.0.3/tests/test_prep_words.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.2/tests/test_quantity_range_regex.py` & `ingredient_slicer-1.0.3/tests/test_quantity_range_regex.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.2/tests/test_quantity_units_regex.py` & `ingredient_slicer-1.0.3/tests/test_quantity_units_regex.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.2/tests/test_remove_repeat_units_in_ranges.py` & `ingredient_slicer-1.0.3/tests/test_remove_repeat_units_in_ranges.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.2/tests/test_remove_x_separators.py` & `ingredient_slicer-1.0.3/tests/test_remove_x_separators.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.2/tests/test_replace_a_or_an_quantities.py` & `ingredient_slicer-1.0.3/tests/test_replace_a_or_an_quantities.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.2/tests/test_separate_dimensions.py` & `ingredient_slicer-1.0.3/tests/test_separate_dimensions.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.2/tests/test_size_modifiers.py` & `ingredient_slicer-1.0.3/tests/test_size_modifiers.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.2/tests/test_spaced_numbers.py` & `ingredient_slicer-1.0.3/tests/test_spaced_numbers.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.2/tests/test_unit_regex.py` & `ingredient_slicer-1.0.3/tests/test_unit_regex.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.2/tests/test_wild_ingredients.py` & `ingredient_slicer-1.0.3/tests/test_wild_ingredients.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.2/tests/test_word_fractions.py` & `ingredient_slicer-1.0.3/tests/test_word_fractions.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.2/tests/test_word_numbers.py` & `ingredient_slicer-1.0.3/tests/test_word_numbers.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.2/tests/test_x_after_number_regex.py` & `ingredient_slicer-1.0.3/tests/test_x_after_number_regex.py`

 * *Files identical despite different names*

