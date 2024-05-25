# Comparing `tmp/pypipr-1.0.98.tar.gz` & `tmp/pypipr-1.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypipr-1.0.98.tar", max compression
+gzip compressed data, was "pypipr-1.0.99.tar", max compression
```

## Comparing `pypipr-1.0.98.tar` & `pypipr-1.0.99.tar`

### file list

```diff
@@ -1,78 +1,78 @@
--rw-r--r--   0        0        0     3487 2024-04-28 13:23:42.904396 pypipr-1.0.98/pypipr/__init__.py
--rw-r--r--   0        0        0     2229 2024-03-17 17:38:37.508083 pypipr-1.0.98/pypipr/ibuiltins/ComparePerformance.py
--rw-r--r--   0        0        0      100 2024-03-17 17:38:37.508083 pypipr-1.0.98/pypipr/ibuiltins/LINUX.py
--rw-r--r--   0        0        0     7358 2024-04-23 10:50:10.015024 pypipr-1.0.98/pypipr/ibuiltins/RunParallel.py
--rw-r--r--   0        0        0      105 2024-03-17 17:38:37.508083 pypipr-1.0.98/pypipr/ibuiltins/WINDOWS.py
--rw-r--r--   0        0        0        0 2024-03-17 17:38:37.508083 pypipr-1.0.98/pypipr/ibuiltins/__init__.py
--rw-r--r--   0        0        0      218 2024-03-17 17:38:37.508083 pypipr-1.0.98/pypipr/ibuiltins/avg.py
--rw-r--r--   0        0        0      194 2024-03-17 17:38:37.508083 pypipr-1.0.98/pypipr/ibuiltins/basename.py
--rw-r--r--   0        0        0      714 2024-04-28 13:23:17.812396 pypipr-1.0.98/pypipr/ibuiltins/chr_to_int.py
--rw-r--r--   0        0        0      385 2024-04-22 13:19:16.948654 pypipr-1.0.98/pypipr/ibuiltins/chunk_array.py
--rw-r--r--   0        0        0      500 2024-03-17 17:38:37.508083 pypipr-1.0.98/pypipr/ibuiltins/create_folder.py
--rw-r--r--   0        0        0      466 2024-03-17 17:38:37.508083 pypipr-1.0.98/pypipr/ibuiltins/datetime_from_string.py
--rw-r--r--   0        0        0      476 2024-03-17 17:38:37.508083 pypipr-1.0.98/pypipr/ibuiltins/datetime_now.py
--rw-r--r--   0        0        0      377 2024-03-17 17:38:37.508083 pypipr-1.0.98/pypipr/ibuiltins/dict_first.py
--rw-r--r--   0        0        0      229 2024-03-17 17:38:37.508083 pypipr-1.0.98/pypipr/ibuiltins/dirname.py
--rw-r--r--   0        0        0      321 2024-04-20 11:53:09.914721 pypipr-1.0.98/pypipr/ibuiltins/exit_if_empty.py
--rw-r--r--   0        0        0      543 2024-03-17 17:38:37.508083 pypipr-1.0.98/pypipr/ibuiltins/filter_empty.py
--rw-r--r--   0        0        0      335 2024-04-23 12:23:59.246031 pypipr-1.0.98/pypipr/ibuiltins/get_by_index.py
--rw-r--r--   0        0        0      639 2024-04-22 21:58:29.290425 pypipr-1.0.98/pypipr/ibuiltins/get_class_method.py
--rw-r--r--   0        0        0      227 2024-03-17 17:38:37.508083 pypipr-1.0.98/pypipr/ibuiltins/get_filemtime.py
--rw-r--r--   0        0        0      196 2024-03-17 17:38:37.508083 pypipr-1.0.98/pypipr/ibuiltins/get_filesize.py
--rw-r--r--   0        0        0      610 2024-04-28 13:08:11.692396 pypipr-1.0.98/pypipr/ibuiltins/int_to_chr.py
--rw-r--r--   0        0        0      683 2024-04-20 11:02:21.923096 pypipr-1.0.98/pypipr/ibuiltins/is_empty.py
--rw-r--r--   0        0        0      922 2024-03-17 17:38:37.508083 pypipr-1.0.98/pypipr/ibuiltins/is_iterable.py
--rw-r--r--   0        0        0     1008 2024-03-17 17:38:37.508083 pypipr-1.0.98/pypipr/ibuiltins/is_valid_url.py
--rw-r--r--   0        0        0      899 2024-04-23 09:16:42.841403 pypipr-1.0.98/pypipr/ibuiltins/ivars.py
--rw-r--r--   0        0        0      496 2024-03-17 17:38:37.508083 pypipr-1.0.98/pypipr/ibuiltins/password_generator.py
--rw-r--r--   0        0        0      405 2024-03-17 17:38:37.508083 pypipr-1.0.98/pypipr/ibuiltins/random_bool.py
--rw-r--r--   0        0        0      114 2024-04-25 14:37:53.772148 pypipr-1.0.98/pypipr/ibuiltins/restart.py
--rw-r--r--   0        0        0      698 2024-03-17 17:38:37.512083 pypipr-1.0.98/pypipr/ibuiltins/set_timeout.py
--rw-r--r--   0        0        0      325 2024-03-17 17:38:37.512083 pypipr-1.0.98/pypipr/ibuiltins/sets_ordered.py
--rw-r--r--   0        0        0      377 2024-03-17 17:38:37.512083 pypipr-1.0.98/pypipr/ibuiltins/str_cmp.py
--rw-r--r--   0        0        0      597 2024-03-17 17:38:37.512083 pypipr-1.0.98/pypipr/ibuiltins/to_str.py
--rw-r--r--   0        0        0        0 2024-03-17 17:38:37.512083 pypipr-1.0.98/pypipr/iconsole/__init__.py
--rw-r--r--   0        0        0     1686 2024-03-17 17:38:37.512083 pypipr-1.0.98/pypipr/iconsole/choices.py
--rw-r--r--   0        0        0      525 2024-03-17 17:38:37.512083 pypipr-1.0.98/pypipr/iconsole/console_run.py
--rw-r--r--   0        0        0     1030 2024-04-23 12:02:12.950032 pypipr-1.0.98/pypipr/iconsole/input_char.py
--rw-r--r--   0        0        0     1041 2024-03-17 17:38:37.512083 pypipr-1.0.98/pypipr/iconsole/log.py
--rw-r--r--   0        0        0      541 2024-04-27 07:44:48.048476 pypipr-1.0.98/pypipr/iconsole/print_colorize.py
--rw-r--r--   0        0        0      930 2024-04-22 21:43:34.984645 pypipr-1.0.98/pypipr/iconsole/print_dir.py
--rw-r--r--   0        0        0      282 2024-04-22 21:44:47.788645 pypipr-1.0.98/pypipr/iconsole/print_log.py
--rw-r--r--   0        0        0      914 2024-04-24 02:48:07.180538 pypipr-1.0.98/pypipr/iconsole/print_to_last_line.py
--rw-r--r--   0        0        0      396 2024-03-17 17:38:37.512083 pypipr-1.0.98/pypipr/iconsole/text_colorize.py
--rw-r--r--   0        0        0     1093 2024-03-17 17:38:37.512083 pypipr-1.0.98/pypipr/idjango/APIMixinView.py
--rw-r--r--   0        0        0        0 2024-03-17 17:38:37.512083 pypipr-1.0.98/pypipr/idjango/__init__.py
--rw-r--r--   0        0        0      222 2024-03-17 17:38:37.512083 pypipr-1.0.98/pypipr/iengineering/PintUreg.py
--rw-r--r--   0        0        0      118 2024-03-17 17:38:37.512083 pypipr-1.0.98/pypipr/iengineering/PintUregQuantity.py
--rw-r--r--   0        0        0        0 2024-03-17 17:38:37.512083 pypipr-1.0.98/pypipr/iengineering/__init__.py
--rw-r--r--   0        0        0      695 2024-04-22 21:59:57.598425 pypipr-1.0.98/pypipr/iengineering/batch_calculate.py
--rw-r--r--   0        0        0     1277 2024-03-17 17:38:37.512083 pypipr-1.0.98/pypipr/iengineering/batchmaker.py
--rw-r--r--   0        0        0      805 2024-03-17 17:38:37.512083 pypipr-1.0.98/pypipr/iengineering/calculate.py
--rw-r--r--   0        0        0      966 2024-04-23 11:50:40.860964 pypipr-1.0.98/pypipr/iflow/auto_reload.py
--rw-r--r--   0        0        0      243 2024-03-17 17:38:37.516083 pypipr-1.0.98/pypipr/iflow/github_pull.py
--rw-r--r--   0        0        0      951 2024-03-17 17:38:37.516083 pypipr-1.0.98/pypipr/iflow/github_push.py
--rw-r--r--   0        0        0      600 2024-03-17 17:38:37.516083 pypipr-1.0.98/pypipr/iflow/github_user.py
--rw-r--r--   0        0        0      839 2024-04-20 02:24:51.624107 pypipr-1.0.98/pypipr/iflow/pip_freeze_without_version.py
--rw-r--r--   0        0        0      409 2024-03-17 17:38:37.516083 pypipr-1.0.98/pypipr/iflow/poetry_publish.py
--rw-r--r--   0        0        0      622 2024-03-17 17:38:37.516083 pypipr-1.0.98/pypipr/iflow/poetry_update_version.py
--rw-r--r--   0        0        0        0 2024-03-17 17:38:37.516083 pypipr-1.0.98/pypipr/ifunctions/__init__.py
--rw-r--r--   0        0        0      552 2024-04-24 08:03:08.734958 pypipr-1.0.98/pypipr/ifunctions/iargv.py
--rw-r--r--   0        0        0      748 2024-03-17 17:38:37.516083 pypipr-1.0.98/pypipr/ifunctions/idumps.py
--rw-r--r--   0        0        0     1423 2024-03-17 17:38:37.516083 pypipr-1.0.98/pypipr/ifunctions/idumps_html.py
--rw-r--r--   0        0        0      679 2024-04-23 11:41:52.328964 pypipr-1.0.98/pypipr/ifunctions/ienv.py
--rw-r--r--   0        0        0      465 2024-03-17 17:38:37.516083 pypipr-1.0.98/pypipr/ifunctions/iexec.py
--rw-r--r--   0        0        0     2069 2024-03-17 17:38:37.516083 pypipr-1.0.98/pypipr/ifunctions/ijoin.py
--rw-r--r--   0        0        0      638 2024-04-22 21:36:07.164645 pypipr-1.0.98/pypipr/ifunctions/iloads.py
--rw-r--r--   0        0        0     4146 2024-04-22 21:40:17.264645 pypipr-1.0.98/pypipr/ifunctions/iloads_html.py
--rw-r--r--   0        0        0     2808 2024-03-17 17:38:37.516083 pypipr-1.0.98/pypipr/ifunctions/iopen.py
--rw-r--r--   0        0        0      849 2024-04-22 21:41:31.764645 pypipr-1.0.98/pypipr/ifunctions/iprint.py
--rw-r--r--   0        0        0     2407 2024-03-17 17:38:37.516083 pypipr-1.0.98/pypipr/ifunctions/irange.py
--rw-r--r--   0        0        0      722 2024-03-17 17:38:37.516083 pypipr-1.0.98/pypipr/ifunctions/ireplace.py
--rw-r--r--   0        0        0      748 2024-04-23 09:11:14.125403 pypipr-1.0.98/pypipr/ifunctions/iscandir.py
--rw-r--r--   0        0        0      383 2024-03-17 17:38:37.520083 pypipr-1.0.98/pypipr/ifunctions/isplit.py
--rw-r--r--   0        0        0     1061 2024-04-20 02:38:18.131451 pypipr-1.0.98/pypipr/pypipr.py.bak
--rw-r--r--   0        0        0     1800 2024-04-24 08:29:46.253049 pypipr-1.0.98/pypipr/terminal.py
--rw-r--r--   0        0        0      544 2024-04-28 13:23:53.456396 pypipr-1.0.98/pyproject.toml
--rw-r--r--   0        0        0    50405 2024-04-28 13:23:47.860396 pypipr-1.0.98/readme.md
--rw-r--r--   0        0        0    51091 1970-01-01 00:00:00.000000 pypipr-1.0.98/PKG-INFO
+-rw-r--r--   0        0        0     3488 2024-04-29 02:05:49.002641 pypipr-1.0.99/pypipr/__init__.py
+-rw-r--r--   0        0        0     2229 2024-03-17 17:38:37.508083 pypipr-1.0.99/pypipr/ibuiltins/ComparePerformance.py
+-rw-r--r--   0        0        0      100 2024-03-17 17:38:37.508083 pypipr-1.0.99/pypipr/ibuiltins/LINUX.py
+-rw-r--r--   0        0        0     7358 2024-04-23 10:50:10.015024 pypipr-1.0.99/pypipr/ibuiltins/RunParallel.py
+-rw-r--r--   0        0        0      105 2024-03-17 17:38:37.508083 pypipr-1.0.99/pypipr/ibuiltins/WINDOWS.py
+-rw-r--r--   0        0        0        0 2024-03-17 17:38:37.508083 pypipr-1.0.99/pypipr/ibuiltins/__init__.py
+-rw-r--r--   0        0        0      218 2024-03-17 17:38:37.508083 pypipr-1.0.99/pypipr/ibuiltins/avg.py
+-rw-r--r--   0        0        0      194 2024-03-17 17:38:37.508083 pypipr-1.0.99/pypipr/ibuiltins/basename.py
+-rw-r--r--   0        0        0      714 2024-04-28 13:23:17.812396 pypipr-1.0.99/pypipr/ibuiltins/chr_to_int.py
+-rw-r--r--   0        0        0      385 2024-04-22 13:19:16.948654 pypipr-1.0.99/pypipr/ibuiltins/chunk_array.py
+-rw-r--r--   0        0        0      500 2024-03-17 17:38:37.508083 pypipr-1.0.99/pypipr/ibuiltins/create_folder.py
+-rw-r--r--   0        0        0      466 2024-03-17 17:38:37.508083 pypipr-1.0.99/pypipr/ibuiltins/datetime_from_string.py
+-rw-r--r--   0        0        0      476 2024-03-17 17:38:37.508083 pypipr-1.0.99/pypipr/ibuiltins/datetime_now.py
+-rw-r--r--   0        0        0      377 2024-03-17 17:38:37.508083 pypipr-1.0.99/pypipr/ibuiltins/dict_first.py
+-rw-r--r--   0        0        0      229 2024-03-17 17:38:37.508083 pypipr-1.0.99/pypipr/ibuiltins/dirname.py
+-rw-r--r--   0        0        0      321 2024-04-20 11:53:09.914721 pypipr-1.0.99/pypipr/ibuiltins/exit_if_empty.py
+-rw-r--r--   0        0        0      543 2024-03-17 17:38:37.508083 pypipr-1.0.99/pypipr/ibuiltins/filter_empty.py
+-rw-r--r--   0        0        0      335 2024-04-23 12:23:59.246031 pypipr-1.0.99/pypipr/ibuiltins/get_by_index.py
+-rw-r--r--   0        0        0      639 2024-04-22 21:58:29.290425 pypipr-1.0.99/pypipr/ibuiltins/get_class_method.py
+-rw-r--r--   0        0        0      227 2024-03-17 17:38:37.508083 pypipr-1.0.99/pypipr/ibuiltins/get_filemtime.py
+-rw-r--r--   0        0        0      196 2024-03-17 17:38:37.508083 pypipr-1.0.99/pypipr/ibuiltins/get_filesize.py
+-rw-r--r--   0        0        0      610 2024-04-28 13:08:11.692396 pypipr-1.0.99/pypipr/ibuiltins/int_to_chr.py
+-rw-r--r--   0        0        0      683 2024-04-20 11:02:21.923096 pypipr-1.0.99/pypipr/ibuiltins/is_empty.py
+-rw-r--r--   0        0        0      922 2024-03-17 17:38:37.508083 pypipr-1.0.99/pypipr/ibuiltins/is_iterable.py
+-rw-r--r--   0        0        0     1008 2024-03-17 17:38:37.508083 pypipr-1.0.99/pypipr/ibuiltins/is_valid_url.py
+-rw-r--r--   0        0        0      496 2024-03-17 17:38:37.508083 pypipr-1.0.99/pypipr/ibuiltins/password_generator.py
+-rw-r--r--   0        0        0      405 2024-03-17 17:38:37.508083 pypipr-1.0.99/pypipr/ibuiltins/random_bool.py
+-rw-r--r--   0        0        0      114 2024-04-25 14:37:53.772148 pypipr-1.0.99/pypipr/ibuiltins/restart.py
+-rw-r--r--   0        0        0      698 2024-03-17 17:38:37.512083 pypipr-1.0.99/pypipr/ibuiltins/set_timeout.py
+-rw-r--r--   0        0        0      325 2024-03-17 17:38:37.512083 pypipr-1.0.99/pypipr/ibuiltins/sets_ordered.py
+-rw-r--r--   0        0        0      377 2024-03-17 17:38:37.512083 pypipr-1.0.99/pypipr/ibuiltins/str_cmp.py
+-rw-r--r--   0        0        0      597 2024-03-17 17:38:37.512083 pypipr-1.0.99/pypipr/ibuiltins/to_str.py
+-rw-r--r--   0        0        0        0 2024-03-17 17:38:37.512083 pypipr-1.0.99/pypipr/iconsole/__init__.py
+-rw-r--r--   0        0        0     1686 2024-03-17 17:38:37.512083 pypipr-1.0.99/pypipr/iconsole/choices.py
+-rw-r--r--   0        0        0      525 2024-03-17 17:38:37.512083 pypipr-1.0.99/pypipr/iconsole/console_run.py
+-rw-r--r--   0        0        0     1030 2024-04-23 12:02:12.950032 pypipr-1.0.99/pypipr/iconsole/input_char.py
+-rw-r--r--   0        0        0     1041 2024-03-17 17:38:37.512083 pypipr-1.0.99/pypipr/iconsole/log.py
+-rw-r--r--   0        0        0      541 2024-04-27 07:44:48.048476 pypipr-1.0.99/pypipr/iconsole/print_colorize.py
+-rw-r--r--   0        0        0      930 2024-04-22 21:43:34.984645 pypipr-1.0.99/pypipr/iconsole/print_dir.py
+-rw-r--r--   0        0        0      282 2024-04-22 21:44:47.788645 pypipr-1.0.99/pypipr/iconsole/print_log.py
+-rw-r--r--   0        0        0      914 2024-04-24 02:48:07.180538 pypipr-1.0.99/pypipr/iconsole/print_to_last_line.py
+-rw-r--r--   0        0        0      396 2024-03-17 17:38:37.512083 pypipr-1.0.99/pypipr/iconsole/text_colorize.py
+-rw-r--r--   0        0        0     1093 2024-03-17 17:38:37.512083 pypipr-1.0.99/pypipr/idjango/APIMixinView.py
+-rw-r--r--   0        0        0        0 2024-03-17 17:38:37.512083 pypipr-1.0.99/pypipr/idjango/__init__.py
+-rw-r--r--   0        0        0      222 2024-03-17 17:38:37.512083 pypipr-1.0.99/pypipr/iengineering/PintUreg.py
+-rw-r--r--   0        0        0      118 2024-03-17 17:38:37.512083 pypipr-1.0.99/pypipr/iengineering/PintUregQuantity.py
+-rw-r--r--   0        0        0        0 2024-03-17 17:38:37.512083 pypipr-1.0.99/pypipr/iengineering/__init__.py
+-rw-r--r--   0        0        0      695 2024-04-22 21:59:57.598425 pypipr-1.0.99/pypipr/iengineering/batch_calculate.py
+-rw-r--r--   0        0        0     1277 2024-03-17 17:38:37.512083 pypipr-1.0.99/pypipr/iengineering/batchmaker.py
+-rw-r--r--   0        0        0      805 2024-03-17 17:38:37.512083 pypipr-1.0.99/pypipr/iengineering/calculate.py
+-rw-r--r--   0        0        0      966 2024-04-23 11:50:40.860964 pypipr-1.0.99/pypipr/iflow/auto_reload.py
+-rw-r--r--   0        0        0      243 2024-03-17 17:38:37.516083 pypipr-1.0.99/pypipr/iflow/github_pull.py
+-rw-r--r--   0        0        0      951 2024-03-17 17:38:37.516083 pypipr-1.0.99/pypipr/iflow/github_push.py
+-rw-r--r--   0        0        0      600 2024-03-17 17:38:37.516083 pypipr-1.0.99/pypipr/iflow/github_user.py
+-rw-r--r--   0        0        0      839 2024-04-20 02:24:51.624107 pypipr-1.0.99/pypipr/iflow/pip_freeze_without_version.py
+-rw-r--r--   0        0        0      409 2024-03-17 17:38:37.516083 pypipr-1.0.99/pypipr/iflow/poetry_publish.py
+-rw-r--r--   0        0        0      622 2024-03-17 17:38:37.516083 pypipr-1.0.99/pypipr/iflow/poetry_update_version.py
+-rw-r--r--   0        0        0        0 2024-03-17 17:38:37.516083 pypipr-1.0.99/pypipr/ifunctions/__init__.py
+-rw-r--r--   0        0        0      552 2024-04-24 08:03:08.734958 pypipr-1.0.99/pypipr/ifunctions/iargv.py
+-rw-r--r--   0        0        0      748 2024-03-17 17:38:37.516083 pypipr-1.0.99/pypipr/ifunctions/idumps.py
+-rw-r--r--   0        0        0     1423 2024-03-17 17:38:37.516083 pypipr-1.0.99/pypipr/ifunctions/idumps_html.py
+-rw-r--r--   0        0        0      679 2024-04-23 11:41:52.328964 pypipr-1.0.99/pypipr/ifunctions/ienv.py
+-rw-r--r--   0        0        0      465 2024-03-17 17:38:37.516083 pypipr-1.0.99/pypipr/ifunctions/iexec.py
+-rw-r--r--   0        0        0     2069 2024-03-17 17:38:37.516083 pypipr-1.0.99/pypipr/ifunctions/ijoin.py
+-rw-r--r--   0        0        0      638 2024-04-22 21:36:07.164645 pypipr-1.0.99/pypipr/ifunctions/iloads.py
+-rw-r--r--   0        0        0     4146 2024-04-22 21:40:17.264645 pypipr-1.0.99/pypipr/ifunctions/iloads_html.py
+-rw-r--r--   0        0        0     2808 2024-03-17 17:38:37.516083 pypipr-1.0.99/pypipr/ifunctions/iopen.py
+-rw-r--r--   0        0        0      849 2024-04-22 21:41:31.764645 pypipr-1.0.99/pypipr/ifunctions/iprint.py
+-rw-r--r--   0        0        0     2407 2024-03-17 17:38:37.516083 pypipr-1.0.99/pypipr/ifunctions/irange.py
+-rw-r--r--   0        0        0      722 2024-03-17 17:38:37.516083 pypipr-1.0.99/pypipr/ifunctions/ireplace.py
+-rw-r--r--   0        0        0      748 2024-04-23 09:11:14.125403 pypipr-1.0.99/pypipr/ifunctions/iscandir.py
+-rw-r--r--   0        0        0      383 2024-03-17 17:38:37.520083 pypipr-1.0.99/pypipr/ifunctions/isplit.py
+-rw-r--r--   0        0        0      899 2024-04-29 02:04:28.166641 pypipr-1.0.99/pypipr/ifunctions/ivars.py
+-rw-r--r--   0        0        0     1061 2024-04-20 02:38:18.131451 pypipr-1.0.99/pypipr/pypipr.py.bak
+-rw-r--r--   0        0        0     1800 2024-04-24 08:29:46.253049 pypipr-1.0.99/pypipr/terminal.py
+-rw-r--r--   0        0        0      544 2024-04-29 02:06:03.994641 pypipr-1.0.99/pyproject.toml
+-rw-r--r--   0        0        0    50983 2024-04-29 02:05:55.486641 pypipr-1.0.99/readme.md
+-rw-r--r--   0        0        0    51669 1970-01-01 00:00:00.000000 pypipr-1.0.99/PKG-INFO
```

### Comparing `pypipr-1.0.98/pypipr/__init__.py` & `pypipr-1.0.99/pypipr/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 from .ibuiltins.get_class_method import get_class_method
 from .ibuiltins.get_filemtime import get_filemtime
 from .ibuiltins.get_filesize import get_filesize
 from .ibuiltins.int_to_chr import int_to_chr
 from .ibuiltins.is_empty import is_empty
 from .ibuiltins.is_iterable import is_iterable
 from .ibuiltins.is_valid_url import is_valid_url
-from .ibuiltins.ivars import ivars
 from .ibuiltins.password_generator import password_generator
 from .ibuiltins.random_bool import random_bool
 from .ibuiltins.restart import restart
 from .ibuiltins.set_timeout import set_timeout
 from .ibuiltins.sets_ordered import sets_ordered
 from .ibuiltins.str_cmp import str_cmp
 from .ibuiltins.to_str import to_str
@@ -61,14 +60,15 @@
 from .ifunctions.iloads_html import iloads_html
 from .ifunctions.iopen import iopen
 from .ifunctions.iprint import iprint
 from .ifunctions.irange import irange
 from .ifunctions.ireplace import ireplace
 from .ifunctions.iscandir import iscandir
 from .ifunctions.isplit import isplit
+from .ifunctions.ivars import ivars
 import asyncio
 import colorama
 import csv
 import datetime
 import functools
 import inspect
 import io
```

### Comparing `pypipr-1.0.98/pypipr/ibuiltins/ComparePerformance.py` & `pypipr-1.0.99/pypipr/ibuiltins/ComparePerformance.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.98/pypipr/ibuiltins/RunParallel.py` & `pypipr-1.0.99/pypipr/ibuiltins/RunParallel.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.98/pypipr/ibuiltins/chr_to_int.py` & `pypipr-1.0.99/pypipr/ibuiltins/chr_to_int.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.98/pypipr/ibuiltins/filter_empty.py` & `pypipr-1.0.99/pypipr/ibuiltins/filter_empty.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.98/pypipr/ibuiltins/get_class_method.py` & `pypipr-1.0.99/pypipr/ibuiltins/get_class_method.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.98/pypipr/ibuiltins/int_to_chr.py` & `pypipr-1.0.99/pypipr/ibuiltins/int_to_chr.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.98/pypipr/ibuiltins/is_empty.py` & `pypipr-1.0.99/pypipr/ibuiltins/is_empty.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.98/pypipr/ibuiltins/is_iterable.py` & `pypipr-1.0.99/pypipr/ibuiltins/is_iterable.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.98/pypipr/ibuiltins/is_valid_url.py` & `pypipr-1.0.99/pypipr/ibuiltins/is_valid_url.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.98/pypipr/ibuiltins/ivars.py` & `pypipr-1.0.99/pypipr/ifunctions/ivars.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.98/pypipr/ibuiltins/set_timeout.py` & `pypipr-1.0.99/pypipr/ibuiltins/set_timeout.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.98/pypipr/ibuiltins/to_str.py` & `pypipr-1.0.99/pypipr/ibuiltins/to_str.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.98/pypipr/iconsole/choices.py` & `pypipr-1.0.99/pypipr/iconsole/choices.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.98/pypipr/iconsole/console_run.py` & `pypipr-1.0.99/pypipr/iconsole/console_run.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.98/pypipr/iconsole/input_char.py` & `pypipr-1.0.99/pypipr/iconsole/input_char.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.98/pypipr/iconsole/log.py` & `pypipr-1.0.99/pypipr/iconsole/log.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.98/pypipr/iconsole/print_colorize.py` & `pypipr-1.0.99/pypipr/iconsole/print_colorize.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.98/pypipr/iconsole/print_dir.py` & `pypipr-1.0.99/pypipr/iconsole/print_dir.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.98/pypipr/iconsole/print_to_last_line.py` & `pypipr-1.0.99/pypipr/iconsole/print_to_last_line.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.98/pypipr/idjango/APIMixinView.py` & `pypipr-1.0.99/pypipr/idjango/APIMixinView.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.98/pypipr/iengineering/batch_calculate.py` & `pypipr-1.0.99/pypipr/iengineering/batch_calculate.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.98/pypipr/iengineering/batchmaker.py` & `pypipr-1.0.99/pypipr/iengineering/batchmaker.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.98/pypipr/iengineering/calculate.py` & `pypipr-1.0.99/pypipr/iengineering/calculate.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.98/pypipr/iflow/auto_reload.py` & `pypipr-1.0.99/pypipr/iflow/auto_reload.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.98/pypipr/iflow/github_push.py` & `pypipr-1.0.99/pypipr/iflow/github_push.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.98/pypipr/iflow/github_user.py` & `pypipr-1.0.99/pypipr/iflow/github_user.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.98/pypipr/iflow/pip_freeze_without_version.py` & `pypipr-1.0.99/pypipr/iflow/pip_freeze_without_version.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.98/pypipr/iflow/poetry_update_version.py` & `pypipr-1.0.99/pypipr/iflow/poetry_update_version.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.98/pypipr/ifunctions/iargv.py` & `pypipr-1.0.99/pypipr/ifunctions/iargv.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.98/pypipr/ifunctions/idumps.py` & `pypipr-1.0.99/pypipr/ifunctions/idumps.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.98/pypipr/ifunctions/idumps_html.py` & `pypipr-1.0.99/pypipr/ifunctions/idumps_html.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.98/pypipr/ifunctions/ienv.py` & `pypipr-1.0.99/pypipr/ifunctions/ienv.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.98/pypipr/ifunctions/ijoin.py` & `pypipr-1.0.99/pypipr/ifunctions/ijoin.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.98/pypipr/ifunctions/iloads.py` & `pypipr-1.0.99/pypipr/ifunctions/iloads.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.98/pypipr/ifunctions/iloads_html.py` & `pypipr-1.0.99/pypipr/ifunctions/iloads_html.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.98/pypipr/ifunctions/iopen.py` & `pypipr-1.0.99/pypipr/ifunctions/iopen.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.98/pypipr/ifunctions/iprint.py` & `pypipr-1.0.99/pypipr/ifunctions/iprint.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.98/pypipr/ifunctions/irange.py` & `pypipr-1.0.99/pypipr/ifunctions/irange.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.98/pypipr/ifunctions/ireplace.py` & `pypipr-1.0.99/pypipr/ifunctions/ireplace.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.98/pypipr/ifunctions/iscandir.py` & `pypipr-1.0.99/pypipr/ifunctions/iscandir.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.98/pypipr/pypipr.py.bak` & `pypipr-1.0.99/pypipr/pypipr.py.bak`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.98/pypipr/terminal.py` & `pypipr-1.0.99/pypipr/terminal.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.98/pyproject.toml` & `pypipr-1.0.99/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pypipr"
-version = "1.0.98"
+version = "1.0.99"
 description = "The Python Package Index Project"
 authors = ["ufiapjj <ufiapjj@gmail.com>"]
 readme = "readme.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9"
 getch = { version = "*", markers = "platform_system == 'Linux'" }
```

### Comparing `pypipr-1.0.98/readme.md` & `pypipr-1.0.99/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,30 @@
+Metadata-Version: 2.1
+Name: pypipr
+Version: 1.0.99
+Summary: The Python Package Index Project
+Author: ufiapjj
+Author-email: ufiapjj@gmail.com
+Requires-Python: >=3.9
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: colorama
+Requires-Dist: cssselect
+Requires-Dist: django
+Requires-Dist: getch ; platform_system == "Linux"
+Requires-Dist: lxml
+Requires-Dist: pint
+Requires-Dist: pyyaml
+Requires-Dist: requests
+Requires-Dist: tzdata
+Description-Content-Type: text/markdown
+
 
 # About
 The Python Package Index Project (pypipr)
 
 pypi : https://pypi.org/project/pypipr
 
 
@@ -93,15 +116,15 @@
 arr = [2, 3, 12, 3, 3, 42, 42, 1, 43, 2, 42, 41, 4, 24, 32, 42, 3, 12, 32, 42, 42]  
 print(chunk_array(arr, 5))  
 print(list(chunk_array(arr, 5)))  
 ```
 
 Output:
 ```py
-<generator object chunk_array at 0x776a6b4140>
+<generator object chunk_array at 0x77ab274140>
 [[2, 3, 12, 3, 3], [42, 42, 1, 43, 2], [42, 41, 4, 24, 32], [42, 3, 12, 32, 42], [42]]
 ```
 
 ## create_folder
 
 `create_folder(folder_name)`
 
@@ -144,17 +167,17 @@
 print(datetime_now("Asia/Jakarta"))  
 print(datetime_now("GMT"))  
 print(datetime_now("Etc/GMT+7"))  
 ```
 
 Output:
 ```py
-2024-04-28 20:23:44.929045+07:00
-2024-04-28 13:23:44.930043+00:00
-2024-04-28 06:23:44.931315-07:00
+2024-04-29 09:05:51.123977+07:00
+2024-04-29 02:05:51.125969+00:00
+2024-04-28 19:05:51.130704-07:00
 ```
 
 ## dict_first
 
 `dict_first(d: dict, remove=False)`
 
 Mengambil nilai (key, value) pertama dari dictionary dalam bentuk tuple.  
@@ -213,15 +236,15 @@
 ```python  
 var = [1, None, False, 0, "0", True, {}, ['eee']]  
 print(filter_empty(var))  
 ```
 
 Output:
 ```py
-<generator object filter_empty at 0x776a646d40>
+<generator object filter_empty at 0x77ab206d40>
 ```
 
 ## get_by_index
 
 `get_by_index(obj, index, on_error=None)`
 
 Mendapatkan value dari object berdasarkan indexnya.  
@@ -259,16 +282,16 @@
   
 print(get_class_method(ExampleGetClassMethod))  
 print(list(get_class_method(ExampleGetClassMethod)))  
 ```
 
 Output:
 ```py
-<generator object get_class_method at 0x776a647010>
-[<function ExampleGetClassMethod.a at 0x776a6b9760>, <function ExampleGetClassMethod.b at 0x776a6b9620>, <function ExampleGetClassMethod.c at 0x776a6b9800>, <function ExampleGetClassMethod.d at 0x776a6b98a0>]
+<generator object get_class_method at 0x77ab207010>
+[<function ExampleGetClassMethod.a at 0x77ab279760>, <function ExampleGetClassMethod.b at 0x77ab279620>, <function ExampleGetClassMethod.c at 0x77ab279800>, <function ExampleGetClassMethod.d at 0x77ab2798a0>]
 ```
 
 ## get_filemtime
 
 `get_filemtime(filename)`
 
 Mengambil informasi last modification time file dalam nano seconds  
@@ -416,146 +439,27 @@
 
 Output:
 ```py
 True
 True
 ```
 
-## ivars
-
-`ivars(obj, skip_underscore=True)`
-
-Membuat dictionary berdasarkan kategori untuk setiap  
-member dari object.  
-  
-```python  
-iprint(ivars(__import__('pypipr')))  
-```
-
-Output:
-```py
-{'module': {'ibuiltins': <module 'pypipr.ibuiltins' from '/data/data/com.termux/files/home/pypipr/pypipr/ibuiltins/__init__.py'>,
-            'iconsole': <module 'pypipr.iconsole' from '/data/data/com.termux/files/home/pypipr/pypipr/iconsole/__init__.py'>,
-            'idjango': <module 'pypipr.idjango' from '/data/data/com.termux/files/home/pypipr/pypipr/idjango/__init__.py'>,
-            'iengineering': <module 'pypipr.iengineering' from '/data/data/com.termux/files/home/pypipr/pypipr/iengineering/__init__.py'>,
-            'ifunctions': <module 'pypipr.ifunctions' from '/data/data/com.termux/files/home/pypipr/pypipr/ifunctions/__init__.py'>,
-            'iflow': <module 'pypipr.iflow' (<_frozen_importlib_external.NamespaceLoader object at 0x7770ee6f90>)>,
-            'asyncio': <module 'asyncio' from '/data/data/com.termux/files/usr/lib/python3.11/asyncio/__init__.py'>,
-            'colorama': <module 'colorama' from '/data/data/com.termux/files/usr/lib/python3.11/site-packages/colorama/__init__.py'>,
-            'csv': <module 'csv' from '/data/data/com.termux/files/usr/lib/python3.11/csv.py'>,
-            'datetime': <module 'datetime' from '/data/data/com.termux/files/usr/lib/python3.11/datetime.py'>,
-            'functools': <module 'functools' from '/data/data/com.termux/files/usr/lib/python3.11/functools.py'>,
-            'inspect': <module 'inspect' from '/data/data/com.termux/files/usr/lib/python3.11/inspect.py'>,
-            'io': <module 'io' (frozen)>,
-            'json': <module 'json' from '/data/data/com.termux/files/usr/lib/python3.11/json/__init__.py'>,
-            'lxml': <module 'lxml' from '/data/data/com.termux/files/usr/lib/python3.11/site-packages/lxml/__init__.py'>,
-            'math': <module 'math' from '/data/data/com.termux/files/usr/lib/python3.11/lib-dynload/math.cpython-311.so'>,
-            'multiprocessing': <module 'multiprocessing' from '/data/data/com.termux/files/usr/lib/python3.11/multiprocessing/__init__.py'>,
-            'operator': <module 'operator' from '/data/data/com.termux/files/usr/lib/python3.11/operator.py'>,
-            'os': <module 'os' (frozen)>,
-            'pathlib': <module 'pathlib' from '/data/data/com.termux/files/usr/lib/python3.11/pathlib.py'>,
-            'pint': <module 'pint' from '/data/data/com.termux/files/usr/lib/python3.11/site-packages/pint/__init__.py'>,
-            'pprint': <module 'pprint' from '/data/data/com.termux/files/usr/lib/python3.11/pprint.py'>,
-            'queue': <module 'queue' from '/data/data/com.termux/files/usr/lib/python3.11/queue.py'>,
-            'random': <module 'random' from '/data/data/com.termux/files/usr/lib/python3.11/random.py'>,
-            're': <module 're' from '/data/data/com.termux/files/usr/lib/python3.11/re/__init__.py'>,
-            'requests': <module 'requests' from '/data/data/com.termux/files/usr/lib/python3.11/site-packages/requests/__init__.py'>,
-            'string': <module 'string' from '/data/data/com.termux/files/usr/lib/python3.11/string.py'>,
-            'subprocess': <module 'subprocess' from '/data/data/com.termux/files/usr/lib/python3.11/subprocess.py'>,
-            'sys': <module 'sys' (built-in)>,
-            'textwrap': <module 'textwrap' from '/data/data/com.termux/files/usr/lib/python3.11/textwrap.py'>,
-            'threading': <module 'threading' from '/data/data/com.termux/files/usr/lib/python3.11/threading.py'>,
-            'time': <module 'time' (built-in)>,
-            'tzdata': <module 'tzdata' from '/data/data/com.termux/files/usr/lib/python3.11/site-packages/tzdata/__init__.py'>,
-            'uuid': <module 'uuid' from '/data/data/com.termux/files/usr/lib/python3.11/uuid.py'>,
-            'webbrowser': <module 'webbrowser' from '/data/data/com.termux/files/usr/lib/python3.11/webbrowser.py'>,
-            'yaml': <module 'yaml' from '/data/data/com.termux/files/usr/lib/python3.11/site-packages/yaml/__init__.py'>,
-            'zoneinfo': <module 'zoneinfo' from '/data/data/com.termux/files/usr/lib/python3.11/zoneinfo/__init__.py'>},
- 'class': {'ComparePerformance': <class 'pypipr.ibuiltins.ComparePerformance.ComparePerformance'>,
-           'RunParallel': <class 'pypipr.ibuiltins.RunParallel.RunParallel'>,
-           'APIMixinView': <class 'pypipr.idjango.APIMixinView.APIMixinView'>,
-           'PintUregQuantity': <class 'pint.Quantity'>},
- 'variable': {'LINUX': True,
-              'WINDOWS': False,
-              'PintUreg': <pint.registry.UnitRegistry object at 0x7776e3fd50>},
- 'function': {'avg': <function avg at 0x777bfb6d40>,
-              'basename': <function basename at 0x777bf868e0>,
-              'chr_to_int': <function chr_to_int at 0x7776d79080>,
-              'chunk_array': <function chunk_array at 0x7776d791c0>,
-              'create_folder': <function create_folder at 0x7776d793a0>,
-              'datetime_from_string': <function datetime_from_string at 0x7776d79580>,
-              'datetime_now': <function datetime_now at 0x7776e21620>,
-              'dict_first': <function dict_first at 0x7776e21580>,
-              'dirname': <function dirname at 0x7776e214e0>,
-              'exit_if_empty': <function exit_if_empty at 0x7776e213a0>,
-              'filter_empty': <function filter_empty at 0x7776e211c0>,
-              'get_by_index': <function get_by_index at 0x7776e20e00>,
-              'get_class_method': <function get_class_method at 0x7776e20cc0>,
-              'get_filemtime': <function get_filemtime at 0x7776e20b80>,
-              'get_filesize': <function get_filesize at 0x7776e209a0>,
-              'int_to_chr': <function int_to_chr at 0x7776e20900>,
-              'is_empty': <function is_empty at 0x7776e21260>,
-              'is_iterable': <function is_iterable at 0x7776e20fe0>,
-              'is_valid_url': <function is_valid_url at 0x7776e207c0>,
-              'ivars': <function ivars at 0x7776e20720>,
-              'password_generator': <function password_generator at 0x7776e205e0>,
-              'random_bool': <function random_bool at 0x7776e20400>,
-              'restart': <function restart at 0x7776e23880>,
-              'set_timeout': <function set_timeout at 0x7776e239c0>,
-              'sets_ordered': <function sets_ordered at 0x7776e23b00>,
-              'str_cmp': <function str_cmp at 0x7776e23ba0>,
-              'to_str': <function to_str at 0x7776e20f40>,
-              'choices': <function choices at 0x7776e23c40>,
-              'console_run': <function console_run at 0x7776e23ec0>,
-              'input_char': <function input_char at 0x7776e44040>,
-              'log': <function log at 0x7776e44220>,
-              'print_colorize': <function print_colorize at 0x7776e442c0>,
-              'print_dir': <function print_dir at 0x7776e44400>,
-              'print_log': <function print_log at 0x7776e440e0>,
-              'print_to_last_line': <function print_to_last_line at 0x7776e23e20>,
-              'text_colorize': <function text_colorize at 0x7776e23f60>,
-              'batch_calculate': <function batch_calculate at 0x7770ef1760>,
-              'batchmaker': <function batchmaker at 0x7776e44540>,
-              'calculate': <function calculate at 0x7770ef2480>,
-              'auto_reload': <function auto_reload at 0x7770ef2700>,
-              'github_pull': <function github_pull at 0x7770ef2200>,
-              'github_push': <function github_push at 0x7770ef28e0>,
-              'github_user': <function github_user at 0x7770ef2c00>,
-              'pip_freeze_without_version': <function pip_freeze_without_version at 0x7770c22160>,
-              'poetry_publish': <function poetry_publish at 0x7770c22340>,
-              'poetry_update_version': <function poetry_update_version at 0x7770c46b60>,
-              'iargv': <function iargv at 0x776d2702c0>,
-              'idumps': <function idumps at 0x776d270400>,
-              'idumps_html': <function idumps_html at 0x776d2d4e00>,
-              'ienv': <function ienv at 0x776d270540>,
-              'iexec': <function iexec at 0x776d2d5080>,
-              'ijoin': <function ijoin at 0x7770c220c0>,
-              'iloads': <function iloads at 0x776d2d5120>,
-              'iloads_html': <function iloads_html at 0x776d2d53a0>,
-              'iopen': <function iopen at 0x7770c223e0>,
-              'iprint': <function iprint at 0x776d2d5260>,
-              'irange': <function irange at 0x7770ef25c0>,
-              'ireplace': <function ireplace at 0x776d2d5440>,
-              'iscandir': <function iscandir at 0x776d2d7060>,
-              'isplit': <function isplit at 0x776d2d7100>}}
-```
-
 ## password_generator
 
 `password_generator(length=8, characters='abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789!"#$%&\'()*+,-./:;<=>?@[\\]^_`{|}~')`
 
 Membuat pssword secara acak  
   
 ```python  
 print(password_generator())  
 ```
 
 Output:
 ```py
-5M|h(ik`
+A"0&%upF
 ```
 
 ## random_bool
 
 `random_bool()`
 
 Menghasilkan nilai random True atau False.  
@@ -565,15 +469,15 @@
   
 ```python  
 print(random_bool())  
 ```
 
 Output:
 ```py
-True
+False
 ```
 
 ## restart
 
 `restart(*argv)`
 
 ## set_timeout
@@ -591,15 +495,15 @@
 print(x)  
 print("menghentikan timeout 7")  
 x.cancel()  
 ```
 
 Output:
 ```py
-<Timer(Thread-2, started 512858504432)>
+<Timer(Thread-2, started 513948798192)>
 menghentikan timeout 7
 ```
 
 ## sets_ordered
 
 `sets_ordered(iterator)`
 
@@ -609,15 +513,15 @@
 array = [2, 3, 12, 3, 3, 42, 42, 1, 43, 2, 42, 41, 4, 24, 32, 42, 3, 12, 32, 42, 42]  
 print(sets_ordered(array))  
 print(list(sets_ordered(array)))  
 ```
 
 Output:
 ```py
-<generator object sets_ordered at 0x776a6c42b0>
+<generator object sets_ordered at 0x77ab2842b0>
 [2, 3, 12, 42, 1, 43, 41, 4, 24, 32]
 ```
 
 ## str_cmp
 
 `str_cmp(t1, t2)`
 
@@ -763,29 +667,29 @@
              __doc__ : Path subclass for non-Windows systems.
 
     On a POSIX system, instantiating a Path should return this object.
     
            __enter__ : https:/www.google.com
           __fspath__ : https:/www.google.com
         __getstate__ : (None, {'_drv': '', '_root': '', '_parts': ['https:', 'www.google.com'], '_str': 'https:/www.google.com'})
-            __hash__ : -1747193618484435558
+            __hash__ : 8929491664327124594
             __init__ : None
    __init_subclass__ : None
           __module__ : pathlib
           __reduce__ : (<class 'pathlib.PosixPath'>, ('https:', 'www.google.com'))
             __repr__ : PosixPath('https:/www.google.com')
           __sizeof__ : 72
            __slots__ : ()
              __str__ : https:/www.google.com
     __subclasshook__ : NotImplemented
       _cached_cparts : ['https:', 'www.google.com']
              _cparts : ['https:', 'www.google.com']
                 _drv : 
-            _flavour : <pathlib._PosixFlavour object at 0x7776df0bd0>
-               _hash : -1747193618484435558
+            _flavour : <pathlib._PosixFlavour object at 0x77c09d8a90>
+               _hash : 8929491664327124594
               _parts : ['https:', 'www.google.com']
                _root : 
                 _str : https:/www.google.com
             absolute : /data/data/com.termux/files/home/pypipr/https:/www.google.com
               anchor : 
             as_posix : https:/www.google.com
                  cwd : /data/data/com.termux/files/home/pypipr
@@ -799,15 +703,15 @@
               is_dir : False
              is_fifo : False
              is_file : False
             is_mount : False
          is_reserved : False
            is_socket : False
           is_symlink : False
-             iterdir : <generator object Path.iterdir at 0x776a69c740>
+             iterdir : <generator object Path.iterdir at 0x77ab25cba0>
             joinpath : https:/www.google.com
                 name : www.google.com
               parent : https:
              parents : <PosixPath.parents>
                parts : ('https:', 'www.google.com')
              resolve : /data/data/com.termux/files/home/pypipr/https:/www.google.com
                 root : 
@@ -866,15 +770,15 @@
 ```python  
 print(batch_calculate("{1 10} m ** {1 3}"))  
 print(list(batch_calculate("{1 10} m ** {1 3}")))  
 ```
 
 Output:
 ```py
-<generator object batch_calculate at 0x776a647b50>
+<generator object batch_calculate at 0x77ab207b50>
 [('1 m ** 1', <Quantity(1, 'meter')>), ('1 m ** 2', <Quantity(1, 'meter ** 2')>), ('1 m ** 3', <Quantity(1, 'meter ** 3')>), ('2 m ** 1', <Quantity(2, 'meter')>), ('2 m ** 2', <Quantity(2, 'meter ** 2')>), ('2 m ** 3', <Quantity(2, 'meter ** 3')>), ('3 m ** 1', <Quantity(3, 'meter')>), ('3 m ** 2', <Quantity(3, 'meter ** 2')>), ('3 m ** 3', <Quantity(3, 'meter ** 3')>), ('4 m ** 1', <Quantity(4, 'meter')>), ('4 m ** 2', <Quantity(4, 'meter ** 2')>), ('4 m ** 3', <Quantity(4, 'meter ** 3')>), ('5 m ** 1', <Quantity(5, 'meter')>), ('5 m ** 2', <Quantity(5, 'meter ** 2')>), ('5 m ** 3', <Quantity(5, 'meter ** 3')>), ('6 m ** 1', <Quantity(6, 'meter')>), ('6 m ** 2', <Quantity(6, 'meter ** 2')>), ('6 m ** 3', <Quantity(6, 'meter ** 3')>), ('7 m ** 1', <Quantity(7, 'meter')>), ('7 m ** 2', <Quantity(7, 'meter ** 2')>), ('7 m ** 3', <Quantity(7, 'meter ** 3')>), ('8 m ** 1', <Quantity(8, 'meter')>), ('8 m ** 2', <Quantity(8, 'meter ** 2')>), ('8 m ** 3', <Quantity(8, 'meter ** 3')>), ('9 m ** 1', <Quantity(9, 'meter')>), ('9 m ** 2', <Quantity(9, 'meter ** 2')>), ('9 m ** 3', <Quantity(9, 'meter ** 3')>), ('10 m ** 1', <Quantity(10, 'meter')>), ('10 m ** 2', <Quantity(10, 'meter ** 2')>), ('10 m ** 3', <Quantity(10, 'meter ** 3')>)]
 ```
 
 ## batchmaker
 
 `batchmaker(pattern: str)`
 
@@ -891,15 +795,15 @@
 s = "Urutan {1/6/3} dan {10:9} dan {j k} dan {Z - A - 15} saja."  
 print(batchmaker(s))  
 print(list(batchmaker(s)))  
 ```
 
 Output:
 ```py
-<generator object batchmaker at 0x776a6b03a0>
+<generator object batchmaker at 0x77ab26c3a0>
 ['Urutan 1 dan 10 dan j dan Z saja.', 'Urutan 1 dan 10 dan j dan K saja.', 'Urutan 1 dan 10 dan k dan Z saja.', 'Urutan 1 dan 10 dan k dan K saja.', 'Urutan 1 dan 9 dan j dan Z saja.', 'Urutan 1 dan 9 dan j dan K saja.', 'Urutan 1 dan 9 dan k dan Z saja.', 'Urutan 1 dan 9 dan k dan K saja.', 'Urutan 4 dan 10 dan j dan Z saja.', 'Urutan 4 dan 10 dan j dan K saja.', 'Urutan 4 dan 10 dan k dan Z saja.', 'Urutan 4 dan 10 dan k dan K saja.', 'Urutan 4 dan 9 dan j dan Z saja.', 'Urutan 4 dan 9 dan j dan K saja.', 'Urutan 4 dan 9 dan k dan Z saja.', 'Urutan 4 dan 9 dan k dan K saja.']
 ```
 
 ## calculate
 
 `calculate(teks)`
 
@@ -1320,133 +1224,182 @@
 pprint.pprint(iloads_html(iopen("https://harga-emas.org/")), depth=10)  
 pprint.pprint(iloads_html(iopen("https://harga-emas.org/1-gram/")), depth=10)  
 ```
 
 Output:
 ```py
 (['Home', 'Emas 1 Gram', 'History', 'Trend', 'Perak 1 Gram', 'Pluang'],
- [['Harga Emas Hari Ini - Minggu, 28 April 2024'],
-  ['Spot Emas USD↑2.337,94 (+3,37) / oz',
+ [['Harga Emas Hari Ini - Senin, 29 April 2024'],
+  ['Spot Emas USD↓2.330,95 (-6,99) / oz',
    'Kurs IDR16.208,00 / USD',
-   'Emas IDR↑1.218.299 (+1.756) / gr'],
-  ['LM Antam (Jual)1.326.000 / gr', 'LM Antam (Beli)1.222.000 / gr']],
+   'Emas IDR↓1.214.656 (-3.642) / gr'],
+  ['LM Antam (Jual)↓1.325.000 (-1.000) / gr',
+   'LM Antam (Beli)↓1.221.000 (-1.000) / gr']],
  [['Harga Emas Hari Ini'],
   ['Gram', 'Gedung Antam Jakarta', 'Pegadaian'],
   ['per Gram (Rp)', 'per Batangan (Rp)', 'per Gram (Rp)', 'per Batangan (Rp)'],
   ['1000',
-   '1.267',
-   '1.266.600',
+   '1.266 (-1)',
+   '1.265.600 (-1.000)',
    '1.043.040 (+8.200)',
    '1.043.040.000 (+8.200.000)'],
   ['500',
-   '2.533',
-   '1.266.640',
+   '2.531 (-2)',
+   '1.265.640 (-1.000)',
    '1.043.082 (+8.200)',
    '521.541.000 (+4.100.000)'],
   ['250',
-   '5.068',
-   '1.267.060',
+   '5.064 (-4)',
+   '1.266.060 (-1.000)',
    '1.043.512 (+8.200)',
    '260.878.000 (+2.050.000)'],
   ['100',
-   '12.681',
-   '1.268.120',
+   '12.671 (-10)',
+   '1.267.120 (-1.000)',
    '1.044.600 (+8.200)',
    '104.460.000 (+820.000)'],
-  ['50', '25.378', '1.268.900', '1.045.400 (+8.200)', '52.270.000 (+410.000)'],
-  ['25', '50.819', '1.270.480', '1.047.040 (+8.200)', '26.176.000 (+205.000)'],
-  ['10', '127.550', '1.275.500', '1.052.200 (+8.200)', '10.522.000 (+82.000)'],
-  ['5', '256.200', '1.281.000', '1.057.800 (+8.200)', '5.289.000 (+41.000)'],
-  ['3', '429.222', '1.287.667', '1.064.667 (+8.000)', '3.194.000 (+24.000)'],
-  ['2', '648.000', '1.296.000', '1.073.500 (+8.500)', '2.147.000 (+17.000)'],
-  ['1', '1.326.000', '1.326.000', '1.104.000 (+8.000)', '1.104.000 (+8.000)'],
-  ['0.5', '2.852.000', '1.426.000', '1.208.000 (+8.000)', '604.000 (+4.000)'],
-  ['Update harga LM Antam :28 April 2024, pukul 08:07Harga pembelian kembali '
-   ':Rp. 1.222.000/gram',
+  ['50',
+   '25.358 (-20)',
+   '1.267.900 (-1.000)',
+   '1.045.400 (+8.200)',
+   '52.270.000 (+410.000)'],
+  ['25',
+   '50.779 (-40)',
+   '1.269.480 (-1.000)',
+   '1.047.040 (+8.200)',
+   '26.176.000 (+205.000)'],
+  ['10',
+   '127.450 (-100)',
+   '1.274.500 (-1.000)',
+   '1.052.200 (+8.200)',
+   '10.522.000 (+82.000)'],
+  ['5',
+   '256.000 (-200)',
+   '1.280.000 (-1.000)',
+   '1.057.800 (+8.200)',
+   '5.289.000 (+41.000)'],
+  ['3',
+   '428.889 (-333)',
+   '1.286.667 (-1.000)',
+   '1.064.667 (+8.000)',
+   '3.194.000 (+24.000)'],
+  ['2',
+   '647.500 (-500)',
+   '1.295.000 (-1.000)',
+   '1.073.500 (+8.500)',
+   '2.147.000 (+17.000)'],
+  ['1',
+   '1.325.000 (-1.000)',
+   '1.325.000 (-1.000)',
+   '1.104.000 (+8.000)',
+   '1.104.000 (+8.000)'],
+  ['0.5',
+   '2.850.000 (-2.000)',
+   '1.425.000 (-1.000)',
+   '1.208.000 (+8.000)',
+   '604.000 (+4.000)'],
+  ['Update harga LM Antam :29 April 2024, pukul 07:56Harga pembelian kembali '
+   ':Rp. 1.221.000/gram (-1.000)',
    'Update harga LM Pegadaian :31 Agustus 2023']],
- [['Spot Harga Emas Hari Ini (Market Close)'],
+ [['Spot Harga Emas Hari Ini (Market Open)'],
   ['Satuan', 'USD', 'Kurs\xa0Dollar', 'IDR'],
-  ['Ounce\xa0(oz)', '2.337,94 (+3,37)', '16.208,00', '37.893.332'],
-  ['Gram\xa0(gr)', '75,17', '16.208,00', '1.218.299 (+1.756)'],
-  ['Kilogram\xa0(kg)', '75.166,52', '16.208,00', '1.218.298.900'],
-  ['Update harga emas :28 April 2024, pukul 20:23Update kurs :28 April 2024, '
+  ['Ounce\xa0(oz)', '2.330,95 (-6,99)', '16.208,00', '37.780.038'],
+  ['Gram\xa0(gr)', '74,94', '16.208,00', '1.214.656 (-3.642)'],
+  ['Kilogram\xa0(kg)', '74.941,78', '16.208,00', '1.214.656.415'],
+  ['Update harga emas :29 April 2024, pukul 09:04Update kurs :28 April 2024, '
    'pukul 13:10']],
  [['Gram', 'UBS Gold 99.99%'],
   ['Jual', 'Beli'],
   ['/ Batang', '/ Gram', '/ Batang', '/ Gram'],
-  ['100', '126.812.000', '1.268.120', '124.985.000', '1.249.850'],
-  ['50', '63.445.000', '1.268.900', '62.545.000', '1.250.900'],
-  ['25', '31.762.000', '1.270.480', '31.375.000', '1.255.000'],
-  ['10', '12.755.000', '1.275.500', '12.600.000', '1.260.000'],
-  ['5', '6.405.000', '1.281.000', '6.352.000', '1.270.400'],
-  ['1', '1.326.000', '1.326.000', '1.303.000', '1.303.000'],
+  ['100',
+   '126.712.000 (-100.000)',
+   '1.267.120 (-1.000)',
+   '124.985.000',
+   '1.249.850'],
+  ['50',
+   '63.395.000 (-50.000)',
+   '1.267.900 (-1.000)',
+   '62.545.000',
+   '1.250.900'],
+  ['25',
+   '31.737.000 (-25.000)',
+   '1.269.480 (-1.000)',
+   '31.375.000',
+   '1.255.000'],
+  ['10',
+   '12.745.000 (-10.000)',
+   '1.274.500 (-1.000)',
+   '12.600.000',
+   '1.260.000'],
+  ['5', '6.400.000 (-5.000)', '1.280.000 (-1.000)', '6.352.000', '1.270.400'],
+  ['1', '1.325.000 (-1.000)', '1.325.000 (-1.000)', '1.303.000', '1.303.000'],
   ['', 'Update :26 April 2024, pukul 13:52']],
  [['Konversi Satuan'],
   ['Satuan', 'Ounce (oz)', 'Gram (gr)', 'Kilogram (kg)'],
   ['Ounce\xa0(oz)', '1', '31,1034767696', '0,0311034768'],
   ['Gram\xa0(gr)', '0,0321507466', '1', '0.001'],
   ['Kilogram\xa0(kg)', '32,1507466000', '1.000', '1']],
  [['Pergerakan Harga Emas Dunia'],
   ['Waktu', 'Emas'],
   ['Unit', 'USD', 'IDR'],
   ['Angka', '+/-', 'Angka', '+/-'],
   ['Hari Ini', 'Kurs', '', '', '16.208', '%'],
-  ['oz', '2.334,57', '+3,37+0,14%', '37.838.711', '+54.621+0,14%'],
-  ['gr', '75,06', '+0,11+0,14%', '1.216.543', '+1.756+0,14%'],
+  ['oz', '2.337,94', '-6,99-0,30%', '37.893.332', '-113.294-0,30%'],
+  ['gr', '75,17', '-0,22-0,30%', '1.218.299', '-3.642-0,30%'],
   ['30 Hari', 'Kurs', '', '', '15.853', '+355+2,24%'],
-  ['oz', '2.232,75', '+105,19+4,71%', '35.395.786', '+2.497.546+7,06%'],
-  ['gr', '71,78', '+3,38+4,71%', '1.138.001', '+80.298+7,06%'],
-  ['2 Bulan', 'Kurs', '', '', '15.655', '+553+3,53%'],
-  ['oz', '2.033,12', '+304,82+14,99%', '31.828.494', '+6.064.838+19,05%'],
-  ['gr', '65,37', '+9,80+14,99', '1.023.310', '+194.989+19,05%'],
-  ['6 Bulan', 'Kurs', '', '', '15.916', '+292+1,83%'],
-  ['oz', '1.991,61', '+346,33+17,39%', '31.698.465', '+6.194.867+19,54%'],
-  ['gr', '64,03', '+11,13+17,39%', '1.019.129', '+199.170+19,54%'],
+  ['oz', '2.232,75', '+98,20+4,40%', '35.395.786', '+2.384.252+6,74%'],
+  ['gr', '71,78', '+3,16+4,40%', '1.138.001', '+76.655+6,74%'],
+  ['2 Bulan', 'Kurs', '', '', '15.673', '+535+3,41%'],
+  ['oz', '2.045,83', '+285,12+13,94%', '32.064.294', '+5.715.744+17,83%'],
+  ['gr', '65,77', '+9,17+13,94', '1.030.891', '+183.765+17,83%'],
+  ['6 Bulan', 'Kurs', '', '', '15.897', '+311+1,96%'],
+  ['oz', '1.977,80', '+353,15+17,86%', '31.441.087', '+6.338.951+20,16%'],
+  ['gr', '63,59', '+11,35+17,86%', '1.010.854', '+203.802+20,16%'],
   ['1 Tahun', 'Kurs', '', '', '15.731', '+477+3,03%'],
-  ['oz', '1.823,86', '+514,08+28,19%', '28.691.142', '+9.202.190+32,07%'],
-  ['gr', '58,64', '+16,53+28,19%', '922.442', '+295.857+32,07%'],
+  ['oz', '1.823,86', '+507,09+27,80%', '28.691.142', '+9.088.896+31,68%'],
+  ['gr', '58,64', '+16,30+27,80%', '922.442', '+292.215+31,68%'],
   ['2 Tahun', 'Kurs', '', '', '14.418', '+1.790+12,42%'],
-  ['oz', '1.908,16', '+429,78+22,52%', '27.511.851', '+10.381.481+37,73%'],
-  ['gr', '61,35', '+13,82+22,52%', '884.527', '+333.772+37,73%'],
-  ['3 Tahun', 'Kurs', '', '', '14.510', '+1.698+11,70%'],
-  ['oz', '1.768,76', '+569,18+32,18%', '25.664.708', '+12.228.624+47,65%'],
-  ['gr', '56,87', '+18,30+32,18%', '825.140', '+393.159+47,65%'],
+  ['oz', '1.896,95', '+434,00+22,88%', '27.350.225', '+10.429.813+38,13%'],
+  ['gr', '60,99', '+13,95+22,88%', '879.330', '+335.326+38,13%'],
+  ['3 Tahun', 'Kurs', '', '', '14.468', '+1.740+12,03%'],
+  ['oz', '1.767,08', '+563,87+31,91%', '25.566.113', '+12.213.924+47,77%'],
+  ['gr', '56,81', '+18,13+31,91%', '821.970', '+392.687+47,77%'],
   ['5 Tahun', 'Kurs', '', '', '14.215', '+1.993+14,02%'],
-  ['oz', '1.283,64', '+1.054,30+82,13%', '18.246.943', '+19.646.389+107,67%'],
-  ['gr', '41,27', '+33,90+82,13%', '586.653', '+631.646+107,67%']])
+  ['oz', '1.280,61', '+1.050,34+82,02%', '18.203.871', '+19.576.166+107,54%'],
+  ['gr', '41,17', '+33,77+82,02%', '585.268', '+629.388+107,54%']])
 (['Home', 'Emas 1 Gram', 'History', 'Trend', 'Perak 1 Gram', 'Pluang'],
  [[''],
   ['Emas 24 KaratHarga Emas 1 Gram', ''],
-  ['USD', '75,17↓', '%'],
-  ['KURS', '16.241,30↓', '%'],
-  ['IDR', '1.220.801,94↓', '%'],
-  ['Minggu, 28 April 2024 20:23']],
+  ['USD', '74,92↓', '-0,25-0,33%'],
+  ['KURS', '16.234,15↓', '-7,15-0,04%'],
+  ['IDR', '1.216.308,20↓', '-4.493,74-0,37%'],
+  ['Senin, 29 April 2024 09:05']],
  [[''],
   ['Emas 1 Gram (IDR)Emas 1 Gram (USD)Kurs USD-IDR',
    'Hari Ini',
    '1 Bulan',
    '1 Tahun',
    '5 Tahun',
    'Max',
    '']],
  [['Pergerakkan Harga Emas 1 Gram'],
   ['', 'Penutupan Kemarin', 'Pergerakkan Hari Ini', 'Rata-rata'],
-  ['USD', '75,17', '75,17 - 75,17', '75,17'],
-  ['KURS', '16.241,30', '16.241,30 - 16.241,30', '16.241,30'],
-  ['IDR', '1.220.801,94', '1.220.801,94 - 1.220.801,94', '1.220.801,94'],
+  ['USD', '75,17', '74,92 - 75,17', '75,05'],
+  ['KURS', '16.241,30', '16.234,15 - 16.241,30', '16.237,73'],
+  ['IDR', '1.220.801,94', '1.216.308,20 - 1.220.801,94', '1.218.555,07'],
   [''],
   ['', 'Awal Tahun', 'Pergerakkan YTD', '+/- YTD'],
-  ['USD', '66,32', '64,07 - 77,14', '+8,85 (13,34%)'],
-  ['KURS', '15.390,10', '15.390,00 - 16.307,80', '+851,20 (5,53%)'],
-  ['IDR', '1.020.729,53', '997.660,12 - 1.256.829,06', '+200.072,41 (19,60%)'],
+  ['USD', '66,32', '64,07 - 77,14', '+8,60 (12,97%)'],
+  ['KURS', '15.390,10', '15.390,00 - 16.307,80', '+844,05 (5,48%)'],
+  ['IDR', '1.020.729,53', '997.660,12 - 1.256.829,06', '+195.578,67 (19,16%)'],
   [''],
   ['', 'Tahun Lalu / 52 Minggu', 'Pergerakkan 52 Minggu', '+/- 52 Minggu'],
-  ['USD', '63,78', '58,43 - 77,14', '+11,39 (17,86%)'],
-  ['KURS', '14.708,55', '14.669,40 - 16.307,80', '+1.532,75 (10,42%)'],
-  ['IDR', '938.054,69', '912.925,68 - 1.256.829,06', '+282.747,25 (30,14%)']])
+  ['USD', '64,04', '58,43 - 77,14', '+10,88 (16,99%)'],
+  ['KURS', '14.671,35', '14.669,40 - 16.307,80', '+1.562,80 (10,65%)'],
+  ['IDR', '939.568,98', '912.925,68 - 1.256.829,06', '+276.739,22 (29,45%)']])
 ```
 
 ## iopen
 
 `iopen(path, data=None, regex=None, css_select=None, xpath=None, file_append=False)`
 
 Membaca atau Tulis pada path yang bisa merupakan FILE maupun URL.  
@@ -1480,15 +1433,16 @@
 print(iopen("https://www.google.com/", dict(coba="dulu"), xpath="//a"))  
 ```
 
 Output:
 ```py
 8
 ['mana', 'aja']
-[<Element a at 0x776a6a7d90>, <Element a at 0x776a6f2990>, <Element a at 0x776a6f2a30>, <Element a at 0x776a6f2a80>, <Element a at 0x776a6f2ad0>, <Element a at 0x776a6f2b20>, <Element a at 0x776a6f2b70>, <Element a at 0x776a6f2bc0>, <Element a at 0x776a6f2c10>, <Element a at 0x776a6f2c60>, <Element a at 0x776a6f2cb0>, <Element a at 0x776a6f2d00>, <Element a at 0x776a6f2d50>, <Element a at 0x776a6f2da0>, <Element a at 0x776a6f2df0>, <Element a at 0x776a6f2e40>, <Element a at 0x776a6f2e90>, <Element a at 0x776a6f2ee0>]
+Timeout 3
+[<Element a at 0x77ab267200>, <Element a at 0x77ab2b2800>, <Element a at 0x77ab2b28a0>, <Element a at 0x77ab2b28f0>, <Element a at 0x77ab2b2940>, <Element a at 0x77ab2b2990>, <Element a at 0x77ab2b29e0>, <Element a at 0x77ab2b2a30>, <Element a at 0x77ab2b2a80>, <Element a at 0x77ab2b2ad0>, <Element a at 0x77ab2b2b20>, <Element a at 0x77ab2b2b70>, <Element a at 0x77ab2b2bc0>, <Element a at 0x77ab2b2c10>, <Element a at 0x77ab2b2c60>, <Element a at 0x77ab2b2cb0>, <Element a at 0x77ab2b2d00>, <Element a at 0x77ab2b2d50>, <Element a at 0x77ab2b2da0>, <Element a at 0x77ab2b2df0>]
 False
 ```
 
 ## iprint
 
 `iprint(*args, color=None, sort_dicts=False, **kwargs)`
 
@@ -1521,16 +1475,16 @@
 print(list(irange('a', 'z', 10)))  
 print(list(irange(1, '7')))  
 print(list(irange(10, 5)))  
 ```
 
 Output:
 ```py
-<generator object irange at 0x776a67abd0>
-<generator object irange at 0x776a67abd0>
+<generator object irange at 0x77ab23aac0>
+<generator object irange at 0x77ab23aac0>
 ['a', 'k', 'u']
 [1, 2, 3, 4, 5, 6, 7]
 [10, 9, 8, 7, 6, 5]
 ```
 
 ## ireplace
 
@@ -1565,15 +1519,15 @@
 ```python  
 print(iscandir())  
 print(list(iscandir("./", recursive=False, scan_file=False)))  
 ```
 
 Output:
 ```py
-<generator object iscandir at 0x776a6b4740>
+<generator object iscandir at 0x77ab274740>
 [PosixPath('.git'), PosixPath('.vscode'), PosixPath('pypipr'), PosixPath('__pycache__'), PosixPath('dist')]
 ```
 
 ## isplit
 
 `isplit(text, separator='', include_separator=False)`
 
@@ -1585,14 +1539,133 @@
 ```
 
 Output:
 ```py
 ['', 'ini', 'contoh', 'path', '']
 ```
 
+## ivars
+
+`ivars(obj, skip_underscore=True)`
+
+Membuat dictionary berdasarkan kategori untuk setiap  
+member dari object.  
+  
+```python  
+iprint(ivars(__import__('pypipr')))  
+```
+
+Output:
+```py
+{'module': {'ibuiltins': <module 'pypipr.ibuiltins' from '/data/data/com.termux/files/home/pypipr/pypipr/ibuiltins/__init__.py'>,
+            'iconsole': <module 'pypipr.iconsole' from '/data/data/com.termux/files/home/pypipr/pypipr/iconsole/__init__.py'>,
+            'idjango': <module 'pypipr.idjango' from '/data/data/com.termux/files/home/pypipr/pypipr/idjango/__init__.py'>,
+            'iengineering': <module 'pypipr.iengineering' from '/data/data/com.termux/files/home/pypipr/pypipr/iengineering/__init__.py'>,
+            'ifunctions': <module 'pypipr.ifunctions' from '/data/data/com.termux/files/home/pypipr/pypipr/ifunctions/__init__.py'>,
+            'iflow': <module 'pypipr.iflow' (<_frozen_importlib_external.NamespaceLoader object at 0x77b33bf290>)>,
+            'asyncio': <module 'asyncio' from '/data/data/com.termux/files/usr/lib/python3.11/asyncio/__init__.py'>,
+            'colorama': <module 'colorama' from '/data/data/com.termux/files/usr/lib/python3.11/site-packages/colorama/__init__.py'>,
+            'csv': <module 'csv' from '/data/data/com.termux/files/usr/lib/python3.11/csv.py'>,
+            'datetime': <module 'datetime' from '/data/data/com.termux/files/usr/lib/python3.11/datetime.py'>,
+            'functools': <module 'functools' from '/data/data/com.termux/files/usr/lib/python3.11/functools.py'>,
+            'inspect': <module 'inspect' from '/data/data/com.termux/files/usr/lib/python3.11/inspect.py'>,
+            'io': <module 'io' (frozen)>,
+            'json': <module 'json' from '/data/data/com.termux/files/usr/lib/python3.11/json/__init__.py'>,
+            'lxml': <module 'lxml' from '/data/data/com.termux/files/usr/lib/python3.11/site-packages/lxml/__init__.py'>,
+            'math': <module 'math' from '/data/data/com.termux/files/usr/lib/python3.11/lib-dynload/math.cpython-311.so'>,
+            'multiprocessing': <module 'multiprocessing' from '/data/data/com.termux/files/usr/lib/python3.11/multiprocessing/__init__.py'>,
+            'operator': <module 'operator' from '/data/data/com.termux/files/usr/lib/python3.11/operator.py'>,
+            'os': <module 'os' (frozen)>,
+            'pathlib': <module 'pathlib' from '/data/data/com.termux/files/usr/lib/python3.11/pathlib.py'>,
+            'pint': <module 'pint' from '/data/data/com.termux/files/usr/lib/python3.11/site-packages/pint/__init__.py'>,
+            'pprint': <module 'pprint' from '/data/data/com.termux/files/usr/lib/python3.11/pprint.py'>,
+            'queue': <module 'queue' from '/data/data/com.termux/files/usr/lib/python3.11/queue.py'>,
+            'random': <module 'random' from '/data/data/com.termux/files/usr/lib/python3.11/random.py'>,
+            're': <module 're' from '/data/data/com.termux/files/usr/lib/python3.11/re/__init__.py'>,
+            'requests': <module 'requests' from '/data/data/com.termux/files/usr/lib/python3.11/site-packages/requests/__init__.py'>,
+            'string': <module 'string' from '/data/data/com.termux/files/usr/lib/python3.11/string.py'>,
+            'subprocess': <module 'subprocess' from '/data/data/com.termux/files/usr/lib/python3.11/subprocess.py'>,
+            'sys': <module 'sys' (built-in)>,
+            'textwrap': <module 'textwrap' from '/data/data/com.termux/files/usr/lib/python3.11/textwrap.py'>,
+            'threading': <module 'threading' from '/data/data/com.termux/files/usr/lib/python3.11/threading.py'>,
+            'time': <module 'time' (built-in)>,
+            'tzdata': <module 'tzdata' from '/data/data/com.termux/files/usr/lib/python3.11/site-packages/tzdata/__init__.py'>,
+            'uuid': <module 'uuid' from '/data/data/com.termux/files/usr/lib/python3.11/uuid.py'>,
+            'webbrowser': <module 'webbrowser' from '/data/data/com.termux/files/usr/lib/python3.11/webbrowser.py'>,
+            'yaml': <module 'yaml' from '/data/data/com.termux/files/usr/lib/python3.11/site-packages/yaml/__init__.py'>,
+            'zoneinfo': <module 'zoneinfo' from '/data/data/com.termux/files/usr/lib/python3.11/zoneinfo/__init__.py'>},
+ 'class': {'ComparePerformance': <class 'pypipr.ibuiltins.ComparePerformance.ComparePerformance'>,
+           'RunParallel': <class 'pypipr.ibuiltins.RunParallel.RunParallel'>,
+           'APIMixinView': <class 'pypipr.idjango.APIMixinView.APIMixinView'>,
+           'PintUregQuantity': <class 'pint.Quantity'>},
+ 'variable': {'LINUX': True,
+              'WINDOWS': False,
+              'PintUreg': <pint.registry.UnitRegistry object at 0x77b794b750>},
+ 'function': {'avg': <function avg at 0x77c3b2ed40>,
+              'basename': <function basename at 0x77c3afe8e0>,
+              'chr_to_int': <function chr_to_int at 0x77c0961080>,
+              'chunk_array': <function chunk_array at 0x77c09611c0>,
+              'create_folder': <function create_folder at 0x77c09613a0>,
+              'datetime_from_string': <function datetime_from_string at 0x77c0961580>,
+              'datetime_now': <function datetime_now at 0x77c0a09620>,
+              'dict_first': <function dict_first at 0x77c0a09580>,
+              'dirname': <function dirname at 0x77c0a094e0>,
+              'exit_if_empty': <function exit_if_empty at 0x77c0a093a0>,
+              'filter_empty': <function filter_empty at 0x77c0a091c0>,
+              'get_by_index': <function get_by_index at 0x77c0a08e00>,
+              'get_class_method': <function get_class_method at 0x77c0a08cc0>,
+              'get_filemtime': <function get_filemtime at 0x77c0a08b80>,
+              'get_filesize': <function get_filesize at 0x77c0a089a0>,
+              'int_to_chr': <function int_to_chr at 0x77c0a08900>,
+              'is_empty': <function is_empty at 0x77c0a09260>,
+              'is_iterable': <function is_iterable at 0x77c0a08fe0>,
+              'is_valid_url': <function is_valid_url at 0x77c0a087c0>,
+              'password_generator': <function password_generator at 0x77c0a08680>,
+              'random_bool': <function random_bool at 0x77c0a084a0>,
+              'restart': <function restart at 0x77c0a0b7e0>,
+              'set_timeout': <function set_timeout at 0x77c0a0b920>,
+              'sets_ordered': <function sets_ordered at 0x77c0a0ba60>,
+              'str_cmp': <function str_cmp at 0x77c0a0bb00>,
+              'to_str': <function to_str at 0x77c0a08f40>,
+              'choices': <function choices at 0x77c0a0bba0>,
+              'console_run': <function console_run at 0x77c0a0be20>,
+              'input_char': <function input_char at 0x77c0a0bf60>,
+              'log': <function log at 0x77c0a2c180>,
+              'print_colorize': <function print_colorize at 0x77c0a2c220>,
+              'print_dir': <function print_dir at 0x77c0a2c360>,
+              'print_log': <function print_log at 0x77c0a2c040>,
+              'print_to_last_line': <function print_to_last_line at 0x77c0a0bd80>,
+              'text_colorize': <function text_colorize at 0x77c0a0bec0>,
+              'batch_calculate': <function batch_calculate at 0x77b33d96c0>,
+              'batchmaker': <function batchmaker at 0x77b33da160>,
+              'calculate': <function calculate at 0x77b33da3e0>,
+              'auto_reload': <function auto_reload at 0x77b33da660>,
+              'github_pull': <function github_pull at 0x77b33da5c0>,
+              'github_push': <function github_push at 0x77b33da840>,
+              'github_user': <function github_user at 0x77b33dab60>,
+              'pip_freeze_without_version': <function pip_freeze_without_version at 0x77b31020c0>,
+              'poetry_publish': <function poetry_publish at 0x77b31022a0>,
+              'poetry_update_version': <function poetry_update_version at 0x77b3126ac0>,
+              'iargv': <function iargv at 0x77ab484220>,
+              'idumps': <function idumps at 0x77ab484360>,
+              'idumps_html': <function idumps_html at 0x77ab4ecd60>,
+              'ienv': <function ienv at 0x77ab4844a0>,
+              'iexec': <function iexec at 0x77ab4ecfe0>,
+              'ijoin': <function ijoin at 0x77b3102020>,
+              'iloads': <function iloads at 0x77ab4ed080>,
+              'iloads_html': <function iloads_html at 0x77ab4ed300>,
+              'iopen': <function iopen at 0x77b3102340>,
+              'iprint': <function iprint at 0x77ab4ed1c0>,
+              'irange': <function irange at 0x77b33da520>,
+              'ireplace': <function ireplace at 0x77ab4ed3a0>,
+              'iscandir': <function iscandir at 0x77ab4eefc0>,
+              'isplit': <function isplit at 0x77ab4ef060>,
+              'ivars': <function ivars at 0x77ab4ef100>}}
+```
+
 # CLASS
 
 ## ComparePerformance
 
 `ComparePerformance()`
 
 Menjalankan seluruh method dalam class,  
@@ -1622,15 +1695,15 @@
 print(ExampleComparePerformance().compare_performance())  
 print(ExampleComparePerformance().compare_performance())  
 print(ExampleComparePerformance().compare_performance())  
 ```
 
 Output:
 ```py
-{'a': <generator object ExampleComparePerformance.a.<locals>.<genexpr> at 0x776a6c45f0>,
+{'a': <generator object ExampleComparePerformance.a.<locals>.<genexpr> at 0x77ab284450>,
  'b': (0, 1, 2, 3, 4, 5, 6, 7, 8, 9),
  'c': [0, 1, 2, 3, 4, 5, 6, 7, 8, 9],
  'd': [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]}
 {'a': 0, 'b': 0, 'c': 0, 'd': 0}
 {'a': 0, 'b': 0, 'c': 0, 'd': 0}
 {'a': 0, 'b': 0, 'c': 0, 'd': 0}
 {'a': 0, 'b': 0, 'c': 0, 'd': 0}
@@ -1754,7 +1827,8 @@
 class ExampleAPIView(APIMixinView, View):  
     pass  
 ```
 
 ## PintUregQuantity
 
 `PintUregQuantity(value, units=None)`
+
```

### Comparing `pypipr-1.0.98/PKG-INFO` & `pypipr-1.0.99/readme.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,7 @@
-Metadata-Version: 2.1
-Name: pypipr
-Version: 1.0.98
-Summary: The Python Package Index Project
-Author: ufiapjj
-Author-email: ufiapjj@gmail.com
-Requires-Python: >=3.9
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: colorama
-Requires-Dist: cssselect
-Requires-Dist: django
-Requires-Dist: getch ; platform_system == "Linux"
-Requires-Dist: lxml
-Requires-Dist: pint
-Requires-Dist: pyyaml
-Requires-Dist: requests
-Requires-Dist: tzdata
-Description-Content-Type: text/markdown
-
 
 # About
 The Python Package Index Project (pypipr)
 
 pypi : https://pypi.org/project/pypipr
 
 
@@ -116,15 +93,15 @@
 arr = [2, 3, 12, 3, 3, 42, 42, 1, 43, 2, 42, 41, 4, 24, 32, 42, 3, 12, 32, 42, 42]  
 print(chunk_array(arr, 5))  
 print(list(chunk_array(arr, 5)))  
 ```
 
 Output:
 ```py
-<generator object chunk_array at 0x776a6b4140>
+<generator object chunk_array at 0x77ab274140>
 [[2, 3, 12, 3, 3], [42, 42, 1, 43, 2], [42, 41, 4, 24, 32], [42, 3, 12, 32, 42], [42]]
 ```
 
 ## create_folder
 
 `create_folder(folder_name)`
 
@@ -167,17 +144,17 @@
 print(datetime_now("Asia/Jakarta"))  
 print(datetime_now("GMT"))  
 print(datetime_now("Etc/GMT+7"))  
 ```
 
 Output:
 ```py
-2024-04-28 20:23:44.929045+07:00
-2024-04-28 13:23:44.930043+00:00
-2024-04-28 06:23:44.931315-07:00
+2024-04-29 09:05:51.123977+07:00
+2024-04-29 02:05:51.125969+00:00
+2024-04-28 19:05:51.130704-07:00
 ```
 
 ## dict_first
 
 `dict_first(d: dict, remove=False)`
 
 Mengambil nilai (key, value) pertama dari dictionary dalam bentuk tuple.  
@@ -236,15 +213,15 @@
 ```python  
 var = [1, None, False, 0, "0", True, {}, ['eee']]  
 print(filter_empty(var))  
 ```
 
 Output:
 ```py
-<generator object filter_empty at 0x776a646d40>
+<generator object filter_empty at 0x77ab206d40>
 ```
 
 ## get_by_index
 
 `get_by_index(obj, index, on_error=None)`
 
 Mendapatkan value dari object berdasarkan indexnya.  
@@ -282,16 +259,16 @@
   
 print(get_class_method(ExampleGetClassMethod))  
 print(list(get_class_method(ExampleGetClassMethod)))  
 ```
 
 Output:
 ```py
-<generator object get_class_method at 0x776a647010>
-[<function ExampleGetClassMethod.a at 0x776a6b9760>, <function ExampleGetClassMethod.b at 0x776a6b9620>, <function ExampleGetClassMethod.c at 0x776a6b9800>, <function ExampleGetClassMethod.d at 0x776a6b98a0>]
+<generator object get_class_method at 0x77ab207010>
+[<function ExampleGetClassMethod.a at 0x77ab279760>, <function ExampleGetClassMethod.b at 0x77ab279620>, <function ExampleGetClassMethod.c at 0x77ab279800>, <function ExampleGetClassMethod.d at 0x77ab2798a0>]
 ```
 
 ## get_filemtime
 
 `get_filemtime(filename)`
 
 Mengambil informasi last modification time file dalam nano seconds  
@@ -439,146 +416,27 @@
 
 Output:
 ```py
 True
 True
 ```
 
-## ivars
-
-`ivars(obj, skip_underscore=True)`
-
-Membuat dictionary berdasarkan kategori untuk setiap  
-member dari object.  
-  
-```python  
-iprint(ivars(__import__('pypipr')))  
-```
-
-Output:
-```py
-{'module': {'ibuiltins': <module 'pypipr.ibuiltins' from '/data/data/com.termux/files/home/pypipr/pypipr/ibuiltins/__init__.py'>,
-            'iconsole': <module 'pypipr.iconsole' from '/data/data/com.termux/files/home/pypipr/pypipr/iconsole/__init__.py'>,
-            'idjango': <module 'pypipr.idjango' from '/data/data/com.termux/files/home/pypipr/pypipr/idjango/__init__.py'>,
-            'iengineering': <module 'pypipr.iengineering' from '/data/data/com.termux/files/home/pypipr/pypipr/iengineering/__init__.py'>,
-            'ifunctions': <module 'pypipr.ifunctions' from '/data/data/com.termux/files/home/pypipr/pypipr/ifunctions/__init__.py'>,
-            'iflow': <module 'pypipr.iflow' (<_frozen_importlib_external.NamespaceLoader object at 0x7770ee6f90>)>,
-            'asyncio': <module 'asyncio' from '/data/data/com.termux/files/usr/lib/python3.11/asyncio/__init__.py'>,
-            'colorama': <module 'colorama' from '/data/data/com.termux/files/usr/lib/python3.11/site-packages/colorama/__init__.py'>,
-            'csv': <module 'csv' from '/data/data/com.termux/files/usr/lib/python3.11/csv.py'>,
-            'datetime': <module 'datetime' from '/data/data/com.termux/files/usr/lib/python3.11/datetime.py'>,
-            'functools': <module 'functools' from '/data/data/com.termux/files/usr/lib/python3.11/functools.py'>,
-            'inspect': <module 'inspect' from '/data/data/com.termux/files/usr/lib/python3.11/inspect.py'>,
-            'io': <module 'io' (frozen)>,
-            'json': <module 'json' from '/data/data/com.termux/files/usr/lib/python3.11/json/__init__.py'>,
-            'lxml': <module 'lxml' from '/data/data/com.termux/files/usr/lib/python3.11/site-packages/lxml/__init__.py'>,
-            'math': <module 'math' from '/data/data/com.termux/files/usr/lib/python3.11/lib-dynload/math.cpython-311.so'>,
-            'multiprocessing': <module 'multiprocessing' from '/data/data/com.termux/files/usr/lib/python3.11/multiprocessing/__init__.py'>,
-            'operator': <module 'operator' from '/data/data/com.termux/files/usr/lib/python3.11/operator.py'>,
-            'os': <module 'os' (frozen)>,
-            'pathlib': <module 'pathlib' from '/data/data/com.termux/files/usr/lib/python3.11/pathlib.py'>,
-            'pint': <module 'pint' from '/data/data/com.termux/files/usr/lib/python3.11/site-packages/pint/__init__.py'>,
-            'pprint': <module 'pprint' from '/data/data/com.termux/files/usr/lib/python3.11/pprint.py'>,
-            'queue': <module 'queue' from '/data/data/com.termux/files/usr/lib/python3.11/queue.py'>,
-            'random': <module 'random' from '/data/data/com.termux/files/usr/lib/python3.11/random.py'>,
-            're': <module 're' from '/data/data/com.termux/files/usr/lib/python3.11/re/__init__.py'>,
-            'requests': <module 'requests' from '/data/data/com.termux/files/usr/lib/python3.11/site-packages/requests/__init__.py'>,
-            'string': <module 'string' from '/data/data/com.termux/files/usr/lib/python3.11/string.py'>,
-            'subprocess': <module 'subprocess' from '/data/data/com.termux/files/usr/lib/python3.11/subprocess.py'>,
-            'sys': <module 'sys' (built-in)>,
-            'textwrap': <module 'textwrap' from '/data/data/com.termux/files/usr/lib/python3.11/textwrap.py'>,
-            'threading': <module 'threading' from '/data/data/com.termux/files/usr/lib/python3.11/threading.py'>,
-            'time': <module 'time' (built-in)>,
-            'tzdata': <module 'tzdata' from '/data/data/com.termux/files/usr/lib/python3.11/site-packages/tzdata/__init__.py'>,
-            'uuid': <module 'uuid' from '/data/data/com.termux/files/usr/lib/python3.11/uuid.py'>,
-            'webbrowser': <module 'webbrowser' from '/data/data/com.termux/files/usr/lib/python3.11/webbrowser.py'>,
-            'yaml': <module 'yaml' from '/data/data/com.termux/files/usr/lib/python3.11/site-packages/yaml/__init__.py'>,
-            'zoneinfo': <module 'zoneinfo' from '/data/data/com.termux/files/usr/lib/python3.11/zoneinfo/__init__.py'>},
- 'class': {'ComparePerformance': <class 'pypipr.ibuiltins.ComparePerformance.ComparePerformance'>,
-           'RunParallel': <class 'pypipr.ibuiltins.RunParallel.RunParallel'>,
-           'APIMixinView': <class 'pypipr.idjango.APIMixinView.APIMixinView'>,
-           'PintUregQuantity': <class 'pint.Quantity'>},
- 'variable': {'LINUX': True,
-              'WINDOWS': False,
-              'PintUreg': <pint.registry.UnitRegistry object at 0x7776e3fd50>},
- 'function': {'avg': <function avg at 0x777bfb6d40>,
-              'basename': <function basename at 0x777bf868e0>,
-              'chr_to_int': <function chr_to_int at 0x7776d79080>,
-              'chunk_array': <function chunk_array at 0x7776d791c0>,
-              'create_folder': <function create_folder at 0x7776d793a0>,
-              'datetime_from_string': <function datetime_from_string at 0x7776d79580>,
-              'datetime_now': <function datetime_now at 0x7776e21620>,
-              'dict_first': <function dict_first at 0x7776e21580>,
-              'dirname': <function dirname at 0x7776e214e0>,
-              'exit_if_empty': <function exit_if_empty at 0x7776e213a0>,
-              'filter_empty': <function filter_empty at 0x7776e211c0>,
-              'get_by_index': <function get_by_index at 0x7776e20e00>,
-              'get_class_method': <function get_class_method at 0x7776e20cc0>,
-              'get_filemtime': <function get_filemtime at 0x7776e20b80>,
-              'get_filesize': <function get_filesize at 0x7776e209a0>,
-              'int_to_chr': <function int_to_chr at 0x7776e20900>,
-              'is_empty': <function is_empty at 0x7776e21260>,
-              'is_iterable': <function is_iterable at 0x7776e20fe0>,
-              'is_valid_url': <function is_valid_url at 0x7776e207c0>,
-              'ivars': <function ivars at 0x7776e20720>,
-              'password_generator': <function password_generator at 0x7776e205e0>,
-              'random_bool': <function random_bool at 0x7776e20400>,
-              'restart': <function restart at 0x7776e23880>,
-              'set_timeout': <function set_timeout at 0x7776e239c0>,
-              'sets_ordered': <function sets_ordered at 0x7776e23b00>,
-              'str_cmp': <function str_cmp at 0x7776e23ba0>,
-              'to_str': <function to_str at 0x7776e20f40>,
-              'choices': <function choices at 0x7776e23c40>,
-              'console_run': <function console_run at 0x7776e23ec0>,
-              'input_char': <function input_char at 0x7776e44040>,
-              'log': <function log at 0x7776e44220>,
-              'print_colorize': <function print_colorize at 0x7776e442c0>,
-              'print_dir': <function print_dir at 0x7776e44400>,
-              'print_log': <function print_log at 0x7776e440e0>,
-              'print_to_last_line': <function print_to_last_line at 0x7776e23e20>,
-              'text_colorize': <function text_colorize at 0x7776e23f60>,
-              'batch_calculate': <function batch_calculate at 0x7770ef1760>,
-              'batchmaker': <function batchmaker at 0x7776e44540>,
-              'calculate': <function calculate at 0x7770ef2480>,
-              'auto_reload': <function auto_reload at 0x7770ef2700>,
-              'github_pull': <function github_pull at 0x7770ef2200>,
-              'github_push': <function github_push at 0x7770ef28e0>,
-              'github_user': <function github_user at 0x7770ef2c00>,
-              'pip_freeze_without_version': <function pip_freeze_without_version at 0x7770c22160>,
-              'poetry_publish': <function poetry_publish at 0x7770c22340>,
-              'poetry_update_version': <function poetry_update_version at 0x7770c46b60>,
-              'iargv': <function iargv at 0x776d2702c0>,
-              'idumps': <function idumps at 0x776d270400>,
-              'idumps_html': <function idumps_html at 0x776d2d4e00>,
-              'ienv': <function ienv at 0x776d270540>,
-              'iexec': <function iexec at 0x776d2d5080>,
-              'ijoin': <function ijoin at 0x7770c220c0>,
-              'iloads': <function iloads at 0x776d2d5120>,
-              'iloads_html': <function iloads_html at 0x776d2d53a0>,
-              'iopen': <function iopen at 0x7770c223e0>,
-              'iprint': <function iprint at 0x776d2d5260>,
-              'irange': <function irange at 0x7770ef25c0>,
-              'ireplace': <function ireplace at 0x776d2d5440>,
-              'iscandir': <function iscandir at 0x776d2d7060>,
-              'isplit': <function isplit at 0x776d2d7100>}}
-```
-
 ## password_generator
 
 `password_generator(length=8, characters='abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789!"#$%&\'()*+,-./:;<=>?@[\\]^_`{|}~')`
 
 Membuat pssword secara acak  
   
 ```python  
 print(password_generator())  
 ```
 
 Output:
 ```py
-5M|h(ik`
+A"0&%upF
 ```
 
 ## random_bool
 
 `random_bool()`
 
 Menghasilkan nilai random True atau False.  
@@ -588,15 +446,15 @@
   
 ```python  
 print(random_bool())  
 ```
 
 Output:
 ```py
-True
+False
 ```
 
 ## restart
 
 `restart(*argv)`
 
 ## set_timeout
@@ -614,15 +472,15 @@
 print(x)  
 print("menghentikan timeout 7")  
 x.cancel()  
 ```
 
 Output:
 ```py
-<Timer(Thread-2, started 512858504432)>
+<Timer(Thread-2, started 513948798192)>
 menghentikan timeout 7
 ```
 
 ## sets_ordered
 
 `sets_ordered(iterator)`
 
@@ -632,15 +490,15 @@
 array = [2, 3, 12, 3, 3, 42, 42, 1, 43, 2, 42, 41, 4, 24, 32, 42, 3, 12, 32, 42, 42]  
 print(sets_ordered(array))  
 print(list(sets_ordered(array)))  
 ```
 
 Output:
 ```py
-<generator object sets_ordered at 0x776a6c42b0>
+<generator object sets_ordered at 0x77ab2842b0>
 [2, 3, 12, 42, 1, 43, 41, 4, 24, 32]
 ```
 
 ## str_cmp
 
 `str_cmp(t1, t2)`
 
@@ -786,29 +644,29 @@
              __doc__ : Path subclass for non-Windows systems.
 
     On a POSIX system, instantiating a Path should return this object.
     
            __enter__ : https:/www.google.com
           __fspath__ : https:/www.google.com
         __getstate__ : (None, {'_drv': '', '_root': '', '_parts': ['https:', 'www.google.com'], '_str': 'https:/www.google.com'})
-            __hash__ : -1747193618484435558
+            __hash__ : 8929491664327124594
             __init__ : None
    __init_subclass__ : None
           __module__ : pathlib
           __reduce__ : (<class 'pathlib.PosixPath'>, ('https:', 'www.google.com'))
             __repr__ : PosixPath('https:/www.google.com')
           __sizeof__ : 72
            __slots__ : ()
              __str__ : https:/www.google.com
     __subclasshook__ : NotImplemented
       _cached_cparts : ['https:', 'www.google.com']
              _cparts : ['https:', 'www.google.com']
                 _drv : 
-            _flavour : <pathlib._PosixFlavour object at 0x7776df0bd0>
-               _hash : -1747193618484435558
+            _flavour : <pathlib._PosixFlavour object at 0x77c09d8a90>
+               _hash : 8929491664327124594
               _parts : ['https:', 'www.google.com']
                _root : 
                 _str : https:/www.google.com
             absolute : /data/data/com.termux/files/home/pypipr/https:/www.google.com
               anchor : 
             as_posix : https:/www.google.com
                  cwd : /data/data/com.termux/files/home/pypipr
@@ -822,15 +680,15 @@
               is_dir : False
              is_fifo : False
              is_file : False
             is_mount : False
          is_reserved : False
            is_socket : False
           is_symlink : False
-             iterdir : <generator object Path.iterdir at 0x776a69c740>
+             iterdir : <generator object Path.iterdir at 0x77ab25cba0>
             joinpath : https:/www.google.com
                 name : www.google.com
               parent : https:
              parents : <PosixPath.parents>
                parts : ('https:', 'www.google.com')
              resolve : /data/data/com.termux/files/home/pypipr/https:/www.google.com
                 root : 
@@ -889,15 +747,15 @@
 ```python  
 print(batch_calculate("{1 10} m ** {1 3}"))  
 print(list(batch_calculate("{1 10} m ** {1 3}")))  
 ```
 
 Output:
 ```py
-<generator object batch_calculate at 0x776a647b50>
+<generator object batch_calculate at 0x77ab207b50>
 [('1 m ** 1', <Quantity(1, 'meter')>), ('1 m ** 2', <Quantity(1, 'meter ** 2')>), ('1 m ** 3', <Quantity(1, 'meter ** 3')>), ('2 m ** 1', <Quantity(2, 'meter')>), ('2 m ** 2', <Quantity(2, 'meter ** 2')>), ('2 m ** 3', <Quantity(2, 'meter ** 3')>), ('3 m ** 1', <Quantity(3, 'meter')>), ('3 m ** 2', <Quantity(3, 'meter ** 2')>), ('3 m ** 3', <Quantity(3, 'meter ** 3')>), ('4 m ** 1', <Quantity(4, 'meter')>), ('4 m ** 2', <Quantity(4, 'meter ** 2')>), ('4 m ** 3', <Quantity(4, 'meter ** 3')>), ('5 m ** 1', <Quantity(5, 'meter')>), ('5 m ** 2', <Quantity(5, 'meter ** 2')>), ('5 m ** 3', <Quantity(5, 'meter ** 3')>), ('6 m ** 1', <Quantity(6, 'meter')>), ('6 m ** 2', <Quantity(6, 'meter ** 2')>), ('6 m ** 3', <Quantity(6, 'meter ** 3')>), ('7 m ** 1', <Quantity(7, 'meter')>), ('7 m ** 2', <Quantity(7, 'meter ** 2')>), ('7 m ** 3', <Quantity(7, 'meter ** 3')>), ('8 m ** 1', <Quantity(8, 'meter')>), ('8 m ** 2', <Quantity(8, 'meter ** 2')>), ('8 m ** 3', <Quantity(8, 'meter ** 3')>), ('9 m ** 1', <Quantity(9, 'meter')>), ('9 m ** 2', <Quantity(9, 'meter ** 2')>), ('9 m ** 3', <Quantity(9, 'meter ** 3')>), ('10 m ** 1', <Quantity(10, 'meter')>), ('10 m ** 2', <Quantity(10, 'meter ** 2')>), ('10 m ** 3', <Quantity(10, 'meter ** 3')>)]
 ```
 
 ## batchmaker
 
 `batchmaker(pattern: str)`
 
@@ -914,15 +772,15 @@
 s = "Urutan {1/6/3} dan {10:9} dan {j k} dan {Z - A - 15} saja."  
 print(batchmaker(s))  
 print(list(batchmaker(s)))  
 ```
 
 Output:
 ```py
-<generator object batchmaker at 0x776a6b03a0>
+<generator object batchmaker at 0x77ab26c3a0>
 ['Urutan 1 dan 10 dan j dan Z saja.', 'Urutan 1 dan 10 dan j dan K saja.', 'Urutan 1 dan 10 dan k dan Z saja.', 'Urutan 1 dan 10 dan k dan K saja.', 'Urutan 1 dan 9 dan j dan Z saja.', 'Urutan 1 dan 9 dan j dan K saja.', 'Urutan 1 dan 9 dan k dan Z saja.', 'Urutan 1 dan 9 dan k dan K saja.', 'Urutan 4 dan 10 dan j dan Z saja.', 'Urutan 4 dan 10 dan j dan K saja.', 'Urutan 4 dan 10 dan k dan Z saja.', 'Urutan 4 dan 10 dan k dan K saja.', 'Urutan 4 dan 9 dan j dan Z saja.', 'Urutan 4 dan 9 dan j dan K saja.', 'Urutan 4 dan 9 dan k dan Z saja.', 'Urutan 4 dan 9 dan k dan K saja.']
 ```
 
 ## calculate
 
 `calculate(teks)`
 
@@ -1343,133 +1201,182 @@
 pprint.pprint(iloads_html(iopen("https://harga-emas.org/")), depth=10)  
 pprint.pprint(iloads_html(iopen("https://harga-emas.org/1-gram/")), depth=10)  
 ```
 
 Output:
 ```py
 (['Home', 'Emas 1 Gram', 'History', 'Trend', 'Perak 1 Gram', 'Pluang'],
- [['Harga Emas Hari Ini - Minggu, 28 April 2024'],
-  ['Spot Emas USD↑2.337,94 (+3,37) / oz',
+ [['Harga Emas Hari Ini - Senin, 29 April 2024'],
+  ['Spot Emas USD↓2.330,95 (-6,99) / oz',
    'Kurs IDR16.208,00 / USD',
-   'Emas IDR↑1.218.299 (+1.756) / gr'],
-  ['LM Antam (Jual)1.326.000 / gr', 'LM Antam (Beli)1.222.000 / gr']],
+   'Emas IDR↓1.214.656 (-3.642) / gr'],
+  ['LM Antam (Jual)↓1.325.000 (-1.000) / gr',
+   'LM Antam (Beli)↓1.221.000 (-1.000) / gr']],
  [['Harga Emas Hari Ini'],
   ['Gram', 'Gedung Antam Jakarta', 'Pegadaian'],
   ['per Gram (Rp)', 'per Batangan (Rp)', 'per Gram (Rp)', 'per Batangan (Rp)'],
   ['1000',
-   '1.267',
-   '1.266.600',
+   '1.266 (-1)',
+   '1.265.600 (-1.000)',
    '1.043.040 (+8.200)',
    '1.043.040.000 (+8.200.000)'],
   ['500',
-   '2.533',
-   '1.266.640',
+   '2.531 (-2)',
+   '1.265.640 (-1.000)',
    '1.043.082 (+8.200)',
    '521.541.000 (+4.100.000)'],
   ['250',
-   '5.068',
-   '1.267.060',
+   '5.064 (-4)',
+   '1.266.060 (-1.000)',
    '1.043.512 (+8.200)',
    '260.878.000 (+2.050.000)'],
   ['100',
-   '12.681',
-   '1.268.120',
+   '12.671 (-10)',
+   '1.267.120 (-1.000)',
    '1.044.600 (+8.200)',
    '104.460.000 (+820.000)'],
-  ['50', '25.378', '1.268.900', '1.045.400 (+8.200)', '52.270.000 (+410.000)'],
-  ['25', '50.819', '1.270.480', '1.047.040 (+8.200)', '26.176.000 (+205.000)'],
-  ['10', '127.550', '1.275.500', '1.052.200 (+8.200)', '10.522.000 (+82.000)'],
-  ['5', '256.200', '1.281.000', '1.057.800 (+8.200)', '5.289.000 (+41.000)'],
-  ['3', '429.222', '1.287.667', '1.064.667 (+8.000)', '3.194.000 (+24.000)'],
-  ['2', '648.000', '1.296.000', '1.073.500 (+8.500)', '2.147.000 (+17.000)'],
-  ['1', '1.326.000', '1.326.000', '1.104.000 (+8.000)', '1.104.000 (+8.000)'],
-  ['0.5', '2.852.000', '1.426.000', '1.208.000 (+8.000)', '604.000 (+4.000)'],
-  ['Update harga LM Antam :28 April 2024, pukul 08:07Harga pembelian kembali '
-   ':Rp. 1.222.000/gram',
+  ['50',
+   '25.358 (-20)',
+   '1.267.900 (-1.000)',
+   '1.045.400 (+8.200)',
+   '52.270.000 (+410.000)'],
+  ['25',
+   '50.779 (-40)',
+   '1.269.480 (-1.000)',
+   '1.047.040 (+8.200)',
+   '26.176.000 (+205.000)'],
+  ['10',
+   '127.450 (-100)',
+   '1.274.500 (-1.000)',
+   '1.052.200 (+8.200)',
+   '10.522.000 (+82.000)'],
+  ['5',
+   '256.000 (-200)',
+   '1.280.000 (-1.000)',
+   '1.057.800 (+8.200)',
+   '5.289.000 (+41.000)'],
+  ['3',
+   '428.889 (-333)',
+   '1.286.667 (-1.000)',
+   '1.064.667 (+8.000)',
+   '3.194.000 (+24.000)'],
+  ['2',
+   '647.500 (-500)',
+   '1.295.000 (-1.000)',
+   '1.073.500 (+8.500)',
+   '2.147.000 (+17.000)'],
+  ['1',
+   '1.325.000 (-1.000)',
+   '1.325.000 (-1.000)',
+   '1.104.000 (+8.000)',
+   '1.104.000 (+8.000)'],
+  ['0.5',
+   '2.850.000 (-2.000)',
+   '1.425.000 (-1.000)',
+   '1.208.000 (+8.000)',
+   '604.000 (+4.000)'],
+  ['Update harga LM Antam :29 April 2024, pukul 07:56Harga pembelian kembali '
+   ':Rp. 1.221.000/gram (-1.000)',
    'Update harga LM Pegadaian :31 Agustus 2023']],
- [['Spot Harga Emas Hari Ini (Market Close)'],
+ [['Spot Harga Emas Hari Ini (Market Open)'],
   ['Satuan', 'USD', 'Kurs\xa0Dollar', 'IDR'],
-  ['Ounce\xa0(oz)', '2.337,94 (+3,37)', '16.208,00', '37.893.332'],
-  ['Gram\xa0(gr)', '75,17', '16.208,00', '1.218.299 (+1.756)'],
-  ['Kilogram\xa0(kg)', '75.166,52', '16.208,00', '1.218.298.900'],
-  ['Update harga emas :28 April 2024, pukul 20:23Update kurs :28 April 2024, '
+  ['Ounce\xa0(oz)', '2.330,95 (-6,99)', '16.208,00', '37.780.038'],
+  ['Gram\xa0(gr)', '74,94', '16.208,00', '1.214.656 (-3.642)'],
+  ['Kilogram\xa0(kg)', '74.941,78', '16.208,00', '1.214.656.415'],
+  ['Update harga emas :29 April 2024, pukul 09:04Update kurs :28 April 2024, '
    'pukul 13:10']],
  [['Gram', 'UBS Gold 99.99%'],
   ['Jual', 'Beli'],
   ['/ Batang', '/ Gram', '/ Batang', '/ Gram'],
-  ['100', '126.812.000', '1.268.120', '124.985.000', '1.249.850'],
-  ['50', '63.445.000', '1.268.900', '62.545.000', '1.250.900'],
-  ['25', '31.762.000', '1.270.480', '31.375.000', '1.255.000'],
-  ['10', '12.755.000', '1.275.500', '12.600.000', '1.260.000'],
-  ['5', '6.405.000', '1.281.000', '6.352.000', '1.270.400'],
-  ['1', '1.326.000', '1.326.000', '1.303.000', '1.303.000'],
+  ['100',
+   '126.712.000 (-100.000)',
+   '1.267.120 (-1.000)',
+   '124.985.000',
+   '1.249.850'],
+  ['50',
+   '63.395.000 (-50.000)',
+   '1.267.900 (-1.000)',
+   '62.545.000',
+   '1.250.900'],
+  ['25',
+   '31.737.000 (-25.000)',
+   '1.269.480 (-1.000)',
+   '31.375.000',
+   '1.255.000'],
+  ['10',
+   '12.745.000 (-10.000)',
+   '1.274.500 (-1.000)',
+   '12.600.000',
+   '1.260.000'],
+  ['5', '6.400.000 (-5.000)', '1.280.000 (-1.000)', '6.352.000', '1.270.400'],
+  ['1', '1.325.000 (-1.000)', '1.325.000 (-1.000)', '1.303.000', '1.303.000'],
   ['', 'Update :26 April 2024, pukul 13:52']],
  [['Konversi Satuan'],
   ['Satuan', 'Ounce (oz)', 'Gram (gr)', 'Kilogram (kg)'],
   ['Ounce\xa0(oz)', '1', '31,1034767696', '0,0311034768'],
   ['Gram\xa0(gr)', '0,0321507466', '1', '0.001'],
   ['Kilogram\xa0(kg)', '32,1507466000', '1.000', '1']],
  [['Pergerakan Harga Emas Dunia'],
   ['Waktu', 'Emas'],
   ['Unit', 'USD', 'IDR'],
   ['Angka', '+/-', 'Angka', '+/-'],
   ['Hari Ini', 'Kurs', '', '', '16.208', '%'],
-  ['oz', '2.334,57', '+3,37+0,14%', '37.838.711', '+54.621+0,14%'],
-  ['gr', '75,06', '+0,11+0,14%', '1.216.543', '+1.756+0,14%'],
+  ['oz', '2.337,94', '-6,99-0,30%', '37.893.332', '-113.294-0,30%'],
+  ['gr', '75,17', '-0,22-0,30%', '1.218.299', '-3.642-0,30%'],
   ['30 Hari', 'Kurs', '', '', '15.853', '+355+2,24%'],
-  ['oz', '2.232,75', '+105,19+4,71%', '35.395.786', '+2.497.546+7,06%'],
-  ['gr', '71,78', '+3,38+4,71%', '1.138.001', '+80.298+7,06%'],
-  ['2 Bulan', 'Kurs', '', '', '15.655', '+553+3,53%'],
-  ['oz', '2.033,12', '+304,82+14,99%', '31.828.494', '+6.064.838+19,05%'],
-  ['gr', '65,37', '+9,80+14,99', '1.023.310', '+194.989+19,05%'],
-  ['6 Bulan', 'Kurs', '', '', '15.916', '+292+1,83%'],
-  ['oz', '1.991,61', '+346,33+17,39%', '31.698.465', '+6.194.867+19,54%'],
-  ['gr', '64,03', '+11,13+17,39%', '1.019.129', '+199.170+19,54%'],
+  ['oz', '2.232,75', '+98,20+4,40%', '35.395.786', '+2.384.252+6,74%'],
+  ['gr', '71,78', '+3,16+4,40%', '1.138.001', '+76.655+6,74%'],
+  ['2 Bulan', 'Kurs', '', '', '15.673', '+535+3,41%'],
+  ['oz', '2.045,83', '+285,12+13,94%', '32.064.294', '+5.715.744+17,83%'],
+  ['gr', '65,77', '+9,17+13,94', '1.030.891', '+183.765+17,83%'],
+  ['6 Bulan', 'Kurs', '', '', '15.897', '+311+1,96%'],
+  ['oz', '1.977,80', '+353,15+17,86%', '31.441.087', '+6.338.951+20,16%'],
+  ['gr', '63,59', '+11,35+17,86%', '1.010.854', '+203.802+20,16%'],
   ['1 Tahun', 'Kurs', '', '', '15.731', '+477+3,03%'],
-  ['oz', '1.823,86', '+514,08+28,19%', '28.691.142', '+9.202.190+32,07%'],
-  ['gr', '58,64', '+16,53+28,19%', '922.442', '+295.857+32,07%'],
+  ['oz', '1.823,86', '+507,09+27,80%', '28.691.142', '+9.088.896+31,68%'],
+  ['gr', '58,64', '+16,30+27,80%', '922.442', '+292.215+31,68%'],
   ['2 Tahun', 'Kurs', '', '', '14.418', '+1.790+12,42%'],
-  ['oz', '1.908,16', '+429,78+22,52%', '27.511.851', '+10.381.481+37,73%'],
-  ['gr', '61,35', '+13,82+22,52%', '884.527', '+333.772+37,73%'],
-  ['3 Tahun', 'Kurs', '', '', '14.510', '+1.698+11,70%'],
-  ['oz', '1.768,76', '+569,18+32,18%', '25.664.708', '+12.228.624+47,65%'],
-  ['gr', '56,87', '+18,30+32,18%', '825.140', '+393.159+47,65%'],
+  ['oz', '1.896,95', '+434,00+22,88%', '27.350.225', '+10.429.813+38,13%'],
+  ['gr', '60,99', '+13,95+22,88%', '879.330', '+335.326+38,13%'],
+  ['3 Tahun', 'Kurs', '', '', '14.468', '+1.740+12,03%'],
+  ['oz', '1.767,08', '+563,87+31,91%', '25.566.113', '+12.213.924+47,77%'],
+  ['gr', '56,81', '+18,13+31,91%', '821.970', '+392.687+47,77%'],
   ['5 Tahun', 'Kurs', '', '', '14.215', '+1.993+14,02%'],
-  ['oz', '1.283,64', '+1.054,30+82,13%', '18.246.943', '+19.646.389+107,67%'],
-  ['gr', '41,27', '+33,90+82,13%', '586.653', '+631.646+107,67%']])
+  ['oz', '1.280,61', '+1.050,34+82,02%', '18.203.871', '+19.576.166+107,54%'],
+  ['gr', '41,17', '+33,77+82,02%', '585.268', '+629.388+107,54%']])
 (['Home', 'Emas 1 Gram', 'History', 'Trend', 'Perak 1 Gram', 'Pluang'],
  [[''],
   ['Emas 24 KaratHarga Emas 1 Gram', ''],
-  ['USD', '75,17↓', '%'],
-  ['KURS', '16.241,30↓', '%'],
-  ['IDR', '1.220.801,94↓', '%'],
-  ['Minggu, 28 April 2024 20:23']],
+  ['USD', '74,92↓', '-0,25-0,33%'],
+  ['KURS', '16.234,15↓', '-7,15-0,04%'],
+  ['IDR', '1.216.308,20↓', '-4.493,74-0,37%'],
+  ['Senin, 29 April 2024 09:05']],
  [[''],
   ['Emas 1 Gram (IDR)Emas 1 Gram (USD)Kurs USD-IDR',
    'Hari Ini',
    '1 Bulan',
    '1 Tahun',
    '5 Tahun',
    'Max',
    '']],
  [['Pergerakkan Harga Emas 1 Gram'],
   ['', 'Penutupan Kemarin', 'Pergerakkan Hari Ini', 'Rata-rata'],
-  ['USD', '75,17', '75,17 - 75,17', '75,17'],
-  ['KURS', '16.241,30', '16.241,30 - 16.241,30', '16.241,30'],
-  ['IDR', '1.220.801,94', '1.220.801,94 - 1.220.801,94', '1.220.801,94'],
+  ['USD', '75,17', '74,92 - 75,17', '75,05'],
+  ['KURS', '16.241,30', '16.234,15 - 16.241,30', '16.237,73'],
+  ['IDR', '1.220.801,94', '1.216.308,20 - 1.220.801,94', '1.218.555,07'],
   [''],
   ['', 'Awal Tahun', 'Pergerakkan YTD', '+/- YTD'],
-  ['USD', '66,32', '64,07 - 77,14', '+8,85 (13,34%)'],
-  ['KURS', '15.390,10', '15.390,00 - 16.307,80', '+851,20 (5,53%)'],
-  ['IDR', '1.020.729,53', '997.660,12 - 1.256.829,06', '+200.072,41 (19,60%)'],
+  ['USD', '66,32', '64,07 - 77,14', '+8,60 (12,97%)'],
+  ['KURS', '15.390,10', '15.390,00 - 16.307,80', '+844,05 (5,48%)'],
+  ['IDR', '1.020.729,53', '997.660,12 - 1.256.829,06', '+195.578,67 (19,16%)'],
   [''],
   ['', 'Tahun Lalu / 52 Minggu', 'Pergerakkan 52 Minggu', '+/- 52 Minggu'],
-  ['USD', '63,78', '58,43 - 77,14', '+11,39 (17,86%)'],
-  ['KURS', '14.708,55', '14.669,40 - 16.307,80', '+1.532,75 (10,42%)'],
-  ['IDR', '938.054,69', '912.925,68 - 1.256.829,06', '+282.747,25 (30,14%)']])
+  ['USD', '64,04', '58,43 - 77,14', '+10,88 (16,99%)'],
+  ['KURS', '14.671,35', '14.669,40 - 16.307,80', '+1.562,80 (10,65%)'],
+  ['IDR', '939.568,98', '912.925,68 - 1.256.829,06', '+276.739,22 (29,45%)']])
 ```
 
 ## iopen
 
 `iopen(path, data=None, regex=None, css_select=None, xpath=None, file_append=False)`
 
 Membaca atau Tulis pada path yang bisa merupakan FILE maupun URL.  
@@ -1503,15 +1410,16 @@
 print(iopen("https://www.google.com/", dict(coba="dulu"), xpath="//a"))  
 ```
 
 Output:
 ```py
 8
 ['mana', 'aja']
-[<Element a at 0x776a6a7d90>, <Element a at 0x776a6f2990>, <Element a at 0x776a6f2a30>, <Element a at 0x776a6f2a80>, <Element a at 0x776a6f2ad0>, <Element a at 0x776a6f2b20>, <Element a at 0x776a6f2b70>, <Element a at 0x776a6f2bc0>, <Element a at 0x776a6f2c10>, <Element a at 0x776a6f2c60>, <Element a at 0x776a6f2cb0>, <Element a at 0x776a6f2d00>, <Element a at 0x776a6f2d50>, <Element a at 0x776a6f2da0>, <Element a at 0x776a6f2df0>, <Element a at 0x776a6f2e40>, <Element a at 0x776a6f2e90>, <Element a at 0x776a6f2ee0>]
+Timeout 3
+[<Element a at 0x77ab267200>, <Element a at 0x77ab2b2800>, <Element a at 0x77ab2b28a0>, <Element a at 0x77ab2b28f0>, <Element a at 0x77ab2b2940>, <Element a at 0x77ab2b2990>, <Element a at 0x77ab2b29e0>, <Element a at 0x77ab2b2a30>, <Element a at 0x77ab2b2a80>, <Element a at 0x77ab2b2ad0>, <Element a at 0x77ab2b2b20>, <Element a at 0x77ab2b2b70>, <Element a at 0x77ab2b2bc0>, <Element a at 0x77ab2b2c10>, <Element a at 0x77ab2b2c60>, <Element a at 0x77ab2b2cb0>, <Element a at 0x77ab2b2d00>, <Element a at 0x77ab2b2d50>, <Element a at 0x77ab2b2da0>, <Element a at 0x77ab2b2df0>]
 False
 ```
 
 ## iprint
 
 `iprint(*args, color=None, sort_dicts=False, **kwargs)`
 
@@ -1544,16 +1452,16 @@
 print(list(irange('a', 'z', 10)))  
 print(list(irange(1, '7')))  
 print(list(irange(10, 5)))  
 ```
 
 Output:
 ```py
-<generator object irange at 0x776a67abd0>
-<generator object irange at 0x776a67abd0>
+<generator object irange at 0x77ab23aac0>
+<generator object irange at 0x77ab23aac0>
 ['a', 'k', 'u']
 [1, 2, 3, 4, 5, 6, 7]
 [10, 9, 8, 7, 6, 5]
 ```
 
 ## ireplace
 
@@ -1588,15 +1496,15 @@
 ```python  
 print(iscandir())  
 print(list(iscandir("./", recursive=False, scan_file=False)))  
 ```
 
 Output:
 ```py
-<generator object iscandir at 0x776a6b4740>
+<generator object iscandir at 0x77ab274740>
 [PosixPath('.git'), PosixPath('.vscode'), PosixPath('pypipr'), PosixPath('__pycache__'), PosixPath('dist')]
 ```
 
 ## isplit
 
 `isplit(text, separator='', include_separator=False)`
 
@@ -1608,14 +1516,133 @@
 ```
 
 Output:
 ```py
 ['', 'ini', 'contoh', 'path', '']
 ```
 
+## ivars
+
+`ivars(obj, skip_underscore=True)`
+
+Membuat dictionary berdasarkan kategori untuk setiap  
+member dari object.  
+  
+```python  
+iprint(ivars(__import__('pypipr')))  
+```
+
+Output:
+```py
+{'module': {'ibuiltins': <module 'pypipr.ibuiltins' from '/data/data/com.termux/files/home/pypipr/pypipr/ibuiltins/__init__.py'>,
+            'iconsole': <module 'pypipr.iconsole' from '/data/data/com.termux/files/home/pypipr/pypipr/iconsole/__init__.py'>,
+            'idjango': <module 'pypipr.idjango' from '/data/data/com.termux/files/home/pypipr/pypipr/idjango/__init__.py'>,
+            'iengineering': <module 'pypipr.iengineering' from '/data/data/com.termux/files/home/pypipr/pypipr/iengineering/__init__.py'>,
+            'ifunctions': <module 'pypipr.ifunctions' from '/data/data/com.termux/files/home/pypipr/pypipr/ifunctions/__init__.py'>,
+            'iflow': <module 'pypipr.iflow' (<_frozen_importlib_external.NamespaceLoader object at 0x77b33bf290>)>,
+            'asyncio': <module 'asyncio' from '/data/data/com.termux/files/usr/lib/python3.11/asyncio/__init__.py'>,
+            'colorama': <module 'colorama' from '/data/data/com.termux/files/usr/lib/python3.11/site-packages/colorama/__init__.py'>,
+            'csv': <module 'csv' from '/data/data/com.termux/files/usr/lib/python3.11/csv.py'>,
+            'datetime': <module 'datetime' from '/data/data/com.termux/files/usr/lib/python3.11/datetime.py'>,
+            'functools': <module 'functools' from '/data/data/com.termux/files/usr/lib/python3.11/functools.py'>,
+            'inspect': <module 'inspect' from '/data/data/com.termux/files/usr/lib/python3.11/inspect.py'>,
+            'io': <module 'io' (frozen)>,
+            'json': <module 'json' from '/data/data/com.termux/files/usr/lib/python3.11/json/__init__.py'>,
+            'lxml': <module 'lxml' from '/data/data/com.termux/files/usr/lib/python3.11/site-packages/lxml/__init__.py'>,
+            'math': <module 'math' from '/data/data/com.termux/files/usr/lib/python3.11/lib-dynload/math.cpython-311.so'>,
+            'multiprocessing': <module 'multiprocessing' from '/data/data/com.termux/files/usr/lib/python3.11/multiprocessing/__init__.py'>,
+            'operator': <module 'operator' from '/data/data/com.termux/files/usr/lib/python3.11/operator.py'>,
+            'os': <module 'os' (frozen)>,
+            'pathlib': <module 'pathlib' from '/data/data/com.termux/files/usr/lib/python3.11/pathlib.py'>,
+            'pint': <module 'pint' from '/data/data/com.termux/files/usr/lib/python3.11/site-packages/pint/__init__.py'>,
+            'pprint': <module 'pprint' from '/data/data/com.termux/files/usr/lib/python3.11/pprint.py'>,
+            'queue': <module 'queue' from '/data/data/com.termux/files/usr/lib/python3.11/queue.py'>,
+            'random': <module 'random' from '/data/data/com.termux/files/usr/lib/python3.11/random.py'>,
+            're': <module 're' from '/data/data/com.termux/files/usr/lib/python3.11/re/__init__.py'>,
+            'requests': <module 'requests' from '/data/data/com.termux/files/usr/lib/python3.11/site-packages/requests/__init__.py'>,
+            'string': <module 'string' from '/data/data/com.termux/files/usr/lib/python3.11/string.py'>,
+            'subprocess': <module 'subprocess' from '/data/data/com.termux/files/usr/lib/python3.11/subprocess.py'>,
+            'sys': <module 'sys' (built-in)>,
+            'textwrap': <module 'textwrap' from '/data/data/com.termux/files/usr/lib/python3.11/textwrap.py'>,
+            'threading': <module 'threading' from '/data/data/com.termux/files/usr/lib/python3.11/threading.py'>,
+            'time': <module 'time' (built-in)>,
+            'tzdata': <module 'tzdata' from '/data/data/com.termux/files/usr/lib/python3.11/site-packages/tzdata/__init__.py'>,
+            'uuid': <module 'uuid' from '/data/data/com.termux/files/usr/lib/python3.11/uuid.py'>,
+            'webbrowser': <module 'webbrowser' from '/data/data/com.termux/files/usr/lib/python3.11/webbrowser.py'>,
+            'yaml': <module 'yaml' from '/data/data/com.termux/files/usr/lib/python3.11/site-packages/yaml/__init__.py'>,
+            'zoneinfo': <module 'zoneinfo' from '/data/data/com.termux/files/usr/lib/python3.11/zoneinfo/__init__.py'>},
+ 'class': {'ComparePerformance': <class 'pypipr.ibuiltins.ComparePerformance.ComparePerformance'>,
+           'RunParallel': <class 'pypipr.ibuiltins.RunParallel.RunParallel'>,
+           'APIMixinView': <class 'pypipr.idjango.APIMixinView.APIMixinView'>,
+           'PintUregQuantity': <class 'pint.Quantity'>},
+ 'variable': {'LINUX': True,
+              'WINDOWS': False,
+              'PintUreg': <pint.registry.UnitRegistry object at 0x77b794b750>},
+ 'function': {'avg': <function avg at 0x77c3b2ed40>,
+              'basename': <function basename at 0x77c3afe8e0>,
+              'chr_to_int': <function chr_to_int at 0x77c0961080>,
+              'chunk_array': <function chunk_array at 0x77c09611c0>,
+              'create_folder': <function create_folder at 0x77c09613a0>,
+              'datetime_from_string': <function datetime_from_string at 0x77c0961580>,
+              'datetime_now': <function datetime_now at 0x77c0a09620>,
+              'dict_first': <function dict_first at 0x77c0a09580>,
+              'dirname': <function dirname at 0x77c0a094e0>,
+              'exit_if_empty': <function exit_if_empty at 0x77c0a093a0>,
+              'filter_empty': <function filter_empty at 0x77c0a091c0>,
+              'get_by_index': <function get_by_index at 0x77c0a08e00>,
+              'get_class_method': <function get_class_method at 0x77c0a08cc0>,
+              'get_filemtime': <function get_filemtime at 0x77c0a08b80>,
+              'get_filesize': <function get_filesize at 0x77c0a089a0>,
+              'int_to_chr': <function int_to_chr at 0x77c0a08900>,
+              'is_empty': <function is_empty at 0x77c0a09260>,
+              'is_iterable': <function is_iterable at 0x77c0a08fe0>,
+              'is_valid_url': <function is_valid_url at 0x77c0a087c0>,
+              'password_generator': <function password_generator at 0x77c0a08680>,
+              'random_bool': <function random_bool at 0x77c0a084a0>,
+              'restart': <function restart at 0x77c0a0b7e0>,
+              'set_timeout': <function set_timeout at 0x77c0a0b920>,
+              'sets_ordered': <function sets_ordered at 0x77c0a0ba60>,
+              'str_cmp': <function str_cmp at 0x77c0a0bb00>,
+              'to_str': <function to_str at 0x77c0a08f40>,
+              'choices': <function choices at 0x77c0a0bba0>,
+              'console_run': <function console_run at 0x77c0a0be20>,
+              'input_char': <function input_char at 0x77c0a0bf60>,
+              'log': <function log at 0x77c0a2c180>,
+              'print_colorize': <function print_colorize at 0x77c0a2c220>,
+              'print_dir': <function print_dir at 0x77c0a2c360>,
+              'print_log': <function print_log at 0x77c0a2c040>,
+              'print_to_last_line': <function print_to_last_line at 0x77c0a0bd80>,
+              'text_colorize': <function text_colorize at 0x77c0a0bec0>,
+              'batch_calculate': <function batch_calculate at 0x77b33d96c0>,
+              'batchmaker': <function batchmaker at 0x77b33da160>,
+              'calculate': <function calculate at 0x77b33da3e0>,
+              'auto_reload': <function auto_reload at 0x77b33da660>,
+              'github_pull': <function github_pull at 0x77b33da5c0>,
+              'github_push': <function github_push at 0x77b33da840>,
+              'github_user': <function github_user at 0x77b33dab60>,
+              'pip_freeze_without_version': <function pip_freeze_without_version at 0x77b31020c0>,
+              'poetry_publish': <function poetry_publish at 0x77b31022a0>,
+              'poetry_update_version': <function poetry_update_version at 0x77b3126ac0>,
+              'iargv': <function iargv at 0x77ab484220>,
+              'idumps': <function idumps at 0x77ab484360>,
+              'idumps_html': <function idumps_html at 0x77ab4ecd60>,
+              'ienv': <function ienv at 0x77ab4844a0>,
+              'iexec': <function iexec at 0x77ab4ecfe0>,
+              'ijoin': <function ijoin at 0x77b3102020>,
+              'iloads': <function iloads at 0x77ab4ed080>,
+              'iloads_html': <function iloads_html at 0x77ab4ed300>,
+              'iopen': <function iopen at 0x77b3102340>,
+              'iprint': <function iprint at 0x77ab4ed1c0>,
+              'irange': <function irange at 0x77b33da520>,
+              'ireplace': <function ireplace at 0x77ab4ed3a0>,
+              'iscandir': <function iscandir at 0x77ab4eefc0>,
+              'isplit': <function isplit at 0x77ab4ef060>,
+              'ivars': <function ivars at 0x77ab4ef100>}}
+```
+
 # CLASS
 
 ## ComparePerformance
 
 `ComparePerformance()`
 
 Menjalankan seluruh method dalam class,  
@@ -1645,15 +1672,15 @@
 print(ExampleComparePerformance().compare_performance())  
 print(ExampleComparePerformance().compare_performance())  
 print(ExampleComparePerformance().compare_performance())  
 ```
 
 Output:
 ```py
-{'a': <generator object ExampleComparePerformance.a.<locals>.<genexpr> at 0x776a6c45f0>,
+{'a': <generator object ExampleComparePerformance.a.<locals>.<genexpr> at 0x77ab284450>,
  'b': (0, 1, 2, 3, 4, 5, 6, 7, 8, 9),
  'c': [0, 1, 2, 3, 4, 5, 6, 7, 8, 9],
  'd': [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]}
 {'a': 0, 'b': 0, 'c': 0, 'd': 0}
 {'a': 0, 'b': 0, 'c': 0, 'd': 0}
 {'a': 0, 'b': 0, 'c': 0, 'd': 0}
 {'a': 0, 'b': 0, 'c': 0, 'd': 0}
@@ -1777,8 +1804,7 @@
 class ExampleAPIView(APIMixinView, View):  
     pass  
 ```
 
 ## PintUregQuantity
 
 `PintUregQuantity(value, units=None)`
-
```

