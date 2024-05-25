# Comparing `tmp/afeng-py-tools-0.0.98.tar.gz` & `tmp/afeng-py-tools-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "afeng-py-tools-0.0.98.tar", last modified: Mon Feb  5 16:10:10 2024, max compression
+gzip compressed data, was "afeng-py-tools-0.0.99.tar", last modified: Mon Feb  5 18:37:32 2024, max compression
```

## Comparing `afeng-py-tools-0.0.98.tar` & `afeng-py-tools-0.0.99.tar`

### file list

```diff
@@ -1,468 +1,472 @@
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:10.196810 afeng-py-tools-0.0.98/
--rw-rw-rw-   0        0        0     2182 2023-12-06 19:02:40.000000 afeng-py-tools-0.0.98/.gitignore
--rw-rw-rw-   0        0        0     9719 2023-12-06 05:03:07.000000 afeng-py-tools-0.0.98/LICENSE
--rw-rw-rw-   0        0        0    12634 2024-02-05 16:10:10.194625 afeng-py-tools-0.0.98/PKG-INFO
--rw-rw-rw-   0        0        0     1003 2023-12-06 18:55:31.000000 afeng-py-tools-0.0.98/README.md
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:09.467435 afeng-py-tools-0.0.98/doc/
--rw-rw-rw-   0        0        0     1062 2024-02-03 00:40:19.000000 afeng-py-tools-0.0.98/doc/项目打包流程.md
--rw-rw-rw-   0        0        0     1229 2023-12-07 08:22:37.000000 afeng-py-tools-0.0.98/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-02-05 16:10:10.196810 afeng-py-tools-0.0.98/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:09.468562 afeng-py-tools-0.0.98/src/
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:10.192394 afeng-py-tools-0.0.98/src/afeng_py_tools.egg-info/
--rw-rw-rw-   0        0        0    12634 2024-02-05 16:10:08.000000 afeng-py-tools-0.0.98/src/afeng_py_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    18109 2024-02-05 16:10:09.000000 afeng-py-tools-0.0.98/src/afeng_py_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-05 16:10:08.000000 afeng-py-tools-0.0.98/src/afeng_py_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2024-02-05 16:10:08.000000 afeng-py-tools-0.0.98/src/afeng_py_tools.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:09.482093 afeng-py-tools-0.0.98/src/afeng_tools/
--rw-rw-rw-   0        0        0       88 2023-12-06 18:41:42.000000 afeng-py-tools-0.0.98/src/afeng_tools/__init__.py
--rw-rw-rw-   0        0        0      483 2024-02-05 16:10:07.000000 afeng-py-tools-0.0.98/src/afeng_tools/__version__.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:09.490972 afeng-py-tools-0.0.98/src/afeng_tools/aliyun_pan_tool/
--rw-rw-rw-   0        0        0      155 2023-10-07 09:49:34.000000 afeng-py-tools-0.0.98/src/afeng_tools/aliyun_pan_tool/__init__.py
--rw-rw-rw-   0        0        0     8377 2023-12-27 21:54:39.000000 afeng-py-tools-0.0.98/src/afeng_tools/aliyun_pan_tool/aliyun_pan_share_tools.py
--rw-rw-rw-   0        0        0     1695 2023-12-27 21:54:39.000000 afeng-py-tools-0.0.98/src/afeng_tools/aliyun_pan_tool/aliyun_pan_sign_in_tools.py
--rw-rw-rw-   0        0        0    11650 2023-12-27 21:54:33.000000 afeng-py-tools-0.0.98/src/afeng_tools/aliyun_pan_tool/aliyun_pan_tools.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:09.495297 afeng-py-tools-0.0.98/src/afeng_tools/aliyun_pan_tool/demo/
--rw-rw-rw-   0        0        0        0 2023-10-07 08:20:48.000000 afeng-py-tools-0.0.98/src/afeng_tools/aliyun_pan_tool/demo/__init__.py
--rw-rw-rw-   0        0        0     2399 2023-12-11 07:11:01.000000 afeng-py-tools-0.0.98/src/afeng_tools/aliyun_pan_tool/demo/run_demo.py
--rw-rw-rw-   0        0        0      729 2023-12-11 07:11:01.000000 afeng-py-tools-0.0.98/src/afeng_tools/aliyun_pan_tool/demo/share_demo.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:09.511669 afeng-py-tools-0.0.98/src/afeng_tools/appium_tool/
--rw-rw-rw-   0        0        0      107 2023-09-28 15:44:05.000000 afeng-py-tools-0.0.98/src/afeng_tools/appium_tool/__init__.py
--rw-rw-rw-   0        0        0     5604 2023-12-07 06:09:44.000000 afeng-py-tools-0.0.98/src/afeng_tools/appium_tool/appium_client_tool.py
--rw-rw-rw-   0        0        0      855 2023-12-07 06:09:44.000000 afeng-py-tools-0.0.98/src/afeng_tools/appium_tool/appium_options_tools.py
--rw-rw-rw-   0        0        0     1953 2023-09-28 17:54:35.000000 afeng-py-tools-0.0.98/src/afeng_tools/appium_tool/appium_touch_tools.py
--rw-rw-rw-   0        0        0     3439 2023-12-07 06:09:44.000000 afeng-py-tools-0.0.98/src/afeng_tools/appium_tool/mobile_adb_tools.py
--rw-rw-rw-   0        0        0     2446 2023-12-07 06:09:44.000000 afeng-py-tools-0.0.98/src/afeng_tools/appium_tool/mobile_app_tools.py
--rw-rw-rw-   0        0        0     2435 2023-08-07 07:52:58.000000 afeng-py-tools-0.0.98/src/afeng_tools/appium_tool/mobile_keycode.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:09.521607 afeng-py-tools-0.0.98/src/afeng_tools/application_tool/
--rw-rw-rw-   0        0        0      275 2023-10-15 16:38:39.000000 afeng-py-tools-0.0.98/src/afeng_tools/application_tool/README.md
--rw-rw-rw-   0        0        0        0 2023-10-15 12:57:28.000000 afeng-py-tools-0.0.98/src/afeng_tools/application_tool/__init__.py
--rw-rw-rw-   0        0        0     2940 2024-02-03 18:47:56.000000 afeng-py-tools-0.0.98/src/afeng_tools/application_tool/application_models.py
--rw-rw-rw-   0        0        0     2500 2023-12-07 06:29:26.000000 afeng-py-tools-0.0.98/src/afeng_tools/application_tool/application_tools.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:09.524880 afeng-py-tools-0.0.98/src/afeng_tools/application_tool/demo/
--rw-rw-rw-   0        0        0        0 2023-10-16 05:26:55.000000 afeng-py-tools-0.0.98/src/afeng_tools/application_tool/demo/__init__.py
--rw-rw-rw-   0        0        0      799 2023-12-07 06:29:26.000000 afeng-py-tools-0.0.98/src/afeng_tools/application_tool/demo/settings.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:09.532652 afeng-py-tools-0.0.98/src/afeng_tools/application_tool/demo/yaml_demo/
--rw-rw-rw-   0        0        0       28 2023-10-15 17:40:37.000000 afeng-py-tools-0.0.98/src/afeng_tools/application_tool/demo/yaml_demo/application-dev.yml
--rw-rw-rw-   0        0        0       26 2023-10-15 15:54:14.000000 afeng-py-tools-0.0.98/src/afeng_tools/application_tool/demo/yaml_demo/application-prod.yml
--rw-rw-rw-   0        0        0       26 2023-10-15 15:53:55.000000 afeng-py-tools-0.0.98/src/afeng_tools/application_tool/demo/yaml_demo/application-test.yml
--rw-rw-rw-   0        0        0      811 2023-10-25 00:23:53.000000 afeng-py-tools-0.0.98/src/afeng_tools/application_tool/demo/yaml_demo/application.yml
--rw-rw-rw-   0        0        0     4717 2024-02-03 16:18:03.000000 afeng-py-tools-0.0.98/src/afeng_tools/application_tool/settings_enum.py
--rw-rw-rw-   0        0        0     6103 2023-12-24 16:13:37.000000 afeng-py-tools-0.0.98/src/afeng_tools/application_tool/settings_tools.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:09.542456 afeng-py-tools-0.0.98/src/afeng_tools/baidu_pan_tool/
--rw-rw-rw-   0        0        0      202 2023-10-01 05:20:31.000000 afeng-py-tools-0.0.98/src/afeng_tools/baidu_pan_tool/__init__.py
--rw-rw-rw-   0        0        0      376 2023-12-07 06:52:24.000000 afeng-py-tools-0.0.98/src/afeng_tools/baidu_pan_tool/baidu_pan_enum.py
--rw-rw-rw-   0        0        0     1560 2023-12-08 07:11:59.000000 afeng-py-tools-0.0.98/src/afeng_tools/baidu_pan_tool/baidu_pan_settings.py
--rw-rw-rw-   0        0        0     8278 2023-12-08 06:56:26.000000 afeng-py-tools-0.0.98/src/afeng_tools/baidu_pan_tool/baidu_pan_tools.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:09.550214 afeng-py-tools-0.0.98/src/afeng_tools/baidu_pan_tool/core/
--rw-rw-rw-   0        0        0        0 2023-10-01 03:30:27.000000 afeng-py-tools-0.0.98/src/afeng_tools/baidu_pan_tool/core/__init__.py
--rw-rw-rw-   0        0        0      664 2023-12-12 13:05:57.000000 afeng-py-tools-0.0.98/src/afeng_tools/baidu_pan_tool/core/baidu_pan_api_tools.py
--rw-rw-rw-   0        0        0     3285 2023-12-07 07:10:09.000000 afeng-py-tools-0.0.98/src/afeng_tools/baidu_pan_tool/core/baidu_pan_decorator_tools.py
--rw-rw-rw-   0        0        0    26274 2023-12-07 07:10:20.000000 afeng-py-tools-0.0.98/src/afeng_tools/baidu_pan_tool/core/baidu_pan_models.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:09.554537 afeng-py-tools-0.0.98/src/afeng_tools/baidu_pan_tool/demo/
--rw-rw-rw-   0        0        0        0 2023-10-01 04:22:46.000000 afeng-py-tools-0.0.98/src/afeng_tools/baidu_pan_tool/demo/__init__.py
--rw-rw-rw-   0        0        0     5019 2023-12-07 23:18:53.000000 afeng-py-tools-0.0.98/src/afeng_tools/baidu_pan_tool/demo/baidupan_demo.py
--rw-rw-rw-   0        0        0      995 2023-10-07 11:42:27.000000 afeng-py-tools-0.0.98/src/afeng_tools/baidu_pan_tool/demo/share_msg.txt
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:09.581255 afeng-py-tools-0.0.98/src/afeng_tools/baidu_pan_tool/tools/
--rw-rw-rw-   0        0        0       28 2023-10-02 06:37:06.000000 afeng-py-tools-0.0.98/src/afeng_tools/baidu_pan_tool/tools/__init__.py
--rw-rw-rw-   0        0        0     5118 2023-12-07 06:59:50.000000 afeng-py-tools-0.0.98/src/afeng_tools/baidu_pan_tool/tools/audio_file_tools.py
--rw-rw-rw-   0        0        0     9031 2023-12-07 07:03:37.000000 afeng-py-tools-0.0.98/src/afeng_tools/baidu_pan_tool/tools/auth_tools.py
--rw-rw-rw-   0        0        0     7215 2023-12-08 06:55:39.000000 afeng-py-tools-0.0.98/src/afeng_tools/baidu_pan_tool/tools/auth_web_tools.py
--rw-rw-rw-   0        0        0     6502 2023-12-07 07:04:33.000000 afeng-py-tools-0.0.98/src/afeng_tools/baidu_pan_tool/tools/file_download_tools.py
--rw-rw-rw-   0        0        0    12885 2023-12-07 07:04:33.000000 afeng-py-tools-0.0.98/src/afeng_tools/baidu_pan_tool/tools/file_manager_tools.py
--rw-rw-rw-   0        0        0     4155 2023-12-07 07:09:42.000000 afeng-py-tools-0.0.98/src/afeng_tools/baidu_pan_tool/tools/file_meta_tools.py
--rw-rw-rw-   0        0        0    22055 2024-01-26 17:28:32.000000 afeng-py-tools-0.0.98/src/afeng_tools/baidu_pan_tool/tools/file_path_tools.py
--rw-rw-rw-   0        0        0    14999 2023-12-07 07:09:42.000000 afeng-py-tools-0.0.98/src/afeng_tools/baidu_pan_tool/tools/file_upload_tools.py
--rw-rw-rw-   0        0        0       44 2023-10-04 15:36:53.000000 afeng-py-tools-0.0.98/src/afeng_tools/baidu_pan_tool/tools/image_file_tools.py
--rw-rw-rw-   0        0        0     9863 2023-12-07 07:09:42.000000 afeng-py-tools-0.0.98/src/afeng_tools/baidu_pan_tool/tools/share_tools.py
--rw-rw-rw-   0        0        0     2594 2023-12-07 07:09:42.000000 afeng-py-tools-0.0.98/src/afeng_tools/baidu_pan_tool/tools/user_tools.py
--rw-rw-rw-   0        0        0     3869 2023-12-07 07:09:42.000000 afeng-py-tools-0.0.98/src/afeng_tools/baidu_pan_tool/tools/video_file_tools.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:09.587775 afeng-py-tools-0.0.98/src/afeng_tools/cache_tool/
--rw-rw-rw-   0        0        0       22 2023-12-11 01:20:06.000000 afeng-py-tools-0.0.98/src/afeng_tools/cache_tool/__init__.py
--rw-rw-rw-   0        0        0     1539 2023-12-11 12:02:47.000000 afeng-py-tools-0.0.98/src/afeng_tools/cache_tool/cache_decorator.py
--rw-rw-rw-   0        0        0     1271 2024-02-04 14:09:59.000000 afeng-py-tools-0.0.98/src/afeng_tools/cache_tool/cache_memory_tools.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:09.591013 afeng-py-tools-0.0.98/src/afeng_tools/compression_tool/
--rw-rw-rw-   0        0        0       34 2023-12-06 21:29:52.000000 afeng-py-tools-0.0.98/src/afeng_tools/compression_tool/__init__.py
--rw-rw-rw-   0        0        0     3177 2023-12-11 07:06:12.000000 afeng-py-tools-0.0.98/src/afeng_tools/compression_tool/zip_tools.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:09.596343 afeng-py-tools-0.0.98/src/afeng_tools/convert_tool/
--rw-rw-rw-   0        0        0       22 2023-12-06 21:26:54.000000 afeng-py-tools-0.0.98/src/afeng_tools/convert_tool/__init__.py
--rw-rw-rw-   0        0        0     2511 2023-12-11 14:44:37.000000 afeng-py-tools-0.0.98/src/afeng_tools/convert_tool/type_convert_tools.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:09.601895 afeng-py-tools-0.0.98/src/afeng_tools/crawler_tool/
--rw-rw-rw-   0        0        0       22 2023-12-06 21:28:37.000000 afeng-py-tools-0.0.98/src/afeng_tools/crawler_tool/__init__.py
--rw-rw-rw-   0        0        0     3723 2023-10-06 15:31:26.000000 afeng-py-tools-0.0.98/src/afeng_tools/crawler_tool/pyquery_tools.py
--rw-rw-rw-   0        0        0      423 2023-12-06 21:28:37.000000 afeng-py-tools-0.0.98/src/afeng_tools/crawler_tool/xpath_tools.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:09.607399 afeng-py-tools-0.0.98/src/afeng_tools/datetime_tool/
--rw-rw-rw-   0        0        0       28 2023-12-06 19:25:21.000000 afeng-py-tools-0.0.98/src/afeng_tools/datetime_tool/__init__.py
--rw-rw-rw-   0        0        0     1080 2023-12-11 14:38:46.000000 afeng-py-tools-0.0.98/src/afeng_tools/datetime_tool/datetime_tools.py
--rw-rw-rw-   0        0        0      618 2023-12-07 06:10:33.000000 afeng-py-tools-0.0.98/src/afeng_tools/datetime_tool/time_monitor_tools.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:09.613010 afeng-py-tools-0.0.98/src/afeng_tools/decorator_tool/
--rw-rw-rw-   0        0        0       25 2023-12-06 19:25:14.000000 afeng-py-tools-0.0.98/src/afeng_tools/decorator_tool/__init__.py
--rw-rw-rw-   0        0        0     1572 2023-12-06 19:25:10.000000 afeng-py-tools-0.0.98/src/afeng_tools/decorator_tool/decorator_tools.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:09.615227 afeng-py-tools-0.0.98/src/afeng_tools/east_money_tool/
--rw-rw-rw-   0        0        0      100 2023-12-07 06:24:05.000000 afeng-py-tools-0.0.98/src/afeng_tools/east_money_tool/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:09.617390 afeng-py-tools-0.0.98/src/afeng_tools/east_money_tool/config/
--rw-rw-rw-   0        0        0        0 2023-09-08 02:58:20.000000 afeng-py-tools-0.0.98/src/afeng_tools/east_money_tool/config/__init__.py
--rw-rw-rw-   0        0        0     9569 2023-09-11 15:12:14.000000 afeng-py-tools-0.0.98/src/afeng_tools/east_money_tool/config/web_url_config.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:09.630799 afeng-py-tools-0.0.98/src/afeng_tools/east_money_tool/quote_info/
--rw-rw-rw-   0        0        0        0 2023-09-11 03:24:53.000000 afeng-py-tools-0.0.98/src/afeng_tools/east_money_tool/quote_info/__init__.py
--rw-rw-rw-   0        0        0      841 2023-12-07 06:23:04.000000 afeng-py-tools-0.0.98/src/afeng_tools/east_money_tool/quote_info/east_money_quote_data_tools.py
--rw-rw-rw-   0        0        0     3156 2023-12-07 06:24:05.000000 afeng-py-tools-0.0.98/src/afeng_tools/east_money_tool/quote_info/quote_field_enum.py
--rw-rw-rw-   0        0        0    77497 2023-12-07 06:24:05.000000 afeng-py-tools-0.0.98/src/afeng_tools/east_money_tool/quote_info/quote_info_config.py
--rw-rw-rw-   0        0        0     2087 2023-12-07 06:24:05.000000 afeng-py-tools-0.0.98/src/afeng_tools/east_money_tool/quote_info/quote_item_tools.py
--rw-rw-rw-   0        0        0     3813 2023-09-14 03:37:24.000000 afeng-py-tools-0.0.98/src/afeng_tools/east_money_tool/quote_info/quote_models.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:09.636321 afeng-py-tools-0.0.98/src/afeng_tools/east_money_tool/stock_comment/
--rw-rw-rw-   0        0        0      108 2023-09-08 18:14:30.000000 afeng-py-tools-0.0.98/src/afeng_tools/east_money_tool/stock_comment/__init__.py
--rw-rw-rw-   0        0        0      737 2023-12-07 06:23:04.000000 afeng-py-tools-0.0.98/src/afeng_tools/east_money_tool/stock_comment/east_money_zhpj_tools.py
--rw-rw-rw-   0        0        0     1388 2023-12-07 06:23:04.000000 afeng-py-tools-0.0.98/src/afeng_tools/east_money_tool/stock_comment/east_money_zlkp_tools.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:09.644046 afeng-py-tools-0.0.98/src/afeng_tools/east_money_tool/tool/
--rw-rw-rw-   0        0        0       31 2023-09-08 18:12:36.000000 afeng-py-tools-0.0.98/src/afeng_tools/east_money_tool/tool/__init__.py
--rw-rw-rw-   0        0        0     3359 2023-12-07 06:23:04.000000 afeng-py-tools-0.0.98/src/afeng_tools/east_money_tool/tool/east_money_http_tools.py
--rw-rw-rw-   0        0        0      708 2023-12-07 06:23:04.000000 afeng-py-tools-0.0.98/src/afeng_tools/east_money_tool/tool/east_money_load_auth_tools.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:09.648396 afeng-py-tools-0.0.98/src/afeng_tools/email_tool/
--rw-rw-rw-   0        0        0        0 2023-11-22 02:35:24.000000 afeng-py-tools-0.0.98/src/afeng_tools/email_tool/__init__.py
--rw-rw-rw-   0        0        0     5330 2023-12-07 06:11:25.000000 afeng-py-tools-0.0.98/src/afeng_tools/email_tool/email_send_tools.py
--rw-rw-rw-   0        0        0     1365 2023-11-22 14:36:51.000000 afeng-py-tools-0.0.98/src/afeng_tools/email_tool/email_tools.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:09.651693 afeng-py-tools-0.0.98/src/afeng_tools/encryption_tool/
--rw-rw-rw-   0        0        0       31 2023-12-06 21:33:22.000000 afeng-py-tools-0.0.98/src/afeng_tools/encryption_tool/__init__.py
--rw-rw-rw-   0        0        0     2202 2024-01-18 17:58:56.000000 afeng-py-tools-0.0.98/src/afeng_tools/encryption_tool/hashlib_tools.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:09.669525 afeng-py-tools-0.0.98/src/afeng_tools/fastapi_tool/
--rw-rw-rw-   0        0        0      167 2023-12-07 06:43:42.000000 afeng-py-tools-0.0.98/src/afeng_tools/fastapi_tool/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:09.679530 afeng-py-tools-0.0.98/src/afeng_tools/fastapi_tool/admin/
--rw-rw-rw-   0        0        0        0 2023-10-22 09:08:44.000000 afeng-py-tools-0.0.98/src/afeng_tools/fastapi_tool/admin/__init__.py
--rw-rw-rw-   0        0        0     1714 2023-12-25 06:21:33.000000 afeng-py-tools-0.0.98/src/afeng_tools/fastapi_tool/admin/admin_router_model.py
--rw-rw-rw-   0        0        0    12573 2023-12-26 11:04:12.000000 afeng-py-tools-0.0.98/src/afeng_tools/fastapi_tool/admin/admin_views_template.py
--rw-rw-rw-   0        0        0     7129 2023-12-25 06:54:10.000000 afeng-py-tools-0.0.98/src/afeng_tools/fastapi_tool/admin/admin_views_tools.py
--rw-rw-rw-   0        0        0      249 2023-11-25 18:56:00.000000 afeng-py-tools-0.0.98/src/afeng_tools/fastapi_tool/admin/auto_covert_func.template
--rw-rw-rw-   0        0        0     2396 2023-12-07 06:47:56.000000 afeng-py-tools-0.0.98/src/afeng_tools/fastapi_tool/admin/fastapi_api_doc_tools.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:09.687203 afeng-py-tools-0.0.98/src/afeng_tools/fastapi_tool/core/
--rw-rw-rw-   0        0        0        0 2023-12-08 14:20:15.000000 afeng-py-tools-0.0.98/src/afeng_tools/fastapi_tool/core/__init__.py
--rw-rw-rw-   0        0        0     4600 2024-01-28 21:17:24.000000 afeng-py-tools-0.0.98/src/afeng_tools/fastapi_tool/core/fastapi_app_tools.py
--rw-rw-rw-   0        0        0      409 2023-12-20 08:13:22.000000 afeng-py-tools-0.0.98/src/afeng_tools/fastapi_tool/core/fastapi_enums.py
--rw-rw-rw-   0        0        0      946 2023-12-20 08:50:05.000000 afeng-py-tools-0.0.98/src/afeng_tools/fastapi_tool/core/fastapi_items.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:09.692702 afeng-py-tools-0.0.98/src/afeng_tools/fastapi_tool/demo/
--rw-rw-rw-   0        0        0        0 2023-10-16 02:43:46.000000 afeng-py-tools-0.0.98/src/afeng_tools/fastapi_tool/demo/__init__.py
--rw-rw-rw-   0        0        0      408 2023-12-11 07:11:01.000000 afeng-py-tools-0.0.98/src/afeng_tools/fastapi_tool/demo/apps.py
--rw-rw-rw-   0        0        0      703 2023-12-11 07:11:01.000000 afeng-py-tools-0.0.98/src/afeng_tools/fastapi_tool/demo/main.py
--rw-rw-rw-   0        0        0     1349 2024-02-03 19:02:10.000000 afeng-py-tools-0.0.98/src/afeng_tools/fastapi_tool/fastapi_auto_tools.py
--rw-rw-rw-   0        0        0     1503 2023-12-12 05:25:20.000000 afeng-py-tools-0.0.98/src/afeng_tools/fastapi_tool/fastapi_depends_tools.py
--rw-rw-rw-   0        0        0     2024 2024-02-04 13:14:12.000000 afeng-py-tools-0.0.98/src/afeng_tools/fastapi_tool/fastapi_jinja2_tools.py
--rw-rw-rw-   0        0        0      635 2024-02-05 06:30:06.000000 afeng-py-tools-0.0.98/src/afeng_tools/fastapi_tool/fastapi_json_tools.py
--rw-rw-rw-   0        0        0     1294 2023-12-11 11:57:00.000000 afeng-py-tools-0.0.98/src/afeng_tools/fastapi_tool/fastapi_request_tools.py
--rw-rw-rw-   0        0        0     6742 2024-02-02 22:41:43.000000 afeng-py-tools-0.0.98/src/afeng_tools/fastapi_tool/fastapi_response_tools.py
--rw-rw-rw-   0        0        0     2532 2024-02-03 19:58:01.000000 afeng-py-tools-0.0.98/src/afeng_tools/fastapi_tool/fastapi_router_tools.py
--rw-rw-rw-   0        0        0     1209 2023-12-20 08:14:29.000000 afeng-py-tools-0.0.98/src/afeng_tools/fastapi_tool/fastapi_settings.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:09.704634 afeng-py-tools-0.0.98/src/afeng_tools/file_tool/
--rw-rw-rw-   0        0        0       22 2023-12-06 19:27:38.000000 afeng-py-tools-0.0.98/src/afeng_tools/file_tool/__init__.py
--rw-rw-rw-   0        0        0     1062 2023-12-06 21:32:01.000000 afeng-py-tools-0.0.98/src/afeng_tools/file_tool/csv_tools.py
--rw-rw-rw-   0        0        0    12308 2024-02-05 15:54:55.000000 afeng-py-tools-0.0.98/src/afeng_tools/file_tool/file_tools.py
--rw-rw-rw-   0        0        0     1488 2023-12-06 21:36:49.000000 afeng-py-tools-0.0.98/src/afeng_tools/file_tool/tmp_file_tools.py
--rw-rw-rw-   0        0        0      316 2023-10-15 15:07:50.000000 afeng-py-tools-0.0.98/src/afeng_tools/file_tool/yaml_tools.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:09.711095 afeng-py-tools-0.0.98/src/afeng_tools/flask_tool/
--rw-rw-rw-   0        0        0      407 2023-12-07 06:20:25.000000 afeng-py-tools-0.0.98/src/afeng_tools/flask_tool/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:09.716546 afeng-py-tools-0.0.98/src/afeng_tools/flask_tool/demo/
--rw-rw-rw-   0        0        0        0 2023-10-16 02:40:14.000000 afeng-py-tools-0.0.98/src/afeng_tools/flask_tool/demo/__init__.py
--rw-rw-rw-   0        0        0      276 2023-10-16 02:40:23.000000 afeng-py-tools-0.0.98/src/afeng_tools/flask_tool/demo/apps.py
--rw-rw-rw-   0        0        0      437 2023-10-16 02:36:06.000000 afeng-py-tools-0.0.98/src/afeng_tools/flask_tool/demo/urls.py
--rw-rw-rw-   0        0        0     1568 2023-12-07 06:19:17.000000 afeng-py-tools-0.0.98/src/afeng_tools/flask_tool/flask_app_tools.py
--rw-rw-rw-   0        0        0      201 2023-10-16 02:31:42.000000 afeng-py-tools-0.0.98/src/afeng_tools/flask_tool/flask_models.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:09.722551 afeng-py-tools-0.0.98/src/afeng_tools/generic_tool/
--rw-rw-rw-   0        0        0       22 2023-12-06 19:26:14.000000 afeng-py-tools-0.0.98/src/afeng_tools/generic_tool/__init__.py
--rw-rw-rw-   0        0        0      607 2023-12-06 19:26:49.000000 afeng-py-tools-0.0.98/src/afeng_tools/generic_tool/generic_tools.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:09.737775 afeng-py-tools-0.0.98/src/afeng_tools/http_tool/
--rw-rw-rw-   0        0        0        0 2023-09-08 02:46:02.000000 afeng-py-tools-0.0.98/src/afeng_tools/http_tool/__init__.py
--rw-rw-rw-   0        0        0      725 2023-12-07 06:04:30.000000 afeng-py-tools-0.0.98/src/afeng_tools/http_tool/aria2c_download_tools.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:09.742113 afeng-py-tools-0.0.98/src/afeng_tools/http_tool/decorator/
--rw-rw-rw-   0        0        0       23 2023-09-10 15:02:56.000000 afeng-py-tools-0.0.98/src/afeng_tools/http_tool/decorator/__init__.py
--rw-rw-rw-   0        0        0     1149 2023-12-07 06:04:30.000000 afeng-py-tools-0.0.98/src/afeng_tools/http_tool/decorator/http_auto_retry_tools.py
--rw-rw-rw-   0        0        0     6133 2023-12-08 07:20:45.000000 afeng-py-tools-0.0.98/src/afeng_tools/http_tool/http_download_tools.py
--rw-rw-rw-   0        0        0      505 2024-01-15 15:31:26.000000 afeng-py-tools-0.0.98/src/afeng_tools/http_tool/http_enums.py
--rw-rw-rw-   0        0        0      375 2023-10-20 07:28:35.000000 afeng-py-tools-0.0.98/src/afeng_tools/http_tool/http_html_tools.py
--rw-rw-rw-   0        0        0      259 2023-08-31 03:43:08.000000 afeng-py-tools-0.0.98/src/afeng_tools/http_tool/http_mimetype_tools.py
--rw-rw-rw-   0        0        0      327 2023-10-02 04:43:59.000000 afeng-py-tools-0.0.98/src/afeng_tools/http_tool/http_params_tools.py
--rw-rw-rw-   0        0        0     1609 2023-12-07 06:07:33.000000 afeng-py-tools-0.0.98/src/afeng_tools/http_tool/http_tools.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:09.747564 afeng-py-tools-0.0.98/src/afeng_tools/http_tool/httpx/
--rw-rw-rw-   0        0        0        0 2023-09-08 03:23:18.000000 afeng-py-tools-0.0.98/src/afeng_tools/http_tool/httpx/__init__.py
--rw-rw-rw-   0        0        0      654 2023-12-07 06:07:51.000000 afeng-py-tools-0.0.98/src/afeng_tools/http_tool/httpx/async_http.py
--rw-rw-rw-   0        0        0      679 2023-01-20 11:38:01.000000 afeng-py-tools-0.0.98/src/afeng_tools/http_tool/httpx/sync_http.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:09.753307 afeng-py-tools-0.0.98/src/afeng_tools/id_code_tool/
--rw-rw-rw-   0        0        0       27 2023-12-06 19:28:37.000000 afeng-py-tools-0.0.98/src/afeng_tools/id_code_tool/__init__.py
--rw-rw-rw-   0        0        0      466 2023-12-27 09:12:18.000000 afeng-py-tools-0.0.98/src/afeng_tools/id_code_tool/id_code_tools.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:09.758766 afeng-py-tools-0.0.98/src/afeng_tools/image_tool/
--rw-rw-rw-   0        0        0        0 2023-10-28 15:52:08.000000 afeng-py-tools-0.0.98/src/afeng_tools/image_tool/__init__.py
--rw-rw-rw-   0        0        0     1045 2023-12-07 06:17:36.000000 afeng-py-tools-0.0.98/src/afeng_tools/image_tool/image_base64_tools.py
--rw-rw-rw-   0        0        0      155 2023-12-28 16:39:19.000000 afeng-py-tools-0.0.98/src/afeng_tools/image_tool/image_watermark_tools.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:09.762059 afeng-py-tools-0.0.98/src/afeng_tools/import_tool/
--rw-rw-rw-   0        0        0       28 2023-12-06 19:29:56.000000 afeng-py-tools-0.0.98/src/afeng_tools/import_tool/__init__.py
--rw-rw-rw-   0        0        0      703 2023-12-06 19:30:40.000000 afeng-py-tools-0.0.98/src/afeng_tools/import_tool/import_tools.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:09.766514 afeng-py-tools-0.0.98/src/afeng_tools/javascript_tool/
--rw-rw-rw-   0        0        0        0 2023-09-13 01:05:07.000000 afeng-py-tools-0.0.98/src/afeng_tools/javascript_tool/__init__.py
--rw-rw-rw-   0        0        0     1255 2023-12-07 06:34:23.000000 afeng-py-tools-0.0.98/src/afeng_tools/javascript_tool/javascript_tools.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:09.774051 afeng-py-tools-0.0.98/src/afeng_tools/jinja2_tool/
--rw-rw-rw-   0        0        0        0 2023-09-27 00:07:32.000000 afeng-py-tools-0.0.98/src/afeng_tools/jinja2_tool/__init__.py
--rw-rw-rw-   0        0        0      591 2023-12-07 06:31:20.000000 afeng-py-tools-0.0.98/src/afeng_tools/jinja2_tool/jinja2_decorator_tools.py
--rw-rw-rw-   0        0        0      999 2023-12-07 06:31:20.000000 afeng-py-tools-0.0.98/src/afeng_tools/jinja2_tool/jinja2_filters.py
--rw-rw-rw-   0        0        0     1729 2023-12-07 06:31:38.000000 afeng-py-tools-0.0.98/src/afeng_tools/jinja2_tool/jinja2_tools.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:09.777334 afeng-py-tools-0.0.98/src/afeng_tools/json_tool/
--rw-rw-rw-   0        0        0       20 2023-12-06 19:31:29.000000 afeng-py-tools-0.0.98/src/afeng_tools/json_tool/__init__.py
--rw-rw-rw-   0        0        0     2308 2023-12-11 08:20:44.000000 afeng-py-tools-0.0.98/src/afeng_tools/json_tool/json_tools.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:09.780947 afeng-py-tools-0.0.98/src/afeng_tools/layui_tool/
--rw-rw-rw-   0        0        0      160 2023-12-07 06:33:01.000000 afeng-py-tools-0.0.98/src/afeng_tools/layui_tool/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:09.784191 afeng-py-tools-0.0.98/src/afeng_tools/layui_tool/core/
--rw-rw-rw-   0        0        0        0 2023-11-23 22:49:49.000000 afeng-py-tools-0.0.98/src/afeng_tools/layui_tool/core/__init__.py
--rw-rw-rw-   0        0        0     3343 2023-12-12 07:31:42.000000 afeng-py-tools-0.0.98/src/afeng_tools/layui_tool/core/layui_models.py
--rw-rw-rw-   0        0        0     5254 2023-12-07 06:33:01.000000 afeng-py-tools-0.0.98/src/afeng_tools/layui_tool/layui_template_tools.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:09.405717 afeng-py-tools-0.0.98/src/afeng_tools/layui_tool/template/
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:09.785264 afeng-py-tools-0.0.98/src/afeng_tools/layui_tool/template/form/
--rw-rw-rw-   0        0        0    17518 2023-11-29 06:33:34.000000 afeng-py-tools-0.0.98/src/afeng_tools/layui_tool/template/form/step_form.html
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:09.792905 afeng-py-tools-0.0.98/src/afeng_tools/layui_tool/template/table/
--rw-rw-rw-   0        0        0    13217 2023-12-01 00:51:05.000000 afeng-py-tools-0.0.98/src/afeng_tools/layui_tool/template/table/add.html
--rw-rw-rw-   0        0        0    13387 2023-12-01 00:51:10.000000 afeng-py-tools-0.0.98/src/afeng_tools/layui_tool/template/table/edit.html
--rw-rw-rw-   0        0        0    11537 2023-12-12 07:33:26.000000 afeng-py-tools-0.0.98/src/afeng_tools/layui_tool/template/table/list.html
--rw-rw-rw-   0        0        0     5513 2023-12-01 00:50:37.000000 afeng-py-tools-0.0.98/src/afeng_tools/layui_tool/template/table/show.html
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:09.800610 afeng-py-tools-0.0.98/src/afeng_tools/linux_tool/
--rw-rw-rw-   0        0        0       30 2023-12-06 19:28:07.000000 afeng-py-tools-0.0.98/src/afeng_tools/linux_tool/__init__.py
--rw-rw-rw-   0        0        0      811 2023-09-27 01:17:04.000000 afeng-py-tools-0.0.98/src/afeng_tools/linux_tool/linux_match_tools.py
--rw-rw-rw-   0        0        0      556 2024-01-31 23:35:13.000000 afeng-py-tools-0.0.98/src/afeng_tools/linux_tool/sh_tools.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:09.809303 afeng-py-tools-0.0.98/src/afeng_tools/log_tool/
--rw-rw-rw-   0        0        0        0 2023-12-06 22:51:06.000000 afeng-py-tools-0.0.98/src/afeng_tools/log_tool/__init__.py
--rw-rw-rw-   0        0        0      221 2023-12-06 23:00:18.000000 afeng-py-tools-0.0.98/src/afeng_tools/log_tool/logger_enums.py
--rw-rw-rw-   0        0        0      776 2023-12-08 06:33:33.000000 afeng-py-tools-0.0.98/src/afeng_tools/log_tool/logger_settings.py
--rw-rw-rw-   0        0        0     1036 2023-12-06 23:00:35.000000 afeng-py-tools-0.0.98/src/afeng_tools/log_tool/logging_tools.py
--rw-rw-rw-   0        0        0     1016 2023-12-08 00:27:19.000000 afeng-py-tools-0.0.98/src/afeng_tools/log_tool/loguru_tools.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:09.815970 afeng-py-tools-0.0.98/src/afeng_tools/math_tool/
--rw-rw-rw-   0        0        0       22 2023-12-06 21:21:05.000000 afeng-py-tools-0.0.98/src/afeng_tools/math_tool/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:09.819237 afeng-py-tools-0.0.98/src/afeng_tools/math_tool/core/
--rw-rw-rw-   0        0        0        0 2023-12-24 00:27:13.000000 afeng-py-tools-0.0.98/src/afeng_tools/math_tool/core/__init__.py
--rw-rw-rw-   0        0        0     3291 2023-12-24 01:00:22.000000 afeng-py-tools-0.0.98/src/afeng_tools/math_tool/core/number_to_chinese.py
--rw-rw-rw-   0        0        0      450 2023-12-24 00:46:29.000000 afeng-py-tools-0.0.98/src/afeng_tools/math_tool/number_tools.py
--rw-rw-rw-   0        0        0      897 2023-12-07 09:27:40.000000 afeng-py-tools-0.0.98/src/afeng_tools/math_tool/random_tools.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:09.824815 afeng-py-tools-0.0.98/src/afeng_tools/os_tool/
--rw-rw-rw-   0        0        0       18 2023-12-06 19:33:22.000000 afeng-py-tools-0.0.98/src/afeng_tools/os_tool/__init__.py
--rw-rw-rw-   0        0        0      711 2023-12-06 19:34:05.000000 afeng-py-tools-0.0.98/src/afeng_tools/os_tool/os_platform_tools.py
--rw-rw-rw-   0        0        0      134 2023-12-08 07:01:16.000000 afeng-py-tools-0.0.98/src/afeng_tools/os_tool/os_tools.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:09.828245 afeng-py-tools-0.0.98/src/afeng_tools/pandas_tool/
--rw-rw-rw-   0        0        0        0 2023-09-07 10:17:43.000000 afeng-py-tools-0.0.98/src/afeng_tools/pandas_tool/__init__.py
--rw-rw-rw-   0        0        0      890 2023-12-07 06:12:11.000000 afeng-py-tools-0.0.98/src/afeng_tools/pandas_tool/pandas_tools.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:09.839246 afeng-py-tools-0.0.98/src/afeng_tools/playwright_tool/
--rw-rw-rw-   0        0        0      106 2023-09-25 00:06:07.000000 afeng-py-tools-0.0.98/src/afeng_tools/playwright_tool/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:09.846977 afeng-py-tools-0.0.98/src/afeng_tools/playwright_tool/decorator/
--rw-rw-rw-   0        0        0       41 2023-09-08 17:53:07.000000 afeng-py-tools-0.0.98/src/afeng_tools/playwright_tool/decorator/__init__.py
--rw-rw-rw-   0        0        0     2101 2023-12-11 07:11:01.000000 afeng-py-tools-0.0.98/src/afeng_tools/playwright_tool/decorator/playwright_async_decorators.py
--rw-rw-rw-   0        0        0     2333 2023-12-11 07:11:01.000000 afeng-py-tools-0.0.98/src/afeng_tools/playwright_tool/decorator/playwright_decorators.py
--rw-rw-rw-   0        0        0     1942 2023-12-07 06:04:30.000000 afeng-py-tools-0.0.98/src/afeng_tools/playwright_tool/http_cookie_tools.py
--rw-rw-rw-   0        0        0     1549 2023-12-07 06:04:30.000000 afeng-py-tools-0.0.98/src/afeng_tools/playwright_tool/http_header_tools.py
--rw-rw-rw-   0        0        0     1275 2023-12-07 06:04:47.000000 afeng-py-tools-0.0.98/src/afeng_tools/playwright_tool/http_storage_tools.py
--rw-rw-rw-   0        0        0     2008 2023-12-07 06:07:26.000000 afeng-py-tools-0.0.98/src/afeng_tools/playwright_tool/playwright_tools.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:09.850277 afeng-py-tools-0.0.98/src/afeng_tools/playwright_tool/spider/
--rw-rw-rw-   0        0        0        0 2023-12-20 06:49:24.000000 afeng-py-tools-0.0.98/src/afeng_tools/playwright_tool/spider/__init__.py
--rw-rw-rw-   0        0        0     2775 2023-12-21 05:01:06.000000 afeng-py-tools-0.0.98/src/afeng_tools/playwright_tool/spider/base_spider.py
--rw-rw-rw-   0        0        0      926 2023-12-07 06:07:26.000000 afeng-py-tools-0.0.98/src/afeng_tools/playwright_tool/test001.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:09.853513 afeng-py-tools-0.0.98/src/afeng_tools/pydantic_tool/
--rw-rw-rw-   0        0        0        0 2023-10-22 09:32:57.000000 afeng-py-tools-0.0.98/src/afeng_tools/pydantic_tool/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:09.856950 afeng-py-tools-0.0.98/src/afeng_tools/pydantic_tool/model/
--rw-rw-rw-   0        0        0        0 2023-12-11 07:42:54.000000 afeng-py-tools-0.0.98/src/afeng_tools/pydantic_tool/model/__init__.py
--rw-rw-rw-   0        0        0     1010 2024-02-04 16:33:50.000000 afeng-py-tools-0.0.98/src/afeng_tools/pydantic_tool/model/common_models.py
--rw-rw-rw-   0        0        0     1595 2023-12-25 06:27:58.000000 afeng-py-tools-0.0.98/src/afeng_tools/pydantic_tool/pydantic_tools.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:09.861273 afeng-py-tools-0.0.98/src/afeng_tools/python_tool/
--rw-rw-rw-   0        0        0        0 2023-12-24 11:47:52.000000 afeng-py-tools-0.0.98/src/afeng_tools/python_tool/__init__.py
--rw-rw-rw-   0        0        0     2525 2023-12-24 12:08:53.000000 afeng-py-tools-0.0.98/src/afeng_tools/python_tool/dict_tools.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:09.867851 afeng-py-tools-0.0.98/src/afeng_tools/qrcode_tool/
--rw-rw-rw-   0        0        0        0 2023-11-10 20:49:35.000000 afeng-py-tools-0.0.98/src/afeng_tools/qrcode_tool/__init__.py
--rw-rw-rw-   0        0        0      707 2023-12-07 05:59:34.000000 afeng-py-tools-0.0.98/src/afeng_tools/qrcode_tool/qrcode_demo.py
--rw-rw-rw-   0        0        0     2860 2023-12-07 05:58:58.000000 afeng-py-tools-0.0.98/src/afeng_tools/qrcode_tool/qrcode_image_tools.py
--rw-rw-rw-   0        0        0     3258 2023-11-10 21:01:34.000000 afeng-py-tools-0.0.98/src/afeng_tools/qrcode_tool/qrcode_tools.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:09.871124 afeng-py-tools-0.0.98/src/afeng_tools/re_tool/
--rw-rw-rw-   0        0        0       22 2023-12-06 21:21:53.000000 afeng-py-tools-0.0.98/src/afeng_tools/re_tool/__init__.py
--rw-rw-rw-   0        0        0     1411 2023-12-06 21:23:39.000000 afeng-py-tools-0.0.98/src/afeng_tools/re_tool/re_tools.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:09.880057 afeng-py-tools-0.0.98/src/afeng_tools/scrapy_tool/
--rw-rw-rw-   0        0        0        0 2024-01-15 12:55:42.000000 afeng-py-tools-0.0.98/src/afeng_tools/scrapy_tool/__init__.py
--rw-rw-rw-   0        0        0     1186 2024-02-05 16:06:55.000000 afeng-py-tools-0.0.98/src/afeng_tools/scrapy_tool/scrapy_request_tools.py
--rw-rw-rw-   0        0        0     1721 2024-01-29 04:26:00.000000 afeng-py-tools-0.0.98/src/afeng_tools/scrapy_tool/scrapy_run_tools.py
--rw-rw-rw-   0        0        0      992 2024-02-05 04:52:37.000000 afeng-py-tools-0.0.98/src/afeng_tools/scrapy_tool/scrapy_selector_tools.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:09.883339 afeng-py-tools-0.0.98/src/afeng_tools/serialization_tool/
--rw-rw-rw-   0        0        0       34 2023-12-06 21:18:45.000000 afeng-py-tools-0.0.98/src/afeng_tools/serialization_tool/__init__.py
--rw-rw-rw-   0        0        0      577 2023-12-06 21:19:25.000000 afeng-py-tools-0.0.98/src/afeng_tools/serialization_tool/pickle_tools.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:09.892205 afeng-py-tools-0.0.98/src/afeng_tools/sqlalchemy_tool/
--rw-rw-rw-   0        0        0      194 2023-12-24 06:26:30.000000 afeng-py-tools-0.0.98/src/afeng_tools/sqlalchemy_tool/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:09.909867 afeng-py-tools-0.0.98/src/afeng_tools/sqlalchemy_tool/core/
--rw-rw-rw-   0        0        0       32 2023-12-06 22:34:44.000000 afeng-py-tools-0.0.98/src/afeng_tools/sqlalchemy_tool/core/__init__.py
--rw-rw-rw-   0        0        0     5051 2023-12-08 06:39:50.000000 afeng-py-tools-0.0.98/src/afeng_tools/sqlalchemy_tool/core/orm_model_tools.py
--rw-rw-rw-   0        0        0      752 2023-12-06 22:48:04.000000 afeng-py-tools-0.0.98/src/afeng_tools/sqlalchemy_tool/core/sqlalchemy_base_model.py
--rw-rw-rw-   0        0        0     1713 2023-12-06 22:44:38.000000 afeng-py-tools-0.0.98/src/afeng_tools/sqlalchemy_tool/core/sqlalchemy_db_tools.py
--rw-rw-rw-   0        0        0      120 2023-12-07 02:08:00.000000 afeng-py-tools-0.0.98/src/afeng_tools/sqlalchemy_tool/core/sqlalchemy_enums.py
--rw-rw-rw-   0        0        0      518 2023-12-07 02:04:04.000000 afeng-py-tools-0.0.98/src/afeng_tools/sqlalchemy_tool/core/sqlalchemy_item.py
--rw-rw-rw-   0        0        0     2603 2023-12-07 01:24:48.000000 afeng-py-tools-0.0.98/src/afeng_tools/sqlalchemy_tool/core/sqlalchemy_meta_class.py
--rw-rw-rw-   0        0        0     1866 2023-12-09 05:14:18.000000 afeng-py-tools-0.0.98/src/afeng_tools/sqlalchemy_tool/core/sqlalchemy_model_utils.py
--rw-rw-rw-   0        0        0     2924 2023-12-07 04:12:13.000000 afeng-py-tools-0.0.98/src/afeng_tools/sqlalchemy_tool/core/sqlalchemy_session_decorator.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:09.922995 afeng-py-tools-0.0.98/src/afeng_tools/sqlalchemy_tool/crdu/
--rw-rw-rw-   0        0        0       38 2023-12-06 22:49:26.000000 afeng-py-tools-0.0.98/src/afeng_tools/sqlalchemy_tool/crdu/__init__.py
--rw-rw-rw-   0        0        0     7449 2023-12-11 23:22:06.000000 afeng-py-tools-0.0.98/src/afeng_tools/sqlalchemy_tool/crdu/base_crdu.py
--rw-rw-rw-   0        0        0      291 2023-09-07 20:22:22.000000 afeng-py-tools-0.0.98/src/afeng_tools/sqlalchemy_tool/crdu/ddl_crdu.py
--rw-rw-rw-   0        0        0     1429 2023-12-22 23:33:25.000000 afeng-py-tools-0.0.98/src/afeng_tools/sqlalchemy_tool/crdu/sequence_crdu.py
--rw-rw-rw-   0        0        0     6552 2023-12-08 06:39:50.000000 afeng-py-tools-0.0.98/src/afeng_tools/sqlalchemy_tool/crdu/session_crdu.py
--rw-rw-rw-   0        0        0      781 2023-12-07 05:53:31.000000 afeng-py-tools-0.0.98/src/afeng_tools/sqlalchemy_tool/crdu/sql_crdu.py
--rw-rw-rw-   0        0        0     4129 2023-12-09 19:18:50.000000 afeng-py-tools-0.0.98/src/afeng_tools/sqlalchemy_tool/sqlalchemy_db_copy_tools.py
--rw-rw-rw-   0        0        0     1038 2023-12-07 23:21:41.000000 afeng-py-tools-0.0.98/src/afeng_tools/sqlalchemy_tool/sqlalchemy_settings.py
--rw-rw-rw-   0        0        0     1815 2023-12-07 05:51:24.000000 afeng-py-tools-0.0.98/src/afeng_tools/sqlalchemy_tool/sqlalchemy_tools.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:09.928562 afeng-py-tools-0.0.98/src/afeng_tools/sqlalchemy_tools/
--rw-rw-rw-   0        0        0      100 2023-12-24 04:50:28.000000 afeng-py-tools-0.0.98/src/afeng_tools/sqlalchemy_tools/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:09.942957 afeng-py-tools-0.0.98/src/afeng_tools/sqlalchemy_tools/core/
--rw-rw-rw-   0        0        0        0 2023-12-24 04:56:52.000000 afeng-py-tools-0.0.98/src/afeng_tools/sqlalchemy_tools/core/__init__.py
--rw-rw-rw-   0        0        0     1303 2023-12-25 11:20:50.000000 afeng-py-tools-0.0.98/src/afeng_tools/sqlalchemy_tools/core/sqlalchemy_base_model.py
--rw-rw-rw-   0        0        0     1466 2023-12-24 05:36:20.000000 afeng-py-tools-0.0.98/src/afeng_tools/sqlalchemy_tools/core/sqlalchemy_class.py
--rw-rw-rw-   0        0        0      120 2023-12-07 02:08:00.000000 afeng-py-tools-0.0.98/src/afeng_tools/sqlalchemy_tools/core/sqlalchemy_enums.py
--rw-rw-rw-   0        0        0      702 2023-12-24 05:06:32.000000 afeng-py-tools-0.0.98/src/afeng_tools/sqlalchemy_tools/core/sqlalchemy_items.py
--rw-rw-rw-   0        0        0     2950 2024-01-19 19:04:33.000000 afeng-py-tools-0.0.98/src/afeng_tools/sqlalchemy_tools/core/sqlalchemy_meta_class.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:09.952723 afeng-py-tools-0.0.98/src/afeng_tools/sqlalchemy_tools/crdu/
--rw-rw-rw-   0        0        0       38 2023-12-24 06:02:01.000000 afeng-py-tools-0.0.98/src/afeng_tools/sqlalchemy_tools/crdu/__init__.py
--rw-rw-rw-   0        0        0     7303 2023-12-24 06:18:59.000000 afeng-py-tools-0.0.98/src/afeng_tools/sqlalchemy_tools/crdu/base_crdu.py
--rw-rw-rw-   0        0        0     1471 2023-12-24 06:20:31.000000 afeng-py-tools-0.0.98/src/afeng_tools/sqlalchemy_tools/crdu/sequence_crdu.py
--rw-rw-rw-   0        0        0     6447 2023-12-24 06:20:31.000000 afeng-py-tools-0.0.98/src/afeng_tools/sqlalchemy_tools/crdu/session_crdu.py
--rw-rw-rw-   0        0        0      511 2023-12-24 06:23:34.000000 afeng-py-tools-0.0.98/src/afeng_tools/sqlalchemy_tools/crdu/sql_crdu.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:09.956117 afeng-py-tools-0.0.98/src/afeng_tools/sqlalchemy_tools/decorator/
--rw-rw-rw-   0        0        0       29 2023-12-24 06:02:12.000000 afeng-py-tools-0.0.98/src/afeng_tools/sqlalchemy_tools/decorator/__init__.py
--rw-rw-rw-   0        0        0     4135 2023-12-24 09:36:16.000000 afeng-py-tools-0.0.98/src/afeng_tools/sqlalchemy_tools/decorator/sqlalchemy_session_decorator.py
--rw-rw-rw-   0        0        0     4170 2023-12-24 06:23:34.000000 afeng-py-tools-0.0.98/src/afeng_tools/sqlalchemy_tools/sqlalchemy_db_copy_tools.py
--rw-rw-rw-   0        0        0     1016 2023-12-24 05:27:18.000000 afeng-py-tools-0.0.98/src/afeng_tools/sqlalchemy_tools/sqlalchemy_settings.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:09.960440 afeng-py-tools-0.0.98/src/afeng_tools/sqlalchemy_tools/tool/
--rw-rw-rw-   0        0        0        0 2023-12-24 05:57:19.000000 afeng-py-tools-0.0.98/src/afeng_tools/sqlalchemy_tools/tool/__init__.py
--rw-rw-rw-   0        0        0     4961 2023-12-24 05:58:06.000000 afeng-py-tools-0.0.98/src/afeng_tools/sqlalchemy_tools/tool/orm_model_tools.py
--rw-rw-rw-   0        0        0     1785 2023-12-24 06:18:59.000000 afeng-py-tools-0.0.98/src/afeng_tools/sqlalchemy_tools/tool/sqlalchemy_model_tools.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:09.969401 afeng-py-tools-0.0.98/src/afeng_tools/template_tool/
--rw-rw-rw-   0        0        0     1866 2023-12-11 07:11:01.000000 afeng-py-tools-0.0.98/src/afeng_tools/template_tool/README.md
--rw-rw-rw-   0        0        0       24 2023-12-08 09:44:41.000000 afeng-py-tools-0.0.98/src/afeng_tools/template_tool/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:09.983757 afeng-py-tools-0.0.98/src/afeng_tools/template_tool/core/
--rw-rw-rw-   0        0        0        0 2023-12-07 23:23:10.000000 afeng-py-tools-0.0.98/src/afeng_tools/template_tool/core/__init__.py
--rw-rw-rw-   0        0        0     1866 2023-12-09 03:01:10.000000 afeng-py-tools-0.0.98/src/afeng_tools/template_tool/core/calmjs_tools.py
--rw-rw-rw-   0        0        0      410 2023-12-09 03:01:06.000000 afeng-py-tools-0.0.98/src/afeng_tools/template_tool/core/html_tools.py
--rw-rw-rw-   0        0        0     1227 2023-12-09 03:01:02.000000 afeng-py-tools-0.0.98/src/afeng_tools/template_tool/core/js_tools.py
--rw-rw-rw-   0        0        0      824 2023-12-06 15:29:51.000000 afeng-py-tools-0.0.98/src/afeng_tools/template_tool/core/less_tools.py
--rw-rw-rw-   0        0        0      318 2023-12-09 03:01:16.000000 afeng-py-tools-0.0.98/src/afeng_tools/template_tool/core/scss_tools.py
--rw-rw-rw-   0        0        0     1120 2023-12-09 03:01:22.000000 afeng-py-tools-0.0.98/src/afeng_tools/template_tool/core/vue_tools.py
--rw-rw-rw-   0        0        0     5517 2023-12-07 06:27:14.000000 afeng-py-tools-0.0.98/src/afeng_tools/template_tool/template_auto_tools.py
--rw-rw-rw-   0        0        0      597 2023-12-07 06:27:14.000000 afeng-py-tools-0.0.98/src/afeng_tools/template_tool/template_decorator_tools.py
--rw-rw-rw-   0        0        0     4639 2023-12-08 09:44:57.000000 afeng-py-tools-0.0.98/src/afeng_tools/template_tool/template_tools.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:09.985918 afeng-py-tools-0.0.98/src/afeng_tools/template_tool/vue_demo/
--rw-rw-rw-   0        0        0     1208 2023-12-06 17:02:58.000000 afeng-py-tools-0.0.98/src/afeng_tools/template_tool/vue_demo/python_component.vue
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:09.989245 afeng-py-tools-0.0.98/src/afeng_tools/text_tool/
--rw-rw-rw-   0        0        0       22 2023-12-06 21:38:05.000000 afeng-py-tools-0.0.98/src/afeng_tools/text_tool/__init__.py
--rw-rw-rw-   0        0        0     2117 2023-08-26 09:17:28.000000 afeng-py-tools-0.0.98/src/afeng_tools/text_tool/article_split_tools.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:09.994729 afeng-py-tools-0.0.98/src/afeng_tools/text_tool/word_break_tool/
--rw-rw-rw-   0        0        0       22 2023-12-06 21:38:24.000000 afeng-py-tools-0.0.98/src/afeng_tools/text_tool/word_break_tool/__init__.py
--rw-rw-rw-   0        0        0     1284 2023-11-23 09:36:58.000000 afeng-py-tools-0.0.98/src/afeng_tools/text_tool/word_break_tool/jieba_tools.py
--rw-rw-rw-   0        0        0      305 2023-12-06 21:38:37.000000 afeng-py-tools-0.0.98/src/afeng_tools/text_tool/word_break_tool/word_break_tools.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:10.000314 afeng-py-tools-0.0.98/src/afeng_tools/trade_tool/
--rw-rw-rw-   0        0        0        0 2023-09-12 16:53:42.000000 afeng-py-tools-0.0.98/src/afeng_tools/trade_tool/__init__.py
--rw-rw-rw-   0        0        0     1559 2023-12-07 06:15:44.000000 afeng-py-tools-0.0.98/src/afeng_tools/trade_tool/trade_calendar_tools.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:10.003599 afeng-py-tools-0.0.98/src/afeng_tools/tushare_tool/
--rw-rw-rw-   0        0        0       29 2023-12-07 06:16:15.000000 afeng-py-tools-0.0.98/src/afeng_tools/tushare_tool/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:10.006836 afeng-py-tools-0.0.98/src/afeng_tools/tushare_tool/sh_sz_stock/
--rw-rw-rw-   0        0        0        0 2023-09-08 00:16:18.000000 afeng-py-tools-0.0.98/src/afeng_tools/tushare_tool/sh_sz_stock/__init__.py
--rw-rw-rw-   0        0        0     1123 2023-12-07 06:13:43.000000 afeng-py-tools-0.0.98/src/afeng_tools/tushare_tool/sh_sz_stock/stock_basic_tools.py
--rw-rw-rw-   0        0        0      149 2023-12-07 06:16:15.000000 afeng-py-tools-0.0.98/src/afeng_tools/tushare_tool/tushare_tools.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:10.015707 afeng-py-tools-0.0.98/src/afeng_tools/web_tool/
--rw-rw-rw-   0        0        0       22 2023-12-06 21:20:21.000000 afeng-py-tools-0.0.98/src/afeng_tools/web_tool/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:10.020157 afeng-py-tools-0.0.98/src/afeng_tools/web_tool/core/
--rw-rw-rw-   0        0        0        0 2023-12-10 21:21:46.000000 afeng-py-tools-0.0.98/src/afeng_tools/web_tool/core/__init__.py
--rw-rw-rw-   0        0        0      203 2023-12-10 21:24:06.000000 afeng-py-tools-0.0.98/src/afeng_tools/web_tool/core/web_common_models.py
--rw-rw-rw-   0        0        0      877 2023-12-06 21:41:14.000000 afeng-py-tools-0.0.98/src/afeng_tools/web_tool/request_tools.py
--rw-rw-rw-   0        0        0     1442 2023-12-25 06:43:59.000000 afeng-py-tools-0.0.98/src/afeng_tools/web_tool/response_tools.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:10.030128 afeng-py-tools-0.0.98/src/afeng_tools/weixin_min_program/
--rw-rw-rw-   0        0        0        0 2023-12-10 12:27:13.000000 afeng-py-tools-0.0.98/src/afeng_tools/weixin_min_program/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:10.039868 afeng-py-tools-0.0.98/src/afeng_tools/weixin_min_program/core/
--rw-rw-rw-   0        0        0        0 2023-12-10 12:34:44.000000 afeng-py-tools-0.0.98/src/afeng_tools/weixin_min_program/core/__init__.py
--rw-rw-rw-   0        0        0     4099 2023-12-16 06:42:03.000000 afeng-py-tools-0.0.98/src/afeng_tools/weixin_min_program/core/weixin_mp_api_service.py
--rw-rw-rw-   0        0        0     1158 2023-12-10 22:29:12.000000 afeng-py-tools-0.0.98/src/afeng_tools/weixin_min_program/core/weixin_mp_decrypt.py
--rw-rw-rw-   0        0        0     2063 2023-12-16 10:03:08.000000 afeng-py-tools-0.0.98/src/afeng_tools/weixin_min_program/core/weixin_mp_models.py
--rw-rw-rw-   0        0        0     4311 2023-12-16 09:50:07.000000 afeng-py-tools-0.0.98/src/afeng_tools/weixin_min_program/core/weixin_mp_service.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:10.045517 afeng-py-tools-0.0.98/src/afeng_tools/weixin_min_program/model/
--rw-rw-rw-   0        0        0        0 2023-12-10 12:27:13.000000 afeng-py-tools-0.0.98/src/afeng_tools/weixin_min_program/model/__init__.py
--rw-rw-rw-   0        0        0     1503 2023-12-16 09:48:30.000000 afeng-py-tools-0.0.98/src/afeng_tools/weixin_min_program/model/weixin_mp_enums.py
--rw-rw-rw-   0        0        0     1090 2023-12-16 09:49:29.000000 afeng-py-tools-0.0.98/src/afeng_tools/weixin_min_program/model/weixin_mp_open_models.py
--rw-rw-rw-   0        0        0     1544 2023-12-16 09:46:54.000000 afeng-py-tools-0.0.98/src/afeng_tools/weixin_min_program/weixin_mp_settings.py
--rw-rw-rw-   0        0        0     1407 2023-12-16 02:29:14.000000 afeng-py-tools-0.0.98/src/afeng_tools/weixin_min_program/weixin_mp_tools.py
--rw-rw-rw-   0        0        0     1459 2023-12-16 10:02:58.000000 afeng-py-tools-0.0.98/src/afeng_tools/weixin_min_program/weixin_mp_views.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:10.051053 afeng-py-tools-0.0.98/src/afeng_tools/weixin_tool/
--rw-rw-rw-   0        0        0      196 2023-12-06 21:47:34.000000 afeng-py-tools-0.0.98/src/afeng_tools/weixin_tool/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:10.061061 afeng-py-tools-0.0.98/src/afeng_tools/weixin_tool/core/
--rw-rw-rw-   0        0        0        0 2023-11-14 21:09:25.000000 afeng-py-tools-0.0.98/src/afeng_tools/weixin_tool/core/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:10.064418 afeng-py-tools-0.0.98/src/afeng_tools/weixin_tool/core/format/
--rw-rw-rw-   0        0        0       25 2023-12-06 21:52:19.000000 afeng-py-tools-0.0.98/src/afeng_tools/weixin_tool/core/format/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:10.070859 afeng-py-tools-0.0.98/src/afeng_tools/weixin_tool/core/format/reply_msg/
--rw-rw-rw-   0        0        0       28 2023-12-06 21:46:21.000000 afeng-py-tools-0.0.98/src/afeng_tools/weixin_tool/core/format/reply_msg/__init__.py
--rw-rw-rw-   0        0        0      301 2023-11-15 02:51:53.000000 afeng-py-tools-0.0.98/src/afeng_tools/weixin_tool/core/format/reply_msg/weixin_format_tool.py
--rw-rw-rw-   0        0        0     3239 2023-11-15 02:55:54.000000 afeng-py-tools-0.0.98/src/afeng_tools/weixin_tool/core/format/reply_msg/weixin_models.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:10.091535 afeng-py-tools-0.0.98/src/afeng_tools/weixin_tool/core/format/reply_msg/xml/
--rw-rw-rw-   0        0        0      271 2022-12-27 04:24:36.000000 afeng-py-tools-0.0.98/src/afeng_tools/weixin_tool/core/format/reply_msg/xml/image_msg.xml
--rw-rw-rw-   0        0        0      492 2022-12-27 04:57:50.000000 afeng-py-tools-0.0.98/src/afeng_tools/weixin_tool/core/format/reply_msg/xml/music_msg.xml
--rw-rw-rw-   0        0        0      297 2022-12-27 05:09:48.000000 afeng-py-tools-0.0.98/src/afeng_tools/weixin_tool/core/format/reply_msg/xml/news_msg.xml
--rw-rw-rw-   0        0        0      191 2022-12-27 05:09:48.000000 afeng-py-tools-0.0.98/src/afeng_tools/weixin_tool/core/format/reply_msg/xml/news_msg_item.xml
--rw-rw-rw-   0        0        0      244 2022-12-27 04:24:36.000000 afeng-py-tools-0.0.98/src/afeng_tools/weixin_tool/core/format/reply_msg/xml/text_msg.xml
--rw-rw-rw-   0        0        0      363 2022-12-27 04:49:51.000000 afeng-py-tools-0.0.98/src/afeng_tools/weixin_tool/core/format/reply_msg/xml/video_msg.xml
--rw-rw-rw-   0        0        0      271 2022-12-27 04:37:13.000000 afeng-py-tools-0.0.98/src/afeng_tools/weixin_tool/core/format/reply_msg/xml/voice_msg.xml
--rw-rw-rw-   0        0        0      597 2023-12-06 21:52:19.000000 afeng-py-tools-0.0.98/src/afeng_tools/weixin_tool/core/format/weixin_format_replay.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:10.094950 afeng-py-tools-0.0.98/src/afeng_tools/weixin_tool/core/model/
--rw-rw-rw-   0        0        0        0 2022-12-26 19:26:44.000000 afeng-py-tools-0.0.98/src/afeng_tools/weixin_tool/core/model/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:10.101454 afeng-py-tools-0.0.98/src/afeng_tools/weixin_tool/core/model/item/
--rw-rw-rw-   0        0        0        0 2023-11-14 23:46:01.000000 afeng-py-tools-0.0.98/src/afeng_tools/weixin_tool/core/model/item/__init__.py
--rw-rw-rw-   0        0        0     2352 2023-12-08 00:26:45.000000 afeng-py-tools-0.0.98/src/afeng_tools/weixin_tool/core/model/item/wx_receive_event_models.py
--rw-rw-rw-   0        0        0     2726 2023-11-15 02:32:47.000000 afeng-py-tools-0.0.98/src/afeng_tools/weixin_tool/core/model/item/wx_receive_msg_models.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:10.107010 afeng-py-tools-0.0.98/src/afeng_tools/weixin_tool/core/model/po/
--rw-rw-rw-   0        0        0      117 2023-12-06 22:39:11.000000 afeng-py-tools-0.0.98/src/afeng_tools/weixin_tool/core/model/po/__init__.py
--rw-rw-rw-   0        0        0     3177 2023-12-25 06:27:58.000000 afeng-py-tools-0.0.98/src/afeng_tools/weixin_tool/core/model/po/wx_receive_event_models.py
--rw-rw-rw-   0        0        0     3834 2023-12-25 06:27:58.000000 afeng-py-tools-0.0.98/src/afeng_tools/weixin_tool/core/model/po/wx_receive_msg_models.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:10.110322 afeng-py-tools-0.0.98/src/afeng_tools/weixin_tool/core/parse/
--rw-rw-rw-   0        0        0        0 2022-12-27 02:17:10.000000 afeng-py-tools-0.0.98/src/afeng_tools/weixin_tool/core/parse/__init__.py
--rw-rw-rw-   0        0        0     1442 2023-12-07 22:49:24.000000 afeng-py-tools-0.0.98/src/afeng_tools/weixin_tool/core/parse/parse_receive.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:10.115748 afeng-py-tools-0.0.98/src/afeng_tools/weixin_tool/core/parse/receive_event/
--rw-rw-rw-   0        0        0        0 2022-12-27 03:35:50.000000 afeng-py-tools-0.0.98/src/afeng_tools/weixin_tool/core/parse/receive_event/__init__.py
--rw-rw-rw-   0        0        0     3382 2023-12-07 22:49:24.000000 afeng-py-tools-0.0.98/src/afeng_tools/weixin_tool/core/parse/receive_event/parse_event.py
--rw-rw-rw-   0        0        0      716 2023-12-07 22:49:24.000000 afeng-py-tools-0.0.98/src/afeng_tools/weixin_tool/core/parse/receive_event/parse_tool.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:10.124834 afeng-py-tools-0.0.98/src/afeng_tools/weixin_tool/core/parse/receive_msg/
--rw-rw-rw-   0        0        0        0 2022-12-26 16:34:18.000000 afeng-py-tools-0.0.98/src/afeng_tools/weixin_tool/core/parse/receive_msg/__init__.py
--rw-rw-rw-   0        0        0     3840 2023-12-07 22:49:24.000000 afeng-py-tools-0.0.98/src/afeng_tools/weixin_tool/core/parse/receive_msg/parse_msg.py
--rw-rw-rw-   0        0        0     2300 2023-12-07 22:49:24.000000 afeng-py-tools-0.0.98/src/afeng_tools/weixin_tool/core/parse/receive_msg/parse_tool.py
--rw-rw-rw-   0        0        0      240 2022-12-27 05:37:11.000000 afeng-py-tools-0.0.98/src/afeng_tools/weixin_tool/core/response.py
--rw-rw-rw-   0        0        0     1418 2023-12-07 23:12:28.000000 afeng-py-tools-0.0.98/src/afeng_tools/weixin_tool/core/weixin_depends.py
--rw-rw-rw-   0        0        0     1880 2023-12-16 02:20:46.000000 afeng-py-tools-0.0.98/src/afeng_tools/weixin_tool/core/weixin_enums.py
--rw-rw-rw-   0        0        0      694 2023-12-07 23:52:20.000000 afeng-py-tools-0.0.98/src/afeng_tools/weixin_tool/core/weixin_reply_tool.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:10.131484 afeng-py-tools-0.0.98/src/afeng_tools/weixin_tool/custom_menu/
--rw-rw-rw-   0        0        0       27 2023-11-22 20:49:32.000000 afeng-py-tools-0.0.98/src/afeng_tools/weixin_tool/custom_menu/__init__.py
--rw-rw-rw-   0        0        0     5111 2023-11-22 21:48:05.000000 afeng-py-tools-0.0.98/src/afeng_tools/weixin_tool/custom_menu/wx_custome_menu_models.py
--rw-rw-rw-   0        0        0     1861 2023-12-07 23:16:19.000000 afeng-py-tools-0.0.98/src/afeng_tools/weixin_tool/custom_menu/wx_custome_menu_tools.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:10.138105 afeng-py-tools-0.0.98/src/afeng_tools/weixin_tool/token/
--rw-rw-rw-   0        0        0      129 2023-11-22 20:50:34.000000 afeng-py-tools-0.0.98/src/afeng_tools/weixin_tool/token/__init__.py
--rw-rw-rw-   0        0        0      322 2023-11-22 21:02:34.000000 afeng-py-tools-0.0.98/src/afeng_tools/weixin_tool/token/wx_token_models.py
--rw-rw-rw-   0        0        0     2877 2023-12-08 07:15:41.000000 afeng-py-tools-0.0.98/src/afeng_tools/weixin_tool/token/wx_token_tools.py
--rw-rw-rw-   0        0        0     1264 2023-12-16 04:41:08.000000 afeng-py-tools-0.0.98/src/afeng_tools/weixin_tool/weixin_settings.py
--rw-rw-rw-   0        0        0     1673 2023-12-21 00:21:43.000000 afeng-py-tools-0.0.98/src/afeng_tools/weixin_tool/weixin_views.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:10.150123 afeng-py-tools-0.0.98/src/afeng_tools/windows_tool/
--rw-rw-rw-   0        0        0       26 2023-12-06 21:39:27.000000 afeng-py-tools-0.0.98/src/afeng_tools/windows_tool/__init__.py
--rw-rw-rw-   0        0        0      417 2023-12-06 21:40:16.000000 afeng-py-tools-0.0.98/src/afeng_tools/windows_tool/image_tools.py
--rw-rw-rw-   0        0        0      762 2023-09-24 23:57:02.000000 afeng-py-tools-0.0.98/src/afeng_tools/windows_tool/notify_tools.py
--rw-rw-rw-   0        0        0      301 2023-09-24 23:55:52.000000 afeng-py-tools-0.0.98/src/afeng_tools/windows_tool/tts_tools.py
--rw-rw-rw-   0        0        0      294 2023-10-07 10:10:04.000000 afeng-py-tools-0.0.98/src/afeng_tools/windows_tool/window_tools.py
--rw-rw-rw-   0        0        0     1146 2024-01-31 23:36:01.000000 afeng-py-tools-0.0.98/src/afeng_tools/windows_tool/windows_sh_tools.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:10.163693 afeng-py-tools-0.0.98/src/openapi_client/
--rw-rw-rw-   0        0        0      662 2022-06-16 10:13:37.000000 afeng-py-tools-0.0.98/src/openapi_client/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:10.175896 afeng-py-tools-0.0.98/src/openapi_client/api/
--rw-rw-rw-   0        0        0      235 2022-06-16 10:13:37.000000 afeng-py-tools-0.0.98/src/openapi_client/api/__init__.py
--rw-rw-rw-   0        0        0    23616 2022-06-16 10:13:37.000000 afeng-py-tools-0.0.98/src/openapi_client/api/auth_api.py
--rw-rw-rw-   0        0        0    25848 2022-06-16 10:13:37.000000 afeng-py-tools-0.0.98/src/openapi_client/api/fileinfo_api.py
--rw-rw-rw-   0        0        0    23597 2022-06-16 10:13:37.000000 afeng-py-tools-0.0.98/src/openapi_client/api/filemanager_api.py
--rw-rw-rw-   0        0        0    21377 2022-06-16 10:13:37.000000 afeng-py-tools-0.0.98/src/openapi_client/api/fileupload_api.py
--rw-rw-rw-   0        0        0    13681 2022-06-16 10:13:37.000000 afeng-py-tools-0.0.98/src/openapi_client/api/multimediafile_api.py
--rw-rw-rw-   0        0        0    10977 2022-06-16 10:13:37.000000 afeng-py-tools-0.0.98/src/openapi_client/api/userinfo_api.py
--rw-rw-rw-   0        0        0    37573 2022-06-16 10:13:37.000000 afeng-py-tools-0.0.98/src/openapi_client/api_client.py
--rw-rw-rw-   0        0        0    16414 2022-06-16 10:13:37.000000 afeng-py-tools-0.0.98/src/openapi_client/configuration.py
--rw-rw-rw-   0        0        0     5565 2022-06-16 10:13:37.000000 afeng-py-tools-0.0.98/src/openapi_client/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-02-05 16:10:10.190224 afeng-py-tools-0.0.98/src/openapi_client/model/
--rw-rw-rw-   0        0        0      348 2022-06-16 10:13:37.000000 afeng-py-tools-0.0.98/src/openapi_client/model/__init__.py
--rw-rw-rw-   0        0        0    12130 2022-06-16 10:13:37.000000 afeng-py-tools-0.0.98/src/openapi_client/model/oauth_token_authorization_code_response.py
--rw-rw-rw-   0        0        0    12104 2022-06-16 10:13:37.000000 afeng-py-tools-0.0.98/src/openapi_client/model/oauth_token_device_code_response.py
--rw-rw-rw-   0        0        0    12112 2022-06-16 10:13:37.000000 afeng-py-tools-0.0.98/src/openapi_client/model/oauth_token_device_token_response.py
--rw-rw-rw-   0        0        0    12115 2022-06-16 10:13:37.000000 afeng-py-tools-0.0.98/src/openapi_client/model/oauth_token_refresh_token_response.py
--rw-rw-rw-   0        0        0    11912 2022-06-16 10:13:37.000000 afeng-py-tools-0.0.98/src/openapi_client/model/quotaresponse.py
--rw-rw-rw-   0        0        0    12370 2022-06-16 10:13:37.000000 afeng-py-tools-0.0.98/src/openapi_client/model/uinforesponse.py
--rw-rw-rw-   0        0        0    81982 2023-12-16 05:11:02.000000 afeng-py-tools-0.0.98/src/openapi_client/model_utils.py
--rw-rw-rw-   0        0        0    14763 2022-06-16 10:13:37.000000 afeng-py-tools-0.0.98/src/openapi_client/rest.py
--rw-rw-rw-   0        0        0     1822 2023-12-07 09:17:51.000000 afeng-py-tools-0.0.98/src/version_helper.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:32.417281 afeng-py-tools-0.0.99/
+-rw-rw-rw-   0        0        0     2182 2023-12-06 19:02:40.000000 afeng-py-tools-0.0.99/.gitignore
+-rw-rw-rw-   0        0        0     9719 2023-12-06 05:03:07.000000 afeng-py-tools-0.0.99/LICENSE
+-rw-rw-rw-   0        0        0    12634 2024-02-05 18:37:32.415065 afeng-py-tools-0.0.99/PKG-INFO
+-rw-rw-rw-   0        0        0     1003 2023-12-06 18:55:31.000000 afeng-py-tools-0.0.99/README.md
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:31.400375 afeng-py-tools-0.0.99/doc/
+-rw-rw-rw-   0        0        0     1062 2024-02-03 00:40:19.000000 afeng-py-tools-0.0.99/doc/项目打包流程.md
+-rw-rw-rw-   0        0        0     1229 2023-12-07 08:22:37.000000 afeng-py-tools-0.0.99/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-02-05 18:37:32.418337 afeng-py-tools-0.0.99/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:31.403620 afeng-py-tools-0.0.99/src/
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:32.413917 afeng-py-tools-0.0.99/src/afeng_py_tools.egg-info/
+-rw-rw-rw-   0        0        0    12634 2024-02-05 18:37:30.000000 afeng-py-tools-0.0.99/src/afeng_py_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    18283 2024-02-05 18:37:31.000000 afeng-py-tools-0.0.99/src/afeng_py_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-02-05 18:37:30.000000 afeng-py-tools-0.0.99/src/afeng_py_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2024-02-05 18:37:30.000000 afeng-py-tools-0.0.99/src/afeng_py_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:31.424808 afeng-py-tools-0.0.99/src/afeng_tools/
+-rw-rw-rw-   0        0        0       88 2023-12-06 18:41:42.000000 afeng-py-tools-0.0.99/src/afeng_tools/__init__.py
+-rw-rw-rw-   0        0        0      483 2024-02-05 18:37:29.000000 afeng-py-tools-0.0.99/src/afeng_tools/__version__.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:31.437071 afeng-py-tools-0.0.99/src/afeng_tools/aliyun_pan_tool/
+-rw-rw-rw-   0        0        0      155 2023-10-07 09:49:34.000000 afeng-py-tools-0.0.99/src/afeng_tools/aliyun_pan_tool/__init__.py
+-rw-rw-rw-   0        0        0     8377 2023-12-27 21:54:39.000000 afeng-py-tools-0.0.99/src/afeng_tools/aliyun_pan_tool/aliyun_pan_share_tools.py
+-rw-rw-rw-   0        0        0     1695 2023-12-27 21:54:39.000000 afeng-py-tools-0.0.99/src/afeng_tools/aliyun_pan_tool/aliyun_pan_sign_in_tools.py
+-rw-rw-rw-   0        0        0    11650 2023-12-27 21:54:33.000000 afeng-py-tools-0.0.99/src/afeng_tools/aliyun_pan_tool/aliyun_pan_tools.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:31.443516 afeng-py-tools-0.0.99/src/afeng_tools/aliyun_pan_tool/demo/
+-rw-rw-rw-   0        0        0        0 2023-10-07 08:20:48.000000 afeng-py-tools-0.0.99/src/afeng_tools/aliyun_pan_tool/demo/__init__.py
+-rw-rw-rw-   0        0        0     2399 2023-12-11 07:11:01.000000 afeng-py-tools-0.0.99/src/afeng_tools/aliyun_pan_tool/demo/run_demo.py
+-rw-rw-rw-   0        0        0      729 2023-12-11 07:11:01.000000 afeng-py-tools-0.0.99/src/afeng_tools/aliyun_pan_tool/demo/share_demo.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:31.462031 afeng-py-tools-0.0.99/src/afeng_tools/appium_tool/
+-rw-rw-rw-   0        0        0      107 2023-09-28 15:44:05.000000 afeng-py-tools-0.0.99/src/afeng_tools/appium_tool/__init__.py
+-rw-rw-rw-   0        0        0     5604 2023-12-07 06:09:44.000000 afeng-py-tools-0.0.99/src/afeng_tools/appium_tool/appium_client_tool.py
+-rw-rw-rw-   0        0        0      855 2023-12-07 06:09:44.000000 afeng-py-tools-0.0.99/src/afeng_tools/appium_tool/appium_options_tools.py
+-rw-rw-rw-   0        0        0     1953 2023-09-28 17:54:35.000000 afeng-py-tools-0.0.99/src/afeng_tools/appium_tool/appium_touch_tools.py
+-rw-rw-rw-   0        0        0     3439 2023-12-07 06:09:44.000000 afeng-py-tools-0.0.99/src/afeng_tools/appium_tool/mobile_adb_tools.py
+-rw-rw-rw-   0        0        0     2446 2023-12-07 06:09:44.000000 afeng-py-tools-0.0.99/src/afeng_tools/appium_tool/mobile_app_tools.py
+-rw-rw-rw-   0        0        0     2435 2023-08-07 07:52:58.000000 afeng-py-tools-0.0.99/src/afeng_tools/appium_tool/mobile_keycode.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:31.478479 afeng-py-tools-0.0.99/src/afeng_tools/application_tool/
+-rw-rw-rw-   0        0        0      275 2023-10-15 16:38:39.000000 afeng-py-tools-0.0.99/src/afeng_tools/application_tool/README.md
+-rw-rw-rw-   0        0        0        0 2023-10-15 12:57:28.000000 afeng-py-tools-0.0.99/src/afeng_tools/application_tool/__init__.py
+-rw-rw-rw-   0        0        0     2940 2024-02-03 18:47:56.000000 afeng-py-tools-0.0.99/src/afeng_tools/application_tool/application_models.py
+-rw-rw-rw-   0        0        0     2500 2023-12-07 06:29:26.000000 afeng-py-tools-0.0.99/src/afeng_tools/application_tool/application_tools.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:31.485617 afeng-py-tools-0.0.99/src/afeng_tools/application_tool/demo/
+-rw-rw-rw-   0        0        0        0 2023-10-16 05:26:55.000000 afeng-py-tools-0.0.99/src/afeng_tools/application_tool/demo/__init__.py
+-rw-rw-rw-   0        0        0      799 2023-12-07 06:29:26.000000 afeng-py-tools-0.0.99/src/afeng_tools/application_tool/demo/settings.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:31.495548 afeng-py-tools-0.0.99/src/afeng_tools/application_tool/demo/yaml_demo/
+-rw-rw-rw-   0        0        0       28 2023-10-15 17:40:37.000000 afeng-py-tools-0.0.99/src/afeng_tools/application_tool/demo/yaml_demo/application-dev.yml
+-rw-rw-rw-   0        0        0       26 2023-10-15 15:54:14.000000 afeng-py-tools-0.0.99/src/afeng_tools/application_tool/demo/yaml_demo/application-prod.yml
+-rw-rw-rw-   0        0        0       26 2023-10-15 15:53:55.000000 afeng-py-tools-0.0.99/src/afeng_tools/application_tool/demo/yaml_demo/application-test.yml
+-rw-rw-rw-   0        0        0      811 2023-10-25 00:23:53.000000 afeng-py-tools-0.0.99/src/afeng_tools/application_tool/demo/yaml_demo/application.yml
+-rw-rw-rw-   0        0        0     4717 2024-02-03 16:18:03.000000 afeng-py-tools-0.0.99/src/afeng_tools/application_tool/settings_enum.py
+-rw-rw-rw-   0        0        0     6103 2023-12-24 16:13:37.000000 afeng-py-tools-0.0.99/src/afeng_tools/application_tool/settings_tools.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:31.505497 afeng-py-tools-0.0.99/src/afeng_tools/baidu_pan_tool/
+-rw-rw-rw-   0        0        0      202 2023-10-01 05:20:31.000000 afeng-py-tools-0.0.99/src/afeng_tools/baidu_pan_tool/__init__.py
+-rw-rw-rw-   0        0        0      376 2023-12-07 06:52:24.000000 afeng-py-tools-0.0.99/src/afeng_tools/baidu_pan_tool/baidu_pan_enum.py
+-rw-rw-rw-   0        0        0     1560 2023-12-08 07:11:59.000000 afeng-py-tools-0.0.99/src/afeng_tools/baidu_pan_tool/baidu_pan_settings.py
+-rw-rw-rw-   0        0        0     8278 2023-12-08 06:56:26.000000 afeng-py-tools-0.0.99/src/afeng_tools/baidu_pan_tool/baidu_pan_tools.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:31.517628 afeng-py-tools-0.0.99/src/afeng_tools/baidu_pan_tool/core/
+-rw-rw-rw-   0        0        0        0 2023-10-01 03:30:27.000000 afeng-py-tools-0.0.99/src/afeng_tools/baidu_pan_tool/core/__init__.py
+-rw-rw-rw-   0        0        0      664 2023-12-12 13:05:57.000000 afeng-py-tools-0.0.99/src/afeng_tools/baidu_pan_tool/core/baidu_pan_api_tools.py
+-rw-rw-rw-   0        0        0     3285 2023-12-07 07:10:09.000000 afeng-py-tools-0.0.99/src/afeng_tools/baidu_pan_tool/core/baidu_pan_decorator_tools.py
+-rw-rw-rw-   0        0        0    26274 2023-12-07 07:10:20.000000 afeng-py-tools-0.0.99/src/afeng_tools/baidu_pan_tool/core/baidu_pan_models.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:31.525410 afeng-py-tools-0.0.99/src/afeng_tools/baidu_pan_tool/demo/
+-rw-rw-rw-   0        0        0        0 2023-10-01 04:22:46.000000 afeng-py-tools-0.0.99/src/afeng_tools/baidu_pan_tool/demo/__init__.py
+-rw-rw-rw-   0        0        0     5019 2023-12-07 23:18:53.000000 afeng-py-tools-0.0.99/src/afeng_tools/baidu_pan_tool/demo/baidupan_demo.py
+-rw-rw-rw-   0        0        0      995 2023-10-07 11:42:27.000000 afeng-py-tools-0.0.99/src/afeng_tools/baidu_pan_tool/demo/share_msg.txt
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:31.559816 afeng-py-tools-0.0.99/src/afeng_tools/baidu_pan_tool/tools/
+-rw-rw-rw-   0        0        0       28 2023-10-02 06:37:06.000000 afeng-py-tools-0.0.99/src/afeng_tools/baidu_pan_tool/tools/__init__.py
+-rw-rw-rw-   0        0        0     5118 2023-12-07 06:59:50.000000 afeng-py-tools-0.0.99/src/afeng_tools/baidu_pan_tool/tools/audio_file_tools.py
+-rw-rw-rw-   0        0        0     9031 2023-12-07 07:03:37.000000 afeng-py-tools-0.0.99/src/afeng_tools/baidu_pan_tool/tools/auth_tools.py
+-rw-rw-rw-   0        0        0     7215 2023-12-08 06:55:39.000000 afeng-py-tools-0.0.99/src/afeng_tools/baidu_pan_tool/tools/auth_web_tools.py
+-rw-rw-rw-   0        0        0     6502 2023-12-07 07:04:33.000000 afeng-py-tools-0.0.99/src/afeng_tools/baidu_pan_tool/tools/file_download_tools.py
+-rw-rw-rw-   0        0        0    12885 2023-12-07 07:04:33.000000 afeng-py-tools-0.0.99/src/afeng_tools/baidu_pan_tool/tools/file_manager_tools.py
+-rw-rw-rw-   0        0        0     4155 2023-12-07 07:09:42.000000 afeng-py-tools-0.0.99/src/afeng_tools/baidu_pan_tool/tools/file_meta_tools.py
+-rw-rw-rw-   0        0        0    22055 2024-01-26 17:28:32.000000 afeng-py-tools-0.0.99/src/afeng_tools/baidu_pan_tool/tools/file_path_tools.py
+-rw-rw-rw-   0        0        0    14999 2023-12-07 07:09:42.000000 afeng-py-tools-0.0.99/src/afeng_tools/baidu_pan_tool/tools/file_upload_tools.py
+-rw-rw-rw-   0        0        0       44 2023-10-04 15:36:53.000000 afeng-py-tools-0.0.99/src/afeng_tools/baidu_pan_tool/tools/image_file_tools.py
+-rw-rw-rw-   0        0        0     9863 2023-12-07 07:09:42.000000 afeng-py-tools-0.0.99/src/afeng_tools/baidu_pan_tool/tools/share_tools.py
+-rw-rw-rw-   0        0        0     2594 2023-12-07 07:09:42.000000 afeng-py-tools-0.0.99/src/afeng_tools/baidu_pan_tool/tools/user_tools.py
+-rw-rw-rw-   0        0        0     3869 2023-12-07 07:09:42.000000 afeng-py-tools-0.0.99/src/afeng_tools/baidu_pan_tool/tools/video_file_tools.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:31.566357 afeng-py-tools-0.0.99/src/afeng_tools/cache_tool/
+-rw-rw-rw-   0        0        0       22 2023-12-11 01:20:06.000000 afeng-py-tools-0.0.99/src/afeng_tools/cache_tool/__init__.py
+-rw-rw-rw-   0        0        0     1539 2023-12-11 12:02:47.000000 afeng-py-tools-0.0.99/src/afeng_tools/cache_tool/cache_decorator.py
+-rw-rw-rw-   0        0        0     1271 2024-02-04 14:09:59.000000 afeng-py-tools-0.0.99/src/afeng_tools/cache_tool/cache_memory_tools.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:31.572311 afeng-py-tools-0.0.99/src/afeng_tools/compression_tool/
+-rw-rw-rw-   0        0        0       34 2023-12-06 21:29:52.000000 afeng-py-tools-0.0.99/src/afeng_tools/compression_tool/__init__.py
+-rw-rw-rw-   0        0        0     3177 2023-12-11 07:06:12.000000 afeng-py-tools-0.0.99/src/afeng_tools/compression_tool/zip_tools.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:31.578044 afeng-py-tools-0.0.99/src/afeng_tools/convert_tool/
+-rw-rw-rw-   0        0        0       22 2023-12-06 21:26:54.000000 afeng-py-tools-0.0.99/src/afeng_tools/convert_tool/__init__.py
+-rw-rw-rw-   0        0        0     2511 2023-12-11 14:44:37.000000 afeng-py-tools-0.0.99/src/afeng_tools/convert_tool/type_convert_tools.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:31.584740 afeng-py-tools-0.0.99/src/afeng_tools/crawler_tool/
+-rw-rw-rw-   0        0        0       22 2023-12-06 21:28:37.000000 afeng-py-tools-0.0.99/src/afeng_tools/crawler_tool/__init__.py
+-rw-rw-rw-   0        0        0     3723 2023-10-06 15:31:26.000000 afeng-py-tools-0.0.99/src/afeng_tools/crawler_tool/pyquery_tools.py
+-rw-rw-rw-   0        0        0      423 2023-12-06 21:28:37.000000 afeng-py-tools-0.0.99/src/afeng_tools/crawler_tool/xpath_tools.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:31.593723 afeng-py-tools-0.0.99/src/afeng_tools/datetime_tool/
+-rw-rw-rw-   0        0        0       28 2023-12-06 19:25:21.000000 afeng-py-tools-0.0.99/src/afeng_tools/datetime_tool/__init__.py
+-rw-rw-rw-   0        0        0     1080 2023-12-11 14:38:46.000000 afeng-py-tools-0.0.99/src/afeng_tools/datetime_tool/datetime_tools.py
+-rw-rw-rw-   0        0        0      618 2023-12-07 06:10:33.000000 afeng-py-tools-0.0.99/src/afeng_tools/datetime_tool/time_monitor_tools.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:31.597314 afeng-py-tools-0.0.99/src/afeng_tools/decorator_tool/
+-rw-rw-rw-   0        0        0       25 2023-12-06 19:25:14.000000 afeng-py-tools-0.0.99/src/afeng_tools/decorator_tool/__init__.py
+-rw-rw-rw-   0        0        0     1572 2023-12-06 19:25:10.000000 afeng-py-tools-0.0.99/src/afeng_tools/decorator_tool/decorator_tools.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:31.600628 afeng-py-tools-0.0.99/src/afeng_tools/east_money_tool/
+-rw-rw-rw-   0        0        0      100 2023-12-07 06:24:05.000000 afeng-py-tools-0.0.99/src/afeng_tools/east_money_tool/__init__.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:31.603939 afeng-py-tools-0.0.99/src/afeng_tools/east_money_tool/config/
+-rw-rw-rw-   0        0        0        0 2023-09-08 02:58:20.000000 afeng-py-tools-0.0.99/src/afeng_tools/east_money_tool/config/__init__.py
+-rw-rw-rw-   0        0        0     9569 2023-09-11 15:12:14.000000 afeng-py-tools-0.0.99/src/afeng_tools/east_money_tool/config/web_url_config.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:31.621183 afeng-py-tools-0.0.99/src/afeng_tools/east_money_tool/quote_info/
+-rw-rw-rw-   0        0        0        0 2023-09-11 03:24:53.000000 afeng-py-tools-0.0.99/src/afeng_tools/east_money_tool/quote_info/__init__.py
+-rw-rw-rw-   0        0        0      841 2023-12-07 06:23:04.000000 afeng-py-tools-0.0.99/src/afeng_tools/east_money_tool/quote_info/east_money_quote_data_tools.py
+-rw-rw-rw-   0        0        0     3156 2023-12-07 06:24:05.000000 afeng-py-tools-0.0.99/src/afeng_tools/east_money_tool/quote_info/quote_field_enum.py
+-rw-rw-rw-   0        0        0    77497 2023-12-07 06:24:05.000000 afeng-py-tools-0.0.99/src/afeng_tools/east_money_tool/quote_info/quote_info_config.py
+-rw-rw-rw-   0        0        0     2087 2023-12-07 06:24:05.000000 afeng-py-tools-0.0.99/src/afeng_tools/east_money_tool/quote_info/quote_item_tools.py
+-rw-rw-rw-   0        0        0     3813 2023-09-14 03:37:24.000000 afeng-py-tools-0.0.99/src/afeng_tools/east_money_tool/quote_info/quote_models.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:31.630234 afeng-py-tools-0.0.99/src/afeng_tools/east_money_tool/stock_comment/
+-rw-rw-rw-   0        0        0      108 2023-09-08 18:14:30.000000 afeng-py-tools-0.0.99/src/afeng_tools/east_money_tool/stock_comment/__init__.py
+-rw-rw-rw-   0        0        0      737 2023-12-07 06:23:04.000000 afeng-py-tools-0.0.99/src/afeng_tools/east_money_tool/stock_comment/east_money_zhpj_tools.py
+-rw-rw-rw-   0        0        0     1388 2023-12-07 06:23:04.000000 afeng-py-tools-0.0.99/src/afeng_tools/east_money_tool/stock_comment/east_money_zlkp_tools.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:31.639963 afeng-py-tools-0.0.99/src/afeng_tools/east_money_tool/tool/
+-rw-rw-rw-   0        0        0       31 2023-09-08 18:12:36.000000 afeng-py-tools-0.0.99/src/afeng_tools/east_money_tool/tool/__init__.py
+-rw-rw-rw-   0        0        0     3359 2023-12-07 06:23:04.000000 afeng-py-tools-0.0.99/src/afeng_tools/east_money_tool/tool/east_money_http_tools.py
+-rw-rw-rw-   0        0        0      708 2023-12-07 06:23:04.000000 afeng-py-tools-0.0.99/src/afeng_tools/east_money_tool/tool/east_money_load_auth_tools.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:31.646549 afeng-py-tools-0.0.99/src/afeng_tools/email_tool/
+-rw-rw-rw-   0        0        0        0 2023-11-22 02:35:24.000000 afeng-py-tools-0.0.99/src/afeng_tools/email_tool/__init__.py
+-rw-rw-rw-   0        0        0     5330 2023-12-07 06:11:25.000000 afeng-py-tools-0.0.99/src/afeng_tools/email_tool/email_send_tools.py
+-rw-rw-rw-   0        0        0     1365 2023-11-22 14:36:51.000000 afeng-py-tools-0.0.99/src/afeng_tools/email_tool/email_tools.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:31.653499 afeng-py-tools-0.0.99/src/afeng_tools/encryption_tool/
+-rw-rw-rw-   0        0        0       31 2023-12-06 21:33:22.000000 afeng-py-tools-0.0.99/src/afeng_tools/encryption_tool/__init__.py
+-rw-rw-rw-   0        0        0     2202 2024-01-18 17:58:56.000000 afeng-py-tools-0.0.99/src/afeng_tools/encryption_tool/hashlib_tools.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:31.678087 afeng-py-tools-0.0.99/src/afeng_tools/fastapi_tool/
+-rw-rw-rw-   0        0        0      167 2023-12-07 06:43:42.000000 afeng-py-tools-0.0.99/src/afeng_tools/fastapi_tool/__init__.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:31.693626 afeng-py-tools-0.0.99/src/afeng_tools/fastapi_tool/admin/
+-rw-rw-rw-   0        0        0        0 2023-10-22 09:08:44.000000 afeng-py-tools-0.0.99/src/afeng_tools/fastapi_tool/admin/__init__.py
+-rw-rw-rw-   0        0        0     1714 2023-12-25 06:21:33.000000 afeng-py-tools-0.0.99/src/afeng_tools/fastapi_tool/admin/admin_router_model.py
+-rw-rw-rw-   0        0        0    12573 2023-12-26 11:04:12.000000 afeng-py-tools-0.0.99/src/afeng_tools/fastapi_tool/admin/admin_views_template.py
+-rw-rw-rw-   0        0        0     7129 2023-12-25 06:54:10.000000 afeng-py-tools-0.0.99/src/afeng_tools/fastapi_tool/admin/admin_views_tools.py
+-rw-rw-rw-   0        0        0      249 2023-11-25 18:56:00.000000 afeng-py-tools-0.0.99/src/afeng_tools/fastapi_tool/admin/auto_covert_func.template
+-rw-rw-rw-   0        0        0     2396 2023-12-07 06:47:56.000000 afeng-py-tools-0.0.99/src/afeng_tools/fastapi_tool/admin/fastapi_api_doc_tools.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:31.704673 afeng-py-tools-0.0.99/src/afeng_tools/fastapi_tool/core/
+-rw-rw-rw-   0        0        0        0 2023-12-08 14:20:15.000000 afeng-py-tools-0.0.99/src/afeng_tools/fastapi_tool/core/__init__.py
+-rw-rw-rw-   0        0        0     4600 2024-01-28 21:17:24.000000 afeng-py-tools-0.0.99/src/afeng_tools/fastapi_tool/core/fastapi_app_tools.py
+-rw-rw-rw-   0        0        0      409 2023-12-20 08:13:22.000000 afeng-py-tools-0.0.99/src/afeng_tools/fastapi_tool/core/fastapi_enums.py
+-rw-rw-rw-   0        0        0      946 2023-12-20 08:50:05.000000 afeng-py-tools-0.0.99/src/afeng_tools/fastapi_tool/core/fastapi_items.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:31.711262 afeng-py-tools-0.0.99/src/afeng_tools/fastapi_tool/demo/
+-rw-rw-rw-   0        0        0        0 2023-10-16 02:43:46.000000 afeng-py-tools-0.0.99/src/afeng_tools/fastapi_tool/demo/__init__.py
+-rw-rw-rw-   0        0        0      408 2023-12-11 07:11:01.000000 afeng-py-tools-0.0.99/src/afeng_tools/fastapi_tool/demo/apps.py
+-rw-rw-rw-   0        0        0      703 2023-12-11 07:11:01.000000 afeng-py-tools-0.0.99/src/afeng_tools/fastapi_tool/demo/main.py
+-rw-rw-rw-   0        0        0     1349 2024-02-03 19:02:10.000000 afeng-py-tools-0.0.99/src/afeng_tools/fastapi_tool/fastapi_auto_tools.py
+-rw-rw-rw-   0        0        0     1503 2023-12-12 05:25:20.000000 afeng-py-tools-0.0.99/src/afeng_tools/fastapi_tool/fastapi_depends_tools.py
+-rw-rw-rw-   0        0        0     2024 2024-02-04 13:14:12.000000 afeng-py-tools-0.0.99/src/afeng_tools/fastapi_tool/fastapi_jinja2_tools.py
+-rw-rw-rw-   0        0        0      635 2024-02-05 06:30:06.000000 afeng-py-tools-0.0.99/src/afeng_tools/fastapi_tool/fastapi_json_tools.py
+-rw-rw-rw-   0        0        0     1294 2023-12-11 11:57:00.000000 afeng-py-tools-0.0.99/src/afeng_tools/fastapi_tool/fastapi_request_tools.py
+-rw-rw-rw-   0        0        0     6742 2024-02-02 22:41:43.000000 afeng-py-tools-0.0.99/src/afeng_tools/fastapi_tool/fastapi_response_tools.py
+-rw-rw-rw-   0        0        0     2532 2024-02-03 19:58:01.000000 afeng-py-tools-0.0.99/src/afeng_tools/fastapi_tool/fastapi_router_tools.py
+-rw-rw-rw-   0        0        0     1209 2023-12-20 08:14:29.000000 afeng-py-tools-0.0.99/src/afeng_tools/fastapi_tool/fastapi_settings.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:31.724933 afeng-py-tools-0.0.99/src/afeng_tools/file_tool/
+-rw-rw-rw-   0        0        0       22 2023-12-06 19:27:38.000000 afeng-py-tools-0.0.99/src/afeng_tools/file_tool/__init__.py
+-rw-rw-rw-   0        0        0     1062 2023-12-06 21:32:01.000000 afeng-py-tools-0.0.99/src/afeng_tools/file_tool/csv_tools.py
+-rw-rw-rw-   0        0        0    12308 2024-02-05 15:54:55.000000 afeng-py-tools-0.0.99/src/afeng_tools/file_tool/file_tools.py
+-rw-rw-rw-   0        0        0     1488 2023-12-06 21:36:49.000000 afeng-py-tools-0.0.99/src/afeng_tools/file_tool/tmp_file_tools.py
+-rw-rw-rw-   0        0        0      316 2023-10-15 15:07:50.000000 afeng-py-tools-0.0.99/src/afeng_tools/file_tool/yaml_tools.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:31.731710 afeng-py-tools-0.0.99/src/afeng_tools/flask_tool/
+-rw-rw-rw-   0        0        0      407 2023-12-07 06:20:25.000000 afeng-py-tools-0.0.99/src/afeng_tools/flask_tool/__init__.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:31.738244 afeng-py-tools-0.0.99/src/afeng_tools/flask_tool/demo/
+-rw-rw-rw-   0        0        0        0 2023-10-16 02:40:14.000000 afeng-py-tools-0.0.99/src/afeng_tools/flask_tool/demo/__init__.py
+-rw-rw-rw-   0        0        0      276 2023-10-16 02:40:23.000000 afeng-py-tools-0.0.99/src/afeng_tools/flask_tool/demo/apps.py
+-rw-rw-rw-   0        0        0      437 2023-10-16 02:36:06.000000 afeng-py-tools-0.0.99/src/afeng_tools/flask_tool/demo/urls.py
+-rw-rw-rw-   0        0        0     1568 2023-12-07 06:19:17.000000 afeng-py-tools-0.0.99/src/afeng_tools/flask_tool/flask_app_tools.py
+-rw-rw-rw-   0        0        0      201 2023-10-16 02:31:42.000000 afeng-py-tools-0.0.99/src/afeng_tools/flask_tool/flask_models.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:31.741550 afeng-py-tools-0.0.99/src/afeng_tools/generic_tool/
+-rw-rw-rw-   0        0        0       22 2023-12-06 19:26:14.000000 afeng-py-tools-0.0.99/src/afeng_tools/generic_tool/__init__.py
+-rw-rw-rw-   0        0        0      607 2023-12-06 19:26:49.000000 afeng-py-tools-0.0.99/src/afeng_tools/generic_tool/generic_tools.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:31.762567 afeng-py-tools-0.0.99/src/afeng_tools/http_tool/
+-rw-rw-rw-   0        0        0        0 2023-09-08 02:46:02.000000 afeng-py-tools-0.0.99/src/afeng_tools/http_tool/__init__.py
+-rw-rw-rw-   0        0        0      725 2023-12-07 06:04:30.000000 afeng-py-tools-0.0.99/src/afeng_tools/http_tool/aria2c_download_tools.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:31.770344 afeng-py-tools-0.0.99/src/afeng_tools/http_tool/decorator/
+-rw-rw-rw-   0        0        0       23 2023-09-10 15:02:56.000000 afeng-py-tools-0.0.99/src/afeng_tools/http_tool/decorator/__init__.py
+-rw-rw-rw-   0        0        0     1149 2023-12-07 06:04:30.000000 afeng-py-tools-0.0.99/src/afeng_tools/http_tool/decorator/http_auto_retry_tools.py
+-rw-rw-rw-   0        0        0     6133 2023-12-08 07:20:45.000000 afeng-py-tools-0.0.99/src/afeng_tools/http_tool/http_download_tools.py
+-rw-rw-rw-   0        0        0      505 2024-01-15 15:31:26.000000 afeng-py-tools-0.0.99/src/afeng_tools/http_tool/http_enums.py
+-rw-rw-rw-   0        0        0      375 2023-10-20 07:28:35.000000 afeng-py-tools-0.0.99/src/afeng_tools/http_tool/http_html_tools.py
+-rw-rw-rw-   0        0        0      259 2023-08-31 03:43:08.000000 afeng-py-tools-0.0.99/src/afeng_tools/http_tool/http_mimetype_tools.py
+-rw-rw-rw-   0        0        0      327 2023-10-02 04:43:59.000000 afeng-py-tools-0.0.99/src/afeng_tools/http_tool/http_params_tools.py
+-rw-rw-rw-   0        0        0     1609 2023-12-07 06:07:33.000000 afeng-py-tools-0.0.99/src/afeng_tools/http_tool/http_tools.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:31.782808 afeng-py-tools-0.0.99/src/afeng_tools/http_tool/httpx/
+-rw-rw-rw-   0        0        0        0 2023-09-08 03:23:18.000000 afeng-py-tools-0.0.99/src/afeng_tools/http_tool/httpx/__init__.py
+-rw-rw-rw-   0        0        0      654 2023-12-07 06:07:51.000000 afeng-py-tools-0.0.99/src/afeng_tools/http_tool/httpx/async_http.py
+-rw-rw-rw-   0        0        0      679 2023-01-20 11:38:01.000000 afeng-py-tools-0.0.99/src/afeng_tools/http_tool/httpx/sync_http.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:31.790513 afeng-py-tools-0.0.99/src/afeng_tools/id_code_tool/
+-rw-rw-rw-   0        0        0       27 2023-12-06 19:28:37.000000 afeng-py-tools-0.0.99/src/afeng_tools/id_code_tool/__init__.py
+-rw-rw-rw-   0        0        0      466 2023-12-27 09:12:18.000000 afeng-py-tools-0.0.99/src/afeng_tools/id_code_tool/id_code_tools.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:31.802190 afeng-py-tools-0.0.99/src/afeng_tools/image_tool/
+-rw-rw-rw-   0        0        0        0 2023-10-28 15:52:08.000000 afeng-py-tools-0.0.99/src/afeng_tools/image_tool/__init__.py
+-rw-rw-rw-   0        0        0     1045 2023-12-07 06:17:36.000000 afeng-py-tools-0.0.99/src/afeng_tools/image_tool/image_base64_tools.py
+-rw-rw-rw-   0        0        0      155 2023-12-28 16:39:19.000000 afeng-py-tools-0.0.99/src/afeng_tools/image_tool/image_watermark_tools.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:31.807762 afeng-py-tools-0.0.99/src/afeng_tools/import_tool/
+-rw-rw-rw-   0        0        0       28 2023-12-06 19:29:56.000000 afeng-py-tools-0.0.99/src/afeng_tools/import_tool/__init__.py
+-rw-rw-rw-   0        0        0      703 2023-12-06 19:30:40.000000 afeng-py-tools-0.0.99/src/afeng_tools/import_tool/import_tools.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:31.812244 afeng-py-tools-0.0.99/src/afeng_tools/javascript_tool/
+-rw-rw-rw-   0        0        0        0 2023-09-13 01:05:07.000000 afeng-py-tools-0.0.99/src/afeng_tools/javascript_tool/__init__.py
+-rw-rw-rw-   0        0        0     1255 2023-12-07 06:34:23.000000 afeng-py-tools-0.0.99/src/afeng_tools/javascript_tool/javascript_tools.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:31.822283 afeng-py-tools-0.0.99/src/afeng_tools/jinja2_tool/
+-rw-rw-rw-   0        0        0        0 2023-09-27 00:07:32.000000 afeng-py-tools-0.0.99/src/afeng_tools/jinja2_tool/__init__.py
+-rw-rw-rw-   0        0        0      591 2023-12-07 06:31:20.000000 afeng-py-tools-0.0.99/src/afeng_tools/jinja2_tool/jinja2_decorator_tools.py
+-rw-rw-rw-   0        0        0      999 2023-12-07 06:31:20.000000 afeng-py-tools-0.0.99/src/afeng_tools/jinja2_tool/jinja2_filters.py
+-rw-rw-rw-   0        0        0     1729 2023-12-07 06:31:38.000000 afeng-py-tools-0.0.99/src/afeng_tools/jinja2_tool/jinja2_tools.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:31.829045 afeng-py-tools-0.0.99/src/afeng_tools/json_tool/
+-rw-rw-rw-   0        0        0       20 2023-12-06 19:31:29.000000 afeng-py-tools-0.0.99/src/afeng_tools/json_tool/__init__.py
+-rw-rw-rw-   0        0        0     2308 2023-12-11 08:20:44.000000 afeng-py-tools-0.0.99/src/afeng_tools/json_tool/json_tools.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:31.836955 afeng-py-tools-0.0.99/src/afeng_tools/layui_tool/
+-rw-rw-rw-   0        0        0      160 2023-12-07 06:33:01.000000 afeng-py-tools-0.0.99/src/afeng_tools/layui_tool/__init__.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:31.844991 afeng-py-tools-0.0.99/src/afeng_tools/layui_tool/core/
+-rw-rw-rw-   0        0        0        0 2023-11-23 22:49:49.000000 afeng-py-tools-0.0.99/src/afeng_tools/layui_tool/core/__init__.py
+-rw-rw-rw-   0        0        0     3343 2023-12-12 07:31:42.000000 afeng-py-tools-0.0.99/src/afeng_tools/layui_tool/core/layui_models.py
+-rw-rw-rw-   0        0        0     5254 2023-12-07 06:33:01.000000 afeng-py-tools-0.0.99/src/afeng_tools/layui_tool/layui_template_tools.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:31.301790 afeng-py-tools-0.0.99/src/afeng_tools/layui_tool/template/
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:31.848310 afeng-py-tools-0.0.99/src/afeng_tools/layui_tool/template/form/
+-rw-rw-rw-   0        0        0    17518 2023-11-29 06:33:34.000000 afeng-py-tools-0.0.99/src/afeng_tools/layui_tool/template/form/step_form.html
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:31.862925 afeng-py-tools-0.0.99/src/afeng_tools/layui_tool/template/table/
+-rw-rw-rw-   0        0        0    13217 2023-12-01 00:51:05.000000 afeng-py-tools-0.0.99/src/afeng_tools/layui_tool/template/table/add.html
+-rw-rw-rw-   0        0        0    13387 2023-12-01 00:51:10.000000 afeng-py-tools-0.0.99/src/afeng_tools/layui_tool/template/table/edit.html
+-rw-rw-rw-   0        0        0    11537 2023-12-12 07:33:26.000000 afeng-py-tools-0.0.99/src/afeng_tools/layui_tool/template/table/list.html
+-rw-rw-rw-   0        0        0     5513 2023-12-01 00:50:37.000000 afeng-py-tools-0.0.99/src/afeng_tools/layui_tool/template/table/show.html
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:31.869568 afeng-py-tools-0.0.99/src/afeng_tools/linux_tool/
+-rw-rw-rw-   0        0        0       30 2023-12-06 19:28:07.000000 afeng-py-tools-0.0.99/src/afeng_tools/linux_tool/__init__.py
+-rw-rw-rw-   0        0        0      811 2023-09-27 01:17:04.000000 afeng-py-tools-0.0.99/src/afeng_tools/linux_tool/linux_match_tools.py
+-rw-rw-rw-   0        0        0      556 2024-01-31 23:35:13.000000 afeng-py-tools-0.0.99/src/afeng_tools/linux_tool/sh_tools.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:31.881949 afeng-py-tools-0.0.99/src/afeng_tools/log_tool/
+-rw-rw-rw-   0        0        0        0 2023-12-06 22:51:06.000000 afeng-py-tools-0.0.99/src/afeng_tools/log_tool/__init__.py
+-rw-rw-rw-   0        0        0      221 2023-12-06 23:00:18.000000 afeng-py-tools-0.0.99/src/afeng_tools/log_tool/logger_enums.py
+-rw-rw-rw-   0        0        0      776 2023-12-08 06:33:33.000000 afeng-py-tools-0.0.99/src/afeng_tools/log_tool/logger_settings.py
+-rw-rw-rw-   0        0        0     1036 2023-12-06 23:00:35.000000 afeng-py-tools-0.0.99/src/afeng_tools/log_tool/logging_tools.py
+-rw-rw-rw-   0        0        0     1016 2023-12-08 00:27:19.000000 afeng-py-tools-0.0.99/src/afeng_tools/log_tool/loguru_tools.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:31.888720 afeng-py-tools-0.0.99/src/afeng_tools/math_tool/
+-rw-rw-rw-   0        0        0       22 2023-12-06 21:21:05.000000 afeng-py-tools-0.0.99/src/afeng_tools/math_tool/__init__.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:31.893119 afeng-py-tools-0.0.99/src/afeng_tools/math_tool/core/
+-rw-rw-rw-   0        0        0        0 2023-12-24 00:27:13.000000 afeng-py-tools-0.0.99/src/afeng_tools/math_tool/core/__init__.py
+-rw-rw-rw-   0        0        0     3291 2023-12-24 01:00:22.000000 afeng-py-tools-0.0.99/src/afeng_tools/math_tool/core/number_to_chinese.py
+-rw-rw-rw-   0        0        0      450 2023-12-24 00:46:29.000000 afeng-py-tools-0.0.99/src/afeng_tools/math_tool/number_tools.py
+-rw-rw-rw-   0        0        0      897 2023-12-07 09:27:40.000000 afeng-py-tools-0.0.99/src/afeng_tools/math_tool/random_tools.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:31.900840 afeng-py-tools-0.0.99/src/afeng_tools/os_tool/
+-rw-rw-rw-   0        0        0       18 2023-12-06 19:33:22.000000 afeng-py-tools-0.0.99/src/afeng_tools/os_tool/__init__.py
+-rw-rw-rw-   0        0        0      711 2023-12-06 19:34:05.000000 afeng-py-tools-0.0.99/src/afeng_tools/os_tool/os_platform_tools.py
+-rw-rw-rw-   0        0        0      134 2023-12-08 07:01:16.000000 afeng-py-tools-0.0.99/src/afeng_tools/os_tool/os_tools.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:31.905478 afeng-py-tools-0.0.99/src/afeng_tools/pandas_tool/
+-rw-rw-rw-   0        0        0        0 2023-09-07 10:17:43.000000 afeng-py-tools-0.0.99/src/afeng_tools/pandas_tool/__init__.py
+-rw-rw-rw-   0        0        0      890 2023-12-07 06:12:11.000000 afeng-py-tools-0.0.99/src/afeng_tools/pandas_tool/pandas_tools.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:31.926672 afeng-py-tools-0.0.99/src/afeng_tools/playwright_tool/
+-rw-rw-rw-   0        0        0      106 2023-09-25 00:06:07.000000 afeng-py-tools-0.0.99/src/afeng_tools/playwright_tool/__init__.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:31.935748 afeng-py-tools-0.0.99/src/afeng_tools/playwright_tool/decorator/
+-rw-rw-rw-   0        0        0       41 2023-09-08 17:53:07.000000 afeng-py-tools-0.0.99/src/afeng_tools/playwright_tool/decorator/__init__.py
+-rw-rw-rw-   0        0        0     2101 2023-12-11 07:11:01.000000 afeng-py-tools-0.0.99/src/afeng_tools/playwright_tool/decorator/playwright_async_decorators.py
+-rw-rw-rw-   0        0        0     2333 2023-12-11 07:11:01.000000 afeng-py-tools-0.0.99/src/afeng_tools/playwright_tool/decorator/playwright_decorators.py
+-rw-rw-rw-   0        0        0     1942 2023-12-07 06:04:30.000000 afeng-py-tools-0.0.99/src/afeng_tools/playwright_tool/http_cookie_tools.py
+-rw-rw-rw-   0        0        0     1549 2023-12-07 06:04:30.000000 afeng-py-tools-0.0.99/src/afeng_tools/playwright_tool/http_header_tools.py
+-rw-rw-rw-   0        0        0     1275 2023-12-07 06:04:47.000000 afeng-py-tools-0.0.99/src/afeng_tools/playwright_tool/http_storage_tools.py
+-rw-rw-rw-   0        0        0     2008 2023-12-07 06:07:26.000000 afeng-py-tools-0.0.99/src/afeng_tools/playwright_tool/playwright_tools.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:31.942593 afeng-py-tools-0.0.99/src/afeng_tools/playwright_tool/spider/
+-rw-rw-rw-   0        0        0        0 2023-12-20 06:49:24.000000 afeng-py-tools-0.0.99/src/afeng_tools/playwright_tool/spider/__init__.py
+-rw-rw-rw-   0        0        0     2775 2023-12-21 05:01:06.000000 afeng-py-tools-0.0.99/src/afeng_tools/playwright_tool/spider/base_spider.py
+-rw-rw-rw-   0        0        0      926 2023-12-07 06:07:26.000000 afeng-py-tools-0.0.99/src/afeng_tools/playwright_tool/test001.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:31.949262 afeng-py-tools-0.0.99/src/afeng_tools/pydantic_tool/
+-rw-rw-rw-   0        0        0        0 2023-10-22 09:32:57.000000 afeng-py-tools-0.0.99/src/afeng_tools/pydantic_tool/__init__.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:31.957522 afeng-py-tools-0.0.99/src/afeng_tools/pydantic_tool/model/
+-rw-rw-rw-   0        0        0        0 2023-12-11 07:42:54.000000 afeng-py-tools-0.0.99/src/afeng_tools/pydantic_tool/model/__init__.py
+-rw-rw-rw-   0        0        0     1010 2024-02-04 16:33:50.000000 afeng-py-tools-0.0.99/src/afeng_tools/pydantic_tool/model/common_models.py
+-rw-rw-rw-   0        0        0     1595 2023-12-25 06:27:58.000000 afeng-py-tools-0.0.99/src/afeng_tools/pydantic_tool/pydantic_tools.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:31.964123 afeng-py-tools-0.0.99/src/afeng_tools/python_tool/
+-rw-rw-rw-   0        0        0        0 2023-12-24 11:47:52.000000 afeng-py-tools-0.0.99/src/afeng_tools/python_tool/__init__.py
+-rw-rw-rw-   0        0        0     2525 2023-12-24 12:08:53.000000 afeng-py-tools-0.0.99/src/afeng_tools/python_tool/dict_tools.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:31.977785 afeng-py-tools-0.0.99/src/afeng_tools/qrcode_tool/
+-rw-rw-rw-   0        0        0        0 2023-11-10 20:49:35.000000 afeng-py-tools-0.0.99/src/afeng_tools/qrcode_tool/__init__.py
+-rw-rw-rw-   0        0        0      707 2023-12-07 05:59:34.000000 afeng-py-tools-0.0.99/src/afeng_tools/qrcode_tool/qrcode_demo.py
+-rw-rw-rw-   0        0        0     2860 2023-12-07 05:58:58.000000 afeng-py-tools-0.0.99/src/afeng_tools/qrcode_tool/qrcode_image_tools.py
+-rw-rw-rw-   0        0        0     3258 2023-11-10 21:01:34.000000 afeng-py-tools-0.0.99/src/afeng_tools/qrcode_tool/qrcode_tools.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:31.983451 afeng-py-tools-0.0.99/src/afeng_tools/re_tool/
+-rw-rw-rw-   0        0        0       22 2023-12-06 21:21:53.000000 afeng-py-tools-0.0.99/src/afeng_tools/re_tool/__init__.py
+-rw-rw-rw-   0        0        0     1411 2023-12-06 21:23:39.000000 afeng-py-tools-0.0.99/src/afeng_tools/re_tool/re_tools.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:31.996828 afeng-py-tools-0.0.99/src/afeng_tools/scrapy_tool/
+-rw-rw-rw-   0        0        0        0 2024-01-15 12:55:42.000000 afeng-py-tools-0.0.99/src/afeng_tools/scrapy_tool/__init__.py
+-rw-rw-rw-   0        0        0     1186 2024-02-05 16:06:55.000000 afeng-py-tools-0.0.99/src/afeng_tools/scrapy_tool/scrapy_request_tools.py
+-rw-rw-rw-   0        0        0     1721 2024-01-29 04:26:00.000000 afeng-py-tools-0.0.99/src/afeng_tools/scrapy_tool/scrapy_run_tools.py
+-rw-rw-rw-   0        0        0      992 2024-02-05 04:52:37.000000 afeng-py-tools-0.0.99/src/afeng_tools/scrapy_tool/scrapy_selector_tools.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:32.008094 afeng-py-tools-0.0.99/src/afeng_tools/scrapy_tool/scrapy_wiki/
+-rw-rw-rw-   0        0        0        0 2024-02-05 18:33:35.000000 afeng-py-tools-0.0.99/src/afeng_tools/scrapy_tool/scrapy_wiki/__init__.py
+-rw-rw-rw-   0        0        0     1025 2024-02-05 18:04:30.000000 afeng-py-tools-0.0.99/src/afeng_tools/scrapy_tool/scrapy_wiki/spider_wiki_items.py
+-rw-rw-rw-   0        0        0     2236 2024-02-05 18:36:34.000000 afeng-py-tools-0.0.99/src/afeng_tools/scrapy_tool/scrapy_wiki/spider_wiki_tools.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:32.014993 afeng-py-tools-0.0.99/src/afeng_tools/serialization_tool/
+-rw-rw-rw-   0        0        0       34 2023-12-06 21:18:45.000000 afeng-py-tools-0.0.99/src/afeng_tools/serialization_tool/__init__.py
+-rw-rw-rw-   0        0        0      577 2023-12-06 21:19:25.000000 afeng-py-tools-0.0.99/src/afeng_tools/serialization_tool/pickle_tools.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:32.028205 afeng-py-tools-0.0.99/src/afeng_tools/sqlalchemy_tool/
+-rw-rw-rw-   0        0        0      194 2023-12-24 06:26:30.000000 afeng-py-tools-0.0.99/src/afeng_tools/sqlalchemy_tool/__init__.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:32.062521 afeng-py-tools-0.0.99/src/afeng_tools/sqlalchemy_tool/core/
+-rw-rw-rw-   0        0        0       32 2023-12-06 22:34:44.000000 afeng-py-tools-0.0.99/src/afeng_tools/sqlalchemy_tool/core/__init__.py
+-rw-rw-rw-   0        0        0     5051 2023-12-08 06:39:50.000000 afeng-py-tools-0.0.99/src/afeng_tools/sqlalchemy_tool/core/orm_model_tools.py
+-rw-rw-rw-   0        0        0      752 2023-12-06 22:48:04.000000 afeng-py-tools-0.0.99/src/afeng_tools/sqlalchemy_tool/core/sqlalchemy_base_model.py
+-rw-rw-rw-   0        0        0     1713 2023-12-06 22:44:38.000000 afeng-py-tools-0.0.99/src/afeng_tools/sqlalchemy_tool/core/sqlalchemy_db_tools.py
+-rw-rw-rw-   0        0        0      120 2023-12-07 02:08:00.000000 afeng-py-tools-0.0.99/src/afeng_tools/sqlalchemy_tool/core/sqlalchemy_enums.py
+-rw-rw-rw-   0        0        0      518 2023-12-07 02:04:04.000000 afeng-py-tools-0.0.99/src/afeng_tools/sqlalchemy_tool/core/sqlalchemy_item.py
+-rw-rw-rw-   0        0        0     2603 2023-12-07 01:24:48.000000 afeng-py-tools-0.0.99/src/afeng_tools/sqlalchemy_tool/core/sqlalchemy_meta_class.py
+-rw-rw-rw-   0        0        0     1866 2023-12-09 05:14:18.000000 afeng-py-tools-0.0.99/src/afeng_tools/sqlalchemy_tool/core/sqlalchemy_model_utils.py
+-rw-rw-rw-   0        0        0     2924 2023-12-07 04:12:13.000000 afeng-py-tools-0.0.99/src/afeng_tools/sqlalchemy_tool/core/sqlalchemy_session_decorator.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:32.084730 afeng-py-tools-0.0.99/src/afeng_tools/sqlalchemy_tool/crdu/
+-rw-rw-rw-   0        0        0       38 2023-12-06 22:49:26.000000 afeng-py-tools-0.0.99/src/afeng_tools/sqlalchemy_tool/crdu/__init__.py
+-rw-rw-rw-   0        0        0     7449 2023-12-11 23:22:06.000000 afeng-py-tools-0.0.99/src/afeng_tools/sqlalchemy_tool/crdu/base_crdu.py
+-rw-rw-rw-   0        0        0      291 2023-09-07 20:22:22.000000 afeng-py-tools-0.0.99/src/afeng_tools/sqlalchemy_tool/crdu/ddl_crdu.py
+-rw-rw-rw-   0        0        0     1429 2023-12-22 23:33:25.000000 afeng-py-tools-0.0.99/src/afeng_tools/sqlalchemy_tool/crdu/sequence_crdu.py
+-rw-rw-rw-   0        0        0     6552 2023-12-08 06:39:50.000000 afeng-py-tools-0.0.99/src/afeng_tools/sqlalchemy_tool/crdu/session_crdu.py
+-rw-rw-rw-   0        0        0      781 2023-12-07 05:53:31.000000 afeng-py-tools-0.0.99/src/afeng_tools/sqlalchemy_tool/crdu/sql_crdu.py
+-rw-rw-rw-   0        0        0     4129 2023-12-09 19:18:50.000000 afeng-py-tools-0.0.99/src/afeng_tools/sqlalchemy_tool/sqlalchemy_db_copy_tools.py
+-rw-rw-rw-   0        0        0     1038 2023-12-07 23:21:41.000000 afeng-py-tools-0.0.99/src/afeng_tools/sqlalchemy_tool/sqlalchemy_settings.py
+-rw-rw-rw-   0        0        0     1815 2023-12-07 05:51:24.000000 afeng-py-tools-0.0.99/src/afeng_tools/sqlalchemy_tool/sqlalchemy_tools.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:32.097637 afeng-py-tools-0.0.99/src/afeng_tools/sqlalchemy_tools/
+-rw-rw-rw-   0        0        0      100 2023-12-24 04:50:28.000000 afeng-py-tools-0.0.99/src/afeng_tools/sqlalchemy_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:32.113310 afeng-py-tools-0.0.99/src/afeng_tools/sqlalchemy_tools/core/
+-rw-rw-rw-   0        0        0        0 2023-12-24 04:56:52.000000 afeng-py-tools-0.0.99/src/afeng_tools/sqlalchemy_tools/core/__init__.py
+-rw-rw-rw-   0        0        0     1303 2023-12-25 11:20:50.000000 afeng-py-tools-0.0.99/src/afeng_tools/sqlalchemy_tools/core/sqlalchemy_base_model.py
+-rw-rw-rw-   0        0        0     1466 2023-12-24 05:36:20.000000 afeng-py-tools-0.0.99/src/afeng_tools/sqlalchemy_tools/core/sqlalchemy_class.py
+-rw-rw-rw-   0        0        0      120 2023-12-07 02:08:00.000000 afeng-py-tools-0.0.99/src/afeng_tools/sqlalchemy_tools/core/sqlalchemy_enums.py
+-rw-rw-rw-   0        0        0      702 2023-12-24 05:06:32.000000 afeng-py-tools-0.0.99/src/afeng_tools/sqlalchemy_tools/core/sqlalchemy_items.py
+-rw-rw-rw-   0        0        0     2950 2024-01-19 19:04:33.000000 afeng-py-tools-0.0.99/src/afeng_tools/sqlalchemy_tools/core/sqlalchemy_meta_class.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:32.128876 afeng-py-tools-0.0.99/src/afeng_tools/sqlalchemy_tools/crdu/
+-rw-rw-rw-   0        0        0       38 2023-12-24 06:02:01.000000 afeng-py-tools-0.0.99/src/afeng_tools/sqlalchemy_tools/crdu/__init__.py
+-rw-rw-rw-   0        0        0     7303 2023-12-24 06:18:59.000000 afeng-py-tools-0.0.99/src/afeng_tools/sqlalchemy_tools/crdu/base_crdu.py
+-rw-rw-rw-   0        0        0     1471 2023-12-24 06:20:31.000000 afeng-py-tools-0.0.99/src/afeng_tools/sqlalchemy_tools/crdu/sequence_crdu.py
+-rw-rw-rw-   0        0        0     6447 2023-12-24 06:20:31.000000 afeng-py-tools-0.0.99/src/afeng_tools/sqlalchemy_tools/crdu/session_crdu.py
+-rw-rw-rw-   0        0        0      511 2023-12-24 06:23:34.000000 afeng-py-tools-0.0.99/src/afeng_tools/sqlalchemy_tools/crdu/sql_crdu.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:32.133394 afeng-py-tools-0.0.99/src/afeng_tools/sqlalchemy_tools/decorator/
+-rw-rw-rw-   0        0        0       29 2023-12-24 06:02:12.000000 afeng-py-tools-0.0.99/src/afeng_tools/sqlalchemy_tools/decorator/__init__.py
+-rw-rw-rw-   0        0        0     4135 2023-12-24 09:36:16.000000 afeng-py-tools-0.0.99/src/afeng_tools/sqlalchemy_tools/decorator/sqlalchemy_session_decorator.py
+-rw-rw-rw-   0        0        0     4170 2023-12-24 06:23:34.000000 afeng-py-tools-0.0.99/src/afeng_tools/sqlalchemy_tools/sqlalchemy_db_copy_tools.py
+-rw-rw-rw-   0        0        0     1016 2023-12-24 05:27:18.000000 afeng-py-tools-0.0.99/src/afeng_tools/sqlalchemy_tools/sqlalchemy_settings.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:32.140050 afeng-py-tools-0.0.99/src/afeng_tools/sqlalchemy_tools/tool/
+-rw-rw-rw-   0        0        0        0 2023-12-24 05:57:19.000000 afeng-py-tools-0.0.99/src/afeng_tools/sqlalchemy_tools/tool/__init__.py
+-rw-rw-rw-   0        0        0     4961 2023-12-24 05:58:06.000000 afeng-py-tools-0.0.99/src/afeng_tools/sqlalchemy_tools/tool/orm_model_tools.py
+-rw-rw-rw-   0        0        0     1785 2023-12-24 06:18:59.000000 afeng-py-tools-0.0.99/src/afeng_tools/sqlalchemy_tools/tool/sqlalchemy_model_tools.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:32.154563 afeng-py-tools-0.0.99/src/afeng_tools/template_tool/
+-rw-rw-rw-   0        0        0     1866 2023-12-11 07:11:01.000000 afeng-py-tools-0.0.99/src/afeng_tools/template_tool/README.md
+-rw-rw-rw-   0        0        0       24 2023-12-08 09:44:41.000000 afeng-py-tools-0.0.99/src/afeng_tools/template_tool/__init__.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:32.172182 afeng-py-tools-0.0.99/src/afeng_tools/template_tool/core/
+-rw-rw-rw-   0        0        0        0 2023-12-07 23:23:10.000000 afeng-py-tools-0.0.99/src/afeng_tools/template_tool/core/__init__.py
+-rw-rw-rw-   0        0        0     1866 2023-12-09 03:01:10.000000 afeng-py-tools-0.0.99/src/afeng_tools/template_tool/core/calmjs_tools.py
+-rw-rw-rw-   0        0        0      410 2023-12-09 03:01:06.000000 afeng-py-tools-0.0.99/src/afeng_tools/template_tool/core/html_tools.py
+-rw-rw-rw-   0        0        0     1227 2023-12-09 03:01:02.000000 afeng-py-tools-0.0.99/src/afeng_tools/template_tool/core/js_tools.py
+-rw-rw-rw-   0        0        0      824 2023-12-06 15:29:51.000000 afeng-py-tools-0.0.99/src/afeng_tools/template_tool/core/less_tools.py
+-rw-rw-rw-   0        0        0      318 2023-12-09 03:01:16.000000 afeng-py-tools-0.0.99/src/afeng_tools/template_tool/core/scss_tools.py
+-rw-rw-rw-   0        0        0     1120 2023-12-09 03:01:22.000000 afeng-py-tools-0.0.99/src/afeng_tools/template_tool/core/vue_tools.py
+-rw-rw-rw-   0        0        0     5517 2023-12-07 06:27:14.000000 afeng-py-tools-0.0.99/src/afeng_tools/template_tool/template_auto_tools.py
+-rw-rw-rw-   0        0        0      597 2023-12-07 06:27:14.000000 afeng-py-tools-0.0.99/src/afeng_tools/template_tool/template_decorator_tools.py
+-rw-rw-rw-   0        0        0     4639 2023-12-08 09:44:57.000000 afeng-py-tools-0.0.99/src/afeng_tools/template_tool/template_tools.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:32.174366 afeng-py-tools-0.0.99/src/afeng_tools/template_tool/vue_demo/
+-rw-rw-rw-   0        0        0     1208 2023-12-06 17:02:58.000000 afeng-py-tools-0.0.99/src/afeng_tools/template_tool/vue_demo/python_component.vue
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:32.181382 afeng-py-tools-0.0.99/src/afeng_tools/text_tool/
+-rw-rw-rw-   0        0        0       22 2023-12-06 21:38:05.000000 afeng-py-tools-0.0.99/src/afeng_tools/text_tool/__init__.py
+-rw-rw-rw-   0        0        0     2117 2023-08-26 09:17:28.000000 afeng-py-tools-0.0.99/src/afeng_tools/text_tool/article_split_tools.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:32.188006 afeng-py-tools-0.0.99/src/afeng_tools/text_tool/word_break_tool/
+-rw-rw-rw-   0        0        0       22 2023-12-06 21:38:24.000000 afeng-py-tools-0.0.99/src/afeng_tools/text_tool/word_break_tool/__init__.py
+-rw-rw-rw-   0        0        0     1284 2023-11-23 09:36:58.000000 afeng-py-tools-0.0.99/src/afeng_tools/text_tool/word_break_tool/jieba_tools.py
+-rw-rw-rw-   0        0        0      305 2023-12-06 21:38:37.000000 afeng-py-tools-0.0.99/src/afeng_tools/text_tool/word_break_tool/word_break_tools.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:32.191376 afeng-py-tools-0.0.99/src/afeng_tools/trade_tool/
+-rw-rw-rw-   0        0        0        0 2023-09-12 16:53:42.000000 afeng-py-tools-0.0.99/src/afeng_tools/trade_tool/__init__.py
+-rw-rw-rw-   0        0        0     1559 2023-12-07 06:15:44.000000 afeng-py-tools-0.0.99/src/afeng_tools/trade_tool/trade_calendar_tools.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:32.195801 afeng-py-tools-0.0.99/src/afeng_tools/tushare_tool/
+-rw-rw-rw-   0        0        0       29 2023-12-07 06:16:15.000000 afeng-py-tools-0.0.99/src/afeng_tools/tushare_tool/__init__.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:32.200168 afeng-py-tools-0.0.99/src/afeng_tools/tushare_tool/sh_sz_stock/
+-rw-rw-rw-   0        0        0        0 2023-09-08 00:16:18.000000 afeng-py-tools-0.0.99/src/afeng_tools/tushare_tool/sh_sz_stock/__init__.py
+-rw-rw-rw-   0        0        0     1123 2023-12-07 06:13:43.000000 afeng-py-tools-0.0.99/src/afeng_tools/tushare_tool/sh_sz_stock/stock_basic_tools.py
+-rw-rw-rw-   0        0        0      149 2023-12-07 06:16:15.000000 afeng-py-tools-0.0.99/src/afeng_tools/tushare_tool/tushare_tools.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:32.206851 afeng-py-tools-0.0.99/src/afeng_tools/web_tool/
+-rw-rw-rw-   0        0        0       22 2023-12-06 21:20:21.000000 afeng-py-tools-0.0.99/src/afeng_tools/web_tool/__init__.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:32.211377 afeng-py-tools-0.0.99/src/afeng_tools/web_tool/core/
+-rw-rw-rw-   0        0        0        0 2023-12-10 21:21:46.000000 afeng-py-tools-0.0.99/src/afeng_tools/web_tool/core/__init__.py
+-rw-rw-rw-   0        0        0      203 2023-12-10 21:24:06.000000 afeng-py-tools-0.0.99/src/afeng_tools/web_tool/core/web_common_models.py
+-rw-rw-rw-   0        0        0      877 2023-12-06 21:41:14.000000 afeng-py-tools-0.0.99/src/afeng_tools/web_tool/request_tools.py
+-rw-rw-rw-   0        0        0     1442 2023-12-25 06:43:59.000000 afeng-py-tools-0.0.99/src/afeng_tools/web_tool/response_tools.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:32.221173 afeng-py-tools-0.0.99/src/afeng_tools/weixin_min_program/
+-rw-rw-rw-   0        0        0        0 2023-12-10 12:27:13.000000 afeng-py-tools-0.0.99/src/afeng_tools/weixin_min_program/__init__.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:32.233548 afeng-py-tools-0.0.99/src/afeng_tools/weixin_min_program/core/
+-rw-rw-rw-   0        0        0        0 2023-12-10 12:34:44.000000 afeng-py-tools-0.0.99/src/afeng_tools/weixin_min_program/core/__init__.py
+-rw-rw-rw-   0        0        0     4099 2023-12-16 06:42:03.000000 afeng-py-tools-0.0.99/src/afeng_tools/weixin_min_program/core/weixin_mp_api_service.py
+-rw-rw-rw-   0        0        0     1158 2023-12-10 22:29:12.000000 afeng-py-tools-0.0.99/src/afeng_tools/weixin_min_program/core/weixin_mp_decrypt.py
+-rw-rw-rw-   0        0        0     2063 2023-12-16 10:03:08.000000 afeng-py-tools-0.0.99/src/afeng_tools/weixin_min_program/core/weixin_mp_models.py
+-rw-rw-rw-   0        0        0     4311 2023-12-16 09:50:07.000000 afeng-py-tools-0.0.99/src/afeng_tools/weixin_min_program/core/weixin_mp_service.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:32.241222 afeng-py-tools-0.0.99/src/afeng_tools/weixin_min_program/model/
+-rw-rw-rw-   0        0        0        0 2023-12-10 12:27:13.000000 afeng-py-tools-0.0.99/src/afeng_tools/weixin_min_program/model/__init__.py
+-rw-rw-rw-   0        0        0     1503 2023-12-16 09:48:30.000000 afeng-py-tools-0.0.99/src/afeng_tools/weixin_min_program/model/weixin_mp_enums.py
+-rw-rw-rw-   0        0        0     1090 2023-12-16 09:49:29.000000 afeng-py-tools-0.0.99/src/afeng_tools/weixin_min_program/model/weixin_mp_open_models.py
+-rw-rw-rw-   0        0        0     1544 2023-12-16 09:46:54.000000 afeng-py-tools-0.0.99/src/afeng_tools/weixin_min_program/weixin_mp_settings.py
+-rw-rw-rw-   0        0        0     1407 2023-12-16 02:29:14.000000 afeng-py-tools-0.0.99/src/afeng_tools/weixin_min_program/weixin_mp_tools.py
+-rw-rw-rw-   0        0        0     1459 2023-12-16 10:02:58.000000 afeng-py-tools-0.0.99/src/afeng_tools/weixin_min_program/weixin_mp_views.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:32.247871 afeng-py-tools-0.0.99/src/afeng_tools/weixin_tool/
+-rw-rw-rw-   0        0        0      196 2023-12-06 21:47:34.000000 afeng-py-tools-0.0.99/src/afeng_tools/weixin_tool/__init__.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:32.260308 afeng-py-tools-0.0.99/src/afeng_tools/weixin_tool/core/
+-rw-rw-rw-   0        0        0        0 2023-11-14 21:09:25.000000 afeng-py-tools-0.0.99/src/afeng_tools/weixin_tool/core/__init__.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:32.264687 afeng-py-tools-0.0.99/src/afeng_tools/weixin_tool/core/format/
+-rw-rw-rw-   0        0        0       25 2023-12-06 21:52:19.000000 afeng-py-tools-0.0.99/src/afeng_tools/weixin_tool/core/format/__init__.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:32.271556 afeng-py-tools-0.0.99/src/afeng_tools/weixin_tool/core/format/reply_msg/
+-rw-rw-rw-   0        0        0       28 2023-12-06 21:46:21.000000 afeng-py-tools-0.0.99/src/afeng_tools/weixin_tool/core/format/reply_msg/__init__.py
+-rw-rw-rw-   0        0        0      301 2023-11-15 02:51:53.000000 afeng-py-tools-0.0.99/src/afeng_tools/weixin_tool/core/format/reply_msg/weixin_format_tool.py
+-rw-rw-rw-   0        0        0     3239 2023-11-15 02:55:54.000000 afeng-py-tools-0.0.99/src/afeng_tools/weixin_tool/core/format/reply_msg/weixin_models.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:32.289517 afeng-py-tools-0.0.99/src/afeng_tools/weixin_tool/core/format/reply_msg/xml/
+-rw-rw-rw-   0        0        0      271 2022-12-27 04:24:36.000000 afeng-py-tools-0.0.99/src/afeng_tools/weixin_tool/core/format/reply_msg/xml/image_msg.xml
+-rw-rw-rw-   0        0        0      492 2022-12-27 04:57:50.000000 afeng-py-tools-0.0.99/src/afeng_tools/weixin_tool/core/format/reply_msg/xml/music_msg.xml
+-rw-rw-rw-   0        0        0      297 2022-12-27 05:09:48.000000 afeng-py-tools-0.0.99/src/afeng_tools/weixin_tool/core/format/reply_msg/xml/news_msg.xml
+-rw-rw-rw-   0        0        0      191 2022-12-27 05:09:48.000000 afeng-py-tools-0.0.99/src/afeng_tools/weixin_tool/core/format/reply_msg/xml/news_msg_item.xml
+-rw-rw-rw-   0        0        0      244 2022-12-27 04:24:36.000000 afeng-py-tools-0.0.99/src/afeng_tools/weixin_tool/core/format/reply_msg/xml/text_msg.xml
+-rw-rw-rw-   0        0        0      363 2022-12-27 04:49:51.000000 afeng-py-tools-0.0.99/src/afeng_tools/weixin_tool/core/format/reply_msg/xml/video_msg.xml
+-rw-rw-rw-   0        0        0      271 2022-12-27 04:37:13.000000 afeng-py-tools-0.0.99/src/afeng_tools/weixin_tool/core/format/reply_msg/xml/voice_msg.xml
+-rw-rw-rw-   0        0        0      597 2023-12-06 21:52:19.000000 afeng-py-tools-0.0.99/src/afeng_tools/weixin_tool/core/format/weixin_format_replay.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:32.292855 afeng-py-tools-0.0.99/src/afeng_tools/weixin_tool/core/model/
+-rw-rw-rw-   0        0        0        0 2022-12-26 19:26:44.000000 afeng-py-tools-0.0.99/src/afeng_tools/weixin_tool/core/model/__init__.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:32.300601 afeng-py-tools-0.0.99/src/afeng_tools/weixin_tool/core/model/item/
+-rw-rw-rw-   0        0        0        0 2023-11-14 23:46:01.000000 afeng-py-tools-0.0.99/src/afeng_tools/weixin_tool/core/model/item/__init__.py
+-rw-rw-rw-   0        0        0     2352 2023-12-08 00:26:45.000000 afeng-py-tools-0.0.99/src/afeng_tools/weixin_tool/core/model/item/wx_receive_event_models.py
+-rw-rw-rw-   0        0        0     2726 2023-11-15 02:32:47.000000 afeng-py-tools-0.0.99/src/afeng_tools/weixin_tool/core/model/item/wx_receive_msg_models.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:32.307348 afeng-py-tools-0.0.99/src/afeng_tools/weixin_tool/core/model/po/
+-rw-rw-rw-   0        0        0      117 2023-12-06 22:39:11.000000 afeng-py-tools-0.0.99/src/afeng_tools/weixin_tool/core/model/po/__init__.py
+-rw-rw-rw-   0        0        0     3177 2023-12-25 06:27:58.000000 afeng-py-tools-0.0.99/src/afeng_tools/weixin_tool/core/model/po/wx_receive_event_models.py
+-rw-rw-rw-   0        0        0     3834 2023-12-25 06:27:58.000000 afeng-py-tools-0.0.99/src/afeng_tools/weixin_tool/core/model/po/wx_receive_msg_models.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:32.311738 afeng-py-tools-0.0.99/src/afeng_tools/weixin_tool/core/parse/
+-rw-rw-rw-   0        0        0        0 2022-12-27 02:17:10.000000 afeng-py-tools-0.0.99/src/afeng_tools/weixin_tool/core/parse/__init__.py
+-rw-rw-rw-   0        0        0     1442 2023-12-07 22:49:24.000000 afeng-py-tools-0.0.99/src/afeng_tools/weixin_tool/core/parse/parse_receive.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:32.319492 afeng-py-tools-0.0.99/src/afeng_tools/weixin_tool/core/parse/receive_event/
+-rw-rw-rw-   0        0        0        0 2022-12-27 03:35:50.000000 afeng-py-tools-0.0.99/src/afeng_tools/weixin_tool/core/parse/receive_event/__init__.py
+-rw-rw-rw-   0        0        0     3382 2023-12-07 22:49:24.000000 afeng-py-tools-0.0.99/src/afeng_tools/weixin_tool/core/parse/receive_event/parse_event.py
+-rw-rw-rw-   0        0        0      716 2023-12-07 22:49:24.000000 afeng-py-tools-0.0.99/src/afeng_tools/weixin_tool/core/parse/receive_event/parse_tool.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:32.326088 afeng-py-tools-0.0.99/src/afeng_tools/weixin_tool/core/parse/receive_msg/
+-rw-rw-rw-   0        0        0        0 2022-12-26 16:34:18.000000 afeng-py-tools-0.0.99/src/afeng_tools/weixin_tool/core/parse/receive_msg/__init__.py
+-rw-rw-rw-   0        0        0     3840 2023-12-07 22:49:24.000000 afeng-py-tools-0.0.99/src/afeng_tools/weixin_tool/core/parse/receive_msg/parse_msg.py
+-rw-rw-rw-   0        0        0     2300 2023-12-07 22:49:24.000000 afeng-py-tools-0.0.99/src/afeng_tools/weixin_tool/core/parse/receive_msg/parse_tool.py
+-rw-rw-rw-   0        0        0      240 2022-12-27 05:37:11.000000 afeng-py-tools-0.0.99/src/afeng_tools/weixin_tool/core/response.py
+-rw-rw-rw-   0        0        0     1418 2023-12-07 23:12:28.000000 afeng-py-tools-0.0.99/src/afeng_tools/weixin_tool/core/weixin_depends.py
+-rw-rw-rw-   0        0        0     1880 2023-12-16 02:20:46.000000 afeng-py-tools-0.0.99/src/afeng_tools/weixin_tool/core/weixin_enums.py
+-rw-rw-rw-   0        0        0      694 2023-12-07 23:52:20.000000 afeng-py-tools-0.0.99/src/afeng_tools/weixin_tool/core/weixin_reply_tool.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:32.334923 afeng-py-tools-0.0.99/src/afeng_tools/weixin_tool/custom_menu/
+-rw-rw-rw-   0        0        0       27 2023-11-22 20:49:32.000000 afeng-py-tools-0.0.99/src/afeng_tools/weixin_tool/custom_menu/__init__.py
+-rw-rw-rw-   0        0        0     5111 2023-11-22 21:48:05.000000 afeng-py-tools-0.0.99/src/afeng_tools/weixin_tool/custom_menu/wx_custome_menu_models.py
+-rw-rw-rw-   0        0        0     1861 2023-12-07 23:16:19.000000 afeng-py-tools-0.0.99/src/afeng_tools/weixin_tool/custom_menu/wx_custome_menu_tools.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:32.342650 afeng-py-tools-0.0.99/src/afeng_tools/weixin_tool/token/
+-rw-rw-rw-   0        0        0      129 2023-11-22 20:50:34.000000 afeng-py-tools-0.0.99/src/afeng_tools/weixin_tool/token/__init__.py
+-rw-rw-rw-   0        0        0      322 2023-11-22 21:02:34.000000 afeng-py-tools-0.0.99/src/afeng_tools/weixin_tool/token/wx_token_models.py
+-rw-rw-rw-   0        0        0     2877 2023-12-08 07:15:41.000000 afeng-py-tools-0.0.99/src/afeng_tools/weixin_tool/token/wx_token_tools.py
+-rw-rw-rw-   0        0        0     1264 2023-12-16 04:41:08.000000 afeng-py-tools-0.0.99/src/afeng_tools/weixin_tool/weixin_settings.py
+-rw-rw-rw-   0        0        0     1673 2023-12-21 00:21:43.000000 afeng-py-tools-0.0.99/src/afeng_tools/weixin_tool/weixin_views.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:32.356975 afeng-py-tools-0.0.99/src/afeng_tools/windows_tool/
+-rw-rw-rw-   0        0        0       26 2023-12-06 21:39:27.000000 afeng-py-tools-0.0.99/src/afeng_tools/windows_tool/__init__.py
+-rw-rw-rw-   0        0        0      417 2023-12-06 21:40:16.000000 afeng-py-tools-0.0.99/src/afeng_tools/windows_tool/image_tools.py
+-rw-rw-rw-   0        0        0      762 2023-09-24 23:57:02.000000 afeng-py-tools-0.0.99/src/afeng_tools/windows_tool/notify_tools.py
+-rw-rw-rw-   0        0        0      301 2023-09-24 23:55:52.000000 afeng-py-tools-0.0.99/src/afeng_tools/windows_tool/tts_tools.py
+-rw-rw-rw-   0        0        0      294 2023-10-07 10:10:04.000000 afeng-py-tools-0.0.99/src/afeng_tools/windows_tool/window_tools.py
+-rw-rw-rw-   0        0        0     1146 2024-01-31 23:36:01.000000 afeng-py-tools-0.0.99/src/afeng_tools/windows_tool/windows_sh_tools.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:32.373648 afeng-py-tools-0.0.99/src/openapi_client/
+-rw-rw-rw-   0        0        0      662 2022-06-16 10:13:37.000000 afeng-py-tools-0.0.99/src/openapi_client/__init__.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:32.391550 afeng-py-tools-0.0.99/src/openapi_client/api/
+-rw-rw-rw-   0        0        0      235 2022-06-16 10:13:37.000000 afeng-py-tools-0.0.99/src/openapi_client/api/__init__.py
+-rw-rw-rw-   0        0        0    23616 2022-06-16 10:13:37.000000 afeng-py-tools-0.0.99/src/openapi_client/api/auth_api.py
+-rw-rw-rw-   0        0        0    25848 2022-06-16 10:13:37.000000 afeng-py-tools-0.0.99/src/openapi_client/api/fileinfo_api.py
+-rw-rw-rw-   0        0        0    23597 2022-06-16 10:13:37.000000 afeng-py-tools-0.0.99/src/openapi_client/api/filemanager_api.py
+-rw-rw-rw-   0        0        0    21377 2022-06-16 10:13:37.000000 afeng-py-tools-0.0.99/src/openapi_client/api/fileupload_api.py
+-rw-rw-rw-   0        0        0    13681 2022-06-16 10:13:37.000000 afeng-py-tools-0.0.99/src/openapi_client/api/multimediafile_api.py
+-rw-rw-rw-   0        0        0    10977 2022-06-16 10:13:37.000000 afeng-py-tools-0.0.99/src/openapi_client/api/userinfo_api.py
+-rw-rw-rw-   0        0        0    37573 2022-06-16 10:13:37.000000 afeng-py-tools-0.0.99/src/openapi_client/api_client.py
+-rw-rw-rw-   0        0        0    16414 2022-06-16 10:13:37.000000 afeng-py-tools-0.0.99/src/openapi_client/configuration.py
+-rw-rw-rw-   0        0        0     5565 2022-06-16 10:13:37.000000 afeng-py-tools-0.0.99/src/openapi_client/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-02-05 18:37:32.410723 afeng-py-tools-0.0.99/src/openapi_client/model/
+-rw-rw-rw-   0        0        0      348 2022-06-16 10:13:37.000000 afeng-py-tools-0.0.99/src/openapi_client/model/__init__.py
+-rw-rw-rw-   0        0        0    12130 2022-06-16 10:13:37.000000 afeng-py-tools-0.0.99/src/openapi_client/model/oauth_token_authorization_code_response.py
+-rw-rw-rw-   0        0        0    12104 2022-06-16 10:13:37.000000 afeng-py-tools-0.0.99/src/openapi_client/model/oauth_token_device_code_response.py
+-rw-rw-rw-   0        0        0    12112 2022-06-16 10:13:37.000000 afeng-py-tools-0.0.99/src/openapi_client/model/oauth_token_device_token_response.py
+-rw-rw-rw-   0        0        0    12115 2022-06-16 10:13:37.000000 afeng-py-tools-0.0.99/src/openapi_client/model/oauth_token_refresh_token_response.py
+-rw-rw-rw-   0        0        0    11912 2022-06-16 10:13:37.000000 afeng-py-tools-0.0.99/src/openapi_client/model/quotaresponse.py
+-rw-rw-rw-   0        0        0    12370 2022-06-16 10:13:37.000000 afeng-py-tools-0.0.99/src/openapi_client/model/uinforesponse.py
+-rw-rw-rw-   0        0        0    81982 2023-12-16 05:11:02.000000 afeng-py-tools-0.0.99/src/openapi_client/model_utils.py
+-rw-rw-rw-   0        0        0    14763 2022-06-16 10:13:37.000000 afeng-py-tools-0.0.99/src/openapi_client/rest.py
+-rw-rw-rw-   0        0        0     1822 2023-12-07 09:17:51.000000 afeng-py-tools-0.0.99/src/version_helper.py
```

### Comparing `afeng-py-tools-0.0.98/.gitignore` & `afeng-py-tools-0.0.99/.gitignore`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/LICENSE` & `afeng-py-tools-0.0.99/LICENSE`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/PKG-INFO` & `afeng-py-tools-0.0.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: afeng-py-tools
-Version: 0.0.98
+Version: 0.0.99
 Summary: 阿锋的Python工具集
 Author-email: chentiefeng <imchentiefeng@aliyun.com>
 Maintainer-email: chentiefeng <imchentiefeng@aliyun.com>
 License:                      木兰宽松许可证, 第2版
         
            木兰宽松许可证， 第2版 
            2020年1月 http://license.coscl.org.cn/MulanPSL2
```

### Comparing `afeng-py-tools-0.0.98/README.md` & `afeng-py-tools-0.0.99/README.md`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/doc/项目打包流程.md` & `afeng-py-tools-0.0.99/doc/项目打包流程.md`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/pyproject.toml` & `afeng-py-tools-0.0.99/pyproject.toml`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_py_tools.egg-info/PKG-INFO` & `afeng-py-tools-0.0.99/src/afeng_py_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: afeng-py-tools
-Version: 0.0.98
+Version: 0.0.99
 Summary: 阿锋的Python工具集
 Author-email: chentiefeng <imchentiefeng@aliyun.com>
 Maintainer-email: chentiefeng <imchentiefeng@aliyun.com>
 License:                      木兰宽松许可证, 第2版
         
            木兰宽松许可证， 第2版 
            2020年1月 http://license.coscl.org.cn/MulanPSL2
```

### Comparing `afeng-py-tools-0.0.98/src/afeng_py_tools.egg-info/SOURCES.txt` & `afeng-py-tools-0.0.99/src/afeng_py_tools.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -208,14 +208,17 @@
 src/afeng_tools/qrcode_tool/qrcode_tools.py
 src/afeng_tools/re_tool/__init__.py
 src/afeng_tools/re_tool/re_tools.py
 src/afeng_tools/scrapy_tool/__init__.py
 src/afeng_tools/scrapy_tool/scrapy_request_tools.py
 src/afeng_tools/scrapy_tool/scrapy_run_tools.py
 src/afeng_tools/scrapy_tool/scrapy_selector_tools.py
+src/afeng_tools/scrapy_tool/scrapy_wiki/__init__.py
+src/afeng_tools/scrapy_tool/scrapy_wiki/spider_wiki_items.py
+src/afeng_tools/scrapy_tool/scrapy_wiki/spider_wiki_tools.py
 src/afeng_tools/serialization_tool/__init__.py
 src/afeng_tools/serialization_tool/pickle_tools.py
 src/afeng_tools/sqlalchemy_tool/__init__.py
 src/afeng_tools/sqlalchemy_tool/sqlalchemy_db_copy_tools.py
 src/afeng_tools/sqlalchemy_tool/sqlalchemy_settings.py
 src/afeng_tools/sqlalchemy_tool/sqlalchemy_tools.py
 src/afeng_tools/sqlalchemy_tool/core/__init__.py
```

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/aliyun_pan_tool/aliyun_pan_share_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/aliyun_pan_tool/aliyun_pan_share_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/aliyun_pan_tool/aliyun_pan_sign_in_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/aliyun_pan_tool/aliyun_pan_sign_in_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/aliyun_pan_tool/aliyun_pan_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/aliyun_pan_tool/aliyun_pan_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/aliyun_pan_tool/demo/run_demo.py` & `afeng-py-tools-0.0.99/src/afeng_tools/aliyun_pan_tool/demo/run_demo.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/aliyun_pan_tool/demo/share_demo.py` & `afeng-py-tools-0.0.99/src/afeng_tools/aliyun_pan_tool/demo/share_demo.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/appium_tool/appium_client_tool.py` & `afeng-py-tools-0.0.99/src/afeng_tools/appium_tool/appium_client_tool.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/appium_tool/appium_options_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/appium_tool/appium_options_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/appium_tool/appium_touch_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/appium_tool/appium_touch_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/appium_tool/mobile_adb_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/appium_tool/mobile_adb_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/appium_tool/mobile_app_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/appium_tool/mobile_app_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/appium_tool/mobile_keycode.py` & `afeng-py-tools-0.0.99/src/afeng_tools/appium_tool/mobile_keycode.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/application_tool/application_models.py` & `afeng-py-tools-0.0.99/src/afeng_tools/application_tool/application_models.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/application_tool/application_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/application_tool/application_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/application_tool/demo/settings.py` & `afeng-py-tools-0.0.99/src/afeng_tools/application_tool/demo/settings.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/application_tool/demo/yaml_demo/application.yml` & `afeng-py-tools-0.0.99/src/afeng_tools/application_tool/demo/yaml_demo/application.yml`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/application_tool/settings_enum.py` & `afeng-py-tools-0.0.99/src/afeng_tools/application_tool/settings_enum.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/application_tool/settings_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/application_tool/settings_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/baidu_pan_tool/baidu_pan_settings.py` & `afeng-py-tools-0.0.99/src/afeng_tools/baidu_pan_tool/baidu_pan_settings.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/baidu_pan_tool/baidu_pan_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/baidu_pan_tool/baidu_pan_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/baidu_pan_tool/core/baidu_pan_api_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/baidu_pan_tool/core/baidu_pan_api_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/baidu_pan_tool/core/baidu_pan_decorator_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/baidu_pan_tool/core/baidu_pan_decorator_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/baidu_pan_tool/core/baidu_pan_models.py` & `afeng-py-tools-0.0.99/src/afeng_tools/baidu_pan_tool/core/baidu_pan_models.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/baidu_pan_tool/demo/baidupan_demo.py` & `afeng-py-tools-0.0.99/src/afeng_tools/baidu_pan_tool/demo/baidupan_demo.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/baidu_pan_tool/demo/share_msg.txt` & `afeng-py-tools-0.0.99/src/afeng_tools/baidu_pan_tool/demo/share_msg.txt`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/baidu_pan_tool/tools/audio_file_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/baidu_pan_tool/tools/audio_file_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/baidu_pan_tool/tools/auth_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/baidu_pan_tool/tools/auth_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/baidu_pan_tool/tools/auth_web_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/baidu_pan_tool/tools/auth_web_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/baidu_pan_tool/tools/file_download_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/baidu_pan_tool/tools/file_download_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/baidu_pan_tool/tools/file_manager_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/baidu_pan_tool/tools/file_manager_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/baidu_pan_tool/tools/file_meta_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/baidu_pan_tool/tools/file_meta_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/baidu_pan_tool/tools/file_path_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/baidu_pan_tool/tools/file_path_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/baidu_pan_tool/tools/file_upload_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/baidu_pan_tool/tools/file_upload_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/baidu_pan_tool/tools/share_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/baidu_pan_tool/tools/share_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/baidu_pan_tool/tools/user_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/baidu_pan_tool/tools/user_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/baidu_pan_tool/tools/video_file_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/baidu_pan_tool/tools/video_file_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/cache_tool/cache_decorator.py` & `afeng-py-tools-0.0.99/src/afeng_tools/cache_tool/cache_decorator.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/cache_tool/cache_memory_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/cache_tool/cache_memory_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/compression_tool/zip_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/compression_tool/zip_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/convert_tool/type_convert_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/convert_tool/type_convert_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/crawler_tool/pyquery_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/crawler_tool/pyquery_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/datetime_tool/datetime_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/datetime_tool/datetime_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/datetime_tool/time_monitor_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/datetime_tool/time_monitor_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/decorator_tool/decorator_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/decorator_tool/decorator_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/east_money_tool/config/web_url_config.py` & `afeng-py-tools-0.0.99/src/afeng_tools/east_money_tool/config/web_url_config.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/east_money_tool/quote_info/east_money_quote_data_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/east_money_tool/quote_info/east_money_quote_data_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/east_money_tool/quote_info/quote_field_enum.py` & `afeng-py-tools-0.0.99/src/afeng_tools/east_money_tool/quote_info/quote_field_enum.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/east_money_tool/quote_info/quote_info_config.py` & `afeng-py-tools-0.0.99/src/afeng_tools/east_money_tool/quote_info/quote_info_config.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/east_money_tool/quote_info/quote_item_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/east_money_tool/quote_info/quote_item_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/east_money_tool/quote_info/quote_models.py` & `afeng-py-tools-0.0.99/src/afeng_tools/east_money_tool/quote_info/quote_models.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/east_money_tool/stock_comment/east_money_zhpj_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/east_money_tool/stock_comment/east_money_zhpj_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/east_money_tool/stock_comment/east_money_zlkp_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/east_money_tool/stock_comment/east_money_zlkp_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/east_money_tool/tool/east_money_http_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/east_money_tool/tool/east_money_http_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/east_money_tool/tool/east_money_load_auth_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/east_money_tool/tool/east_money_load_auth_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/email_tool/email_send_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/email_tool/email_send_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/email_tool/email_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/email_tool/email_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/encryption_tool/hashlib_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/encryption_tool/hashlib_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/fastapi_tool/admin/admin_router_model.py` & `afeng-py-tools-0.0.99/src/afeng_tools/fastapi_tool/admin/admin_router_model.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/fastapi_tool/admin/admin_views_template.py` & `afeng-py-tools-0.0.99/src/afeng_tools/fastapi_tool/admin/admin_views_template.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/fastapi_tool/admin/admin_views_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/fastapi_tool/admin/admin_views_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/fastapi_tool/admin/fastapi_api_doc_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/fastapi_tool/admin/fastapi_api_doc_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/fastapi_tool/core/fastapi_app_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/fastapi_tool/core/fastapi_app_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/fastapi_tool/core/fastapi_items.py` & `afeng-py-tools-0.0.99/src/afeng_tools/fastapi_tool/core/fastapi_items.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/fastapi_tool/demo/main.py` & `afeng-py-tools-0.0.99/src/afeng_tools/fastapi_tool/demo/main.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/fastapi_tool/fastapi_auto_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/fastapi_tool/fastapi_auto_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/fastapi_tool/fastapi_depends_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/fastapi_tool/fastapi_depends_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/fastapi_tool/fastapi_jinja2_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/fastapi_tool/fastapi_jinja2_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/fastapi_tool/fastapi_json_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/fastapi_tool/fastapi_json_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/fastapi_tool/fastapi_request_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/fastapi_tool/fastapi_request_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/fastapi_tool/fastapi_response_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/fastapi_tool/fastapi_response_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/fastapi_tool/fastapi_router_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/fastapi_tool/fastapi_router_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/fastapi_tool/fastapi_settings.py` & `afeng-py-tools-0.0.99/src/afeng_tools/fastapi_tool/fastapi_settings.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/file_tool/csv_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/file_tool/csv_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/file_tool/file_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/file_tool/file_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/file_tool/tmp_file_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/file_tool/tmp_file_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/flask_tool/flask_app_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/flask_tool/flask_app_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/generic_tool/generic_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/generic_tool/generic_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/http_tool/aria2c_download_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/http_tool/aria2c_download_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/http_tool/decorator/http_auto_retry_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/http_tool/decorator/http_auto_retry_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/http_tool/http_download_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/http_tool/http_download_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/http_tool/http_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/http_tool/http_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/http_tool/httpx/async_http.py` & `afeng-py-tools-0.0.99/src/afeng_tools/http_tool/httpx/async_http.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/http_tool/httpx/sync_http.py` & `afeng-py-tools-0.0.99/src/afeng_tools/http_tool/httpx/sync_http.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/image_tool/image_base64_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/image_tool/image_base64_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/import_tool/import_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/import_tool/import_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/javascript_tool/javascript_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/javascript_tool/javascript_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/jinja2_tool/jinja2_decorator_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/jinja2_tool/jinja2_decorator_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/jinja2_tool/jinja2_filters.py` & `afeng-py-tools-0.0.99/src/afeng_tools/jinja2_tool/jinja2_filters.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/jinja2_tool/jinja2_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/jinja2_tool/jinja2_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/json_tool/json_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/json_tool/json_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/layui_tool/core/layui_models.py` & `afeng-py-tools-0.0.99/src/afeng_tools/layui_tool/core/layui_models.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/layui_tool/layui_template_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/layui_tool/layui_template_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/layui_tool/template/form/step_form.html` & `afeng-py-tools-0.0.99/src/afeng_tools/layui_tool/template/form/step_form.html`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/layui_tool/template/table/add.html` & `afeng-py-tools-0.0.99/src/afeng_tools/layui_tool/template/table/add.html`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/layui_tool/template/table/edit.html` & `afeng-py-tools-0.0.99/src/afeng_tools/layui_tool/template/table/edit.html`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/layui_tool/template/table/list.html` & `afeng-py-tools-0.0.99/src/afeng_tools/layui_tool/template/table/list.html`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/layui_tool/template/table/show.html` & `afeng-py-tools-0.0.99/src/afeng_tools/layui_tool/template/table/show.html`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/linux_tool/linux_match_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/linux_tool/linux_match_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/linux_tool/sh_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/linux_tool/sh_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/log_tool/logger_settings.py` & `afeng-py-tools-0.0.99/src/afeng_tools/log_tool/logger_settings.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/log_tool/logging_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/log_tool/logging_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/log_tool/loguru_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/log_tool/loguru_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/math_tool/core/number_to_chinese.py` & `afeng-py-tools-0.0.99/src/afeng_tools/math_tool/core/number_to_chinese.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/math_tool/random_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/math_tool/random_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/os_tool/os_platform_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/os_tool/os_platform_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/pandas_tool/pandas_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/pandas_tool/pandas_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/playwright_tool/decorator/playwright_async_decorators.py` & `afeng-py-tools-0.0.99/src/afeng_tools/playwright_tool/decorator/playwright_async_decorators.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/playwright_tool/decorator/playwright_decorators.py` & `afeng-py-tools-0.0.99/src/afeng_tools/playwright_tool/decorator/playwright_decorators.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/playwright_tool/http_cookie_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/playwright_tool/http_cookie_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/playwright_tool/http_header_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/playwright_tool/http_header_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/playwright_tool/http_storage_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/playwright_tool/http_storage_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/playwright_tool/playwright_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/playwright_tool/playwright_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/playwright_tool/spider/base_spider.py` & `afeng-py-tools-0.0.99/src/afeng_tools/playwright_tool/spider/base_spider.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/playwright_tool/test001.py` & `afeng-py-tools-0.0.99/src/afeng_tools/playwright_tool/test001.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/pydantic_tool/model/common_models.py` & `afeng-py-tools-0.0.99/src/afeng_tools/pydantic_tool/model/common_models.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/pydantic_tool/pydantic_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/pydantic_tool/pydantic_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/python_tool/dict_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/python_tool/dict_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/qrcode_tool/qrcode_demo.py` & `afeng-py-tools-0.0.99/src/afeng_tools/qrcode_tool/qrcode_demo.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/qrcode_tool/qrcode_image_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/qrcode_tool/qrcode_image_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/qrcode_tool/qrcode_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/qrcode_tool/qrcode_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/re_tool/re_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/re_tool/re_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/scrapy_tool/scrapy_request_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/scrapy_tool/scrapy_request_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/scrapy_tool/scrapy_run_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/scrapy_tool/scrapy_run_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/scrapy_tool/scrapy_selector_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/scrapy_tool/scrapy_selector_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/serialization_tool/pickle_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/serialization_tool/pickle_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/sqlalchemy_tool/core/orm_model_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/sqlalchemy_tool/core/orm_model_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/sqlalchemy_tool/core/sqlalchemy_base_model.py` & `afeng-py-tools-0.0.99/src/afeng_tools/sqlalchemy_tool/core/sqlalchemy_base_model.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/sqlalchemy_tool/core/sqlalchemy_db_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/sqlalchemy_tool/core/sqlalchemy_db_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/sqlalchemy_tool/core/sqlalchemy_item.py` & `afeng-py-tools-0.0.99/src/afeng_tools/sqlalchemy_tool/core/sqlalchemy_item.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/sqlalchemy_tool/core/sqlalchemy_meta_class.py` & `afeng-py-tools-0.0.99/src/afeng_tools/sqlalchemy_tool/core/sqlalchemy_meta_class.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/sqlalchemy_tool/core/sqlalchemy_model_utils.py` & `afeng-py-tools-0.0.99/src/afeng_tools/sqlalchemy_tool/core/sqlalchemy_model_utils.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/sqlalchemy_tool/core/sqlalchemy_session_decorator.py` & `afeng-py-tools-0.0.99/src/afeng_tools/sqlalchemy_tool/core/sqlalchemy_session_decorator.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/sqlalchemy_tool/crdu/base_crdu.py` & `afeng-py-tools-0.0.99/src/afeng_tools/sqlalchemy_tool/crdu/base_crdu.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/sqlalchemy_tool/crdu/sequence_crdu.py` & `afeng-py-tools-0.0.99/src/afeng_tools/sqlalchemy_tool/crdu/sequence_crdu.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/sqlalchemy_tool/crdu/session_crdu.py` & `afeng-py-tools-0.0.99/src/afeng_tools/sqlalchemy_tool/crdu/session_crdu.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/sqlalchemy_tool/crdu/sql_crdu.py` & `afeng-py-tools-0.0.99/src/afeng_tools/sqlalchemy_tool/crdu/sql_crdu.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/sqlalchemy_tool/sqlalchemy_db_copy_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/sqlalchemy_tool/sqlalchemy_db_copy_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/sqlalchemy_tool/sqlalchemy_settings.py` & `afeng-py-tools-0.0.99/src/afeng_tools/sqlalchemy_tool/sqlalchemy_settings.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/sqlalchemy_tool/sqlalchemy_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/sqlalchemy_tool/sqlalchemy_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/sqlalchemy_tools/core/sqlalchemy_base_model.py` & `afeng-py-tools-0.0.99/src/afeng_tools/sqlalchemy_tools/core/sqlalchemy_base_model.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/sqlalchemy_tools/core/sqlalchemy_class.py` & `afeng-py-tools-0.0.99/src/afeng_tools/sqlalchemy_tools/core/sqlalchemy_class.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/sqlalchemy_tools/core/sqlalchemy_items.py` & `afeng-py-tools-0.0.99/src/afeng_tools/sqlalchemy_tools/core/sqlalchemy_items.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/sqlalchemy_tools/core/sqlalchemy_meta_class.py` & `afeng-py-tools-0.0.99/src/afeng_tools/sqlalchemy_tools/core/sqlalchemy_meta_class.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/sqlalchemy_tools/crdu/base_crdu.py` & `afeng-py-tools-0.0.99/src/afeng_tools/sqlalchemy_tools/crdu/base_crdu.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/sqlalchemy_tools/crdu/sequence_crdu.py` & `afeng-py-tools-0.0.99/src/afeng_tools/sqlalchemy_tools/crdu/sequence_crdu.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/sqlalchemy_tools/crdu/session_crdu.py` & `afeng-py-tools-0.0.99/src/afeng_tools/sqlalchemy_tools/crdu/session_crdu.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/sqlalchemy_tools/decorator/sqlalchemy_session_decorator.py` & `afeng-py-tools-0.0.99/src/afeng_tools/sqlalchemy_tools/decorator/sqlalchemy_session_decorator.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/sqlalchemy_tools/sqlalchemy_db_copy_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/sqlalchemy_tools/sqlalchemy_db_copy_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/sqlalchemy_tools/sqlalchemy_settings.py` & `afeng-py-tools-0.0.99/src/afeng_tools/sqlalchemy_tools/sqlalchemy_settings.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/sqlalchemy_tools/tool/orm_model_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/sqlalchemy_tools/tool/orm_model_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/sqlalchemy_tools/tool/sqlalchemy_model_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/sqlalchemy_tools/tool/sqlalchemy_model_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/template_tool/README.md` & `afeng-py-tools-0.0.99/src/afeng_tools/template_tool/README.md`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/template_tool/core/calmjs_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/template_tool/core/calmjs_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/template_tool/core/js_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/template_tool/core/js_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/template_tool/core/less_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/template_tool/core/less_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/template_tool/core/vue_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/template_tool/core/vue_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/template_tool/template_auto_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/template_tool/template_auto_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/template_tool/template_decorator_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/template_tool/template_decorator_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/template_tool/template_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/template_tool/template_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/template_tool/vue_demo/python_component.vue` & `afeng-py-tools-0.0.99/src/afeng_tools/template_tool/vue_demo/python_component.vue`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/text_tool/article_split_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/text_tool/article_split_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/text_tool/word_break_tool/jieba_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/text_tool/word_break_tool/jieba_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/trade_tool/trade_calendar_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/trade_tool/trade_calendar_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/tushare_tool/sh_sz_stock/stock_basic_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/tushare_tool/sh_sz_stock/stock_basic_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/web_tool/request_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/web_tool/request_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/web_tool/response_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/web_tool/response_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/weixin_min_program/core/weixin_mp_api_service.py` & `afeng-py-tools-0.0.99/src/afeng_tools/weixin_min_program/core/weixin_mp_api_service.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/weixin_min_program/core/weixin_mp_decrypt.py` & `afeng-py-tools-0.0.99/src/afeng_tools/weixin_min_program/core/weixin_mp_decrypt.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/weixin_min_program/core/weixin_mp_models.py` & `afeng-py-tools-0.0.99/src/afeng_tools/weixin_min_program/core/weixin_mp_models.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/weixin_min_program/core/weixin_mp_service.py` & `afeng-py-tools-0.0.99/src/afeng_tools/weixin_min_program/core/weixin_mp_service.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/weixin_min_program/model/weixin_mp_enums.py` & `afeng-py-tools-0.0.99/src/afeng_tools/weixin_min_program/model/weixin_mp_enums.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/weixin_min_program/model/weixin_mp_open_models.py` & `afeng-py-tools-0.0.99/src/afeng_tools/weixin_min_program/model/weixin_mp_open_models.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/weixin_min_program/weixin_mp_settings.py` & `afeng-py-tools-0.0.99/src/afeng_tools/weixin_min_program/weixin_mp_settings.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/weixin_min_program/weixin_mp_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/weixin_min_program/weixin_mp_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/weixin_min_program/weixin_mp_views.py` & `afeng-py-tools-0.0.99/src/afeng_tools/weixin_min_program/weixin_mp_views.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/weixin_tool/core/format/reply_msg/weixin_models.py` & `afeng-py-tools-0.0.99/src/afeng_tools/weixin_tool/core/format/reply_msg/weixin_models.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/weixin_tool/core/format/weixin_format_replay.py` & `afeng-py-tools-0.0.99/src/afeng_tools/weixin_tool/core/format/weixin_format_replay.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/weixin_tool/core/model/item/wx_receive_event_models.py` & `afeng-py-tools-0.0.99/src/afeng_tools/weixin_tool/core/model/item/wx_receive_event_models.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/weixin_tool/core/model/item/wx_receive_msg_models.py` & `afeng-py-tools-0.0.99/src/afeng_tools/weixin_tool/core/model/item/wx_receive_msg_models.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/weixin_tool/core/model/po/wx_receive_event_models.py` & `afeng-py-tools-0.0.99/src/afeng_tools/weixin_tool/core/model/po/wx_receive_event_models.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/weixin_tool/core/model/po/wx_receive_msg_models.py` & `afeng-py-tools-0.0.99/src/afeng_tools/weixin_tool/core/model/po/wx_receive_msg_models.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/weixin_tool/core/parse/parse_receive.py` & `afeng-py-tools-0.0.99/src/afeng_tools/weixin_tool/core/parse/parse_receive.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/weixin_tool/core/parse/receive_event/parse_event.py` & `afeng-py-tools-0.0.99/src/afeng_tools/weixin_tool/core/parse/receive_event/parse_event.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/weixin_tool/core/parse/receive_event/parse_tool.py` & `afeng-py-tools-0.0.99/src/afeng_tools/weixin_tool/core/parse/receive_event/parse_tool.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/weixin_tool/core/parse/receive_msg/parse_msg.py` & `afeng-py-tools-0.0.99/src/afeng_tools/weixin_tool/core/parse/receive_msg/parse_msg.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/weixin_tool/core/parse/receive_msg/parse_tool.py` & `afeng-py-tools-0.0.99/src/afeng_tools/weixin_tool/core/parse/receive_msg/parse_tool.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/weixin_tool/core/weixin_depends.py` & `afeng-py-tools-0.0.99/src/afeng_tools/weixin_tool/core/weixin_depends.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/weixin_tool/core/weixin_enums.py` & `afeng-py-tools-0.0.99/src/afeng_tools/weixin_tool/core/weixin_enums.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/weixin_tool/core/weixin_reply_tool.py` & `afeng-py-tools-0.0.99/src/afeng_tools/weixin_tool/core/weixin_reply_tool.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/weixin_tool/custom_menu/wx_custome_menu_models.py` & `afeng-py-tools-0.0.99/src/afeng_tools/weixin_tool/custom_menu/wx_custome_menu_models.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/weixin_tool/custom_menu/wx_custome_menu_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/weixin_tool/custom_menu/wx_custome_menu_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/weixin_tool/token/wx_token_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/weixin_tool/token/wx_token_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/weixin_tool/weixin_settings.py` & `afeng-py-tools-0.0.99/src/afeng_tools/weixin_tool/weixin_settings.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/weixin_tool/weixin_views.py` & `afeng-py-tools-0.0.99/src/afeng_tools/weixin_tool/weixin_views.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/windows_tool/notify_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/windows_tool/notify_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/afeng_tools/windows_tool/windows_sh_tools.py` & `afeng-py-tools-0.0.99/src/afeng_tools/windows_tool/windows_sh_tools.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/openapi_client/__init__.py` & `afeng-py-tools-0.0.99/src/openapi_client/__init__.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/openapi_client/api/auth_api.py` & `afeng-py-tools-0.0.99/src/openapi_client/api/auth_api.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/openapi_client/api/fileinfo_api.py` & `afeng-py-tools-0.0.99/src/openapi_client/api/fileinfo_api.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/openapi_client/api/filemanager_api.py` & `afeng-py-tools-0.0.99/src/openapi_client/api/filemanager_api.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/openapi_client/api/fileupload_api.py` & `afeng-py-tools-0.0.99/src/openapi_client/api/fileupload_api.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/openapi_client/api/multimediafile_api.py` & `afeng-py-tools-0.0.99/src/openapi_client/api/multimediafile_api.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/openapi_client/api/userinfo_api.py` & `afeng-py-tools-0.0.99/src/openapi_client/api/userinfo_api.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/openapi_client/api_client.py` & `afeng-py-tools-0.0.99/src/openapi_client/api_client.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/openapi_client/configuration.py` & `afeng-py-tools-0.0.99/src/openapi_client/configuration.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/openapi_client/exceptions.py` & `afeng-py-tools-0.0.99/src/openapi_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/openapi_client/model/oauth_token_authorization_code_response.py` & `afeng-py-tools-0.0.99/src/openapi_client/model/oauth_token_authorization_code_response.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/openapi_client/model/oauth_token_device_code_response.py` & `afeng-py-tools-0.0.99/src/openapi_client/model/oauth_token_device_code_response.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/openapi_client/model/oauth_token_device_token_response.py` & `afeng-py-tools-0.0.99/src/openapi_client/model/oauth_token_device_token_response.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/openapi_client/model/oauth_token_refresh_token_response.py` & `afeng-py-tools-0.0.99/src/openapi_client/model/oauth_token_refresh_token_response.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/openapi_client/model/quotaresponse.py` & `afeng-py-tools-0.0.99/src/openapi_client/model/quotaresponse.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/openapi_client/model/uinforesponse.py` & `afeng-py-tools-0.0.99/src/openapi_client/model/uinforesponse.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/openapi_client/model_utils.py` & `afeng-py-tools-0.0.99/src/openapi_client/model_utils.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/openapi_client/rest.py` & `afeng-py-tools-0.0.99/src/openapi_client/rest.py`

 * *Files identical despite different names*

### Comparing `afeng-py-tools-0.0.98/src/version_helper.py` & `afeng-py-tools-0.0.99/src/version_helper.py`

 * *Files identical despite different names*

