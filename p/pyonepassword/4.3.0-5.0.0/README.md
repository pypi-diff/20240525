# Comparing `tmp/pyonepassword-4.3.0.tar.gz` & `tmp/pyonepassword-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyonepassword-4.3.0.tar", last modified: Thu Mar 28 19:10:20 2024, max compression
+gzip compressed data, was "pyonepassword-5.0.0.tar", last modified: Sat May 25 00:40:01 2024, max compression
```

## Comparing `pyonepassword-4.3.0.tar` & `pyonepassword-5.0.0.tar`

### file list

```diff
@@ -1,133 +1,143 @@
-drwxr-xr-x   0 zach       (503) staff       (20)        0 2024-03-28 19:10:20.852979 pyonepassword-4.3.0/
--rw-r--r--   0 zach       (503) staff       (20)     1071 2019-08-09 16:32:59.000000 pyonepassword-4.3.0/LICENSE
--rw-r--r--   0 zach       (503) staff       (20)    12257 2024-03-28 19:10:20.852869 pyonepassword-4.3.0/PKG-INFO
--rw-r--r--   0 zach       (503) staff       (20)    11055 2023-12-24 00:26:48.000000 pyonepassword-4.3.0/README.md
-drwxr-xr-x   0 zach       (503) staff       (20)        0 2024-03-28 19:10:20.840206 pyonepassword-4.3.0/pyonepassword/
--rw-r--r--   0 zach       (503) staff       (20)      523 2024-03-28 19:09:15.000000 pyonepassword-4.3.0/pyonepassword/__about__.py
--rw-r--r--   0 zach       (503) staff       (20)      626 2024-01-21 04:03:48.000000 pyonepassword-4.3.0/pyonepassword/__init__.py
--rw-r--r--   0 zach       (503) staff       (20)     2276 2023-02-15 22:33:25.000000 pyonepassword-4.3.0/pyonepassword/_abc_meta.py
--rw-r--r--   0 zach       (503) staff       (20)      494 2022-06-22 01:21:11.000000 pyonepassword-4.3.0/pyonepassword/_api_initializer.py
--rw-r--r--   0 zach       (503) staff       (20)      896 2023-11-06 19:24:22.000000 pyonepassword-4.3.0/pyonepassword/_datetime.py
--rw-r--r--   0 zach       (503) staff       (20)     3910 2023-11-06 19:24:22.000000 pyonepassword-4.3.0/pyonepassword/_field_assignment.py
--rw-r--r--   0 zach       (503) staff       (20)     4420 2023-11-28 22:49:32.000000 pyonepassword-4.3.0/pyonepassword/_op_cli.py
--rw-r--r--   0 zach       (503) staff       (20)    19677 2024-03-27 03:27:20.000000 pyonepassword-4.3.0/pyonepassword/_op_cli_argv.py
--rw-r--r--   0 zach       (503) staff       (20)     4406 2023-01-22 17:09:56.000000 pyonepassword-4.3.0/pyonepassword/_op_cli_config.py
--rw-r--r--   0 zach       (503) staff       (20)    45720 2024-03-28 19:09:15.000000 pyonepassword-4.3.0/pyonepassword/_op_commands.py
--rw-r--r--   0 zach       (503) staff       (20)     3183 2023-06-06 01:37:33.000000 pyonepassword-4.3.0/pyonepassword/_py_op_deprecation.py
--rw-r--r--   0 zach       (503) staff       (20)     9121 2023-06-21 22:10:14.000000 pyonepassword-4.3.0/pyonepassword/_svc_account.py
--rw-r--r--   0 zach       (503) staff       (20)     2469 2023-11-06 19:24:22.000000 pyonepassword-4.3.0/pyonepassword/account.py
-drwxr-xr-x   0 zach       (503) staff       (20)        0 2024-03-28 19:10:20.842138 pyonepassword-4.3.0/pyonepassword/api/
--rw-r--r--   0 zach       (503) staff       (20)        0 2023-02-07 19:47:51.000000 pyonepassword-4.3.0/pyonepassword/api/__init__.py
--rw-r--r--   0 zach       (503) staff       (20)      457 2023-11-28 22:49:32.000000 pyonepassword-4.3.0/pyonepassword/api/authentication.py
--rw-r--r--   0 zach       (503) staff       (20)      432 2023-01-22 17:09:56.000000 pyonepassword-4.3.0/pyonepassword/api/constants.py
--rw-r--r--   0 zach       (503) staff       (20)      319 2023-03-14 04:31:28.000000 pyonepassword-4.3.0/pyonepassword/api/decorators.py
--rw-r--r--   0 zach       (503) staff       (20)     1691 2023-03-14 04:31:28.000000 pyonepassword-4.3.0/pyonepassword/api/descriptor_types.py
--rw-r--r--   0 zach       (503) staff       (20)     4004 2023-12-18 05:37:27.000000 pyonepassword-4.3.0/pyonepassword/api/exceptions.py
--rw-r--r--   0 zach       (503) staff       (20)     2732 2024-03-20 03:45:18.000000 pyonepassword-4.3.0/pyonepassword/api/object_types.py
--rw-r--r--   0 zach       (503) staff       (20)      512 2023-02-15 22:33:25.000000 pyonepassword-4.3.0/pyonepassword/api/validation.py
-drwxr-xr-x   0 zach       (503) staff       (20)        0 2024-03-28 19:10:20.845349 pyonepassword-4.3.0/pyonepassword/data/
--rw-r--r--   0 zach       (503) staff       (20)       93 2023-06-06 01:37:33.000000 pyonepassword-4.3.0/pyonepassword/data/__init__.py
-drwxr-xr-x   0 zach       (503) staff       (20)        0 2024-03-28 19:10:20.845485 pyonepassword-4.3.0/pyonepassword/data/__pycache__/
--rw-r--r--   0 zach       (503) staff       (20)      277 2024-01-09 21:51:24.000000 pyonepassword-4.3.0/pyonepassword/data/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0 zach       (503) staff       (20)      940 2023-10-13 02:10:56.000000 pyonepassword-4.3.0/pyonepassword/data/api_credential.json
--rw-r--r--   0 zach       (503) staff       (20)     1552 2023-10-13 02:10:45.000000 pyonepassword-4.3.0/pyonepassword/data/bank_account.json
--rw-r--r--   0 zach       (503) staff       (20)     3084 2023-10-13 02:10:48.000000 pyonepassword-4.3.0/pyonepassword/data/credit_card.json
--rw-r--r--   0 zach       (503) staff       (20)      701 2023-10-13 02:11:59.000000 pyonepassword-4.3.0/pyonepassword/data/crypto_wallet.json
--rw-r--r--   0 zach       (503) staff       (20)     1137 2023-10-13 02:10:48.000000 pyonepassword-4.3.0/pyonepassword/data/database.json
--rw-r--r--   0 zach       (503) staff       (20)      198 2023-10-13 02:10:53.000000 pyonepassword-4.3.0/pyonepassword/data/document.json
--rw-r--r--   0 zach       (503) staff       (20)     1384 2023-10-13 02:10:49.000000 pyonepassword-4.3.0/pyonepassword/data/driver_license.json
--rw-r--r--   0 zach       (503) staff       (20)     3125 2023-10-13 02:10:54.000000 pyonepassword-4.3.0/pyonepassword/data/email_account.json
--rw-r--r--   0 zach       (503) staff       (20)     5190 2023-10-13 02:10:57.000000 pyonepassword-4.3.0/pyonepassword/data/identity.json
--rw-r--r--   0 zach       (503) staff       (20)      536 2023-10-13 02:10:50.000000 pyonepassword-4.3.0/pyonepassword/data/login.json
--rw-r--r--   0 zach       (503) staff       (20)     1425 2023-10-13 02:10:46.000000 pyonepassword-4.3.0/pyonepassword/data/medical_record.json
--rw-r--r--   0 zach       (503) staff       (20)     1064 2023-10-13 02:10:54.000000 pyonepassword-4.3.0/pyonepassword/data/membership.json
--rw-r--r--   0 zach       (503) staff       (20)      941 2023-10-13 02:10:50.000000 pyonepassword-4.3.0/pyonepassword/data/outdoor_license.json
--rw-r--r--   0 zach       (503) staff       (20)     1404 2023-10-13 02:10:58.000000 pyonepassword-4.3.0/pyonepassword/data/passport.json
--rw-r--r--   0 zach       (503) staff       (20)      404 2023-10-13 02:10:59.000000 pyonepassword-4.3.0/pyonepassword/data/password.json
--rw-r--r--   0 zach       (503) staff       (20)     1770 2023-10-13 02:10:51.000000 pyonepassword-4.3.0/pyonepassword/data/reward_program.json
--rw-r--r--   0 zach       (503) staff       (20)      201 2023-10-13 02:10:52.000000 pyonepassword-4.3.0/pyonepassword/data/secure_note.json
--rw-r--r--   0 zach       (503) staff       (20)     2222 2023-10-13 02:10:55.000000 pyonepassword-4.3.0/pyonepassword/data/server.json
--rw-r--r--   0 zach       (503) staff       (20)      415 2023-10-13 02:10:55.000000 pyonepassword-4.3.0/pyonepassword/data/social_security_number.json
--rw-r--r--   0 zach       (503) staff       (20)     2756 2023-10-13 02:10:47.000000 pyonepassword-4.3.0/pyonepassword/data/software_license.json
--rw-r--r--   0 zach       (503) staff       (20)      309 2023-10-13 02:10:52.000000 pyonepassword-4.3.0/pyonepassword/data/ssh_key.json
-drwxr-xr-x   0 zach       (503) staff       (20)        0 2024-03-28 19:10:20.846708 pyonepassword-4.3.0/pyonepassword/data/svc_acct_commands/
--rw-r--r--   0 zach       (503) staff       (20)     1764 2023-06-06 01:37:33.000000 pyonepassword-4.3.0/pyonepassword/data/svc_acct_commands/README.md
--rw-r--r--   0 zach       (503) staff       (20)        0 2023-06-06 01:37:33.000000 pyonepassword-4.3.0/pyonepassword/data/svc_acct_commands/__init__.py
--rw-r--r--   0 zach       (503) staff       (20)      197 2023-06-06 01:37:33.000000 pyonepassword-4.3.0/pyonepassword/data/svc_acct_commands/account.json
--rw-r--r--   0 zach       (503) staff       (20)      483 2023-11-28 22:49:32.000000 pyonepassword-4.3.0/pyonepassword/data/svc_acct_commands/document.json
--rw-r--r--   0 zach       (503) staff       (20)      298 2023-06-06 01:37:33.000000 pyonepassword-4.3.0/pyonepassword/data/svc_acct_commands/group.json
--rw-r--r--   0 zach       (503) staff       (20)      815 2023-11-06 19:24:22.000000 pyonepassword-4.3.0/pyonepassword/data/svc_acct_commands/item.json
--rw-r--r--   0 zach       (503) staff       (20)      168 2023-06-06 01:37:33.000000 pyonepassword-4.3.0/pyonepassword/data/svc_acct_commands/signout.json
--rw-r--r--   0 zach       (503) staff       (20)      297 2023-06-06 01:37:33.000000 pyonepassword-4.3.0/pyonepassword/data/svc_acct_commands/user.json
--rw-r--r--   0 zach       (503) staff       (20)      342 2023-06-06 01:37:33.000000 pyonepassword-4.3.0/pyonepassword/data/svc_acct_commands/vault.json
--rw-r--r--   0 zach       (503) staff       (20)      167 2023-06-06 01:37:33.000000 pyonepassword-4.3.0/pyonepassword/data/svc_acct_commands/whoami.json
--rw-r--r--   0 zach       (503) staff       (20)      829 2023-10-13 02:10:59.000000 pyonepassword-4.3.0/pyonepassword/data/template-registry.json
--rw-r--r--   0 zach       (503) staff       (20)     1165 2023-10-13 02:10:46.000000 pyonepassword-4.3.0/pyonepassword/data/wireless_router.json
--rw-r--r--   0 zach       (503) staff       (20)      257 2022-06-22 00:58:09.000000 pyonepassword-4.3.0/pyonepassword/json.py
--rw-r--r--   0 zach       (503) staff       (20)      366 2023-11-06 23:06:12.000000 pyonepassword-4.3.0/pyonepassword/logging.py
--rw-r--r--   0 zach       (503) staff       (20)     4521 2023-08-27 03:32:16.000000 pyonepassword-4.3.0/pyonepassword/op_cli_version.py
-drwxr-xr-x   0 zach       (503) staff       (20)        0 2024-03-28 19:10:20.848241 pyonepassword-4.3.0/pyonepassword/op_items/
--rw-r--r--   0 zach       (503) staff       (20)      214 2023-03-14 04:31:28.000000 pyonepassword-4.3.0/pyonepassword/op_items/__init__.py
--rw-r--r--   0 zach       (503) staff       (20)      676 2023-03-14 04:31:28.000000 pyonepassword-4.3.0/pyonepassword/op_items/_item_descriptor_registry.py
--rw-r--r--   0 zach       (503) staff       (20)     1652 2023-03-14 04:31:28.000000 pyonepassword-4.3.0/pyonepassword/op_items/_item_list.py
--rw-r--r--   0 zach       (503) staff       (20)     4693 2023-03-14 04:31:28.000000 pyonepassword-4.3.0/pyonepassword/op_items/_item_type_registry.py
--rw-r--r--   0 zach       (503) staff       (20)     4506 2023-11-16 05:05:48.000000 pyonepassword-4.3.0/pyonepassword/op_items/_new_field_registry.py
--rw-r--r--   0 zach       (503) staff       (20)    10376 2023-11-16 05:03:07.000000 pyonepassword-4.3.0/pyonepassword/op_items/_new_item.py
--rw-r--r--   0 zach       (503) staff       (20)      907 2023-03-14 04:31:28.000000 pyonepassword-4.3.0/pyonepassword/op_items/field_registry.py
-drwxr-xr-x   0 zach       (503) staff       (20)        0 2024-03-28 19:10:20.848900 pyonepassword-4.3.0/pyonepassword/op_items/fields_sections/
--rw-r--r--   0 zach       (503) staff       (20)        0 2023-03-14 04:31:28.000000 pyonepassword-4.3.0/pyonepassword/op_items/fields_sections/__init__.py
--rw-r--r--   0 zach       (503) staff       (20)     6800 2023-11-06 19:24:22.000000 pyonepassword-4.3.0/pyonepassword/op_items/fields_sections/_new_fields.py
--rw-r--r--   0 zach       (503) staff       (20)      602 2023-11-06 19:24:22.000000 pyonepassword-4.3.0/pyonepassword/op_items/fields_sections/item_field.py
--rw-r--r--   0 zach       (503) staff       (20)     3055 2023-11-06 19:24:22.000000 pyonepassword-4.3.0/pyonepassword/op_items/fields_sections/item_field_base.py
--rw-r--r--   0 zach       (503) staff       (20)     5419 2023-11-06 19:24:22.000000 pyonepassword-4.3.0/pyonepassword/op_items/fields_sections/item_section.py
-drwxr-xr-x   0 zach       (503) staff       (20)        0 2024-03-28 19:10:20.850671 pyonepassword-4.3.0/pyonepassword/op_items/item_types/
--rw-r--r--   0 zach       (503) staff       (20)        0 2023-03-14 04:31:28.000000 pyonepassword-4.3.0/pyonepassword/op_items/item_types/__init__.py
--rw-r--r--   0 zach       (503) staff       (20)    11801 2024-03-20 03:45:18.000000 pyonepassword-4.3.0/pyonepassword/op_items/item_types/_item_base.py
--rw-r--r--   0 zach       (503) staff       (20)     1895 2023-03-14 04:31:28.000000 pyonepassword-4.3.0/pyonepassword/op_items/item_types/_item_descriptor_base.py
--rw-r--r--   0 zach       (503) staff       (20)     3665 2023-04-11 04:56:27.000000 pyonepassword-4.3.0/pyonepassword/op_items/item_types/api_credential.py
--rw-r--r--   0 zach       (503) staff       (20)     2550 2023-04-11 04:56:27.000000 pyonepassword-4.3.0/pyonepassword/op_items/item_types/credit_card.py
--rw-r--r--   0 zach       (503) staff       (20)     8831 2023-03-28 00:38:01.000000 pyonepassword-4.3.0/pyonepassword/op_items/item_types/database.py
--rw-r--r--   0 zach       (503) staff       (20)     1510 2024-03-20 03:45:18.000000 pyonepassword-4.3.0/pyonepassword/op_items/item_types/document.py
--rw-r--r--   0 zach       (503) staff       (20)     1312 2023-03-14 04:31:28.000000 pyonepassword-4.3.0/pyonepassword/op_items/item_types/generic_item.py
--rw-r--r--   0 zach       (503) staff       (20)      325 2023-03-14 04:31:28.000000 pyonepassword-4.3.0/pyonepassword/op_items/item_types/identity.py
--rw-r--r--   0 zach       (503) staff       (20)     6760 2023-11-06 23:06:12.000000 pyonepassword-4.3.0/pyonepassword/op_items/item_types/login.py
--rw-r--r--   0 zach       (503) staff       (20)     1885 2023-03-14 04:31:28.000000 pyonepassword-4.3.0/pyonepassword/op_items/item_types/password.py
--rw-r--r--   0 zach       (503) staff       (20)     1599 2023-03-14 04:31:28.000000 pyonepassword-4.3.0/pyonepassword/op_items/item_types/secure_note.py
--rw-r--r--   0 zach       (503) staff       (20)     3373 2023-11-06 19:24:22.000000 pyonepassword-4.3.0/pyonepassword/op_items/item_types/server.py
--rw-r--r--   0 zach       (503) staff       (20)     1758 2023-11-16 05:03:07.000000 pyonepassword-4.3.0/pyonepassword/op_items/item_types/ssh_key.py
--rw-r--r--   0 zach       (503) staff       (20)     5533 2023-02-15 22:33:25.000000 pyonepassword-4.3.0/pyonepassword/op_items/item_validation_policy.py
--rw-r--r--   0 zach       (503) staff       (20)     3842 2023-11-06 19:24:22.000000 pyonepassword-4.3.0/pyonepassword/op_items/password_recipe.py
--rw-r--r--   0 zach       (503) staff       (20)      519 2023-01-22 17:09:56.000000 pyonepassword-4.3.0/pyonepassword/op_items/template_directory.py
--rw-r--r--   0 zach       (503) staff       (20)      898 2022-06-22 00:58:09.000000 pyonepassword-4.3.0/pyonepassword/op_items/totp.py
--rw-r--r--   0 zach       (503) staff       (20)     1809 2023-11-16 05:03:07.000000 pyonepassword-4.3.0/pyonepassword/op_items/uuid.py
--rw-r--r--   0 zach       (503) staff       (20)    11729 2023-09-12 02:30:34.000000 pyonepassword-4.3.0/pyonepassword/op_objects.py
--rw-r--r--   0 zach       (503) staff       (20)     1710 2022-11-09 19:14:03.000000 pyonepassword-4.3.0/pyonepassword/opconfig_main.py
--rw-r--r--   0 zach       (503) staff       (20)      720 2023-06-06 01:37:33.000000 pyonepassword-4.3.0/pyonepassword/pkg_resources.py
--rw-r--r--   0 zach       (503) staff       (20)        0 2023-01-22 17:09:56.000000 pyonepassword-4.3.0/pyonepassword/py.typed
--rw-r--r--   0 zach       (503) staff       (20)    11137 2023-12-18 05:37:27.000000 pyonepassword-4.3.0/pyonepassword/py_op_exceptions.py
--rw-r--r--   0 zach       (503) staff       (20)    80302 2024-03-27 21:35:50.000000 pyonepassword-4.3.0/pyonepassword/pyonepassword.py
--rw-r--r--   0 zach       (503) staff       (20)     2941 2023-12-12 03:45:52.000000 pyonepassword-4.3.0/pyonepassword/string.py
--rw-r--r--   0 zach       (503) staff       (20)      972 2023-01-22 17:09:56.000000 pyonepassword-4.3.0/pyonepassword/version.py
-drwxr-xr-x   0 zach       (503) staff       (20)        0 2024-03-28 19:10:20.852474 pyonepassword-4.3.0/pyonepassword.egg-info/
--rw-r--r--   0 zach       (503) staff       (20)    12257 2024-03-28 19:10:20.000000 pyonepassword-4.3.0/pyonepassword.egg-info/PKG-INFO
--rw-r--r--   0 zach       (503) staff       (20)     4414 2024-03-28 19:10:20.000000 pyonepassword-4.3.0/pyonepassword.egg-info/SOURCES.txt
--rw-r--r--   0 zach       (503) staff       (20)        1 2024-03-28 19:10:20.000000 pyonepassword-4.3.0/pyonepassword.egg-info/dependency_links.txt
--rw-r--r--   0 zach       (503) staff       (20)       62 2024-03-28 19:10:20.000000 pyonepassword-4.3.0/pyonepassword.egg-info/entry_points.txt
--rw-r--r--   0 zach       (503) staff       (20)       29 2024-03-28 19:10:20.000000 pyonepassword-4.3.0/pyonepassword.egg-info/requires.txt
--rw-r--r--   0 zach       (503) staff       (20)       14 2024-03-28 19:10:20.000000 pyonepassword-4.3.0/pyonepassword.egg-info/top_level.txt
--rw-r--r--   0 zach       (503) staff       (20)      602 2024-03-28 19:10:20.853257 pyonepassword-4.3.0/setup.cfg
--rw-r--r--   0 zach       (503) staff       (20)     2961 2023-12-18 05:37:27.000000 pyonepassword-4.3.0/setup.py
-drwxr-xr-x   0 zach       (503) staff       (20)        0 2024-03-28 19:10:20.852295 pyonepassword-4.3.0/tests/
--rw-r--r--   0 zach       (503) staff       (20)     1765 2023-08-24 04:54:27.000000 pyonepassword-4.3.0/tests/test_abstract_base_meta.py
--rw-r--r--   0 zach       (503) staff       (20)     2782 2023-06-06 01:37:33.000000 pyonepassword-4.3.0/tests/test_cli_version.py
--rw-r--r--   0 zach       (503) staff       (20)      806 2022-06-22 00:58:09.000000 pyonepassword-4.3.0/tests/test_datetime.py
--rw-r--r--   0 zach       (503) staff       (20)     1949 2023-11-06 19:24:22.000000 pyonepassword-4.3.0/tests/test_deprecation_warnings.py
--rw-r--r--   0 zach       (503) staff       (20)     2844 2023-02-15 22:33:25.000000 pyonepassword-4.3.0/tests/test_exports.py
--rw-r--r--   0 zach       (503) staff       (20)     5441 2023-11-06 19:24:22.000000 pyonepassword-4.3.0/tests/test_item_errors.py
--rw-r--r--   0 zach       (503) staff       (20)     9706 2023-01-22 17:09:56.000000 pyonepassword-4.3.0/tests/test_item_field.py
--rw-r--r--   0 zach       (503) staff       (20)     5534 2023-11-06 19:24:22.000000 pyonepassword-4.3.0/tests/test_item_section.py
--rw-r--r--   0 zach       (503) staff       (20)      953 2023-06-06 01:37:33.000000 pyonepassword-4.3.0/tests/test_op_cli.py
--rw-r--r--   0 zach       (503) staff       (20)     8367 2023-06-21 22:13:21.000000 pyonepassword-4.3.0/tests/test_op_cli_config.py
--rw-r--r--   0 zach       (503) staff       (20)     6218 2023-11-06 19:24:22.000000 pyonepassword-4.3.0/tests/test_password_recipe.py
--rw-r--r--   0 zach       (503) staff       (20)      442 2023-01-22 17:09:56.000000 pyonepassword-4.3.0/tests/test_pyop_about.py
--rw-r--r--   0 zach       (503) staff       (20)     6797 2023-06-22 22:42:57.000000 pyonepassword-4.3.0/tests/test_redacted_string.py
+drwxr-xr-x   0 zach       (503) staff       (20)        0 2024-05-25 00:40:01.290078 pyonepassword-5.0.0/
+-rw-r--r--   0 zach       (503) staff       (20)     1071 2019-08-09 16:32:59.000000 pyonepassword-5.0.0/LICENSE
+-rw-r--r--   0 zach       (503) staff       (20)      115 2024-05-24 23:49:56.000000 pyonepassword-5.0.0/MANIFEST.in
+-rw-r--r--   0 zach       (503) staff       (20)    12582 2024-05-25 00:40:01.289964 pyonepassword-5.0.0/PKG-INFO
+-rw-r--r--   0 zach       (503) staff       (20)    11380 2024-05-24 23:49:56.000000 pyonepassword-5.0.0/README.md
+-rw-r--r--   0 zach       (503) staff       (20)    11444 2024-05-24 23:49:56.000000 pyonepassword-5.0.0/_readme_template.md
+drwxr-xr-x   0 zach       (503) staff       (20)        0 2024-05-25 00:40:01.267184 pyonepassword-5.0.0/pyonepassword/
+-rw-r--r--   0 zach       (503) staff       (20)      523 2024-05-24 23:51:42.000000 pyonepassword-5.0.0/pyonepassword/__about__.py
+-rw-r--r--   0 zach       (503) staff       (20)      626 2024-01-21 04:03:48.000000 pyonepassword-5.0.0/pyonepassword/__init__.py
+-rw-r--r--   0 zach       (503) staff       (20)     2276 2023-02-15 22:33:25.000000 pyonepassword-5.0.0/pyonepassword/_abc_meta.py
+-rw-r--r--   0 zach       (503) staff       (20)      494 2022-06-22 01:21:11.000000 pyonepassword-5.0.0/pyonepassword/_api_initializer.py
+-rw-r--r--   0 zach       (503) staff       (20)      896 2023-11-06 19:24:22.000000 pyonepassword-5.0.0/pyonepassword/_datetime.py
+-rw-r--r--   0 zach       (503) staff       (20)     3910 2023-11-06 19:24:22.000000 pyonepassword-5.0.0/pyonepassword/_field_assignment.py
+-rw-r--r--   0 zach       (503) staff       (20)     4628 2024-05-24 23:49:56.000000 pyonepassword-5.0.0/pyonepassword/_op_cli.py
+-rw-r--r--   0 zach       (503) staff       (20)    19677 2024-03-27 03:27:20.000000 pyonepassword-5.0.0/pyonepassword/_op_cli_argv.py
+-rw-r--r--   0 zach       (503) staff       (20)     4406 2023-01-22 17:09:56.000000 pyonepassword-5.0.0/pyonepassword/_op_cli_config.py
+-rw-r--r--   0 zach       (503) staff       (20)     7359 2024-05-24 23:49:56.000000 pyonepassword-5.0.0/pyonepassword/_op_cli_version.py
+-rw-r--r--   0 zach       (503) staff       (20)    47147 2024-05-24 23:49:56.000000 pyonepassword-5.0.0/pyonepassword/_op_commands.py
+-rw-r--r--   0 zach       (503) staff       (20)     3238 2024-05-24 23:49:56.000000 pyonepassword-5.0.0/pyonepassword/_py_op_deprecation.py
+-rw-r--r--   0 zach       (503) staff       (20)     9151 2024-05-24 23:49:56.000000 pyonepassword-5.0.0/pyonepassword/_svc_account.py
+-rw-r--r--   0 zach       (503) staff       (20)     2469 2023-11-06 19:24:22.000000 pyonepassword-5.0.0/pyonepassword/account.py
+drwxr-xr-x   0 zach       (503) staff       (20)        0 2024-05-25 00:40:01.269076 pyonepassword-5.0.0/pyonepassword/api/
+-rw-r--r--   0 zach       (503) staff       (20)        0 2023-02-07 19:47:51.000000 pyonepassword-5.0.0/pyonepassword/api/__init__.py
+-rw-r--r--   0 zach       (503) staff       (20)      457 2023-11-28 22:49:32.000000 pyonepassword-5.0.0/pyonepassword/api/authentication.py
+-rw-r--r--   0 zach       (503) staff       (20)      288 2024-05-24 23:49:56.000000 pyonepassword-5.0.0/pyonepassword/api/cli_version.py
+-rw-r--r--   0 zach       (503) staff       (20)      432 2023-01-22 17:09:56.000000 pyonepassword-5.0.0/pyonepassword/api/constants.py
+-rw-r--r--   0 zach       (503) staff       (20)      319 2023-03-14 04:31:28.000000 pyonepassword-5.0.0/pyonepassword/api/decorators.py
+-rw-r--r--   0 zach       (503) staff       (20)     1691 2023-03-14 04:31:28.000000 pyonepassword-5.0.0/pyonepassword/api/descriptor_types.py
+-rw-r--r--   0 zach       (503) staff       (20)     3817 2024-05-24 23:49:56.000000 pyonepassword-5.0.0/pyonepassword/api/exceptions.py
+-rw-r--r--   0 zach       (503) staff       (20)     2732 2024-05-24 23:51:29.000000 pyonepassword-5.0.0/pyonepassword/api/object_types.py
+-rw-r--r--   0 zach       (503) staff       (20)      512 2023-02-15 22:33:25.000000 pyonepassword-5.0.0/pyonepassword/api/validation.py
+drwxr-xr-x   0 zach       (503) staff       (20)        0 2024-05-25 00:40:01.278880 pyonepassword-5.0.0/pyonepassword/data/
+-rw-r--r--   0 zach       (503) staff       (20)      184 2024-05-24 23:49:56.000000 pyonepassword-5.0.0/pyonepassword/data/__init__.py
+drwxr-xr-x   0 zach       (503) staff       (20)        0 2024-05-25 00:40:01.279267 pyonepassword-5.0.0/pyonepassword/data/__pycache__/
+-rw-r--r--   0 zach       (503) staff       (20)      406 2024-05-24 23:49:56.000000 pyonepassword-5.0.0/pyonepassword/data/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0 zach       (503) staff       (20)      940 2023-10-13 02:10:56.000000 pyonepassword-5.0.0/pyonepassword/data/api_credential.json
+-rw-r--r--   0 zach       (503) staff       (20)     1552 2023-10-13 02:10:45.000000 pyonepassword-5.0.0/pyonepassword/data/bank_account.json
+-rw-r--r--   0 zach       (503) staff       (20)     3084 2023-10-13 02:10:48.000000 pyonepassword-5.0.0/pyonepassword/data/credit_card.json
+-rw-r--r--   0 zach       (503) staff       (20)      701 2023-10-13 02:11:59.000000 pyonepassword-5.0.0/pyonepassword/data/crypto_wallet.json
+-rw-r--r--   0 zach       (503) staff       (20)     1137 2023-10-13 02:10:48.000000 pyonepassword-5.0.0/pyonepassword/data/database.json
+-rw-r--r--   0 zach       (503) staff       (20)      198 2023-10-13 02:10:53.000000 pyonepassword-5.0.0/pyonepassword/data/document.json
+-rw-r--r--   0 zach       (503) staff       (20)     1384 2023-10-13 02:10:49.000000 pyonepassword-5.0.0/pyonepassword/data/driver_license.json
+-rw-r--r--   0 zach       (503) staff       (20)     3125 2023-10-13 02:10:54.000000 pyonepassword-5.0.0/pyonepassword/data/email_account.json
+-rw-r--r--   0 zach       (503) staff       (20)     5190 2023-10-13 02:10:57.000000 pyonepassword-5.0.0/pyonepassword/data/identity.json
+-rw-r--r--   0 zach       (503) staff       (20)      536 2023-10-13 02:10:50.000000 pyonepassword-5.0.0/pyonepassword/data/login.json
+-rw-r--r--   0 zach       (503) staff       (20)     1425 2023-10-13 02:10:46.000000 pyonepassword-5.0.0/pyonepassword/data/medical_record.json
+-rw-r--r--   0 zach       (503) staff       (20)     1064 2023-10-13 02:10:54.000000 pyonepassword-5.0.0/pyonepassword/data/membership.json
+drwxr-xr-x   0 zach       (503) staff       (20)        0 2024-05-25 00:40:01.279613 pyonepassword-5.0.0/pyonepassword/data/op_versions/
+-rw-r--r--   0 zach       (503) staff       (20)        0 2024-05-24 23:49:56.000000 pyonepassword-5.0.0/pyonepassword/data/op_versions/__init__.py
+-rw-r--r--   0 zach       (503) staff       (20)      387 2024-05-24 23:49:56.000000 pyonepassword-5.0.0/pyonepassword/data/op_versions/version_support.json
+-rw-r--r--   0 zach       (503) staff       (20)     1230 2024-05-24 23:49:56.000000 pyonepassword-5.0.0/pyonepassword/data/op_versions/version_support_readme.md
+-rw-r--r--   0 zach       (503) staff       (20)      941 2023-10-13 02:10:50.000000 pyonepassword-5.0.0/pyonepassword/data/outdoor_license.json
+-rw-r--r--   0 zach       (503) staff       (20)     1404 2023-10-13 02:10:58.000000 pyonepassword-5.0.0/pyonepassword/data/passport.json
+-rw-r--r--   0 zach       (503) staff       (20)      404 2023-10-13 02:10:59.000000 pyonepassword-5.0.0/pyonepassword/data/password.json
+-rw-r--r--   0 zach       (503) staff       (20)     1770 2023-10-13 02:10:51.000000 pyonepassword-5.0.0/pyonepassword/data/reward_program.json
+-rw-r--r--   0 zach       (503) staff       (20)      201 2023-10-13 02:10:52.000000 pyonepassword-5.0.0/pyonepassword/data/secure_note.json
+-rw-r--r--   0 zach       (503) staff       (20)     2222 2023-10-13 02:10:55.000000 pyonepassword-5.0.0/pyonepassword/data/server.json
+-rw-r--r--   0 zach       (503) staff       (20)      415 2023-10-13 02:10:55.000000 pyonepassword-5.0.0/pyonepassword/data/social_security_number.json
+-rw-r--r--   0 zach       (503) staff       (20)     2756 2023-10-13 02:10:47.000000 pyonepassword-5.0.0/pyonepassword/data/software_license.json
+-rw-r--r--   0 zach       (503) staff       (20)      309 2023-10-13 02:10:52.000000 pyonepassword-5.0.0/pyonepassword/data/ssh_key.json
+drwxr-xr-x   0 zach       (503) staff       (20)        0 2024-05-25 00:40:01.282907 pyonepassword-5.0.0/pyonepassword/data/svc_acct_commands/
+-rw-r--r--   0 zach       (503) staff       (20)     1764 2023-06-06 01:37:33.000000 pyonepassword-5.0.0/pyonepassword/data/svc_acct_commands/README.md
+-rw-r--r--   0 zach       (503) staff       (20)        0 2023-06-06 01:37:33.000000 pyonepassword-5.0.0/pyonepassword/data/svc_acct_commands/__init__.py
+-rw-r--r--   0 zach       (503) staff       (20)      197 2023-06-06 01:37:33.000000 pyonepassword-5.0.0/pyonepassword/data/svc_acct_commands/account.json
+-rw-r--r--   0 zach       (503) staff       (20)      483 2023-11-28 22:49:32.000000 pyonepassword-5.0.0/pyonepassword/data/svc_acct_commands/document.json
+-rw-r--r--   0 zach       (503) staff       (20)      298 2023-06-06 01:37:33.000000 pyonepassword-5.0.0/pyonepassword/data/svc_acct_commands/group.json
+-rw-r--r--   0 zach       (503) staff       (20)      815 2023-11-06 19:24:22.000000 pyonepassword-5.0.0/pyonepassword/data/svc_acct_commands/item.json
+-rw-r--r--   0 zach       (503) staff       (20)      168 2023-06-06 01:37:33.000000 pyonepassword-5.0.0/pyonepassword/data/svc_acct_commands/signout.json
+-rw-r--r--   0 zach       (503) staff       (20)      297 2023-06-06 01:37:33.000000 pyonepassword-5.0.0/pyonepassword/data/svc_acct_commands/user.json
+-rw-r--r--   0 zach       (503) staff       (20)      342 2023-06-06 01:37:33.000000 pyonepassword-5.0.0/pyonepassword/data/svc_acct_commands/vault.json
+-rw-r--r--   0 zach       (503) staff       (20)      167 2023-06-06 01:37:33.000000 pyonepassword-5.0.0/pyonepassword/data/svc_acct_commands/whoami.json
+-rw-r--r--   0 zach       (503) staff       (20)      829 2023-10-13 02:10:59.000000 pyonepassword-5.0.0/pyonepassword/data/template-registry.json
+-rw-r--r--   0 zach       (503) staff       (20)     1165 2023-10-13 02:10:46.000000 pyonepassword-5.0.0/pyonepassword/data/wireless_router.json
+-rw-r--r--   0 zach       (503) staff       (20)      257 2022-06-22 00:58:09.000000 pyonepassword-5.0.0/pyonepassword/json.py
+-rw-r--r--   0 zach       (503) staff       (20)      366 2023-11-06 23:06:12.000000 pyonepassword-5.0.0/pyonepassword/logging.py
+drwxr-xr-x   0 zach       (503) staff       (20)        0 2024-05-25 00:40:01.284714 pyonepassword-5.0.0/pyonepassword/op_items/
+-rw-r--r--   0 zach       (503) staff       (20)      214 2023-03-14 04:31:28.000000 pyonepassword-5.0.0/pyonepassword/op_items/__init__.py
+-rw-r--r--   0 zach       (503) staff       (20)      676 2023-03-14 04:31:28.000000 pyonepassword-5.0.0/pyonepassword/op_items/_item_descriptor_registry.py
+-rw-r--r--   0 zach       (503) staff       (20)     1652 2023-03-14 04:31:28.000000 pyonepassword-5.0.0/pyonepassword/op_items/_item_list.py
+-rw-r--r--   0 zach       (503) staff       (20)     4693 2023-03-14 04:31:28.000000 pyonepassword-5.0.0/pyonepassword/op_items/_item_type_registry.py
+-rw-r--r--   0 zach       (503) staff       (20)     4506 2023-11-16 05:05:48.000000 pyonepassword-5.0.0/pyonepassword/op_items/_new_field_registry.py
+-rw-r--r--   0 zach       (503) staff       (20)    10376 2023-11-16 05:03:07.000000 pyonepassword-5.0.0/pyonepassword/op_items/_new_item.py
+-rw-r--r--   0 zach       (503) staff       (20)      907 2023-03-14 04:31:28.000000 pyonepassword-5.0.0/pyonepassword/op_items/field_registry.py
+drwxr-xr-x   0 zach       (503) staff       (20)        0 2024-05-25 00:40:01.285318 pyonepassword-5.0.0/pyonepassword/op_items/fields_sections/
+-rw-r--r--   0 zach       (503) staff       (20)        0 2023-03-14 04:31:28.000000 pyonepassword-5.0.0/pyonepassword/op_items/fields_sections/__init__.py
+-rw-r--r--   0 zach       (503) staff       (20)     6800 2023-11-06 19:24:22.000000 pyonepassword-5.0.0/pyonepassword/op_items/fields_sections/_new_fields.py
+-rw-r--r--   0 zach       (503) staff       (20)      602 2023-11-06 19:24:22.000000 pyonepassword-5.0.0/pyonepassword/op_items/fields_sections/item_field.py
+-rw-r--r--   0 zach       (503) staff       (20)     3055 2023-11-06 19:24:22.000000 pyonepassword-5.0.0/pyonepassword/op_items/fields_sections/item_field_base.py
+-rw-r--r--   0 zach       (503) staff       (20)     5419 2023-11-06 19:24:22.000000 pyonepassword-5.0.0/pyonepassword/op_items/fields_sections/item_section.py
+drwxr-xr-x   0 zach       (503) staff       (20)        0 2024-05-25 00:40:01.287148 pyonepassword-5.0.0/pyonepassword/op_items/item_types/
+-rw-r--r--   0 zach       (503) staff       (20)        0 2023-03-14 04:31:28.000000 pyonepassword-5.0.0/pyonepassword/op_items/item_types/__init__.py
+-rw-r--r--   0 zach       (503) staff       (20)    11801 2024-05-24 23:51:29.000000 pyonepassword-5.0.0/pyonepassword/op_items/item_types/_item_base.py
+-rw-r--r--   0 zach       (503) staff       (20)     1895 2023-03-14 04:31:28.000000 pyonepassword-5.0.0/pyonepassword/op_items/item_types/_item_descriptor_base.py
+-rw-r--r--   0 zach       (503) staff       (20)     3665 2023-04-11 04:56:27.000000 pyonepassword-5.0.0/pyonepassword/op_items/item_types/api_credential.py
+-rw-r--r--   0 zach       (503) staff       (20)     2550 2023-04-11 04:56:27.000000 pyonepassword-5.0.0/pyonepassword/op_items/item_types/credit_card.py
+-rw-r--r--   0 zach       (503) staff       (20)     8831 2023-03-28 00:38:01.000000 pyonepassword-5.0.0/pyonepassword/op_items/item_types/database.py
+-rw-r--r--   0 zach       (503) staff       (20)     1510 2024-05-24 23:51:29.000000 pyonepassword-5.0.0/pyonepassword/op_items/item_types/document.py
+-rw-r--r--   0 zach       (503) staff       (20)     1312 2023-03-14 04:31:28.000000 pyonepassword-5.0.0/pyonepassword/op_items/item_types/generic_item.py
+-rw-r--r--   0 zach       (503) staff       (20)      325 2023-03-14 04:31:28.000000 pyonepassword-5.0.0/pyonepassword/op_items/item_types/identity.py
+-rw-r--r--   0 zach       (503) staff       (20)     6760 2023-11-06 23:06:12.000000 pyonepassword-5.0.0/pyonepassword/op_items/item_types/login.py
+-rw-r--r--   0 zach       (503) staff       (20)     1885 2023-03-14 04:31:28.000000 pyonepassword-5.0.0/pyonepassword/op_items/item_types/password.py
+-rw-r--r--   0 zach       (503) staff       (20)     1599 2023-03-14 04:31:28.000000 pyonepassword-5.0.0/pyonepassword/op_items/item_types/secure_note.py
+-rw-r--r--   0 zach       (503) staff       (20)     3373 2023-11-06 19:24:22.000000 pyonepassword-5.0.0/pyonepassword/op_items/item_types/server.py
+-rw-r--r--   0 zach       (503) staff       (20)     1758 2023-11-16 05:03:07.000000 pyonepassword-5.0.0/pyonepassword/op_items/item_types/ssh_key.py
+-rw-r--r--   0 zach       (503) staff       (20)     5533 2023-02-15 22:33:25.000000 pyonepassword-5.0.0/pyonepassword/op_items/item_validation_policy.py
+-rw-r--r--   0 zach       (503) staff       (20)     3842 2023-11-06 19:24:22.000000 pyonepassword-5.0.0/pyonepassword/op_items/password_recipe.py
+-rw-r--r--   0 zach       (503) staff       (20)      519 2023-01-22 17:09:56.000000 pyonepassword-5.0.0/pyonepassword/op_items/template_directory.py
+-rw-r--r--   0 zach       (503) staff       (20)      898 2022-06-22 00:58:09.000000 pyonepassword-5.0.0/pyonepassword/op_items/totp.py
+-rw-r--r--   0 zach       (503) staff       (20)     1809 2023-11-16 05:03:07.000000 pyonepassword-5.0.0/pyonepassword/op_items/uuid.py
+-rw-r--r--   0 zach       (503) staff       (20)    11729 2023-09-12 02:30:34.000000 pyonepassword-5.0.0/pyonepassword/op_objects.py
+-rw-r--r--   0 zach       (503) staff       (20)     1710 2024-05-07 02:46:14.000000 pyonepassword-5.0.0/pyonepassword/opconfig_main.py
+-rw-r--r--   0 zach       (503) staff       (20)     1327 2024-05-24 23:49:56.000000 pyonepassword-5.0.0/pyonepassword/opversion_main.py
+-rw-r--r--   0 zach       (503) staff       (20)      652 2024-05-24 23:49:56.000000 pyonepassword-5.0.0/pyonepassword/pkg_resources.py
+-rw-r--r--   0 zach       (503) staff       (20)        0 2023-01-22 17:09:56.000000 pyonepassword-5.0.0/pyonepassword/py.typed
+-rw-r--r--   0 zach       (503) staff       (20)    11142 2024-05-24 23:49:56.000000 pyonepassword-5.0.0/pyonepassword/py_op_exceptions.py
+-rw-r--r--   0 zach       (503) staff       (20)    82976 2024-05-24 23:49:56.000000 pyonepassword-5.0.0/pyonepassword/pyonepassword.py
+-rw-r--r--   0 zach       (503) staff       (20)     2941 2023-12-12 03:45:52.000000 pyonepassword-5.0.0/pyonepassword/string.py
+-rw-r--r--   0 zach       (503) staff       (20)      972 2023-01-22 17:09:56.000000 pyonepassword-5.0.0/pyonepassword/version.py
+drwxr-xr-x   0 zach       (503) staff       (20)        0 2024-05-25 00:40:01.289710 pyonepassword-5.0.0/pyonepassword.egg-info/
+-rw-r--r--   0 zach       (503) staff       (20)    12582 2024-05-25 00:40:01.000000 pyonepassword-5.0.0/pyonepassword.egg-info/PKG-INFO
+-rw-r--r--   0 zach       (503) staff       (20)     4678 2024-05-25 00:40:01.000000 pyonepassword-5.0.0/pyonepassword.egg-info/SOURCES.txt
+-rw-r--r--   0 zach       (503) staff       (20)        1 2024-05-25 00:40:01.000000 pyonepassword-5.0.0/pyonepassword.egg-info/dependency_links.txt
+-rw-r--r--   0 zach       (503) staff       (20)      108 2024-05-25 00:40:01.000000 pyonepassword-5.0.0/pyonepassword.egg-info/entry_points.txt
+-rw-r--r--   0 zach       (503) staff       (20)       29 2024-05-25 00:40:01.000000 pyonepassword-5.0.0/pyonepassword.egg-info/requires.txt
+-rw-r--r--   0 zach       (503) staff       (20)       14 2024-05-25 00:40:01.000000 pyonepassword-5.0.0/pyonepassword.egg-info/top_level.txt
+-rw-r--r--   0 zach       (503) staff       (20)      146 2024-05-24 23:49:56.000000 pyonepassword-5.0.0/pyproject.toml
+drwxr-xr-x   0 zach       (503) staff       (20)        0 2024-05-25 00:40:01.287278 pyonepassword-5.0.0/scripts/
+-rwxr-xr-x   0 zach       (503) staff       (20)     1570 2024-05-24 23:49:56.000000 pyonepassword-5.0.0/scripts/update_readme.py
+-rw-r--r--   0 zach       (503) staff       (20)      602 2024-05-25 00:40:01.290358 pyonepassword-5.0.0/setup.cfg
+-rw-r--r--   0 zach       (503) staff       (20)     3462 2024-05-24 23:49:56.000000 pyonepassword-5.0.0/setup.py
+drwxr-xr-x   0 zach       (503) staff       (20)        0 2024-05-25 00:40:01.289118 pyonepassword-5.0.0/tests/
+-rw-r--r--   0 zach       (503) staff       (20)     1765 2023-08-24 04:54:27.000000 pyonepassword-5.0.0/tests/test_abstract_base_meta.py
+-rw-r--r--   0 zach       (503) staff       (20)      806 2022-06-22 00:58:09.000000 pyonepassword-5.0.0/tests/test_datetime.py
+-rw-r--r--   0 zach       (503) staff       (20)     2016 2024-05-24 23:49:56.000000 pyonepassword-5.0.0/tests/test_deprecation_warnings.py
+-rw-r--r--   0 zach       (503) staff       (20)     2844 2023-02-15 22:33:25.000000 pyonepassword-5.0.0/tests/test_exports.py
+-rw-r--r--   0 zach       (503) staff       (20)     5441 2023-11-06 19:24:22.000000 pyonepassword-5.0.0/tests/test_item_errors.py
+-rw-r--r--   0 zach       (503) staff       (20)     9706 2023-01-22 17:09:56.000000 pyonepassword-5.0.0/tests/test_item_field.py
+-rw-r--r--   0 zach       (503) staff       (20)     5534 2023-11-06 19:24:22.000000 pyonepassword-5.0.0/tests/test_item_section.py
+-rw-r--r--   0 zach       (503) staff       (20)      990 2024-05-24 23:49:56.000000 pyonepassword-5.0.0/tests/test_op_cli.py
+-rw-r--r--   0 zach       (503) staff       (20)     8367 2023-06-21 22:13:21.000000 pyonepassword-5.0.0/tests/test_op_cli_config.py
+-rw-r--r--   0 zach       (503) staff       (20)     6218 2023-11-06 19:24:22.000000 pyonepassword-5.0.0/tests/test_password_recipe.py
+-rw-r--r--   0 zach       (503) staff       (20)      442 2023-01-22 17:09:56.000000 pyonepassword-5.0.0/tests/test_pyop_about.py
+-rw-r--r--   0 zach       (503) staff       (20)     6797 2023-06-22 22:42:57.000000 pyonepassword-5.0.0/tests/test_redacted_string.py
```

### Comparing `pyonepassword-4.3.0/LICENSE` & `pyonepassword-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyonepassword-4.3.0/PKG-INFO` & `pyonepassword-5.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyonepassword
-Version: 4.3.0
+Version: 5.0.0
 Summary: A python API to query a 1Password account using the 'op' command-line tool
 Home-page: https://github.com/zcutlip/pyonepassword
 Author: Zachary Cutlip
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -31,20 +31,24 @@
 ## Description
 
 A Python API to sign into and query a 1Password account using the `op` command.
 
 ## Requirements
 
 - Python >= 3.9
-- 1Password command-line tool >= 2.0.0
-  - see [1Password Developer Documentation](https://developer.1password.com/docs/cli)
+- 1Password command-line tool >= 2.24.0
+  - Versions >= 2.19.0, < 2.24.0 supported but deprecated
+  - Versions < 2.19.0 are unsupported and an exception will be raised
+  - See [1Password Developer Documentation](https://developer.1password.com/docs/cli)
 - Internet connectivity to 1Password.com
   - The `op` command queries your online account, not your local vault
 
-> Note: This version of `pyonepassword` does not support deprecated `op` 1.x versions. Support for those versions is still available, albeit with minimal maintanence. See [pyonepassword-legacy](https://github.com/zcutlip/pyonepassword-legacy) for more information.
+> Notes:
+> - Generally `pyonepassword` will support up to 5 patch versions, including the current. E.g., 2.{24-28}.0. Five additional patch versions, e.g., 2.{19-23}.0, will be considered deprecated.
+> - This version of `pyonepassword` does not support deprecated `op` 1.x versions. Support for those versions is still available, albeit with minimal maintanence. See [pyonepassword-legacy](https://github.com/zcutlip/pyonepassword-legacy) for more information.
 
 ## Installation
 
 ```shell
 python3 -m pip install pyonepassword
 ```
```

### Comparing `pyonepassword-4.3.0/README.md` & `pyonepassword-5.0.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -10,20 +10,24 @@
 ## Description
 
 A Python API to sign into and query a 1Password account using the `op` command.
 
 ## Requirements
 
 - Python >= 3.9
-- 1Password command-line tool >= 2.0.0
-  - see [1Password Developer Documentation](https://developer.1password.com/docs/cli)
+- 1Password command-line tool >= 2.24.0
+  - Versions >= 2.19.0, < 2.24.0 supported but deprecated
+  - Versions < 2.19.0 are unsupported and an exception will be raised
+  - See [1Password Developer Documentation](https://developer.1password.com/docs/cli)
 - Internet connectivity to 1Password.com
   - The `op` command queries your online account, not your local vault
 
-> Note: This version of `pyonepassword` does not support deprecated `op` 1.x versions. Support for those versions is still available, albeit with minimal maintanence. See [pyonepassword-legacy](https://github.com/zcutlip/pyonepassword-legacy) for more information.
+> Notes:
+> - Generally `pyonepassword` will support up to 5 patch versions, including the current. E.g., 2.{24-28}.0. Five additional patch versions, e.g., 2.{19-23}.0, will be considered deprecated.
+> - This version of `pyonepassword` does not support deprecated `op` 1.x versions. Support for those versions is still available, albeit with minimal maintanence. See [pyonepassword-legacy](https://github.com/zcutlip/pyonepassword-legacy) for more information.
 
 ## Installation
 
 ```shell
 python3 -m pip install pyonepassword
 ```
```

### Comparing `pyonepassword-4.3.0/pyonepassword/__about__.py` & `pyonepassword-5.0.0/pyonepassword/__about__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 __title__ = "pyonepassword"
-__version__ = "4.3.0"
+__version__ = "5.0.0"
 __summary__ = "A python API to query a 1Password account using the 'op' command-line tool"
 
 """
 See PEP 440 for version scheme
 https://www.python.org/dev/peps/pep-0440/#examples-of-compliant-version-schemes
 Examples:
```

### Comparing `pyonepassword-4.3.0/pyonepassword/__init__.py` & `pyonepassword-5.0.0/pyonepassword/__init__.py`

 * *Files identical despite different names*

### Comparing `pyonepassword-4.3.0/pyonepassword/_abc_meta.py` & `pyonepassword-5.0.0/pyonepassword/_abc_meta.py`

 * *Files identical despite different names*

### Comparing `pyonepassword-4.3.0/pyonepassword/_datetime.py` & `pyonepassword-5.0.0/pyonepassword/_datetime.py`

 * *Files identical despite different names*

### Comparing `pyonepassword-4.3.0/pyonepassword/_field_assignment.py` & `pyonepassword-5.0.0/pyonepassword/_field_assignment.py`

 * *Files identical despite different names*

### Comparing `pyonepassword-4.3.0/pyonepassword/_op_cli.py` & `pyonepassword-5.0.0/pyonepassword/_op_cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,14 +33,20 @@
             cls.set_logger(logger)
         return super().__new__(cls)
     """
     Class for logging into and querying a 1Password account via the 'op' cli command.
     """
 
     @classmethod
+    def _reset_class_logger(cls):
+        # For use when resetting state between test cases
+        cls.logger = logging.getLogger("_OPCLIExecute")
+        cls.logger.setLevel(logging.INFO)
+
+    @classmethod
     def _should_log_op_errors(cls) -> bool:
         should_log = False
         if environ.get(LOG_OP_ERR_ENV_NAME) == "1":
             should_log = True
         return should_log
 
     @classmethod
```

### Comparing `pyonepassword-4.3.0/pyonepassword/_op_cli_argv.py` & `pyonepassword-5.0.0/pyonepassword/_op_cli_argv.py`

 * *Files identical despite different names*

### Comparing `pyonepassword-4.3.0/pyonepassword/_op_cli_config.py` & `pyonepassword-5.0.0/pyonepassword/_op_cli_config.py`

 * *Files identical despite different names*

### Comparing `pyonepassword-4.3.0/pyonepassword/_op_commands.py` & `pyonepassword-5.0.0/pyonepassword/_op_commands.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 """
 Description: A module that maps methods to to `op` commands and subcommands
 """
 from __future__ import annotations
 
 import enum
 import logging
+import os
+import shutil
 from os import environ
-from typing import TYPE_CHECKING, Dict, List, Mapping, Optional, Union
+from typing import TYPE_CHECKING, Dict, List, Mapping, Optional, Tuple, Union
 
 if TYPE_CHECKING:  # pragma: no coverage
     from pyonepassword._field_assignment import OPFieldTypeEnum
 
 from ._op_cli import _OPCLIExecute
 from ._op_cli_argv import _OPArgv
 from ._op_cli_config import OPCLIConfig
+from ._op_cli_version import OPCLIVersion, OPVersionSupport
 from ._svc_account import (
     SVC_ACCT_CMD_NOT_SUPPORTED,
     SVC_ACCT_INCOMPAT_OPTIONS,
     SVC_ACCT_SUPPORTED,
     OPSvcAcctCommandNotSupportedException
 )
 from .account import OPAccount, OPAccountList
-from .op_cli_version import (
-    DOCUMENT_BYTES_BUG_VERSION,
-    MINIMUM_SERVICE_ACCOUNT_VERSION,
-    OPCLIVersion
-)
 from .op_items.password_recipe import OPPasswordRecipe
 from .py_op_exceptions import (
     OPAuthenticationException,
     OPCmdFailedException,
     OPCmdMalformedSvcAcctTokenException,
     OPConfigNotFoundException,
     OPDocumentDeleteException,
@@ -38,14 +36,15 @@
     OPGroupGetException,
     OPGroupListException,
     OPItemCreateException,
     OPItemDeleteException,
     OPItemEditException,
     OPItemGetException,
     OPItemListException,
+    OPNotFoundException,
     OPSigninException,
     OPUnknownAccountException,
     OPUserEditException,
     OPUserGetException,
     OPUserListException,
     OPVaultGetException,
     OPVaultListException,
@@ -77,14 +76,17 @@
     ACCT_IS_NOT_SIGNED_IN_TEXT = "account is not signed in"
     SVC_ACCT_TOKEN_MALFORMED_TEXT = "failed to DecodeSACCredentials"
     SVC_ACCT_TOKEN_NOT_AUTH_TXT = "service account token set, but not authenticated yet"
 
     OP_SVC_ACCOUNT_ENV_VAR = "OP_SERVICE_ACCOUNT_TOKEN"
     OP_PATH = 'op'  # let subprocess find 'op' in the system path
 
+    _version_support = OPVersionSupport()
+    _op_paths_checked: set[Tuple[int, float]] = set()
+
     def __init__(self,
                  account: str = None,
                  password: str = None,
                  existing_auth: ExistingAuthEnum = EXISTING_AUTH_IGNORE,
                  vault: str = None,
                  password_prompt: bool = True,
                  op_path: str = OP_PATH,
@@ -115,28 +117,25 @@
         # part of exception message in case incompatible authentication parameters
         # are provided
         auth_pref_source = "preference passed as argument"
         if self.svc_account_env_var_set():
             # - 'op' won't prompt for authentication of OP_SERVICE_ACCOUNT_TOKEN is set
             # - Even if we explicitly call signin and succeed, it ignores that authentication
             # so we need to suppress any path that tries to or expects to authenticate
-            if self._cli_version < MINIMUM_SERVICE_ACCOUNT_VERSION:
-                raise OPAuthenticationException(
-                    f"Version {self._cli_version} not supported with service accounts. Minimum version: {MINIMUM_SERVICE_ACCOUNT_VERSION}")
             if existing_auth != EXISTING_AUTH_REQD:
                 auth_pref_source = "preference upgraded due to service account environment variable"
                 self.logger.info(
                     f"{self.OP_SVC_ACCOUNT_ENV_VAR} was set. Upgrading existing auth flag to REQUIRED")
                 existing_auth = EXISTING_AUTH_REQD
 
         if existing_auth == EXISTING_AUTH_REQD and password is not None:
             # if a password is passed in but existing_auth is required, caller may be confused:
             # - intentionally passed in incompatible options
             # - possibly has OP_SERVICE_ACCOUNT_TOKEN set accidentally
-            msg = f"Password argument passed but EXISTING_AUTH_REQD flag is set. flag source: {auth_pref_source}"
+            msg = f"Password argument passed but EXISTING_AUTH_REQD flag is set. flag source: {auth_pref_source}"  # nopep8
             self.logger.error(msg)
             raise OPAuthenticationException(msg)
 
         # So far everything above has been fairly lightweight, with no remote
         # contact to the 1Password account.
         # The next steps will attempt to talk to the 1Password account, and
         # failing that, may attempt to authenticate to the 1Password account
@@ -155,23 +154,67 @@
                 # if we weren't provided an account identifier,
                 # we can now get it from the signed-in account object
                 # and compute the session environment variable name
                 self._account_identifier = account_obj.user_uuid
                 self._sess_var = self._compute_session_var_name()
             environ[self._sess_var] = self.token
 
+    @classmethod
+    def _reset_class(cls):
+        """
+        Reset class state
+
+        Primarily for use in pytest between test cases
+        """
+        cls._version_support = OPVersionSupport()
+        cls._op_paths_checked = set()
+        cls._reset_class_logger()
+
     @property
     def token(self) -> str:
         return self._token
 
     @property
     def session_var(self) -> str:
         return self._sess_var
 
     @classmethod
+    def _op_path_size_mtime(cls, op_path):
+        # get fully-qualified path even if "op" was provided
+        new_op_path = shutil.which(op_path)
+        if new_op_path:
+            op_path = new_op_path
+        stat_result = os.stat(op_path)
+        sz = stat_result.st_size
+        mt = stat_result.st_mtime
+        return (sz, mt)
+
+    @classmethod
+    def _check_op_version(cls, op_path, cli_version=None):
+        if not isinstance(op_path, str):
+            op_path = str(op_path)
+        try:
+            sz_mt = cls._op_path_size_mtime(op_path)
+        except FileNotFoundError as err:
+            raise OPNotFoundException(op_path, err.errno)
+
+        # don't check 'op' at the same path more than once
+        # but allow for different 'op' executables to be used
+        # over the course of execution
+        if sz_mt not in cls._op_paths_checked:
+            if cli_version:
+                ver = cli_version
+            else:
+                ver = cls._get_cli_version(op_path)
+            # exception is raised if version is unsupported
+            # deprecation warning is issued if version support is deprecated
+            cls._version_support.check_version_support(ver)
+            cls._op_paths_checked.add(sz_mt)
+
+    @classmethod
     def svc_account_env_var_set(cls):
         svc_acct_set = False
         if environ.get(cls.OP_SVC_ACCOUNT_ENV_VAR):
             svc_acct_set = True
         return svc_acct_set
 
     @classmethod
@@ -192,29 +235,30 @@
                     continue
                 # There is at least one account_shorthand found in `op account list`
                 uses_bio = False
                 break
         return uses_bio
 
     def _gather_facts(self):
+        self._cli_version = self._get_cli_version(self.op_path)
+        self._check_op_version(self.op_path, cli_version=self._cli_version)
         self._uses_bio = self.uses_biometric(
             op_path=self.op_path, account_list=self._account_list)
         self.logger.debug(f"uses bio: {self._uses_bio}")
         try:
             # if we haven't done a sign-in via the CLI/without desktop app integration
             # there won't be a config
             self._op_config = OPCLIConfig()
         except OPConfigNotFoundException:
             if self._uses_bio:
                 # set this to None. We should only use it if biometric is diabled,
                 # in which case this should be a hard error
                 self._op_config = None
             else:
                 raise
-        self._cli_version = self._get_cli_version(self.op_path)
         self._account_list = self._get_account_list(self.op_path)
 
         self._account_identifier = self._normalize_account_id()
         self._sess_var = self._compute_session_var_name()
 
     @classmethod
     def _get_cli_version(cls, op_path: str) -> OPCLIVersion:
@@ -411,14 +455,16 @@
         # under the hood, it calls 'whoami' which will fail if not authenticated
         #
         # We need to remove this as soon as possible if a better way becomes available
         # among the problems:
         # - this method is racey, since authentication may expire between the check and the
         #   operation
         # - this adds roughly 20% overhead (as measured by the full suite of pytest tests)
+
+        cls._check_op_version(op_path)
         if cls._auth_expired(op_path, account):
             raise OPAuthenticationException(
                 "Authentication has expired")  # pragma: no cover
 
         if cls.svc_account_env_var_set():
             err_msg = None
             supported = argv.svc_account_supported()
@@ -439,24 +485,26 @@
                         capture_stdout=capture_stdout,
                         input=input,
                         decode=decode,
                         env=env)
 
     @classmethod
     def _item_template_list_special(cls, op_path,  env: Dict[str, str] = None):
+        cls._check_op_version(op_path)
         if not env:
             env = dict(environ)
         # special "template list" class method we can use for testing authentication
         argv = _OPArgv.item_template_list_argv(op_path)
         template_list_json = cls._run(
             argv, capture_stdout=True, decode="utf-8", env=env)
         return template_list_json
 
     @classmethod
     def _whoami_base(cls, op_path, env: Dict[str, str] = None, account: str = None):
+        cls._check_op_version(op_path)
         if not env:
             env = dict(environ)
         argv = _OPArgv.whoami_argv(op_path, account=account)
         account_json = cls._run(
             argv, capture_stdout=True, decode="utf-8", env=env)
         return account_json
 
@@ -535,23 +583,14 @@
 
         try:
             document_bytes = self._run_with_auth_check(
                 self.op_path, self._account_identifier, get_document_argv, capture_stdout=True)
         except OPCmdFailedException as ocfe:
             raise OPDocumentGetException.from_opexception(ocfe) from ocfe
 
-        if self._cli_version <= DOCUMENT_BYTES_BUG_VERSION:  # pragma: no cover
-            # op versions 2.0.0 - 2.2.0 append an erroneous \x0a ('\n') byte to document bytes
-            # trim it off if its present
-            if document_bytes[-1] == 0x0a:
-                document_bytes = document_bytes[:-1]
-            else:
-                # this shouldn't happen but maybe an edge case?
-                pass
-
         return document_bytes
 
     def _document_edit(self,
                        document_identifier: str,
                        document_bytes: bytes,
                        file_name: Optional[str] = None,
                        new_title: Optional[str] = None,
@@ -635,14 +674,15 @@
         except OPCmdFailedException as ocfe:
             raise OPItemGetException.from_opexception(ocfe) from ocfe
 
         return output
 
     @classmethod
     def _signed_in_accounts(cls, op_path, decode="utf-8"):
+        cls._check_op_version(op_path)
         account_list_argv = cls._account_list_argv(op_path, encoding=decode)
         output = cls._run(account_list_argv,
                           capture_stdout=True, decode=decode)
         return output
 
     def _user_get(self, user_name_or_id: str, decode: str = "utf-8") -> str:
         user_get_argv = self._user_get_argv(user_name_or_id)
@@ -725,14 +765,18 @@
                 "Biometric is enabled. 'forget' operation will have no effect.")
         argv = _OPArgv.signout_argv(
             self.op_path, account, session, forget=forget, uses_bio=self._uses_bio)
         self._run(argv)
 
     @classmethod
     def _account_forget(cls, account: str, op_path=None):   # pragma: no cover
+        # don't call _check_op_version()
+        # this probably won't fail, and at any rate
+        # shouldn't be in the critical path for any other operation
+        # there's no reason to prevent "account forget" from working here
         if not op_path:
             op_path = cls.OP_PATH
         argv = _OPArgv.account_forget_argv(op_path, account)
         cls._run(argv)
 
     def _item_list(self, categories=[], include_archive=False, tags=[], vault=None, decode="utf-8"):
         # default lists to the categories & list kwargs
```

### Comparing `pyonepassword-4.3.0/pyonepassword/_py_op_deprecation.py` & `pyonepassword-5.0.0/pyonepassword/_py_op_deprecation.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         if self.extra:
             msg += ": {}".format(self.extra)
 
         init = cls.__init__
 
         def wrapped(_self, *args, **kwargs):
             if not getattr(_self, "_skip_drecation_warn", False):
-                warnings.warn(msg, category=FutureWarning)
+                warnings.warn(msg, category=DeprecationWarning)
             return init(_self, *args, **kwargs)
         cls.__init__ = wrapped
 
         wrapped.__name__ = '__init__'
         wrapped.__doc__ = self._update_doc(init.__doc__)
 
         # mypy doesn't like wrapped.deprecated_original = init
@@ -46,15 +46,15 @@
 
         msg = "Function %s is deprecated" % fun.__name__
         if self.extra:
             msg += "; %s" % self.extra
 
         @functools.wraps(fun)
         def wrapped(*args, **kwargs):
-            warnings.warn(msg, category=FutureWarning)
+            warnings.warn(msg, category=DeprecationWarning)
             return fun(*args, **kwargs)
 
         wrapped.__doc__ = self._update_doc(wrapped.__doc__)
 
         return wrapped
 
     def _update_doc(self, olddoc):
@@ -62,15 +62,15 @@
         if self.extra:
             newdoc = "%s: %s" % (newdoc, self.extra)
         if olddoc:
             newdoc = "%s\n\n    %s" % (newdoc, olddoc)
         return newdoc
 
 
-def deprecated_kwargs(**kwarg_aliases: str) -> Callable:
+def deprecated_kwargs(**kwarg_aliases: str) -> Callable:  # pragma: no cover
     """Decorator for deprecated function and method arguments.
 
     Use as follows:
 
     @deprecated_kwargs(old_arg='new_arg')
     def myfunc(new_arg):
         ...
@@ -90,19 +90,19 @@
 
 def _rename_kwargs(func_name: str, kwargs: Dict[str, Any], kwarg_aliases: Dict[str, str]):  # pragma: no cover
     """Helper function for deprecating function arguments."""
     for old_kwarg, new_kwarg in kwarg_aliases.items():
         if old_kwarg in kwargs:
             if new_kwarg in kwargs:
                 raise TypeError(
-                    f"{func_name} received both {old_kwarg} and {new_kwarg} as arguments!"
+                    f"{func_name} received both {old_kwarg} and {new_kwarg} as arguments!"  # nopep8
                     f" {old_kwarg} is deprecated, use {new_kwarg} instead."
                 )
             warnings.warn(
                 message=(
-                    f"`{old_kwarg}` is deprecated as an argument to `{func_name}`; use"
+                    f"`{old_kwarg}` is deprecated as an argument to `{func_name}`; use"  # nopep8
                     f" `{new_kwarg}` instead."
                 ),
-                category=FutureWarning,
+                category=DeprecationWarning,
                 stacklevel=3,
             )
             kwargs[new_kwarg] = kwargs.pop(old_kwarg)
```

### Comparing `pyonepassword-4.3.0/pyonepassword/_svc_account.py` & `pyonepassword-5.0.0/pyonepassword/_svc_account.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,15 +175,15 @@
             cmd_dict = cmd_spec.command_lookup(subcommand_list=subcommands)
 
         # if we either failed to find a command spec or
         # we found a command spec but not a subcommand dictionary
         # then command is not supported
         _cmd_not_found = command is not None and cmd_spec is None
         if (cmd_spec and not cmd_dict) or _cmd_not_found:
-            _support_msg = f"Command or subcommand not supported: [{command} {' '.join(subcommands)}]"
+            _support_msg = f"Command or subcommand not supported: [{command} {' '.join(subcommands)}]"  # nopep8
             _support_code = SVC_ACCT_CMD_NOT_SUPPORTED
 
         if cmd_dict and _support_code == _SVC_ACCT_CMD_NOT_VALIDATED:
             required_options = set(cmd_dict["required_options"])
 
             # how many required options remain after we mask out
             # the provided options? Hopefully none
@@ -216,18 +216,18 @@
             if required_opt_satified and prohibited_opt_satisfied:
                 # if both
                 _support_code = SVC_ACCT_SUPPORTED
 
         if _support_code == SVC_ACCT_INCOMPAT_OPTIONS:
             _support_msg = ""
             if not required_opt_satified:
-                _support_msg += f"Required options not provided: [{','.join(list(reqd_opt_diff))}]"
+                _support_msg += f"Required options not provided: [{','.join(list(reqd_opt_diff))}]"  # nopep8
 
             if not prohibited_opt_satisfied:
-                _support_msg += f" Prohibited options found: [{','.join(list(prohib_opt_diff))}]"
+                _support_msg += f" Prohibited options found: [{','.join(list(prohib_opt_diff))}]"  # nopep8
 
             _support_msg = _support_msg.lstrip()
 
         if _support_code == _SVC_ACCT_CMD_NOT_VALIDATED:  # pragma: no cover
             # something's gone wrong if we reach this point
             raise Exception("Failed to validate service account compatibility")
```

### Comparing `pyonepassword-4.3.0/pyonepassword/account.py` & `pyonepassword-5.0.0/pyonepassword/account.py`

 * *Files identical despite different names*

### Comparing `pyonepassword-4.3.0/pyonepassword/api/descriptor_types.py` & `pyonepassword-5.0.0/pyonepassword/api/descriptor_types.py`

 * *Files identical despite different names*

### Comparing `pyonepassword-4.3.0/pyonepassword/api/object_types.py` & `pyonepassword-5.0.0/pyonepassword/api/object_types.py`

 * *Files identical despite different names*

### Comparing `pyonepassword-4.3.0/pyonepassword/api/validation.py` & `pyonepassword-5.0.0/pyonepassword/api/validation.py`

 * *Files identical despite different names*

### Comparing `pyonepassword-4.3.0/pyonepassword/data/api_credential.json` & `pyonepassword-5.0.0/pyonepassword/data/api_credential.json`

 * *Files identical despite different names*

### Comparing `pyonepassword-4.3.0/pyonepassword/data/bank_account.json` & `pyonepassword-5.0.0/pyonepassword/data/bank_account.json`

 * *Files identical despite different names*

### Comparing `pyonepassword-4.3.0/pyonepassword/data/credit_card.json` & `pyonepassword-5.0.0/pyonepassword/data/credit_card.json`

 * *Files identical despite different names*

### Comparing `pyonepassword-4.3.0/pyonepassword/data/crypto_wallet.json` & `pyonepassword-5.0.0/pyonepassword/data/crypto_wallet.json`

 * *Files identical despite different names*

### Comparing `pyonepassword-4.3.0/pyonepassword/data/database.json` & `pyonepassword-5.0.0/pyonepassword/data/database.json`

 * *Files identical despite different names*

### Comparing `pyonepassword-4.3.0/pyonepassword/data/driver_license.json` & `pyonepassword-5.0.0/pyonepassword/data/driver_license.json`

 * *Files identical despite different names*

### Comparing `pyonepassword-4.3.0/pyonepassword/data/email_account.json` & `pyonepassword-5.0.0/pyonepassword/data/email_account.json`

 * *Files identical despite different names*

### Comparing `pyonepassword-4.3.0/pyonepassword/data/identity.json` & `pyonepassword-5.0.0/pyonepassword/data/identity.json`

 * *Files identical despite different names*

### Comparing `pyonepassword-4.3.0/pyonepassword/data/login.json` & `pyonepassword-5.0.0/pyonepassword/data/login.json`

 * *Files identical despite different names*

### Comparing `pyonepassword-4.3.0/pyonepassword/data/medical_record.json` & `pyonepassword-5.0.0/pyonepassword/data/medical_record.json`

 * *Files identical despite different names*

### Comparing `pyonepassword-4.3.0/pyonepassword/data/membership.json` & `pyonepassword-5.0.0/pyonepassword/data/membership.json`

 * *Files identical despite different names*

### Comparing `pyonepassword-4.3.0/pyonepassword/data/outdoor_license.json` & `pyonepassword-5.0.0/pyonepassword/data/outdoor_license.json`

 * *Files identical despite different names*

### Comparing `pyonepassword-4.3.0/pyonepassword/data/passport.json` & `pyonepassword-5.0.0/pyonepassword/data/passport.json`

 * *Files identical despite different names*

### Comparing `pyonepassword-4.3.0/pyonepassword/data/reward_program.json` & `pyonepassword-5.0.0/pyonepassword/data/reward_program.json`

 * *Files identical despite different names*

### Comparing `pyonepassword-4.3.0/pyonepassword/data/server.json` & `pyonepassword-5.0.0/pyonepassword/data/server.json`

 * *Files identical despite different names*

### Comparing `pyonepassword-4.3.0/pyonepassword/data/software_license.json` & `pyonepassword-5.0.0/pyonepassword/data/software_license.json`

 * *Files identical despite different names*

### Comparing `pyonepassword-4.3.0/pyonepassword/data/svc_acct_commands/README.md` & `pyonepassword-5.0.0/pyonepassword/data/svc_acct_commands/README.md`

 * *Files identical despite different names*

### Comparing `pyonepassword-4.3.0/pyonepassword/data/svc_acct_commands/item.json` & `pyonepassword-5.0.0/pyonepassword/data/svc_acct_commands/item.json`

 * *Files identical despite different names*

### Comparing `pyonepassword-4.3.0/pyonepassword/data/template-registry.json` & `pyonepassword-5.0.0/pyonepassword/data/template-registry.json`

 * *Files identical despite different names*

### Comparing `pyonepassword-4.3.0/pyonepassword/data/wireless_router.json` & `pyonepassword-5.0.0/pyonepassword/data/wireless_router.json`

 * *Files identical despite different names*

### Comparing `pyonepassword-4.3.0/pyonepassword/op_items/_item_descriptor_registry.py` & `pyonepassword-5.0.0/pyonepassword/op_items/_item_descriptor_registry.py`

 * *Files identical despite different names*

### Comparing `pyonepassword-4.3.0/pyonepassword/op_items/_item_list.py` & `pyonepassword-5.0.0/pyonepassword/op_items/_item_list.py`

 * *Files identical despite different names*

### Comparing `pyonepassword-4.3.0/pyonepassword/op_items/_item_type_registry.py` & `pyonepassword-5.0.0/pyonepassword/op_items/_item_type_registry.py`

 * *Files identical despite different names*

### Comparing `pyonepassword-4.3.0/pyonepassword/op_items/_new_field_registry.py` & `pyonepassword-5.0.0/pyonepassword/op_items/_new_field_registry.py`

 * *Files identical despite different names*

### Comparing `pyonepassword-4.3.0/pyonepassword/op_items/_new_item.py` & `pyonepassword-5.0.0/pyonepassword/op_items/_new_item.py`

 * *Files identical despite different names*

### Comparing `pyonepassword-4.3.0/pyonepassword/op_items/field_registry.py` & `pyonepassword-5.0.0/pyonepassword/op_items/field_registry.py`

 * *Files identical despite different names*

### Comparing `pyonepassword-4.3.0/pyonepassword/op_items/fields_sections/_new_fields.py` & `pyonepassword-5.0.0/pyonepassword/op_items/fields_sections/_new_fields.py`

 * *Files identical despite different names*

### Comparing `pyonepassword-4.3.0/pyonepassword/op_items/fields_sections/item_field.py` & `pyonepassword-5.0.0/pyonepassword/op_items/fields_sections/item_field.py`

 * *Files identical despite different names*

### Comparing `pyonepassword-4.3.0/pyonepassword/op_items/fields_sections/item_field_base.py` & `pyonepassword-5.0.0/pyonepassword/op_items/fields_sections/item_field_base.py`

 * *Files identical despite different names*

### Comparing `pyonepassword-4.3.0/pyonepassword/op_items/fields_sections/item_section.py` & `pyonepassword-5.0.0/pyonepassword/op_items/fields_sections/item_section.py`

 * *Files identical despite different names*

### Comparing `pyonepassword-4.3.0/pyonepassword/op_items/item_types/_item_base.py` & `pyonepassword-5.0.0/pyonepassword/op_items/item_types/_item_base.py`

 * *Files identical despite different names*

### Comparing `pyonepassword-4.3.0/pyonepassword/op_items/item_types/_item_descriptor_base.py` & `pyonepassword-5.0.0/pyonepassword/op_items/item_types/_item_descriptor_base.py`

 * *Files identical despite different names*

### Comparing `pyonepassword-4.3.0/pyonepassword/op_items/item_types/api_credential.py` & `pyonepassword-5.0.0/pyonepassword/op_items/item_types/api_credential.py`

 * *Files identical despite different names*

### Comparing `pyonepassword-4.3.0/pyonepassword/op_items/item_types/credit_card.py` & `pyonepassword-5.0.0/pyonepassword/op_items/item_types/credit_card.py`

 * *Files identical despite different names*

### Comparing `pyonepassword-4.3.0/pyonepassword/op_items/item_types/database.py` & `pyonepassword-5.0.0/pyonepassword/op_items/item_types/database.py`

 * *Files identical despite different names*

### Comparing `pyonepassword-4.3.0/pyonepassword/op_items/item_types/document.py` & `pyonepassword-5.0.0/pyonepassword/op_items/item_types/document.py`

 * *Files identical despite different names*

### Comparing `pyonepassword-4.3.0/pyonepassword/op_items/item_types/generic_item.py` & `pyonepassword-5.0.0/pyonepassword/op_items/item_types/generic_item.py`

 * *Files identical despite different names*

### Comparing `pyonepassword-4.3.0/pyonepassword/op_items/item_types/login.py` & `pyonepassword-5.0.0/pyonepassword/op_items/item_types/login.py`

 * *Files identical despite different names*

### Comparing `pyonepassword-4.3.0/pyonepassword/op_items/item_types/password.py` & `pyonepassword-5.0.0/pyonepassword/op_items/item_types/password.py`

 * *Files identical despite different names*

### Comparing `pyonepassword-4.3.0/pyonepassword/op_items/item_types/secure_note.py` & `pyonepassword-5.0.0/pyonepassword/op_items/item_types/secure_note.py`

 * *Files identical despite different names*

### Comparing `pyonepassword-4.3.0/pyonepassword/op_items/item_types/server.py` & `pyonepassword-5.0.0/pyonepassword/op_items/item_types/server.py`

 * *Files identical despite different names*

### Comparing `pyonepassword-4.3.0/pyonepassword/op_items/item_types/ssh_key.py` & `pyonepassword-5.0.0/pyonepassword/op_items/item_types/ssh_key.py`

 * *Files identical despite different names*

### Comparing `pyonepassword-4.3.0/pyonepassword/op_items/item_validation_policy.py` & `pyonepassword-5.0.0/pyonepassword/op_items/item_validation_policy.py`

 * *Files identical despite different names*

### Comparing `pyonepassword-4.3.0/pyonepassword/op_items/password_recipe.py` & `pyonepassword-5.0.0/pyonepassword/op_items/password_recipe.py`

 * *Files identical despite different names*

### Comparing `pyonepassword-4.3.0/pyonepassword/op_items/template_directory.py` & `pyonepassword-5.0.0/pyonepassword/op_items/template_directory.py`

 * *Files identical despite different names*

### Comparing `pyonepassword-4.3.0/pyonepassword/op_items/totp.py` & `pyonepassword-5.0.0/pyonepassword/op_items/totp.py`

 * *Files identical despite different names*

### Comparing `pyonepassword-4.3.0/pyonepassword/op_items/uuid.py` & `pyonepassword-5.0.0/pyonepassword/op_items/uuid.py`

 * *Files identical despite different names*

### Comparing `pyonepassword-4.3.0/pyonepassword/op_objects.py` & `pyonepassword-5.0.0/pyonepassword/op_objects.py`

 * *Files identical despite different names*

### Comparing `pyonepassword-4.3.0/pyonepassword/opconfig_main.py` & `pyonepassword-5.0.0/pyonepassword/opconfig_main.py`

 * *Files identical despite different names*

### Comparing `pyonepassword-4.3.0/pyonepassword/py_op_exceptions.py` & `pyonepassword-5.0.0/pyonepassword/py_op_exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -364,11 +364,11 @@
     # module level __getattr__() is valid as of python 3.7, pep-562
     # handling deprecation warnings on import is a key use-case
     # https://peps.python.org/pep-0562/
     if name in _deprecated_exceptions:
         _deprecated_name = f"_{name}"
         alternate = _deprecated_exceptions[name]
         warnings.warn(
-            f"Exception class {name} is deprecated. Use {alternate}", category=FutureWarning)
+            f"Exception class {name} is deprecated. Use {alternate}", category=DeprecationWarning)
         return globals()[_deprecated_name]
 
     raise AttributeError(f"module {__name__!r} has no attribute {name!r}")
```

### Comparing `pyonepassword-4.3.0/pyonepassword/pyonepassword.py` & `pyonepassword-5.0.0/pyonepassword/pyonepassword.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from pathlib import Path
 from typing import TYPE_CHECKING, List, Optional, Type, Union
 
 if TYPE_CHECKING:  # pragma: no coverage
     from .op_items.fields_sections.item_field import OPItemField
 
 from ._field_assignment import OPFieldTypeEnum
+from ._op_cli_version import OPCLIVersion
 from ._op_commands import (
     EXISTING_AUTH_IGNORE,
     ExistingAuthEnum,
     _OPCommandInterface
 )
 from .account import OPAccountList
 from .op_items._item_list import OPItemList
@@ -1879,14 +1880,93 @@
         """
 
         try:
             cls._account_forget(account, op_path=op_path)
         except OPCmdFailedException as ocfe:
             raise OPForgetException.from_opexception(ocfe) from ocfe
 
+    @classmethod
+    def check_op_version(cls, op_path="op") -> None:
+        """
+        Check support for the 'op' version in use.
+
+        If the version is supported but deprecated, DeprecationWarning is issued
+
+        If the version is unsupported, OPCLIVersionSupportException is raised
+
+        Parameters
+        ----------
+        op_path: str, optional
+            Path to an 'op' executable to use for this action, by default "op"
+
+        Raises
+        ------
+        OPCLIVersionSupportException
+            If the op version is less than the minimum supported version
+
+        Service Account Support
+        -----------------------
+        Supported
+        """
+        cls._check_op_version(op_path)
+
+    @classmethod
+    def supported_op_version(cls) -> OPCLIVersion:
+        """
+        Return the minimum supported 'op' CLI version.
+        Versions less than this value are either deprecated or unsupported.
+
+        Notes:
+            - The OPCLIVersion object may be converted to a string via str()
+            - The version object may be compared to other version objects via less-than
+              greater-than, etc
+            - The version object may be compared to other version strings in the same way
+            - Beta versions are considered less than release version, so e.g.,
+              2.28.0-beta.01 < 2.28.0
+
+        Returns
+        -------
+        OPCLIVersion
+            The object representing the deprecated version threshold
+
+        Service Account Support
+        -----------------------
+        Supported
+        """
+        version = cls._version_support.supported_version
+        return version
+
+    @classmethod
+    def minimum_op_version(cls) -> OPCLIVersion:
+        """
+        Return the minimum supported but deprecated 'op' CLI version.
+
+        A deprecation warning is issued if versions
+        Versions less than this are unsupported
+
+        Notes:
+            - The OPCLIVersion object may be converted to a string via str()
+            - The version object may be compared to other version objects via less-than
+              greater-than, etc
+            - The version object may be compared to other version strings in the same way
+            - Beta versions are considered less than release version, so e.g.,
+              2.28.0-beta.01 < 2.28.0
+
+        Returns
+        -------
+        OPCLIVersion
+            The object representing the minimum supported version threshold
+
+        Service Account Support
+        -----------------------
+        Supported
+        """
+        version = cls._version_support.minimum_version
+        return version
+
     def _sanitize(self):  # pragma: no coverage
         self._token = None
         if self._sess_var:
             try:
                 env.pop(self._sess_var)
             except KeyError:
                 pass
@@ -2015,15 +2095,15 @@
                 break
 
         if not field:
             if not section_label:
                 msg = f"No field found '{field_label}' that lacks a section"
                 raise OPFieldNotFoundException(msg)
             else:
-                msg = f"Section '{section_label}', field '{field_label}' not found"
+                msg = f"Section '{section_label}', field '{field_label}' not found"  # nopep8
                 raise OPFieldNotFoundException(msg)
         return field
 
     def _validate_item_field_does_not_exist(self,
                                             item: OPAbstractItem,
                                             field_label: str,
                                             section_label: Optional[str]) -> None:
```

### Comparing `pyonepassword-4.3.0/pyonepassword/string.py` & `pyonepassword-5.0.0/pyonepassword/string.py`

 * *Files identical despite different names*

### Comparing `pyonepassword-4.3.0/pyonepassword/version.py` & `pyonepassword-5.0.0/pyonepassword/version.py`

 * *Files identical despite different names*

### Comparing `pyonepassword-4.3.0/pyonepassword.egg-info/PKG-INFO` & `pyonepassword-5.0.0/pyonepassword.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyonepassword
-Version: 4.3.0
+Version: 5.0.0
 Summary: A python API to query a 1Password account using the 'op' command-line tool
 Home-page: https://github.com/zcutlip/pyonepassword
 Author: Zachary Cutlip
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -31,20 +31,24 @@
 ## Description
 
 A Python API to sign into and query a 1Password account using the `op` command.
 
 ## Requirements
 
 - Python >= 3.9
-- 1Password command-line tool >= 2.0.0
-  - see [1Password Developer Documentation](https://developer.1password.com/docs/cli)
+- 1Password command-line tool >= 2.24.0
+  - Versions >= 2.19.0, < 2.24.0 supported but deprecated
+  - Versions < 2.19.0 are unsupported and an exception will be raised
+  - See [1Password Developer Documentation](https://developer.1password.com/docs/cli)
 - Internet connectivity to 1Password.com
   - The `op` command queries your online account, not your local vault
 
-> Note: This version of `pyonepassword` does not support deprecated `op` 1.x versions. Support for those versions is still available, albeit with minimal maintanence. See [pyonepassword-legacy](https://github.com/zcutlip/pyonepassword-legacy) for more information.
+> Notes:
+> - Generally `pyonepassword` will support up to 5 patch versions, including the current. E.g., 2.{24-28}.0. Five additional patch versions, e.g., 2.{19-23}.0, will be considered deprecated.
+> - This version of `pyonepassword` does not support deprecated `op` 1.x versions. Support for those versions is still available, albeit with minimal maintanence. See [pyonepassword-legacy](https://github.com/zcutlip/pyonepassword-legacy) for more information.
 
 ## Installation
 
 ```shell
 python3 -m pip install pyonepassword
 ```
```

### Comparing `pyonepassword-4.3.0/pyonepassword.egg-info/SOURCES.txt` & `pyonepassword-5.0.0/pyonepassword.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,43 +1,48 @@
 LICENSE
+MANIFEST.in
 README.md
+_readme_template.md
+pyproject.toml
 setup.cfg
 setup.py
 pyonepassword/__about__.py
 pyonepassword/__init__.py
 pyonepassword/_abc_meta.py
 pyonepassword/_api_initializer.py
 pyonepassword/_datetime.py
 pyonepassword/_field_assignment.py
 pyonepassword/_op_cli.py
 pyonepassword/_op_cli_argv.py
 pyonepassword/_op_cli_config.py
+pyonepassword/_op_cli_version.py
 pyonepassword/_op_commands.py
 pyonepassword/_py_op_deprecation.py
 pyonepassword/_svc_account.py
 pyonepassword/account.py
 pyonepassword/json.py
 pyonepassword/logging.py
-pyonepassword/op_cli_version.py
 pyonepassword/op_objects.py
 pyonepassword/opconfig_main.py
+pyonepassword/opversion_main.py
 pyonepassword/pkg_resources.py
 pyonepassword/py.typed
 pyonepassword/py_op_exceptions.py
 pyonepassword/pyonepassword.py
 pyonepassword/string.py
 pyonepassword/version.py
 pyonepassword.egg-info/PKG-INFO
 pyonepassword.egg-info/SOURCES.txt
 pyonepassword.egg-info/dependency_links.txt
 pyonepassword.egg-info/entry_points.txt
 pyonepassword.egg-info/requires.txt
 pyonepassword.egg-info/top_level.txt
 pyonepassword/api/__init__.py
 pyonepassword/api/authentication.py
+pyonepassword/api/cli_version.py
 pyonepassword/api/constants.py
 pyonepassword/api/decorators.py
 pyonepassword/api/descriptor_types.py
 pyonepassword/api/exceptions.py
 pyonepassword/api/object_types.py
 pyonepassword/api/validation.py
 pyonepassword/data/__init__.py
@@ -61,14 +66,17 @@
 pyonepassword/data/server.json
 pyonepassword/data/social_security_number.json
 pyonepassword/data/software_license.json
 pyonepassword/data/ssh_key.json
 pyonepassword/data/template-registry.json
 pyonepassword/data/wireless_router.json
 pyonepassword/data/__pycache__/__init__.cpython-312.pyc
+pyonepassword/data/op_versions/__init__.py
+pyonepassword/data/op_versions/version_support.json
+pyonepassword/data/op_versions/version_support_readme.md
 pyonepassword/data/svc_acct_commands/README.md
 pyonepassword/data/svc_acct_commands/__init__.py
 pyonepassword/data/svc_acct_commands/account.json
 pyonepassword/data/svc_acct_commands/document.json
 pyonepassword/data/svc_acct_commands/group.json
 pyonepassword/data/svc_acct_commands/item.json
 pyonepassword/data/svc_acct_commands/signout.json
@@ -102,16 +110,16 @@
 pyonepassword/op_items/item_types/generic_item.py
 pyonepassword/op_items/item_types/identity.py
 pyonepassword/op_items/item_types/login.py
 pyonepassword/op_items/item_types/password.py
 pyonepassword/op_items/item_types/secure_note.py
 pyonepassword/op_items/item_types/server.py
 pyonepassword/op_items/item_types/ssh_key.py
+scripts/update_readme.py
 tests/test_abstract_base_meta.py
-tests/test_cli_version.py
 tests/test_datetime.py
 tests/test_deprecation_warnings.py
 tests/test_exports.py
 tests/test_item_errors.py
 tests/test_item_field.py
 tests/test_item_section.py
 tests/test_op_cli.py
```

### Comparing `pyonepassword-4.3.0/setup.cfg` & `pyonepassword-5.0.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyonepassword-4.3.0/tests/test_abstract_base_meta.py` & `pyonepassword-5.0.0/tests/test_abstract_base_meta.py`

 * *Files identical despite different names*

### Comparing `pyonepassword-4.3.0/tests/test_datetime.py` & `pyonepassword-5.0.0/tests/test_datetime.py`

 * *Files identical despite different names*

### Comparing `pyonepassword-4.3.0/tests/test_deprecation_warnings.py` & `pyonepassword-5.0.0/tests/test_deprecation_warnings.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
-import warnings
 from typing import TYPE_CHECKING
 
+import pytest
+
 from pyonepassword.api.object_types import OPLoginItem
 
 if TYPE_CHECKING:
     from .fixtures.valid_data import ValidData
 # disabled but left as example
 # def example_test_import_deprecation_01():
 #     """
@@ -45,11 +46,12 @@
     """
     field_label = "Example Field"
     section_label = "Example Section 1"
 
     valid_item_dict = valid_data.data_for_name("example-login-with-fields")
     result_login_item = OPLoginItem(valid_item_dict)
 
-    with warnings.catch_warnings(record=True) as warnings_list:
+    # not useful to inspect the warnings_list produced by warns()
+    # it may collect other warnings not relevent to the test
+    with pytest.warns(DeprecationWarning):
         result_login_item.field_value_by_section_title(
             section_label, field_label)
-        assert len(warnings_list) > 0
```

### Comparing `pyonepassword-4.3.0/tests/test_exports.py` & `pyonepassword-5.0.0/tests/test_exports.py`

 * *Files identical despite different names*

### Comparing `pyonepassword-4.3.0/tests/test_item_errors.py` & `pyonepassword-5.0.0/tests/test_item_errors.py`

 * *Files identical despite different names*

### Comparing `pyonepassword-4.3.0/tests/test_item_field.py` & `pyonepassword-5.0.0/tests/test_item_field.py`

 * *Files identical despite different names*

### Comparing `pyonepassword-4.3.0/tests/test_item_section.py` & `pyonepassword-5.0.0/tests/test_item_section.py`

 * *Files identical despite different names*

### Comparing `pyonepassword-4.3.0/tests/test_op_cli.py` & `pyonepassword-5.0.0/tests/test_op_cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,17 +5,17 @@
     OPCLIPanicException,
     OPNotFoundException,
     OPSigninException
 )
 
 
 @pytest.mark.usefixtures("valid_op_cli_config_homedir")
-def test_missing_op():
+def test_missing_op(console_logger):
     with pytest.raises(OPNotFoundException):
-        OP(op_path="no-such-op")
+        OP(op_path="no-such-op", logger=console_logger)
 
 
 @pytest.mark.usefixtures("valid_op_cli_config_homedir")
 @pytest.mark.usefixtures("setup_normal_op_env_signin_failure")
 def test_signin_fail():
     with pytest.raises(OPSigninException):
         OP(op_path="mock-op")
```

### Comparing `pyonepassword-4.3.0/tests/test_op_cli_config.py` & `pyonepassword-5.0.0/tests/test_op_cli_config.py`

 * *Files identical despite different names*

### Comparing `pyonepassword-4.3.0/tests/test_password_recipe.py` & `pyonepassword-5.0.0/tests/test_password_recipe.py`

 * *Files identical despite different names*

### Comparing `pyonepassword-4.3.0/tests/test_redacted_string.py` & `pyonepassword-5.0.0/tests/test_redacted_string.py`

 * *Files identical despite different names*

