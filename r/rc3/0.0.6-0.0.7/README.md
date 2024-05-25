# Comparing `tmp/rc3-0.0.6.tar.gz` & `tmp/rc3-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rc3-0.0.6.tar", last modified: Fri May 17 16:45:44 2024, max compression
+gzip compressed data, was "rc3-0.0.7.tar", last modified: Sat May 25 17:54:45 2024, max compression
```

## Comparing `rc3-0.0.6.tar` & `rc3-0.0.7.tar`

### file list

```diff
@@ -1,152 +1,154 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 16:45:44.238582 rc3-0.0.6/
--rw-rw-rw-   0        0        0     3141 2024-05-06 19:59:38.000000 rc3-0.0.6/.gitignore
--rw-rw-rw-   0        0        0     1087 2024-05-06 20:36:33.000000 rc3-0.0.6/LICENSE
--rw-rw-rw-   0        0        0    11541 2024-05-17 16:45:44.237582 rc3-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     9437 2024-05-15 20:01:38.000000 rc3-0.0.6/README.md
--rw-rw-rw-   0        0        0     1044 2024-05-07 23:16:04.000000 rc3-0.0.6/WINDOWS_SETUP.md
--rw-rw-rw-   0        0        0      828 2024-05-17 16:41:36.000000 rc3-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0      475 2024-05-06 20:07:47.000000 rc3-0.0.6/rc3.iml
--rw-rw-rw-   0        0        0       97 2024-05-17 16:45:44.239582 rc3-0.0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-17 16:45:44.054067 rc3-0.0.6/src/
-drwxrwxrwx   0        0        0        0 2024-05-17 16:45:44.078325 rc3-0.0.6/src/rc3/
--rw-rw-rw-   0        0        0      246 2024-05-06 19:59:38.000000 rc3-0.0.6/src/rc3/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-17 16:45:44.091677 rc3-0.0.6/src/rc3/archive/
--rw-rw-rw-   0        0        0        0 2024-05-06 19:59:38.000000 rc3-0.0.6/src/rc3/archive/__init__.py
--rw-rw-rw-   0        0        0      406 2024-05-06 20:00:31.000000 rc3-0.0.6/src/rc3/archive/cmd_home.py
--rw-rw-rw-   0        0        0      637 2024-05-06 20:00:31.000000 rc3-0.0.6/src/rc3/archive/cmd_root.py
--rw-rw-rw-   0        0        0     1125 2024-05-06 20:00:31.000000 rc3-0.0.6/src/rc3/archive/cmd_subs.py
--rw-rw-rw-   0        0        0     1924 2024-05-07 23:36:03.000000 rc3-0.0.6/src/rc3/cli.py
-drwxrwxrwx   0        0        0        0 2024-05-17 16:45:44.106666 rc3-0.0.6/src/rc3/commands/
--rw-rw-rw-   0        0        0        0 2024-05-06 19:59:38.000000 rc3-0.0.6/src/rc3/commands/__init__.py
--rw-rw-rw-   0        0        0     3415 2024-05-06 22:52:43.000000 rc3-0.0.6/src/rc3/commands/cmd_collection.py
--rw-rw-rw-   0        0        0     5467 2024-05-07 23:33:42.000000 rc3-0.0.6/src/rc3/commands/cmd_environment.py
--rw-rw-rw-   0        0        0     1454 2024-05-07 23:35:00.000000 rc3-0.0.6/src/rc3/commands/cmd_global.py
--rw-rw-rw-   0        0        0      524 2024-05-06 19:59:38.000000 rc3-0.0.6/src/rc3/commands/cmd_hello.py
--rw-rw-rw-   0        0        0     3414 2024-05-15 20:01:43.000000 rc3-0.0.6/src/rc3/commands/cmd_init.py
--rw-rw-rw-   0        0        0     2136 2024-05-08 19:24:17.000000 rc3-0.0.6/src/rc3/commands/cmd_list.py
--rw-rw-rw-   0        0        0     4322 2024-05-06 20:00:31.000000 rc3-0.0.6/src/rc3/commands/cmd_request.py
--rw-rw-rw-   0        0        0     9478 2024-05-08 18:59:18.000000 rc3-0.0.6/src/rc3/commands/cmd_send.py
--rw-rw-rw-   0        0        0     1368 2024-05-08 18:10:08.000000 rc3-0.0.6/src/rc3/commands/cmd_settings.py
-drwxrwxrwx   0        0        0        0 2024-05-17 16:45:44.118656 rc3-0.0.6/src/rc3/common/
--rw-rw-rw-   0        0        0        0 2024-05-06 19:59:39.000000 rc3-0.0.6/src/rc3/common/__init__.py
--rw-rw-rw-   0        0        0      524 2024-05-06 19:59:39.000000 rc3-0.0.6/src/rc3/common/config_helper.py
--rw-rw-rw-   0        0        0      869 2024-05-06 22:59:13.000000 rc3-0.0.6/src/rc3/common/data_helper.py
--rw-rw-rw-   0        0        0      936 2024-05-06 19:59:39.000000 rc3-0.0.6/src/rc3/common/decorators.py
--rw-rw-rw-   0        0        0     2670 2024-05-06 20:00:31.000000 rc3-0.0.6/src/rc3/common/env_helper.py
--rw-rw-rw-   0        0        0     1364 2024-05-06 22:52:57.000000 rc3-0.0.6/src/rc3/common/inherit_helper.py
--rw-rw-rw-   0        0        0    10723 2024-05-08 18:47:05.000000 rc3-0.0.6/src/rc3/common/json_helper.py
--rw-rw-rw-   0        0        0     2503 2024-05-08 19:08:29.000000 rc3-0.0.6/src/rc3/common/print_helper.py
--rw-rw-rw-   0        0        0       86 2024-05-06 19:59:39.000000 rc3-0.0.6/src/rc3/common/rc_globals.py
-drwxrwxrwx   0        0        0        0 2024-05-17 16:45:44.119655 rc3-0.0.6/src/rc3/data/
--rw-rw-rw-   0        0        0        0 2024-05-06 19:59:39.000000 rc3-0.0.6/src/rc3/data/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-17 16:45:44.120655 rc3-0.0.6/src/rc3/data/collection/
-drwxrwxrwx   0        0        0        0 2024-05-17 16:45:44.126651 rc3-0.0.6/src/rc3/data/collection/environments/
--rw-rw-rw-   0        0        0        6 2024-05-15 19:30:06.000000 rc3-0.0.6/src/rc3/data/collection/environments/.gitignore
--rw-rw-rw-   0        0        0      277 2024-05-07 23:02:08.000000 rc3-0.0.6/src/rc3/data/collection/environments/dev.defaults
--rw-rw-rw-   0        0        0      307 2024-05-07 23:02:08.000000 rc3-0.0.6/src/rc3/data/collection/environments/localhost.defaults
-drwxrwxrwx   0        0        0        0 2024-05-17 16:45:44.143640 rc3-0.0.6/src/rc3/data/collection/examples/
--rw-rw-rw-   0        0        0      247 2024-05-07 23:02:08.000000 rc3-0.0.6/src/rc3/data/collection/examples/example_Auth_Basic.request
--rw-rw-rw-   0        0        0      914 2024-05-07 23:02:08.000000 rc3-0.0.6/src/rc3/data/collection/examples/example_Auth_Bearer.request
--rw-rw-rw-   0        0        0      960 2024-05-07 23:02:08.000000 rc3-0.0.6/src/rc3/data/collection/examples/example_Auth_Token.request
--rw-rw-rw-   0        0        0      436 2024-05-07 23:02:08.000000 rc3-0.0.6/src/rc3/data/collection/examples/example_Extract_JsonPath.request
--rw-rw-rw-   0        0        0      455 2024-05-07 23:02:08.000000 rc3-0.0.6/src/rc3/data/collection/examples/example_Extract_Regex.request
--rw-rw-rw-   0        0        0      190 2024-05-07 23:02:08.000000 rc3-0.0.6/src/rc3/data/collection/examples/example_GET.request
--rw-rw-rw-   0        0        0      799 2024-05-07 23:02:08.000000 rc3-0.0.6/src/rc3/data/collection/examples/example_KitchenSink.request
--rw-rw-rw-   0        0        0      401 2024-05-07 23:02:08.000000 rc3-0.0.6/src/rc3/data/collection/examples/example_MintOauth2Token.request
--rw-rw-rw-   0        0        0      275 2024-05-07 23:02:08.000000 rc3-0.0.6/src/rc3/data/collection/examples/example_POST_json.request
--rw-rw-rw-   0        0        0      231 2024-05-07 23:02:08.000000 rc3-0.0.6/src/rc3/data/collection/examples/example_POST_text-plain.request
--rw-rw-rw-   0        0        0      240 2024-05-07 23:02:08.000000 rc3-0.0.6/src/rc3/data/collection/examples/example_QueryParams.request
--rw-rw-rw-   0        0        0      227 2024-05-07 23:02:08.000000 rc3-0.0.6/src/rc3/data/collection/examples/example_UseOauth2Token.request
--rw-rw-rw-   0        0        0      272 2024-05-07 23:02:08.000000 rc3-0.0.6/src/rc3/data/collection/examples/folder.json
-drwxrwxrwx   0        0        0        0 2024-05-17 16:45:44.150636 rc3-0.0.6/src/rc3/data/collection/greetings-basic/
--rw-rw-rw-   0        0        0      384 2024-05-07 23:02:08.000000 rc3-0.0.6/src/rc3/data/collection/greetings-basic/greeting.request
--rw-rw-rw-   0        0        0      180 2024-05-07 23:02:08.000000 rc3-0.0.6/src/rc3/data/collection/greetings-basic/greetings.request
--rw-rw-rw-   0        0        0      291 2024-05-07 23:02:08.000000 rc3-0.0.6/src/rc3/data/collection/greetings-basic/new-greeting.request
--rw-rw-rw-   0        0        0      297 2024-05-07 23:02:08.000000 rc3-0.0.6/src/rc3/data/collection/greetings-basic/rc-folder.json
--rw-rw-rw-   0        0        0      185 2024-05-07 23:02:08.000000 rc3-0.0.6/src/rc3/data/collection/greetings-basic/remove-greeting.request
--rw-rw-rw-   0        0        0      313 2024-05-07 23:02:08.000000 rc3-0.0.6/src/rc3/data/collection/greetings-basic/update-greeting.request
-drwxrwxrwx   0        0        0        0 2024-05-17 16:45:44.154635 rc3-0.0.6/src/rc3/data/collection/greetings-oauth2/
--rw-rw-rw-   0        0        0      218 2024-05-07 23:02:08.000000 rc3-0.0.6/src/rc3/data/collection/greetings-oauth2/greeting.request
--rw-rw-rw-   0        0        0      466 2024-05-07 23:02:08.000000 rc3-0.0.6/src/rc3/data/collection/greetings-oauth2/mint-admin-token.request
--rw-rw-rw-   0        0        0      465 2024-05-07 23:02:08.000000 rc3-0.0.6/src/rc3/data/collection/greetings-oauth2/mint-token.request
--rw-rw-rw-   0        0        0      247 2024-05-08 14:58:01.000000 rc3-0.0.6/src/rc3/data/collection/rc-collection.json
-drwxrwxrwx   0        0        0        0 2024-05-17 16:45:44.158631 rc3-0.0.6/src/rc3/data/home/
--rw-rw-rw-   0        0        0      130 2024-05-07 23:02:08.000000 rc3-0.0.6/src/rc3/data/home/rc-global.json
--rw-rw-rw-   0        0        0      354 2024-05-07 23:02:39.000000 rc3-0.0.6/src/rc3/data/home/rc-settings.json
-drwxrwxrwx   0        0        0        0 2024-05-17 16:45:44.166626 rc3-0.0.6/src/rc3/data/home/schemas/
--rw-rw-rw-   0        0        0     1151 2024-05-07 23:02:08.000000 rc3-0.0.6/src/rc3/data/home/schemas/rc3-auth-0.0.3.json
--rw-rw-rw-   0        0        0      918 2024-05-07 23:02:08.000000 rc3-0.0.6/src/rc3/data/home/schemas/rc3-collection-0.0.3.json
--rw-rw-rw-   0        0        0      473 2024-05-07 23:02:08.000000 rc3-0.0.6/src/rc3/data/home/schemas/rc3-environment-0.0.3.json
--rw-rw-rw-   0        0        0      605 2024-05-07 23:02:08.000000 rc3-0.0.6/src/rc3/data/home/schemas/rc3-folder-0.0.3.json
--rw-rw-rw-   0        0        0     3241 2024-05-07 23:02:08.000000 rc3-0.0.6/src/rc3/data/home/schemas/rc3-request-0.0.3.json
--rw-rw-rw-   0        0        0     2259 2024-05-07 23:02:08.000000 rc3-0.0.6/src/rc3/data/home/schemas/rc3-settings-0.0.3.json
-drwxrwxrwx   0        0        0        0 2024-05-17 16:45:44.235592 rc3-0.0.6/src/rc3.egg-info/
--rw-rw-rw-   0        0        0    11541 2024-05-17 16:45:43.000000 rc3-0.0.6/src/rc3.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5196 2024-05-17 16:45:44.000000 rc3-0.0.6/src/rc3.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 16:45:43.000000 rc3-0.0.6/src/rc3.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2024-05-17 16:45:43.000000 rc3-0.0.6/src/rc3.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      100 2024-05-17 16:45:43.000000 rc3-0.0.6/src/rc3.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-05-17 16:45:43.000000 rc3-0.0.6/src/rc3.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-17 16:45:44.167629 rc3-0.0.6/temp-collection/
-drwxrwxrwx   0        0        0        0 2024-05-17 16:45:44.172622 rc3-0.0.6/temp-collection/environments/
--rw-rw-rw-   0        0        0        6 2024-05-15 19:30:06.000000 rc3-0.0.6/temp-collection/environments/.gitignore
--rw-rw-rw-   0        0        0      277 2024-05-07 23:02:08.000000 rc3-0.0.6/temp-collection/environments/dev.defaults
--rw-rw-rw-   0        0        0      307 2024-05-07 23:02:08.000000 rc3-0.0.6/temp-collection/environments/localhost.defaults
-drwxrwxrwx   0        0        0        0 2024-05-17 16:45:44.189612 rc3-0.0.6/temp-collection/examples/
--rw-rw-rw-   0        0        0      247 2024-05-07 23:02:08.000000 rc3-0.0.6/temp-collection/examples/example_Auth_Basic.request
--rw-rw-rw-   0        0        0      914 2024-05-07 23:02:08.000000 rc3-0.0.6/temp-collection/examples/example_Auth_Bearer.request
--rw-rw-rw-   0        0        0      960 2024-05-07 23:02:08.000000 rc3-0.0.6/temp-collection/examples/example_Auth_Token.request
--rw-rw-rw-   0        0        0      436 2024-05-07 23:02:08.000000 rc3-0.0.6/temp-collection/examples/example_Extract_JsonPath.request
--rw-rw-rw-   0        0        0      455 2024-05-07 23:02:08.000000 rc3-0.0.6/temp-collection/examples/example_Extract_Regex.request
--rw-rw-rw-   0        0        0      190 2024-05-07 23:02:08.000000 rc3-0.0.6/temp-collection/examples/example_GET.request
--rw-rw-rw-   0        0        0      799 2024-05-07 23:02:08.000000 rc3-0.0.6/temp-collection/examples/example_KitchenSink.request
--rw-rw-rw-   0        0        0      401 2024-05-07 23:02:08.000000 rc3-0.0.6/temp-collection/examples/example_MintOauth2Token.request
--rw-rw-rw-   0        0        0      275 2024-05-07 23:02:08.000000 rc3-0.0.6/temp-collection/examples/example_POST_json.request
--rw-rw-rw-   0        0        0      231 2024-05-07 23:02:08.000000 rc3-0.0.6/temp-collection/examples/example_POST_text-plain.request
--rw-rw-rw-   0        0        0      240 2024-05-07 23:02:08.000000 rc3-0.0.6/temp-collection/examples/example_QueryParams.request
--rw-rw-rw-   0        0        0      227 2024-05-07 23:02:08.000000 rc3-0.0.6/temp-collection/examples/example_UseOauth2Token.request
--rw-rw-rw-   0        0        0      272 2024-05-07 23:02:08.000000 rc3-0.0.6/temp-collection/examples/folder.json
-drwxrwxrwx   0        0        0        0 2024-05-17 16:45:44.197607 rc3-0.0.6/temp-collection/greetings-basic/
--rw-rw-rw-   0        0        0      384 2024-05-07 23:02:08.000000 rc3-0.0.6/temp-collection/greetings-basic/greeting.request
--rw-rw-rw-   0        0        0      180 2024-05-07 23:02:08.000000 rc3-0.0.6/temp-collection/greetings-basic/greetings.request
--rw-rw-rw-   0        0        0      291 2024-05-07 23:02:08.000000 rc3-0.0.6/temp-collection/greetings-basic/new-greeting.request
--rw-rw-rw-   0        0        0      297 2024-05-07 23:02:08.000000 rc3-0.0.6/temp-collection/greetings-basic/rc-folder.json
--rw-rw-rw-   0        0        0      185 2024-05-07 23:02:08.000000 rc3-0.0.6/temp-collection/greetings-basic/remove-greeting.request
--rw-rw-rw-   0        0        0      313 2024-05-07 23:02:08.000000 rc3-0.0.6/temp-collection/greetings-basic/update-greeting.request
-drwxrwxrwx   0        0        0        0 2024-05-17 16:45:44.200605 rc3-0.0.6/temp-collection/greetings-oauth2/
--rw-rw-rw-   0        0        0      218 2024-05-07 23:02:08.000000 rc3-0.0.6/temp-collection/greetings-oauth2/greeting.request
--rw-rw-rw-   0        0        0      466 2024-05-07 23:02:08.000000 rc3-0.0.6/temp-collection/greetings-oauth2/mint-admin-token.request
--rw-rw-rw-   0        0        0      465 2024-05-07 23:02:08.000000 rc3-0.0.6/temp-collection/greetings-oauth2/mint-token.request
--rw-rw-rw-   0        0        0      247 2024-05-08 14:58:01.000000 rc3-0.0.6/temp-collection/rc-collection.json
-drwxrwxrwx   0        0        0        0 2024-05-17 16:45:44.204602 rc3-0.0.6/tests/
--rw-rw-rw-   0        0        0        0 2024-05-06 19:59:39.000000 rc3-0.0.6/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-17 16:45:44.213596 rc3-0.0.6/tests/commands/
--rw-rw-rw-   0        0        0        0 2024-05-06 19:59:39.000000 rc3-0.0.6/tests/commands/__init__.py
--rw-rw-rw-   0        0        0      599 2024-05-06 20:00:31.000000 rc3-0.0.6/tests/commands/test_collection.py
--rw-rw-rw-   0        0        0     5698 2024-05-06 20:00:31.000000 rc3-0.0.6/tests/commands/test_environment.py
--rw-rw-rw-   0        0        0     1856 2024-05-08 19:17:23.000000 rc3-0.0.6/tests/commands/test_init.py
--rw-rw-rw-   0        0        0      427 2024-05-06 20:00:31.000000 rc3-0.0.6/tests/commands/test_list.py
--rw-rw-rw-   0        0        0     5923 2024-05-06 20:00:31.000000 rc3-0.0.6/tests/commands/test_request.py
--rw-rw-rw-   0        0        0     6322 2024-05-06 20:00:31.000000 rc3-0.0.6/tests/commands/test_send.py
-drwxrwxrwx   0        0        0        0 2024-05-17 16:45:44.226590 rc3-0.0.6/tests/commands/test_send_files/
--rw-rw-rw-   0        0        0      263 2024-05-06 19:59:39.000000 rc3-0.0.6/tests/commands/test_send_files/test_is_verbose.yaml
--rw-rw-rw-   0        0        0     1178 2024-05-06 19:59:39.000000 rc3-0.0.6/tests/commands/test_send_files/test_mint_extract_use_token.yaml
--rw-rw-rw-   0        0        0      263 2024-05-06 19:59:39.000000 rc3-0.0.6/tests/commands/test_send_files/test_not_verbose.yaml
--rw-rw-rw-   0        0        0      263 2024-05-06 19:59:39.000000 rc3-0.0.6/tests/commands/test_send_files/test_request_no_responses.yaml
--rw-rw-rw-   0        0        0      263 2024-05-06 19:59:39.000000 rc3-0.0.6/tests/commands/test_send_files/test_send_1.yaml
--rw-rw-rw-   0        0        0      663 2024-05-06 19:59:39.000000 rc3-0.0.6/tests/commands/test_send_files/test_send_2.yaml
--rw-rw-rw-   0        0        0     1098 2024-05-06 19:59:39.000000 rc3-0.0.6/tests/commands/test_send_files/test_send_basics.yaml
--rw-rw-rw-   0        0        0      263 2024-05-06 19:59:39.000000 rc3-0.0.6/tests/commands/test_send_files/test_settings_no_responses.yaml
--rw-rw-rw-   0        0        0      263 2024-05-06 19:59:39.000000 rc3-0.0.6/tests/commands/test_send_files/test_settings_with_responses.yaml
-drwxrwxrwx   0        0        0        0 2024-05-17 16:45:44.230587 rc3-0.0.6/tests/common/
--rw-rw-rw-   0        0        0        0 2024-05-06 19:59:39.000000 rc3-0.0.6/tests/common/__init__.py
--rw-rw-rw-   0        0        0     5211 2024-05-06 20:00:31.000000 rc3-0.0.6/tests/common/test_env_helper.py
--rw-rw-rw-   0        0        0     3345 2024-05-06 22:51:48.000000 rc3-0.0.6/tests/common/test_inherit_helper.py
--rw-rw-rw-   0        0        0     1124 2024-05-06 20:00:31.000000 rc3-0.0.6/tests/conftest.py
-drwxrwxrwx   0        0        0        0 2024-05-17 16:45:44.232586 rc3-0.0.6/tests/learning/
--rw-rw-rw-   0        0        0        0 2024-05-06 19:59:39.000000 rc3-0.0.6/tests/learning/__init__.py
--rw-rw-rw-   0        0        0      518 2024-05-06 19:59:39.000000 rc3-0.0.6/tests/learning/test_sample.py
--rw-rw-rw-   0        0        0     1665 2024-05-06 20:00:31.000000 rc3-0.0.6/tests/test_cli.py
-drwxrwxrwx   0        0        0        0 2024-05-17 16:45:44.234585 rc3-0.0.6/tests/util/
--rw-rw-rw-   0        0        0        0 2024-05-06 19:59:39.000000 rc3-0.0.6/tests/util/__init__.py
--rw-rw-rw-   0        0        0     1407 2024-05-06 19:59:39.000000 rc3-0.0.6/tests/util/decorators.py
+drwxrwxrwx   0        0        0        0 2024-05-25 17:54:45.611493 rc3-0.0.7/
+-rw-rw-rw-   0        0        0     3141 2024-05-06 19:59:38.000000 rc3-0.0.7/.gitignore
+-rw-rw-rw-   0        0        0     1087 2024-05-25 17:43:52.000000 rc3-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0    13086 2024-05-25 17:54:45.611493 rc3-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0    10982 2024-05-25 16:01:40.000000 rc3-0.0.7/README.md
+-rw-rw-rw-   0        0        0     1044 2024-05-07 23:16:04.000000 rc3-0.0.7/WINDOWS_SETUP.md
+-rw-rw-rw-   0        0        0      828 2024-05-25 16:05:08.000000 rc3-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0      475 2024-05-06 20:07:47.000000 rc3-0.0.7/rc3.iml
+-rw-rw-rw-   0        0        0       97 2024-05-25 17:54:45.612492 rc3-0.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-25 17:54:45.427606 rc3-0.0.7/src/
+drwxrwxrwx   0        0        0        0 2024-05-25 17:54:45.448594 rc3-0.0.7/src/rc3/
+-rw-rw-rw-   0        0        0      246 2024-05-06 19:59:38.000000 rc3-0.0.7/src/rc3/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-25 17:54:45.460585 rc3-0.0.7/src/rc3/archive/
+-rw-rw-rw-   0        0        0        0 2024-05-06 19:59:38.000000 rc3-0.0.7/src/rc3/archive/__init__.py
+-rw-rw-rw-   0        0        0      406 2024-05-06 20:00:31.000000 rc3-0.0.7/src/rc3/archive/cmd_home.py
+-rw-rw-rw-   0        0        0     3414 2024-05-15 20:01:43.000000 rc3-0.0.7/src/rc3/archive/cmd_init.py
+-rw-rw-rw-   0        0        0      637 2024-05-06 20:00:31.000000 rc3-0.0.7/src/rc3/archive/cmd_root.py
+-rw-rw-rw-   0        0        0     1125 2024-05-06 20:00:31.000000 rc3-0.0.7/src/rc3/archive/cmd_subs.py
+-rw-rw-rw-   0        0        0     2705 2024-05-25 16:18:57.000000 rc3-0.0.7/src/rc3/cli.py
+drwxrwxrwx   0        0        0        0 2024-05-25 17:54:45.474578 rc3-0.0.7/src/rc3/commands/
+-rw-rw-rw-   0        0        0        0 2024-05-06 19:59:38.000000 rc3-0.0.7/src/rc3/commands/__init__.py
+-rw-rw-rw-   0        0        0     3415 2024-05-06 22:52:43.000000 rc3-0.0.7/src/rc3/commands/cmd_collection.py
+-rw-rw-rw-   0        0        0     5467 2024-05-07 23:33:42.000000 rc3-0.0.7/src/rc3/commands/cmd_environment.py
+-rw-rw-rw-   0        0        0     1454 2024-05-07 23:35:00.000000 rc3-0.0.7/src/rc3/commands/cmd_global.py
+-rw-rw-rw-   0        0        0      524 2024-05-25 16:27:10.000000 rc3-0.0.7/src/rc3/commands/cmd_hello.py
+-rw-rw-rw-   0        0        0      767 2024-05-25 14:23:13.000000 rc3-0.0.7/src/rc3/commands/cmd_import.py
+-rw-rw-rw-   0        0        0     2136 2024-05-08 19:24:17.000000 rc3-0.0.7/src/rc3/commands/cmd_list.py
+-rw-rw-rw-   0        0        0     3794 2024-05-25 14:26:29.000000 rc3-0.0.7/src/rc3/commands/cmd_new.py
+-rw-rw-rw-   0        0        0     4633 2024-05-25 17:34:38.000000 rc3-0.0.7/src/rc3/commands/cmd_request.py
+-rw-rw-rw-   0        0        0     9545 2024-05-25 17:24:31.000000 rc3-0.0.7/src/rc3/commands/cmd_send.py
+-rw-rw-rw-   0        0        0     1368 2024-05-08 18:10:08.000000 rc3-0.0.7/src/rc3/commands/cmd_settings.py
+drwxrwxrwx   0        0        0        0 2024-05-25 17:54:45.484571 rc3-0.0.7/src/rc3/common/
+-rw-rw-rw-   0        0        0        0 2024-05-06 19:59:39.000000 rc3-0.0.7/src/rc3/common/__init__.py
+-rw-rw-rw-   0        0        0     1366 2024-05-25 12:49:39.000000 rc3-0.0.7/src/rc3/common/config_helper.py
+-rw-rw-rw-   0        0        0      869 2024-05-06 22:59:13.000000 rc3-0.0.7/src/rc3/common/data_helper.py
+-rw-rw-rw-   0        0        0      936 2024-05-06 19:59:39.000000 rc3-0.0.7/src/rc3/common/decorators.py
+-rw-rw-rw-   0        0        0     3394 2024-05-25 16:57:33.000000 rc3-0.0.7/src/rc3/common/env_helper.py
+-rw-rw-rw-   0        0        0     1364 2024-05-06 22:52:57.000000 rc3-0.0.7/src/rc3/common/inherit_helper.py
+-rw-rw-rw-   0        0        0    10968 2024-05-25 14:11:47.000000 rc3-0.0.7/src/rc3/common/json_helper.py
+-rw-rw-rw-   0        0        0     2503 2024-05-08 19:08:29.000000 rc3-0.0.7/src/rc3/common/print_helper.py
+-rw-rw-rw-   0        0        0       86 2024-05-06 19:59:39.000000 rc3-0.0.7/src/rc3/common/rc_globals.py
+drwxrwxrwx   0        0        0        0 2024-05-25 17:54:45.485570 rc3-0.0.7/src/rc3/data/
+-rw-rw-rw-   0        0        0        0 2024-05-06 19:59:39.000000 rc3-0.0.7/src/rc3/data/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-25 17:54:45.486570 rc3-0.0.7/src/rc3/data/collection/
+drwxrwxrwx   0        0        0        0 2024-05-25 17:54:45.490568 rc3-0.0.7/src/rc3/data/collection/environments/
+-rw-rw-rw-   0        0        0        6 2024-05-15 19:30:06.000000 rc3-0.0.7/src/rc3/data/collection/environments/.gitignore
+-rw-rw-rw-   0        0        0      277 2024-05-07 23:02:08.000000 rc3-0.0.7/src/rc3/data/collection/environments/dev.defaults
+-rw-rw-rw-   0        0        0      307 2024-05-07 23:02:08.000000 rc3-0.0.7/src/rc3/data/collection/environments/localhost.defaults
+drwxrwxrwx   0        0        0        0 2024-05-25 17:54:45.511555 rc3-0.0.7/src/rc3/data/collection/examples/
+-rw-rw-rw-   0        0        0      247 2024-05-07 23:02:08.000000 rc3-0.0.7/src/rc3/data/collection/examples/example_Auth_Basic.request
+-rw-rw-rw-   0        0        0      914 2024-05-07 23:02:08.000000 rc3-0.0.7/src/rc3/data/collection/examples/example_Auth_Bearer.request
+-rw-rw-rw-   0        0        0      960 2024-05-07 23:02:08.000000 rc3-0.0.7/src/rc3/data/collection/examples/example_Auth_Token.request
+-rw-rw-rw-   0        0        0      436 2024-05-07 23:02:08.000000 rc3-0.0.7/src/rc3/data/collection/examples/example_Extract_JsonPath.request
+-rw-rw-rw-   0        0        0      455 2024-05-07 23:02:08.000000 rc3-0.0.7/src/rc3/data/collection/examples/example_Extract_Regex.request
+-rw-rw-rw-   0        0        0      190 2024-05-07 23:02:08.000000 rc3-0.0.7/src/rc3/data/collection/examples/example_GET.request
+-rw-rw-rw-   0        0        0      799 2024-05-07 23:02:08.000000 rc3-0.0.7/src/rc3/data/collection/examples/example_KitchenSink.request
+-rw-rw-rw-   0        0        0      401 2024-05-07 23:02:08.000000 rc3-0.0.7/src/rc3/data/collection/examples/example_MintOauth2Token.request
+-rw-rw-rw-   0        0        0      275 2024-05-07 23:02:08.000000 rc3-0.0.7/src/rc3/data/collection/examples/example_POST_json.request
+-rw-rw-rw-   0        0        0      231 2024-05-07 23:02:08.000000 rc3-0.0.7/src/rc3/data/collection/examples/example_POST_text-plain.request
+-rw-rw-rw-   0        0        0      240 2024-05-07 23:02:08.000000 rc3-0.0.7/src/rc3/data/collection/examples/example_QueryParams.request
+-rw-rw-rw-   0        0        0      227 2024-05-07 23:02:08.000000 rc3-0.0.7/src/rc3/data/collection/examples/example_UseOauth2Token.request
+-rw-rw-rw-   0        0        0      272 2024-05-07 23:02:08.000000 rc3-0.0.7/src/rc3/data/collection/examples/folder.json
+drwxrwxrwx   0        0        0        0 2024-05-25 17:54:45.522548 rc3-0.0.7/src/rc3/data/collection/greetings-basic/
+-rw-rw-rw-   0        0        0      384 2024-05-07 23:02:08.000000 rc3-0.0.7/src/rc3/data/collection/greetings-basic/greeting.request
+-rw-rw-rw-   0        0        0      180 2024-05-07 23:02:08.000000 rc3-0.0.7/src/rc3/data/collection/greetings-basic/greetings.request
+-rw-rw-rw-   0        0        0      291 2024-05-07 23:02:08.000000 rc3-0.0.7/src/rc3/data/collection/greetings-basic/new-greeting.request
+-rw-rw-rw-   0        0        0      297 2024-05-07 23:02:08.000000 rc3-0.0.7/src/rc3/data/collection/greetings-basic/rc-folder.json
+-rw-rw-rw-   0        0        0      185 2024-05-07 23:02:08.000000 rc3-0.0.7/src/rc3/data/collection/greetings-basic/remove-greeting.request
+-rw-rw-rw-   0        0        0      313 2024-05-07 23:02:08.000000 rc3-0.0.7/src/rc3/data/collection/greetings-basic/update-greeting.request
+drwxrwxrwx   0        0        0        0 2024-05-25 17:54:45.527545 rc3-0.0.7/src/rc3/data/collection/greetings-oauth2/
+-rw-rw-rw-   0        0        0      218 2024-05-07 23:02:08.000000 rc3-0.0.7/src/rc3/data/collection/greetings-oauth2/greeting.request
+-rw-rw-rw-   0        0        0      466 2024-05-07 23:02:08.000000 rc3-0.0.7/src/rc3/data/collection/greetings-oauth2/mint-admin-token.request
+-rw-rw-rw-   0        0        0      465 2024-05-07 23:02:08.000000 rc3-0.0.7/src/rc3/data/collection/greetings-oauth2/mint-token.request
+-rw-rw-rw-   0        0        0      247 2024-05-08 14:58:01.000000 rc3-0.0.7/src/rc3/data/collection/rc-collection.json
+drwxrwxrwx   0        0        0        0 2024-05-25 17:54:45.530544 rc3-0.0.7/src/rc3/data/home/
+-rw-rw-rw-   0        0        0      130 2024-05-07 23:02:08.000000 rc3-0.0.7/src/rc3/data/home/rc-global.json
+-rw-rw-rw-   0        0        0      354 2024-05-07 23:02:39.000000 rc3-0.0.7/src/rc3/data/home/rc-settings.json
+drwxrwxrwx   0        0        0        0 2024-05-25 17:54:45.542535 rc3-0.0.7/src/rc3/data/home/schemas/
+-rw-rw-rw-   0        0        0     1151 2024-05-07 23:02:08.000000 rc3-0.0.7/src/rc3/data/home/schemas/rc3-auth-0.0.3.json
+-rw-rw-rw-   0        0        0      918 2024-05-07 23:02:08.000000 rc3-0.0.7/src/rc3/data/home/schemas/rc3-collection-0.0.3.json
+-rw-rw-rw-   0        0        0      473 2024-05-07 23:02:08.000000 rc3-0.0.7/src/rc3/data/home/schemas/rc3-environment-0.0.3.json
+-rw-rw-rw-   0        0        0      605 2024-05-07 23:02:08.000000 rc3-0.0.7/src/rc3/data/home/schemas/rc3-folder-0.0.3.json
+-rw-rw-rw-   0        0        0     3241 2024-05-07 23:02:08.000000 rc3-0.0.7/src/rc3/data/home/schemas/rc3-request-0.0.3.json
+-rw-rw-rw-   0        0        0     2259 2024-05-07 23:02:08.000000 rc3-0.0.7/src/rc3/data/home/schemas/rc3-settings-0.0.3.json
+drwxrwxrwx   0        0        0        0 2024-05-25 17:54:45.609495 rc3-0.0.7/src/rc3.egg-info/
+-rw-rw-rw-   0        0        0    13086 2024-05-25 17:54:45.000000 rc3-0.0.7/src/rc3.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5253 2024-05-25 17:54:45.000000 rc3-0.0.7/src/rc3.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 17:54:45.000000 rc3-0.0.7/src/rc3.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2024-05-25 17:54:45.000000 rc3-0.0.7/src/rc3.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      100 2024-05-25 17:54:45.000000 rc3-0.0.7/src/rc3.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-05-25 17:54:45.000000 rc3-0.0.7/src/rc3.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-25 17:54:45.544535 rc3-0.0.7/temp-collection/
+drwxrwxrwx   0        0        0        0 2024-05-25 17:54:45.552530 rc3-0.0.7/temp-collection/environments/
+-rw-rw-rw-   0        0        0        6 2024-05-15 19:30:06.000000 rc3-0.0.7/temp-collection/environments/.gitignore
+-rw-rw-rw-   0        0        0      277 2024-05-07 23:02:08.000000 rc3-0.0.7/temp-collection/environments/dev.defaults
+-rw-rw-rw-   0        0        0      307 2024-05-07 23:02:08.000000 rc3-0.0.7/temp-collection/environments/localhost.defaults
+drwxrwxrwx   0        0        0        0 2024-05-25 17:54:45.568520 rc3-0.0.7/temp-collection/examples/
+-rw-rw-rw-   0        0        0      247 2024-05-07 23:02:08.000000 rc3-0.0.7/temp-collection/examples/example_Auth_Basic.request
+-rw-rw-rw-   0        0        0      914 2024-05-07 23:02:08.000000 rc3-0.0.7/temp-collection/examples/example_Auth_Bearer.request
+-rw-rw-rw-   0        0        0      960 2024-05-07 23:02:08.000000 rc3-0.0.7/temp-collection/examples/example_Auth_Token.request
+-rw-rw-rw-   0        0        0      436 2024-05-07 23:02:08.000000 rc3-0.0.7/temp-collection/examples/example_Extract_JsonPath.request
+-rw-rw-rw-   0        0        0      455 2024-05-07 23:02:08.000000 rc3-0.0.7/temp-collection/examples/example_Extract_Regex.request
+-rw-rw-rw-   0        0        0      190 2024-05-07 23:02:08.000000 rc3-0.0.7/temp-collection/examples/example_GET.request
+-rw-rw-rw-   0        0        0      799 2024-05-07 23:02:08.000000 rc3-0.0.7/temp-collection/examples/example_KitchenSink.request
+-rw-rw-rw-   0        0        0      401 2024-05-07 23:02:08.000000 rc3-0.0.7/temp-collection/examples/example_MintOauth2Token.request
+-rw-rw-rw-   0        0        0      275 2024-05-07 23:02:08.000000 rc3-0.0.7/temp-collection/examples/example_POST_json.request
+-rw-rw-rw-   0        0        0      231 2024-05-07 23:02:08.000000 rc3-0.0.7/temp-collection/examples/example_POST_text-plain.request
+-rw-rw-rw-   0        0        0      240 2024-05-07 23:02:08.000000 rc3-0.0.7/temp-collection/examples/example_QueryParams.request
+-rw-rw-rw-   0        0        0      227 2024-05-07 23:02:08.000000 rc3-0.0.7/temp-collection/examples/example_UseOauth2Token.request
+-rw-rw-rw-   0        0        0      272 2024-05-07 23:02:08.000000 rc3-0.0.7/temp-collection/examples/folder.json
+drwxrwxrwx   0        0        0        0 2024-05-25 17:54:45.575516 rc3-0.0.7/temp-collection/greetings-basic/
+-rw-rw-rw-   0        0        0      384 2024-05-07 23:02:08.000000 rc3-0.0.7/temp-collection/greetings-basic/greeting.request
+-rw-rw-rw-   0        0        0      180 2024-05-07 23:02:08.000000 rc3-0.0.7/temp-collection/greetings-basic/greetings.request
+-rw-rw-rw-   0        0        0      291 2024-05-07 23:02:08.000000 rc3-0.0.7/temp-collection/greetings-basic/new-greeting.request
+-rw-rw-rw-   0        0        0      297 2024-05-07 23:02:08.000000 rc3-0.0.7/temp-collection/greetings-basic/rc-folder.json
+-rw-rw-rw-   0        0        0      185 2024-05-07 23:02:08.000000 rc3-0.0.7/temp-collection/greetings-basic/remove-greeting.request
+-rw-rw-rw-   0        0        0      313 2024-05-07 23:02:08.000000 rc3-0.0.7/temp-collection/greetings-basic/update-greeting.request
+drwxrwxrwx   0        0        0        0 2024-05-25 17:54:45.579512 rc3-0.0.7/temp-collection/greetings-oauth2/
+-rw-rw-rw-   0        0        0      218 2024-05-07 23:02:08.000000 rc3-0.0.7/temp-collection/greetings-oauth2/greeting.request
+-rw-rw-rw-   0        0        0      466 2024-05-07 23:02:08.000000 rc3-0.0.7/temp-collection/greetings-oauth2/mint-admin-token.request
+-rw-rw-rw-   0        0        0      465 2024-05-07 23:02:08.000000 rc3-0.0.7/temp-collection/greetings-oauth2/mint-token.request
+-rw-rw-rw-   0        0        0      247 2024-05-08 14:58:01.000000 rc3-0.0.7/temp-collection/rc-collection.json
+drwxrwxrwx   0        0        0        0 2024-05-25 17:54:45.582511 rc3-0.0.7/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-06 19:59:39.000000 rc3-0.0.7/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-25 17:54:45.589507 rc3-0.0.7/tests/commands/
+-rw-rw-rw-   0        0        0        0 2024-05-06 19:59:39.000000 rc3-0.0.7/tests/commands/__init__.py
+-rw-rw-rw-   0        0        0      599 2024-05-06 20:00:31.000000 rc3-0.0.7/tests/commands/test_collection.py
+-rw-rw-rw-   0        0        0     5698 2024-05-06 20:00:31.000000 rc3-0.0.7/tests/commands/test_environment.py
+-rw-rw-rw-   0        0        0      427 2024-05-06 20:00:31.000000 rc3-0.0.7/tests/commands/test_list.py
+-rw-rw-rw-   0        0        0     1915 2024-05-25 14:50:57.000000 rc3-0.0.7/tests/commands/test_new.py
+-rw-rw-rw-   0        0        0     5923 2024-05-06 20:00:31.000000 rc3-0.0.7/tests/commands/test_request.py
+-rw-rw-rw-   0        0        0     6322 2024-05-06 20:00:31.000000 rc3-0.0.7/tests/commands/test_send.py
+drwxrwxrwx   0        0        0        0 2024-05-25 17:54:45.600500 rc3-0.0.7/tests/commands/test_send_files/
+-rw-rw-rw-   0        0        0      263 2024-05-06 19:59:39.000000 rc3-0.0.7/tests/commands/test_send_files/test_is_verbose.yaml
+-rw-rw-rw-   0        0        0     1178 2024-05-06 19:59:39.000000 rc3-0.0.7/tests/commands/test_send_files/test_mint_extract_use_token.yaml
+-rw-rw-rw-   0        0        0      263 2024-05-06 19:59:39.000000 rc3-0.0.7/tests/commands/test_send_files/test_not_verbose.yaml
+-rw-rw-rw-   0        0        0      263 2024-05-06 19:59:39.000000 rc3-0.0.7/tests/commands/test_send_files/test_request_no_responses.yaml
+-rw-rw-rw-   0        0        0      263 2024-05-06 19:59:39.000000 rc3-0.0.7/tests/commands/test_send_files/test_send_1.yaml
+-rw-rw-rw-   0        0        0      663 2024-05-06 19:59:39.000000 rc3-0.0.7/tests/commands/test_send_files/test_send_2.yaml
+-rw-rw-rw-   0        0        0     1098 2024-05-06 19:59:39.000000 rc3-0.0.7/tests/commands/test_send_files/test_send_basics.yaml
+-rw-rw-rw-   0        0        0      263 2024-05-06 19:59:39.000000 rc3-0.0.7/tests/commands/test_send_files/test_settings_no_responses.yaml
+-rw-rw-rw-   0        0        0      263 2024-05-06 19:59:39.000000 rc3-0.0.7/tests/commands/test_send_files/test_settings_with_responses.yaml
+drwxrwxrwx   0        0        0        0 2024-05-25 17:54:45.604498 rc3-0.0.7/tests/common/
+-rw-rw-rw-   0        0        0        0 2024-05-06 19:59:39.000000 rc3-0.0.7/tests/common/__init__.py
+-rw-rw-rw-   0        0        0     8675 2024-05-25 17:12:03.000000 rc3-0.0.7/tests/common/test_env_helper.py
+-rw-rw-rw-   0        0        0     3345 2024-05-06 22:51:48.000000 rc3-0.0.7/tests/common/test_inherit_helper.py
+-rw-rw-rw-   0        0        0     1155 2024-05-25 14:44:52.000000 rc3-0.0.7/tests/conftest.py
+drwxrwxrwx   0        0        0        0 2024-05-25 17:54:45.606497 rc3-0.0.7/tests/learning/
+-rw-rw-rw-   0        0        0        0 2024-05-06 19:59:39.000000 rc3-0.0.7/tests/learning/__init__.py
+-rw-rw-rw-   0        0        0      518 2024-05-06 19:59:39.000000 rc3-0.0.7/tests/learning/test_sample.py
+-rw-rw-rw-   0        0        0     1671 2024-05-25 14:49:50.000000 rc3-0.0.7/tests/test_cli.py
+drwxrwxrwx   0        0        0        0 2024-05-25 17:54:45.608495 rc3-0.0.7/tests/util/
+-rw-rw-rw-   0        0        0        0 2024-05-06 19:59:39.000000 rc3-0.0.7/tests/util/__init__.py
+-rw-rw-rw-   0        0        0     1407 2024-05-06 19:59:39.000000 rc3-0.0.7/tests/util/decorators.py
```

### Comparing `rc3-0.0.6/.gitignore` & `rc3-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `rc3-0.0.6/LICENSE` & `rc3-0.0.7/LICENSE`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2018 Real Python
+Copyright (c) 2024 Gary Wilcox
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `rc3-0.0.6/PKG-INFO` & `rc3-0.0.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: rc3
-Version: 0.0.6
+Version: 0.0.7
 Summary: Rest CLI (rc)
 Home-page: https://github.com/gswilcox01/rc3
 Author: Gary Wilcox
 Author-email: gary@dugan-wilcox.com
 License: MIT License
         
-        Copyright (c) 2018 Real Python
+        Copyright (c) 2024 Gary Wilcox
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
@@ -55,43 +55,61 @@
 ## Overview
 * A Collection is a local directory (optionally checked in as a git repository somewhere).
 * A Collection contains *.request files that each represent a single REST API Request that can be executed
 * The output from executing a *.request file is normally:
     * The HTTP response body to standard out
     * A detailed *.response file saved in the same directory as the *.request file sent
 
-## Installation
+## Installation & Upgrade
 * Pre-reqs
     * Python 3.12+ (required)
     * VSCode (optional, but highly recommended)
 * Install
     * pip install rc3
+* Upgrade
+    * pip install --upgrade rc3
 * Windows User?
     * See:  [Windows Setup Issues](WINDOWS_SETUP.md)
 
-## Setup & Sending your first request
+## Setup & Send your first request
 * First create an empty directory somewhere (any name & location is fine)
   ```
   $ mkdir temp-collection
   $ cd temp-collection
   ```
-* Next run "rc init" to do 0-4 things
-  1. Will create the RC_HOME directory if it doesn't exist.
-  2. Will create RC_HOME/settings, global env, and schemas dir if they don't exist.
-  3. Will initialize a new example Collection if ran from an empty directory.
-  4. Will import the current directory if it contains a valid collection.json file.
-  ```
-  $ rc init
-  Creating C:\Users\Gary\.rc\rc-settings.json
-  Creating C:\Users\Gary\.rc\rc-global.json                            
-  Creating C:\Users\Gary\.rc\schemas                                   
-  CWD is empty, creating sample Collection here: C:\dev\temp-collection
-  Importing collection from: C:\dev\temp-collection
-  2 default environment(s) initialized in your collection
-  Adding collection to global settings: example-collection
+* Next run "rc new" to create a new collection
+  * Choose all default values, and you'll get an example collection you can explore
+  ```
+  $ rc new
+  Enter a NAME for this COLLECTION [temp-collection]:
+  Include example Requests in your new collection? [Y/n]:
+  Importing collection into RC_HOME/rc-settings.json
+  Collection 'temp-collection' has been successfully imported, try 'rc list' next...
+  ```
+* Next run "rc list" to see what's in the example collection you just created
+  ```
+  $ rc list
+  Listing COLLECTIONS found in settings.json:
+  NUM:   NAME:             LOCATION:                             
+  1      example-rc        C:\git\example-rc
+  2*     temp-collection   C:\temp-collection
+  Listing ENVIRONMENTS found in current_collection:
+  NUM:   NAME:       baseUrl:
+  1*     dev         https://greetings-mvrsygo3gq-uc.a.run.app
+  2      localhost   http://localhost:8080
+  Listing REQUESTS found in current_collection:
+  NUM:   FOLDER:             METHOD:   NAME:
+  1*     /greetings-basic    GET       greeting
+  2      /greetings-basic    GET       greetings
+  3      /greetings-basic    POST      new-greeting
+  4      /greetings-basic    DELETE    remove-greeting
+  5      /greetings-basic    PUT       update-greeting
+  6      /greetings-oauth2   GET       greeting
+  7      /greetings-oauth2   POST      mint-admin-token
+  8      /greetings-oauth2   POST      mint-token
   ```
 * Next send the "greeting" request with the rc send command
   * Wait for it…
     * A greetings-demo project is running on Google Cloud Run
     * And it scales down to 0 instances when there is no demand (i.e. your first few requests will be SLOW…)  
   ```
   $ rc send greeting
@@ -178,14 +196,35 @@
     * rc
 * View help for specific sub-commands
     * rc request --help
     * rc collection --help
     * rc environment --help
 
 ## Additional Concepts
+## Import an existing collection from a git repo
+* The example collection you created with the "rc new" command is also checked into a git repository here:
+* https://github.com/gswilcox01/example-rc
+* You can clone & import collections following the example below:
+  ```
+  $ git clone https://github.com/gswilcox01/example-rc.git
+  Cloning into 'example-rc'...
+  remote: Enumerating objects: 33, done.
+  remote: Counting objects: 100% (33/33), done.
+  remote: Compressing objects: 100% (17/17), done.
+  remote: Total 33 (delta 14), reused 33 (delta 14), pack-reused 0
+  Receiving objects: 100% (33/33), 4.87 KiB | 262.00 KiB/s, done.
+  Resolving deltas: 100% (14/14), done.
+  
+  $ cd example-rc 
+  
+  $ rc import
+  Importing collection into RC_HOME/rc-settings.json
+  Collection 'example-rc' has been successfully imported, try 'rc list' next...
+  ```
+
 ## Authentication
 * Authentication can be defined in a Request, Folder, or in the collection.json file in the root of your collection
 * Inheritance is walked until auth is defined, or the root of the collection is found in this order:
     * request > folder > parent folder > collection.json
 * For examples of authentication see the following files in the example collection:
     * /greetings-basic/folder.json
     * /greetings-basic/greeting.request
```

### Comparing `rc3-0.0.6/README.md` & `rc3-0.0.7/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -7,43 +7,61 @@
 ## Overview
 * A Collection is a local directory (optionally checked in as a git repository somewhere).
 * A Collection contains *.request files that each represent a single REST API Request that can be executed
 * The output from executing a *.request file is normally:
     * The HTTP response body to standard out
     * A detailed *.response file saved in the same directory as the *.request file sent
 
-## Installation
+## Installation & Upgrade
 * Pre-reqs
     * Python 3.12+ (required)
     * VSCode (optional, but highly recommended)
 * Install
     * pip install rc3
+* Upgrade
+    * pip install --upgrade rc3
 * Windows User?
     * See:  [Windows Setup Issues](WINDOWS_SETUP.md)
 
-## Setup & Sending your first request
+## Setup & Send your first request
 * First create an empty directory somewhere (any name & location is fine)
   ```
   $ mkdir temp-collection
   $ cd temp-collection
   ```
-* Next run "rc init" to do 0-4 things
-  1. Will create the RC_HOME directory if it doesn't exist.
-  2. Will create RC_HOME/settings, global env, and schemas dir if they don't exist.
-  3. Will initialize a new example Collection if ran from an empty directory.
-  4. Will import the current directory if it contains a valid collection.json file.
-  ```
-  $ rc init
-  Creating C:\Users\Gary\.rc\rc-settings.json
-  Creating C:\Users\Gary\.rc\rc-global.json                            
-  Creating C:\Users\Gary\.rc\schemas                                   
-  CWD is empty, creating sample Collection here: C:\dev\temp-collection
-  Importing collection from: C:\dev\temp-collection
-  2 default environment(s) initialized in your collection
-  Adding collection to global settings: example-collection
+* Next run "rc new" to create a new collection
+  * Choose all default values, and you'll get an example collection you can explore
+  ```
+  $ rc new
+  Enter a NAME for this COLLECTION [temp-collection]:
+  Include example Requests in your new collection? [Y/n]:
+  Importing collection into RC_HOME/rc-settings.json
+  Collection 'temp-collection' has been successfully imported, try 'rc list' next...
+  ```
+* Next run "rc list" to see what's in the example collection you just created
+  ```
+  $ rc list
+  Listing COLLECTIONS found in settings.json:
+  NUM:   NAME:             LOCATION:                             
+  1      example-rc        C:\git\example-rc
+  2*     temp-collection   C:\temp-collection
+  Listing ENVIRONMENTS found in current_collection:
+  NUM:   NAME:       baseUrl:
+  1*     dev         https://greetings-mvrsygo3gq-uc.a.run.app
+  2      localhost   http://localhost:8080
+  Listing REQUESTS found in current_collection:
+  NUM:   FOLDER:             METHOD:   NAME:
+  1*     /greetings-basic    GET       greeting
+  2      /greetings-basic    GET       greetings
+  3      /greetings-basic    POST      new-greeting
+  4      /greetings-basic    DELETE    remove-greeting
+  5      /greetings-basic    PUT       update-greeting
+  6      /greetings-oauth2   GET       greeting
+  7      /greetings-oauth2   POST      mint-admin-token
+  8      /greetings-oauth2   POST      mint-token
   ```
 * Next send the "greeting" request with the rc send command
   * Wait for it…
     * A greetings-demo project is running on Google Cloud Run
     * And it scales down to 0 instances when there is no demand (i.e. your first few requests will be SLOW…)  
   ```
   $ rc send greeting
@@ -130,14 +148,35 @@
     * rc
 * View help for specific sub-commands
     * rc request --help
     * rc collection --help
     * rc environment --help
 
 ## Additional Concepts
+## Import an existing collection from a git repo
+* The example collection you created with the "rc new" command is also checked into a git repository here:
+* https://github.com/gswilcox01/example-rc
+* You can clone & import collections following the example below:
+  ```
+  $ git clone https://github.com/gswilcox01/example-rc.git
+  Cloning into 'example-rc'...
+  remote: Enumerating objects: 33, done.
+  remote: Counting objects: 100% (33/33), done.
+  remote: Compressing objects: 100% (17/17), done.
+  remote: Total 33 (delta 14), reused 33 (delta 14), pack-reused 0
+  Receiving objects: 100% (33/33), 4.87 KiB | 262.00 KiB/s, done.
+  Resolving deltas: 100% (14/14), done.
+  
+  $ cd example-rc 
+  
+  $ rc import
+  Importing collection into RC_HOME/rc-settings.json
+  Collection 'example-rc' has been successfully imported, try 'rc list' next...
+  ```
+
 ## Authentication
 * Authentication can be defined in a Request, Folder, or in the collection.json file in the root of your collection
 * Inheritance is walked until auth is defined, or the root of the collection is found in this order:
     * request > folder > parent folder > collection.json
 * For examples of authentication see the following files in the example collection:
     * /greetings-basic/folder.json
     * /greetings-basic/greeting.request
```

### Comparing `rc3-0.0.6/WINDOWS_SETUP.md` & `rc3-0.0.7/WINDOWS_SETUP.md`

 * *Files identical despite different names*

### Comparing `rc3-0.0.6/pyproject.toml` & `rc3-0.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0","setuptools-scm","wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rc3"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Gary Wilcox" },
   { email="gary@dugan-wilcox.com" }
 ]
 readme = "README.md"
 license = { file = "LICENSE" }
 description = "Rest CLI (rc)"
```

### Comparing `rc3-0.0.6/src/rc3/archive/cmd_root.py` & `rc3-0.0.7/src/rc3/archive/cmd_root.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.6/src/rc3/archive/cmd_subs.py` & `rc3-0.0.7/src/rc3/archive/cmd_subs.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.6/src/rc3/commands/cmd_collection.py` & `rc3-0.0.7/src/rc3/commands/cmd_collection.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.6/src/rc3/commands/cmd_environment.py` & `rc3-0.0.7/src/rc3/commands/cmd_environment.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.6/src/rc3/commands/cmd_global.py` & `rc3-0.0.7/src/rc3/commands/cmd_global.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.6/src/rc3/commands/cmd_hello.py` & `rc3-0.0.7/src/rc3/commands/cmd_hello.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.6/src/rc3/commands/cmd_init.py` & `rc3-0.0.7/src/rc3/archive/cmd_init.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.6/src/rc3/commands/cmd_list.py` & `rc3-0.0.7/src/rc3/commands/cmd_list.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.6/src/rc3/commands/cmd_request.py` & `rc3-0.0.7/src/rc3/commands/cmd_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import json
 import os
 import click
 
-from rc3.commands import cmd_list
+from rc3.commands import cmd_list, cmd_send
 from rc3.common import json_helper, print_helper
 
 
 @click.command("request", short_help="Manage REQUESTS in current_collection.")
 @click.option('-l', '--list', '_list', is_flag=True, default=False, help="List REQUESTS in collection.")
 @click.option('-n', '--new', is_flag=True, default=False, help="Create a new REQUEST.")
 @click.option('-i', '--info', is_flag=True, default=False, help="Display json of current REQUEST.")
 @click.option('-p', '--pick', is_flag=True, default=False, help="Pick an item as current REQUEST.")
 @click.option('-e', '--edit', is_flag=True, default=False, help="Edit a REQUEST with system editor.")
+@click.option('-s', '--send', is_flag=True, default=False, help="Send the current REQUEST.")
 @click.argument('request_name', type=str, required=False)
-def cli(_list, new, info, pick, edit, request_name):
+def cli(_list, new, info, pick, edit, send, request_name):
     """\b
     Manages REQUEST objects/files in the current collection.
 
     \b
     REQUEST_NAME is optional.
     REQUEST_NAME will default to the current_request, or prompt you to pick.
     REQUEST_NAME if used should be one of:
@@ -26,26 +27,33 @@
 
     """
     if _list:
         cmd_list.list_requests()
     elif new:
         click.echo("NOT IMPLEMENTED! Please use VSCode to edit your collection.")
     elif edit:
-        edit_request(request_name)
+        r = edit_request(request_name)
+        if send: cmd_send.send(r)
     elif info:
         print_info(request_name)
     elif pick:
-        pick_request(request_name)
+        r = pick_request(request_name)
+        if send: cmd_send.send(r)
+    elif send:
+        cmd_send.lookup_and_send(request_name)
     elif request_name is None:
         # DEFAULT to list() if no REQUEST_NAME
         cmd_list.list_requests()
     else:
         # DEFAULT to pick() if REQUEST_NAME
         pick_request(request_name)
 
+    # if send:
+    #     cmd_send.lookup_and_send(request_name)
+
 
 def pick_request(name=None):
     r = lookup_or_prompt(name)
     if r is None:
         return None
 
     c, c_wrapper = json_helper.read_current_collection()
@@ -124,8 +132,7 @@
         return None
 
 
 def save_request(r, wrapper):
     json_helper.write_request(r, wrapper)
     print("REQUEST saved: ")
     print(wrapper.get('_display_ref'))
-
```

### Comparing `rc3-0.0.6/src/rc3/commands/cmd_send.py` & `rc3-0.0.7/src/rc3/commands/cmd_send.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,16 +36,20 @@
     elif pick:
         r = cmd_request.pick_request(request_name)
         send(r)
     elif edit:
         r = cmd_request.edit_request(request_name)
         send(r)
     else:
-        r = lookup_request(request_name)
-        send(r)
+        lookup_and_send(request_name)
+
+
+def lookup_and_send(request_name):
+    r = lookup_request(request_name)
+    send(r)
 
 
 def lookup_request(request_name):
     r = cmd_request.lookup_request(request_name)
     if r is None and request_name is None:
         raise click.ClickException("There is no current REQUEST, exiting...")
     if r is None:
```

### Comparing `rc3-0.0.6/src/rc3/commands/cmd_settings.py` & `rc3-0.0.7/src/rc3/commands/cmd_settings.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.6/src/rc3/common/data_helper.py` & `rc3-0.0.7/src/rc3/common/data_helper.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.6/src/rc3/common/decorators.py` & `rc3-0.0.7/src/rc3/common/decorators.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.6/src/rc3/common/env_helper.py` & `rc3-0.0.7/src/rc3/common/env_helper.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import json
 import os
 import re
 import click
 
 from rc3.common import json_helper, print_helper
 
+PATTERN = re.compile(r'{{(.*?)}}')
+
 
 def process_subs(wrapper):
     if has_vars(wrapper):
         sub_vars(wrapper)
     # print_helper.print_json(r.get('_original', None))
 
 
@@ -35,62 +37,78 @@
     if _json is not None:
         json_string = json.dumps(_json)
         new_string = sub_in_string(envs, json_string)
         if new_string != json_string:
             r.get('body')['json'] = json.loads(new_string)
 
 
-def lookup_var_value(envs, var):
+def lookup_var_value(envs, var, seen=None):
+    # seen just holds vars that have already seen for THIS lookup
+    # if already seen, then we have an infinite loop...
+    if seen is None:
+        seen = []
+    if var in seen:
+        raise click.ClickException(
+            f'var {{{{{var}}}}} has caused an infinite loop during lookup, please check/update your vars!')
+    else:
+        seen.append(var)
+
     for env in envs:
         if var in env:
-            return env.get(var)
-    raise click.ClickException(f'var {{{{{var}}}}} is in the REQUEST but cannot be found in the current, global, or OS environment')
+            outer_value = env.get(var)
+            for match in PATTERN.finditer(outer_value):
+                inner_var = match.group(1).strip()
+                inner_value = lookup_var_value(envs, inner_var, seen)
+                outer_value = outer_value.replace(match.group(0), inner_value)
+            return outer_value
+    raise click.ClickException(
+        f'var {{{{{var}}}}} is in the REQUEST but cannot be found in the current, global, or OS environment')
 
 
 def sub_in_dict(envs, d):
     if d is None:
         return
-    pattern = re.compile(r'{{(.*?)}}')
+    # pattern = re.compile(r'{{(.*?)}}')
     for key, value in d.items():
         new_value = value
-        for match in pattern.finditer(value):
+        for match in PATTERN.finditer(value):
             var = match.group(1).strip()
             var_value = lookup_var_value(envs, var)
             # this allows multiple vars to be used in a single value (each gets replaced)
             new_value = new_value.replace(match.group(0), var_value)
         d[key] = new_value
 
 
 def sub_in_string(envs, s):
     if s is None:
         return None
-    pattern = re.compile(r'{{(.*?)}}')
-    for match in pattern.finditer(s):
+    # pattern = re.compile(r'{{(.*?)}}')
+    for match in PATTERN.finditer(s):
         var = match.group(1).strip()
         var_value = lookup_var_value(envs, var)
         s = s.replace(match.group(0), var_value)
     return s
 
 
 def has_vars(wrapper):
     r = wrapper.get('_original')
     dicts = [
-        r.get('form_data',{}),
-        r.get('headers',{}),
-        r.get('params',{}),
-        r.get('auth',{})
+        r.get('form_data', {}),
+        r.get('headers', {}),
+        r.get('params', {}),
+        r.get('auth', {})
     ]
     strings = [
-        r.get('url',''),
-        r.get('body', {}).get('text',''),
-        json.dumps(r.get('body', {}).get('json',{}))
+        r.get('url', ''),
+        r.get('body', {}).get('text', ''),
+        json.dumps(r.get('body', {}).get('json', {}))
     ]
     for d in dicts:
         for v in d.values():
             strings.append(v)
 
-    pattern = re.compile(r'{{(.*?)}}')
+    # pattern = re.compile(r'{{(.*?)}}')
     for s in strings:
-        match = pattern.search(s)
+        match = PATTERN.search(s)
         if match is not None:
             return True
     return False
```

### Comparing `rc3-0.0.6/src/rc3/common/inherit_helper.py` & `rc3-0.0.7/src/rc3/common/inherit_helper.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.6/src/rc3/common/json_helper.py` & `rc3-0.0.7/src/rc3/common/json_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,14 +118,15 @@
         # print(vars(error)) # use to look at what other attributes are available...
         print(" * json path: /" + '.'.join(error.path))
         print(" * error: " + error.message)
     print("If needed, please use VSCode to see validation errors w/ squiggles & hovers")
     sys.exit()
 
 
+@rc_print_durations
 def validate_schemas():
     check_schema(data_helper.get_schema_file('auth'))
     check_schema(data_helper.get_schema_file('collection'))
     check_schema(data_helper.get_schema_file('environment'))
     check_schema(data_helper.get_schema_file('folder'))
     check_schema(data_helper.get_schema_file('request'))
     check_schema(data_helper.get_schema_file('settings'))
@@ -196,17 +197,27 @@
     c = load_and_validate(COLLECTION_FILENAME, _dir=current['location'])
     return c, {
         '_dir': current['location'],
         '_original': c
     }
 
 
-def write_collection(c):
-    location = c['_dir']
-    write_json(os.path.join(location, COLLECTION_FILENAME), c['_original'])
+def read_collection(_dir=None):
+    if _dir is None:
+        _dir = os.getcwd()
+    c = load_and_validate(COLLECTION_FILENAME, _dir=_dir)
+    return c, {
+        '_dir': _dir,
+        '_original': c
+    }
+
+
+def write_collection(wrapper):
+    location = wrapper['_dir']
+    write_json(os.path.join(location, COLLECTION_FILENAME), wrapper['_original'])
 
 
 @rc_print_durations
 @rc_memoized
 def read_request_list():
     c, c_wrapper = read_current_collection()
     root = c_wrapper['_dir']
```

### Comparing `rc3-0.0.6/src/rc3/common/print_helper.py` & `rc3-0.0.7/src/rc3/common/print_helper.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.6/src/rc3/data/collection/examples/example_Auth_Bearer.request` & `rc3-0.0.7/src/rc3/data/collection/examples/example_Auth_Bearer.request`

 * *Files identical despite different names*

### Comparing `rc3-0.0.6/src/rc3/data/collection/examples/example_Auth_Token.request` & `rc3-0.0.7/src/rc3/data/collection/examples/example_Auth_Token.request`

 * *Files identical despite different names*

### Comparing `rc3-0.0.6/src/rc3/data/collection/examples/example_KitchenSink.request` & `rc3-0.0.7/src/rc3/data/collection/examples/example_KitchenSink.request`

 * *Files identical despite different names*

### Comparing `rc3-0.0.6/src/rc3/data/home/schemas/rc3-auth-0.0.3.json` & `rc3-0.0.7/src/rc3/data/home/schemas/rc3-auth-0.0.3.json`

 * *Files identical despite different names*

### Comparing `rc3-0.0.6/src/rc3/data/home/schemas/rc3-collection-0.0.3.json` & `rc3-0.0.7/src/rc3/data/home/schemas/rc3-collection-0.0.3.json`

 * *Files identical despite different names*

### Comparing `rc3-0.0.6/src/rc3/data/home/schemas/rc3-folder-0.0.3.json` & `rc3-0.0.7/src/rc3/data/home/schemas/rc3-folder-0.0.3.json`

 * *Files identical despite different names*

### Comparing `rc3-0.0.6/src/rc3/data/home/schemas/rc3-request-0.0.3.json` & `rc3-0.0.7/src/rc3/data/home/schemas/rc3-request-0.0.3.json`

 * *Files identical despite different names*

### Comparing `rc3-0.0.6/src/rc3/data/home/schemas/rc3-settings-0.0.3.json` & `rc3-0.0.7/src/rc3/data/home/schemas/rc3-settings-0.0.3.json`

 * *Files identical despite different names*

### Comparing `rc3-0.0.6/src/rc3.egg-info/PKG-INFO` & `rc3-0.0.7/src/rc3.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: rc3
-Version: 0.0.6
+Version: 0.0.7
 Summary: Rest CLI (rc)
 Home-page: https://github.com/gswilcox01/rc3
 Author: Gary Wilcox
 Author-email: gary@dugan-wilcox.com
 License: MIT License
         
-        Copyright (c) 2018 Real Python
+        Copyright (c) 2024 Gary Wilcox
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
@@ -55,43 +55,61 @@
 ## Overview
 * A Collection is a local directory (optionally checked in as a git repository somewhere).
 * A Collection contains *.request files that each represent a single REST API Request that can be executed
 * The output from executing a *.request file is normally:
     * The HTTP response body to standard out
     * A detailed *.response file saved in the same directory as the *.request file sent
 
-## Installation
+## Installation & Upgrade
 * Pre-reqs
     * Python 3.12+ (required)
     * VSCode (optional, but highly recommended)
 * Install
     * pip install rc3
+* Upgrade
+    * pip install --upgrade rc3
 * Windows User?
     * See:  [Windows Setup Issues](WINDOWS_SETUP.md)
 
-## Setup & Sending your first request
+## Setup & Send your first request
 * First create an empty directory somewhere (any name & location is fine)
   ```
   $ mkdir temp-collection
   $ cd temp-collection
   ```
-* Next run "rc init" to do 0-4 things
-  1. Will create the RC_HOME directory if it doesn't exist.
-  2. Will create RC_HOME/settings, global env, and schemas dir if they don't exist.
-  3. Will initialize a new example Collection if ran from an empty directory.
-  4. Will import the current directory if it contains a valid collection.json file.
-  ```
-  $ rc init
-  Creating C:\Users\Gary\.rc\rc-settings.json
-  Creating C:\Users\Gary\.rc\rc-global.json                            
-  Creating C:\Users\Gary\.rc\schemas                                   
-  CWD is empty, creating sample Collection here: C:\dev\temp-collection
-  Importing collection from: C:\dev\temp-collection
-  2 default environment(s) initialized in your collection
-  Adding collection to global settings: example-collection
+* Next run "rc new" to create a new collection
+  * Choose all default values, and you'll get an example collection you can explore
+  ```
+  $ rc new
+  Enter a NAME for this COLLECTION [temp-collection]:
+  Include example Requests in your new collection? [Y/n]:
+  Importing collection into RC_HOME/rc-settings.json
+  Collection 'temp-collection' has been successfully imported, try 'rc list' next...
+  ```
+* Next run "rc list" to see what's in the example collection you just created
+  ```
+  $ rc list
+  Listing COLLECTIONS found in settings.json:
+  NUM:   NAME:             LOCATION:                             
+  1      example-rc        C:\git\example-rc
+  2*     temp-collection   C:\temp-collection
+  Listing ENVIRONMENTS found in current_collection:
+  NUM:   NAME:       baseUrl:
+  1*     dev         https://greetings-mvrsygo3gq-uc.a.run.app
+  2      localhost   http://localhost:8080
+  Listing REQUESTS found in current_collection:
+  NUM:   FOLDER:             METHOD:   NAME:
+  1*     /greetings-basic    GET       greeting
+  2      /greetings-basic    GET       greetings
+  3      /greetings-basic    POST      new-greeting
+  4      /greetings-basic    DELETE    remove-greeting
+  5      /greetings-basic    PUT       update-greeting
+  6      /greetings-oauth2   GET       greeting
+  7      /greetings-oauth2   POST      mint-admin-token
+  8      /greetings-oauth2   POST      mint-token
   ```
 * Next send the "greeting" request with the rc send command
   * Wait for it…
     * A greetings-demo project is running on Google Cloud Run
     * And it scales down to 0 instances when there is no demand (i.e. your first few requests will be SLOW…)  
   ```
   $ rc send greeting
@@ -178,14 +196,35 @@
     * rc
 * View help for specific sub-commands
     * rc request --help
     * rc collection --help
     * rc environment --help
 
 ## Additional Concepts
+## Import an existing collection from a git repo
+* The example collection you created with the "rc new" command is also checked into a git repository here:
+* https://github.com/gswilcox01/example-rc
+* You can clone & import collections following the example below:
+  ```
+  $ git clone https://github.com/gswilcox01/example-rc.git
+  Cloning into 'example-rc'...
+  remote: Enumerating objects: 33, done.
+  remote: Counting objects: 100% (33/33), done.
+  remote: Compressing objects: 100% (17/17), done.
+  remote: Total 33 (delta 14), reused 33 (delta 14), pack-reused 0
+  Receiving objects: 100% (33/33), 4.87 KiB | 262.00 KiB/s, done.
+  Resolving deltas: 100% (14/14), done.
+  
+  $ cd example-rc 
+  
+  $ rc import
+  Importing collection into RC_HOME/rc-settings.json
+  Collection 'example-rc' has been successfully imported, try 'rc list' next...
+  ```
+
 ## Authentication
 * Authentication can be defined in a Request, Folder, or in the collection.json file in the root of your collection
 * Inheritance is walked until auth is defined, or the root of the collection is found in this order:
     * request > folder > parent folder > collection.json
 * For examples of authentication see the following files in the example collection:
     * /greetings-basic/folder.json
     * /greetings-basic/greeting.request
```

### Comparing `rc3-0.0.6/src/rc3.egg-info/SOURCES.txt` & `rc3-0.0.7/src/rc3.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -11,23 +11,25 @@
 src/rc3.egg-info/SOURCES.txt
 src/rc3.egg-info/dependency_links.txt
 src/rc3.egg-info/entry_points.txt
 src/rc3.egg-info/requires.txt
 src/rc3.egg-info/top_level.txt
 src/rc3/archive/__init__.py
 src/rc3/archive/cmd_home.py
+src/rc3/archive/cmd_init.py
 src/rc3/archive/cmd_root.py
 src/rc3/archive/cmd_subs.py
 src/rc3/commands/__init__.py
 src/rc3/commands/cmd_collection.py
 src/rc3/commands/cmd_environment.py
 src/rc3/commands/cmd_global.py
 src/rc3/commands/cmd_hello.py
-src/rc3/commands/cmd_init.py
+src/rc3/commands/cmd_import.py
 src/rc3/commands/cmd_list.py
+src/rc3/commands/cmd_new.py
 src/rc3/commands/cmd_request.py
 src/rc3/commands/cmd_send.py
 src/rc3/commands/cmd_settings.py
 src/rc3/common/__init__.py
 src/rc3/common/config_helper.py
 src/rc3/common/data_helper.py
 src/rc3/common/decorators.py
@@ -99,16 +101,16 @@
 temp-collection/greetings-oauth2/mint-token.request
 tests/__init__.py
 tests/conftest.py
 tests/test_cli.py
 tests/commands/__init__.py
 tests/commands/test_collection.py
 tests/commands/test_environment.py
-tests/commands/test_init.py
 tests/commands/test_list.py
+tests/commands/test_new.py
 tests/commands/test_request.py
 tests/commands/test_send.py
 tests/commands/test_send_files/test_is_verbose.yaml
 tests/commands/test_send_files/test_mint_extract_use_token.yaml
 tests/commands/test_send_files/test_not_verbose.yaml
 tests/commands/test_send_files/test_request_no_responses.yaml
 tests/commands/test_send_files/test_send_1.yaml
```

### Comparing `rc3-0.0.6/temp-collection/examples/example_Auth_Bearer.request` & `rc3-0.0.7/temp-collection/examples/example_Auth_Bearer.request`

 * *Files identical despite different names*

### Comparing `rc3-0.0.6/temp-collection/examples/example_Auth_Token.request` & `rc3-0.0.7/temp-collection/examples/example_Auth_Token.request`

 * *Files identical despite different names*

### Comparing `rc3-0.0.6/temp-collection/examples/example_KitchenSink.request` & `rc3-0.0.7/temp-collection/examples/example_KitchenSink.request`

 * *Files identical despite different names*

### Comparing `rc3-0.0.6/tests/commands/test_collection.py` & `rc3-0.0.7/tests/commands/test_collection.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.6/tests/commands/test_environment.py` & `rc3-0.0.7/tests/commands/test_environment.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.6/tests/commands/test_init.py` & `rc3-0.0.7/tests/commands/test_new.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,47 +4,47 @@
 import pytest
 
 from rc3 import cli
 from rc3.common import json_helper, config_helper
 from rc3.common.data_helper import SETTINGS_FILENAME, COLLECTION_FILENAME, GLOBAL_ENV_FILENAME
 
 
-def test_init_from_empty(clean_home, clean_empty, runner):
+def test_new_from_empty(clean_home, clean_empty, runner):
     # pre-test RC_HOME doesn't exist
     rc_home = os.path.join(clean_home, '.rc')
     assert not os.path.exists(rc_home)
 
     # change to empty dir, and run init
     os.chdir(clean_empty)
-    result = runner.invoke(cli.cli, ['init'])
+    result = runner.invoke(cli.cli, ['new'], input='example-collection\n\n')
     assert result.exit_code == 0
 
     # test it exists now AND is empty
     assert os.path.exists(rc_home)
     assert os.listdir(rc_home) == [GLOBAL_ENV_FILENAME, SETTINGS_FILENAME, 'schemas']
     assert os.listdir(clean_empty) == ['environments',
                                        'examples',
                                        'greetings-basic',
                                        'greetings-oauth2',
                                        COLLECTION_FILENAME]
     settings = json_helper.read_settings()
     assert settings.get('current_collection') == "example-collection"
 
 
-def test_init_from_NOT_empty(clean_home, clean_empty, runner):
+def test_new_from_NOT_empty(clean_home, clean_empty, runner):
     # pre-test RC_HOME doesn't exist
     rc_home = os.path.join(clean_home, '.rc')
     assert not os.path.exists(rc_home)
 
     # change to empty dir, create tempfile
-    # and then run init
+    # and then run new
     os.chdir(clean_empty)
     json_helper.write_json("temp.json",{})
-    result = runner.invoke(cli.cli, ['init'])
-    assert result.exit_code == 0
+    result = runner.invoke(cli.cli, ['new'], input='example-collection\n\n')
+    assert result.exit_code == 1
 
     # test that we DO STILL init RC_HOME
     assert os.path.exists(rc_home)
     assert os.listdir(rc_home) == [GLOBAL_ENV_FILENAME, SETTINGS_FILENAME, 'schemas']
     # BUT we DON'T init the CWD, or import a collection
     assert os.listdir(clean_empty) == ['temp.json']
     settings = json_helper.read_settings()
```

### Comparing `rc3-0.0.6/tests/commands/test_request.py` & `rc3-0.0.7/tests/commands/test_request.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.6/tests/commands/test_send.py` & `rc3-0.0.7/tests/commands/test_send.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.6/tests/commands/test_send_files/test_mint_extract_use_token.yaml` & `rc3-0.0.7/tests/commands/test_send_files/test_mint_extract_use_token.yaml`

 * *Files identical despite different names*

### Comparing `rc3-0.0.6/tests/commands/test_send_files/test_send_2.yaml` & `rc3-0.0.7/tests/commands/test_send_files/test_send_2.yaml`

 * *Files identical despite different names*

### Comparing `rc3-0.0.6/tests/commands/test_send_files/test_send_basics.yaml` & `rc3-0.0.7/tests/commands/test_send_files/test_send_basics.yaml`

 * *Files identical despite different names*

### Comparing `rc3-0.0.6/tests/common/test_env_helper.py` & `rc3-0.0.7/tests/common/test_env_helper.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 import re
 
+import click
 import pytest
 from click import ClickException
 
 from rc3 import cli
 from rc3.common import json_helper, print_helper, env_helper
 from tests.commands import test_request
 
@@ -146,7 +147,98 @@
     env_helper.process_subs(wrapper)
 
     json_string = print_helper.get_json_string(r)
     assert len(re.findall(r'{{ bob }}', json_string)) == 0
     assert len(re.findall(r'current_bob', json_string)) == 0
     assert len(re.findall(r'global_bob', json_string)) == 1
     assert len(re.findall(r'galactic_bob', json_string)) == 0
+
+
+def test_recursive_sub(example_collection, runner):
+    r, wrapper = test_request.lookup_current()
+    r['auth']["username"] = "{{ bob }}"
+    add_to_current("bob", "{{linda}}")
+    add_to_current("linda", "miller")
+
+    json_string = print_helper.get_json_string(r)
+    assert len(re.findall(r'{{ bob }}', json_string)) == 1
+    assert len(re.findall(r'linda', json_string)) == 0
+    assert len(re.findall(r'miller', json_string)) == 0
+
+    env_helper.process_subs(wrapper)
+
+    json_string = print_helper.get_json_string(r)
+    assert len(re.findall(r'{{ bob }}', json_string)) == 0
+    assert len(re.findall(r'linda', json_string)) == 0
+    assert len(re.findall(r'miller', json_string)) == 1
+
+
+def test_3x_recursive_sub(example_collection, runner):
+    r, wrapper = test_request.lookup_current()
+    r['auth']["username"] = "{{ bob }}"
+    add_to_current("bob", "{{linda}}")
+    add_to_current("linda", "{{stacy}}")
+    add_to_current("stacy", "Wilcox")
+
+    json_string = print_helper.get_json_string(r)
+    assert len(re.findall(r'{{ bob }}', json_string)) == 1
+    assert len(re.findall(r'linda', json_string)) == 0
+    assert len(re.findall(r'stacy', json_string)) == 0
+    assert len(re.findall(r'Wilcox', json_string)) == 0
+
+    env_helper.process_subs(wrapper)
+
+    json_string = print_helper.get_json_string(r)
+    assert len(re.findall(r'{{ bob }}', json_string)) == 0
+    assert len(re.findall(r'linda', json_string)) == 0
+    assert len(re.findall(r'stacy', json_string)) == 0
+    assert len(re.findall(r'Wilcox', json_string)) == 1
+
+
+def test_double_sub(example_collection, runner):
+    r, wrapper = test_request.lookup_current()
+    r['auth']["username"] = "{{ bob }} {{ linda }}"
+    add_to_current("bob", "Miller")
+    add_to_current("linda", "Indermuehle")
+
+    json_string = print_helper.get_json_string(r)
+    assert len(re.findall(r'{{ bob }}', json_string)) == 1
+    assert len(re.findall(r'linda', json_string)) == 1
+    assert len(re.findall(r'Miller', json_string)) == 0
+    assert len(re.findall(r'Indermuehle', json_string)) == 0
+
+    env_helper.process_subs(wrapper)
+
+    json_string = print_helper.get_json_string(r)
+    assert len(re.findall(r'{{ bob }}', json_string)) == 0
+    assert len(re.findall(r'linda', json_string)) == 0
+    assert len(re.findall(r'Miller Indermuehle', json_string)) == 1
+
+
+def test_infinite_loop_sub(example_collection, runner):
+    r, wrapper = test_request.lookup_current()
+    r['auth']["username"] = "{{ bob }}"
+    add_to_current("bob", "{{linda}}")
+    add_to_current("linda", "{{bob}}")
+
+    json_string = print_helper.get_json_string(r)
+    assert len(re.findall(r'{{ bob }}', json_string)) == 1
+    assert len(re.findall(r'linda', json_string)) == 0
+    assert len(re.findall(r'miller', json_string)) == 0
+
+    with pytest.raises(click.exceptions.ClickException) as exception_info:
+        env_helper.process_subs(wrapper)
+
+    assert "has caused an infinite loop during lookup" in str(exception_info.value)
+
+
+def test_3x_recursive_loop_caught(example_collection, runner):
+    r, wrapper = test_request.lookup_current()
+    r['auth']["username"] = "{{ bob }}"
+    add_to_current("bob", "{{linda}}")
+    add_to_current("linda", "{{stacy}}")
+    add_to_current("stacy", "{{bob}}")
+
+    with pytest.raises(click.exceptions.ClickException) as exception_info:
+        env_helper.process_subs(wrapper)
+
+    assert "has caused an infinite loop during lookup" in str(exception_info.value)
```

### Comparing `rc3-0.0.6/tests/common/test_inherit_helper.py` & `rc3-0.0.7/tests/common/test_inherit_helper.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.6/tests/conftest.py` & `rc3-0.0.7/tests/conftest.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,10 +37,10 @@
     os.mkdir(empty_dir)
     yield empty_dir
 
 
 @pytest.fixture(scope="function")
 def example_collection(clean_empty, runner):
     os.chdir(clean_empty)
-    result = runner.invoke(cli.cli, ['init'])
+    result = runner.invoke(cli.cli, ['new'], input='example-collection\n\n')
     assert result.exit_code == 0
     yield clean_empty
```

### Comparing `rc3-0.0.6/tests/learning/test_sample.py` & `rc3-0.0.7/tests/learning/test_sample.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.6/tests/test_cli.py` & `rc3-0.0.7/tests/test_cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,27 +8,27 @@
 def test_first_run_help(runner):
     result = runner.invoke(cli.cli)
     assert result.exit_code == 0
     assert "Usage" in result.output
     assert "Show this message and exit" in result.output
 
 
-def test_any_command_creates_empty_rc_home(clean_home, runner):
+def test_any_command_creates_initialized_rc_home(clean_home, runner):
     # pre-test it doesn't exist from a pytest fixture
     rc_home = os.path.join(clean_home, '.rc')
     assert not os.path.exists(rc_home)
 
     # hello cmd doesn't matter, we just need some cmd some cli.cli is invoked instead of help displayed
     result = runner.invoke(cli.cli, ['hello'])
     assert result.exit_code == 0
     assert "Hello" in result.output
 
     # test it exists now AND is empty
     assert os.path.exists(rc_home)
-    assert len(os.listdir(rc_home)) == 0
+    assert len(os.listdir(rc_home)) == 3
 
 
 def test_shortcuts_work(example_collection, runner):
     result = runner.invoke(cli.cli, ['r', '--list'])
     assert result.exit_code == 0
     assert "Listing REQUESTS" in result.output
     result2 = runner.invoke(cli.cli, ['request', '--list'])
```

### Comparing `rc3-0.0.6/tests/util/decorators.py` & `rc3-0.0.7/tests/util/decorators.py`

 * *Files identical despite different names*

