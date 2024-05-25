# Comparing `tmp/icpp-candid-3.8.1.tar.gz` & `tmp/icpp-candid-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icpp-candid-3.8.1.tar", last modified: Mon Nov 27 16:06:58 2023, max compression
+gzip compressed data, was "icpp-candid-3.9.0.tar", last modified: Fri Dec  8 19:57:19 2023, max compression
```

## Comparing `icpp-candid-3.8.1.tar` & `icpp-candid-3.9.0.tar`

### file list

```diff
@@ -1,192 +1,192 @@
-drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-11-27 16:06:58.396269 icpp-candid-3.8.1/
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1066 2023-10-03 19:33:28.000000 icpp-candid-3.8.1/LICENSE
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2287 2023-11-27 16:06:58.396269 icpp-candid-3.8.1/PKG-INFO
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1339 2023-10-18 15:36:18.000000 icpp-candid-3.8.1/README.md
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      469 2023-11-25 14:22:42.000000 icpp-candid-3.8.1/pyproject.toml
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)       38 2023-11-27 16:06:58.396269 icpp-candid-3.8.1/setup.cfg
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     9863 2023-10-03 19:33:28.000000 icpp-candid-3.8.1/setup.py
-drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-11-27 16:06:58.364269 icpp-candid-3.8.1/src/
-drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-11-27 16:06:58.364269 icpp-candid-3.8.1/src/icpp_candid/
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      652 2023-10-03 19:33:28.000000 icpp-candid-3.8.1/src/icpp_candid/__init__.py
-drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-11-27 16:06:58.388269 icpp-candid-3.8.1/src/icpp_candid/candid/
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)      852 2023-10-28 13:16:25.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_args.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      362 2023-10-18 15:35:50.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_args.h
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1684 2023-10-18 15:36:18.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_assert.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      613 2023-10-03 19:33:28.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_assert.h
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)       92 2023-10-23 17:52:03.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_constants.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      110 2023-11-27 11:29:06.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_debug_config.h
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)    33844 2023-11-25 12:41:09.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_deserialize.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1732 2023-10-26 11:12:21.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_deserialize.h
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)    11216 2023-11-18 12:29:10.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_opcode.cpp
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     3128 2023-11-15 20:50:24.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_opcode.h
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     3591 2023-11-20 11:37:46.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_serialize.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      753 2023-10-18 15:35:50.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_serialize.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     3880 2023-10-18 15:40:20.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_serialize_type_table_registry.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2714 2023-10-18 15:40:20.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_serialize_type_table_registry.h
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     3616 2023-11-12 14:31:22.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2452 2023-11-12 14:32:18.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_all_includes.h
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     6462 2023-11-18 12:02:10.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_base.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     5868 2023-11-20 11:30:37.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_base.h
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     2078 2023-10-25 11:07:54.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_bool.cpp
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)      958 2023-10-25 11:07:54.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_bool.h
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1186 2023-10-25 11:07:54.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_empty.cpp
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)      812 2023-10-25 11:07:54.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_empty.h
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     2280 2023-10-25 11:07:54.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_float32.cpp
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)      993 2023-10-25 11:07:54.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_float32.h
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     2287 2023-10-25 11:07:54.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_float64.cpp
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1001 2023-10-25 11:07:54.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_float64.h
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1995 2023-10-25 11:07:54.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_int.cpp
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)      998 2023-10-25 11:07:54.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_int.h
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     2046 2023-10-25 11:07:54.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_int16.cpp
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)      991 2023-10-25 11:07:54.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_int16.h
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     2046 2023-10-25 11:07:54.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_int32.cpp
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)      991 2023-10-25 11:07:54.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_int32.h
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     2046 2023-10-25 11:07:54.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_int64.cpp
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)      991 2023-10-25 11:07:54.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_int64.h
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     2019 2023-10-25 11:07:54.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_int8.cpp
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)      974 2023-10-25 11:07:54.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_int8.h
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     2016 2023-10-25 11:07:55.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_nat.cpp
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1005 2023-10-25 11:07:55.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_nat.h
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     2038 2023-10-25 11:07:54.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_nat16.cpp
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)      999 2023-10-25 11:07:54.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_nat16.h
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     2038 2023-10-25 11:07:54.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_nat32.cpp
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)      999 2023-10-25 11:07:54.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_nat32.h
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     2038 2023-10-25 11:07:55.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_nat64.cpp
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)      999 2023-10-25 11:07:55.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_nat64.h
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     2011 2023-10-25 11:07:55.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_nat8.cpp
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)      982 2023-10-25 11:07:55.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_nat8.h
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)      816 2023-10-18 15:30:28.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_null.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      835 2023-10-21 12:29:07.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_null.h
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     4570 2023-10-26 19:01:54.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_opt_bool.cpp
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1101 2023-10-25 11:07:55.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_opt_bool.h
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     4616 2023-10-26 19:01:54.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_opt_float32.cpp
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1130 2023-10-25 11:07:55.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_opt_float32.h
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     4622 2023-10-26 19:01:54.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_opt_float64.cpp
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1138 2023-10-25 11:07:55.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_opt_float64.h
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     4535 2023-10-26 19:01:54.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_opt_int.cpp
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1142 2023-10-25 11:07:55.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_opt_int.h
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     4572 2023-10-26 19:01:54.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_opt_int16.cpp
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1132 2023-10-25 11:07:55.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_opt_int16.h
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     4573 2023-10-26 19:01:54.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_opt_int32.cpp
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1134 2023-10-25 11:07:55.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_opt_int32.h
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     4573 2023-10-26 19:01:54.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_opt_int64.cpp
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1132 2023-10-25 11:07:55.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_opt_int64.h
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     4542 2023-10-26 19:01:54.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_opt_int8.cpp
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1117 2023-10-25 11:07:55.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_opt_int8.h
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     4541 2023-10-26 19:01:54.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_opt_nat.cpp
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1150 2023-10-25 11:07:55.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_opt_nat.h
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     4579 2023-10-26 19:01:54.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_opt_nat16.cpp
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1140 2023-10-25 11:07:55.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_opt_nat16.h
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     4579 2023-10-26 19:01:54.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_opt_nat32.cpp
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1140 2023-10-25 11:07:55.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_opt_nat32.h
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     4579 2023-10-26 19:01:54.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_opt_nat64.cpp
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1140 2023-10-25 11:07:55.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_opt_nat64.h
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     4548 2023-10-26 19:01:54.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_opt_nat8.cpp
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1125 2023-10-25 11:07:55.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_opt_nat8.h
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     3875 2023-10-26 19:01:54.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_opt_null.cpp
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1074 2023-10-25 11:07:55.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_opt_null.h
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     4902 2023-10-26 19:01:54.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_opt_principal.cpp
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1194 2023-10-25 11:07:55.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_opt_principal.h
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     7167 2023-11-18 11:41:26.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_opt_record.cpp
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1782 2023-11-14 13:15:21.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_opt_record.h
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     4846 2023-10-26 19:01:54.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_opt_text.cpp
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1157 2023-10-25 11:07:55.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_opt_text.h
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     7252 2023-11-14 17:07:33.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_opt_variant.cpp
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1796 2023-11-14 13:15:25.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_opt_variant.h
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)    10187 2023-11-14 17:07:57.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_opt_vec.cpp
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     3481 2023-11-14 13:04:18.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_opt_vec.h
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     9833 2023-10-25 11:07:55.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_principal.cpp
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     2133 2023-10-25 11:07:55.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_principal.h
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)    37370 2023-11-25 12:42:37.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_record.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1415 2023-10-28 11:36:08.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_record.h
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1116 2023-10-25 11:07:55.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_reserved.cpp
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)      828 2023-10-25 11:07:55.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_reserved.h
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     5518 2023-11-20 11:48:23.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_table.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1335 2023-11-08 11:32:54.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_table.h
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     2841 2023-10-25 11:07:55.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_text.cpp
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1067 2023-10-25 11:07:55.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_text.h
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)    34578 2023-11-25 12:42:34.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_variant.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1874 2023-11-08 12:19:11.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_variant.h
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     4672 2023-10-26 19:01:54.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_vec_bool.cpp
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1052 2023-10-25 11:07:55.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_vec_bool.h
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     4668 2023-10-26 19:01:54.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_vec_float32.cpp
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1081 2023-10-25 11:07:55.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_vec_float32.h
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     4675 2023-10-26 19:01:54.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_vec_float64.cpp
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1089 2023-10-25 11:07:55.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_vec_float64.h
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     4568 2023-10-26 19:01:54.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_vec_int.cpp
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1092 2023-10-25 11:07:55.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_vec_int.h
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     4665 2023-10-26 19:01:54.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_vec_int16.cpp
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1083 2023-10-25 11:07:55.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_vec_int16.h
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     4665 2023-10-26 19:01:54.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_vec_int32.cpp
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1083 2023-10-25 11:07:55.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_vec_int32.h
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     4665 2023-10-26 19:01:54.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_vec_int64.cpp
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1083 2023-10-25 11:07:55.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_vec_int64.h
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     4632 2023-10-26 19:01:54.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_vec_int8.cpp
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1068 2023-10-25 11:07:55.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_vec_int8.h
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     4615 2023-10-26 19:01:54.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_vec_nat.cpp
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1101 2023-10-25 11:07:55.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_vec_nat.h
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     4680 2023-10-26 19:01:54.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_vec_nat16.cpp
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1091 2023-10-25 11:07:55.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_vec_nat16.h
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     4680 2023-10-26 19:01:54.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_vec_nat32.cpp
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1091 2023-10-25 11:07:55.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_vec_nat32.h
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     4680 2023-10-26 19:01:54.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_vec_nat64.cpp
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1091 2023-10-25 11:07:55.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_vec_nat64.h
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     4646 2023-10-26 19:01:54.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_vec_nat8.cpp
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1076 2023-10-25 11:07:55.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_vec_nat8.h
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     4903 2023-10-26 19:01:54.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_vec_principal.cpp
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1143 2023-10-25 11:07:55.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_vec_principal.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)    10852 2023-11-25 14:11:11.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_vec_record.cpp
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1635 2023-11-18 12:27:30.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_vec_record.h
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     4911 2023-10-26 19:01:54.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_vec_text.cpp
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1109 2023-10-25 11:07:55.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_vec_text.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     4504 2023-11-13 11:23:16.000000 icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_visitors.h
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)    21837 2023-10-31 10:06:33.000000 icpp-candid-3.8.1/src/icpp_candid/candid/vec_bytes.cpp
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     5406 2023-10-31 10:06:33.000000 icpp-candid-3.8.1/src/icpp_candid/candid/vec_bytes.h
-drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-11-27 16:06:58.388269 icpp-candid-3.8.1/src/icpp_candid/hooks/
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     3477 2023-10-18 15:36:18.000000 icpp-candid-3.8.1/src/icpp_candid/hooks/icpp_hooks.cpp
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1192 2023-10-18 15:30:28.000000 icpp-candid-3.8.1/src/icpp_candid/hooks/icpp_hooks.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)       98 2023-10-03 19:33:28.000000 icpp-candid-3.8.1/src/icpp_candid/py.typed
-drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-11-27 16:06:58.364269 icpp-candid-3.8.1/src/icpp_candid/vendors/
-drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-11-27 16:06:58.392269 icpp-candid-3.8.1/src/icpp_candid/vendors/cppcodec/
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1155 2023-10-03 19:33:28.000000 icpp-candid-3.8.1/src/icpp_candid/vendors/cppcodec/LICENSE
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     3933 2023-10-03 19:33:28.000000 icpp-candid-3.8.1/src/icpp_candid/vendors/cppcodec/base32_crockford.hpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1366 2023-10-03 19:33:28.000000 icpp-candid-3.8.1/src/icpp_candid/vendors/cppcodec/base32_default_crockford.hpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1342 2023-10-03 19:33:28.000000 icpp-candid-3.8.1/src/icpp_candid/vendors/cppcodec/base32_default_hex.hpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1356 2023-10-03 19:33:28.000000 icpp-candid-3.8.1/src/icpp_candid/vendors/cppcodec/base32_default_rfc4648.hpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     3090 2023-10-03 19:33:28.000000 icpp-candid-3.8.1/src/icpp_candid/vendors/cppcodec/base32_hex.hpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     3143 2023-10-03 19:33:28.000000 icpp-candid-3.8.1/src/icpp_candid/vendors/cppcodec/base32_rfc4648.hpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1356 2023-10-03 19:33:28.000000 icpp-candid-3.8.1/src/icpp_candid/vendors/cppcodec/base64_default_rfc4648.hpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1336 2023-10-03 19:33:28.000000 icpp-candid-3.8.1/src/icpp_candid/vendors/cppcodec/base64_default_url.hpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1381 2023-10-03 19:33:28.000000 icpp-candid-3.8.1/src/icpp_candid/vendors/cppcodec/base64_default_url_unpadded.hpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     3070 2023-10-03 19:33:28.000000 icpp-candid-3.8.1/src/icpp_candid/vendors/cppcodec/base64_rfc4648.hpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     3201 2023-10-03 19:33:28.000000 icpp-candid-3.8.1/src/icpp_candid/vendors/cppcodec/base64_url.hpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1805 2023-10-03 19:33:28.000000 icpp-candid-3.8.1/src/icpp_candid/vendors/cppcodec/base64_url_unpadded.hpp
-drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-11-27 16:06:58.392269 icpp-candid-3.8.1/src/icpp_candid/vendors/cppcodec/data/
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)    12087 2023-10-03 19:33:28.000000 icpp-candid-3.8.1/src/icpp_candid/vendors/cppcodec/data/access.hpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2352 2023-10-03 19:33:28.000000 icpp-candid-3.8.1/src/icpp_candid/vendors/cppcodec/data/raw_result_buffer.hpp
-drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-11-27 16:06:58.396269 icpp-candid-3.8.1/src/icpp_candid/vendors/cppcodec/detail/
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     7994 2023-10-03 19:33:28.000000 icpp-candid-3.8.1/src/icpp_candid/vendors/cppcodec/detail/base32.hpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     5692 2023-10-03 19:33:28.000000 icpp-candid-3.8.1/src/icpp_candid/vendors/cppcodec/detail/base64.hpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)    11905 2023-10-03 19:33:28.000000 icpp-candid-3.8.1/src/icpp_candid/vendors/cppcodec/detail/codec.hpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1606 2023-10-03 19:33:28.000000 icpp-candid-3.8.1/src/icpp_candid/vendors/cppcodec/detail/config.hpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     4545 2023-10-03 19:33:28.000000 icpp-candid-3.8.1/src/icpp_candid/vendors/cppcodec/detail/hex.hpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)    19664 2023-10-03 19:33:28.000000 icpp-candid-3.8.1/src/icpp_candid/vendors/cppcodec/detail/stream_codec.hpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1328 2023-10-03 19:33:28.000000 icpp-candid-3.8.1/src/icpp_candid/vendors/cppcodec/hex_default_lower.hpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1328 2023-10-03 19:33:28.000000 icpp-candid-3.8.1/src/icpp_candid/vendors/cppcodec/hex_default_upper.hpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     3009 2023-10-03 19:33:28.000000 icpp-candid-3.8.1/src/icpp_candid/vendors/cppcodec/hex_lower.hpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2994 2023-10-03 19:33:28.000000 icpp-candid-3.8.1/src/icpp_candid/vendors/cppcodec/hex_upper.hpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     3283 2023-10-03 19:33:28.000000 icpp-candid-3.8.1/src/icpp_candid/vendors/cppcodec/parse_error.hpp
-drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-11-27 16:06:58.396269 icpp-candid-3.8.1/src/icpp_candid/vendors/hash-library/
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      861 2023-10-03 19:33:28.000000 icpp-candid-3.8.1/src/icpp_candid/vendors/hash-library/LICENSE
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)    31026 2023-10-03 19:33:28.000000 icpp-candid-3.8.1/src/icpp_candid/vendors/hash-library/crc32.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1736 2023-10-03 19:33:28.000000 icpp-candid-3.8.1/src/icpp_candid/vendors/hash-library/crc32.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1758 2023-10-03 19:33:28.000000 icpp-candid-3.8.1/src/icpp_candid/vendors/hash-library/readme.md
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)    15133 2023-10-03 19:33:28.000000 icpp-candid-3.8.1/src/icpp_candid/vendors/hash-library/sha256.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1968 2023-10-03 19:33:28.000000 icpp-candid-3.8.1/src/icpp_candid/vendors/hash-library/sha256.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      322 2023-11-27 11:29:17.000000 icpp-candid-3.8.1/src/icpp_candid/version.py
-drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-11-27 16:06:58.396269 icpp-candid-3.8.1/src/icpp_candid.egg-info/
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2287 2023-11-27 16:06:58.000000 icpp-candid-3.8.1/src/icpp_candid.egg-info/PKG-INFO
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     8182 2023-11-27 16:06:58.000000 icpp-candid-3.8.1/src/icpp_candid.egg-info/SOURCES.txt
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)        1 2023-11-27 16:06:58.000000 icpp-candid-3.8.1/src/icpp_candid.egg-info/dependency_links.txt
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)       45 2023-11-27 16:06:58.000000 icpp-candid-3.8.1/src/icpp_candid.egg-info/requires.txt
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)       12 2023-11-27 16:06:58.000000 icpp-candid-3.8.1/src/icpp_candid.egg-info/top_level.txt
+drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-12-08 19:57:19.484386 icpp-candid-3.9.0/
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1066 2023-10-03 19:33:28.000000 icpp-candid-3.9.0/LICENSE
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2287 2023-12-08 19:57:19.484386 icpp-candid-3.9.0/PKG-INFO
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1339 2023-10-18 15:36:18.000000 icpp-candid-3.9.0/README.md
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      469 2023-11-25 14:22:42.000000 icpp-candid-3.9.0/pyproject.toml
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)       38 2023-12-08 19:57:19.484386 icpp-candid-3.9.0/setup.cfg
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     9863 2023-10-03 19:33:28.000000 icpp-candid-3.9.0/setup.py
+drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-12-08 19:57:19.444386 icpp-candid-3.9.0/src/
+drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-12-08 19:57:19.448386 icpp-candid-3.9.0/src/icpp_candid/
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      652 2023-10-03 19:33:28.000000 icpp-candid-3.9.0/src/icpp_candid/__init__.py
+drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-12-08 19:57:19.476386 icpp-candid-3.9.0/src/icpp_candid/candid/
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)      852 2023-10-28 13:16:25.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_args.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      362 2023-10-18 15:35:50.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_args.h
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1684 2023-10-18 15:36:18.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_assert.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      613 2023-10-03 19:33:28.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_assert.h
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)       92 2023-10-23 17:52:03.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_constants.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      110 2023-12-08 19:46:33.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_debug_config.h
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)    33844 2023-11-25 12:41:09.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_deserialize.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1732 2023-10-26 11:12:21.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_deserialize.h
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)    11216 2023-11-18 12:29:10.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_opcode.cpp
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     3128 2023-11-15 20:50:24.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_opcode.h
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     3591 2023-11-20 11:37:46.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_serialize.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      753 2023-10-18 15:35:50.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_serialize.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     3880 2023-10-18 15:40:20.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_serialize_type_table_registry.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2714 2023-10-18 15:40:20.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_serialize_type_table_registry.h
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     3616 2023-11-12 14:31:22.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2452 2023-11-12 14:32:18.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_all_includes.h
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     6462 2023-11-18 12:02:10.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_base.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     5868 2023-11-20 11:30:37.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_base.h
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     2078 2023-10-25 11:07:54.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_bool.cpp
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)      958 2023-10-25 11:07:54.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_bool.h
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1186 2023-10-25 11:07:54.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_empty.cpp
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)      812 2023-10-25 11:07:54.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_empty.h
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     2280 2023-10-25 11:07:54.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_float32.cpp
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)      993 2023-10-25 11:07:54.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_float32.h
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     2287 2023-10-25 11:07:54.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_float64.cpp
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1001 2023-10-25 11:07:54.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_float64.h
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1995 2023-10-25 11:07:54.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_int.cpp
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)      998 2023-10-25 11:07:54.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_int.h
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     2046 2023-10-25 11:07:54.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_int16.cpp
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)      991 2023-10-25 11:07:54.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_int16.h
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     2046 2023-10-25 11:07:54.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_int32.cpp
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)      991 2023-10-25 11:07:54.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_int32.h
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     2046 2023-10-25 11:07:54.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_int64.cpp
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)      991 2023-10-25 11:07:54.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_int64.h
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     2019 2023-10-25 11:07:54.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_int8.cpp
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)      974 2023-10-25 11:07:54.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_int8.h
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     2016 2023-10-25 11:07:55.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_nat.cpp
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1005 2023-10-25 11:07:55.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_nat.h
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     2038 2023-10-25 11:07:54.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_nat16.cpp
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)      999 2023-10-25 11:07:54.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_nat16.h
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     2038 2023-10-25 11:07:54.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_nat32.cpp
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)      999 2023-10-25 11:07:54.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_nat32.h
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     2038 2023-10-25 11:07:55.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_nat64.cpp
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)      999 2023-10-25 11:07:55.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_nat64.h
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     2011 2023-10-25 11:07:55.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_nat8.cpp
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)      982 2023-10-25 11:07:55.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_nat8.h
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)      816 2023-10-18 15:30:28.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_null.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      835 2023-10-21 12:29:07.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_null.h
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     4570 2023-10-26 19:01:54.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_opt_bool.cpp
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1101 2023-10-25 11:07:55.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_opt_bool.h
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     4616 2023-10-26 19:01:54.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_opt_float32.cpp
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1130 2023-10-25 11:07:55.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_opt_float32.h
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     4622 2023-10-26 19:01:54.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_opt_float64.cpp
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1138 2023-10-25 11:07:55.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_opt_float64.h
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     4535 2023-10-26 19:01:54.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_opt_int.cpp
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1142 2023-10-25 11:07:55.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_opt_int.h
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     4572 2023-10-26 19:01:54.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_opt_int16.cpp
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1132 2023-10-25 11:07:55.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_opt_int16.h
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     4573 2023-10-26 19:01:54.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_opt_int32.cpp
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1134 2023-10-25 11:07:55.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_opt_int32.h
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     4573 2023-10-26 19:01:54.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_opt_int64.cpp
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1132 2023-10-25 11:07:55.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_opt_int64.h
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     4542 2023-10-26 19:01:54.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_opt_int8.cpp
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1117 2023-10-25 11:07:55.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_opt_int8.h
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     4541 2023-10-26 19:01:54.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_opt_nat.cpp
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1150 2023-10-25 11:07:55.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_opt_nat.h
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     4579 2023-10-26 19:01:54.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_opt_nat16.cpp
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1140 2023-10-25 11:07:55.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_opt_nat16.h
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     4579 2023-10-26 19:01:54.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_opt_nat32.cpp
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1140 2023-10-25 11:07:55.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_opt_nat32.h
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     4579 2023-10-26 19:01:54.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_opt_nat64.cpp
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1140 2023-10-25 11:07:55.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_opt_nat64.h
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     4548 2023-10-26 19:01:54.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_opt_nat8.cpp
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1125 2023-10-25 11:07:55.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_opt_nat8.h
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     3875 2023-10-26 19:01:54.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_opt_null.cpp
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1074 2023-10-25 11:07:55.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_opt_null.h
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     4902 2023-10-26 19:01:54.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_opt_principal.cpp
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1194 2023-10-25 11:07:55.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_opt_principal.h
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     7167 2023-11-18 11:41:26.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_opt_record.cpp
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1782 2023-11-14 13:15:21.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_opt_record.h
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     4846 2023-10-26 19:01:54.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_opt_text.cpp
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1157 2023-10-25 11:07:55.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_opt_text.h
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     7252 2023-11-14 17:07:33.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_opt_variant.cpp
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1796 2023-11-14 13:15:25.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_opt_variant.h
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)    10187 2023-11-14 17:07:57.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_opt_vec.cpp
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     3481 2023-11-14 13:04:18.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_opt_vec.h
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     9833 2023-10-25 11:07:55.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_principal.cpp
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     2133 2023-10-25 11:07:55.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_principal.h
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)    39104 2023-12-08 19:53:17.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_record.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1415 2023-10-28 11:36:08.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_record.h
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1116 2023-10-25 11:07:55.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_reserved.cpp
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)      828 2023-10-25 11:07:55.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_reserved.h
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     5518 2023-11-20 11:48:23.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_table.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1335 2023-11-08 11:32:54.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_table.h
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     2841 2023-10-25 11:07:55.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_text.cpp
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1067 2023-10-25 11:07:55.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_text.h
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)    36149 2023-12-08 19:53:17.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_variant.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1874 2023-11-08 12:19:11.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_variant.h
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     4672 2023-10-26 19:01:54.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_vec_bool.cpp
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1052 2023-10-25 11:07:55.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_vec_bool.h
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     4668 2023-10-26 19:01:54.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_vec_float32.cpp
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1081 2023-10-25 11:07:55.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_vec_float32.h
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     4675 2023-10-26 19:01:54.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_vec_float64.cpp
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1089 2023-10-25 11:07:55.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_vec_float64.h
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     4568 2023-10-26 19:01:54.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_vec_int.cpp
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1092 2023-10-25 11:07:55.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_vec_int.h
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     4665 2023-10-26 19:01:54.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_vec_int16.cpp
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1083 2023-10-25 11:07:55.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_vec_int16.h
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     4665 2023-10-26 19:01:54.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_vec_int32.cpp
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1083 2023-10-25 11:07:55.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_vec_int32.h
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     4665 2023-10-26 19:01:54.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_vec_int64.cpp
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1083 2023-10-25 11:07:55.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_vec_int64.h
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     4632 2023-10-26 19:01:54.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_vec_int8.cpp
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1068 2023-10-25 11:07:55.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_vec_int8.h
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     4615 2023-10-26 19:01:54.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_vec_nat.cpp
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1101 2023-10-25 11:07:55.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_vec_nat.h
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     4680 2023-10-26 19:01:54.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_vec_nat16.cpp
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1091 2023-10-25 11:07:55.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_vec_nat16.h
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     4680 2023-10-26 19:01:54.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_vec_nat32.cpp
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1091 2023-10-25 11:07:55.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_vec_nat32.h
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     4680 2023-10-26 19:01:54.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_vec_nat64.cpp
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1091 2023-10-25 11:07:55.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_vec_nat64.h
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     4646 2023-10-26 19:01:54.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_vec_nat8.cpp
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1076 2023-10-25 11:07:55.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_vec_nat8.h
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     4903 2023-10-26 19:01:54.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_vec_principal.cpp
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1143 2023-10-25 11:07:55.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_vec_principal.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)    10852 2023-11-25 14:11:11.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_vec_record.cpp
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1635 2023-11-18 12:27:30.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_vec_record.h
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     4911 2023-10-26 19:01:54.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_vec_text.cpp
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1109 2023-10-25 11:07:55.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_vec_text.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     4504 2023-11-13 11:23:16.000000 icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_visitors.h
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)    21837 2023-10-31 10:06:33.000000 icpp-candid-3.9.0/src/icpp_candid/candid/vec_bytes.cpp
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     5406 2023-10-31 10:06:33.000000 icpp-candid-3.9.0/src/icpp_candid/candid/vec_bytes.h
+drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-12-08 19:57:19.476386 icpp-candid-3.9.0/src/icpp_candid/hooks/
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     3477 2023-10-18 15:36:18.000000 icpp-candid-3.9.0/src/icpp_candid/hooks/icpp_hooks.cpp
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     1192 2023-10-18 15:30:28.000000 icpp-candid-3.9.0/src/icpp_candid/hooks/icpp_hooks.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)       98 2023-10-03 19:33:28.000000 icpp-candid-3.9.0/src/icpp_candid/py.typed
+drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-12-08 19:57:19.448386 icpp-candid-3.9.0/src/icpp_candid/vendors/
+drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-12-08 19:57:19.480386 icpp-candid-3.9.0/src/icpp_candid/vendors/cppcodec/
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1155 2023-10-03 19:33:28.000000 icpp-candid-3.9.0/src/icpp_candid/vendors/cppcodec/LICENSE
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     3933 2023-10-03 19:33:28.000000 icpp-candid-3.9.0/src/icpp_candid/vendors/cppcodec/base32_crockford.hpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1366 2023-10-03 19:33:28.000000 icpp-candid-3.9.0/src/icpp_candid/vendors/cppcodec/base32_default_crockford.hpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1342 2023-10-03 19:33:28.000000 icpp-candid-3.9.0/src/icpp_candid/vendors/cppcodec/base32_default_hex.hpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1356 2023-10-03 19:33:28.000000 icpp-candid-3.9.0/src/icpp_candid/vendors/cppcodec/base32_default_rfc4648.hpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     3090 2023-10-03 19:33:28.000000 icpp-candid-3.9.0/src/icpp_candid/vendors/cppcodec/base32_hex.hpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     3143 2023-10-03 19:33:28.000000 icpp-candid-3.9.0/src/icpp_candid/vendors/cppcodec/base32_rfc4648.hpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1356 2023-10-03 19:33:28.000000 icpp-candid-3.9.0/src/icpp_candid/vendors/cppcodec/base64_default_rfc4648.hpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1336 2023-10-03 19:33:28.000000 icpp-candid-3.9.0/src/icpp_candid/vendors/cppcodec/base64_default_url.hpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1381 2023-10-03 19:33:28.000000 icpp-candid-3.9.0/src/icpp_candid/vendors/cppcodec/base64_default_url_unpadded.hpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     3070 2023-10-03 19:33:28.000000 icpp-candid-3.9.0/src/icpp_candid/vendors/cppcodec/base64_rfc4648.hpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     3201 2023-10-03 19:33:28.000000 icpp-candid-3.9.0/src/icpp_candid/vendors/cppcodec/base64_url.hpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1805 2023-10-03 19:33:28.000000 icpp-candid-3.9.0/src/icpp_candid/vendors/cppcodec/base64_url_unpadded.hpp
+drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-12-08 19:57:19.480386 icpp-candid-3.9.0/src/icpp_candid/vendors/cppcodec/data/
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)    12087 2023-10-03 19:33:28.000000 icpp-candid-3.9.0/src/icpp_candid/vendors/cppcodec/data/access.hpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2352 2023-10-03 19:33:28.000000 icpp-candid-3.9.0/src/icpp_candid/vendors/cppcodec/data/raw_result_buffer.hpp
+drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-12-08 19:57:19.480386 icpp-candid-3.9.0/src/icpp_candid/vendors/cppcodec/detail/
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     7994 2023-10-03 19:33:28.000000 icpp-candid-3.9.0/src/icpp_candid/vendors/cppcodec/detail/base32.hpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     5692 2023-10-03 19:33:28.000000 icpp-candid-3.9.0/src/icpp_candid/vendors/cppcodec/detail/base64.hpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)    11905 2023-10-03 19:33:28.000000 icpp-candid-3.9.0/src/icpp_candid/vendors/cppcodec/detail/codec.hpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1606 2023-10-03 19:33:28.000000 icpp-candid-3.9.0/src/icpp_candid/vendors/cppcodec/detail/config.hpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     4545 2023-10-03 19:33:28.000000 icpp-candid-3.9.0/src/icpp_candid/vendors/cppcodec/detail/hex.hpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)    19664 2023-10-03 19:33:28.000000 icpp-candid-3.9.0/src/icpp_candid/vendors/cppcodec/detail/stream_codec.hpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1328 2023-10-03 19:33:28.000000 icpp-candid-3.9.0/src/icpp_candid/vendors/cppcodec/hex_default_lower.hpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1328 2023-10-03 19:33:28.000000 icpp-candid-3.9.0/src/icpp_candid/vendors/cppcodec/hex_default_upper.hpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     3009 2023-10-03 19:33:28.000000 icpp-candid-3.9.0/src/icpp_candid/vendors/cppcodec/hex_lower.hpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2994 2023-10-03 19:33:28.000000 icpp-candid-3.9.0/src/icpp_candid/vendors/cppcodec/hex_upper.hpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     3283 2023-10-03 19:33:28.000000 icpp-candid-3.9.0/src/icpp_candid/vendors/cppcodec/parse_error.hpp
+drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-12-08 19:57:19.484386 icpp-candid-3.9.0/src/icpp_candid/vendors/hash-library/
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      861 2023-10-03 19:33:28.000000 icpp-candid-3.9.0/src/icpp_candid/vendors/hash-library/LICENSE
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)    31026 2023-10-03 19:33:28.000000 icpp-candid-3.9.0/src/icpp_candid/vendors/hash-library/crc32.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1736 2023-10-03 19:33:28.000000 icpp-candid-3.9.0/src/icpp_candid/vendors/hash-library/crc32.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1758 2023-10-03 19:33:28.000000 icpp-candid-3.9.0/src/icpp_candid/vendors/hash-library/readme.md
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)    15133 2023-10-03 19:33:28.000000 icpp-candid-3.9.0/src/icpp_candid/vendors/hash-library/sha256.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1968 2023-10-03 19:33:28.000000 icpp-candid-3.9.0/src/icpp_candid/vendors/hash-library/sha256.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      322 2023-12-08 19:55:22.000000 icpp-candid-3.9.0/src/icpp_candid/version.py
+drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-12-08 19:57:19.484386 icpp-candid-3.9.0/src/icpp_candid.egg-info/
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2287 2023-12-08 19:57:19.000000 icpp-candid-3.9.0/src/icpp_candid.egg-info/PKG-INFO
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     8182 2023-12-08 19:57:19.000000 icpp-candid-3.9.0/src/icpp_candid.egg-info/SOURCES.txt
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)        1 2023-12-08 19:57:19.000000 icpp-candid-3.9.0/src/icpp_candid.egg-info/dependency_links.txt
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)       45 2023-12-08 19:57:19.000000 icpp-candid-3.9.0/src/icpp_candid.egg-info/requires.txt
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)       12 2023-12-08 19:57:19.000000 icpp-candid-3.9.0/src/icpp_candid.egg-info/top_level.txt
```

### Comparing `icpp-candid-3.8.1/LICENSE` & `icpp-candid-3.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/PKG-INFO` & `icpp-candid-3.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icpp-candid
-Version: 3.8.1
+Version: 3.9.0
 Summary: C++ Candid Library
 Home-page: https://docs.icpp.world/
 Author: icppWorld
 Author-email: icpp@icpp.world
 License: MIT
 Keywords: C++ Candid Library,Internet Computer,C++,Candid,blockchain
 Classifier: Development Status :: 4 - Beta
```

### Comparing `icpp-candid-3.8.1/README.md` & `icpp-candid-3.9.0/README.md`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/setup.py` & `icpp-candid-3.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/__init__.py` & `icpp-candid-3.9.0/src/icpp_candid/__init__.py`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_args.cpp` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_args.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_assert.cpp` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_assert.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_assert.h` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_assert.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_deserialize.cpp` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_deserialize.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_deserialize.h` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_deserialize.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_opcode.cpp` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_opcode.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_opcode.h` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_opcode.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_serialize.cpp` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_serialize.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_serialize.h` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_serialize.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_serialize_type_table_registry.cpp` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_serialize_type_table_registry.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_serialize_type_table_registry.h` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_serialize_type_table_registry.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type.h` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_all_includes.h` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_all_includes.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_base.cpp` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_base.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_base.h` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_base.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_bool.cpp` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_bool.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_bool.h` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_bool.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_empty.cpp` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_empty.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_empty.h` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_empty.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_float32.cpp` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_float32.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_float32.h` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_float32.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_float64.cpp` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_float64.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_float64.h` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_float64.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_int.cpp` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_int.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_int.h` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_int.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_int16.cpp` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_int16.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_int16.h` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_int16.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_int32.cpp` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_int32.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_int32.h` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_int32.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_int64.cpp` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_int64.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_int64.h` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_int64.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_int8.cpp` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_int8.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_int8.h` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_int8.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_nat.cpp` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_nat.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_nat.h` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_nat.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_nat16.cpp` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_nat16.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_nat16.h` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_nat16.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_nat32.cpp` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_nat32.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_nat32.h` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_nat32.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_nat64.cpp` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_nat64.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_nat64.h` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_nat64.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_nat8.cpp` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_nat8.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_nat8.h` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_nat8.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_null.cpp` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_null.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_null.h` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_null.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_opt_bool.cpp` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_opt_bool.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_opt_bool.h` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_opt_bool.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_opt_float32.cpp` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_opt_float32.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_opt_float32.h` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_opt_float32.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_opt_float64.cpp` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_opt_float64.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_opt_float64.h` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_opt_float64.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_opt_int.cpp` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_opt_int.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_opt_int.h` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_opt_int.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_opt_int16.cpp` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_opt_int16.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_opt_int16.h` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_opt_int16.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_opt_int32.cpp` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_opt_int32.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_opt_int32.h` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_opt_int32.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_opt_int64.cpp` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_opt_int64.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_opt_int64.h` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_opt_int64.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_opt_int8.cpp` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_opt_int8.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_opt_int8.h` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_opt_int8.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_opt_nat.cpp` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_opt_nat.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_opt_nat.h` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_opt_nat.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_opt_nat16.cpp` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_opt_nat16.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_opt_nat16.h` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_opt_nat16.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_opt_nat32.cpp` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_opt_nat32.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_opt_nat32.h` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_opt_nat32.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_opt_nat64.cpp` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_opt_nat64.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_opt_nat64.h` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_opt_nat64.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_opt_nat8.cpp` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_opt_nat8.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_opt_nat8.h` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_opt_nat8.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_opt_null.cpp` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_opt_null.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_opt_null.h` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_opt_null.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_opt_principal.cpp` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_opt_principal.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_opt_principal.h` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_opt_principal.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_opt_record.cpp` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_opt_record.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_opt_record.h` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_opt_record.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_opt_text.cpp` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_opt_text.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_opt_text.h` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_opt_text.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_opt_variant.cpp` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_opt_variant.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_opt_variant.h` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_opt_variant.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_opt_vec.cpp` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_opt_vec.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_opt_vec.h` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_opt_vec.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_principal.cpp` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_principal.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_principal.h` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_principal.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_record.cpp` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_record.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -603,18 +603,19 @@
                  std::to_string(field_content_opcode_wire) + " (" +
                  field_content_name_wire + ")");
     }
     ICPP_HOOKS::debug_print(msg);
   }
 
   decoder = nullptr;
-  bool field_error{false};
+  bool error{false};
+  std::string error_msg;
   if (field_id_wire == field_id_expected) {
     // field Ids (the hash) of expected & wire match
-    // ==> Follow exact same logic as for args in candid_type_deserialize
+    // ==> Follow exact same logic as for args in candid_deserialize
     if (((field_opcode_wire != candidOpcode.Opt &&
           field_opcode_wire == field_opcode_expected) ||
          (field_opcode_wire == candidOpcode.Opt &&
           field_opcode_expected == candidOpcode.Opt &&
           field_content_opcode_wire == field_content_opcode_expected) ||
          (field_opcode_wire == candidOpcode.Vec &&
           field_opcode_expected == candidOpcode.Vec &&
@@ -632,14 +633,15 @@
         // record { record } or record {variant}
         int field_datatype_wire = m_field_datatypes_wire[j];
         auto p_wire =
             de.get_typetables_wire()[field_datatype_wire].get_p_wire();
         decoder->set_fields_wire(p_wire);
       } else if (field_opcode_expected == candidOpcode.Opt &&
                  field_content_opcode_wire == candidOpcode.Vec) {
+        // TODO: add same logic here/Record/Variant for OptVecVariant
         // record { opt {vec} }
         CandidType c_decoder = decoder->toCandidType();
         CandidTypeOptVec *p_opt_vec = std::get_if<CandidTypeOptVec>(&c_decoder);
         if (p_opt_vec) {
           int field_content_datatype_wire = m_field_content_datatypes_wire[j];
           auto p_content_wire =
               de.get_typetables_wire()[field_content_datatype_wire]
@@ -654,66 +656,109 @@
 
               CandidType c_content = p_opt_vec->get_pv()->toCandidType();
               CandidTypeVecRecord *p_vec_record =
                   std::get_if<CandidTypeVecRecord>(&c_content);
               p_vec_record->get_pvs()->set_fields_wire(p_record_wire);
             }
           } else {
+            error = true;
+            error_msg =
+                "p_content_wire is a nullptr, likely a bug. for Record field CandidTypeOptVecRecord";
             ICPP_HOOKS::trap(
                 "ERROR: p_content_wire is a nullptr, likely a bug. for Record field CandidTypeOptVecRecord - " +
                 std::string(__func__));
           }
         }
-      } else if (field_opcode_expected == candidOpcode.Opt &&
-                 field_content_opcode_wire == candidOpcode.Record) {
-        int field_content_datatype_wire = m_field_content_datatypes_wire[j];
-        auto p_content_wire =
-            de.get_typetables_wire()[field_content_datatype_wire].get_p_wire();
-        CandidType c_content_wire = p_content_wire->toCandidType();
-        CandidTypeRecord *p_content_record =
-            std::get_if<CandidTypeRecord>(&c_content_wire);
-
-        CandidType c_decoder = decoder->toCandidType();
-        CandidTypeOptRecord *p_opt_record =
-            std::get_if<CandidTypeOptRecord>(&c_decoder);
-        if (p_opt_record && p_content_record) {
-          p_opt_record->get_pv()->set_fields_wire(p_content_wire);
+      } else if (field_content_opcode_wire == candidOpcode.Record) {
+        if (field_opcode_expected == candidOpcode.Opt ||
+            field_opcode_expected == candidOpcode.Vec) {
+          // OptRecord, VecRecord
+          int field_content_datatype_wire = m_field_content_datatypes_wire[j];
+          auto p_content_wire =
+              de.get_typetables_wire()[field_content_datatype_wire]
+                  .get_p_wire();
+          if (p_content_wire) {
+            CandidType c_decoder = decoder->toCandidType();
+            if (field_opcode_expected == candidOpcode.Opt) {
+              CandidTypeOptRecord *p_opt_record =
+                  std::get_if<CandidTypeOptRecord>(&c_decoder);
+              if (p_opt_record) {
+                p_opt_record->get_pv()->set_fields_wire(p_content_wire);
+              } else {
+                error = true;
+                error_msg = "p_opt_record is a nullptr, likely a bug.";
+              }
+            } else if (field_opcode_expected == candidOpcode.Vec) {
+              // A VecRecord uses a dummy record during decoding
+              CandidTypeVecRecord *p_vec_record =
+                  std::get_if<CandidTypeVecRecord>(&c_decoder);
+              if (p_vec_record) {
+                p_vec_record->get_pr()->set_fields_wire(p_content_wire);
+                // not used
+                p_vec_record->get_pv()->set_fields_wire(p_content_wire);
+              } else {
+                error = true;
+                error_msg = "p_vec_record is a nullptr, likely a bug.";
+              }
+            } else {
+              error = true;
+              error_msg = "ERROR: ... ";
+            }
+          } else {
+            error = true;
+            error_msg = "p_content_wire is a nullptr, likely a bug.";
+          }
         } else {
-          ICPP_HOOKS::trap(
-              "ERROR: Unexpected type-table for Record field CandidTypeOptRecord - " +
-              std::string(__func__));
+          error = true;
+          error_msg = "We do NOT yet handle this.";
         }
-      } else if (field_opcode_expected == candidOpcode.Opt &&
-                 field_content_opcode_wire == candidOpcode.Variant) {
-        int field_content_datatype_wire = m_field_content_datatypes_wire[j];
-        auto p_content_wire =
-            de.get_typetables_wire()[field_content_datatype_wire].get_p_wire();
-        CandidType c_content_wire = p_content_wire->toCandidType();
-        CandidTypeVariant *p_content_variant =
-            std::get_if<CandidTypeVariant>(&c_content_wire);
-
-        CandidType c_decoder = decoder->toCandidType();
-        CandidTypeOptVariant *p_opt_variant =
-            std::get_if<CandidTypeOptVariant>(&c_decoder);
-        if (p_opt_variant && p_content_variant) {
-          p_opt_variant->get_pv()->set_fields_wire(p_content_wire);
+      } else if (field_content_opcode_wire == candidOpcode.Variant) {
+        if (field_opcode_expected == candidOpcode.Opt ||
+            field_opcode_expected == candidOpcode.Vec) {
+          // OptVariant, VecVariant
+          int field_content_datatype_wire = m_field_content_datatypes_wire[j];
+          auto p_content_wire =
+              de.get_typetables_wire()[field_content_datatype_wire]
+                  .get_p_wire();
+          if (p_content_wire) {
+            CandidType c_decoder = decoder->toCandidType();
+            if (field_opcode_expected == candidOpcode.Opt) {
+              CandidTypeOptVariant *p_opt_variant =
+                  std::get_if<CandidTypeOptVariant>(&c_decoder);
+              if (p_opt_variant) {
+                p_opt_variant->get_pv()->set_fields_wire(p_content_wire);
+              } else {
+                error = true;
+                error_msg = "p_opt_variant is a nullptr, likely a bug.";
+              }
+            } else if (field_opcode_expected == candidOpcode.Vec) {
+              ICPP_HOOKS::trap("TODO: Implement for CandidTypeVecVariant.");
+              // // A VecVariant uses a dummy record during decoding
+              // CandidTypeVecVariant *p_vec_variant =
+              //     std::get_if<CandidTypeVecVariant>(&c_decoder);
+              // if (p_vec_variant) {
+              //   p_vec_variant->get_pr()->set_fields_wire(p_content_wire);
+              //   // not used
+              //   p_vec_variant->get_pv()->set_fields_wire(p_content_wire);
+              // } else {
+              //   error = true;
+              //   error_msg = "p_vec_variant is a nullptr, likely a bug.";
+              // }
+            } else {
+              error = true;
+              error_msg = "ERROR: ... ";
+            }
+          } else {
+            error = true;
+            error_msg = "p_content_wire is a nullptr, likely a bug.";
+          }
         } else {
-          ICPP_HOOKS::trap(
-              "ERROR: Unexpected type-table for Record field CandidTypeOptVariant - " +
-              std::string(__func__));
+          error = true;
+          error_msg = "We do NOT yet handle this.";
         }
-      } else if ((field_content_opcode_wire == candidOpcode.Record) ||
-                 (field_content_opcode_wire == candidOpcode.Variant)) {
-        ICPP_HOOKS::trap(
-            "ERROR: We do NOT yet handle this field type: \n " +
-            std::to_string(field_opcode_wire) + " (" +
-            candidOpcode.name_from_opcode(field_opcode_wire) +
-            std::to_string(field_content_opcode_wire) + " (" +
-            candidOpcode.name_from_opcode(field_content_opcode_wire) + " - " +
-            std::string(__func__));
       }
     } else if (field_opcode_wire == candidOpcode.Null &&
                field_opcode_expected == candidOpcode.Opt) {
       // Special case, Expected opt found as '(null)'
       if (CANDID_DESERIALIZE_DEBUG_PRINT) {
         ICPP_HOOKS::debug_print(
             "--> This field is an expected Opt and found as 'null' on wire.\n    There is nothing to decode.");
@@ -745,15 +790,16 @@
             "--> This field is an expected Opt that we cannot find on the wire.\n    We will skip the expected arg.");
       }
       decoder = nullptr;
       decoder_name = "skip-expected-opt-not-found-on-wire";
     } else {
       // Wrong type on wire
       // TODO:  IMPLEMENT CHECK ON COVARIANCE/CONTRAVARIANCE
-      field_error = true;
+      error = true;
+      error_msg = "Wrong type on wire.";
     }
   } else {
     // field Ids (the hash) of expected & wire do not match
     // -> Only allowed if one or both are Opt fields
 
     // Is the field_id on the wire one of the next expected fields?
     // - yes: only allowed if expected is an Opt, which has been omitted
@@ -781,21 +827,22 @@
             "--> This field is an unexpected additional Opt found on wire.\n    We will decode M & discard the data.");
       }
       decoder = build_decoder_wire_for_additional_opt_field(de, j);
       decoder_name = "read-and-discard-additional-wire-opt";
     } else {
       // Wrong type on wire
       // TODO:  IMPLEMENT CHECK ON COVARIANCE/CONTRAVARIANCE
-      field_error = true;
+      error = true;
+      error_msg = "Wrong type on wire.";
     }
   }
 
-  if (field_error) {
+  if (error) {
     std::string msg;
-    msg.append("ERROR: Wrong Record field on wire:\n");
+    msg.append("ERROR: " + error_msg + "\n");
     msg.append("\nexpected field at index " + std::to_string(i));
     msg.append("\n- Opcode   = " + std::to_string(field_opcode_expected) +
                " (" + candidOpcode.name_from_opcode(field_opcode_expected) +
                ")");
     if (field_opcode_expected == candidOpcode.Opt) {
       msg.append("\n- field_content_opcode_expected = " +
                  std::to_string(field_content_opcode_expected) + " (" +
```

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_record.h` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_record.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_reserved.cpp` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_reserved.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_reserved.h` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_reserved.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_table.cpp` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_table.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_table.h` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_table.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_text.cpp` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_text.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_text.h` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_text.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_variant.cpp` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_variant.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -550,15 +550,16 @@
                  std::to_string(field_content_opcode_wire) + " (" +
                  field_content_name_wire + ")");
     }
     ICPP_HOOKS::debug_print(msg);
   }
 
   decoder = nullptr;
-  bool field_error{false};
+  bool error{false};
+  std::string error_msg;
   if (field_id_wire == field_id_expected) {
     // field Ids (the hash) of expected & wire match
     // ==> Follow exact same logic as for args in candid_type_deserialize
     if (((field_opcode_wire != candidOpcode.Opt &&
           field_opcode_wire == field_opcode_expected) ||
          (field_opcode_wire == candidOpcode.Opt &&
           field_opcode_expected == candidOpcode.Opt &&
@@ -606,61 +607,101 @@
             }
           } else {
             ICPP_HOOKS::trap(
                 "ERROR: p_content_wire is a nullptr, likely a bug. for Variant field CandidTypeOptVecRecord - " +
                 std::string(__func__));
           }
         }
-      } else if (field_opcode_expected == candidOpcode.Opt &&
-                 field_content_opcode_wire == candidOpcode.Record) {
-        int field_content_datatype_wire = m_field_content_datatypes_wire[j];
-        auto p_content_wire =
-            de.get_typetables_wire()[field_content_datatype_wire].get_p_wire();
-        CandidType c_content_wire = p_content_wire->toCandidType();
-        CandidTypeRecord *p_content_record =
-            std::get_if<CandidTypeRecord>(&c_content_wire);
-
-        CandidType c_decoder = decoder->toCandidType();
-        CandidTypeOptRecord *p_opt_record =
-            std::get_if<CandidTypeOptRecord>(&c_decoder);
-        if (p_opt_record && p_content_record) {
-          p_opt_record->get_pv()->set_fields_wire(p_content_wire);
+      } else if (field_content_opcode_wire == candidOpcode.Record) {
+        if (field_opcode_expected == candidOpcode.Opt ||
+            field_opcode_expected == candidOpcode.Vec) {
+          // OptRecord, VecRecord
+          int field_content_datatype_wire = m_field_content_datatypes_wire[j];
+          auto p_content_wire =
+              de.get_typetables_wire()[field_content_datatype_wire]
+                  .get_p_wire();
+          if (p_content_wire) {
+            CandidType c_decoder = decoder->toCandidType();
+            if (field_opcode_expected == candidOpcode.Opt) {
+              CandidTypeOptRecord *p_opt_record =
+                  std::get_if<CandidTypeOptRecord>(&c_decoder);
+              if (p_opt_record) {
+                p_opt_record->get_pv()->set_fields_wire(p_content_wire);
+              } else {
+                error = true;
+                error_msg = "p_opt_record is a nullptr, likely a bug.";
+              }
+            } else if (field_opcode_expected == candidOpcode.Vec) {
+              // A VecRecord uses a dummy record during decoding
+              CandidTypeVecRecord *p_vec_record =
+                  std::get_if<CandidTypeVecRecord>(&c_decoder);
+              if (p_vec_record) {
+                p_vec_record->get_pr()->set_fields_wire(p_content_wire);
+                // not used
+                p_vec_record->get_pv()->set_fields_wire(p_content_wire);
+              } else {
+                error = true;
+                error_msg = "p_vec_record is a nullptr, likely a bug.";
+              }
+            } else {
+              error = true;
+              error_msg = "ERROR: ... ";
+            }
+          } else {
+            error = true;
+            error_msg = "p_content_wire is a nullptr, likely a bug.";
+          }
         } else {
-          ICPP_HOOKS::trap(
-              "ERROR: Unexpected type-table for Variant field CandidTypeOptRecord - " +
-              std::string(__func__));
+          error = true;
+          error_msg = "We do NOT yet handle this.";
         }
-      } else if (field_opcode_expected == candidOpcode.Opt &&
-                 field_content_opcode_wire == candidOpcode.Variant) {
-        int field_content_datatype_wire = m_field_content_datatypes_wire[j];
-        auto p_content_wire =
-            de.get_typetables_wire()[field_content_datatype_wire].get_p_wire();
-        CandidType c_content_wire = p_content_wire->toCandidType();
-        CandidTypeVariant *p_content_variant =
-            std::get_if<CandidTypeVariant>(&c_content_wire);
-
-        CandidType c_decoder = decoder->toCandidType();
-        CandidTypeOptVariant *p_opt_variant =
-            std::get_if<CandidTypeOptVariant>(&c_decoder);
-        if (p_opt_variant && p_content_variant) {
-          p_opt_variant->get_pv()->set_fields_wire(p_content_wire);
+      } else if (field_content_opcode_wire == candidOpcode.Variant) {
+        if (field_opcode_expected == candidOpcode.Opt ||
+            field_opcode_expected == candidOpcode.Vec) {
+          // OptVariant, VecVariant
+          int field_content_datatype_wire = m_field_content_datatypes_wire[j];
+          auto p_content_wire =
+              de.get_typetables_wire()[field_content_datatype_wire]
+                  .get_p_wire();
+          if (p_content_wire) {
+            CandidType c_decoder = decoder->toCandidType();
+            if (field_opcode_expected == candidOpcode.Opt) {
+              CandidTypeOptVariant *p_opt_variant =
+                  std::get_if<CandidTypeOptVariant>(&c_decoder);
+              if (p_opt_variant) {
+                p_opt_variant->get_pv()->set_fields_wire(p_content_wire);
+              } else {
+                error = true;
+                error_msg = "p_opt_variant is a nullptr, likely a bug.";
+              }
+            } else if (field_opcode_expected == candidOpcode.Vec) {
+              ICPP_HOOKS::trap("TODO: Implement for CandidTypeVecVariant.");
+              // // A VecVariant uses a dummy record during decoding
+              // CandidTypeVecVariant *p_vec_variant =
+              //     std::get_if<CandidTypeVecVariant>(&c_decoder);
+              // if (p_vec_variant) {
+              //   p_vec_variant->get_pr()->set_fields_wire(p_content_wire);
+              //   // not used
+              //   p_vec_variant->get_pv()->set_fields_wire(p_content_wire);
+              // } else {
+              //   error = true;
+              //   error_msg = "p_vec_variant is a nullptr, likely a bug.";
+              // }
+            } else {
+              error = true;
+              error_msg = "ERROR: ... ";
+            }
+          } else {
+            error = true;
+            error_msg = "p_content_wire is a nullptr, likely a bug.";
+          }
         } else {
-          ICPP_HOOKS::trap(
-              "ERROR: Unexpected type-table for Variant field CandidTypeOptVariant - " +
-              std::string(__func__));
+          error = true;
+          error_msg = "We do NOT yet handle this.";
         }
-      } else if ((field_content_opcode_wire == candidOpcode.Record) ||
-                 (field_content_opcode_wire == candidOpcode.Variant)) {
-        ICPP_HOOKS::trap(
-            "ERROR: We do NOT yet handle this field type: \n " +
-            std::to_string(field_opcode_wire) + " (" +
-            candidOpcode.name_from_opcode(field_opcode_wire) +
-            std::to_string(field_content_opcode_wire) + " (" +
-            candidOpcode.name_from_opcode(field_content_opcode_wire) + " - " +
-            std::string(__func__));
       }
     } else if (field_opcode_wire == candidOpcode.Null &&
                field_opcode_expected == candidOpcode.Opt) {
       // Special case, Expected opt found as '(null)'
       if (CANDID_DESERIALIZE_DEBUG_PRINT) {
         ICPP_HOOKS::debug_print(
             "--> This field is an expected Opt and found as 'null' on wire.\n    There is nothing to decode.");
@@ -692,15 +733,16 @@
             "--> This field is an expected Opt that we cannot find on the wire.\n    We will skip the expected arg.");
       }
       decoder = nullptr;
       decoder_name = "skip-expected-opt-not-found-on-wire";
     } else {
       // Wrong type on wire
       // TODO:  IMPLEMENT CHECK ON COVARIANCE/CONTRAVARIANCE
-      field_error = true;
+      error = true;
+      error_msg = "Wrong type on wire.";
     }
   } else {
     // field Ids (the hash) of expected & wire do not match
     // -> Only allowed if one or both are Opt fields
 
     // Is the field_id on the wire one of the next expected fields?
     // - yes: only allowed if expected is an Opt, which has been omitted
@@ -728,20 +770,22 @@
             "--> This field is an unexpected additional Opt found on wire.\n    We will decode M & discard the data.");
       }
       decoder = build_decoder_wire_for_additional_opt_field(de, j);
       decoder_name = "read-and-discard-additional-wire-opt";
     } else {
       // Wrong type on wire
       // TODO:  IMPLEMENT CHECK ON COVARIANCE/CONTRAVARIANCE
-      field_error = true;
+      error = true;
+      error_msg = "Wrong type on wire.";
     }
   }
 
-  if (field_error) {
+  if (error) {
     std::string msg;
+    msg.append("ERROR: " + error_msg + "\n");
     msg.append("ERROR: Wrong Variant field on wire:\n");
     msg.append("\nexpected field has index " + std::to_string(i));
     msg.append("\n- Opcode   = " + std::to_string(field_opcode_expected) +
                " (" + candidOpcode.name_from_opcode(field_opcode_expected) +
                ")");
     if (field_opcode_expected == candidOpcode.Opt) {
       msg.append("\n- field_content_opcode_expected = " +
```

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_variant.h` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_variant.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_vec_bool.cpp` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_vec_bool.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_vec_bool.h` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_vec_bool.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_vec_float32.cpp` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_vec_float32.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_vec_float32.h` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_vec_float32.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_vec_float64.cpp` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_vec_float64.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_vec_float64.h` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_vec_float64.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_vec_int.cpp` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_vec_int.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_vec_int.h` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_vec_int.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_vec_int16.cpp` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_vec_int16.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_vec_int16.h` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_vec_int16.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_vec_int32.cpp` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_vec_int32.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_vec_int32.h` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_vec_int32.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_vec_int64.cpp` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_vec_int64.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_vec_int64.h` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_vec_int64.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_vec_int8.cpp` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_vec_int8.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_vec_int8.h` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_vec_int8.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_vec_nat.cpp` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_vec_nat.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_vec_nat.h` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_vec_nat.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_vec_nat16.cpp` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_vec_nat16.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_vec_nat16.h` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_vec_nat16.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_vec_nat32.cpp` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_vec_nat32.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_vec_nat32.h` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_vec_nat32.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_vec_nat64.cpp` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_vec_nat64.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_vec_nat64.h` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_vec_nat64.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_vec_nat8.cpp` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_vec_nat8.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_vec_nat8.h` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_vec_nat8.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_vec_principal.cpp` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_vec_principal.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_vec_principal.h` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_vec_principal.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_vec_record.cpp` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_vec_record.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_vec_record.h` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_vec_record.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_vec_text.cpp` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_vec_text.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_vec_text.h` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_vec_text.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/candid_type_visitors.h` & `icpp-candid-3.9.0/src/icpp_candid/candid/candid_type_visitors.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/vec_bytes.cpp` & `icpp-candid-3.9.0/src/icpp_candid/candid/vec_bytes.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/candid/vec_bytes.h` & `icpp-candid-3.9.0/src/icpp_candid/candid/vec_bytes.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/hooks/icpp_hooks.cpp` & `icpp-candid-3.9.0/src/icpp_candid/hooks/icpp_hooks.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/hooks/icpp_hooks.h` & `icpp-candid-3.9.0/src/icpp_candid/hooks/icpp_hooks.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/vendors/cppcodec/LICENSE` & `icpp-candid-3.9.0/src/icpp_candid/vendors/cppcodec/LICENSE`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/vendors/cppcodec/base32_crockford.hpp` & `icpp-candid-3.9.0/src/icpp_candid/vendors/cppcodec/base32_crockford.hpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/vendors/cppcodec/base32_default_crockford.hpp` & `icpp-candid-3.9.0/src/icpp_candid/vendors/cppcodec/base32_default_crockford.hpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/vendors/cppcodec/base32_default_hex.hpp` & `icpp-candid-3.9.0/src/icpp_candid/vendors/cppcodec/base32_default_hex.hpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/vendors/cppcodec/base32_default_rfc4648.hpp` & `icpp-candid-3.9.0/src/icpp_candid/vendors/cppcodec/base32_default_rfc4648.hpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/vendors/cppcodec/base32_hex.hpp` & `icpp-candid-3.9.0/src/icpp_candid/vendors/cppcodec/base32_hex.hpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/vendors/cppcodec/base32_rfc4648.hpp` & `icpp-candid-3.9.0/src/icpp_candid/vendors/cppcodec/base32_rfc4648.hpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/vendors/cppcodec/base64_default_rfc4648.hpp` & `icpp-candid-3.9.0/src/icpp_candid/vendors/cppcodec/base64_default_rfc4648.hpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/vendors/cppcodec/base64_default_url.hpp` & `icpp-candid-3.9.0/src/icpp_candid/vendors/cppcodec/base64_default_url.hpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/vendors/cppcodec/base64_default_url_unpadded.hpp` & `icpp-candid-3.9.0/src/icpp_candid/vendors/cppcodec/base64_default_url_unpadded.hpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/vendors/cppcodec/base64_rfc4648.hpp` & `icpp-candid-3.9.0/src/icpp_candid/vendors/cppcodec/base64_rfc4648.hpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/vendors/cppcodec/base64_url.hpp` & `icpp-candid-3.9.0/src/icpp_candid/vendors/cppcodec/base64_url.hpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/vendors/cppcodec/base64_url_unpadded.hpp` & `icpp-candid-3.9.0/src/icpp_candid/vendors/cppcodec/base64_url_unpadded.hpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/vendors/cppcodec/data/access.hpp` & `icpp-candid-3.9.0/src/icpp_candid/vendors/cppcodec/data/access.hpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/vendors/cppcodec/data/raw_result_buffer.hpp` & `icpp-candid-3.9.0/src/icpp_candid/vendors/cppcodec/data/raw_result_buffer.hpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/vendors/cppcodec/detail/base32.hpp` & `icpp-candid-3.9.0/src/icpp_candid/vendors/cppcodec/detail/base32.hpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/vendors/cppcodec/detail/base64.hpp` & `icpp-candid-3.9.0/src/icpp_candid/vendors/cppcodec/detail/base64.hpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/vendors/cppcodec/detail/codec.hpp` & `icpp-candid-3.9.0/src/icpp_candid/vendors/cppcodec/detail/codec.hpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/vendors/cppcodec/detail/config.hpp` & `icpp-candid-3.9.0/src/icpp_candid/vendors/cppcodec/detail/config.hpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/vendors/cppcodec/detail/hex.hpp` & `icpp-candid-3.9.0/src/icpp_candid/vendors/cppcodec/detail/hex.hpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/vendors/cppcodec/detail/stream_codec.hpp` & `icpp-candid-3.9.0/src/icpp_candid/vendors/cppcodec/detail/stream_codec.hpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/vendors/cppcodec/hex_default_lower.hpp` & `icpp-candid-3.9.0/src/icpp_candid/vendors/cppcodec/hex_default_lower.hpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/vendors/cppcodec/hex_default_upper.hpp` & `icpp-candid-3.9.0/src/icpp_candid/vendors/cppcodec/hex_default_upper.hpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/vendors/cppcodec/hex_lower.hpp` & `icpp-candid-3.9.0/src/icpp_candid/vendors/cppcodec/hex_lower.hpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/vendors/cppcodec/hex_upper.hpp` & `icpp-candid-3.9.0/src/icpp_candid/vendors/cppcodec/hex_upper.hpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/vendors/cppcodec/parse_error.hpp` & `icpp-candid-3.9.0/src/icpp_candid/vendors/cppcodec/parse_error.hpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/vendors/hash-library/LICENSE` & `icpp-candid-3.9.0/src/icpp_candid/vendors/hash-library/LICENSE`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/vendors/hash-library/crc32.cpp` & `icpp-candid-3.9.0/src/icpp_candid/vendors/hash-library/crc32.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/vendors/hash-library/crc32.h` & `icpp-candid-3.9.0/src/icpp_candid/vendors/hash-library/crc32.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/vendors/hash-library/readme.md` & `icpp-candid-3.9.0/src/icpp_candid/vendors/hash-library/readme.md`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/vendors/hash-library/sha256.cpp` & `icpp-candid-3.9.0/src/icpp_candid/vendors/hash-library/sha256.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid/vendors/hash-library/sha256.h` & `icpp-candid-3.9.0/src/icpp_candid/vendors/hash-library/sha256.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-3.8.1/src/icpp_candid.egg-info/PKG-INFO` & `icpp-candid-3.9.0/src/icpp_candid.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icpp-candid
-Version: 3.8.1
+Version: 3.9.0
 Summary: C++ Candid Library
 Home-page: https://docs.icpp.world/
 Author: icppWorld
 Author-email: icpp@icpp.world
 License: MIT
 Keywords: C++ Candid Library,Internet Computer,C++,Candid,blockchain
 Classifier: Development Status :: 4 - Beta
```

### Comparing `icpp-candid-3.8.1/src/icpp_candid.egg-info/SOURCES.txt` & `icpp-candid-3.9.0/src/icpp_candid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

