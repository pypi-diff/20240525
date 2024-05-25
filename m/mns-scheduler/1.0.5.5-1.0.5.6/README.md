# Comparing `tmp/mns-scheduler-1.0.5.5.tar.gz` & `tmp/mns-scheduler-1.0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mns-scheduler-1.0.5.5.tar", last modified: Thu May 23 15:10:53 2024, max compression
+gzip compressed data, was "mns-scheduler-1.0.5.6.tar", last modified: Fri May 24 15:37:11 2024, max compression
```

## Comparing `mns-scheduler-1.0.5.5.tar` & `mns-scheduler-1.0.5.6.tar`

### file list

```diff
@@ -1,130 +1,134 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 15:10:53.442115 mns-scheduler-1.0.5.5/
--rw-rw-rw-   0        0        0       62 2024-05-23 15:10:53.441602 mns-scheduler-1.0.5.5/PKG-INFO
--rw-rw-rw-   0        0        0     1357 2023-12-16 03:56:24.000000 mns-scheduler-1.0.5.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 15:10:53.390763 mns-scheduler-1.0.5.5/mns_scheduler/
--rw-rw-rw-   0        0        0      165 2024-05-20 12:48:16.000000 mns-scheduler-1.0.5.5/mns_scheduler/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 15:10:53.392757 mns-scheduler-1.0.5.5/mns_scheduler/backup/
--rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.5/mns_scheduler/backup/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 15:10:53.394287 mns-scheduler-1.0.5.5/mns_scheduler/backup/app/
--rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.5/mns_scheduler/backup/app/__init__.py
--rw-rw-rw-   0        0        0     5148 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.5/mns_scheduler/backup/app/ths_new_concept_sync_app.py
-drwxrwxrwx   0        0        0        0 2024-05-23 15:10:53.395790 mns-scheduler-1.0.5.5/mns_scheduler/backup/em/
--rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.5/mns_scheduler/backup/em/__init__.py
--rw-rw-rw-   0        0        0     4992 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.5/mns_scheduler/backup/em/em_new_concept_his_sync.py
--rw-rw-rw-   0        0        0     7083 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.5/mns_scheduler/backup/em/em_new_concept_sync_common_api.py
--rw-rw-rw-   0        0        0     2334 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.5/mns_scheduler/backup/em/em_new_concept_sync_web.py
-drwxrwxrwx   0        0        0        0 2024-05-23 15:10:53.396787 mns-scheduler-1.0.5.5/mns_scheduler/backup/wen_cai/
--rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.5/mns_scheduler/backup/wen_cai/__init__.py
--rw-rw-rw-   0        0        0     1747 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.5/mns_scheduler/backup/wen_cai/wen_cai_concept_sync.py
-drwxrwxrwx   0        0        0        0 2024-05-23 15:10:53.397785 mns-scheduler-1.0.5.5/mns_scheduler/big_deal/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.5/mns_scheduler/big_deal/__init__.py
--rw-rw-rw-   0        0        0     4555 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.5/mns_scheduler/big_deal/ths_big_deal_sync.py
-drwxrwxrwx   0        0        0        0 2024-05-23 15:10:53.400818 mns-scheduler-1.0.5.5/mns_scheduler/company_info/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.5/mns_scheduler/company_info/__init__.py
--rw-rw-rw-   0        0        0    14306 2024-05-17 08:56:50.000000 mns-scheduler-1.0.5.5/mns_scheduler/company_info/company_constant_data.py
--rw-rw-rw-   0        0        0    21598 2024-05-20 14:38:40.000000 mns-scheduler-1.0.5.5/mns_scheduler/company_info/company_info_sync_api.py
--rw-rw-rw-   0        0        0     1993 2024-05-17 07:32:00.000000 mns-scheduler-1.0.5.5/mns_scheduler/company_info/de_list_stock_service.py
-drwxrwxrwx   0        0        0        0 2024-05-23 15:10:53.400818 mns-scheduler-1.0.5.5/mns_scheduler/concept/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.5/mns_scheduler/concept/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 15:10:53.402814 mns-scheduler-1.0.5.5/mns_scheduler/concept/clean/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.5/mns_scheduler/concept/clean/__init__.py
--rw-rw-rw-   0        0        0     4512 2024-05-09 14:49:14.000000 mns-scheduler-1.0.5.5/mns_scheduler/concept/clean/kpl_concept_clean_api.py
--rw-rw-rw-   0        0        0     5907 2024-05-09 07:47:40.000000 mns-scheduler-1.0.5.5/mns_scheduler/concept/clean/ths_concept_clean_api.py
-drwxrwxrwx   0        0        0        0 2024-05-23 15:10:53.402814 mns-scheduler-1.0.5.5/mns_scheduler/concept/ths/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.5/mns_scheduler/concept/ths/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 15:10:53.404809 mns-scheduler-1.0.5.5/mns_scheduler/concept/ths/common/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.5/mns_scheduler/concept/ths/common/__init__.py
--rw-rw-rw-   0        0        0     6724 2024-04-30 12:29:06.000000 mns-scheduler-1.0.5.5/mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py
--rw-rw-rw-   0        0        0     4460 2024-04-30 09:34:23.000000 mns-scheduler-1.0.5.5/mns_scheduler/concept/ths/common/ths_concept_update_common_api.py
-drwxrwxrwx   0        0        0        0 2024-05-23 15:10:53.406335 mns-scheduler-1.0.5.5/mns_scheduler/concept/ths/sync_new_index/
--rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.5/mns_scheduler/concept/ths/sync_new_index/__init__.py
--rw-rw-rw-   0        0        0     5001 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.5/mns_scheduler/concept/ths/sync_new_index/sync_ths_concept_by_ak_api.py
--rw-rw-rw-   0        0        0     3605 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.5/mns_scheduler/concept/ths/sync_new_index/sync_ths_new_concept_by_web_api.py
-drwxrwxrwx   0        0        0        0 2024-05-23 15:10:53.407840 mns-scheduler-1.0.5.5/mns_scheduler/concept/ths/update_concept_info/
--rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.5/mns_scheduler/concept/ths/update_concept_info/__init__.py
--rw-rw-rw-   0        0        0     1928 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.5/mns_scheduler/concept/ths/update_concept_info/sync_one_concept_all_symbols_api.py
--rw-rw-rw-   0        0        0     8764 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.5/mns_scheduler/concept/ths/update_concept_info/sync_one_symbol_all_concepts_api.py
-drwxrwxrwx   0        0        0        0 2024-05-23 15:10:53.409834 mns-scheduler-1.0.5.5/mns_scheduler/db/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.5/mns_scheduler/db/__init__.py
--rw-rw-rw-   0        0        0     3952 2024-05-10 13:05:35.000000 mns-scheduler-1.0.5.5/mns_scheduler/db/col_move_service.py
--rw-rw-rw-   0        0        0      747 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.5/mns_scheduler/db/db_status.py
-drwxrwxrwx   0        0        0        0 2024-05-23 15:10:53.411363 mns-scheduler-1.0.5.5/mns_scheduler/dt/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.5/mns_scheduler/dt/__init__.py
--rw-rw-rw-   0        0        0     3466 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.5/mns_scheduler/dt/stock_dt_pool_sync.py
-drwxrwxrwx   0        0        0        0 2024-05-23 15:10:53.415910 mns-scheduler-1.0.5.5/mns_scheduler/finance/
--rw-rw-rw-   0        0        0      163 2024-05-15 14:37:41.000000 mns-scheduler-1.0.5.5/mns_scheduler/finance/__init__.py
--rw-rw-rw-   0        0        0    19437 2024-05-16 00:08:00.000000 mns-scheduler-1.0.5.5/mns_scheduler/finance/em_financial_asset_liability_sync_service_api.py
--rw-rw-rw-   0        0        0    14145 2024-05-16 00:05:34.000000 mns-scheduler-1.0.5.5/mns_scheduler/finance/em_financial_profit_sync_service_api.py
--rw-rw-rw-   0        0        0     2471 2024-05-16 08:53:00.000000 mns-scheduler-1.0.5.5/mns_scheduler/finance/finance_common_api.py
--rw-rw-rw-   0        0        0    10561 2024-05-16 09:27:25.000000 mns-scheduler-1.0.5.5/mns_scheduler/finance/financial_high_risk_stock_clean_service_api.py
--rw-rw-rw-   0        0        0     5042 2024-05-16 09:27:25.000000 mns-scheduler-1.0.5.5/mns_scheduler/finance/sync_financial_report_service_api.py
-drwxrwxrwx   0        0        0        0 2024-05-23 15:10:53.416937 mns-scheduler-1.0.5.5/mns_scheduler/finance/test/
--rw-rw-rw-   0        0        0      163 2024-05-16 01:05:27.000000 mns-scheduler-1.0.5.5/mns_scheduler/finance/test/__init__.py
--rw-rw-rw-   0        0        0     1304 2024-05-16 06:04:02.000000 mns-scheduler-1.0.5.5/mns_scheduler/finance/test/fix_blask_list.py
-drwxrwxrwx   0        0        0        0 2024-05-23 15:10:53.417969 mns-scheduler-1.0.5.5/mns_scheduler/hk/
--rw-rw-rw-   0        0        0      163 2024-05-16 07:31:10.000000 mns-scheduler-1.0.5.5/mns_scheduler/hk/__init__.py
--rw-rw-rw-   0        0        0     3661 2024-05-17 08:14:15.000000 mns-scheduler-1.0.5.5/mns_scheduler/hk/hk_company_info_sync_service_api.py
-drwxrwxrwx   0        0        0        0 2024-05-23 15:10:53.419002 mns-scheduler-1.0.5.5/mns_scheduler/irm/
--rw-rw-rw-   0        0        0      163 2024-05-20 12:48:16.000000 mns-scheduler-1.0.5.5/mns_scheduler/irm/__init__.py
--rw-rw-rw-   0        0        0     2086 2024-05-21 05:28:39.000000 mns-scheduler-1.0.5.5/mns_scheduler/irm/stock_irm_cninfo_service.py
-drwxrwxrwx   0        0        0        0 2024-05-23 15:10:53.419515 mns-scheduler-1.0.5.5/mns_scheduler/k_line/
--rw-rw-rw-   0        0        0      161 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.5/mns_scheduler/k_line/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 15:10:53.421663 mns-scheduler-1.0.5.5/mns_scheduler/k_line/clean/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.5/mns_scheduler/k_line/clean/__init__.py
--rw-rw-rw-   0        0        0    22262 2024-05-23 09:26:20.000000 mns-scheduler-1.0.5.5/mns_scheduler/k_line/clean/k_line_info_clean_impl.py
--rw-rw-rw-   0        0        0     8118 2024-05-23 15:00:37.000000 mns-scheduler-1.0.5.5/mns_scheduler/k_line/clean/k_line_info_clean_service.py
--rw-rw-rw-   0        0        0     2628 2024-05-23 15:06:42.000000 mns-scheduler-1.0.5.5/mns_scheduler/k_line/clean/recent_hot_stocks_clean_service.py
-drwxrwxrwx   0        0        0        0 2024-05-23 15:10:53.422691 mns-scheduler-1.0.5.5/mns_scheduler/k_line/sync/
--rw-rw-rw-   0        0        0      161 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.5/mns_scheduler/k_line/sync/__init__.py
--rw-rw-rw-   0        0        0     5652 2024-05-11 03:27:17.000000 mns-scheduler-1.0.5.5/mns_scheduler/k_line/sync/daily_week_month_line_sync.py
-drwxrwxrwx   0        0        0        0 2024-05-23 15:10:53.423204 mns-scheduler-1.0.5.5/mns_scheduler/kpl/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.5/mns_scheduler/kpl/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 15:10:53.423720 mns-scheduler-1.0.5.5/mns_scheduler/kpl/selection/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.5/mns_scheduler/kpl/selection/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 15:10:53.425098 mns-scheduler-1.0.5.5/mns_scheduler/kpl/selection/index/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.5/mns_scheduler/kpl/selection/index/__init__.py
--rw-rw-rw-   0        0        0     4748 2024-05-09 13:26:15.000000 mns-scheduler-1.0.5.5/mns_scheduler/kpl/selection/index/sync_best_choose_his_index.py
--rw-rw-rw-   0        0        0     8016 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.5/mns_scheduler/kpl/selection/index/sync_best_choose_index.py
-drwxrwxrwx   0        0        0        0 2024-05-23 15:10:53.426126 mns-scheduler-1.0.5.5/mns_scheduler/kpl/selection/symbol/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.5/mns_scheduler/kpl/selection/symbol/__init__.py
--rw-rw-rw-   0        0        0     4679 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.5/mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py
-drwxrwxrwx   0        0        0        0 2024-05-23 15:10:53.427670 mns-scheduler-1.0.5.5/mns_scheduler/kpl/selection/total/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.5/mns_scheduler/kpl/selection/total/__init__.py
--rw-rw-rw-   0        0        0    10461 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.5/mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py
-drwxrwxrwx   0        0        0        0 2024-05-23 15:10:53.428707 mns-scheduler-1.0.5.5/mns_scheduler/lhb/
--rw-rw-rw-   0        0        0      163 2024-05-22 07:47:25.000000 mns-scheduler-1.0.5.5/mns_scheduler/lhb/__init__.py
--rw-rw-rw-   0        0        0      641 2024-05-22 07:52:36.000000 mns-scheduler-1.0.5.5/mns_scheduler/lhb/stock_lhb_sync_service.py
-drwxrwxrwx   0        0        0        0 2024-05-23 15:10:53.430256 mns-scheduler-1.0.5.5/mns_scheduler/real_time/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.5/mns_scheduler/real_time/__init__.py
--rw-rw-rw-   0        0        0     1066 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.5/mns_scheduler/real_time/realtime_quotes_now_create_db_index.py
--rw-rw-rw-   0        0        0     9165 2024-05-06 01:29:24.000000 mns-scheduler-1.0.5.5/mns_scheduler/real_time/realtime_quotes_now_sync.py
-drwxrwxrwx   0        0        0        0 2024-05-23 15:10:53.432314 mns-scheduler-1.0.5.5/mns_scheduler/risk/
--rw-rw-rw-   0        0        0      163 2024-05-22 07:47:47.000000 mns-scheduler-1.0.5.5/mns_scheduler/risk/__init__.py
--rw-rw-rw-   0        0        0     5086 2024-05-17 13:05:26.000000 mns-scheduler-1.0.5.5/mns_scheduler/risk/register_and_investigate_stock_sync_api.py
--rw-rw-rw-   0        0        0      871 2024-05-18 01:43:32.000000 mns-scheduler-1.0.5.5/mns_scheduler/risk/stock_equity_mortgage_sync_api.py
-drwxrwxrwx   0        0        0        0 2024-05-23 15:10:53.434406 mns-scheduler-1.0.5.5/mns_scheduler/trade/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.5/mns_scheduler/trade/__init__.py
--rw-rw-rw-   0        0        0      377 2024-04-28 03:16:51.000000 mns-scheduler-1.0.5.5/mns_scheduler/trade/auto_ipo_buy_api.py
--rw-rw-rw-   0        0        0     4423 2024-04-28 08:59:05.000000 mns-scheduler-1.0.5.5/mns_scheduler/trade/auto_sell_service_api.py
--rw-rw-rw-   0        0        0     2739 2024-04-28 08:08:30.000000 mns-scheduler-1.0.5.5/mns_scheduler/trade/sync_position_api.py
-drwxrwxrwx   0        0        0        0 2024-05-23 15:10:53.435957 mns-scheduler-1.0.5.5/mns_scheduler/zb/
--rw-rw-rw-   0        0        0      165 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.5/mns_scheduler/zb/__init__.py
--rw-rw-rw-   0        0        0     1936 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.5/mns_scheduler/zb/stock_zb_pool_sync.py
-drwxrwxrwx   0        0        0        0 2024-05-23 15:10:53.439548 mns-scheduler-1.0.5.5/mns_scheduler/zt/
--rw-rw-rw-   0        0        0     1641 2024-05-22 03:34:21.000000 mns-scheduler-1.0.5.5/mns_scheduler/zt/__init__.py
--rw-rw-rw-   0        0        0     4015 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.5/mns_scheduler/zt/export_open_data_to_excel.py
--rw-rw-rw-   0        0        0    17525 2024-05-21 15:36:02.000000 mns-scheduler-1.0.5.5/mns_scheduler/zt/realtime_quotes_now_zt_kc_sync.py
--rw-rw-rw-   0        0        0    21283 2024-05-17 08:14:54.000000 mns-scheduler-1.0.5.5/mns_scheduler/zt/today_high_chg_pool_sync_api.py
--rw-rw-rw-   0        0        0    10916 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.5/mns_scheduler/zt/zt_five_boards_sync_api.py
--rw-rw-rw-   0        0        0     7604 2024-05-18 00:16:23.000000 mns-scheduler-1.0.5.5/mns_scheduler/zt/zt_pool_sync_api.py
-drwxrwxrwx   0        0        0        0 2024-05-23 15:10:53.441085 mns-scheduler-1.0.5.5/mns_scheduler/zz_task/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.5/mns_scheduler/zz_task/__init__.py
--rw-rw-rw-   0        0        0    16262 2024-05-18 00:16:23.000000 mns-scheduler-1.0.5.5/mns_scheduler/zz_task/data_sync_task.py
--rw-rw-rw-   0        0        0      932 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.5/mns_scheduler/zz_task/sync_realtime_quotes_task.py
-drwxrwxrwx   0        0        0        0 2024-05-23 15:10:53.441602 mns-scheduler-1.0.5.5/mns_scheduler.egg-info/
--rw-rw-rw-   0        0        0       62 2024-05-23 15:10:53.000000 mns-scheduler-1.0.5.5/mns_scheduler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4215 2024-05-23 15:10:53.000000 mns-scheduler-1.0.5.5/mns_scheduler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 15:10:53.000000 mns-scheduler-1.0.5.5/mns_scheduler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-05-23 15:10:53.000000 mns-scheduler-1.0.5.5/mns_scheduler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-23 15:10:53.442115 mns-scheduler-1.0.5.5/setup.cfg
--rw-rw-rw-   0        0        0      212 2024-05-23 15:10:27.000000 mns-scheduler-1.0.5.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:11.516172 mns-scheduler-1.0.5.6/
+-rw-rw-rw-   0        0        0       62 2024-05-24 15:37:11.515175 mns-scheduler-1.0.5.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1357 2023-12-16 03:56:24.000000 mns-scheduler-1.0.5.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:11.470295 mns-scheduler-1.0.5.6/mns_scheduler/
+-rw-rw-rw-   0        0        0      165 2024-05-20 12:48:16.000000 mns-scheduler-1.0.5.6/mns_scheduler/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:11.472289 mns-scheduler-1.0.5.6/mns_scheduler/backup/
+-rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.6/mns_scheduler/backup/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:11.473287 mns-scheduler-1.0.5.6/mns_scheduler/backup/app/
+-rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.6/mns_scheduler/backup/app/__init__.py
+-rw-rw-rw-   0        0        0     5148 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.6/mns_scheduler/backup/app/ths_new_concept_sync_app.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:11.475281 mns-scheduler-1.0.5.6/mns_scheduler/backup/em/
+-rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.6/mns_scheduler/backup/em/__init__.py
+-rw-rw-rw-   0        0        0     4992 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.6/mns_scheduler/backup/em/em_new_concept_his_sync.py
+-rw-rw-rw-   0        0        0     7083 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.6/mns_scheduler/backup/em/em_new_concept_sync_common_api.py
+-rw-rw-rw-   0        0        0     2334 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.6/mns_scheduler/backup/em/em_new_concept_sync_web.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:11.476399 mns-scheduler-1.0.5.6/mns_scheduler/backup/wen_cai/
+-rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.6/mns_scheduler/backup/wen_cai/__init__.py
+-rw-rw-rw-   0        0        0     1747 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.6/mns_scheduler/backup/wen_cai/wen_cai_concept_sync.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:11.477276 mns-scheduler-1.0.5.6/mns_scheduler/big_deal/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.6/mns_scheduler/big_deal/__init__.py
+-rw-rw-rw-   0        0        0     4555 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.6/mns_scheduler/big_deal/ths_big_deal_sync.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:11.479271 mns-scheduler-1.0.5.6/mns_scheduler/company_info/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.6/mns_scheduler/company_info/__init__.py
+-rw-rw-rw-   0        0        0    14306 2024-05-17 08:56:50.000000 mns-scheduler-1.0.5.6/mns_scheduler/company_info/company_constant_data.py
+-rw-rw-rw-   0        0        0    22727 2024-05-24 07:13:02.000000 mns-scheduler-1.0.5.6/mns_scheduler/company_info/company_info_sync_api.py
+-rw-rw-rw-   0        0        0     1993 2024-05-17 07:32:00.000000 mns-scheduler-1.0.5.6/mns_scheduler/company_info/de_list_stock_service.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:11.479271 mns-scheduler-1.0.5.6/mns_scheduler/concept/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.6/mns_scheduler/concept/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:11.481265 mns-scheduler-1.0.5.6/mns_scheduler/concept/clean/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.6/mns_scheduler/concept/clean/__init__.py
+-rw-rw-rw-   0        0        0     4512 2024-05-09 14:49:14.000000 mns-scheduler-1.0.5.6/mns_scheduler/concept/clean/kpl_concept_clean_api.py
+-rw-rw-rw-   0        0        0     5907 2024-05-09 07:47:40.000000 mns-scheduler-1.0.5.6/mns_scheduler/concept/clean/ths_concept_clean_api.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:11.481265 mns-scheduler-1.0.5.6/mns_scheduler/concept/ths/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.6/mns_scheduler/concept/ths/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:11.483260 mns-scheduler-1.0.5.6/mns_scheduler/concept/ths/common/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.6/mns_scheduler/concept/ths/common/__init__.py
+-rw-rw-rw-   0        0        0     6724 2024-04-30 12:29:06.000000 mns-scheduler-1.0.5.6/mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py
+-rw-rw-rw-   0        0        0     4460 2024-04-30 09:34:23.000000 mns-scheduler-1.0.5.6/mns_scheduler/concept/ths/common/ths_concept_update_common_api.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:11.484258 mns-scheduler-1.0.5.6/mns_scheduler/concept/ths/sync_new_index/
+-rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.6/mns_scheduler/concept/ths/sync_new_index/__init__.py
+-rw-rw-rw-   0        0        0     5001 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.6/mns_scheduler/concept/ths/sync_new_index/sync_ths_concept_by_ak_api.py
+-rw-rw-rw-   0        0        0     3605 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.6/mns_scheduler/concept/ths/sync_new_index/sync_ths_new_concept_by_web_api.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:11.486252 mns-scheduler-1.0.5.6/mns_scheduler/concept/ths/update_concept_info/
+-rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.6/mns_scheduler/concept/ths/update_concept_info/__init__.py
+-rw-rw-rw-   0        0        0     1928 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.6/mns_scheduler/concept/ths/update_concept_info/sync_one_concept_all_symbols_api.py
+-rw-rw-rw-   0        0        0     8764 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.6/mns_scheduler/concept/ths/update_concept_info/sync_one_symbol_all_concepts_api.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:11.487249 mns-scheduler-1.0.5.6/mns_scheduler/db/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.6/mns_scheduler/db/__init__.py
+-rw-rw-rw-   0        0        0     3952 2024-05-10 13:05:35.000000 mns-scheduler-1.0.5.6/mns_scheduler/db/col_move_service.py
+-rw-rw-rw-   0        0        0      747 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.6/mns_scheduler/db/db_status.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:11.488247 mns-scheduler-1.0.5.6/mns_scheduler/dt/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.6/mns_scheduler/dt/__init__.py
+-rw-rw-rw-   0        0        0     3466 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.6/mns_scheduler/dt/stock_dt_pool_sync.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:11.491239 mns-scheduler-1.0.5.6/mns_scheduler/finance/
+-rw-rw-rw-   0        0        0      163 2024-05-15 14:37:41.000000 mns-scheduler-1.0.5.6/mns_scheduler/finance/__init__.py
+-rw-rw-rw-   0        0        0    19437 2024-05-16 00:08:00.000000 mns-scheduler-1.0.5.6/mns_scheduler/finance/em_financial_asset_liability_sync_service_api.py
+-rw-rw-rw-   0        0        0    14145 2024-05-16 00:05:34.000000 mns-scheduler-1.0.5.6/mns_scheduler/finance/em_financial_profit_sync_service_api.py
+-rw-rw-rw-   0        0        0     2471 2024-05-16 08:53:00.000000 mns-scheduler-1.0.5.6/mns_scheduler/finance/finance_common_api.py
+-rw-rw-rw-   0        0        0    10561 2024-05-16 09:27:25.000000 mns-scheduler-1.0.5.6/mns_scheduler/finance/financial_high_risk_stock_clean_service_api.py
+-rw-rw-rw-   0        0        0     5042 2024-05-16 09:27:25.000000 mns-scheduler-1.0.5.6/mns_scheduler/finance/sync_financial_report_service_api.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:11.492236 mns-scheduler-1.0.5.6/mns_scheduler/finance/test/
+-rw-rw-rw-   0        0        0      163 2024-05-16 01:05:27.000000 mns-scheduler-1.0.5.6/mns_scheduler/finance/test/__init__.py
+-rw-rw-rw-   0        0        0     1304 2024-05-16 06:04:02.000000 mns-scheduler-1.0.5.6/mns_scheduler/finance/test/fix_blask_list.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:11.493234 mns-scheduler-1.0.5.6/mns_scheduler/hk/
+-rw-rw-rw-   0        0        0      163 2024-05-16 07:31:10.000000 mns-scheduler-1.0.5.6/mns_scheduler/hk/__init__.py
+-rw-rw-rw-   0        0        0     3661 2024-05-17 08:14:15.000000 mns-scheduler-1.0.5.6/mns_scheduler/hk/hk_company_info_sync_service_api.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:11.494231 mns-scheduler-1.0.5.6/mns_scheduler/irm/
+-rw-rw-rw-   0        0        0      163 2024-05-20 12:48:16.000000 mns-scheduler-1.0.5.6/mns_scheduler/irm/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:11.495228 mns-scheduler-1.0.5.6/mns_scheduler/irm/api/
+-rw-rw-rw-   0        0        0      163 2024-05-24 14:59:41.000000 mns-scheduler-1.0.5.6/mns_scheduler/irm/api/__init__.py
+-rw-rw-rw-   0        0        0     4458 2024-05-24 14:51:26.000000 mns-scheduler-1.0.5.6/mns_scheduler/irm/api/sh_stock_sns_sse_info_api.py
+-rw-rw-rw-   0        0        0     6169 2024-05-24 15:02:16.000000 mns-scheduler-1.0.5.6/mns_scheduler/irm/api/sz_stock_sns_sse_info_api.py
+-rw-rw-rw-   0        0        0     7110 2024-05-24 15:24:42.000000 mns-scheduler-1.0.5.6/mns_scheduler/irm/stock_irm_cninfo_service.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:11.496225 mns-scheduler-1.0.5.6/mns_scheduler/k_line/
+-rw-rw-rw-   0        0        0      161 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.6/mns_scheduler/k_line/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:11.498220 mns-scheduler-1.0.5.6/mns_scheduler/k_line/clean/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.6/mns_scheduler/k_line/clean/__init__.py
+-rw-rw-rw-   0        0        0    22262 2024-05-23 09:26:20.000000 mns-scheduler-1.0.5.6/mns_scheduler/k_line/clean/k_line_info_clean_impl.py
+-rw-rw-rw-   0        0        0     8118 2024-05-23 15:00:37.000000 mns-scheduler-1.0.5.6/mns_scheduler/k_line/clean/k_line_info_clean_service.py
+-rw-rw-rw-   0        0        0     2628 2024-05-23 15:06:42.000000 mns-scheduler-1.0.5.6/mns_scheduler/k_line/clean/recent_hot_stocks_clean_service.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:11.499217 mns-scheduler-1.0.5.6/mns_scheduler/k_line/sync/
+-rw-rw-rw-   0        0        0      161 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.6/mns_scheduler/k_line/sync/__init__.py
+-rw-rw-rw-   0        0        0     5652 2024-05-11 03:27:17.000000 mns-scheduler-1.0.5.6/mns_scheduler/k_line/sync/daily_week_month_line_sync.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:11.499217 mns-scheduler-1.0.5.6/mns_scheduler/kpl/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.6/mns_scheduler/kpl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:11.500215 mns-scheduler-1.0.5.6/mns_scheduler/kpl/selection/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.6/mns_scheduler/kpl/selection/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:11.501212 mns-scheduler-1.0.5.6/mns_scheduler/kpl/selection/index/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.6/mns_scheduler/kpl/selection/index/__init__.py
+-rw-rw-rw-   0        0        0     4748 2024-05-09 13:26:15.000000 mns-scheduler-1.0.5.6/mns_scheduler/kpl/selection/index/sync_best_choose_his_index.py
+-rw-rw-rw-   0        0        0     8016 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.6/mns_scheduler/kpl/selection/index/sync_best_choose_index.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:11.502210 mns-scheduler-1.0.5.6/mns_scheduler/kpl/selection/symbol/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.6/mns_scheduler/kpl/selection/symbol/__init__.py
+-rw-rw-rw-   0        0        0     4679 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.6/mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:11.503207 mns-scheduler-1.0.5.6/mns_scheduler/kpl/selection/total/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.6/mns_scheduler/kpl/selection/total/__init__.py
+-rw-rw-rw-   0        0        0    10461 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.6/mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:11.504204 mns-scheduler-1.0.5.6/mns_scheduler/lhb/
+-rw-rw-rw-   0        0        0      163 2024-05-22 07:47:25.000000 mns-scheduler-1.0.5.6/mns_scheduler/lhb/__init__.py
+-rw-rw-rw-   0        0        0      641 2024-05-22 07:52:36.000000 mns-scheduler-1.0.5.6/mns_scheduler/lhb/stock_lhb_sync_service.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:11.505202 mns-scheduler-1.0.5.6/mns_scheduler/real_time/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.6/mns_scheduler/real_time/__init__.py
+-rw-rw-rw-   0        0        0     1066 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.6/mns_scheduler/real_time/realtime_quotes_now_create_db_index.py
+-rw-rw-rw-   0        0        0     9165 2024-05-06 01:29:24.000000 mns-scheduler-1.0.5.6/mns_scheduler/real_time/realtime_quotes_now_sync.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:11.507196 mns-scheduler-1.0.5.6/mns_scheduler/risk/
+-rw-rw-rw-   0        0        0      163 2024-05-22 07:47:47.000000 mns-scheduler-1.0.5.6/mns_scheduler/risk/__init__.py
+-rw-rw-rw-   0        0        0     5086 2024-05-17 13:05:26.000000 mns-scheduler-1.0.5.6/mns_scheduler/risk/register_and_investigate_stock_sync_api.py
+-rw-rw-rw-   0        0        0      871 2024-05-18 01:43:32.000000 mns-scheduler-1.0.5.6/mns_scheduler/risk/stock_equity_mortgage_sync_api.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:11.509191 mns-scheduler-1.0.5.6/mns_scheduler/trade/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.6/mns_scheduler/trade/__init__.py
+-rw-rw-rw-   0        0        0      377 2024-04-28 03:16:51.000000 mns-scheduler-1.0.5.6/mns_scheduler/trade/auto_ipo_buy_api.py
+-rw-rw-rw-   0        0        0     4423 2024-04-28 08:59:05.000000 mns-scheduler-1.0.5.6/mns_scheduler/trade/auto_sell_service_api.py
+-rw-rw-rw-   0        0        0     2739 2024-04-28 08:08:30.000000 mns-scheduler-1.0.5.6/mns_scheduler/trade/sync_position_api.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:11.510188 mns-scheduler-1.0.5.6/mns_scheduler/zb/
+-rw-rw-rw-   0        0        0      165 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.6/mns_scheduler/zb/__init__.py
+-rw-rw-rw-   0        0        0     1936 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.6/mns_scheduler/zb/stock_zb_pool_sync.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:11.513180 mns-scheduler-1.0.5.6/mns_scheduler/zt/
+-rw-rw-rw-   0        0        0     1641 2024-05-22 03:34:21.000000 mns-scheduler-1.0.5.6/mns_scheduler/zt/__init__.py
+-rw-rw-rw-   0        0        0     4015 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.6/mns_scheduler/zt/export_open_data_to_excel.py
+-rw-rw-rw-   0        0        0    17525 2024-05-21 15:36:02.000000 mns-scheduler-1.0.5.6/mns_scheduler/zt/realtime_quotes_now_zt_kc_sync.py
+-rw-rw-rw-   0        0        0    21283 2024-05-17 08:14:54.000000 mns-scheduler-1.0.5.6/mns_scheduler/zt/today_high_chg_pool_sync_api.py
+-rw-rw-rw-   0        0        0    10916 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.6/mns_scheduler/zt/zt_five_boards_sync_api.py
+-rw-rw-rw-   0        0        0     7604 2024-05-18 00:16:23.000000 mns-scheduler-1.0.5.6/mns_scheduler/zt/zt_pool_sync_api.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:11.514177 mns-scheduler-1.0.5.6/mns_scheduler/zz_task/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.6/mns_scheduler/zz_task/__init__.py
+-rw-rw-rw-   0        0        0    16629 2024-05-24 15:31:54.000000 mns-scheduler-1.0.5.6/mns_scheduler/zz_task/data_sync_task.py
+-rw-rw-rw-   0        0        0      932 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.6/mns_scheduler/zz_task/sync_realtime_quotes_task.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:11.515175 mns-scheduler-1.0.5.6/mns_scheduler.egg-info/
+-rw-rw-rw-   0        0        0       62 2024-05-24 15:37:11.000000 mns-scheduler-1.0.5.6/mns_scheduler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4351 2024-05-24 15:37:11.000000 mns-scheduler-1.0.5.6/mns_scheduler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 15:37:11.000000 mns-scheduler-1.0.5.6/mns_scheduler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-24 15:37:11.000000 mns-scheduler-1.0.5.6/mns_scheduler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-24 15:37:11.516172 mns-scheduler-1.0.5.6/setup.cfg
+-rw-rw-rw-   0        0        0      212 2024-05-24 15:36:33.000000 mns-scheduler-1.0.5.6/setup.py
```

### Comparing `mns-scheduler-1.0.5.5/README.md` & `mns-scheduler-1.0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.5/mns_scheduler/backup/app/ths_new_concept_sync_app.py` & `mns-scheduler-1.0.5.6/mns_scheduler/backup/app/ths_new_concept_sync_app.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.5/mns_scheduler/backup/em/em_new_concept_his_sync.py` & `mns-scheduler-1.0.5.6/mns_scheduler/backup/em/em_new_concept_his_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.5/mns_scheduler/backup/em/em_new_concept_sync_common_api.py` & `mns-scheduler-1.0.5.6/mns_scheduler/backup/em/em_new_concept_sync_common_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.5/mns_scheduler/backup/em/em_new_concept_sync_web.py` & `mns-scheduler-1.0.5.6/mns_scheduler/backup/em/em_new_concept_sync_web.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.5/mns_scheduler/backup/wen_cai/wen_cai_concept_sync.py` & `mns-scheduler-1.0.5.6/mns_scheduler/backup/wen_cai/wen_cai_concept_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.5/mns_scheduler/big_deal/ths_big_deal_sync.py` & `mns-scheduler-1.0.5.6/mns_scheduler/big_deal/ths_big_deal_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.5/mns_scheduler/company_info/company_constant_data.py` & `mns-scheduler-1.0.5.6/mns_scheduler/company_info/company_constant_data.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.5/mns_scheduler/company_info/company_info_sync_api.py` & `mns-scheduler-1.0.5.6/mns_scheduler/company_info/company_info_sync_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 import mns_common.component.common_service_fun_api as common_service_fun_api
 import mns_common.component.concept.ths_concept_common_service_api as ths_concept_common_service_api
 from mns_common.db.MongodbUtil import MongodbUtil
 import mns_common.api.kpl.symbol.kpl_real_time_quotes_api as kpl_real_time_quotes_api
 import mns_common.utils.data_frame_util as data_frame_util
 import mns_common.api.kpl.constant.kpl_constant as kpl_constant
 import mns_common.component.company.company_common_service_api as company_common_service_api
-import mns_common.constant.db_name_constant as db_name_constant
 import mns_common.component.k_line.common.k_line_common_service_api as k_line_common_service_api
+import mns_common.constant.db_name_constant as db_name_constant
 
 mongodb_util = MongodbUtil('27017')
 # 分页大小
 MAX_PAGE_NUMBER = 6000
 import threading
 
 # 定义一个全局锁，用于保护 result 变量的访问
@@ -101,15 +101,17 @@
         "market_id",
         "symbol",
         "amount",
         "sync_date",
         "ths_concept_list_info",
         "kpl_plate_name",
         "kpl_most_relative_name",
-        "kpl_plate_list_info"
+        "kpl_plate_list_info",
+        'operate_profit',
+        'total_operate_income'
     ]]
 
 
 def get_east_money_stock_info():
     all_real_time_quotes = east_money_stock_v2_api.get_all_real_time_quotes()
     all_real_time_quotes = all_real_time_quotes[['symbol',
                                                  'name',
@@ -328,14 +330,17 @@
             company_info_type['kpl_plate_list_info'] = '-'
             company_info_type['kpl_plate_name'] = '-'
             company_info_type['kpl_most_relative_name'] = '-'
             now_date = datetime.now()
             str_day = now_date.strftime('%Y-%m-%d')
             deal_days = k_line_common_service_api.get_deal_days(str_day, company_one.symbol)
             company_info_type['deal_days'] = deal_days
+            # 设置年报信息
+            company_info_type = get_recent_year_income(company_one.symbol, company_info_type)
+
             try:
                 if data_frame_util.is_not_empty(kpl_real_time_quotes):
                     kpl_real_time_quotes_one = kpl_real_time_quotes.loc[
                         kpl_real_time_quotes['symbol'] == company_one.symbol]
 
                     if data_frame_util.is_not_empty(kpl_real_time_quotes_one):
                         company_info_type['kpl_plate_name'] = list(kpl_real_time_quotes_one['plate_name_list'])[0]
@@ -476,14 +481,31 @@
         'second_sw_industry',
         'third_industry_code',
         'third_sw_industry'
     ]]
     mongodb_util.save_mongo(third_sw_info, 'sw_industry')
 
 
+# 获取最近年报收入
+def get_recent_year_income(symbol, company_info_type):
+    query = {'symbol': symbol, "REPORT_TYPE": "年报"}
+    em_stock_profit = mongodb_util.descend_query(query, db_name_constant.EM_STOCK_PROFIT, 'REPORT_DATE', 1)
+    if data_frame_util.is_not_empty(em_stock_profit):
+        company_info_type['operate_profit'] = list(em_stock_profit['OPERATE_PROFIT'])[0]
+        company_info_type['total_operate_income'] = list(em_stock_profit['TOTAL_OPERATE_INCOME'])[0]
+    else:
+        company_info_type['operate_profit'] = 0
+        company_info_type['total_operate_income'] = 0
+    company_info_type['operate_profit'] = round(
+        company_info_type['operate_profit'] / common_service_fun_api.HUNDRED_MILLION, 2)
+    company_info_type['total_operate_income'] = round(
+        company_info_type['total_operate_income'] / common_service_fun_api.HUNDRED_MILLION, 2)
+    return company_info_type
+
+
 if __name__ == '__main__':
     # while True:
     #     df = ths_stock_api.get_company_info_detail('000001')
     #     print(df)
     # company_info_update()
     # company_info_type = ths_stock_api.get_company_info_detail('836699')
     # sync_company_base_info()
```

### Comparing `mns-scheduler-1.0.5.5/mns_scheduler/company_info/de_list_stock_service.py` & `mns-scheduler-1.0.5.6/mns_scheduler/company_info/de_list_stock_service.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.5/mns_scheduler/concept/clean/kpl_concept_clean_api.py` & `mns-scheduler-1.0.5.6/mns_scheduler/concept/clean/kpl_concept_clean_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.5/mns_scheduler/concept/clean/ths_concept_clean_api.py` & `mns-scheduler-1.0.5.6/mns_scheduler/concept/clean/ths_concept_clean_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.5/mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py` & `mns-scheduler-1.0.5.6/mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.5/mns_scheduler/concept/ths/common/ths_concept_update_common_api.py` & `mns-scheduler-1.0.5.6/mns_scheduler/concept/ths/common/ths_concept_update_common_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.5/mns_scheduler/concept/ths/sync_new_index/sync_ths_concept_by_ak_api.py` & `mns-scheduler-1.0.5.6/mns_scheduler/concept/ths/sync_new_index/sync_ths_concept_by_ak_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.5/mns_scheduler/concept/ths/sync_new_index/sync_ths_new_concept_by_web_api.py` & `mns-scheduler-1.0.5.6/mns_scheduler/concept/ths/sync_new_index/sync_ths_new_concept_by_web_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.5/mns_scheduler/concept/ths/update_concept_info/sync_one_concept_all_symbols_api.py` & `mns-scheduler-1.0.5.6/mns_scheduler/concept/ths/update_concept_info/sync_one_concept_all_symbols_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.5/mns_scheduler/concept/ths/update_concept_info/sync_one_symbol_all_concepts_api.py` & `mns-scheduler-1.0.5.6/mns_scheduler/concept/ths/update_concept_info/sync_one_symbol_all_concepts_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.5/mns_scheduler/db/col_move_service.py` & `mns-scheduler-1.0.5.6/mns_scheduler/db/col_move_service.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.5/mns_scheduler/db/db_status.py` & `mns-scheduler-1.0.5.6/mns_scheduler/db/db_status.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.5/mns_scheduler/dt/stock_dt_pool_sync.py` & `mns-scheduler-1.0.5.6/mns_scheduler/dt/stock_dt_pool_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.5/mns_scheduler/finance/em_financial_asset_liability_sync_service_api.py` & `mns-scheduler-1.0.5.6/mns_scheduler/finance/em_financial_asset_liability_sync_service_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.5/mns_scheduler/finance/em_financial_profit_sync_service_api.py` & `mns-scheduler-1.0.5.6/mns_scheduler/finance/em_financial_profit_sync_service_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.5/mns_scheduler/finance/finance_common_api.py` & `mns-scheduler-1.0.5.6/mns_scheduler/finance/finance_common_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.5/mns_scheduler/finance/financial_high_risk_stock_clean_service_api.py` & `mns-scheduler-1.0.5.6/mns_scheduler/finance/financial_high_risk_stock_clean_service_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.5/mns_scheduler/finance/sync_financial_report_service_api.py` & `mns-scheduler-1.0.5.6/mns_scheduler/finance/sync_financial_report_service_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.5/mns_scheduler/finance/test/fix_blask_list.py` & `mns-scheduler-1.0.5.6/mns_scheduler/finance/test/fix_blask_list.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.5/mns_scheduler/hk/hk_company_info_sync_service_api.py` & `mns-scheduler-1.0.5.6/mns_scheduler/hk/hk_company_info_sync_service_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.5/mns_scheduler/k_line/clean/k_line_info_clean_impl.py` & `mns-scheduler-1.0.5.6/mns_scheduler/k_line/clean/k_line_info_clean_impl.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.5/mns_scheduler/k_line/clean/k_line_info_clean_service.py` & `mns-scheduler-1.0.5.6/mns_scheduler/k_line/clean/k_line_info_clean_service.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.5/mns_scheduler/k_line/clean/recent_hot_stocks_clean_service.py` & `mns-scheduler-1.0.5.6/mns_scheduler/k_line/clean/recent_hot_stocks_clean_service.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.5/mns_scheduler/k_line/sync/daily_week_month_line_sync.py` & `mns-scheduler-1.0.5.6/mns_scheduler/k_line/sync/daily_week_month_line_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.5/mns_scheduler/kpl/selection/index/sync_best_choose_his_index.py` & `mns-scheduler-1.0.5.6/mns_scheduler/kpl/selection/index/sync_best_choose_his_index.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.5/mns_scheduler/kpl/selection/index/sync_best_choose_index.py` & `mns-scheduler-1.0.5.6/mns_scheduler/kpl/selection/index/sync_best_choose_index.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.5/mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py` & `mns-scheduler-1.0.5.6/mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.5/mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py` & `mns-scheduler-1.0.5.6/mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.5/mns_scheduler/lhb/stock_lhb_sync_service.py` & `mns-scheduler-1.0.5.6/mns_scheduler/lhb/stock_lhb_sync_service.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.5/mns_scheduler/real_time/realtime_quotes_now_create_db_index.py` & `mns-scheduler-1.0.5.6/mns_scheduler/real_time/realtime_quotes_now_create_db_index.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.5/mns_scheduler/real_time/realtime_quotes_now_sync.py` & `mns-scheduler-1.0.5.6/mns_scheduler/real_time/realtime_quotes_now_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.5/mns_scheduler/risk/register_and_investigate_stock_sync_api.py` & `mns-scheduler-1.0.5.6/mns_scheduler/risk/register_and_investigate_stock_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.5/mns_scheduler/risk/stock_equity_mortgage_sync_api.py` & `mns-scheduler-1.0.5.6/mns_scheduler/risk/stock_equity_mortgage_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.5/mns_scheduler/trade/auto_sell_service_api.py` & `mns-scheduler-1.0.5.6/mns_scheduler/trade/auto_sell_service_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.5/mns_scheduler/trade/sync_position_api.py` & `mns-scheduler-1.0.5.6/mns_scheduler/trade/sync_position_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.5/mns_scheduler/zb/stock_zb_pool_sync.py` & `mns-scheduler-1.0.5.6/mns_scheduler/zb/stock_zb_pool_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.5/mns_scheduler/zt/__init__.py` & `mns-scheduler-1.0.5.6/mns_scheduler/zt/__init__.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.5/mns_scheduler/zt/export_open_data_to_excel.py` & `mns-scheduler-1.0.5.6/mns_scheduler/zt/export_open_data_to_excel.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.5/mns_scheduler/zt/realtime_quotes_now_zt_kc_sync.py` & `mns-scheduler-1.0.5.6/mns_scheduler/zt/realtime_quotes_now_zt_kc_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.5/mns_scheduler/zt/today_high_chg_pool_sync_api.py` & `mns-scheduler-1.0.5.6/mns_scheduler/zt/today_high_chg_pool_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.5/mns_scheduler/zt/zt_five_boards_sync_api.py` & `mns-scheduler-1.0.5.6/mns_scheduler/zt/zt_five_boards_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.5/mns_scheduler/zt/zt_pool_sync_api.py` & `mns-scheduler-1.0.5.6/mns_scheduler/zt/zt_pool_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.5/mns_scheduler/zz_task/data_sync_task.py` & `mns-scheduler-1.0.5.6/mns_scheduler/zz_task/data_sync_task.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 import mns_scheduler.company_info.company_info_sync_api as company_info_sync_api
 import mns_scheduler.trade.auto_ipo_buy_api as auto_ipo_buy_api
 import mns_scheduler.kpl.selection.index.sync_best_choose_his_index as sync_best_choose_his_index
 import mns_scheduler.concept.ths.common.ths_concept_update_common_api as ths_concept_update_common_api
 import mns_scheduler.trade.sync_position_api as sync_position_api
 import mns_scheduler.concept.clean.kpl_concept_clean_api as kpl_concept_clean_api
 import mns_scheduler.company_info.de_list_stock_service as de_list_stock_service
+import mns_scheduler.irm.stock_irm_cninfo_service as stock_irm_cninfo_service
 
 
 # 同步交易日期任务完成
 def sync_trade_date():
     trade_date_common_service_api.sync_trade_date()
     logger.info('同步交易日期任务完成')
 
@@ -318,14 +319,20 @@
 
 # 同步被立案调查的股票
 def sync_new_high_risk_stocks():
     logger.info('同步被立案调查的股票')
     register_and_investigate_stock_sync_api.sync_new_high_risk_stocks()
 
 
+# 同步互动回答
+def sync_all_interactive_questions():
+    logger.info('同步互动回答')
+    stock_irm_cninfo_service.sync_all_interactive_questions()
+
+
 # # 定义BlockingScheduler
 blockingScheduler = BlockingScheduler()
 # sync_trade_date 同步交易日期
 blockingScheduler.add_job(sync_trade_date, 'cron', hour='20', minute='43')
 
 # 跌停信息同步
 blockingScheduler.add_job(sync_stock_dt_pool, 'cron', hour='15,17,21,03,07', minute='37')
@@ -393,12 +400,15 @@
 
 # 更新开盘啦指数关系
 blockingScheduler.add_job(sync_position, 'cron', hour='0,08', minute='10')
 
 # 同步被立案调查的股票
 blockingScheduler.add_job(sync_new_high_risk_stocks, 'cron', hour='0,09,12,16', minute='20')
 
+# 同步互动回答
+blockingScheduler.add_job(sync_all_interactive_questions, 'cron', hour='08,12,17', minute='05')
+
 print('定时任务启动成功')
 blockingScheduler.start()
 #
 # if __name__ == '__main__':
 #     sync_kpl_best_his_quotes()
```

### Comparing `mns-scheduler-1.0.5.5/mns_scheduler/zz_task/sync_realtime_quotes_task.py` & `mns-scheduler-1.0.5.6/mns_scheduler/zz_task/sync_realtime_quotes_task.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.5/mns_scheduler.egg-info/SOURCES.txt` & `mns-scheduler-1.0.5.6/mns_scheduler.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -47,14 +47,17 @@
 mns_scheduler/finance/sync_financial_report_service_api.py
 mns_scheduler/finance/test/__init__.py
 mns_scheduler/finance/test/fix_blask_list.py
 mns_scheduler/hk/__init__.py
 mns_scheduler/hk/hk_company_info_sync_service_api.py
 mns_scheduler/irm/__init__.py
 mns_scheduler/irm/stock_irm_cninfo_service.py
+mns_scheduler/irm/api/__init__.py
+mns_scheduler/irm/api/sh_stock_sns_sse_info_api.py
+mns_scheduler/irm/api/sz_stock_sns_sse_info_api.py
 mns_scheduler/k_line/__init__.py
 mns_scheduler/k_line/clean/__init__.py
 mns_scheduler/k_line/clean/k_line_info_clean_impl.py
 mns_scheduler/k_line/clean/k_line_info_clean_service.py
 mns_scheduler/k_line/clean/recent_hot_stocks_clean_service.py
 mns_scheduler/k_line/sync/__init__.py
 mns_scheduler/k_line/sync/daily_week_month_line_sync.py
```

