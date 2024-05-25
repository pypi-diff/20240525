# Comparing `tmp/qis-2.0.8.tar.gz` & `tmp/qis-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qis-2.0.8.tar", max compression
+gzip compressed data, was "qis-2.0.9.tar", max compression
```

## Comparing `qis-2.0.8.tar` & `qis-2.0.9.tar`

### file list

```diff
@@ -1,111 +1,111 @@
--rw-r--r--   0        0        0    35802 2022-12-30 16:28:55.651210 qis-2.0.8/LICENSE.txt
--rw-r--r--   0        0        0     1838 2023-08-31 16:52:40.478134 qis-2.0.8/pyproject.toml
--rw-r--r--   0        0        0     1026 2023-03-30 08:29:12.943307 qis-2.0.8/qis/__init__.py
--rw-r--r--   0        0        0     8706 2023-07-15 18:49:51.554511 qis-2.0.8/qis/examples/bootstrap_analysis.py
--rw-r--r--   0        0        0     4523 2023-02-04 11:08:31.167705 qis-2.0.8/qis/examples/constant_notional.py
--rw-r--r--   0        0        0     2079 2023-08-17 12:31:20.262771 qis-2.0.8/qis/examples/factsheets/multi_assets.py
--rw-r--r--   0        0        0     5133 2023-08-20 18:07:48.766485 qis-2.0.8/qis/examples/factsheets/multi_strategy.py
--rw-r--r--   0        0        0     7529 2023-08-20 18:07:48.739556 qis-2.0.8/qis/examples/factsheets/strategy.py
--rw-r--r--   0        0        0     5488 2023-08-20 18:07:48.718613 qis-2.0.8/qis/examples/factsheets/strategy_benchmark.py
--rw-r--r--   0        0        0  1639897 2023-07-24 20:18:51.348551 qis-2.0.8/qis/examples/figures/multi_strategy.PNG
--rw-r--r--   0        0        0  2042185 2023-07-24 20:17:18.402937 qis-2.0.8/qis/examples/figures/multiassets.PNG
--rw-r--r--   0        0        0   556557 2023-07-24 20:22:33.955807 qis-2.0.8/qis/examples/figures/perf1.PNG
--rw-r--r--   0        0        0   923410 2023-07-24 20:22:37.524967 qis-2.0.8/qis/examples/figures/perf2.PNG
--rw-r--r--   0        0        0   302247 2023-07-24 20:22:40.795836 qis-2.0.8/qis/examples/figures/perf3.PNG
--rw-r--r--   0        0        0  1104330 2023-07-24 20:20:37.807001 qis-2.0.8/qis/examples/figures/strategy.PNG
--rw-r--r--   0        0        0  1437260 2023-07-24 20:23:16.595060 qis-2.0.8/qis/examples/figures/strategy_benchmark.PNG
--rw-r--r--   0        0        0     4425 2023-07-18 20:07:51.000000 qis-2.0.8/qis/examples/ohlc_vol_analysis.py
--rw-r--r--   0        0        0     1793 2023-07-24 20:22:27.175189 qis-2.0.8/qis/examples/performances.py
--rw-r--r--   0        0        0     6183 2023-06-07 13:05:39.000000 qis-2.0.8/qis/examples/price_plots.py
--rw-r--r--   0        0        0    11025 2023-06-22 07:47:30.271035 qis-2.0.8/qis/examples/simulate_quant_strats.py
--rw-r--r--   0        0        0     8041 2023-04-04 08:32:09.000000 qis-2.0.8/qis/examples/test_ewm.py
--rw-r--r--   0        0        0     1599 2023-01-22 21:54:41.000000 qis-2.0.8/qis/examples/test_scatter.py
--rw-r--r--   0        0        0     7071 2023-07-08 08:12:25.236850 qis-2.0.8/qis/examples/try_pybloqs.py
--rw-r--r--   0        0        0    35252 2023-08-16 12:07:46.000000 qis-2.0.8/qis/file_utils.py
--rw-r--r--   0        0        0      991 2023-01-15 20:14:44.057860 qis-2.0.8/qis/local_path.py
--rw-r--r--   0        0        0     2105 2023-08-11 09:02:07.000000 qis-2.0.8/qis/models/__init__.py
--rw-r--r--   0        0        0        0 2021-05-21 09:42:40.000000 qis-2.0.8/qis/models/linear/__init__.py
--rw-r--r--   0        0        0     5515 2023-07-15 12:28:57.386631 qis-2.0.8/qis/models/linear/auto_corr.py
--rw-r--r--   0        0        0     8838 2023-08-11 10:33:45.000000 qis-2.0.8/qis/models/linear/corr_cov_matrix.py
--rw-r--r--   0        0        0    41126 2023-08-14 14:25:43.000000 qis-2.0.8/qis/models/linear/ewm.py
--rw-r--r--   0        0        0     3620 2023-02-18 22:06:06.000000 qis-2.0.8/qis/models/linear/ewm_convolution.py
--rw-r--r--   0        0        0     6908 2023-08-14 15:11:32.000000 qis-2.0.8/qis/models/linear/ewm_factors.py
--rw-r--r--   0        0        0     4032 2023-01-23 14:52:48.000000 qis-2.0.8/qis/models/linear/pca.py
--rw-r--r--   0        0        0     7121 2023-08-18 10:10:08.566817 qis-2.0.8/qis/models/linear/plot_correlations.py
--rw-r--r--   0        0        0    11519 2023-07-16 14:22:12.617158 qis-2.0.8/qis/models/linear/ra_returns.py
--rw-r--r--   0        0        0       24 2023-01-23 21:08:28.000000 qis-2.0.8/qis/models/README.md
--rw-r--r--   0        0        0        0 2021-12-04 12:08:05.446837 qis-2.0.8/qis/models/stats/__init__.py
--rw-r--r--   0        0        0    19511 2023-07-16 05:40:45.921919 qis-2.0.8/qis/models/stats/bootstrap.py
--rw-r--r--   0        0        0     2722 2023-07-18 20:08:16.000000 qis-2.0.8/qis/models/stats/ohlc_vol.py
--rw-r--r--   0        0        0     8556 2023-02-18 22:06:11.000000 qis-2.0.8/qis/models/stats/test_bootstrap.py
--rw-r--r--   0        0        0     2450 2023-08-28 12:41:52.000000 qis-2.0.8/qis/perfstats/__init__.py
--rw-r--r--   0        0        0     7178 2023-01-23 14:52:48.000000 qis-2.0.8/qis/perfstats/cond_regression.py
--rw-r--r--   0        0        0    11454 2023-08-17 13:03:26.545127 qis-2.0.8/qis/perfstats/config.py
--rw-r--r--   0        0        0     7287 2023-07-21 13:43:13.664929 qis-2.0.8/qis/perfstats/desc_table.py
--rw-r--r--   0        0        0    21447 2023-06-06 14:51:04.000000 qis-2.0.8/qis/perfstats/perf_stats.py
--rw-r--r--   0        0        0       24 2023-01-23 21:09:51.000000 qis-2.0.8/qis/perfstats/README.md
--rw-r--r--   0        0        0    20183 2023-08-31 15:47:02.000000 qis-2.0.8/qis/perfstats/regime_classifier.py
--rw-r--r--   0        0        0    31925 2023-08-28 12:40:46.000000 qis-2.0.8/qis/perfstats/returns.py
--rw-r--r--   0        0        0     7920 2023-05-12 14:35:19.552286 qis-2.0.8/qis/perfstats/timeseries_bfill.py
--rw-r--r--   0        0        0     3812 2023-05-31 04:27:08.487324 qis-2.0.8/qis/plots/__init__.py
--rw-r--r--   0        0        0    17328 2023-08-31 15:42:28.000000 qis-2.0.8/qis/plots/bars.py
--rw-r--r--   0        0        0    23159 2023-07-15 15:16:40.000000 qis-2.0.8/qis/plots/boxplot.py
--rw-r--r--   0        0        0     3917 2023-02-18 22:06:06.000000 qis-2.0.8/qis/plots/contour.py
--rw-r--r--   0        0        0        0 2021-03-12 13:47:34.000000 qis-2.0.8/qis/plots/derived/__init__.py
--rw-r--r--   0        0        0     2196 2023-01-07 22:34:01.686282 qis-2.0.8/qis/plots/derived/data_timeseries.py
--rw-r--r--   0        0        0     7464 2023-04-23 14:40:57.890091 qis-2.0.8/qis/plots/derived/drawdowns.py
--rw-r--r--   0        0        0    18835 2023-08-18 10:33:59.167827 qis-2.0.8/qis/plots/derived/perf_table.py
--rw-r--r--   0        0        0    22969 2023-06-06 13:07:17.000000 qis-2.0.8/qis/plots/derived/prices.py
--rw-r--r--   0        0        0     3489 2023-02-18 22:06:08.000000 qis-2.0.8/qis/plots/derived/regime_class_table.py
--rw-r--r--   0        0        0    11938 2023-08-31 15:49:22.000000 qis-2.0.8/qis/plots/derived/regime_data.py
--rw-r--r--   0        0        0     3519 2023-02-18 22:06:07.000000 qis-2.0.8/qis/plots/derived/regime_pdf.py
--rw-r--r--   0        0        0     6590 2023-02-18 22:06:08.000000 qis-2.0.8/qis/plots/derived/regime_scatter.py
--rw-r--r--   0        0        0    18010 2023-03-02 12:04:37.000000 qis-2.0.8/qis/plots/derived/returns_heatmap.py
--rw-r--r--   0        0        0     5173 2023-02-18 22:06:08.000000 qis-2.0.8/qis/plots/derived/returns_scatter.py
--rw-r--r--   0        0        0     4008 2023-02-18 22:06:13.000000 qis-2.0.8/qis/plots/errorbar.py
--rw-r--r--   0        0        0     3643 2023-02-18 22:06:09.000000 qis-2.0.8/qis/plots/heatmap.py
--rw-r--r--   0        0        0    11179 2023-08-28 13:10:19.000000 qis-2.0.8/qis/plots/histogram.py
--rw-r--r--   0        0        0     2917 2023-08-11 07:39:51.000000 qis-2.0.8/qis/plots/histplot2d.py
--rw-r--r--   0        0        0     5424 2023-02-18 22:06:07.000000 qis-2.0.8/qis/plots/lineplot.py
--rw-r--r--   0        0        0     1850 2023-03-21 14:30:08.000000 qis-2.0.8/qis/plots/pie.py
--rw-r--r--   0        0        0     5889 2023-02-18 22:06:10.000000 qis-2.0.8/qis/plots/qqplot.py
--rw-r--r--   0        0        0       24 2023-01-23 21:10:18.000000 qis-2.0.8/qis/plots/README.md
--rw-r--r--   0        0        0    15874 2023-03-14 11:00:14.000000 qis-2.0.8/qis/plots/scatter.py
--rw-r--r--   0        0        0     6009 2023-03-21 06:51:44.000000 qis-2.0.8/qis/plots/stackplot.py
--rw-r--r--   0        0        0    14372 2023-08-20 06:31:30.000000 qis-2.0.8/qis/plots/table.py
--rw-r--r--   0        0        0    21512 2023-05-31 09:52:23.000000 qis-2.0.8/qis/plots/time_series.py
--rw-r--r--   0        0        0    57579 2023-08-27 15:00:22.501948 qis-2.0.8/qis/plots/utils.py
--rw-r--r--   0        0        0      706 2023-08-17 13:24:45.103644 qis-2.0.8/qis/portfolio/__init__.py
--rw-r--r--   0        0        0    11646 2023-06-07 09:56:37.000000 qis-2.0.8/qis/portfolio/backtester.py
--rw-r--r--   0        0        0    27546 2023-08-11 09:00:19.000000 qis-2.0.8/qis/portfolio/multi_portfolio_data.py
--rw-r--r--   0        0        0    37213 2023-08-21 14:19:45.000000 qis-2.0.8/qis/portfolio/portfolio_data.py
--rw-r--r--   0        0        0       24 2023-01-23 21:10:46.000000 qis-2.0.8/qis/portfolio/README.md
--rw-r--r--   0        0        0        0 2023-06-22 07:59:37.604630 qis-2.0.8/qis/portfolio/reports/__init__.py
--rw-r--r--   0        0        0     1856 2023-08-18 14:55:48.000000 qis-2.0.8/qis/portfolio/reports/config.py
--rw-r--r--   0        0        0    17513 2023-08-17 12:48:25.650392 qis-2.0.8/qis/portfolio/reports/multi_assets_factsheet.py
--rw-r--r--   0        0        0     7571 2023-07-08 08:11:22.704374 qis-2.0.8/qis/portfolio/reports/multi_strategy_factsheet.py
--rw-r--r--   0        0        0    12549 2023-08-17 13:32:23.968301 qis-2.0.8/qis/portfolio/reports/strategy_benchmark_factsheet.py
--rw-r--r--   0        0        0    11702 2023-08-23 08:38:13.000000 qis-2.0.8/qis/portfolio/reports/strategy_factsheet.py
--rw-r--r--   0        0        0        0 2022-12-17 17:53:19.519118 qis-2.0.8/qis/portfolio/strats/__init__.py
--rw-r--r--   0        0        0     5778 2023-02-18 22:06:12.000000 qis-2.0.8/qis/portfolio/strats/quant_strats_delta1.py
--rw-r--r--   0        0        0      204 2023-08-31 16:52:40.433254 qis-2.0.8/qis/settings.yaml
--rw-r--r--   0        0        0      443 2023-01-15 20:14:44.028937 qis-2.0.8/qis/sql_engine.py
--rw-r--r--   0        0        0     1261 2023-03-02 12:52:25.000000 qis-2.0.8/qis/test_data.py
--rw-r--r--   0        0        0     4779 2023-07-23 06:50:46.389371 qis-2.0.8/qis/utils/__init__.py
--rw-r--r--   0        0        0    42107 2023-08-17 13:24:45.008898 qis-2.0.8/qis/utils/dates.py
--rw-r--r--   0        0        0    11347 2023-06-07 09:35:59.000000 qis-2.0.8/qis/utils/df_agg.py
--rw-r--r--   0        0        0     8491 2023-01-08 13:32:37.792219 qis-2.0.8/qis/utils/df_cut.py
--rw-r--r--   0        0        0     7964 2023-07-28 06:10:47.082310 qis-2.0.8/qis/utils/df_freq.py
--rw-r--r--   0        0        0    10992 2023-02-18 22:06:12.000000 qis-2.0.8/qis/utils/df_groups.py
--rw-r--r--   0        0        0     6819 2023-02-18 22:06:11.000000 qis-2.0.8/qis/utils/df_melt.py
--rw-r--r--   0        0        0    23956 2023-07-02 06:53:30.708901 qis-2.0.8/qis/utils/df_ops.py
--rw-r--r--   0        0        0     8905 2023-02-18 22:06:10.000000 qis-2.0.8/qis/utils/df_str.py
--rw-r--r--   0        0        0    11344 2022-12-30 16:13:34.048573 qis-2.0.8/qis/utils/df_to_weights.py
--rw-r--r--   0        0        0    10640 2023-05-12 08:13:42.291695 qis-2.0.8/qis/utils/generic.py
--rw-r--r--   0        0        0    15848 2023-07-05 08:50:35.000000 qis-2.0.8/qis/utils/np_ops.py
--rw-r--r--   0        0        0     5576 2023-04-04 20:13:54.941670 qis-2.0.8/qis/utils/ols.py
--rw-r--r--   0        0        0       22 2023-01-23 21:14:19.000000 qis-2.0.8/qis/utils/README.md
--rw-r--r--   0        0        0     4589 2023-02-18 22:06:08.000000 qis-2.0.8/qis/utils/sampling.py
--rw-r--r--   0        0        0     5938 2022-12-16 21:08:07.000000 qis-2.0.8/qis/utils/struct_ops.py
--rw-r--r--   0        0        0     9104 2023-08-21 14:55:14.000000 qis-2.0.8/README.md
--rw-r--r--   0        0        0    10890 1970-01-01 00:00:00.000000 qis-2.0.8/PKG-INFO
+-rw-r--r--   0        0        0    35802 2022-12-30 16:28:55.651210 qis-2.0.9/LICENSE.txt
+-rw-r--r--   0        0        0     1838 2023-08-31 17:59:03.432079 qis-2.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1026 2023-03-30 08:29:12.943307 qis-2.0.9/qis/__init__.py
+-rw-r--r--   0        0        0     8706 2023-07-15 18:49:51.554511 qis-2.0.9/qis/examples/bootstrap_analysis.py
+-rw-r--r--   0        0        0     4523 2023-02-04 11:08:31.167705 qis-2.0.9/qis/examples/constant_notional.py
+-rw-r--r--   0        0        0     2079 2023-08-17 12:31:20.262771 qis-2.0.9/qis/examples/factsheets/multi_assets.py
+-rw-r--r--   0        0        0     5133 2023-08-20 18:07:48.766485 qis-2.0.9/qis/examples/factsheets/multi_strategy.py
+-rw-r--r--   0        0        0     7529 2023-08-20 18:07:48.739556 qis-2.0.9/qis/examples/factsheets/strategy.py
+-rw-r--r--   0        0        0     5488 2023-08-20 18:07:48.718613 qis-2.0.9/qis/examples/factsheets/strategy_benchmark.py
+-rw-r--r--   0        0        0  1639897 2023-07-24 20:18:51.348551 qis-2.0.9/qis/examples/figures/multi_strategy.PNG
+-rw-r--r--   0        0        0  2042185 2023-07-24 20:17:18.402937 qis-2.0.9/qis/examples/figures/multiassets.PNG
+-rw-r--r--   0        0        0   556557 2023-07-24 20:22:33.955807 qis-2.0.9/qis/examples/figures/perf1.PNG
+-rw-r--r--   0        0        0   923410 2023-07-24 20:22:37.524967 qis-2.0.9/qis/examples/figures/perf2.PNG
+-rw-r--r--   0        0        0   302247 2023-07-24 20:22:40.795836 qis-2.0.9/qis/examples/figures/perf3.PNG
+-rw-r--r--   0        0        0  1104330 2023-07-24 20:20:37.807001 qis-2.0.9/qis/examples/figures/strategy.PNG
+-rw-r--r--   0        0        0  1437260 2023-07-24 20:23:16.595060 qis-2.0.9/qis/examples/figures/strategy_benchmark.PNG
+-rw-r--r--   0        0        0     4425 2023-07-18 20:07:51.000000 qis-2.0.9/qis/examples/ohlc_vol_analysis.py
+-rw-r--r--   0        0        0     1793 2023-07-24 20:22:27.175189 qis-2.0.9/qis/examples/performances.py
+-rw-r--r--   0        0        0     6183 2023-06-07 13:05:39.000000 qis-2.0.9/qis/examples/price_plots.py
+-rw-r--r--   0        0        0    11025 2023-06-22 07:47:30.271035 qis-2.0.9/qis/examples/simulate_quant_strats.py
+-rw-r--r--   0        0        0     8041 2023-04-04 08:32:09.000000 qis-2.0.9/qis/examples/test_ewm.py
+-rw-r--r--   0        0        0     1599 2023-01-22 21:54:41.000000 qis-2.0.9/qis/examples/test_scatter.py
+-rw-r--r--   0        0        0     7071 2023-07-08 08:12:25.236850 qis-2.0.9/qis/examples/try_pybloqs.py
+-rw-r--r--   0        0        0    35252 2023-08-16 12:07:46.000000 qis-2.0.9/qis/file_utils.py
+-rw-r--r--   0        0        0      991 2023-01-15 20:14:44.057860 qis-2.0.9/qis/local_path.py
+-rw-r--r--   0        0        0     2105 2023-08-11 09:02:07.000000 qis-2.0.9/qis/models/__init__.py
+-rw-r--r--   0        0        0        0 2021-05-21 09:42:40.000000 qis-2.0.9/qis/models/linear/__init__.py
+-rw-r--r--   0        0        0     5515 2023-07-15 12:28:57.386631 qis-2.0.9/qis/models/linear/auto_corr.py
+-rw-r--r--   0        0        0     8838 2023-08-11 10:33:45.000000 qis-2.0.9/qis/models/linear/corr_cov_matrix.py
+-rw-r--r--   0        0        0    41126 2023-08-14 14:25:43.000000 qis-2.0.9/qis/models/linear/ewm.py
+-rw-r--r--   0        0        0     3620 2023-02-18 22:06:06.000000 qis-2.0.9/qis/models/linear/ewm_convolution.py
+-rw-r--r--   0        0        0     6908 2023-08-14 15:11:32.000000 qis-2.0.9/qis/models/linear/ewm_factors.py
+-rw-r--r--   0        0        0     4032 2023-01-23 14:52:48.000000 qis-2.0.9/qis/models/linear/pca.py
+-rw-r--r--   0        0        0     7121 2023-08-18 10:10:08.566817 qis-2.0.9/qis/models/linear/plot_correlations.py
+-rw-r--r--   0        0        0    11519 2023-07-16 14:22:12.617158 qis-2.0.9/qis/models/linear/ra_returns.py
+-rw-r--r--   0        0        0       24 2023-01-23 21:08:28.000000 qis-2.0.9/qis/models/README.md
+-rw-r--r--   0        0        0        0 2021-12-04 12:08:05.446837 qis-2.0.9/qis/models/stats/__init__.py
+-rw-r--r--   0        0        0    19511 2023-07-16 05:40:45.921919 qis-2.0.9/qis/models/stats/bootstrap.py
+-rw-r--r--   0        0        0     2722 2023-07-18 20:08:16.000000 qis-2.0.9/qis/models/stats/ohlc_vol.py
+-rw-r--r--   0        0        0     8556 2023-02-18 22:06:11.000000 qis-2.0.9/qis/models/stats/test_bootstrap.py
+-rw-r--r--   0        0        0     2450 2023-08-28 12:41:52.000000 qis-2.0.9/qis/perfstats/__init__.py
+-rw-r--r--   0        0        0     7178 2023-01-23 14:52:48.000000 qis-2.0.9/qis/perfstats/cond_regression.py
+-rw-r--r--   0        0        0    11454 2023-08-17 13:03:26.545127 qis-2.0.9/qis/perfstats/config.py
+-rw-r--r--   0        0        0     7287 2023-07-21 13:43:13.664929 qis-2.0.9/qis/perfstats/desc_table.py
+-rw-r--r--   0        0        0    21447 2023-06-06 14:51:04.000000 qis-2.0.9/qis/perfstats/perf_stats.py
+-rw-r--r--   0        0        0       24 2023-01-23 21:09:51.000000 qis-2.0.9/qis/perfstats/README.md
+-rw-r--r--   0        0        0    20183 2023-08-31 15:47:02.000000 qis-2.0.9/qis/perfstats/regime_classifier.py
+-rw-r--r--   0        0        0    31925 2023-08-28 12:40:46.000000 qis-2.0.9/qis/perfstats/returns.py
+-rw-r--r--   0        0        0     7920 2023-05-12 14:35:19.552286 qis-2.0.9/qis/perfstats/timeseries_bfill.py
+-rw-r--r--   0        0        0     3812 2023-05-31 04:27:08.487324 qis-2.0.9/qis/plots/__init__.py
+-rw-r--r--   0        0        0    17328 2023-08-31 15:42:28.000000 qis-2.0.9/qis/plots/bars.py
+-rw-r--r--   0        0        0    23159 2023-07-15 15:16:40.000000 qis-2.0.9/qis/plots/boxplot.py
+-rw-r--r--   0        0        0     3917 2023-02-18 22:06:06.000000 qis-2.0.9/qis/plots/contour.py
+-rw-r--r--   0        0        0        0 2021-03-12 13:47:34.000000 qis-2.0.9/qis/plots/derived/__init__.py
+-rw-r--r--   0        0        0     2196 2023-01-07 22:34:01.686282 qis-2.0.9/qis/plots/derived/data_timeseries.py
+-rw-r--r--   0        0        0     7464 2023-04-23 14:40:57.890091 qis-2.0.9/qis/plots/derived/drawdowns.py
+-rw-r--r--   0        0        0    18835 2023-08-18 10:33:59.167827 qis-2.0.9/qis/plots/derived/perf_table.py
+-rw-r--r--   0        0        0    22969 2023-06-06 13:07:17.000000 qis-2.0.9/qis/plots/derived/prices.py
+-rw-r--r--   0        0        0     3489 2023-02-18 22:06:08.000000 qis-2.0.9/qis/plots/derived/regime_class_table.py
+-rw-r--r--   0        0        0    11938 2023-08-31 15:49:22.000000 qis-2.0.9/qis/plots/derived/regime_data.py
+-rw-r--r--   0        0        0     3519 2023-02-18 22:06:07.000000 qis-2.0.9/qis/plots/derived/regime_pdf.py
+-rw-r--r--   0        0        0     6590 2023-02-18 22:06:08.000000 qis-2.0.9/qis/plots/derived/regime_scatter.py
+-rw-r--r--   0        0        0    18010 2023-03-02 12:04:37.000000 qis-2.0.9/qis/plots/derived/returns_heatmap.py
+-rw-r--r--   0        0        0     5173 2023-02-18 22:06:08.000000 qis-2.0.9/qis/plots/derived/returns_scatter.py
+-rw-r--r--   0        0        0     4008 2023-02-18 22:06:13.000000 qis-2.0.9/qis/plots/errorbar.py
+-rw-r--r--   0        0        0     3643 2023-02-18 22:06:09.000000 qis-2.0.9/qis/plots/heatmap.py
+-rw-r--r--   0        0        0    11179 2023-08-28 13:10:19.000000 qis-2.0.9/qis/plots/histogram.py
+-rw-r--r--   0        0        0     2917 2023-08-11 07:39:51.000000 qis-2.0.9/qis/plots/histplot2d.py
+-rw-r--r--   0        0        0     5424 2023-02-18 22:06:07.000000 qis-2.0.9/qis/plots/lineplot.py
+-rw-r--r--   0        0        0     1850 2023-03-21 14:30:08.000000 qis-2.0.9/qis/plots/pie.py
+-rw-r--r--   0        0        0     5889 2023-02-18 22:06:10.000000 qis-2.0.9/qis/plots/qqplot.py
+-rw-r--r--   0        0        0       24 2023-01-23 21:10:18.000000 qis-2.0.9/qis/plots/README.md
+-rw-r--r--   0        0        0    15874 2023-03-14 11:00:14.000000 qis-2.0.9/qis/plots/scatter.py
+-rw-r--r--   0        0        0     6009 2023-03-21 06:51:44.000000 qis-2.0.9/qis/plots/stackplot.py
+-rw-r--r--   0        0        0    14372 2023-08-20 06:31:30.000000 qis-2.0.9/qis/plots/table.py
+-rw-r--r--   0        0        0    21512 2023-05-31 09:52:23.000000 qis-2.0.9/qis/plots/time_series.py
+-rw-r--r--   0        0        0    57385 2023-08-31 17:00:08.000000 qis-2.0.9/qis/plots/utils.py
+-rw-r--r--   0        0        0      706 2023-08-17 13:24:45.103644 qis-2.0.9/qis/portfolio/__init__.py
+-rw-r--r--   0        0        0    11646 2023-06-07 09:56:37.000000 qis-2.0.9/qis/portfolio/backtester.py
+-rw-r--r--   0        0        0    27546 2023-08-11 09:00:19.000000 qis-2.0.9/qis/portfolio/multi_portfolio_data.py
+-rw-r--r--   0        0        0    37213 2023-08-21 14:19:45.000000 qis-2.0.9/qis/portfolio/portfolio_data.py
+-rw-r--r--   0        0        0       24 2023-01-23 21:10:46.000000 qis-2.0.9/qis/portfolio/README.md
+-rw-r--r--   0        0        0        0 2023-06-22 07:59:37.604630 qis-2.0.9/qis/portfolio/reports/__init__.py
+-rw-r--r--   0        0        0     1856 2023-08-18 14:55:48.000000 qis-2.0.9/qis/portfolio/reports/config.py
+-rw-r--r--   0        0        0    17513 2023-08-17 12:48:25.650392 qis-2.0.9/qis/portfolio/reports/multi_assets_factsheet.py
+-rw-r--r--   0        0        0     7571 2023-07-08 08:11:22.704374 qis-2.0.9/qis/portfolio/reports/multi_strategy_factsheet.py
+-rw-r--r--   0        0        0    12549 2023-08-17 13:32:23.968301 qis-2.0.9/qis/portfolio/reports/strategy_benchmark_factsheet.py
+-rw-r--r--   0        0        0    11702 2023-08-23 08:38:13.000000 qis-2.0.9/qis/portfolio/reports/strategy_factsheet.py
+-rw-r--r--   0        0        0        0 2022-12-17 17:53:19.519118 qis-2.0.9/qis/portfolio/strats/__init__.py
+-rw-r--r--   0        0        0     5778 2023-02-18 22:06:12.000000 qis-2.0.9/qis/portfolio/strats/quant_strats_delta1.py
+-rw-r--r--   0        0        0      204 2023-08-31 17:59:03.398170 qis-2.0.9/qis/settings.yaml
+-rw-r--r--   0        0        0      443 2023-01-15 20:14:44.028937 qis-2.0.9/qis/sql_engine.py
+-rw-r--r--   0        0        0     1261 2023-03-02 12:52:25.000000 qis-2.0.9/qis/test_data.py
+-rw-r--r--   0        0        0     4779 2023-07-23 06:50:46.389371 qis-2.0.9/qis/utils/__init__.py
+-rw-r--r--   0        0        0    42107 2023-08-17 13:24:45.008898 qis-2.0.9/qis/utils/dates.py
+-rw-r--r--   0        0        0    11347 2023-06-07 09:35:59.000000 qis-2.0.9/qis/utils/df_agg.py
+-rw-r--r--   0        0        0     8491 2023-01-08 13:32:37.792219 qis-2.0.9/qis/utils/df_cut.py
+-rw-r--r--   0        0        0     7964 2023-07-28 06:10:47.082310 qis-2.0.9/qis/utils/df_freq.py
+-rw-r--r--   0        0        0    10992 2023-02-18 22:06:12.000000 qis-2.0.9/qis/utils/df_groups.py
+-rw-r--r--   0        0        0     6819 2023-02-18 22:06:11.000000 qis-2.0.9/qis/utils/df_melt.py
+-rw-r--r--   0        0        0    23956 2023-07-02 06:53:30.708901 qis-2.0.9/qis/utils/df_ops.py
+-rw-r--r--   0        0        0     8905 2023-02-18 22:06:10.000000 qis-2.0.9/qis/utils/df_str.py
+-rw-r--r--   0        0        0    11344 2022-12-30 16:13:34.048573 qis-2.0.9/qis/utils/df_to_weights.py
+-rw-r--r--   0        0        0    10640 2023-05-12 08:13:42.291695 qis-2.0.9/qis/utils/generic.py
+-rw-r--r--   0        0        0    15848 2023-07-05 08:50:35.000000 qis-2.0.9/qis/utils/np_ops.py
+-rw-r--r--   0        0        0     5576 2023-04-04 20:13:54.941670 qis-2.0.9/qis/utils/ols.py
+-rw-r--r--   0        0        0       22 2023-01-23 21:14:19.000000 qis-2.0.9/qis/utils/README.md
+-rw-r--r--   0        0        0     4589 2023-02-18 22:06:08.000000 qis-2.0.9/qis/utils/sampling.py
+-rw-r--r--   0        0        0     5938 2022-12-16 21:08:07.000000 qis-2.0.9/qis/utils/struct_ops.py
+-rw-r--r--   0        0        0     9104 2023-08-21 14:55:14.000000 qis-2.0.9/README.md
+-rw-r--r--   0        0        0    10890 1970-01-01 00:00:00.000000 qis-2.0.9/PKG-INFO
```

### Comparing `qis-2.0.8/LICENSE.txt` & `qis-2.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/pyproject.toml` & `qis-2.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b74 6f6f 6c2e 706f 6574 7279 5d0d 0a6e  [tool.poetry]..n
 00000010: 616d 6520 3d20 2271 6973 220d 0a76 6572  ame = "qis"..ver
-00000020: 7369 6f6e 203d 2022 322e 302e 3822 0d0a  sion = "2.0.8"..
+00000020: 7369 6f6e 203d 2022 322e 302e 3922 0d0a  sion = "2.0.9"..
 00000030: 6465 7363 7269 7074 696f 6e20 3d20 2249  description = "I
 00000040: 6d70 6c65 6d65 6e74 6174 696f 6e20 6f66  mplementation of
 00000050: 2076 6973 7561 6c69 7361 7469 6f6e 2061   visualisation a
 00000060: 6e64 2072 6570 6f72 7469 6e67 2061 6e61  nd reporting ana
 00000070: 6c79 7469 6373 2066 6f72 2051 7561 6e74  lytics for Quant
 00000080: 6974 6174 6976 6520 496e 7665 7374 6d65  itative Investme
 00000090: 6e74 2053 7472 6174 6567 6965 7322 0d0a  nt Strategies"..
```

### Comparing `qis-2.0.8/qis/__init__.py` & `qis-2.0.9/qis/__init__.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/examples/bootstrap_analysis.py` & `qis-2.0.9/qis/examples/bootstrap_analysis.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/examples/constant_notional.py` & `qis-2.0.9/qis/examples/constant_notional.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/examples/factsheets/multi_assets.py` & `qis-2.0.9/qis/examples/factsheets/multi_assets.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/examples/factsheets/multi_strategy.py` & `qis-2.0.9/qis/examples/factsheets/multi_strategy.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/examples/factsheets/strategy.py` & `qis-2.0.9/qis/examples/factsheets/strategy.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/examples/factsheets/strategy_benchmark.py` & `qis-2.0.9/qis/examples/factsheets/strategy_benchmark.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/examples/figures/multi_strategy.PNG` & `qis-2.0.9/qis/examples/figures/multi_strategy.PNG`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/examples/figures/multiassets.PNG` & `qis-2.0.9/qis/examples/figures/multiassets.PNG`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/examples/figures/perf1.PNG` & `qis-2.0.9/qis/examples/figures/perf1.PNG`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/examples/figures/perf2.PNG` & `qis-2.0.9/qis/examples/figures/perf2.PNG`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/examples/figures/perf3.PNG` & `qis-2.0.9/qis/examples/figures/perf3.PNG`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/examples/figures/strategy.PNG` & `qis-2.0.9/qis/examples/figures/strategy.PNG`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/examples/figures/strategy_benchmark.PNG` & `qis-2.0.9/qis/examples/figures/strategy_benchmark.PNG`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/examples/ohlc_vol_analysis.py` & `qis-2.0.9/qis/examples/ohlc_vol_analysis.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/examples/performances.py` & `qis-2.0.9/qis/examples/performances.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/examples/price_plots.py` & `qis-2.0.9/qis/examples/price_plots.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/examples/simulate_quant_strats.py` & `qis-2.0.9/qis/examples/simulate_quant_strats.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/examples/test_ewm.py` & `qis-2.0.9/qis/examples/test_ewm.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/examples/test_scatter.py` & `qis-2.0.9/qis/examples/test_scatter.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/examples/try_pybloqs.py` & `qis-2.0.9/qis/examples/try_pybloqs.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/file_utils.py` & `qis-2.0.9/qis/file_utils.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/local_path.py` & `qis-2.0.9/qis/local_path.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/models/__init__.py` & `qis-2.0.9/qis/models/__init__.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/models/linear/auto_corr.py` & `qis-2.0.9/qis/models/linear/auto_corr.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/models/linear/corr_cov_matrix.py` & `qis-2.0.9/qis/models/linear/corr_cov_matrix.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/models/linear/ewm.py` & `qis-2.0.9/qis/models/linear/ewm.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/models/linear/ewm_convolution.py` & `qis-2.0.9/qis/models/linear/ewm_convolution.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/models/linear/ewm_factors.py` & `qis-2.0.9/qis/models/linear/ewm_factors.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/models/linear/pca.py` & `qis-2.0.9/qis/models/linear/pca.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/models/linear/plot_correlations.py` & `qis-2.0.9/qis/models/linear/plot_correlations.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/models/linear/ra_returns.py` & `qis-2.0.9/qis/models/linear/ra_returns.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/models/stats/bootstrap.py` & `qis-2.0.9/qis/models/stats/bootstrap.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/models/stats/ohlc_vol.py` & `qis-2.0.9/qis/models/stats/ohlc_vol.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/models/stats/test_bootstrap.py` & `qis-2.0.9/qis/models/stats/test_bootstrap.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/perfstats/__init__.py` & `qis-2.0.9/qis/perfstats/__init__.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/perfstats/cond_regression.py` & `qis-2.0.9/qis/perfstats/cond_regression.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/perfstats/config.py` & `qis-2.0.9/qis/perfstats/config.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/perfstats/desc_table.py` & `qis-2.0.9/qis/perfstats/desc_table.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/perfstats/perf_stats.py` & `qis-2.0.9/qis/perfstats/perf_stats.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/perfstats/regime_classifier.py` & `qis-2.0.9/qis/perfstats/regime_classifier.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/perfstats/returns.py` & `qis-2.0.9/qis/perfstats/returns.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/perfstats/timeseries_bfill.py` & `qis-2.0.9/qis/perfstats/timeseries_bfill.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/plots/__init__.py` & `qis-2.0.9/qis/plots/__init__.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/plots/bars.py` & `qis-2.0.9/qis/plots/bars.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/plots/boxplot.py` & `qis-2.0.9/qis/plots/boxplot.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/plots/contour.py` & `qis-2.0.9/qis/plots/contour.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/plots/derived/data_timeseries.py` & `qis-2.0.9/qis/plots/derived/data_timeseries.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/plots/derived/drawdowns.py` & `qis-2.0.9/qis/plots/derived/drawdowns.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/plots/derived/perf_table.py` & `qis-2.0.9/qis/plots/derived/perf_table.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/plots/derived/prices.py` & `qis-2.0.9/qis/plots/derived/prices.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/plots/derived/regime_class_table.py` & `qis-2.0.9/qis/plots/derived/regime_class_table.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/plots/derived/regime_data.py` & `qis-2.0.9/qis/plots/derived/regime_data.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/plots/derived/regime_pdf.py` & `qis-2.0.9/qis/plots/derived/regime_pdf.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/plots/derived/regime_scatter.py` & `qis-2.0.9/qis/plots/derived/regime_scatter.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/plots/derived/returns_heatmap.py` & `qis-2.0.9/qis/plots/derived/returns_heatmap.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/plots/derived/returns_scatter.py` & `qis-2.0.9/qis/plots/derived/returns_scatter.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/plots/errorbar.py` & `qis-2.0.9/qis/plots/errorbar.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/plots/heatmap.py` & `qis-2.0.9/qis/plots/heatmap.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/plots/histogram.py` & `qis-2.0.9/qis/plots/histogram.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/plots/histplot2d.py` & `qis-2.0.9/qis/plots/histplot2d.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/plots/lineplot.py` & `qis-2.0.9/qis/plots/lineplot.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/plots/pie.py` & `qis-2.0.9/qis/plots/pie.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/plots/qqplot.py` & `qis-2.0.9/qis/plots/qqplot.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/plots/scatter.py` & `qis-2.0.9/qis/plots/scatter.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/plots/stackplot.py` & `qis-2.0.9/qis/plots/stackplot.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/plots/table.py` & `qis-2.0.9/qis/plots/table.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/plots/time_series.py` & `qis-2.0.9/qis/plots/time_series.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/plots/utils.py` & `qis-2.0.9/qis/plots/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -745,15 +745,15 @@
     AVG_STD_MISSING_ZERO = 18
     MISSING_AVG_LAST = 19
     TOTAL = 20
     MEDIAN = 21
     MEDIAN_MAD = 22
     TSTAT = 23
     AVG_STD_TSTAT = 24
-    LAST_NONNAN = 25
+    LAST_VALUE_ONLY = 25
 
 
 def get_legend_lines(data: Union[pd.DataFrame, pd.Series],
                      legend_stats: LegendStats = LegendStats.NONE,
                      var_format: str = '{:.0f}',
                      tstat_format: str = '{:,.2f}',
                      nan_display: float = np.nan,  # or zero
@@ -773,23 +773,18 @@
         legend_lines = data.columns.to_list()
 
     elif legend_stats == LegendStats.LAST:
         legend_lines = []
         for column in data.columns:
             legend_lines.append(f"{column}: last={var_format.format(data[column].iloc[-1])}")
 
-    elif legend_stats == LegendStats.LAST_NONNAN:
+    elif legend_stats == LegendStats.LAST_VALUE_ONLY:
         legend_lines = []
         for column in data.columns:
-            data_column = data[column]
-            if np.all(np.isnan(data_column)):
-                last_value = nan_display
-            else:
-                last_value = data[column].dropna().iloc[-1]
-            legend_lines.append(f"{column}: last={var_format.format(last_value)}")
+            legend_lines.append(f"{column} = {var_format.format(data[column].iloc[-1])}")
 
     elif legend_stats == LegendStats.AVG:
         legend_lines = []
         for column in data.columns:
             data_column = data[column]
             if np.all(np.isnan(data_column)):
                 avg = nan_display
```

### Comparing `qis-2.0.8/qis/portfolio/__init__.py` & `qis-2.0.9/qis/portfolio/__init__.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/portfolio/backtester.py` & `qis-2.0.9/qis/portfolio/backtester.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/portfolio/multi_portfolio_data.py` & `qis-2.0.9/qis/portfolio/multi_portfolio_data.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/portfolio/portfolio_data.py` & `qis-2.0.9/qis/portfolio/portfolio_data.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/portfolio/reports/config.py` & `qis-2.0.9/qis/portfolio/reports/config.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/portfolio/reports/multi_assets_factsheet.py` & `qis-2.0.9/qis/portfolio/reports/multi_assets_factsheet.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/portfolio/reports/multi_strategy_factsheet.py` & `qis-2.0.9/qis/portfolio/reports/multi_strategy_factsheet.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/portfolio/reports/strategy_benchmark_factsheet.py` & `qis-2.0.9/qis/portfolio/reports/strategy_benchmark_factsheet.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/portfolio/reports/strategy_factsheet.py` & `qis-2.0.9/qis/portfolio/reports/strategy_factsheet.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/portfolio/strats/quant_strats_delta1.py` & `qis-2.0.9/qis/portfolio/strats/quant_strats_delta1.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/test_data.py` & `qis-2.0.9/qis/test_data.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/utils/__init__.py` & `qis-2.0.9/qis/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/utils/dates.py` & `qis-2.0.9/qis/utils/dates.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/utils/df_agg.py` & `qis-2.0.9/qis/utils/df_agg.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/utils/df_cut.py` & `qis-2.0.9/qis/utils/df_cut.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/utils/df_freq.py` & `qis-2.0.9/qis/utils/df_freq.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/utils/df_groups.py` & `qis-2.0.9/qis/utils/df_groups.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/utils/df_melt.py` & `qis-2.0.9/qis/utils/df_melt.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/utils/df_ops.py` & `qis-2.0.9/qis/utils/df_ops.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/utils/df_str.py` & `qis-2.0.9/qis/utils/df_str.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/utils/df_to_weights.py` & `qis-2.0.9/qis/utils/df_to_weights.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/utils/generic.py` & `qis-2.0.9/qis/utils/generic.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/utils/np_ops.py` & `qis-2.0.9/qis/utils/np_ops.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/utils/ols.py` & `qis-2.0.9/qis/utils/ols.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/utils/sampling.py` & `qis-2.0.9/qis/utils/sampling.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/qis/utils/struct_ops.py` & `qis-2.0.9/qis/utils/struct_ops.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/README.md` & `qis-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `qis-2.0.8/PKG-INFO` & `qis-2.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qis
-Version: 2.0.8
+Version: 2.0.9
 Summary: Implementation of visualisation and reporting analytics for Quantitative Investment Strategies
 Home-page: https://github.com/ArturSepp/QuantInvestStrats
 License: LICENSE.txt
 Keywords: quantitative,investing,portfolio optimization,systematic strategies,volatility
 Author: Artur Sepp
 Author-email: artursepp@gmail.com
 Maintainer: Artur Sepp
```

