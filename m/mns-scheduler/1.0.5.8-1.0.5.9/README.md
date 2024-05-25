# Comparing `tmp/mns-scheduler-1.0.5.8.tar.gz` & `tmp/mns-scheduler-1.0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mns-scheduler-1.0.5.8.tar", last modified: Sat May 25 08:42:17 2024, max compression
+gzip compressed data, was "mns-scheduler-1.0.5.9.tar", last modified: Sat May 25 08:51:15 2024, max compression
```

## Comparing `mns-scheduler-1.0.5.8.tar` & `mns-scheduler-1.0.5.9.tar`

### file list

```diff
@@ -1,134 +1,134 @@
-drwxrwxrwx   0        0        0        0 2024-05-25 08:42:17.080921 mns-scheduler-1.0.5.8/
--rw-rw-rw-   0        0        0       62 2024-05-25 08:42:17.080921 mns-scheduler-1.0.5.8/PKG-INFO
--rw-rw-rw-   0        0        0     1357 2023-12-16 03:56:24.000000 mns-scheduler-1.0.5.8/README.md
-drwxrwxrwx   0        0        0        0 2024-05-25 08:42:17.041995 mns-scheduler-1.0.5.8/mns_scheduler/
--rw-rw-rw-   0        0        0      165 2024-05-20 12:48:16.000000 mns-scheduler-1.0.5.8/mns_scheduler/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-25 08:42:17.043990 mns-scheduler-1.0.5.8/mns_scheduler/backup/
--rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.8/mns_scheduler/backup/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-25 08:42:17.044987 mns-scheduler-1.0.5.8/mns_scheduler/backup/app/
--rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.8/mns_scheduler/backup/app/__init__.py
--rw-rw-rw-   0        0        0     5148 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.8/mns_scheduler/backup/app/ths_new_concept_sync_app.py
-drwxrwxrwx   0        0        0        0 2024-05-25 08:42:17.045984 mns-scheduler-1.0.5.8/mns_scheduler/backup/em/
--rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.8/mns_scheduler/backup/em/__init__.py
--rw-rw-rw-   0        0        0     4992 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.8/mns_scheduler/backup/em/em_new_concept_his_sync.py
--rw-rw-rw-   0        0        0     7083 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.8/mns_scheduler/backup/em/em_new_concept_sync_common_api.py
--rw-rw-rw-   0        0        0     2334 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.8/mns_scheduler/backup/em/em_new_concept_sync_web.py
-drwxrwxrwx   0        0        0        0 2024-05-25 08:42:17.046981 mns-scheduler-1.0.5.8/mns_scheduler/backup/wen_cai/
--rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.8/mns_scheduler/backup/wen_cai/__init__.py
--rw-rw-rw-   0        0        0     1747 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.8/mns_scheduler/backup/wen_cai/wen_cai_concept_sync.py
-drwxrwxrwx   0        0        0        0 2024-05-25 08:42:17.047979 mns-scheduler-1.0.5.8/mns_scheduler/big_deal/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.8/mns_scheduler/big_deal/__init__.py
--rw-rw-rw-   0        0        0     4555 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.8/mns_scheduler/big_deal/ths_big_deal_sync.py
-drwxrwxrwx   0        0        0        0 2024-05-25 08:42:17.049974 mns-scheduler-1.0.5.8/mns_scheduler/company_info/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.8/mns_scheduler/company_info/__init__.py
--rw-rw-rw-   0        0        0    14306 2024-05-17 08:56:50.000000 mns-scheduler-1.0.5.8/mns_scheduler/company_info/company_constant_data.py
--rw-rw-rw-   0        0        0    22727 2024-05-24 07:13:02.000000 mns-scheduler-1.0.5.8/mns_scheduler/company_info/company_info_sync_api.py
--rw-rw-rw-   0        0        0     1993 2024-05-17 07:32:00.000000 mns-scheduler-1.0.5.8/mns_scheduler/company_info/de_list_stock_service.py
-drwxrwxrwx   0        0        0        0 2024-05-25 08:42:17.049974 mns-scheduler-1.0.5.8/mns_scheduler/concept/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.8/mns_scheduler/concept/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-25 08:42:17.050971 mns-scheduler-1.0.5.8/mns_scheduler/concept/clean/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.8/mns_scheduler/concept/clean/__init__.py
--rw-rw-rw-   0        0        0     4512 2024-05-09 14:49:14.000000 mns-scheduler-1.0.5.8/mns_scheduler/concept/clean/kpl_concept_clean_api.py
--rw-rw-rw-   0        0        0     5907 2024-05-09 07:47:40.000000 mns-scheduler-1.0.5.8/mns_scheduler/concept/clean/ths_concept_clean_api.py
-drwxrwxrwx   0        0        0        0 2024-05-25 08:42:17.051968 mns-scheduler-1.0.5.8/mns_scheduler/concept/ths/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.8/mns_scheduler/concept/ths/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-25 08:42:17.052965 mns-scheduler-1.0.5.8/mns_scheduler/concept/ths/common/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.8/mns_scheduler/concept/ths/common/__init__.py
--rw-rw-rw-   0        0        0     6724 2024-04-30 12:29:06.000000 mns-scheduler-1.0.5.8/mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py
--rw-rw-rw-   0        0        0     4460 2024-04-30 09:34:23.000000 mns-scheduler-1.0.5.8/mns_scheduler/concept/ths/common/ths_concept_update_common_api.py
-drwxrwxrwx   0        0        0        0 2024-05-25 08:42:17.053963 mns-scheduler-1.0.5.8/mns_scheduler/concept/ths/sync_new_index/
--rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.8/mns_scheduler/concept/ths/sync_new_index/__init__.py
--rw-rw-rw-   0        0        0     5001 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.8/mns_scheduler/concept/ths/sync_new_index/sync_ths_concept_by_ak_api.py
--rw-rw-rw-   0        0        0     3605 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.8/mns_scheduler/concept/ths/sync_new_index/sync_ths_new_concept_by_web_api.py
-drwxrwxrwx   0        0        0        0 2024-05-25 08:42:17.055957 mns-scheduler-1.0.5.8/mns_scheduler/concept/ths/update_concept_info/
--rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.8/mns_scheduler/concept/ths/update_concept_info/__init__.py
--rw-rw-rw-   0        0        0     1928 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.8/mns_scheduler/concept/ths/update_concept_info/sync_one_concept_all_symbols_api.py
--rw-rw-rw-   0        0        0     8764 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.8/mns_scheduler/concept/ths/update_concept_info/sync_one_symbol_all_concepts_api.py
-drwxrwxrwx   0        0        0        0 2024-05-25 08:42:17.056955 mns-scheduler-1.0.5.8/mns_scheduler/db/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.8/mns_scheduler/db/__init__.py
--rw-rw-rw-   0        0        0     3952 2024-05-10 13:05:35.000000 mns-scheduler-1.0.5.8/mns_scheduler/db/col_move_service.py
--rw-rw-rw-   0        0        0      747 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.8/mns_scheduler/db/db_status.py
-drwxrwxrwx   0        0        0        0 2024-05-25 08:42:17.057952 mns-scheduler-1.0.5.8/mns_scheduler/dt/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.8/mns_scheduler/dt/__init__.py
--rw-rw-rw-   0        0        0     3466 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.8/mns_scheduler/dt/stock_dt_pool_sync.py
-drwxrwxrwx   0        0        0        0 2024-05-25 08:42:17.059947 mns-scheduler-1.0.5.8/mns_scheduler/finance/
--rw-rw-rw-   0        0        0      163 2024-05-15 14:37:41.000000 mns-scheduler-1.0.5.8/mns_scheduler/finance/__init__.py
--rw-rw-rw-   0        0        0    19437 2024-05-16 00:08:00.000000 mns-scheduler-1.0.5.8/mns_scheduler/finance/em_financial_asset_liability_sync_service_api.py
--rw-rw-rw-   0        0        0    14145 2024-05-16 00:05:34.000000 mns-scheduler-1.0.5.8/mns_scheduler/finance/em_financial_profit_sync_service_api.py
--rw-rw-rw-   0        0        0     2471 2024-05-16 08:53:00.000000 mns-scheduler-1.0.5.8/mns_scheduler/finance/finance_common_api.py
--rw-rw-rw-   0        0        0    10561 2024-05-16 09:27:25.000000 mns-scheduler-1.0.5.8/mns_scheduler/finance/financial_high_risk_stock_clean_service_api.py
--rw-rw-rw-   0        0        0     5042 2024-05-16 09:27:25.000000 mns-scheduler-1.0.5.8/mns_scheduler/finance/sync_financial_report_service_api.py
-drwxrwxrwx   0        0        0        0 2024-05-25 08:42:17.060944 mns-scheduler-1.0.5.8/mns_scheduler/finance/test/
--rw-rw-rw-   0        0        0      163 2024-05-16 01:05:27.000000 mns-scheduler-1.0.5.8/mns_scheduler/finance/test/__init__.py
--rw-rw-rw-   0        0        0     1304 2024-05-16 06:04:02.000000 mns-scheduler-1.0.5.8/mns_scheduler/finance/test/fix_blask_list.py
-drwxrwxrwx   0        0        0        0 2024-05-25 08:42:17.061942 mns-scheduler-1.0.5.8/mns_scheduler/hk/
--rw-rw-rw-   0        0        0      163 2024-05-16 07:31:10.000000 mns-scheduler-1.0.5.8/mns_scheduler/hk/__init__.py
--rw-rw-rw-   0        0        0     3661 2024-05-17 08:14:15.000000 mns-scheduler-1.0.5.8/mns_scheduler/hk/hk_company_info_sync_service_api.py
-drwxrwxrwx   0        0        0        0 2024-05-25 08:42:17.062939 mns-scheduler-1.0.5.8/mns_scheduler/irm/
--rw-rw-rw-   0        0        0      163 2024-05-20 12:48:16.000000 mns-scheduler-1.0.5.8/mns_scheduler/irm/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-25 08:42:17.063936 mns-scheduler-1.0.5.8/mns_scheduler/irm/api/
--rw-rw-rw-   0        0        0      163 2024-05-24 14:59:41.000000 mns-scheduler-1.0.5.8/mns_scheduler/irm/api/__init__.py
--rw-rw-rw-   0        0        0     4931 2024-05-24 22:45:39.000000 mns-scheduler-1.0.5.8/mns_scheduler/irm/api/sh_stock_sns_sse_info_api.py
--rw-rw-rw-   0        0        0     6199 2024-05-25 08:40:25.000000 mns-scheduler-1.0.5.8/mns_scheduler/irm/api/sz_stock_sns_sse_info_api.py
--rw-rw-rw-   0        0        0     7808 2024-05-25 08:41:17.000000 mns-scheduler-1.0.5.8/mns_scheduler/irm/stock_irm_cninfo_service.py
-drwxrwxrwx   0        0        0        0 2024-05-25 08:42:17.063936 mns-scheduler-1.0.5.8/mns_scheduler/k_line/
--rw-rw-rw-   0        0        0      161 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.8/mns_scheduler/k_line/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-25 08:42:17.065931 mns-scheduler-1.0.5.8/mns_scheduler/k_line/clean/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.8/mns_scheduler/k_line/clean/__init__.py
--rw-rw-rw-   0        0        0    22262 2024-05-23 09:26:20.000000 mns-scheduler-1.0.5.8/mns_scheduler/k_line/clean/k_line_info_clean_impl.py
--rw-rw-rw-   0        0        0     8118 2024-05-23 15:00:37.000000 mns-scheduler-1.0.5.8/mns_scheduler/k_line/clean/k_line_info_clean_service.py
--rw-rw-rw-   0        0        0     2628 2024-05-23 15:06:42.000000 mns-scheduler-1.0.5.8/mns_scheduler/k_line/clean/recent_hot_stocks_clean_service.py
-drwxrwxrwx   0        0        0        0 2024-05-25 08:42:17.066928 mns-scheduler-1.0.5.8/mns_scheduler/k_line/sync/
--rw-rw-rw-   0        0        0      161 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.8/mns_scheduler/k_line/sync/__init__.py
--rw-rw-rw-   0        0        0     5652 2024-05-11 03:27:17.000000 mns-scheduler-1.0.5.8/mns_scheduler/k_line/sync/daily_week_month_line_sync.py
-drwxrwxrwx   0        0        0        0 2024-05-25 08:42:17.066928 mns-scheduler-1.0.5.8/mns_scheduler/kpl/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.8/mns_scheduler/kpl/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-25 08:42:17.067926 mns-scheduler-1.0.5.8/mns_scheduler/kpl/selection/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.8/mns_scheduler/kpl/selection/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-25 08:42:17.068934 mns-scheduler-1.0.5.8/mns_scheduler/kpl/selection/index/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.8/mns_scheduler/kpl/selection/index/__init__.py
--rw-rw-rw-   0        0        0     4748 2024-05-09 13:26:15.000000 mns-scheduler-1.0.5.8/mns_scheduler/kpl/selection/index/sync_best_choose_his_index.py
--rw-rw-rw-   0        0        0     8016 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.8/mns_scheduler/kpl/selection/index/sync_best_choose_index.py
-drwxrwxrwx   0        0        0        0 2024-05-25 08:42:17.069948 mns-scheduler-1.0.5.8/mns_scheduler/kpl/selection/symbol/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.8/mns_scheduler/kpl/selection/symbol/__init__.py
--rw-rw-rw-   0        0        0     4679 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.8/mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py
-drwxrwxrwx   0        0        0        0 2024-05-25 08:42:17.070948 mns-scheduler-1.0.5.8/mns_scheduler/kpl/selection/total/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.8/mns_scheduler/kpl/selection/total/__init__.py
--rw-rw-rw-   0        0        0    10461 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.8/mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py
-drwxrwxrwx   0        0        0        0 2024-05-25 08:42:17.070948 mns-scheduler-1.0.5.8/mns_scheduler/lhb/
--rw-rw-rw-   0        0        0      163 2024-05-22 07:47:25.000000 mns-scheduler-1.0.5.8/mns_scheduler/lhb/__init__.py
--rw-rw-rw-   0        0        0      641 2024-05-22 07:52:36.000000 mns-scheduler-1.0.5.8/mns_scheduler/lhb/stock_lhb_sync_service.py
-drwxrwxrwx   0        0        0        0 2024-05-25 08:42:17.072942 mns-scheduler-1.0.5.8/mns_scheduler/real_time/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.8/mns_scheduler/real_time/__init__.py
--rw-rw-rw-   0        0        0     1066 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.8/mns_scheduler/real_time/realtime_quotes_now_create_db_index.py
--rw-rw-rw-   0        0        0     9165 2024-05-06 01:29:24.000000 mns-scheduler-1.0.5.8/mns_scheduler/real_time/realtime_quotes_now_sync.py
-drwxrwxrwx   0        0        0        0 2024-05-25 08:42:17.073939 mns-scheduler-1.0.5.8/mns_scheduler/risk/
--rw-rw-rw-   0        0        0      163 2024-05-22 07:47:47.000000 mns-scheduler-1.0.5.8/mns_scheduler/risk/__init__.py
--rw-rw-rw-   0        0        0     5086 2024-05-17 13:05:26.000000 mns-scheduler-1.0.5.8/mns_scheduler/risk/register_and_investigate_stock_sync_api.py
--rw-rw-rw-   0        0        0      871 2024-05-18 01:43:32.000000 mns-scheduler-1.0.5.8/mns_scheduler/risk/stock_equity_mortgage_sync_api.py
-drwxrwxrwx   0        0        0        0 2024-05-25 08:42:17.074937 mns-scheduler-1.0.5.8/mns_scheduler/trade/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.8/mns_scheduler/trade/__init__.py
--rw-rw-rw-   0        0        0      377 2024-04-28 03:16:51.000000 mns-scheduler-1.0.5.8/mns_scheduler/trade/auto_ipo_buy_api.py
--rw-rw-rw-   0        0        0     4423 2024-04-28 08:59:05.000000 mns-scheduler-1.0.5.8/mns_scheduler/trade/auto_sell_service_api.py
--rw-rw-rw-   0        0        0     2739 2024-04-28 08:08:30.000000 mns-scheduler-1.0.5.8/mns_scheduler/trade/sync_position_api.py
-drwxrwxrwx   0        0        0        0 2024-05-25 08:42:17.075934 mns-scheduler-1.0.5.8/mns_scheduler/zb/
--rw-rw-rw-   0        0        0      165 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.8/mns_scheduler/zb/__init__.py
--rw-rw-rw-   0        0        0     1936 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.8/mns_scheduler/zb/stock_zb_pool_sync.py
-drwxrwxrwx   0        0        0        0 2024-05-25 08:42:17.078926 mns-scheduler-1.0.5.8/mns_scheduler/zt/
--rw-rw-rw-   0        0        0     1641 2024-05-22 03:34:21.000000 mns-scheduler-1.0.5.8/mns_scheduler/zt/__init__.py
--rw-rw-rw-   0        0        0     4015 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.8/mns_scheduler/zt/export_open_data_to_excel.py
--rw-rw-rw-   0        0        0    17525 2024-05-21 15:36:02.000000 mns-scheduler-1.0.5.8/mns_scheduler/zt/realtime_quotes_now_zt_kc_sync.py
--rw-rw-rw-   0        0        0    21283 2024-05-17 08:14:54.000000 mns-scheduler-1.0.5.8/mns_scheduler/zt/today_high_chg_pool_sync_api.py
--rw-rw-rw-   0        0        0    10916 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.8/mns_scheduler/zt/zt_five_boards_sync_api.py
--rw-rw-rw-   0        0        0     7604 2024-05-18 00:16:23.000000 mns-scheduler-1.0.5.8/mns_scheduler/zt/zt_pool_sync_api.py
-drwxrwxrwx   0        0        0        0 2024-05-25 08:42:17.079923 mns-scheduler-1.0.5.8/mns_scheduler/zz_task/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.8/mns_scheduler/zz_task/__init__.py
--rw-rw-rw-   0        0        0    16633 2024-05-24 15:47:42.000000 mns-scheduler-1.0.5.8/mns_scheduler/zz_task/data_sync_task.py
--rw-rw-rw-   0        0        0      932 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.8/mns_scheduler/zz_task/sync_realtime_quotes_task.py
-drwxrwxrwx   0        0        0        0 2024-05-25 08:42:17.080921 mns-scheduler-1.0.5.8/mns_scheduler.egg-info/
--rw-rw-rw-   0        0        0       62 2024-05-25 08:42:16.000000 mns-scheduler-1.0.5.8/mns_scheduler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4351 2024-05-25 08:42:16.000000 mns-scheduler-1.0.5.8/mns_scheduler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-25 08:42:16.000000 mns-scheduler-1.0.5.8/mns_scheduler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-05-25 08:42:16.000000 mns-scheduler-1.0.5.8/mns_scheduler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-25 08:42:17.080921 mns-scheduler-1.0.5.8/setup.cfg
--rw-rw-rw-   0        0        0      212 2024-05-25 08:41:59.000000 mns-scheduler-1.0.5.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-25 08:51:15.185525 mns-scheduler-1.0.5.9/
+-rw-rw-rw-   0        0        0       62 2024-05-25 08:51:15.185525 mns-scheduler-1.0.5.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1357 2023-12-16 03:56:24.000000 mns-scheduler-1.0.5.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-25 08:51:15.144636 mns-scheduler-1.0.5.9/mns_scheduler/
+-rw-rw-rw-   0        0        0      165 2024-05-20 12:48:16.000000 mns-scheduler-1.0.5.9/mns_scheduler/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-25 08:51:15.146630 mns-scheduler-1.0.5.9/mns_scheduler/backup/
+-rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.9/mns_scheduler/backup/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-25 08:51:15.147627 mns-scheduler-1.0.5.9/mns_scheduler/backup/app/
+-rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.9/mns_scheduler/backup/app/__init__.py
+-rw-rw-rw-   0        0        0     5148 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.9/mns_scheduler/backup/app/ths_new_concept_sync_app.py
+drwxrwxrwx   0        0        0        0 2024-05-25 08:51:15.149621 mns-scheduler-1.0.5.9/mns_scheduler/backup/em/
+-rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.9/mns_scheduler/backup/em/__init__.py
+-rw-rw-rw-   0        0        0     4992 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.9/mns_scheduler/backup/em/em_new_concept_his_sync.py
+-rw-rw-rw-   0        0        0     7083 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.9/mns_scheduler/backup/em/em_new_concept_sync_common_api.py
+-rw-rw-rw-   0        0        0     2334 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.9/mns_scheduler/backup/em/em_new_concept_sync_web.py
+drwxrwxrwx   0        0        0        0 2024-05-25 08:51:15.150619 mns-scheduler-1.0.5.9/mns_scheduler/backup/wen_cai/
+-rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.9/mns_scheduler/backup/wen_cai/__init__.py
+-rw-rw-rw-   0        0        0     1747 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.9/mns_scheduler/backup/wen_cai/wen_cai_concept_sync.py
+drwxrwxrwx   0        0        0        0 2024-05-25 08:51:15.151616 mns-scheduler-1.0.5.9/mns_scheduler/big_deal/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.9/mns_scheduler/big_deal/__init__.py
+-rw-rw-rw-   0        0        0     4555 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.9/mns_scheduler/big_deal/ths_big_deal_sync.py
+drwxrwxrwx   0        0        0        0 2024-05-25 08:51:15.153611 mns-scheduler-1.0.5.9/mns_scheduler/company_info/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.9/mns_scheduler/company_info/__init__.py
+-rw-rw-rw-   0        0        0    14306 2024-05-17 08:56:50.000000 mns-scheduler-1.0.5.9/mns_scheduler/company_info/company_constant_data.py
+-rw-rw-rw-   0        0        0    22727 2024-05-24 07:13:02.000000 mns-scheduler-1.0.5.9/mns_scheduler/company_info/company_info_sync_api.py
+-rw-rw-rw-   0        0        0     1993 2024-05-17 07:32:00.000000 mns-scheduler-1.0.5.9/mns_scheduler/company_info/de_list_stock_service.py
+drwxrwxrwx   0        0        0        0 2024-05-25 08:51:15.153611 mns-scheduler-1.0.5.9/mns_scheduler/concept/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.9/mns_scheduler/concept/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-25 08:51:15.154609 mns-scheduler-1.0.5.9/mns_scheduler/concept/clean/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.9/mns_scheduler/concept/clean/__init__.py
+-rw-rw-rw-   0        0        0     4512 2024-05-09 14:49:14.000000 mns-scheduler-1.0.5.9/mns_scheduler/concept/clean/kpl_concept_clean_api.py
+-rw-rw-rw-   0        0        0     5907 2024-05-09 07:47:40.000000 mns-scheduler-1.0.5.9/mns_scheduler/concept/clean/ths_concept_clean_api.py
+drwxrwxrwx   0        0        0        0 2024-05-25 08:51:15.155605 mns-scheduler-1.0.5.9/mns_scheduler/concept/ths/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.9/mns_scheduler/concept/ths/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-25 08:51:15.156603 mns-scheduler-1.0.5.9/mns_scheduler/concept/ths/common/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.9/mns_scheduler/concept/ths/common/__init__.py
+-rw-rw-rw-   0        0        0     6724 2024-04-30 12:29:06.000000 mns-scheduler-1.0.5.9/mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py
+-rw-rw-rw-   0        0        0     4460 2024-04-30 09:34:23.000000 mns-scheduler-1.0.5.9/mns_scheduler/concept/ths/common/ths_concept_update_common_api.py
+drwxrwxrwx   0        0        0        0 2024-05-25 08:51:15.157601 mns-scheduler-1.0.5.9/mns_scheduler/concept/ths/sync_new_index/
+-rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.9/mns_scheduler/concept/ths/sync_new_index/__init__.py
+-rw-rw-rw-   0        0        0     5001 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.9/mns_scheduler/concept/ths/sync_new_index/sync_ths_concept_by_ak_api.py
+-rw-rw-rw-   0        0        0     3605 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.9/mns_scheduler/concept/ths/sync_new_index/sync_ths_new_concept_by_web_api.py
+drwxrwxrwx   0        0        0        0 2024-05-25 08:51:15.159595 mns-scheduler-1.0.5.9/mns_scheduler/concept/ths/update_concept_info/
+-rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.9/mns_scheduler/concept/ths/update_concept_info/__init__.py
+-rw-rw-rw-   0        0        0     1928 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.9/mns_scheduler/concept/ths/update_concept_info/sync_one_concept_all_symbols_api.py
+-rw-rw-rw-   0        0        0     8764 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.9/mns_scheduler/concept/ths/update_concept_info/sync_one_symbol_all_concepts_api.py
+drwxrwxrwx   0        0        0        0 2024-05-25 08:51:15.160592 mns-scheduler-1.0.5.9/mns_scheduler/db/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.9/mns_scheduler/db/__init__.py
+-rw-rw-rw-   0        0        0     3952 2024-05-10 13:05:35.000000 mns-scheduler-1.0.5.9/mns_scheduler/db/col_move_service.py
+-rw-rw-rw-   0        0        0      747 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.9/mns_scheduler/db/db_status.py
+drwxrwxrwx   0        0        0        0 2024-05-25 08:51:15.161589 mns-scheduler-1.0.5.9/mns_scheduler/dt/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.9/mns_scheduler/dt/__init__.py
+-rw-rw-rw-   0        0        0     3466 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.9/mns_scheduler/dt/stock_dt_pool_sync.py
+drwxrwxrwx   0        0        0        0 2024-05-25 08:51:15.164582 mns-scheduler-1.0.5.9/mns_scheduler/finance/
+-rw-rw-rw-   0        0        0      163 2024-05-15 14:37:41.000000 mns-scheduler-1.0.5.9/mns_scheduler/finance/__init__.py
+-rw-rw-rw-   0        0        0    19437 2024-05-16 00:08:00.000000 mns-scheduler-1.0.5.9/mns_scheduler/finance/em_financial_asset_liability_sync_service_api.py
+-rw-rw-rw-   0        0        0    14145 2024-05-16 00:05:34.000000 mns-scheduler-1.0.5.9/mns_scheduler/finance/em_financial_profit_sync_service_api.py
+-rw-rw-rw-   0        0        0     2471 2024-05-16 08:53:00.000000 mns-scheduler-1.0.5.9/mns_scheduler/finance/finance_common_api.py
+-rw-rw-rw-   0        0        0    10561 2024-05-16 09:27:25.000000 mns-scheduler-1.0.5.9/mns_scheduler/finance/financial_high_risk_stock_clean_service_api.py
+-rw-rw-rw-   0        0        0     5042 2024-05-16 09:27:25.000000 mns-scheduler-1.0.5.9/mns_scheduler/finance/sync_financial_report_service_api.py
+drwxrwxrwx   0        0        0        0 2024-05-25 08:51:15.164582 mns-scheduler-1.0.5.9/mns_scheduler/finance/test/
+-rw-rw-rw-   0        0        0      163 2024-05-16 01:05:27.000000 mns-scheduler-1.0.5.9/mns_scheduler/finance/test/__init__.py
+-rw-rw-rw-   0        0        0     1304 2024-05-16 06:04:02.000000 mns-scheduler-1.0.5.9/mns_scheduler/finance/test/fix_blask_list.py
+drwxrwxrwx   0        0        0        0 2024-05-25 08:51:15.165579 mns-scheduler-1.0.5.9/mns_scheduler/hk/
+-rw-rw-rw-   0        0        0      163 2024-05-16 07:31:10.000000 mns-scheduler-1.0.5.9/mns_scheduler/hk/__init__.py
+-rw-rw-rw-   0        0        0     3661 2024-05-17 08:14:15.000000 mns-scheduler-1.0.5.9/mns_scheduler/hk/hk_company_info_sync_service_api.py
+drwxrwxrwx   0        0        0        0 2024-05-25 08:51:15.166576 mns-scheduler-1.0.5.9/mns_scheduler/irm/
+-rw-rw-rw-   0        0        0      163 2024-05-20 12:48:16.000000 mns-scheduler-1.0.5.9/mns_scheduler/irm/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-25 08:51:15.167574 mns-scheduler-1.0.5.9/mns_scheduler/irm/api/
+-rw-rw-rw-   0        0        0      163 2024-05-24 14:59:41.000000 mns-scheduler-1.0.5.9/mns_scheduler/irm/api/__init__.py
+-rw-rw-rw-   0        0        0     4931 2024-05-24 22:45:39.000000 mns-scheduler-1.0.5.9/mns_scheduler/irm/api/sh_stock_sns_sse_info_api.py
+-rw-rw-rw-   0        0        0     6199 2024-05-25 08:40:25.000000 mns-scheduler-1.0.5.9/mns_scheduler/irm/api/sz_stock_sns_sse_info_api.py
+-rw-rw-rw-   0        0        0     7905 2024-05-25 08:50:29.000000 mns-scheduler-1.0.5.9/mns_scheduler/irm/stock_irm_cninfo_service.py
+drwxrwxrwx   0        0        0        0 2024-05-25 08:51:15.168571 mns-scheduler-1.0.5.9/mns_scheduler/k_line/
+-rw-rw-rw-   0        0        0      161 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.9/mns_scheduler/k_line/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-25 08:51:15.170566 mns-scheduler-1.0.5.9/mns_scheduler/k_line/clean/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.9/mns_scheduler/k_line/clean/__init__.py
+-rw-rw-rw-   0        0        0    22262 2024-05-23 09:26:20.000000 mns-scheduler-1.0.5.9/mns_scheduler/k_line/clean/k_line_info_clean_impl.py
+-rw-rw-rw-   0        0        0     8118 2024-05-23 15:00:37.000000 mns-scheduler-1.0.5.9/mns_scheduler/k_line/clean/k_line_info_clean_service.py
+-rw-rw-rw-   0        0        0     2628 2024-05-23 15:06:42.000000 mns-scheduler-1.0.5.9/mns_scheduler/k_line/clean/recent_hot_stocks_clean_service.py
+drwxrwxrwx   0        0        0        0 2024-05-25 08:51:15.171563 mns-scheduler-1.0.5.9/mns_scheduler/k_line/sync/
+-rw-rw-rw-   0        0        0      161 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.9/mns_scheduler/k_line/sync/__init__.py
+-rw-rw-rw-   0        0        0     5652 2024-05-11 03:27:17.000000 mns-scheduler-1.0.5.9/mns_scheduler/k_line/sync/daily_week_month_line_sync.py
+drwxrwxrwx   0        0        0        0 2024-05-25 08:51:15.171563 mns-scheduler-1.0.5.9/mns_scheduler/kpl/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.9/mns_scheduler/kpl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-25 08:51:15.171563 mns-scheduler-1.0.5.9/mns_scheduler/kpl/selection/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.9/mns_scheduler/kpl/selection/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-25 08:51:15.173558 mns-scheduler-1.0.5.9/mns_scheduler/kpl/selection/index/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.9/mns_scheduler/kpl/selection/index/__init__.py
+-rw-rw-rw-   0        0        0     4748 2024-05-09 13:26:15.000000 mns-scheduler-1.0.5.9/mns_scheduler/kpl/selection/index/sync_best_choose_his_index.py
+-rw-rw-rw-   0        0        0     8016 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.9/mns_scheduler/kpl/selection/index/sync_best_choose_index.py
+drwxrwxrwx   0        0        0        0 2024-05-25 08:51:15.173558 mns-scheduler-1.0.5.9/mns_scheduler/kpl/selection/symbol/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.9/mns_scheduler/kpl/selection/symbol/__init__.py
+-rw-rw-rw-   0        0        0     4679 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.9/mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py
+drwxrwxrwx   0        0        0        0 2024-05-25 08:51:15.174555 mns-scheduler-1.0.5.9/mns_scheduler/kpl/selection/total/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.9/mns_scheduler/kpl/selection/total/__init__.py
+-rw-rw-rw-   0        0        0    10461 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.9/mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py
+drwxrwxrwx   0        0        0        0 2024-05-25 08:51:15.175552 mns-scheduler-1.0.5.9/mns_scheduler/lhb/
+-rw-rw-rw-   0        0        0      163 2024-05-22 07:47:25.000000 mns-scheduler-1.0.5.9/mns_scheduler/lhb/__init__.py
+-rw-rw-rw-   0        0        0      641 2024-05-22 07:52:36.000000 mns-scheduler-1.0.5.9/mns_scheduler/lhb/stock_lhb_sync_service.py
+drwxrwxrwx   0        0        0        0 2024-05-25 08:51:15.176550 mns-scheduler-1.0.5.9/mns_scheduler/real_time/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.9/mns_scheduler/real_time/__init__.py
+-rw-rw-rw-   0        0        0     1066 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.9/mns_scheduler/real_time/realtime_quotes_now_create_db_index.py
+-rw-rw-rw-   0        0        0     9165 2024-05-06 01:29:24.000000 mns-scheduler-1.0.5.9/mns_scheduler/real_time/realtime_quotes_now_sync.py
+drwxrwxrwx   0        0        0        0 2024-05-25 08:51:15.178545 mns-scheduler-1.0.5.9/mns_scheduler/risk/
+-rw-rw-rw-   0        0        0      163 2024-05-22 07:47:47.000000 mns-scheduler-1.0.5.9/mns_scheduler/risk/__init__.py
+-rw-rw-rw-   0        0        0     5086 2024-05-17 13:05:26.000000 mns-scheduler-1.0.5.9/mns_scheduler/risk/register_and_investigate_stock_sync_api.py
+-rw-rw-rw-   0        0        0      871 2024-05-18 01:43:32.000000 mns-scheduler-1.0.5.9/mns_scheduler/risk/stock_equity_mortgage_sync_api.py
+drwxrwxrwx   0        0        0        0 2024-05-25 08:51:15.179542 mns-scheduler-1.0.5.9/mns_scheduler/trade/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.9/mns_scheduler/trade/__init__.py
+-rw-rw-rw-   0        0        0      377 2024-04-28 03:16:51.000000 mns-scheduler-1.0.5.9/mns_scheduler/trade/auto_ipo_buy_api.py
+-rw-rw-rw-   0        0        0     4423 2024-04-28 08:59:05.000000 mns-scheduler-1.0.5.9/mns_scheduler/trade/auto_sell_service_api.py
+-rw-rw-rw-   0        0        0     2739 2024-04-28 08:08:30.000000 mns-scheduler-1.0.5.9/mns_scheduler/trade/sync_position_api.py
+drwxrwxrwx   0        0        0        0 2024-05-25 08:51:15.180539 mns-scheduler-1.0.5.9/mns_scheduler/zb/
+-rw-rw-rw-   0        0        0      165 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.9/mns_scheduler/zb/__init__.py
+-rw-rw-rw-   0        0        0     1936 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.9/mns_scheduler/zb/stock_zb_pool_sync.py
+drwxrwxrwx   0        0        0        0 2024-05-25 08:51:15.183531 mns-scheduler-1.0.5.9/mns_scheduler/zt/
+-rw-rw-rw-   0        0        0     1641 2024-05-22 03:34:21.000000 mns-scheduler-1.0.5.9/mns_scheduler/zt/__init__.py
+-rw-rw-rw-   0        0        0     4015 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.9/mns_scheduler/zt/export_open_data_to_excel.py
+-rw-rw-rw-   0        0        0    17525 2024-05-21 15:36:02.000000 mns-scheduler-1.0.5.9/mns_scheduler/zt/realtime_quotes_now_zt_kc_sync.py
+-rw-rw-rw-   0        0        0    21283 2024-05-17 08:14:54.000000 mns-scheduler-1.0.5.9/mns_scheduler/zt/today_high_chg_pool_sync_api.py
+-rw-rw-rw-   0        0        0    10916 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.9/mns_scheduler/zt/zt_five_boards_sync_api.py
+-rw-rw-rw-   0        0        0     7604 2024-05-18 00:16:23.000000 mns-scheduler-1.0.5.9/mns_scheduler/zt/zt_pool_sync_api.py
+drwxrwxrwx   0        0        0        0 2024-05-25 08:51:15.184528 mns-scheduler-1.0.5.9/mns_scheduler/zz_task/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.9/mns_scheduler/zz_task/__init__.py
+-rw-rw-rw-   0        0        0    16633 2024-05-24 15:47:42.000000 mns-scheduler-1.0.5.9/mns_scheduler/zz_task/data_sync_task.py
+-rw-rw-rw-   0        0        0      932 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.9/mns_scheduler/zz_task/sync_realtime_quotes_task.py
+drwxrwxrwx   0        0        0        0 2024-05-25 08:51:15.184528 mns-scheduler-1.0.5.9/mns_scheduler.egg-info/
+-rw-rw-rw-   0        0        0       62 2024-05-25 08:51:15.000000 mns-scheduler-1.0.5.9/mns_scheduler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4351 2024-05-25 08:51:15.000000 mns-scheduler-1.0.5.9/mns_scheduler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 08:51:15.000000 mns-scheduler-1.0.5.9/mns_scheduler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-25 08:51:15.000000 mns-scheduler-1.0.5.9/mns_scheduler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-25 08:51:15.185525 mns-scheduler-1.0.5.9/setup.cfg
+-rw-rw-rw-   0        0        0      212 2024-05-25 08:51:05.000000 mns-scheduler-1.0.5.9/setup.py
```

### Comparing `mns-scheduler-1.0.5.8/README.md` & `mns-scheduler-1.0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.8/mns_scheduler/backup/app/ths_new_concept_sync_app.py` & `mns-scheduler-1.0.5.9/mns_scheduler/backup/app/ths_new_concept_sync_app.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.8/mns_scheduler/backup/em/em_new_concept_his_sync.py` & `mns-scheduler-1.0.5.9/mns_scheduler/backup/em/em_new_concept_his_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.8/mns_scheduler/backup/em/em_new_concept_sync_common_api.py` & `mns-scheduler-1.0.5.9/mns_scheduler/backup/em/em_new_concept_sync_common_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.8/mns_scheduler/backup/em/em_new_concept_sync_web.py` & `mns-scheduler-1.0.5.9/mns_scheduler/backup/em/em_new_concept_sync_web.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.8/mns_scheduler/backup/wen_cai/wen_cai_concept_sync.py` & `mns-scheduler-1.0.5.9/mns_scheduler/backup/wen_cai/wen_cai_concept_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.8/mns_scheduler/big_deal/ths_big_deal_sync.py` & `mns-scheduler-1.0.5.9/mns_scheduler/big_deal/ths_big_deal_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.8/mns_scheduler/company_info/company_constant_data.py` & `mns-scheduler-1.0.5.9/mns_scheduler/company_info/company_constant_data.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.8/mns_scheduler/company_info/company_info_sync_api.py` & `mns-scheduler-1.0.5.9/mns_scheduler/company_info/company_info_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.8/mns_scheduler/company_info/de_list_stock_service.py` & `mns-scheduler-1.0.5.9/mns_scheduler/company_info/de_list_stock_service.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.8/mns_scheduler/concept/clean/kpl_concept_clean_api.py` & `mns-scheduler-1.0.5.9/mns_scheduler/concept/clean/kpl_concept_clean_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.8/mns_scheduler/concept/clean/ths_concept_clean_api.py` & `mns-scheduler-1.0.5.9/mns_scheduler/concept/clean/ths_concept_clean_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.8/mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py` & `mns-scheduler-1.0.5.9/mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.8/mns_scheduler/concept/ths/common/ths_concept_update_common_api.py` & `mns-scheduler-1.0.5.9/mns_scheduler/concept/ths/common/ths_concept_update_common_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.8/mns_scheduler/concept/ths/sync_new_index/sync_ths_concept_by_ak_api.py` & `mns-scheduler-1.0.5.9/mns_scheduler/concept/ths/sync_new_index/sync_ths_concept_by_ak_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.8/mns_scheduler/concept/ths/sync_new_index/sync_ths_new_concept_by_web_api.py` & `mns-scheduler-1.0.5.9/mns_scheduler/concept/ths/sync_new_index/sync_ths_new_concept_by_web_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.8/mns_scheduler/concept/ths/update_concept_info/sync_one_concept_all_symbols_api.py` & `mns-scheduler-1.0.5.9/mns_scheduler/concept/ths/update_concept_info/sync_one_concept_all_symbols_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.8/mns_scheduler/concept/ths/update_concept_info/sync_one_symbol_all_concepts_api.py` & `mns-scheduler-1.0.5.9/mns_scheduler/concept/ths/update_concept_info/sync_one_symbol_all_concepts_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.8/mns_scheduler/db/col_move_service.py` & `mns-scheduler-1.0.5.9/mns_scheduler/db/col_move_service.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.8/mns_scheduler/db/db_status.py` & `mns-scheduler-1.0.5.9/mns_scheduler/db/db_status.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.8/mns_scheduler/dt/stock_dt_pool_sync.py` & `mns-scheduler-1.0.5.9/mns_scheduler/dt/stock_dt_pool_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.8/mns_scheduler/finance/em_financial_asset_liability_sync_service_api.py` & `mns-scheduler-1.0.5.9/mns_scheduler/finance/em_financial_asset_liability_sync_service_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.8/mns_scheduler/finance/em_financial_profit_sync_service_api.py` & `mns-scheduler-1.0.5.9/mns_scheduler/finance/em_financial_profit_sync_service_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.8/mns_scheduler/finance/finance_common_api.py` & `mns-scheduler-1.0.5.9/mns_scheduler/finance/finance_common_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.8/mns_scheduler/finance/financial_high_risk_stock_clean_service_api.py` & `mns-scheduler-1.0.5.9/mns_scheduler/finance/financial_high_risk_stock_clean_service_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.8/mns_scheduler/finance/sync_financial_report_service_api.py` & `mns-scheduler-1.0.5.9/mns_scheduler/finance/sync_financial_report_service_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.8/mns_scheduler/finance/test/fix_blask_list.py` & `mns-scheduler-1.0.5.9/mns_scheduler/finance/test/fix_blask_list.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.8/mns_scheduler/hk/hk_company_info_sync_service_api.py` & `mns-scheduler-1.0.5.9/mns_scheduler/hk/hk_company_info_sync_service_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.8/mns_scheduler/irm/api/sh_stock_sns_sse_info_api.py` & `mns-scheduler-1.0.5.9/mns_scheduler/irm/api/sh_stock_sns_sse_info_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.8/mns_scheduler/irm/api/sz_stock_sns_sse_info_api.py` & `mns-scheduler-1.0.5.9/mns_scheduler/irm/api/sz_stock_sns_sse_info_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.8/mns_scheduler/irm/stock_irm_cninfo_service.py` & `mns-scheduler-1.0.5.9/mns_scheduler/irm/stock_irm_cninfo_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 sys.path.append(project_path)
 import akshare as ak
 import mns_common.utils.data_frame_util as data_frame_util
 import pandas as pd
 import mns_common.api.em.east_money_stock_api as east_money_stock_api
 import mns_common.component.company.company_common_service_api as company_common_service_api
 from loguru import logger
-from datetime import datetime
+from datetime import datetime, time
 
 import mns_common.utils.date_handle_util as date_handle_util
 
 import mns_common.constant.db_name_constant as db_name_constant
 import mns_common.component.common_service_fun_api as common_service_fun_api
 import mns_scheduler.irm.api.sh_stock_sns_sse_info_api as sh_stock_sns_sse_info_api
 import mns_scheduler.irm.api.sz_stock_sns_sse_info_api as sz_stock_sns_sse_info_api
@@ -137,25 +137,29 @@
             now_date = datetime.now()
             str_day = now_date.strftime('%Y-%m-%d')
             str_now_date = now_date.strftime('%Y-%m-%d %H:%M:%S')
             classification = stock_one.classification
 
             if classification in ['S', 'C']:
                 stock_irm_cninfo_df = get_stock_irm_cninfo_sz_api(stock_one.symbol)
+                time.sleep(1)
             elif classification in ['K', 'H']:
                 stock_irm_cninfo_df = get_stock_irm_cninfo_sh_api(stock_one.symbol)
+                time.sleep(1)
+
             else:
                 continue
             stock_irm_cninfo_df['sync_time'] = str_now_date
             stock_irm_cninfo_df['str_day'] = str_day
             stock_irm_cninfo_df.drop_duplicates('_id', keep='last', inplace=True)
             stock_irm_cninfo_df.fillna("", inplace=True)
             mongodb_util.save_mongo(stock_irm_cninfo_df, db_name_constant.STOCK_INTERACTIVE_QUESTION)
             logger.info("完成同步互动回答到:{}", stock_one.symbol)
         except Exception as e:
+            time.sleep(2)
             logger.error("同步互动问题出现异常:{},{}", stock_one.symbol, e)
 
 
 if __name__ == '__main__':
     fail_symbol_list = ['000638', '002886', '688778', '688766', '688733', '688778', '688793', '688787']
     # get_stock_irm_cninfo_sh_api('603633')
     sync_all_interactive_questions(None)
```

### Comparing `mns-scheduler-1.0.5.8/mns_scheduler/k_line/clean/k_line_info_clean_impl.py` & `mns-scheduler-1.0.5.9/mns_scheduler/k_line/clean/k_line_info_clean_impl.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.8/mns_scheduler/k_line/clean/k_line_info_clean_service.py` & `mns-scheduler-1.0.5.9/mns_scheduler/k_line/clean/k_line_info_clean_service.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.8/mns_scheduler/k_line/clean/recent_hot_stocks_clean_service.py` & `mns-scheduler-1.0.5.9/mns_scheduler/k_line/clean/recent_hot_stocks_clean_service.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.8/mns_scheduler/k_line/sync/daily_week_month_line_sync.py` & `mns-scheduler-1.0.5.9/mns_scheduler/k_line/sync/daily_week_month_line_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.8/mns_scheduler/kpl/selection/index/sync_best_choose_his_index.py` & `mns-scheduler-1.0.5.9/mns_scheduler/kpl/selection/index/sync_best_choose_his_index.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.8/mns_scheduler/kpl/selection/index/sync_best_choose_index.py` & `mns-scheduler-1.0.5.9/mns_scheduler/kpl/selection/index/sync_best_choose_index.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.8/mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py` & `mns-scheduler-1.0.5.9/mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.8/mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py` & `mns-scheduler-1.0.5.9/mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.8/mns_scheduler/lhb/stock_lhb_sync_service.py` & `mns-scheduler-1.0.5.9/mns_scheduler/lhb/stock_lhb_sync_service.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.8/mns_scheduler/real_time/realtime_quotes_now_create_db_index.py` & `mns-scheduler-1.0.5.9/mns_scheduler/real_time/realtime_quotes_now_create_db_index.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.8/mns_scheduler/real_time/realtime_quotes_now_sync.py` & `mns-scheduler-1.0.5.9/mns_scheduler/real_time/realtime_quotes_now_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.8/mns_scheduler/risk/register_and_investigate_stock_sync_api.py` & `mns-scheduler-1.0.5.9/mns_scheduler/risk/register_and_investigate_stock_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.8/mns_scheduler/risk/stock_equity_mortgage_sync_api.py` & `mns-scheduler-1.0.5.9/mns_scheduler/risk/stock_equity_mortgage_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.8/mns_scheduler/trade/auto_sell_service_api.py` & `mns-scheduler-1.0.5.9/mns_scheduler/trade/auto_sell_service_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.8/mns_scheduler/trade/sync_position_api.py` & `mns-scheduler-1.0.5.9/mns_scheduler/trade/sync_position_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.8/mns_scheduler/zb/stock_zb_pool_sync.py` & `mns-scheduler-1.0.5.9/mns_scheduler/zb/stock_zb_pool_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.8/mns_scheduler/zt/__init__.py` & `mns-scheduler-1.0.5.9/mns_scheduler/zt/__init__.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.8/mns_scheduler/zt/export_open_data_to_excel.py` & `mns-scheduler-1.0.5.9/mns_scheduler/zt/export_open_data_to_excel.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.8/mns_scheduler/zt/realtime_quotes_now_zt_kc_sync.py` & `mns-scheduler-1.0.5.9/mns_scheduler/zt/realtime_quotes_now_zt_kc_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.8/mns_scheduler/zt/today_high_chg_pool_sync_api.py` & `mns-scheduler-1.0.5.9/mns_scheduler/zt/today_high_chg_pool_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.8/mns_scheduler/zt/zt_five_boards_sync_api.py` & `mns-scheduler-1.0.5.9/mns_scheduler/zt/zt_five_boards_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.8/mns_scheduler/zt/zt_pool_sync_api.py` & `mns-scheduler-1.0.5.9/mns_scheduler/zt/zt_pool_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.8/mns_scheduler/zz_task/data_sync_task.py` & `mns-scheduler-1.0.5.9/mns_scheduler/zz_task/data_sync_task.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.8/mns_scheduler/zz_task/sync_realtime_quotes_task.py` & `mns-scheduler-1.0.5.9/mns_scheduler/zz_task/sync_realtime_quotes_task.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.8/mns_scheduler.egg-info/SOURCES.txt` & `mns-scheduler-1.0.5.9/mns_scheduler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

