# Comparing `tmp/mns_common-1.1.2.7.tar.gz` & `tmp/mns_common-1.1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mns_common-1.1.2.7.tar", last modified: Fri May 24 09:44:12 2024, max compression
+gzip compressed data, was "mns_common-1.1.2.8.tar", last modified: Fri May 24 10:15:33 2024, max compression
```

## Comparing `mns_common-1.1.2.7.tar` & `mns_common-1.1.2.8.tar`

### file list

```diff
@@ -1,129 +1,127 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 09:44:12.995587 mns_common-1.1.2.7/
--rw-rw-rw-   0        0        0       59 2024-05-24 09:44:12.994590 mns_common-1.1.2.7/PKG-INFO
--rw-rw-rw-   0        0        0     1354 2023-12-14 15:25:31.000000 mns_common-1.1.2.7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-24 09:44:12.957688 mns_common-1.1.2.7/mns_common/
--rw-rw-rw-   0        0        0      163 2024-01-10 10:52:31.000000 mns_common-1.1.2.7/mns_common/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-24 09:44:12.959683 mns_common-1.1.2.7/mns_common/api/
--rw-rw-rw-   0        0        0      163 2023-12-15 04:00:46.000000 mns_common-1.1.2.7/mns_common/api/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-24 09:44:12.962675 mns_common-1.1.2.7/mns_common/api/akshare/
--rw-rw-rw-   0        0        0      165 2023-12-15 04:25:30.000000 mns_common-1.1.2.7/mns_common/api/akshare/__init__.py
--rw-rw-rw-   0        0        0     5057 2023-12-22 09:50:37.000000 mns_common-1.1.2.7/mns_common/api/akshare/k_line_api.py
--rw-rw-rw-   0        0        0     5999 2024-01-05 08:16:46.000000 mns_common-1.1.2.7/mns_common/api/akshare/stock_bid_ask_api.py
--rw-rw-rw-   0        0        0     2245 2023-12-16 12:13:22.000000 mns_common-1.1.2.7/mns_common/api/akshare/stock_dt_pool.py
--rw-rw-rw-   0        0        0     2038 2023-12-16 13:25:10.000000 mns_common-1.1.2.7/mns_common/api/akshare/stock_zb_pool.py
--rw-rw-rw-   0        0        0     1929 2023-12-16 12:13:22.000000 mns_common-1.1.2.7/mns_common/api/akshare/stock_zt_pool_api.py
--rw-rw-rw-   0        0        0     4108 2023-12-16 12:13:22.000000 mns_common-1.1.2.7/mns_common/api/akshare/yjyg_sync_api.py
-drwxrwxrwx   0        0        0        0 2024-05-24 09:44:12.964670 mns_common-1.1.2.7/mns_common/api/em/
--rw-rw-rw-   0        0        0      163 2023-12-15 04:08:44.000000 mns_common-1.1.2.7/mns_common/api/em/__init__.py
--rw-rw-rw-   0        0        0     8352 2024-05-10 13:01:52.000000 mns_common-1.1.2.7/mns_common/api/em/east_money_stock_api.py
--rw-rw-rw-   0        0        0     5504 2023-12-22 09:50:37.000000 mns_common-1.1.2.7/mns_common/api/em/east_money_stock_gdfx_free_top_10_api.py
--rw-rw-rw-   0        0        0     4371 2024-05-17 04:06:34.000000 mns_common-1.1.2.7/mns_common/api/em/east_money_stock_hk_api.py
--rw-rw-rw-   0        0        0    14960 2024-05-10 12:40:48.000000 mns_common-1.1.2.7/mns_common/api/em/east_money_stock_v2_api.py
--rw-rw-rw-   0        0        0     8285 2023-12-22 09:50:37.000000 mns_common-1.1.2.7/mns_common/api/em/em_concept_index_api.py
-drwxrwxrwx   0        0        0        0 2024-05-24 09:44:12.965667 mns_common-1.1.2.7/mns_common/api/kpl/
--rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.1.2.7/mns_common/api/kpl/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-24 09:44:12.966664 mns_common-1.1.2.7/mns_common/api/kpl/common/
--rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.1.2.7/mns_common/api/kpl/common/__init__.py
--rw-rw-rw-   0        0        0     6536 2024-04-24 09:08:22.000000 mns_common-1.1.2.7/mns_common/api/kpl/common/kpl_common_api.py
-drwxrwxrwx   0        0        0        0 2024-05-24 09:44:12.966664 mns_common-1.1.2.7/mns_common/api/kpl/concept/
--rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.1.2.7/mns_common/api/kpl/concept/__init__.py
--rw-rw-rw-   0        0        0      607 2023-12-16 12:13:22.000000 mns_common-1.1.2.7/mns_common/api/kpl/concept/kpl_concept_api.py
-drwxrwxrwx   0        0        0        0 2024-05-24 09:44:12.967661 mns_common-1.1.2.7/mns_common/api/kpl/constant/
--rw-rw-rw-   0        0        0      163 2023-12-22 09:50:37.000000 mns_common-1.1.2.7/mns_common/api/kpl/constant/__init__.py
--rw-rw-rw-   0        0        0      669 2023-12-22 09:50:37.000000 mns_common-1.1.2.7/mns_common/api/kpl/constant/kpl_constant.py
-drwxrwxrwx   0        0        0        0 2024-05-24 09:44:12.968659 mns_common-1.1.2.7/mns_common/api/kpl/industry/
--rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.1.2.7/mns_common/api/kpl/industry/__init__.py
--rw-rw-rw-   0        0        0      565 2023-12-16 12:13:22.000000 mns_common-1.1.2.7/mns_common/api/kpl/industry/kpl_industry_api.py
-drwxrwxrwx   0        0        0        0 2024-05-24 09:44:12.969657 mns_common-1.1.2.7/mns_common/api/kpl/selection/
--rw-rw-rw-   0        0        0      163 2023-12-22 09:50:37.000000 mns_common-1.1.2.7/mns_common/api/kpl/selection/__init__.py
--rw-rw-rw-   0        0        0     1926 2024-05-06 13:55:26.000000 mns_common-1.1.2.7/mns_common/api/kpl/selection/kpl_selection_plate_api.py
-drwxrwxrwx   0        0        0        0 2024-05-24 09:44:12.971651 mns_common-1.1.2.7/mns_common/api/kpl/symbol/
--rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.1.2.7/mns_common/api/kpl/symbol/__init__.py
--rw-rw-rw-   0        0        0     4792 2024-03-22 08:55:03.000000 mns_common-1.1.2.7/mns_common/api/kpl/symbol/kpl_real_time_quotes_api.py
--rw-rw-rw-   0        0        0     1625 2024-03-22 08:56:47.000000 mns_common-1.1.2.7/mns_common/api/kpl/symbol/kpl_symbol_common_field_constant.py
--rw-rw-rw-   0        0        0     4210 2024-04-21 02:03:32.000000 mns_common-1.1.2.7/mns_common/api/kpl/symbol/symbol_his_quotes_api.py
-drwxrwxrwx   0        0        0        0 2024-05-24 09:44:12.971651 mns_common-1.1.2.7/mns_common/api/msg/
--rw-rw-rw-   0        0        0      163 2023-12-22 09:50:37.000000 mns_common-1.1.2.7/mns_common/api/msg/__init__.py
--rw-rw-rw-   0        0        0     1421 2024-02-03 04:57:25.000000 mns_common-1.1.2.7/mns_common/api/msg/push_msg_api.py
-drwxrwxrwx   0        0        0        0 2024-05-24 09:44:12.973646 mns_common-1.1.2.7/mns_common/api/ths/
--rw-rw-rw-   0        0        0      163 2023-12-15 03:59:01.000000 mns_common-1.1.2.7/mns_common/api/ths/__init__.py
--rw-rw-rw-   0        0        0     3614 2023-12-22 09:50:37.000000 mns_common-1.1.2.7/mns_common/api/ths/ths_big_deal_api.py
--rw-rw-rw-   0        0        0    40309 2024-05-14 08:22:47.000000 mns_common-1.1.2.7/mns_common/api/ths/ths_stock_api.py
--rw-rw-rw-   0        0        0     6648 2024-05-20 06:35:22.000000 mns_common-1.1.2.7/mns_common/api/ths/ths_stock_zt_pool_api.py
-drwxrwxrwx   0        0        0        0 2024-05-24 09:44:12.974643 mns_common-1.1.2.7/mns_common/component/
--rw-rw-rw-   0        0        0      163 2023-12-15 04:38:42.000000 mns_common-1.1.2.7/mns_common/component/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-24 09:44:12.975641 mns_common-1.1.2.7/mns_common/component/cache/
--rw-rw-rw-   0        0        0      163 2024-04-28 07:37:23.000000 mns_common-1.1.2.7/mns_common/component/cache/__init__.py
--rw-rw-rw-   0        0        0      809 2024-04-28 07:38:03.000000 mns_common-1.1.2.7/mns_common/component/cache/cache_service.py
-drwxrwxrwx   0        0        0        0 2024-05-24 09:44:12.976638 mns_common-1.1.2.7/mns_common/component/classify/
--rw-rw-rw-   0        0        0      163 2024-01-09 08:35:24.000000 mns_common-1.1.2.7/mns_common/component/classify/__init__.py
--rw-rw-rw-   0        0        0      522 2024-01-09 09:22:06.000000 mns_common-1.1.2.7/mns_common/component/classify/classify_constant.py
--rw-rw-rw-   0        0        0     3880 2024-01-09 08:35:24.000000 mns_common-1.1.2.7/mns_common/component/classify/symbol_classify_api.py
--rw-rw-rw-   0        0        0     4896 2024-05-22 14:19:44.000000 mns_common-1.1.2.7/mns_common/component/common_service_fun_api.py
-drwxrwxrwx   0        0        0        0 2024-05-24 09:44:12.977635 mns_common-1.1.2.7/mns_common/component/company/
--rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.1.2.7/mns_common/component/company/__init__.py
--rw-rw-rw-   0        0        0     7803 2024-05-24 09:36:42.000000 mns_common-1.1.2.7/mns_common/component/company/company_common_service_api.py
-drwxrwxrwx   0        0        0        0 2024-05-24 09:44:12.978632 mns_common-1.1.2.7/mns_common/component/concept/
--rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.1.2.7/mns_common/component/concept/__init__.py
--rw-rw-rw-   0        0        0     3235 2024-05-09 14:23:16.000000 mns_common-1.1.2.7/mns_common/component/concept/kpl_concept_common_service_api.py
--rw-rw-rw-   0        0        0     9637 2024-04-30 09:46:26.000000 mns_common-1.1.2.7/mns_common/component/concept/ths_concept_common_service_api.py
-drwxrwxrwx   0        0        0        0 2024-05-24 09:44:12.979630 mns_common-1.1.2.7/mns_common/component/data/
--rw-rw-rw-   0        0        0      163 2024-04-28 07:37:23.000000 mns_common-1.1.2.7/mns_common/component/data/__init__.py
--rw-rw-rw-   0        0        0     4757 2023-12-17 11:40:38.000000 mns_common-1.1.2.7/mns_common/component/data/data_init_api.py
-drwxrwxrwx   0        0        0        0 2024-05-24 09:44:12.980627 mns_common-1.1.2.7/mns_common/component/industry/
--rw-rw-rw-   0        0        0      163 2024-01-13 08:34:39.000000 mns_common-1.1.2.7/mns_common/component/industry/__init__.py
--rw-rw-rw-   0        0        0     3252 2024-01-13 08:57:34.000000 mns_common-1.1.2.7/mns_common/component/industry/ths_industry_index_api.py
-drwxrwxrwx   0        0        0        0 2024-05-24 09:44:12.980627 mns_common-1.1.2.7/mns_common/component/k_line/
--rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.1.2.7/mns_common/component/k_line/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-24 09:44:12.981625 mns_common-1.1.2.7/mns_common/component/k_line/clean/
--rw-rw-rw-   0        0        0      163 2024-01-09 09:22:06.000000 mns_common-1.1.2.7/mns_common/component/k_line/clean/__init__.py
--rw-rw-rw-   0        0        0      248 2024-01-09 09:22:06.000000 mns_common-1.1.2.7/mns_common/component/k_line/clean/k_line_param.py
--rw-rw-rw-   0        0        0    12593 2024-01-09 10:28:47.000000 mns_common-1.1.2.7/mns_common/component/k_line/clean/sh_small_normal_zt_k_line_check_api.py
-drwxrwxrwx   0        0        0        0 2024-05-24 09:44:12.982622 mns_common-1.1.2.7/mns_common/component/k_line/common/
--rw-rw-rw-   0        0        0      163 2023-12-22 09:41:45.000000 mns_common-1.1.2.7/mns_common/component/k_line/common/__init__.py
--rw-rw-rw-   0        0        0     4770 2024-05-20 14:28:57.000000 mns_common-1.1.2.7/mns_common/component/k_line/common/k_line_common_service_api.py
-drwxrwxrwx   0        0        0        0 2024-05-24 09:44:12.983619 mns_common-1.1.2.7/mns_common/component/k_line/patterns/
--rw-rw-rw-   0        0        0      163 2023-12-22 07:50:10.000000 mns_common-1.1.2.7/mns_common/component/k_line/patterns/__init__.py
--rw-rw-rw-   0        0        0     1809 2023-12-22 08:25:35.000000 mns_common-1.1.2.7/mns_common/component/k_line/patterns/k_line_patterns_service_api.py
--rw-rw-rw-   0        0        0      509 2023-12-22 09:49:23.000000 mns_common-1.1.2.7/mns_common/component/k_line/patterns/pattern_Enum.py
-drwxrwxrwx   0        0        0        0 2024-05-24 09:44:12.984616 mns_common-1.1.2.7/mns_common/component/qmt/
--rw-rw-rw-   0        0        0      163 2024-05-23 13:30:35.000000 mns_common-1.1.2.7/mns_common/component/qmt/__init__.py
--rw-rw-rw-   0        0        0     7540 2024-05-23 14:38:14.000000 mns_common-1.1.2.7/mns_common/component/qmt/qmt_buy_service.py
-drwxrwxrwx   0        0        0        0 2024-05-24 09:44:12.985614 mns_common-1.1.2.7/mns_common/component/real_time/
--rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.1.2.7/mns_common/component/real_time/__init__.py
--rw-rw-rw-   0        0        0     1378 2023-12-16 12:13:22.000000 mns_common-1.1.2.7/mns_common/component/real_time/real_time_common_service_api.py
-drwxrwxrwx   0        0        0        0 2024-05-24 09:44:12.986611 mns_common-1.1.2.7/mns_common/component/self_choose/
--rw-rw-rw-   0        0        0      163 2024-05-14 15:36:27.000000 mns_common-1.1.2.7/mns_common/component/self_choose/__init__.py
--rw-rw-rw-   0        0        0     2232 2024-05-16 05:56:38.000000 mns_common-1.1.2.7/mns_common/component/self_choose/black_list_service_api.py
--rw-rw-rw-   0        0        0      519 2024-05-18 07:01:06.000000 mns_common-1.1.2.7/mns_common/component/self_choose/self_choose_service_api.py
-drwxrwxrwx   0        0        0        0 2024-05-24 09:44:12.987608 mns_common-1.1.2.7/mns_common/component/trade/
--rw-rw-rw-   0        0        0      163 2024-04-27 12:44:35.000000 mns_common-1.1.2.7/mns_common/component/trade/__init__.py
--rw-rw-rw-   0        0        0     3120 2024-05-08 07:34:38.000000 mns_common-1.1.2.7/mns_common/component/trade/trade_service_api.py
-drwxrwxrwx   0        0        0        0 2024-05-24 09:44:12.988606 mns_common-1.1.2.7/mns_common/component/trade_date/
--rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.1.2.7/mns_common/component/trade_date/__init__.py
--rw-rw-rw-   0        0        0     2776 2023-12-28 13:35:59.000000 mns_common-1.1.2.7/mns_common/component/trade_date/trade_date_common_service_api.py
-drwxrwxrwx   0        0        0        0 2024-05-24 09:44:12.988606 mns_common-1.1.2.7/mns_common/component/zt/
--rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.1.2.7/mns_common/component/zt/__init__.py
--rw-rw-rw-   0        0        0     9927 2024-05-22 08:23:47.000000 mns_common-1.1.2.7/mns_common/component/zt/zt_common_service_api.py
-drwxrwxrwx   0        0        0        0 2024-05-24 09:44:12.990600 mns_common-1.1.2.7/mns_common/constant/
--rw-rw-rw-   0        0        0      163 2023-12-17 08:25:43.000000 mns_common-1.1.2.7/mns_common/constant/__init__.py
--rw-rw-rw-   0        0        0     2137 2024-05-23 14:39:22.000000 mns_common-1.1.2.7/mns_common/constant/db_name_constant.py
--rw-rw-rw-   0        0        0     4507 2024-01-25 14:21:07.000000 mns_common-1.1.2.7/mns_common/constant/kpl_selection_no_choose_constant.py
--rw-rw-rw-   0        0        0      492 2024-05-24 09:42:58.000000 mns_common-1.1.2.7/mns_common/constant/self_choose_constant.py
--rw-rw-rw-   0        0        0    12240 2024-03-11 15:08:57.000000 mns_common-1.1.2.7/mns_common/constant/ths_concept_no_choose_constant.py
-drwxrwxrwx   0        0        0        0 2024-05-24 09:44:12.991598 mns_common-1.1.2.7/mns_common/db/
--rw-rw-rw-   0        0        0    11498 2024-05-24 08:29:28.000000 mns_common-1.1.2.7/mns_common/db/MongodbUtil.py
--rw-rw-rw-   0        0        0      163 2023-12-15 04:08:44.000000 mns_common-1.1.2.7/mns_common/db/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-24 09:44:12.993592 mns_common-1.1.2.7/mns_common/utils/
--rw-rw-rw-   0        0        0      163 2023-12-15 04:00:46.000000 mns_common-1.1.2.7/mns_common/utils/__init__.py
--rw-rw-rw-   0        0        0      352 2023-12-15 04:16:28.000000 mns_common-1.1.2.7/mns_common/utils/async_fun.py
--rw-rw-rw-   0        0        0     1316 2023-12-22 08:25:35.000000 mns_common-1.1.2.7/mns_common/utils/data_frame_util.py
--rw-rw-rw-   0        0        0     7379 2023-12-21 03:38:02.000000 mns_common-1.1.2.7/mns_common/utils/date_handle_util.py
--rw-rw-rw-   0        0        0      451 2023-12-15 04:16:28.000000 mns_common-1.1.2.7/mns_common/utils/ip_util.py
-drwxrwxrwx   0        0        0        0 2024-05-24 09:44:12.994590 mns_common-1.1.2.7/mns_common.egg-info/
--rw-rw-rw-   0        0        0       59 2024-05-24 09:44:12.000000 mns_common-1.1.2.7/mns_common.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3953 2024-05-24 09:44:12.000000 mns_common-1.1.2.7/mns_common.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 09:44:12.000000 mns_common-1.1.2.7/mns_common.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-24 09:44:12.000000 mns_common-1.1.2.7/mns_common.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-24 09:44:12.995587 mns_common-1.1.2.7/setup.cfg
--rw-rw-rw-   0        0        0      466 2024-05-24 09:44:11.000000 mns_common-1.1.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 10:15:33.578937 mns_common-1.1.2.8/
+-rw-rw-rw-   0        0        0       59 2024-05-24 10:15:33.578937 mns_common-1.1.2.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1354 2023-12-14 15:25:31.000000 mns_common-1.1.2.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-24 10:15:33.542051 mns_common-1.1.2.8/mns_common/
+-rw-rw-rw-   0        0        0      163 2024-01-10 10:52:31.000000 mns_common-1.1.2.8/mns_common/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 10:15:33.543576 mns_common-1.1.2.8/mns_common/api/
+-rw-rw-rw-   0        0        0      163 2023-12-15 04:00:46.000000 mns_common-1.1.2.8/mns_common/api/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 10:15:33.546571 mns_common-1.1.2.8/mns_common/api/akshare/
+-rw-rw-rw-   0        0        0      165 2023-12-15 04:25:30.000000 mns_common-1.1.2.8/mns_common/api/akshare/__init__.py
+-rw-rw-rw-   0        0        0     5057 2023-12-22 09:50:37.000000 mns_common-1.1.2.8/mns_common/api/akshare/k_line_api.py
+-rw-rw-rw-   0        0        0     5999 2024-01-05 08:16:46.000000 mns_common-1.1.2.8/mns_common/api/akshare/stock_bid_ask_api.py
+-rw-rw-rw-   0        0        0     2245 2023-12-16 12:13:22.000000 mns_common-1.1.2.8/mns_common/api/akshare/stock_dt_pool.py
+-rw-rw-rw-   0        0        0     2038 2023-12-16 13:25:10.000000 mns_common-1.1.2.8/mns_common/api/akshare/stock_zb_pool.py
+-rw-rw-rw-   0        0        0     1929 2023-12-16 12:13:22.000000 mns_common-1.1.2.8/mns_common/api/akshare/stock_zt_pool_api.py
+-rw-rw-rw-   0        0        0     4108 2023-12-16 12:13:22.000000 mns_common-1.1.2.8/mns_common/api/akshare/yjyg_sync_api.py
+drwxrwxrwx   0        0        0        0 2024-05-24 10:15:33.549565 mns_common-1.1.2.8/mns_common/api/em/
+-rw-rw-rw-   0        0        0      163 2023-12-15 04:08:44.000000 mns_common-1.1.2.8/mns_common/api/em/__init__.py
+-rw-rw-rw-   0        0        0     8352 2024-05-10 13:01:52.000000 mns_common-1.1.2.8/mns_common/api/em/east_money_stock_api.py
+-rw-rw-rw-   0        0        0     5504 2023-12-22 09:50:37.000000 mns_common-1.1.2.8/mns_common/api/em/east_money_stock_gdfx_free_top_10_api.py
+-rw-rw-rw-   0        0        0     4371 2024-05-17 04:06:34.000000 mns_common-1.1.2.8/mns_common/api/em/east_money_stock_hk_api.py
+-rw-rw-rw-   0        0        0    14960 2024-05-10 12:40:48.000000 mns_common-1.1.2.8/mns_common/api/em/east_money_stock_v2_api.py
+-rw-rw-rw-   0        0        0     8285 2023-12-22 09:50:37.000000 mns_common-1.1.2.8/mns_common/api/em/em_concept_index_api.py
+drwxrwxrwx   0        0        0        0 2024-05-24 10:15:33.549565 mns_common-1.1.2.8/mns_common/api/kpl/
+-rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.1.2.8/mns_common/api/kpl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 10:15:33.550561 mns_common-1.1.2.8/mns_common/api/kpl/common/
+-rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.1.2.8/mns_common/api/kpl/common/__init__.py
+-rw-rw-rw-   0        0        0     6536 2024-04-24 09:08:22.000000 mns_common-1.1.2.8/mns_common/api/kpl/common/kpl_common_api.py
+drwxrwxrwx   0        0        0        0 2024-05-24 10:15:33.551562 mns_common-1.1.2.8/mns_common/api/kpl/concept/
+-rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.1.2.8/mns_common/api/kpl/concept/__init__.py
+-rw-rw-rw-   0        0        0      607 2023-12-16 12:13:22.000000 mns_common-1.1.2.8/mns_common/api/kpl/concept/kpl_concept_api.py
+drwxrwxrwx   0        0        0        0 2024-05-24 10:15:33.552554 mns_common-1.1.2.8/mns_common/api/kpl/constant/
+-rw-rw-rw-   0        0        0      163 2023-12-22 09:50:37.000000 mns_common-1.1.2.8/mns_common/api/kpl/constant/__init__.py
+-rw-rw-rw-   0        0        0      235 2024-05-24 10:14:14.000000 mns_common-1.1.2.8/mns_common/api/kpl/constant/kpl_constant.py
+drwxrwxrwx   0        0        0        0 2024-05-24 10:15:33.552554 mns_common-1.1.2.8/mns_common/api/kpl/industry/
+-rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.1.2.8/mns_common/api/kpl/industry/__init__.py
+-rw-rw-rw-   0        0        0      565 2023-12-16 12:13:22.000000 mns_common-1.1.2.8/mns_common/api/kpl/industry/kpl_industry_api.py
+drwxrwxrwx   0        0        0        0 2024-05-24 10:15:33.553556 mns_common-1.1.2.8/mns_common/api/kpl/selection/
+-rw-rw-rw-   0        0        0      163 2023-12-22 09:50:37.000000 mns_common-1.1.2.8/mns_common/api/kpl/selection/__init__.py
+-rw-rw-rw-   0        0        0     1926 2024-05-06 13:55:26.000000 mns_common-1.1.2.8/mns_common/api/kpl/selection/kpl_selection_plate_api.py
+drwxrwxrwx   0        0        0        0 2024-05-24 10:15:33.555552 mns_common-1.1.2.8/mns_common/api/kpl/symbol/
+-rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.1.2.8/mns_common/api/kpl/symbol/__init__.py
+-rw-rw-rw-   0        0        0     4792 2024-03-22 08:55:03.000000 mns_common-1.1.2.8/mns_common/api/kpl/symbol/kpl_real_time_quotes_api.py
+-rw-rw-rw-   0        0        0     1625 2024-03-22 08:56:47.000000 mns_common-1.1.2.8/mns_common/api/kpl/symbol/kpl_symbol_common_field_constant.py
+-rw-rw-rw-   0        0        0     4210 2024-04-21 02:03:32.000000 mns_common-1.1.2.8/mns_common/api/kpl/symbol/symbol_his_quotes_api.py
+drwxrwxrwx   0        0        0        0 2024-05-24 10:15:33.556547 mns_common-1.1.2.8/mns_common/api/msg/
+-rw-rw-rw-   0        0        0      163 2023-12-22 09:50:37.000000 mns_common-1.1.2.8/mns_common/api/msg/__init__.py
+-rw-rw-rw-   0        0        0     1421 2024-02-03 04:57:25.000000 mns_common-1.1.2.8/mns_common/api/msg/push_msg_api.py
+drwxrwxrwx   0        0        0        0 2024-05-24 10:15:33.558538 mns_common-1.1.2.8/mns_common/api/ths/
+-rw-rw-rw-   0        0        0      163 2023-12-15 03:59:01.000000 mns_common-1.1.2.8/mns_common/api/ths/__init__.py
+-rw-rw-rw-   0        0        0     3614 2023-12-22 09:50:37.000000 mns_common-1.1.2.8/mns_common/api/ths/ths_big_deal_api.py
+-rw-rw-rw-   0        0        0    40309 2024-05-14 08:22:47.000000 mns_common-1.1.2.8/mns_common/api/ths/ths_stock_api.py
+-rw-rw-rw-   0        0        0     6648 2024-05-20 06:35:22.000000 mns_common-1.1.2.8/mns_common/api/ths/ths_stock_zt_pool_api.py
+drwxrwxrwx   0        0        0        0 2024-05-24 10:15:33.559547 mns_common-1.1.2.8/mns_common/component/
+-rw-rw-rw-   0        0        0      163 2023-12-15 04:38:42.000000 mns_common-1.1.2.8/mns_common/component/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 10:15:33.559547 mns_common-1.1.2.8/mns_common/component/cache/
+-rw-rw-rw-   0        0        0      163 2024-04-28 07:37:23.000000 mns_common-1.1.2.8/mns_common/component/cache/__init__.py
+-rw-rw-rw-   0        0        0      809 2024-04-28 07:38:03.000000 mns_common-1.1.2.8/mns_common/component/cache/cache_service.py
+drwxrwxrwx   0        0        0        0 2024-05-24 10:15:33.561530 mns_common-1.1.2.8/mns_common/component/classify/
+-rw-rw-rw-   0        0        0      163 2024-01-09 08:35:24.000000 mns_common-1.1.2.8/mns_common/component/classify/__init__.py
+-rw-rw-rw-   0        0        0      522 2024-01-09 09:22:06.000000 mns_common-1.1.2.8/mns_common/component/classify/classify_constant.py
+-rw-rw-rw-   0        0        0     3880 2024-01-09 08:35:24.000000 mns_common-1.1.2.8/mns_common/component/classify/symbol_classify_api.py
+-rw-rw-rw-   0        0        0     4896 2024-05-22 14:19:44.000000 mns_common-1.1.2.8/mns_common/component/common_service_fun_api.py
+drwxrwxrwx   0        0        0        0 2024-05-24 10:15:33.561530 mns_common-1.1.2.8/mns_common/component/company/
+-rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.1.2.8/mns_common/component/company/__init__.py
+-rw-rw-rw-   0        0        0     7803 2024-05-24 09:36:42.000000 mns_common-1.1.2.8/mns_common/component/company/company_common_service_api.py
+drwxrwxrwx   0        0        0        0 2024-05-24 10:15:33.563525 mns_common-1.1.2.8/mns_common/component/concept/
+-rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.1.2.8/mns_common/component/concept/__init__.py
+-rw-rw-rw-   0        0        0     3235 2024-05-09 14:23:16.000000 mns_common-1.1.2.8/mns_common/component/concept/kpl_concept_common_service_api.py
+-rw-rw-rw-   0        0        0     9637 2024-04-30 09:46:26.000000 mns_common-1.1.2.8/mns_common/component/concept/ths_concept_common_service_api.py
+drwxrwxrwx   0        0        0        0 2024-05-24 10:15:33.563525 mns_common-1.1.2.8/mns_common/component/data/
+-rw-rw-rw-   0        0        0      163 2024-04-28 07:37:23.000000 mns_common-1.1.2.8/mns_common/component/data/__init__.py
+-rw-rw-rw-   0        0        0     4757 2023-12-17 11:40:38.000000 mns_common-1.1.2.8/mns_common/component/data/data_init_api.py
+drwxrwxrwx   0        0        0        0 2024-05-24 10:15:33.564522 mns_common-1.1.2.8/mns_common/component/industry/
+-rw-rw-rw-   0        0        0      163 2024-01-13 08:34:39.000000 mns_common-1.1.2.8/mns_common/component/industry/__init__.py
+-rw-rw-rw-   0        0        0     3252 2024-01-13 08:57:34.000000 mns_common-1.1.2.8/mns_common/component/industry/ths_industry_index_api.py
+drwxrwxrwx   0        0        0        0 2024-05-24 10:15:33.565610 mns_common-1.1.2.8/mns_common/component/k_line/
+-rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.1.2.8/mns_common/component/k_line/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 10:15:33.566668 mns_common-1.1.2.8/mns_common/component/k_line/clean/
+-rw-rw-rw-   0        0        0      163 2024-01-09 09:22:06.000000 mns_common-1.1.2.8/mns_common/component/k_line/clean/__init__.py
+-rw-rw-rw-   0        0        0      248 2024-01-09 09:22:06.000000 mns_common-1.1.2.8/mns_common/component/k_line/clean/k_line_param.py
+-rw-rw-rw-   0        0        0    12593 2024-01-09 10:28:47.000000 mns_common-1.1.2.8/mns_common/component/k_line/clean/sh_small_normal_zt_k_line_check_api.py
+drwxrwxrwx   0        0        0        0 2024-05-24 10:15:33.567697 mns_common-1.1.2.8/mns_common/component/k_line/common/
+-rw-rw-rw-   0        0        0      163 2023-12-22 09:41:45.000000 mns_common-1.1.2.8/mns_common/component/k_line/common/__init__.py
+-rw-rw-rw-   0        0        0     4770 2024-05-20 14:28:57.000000 mns_common-1.1.2.8/mns_common/component/k_line/common/k_line_common_service_api.py
+drwxrwxrwx   0        0        0        0 2024-05-24 10:15:33.568724 mns_common-1.1.2.8/mns_common/component/k_line/patterns/
+-rw-rw-rw-   0        0        0      163 2023-12-22 07:50:10.000000 mns_common-1.1.2.8/mns_common/component/k_line/patterns/__init__.py
+-rw-rw-rw-   0        0        0     1809 2023-12-22 08:25:35.000000 mns_common-1.1.2.8/mns_common/component/k_line/patterns/k_line_patterns_service_api.py
+-rw-rw-rw-   0        0        0      509 2023-12-22 09:49:23.000000 mns_common-1.1.2.8/mns_common/component/k_line/patterns/pattern_Enum.py
+drwxrwxrwx   0        0        0        0 2024-05-24 10:15:33.569750 mns_common-1.1.2.8/mns_common/component/qmt/
+-rw-rw-rw-   0        0        0      163 2024-05-23 13:30:35.000000 mns_common-1.1.2.8/mns_common/component/qmt/__init__.py
+-rw-rw-rw-   0        0        0     7540 2024-05-23 14:38:14.000000 mns_common-1.1.2.8/mns_common/component/qmt/qmt_buy_service.py
+drwxrwxrwx   0        0        0        0 2024-05-24 10:15:33.570262 mns_common-1.1.2.8/mns_common/component/real_time/
+-rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.1.2.8/mns_common/component/real_time/__init__.py
+-rw-rw-rw-   0        0        0     1378 2023-12-16 12:13:22.000000 mns_common-1.1.2.8/mns_common/component/real_time/real_time_common_service_api.py
+drwxrwxrwx   0        0        0        0 2024-05-24 10:15:33.571802 mns_common-1.1.2.8/mns_common/component/self_choose/
+-rw-rw-rw-   0        0        0      163 2024-05-14 15:36:27.000000 mns_common-1.1.2.8/mns_common/component/self_choose/__init__.py
+-rw-rw-rw-   0        0        0     2232 2024-05-16 05:56:38.000000 mns_common-1.1.2.8/mns_common/component/self_choose/black_list_service_api.py
+-rw-rw-rw-   0        0        0      519 2024-05-18 07:01:06.000000 mns_common-1.1.2.8/mns_common/component/self_choose/self_choose_service_api.py
+drwxrwxrwx   0        0        0        0 2024-05-24 10:15:33.572314 mns_common-1.1.2.8/mns_common/component/trade/
+-rw-rw-rw-   0        0        0      163 2024-04-27 12:44:35.000000 mns_common-1.1.2.8/mns_common/component/trade/__init__.py
+-rw-rw-rw-   0        0        0     3120 2024-05-08 07:34:38.000000 mns_common-1.1.2.8/mns_common/component/trade/trade_service_api.py
+drwxrwxrwx   0        0        0        0 2024-05-24 10:15:33.573351 mns_common-1.1.2.8/mns_common/component/trade_date/
+-rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.1.2.8/mns_common/component/trade_date/__init__.py
+-rw-rw-rw-   0        0        0     2776 2023-12-28 13:35:59.000000 mns_common-1.1.2.8/mns_common/component/trade_date/trade_date_common_service_api.py
+drwxrwxrwx   0        0        0        0 2024-05-24 10:15:33.573863 mns_common-1.1.2.8/mns_common/component/zt/
+-rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.1.2.8/mns_common/component/zt/__init__.py
+-rw-rw-rw-   0        0        0     9927 2024-05-22 08:23:47.000000 mns_common-1.1.2.8/mns_common/component/zt/zt_common_service_api.py
+drwxrwxrwx   0        0        0        0 2024-05-24 10:15:33.575399 mns_common-1.1.2.8/mns_common/constant/
+-rw-rw-rw-   0        0        0      163 2023-12-17 08:25:43.000000 mns_common-1.1.2.8/mns_common/constant/__init__.py
+-rw-rw-rw-   0        0        0     2214 2024-05-24 10:15:22.000000 mns_common-1.1.2.8/mns_common/constant/db_name_constant.py
+-rw-rw-rw-   0        0        0      492 2024-05-24 09:42:58.000000 mns_common-1.1.2.8/mns_common/constant/self_choose_constant.py
+drwxrwxrwx   0        0        0        0 2024-05-24 10:15:33.575913 mns_common-1.1.2.8/mns_common/db/
+-rw-rw-rw-   0        0        0    11498 2024-05-24 08:29:28.000000 mns_common-1.1.2.8/mns_common/db/MongodbUtil.py
+-rw-rw-rw-   0        0        0      163 2023-12-15 04:08:44.000000 mns_common-1.1.2.8/mns_common/db/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 10:15:33.577940 mns_common-1.1.2.8/mns_common/utils/
+-rw-rw-rw-   0        0        0      163 2023-12-15 04:00:46.000000 mns_common-1.1.2.8/mns_common/utils/__init__.py
+-rw-rw-rw-   0        0        0      352 2023-12-15 04:16:28.000000 mns_common-1.1.2.8/mns_common/utils/async_fun.py
+-rw-rw-rw-   0        0        0     1316 2023-12-22 08:25:35.000000 mns_common-1.1.2.8/mns_common/utils/data_frame_util.py
+-rw-rw-rw-   0        0        0     7379 2023-12-21 03:38:02.000000 mns_common-1.1.2.8/mns_common/utils/date_handle_util.py
+-rw-rw-rw-   0        0        0      451 2023-12-15 04:16:28.000000 mns_common-1.1.2.8/mns_common/utils/ip_util.py
+drwxrwxrwx   0        0        0        0 2024-05-24 10:15:33.577940 mns_common-1.1.2.8/mns_common.egg-info/
+-rw-rw-rw-   0        0        0       59 2024-05-24 10:15:33.000000 mns_common-1.1.2.8/mns_common.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3843 2024-05-24 10:15:33.000000 mns_common-1.1.2.8/mns_common.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 10:15:33.000000 mns_common-1.1.2.8/mns_common.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-24 10:15:33.000000 mns_common-1.1.2.8/mns_common.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-24 10:15:33.578937 mns_common-1.1.2.8/setup.cfg
+-rw-rw-rw-   0        0        0      466 2024-05-24 10:15:22.000000 mns_common-1.1.2.8/setup.py
```

### Comparing `mns_common-1.1.2.7/README.md` & `mns_common-1.1.2.8/README.md`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.7/mns_common/api/akshare/k_line_api.py` & `mns_common-1.1.2.8/mns_common/api/akshare/k_line_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.7/mns_common/api/akshare/stock_bid_ask_api.py` & `mns_common-1.1.2.8/mns_common/api/akshare/stock_bid_ask_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.7/mns_common/api/akshare/stock_dt_pool.py` & `mns_common-1.1.2.8/mns_common/api/akshare/stock_dt_pool.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.7/mns_common/api/akshare/stock_zb_pool.py` & `mns_common-1.1.2.8/mns_common/api/akshare/stock_zb_pool.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.7/mns_common/api/akshare/stock_zt_pool_api.py` & `mns_common-1.1.2.8/mns_common/api/akshare/stock_zt_pool_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.7/mns_common/api/akshare/yjyg_sync_api.py` & `mns_common-1.1.2.8/mns_common/api/akshare/yjyg_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.7/mns_common/api/em/east_money_stock_api.py` & `mns_common-1.1.2.8/mns_common/api/em/east_money_stock_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.7/mns_common/api/em/east_money_stock_gdfx_free_top_10_api.py` & `mns_common-1.1.2.8/mns_common/api/em/east_money_stock_gdfx_free_top_10_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.7/mns_common/api/em/east_money_stock_hk_api.py` & `mns_common-1.1.2.8/mns_common/api/em/east_money_stock_hk_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.7/mns_common/api/em/east_money_stock_v2_api.py` & `mns_common-1.1.2.8/mns_common/api/em/east_money_stock_v2_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.7/mns_common/api/em/em_concept_index_api.py` & `mns_common-1.1.2.8/mns_common/api/em/em_concept_index_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.7/mns_common/api/kpl/common/kpl_common_api.py` & `mns_common-1.1.2.8/mns_common/api/kpl/common/kpl_common_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.7/mns_common/api/kpl/concept/kpl_concept_api.py` & `mns_common-1.1.2.8/mns_common/api/kpl/concept/kpl_concept_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.7/mns_common/api/kpl/industry/kpl_industry_api.py` & `mns_common-1.1.2.8/mns_common/api/kpl/industry/kpl_industry_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.7/mns_common/api/kpl/selection/kpl_selection_plate_api.py` & `mns_common-1.1.2.8/mns_common/api/kpl/selection/kpl_selection_plate_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.7/mns_common/api/kpl/symbol/kpl_real_time_quotes_api.py` & `mns_common-1.1.2.8/mns_common/api/kpl/symbol/kpl_real_time_quotes_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.7/mns_common/api/kpl/symbol/kpl_symbol_common_field_constant.py` & `mns_common-1.1.2.8/mns_common/api/kpl/symbol/kpl_symbol_common_field_constant.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.7/mns_common/api/kpl/symbol/symbol_his_quotes_api.py` & `mns_common-1.1.2.8/mns_common/api/kpl/symbol/symbol_his_quotes_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.7/mns_common/api/msg/push_msg_api.py` & `mns_common-1.1.2.8/mns_common/api/msg/push_msg_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.7/mns_common/api/ths/ths_big_deal_api.py` & `mns_common-1.1.2.8/mns_common/api/ths/ths_big_deal_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.7/mns_common/api/ths/ths_stock_api.py` & `mns_common-1.1.2.8/mns_common/api/ths/ths_stock_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.7/mns_common/api/ths/ths_stock_zt_pool_api.py` & `mns_common-1.1.2.8/mns_common/api/ths/ths_stock_zt_pool_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.7/mns_common/component/cache/cache_service.py` & `mns_common-1.1.2.8/mns_common/component/cache/cache_service.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.7/mns_common/component/classify/classify_constant.py` & `mns_common-1.1.2.8/mns_common/component/classify/classify_constant.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.7/mns_common/component/classify/symbol_classify_api.py` & `mns_common-1.1.2.8/mns_common/component/classify/symbol_classify_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.7/mns_common/component/common_service_fun_api.py` & `mns_common-1.1.2.8/mns_common/component/common_service_fun_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.7/mns_common/component/company/company_common_service_api.py` & `mns_common-1.1.2.8/mns_common/component/company/company_common_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.7/mns_common/component/concept/kpl_concept_common_service_api.py` & `mns_common-1.1.2.8/mns_common/component/concept/kpl_concept_common_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.7/mns_common/component/concept/ths_concept_common_service_api.py` & `mns_common-1.1.2.8/mns_common/component/concept/ths_concept_common_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.7/mns_common/component/data/data_init_api.py` & `mns_common-1.1.2.8/mns_common/component/data/data_init_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.7/mns_common/component/industry/ths_industry_index_api.py` & `mns_common-1.1.2.8/mns_common/component/industry/ths_industry_index_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.7/mns_common/component/k_line/clean/sh_small_normal_zt_k_line_check_api.py` & `mns_common-1.1.2.8/mns_common/component/k_line/clean/sh_small_normal_zt_k_line_check_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.7/mns_common/component/k_line/common/k_line_common_service_api.py` & `mns_common-1.1.2.8/mns_common/component/k_line/common/k_line_common_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.7/mns_common/component/k_line/patterns/k_line_patterns_service_api.py` & `mns_common-1.1.2.8/mns_common/component/k_line/patterns/k_line_patterns_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.7/mns_common/component/qmt/qmt_buy_service.py` & `mns_common-1.1.2.8/mns_common/component/qmt/qmt_buy_service.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.7/mns_common/component/real_time/real_time_common_service_api.py` & `mns_common-1.1.2.8/mns_common/component/real_time/real_time_common_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.7/mns_common/component/self_choose/black_list_service_api.py` & `mns_common-1.1.2.8/mns_common/component/self_choose/black_list_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.7/mns_common/component/self_choose/self_choose_service_api.py` & `mns_common-1.1.2.8/mns_common/component/self_choose/self_choose_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.7/mns_common/component/trade/trade_service_api.py` & `mns_common-1.1.2.8/mns_common/component/trade/trade_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.7/mns_common/component/trade_date/trade_date_common_service_api.py` & `mns_common-1.1.2.8/mns_common/component/trade_date/trade_date_common_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.7/mns_common/component/zt/zt_common_service_api.py` & `mns_common-1.1.2.8/mns_common/component/zt/zt_common_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.7/mns_common/constant/db_name_constant.py` & `mns_common-1.1.2.8/mns_common/constant/db_name_constant.py`

 * *Files 12% similar despite different names*

```diff
@@ -76,7 +76,10 @@
 COMPANY_INFO_HK = 'company_info_hk'
 
 # k线前复权
 STOCK_QFQ_DAILY = 'stock_qfq_daily'
 
 # 最近高涨股票
 RECENT_HOT_STOCKS = 'recent_hot_stocks'
+
+# 互动提问
+STOCK_INTERACTIVE_QUESTION = 'stock_interactive_question'
```

### Comparing `mns_common-1.1.2.7/mns_common/db/MongodbUtil.py` & `mns_common-1.1.2.8/mns_common/db/MongodbUtil.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.7/mns_common/utils/data_frame_util.py` & `mns_common-1.1.2.8/mns_common/utils/data_frame_util.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.7/mns_common/utils/date_handle_util.py` & `mns_common-1.1.2.8/mns_common/utils/date_handle_util.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.7/mns_common.egg-info/SOURCES.txt` & `mns_common-1.1.2.8/mns_common.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -76,17 +76,15 @@
 mns_common/component/trade/trade_service_api.py
 mns_common/component/trade_date/__init__.py
 mns_common/component/trade_date/trade_date_common_service_api.py
 mns_common/component/zt/__init__.py
 mns_common/component/zt/zt_common_service_api.py
 mns_common/constant/__init__.py
 mns_common/constant/db_name_constant.py
-mns_common/constant/kpl_selection_no_choose_constant.py
 mns_common/constant/self_choose_constant.py
-mns_common/constant/ths_concept_no_choose_constant.py
 mns_common/db/MongodbUtil.py
 mns_common/db/__init__.py
 mns_common/utils/__init__.py
 mns_common/utils/async_fun.py
 mns_common/utils/data_frame_util.py
 mns_common/utils/date_handle_util.py
 mns_common/utils/ip_util.py
```

