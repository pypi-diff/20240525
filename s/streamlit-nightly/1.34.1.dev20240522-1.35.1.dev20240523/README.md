# Comparing `tmp/streamlit_nightly-1.34.1.dev20240522.tar.gz` & `tmp/streamlit_nightly-1.35.1.dev20240523.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit_nightly-1.34.1.dev20240522.tar", last modified: Thu May 23 06:55:27 2024, max compression
+gzip compressed data, was "streamlit_nightly-1.35.1.dev20240523.tar", last modified: Fri May 24 06:54:55 2024, max compression
```

## Comparing `streamlit_nightly-1.34.1.dev20240522.tar` & `streamlit_nightly-1.35.1.dev20240523.tar`

### file list

```diff
@@ -1,574 +1,574 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:55:27.144568 streamlit_nightly-1.34.1.dev20240522/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8500 2024-05-23 06:55:27.144568 streamlit_nightly-1.34.1.dev20240522/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:55:27.028568 streamlit_nightly-1.34.1.dev20240522/bin/
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/bin/streamlit.cmd
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 06:55:27.144568 streamlit_nightly-1.34.1.dev20240522/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     6787 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:55:27.036568 streamlit_nightly-1.34.1.dev20240522/streamlit/
--rw-r--r--   0 runner    (1001) docker     (127)     8517 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/case_converters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/cli_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/code_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     9330 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/color_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/column_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:55:27.036568 streamlit_nightly-1.34.1.dev20240522/streamlit/commands/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5429 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/commands/execution_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     5042 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/commands/experimental_query_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/commands/logo.py
--rw-r--r--   0 runner    (1001) docker     (127)    12997 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/commands/page_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:55:27.036568 streamlit_nightly-1.34.1.dev20240522/streamlit/components/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:55:27.036568 streamlit_nightly-1.34.1.dev20240522/streamlit/components/lib/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/components/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/components/lib/local_component_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:55:27.036568 streamlit_nightly-1.34.1.dev20240522/streamlit/components/types/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/components/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/components/types/base_component_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     4262 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/components/types/base_custom_component.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:55:27.036568 streamlit_nightly-1.34.1.dev20240522/streamlit/components/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/components/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/components/v1/component_arrow.py
--rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/components/v1/component_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/components/v1/components.py
--rw-r--r--   0 runner    (1001) docker     (127)     9313 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/components/v1/custom_component.py
--rw-r--r--   0 runner    (1001) docker     (127)    43895 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    11469 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/config_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     6015 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/config_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:55:27.040568 streamlit_nightly-1.34.1.dev20240522/streamlit/connections/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/connections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7465 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/connections/base_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    12517 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/connections/snowflake_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     8184 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/connections/snowpark_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    12234 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/connections/sql_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/connections/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6001 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)    28200 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/delta_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6516 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/deprecation_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/development.py
--rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/echo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:55:27.044568 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7432 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/alert.py
--rw-r--r--   0 runner    (1001) docker     (127)    23830 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/arrow.py
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/balloons.py
--rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/bokeh_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/code.py
--rw-r--r--   0 runner    (1001) docker     (127)     6429 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/deck_gl_json_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     7797 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/dialog_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)    16168 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/doc_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/empty.py
--rw-r--r--   0 runner    (1001) docker     (127)     9121 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)    12072 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/form.py
--rw-r--r--   0 runner    (1001) docker     (127)     4557 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/graphviz_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)    11268 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/heading.py
--rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/html.py
--rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/iframe.py
--rw-r--r--   0 runner    (1001) docker     (127)    20394 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/json.py
--rw-r--r--   0 runner    (1001) docker     (127)    28251 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/layouts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:55:27.044568 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/lib/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30666 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/lib/built_in_chart_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    17374 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/lib/column_config_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    51174 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/lib/column_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5685 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/lib/dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/lib/dicttools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/lib/event_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6634 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/lib/mutable_status_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     8079 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/lib/pandas_styler_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8307 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/lib/streamlit_plotly_theme.py
--rw-r--r--   0 runner    (1001) docker     (127)     6246 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/lib/subtitle_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16299 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/map.py
--rw-r--r--   0 runner    (1001) docker     (127)    10384 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/markdown.py
--rw-r--r--   0 runner    (1001) docker     (127)    29678 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/media.py
--rw-r--r--   0 runner    (1001) docker     (127)    10114 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)    15344 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/plotly_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     5844 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/progress.py
--rw-r--r--   0 runner    (1001) docker     (127)     6441 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/pyplot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/snow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/spinner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/toast.py
--rw-r--r--   0 runner    (1001) docker     (127)     8085 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    58273 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/vega_charts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:55:27.048568 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32860 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/widgets/button.py
--rw-r--r--   0 runner    (1001) docker     (127)     9141 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/widgets/camera_input.py
--rw-r--r--   0 runner    (1001) docker     (127)    14320 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/widgets/chat.py
--rw-r--r--   0 runner    (1001) docker     (127)    12573 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/widgets/checkbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     9142 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/widgets/color_picker.py
--rw-r--r--   0 runner    (1001) docker     (127)    35827 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/widgets/data_editor.py
--rw-r--r--   0 runner    (1001) docker     (127)    17656 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/widgets/file_uploader.py
--rw-r--r--   0 runner    (1001) docker     (127)    13752 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/widgets/multiselect.py
--rw-r--r--   0 runner    (1001) docker     (127)    18036 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/widgets/number_input.py
--rw-r--r--   0 runner    (1001) docker     (127)    12824 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/widgets/radio.py
--rw-r--r--   0 runner    (1001) docker     (127)    13442 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/widgets/select_slider.py
--rw-r--r--   0 runner    (1001) docker     (127)    11665 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/widgets/selectbox.py
--rw-r--r--   0 runner    (1001) docker     (127)    26661 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/widgets/slider.py
--rw-r--r--   0 runner    (1001) docker     (127)    22333 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/widgets/text_widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)    30042 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/widgets/time_widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)    20804 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/write.py
--rw-r--r--   0 runner    (1001) docker     (127)    73749 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/emojis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/env_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/error_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:55:27.048568 streamlit_nightly-1.34.1.dev20240522/streamlit/external/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/external/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:55:27.048568 streamlit_nightly-1.34.1.dev20240522/streamlit/external/langchain/
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/external/langchain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15280 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/external/langchain/streamlit_callback_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     7216 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/file_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/folder_black_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/git_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:55:27.048568 streamlit_nightly-1.34.1.dev20240522/streamlit/hello/
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/hello/Hello.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/hello/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:55:27.052568 streamlit_nightly-1.34.1.dev20240522/streamlit/hello/pages/
--rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/hello/pages/0_Animation_Demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/hello/pages/1_Plotting_Demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3826 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/hello/pages/2_Mapping_Demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/hello/pages/3_DataFrame_Demo.py
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/hello/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/js_number.py
--rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    57136 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/material_icon_names.py
--rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/net_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/platform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:55:27.076568 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Alert_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Alert_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/AppPage_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/AppPage_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/ArrowNamedDataSet_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/ArrowNamedDataSet_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/ArrowVegaLiteChart_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/ArrowVegaLiteChart_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Arrow_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Arrow_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Audio_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Audio_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/AutoRerun_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/AutoRerun_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/BackMsg_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5251 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/BackMsg_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Balloons_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Balloons_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4193 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Block_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    12049 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Block_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/BokehChart_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/BokehChart_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Button_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Button_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/CameraInput_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/CameraInput_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/ChatInput_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/ChatInput_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Checkbox_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Checkbox_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/ClientState_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/ClientState_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Code_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Code_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/ColorPicker_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/ColorPicker_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     9670 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Components_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Components_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4394 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/DataFrame_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    15040 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/DataFrame_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/DateInput_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/DateInput_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/DeckGlJsonChart_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/DeckGlJsonChart_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Delta_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Delta_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/DocString_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/DocString_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/DownloadButton_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/DownloadButton_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10146 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Element_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    16972 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Element_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Empty_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Empty_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Exception_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Exception_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Favicon_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Favicon_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/FileUploader_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/FileUploader_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/ForwardMsg_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    12312 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/ForwardMsg_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/GitInfo_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/GitInfo_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/GraphVizChart_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/GraphVizChart_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Heading_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Heading_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Html_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Html_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/IFrame_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/IFrame_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Image_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Image_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Json_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Json_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/LabelVisibilityMessage_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/LabelVisibilityMessage_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/LinkButton_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/LinkButton_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Logo_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Logo_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Markdown_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Markdown_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Metric_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4041 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Metric_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/MultiSelect_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/MultiSelect_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/NamedDataSet_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/NamedDataSet_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/NewSession_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    18437 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/NewSession_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/NumberInput_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5182 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/NumberInput_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/PageConfig_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5480 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/PageConfig_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/PageInfo_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/PageInfo_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/PageLink_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/PageLink_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/PageNotFound_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/PageNotFound_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/PageProfile_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4825 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/PageProfile_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/PagesChanged_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/PagesChanged_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/ParentMessage_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/ParentMessage_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/PlotlyChart_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5103 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/PlotlyChart_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Progress_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Progress_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Radio_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3843 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Radio_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/RootContainer_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/RootContainer_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Selectbox_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Selectbox_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/SessionEvent_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/SessionEvent_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/SessionStatus_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/SessionStatus_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Skeleton_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Skeleton_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Slider_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6044 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Slider_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Snow_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Snow_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Spinner_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Spinner_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/TextArea_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/TextArea_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/TextInput_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/TextInput_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Text_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Text_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/TimeInput_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/TimeInput_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Toast_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Toast_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/VegaLiteChart_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/VegaLiteChart_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Video_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Video_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/WidgetStates_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6240 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/WidgetStates_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5938 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/openmetrics_data_model_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    20476 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/openmetrics_data_model_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:55:27.080568 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36646 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/app_session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:55:27.080568 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/caching/
--rw-r--r--   0 runner    (1001) docker     (127)     4370 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/caching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26393 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/caching/cache_data_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4730 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/caching/cache_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    21616 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/caching/cache_resource_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/caching/cache_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    18329 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/caching/cache_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    17358 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/caching/cached_message_replay.py
--rw-r--r--   0 runner    (1001) docker     (127)    18986 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/caching/hashing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:55:27.084568 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/caching/storage/
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/caching/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8922 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/caching/storage/cache_storage_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/caching/storage/dummy_cache_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     5389 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/caching/storage/in_memory_cache_storage_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     9311 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/caching/storage/local_disk_cache_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    12414 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/connection_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    11500 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     9805 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/forward_msg_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     6390 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/forward_msg_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)    11558 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/fragment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:55:27.084568 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/legacy_caching/
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/legacy_caching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27873 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/legacy_caching/caching.py
--rw-r--r--   0 runner    (1001) docker     (127)    35033 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/legacy_caching/hashing.py
--rw-r--r--   0 runner    (1001) docker     (127)     8510 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/media_file_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/media_file_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/memory_media_file_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/memory_session_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/memory_uploaded_file_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    14267 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/metrics_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    29438 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/runtime_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/script_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:55:27.084568 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/scriptrunner/
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/scriptrunner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9072 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/scriptrunner/magic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/scriptrunner/magic_funcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/scriptrunner/script_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     8027 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/scriptrunner/script_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)     8818 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/scriptrunner/script_run_context.py
--rw-r--r--   0 runner    (1001) docker     (127)    29911 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/scriptrunner/script_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)    12302 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)    13017 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/session_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:55:27.084568 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/state/
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8171 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/state/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     7477 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/state/query_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     7192 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/state/query_params_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     5169 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/state/safe_session_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    27500 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/state/session_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     5469 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/state/session_state_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)    11343 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/state/widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/uploaded_file_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6308 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/websocket_session_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     5749 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/source_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:55:27.088568 streamlit_nightly-1.34.1.dev20240522/streamlit/static/
--rw-r--r--   0 runner    (1001) docker     (127)    14353 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/asset-manifest.json
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-23 06:52:14.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/favicon.png
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:55:27.024568 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:55:27.088568 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)    33275 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/css/3466.8b8f33d6.chunk.css
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/css/5441.e3b876c5.chunk.css
--rw-r--r--   0 runner    (1001) docker     (127)    12090 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/css/8148.49dfd2ce.chunk.css
--rw-r--r--   0 runner    (1001) docker     (127)    29246 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/css/main.3aaaea00.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:55:27.120568 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)     5446 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/1074.73973756.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    15023 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/1168.14f7c6ff.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     5857 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/1307.0f0cca93.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     5024 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/1451.3b0a3e31.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     9618 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/1479.6709db03.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/178.7bea8c5d.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/1792.8bd6ce2a.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    33075 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/2178.90362aae.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    32468 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/2187.9469f035.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/2469.09ea79bb.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/2634.1249dc7a.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    65522 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/2736.4336e2b9.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/3053.7e70ec3b.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)  3637630 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/329.464ed8ec.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/329.464ed8ec.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/3301.1d1b10bb.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)  2306325 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/3466.05d62820.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/3466.05d62820.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/3513.7dedbda2.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/4113.99983645.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     9226 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/4132.49bf3f2c.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/4132.49bf3f2c.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/4177.69f9f18d.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/4319.bf1c86bf.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    20662 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/4477.1bd49702.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/4500.b6f348d1.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    14830 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/4666.c4b22a63.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/474.7eb0c6cd.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/5106.44f0ff51.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    21681 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/5117.04bfe5d3.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)  2263616 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/5249.f2f4070d.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    15117 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/5345.73d26e5d.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    10874 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/5379.6571574f.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    14533 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/5441.1b94928f.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)   107585 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/5791.9a42fb4b.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    11449 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/6013.4ba2d616.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    13239 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/6405.ac5a6f23.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    24494 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/6718.802da17e.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/6853.93dd1c4c.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)   398809 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/6950.70fe55c2.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/6950.70fe55c2.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    88545 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/7142.83028745.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     9607 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/7175.be4076bc.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)  3388121 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/7323.b74cc85b.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/7323.b74cc85b.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)   936700 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/7483.64f23be7.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/7483.64f23be7.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13275 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/7602.e8abc06b.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/7805.acc6316a.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/8005.43974a35.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    51115 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/8148.a17a918e.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/8427.bd0a7cf3.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/8477.de889fe5.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    15493 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/8492.0d93bd08.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    10240 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/8536.f8de3d9a.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    12214 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/8570.6de19120.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    10471 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/8691.9ccf7f89.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/9330.2b4c99e0.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    13574 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/9336.3e046ad7.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    20791 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/937.a1248039.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/937.a1248039.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    22113 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/9656.8c935274.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     4011 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/9865.fd93213d.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)  4405422 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/main.7e42f54d.js
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/main.7e42f54d.js.LICENSE.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:55:27.136568 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/
--rw-r--r--   0 runner    (1001) docker     (127)    28076 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_AMS-Regular.73ea273a72f4aca30ca5.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    63632 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_AMS-Regular.853be92419a6c3766b9a.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    33516 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_AMS-Regular.d562e886c52f12660a41.woff
--rw-r--r--   0 runner    (1001) docker     (127)    12368 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Caligraphic-Bold.7489a2fbfb9bfe704420.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Caligraphic-Bold.a1abf90dfd72792a577a.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     7716 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Caligraphic-Bold.d757c535a2e5902f1325.woff
--rw-r--r--   0 runner    (1001) docker     (127)    12344 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Caligraphic-Regular.7e873d3833eb108a0758.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     6908 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Caligraphic-Regular.d6484fce1ef428d5bd94.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     7656 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Caligraphic-Regular.db074fa22cf224af93d7.woff
--rw-r--r--   0 runner    (1001) docker     (127)    13296 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Fraktur-Bold.354501bac435c3264834.woff
--rw-r--r--   0 runner    (1001) docker     (127)    19584 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Fraktur-Bold.4c761b3711973ab04edf.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    11348 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Fraktur-Bold.931d67ea207ab37ee693.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    11316 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Fraktur-Regular.172d3529b26f8cedef6b.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    13208 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Fraktur-Regular.6fdf0ac577be0ba82a4c.woff
--rw-r--r--   0 runner    (1001) docker     (127)    19572 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Fraktur-Regular.ed305b5434865e06ffde.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    29912 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Main-Bold.0c3b8929d377c0e9b2f3.woff
--rw-r--r--   0 runner    (1001) docker     (127)    25324 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Main-Bold.39890742bc957b368704.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    51336 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Main-Bold.8169508bf58f8bd92ad8.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    16780 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Main-BoldItalic.20f389c4120be058d80a.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    19412 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Main-BoldItalic.428978dc7837d46de091.woff
--rw-r--r--   0 runner    (1001) docker     (127)    32968 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Main-BoldItalic.828abcb200061cffbaae.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    33580 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Main-Italic.fa675e5e4bec9eb250b6.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    19676 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Main-Italic.fd947498bc16392e76c2.woff
--rw-r--r--   0 runner    (1001) docker     (127)    16988 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Main-Italic.fe2176f79edaa716e621.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    30772 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Main-Regular.4f35fbcc9ee8614c2bcc.woff
--rw-r--r--   0 runner    (1001) docker     (127)    53580 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Main-Regular.9eba1d77abcf2aa6e94e.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    26272 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Main-Regular.f650f111a3b890d116f1.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    18668 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Math-BoldItalic.3f07ed67f06c720120ce.woff
--rw-r--r--   0 runner    (1001) docker     (127)    31196 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Math-BoldItalic.bf2d440b3a42ea78a998.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    16400 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Math-BoldItalic.dcbcbd93bac0470b462d.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    16440 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Math-Italic.6d3d25f4820d0da8f01f.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    31308 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Math-Italic.8a5f936332e8028c7278.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    18748 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Math-Italic.96759856b4e70f3a8338.woff
--rw-r--r--   0 runner    (1001) docker     (127)    24504 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_SansSerif-Bold.5b49f4993ae22d7975b4.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    12216 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_SansSerif-Bold.95591a929f0d32aa282a.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    14408 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_SansSerif-Bold.b9cd458ac6d5889ff9c3.woff
--rw-r--r--   0 runner    (1001) docker     (127)    12028 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_SansSerif-Italic.7d393d382f3e7fb1c637.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    14112 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_SansSerif-Italic.8d593cfaa96238d5e2f8.woff
--rw-r--r--   0 runner    (1001) docker     (127)    22364 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_SansSerif-Italic.b257a18c016f37ee4543.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    12316 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_SansSerif-Regular.02271ec5cb9f5b4588ac.woff
--rw-r--r--   0 runner    (1001) docker     (127)    19436 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_SansSerif-Regular.2f7bc363fc5424ebda59.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    10344 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_SansSerif-Regular.cd5e231e0cc53b2cb2c0.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    10588 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Script-Regular.073b3402d036714b4370.woff
--rw-r--r--   0 runner    (1001) docker     (127)     9644 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Script-Regular.c81d1b2a4b75d3eded60.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    16648 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Script-Regular.fc9ba5249878cd8f8d88.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Size1-Regular.0108e89c9003e8c14ea3.woff
--rw-r--r--   0 runner    (1001) docker     (127)    12228 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Size1-Regular.6de7d4b539221a49e9e2.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Size1-Regular.6eec866c69313624be60.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     5208 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Size2-Regular.2960900c4f271311eb36.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     6188 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Size2-Regular.3a99e70aee4076660d38.woff
--rw-r--r--   0 runner    (1001) docker     (127)    11508 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Size2-Regular.57f5c1837853986ea1db.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Size3-Regular.7947224e8a9914fa332b.woff
--rw-r--r--   0 runner    (1001) docker     (127)     7588 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Size3-Regular.8d6b6822586eea3d3b20.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Size3-Regular.e1951519f6f0596f7356.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    10364 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Size4-Regular.4ad7c7e8bb8d10a34bb7.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     5980 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Size4-Regular.aeffd8025cba3647f1a6.woff
--rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Size4-Regular.e418bf257af1052628d8.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    16028 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Typewriter-Regular.4c6b94fd1d07f8beff7c.woff
--rw-r--r--   0 runner    (1001) docker     (127)    13568 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Typewriter-Regular.c295e7f71970f03c0549.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    27556 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Typewriter-Regular.c5c02d763c89380dcb4e.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   247332 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/MaterialSymbols-Outlined.909d2dce4aba724ad02f.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    74492 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/SourceCodePro-Bold.17a68a0751a813474a0e.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    63060 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/SourceCodePro-BoldItalic.d45b7a3df103d441d78b.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    62096 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/SourceCodePro-Italic.ec122a420df4175e74f2.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    74052 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/SourceCodePro-Regular.84b900b88d09398d86b0.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    74132 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/SourceCodePro-SemiBold.17291d1c493cb25eb2c3.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    62988 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/SourceCodePro-SemiBoldItalic.f879ae27307c3926522b.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    76860 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/SourceSansPro-Bold.118dea98980e20a81ced.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    44640 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/SourceSansPro-BoldItalic.1d664be59d2eb5fef029.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    44748 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/SourceSansPro-Italic.8a9bfea74d43927d6eec.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    77664 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/SourceSansPro-Regular.0d69e5ff5e92ac64a0c9.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    77452 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/SourceSansPro-SemiBold.abed79cd0df1827e18cf.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    44608 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/SourceSansPro-SemiBoldItalic.befb0a2824eabc5ce36b.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    72892 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/SourceSerifPro-Bold.d7975b56594770699ae0.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    30756 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/SourceSerifPro-BoldItalic.913697a7178b128caa4c.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    29384 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/SourceSerifPro-Italic.d3529cb5797663ac5d88.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    68356 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/SourceSerifPro-Regular.e6c37aa3926474cc93e1.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    72668 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/SourceSerifPro-SemiBold.5c1d378dd5990ef334ca.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    30628 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/SourceSerifPro-SemiBoldItalic.249e948b885d0c7d30a8.woff2
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/checkmark.29851c8e9e6ef0c3d6c1e4efe3c1bb9e.svg
--rw-r--r--   0 runner    (1001) docker     (127)   101906 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/fireworks.0906f02ea43f1018a6d2.gif
--rw-r--r--   0 runner    (1001) docker     (127)    73528 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/flake-0.beded754e8024c73d9d2.png
--rw-r--r--   0 runner    (1001) docker     (127)    86179 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/flake-1.8077dc154e0bf900aa73.png
--rw-r--r--   0 runner    (1001) docker     (127)    92182 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/flake-2.e3f07d06933dd0e84c24.png
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/logo.83ae4f2fb87e38be7cbb8a5d2beb64d2.svg
--rw-r--r--   0 runner    (1001) docker     (127)    39315 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/rocket.b75b17d2b0a063c6cea230d1a9d77f1e.svg
--rw-r--r--   0 runner    (1001) docker     (127)     6347 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/string_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/temporary_directory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:55:27.136568 streamlit_nightly-1.34.1.dev20240522/streamlit/testing/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:55:27.140568 streamlit_nightly-1.34.1.dev20240522/streamlit/testing/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/testing/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36577 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/testing/v1/app_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    59854 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/testing/v1/element_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/testing/v1/local_script_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/testing/v1/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/time_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    48389 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/type_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/url_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/user_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     6379 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:55:27.140568 streamlit_nightly-1.34.1.dev20240522/streamlit/vendor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/vendor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:55:27.140568 streamlit_nightly-1.34.1.dev20240522/streamlit/vendor/ipython/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/vendor/ipython/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/vendor/ipython/modified_sys_path.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:55:27.140568 streamlit_nightly-1.34.1.dev20240522/streamlit/vendor/pympler/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/vendor/pympler/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    87925 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/vendor/pympler/asizeof.py
--rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:55:27.140568 streamlit_nightly-1.34.1.dev20240522/streamlit/watcher/
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/watcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13980 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/watcher/event_based_path_watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     8238 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/watcher/local_sources_watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/watcher/path_watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/watcher/polling_path_watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     5203 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/watcher/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:55:27.140568 streamlit_nightly-1.34.1.dev20240522/streamlit/web/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14233 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/web/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/web/cache_storage_manager_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    11321 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/web/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:55:27.144568 streamlit_nightly-1.34.1.dev20240522/streamlit/web/server/
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/web/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/web/server/app_static_file_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     7803 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/web/server/browser_websocket_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/web/server/component_request_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5270 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/web/server/media_file_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     9972 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/web/server/routes.py
--rw-r--r--   0 runner    (1001) docker     (127)    14834 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/web/server/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/web/server/server_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/web/server/stats_request_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/web/server/upload_file_request_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/web/server/websocket_headers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:55:27.144568 streamlit_nightly-1.34.1.dev20240522/streamlit_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8500 2024-05-23 06:55:25.000000 streamlit_nightly-1.34.1.dev20240522/streamlit_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    23316 2024-05-23 06:55:25.000000 streamlit_nightly-1.34.1.dev20240522/streamlit_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 06:55:25.000000 streamlit_nightly-1.34.1.dev20240522/streamlit_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-23 06:55:25.000000 streamlit_nightly-1.34.1.dev20240522/streamlit_nightly.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 06:51:43.000000 streamlit_nightly-1.34.1.dev20240522/streamlit_nightly.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-23 06:55:25.000000 streamlit_nightly-1.34.1.dev20240522/streamlit_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-23 06:55:25.000000 streamlit_nightly-1.34.1.dev20240522/streamlit_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:55:27.144568 streamlit_nightly-1.34.1.dev20240522/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/tests/testutil.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 06:54:55.849885 streamlit_nightly-1.35.1.dev20240523/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8500 2024-05-24 06:54:55.849885 streamlit_nightly-1.35.1.dev20240523/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 06:54:55.733885 streamlit_nightly-1.35.1.dev20240523/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/bin/streamlit.cmd
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 06:54:55.849885 streamlit_nightly-1.35.1.dev20240523/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     6787 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 06:54:55.737885 streamlit_nightly-1.35.1.dev20240523/streamlit/
+-rw-r--r--   0 runner    (1001) docker     (127)     8517 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/case_converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/cli_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/code_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9330 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/color_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/column_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 06:54:55.741885 streamlit_nightly-1.35.1.dev20240523/streamlit/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5429 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/commands/execution_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5042 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/commands/experimental_query_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5733 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/commands/logo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12997 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/commands/page_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 06:54:55.741885 streamlit_nightly-1.35.1.dev20240523/streamlit/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 06:54:55.741885 streamlit_nightly-1.35.1.dev20240523/streamlit/components/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/components/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/components/lib/local_component_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 06:54:55.741885 streamlit_nightly-1.35.1.dev20240523/streamlit/components/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/components/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/components/types/base_component_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4262 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/components/types/base_custom_component.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 06:54:55.741885 streamlit_nightly-1.35.1.dev20240523/streamlit/components/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/components/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/components/v1/component_arrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/components/v1/component_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/components/v1/components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9313 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/components/v1/custom_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44105 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11469 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/config_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6015 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/config_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 06:54:55.741885 streamlit_nightly-1.35.1.dev20240523/streamlit/connections/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/connections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7465 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/connections/base_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12517 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/connections/snowflake_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8184 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/connections/snowpark_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12234 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/connections/sql_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/connections/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6001 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28200 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/delta_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6516 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/deprecation_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/development.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/echo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 06:54:55.749885 streamlit_nightly-1.35.1.dev20240523/streamlit/elements/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/elements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7432 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/elements/alert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27716 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/elements/arrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/elements/balloons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4257 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/elements/bokeh_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/elements/code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6895 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/elements/deck_gl_json_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7797 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/elements/dialog_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16168 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/elements/doc_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/elements/empty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9121 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/elements/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12072 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/elements/form.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4887 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/elements/graphviz_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11268 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/elements/heading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/elements/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/elements/iframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20394 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/elements/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/elements/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28251 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/elements/layouts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 06:54:55.749885 streamlit_nightly-1.35.1.dev20240523/streamlit/elements/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/elements/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30696 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/elements/lib/built_in_chart_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17374 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/elements/lib/column_config_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51174 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/elements/lib/column_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5685 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/elements/lib/dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/elements/lib/dicttools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/elements/lib/event_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6634 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/elements/lib/mutable_status_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8079 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/elements/lib/pandas_styler_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8307 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/elements/lib/streamlit_plotly_theme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6246 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/elements/lib/subtitle_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16638 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/elements/map.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10384 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/elements/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29678 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/elements/media.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10114 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/elements/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19195 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/elements/plotly_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5844 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/elements/progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6835 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/elements/pyplot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/elements/snow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/elements/spinner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/elements/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/elements/toast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8085 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/elements/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69993 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/elements/vega_charts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 06:54:55.753885 streamlit_nightly-1.35.1.dev20240523/streamlit/elements/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/elements/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32860 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/elements/widgets/button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9141 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/elements/widgets/camera_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14320 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/elements/widgets/chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12573 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/elements/widgets/checkbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9142 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/elements/widgets/color_picker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36498 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/elements/widgets/data_editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17656 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/elements/widgets/file_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13752 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/elements/widgets/multiselect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18036 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/elements/widgets/number_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12824 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/elements/widgets/radio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13442 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/elements/widgets/select_slider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11665 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/elements/widgets/selectbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26661 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/elements/widgets/slider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22333 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/elements/widgets/text_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30042 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/elements/widgets/time_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20804 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/elements/write.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73749 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/emojis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/env_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/error_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 06:54:55.753885 streamlit_nightly-1.35.1.dev20240523/streamlit/external/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/external/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 06:54:55.753885 streamlit_nightly-1.35.1.dev20240523/streamlit/external/langchain/
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/external/langchain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15280 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/external/langchain/streamlit_callback_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7216 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/file_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/folder_black_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/git_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 06:54:55.753885 streamlit_nightly-1.35.1.dev20240523/streamlit/hello/
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/hello/Hello.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/hello/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 06:54:55.753885 streamlit_nightly-1.35.1.dev20240523/streamlit/hello/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/hello/pages/0_Animation_Demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/hello/pages/1_Plotting_Demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3826 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/hello/pages/2_Mapping_Demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/hello/pages/3_DataFrame_Demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/hello/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/js_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57136 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/material_icon_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/net_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/platform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 06:54:55.781885 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Alert_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Alert_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/AppPage_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/AppPage_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/ArrowNamedDataSet_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/ArrowNamedDataSet_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/ArrowVegaLiteChart_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/ArrowVegaLiteChart_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Arrow_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Arrow_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Audio_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Audio_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/AutoRerun_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/AutoRerun_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/BackMsg_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5251 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/BackMsg_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Balloons_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Balloons_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4193 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Block_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12049 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Block_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/BokehChart_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/BokehChart_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Button_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Button_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/CameraInput_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/CameraInput_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/ChatInput_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/ChatInput_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Checkbox_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Checkbox_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/ClientState_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/ClientState_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Code_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Code_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/ColorPicker_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/ColorPicker_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9670 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Components_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Components_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4394 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/DataFrame_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15040 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/DataFrame_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/DateInput_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/DateInput_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/DeckGlJsonChart_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/DeckGlJsonChart_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Delta_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Delta_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/DocString_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/DocString_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/DownloadButton_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/DownloadButton_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10146 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Element_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16972 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Element_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Empty_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Empty_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Exception_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Exception_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Favicon_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Favicon_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/FileUploader_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/FileUploader_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/ForwardMsg_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12312 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/ForwardMsg_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/GitInfo_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/GitInfo_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/GraphVizChart_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/GraphVizChart_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Heading_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Heading_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Html_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Html_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/IFrame_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/IFrame_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Image_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Image_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Json_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Json_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/LabelVisibilityMessage_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/LabelVisibilityMessage_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/LinkButton_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/LinkButton_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Logo_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Logo_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Markdown_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Markdown_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Metric_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4041 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Metric_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/MultiSelect_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/MultiSelect_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/NamedDataSet_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/NamedDataSet_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/NewSession_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18437 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/NewSession_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/NumberInput_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5182 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/NumberInput_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/PageConfig_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5480 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/PageConfig_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/PageInfo_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/PageInfo_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/PageLink_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/PageLink_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/PageNotFound_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/PageNotFound_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/PageProfile_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4825 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/PageProfile_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/PagesChanged_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/PagesChanged_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/ParentMessage_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/ParentMessage_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/PlotlyChart_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5103 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/PlotlyChart_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Progress_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Progress_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Radio_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3843 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Radio_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/RootContainer_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/RootContainer_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Selectbox_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Selectbox_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/SessionEvent_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/SessionEvent_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/SessionStatus_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/SessionStatus_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Skeleton_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Skeleton_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Slider_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6044 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Slider_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Snow_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Snow_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Spinner_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Spinner_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/TextArea_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/TextArea_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/TextInput_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/TextInput_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Text_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Text_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/TimeInput_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/TimeInput_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Toast_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Toast_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/VegaLiteChart_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/VegaLiteChart_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Video_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Video_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/WidgetStates_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6240 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/WidgetStates_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5938 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/openmetrics_data_model_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20476 2024-05-24 06:51:10.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/proto/openmetrics_data_model_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 06:54:55.785885 streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36716 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/app_session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 06:54:55.789885 streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/caching/
+-rw-r--r--   0 runner    (1001) docker     (127)     4370 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/caching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26393 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/caching/cache_data_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4730 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/caching/cache_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21616 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/caching/cache_resource_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/caching/cache_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18329 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/caching/cache_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17358 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/caching/cached_message_replay.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18986 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/caching/hashing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 06:54:55.789885 streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/caching/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/caching/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8922 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/caching/storage/cache_storage_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/caching/storage/dummy_cache_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5389 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/caching/storage/in_memory_cache_storage_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9311 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/caching/storage/local_disk_cache_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12414 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/connection_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11500 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9805 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/forward_msg_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6390 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/forward_msg_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11558 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/fragment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 06:54:55.789885 streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/legacy_caching/
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/legacy_caching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27873 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/legacy_caching/caching.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35033 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/legacy_caching/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8510 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/media_file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/media_file_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/memory_media_file_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/memory_session_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/memory_uploaded_file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14267 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/metrics_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29438 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/runtime_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/script_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 06:54:55.789885 streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/scriptrunner/
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/scriptrunner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9072 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/scriptrunner/magic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/scriptrunner/magic_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/scriptrunner/script_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8027 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/scriptrunner/script_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8818 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/scriptrunner/script_run_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29911 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/scriptrunner/script_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12302 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13017 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/session_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 06:54:55.793885 streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/state/
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8171 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/state/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7477 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/state/query_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7192 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/state/query_params_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5169 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/state/safe_session_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27500 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/state/session_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5469 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/state/session_state_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11343 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/state/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/uploaded_file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6308 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/websocket_session_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5749 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/source_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 06:54:55.793885 streamlit_nightly-1.35.1.dev20240523/streamlit/static/
+-rw-r--r--   0 runner    (1001) docker     (127)    14353 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/asset-manifest.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-24 06:51:39.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 06:54:55.729884 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 06:54:55.793885 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)    33275 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/css/3466.8b8f33d6.chunk.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/css/5441.e3b876c5.chunk.css
+-rw-r--r--   0 runner    (1001) docker     (127)    12090 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/css/8148.49dfd2ce.chunk.css
+-rw-r--r--   0 runner    (1001) docker     (127)    29246 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/css/main.3aaaea00.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 06:54:55.825885 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     5446 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/1074.73973756.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    15023 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/1168.14f7c6ff.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5857 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/1307.0f0cca93.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5024 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/1451.3b0a3e31.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9618 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/1479.6709db03.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/178.7bea8c5d.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/1792.8bd6ce2a.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    33075 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/2178.90362aae.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    32468 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/2187.9469f035.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/2469.09ea79bb.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/2634.1249dc7a.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    65522 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/2736.4336e2b9.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/3053.7e70ec3b.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)  3637630 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/329.464ed8ec.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/329.464ed8ec.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/3301.1d1b10bb.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)  2306325 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/3466.05d62820.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/3466.05d62820.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/3513.7dedbda2.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/4113.99983645.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9226 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/4132.49bf3f2c.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/4132.49bf3f2c.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/4177.69f9f18d.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/4319.bf1c86bf.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    20662 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/4477.1bd49702.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/4500.b6f348d1.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    14830 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/4666.c4b22a63.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/474.7eb0c6cd.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/5106.44f0ff51.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    21681 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/5117.04bfe5d3.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)  2263616 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/5249.f2f4070d.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    15117 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/5345.73d26e5d.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10874 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/5379.6571574f.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    14533 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/5441.1b94928f.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)   107585 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/5791.9a42fb4b.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    11449 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/6013.4ba2d616.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13239 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/6405.ac5a6f23.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    24494 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/6718.802da17e.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/6853.93dd1c4c.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)   398809 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/6950.70fe55c2.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/6950.70fe55c2.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    88545 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/7142.83028745.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9607 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/7175.be4076bc.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)  3388121 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/7323.b74cc85b.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/7323.b74cc85b.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   936700 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/7483.64f23be7.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/7483.64f23be7.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13275 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/7602.e8abc06b.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/7805.acc6316a.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/8005.43974a35.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    51115 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/8148.a17a918e.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/8427.bd0a7cf3.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/8477.de889fe5.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    15493 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/8492.0d93bd08.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10240 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/8536.f8de3d9a.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12214 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/8570.6de19120.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10471 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/8691.9ccf7f89.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/9330.2b4c99e0.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13574 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/9336.3e046ad7.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    20791 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/937.a1248039.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/937.a1248039.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    22113 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/9656.8c935274.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4011 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/9865.fd93213d.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)  4405422 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/main.7e42f54d.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/main.7e42f54d.js.LICENSE.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 06:54:55.841885 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/
+-rw-r--r--   0 runner    (1001) docker     (127)    28076 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_AMS-Regular.73ea273a72f4aca30ca5.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    63632 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_AMS-Regular.853be92419a6c3766b9a.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    33516 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_AMS-Regular.d562e886c52f12660a41.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    12368 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Caligraphic-Bold.7489a2fbfb9bfe704420.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Caligraphic-Bold.a1abf90dfd72792a577a.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     7716 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Caligraphic-Bold.d757c535a2e5902f1325.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    12344 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Caligraphic-Regular.7e873d3833eb108a0758.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     6908 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Caligraphic-Regular.d6484fce1ef428d5bd94.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     7656 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Caligraphic-Regular.db074fa22cf224af93d7.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    13296 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Fraktur-Bold.354501bac435c3264834.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    19584 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Fraktur-Bold.4c761b3711973ab04edf.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    11348 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Fraktur-Bold.931d67ea207ab37ee693.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    11316 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Fraktur-Regular.172d3529b26f8cedef6b.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    13208 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Fraktur-Regular.6fdf0ac577be0ba82a4c.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    19572 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Fraktur-Regular.ed305b5434865e06ffde.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    29912 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Main-Bold.0c3b8929d377c0e9b2f3.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    25324 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Main-Bold.39890742bc957b368704.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    51336 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Main-Bold.8169508bf58f8bd92ad8.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    16780 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Main-BoldItalic.20f389c4120be058d80a.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    19412 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Main-BoldItalic.428978dc7837d46de091.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    32968 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Main-BoldItalic.828abcb200061cffbaae.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    33580 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Main-Italic.fa675e5e4bec9eb250b6.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    19676 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Main-Italic.fd947498bc16392e76c2.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    16988 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Main-Italic.fe2176f79edaa716e621.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    30772 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Main-Regular.4f35fbcc9ee8614c2bcc.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    53580 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Main-Regular.9eba1d77abcf2aa6e94e.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    26272 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Main-Regular.f650f111a3b890d116f1.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    18668 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Math-BoldItalic.3f07ed67f06c720120ce.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    31196 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Math-BoldItalic.bf2d440b3a42ea78a998.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    16400 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Math-BoldItalic.dcbcbd93bac0470b462d.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    16440 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Math-Italic.6d3d25f4820d0da8f01f.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    31308 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Math-Italic.8a5f936332e8028c7278.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    18748 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Math-Italic.96759856b4e70f3a8338.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    24504 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_SansSerif-Bold.5b49f4993ae22d7975b4.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    12216 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_SansSerif-Bold.95591a929f0d32aa282a.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    14408 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_SansSerif-Bold.b9cd458ac6d5889ff9c3.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    12028 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_SansSerif-Italic.7d393d382f3e7fb1c637.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    14112 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_SansSerif-Italic.8d593cfaa96238d5e2f8.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    22364 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_SansSerif-Italic.b257a18c016f37ee4543.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    12316 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_SansSerif-Regular.02271ec5cb9f5b4588ac.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    19436 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_SansSerif-Regular.2f7bc363fc5424ebda59.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    10344 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_SansSerif-Regular.cd5e231e0cc53b2cb2c0.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    10588 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Script-Regular.073b3402d036714b4370.woff
+-rw-r--r--   0 runner    (1001) docker     (127)     9644 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Script-Regular.c81d1b2a4b75d3eded60.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    16648 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Script-Regular.fc9ba5249878cd8f8d88.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Size1-Regular.0108e89c9003e8c14ea3.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    12228 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Size1-Regular.6de7d4b539221a49e9e2.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Size1-Regular.6eec866c69313624be60.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     5208 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Size2-Regular.2960900c4f271311eb36.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     6188 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Size2-Regular.3a99e70aee4076660d38.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    11508 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Size2-Regular.57f5c1837853986ea1db.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Size3-Regular.7947224e8a9914fa332b.woff
+-rw-r--r--   0 runner    (1001) docker     (127)     7588 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Size3-Regular.8d6b6822586eea3d3b20.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Size3-Regular.e1951519f6f0596f7356.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    10364 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Size4-Regular.4ad7c7e8bb8d10a34bb7.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     5980 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Size4-Regular.aeffd8025cba3647f1a6.woff
+-rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Size4-Regular.e418bf257af1052628d8.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    16028 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Typewriter-Regular.4c6b94fd1d07f8beff7c.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    13568 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Typewriter-Regular.c295e7f71970f03c0549.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    27556 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Typewriter-Regular.c5c02d763c89380dcb4e.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   247332 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/MaterialSymbols-Outlined.909d2dce4aba724ad02f.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    74492 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/SourceCodePro-Bold.17a68a0751a813474a0e.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    63060 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/SourceCodePro-BoldItalic.d45b7a3df103d441d78b.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    62096 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/SourceCodePro-Italic.ec122a420df4175e74f2.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    74052 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/SourceCodePro-Regular.84b900b88d09398d86b0.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    74132 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/SourceCodePro-SemiBold.17291d1c493cb25eb2c3.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    62988 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/SourceCodePro-SemiBoldItalic.f879ae27307c3926522b.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    76860 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/SourceSansPro-Bold.118dea98980e20a81ced.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    44640 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/SourceSansPro-BoldItalic.1d664be59d2eb5fef029.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    44748 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/SourceSansPro-Italic.8a9bfea74d43927d6eec.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    77664 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/SourceSansPro-Regular.0d69e5ff5e92ac64a0c9.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    77452 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/SourceSansPro-SemiBold.abed79cd0df1827e18cf.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    44608 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/SourceSansPro-SemiBoldItalic.befb0a2824eabc5ce36b.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    72892 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/SourceSerifPro-Bold.d7975b56594770699ae0.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    30756 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/SourceSerifPro-BoldItalic.913697a7178b128caa4c.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    29384 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/SourceSerifPro-Italic.d3529cb5797663ac5d88.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    68356 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/SourceSerifPro-Regular.e6c37aa3926474cc93e1.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    72668 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/SourceSerifPro-SemiBold.5c1d378dd5990ef334ca.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    30628 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/SourceSerifPro-SemiBoldItalic.249e948b885d0c7d30a8.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/checkmark.29851c8e9e6ef0c3d6c1e4efe3c1bb9e.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   101906 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/fireworks.0906f02ea43f1018a6d2.gif
+-rw-r--r--   0 runner    (1001) docker     (127)    73528 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/flake-0.beded754e8024c73d9d2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    86179 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/flake-1.8077dc154e0bf900aa73.png
+-rw-r--r--   0 runner    (1001) docker     (127)    92182 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/flake-2.e3f07d06933dd0e84c24.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/logo.83ae4f2fb87e38be7cbb8a5d2beb64d2.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    39315 2024-05-24 06:54:52.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/rocket.b75b17d2b0a063c6cea230d1a9d77f1e.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6347 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/string_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/temporary_directory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 06:54:55.841885 streamlit_nightly-1.35.1.dev20240523/streamlit/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 06:54:55.845885 streamlit_nightly-1.35.1.dev20240523/streamlit/testing/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/testing/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36577 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/testing/v1/app_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59854 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/testing/v1/element_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/testing/v1/local_script_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/testing/v1/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/time_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48389 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/type_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/url_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/user_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6379 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 06:54:55.845885 streamlit_nightly-1.35.1.dev20240523/streamlit/vendor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/vendor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 06:54:55.845885 streamlit_nightly-1.35.1.dev20240523/streamlit/vendor/ipython/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/vendor/ipython/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/vendor/ipython/modified_sys_path.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 06:54:55.845885 streamlit_nightly-1.35.1.dev20240523/streamlit/vendor/pympler/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/vendor/pympler/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    87925 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/vendor/pympler/asizeof.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 06:54:55.845885 streamlit_nightly-1.35.1.dev20240523/streamlit/watcher/
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/watcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13980 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/watcher/event_based_path_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8238 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/watcher/local_sources_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/watcher/path_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/watcher/polling_path_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5203 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/watcher/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 06:54:55.845885 streamlit_nightly-1.35.1.dev20240523/streamlit/web/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14233 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/web/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/web/cache_storage_manager_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11321 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/web/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 06:54:55.845885 streamlit_nightly-1.35.1.dev20240523/streamlit/web/server/
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/web/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/web/server/app_static_file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7971 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/web/server/browser_websocket_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/web/server/component_request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5270 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/web/server/media_file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9972 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/web/server/routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14834 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/web/server/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/web/server/server_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/web/server/stats_request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/web/server/upload_file_request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/streamlit/web/server/websocket_headers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 06:54:55.849885 streamlit_nightly-1.35.1.dev20240523/streamlit_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8500 2024-05-24 06:54:54.000000 streamlit_nightly-1.35.1.dev20240523/streamlit_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    23316 2024-05-24 06:54:54.000000 streamlit_nightly-1.35.1.dev20240523/streamlit_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 06:54:54.000000 streamlit_nightly-1.35.1.dev20240523/streamlit_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-24 06:54:54.000000 streamlit_nightly-1.35.1.dev20240523/streamlit_nightly.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 06:51:07.000000 streamlit_nightly-1.35.1.dev20240523/streamlit_nightly.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-24 06:54:54.000000 streamlit_nightly-1.35.1.dev20240523/streamlit_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-24 06:54:54.000000 streamlit_nightly-1.35.1.dev20240523/streamlit_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 06:54:55.849885 streamlit_nightly-1.35.1.dev20240523/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-05-24 06:49:23.000000 streamlit_nightly-1.35.1.dev20240523/tests/testutil.py
```

### Comparing `streamlit_nightly-1.34.1.dev20240522/PKG-INFO` & `streamlit_nightly-1.35.1.dev20240523/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-nightly
-Version: 1.34.1.dev20240522
+Version: 1.35.1.dev20240523
 Summary: A faster way to build and share data apps
 Home-page: https://streamlit.io
 Author: Snowflake Inc
 Author-email: hello@streamlit.io
 License: Apache License 2.0
 Project-URL: Source Code, https://github.com/streamlit/streamlit
 Project-URL: Bug Tracker, https://github.com/streamlit/streamlit/issues
```

### Comparing `streamlit_nightly-1.34.1.dev20240522/bin/streamlit.cmd` & `streamlit_nightly-1.35.1.dev20240523/bin/streamlit.cmd`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/setup.py` & `streamlit_nightly-1.35.1.dev20240523/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from pathlib import Path
 
 from setuptools import find_packages, setup
 from setuptools.command.install import install
 
 THIS_DIRECTORY = Path(__file__).parent
 
-VERSION = "1.34.1.dev20240522"  # PEP-440
+VERSION = "1.35.1.dev20240523"  # PEP-440
 
 # IMPORTANT: We should try very hard *not* to add dependencies to Streamlit.
 # And if you do add one, make the required version as general as possible:
 # - Include relevant lower bound for any features we use from our dependencies
 # - Always include the lower bound as >= VERSION, to keep testing min versions easy
 # - And include an upper bound that's < NEXT_MAJOR_VERSION
 INSTALL_REQUIRES = [
```

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/__init__.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/__main__.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/__main__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/case_converters.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/case_converters.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/cli_util.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/cli_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/code_util.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/code_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/color_util.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/color_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/column_config.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/column_config.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/commands/__init__.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/commands/execution_control.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/commands/execution_control.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/commands/experimental_query_params.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/commands/experimental_query_params.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/commands/logo.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/net_util.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,100 +8,119 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Handle App logos"""
-
 from __future__ import annotations
 
-from typing import TYPE_CHECKING
+from typing import Final
 
-from streamlit import url_util
-from streamlit.elements.image import AtomicImage, WidthBehaviour, image_to_url
-from streamlit.errors import StreamlitAPIException
-from streamlit.proto.ForwardMsg_pb2 import ForwardMsg
-from streamlit.runtime.metrics_util import gather_metrics
-from streamlit.runtime.scriptrunner import get_script_run_ctx
-
-if TYPE_CHECKING:
-    from PIL import Image
-
-
-def _invalid_logo_text(field_name: str):
-    return f"The {field_name} passed to st.logo is invalid - See [documentation](https://docs.streamlit.io/develop/api-reference/media/st.logo) for more information on valid types"
-
-
-@gather_metrics("logo")
-def logo(
-    image: AtomicImage,
-    *,  # keyword-only args:
-    link: str | None = None,
-    icon_image: AtomicImage | None = None,
-) -> None:
-    """
-    Renders logos in the main and sidebar sections of the page
+from streamlit import util
+from streamlit.logger import get_logger
+
+_LOGGER: Final = get_logger(__name__)
+
+# URLs for checking the current machine's external IP address.
+_AWS_CHECK_IP: Final = "http://checkip.amazonaws.com"
+_AWS_CHECK_IP_HTTPS: Final = "https://checkip.amazonaws.com"
 
-    Parameters
-    ----------
-    image: Anything supported by st.image or str
-        The app logo to be displayed in the top left corner of the sidebar of your app
-        (as well as the main section if icon_image param is not provided).
-    link : str or None
-        The external url to be opened when a user clicks on the logo (must start with
-        http:// or https://)
-    icon_image: numpy.ndarray, BytesIO, str, or None
-        The app logo to be displayed in the top left corner of the main section of your
-        app.
+_external_ip: str | None = None
+_internal_ip: str | None = None
 
-    Example
+
+def get_external_ip() -> str | None:
+    """Get the *external* IP address of the current machine.
+
+    Returns
     -------
-    >>> import streamlit as st
-    >>>
-    >>> st.logo(streamlit_full, link="https://streamlit.io/gallery", icon_image=streamlit_small)
+    string
+        The external IPv4 address of the current machine.
+
     """
+    global _external_ip
 
-    ctx = get_script_run_ctx()
-    if ctx is None:
-        return
+    if _external_ip is not None:
+        return _external_ip
 
-    fwd_msg = ForwardMsg()
+    response = _make_blocking_http_get(_AWS_CHECK_IP, timeout=5)
 
-    try:
-        image_url = image_to_url(
-            image,
-            width=WidthBehaviour.AUTO,
-            clamp=False,
-            channels="RGB",
-            output_format="auto",
-            image_id="logo",
+    if response is None:
+        response = _make_blocking_http_get(_AWS_CHECK_IP_HTTPS, timeout=5)
+
+    if _looks_like_an_ip_adress(response):
+        _external_ip = response
+    else:
+        _LOGGER.warning(
+            # fmt: off
+            "Did not auto detect external IP.\n"
+            "Please go to %s for debugging hints.",
+            # fmt: on
+            util.HELP_DOC
         )
-        fwd_msg.logo.image = image_url
-    except Exception:
-        raise StreamlitAPIException(_invalid_logo_text("image"))
+        _external_ip = None
+
+    return _external_ip
+
+
+def get_internal_ip() -> str | None:
+    """Get the *local* IP address of the current machine.
 
-    if link:
-        # Handle external links:
-        if url_util.is_url(link, ("http", "https")):
-            fwd_msg.logo.link = link
-        else:
-            raise StreamlitAPIException(
-                f"Invalid link: {link} - the link param supports external links only and must start with either http:// or https://."
-            )
+    From: https://stackoverflow.com/a/28950776
+
+    Returns
+    -------
+    string
+        The local IPv4 address of the current machine.
+
+    """
+    global _internal_ip
 
-    if icon_image:
+    if _internal_ip is not None:
+        return _internal_ip
+
+    import socket
+
+    with socket.socket(socket.AF_INET, socket.SOCK_DGRAM) as s:
         try:
-            icon_image_url = image_to_url(
-                icon_image,
-                width=WidthBehaviour.AUTO,
-                clamp=False,
-                channels="RGB",
-                output_format="auto",
-                image_id="icon-image",
-            )
-            fwd_msg.logo.icon_image = icon_image_url
+            # Doesn't even have to be reachable
+            s.connect(("8.8.8.8", 1))
+            _internal_ip = s.getsockname()[0]
         except Exception:
-            raise StreamlitAPIException(_invalid_logo_text("icon_image"))
+            _internal_ip = "127.0.0.1"
+
+    return _internal_ip
+
+
+def _make_blocking_http_get(url: str, timeout: float = 5) -> str | None:
+    import requests
+
+    try:
+        text = requests.get(url, timeout=timeout).text
+        if isinstance(text, str):
+            text = text.strip()
+        return text
+    except Exception:
+        return None
+
+
+def _looks_like_an_ip_adress(address: str | None) -> bool:
+    if address is None:
+        return False
+
+    import socket
+
+    try:
+        socket.inet_pton(socket.AF_INET, address)
+        return True  # Yup, this is an IPv4 address!
+    except (AttributeError, OSError):
+        pass
+
+    try:
+        socket.inet_pton(socket.AF_INET6, address)
+        return True  # Yup, this is an IPv6 address!
+    except (AttributeError, OSError):
+        pass
 
-    ctx.enqueue(fwd_msg)
+    # Nope, this is not an IP address.
+    return False
```

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/commands/page_config.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/commands/page_config.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/components/__init__.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/components/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/components/lib/__init__.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/components/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/components/lib/local_component_registry.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/components/lib/local_component_registry.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/components/types/__init__.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/components/types/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/components/types/base_component_registry.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/components/types/base_component_registry.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/components/types/base_custom_component.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/components/types/base_custom_component.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/components/v1/__init__.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/components/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/components/v1/component_arrow.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/components/v1/component_arrow.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/components/v1/component_registry.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/components/v1/component_registry.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/components/v1/components.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/components/v1/components.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/components/v1/custom_component.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/components/v1/custom_component.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/config.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -339,14 +339,22 @@
     deprecated=True,
     deprecation_text="global.logLevel has been replaced with logger.level",
     expiration_date="2020-11-30",
     replaced_by="logger.level",
 )
 
 _create_option(
+    "global.e2eTest",
+    description="Are we in an e2e (playwright) test? Set automatically when our e2e tests are running.",
+    visibility="hidden",
+    default_val=False,
+    type_=bool,
+)
+
+_create_option(
     "global.unitTest",
     description="Are we in a unit test?",
     visibility="hidden",
     default_val=False,
     type_=bool,
 )
```

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/config_option.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/config_option.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/config_util.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/config_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/connections/__init__.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/connections/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/connections/base_connection.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/connections/base_connection.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/connections/snowflake_connection.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/connections/snowflake_connection.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/connections/snowpark_connection.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/connections/snowpark_connection.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/connections/sql_connection.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/connections/sql_connection.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/connections/util.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/connections/util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/constants.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/constants.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/cursor.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/cursor.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/delta_generator.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/delta_generator.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/deprecation_util.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/deprecation_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/development.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/development.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/echo.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/echo.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/__init__.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/elements/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/alert.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/elements/alert.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/arrow.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/elements/arrow.py`

 * *Files 11% similar despite different names*

```diff
@@ -81,36 +81,78 @@
     "single-column",
     "multi-column",
 }
 
 
 class DataframeSelectionState(TypedDict, total=False):
     """
-    A dictionary representing the current selection state of the dataframe.
+    The schema for the dataframe selection state.
+
+    The selection state is stored in a dictionary-like object that suports both
+    key and attribute notation. Selection states cannot be programmatically
+    changed or set through Session State.
 
     Attributes
     ----------
-    rows
-        The selected rows (numerical indices).
-    columns
-        The selected columns (column names).
+    rows : list[int]
+        The selected rows, identified by their positional index. The positional
+        indices match the original dataframe, even if the user sorts the
+        dataframe in their browser.
+    columns : list[str]
+        The selected columns, identified by their names.
+
+    Example
+    -------
+    The following example has multi-row and multi-column selections enabled.
+    Try selecting some rows. To select multiple columns, hold ``Ctrl`` while
+    selecting columns. Hold ``Shift`` to select a range of columns.
+
+    >>> import streamlit as st
+    >>> import pandas as pd
+    >>> import numpy as np
+    >>>
+    >>> if "df" not in st.session_state:
+    >>>     st.session_state.df = pd.DataFrame(
+    ...         np.random.randn(12, 5), columns=["a", "b", "c", "d", "e"]
+    ...     )
+    >>>
+    >>> event = st.dataframe(
+    ...     st.session_state.df,
+    ...     key="data",
+    ...     on_select="rerun",
+    ...     selection_mode=["multi-row", "multi-column"],
+    ... )
+    >>>
+    >>> event.selection
+
+    .. output::
+        https://doc-dataframe-events-selection-state.streamlit.app
+        height: 600px
+
     """
 
     rows: list[int]
     columns: list[str]
 
 
 class DataframeState(TypedDict, total=False):
     """
-    A dictionary representing the current state of the dataframe.
+    The schema for the dataframe event state.
+
+    The event state is stored in a dictionary-like object that suports both
+    key and attribute notation. Event states cannot be programmatically
+    changed or set through Session State.
+
+    Only selection events are supported at this time.
 
     Attributes
     ----------
     selection : DataframeSelectionState
-        The state of the `on_select` event.
+        The state of the ``on_select`` event.
+
     """
 
     selection: DataframeSelectionState
 
 
 @dataclass
 class DataframeSelectionSerde:
@@ -230,112 +272,165 @@
 
         This command works with dataframes from Pandas, PyArrow, Snowpark, and PySpark.
         It can also display several other types that can be converted to dataframes,
         e.g. numpy arrays, lists, sets and dictionaries.
 
         Parameters
         ----------
-        data : pandas.DataFrame, pandas.Series, pandas.Styler, pandas.Index, pyarrow.Table, numpy.ndarray, pyspark.sql.DataFrame, snowflake.snowpark.dataframe.DataFrame, snowflake.snowpark.table.Table, Iterable, dict, or None
+        data : pandas.DataFrame, pandas.Series, pandas.Styler, pandas.Index, \
+            pyarrow.Table, numpy.ndarray, pyspark.sql.DataFrame, snowflake.snowpark.dataframe.DataFrame, \
+            snowflake.snowpark.table.Table, Iterable, dict, or None
             The data to display.
 
-            If 'data' is a pandas.Styler, it will be used to style its
-            underlying DataFrame. Streamlit supports custom cell
+            If ``data`` is a ``pandas.Styler``, it will be used to style its
+            underlying ``pandas.DataFrame``. Streamlit supports custom cell
             values and colors. It does not support some of the more exotic
             pandas styling features, like bar charts, hovering, and captions.
 
         width : int or None
-            Desired width of the dataframe expressed in pixels. If None, the width
-            will be automatically calculated based on the column content.
+            Desired width of the dataframe expressed in pixels. If ``width`` is
+            ``None`` (default), Streamlit sets the dataframe width to fit its
+            contents up to the width of the parent container. If ``width`` is
+            greater than the width of the parent container, Streamlit sets the
+            dataframe width to match the width of the parent container.
 
         height : int or None
-            Desired height of the dataframe expressed in pixels. If None, a
-            default height is used.
+            Desired height of the dataframe expressed in pixels. If ``height``
+            is ``None`` (default), Streamlit sets the height to show at most
+            ten rows. Vertical scrolling within the dataframe element is
+            enabled when the height does not accomodate all rows.
 
         use_container_width : bool
-            If True, set the dataframe width to the width of the parent container.
-            This takes precedence over the width argument.
+            Whether to override ``width`` with the width of the parent
+            container. If ``use_container_width`` is ``False`` (default),
+            Streamlit sets the dataframe's width according to ``width``. If
+            ``use_container_width`` is ``True``, Streamlit sets the width of
+            the dataframe to match the width of the parent container.
 
         hide_index : bool or None
-            Whether to hide the index column(s). If None (default), the visibility of
-            index columns is automatically determined based on the data.
+            Whether to hide the index column(s). If ``hide_index`` is ``None``
+            (default), the visibility of index columns is automatically
+            determined based on the data.
 
         column_order : Iterable of str or None
-            Specifies the display order of columns. This also affects which columns are
-            visible. For example, ``column_order=("col2", "col1")`` will display 'col2'
-            first, followed by 'col1', and will hide all other non-index columns. If
-            None (default), the order is inherited from the original data structure.
+            The ordered list of columns to display. If ``column_order`` is
+            ``None`` (default), Streamlit displays all columns in the order
+            inherited from the underlying data structure. If ``column_order``
+            is a list, the indicated columns will display in the order they
+            appear within the list. Columns may be omitted or repeated within
+            the list.
+
+            For example, ``column_order=("col2", "col1")`` will display
+            ``"col2"`` first, followed by ``"col1"``, and will hide all other
+            non-index columns.
 
         column_config : dict or None
-            Configures how columns are displayed, e.g. their title, visibility, type, or
-            format. This needs to be a dictionary where each key is a column name and
-            the value is one of:
-
-            * ``None`` to hide the column.
-
-            * A string to set the display label of the column.
-
-            * One of the column types defined under ``st.column_config``, e.g.
-              ``st.column_config.NumberColumn("Dollar values”, format=”$ %d")`` to show
-              a column as dollar amounts. See more info on the available column types
-              and config options `here <https://docs.streamlit.io/library/api-reference/data/st.column_config>`_.
+            Configuration to customize how columns display. If ``column_config``
+            is ``None`` (default), columns are styled based on the underlying
+            data type of each column.
+
+            Column configuration can modify column names, visibility, type,
+            width, or format, among other things. ``column_config`` must be a
+            dictionary where each key is a column name and the associated value
+            is one of the following:
+
+            * ``None``: Streamlit hides the column.
+
+            * A string: Streamlit changes the display label of the column to
+              the given string.
+
+            * A column type within ``st.column_config``: Streamlit applies the
+              defined configuration to the column. For example, use
+              ``st.column_config.NumberColumn("Dollar values”, format=”$ %d")``
+              to change the displayed name of the column to "Dollar values"
+              and add a "$" prefix in each cell. For more info on the
+              available column types and config options, see
+              `Column configuration <https://docs.streamlit.io/library/api-reference/data/st.column_config>`_.
 
             To configure the index column(s), use ``_index`` as the column name.
 
         key : str
-            An optional string to use as the unique key for this element when used in combination
-            with ```on_select```. If this is omitted, a key will be generated for the widget based
-            on its content. Multiple widgets of the same type may not share the same key.
+            An optional string to use for giving this element a stable
+            identity. If ``key`` is ``None`` (default), this element's identity
+            will be determined based on the values of the other parameters.
+
+            Additionally, if selections are activated and ``key`` is provided,
+            Streamlit will register the key in Session State to store the
+            selection state. The selection state is read-only.
 
         on_select : "ignore" or "rerun" or callable
-            Controls the behavior in response to selection events on the table. Can be one of:
-
-            - "ignore" (default): Streamlit will not react to any selection events in the chart.
-            - "rerun": Streamlit will rerun the app when the user selects rows or columns in the table.
-              In this case, ```st.dataframe``` will return the selection data as a dictionary.
-            - callable: If a callable is provided, Streamlit will rerun and execute the callable as a
-              callback function before the rest of the app. The selection data can be retrieved through
-              session state by setting the key parameter.
-
-        selection_mode : "single-row", "multi-row", single-column", "multi-column", or an iterable of these
-            The selection mode of the table. Can be one of:
+            How the dataframe should respond to user selection events. This
+            controls whether or not the dataframe behaves like an input widget.
+            ``on_select`` can be one of the following:
+
+            - ``"ignore"`` (default): Streamlit will not react to any selection
+              events in the dataframe. The dataframe will not behave like an
+              input widget.
+
+            - ``"rerun"``: Streamlit will rerun the app when the user selects
+              rows or columns in the dataframe. In this case, ``st.dataframe``
+              will return the selection data as a dictionary.
+
+            - A ``callable``: Streamlit will rerun the app and execute the
+              ``callable`` as a callback function before the rest of the app.
+              In this case, ``st.dataframe`` will return the selection data
+              as a dictionary.
+
+        selection_mode : "single-row", "multi-row", single-column", \
+            "multi-column", or Iterable of these
+            The types of selections Streamlit should allow. This can be one of
+            the following:
 
             - "multi-row" (default): Multiple rows can be selected at a time.
             - "single-row": Only one row can be selected at a time.
             - "multi-column": Multiple columns can be selected at a time.
             - "single-column": Only one column can be selected at a time.
-            - An iterable of the above options: The table will allow selection based on the modes specified.
+            - An ``Iterable`` of the above options: The table will allow
+              selection based on the modes specified.
+
+            When column selections are enabled, column sorting is disabled.
+
+        Returns
+        -------
+        element or dict
+            If ``on_select`` is ``"ignore"`` (default), this method returns an
+            internal placeholder for the dataframe element that can be used
+            with the ``.add_rows()`` method. Otherwise, this method returns a
+            dictionary-like object that supports both key and attribute
+            notation. The attributes are described by the ``DataframeState``
+            dictionary schema.
 
         Examples
         --------
         >>> import streamlit as st
         >>> import pandas as pd
         >>> import numpy as np
         >>>
         >>> df = pd.DataFrame(np.random.randn(50, 20), columns=("col %d" % i for i in range(20)))
         >>>
         >>> st.dataframe(df)  # Same as st.write(df)
 
         .. output::
            https://doc-dataframe.streamlit.app/
-           height: 410px
+           height: 500px
 
         You can also pass a Pandas Styler object to change the style of
         the rendered DataFrame:
 
         >>> import streamlit as st
         >>> import pandas as pd
         >>> import numpy as np
         >>>
         >>> df = pd.DataFrame(np.random.randn(10, 20), columns=("col %d" % i for i in range(20)))
         >>>
         >>> st.dataframe(df.style.highlight_max(axis=0))
 
         .. output::
            https://doc-dataframe1.streamlit.app/
-           height: 410px
+           height: 500px
 
         Or you can customize the dataframe via ``column_config``, ``hide_index``, or ``column_order``:
 
         >>> import random
         >>> import pandas as pd
         >>> import streamlit as st
         >>>
```

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/balloons.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/elements/balloons.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/bokeh_chart.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/elements/bokeh_chart.py`

 * *Files 10% similar despite different names*

```diff
@@ -39,28 +39,32 @@
         self,
         figure: Figure,
         use_container_width: bool = False,
     ) -> DeltaGenerator:
         """Display an interactive Bokeh chart.
 
         Bokeh is a charting library for Python. The arguments to this function
-        closely follow the ones for Bokeh's `show` function. You can find
+        closely follow the ones for Bokeh's ``show`` function. You can find
         more about Bokeh at https://bokeh.pydata.org.
 
-        To show Bokeh charts in Streamlit, call `st.bokeh_chart`
-        wherever you would call Bokeh's `show`.
+        To show Bokeh charts in Streamlit, call ``st.bokeh_chart``
+        wherever you would call Bokeh's ``show``.
 
         Parameters
         ----------
         figure : bokeh.plotting.figure.Figure
             A Bokeh figure to plot.
 
         use_container_width : bool
-            If True, set the chart width to the column width. This takes
-            precedence over Bokeh's native `width` value.
+            Whether to override the figure's native width with the width of
+            the parent container. If ``use_container_width`` is ``False``
+            (default), Streamlit sets the width of the chart to fit its contents
+            according to the plotting library, up to the width of the parent
+            container. If ``use_container_width`` is ``True``, Streamlit sets
+            the width of the figure to match the width of the parent container.
 
         Example
         -------
         >>> import streamlit as st
         >>> from bokeh.plotting import figure
         >>>
         >>> x = [1, 2, 3, 4, 5]
```

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/code.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/elements/code.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/deck_gl_json_chart.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/elements/deck_gl_json_chart.py`

 * *Files 8% similar despite different names*

```diff
@@ -69,14 +69,20 @@
         https://docs.streamlit.io/library/advanced-features/configuration
 
         Parameters
         ----------
         pydeck_obj: pydeck.Deck or None
             Object specifying the PyDeck chart to draw.
         use_container_width: bool
+            Whether to override the figure's native width with the width of
+            the parent container. If ``use_container_width`` is ``False``
+            (default), Streamlit sets the width of the chart to fit its contents
+            according to the plotting library, up to the width of the parent
+            container. If ``use_container_width`` is ``True``, Streamlit sets
+            the width of the figure to match the width of the parent container.
 
         Example
         -------
         Here's a chart using a HexagonLayer and a ScatterplotLayer. It uses either the
         light or dark map style, based on which Streamlit theme is currently active:
 
         >>> import streamlit as st
```

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/dialog_decorator.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/elements/dialog_decorator.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/doc_string.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/elements/doc_string.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/empty.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/elements/empty.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/exception.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/elements/exception.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/form.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/elements/form.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/graphviz_chart.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/elements/graphviz_chart.py`

 * *Files 7% similar despite different names*

```diff
@@ -46,16 +46,20 @@
 
         Parameters
         ----------
         figure_or_dot : graphviz.dot.Graph, graphviz.dot.Digraph, str
             The Graphlib graph object or dot string to display
 
         use_container_width : bool
-            If True, set the chart width to the column width. This takes
-            precedence over the figure's native `width` value.
+            Whether to override the figure's native width with the width of
+            the parent container. If ``use_container_width`` is ``False``
+            (default), Streamlit sets the width of the chart to fit its contents
+            according to the plotting library, up to the width of the parent
+            container. If ``use_container_width`` is ``True``, Streamlit sets
+            the width of the figure to match the width of the parent container.
 
         Example
         -------
         >>> import streamlit as st
         >>> import graphviz
         >>>
         >>> # Create a graphlib graph object
```

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/heading.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/elements/heading.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/html.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/elements/html.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/iframe.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/elements/iframe.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/image.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/elements/image.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/json.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/elements/json.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/layouts.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/elements/layouts.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/lib/__init__.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/elements/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/lib/built_in_chart_utils.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/elements/lib/built_in_chart_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,16 +114,16 @@
 def generate_chart(
     chart_type: ChartType,
     data: Data | None,
     x_from_user: str | None = None,
     y_from_user: str | Sequence[str] | None = None,
     color_from_user: str | Color | list[Color] | None = None,
     size_from_user: str | float | None = None,
-    width: int = 0,
-    height: int = 0,
+    width: int | None = None,
+    height: int | None = None,
 ) -> tuple[alt.Chart, AddRowsMetadata]:
     """Function to use the chart's type, data columns and indices to figure out the chart's spec."""
     import altair as alt
 
     df = type_util.convert_anything_to_df(data, ensure_copy=True)
 
     # From now on, use "df" instead of "data". Deleting "data" to guarantee we follow this.
@@ -163,16 +163,16 @@
 
     # At this point, x_column is only None if user did not provide one AND df is empty.
 
     # Create a Chart with x and y encodings.
     chart = alt.Chart(
         data=df,
         mark=chart_type.value["mark_type"],
-        width=width,
-        height=height,
+        width=width or 0,
+        height=height or 0,
     ).encode(
         x=_get_x_encoding(df, x_column, x_from_user, chart_type),
         y=_get_y_encoding(df, y_column, y_from_user),
     )
 
     # Set up opacity encoding.
     opacity_enc = _get_opacity_encoding(chart_type, color_column)
```

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/lib/column_config_utils.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/elements/lib/column_config_utils.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/lib/column_types.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/elements/lib/column_types.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/lib/dialog.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/elements/lib/dialog.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/lib/dicttools.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/elements/lib/dicttools.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/lib/event_utils.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/elements/lib/event_utils.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/lib/mutable_status_container.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/elements/lib/mutable_status_container.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/lib/pandas_styler_utils.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/elements/lib/pandas_styler_utils.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/lib/streamlit_plotly_theme.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/elements/lib/streamlit_plotly_theme.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/lib/subtitle_utils.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/elements/lib/subtitle_utils.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/map.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/elements/map.py`

 * *Files 4% similar despite different names*

```diff
@@ -162,16 +162,20 @@
               datapoint to be represented by a circle of a different size.
 
         zoom : int
             Zoom level as specified in
             https://wiki.openstreetmap.org/wiki/Zoom_levels.
 
         use_container_width: bool
-            If True, set the chart width to the column width. This takes
-            precedence over the width argument.
+            Whether to override the map's native width with the width of
+            the parent container. If ``use_container_width`` is ``False``
+            (default), Streamlit sets the width of the chart to fit its contents
+            according to the plotting library, up to the width of the parent
+            container. If ``use_container_width`` is ``True``, Streamlit sets
+            the width of the map to match the width of the parent container.
 
         Examples
         --------
         >>> import streamlit as st
         >>> import pandas as pd
         >>> import numpy as np
         >>>
```

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/markdown.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/elements/markdown.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/media.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/elements/media.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/metric.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/elements/metric.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/plotly_chart.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/elements/plotly_chart.py`

 * *Files 12% similar despite different names*

```diff
@@ -76,50 +76,135 @@
 
 SelectionMode: TypeAlias = Literal["lasso", "points", "box"]
 _SELECTION_MODES: Final[set[SelectionMode]] = {"lasso", "points", "box"}
 
 
 class PlotlySelectionState(TypedDict, total=False):
     """
-    A dictionary representing the current selection state of the plotly chart.
+    The schema for the Plotly chart selection state.
+
+    The selection state is stored in a dictionary-like object that suports both
+    key and attribute notation. Selection states cannot be programmatically
+    changed or set through Session State.
 
     Attributes
     ----------
     points : list[dict[str, Any]]
-        The selected data points in the chart, this also includes
-        the the data points selected by the box and lasso mode.
+        The selected data points in the chart, including the data points
+        selected by the box and lasso mode. The data includes the values
+        associated to each point and a point index used to populate
+        ``point_indices``. If additional information has been assigned to your
+        points, such as size or legend group, this is also included.
 
     point_indices : list[int]
-        The numerical indices of all selected data points in the chart,
-        this also includes the indices of the points selected by the box
-        and lasso mode.
+        The numerical indices of all selected data points in the chart. The
+        details of each identified point are included in ``points``.
 
     box : list[dict[str, Any]]
         The metadata related to the box selection. This includes the
         coordinates of the selected area.
 
     lasso : list[dict[str, Any]]
         The metadata related to the lasso selection. This includes the
         coordinates of the selected area.
+
+    Example
+    -------
+    When working with more complicated graphs, the ``points`` attribute
+    displays additional information. Try selecting points in the following
+    example:
+
+    >>> import streamlit as st
+    >>> import plotly.express as px
+    >>>
+    >>> df = px.data.iris()
+    >>> fig = px.scatter(
+    ...     df,
+    ...     x="sepal_width",
+    ...     y="sepal_length",
+    ...     color="species",
+    ...     size="petal_length",
+    ...     hover_data=["petal_width"],
+    ... )
+    >>>
+    >>> event = st.plotly_chart(fig, key="iris", on_select="rerun")
+    >>>
+    >>> event.selection
+
+    .. output::
+        https://doc-chart-events-plotly-selection-state.streamlit.app
+        height: 600px
+
+    This is an example of the selection state when selecting a single point:
+
+    >>> {
+    >>>   "points": [
+    >>>     {
+    >>>       "curve_number": 2,
+    >>>       "point_number": 9,
+    >>>       "point_index": 9,
+    >>>       "x": 3.6,
+    >>>       "y": 7.2,
+    >>>       "customdata": [
+    >>>         2.5
+    >>>       ],
+    >>>       "marker_size": 6.1,
+    >>>       "legendgroup": "virginica"
+    >>>     }
+    >>>   ],
+    >>>   "point_indices": [
+    >>>     9
+    >>>   ],
+    >>>   "box": [],
+    >>>   "lasso": []
+    >>> }
+
     """
 
     points: list[dict[str, Any]]
     point_indices: list[int]
     box: list[dict[str, Any]]
     lasso: list[dict[str, Any]]
 
 
 class PlotlyState(TypedDict, total=False):
     """
-    A dictionary representing the current selection state of the plotly chart.
+    The schema for the Plotly chart event state.
+
+    The event state is stored in a dictionary-like object that suports both
+    key and attribute notation. Event states cannot be programmatically
+    changed or set through Session State.
+
+    Only selection events are supported at this time.
 
     Attributes
     ----------
     selection : PlotlySelectionState
-        The state of the `on_select` event.
+        The state of the ``on_select`` event.
+
+    Example
+    -------
+    Try selecting points by any of the three available methods (direct click,
+    box, or lasso). The current selection state is available through Session
+    State or as the output of the chart function.
+
+    >>> import streamlit as st
+    >>> import plotly.express as px
+    >>>
+    >>> df = px.data.iris()  # iris is a pandas DataFrame
+    >>> fig = px.scatter(df, x="sepal_width", y="sepal_length")
+    >>>
+    >>> event = st.plotly_chart(fig, key="iris", on_select="rerun")
+    >>>
+    >>> event
+
+    .. output::
+        https://doc-chart-events-plotly-state.streamlit.app
+        height: 600px
+
     """
 
     selection: PlotlySelectionState
 
 
 @dataclass
 class PlotlyChartSelectionSerde:
@@ -220,66 +305,100 @@
         on_select: Literal["rerun", "ignore"] | WidgetCallback = "ignore",
         selection_mode: SelectionMode
         | Iterable[SelectionMode] = ("points", "box", "lasso"),
         **kwargs: Any,
     ) -> DeltaGenerator | PlotlyState:
         """Display an interactive Plotly chart.
 
-        Plotly is a charting library for Python. The arguments to this function
-        closely follow the ones for Plotly's `plot()` function. You can find
-        more about Plotly at https://plot.ly/python.
+        `Plotly <https://plot.ly/python>`_ is a charting library for Python.
+        The arguments to this function closely follow the ones for Plotly's
+        ``plot()`` function.
 
-        To show Plotly charts in Streamlit, call `st.plotly_chart` wherever you
-        would call Plotly's `py.plot` or `py.iplot`.
+        To show Plotly charts in Streamlit, call ``st.plotly_chart`` wherever
+        you would call Plotly's ``py.plot`` or ``py.iplot``.
 
         Parameters
         ----------
         figure_or_data : plotly.graph_objs.Figure, plotly.graph_objs.Data,\
-            dict/list of plotly.graph_objs.Figure/Data
+            or dict/list of plotly.graph_objs.Figure/Data
 
-            See https://plot.ly/python/ for examples of graph descriptions.
+            The Plotly ``Figure`` or ``Data`` object to render. See
+            https://plot.ly/python/ for examples of graph descriptions.
 
         use_container_width : bool
-            If True, set the chart width to the column width. This takes
-            precedence over the figure's native `width` value.
+            Whether to override the figure's native width with the width of
+            the parent container. If ``use_container_width`` is ``False``
+            (default), Streamlit sets the width of the chart to fit its contents
+            according to the plotting library, up to the width of the parent
+            container. If ``use_container_width`` is ``True``, Streamlit sets
+            the width of the figure to match the width of the parent container.
 
         theme : "streamlit" or None
-            The theme of the chart. Currently, we only support "streamlit" for the Streamlit
-            defined design or None to fallback to the default behavior of the library.
+            The theme of the chart. If ``theme`` is ``"streamlit"`` (default),
+            Streamlit uses its own design default. If ``theme`` is ``None``,
+            Streamlit falls back to the default behavior of the library.
 
         key : str
-            An optional string to use as the unique key for this element when used in combination
-            with ```on_select```. If this is omitted, a key will be generated for the widget based
-            on its content. Multiple widgets of the same type may not share the same key.
+            An optional string to use for giving this element a stable
+            identity. If ``key`` is ``None`` (default), this element's identity
+            will be determined based on the values of the other parameters.
+
+            Additionally, if selections are activated and ``key`` is provided,
+            Streamlit will register the key in Session State to store the
+            selection state. The selection state is read-only.
 
         on_select : "ignore" or "rerun" or callable
-            Controls the behavior in response to selection events on the charts. Can be one of:
-            - "ignore" (default): Streamlit will not react to any selection events in the chart.
-            - "rerun: Streamlit will rerun the app when the user selects data in the chart. In this case,
-              ```st.plotly_chart``` will return the selection data as a dictionary.
-            - callable: If a callable is provided, Streamlit will rerun and execute the callable as a
-              callback function before the rest of the app. The selection data can be retrieved through
-              session state by setting the key parameter.
-
-        selection_mode : "points", "box", "lasso" or an iterable of these
-            The selection mode of the table. Can be one of:
-            - "points": The chart will allow selections based on individual data points.
-            - "box": The chart will allow selections based on rectangular areas.
-            - "lasso": The chart will allow selections based on freeform areas.
-            - An iterable of the above options: The chart will allow selections based on the modes specified.
+            How the figure should respond to user selection events. This
+            controls whether or not the figure behaves like an input widget.
+            ``on_select`` can be one of the following:
+
+            - ``"ignore"`` (default): Streamlit will not react to any selection
+              events in the chart. The figure will not behave like an input
+              widget.
+
+            - ``"rerun"``: Streamlit will rerun the app when the user selects
+              data in the chart. In this case, ``st.plotly_chart`` will return
+              the selection data as a dictionary.
+
+            - A ``callable``: Streamlit will rerun the app and execute the
+              ``callable`` as a callback function before the rest of the app.
+              In this case, ``st.plotly_chart`` will return the selection data
+              as a dictionary.
+
+        selection_mode : "points", "box", "lasso" or an Iterable of these
+            The selection mode of the chart. This can be one of the following:
+
+            - ``"points"``: The chart will allow selections based on individual
+              data points.
+            - ``"box"``: The chart will allow selections based on rectangular
+              areas.
+            - ``"lasso"``: The chart will allow selections based on freeform
+              areas.
+            - An ``Iterable`` of the above options: The chart will allow
+              selections based on the modes specified.
 
             All selections modes are activated by default.
 
         **kwargs
-            Any argument accepted by Plotly's `plot()` function.
+            Any argument accepted by Plotly's ``plot()`` function.
+
+        Returns
+        -------
+        element or dict
+            If ``on_select`` is ``"ignore"`` (default), this method returns an
+            internal placeholder for the chart element. Otherwise, this method
+            returns a dictionary-like object that supports both key and
+            attribute notation. The attributes are described by the
+            ``PlotlyState`` dictionary schema.
 
         Example
         -------
         The example below comes straight from the examples at
-        https://plot.ly/python:
+        https://plot.ly/python. Note that ``plotly.figure_factory`` requires
+        ``scipy`` to run.
 
         >>> import streamlit as st
         >>> import numpy as np
         >>> import plotly.figure_factory as ff
         >>>
         >>> # Add histogram data
         >>> x1 = np.random.randn(200) - 2
@@ -296,15 +415,15 @@
         ...         hist_data, group_labels, bin_size=[.1, .25, .5])
         >>>
         >>> # Plot!
         >>> st.plotly_chart(fig, use_container_width=True)
 
         .. output::
            https://doc-plotly-chart.streamlit.app/
-           height: 400px
+           height: 550px
 
         """
         import plotly.io
         import plotly.tools
 
         # NOTE: "figure_or_data" is the name used in Plotly's .plot() method
         # for their main parameter. I don't like the name, but it's best to
```

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/progress.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/elements/progress.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/pyplot.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/elements/pyplot.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,23 +48,28 @@
             The figure to plot. When this argument isn't specified, this
             function will render the global figure (but this is deprecated,
             as described below)
 
         clear_figure : bool
             If True, the figure will be cleared after being rendered.
             If False, the figure will not be cleared after being rendered.
-            If left unspecified, we pick a default based on the value of `fig`.
+            If left unspecified, we pick a default based on the value of ``fig``.
 
-            * If `fig` is set, defaults to `False`.
+            * If ``fig`` is set, defaults to ``False``.
 
-            * If `fig` is not set, defaults to `True`. This simulates Jupyter's
+            * If ``fig`` is not set, defaults to ``True``. This simulates Jupyter's
               approach to matplotlib rendering.
 
         use_container_width : bool
-            If True, set the chart width to the column width. Defaults to `True`.
+            Whether to override the figure's native width with the width of
+            the parent container. If ``use_container_width`` is ``False``
+            (default), Streamlit sets the width of the chart to fit its contents
+            according to the plotting library, up to the width of the parent
+            container. If ``use_container_width`` is ``True``, Streamlit sets
+            the width of the figure to match the width of the parent container.
 
         **kwargs : any
             Arguments to pass to Matplotlib's savefig function.
 
         Example
         -------
         >>> import streamlit as st
```

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/snow.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/elements/snow.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/spinner.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/elements/spinner.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/text.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/elements/text.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/toast.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/elements/toast.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/utils.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/elements/utils.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/vega_charts.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/elements/vega_charts.py`

 * *Files 10% similar despite different names*

```diff
@@ -154,3490 +154,4222 @@
 00000990: 2263 6f6c 756d 6e22 2c0a 7d0a 0a56 6567  "column",.}..Veg
 000009a0: 614c 6974 6553 7065 633a 2054 7970 6541  aLiteSpec: TypeA
 000009b0: 6c69 6173 203d 2022 6469 6374 5b73 7472  lias = "dict[str
 000009c0: 2c20 416e 795d 220a 0a0a 636c 6173 7320  , Any]"...class 
 000009d0: 5665 6761 4c69 7465 5374 6174 6528 5479  VegaLiteState(Ty
 000009e0: 7065 6444 6963 742c 2074 6f74 616c 3d46  pedDict, total=F
 000009f0: 616c 7365 293a 0a20 2020 2022 2222 0a20  alse):.    """. 
-00000a00: 2020 2041 2064 6963 7469 6f6e 6172 7920     A dictionary 
-00000a10: 7265 7072 6573 656e 7469 6e67 2074 6865  representing the
-00000a20: 2063 7572 7265 6e74 2073 656c 6563 7469   current selecti
-00000a30: 6f6e 2073 7461 7465 206f 6620 7468 6520  on state of the 
-00000a40: 5665 6761 4c69 7465 2063 6861 7274 2e0a  VegaLite chart..
-00000a50: 2020 2020 4174 7472 6962 7574 6573 0a20      Attributes. 
-00000a60: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
-00000a70: 2020 7365 6c65 6374 696f 6e20 3a20 4174    selection : At
-00000a80: 7472 6962 7574 6544 6963 7469 6f6e 6172  tributeDictionar
-00000a90: 790a 2020 2020 2020 2020 5468 6520 7374  y.        The st
-00000aa0: 6174 6520 6f66 2074 6865 2060 6f6e 5f73  ate of the `on_s
-00000ab0: 656c 6563 7460 2065 7665 6e74 2e0a 2020  elect` event..  
-00000ac0: 2020 2222 220a 0a20 2020 2073 656c 6563    """..    selec
-00000ad0: 7469 6f6e 3a20 4174 7472 6962 7574 6544  tion: AttributeD
-00000ae0: 6963 7469 6f6e 6172 790a 0a0a 4064 6174  ictionary...@dat
-00000af0: 6163 6c61 7373 0a63 6c61 7373 2056 6567  aclass.class Veg
-00000b00: 614c 6974 6553 7461 7465 5365 7264 653a  aLiteStateSerde:
-00000b10: 0a20 2020 2022 2222 5665 6761 4c69 7465  .    """VegaLite
-00000b20: 5374 6174 6553 6572 6465 2069 7320 7573  StateSerde is us
-00000b30: 6564 2074 6f20 7365 7269 616c 697a 6520  ed to serialize 
-00000b40: 616e 6420 6465 7365 7269 616c 697a 6520  and deserialize 
-00000b50: 7468 6520 5665 6761 4c69 7465 2043 6861  the VegaLite Cha
-00000b60: 7274 2073 7461 7465 2e22 2222 0a0a 2020  rt state."""..  
-00000b70: 2020 7365 6c65 6374 696f 6e5f 7061 7261    selection_para
-00000b80: 6d65 7465 7273 3a20 5365 7175 656e 6365  meters: Sequence
-00000b90: 5b73 7472 5d0a 0a20 2020 2064 6566 2064  [str]..    def d
-00000ba0: 6573 6572 6961 6c69 7a65 2873 656c 662c  eserialize(self,
-00000bb0: 2075 695f 7661 6c75 653a 2073 7472 207c   ui_value: str |
-00000bc0: 204e 6f6e 652c 2077 6964 6765 745f 6964   None, widget_id
-00000bd0: 3a20 7374 7220 3d20 2222 2920 2d3e 2056  : str = "") -> V
-00000be0: 6567 614c 6974 6553 7461 7465 3a0a 2020  egaLiteState:.  
-00000bf0: 2020 2020 2020 656d 7074 795f 7365 6c65        empty_sele
-00000c00: 6374 696f 6e5f 7374 6174 653a 2056 6567  ction_state: Veg
-00000c10: 614c 6974 6553 7461 7465 203d 207b 0a20  aLiteState = {. 
-00000c20: 2020 2020 2020 2020 2020 2022 7365 6c65             "sele
-00000c30: 6374 696f 6e22 3a20 4174 7472 6962 7574  ction": Attribut
-00000c40: 6544 6963 7469 6f6e 6172 7928 0a20 2020  eDictionary(.   
-00000c50: 2020 2020 2020 2020 2020 2020 2023 2049               # I
-00000c60: 6e69 7469 616c 697a 6520 7468 6520 7365  nitialize the se
-00000c70: 6c65 6374 2073 7461 7465 2077 6974 6820  lect state with 
-00000c80: 656d 7074 7920 6469 6374 696f 6e61 7269  empty dictionari
-00000c90: 6573 2066 6f72 2065 6163 6820 7365 6c65  es for each sele
-00000ca0: 6374 696f 6e20 7061 7261 6d65 7465 722e  ction parameter.
-00000cb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000cc0: 207b 7061 7261 6d3a 207b 7d20 666f 7220   {param: {} for 
-00000cd0: 7061 7261 6d20 696e 2073 656c 662e 7365  param in self.se
-00000ce0: 6c65 6374 696f 6e5f 7061 7261 6d65 7465  lection_paramete
-00000cf0: 7273 7d0a 2020 2020 2020 2020 2020 2020  rs}.            
-00000d00: 292c 0a20 2020 2020 2020 207d 0a0a 2020  ),.        }..  
-00000d10: 2020 2020 2020 7365 6c65 6374 696f 6e5f        selection_
-00000d20: 7374 6174 6520 3d20 280a 2020 2020 2020  state = (.      
-00000d30: 2020 2020 2020 656d 7074 795f 7365 6c65        empty_sele
-00000d40: 6374 696f 6e5f 7374 6174 650a 2020 2020  ction_state.    
-00000d50: 2020 2020 2020 2020 6966 2075 695f 7661          if ui_va
-00000d60: 6c75 6520 6973 204e 6f6e 650a 2020 2020  lue is None.    
-00000d70: 2020 2020 2020 2020 656c 7365 2063 6173          else cas
-00000d80: 7428 5665 6761 4c69 7465 5374 6174 652c  t(VegaLiteState,
-00000d90: 2041 7474 7269 6275 7465 4469 6374 696f   AttributeDictio
-00000da0: 6e61 7279 286a 736f 6e2e 6c6f 6164 7328  nary(json.loads(
-00000db0: 7569 5f76 616c 7565 2929 290a 2020 2020  ui_value))).    
-00000dc0: 2020 2020 290a 0a20 2020 2020 2020 2069      )..        i
-00000dd0: 6620 2273 656c 6563 7469 6f6e 2220 6e6f  f "selection" no
-00000de0: 7420 696e 2073 656c 6563 7469 6f6e 5f73  t in selection_s
-00000df0: 7461 7465 3a0a 2020 2020 2020 2020 2020  tate:.          
-00000e00: 2020 7365 6c65 6374 696f 6e5f 7374 6174    selection_stat
-00000e10: 6520 3d20 656d 7074 795f 7365 6c65 6374  e = empty_select
-00000e20: 696f 6e5f 7374 6174 650a 0a20 2020 2020  ion_state..     
-00000e30: 2020 2072 6574 7572 6e20 6361 7374 2856     return cast(V
-00000e40: 6567 614c 6974 6553 7461 7465 2c20 4174  egaLiteState, At
-00000e50: 7472 6962 7574 6544 6963 7469 6f6e 6172  tributeDictionar
-00000e60: 7928 7365 6c65 6374 696f 6e5f 7374 6174  y(selection_stat
-00000e70: 6529 290a 0a20 2020 2064 6566 2073 6572  e))..    def ser
-00000e80: 6961 6c69 7a65 2873 656c 662c 2073 656c  ialize(self, sel
-00000e90: 6563 7469 6f6e 5f73 7461 7465 3a20 5665  ection_state: Ve
-00000ea0: 6761 4c69 7465 5374 6174 6529 202d 3e20  gaLiteState) -> 
-00000eb0: 7374 723a 0a20 2020 2020 2020 2072 6574  str:.        ret
-00000ec0: 7572 6e20 6a73 6f6e 2e64 756d 7073 2873  urn json.dumps(s
-00000ed0: 656c 6563 7469 6f6e 5f73 7461 7465 2c20  election_state, 
-00000ee0: 6465 6661 756c 743d 7374 7229 0a0a 0a64  default=str)...d
-00000ef0: 6566 205f 7072 6570 6172 655f 7665 6761  ef _prepare_vega
-00000f00: 5f6c 6974 655f 7370 6563 280a 2020 2020  _lite_spec(.    
-00000f10: 7370 6563 3a20 5665 6761 4c69 7465 5370  spec: VegaLiteSp
-00000f20: 6563 2c0a 2020 2020 7573 655f 636f 6e74  ec,.    use_cont
-00000f30: 6169 6e65 725f 7769 6474 683a 2062 6f6f  ainer_width: boo
-00000f40: 6c20 3d20 4661 6c73 652c 0a20 2020 202a  l = False,.    *
-00000f50: 2a6b 7761 7267 732c 0a29 202d 3e20 5665  *kwargs,.) -> Ve
-00000f60: 6761 4c69 7465 5370 6563 3a0a 2020 2020  gaLiteSpec:.    
-00000f70: 6966 206c 656e 286b 7761 7267 7329 3a0a  if len(kwargs):.
-00000f80: 2020 2020 2020 2020 2320 5375 7070 6f72          # Suppor
-00000f90: 7420 7061 7373 696e 6720 696e 206b 7761  t passing in kwa
-00000fa0: 7267 732e 2045 7861 6d70 6c65 3a0a 2020  rgs. Example:.  
-00000fb0: 2020 2020 2020 2320 2020 6d61 7273 6861        #   marsha
-00000fc0: 6c6c 2870 726f 746f 2c20 7b66 6f6f 3a20  ll(proto, {foo: 
-00000fd0: 2762 6172 277d 2c20 6261 7a3d 2762 6f7a  'bar'}, baz='boz
-00000fe0: 2729 0a20 2020 2020 2020 2023 204d 6572  ').        # Mer
-00000ff0: 6765 2073 7065 6320 7769 7468 2075 6e66  ge spec with unf
-00001000: 6c61 7474 656e 6564 206b 7761 7267 732c  lattened kwargs,
-00001010: 2077 6865 7265 206b 7761 7267 7320 7461   where kwargs ta
-00001020: 6b65 2070 7265 6365 6465 6e63 652e 0a20  ke precedence.. 
-00001030: 2020 2020 2020 2023 2054 6869 7320 6f6e         # This on
-00001040: 6c79 2077 6f72 6b73 2066 6f72 2073 7472  ly works for str
-00001050: 696e 6720 6b65 7973 2c20 6275 7420 6b77  ing keys, but kw
-00001060: 6172 6720 6b65 7973 2061 7265 2073 7472  arg keys are str
-00001070: 696e 6773 2061 6e79 7761 7973 2e0a 2020  ings anyways..  
-00001080: 2020 2020 2020 7370 6563 203d 2064 6963        spec = dic
-00001090: 7428 7370 6563 2c20 2a2a 6469 6374 746f  t(spec, **dictto
-000010a0: 6f6c 732e 756e 666c 6174 7465 6e28 6b77  ols.unflatten(kw
-000010b0: 6172 6773 2c20 5f43 4841 4e4e 454c 5329  args, _CHANNELS)
-000010c0: 290a 2020 2020 656c 7365 3a0a 2020 2020  ).    else:.    
-000010d0: 2020 2020 2320 436c 6f6e 6520 7468 6520      # Clone the 
-000010e0: 7370 6563 2064 6963 742c 2073 696e 6365  spec dict, since
-000010f0: 2077 6520 6d61 7920 6265 206d 7574 6174   we may be mutat
-00001100: 696e 6720 6974 2e0a 2020 2020 2020 2020  ing it..        
-00001110: 7370 6563 203d 2064 6963 7428 7370 6563  spec = dict(spec
-00001120: 290a 0a20 2020 2069 6620 6c65 6e28 7370  )..    if len(sp
-00001130: 6563 2920 3d3d 2030 3a0a 2020 2020 2020  ec) == 0:.      
-00001140: 2020 7261 6973 6520 5374 7265 616d 6c69    raise Streamli
-00001150: 7441 5049 4578 6365 7074 696f 6e28 2256  tAPIException("V
-00001160: 6567 612d 4c69 7465 2063 6861 7274 7320  ega-Lite charts 
-00001170: 7265 7175 6972 6520 6120 6e6f 6e2d 656d  require a non-em
-00001180: 7074 7920 7370 6563 2064 6963 742e 2229  pty spec dict.")
-00001190: 0a0a 2020 2020 6966 2022 6175 746f 7369  ..    if "autosi
-000011a0: 7a65 2220 6e6f 7420 696e 2073 7065 633a  ze" not in spec:
-000011b0: 0a20 2020 2020 2020 2023 2074 7970 6520  .        # type 
-000011c0: 6669 7420 646f 6573 206e 6f74 2077 6f72  fit does not wor
-000011d0: 6b20 666f 7220 6d61 6e79 2063 6861 7274  k for many chart
-000011e0: 2074 7970 6573 2e20 5468 6973 2063 6861   types. This cha
-000011f0: 6e67 6520 666f 6375 7365 730a 2020 2020  nge focuses.    
-00001200: 2020 2020 2320 6f6e 2076 636f 6e63 6174      # on vconcat
-00001210: 2077 6974 6820 7573 655f 636f 6e74 6169   with use_contai
-00001220: 6e65 725f 7769 6474 683d 5472 7565 2061  ner_width=True a
-00001230: 7320 7468 6572 6520 6172 6520 756e 696e  s there are unin
-00001240: 7465 6e64 6564 0a20 2020 2020 2020 2023  tended.        #
-00001250: 2063 6f6e 7365 7175 656e 6365 7320 6f66   consequences of
-00001260: 2063 6861 6e67 696e 6720 7468 6520 6465   changing the de
-00001270: 6661 756c 7420 6175 746f 7369 7a65 2066  fault autosize f
-00001280: 6f72 2061 6c6c 2063 6861 7274 732e 0a20  or all charts.. 
-00001290: 2020 2020 2020 2023 2066 6974 2d78 2066         # fit-x f
-000012a0: 6974 7320 7468 6520 7769 6474 6820 616e  its the width an
-000012b0: 6420 6865 6967 6874 2063 616e 2062 6520  d height can be 
-000012c0: 6164 6a75 7374 6564 2e0a 2020 2020 2020  adjusted..      
-000012d0: 2020 6966 2022 7663 6f6e 6361 7422 2069    if "vconcat" i
-000012e0: 6e20 7370 6563 2061 6e64 2075 7365 5f63  n spec and use_c
-000012f0: 6f6e 7461 696e 6572 5f77 6964 7468 3a0a  ontainer_width:.
-00001300: 2020 2020 2020 2020 2020 2020 7370 6563              spec
-00001310: 5b22 6175 746f 7369 7a65 225d 203d 207b  ["autosize"] = {
-00001320: 2274 7970 6522 3a20 2266 6974 2d78 222c  "type": "fit-x",
-00001330: 2022 636f 6e74 6169 6e73 223a 2022 7061   "contains": "pa
-00001340: 6464 696e 6722 7d0a 2020 2020 2020 2020  dding"}.        
-00001350: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00001360: 2020 7370 6563 5b22 6175 746f 7369 7a65    spec["autosize
-00001370: 225d 203d 207b 2274 7970 6522 3a20 2266  "] = {"type": "f
-00001380: 6974 222c 2022 636f 6e74 6169 6e73 223a  it", "contains":
-00001390: 2022 7061 6464 696e 6722 7d0a 0a20 2020   "padding"}..   
-000013a0: 2072 6574 7572 6e20 7370 6563 0a0a 0a64   return spec...d
-000013b0: 6566 205f 7365 7269 616c 697a 655f 6461  ef _serialize_da
-000013c0: 7461 2864 6174 613a 2041 6e79 2920 2d3e  ta(data: Any) ->
-000013d0: 2062 7974 6573 3a0a 2020 2020 2222 2253   bytes:.    """S
-000013e0: 6572 6961 6c69 7a65 2074 6865 2061 6e79  erialize the any
-000013f0: 2074 7970 6520 6f66 2064 6174 6120 7374   type of data st
-00001400: 7275 6374 7572 6520 746f 2041 7272 6f77  ructure to Arrow
-00001410: 2049 5043 2066 6f72 6d61 7420 2862 7974   IPC format (byt
-00001420: 6573 292e 2222 220a 2020 2020 696d 706f  es).""".    impo
-00001430: 7274 2070 7961 7272 6f77 2061 7320 7061  rt pyarrow as pa
-00001440: 0a0a 2020 2020 6966 2069 7369 6e73 7461  ..    if isinsta
-00001450: 6e63 6528 6461 7461 2c20 7061 2e54 6162  nce(data, pa.Tab
-00001460: 6c65 293a 0a20 2020 2020 2020 2072 6574  le):.        ret
-00001470: 7572 6e20 7479 7065 5f75 7469 6c2e 7079  urn type_util.py
-00001480: 6172 726f 775f 7461 626c 655f 746f 5f62  arrow_table_to_b
-00001490: 7974 6573 2864 6174 6129 0a0a 2020 2020  ytes(data)..    
-000014a0: 6466 203d 2074 7970 655f 7574 696c 2e63  df = type_util.c
-000014b0: 6f6e 7665 7274 5f61 6e79 7468 696e 675f  onvert_anything_
-000014c0: 746f 5f64 6628 6461 7461 290a 2020 2020  to_df(data).    
-000014d0: 7265 7475 726e 2074 7970 655f 7574 696c  return type_util
-000014e0: 2e64 6174 615f 6672 616d 655f 746f 5f62  .data_frame_to_b
-000014f0: 7974 6573 2864 6629 0a0a 0a64 6566 205f  ytes(df)...def _
-00001500: 6d61 7273 6861 6c6c 5f63 6861 7274 5f64  marshall_chart_d
-00001510: 6174 6128 0a20 2020 2070 726f 746f 3a20  ata(.    proto: 
-00001520: 4172 726f 7756 6567 614c 6974 6543 6861  ArrowVegaLiteCha
-00001530: 7274 5072 6f74 6f2c 0a20 2020 2073 7065  rtProto,.    spe
-00001540: 633a 2056 6567 614c 6974 6553 7065 632c  c: VegaLiteSpec,
-00001550: 0a20 2020 2064 6174 613a 2044 6174 6120  .    data: Data 
-00001560: 3d20 4e6f 6e65 2c0a 2920 2d3e 204e 6f6e  = None,.) -> Non
-00001570: 653a 0a20 2020 2022 2222 4164 6473 2074  e:.    """Adds t
-00001580: 6865 2064 6174 6120 746f 2074 6865 2070  he data to the p
-00001590: 726f 746f 2061 6e64 2072 656d 6f76 6573  roto and removes
-000015a0: 2069 7420 6672 6f6d 2074 6865 2073 7065   it from the spe
-000015b0: 6320 6469 6374 2e0a 2020 2020 5468 6573  c dict..    Thes
-000015c0: 6520 6f70 6572 6174 696f 6e73 2077 696c  e operations wil
-000015d0: 6c20 6861 7070 656e 2069 6e2d 706c 6163  l happen in-plac
-000015e0: 652e 2222 220a 0a20 2020 2023 2050 756c  e."""..    # Pul
-000015f0: 6c20 6461 7461 206f 7574 206f 6620 7370  l data out of sp
-00001600: 6563 2064 6963 7420 7768 656e 2069 7427  ec dict when it'
-00001610: 7320 696e 2061 2027 6461 7461 7365 7473  s in a 'datasets
-00001620: 2720 6b65 793a 0a20 2020 2023 2020 2064  ' key:.    #   d
-00001630: 6174 6173 6574 733a 207b 666f 6f3a 2064  atasets: {foo: d
-00001640: 6631 5f62 7974 6573 2c20 6261 723a 2064  f1_bytes, bar: d
-00001650: 6632 5f62 7974 6573 7d2c 202e 2e2e 7d0a  f2_bytes}, ...}.
-00001660: 2020 2020 6966 2022 6461 7461 7365 7473      if "datasets
-00001670: 2220 696e 2073 7065 633a 0a20 2020 2020  " in spec:.     
-00001680: 2020 2066 6f72 2064 6174 6173 6574 5f6e     for dataset_n
-00001690: 616d 652c 2064 6174 6173 6574 5f64 6174  ame, dataset_dat
-000016a0: 6120 696e 2073 7065 635b 2264 6174 6173  a in spec["datas
-000016b0: 6574 7322 5d2e 6974 656d 7328 293a 0a20  ets"].items():. 
-000016c0: 2020 2020 2020 2020 2020 2064 6174 6173             datas
-000016d0: 6574 203d 2070 726f 746f 2e64 6174 6173  et = proto.datas
-000016e0: 6574 732e 6164 6428 290a 2020 2020 2020  ets.add().      
-000016f0: 2020 2020 2020 6461 7461 7365 742e 6e61        dataset.na
-00001700: 6d65 203d 2073 7472 2864 6174 6173 6574  me = str(dataset
-00001710: 5f6e 616d 6529 0a20 2020 2020 2020 2020  _name).         
-00001720: 2020 2064 6174 6173 6574 2e68 6173 5f6e     dataset.has_n
-00001730: 616d 6520 3d20 5472 7565 0a20 2020 2020  ame = True.     
-00001740: 2020 2020 2020 2023 2054 6865 2049 4420         # The ID 
-00001750: 7472 616e 7366 6f72 6d65 7220 2869 645f  transformer (id_
-00001760: 7472 616e 7366 6f72 6d20 6675 6e63 7469  transform functi
-00001770: 6f6e 2072 6567 6973 7465 7265 6420 6265  on registered be
-00001780: 666f 7265 2063 6f6e 7665 7273 696f 6e20  fore conversion 
-00001790: 746f 2064 6963 7429 0a20 2020 2020 2020  to dict).       
-000017a0: 2020 2020 2023 2061 6c72 6561 6479 2073       # already s
-000017b0: 6572 6961 6c69 7a65 7320 7468 6520 6461  erializes the da
-000017c0: 7461 2069 6e74 6f20 4172 726f 7720 4950  ta into Arrow IP
-000017d0: 4320 666f 726d 6174 2028 6279 7465 7329  C format (bytes)
-000017e0: 2077 6865 6e20 7468 6520 416c 7461 6972   when the Altair
-000017f0: 206f 626a 6563 740a 2020 2020 2020 2020   object.        
-00001800: 2020 2020 2320 6765 7473 2063 6f6e 7665      # gets conve
-00001810: 7274 6564 2069 6e74 6f20 7468 6520 7665  rted into the ve
-00001820: 6761 2d6c 6974 6520 7370 6563 2064 6963  ga-lite spec dic
-00001830: 742e 0a20 2020 2020 2020 2020 2020 2023  t..            #
-00001840: 2049 6620 6974 7320 616c 7265 6164 7920   If its already 
-00001850: 696e 2062 7974 6573 2c20 7765 2064 6f6e  in bytes, we don
-00001860: 2774 206e 6565 6420 746f 2073 6572 6961  't need to seria
-00001870: 6c69 7a65 2069 7420 6865 7265 2061 6761  lize it here aga
-00001880: 696e 2e0a 2020 2020 2020 2020 2020 2020  in..            
-00001890: 2320 5765 206a 7573 7420 6e65 6564 2074  # We just need t
-000018a0: 6f20 7061 7373 2074 6865 2064 6174 6120  o pass the data 
-000018b0: 696e 666f 726d 6174 696f 6e20 696e 746f  information into
-000018c0: 2074 6865 2063 6f72 7265 6374 2070 726f   the correct pro
-000018d0: 746f 2066 6965 6c64 732e 0a0a 2020 2020  to fields...    
-000018e0: 2020 2020 2020 2020 2320 544f 444f 286c          # TODO(l
-000018f0: 756b 6173 6d61 7375 6368 293a 2041 7265  ukasmasuch): Are
-00001900: 2074 6865 7265 2061 6e79 206f 7468 6572   there any other
-00001910: 2063 6173 6573 2077 6865 7265 2077 6520   cases where we 
-00001920: 6e65 6564 2074 6f20 7365 7269 616c 697a  need to serializ
-00001930: 6520 7468 6520 6461 7461 0a20 2020 2020  e the data.     
-00001940: 2020 2020 2020 2023 2020 2020 2020 2020         #        
-00001950: 2020 2020 2020 2020 2020 2020 6f72 2063              or c
-00001960: 616e 2077 6520 7265 6d6f 7665 2074 6865  an we remove the
-00001970: 205f 7365 7269 616c 697a 655f 6461 7461   _serialize_data
-00001980: 2068 6572 653f 0a20 2020 2020 2020 2020   here?.         
-00001990: 2020 2064 6174 6173 6574 2e64 6174 612e     dataset.data.
-000019a0: 6461 7461 203d 2028 0a20 2020 2020 2020  data = (.       
-000019b0: 2020 2020 2020 2020 2064 6174 6173 6574           dataset
-000019c0: 5f64 6174 610a 2020 2020 2020 2020 2020  _data.          
-000019d0: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
-000019e0: 6e63 6528 6461 7461 7365 745f 6461 7461  nce(dataset_data
-000019f0: 2c20 6279 7465 7329 0a20 2020 2020 2020  , bytes).       
-00001a00: 2020 2020 2020 2020 2065 6c73 6520 5f73           else _s
-00001a10: 6572 6961 6c69 7a65 5f64 6174 6128 6461  erialize_data(da
-00001a20: 7461 7365 745f 6461 7461 290a 2020 2020  taset_data).    
-00001a30: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00001a40: 2020 6465 6c20 7370 6563 5b22 6461 7461    del spec["data
-00001a50: 7365 7473 225d 0a0a 2020 2020 2320 5075  sets"]..    # Pu
-00001a60: 6c6c 2064 6174 6120 6f75 7420 6f66 2073  ll data out of s
-00001a70: 7065 6320 6469 6374 2077 6865 6e20 6974  pec dict when it
-00001a80: 2773 2069 6e20 6120 746f 702d 6c65 7665  's in a top-leve
-00001a90: 6c20 2764 6174 6127 206b 6579 3a0a 2020  l 'data' key:.  
-00001aa0: 2020 2320 2020 7b64 6174 613a 2064 667d    #   {data: df}
-00001ab0: 0a20 2020 2023 2020 207b 6461 7461 3a20  .    #   {data: 
-00001ac0: 7b76 616c 7565 733a 2064 662c 202e 2e2e  {values: df, ...
-00001ad0: 7d7d 0a20 2020 2023 2020 207b 6461 7461  }}.    #   {data
-00001ae0: 3a20 7b75 726c 3a20 2775 726c 277d 7d0a  : {url: 'url'}}.
-00001af0: 2020 2020 2320 2020 7b64 6174 613a 207b      #   {data: {
-00001b00: 6e61 6d65 3a20 2766 6f6f 277d 7d0a 2020  name: 'foo'}}.  
-00001b10: 2020 6966 2022 6461 7461 2220 696e 2073    if "data" in s
-00001b20: 7065 633a 0a20 2020 2020 2020 2064 6174  pec:.        dat
-00001b30: 615f 7370 6563 203d 2073 7065 635b 2264  a_spec = spec["d
-00001b40: 6174 6122 5d0a 0a20 2020 2020 2020 2069  ata"]..        i
-00001b50: 6620 6973 696e 7374 616e 6365 2864 6174  f isinstance(dat
-00001b60: 615f 7370 6563 2c20 6469 6374 293a 0a20  a_spec, dict):. 
-00001b70: 2020 2020 2020 2020 2020 2069 6620 2276             if "v
-00001b80: 616c 7565 7322 2069 6e20 6461 7461 5f73  alues" in data_s
-00001b90: 7065 633a 0a20 2020 2020 2020 2020 2020  pec:.           
-00001ba0: 2020 2020 2064 6174 6120 3d20 6461 7461       data = data
-00001bb0: 5f73 7065 635b 2276 616c 7565 7322 5d0a  _spec["values"].
-00001bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001bd0: 6465 6c20 7370 6563 5b22 6461 7461 225d  del spec["data"]
-00001be0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-00001bf0: 2020 2020 2020 2020 2020 2064 6174 6120             data 
-00001c00: 3d20 6461 7461 5f73 7065 630a 2020 2020  = data_spec.    
-00001c10: 2020 2020 2020 2020 6465 6c20 7370 6563          del spec
-00001c20: 5b22 6461 7461 225d 0a0a 2020 2020 6966  ["data"]..    if
-00001c30: 2064 6174 6120 6973 206e 6f74 204e 6f6e   data is not Non
-00001c40: 653a 0a20 2020 2020 2020 2070 726f 746f  e:.        proto
-00001c50: 2e64 6174 612e 6461 7461 203d 205f 7365  .data.data = _se
-00001c60: 7269 616c 697a 655f 6461 7461 2864 6174  rialize_data(dat
-00001c70: 6129 0a0a 0a64 6566 205f 636f 6e76 6572  a)...def _conver
-00001c80: 745f 616c 7461 6972 5f74 6f5f 7665 6761  t_altair_to_vega
-00001c90: 5f6c 6974 655f 7370 6563 2861 6c74 6169  _lite_spec(altai
-00001ca0: 725f 6368 6172 743a 2061 6c74 2e43 6861  r_chart: alt.Cha
-00001cb0: 7274 2920 2d3e 2056 6567 614c 6974 6553  rt) -> VegaLiteS
-00001cc0: 7065 633a 0a20 2020 2022 2222 436f 6e76  pec:.    """Conv
-00001cd0: 6572 7420 616e 2041 6c74 6169 7220 6368  ert an Altair ch
-00001ce0: 6172 7420 6f62 6a65 6374 2074 6f20 6120  art object to a 
-00001cf0: 5665 6761 2d4c 6974 6520 6368 6172 7420  Vega-Lite chart 
-00001d00: 7370 6563 2e22 2222 0a20 2020 2069 6d70  spec.""".    imp
-00001d10: 6f72 7420 616c 7461 6972 2061 7320 616c  ort altair as al
-00001d20: 740a 0a20 2020 2023 204e 6f72 6d61 6c6c  t..    # Normall
-00001d30: 7920 616c 7461 6972 5f63 6861 7274 2e74  y altair_chart.t
-00001d40: 6f5f 6469 6374 2829 2077 6f75 6c64 2074  o_dict() would t
-00001d50: 7261 6e73 666f 726d 2074 6865 2064 6174  ransform the dat
-00001d60: 6166 7261 6d65 2075 7365 6420 6279 2074  aframe used by t
-00001d70: 6865 0a20 2020 2023 2063 6861 7274 2069  he.    # chart i
-00001d80: 6e74 6f20 616e 2061 7272 6179 206f 6620  nto an array of 
-00001d90: 6469 6374 696f 6e61 7269 6573 2e20 546f  dictionaries. To
-00001da0: 2061 766f 6964 2074 6861 742c 2077 6520   avoid that, we 
-00001db0: 696e 7374 616c 6c20 610a 2020 2020 2320  install a.    # 
-00001dc0: 7472 616e 7366 6f72 6d65 7220 7468 6174  transformer that
-00001dd0: 2072 6570 6c61 6365 7320 6461 7461 7365   replaces datase
-00001de0: 7473 2077 6974 6820 6120 7265 6665 7265  ts with a refere
-00001df0: 6e63 6520 6279 2074 6865 206f 626a 6563  nce by the objec
-00001e00: 7420 6964 206f 660a 2020 2020 2320 7468  t id of.    # th
-00001e10: 6520 6461 7461 6672 616d 652e 2057 6520  e dataframe. We 
-00001e20: 7468 656e 2066 696c 6c20 696e 2074 6865  then fill in the
-00001e30: 2064 6174 6173 6574 206d 616e 7561 6c6c   dataset manuall
-00001e40: 7920 6c61 7465 7220 6f6e 2e0a 0a20 2020  y later on...   
-00001e50: 2064 6174 6173 6574 7320 3d20 7b7d 0a0a   datasets = {}..
-00001e60: 2020 2020 6465 6620 6964 5f74 7261 6e73      def id_trans
-00001e70: 666f 726d 2864 6174 6129 202d 3e20 6469  form(data) -> di
-00001e80: 6374 5b73 7472 2c20 7374 725d 3a0a 2020  ct[str, str]:.  
-00001e90: 2020 2020 2020 2222 2241 6c74 6169 7220        """Altair 
-00001ea0: 6461 7461 2074 7261 6e73 666f 726d 6572  data transformer
-00001eb0: 2074 6861 7420 7365 7269 616c 697a 6573   that serializes
-00001ec0: 2074 6865 2064 6174 612c 0a20 2020 2020   the data,.     
-00001ed0: 2020 2063 7265 6174 6573 2061 2073 7461     creates a sta
-00001ee0: 626c 6520 6e61 6d65 2062 6173 6564 206f  ble name based o
-00001ef0: 6e20 7468 6520 6861 7368 206f 6620 7468  n the hash of th
-00001f00: 6520 6461 7461 2c0a 2020 2020 2020 2020  e data,.        
-00001f10: 7374 6f72 6573 2074 6865 2062 7974 6573  stores the bytes
-00001f20: 2069 6e74 6f20 7468 6520 6461 7461 7365   into the datase
-00001f30: 7473 206d 6170 7069 6e67 2061 6e64 0a20  ts mapping and. 
-00001f40: 2020 2020 2020 2072 6574 7572 6e73 2074         returns t
-00001f50: 6869 7320 6e61 6d65 2074 6f20 6861 7665  his name to have
-00001f60: 2069 7420 6265 2075 7365 6420 696e 2041   it be used in A
-00001f70: 6c74 6169 722e 0a20 2020 2020 2020 2022  ltair..        "
-00001f80: 2222 0a20 2020 2020 2020 2023 2041 6c72  "".        # Alr
-00001f90: 6561 6479 2073 6572 6961 6c69 7a65 2074  eady serialize t
-00001fa0: 6865 2064 6174 6120 746f 2062 6520 6162  he data to be ab
-00001fb0: 6c65 2074 6f20 6372 6561 7465 2061 2073  le to create a s
-00001fc0: 7461 626c 650a 2020 2020 2020 2020 2320  table.        # 
-00001fd0: 6461 7461 7365 7420 6e61 6d65 3a0a 2020  dataset name:.  
-00001fe0: 2020 2020 2020 6461 7461 5f62 7974 6573        data_bytes
-00001ff0: 203d 205f 7365 7269 616c 697a 655f 6461   = _serialize_da
-00002000: 7461 2864 6174 6129 0a20 2020 2020 2020  ta(data).       
-00002010: 2023 2055 7365 2074 6865 206d 6435 2068   # Use the md5 h
-00002020: 6173 6820 6f66 2074 6865 2064 6174 6120  ash of the data 
-00002030: 6173 2074 6865 206e 616d 653a 0a20 2020  as the name:.   
-00002040: 2020 2020 2068 203d 2068 6173 686c 6962       h = hashlib
-00002050: 2e6e 6577 2822 6d64 3522 2c20 2a2a 4841  .new("md5", **HA
-00002060: 5348 4c49 425f 4b57 4152 4753 290a 2020  SHLIB_KWARGS).  
-00002070: 2020 2020 2020 682e 7570 6461 7465 2873        h.update(s
-00002080: 7472 2864 6174 615f 6279 7465 7329 2e65  tr(data_bytes).e
-00002090: 6e63 6f64 6528 2275 7466 2d38 2229 290a  ncode("utf-8")).
-000020a0: 2020 2020 2020 2020 6e61 6d65 203d 2068          name = h
-000020b0: 2e68 6578 6469 6765 7374 2829 0a0a 2020  .hexdigest()..  
-000020c0: 2020 2020 2020 6461 7461 7365 7473 5b6e        datasets[n
-000020d0: 616d 655d 203d 2064 6174 615f 6279 7465  ame] = data_byte
-000020e0: 730a 2020 2020 2020 2020 7265 7475 726e  s.        return
-000020f0: 207b 226e 616d 6522 3a20 6e61 6d65 7d0a   {"name": name}.
-00002100: 0a20 2020 2061 6c74 2e64 6174 615f 7472  .    alt.data_tr
-00002110: 616e 7366 6f72 6d65 7273 2e72 6567 6973  ansformers.regis
-00002120: 7465 7228 2269 6422 2c20 6964 5f74 7261  ter("id", id_tra
-00002130: 6e73 666f 726d 2920 2023 2074 7970 653a  nsform)  # type:
-00002140: 2069 676e 6f72 655b 6174 7472 2d64 6566   ignore[attr-def
-00002150: 696e 6564 2c75 6e75 7365 642d 6967 6e6f  ined,unused-igno
-00002160: 7265 5d0a 0a20 2020 2023 2054 6865 2064  re]..    # The d
-00002170: 6566 6175 6c74 2061 6c74 6169 7220 7468  efault altair th
-00002180: 656d 6520 6861 7320 736f 6d65 2077 6964  eme has some wid
-00002190: 7468 2f68 6569 6768 7420 6465 6661 756c  th/height defaul
-000021a0: 7473 2064 6566 696e 6564 0a20 2020 2023  ts defined.    #
-000021b0: 2077 6869 6368 2061 7265 206e 6f74 2075   which are not u
-000021c0: 7365 6675 6c20 666f 7220 5374 7265 616d  seful for Stream
-000021d0: 6c69 742e 2054 6865 7265 666f 7265 2c20  lit. Therefore, 
-000021e0: 7765 2063 6861 6e67 6520 7468 6520 7468  we change the th
-000021f0: 656d 6520 746f 0a20 2020 2023 2022 6e6f  eme to.    # "no
-00002200: 6e65 2220 746f 2061 766f 6964 2074 686f  ne" to avoid tho
-00002210: 7365 2064 6566 6175 6c74 732e 0a20 2020  se defaults..   
-00002220: 2077 6974 6820 616c 742e 7468 656d 6573   with alt.themes
-00002230: 2e65 6e61 626c 6528 226e 6f6e 6522 2920  .enable("none") 
-00002240: 6966 2061 6c74 2e74 6865 6d65 732e 6163  if alt.themes.ac
-00002250: 7469 7665 203d 3d20 2264 6566 6175 6c74  tive == "default
-00002260: 2220 656c 7365 206e 756c 6c63 6f6e 7465  " else nullconte
-00002270: 7874 2829 3a20 2023 2074 7970 653a 2069  xt():  # type: i
-00002280: 676e 6f72 655b 6174 7472 2d64 6566 696e  gnore[attr-defin
-00002290: 6564 2c75 6e75 7365 642d 6967 6e6f 7265  ed,unused-ignore
-000022a0: 5d0a 2020 2020 2020 2020 7769 7468 2061  ].        with a
-000022b0: 6c74 2e64 6174 615f 7472 616e 7366 6f72  lt.data_transfor
-000022c0: 6d65 7273 2e65 6e61 626c 6528 2269 6422  mers.enable("id"
-000022d0: 293a 2020 2320 7479 7065 3a20 6967 6e6f  ):  # type: igno
-000022e0: 7265 5b61 7474 722d 6465 6669 6e65 642c  re[attr-defined,
-000022f0: 756e 7573 6564 2d69 676e 6f72 655d 0a20  unused-ignore]. 
-00002300: 2020 2020 2020 2020 2020 2063 6861 7274             chart
-00002310: 5f64 6963 7420 3d20 616c 7461 6972 5f63  _dict = altair_c
-00002320: 6861 7274 2e74 6f5f 6469 6374 2829 0a0a  hart.to_dict()..
-00002330: 2020 2020 2320 5075 7420 6461 7461 7365      # Put datase
-00002340: 7473 2062 6163 6b20 696e 746f 2074 6865  ts back into the
-00002350: 2063 6861 7274 2064 6963 743a 0a20 2020   chart dict:.   
-00002360: 2063 6861 7274 5f64 6963 745b 2264 6174   chart_dict["dat
-00002370: 6173 6574 7322 5d20 3d20 6461 7461 7365  asets"] = datase
-00002380: 7473 0a20 2020 2072 6574 7572 6e20 6368  ts.    return ch
-00002390: 6172 745f 6469 6374 0a0a 0a64 6566 205f  art_dict...def _
-000023a0: 6469 7361 6c6c 6f77 5f6d 756c 7469 5f76  disallow_multi_v
-000023b0: 6965 775f 6368 6172 7473 2873 7065 633a  iew_charts(spec:
-000023c0: 2056 6567 614c 6974 6553 7065 6329 202d   VegaLiteSpec) -
-000023d0: 3e20 4e6f 6e65 3a0a 2020 2020 2222 2252  > None:.    """R
-000023e0: 6169 7365 2061 6e20 6578 6365 7074 696f  aise an exceptio
-000023f0: 6e20 6966 2074 6865 2073 7065 6320 636f  n if the spec co
-00002400: 6e74 6169 6e73 2061 206d 756c 7469 2d76  ntains a multi-v
-00002410: 6965 7720 6368 6172 7420 2876 6965 7720  iew chart (view 
-00002420: 636f 6d70 6f73 6974 696f 6e29 2e0a 0a20  composition)... 
-00002430: 2020 2054 6869 7320 6973 2069 6e74 656e     This is inten
-00002440: 6465 6420 746f 2062 6520 7573 6564 2061  ded to be used a
-00002450: 7320 6120 7465 6d70 6f72 6172 7920 736f  s a temporary so
-00002460: 6c75 7469 6f6e 2074 6f20 7072 6576 656e  lution to preven
-00002470: 7420 7365 6c65 6374 696f 6e73 206f 6e0a  t selections on.
-00002480: 2020 2020 6d75 6c74 692d 7669 6577 2063      multi-view c
-00002490: 6861 7274 732e 2054 6865 7265 2061 7265  harts. There are
-000024a0: 2074 6f6f 206d 616e 7920 6564 6765 2063   too many edge c
-000024b0: 6173 6573 2074 6f20 6861 6e64 6c65 2073  ases to handle s
-000024c0: 656c 6563 7469 6f6e 7320 6f6e 2074 6865  elections on the
-000024d0: 7365 0a20 2020 2063 6861 7274 7320 636f  se.    charts co
-000024e0: 7272 6563 746c 792c 2073 6f20 7765 2772  rrectly, so we'r
-000024f0: 6520 6469 7361 6c6c 6f77 696e 6720 7468  e disallowing th
-00002500: 656d 2066 6f72 206e 6f77 2e0a 0a20 2020  em for now...   
-00002510: 204d 6f72 6520 696e 666f 726d 6174 696f   More informatio
-00002520: 6e20 6162 6f75 7420 7669 6577 2063 6f6d  n about view com
-00002530: 706f 7369 7469 6f6e 733a 2068 7474 7073  positions: https
-00002540: 3a2f 2f76 6567 612e 6769 7468 7562 2e69  ://vega.github.i
-00002550: 6f2f 7665 6761 2d6c 6974 652f 646f 6373  o/vega-lite/docs
-00002560: 2f63 6f6d 706f 7369 7469 6f6e 2e68 746d  /composition.htm
-00002570: 6c0a 2020 2020 2222 220a 0a20 2020 2069  l.    """..    i
-00002580: 6620 280a 2020 2020 2020 2020 616e 7928  f (.        any(
-00002590: 6b65 7920 696e 2073 7065 6320 666f 7220  key in spec for 
-000025a0: 6b65 7920 696e 205b 226c 6179 6572 222c  key in ["layer",
-000025b0: 2022 6863 6f6e 6361 7422 2c20 2276 636f   "hconcat", "vco
-000025c0: 6e63 6174 222c 2022 636f 6e63 6174 222c  ncat", "concat",
-000025d0: 2022 7370 6563 225d 290a 2020 2020 2020   "spec"]).      
-000025e0: 2020 6f72 2022 656e 636f 6469 6e67 2220    or "encoding" 
-000025f0: 6e6f 7420 696e 2073 7065 630a 2020 2020  not in spec.    
-00002600: 293a 0a20 2020 2020 2020 2072 6169 7365  ):.        raise
-00002610: 2053 7472 6561 6d6c 6974 4150 4945 7863   StreamlitAPIExc
-00002620: 6570 7469 6f6e 280a 2020 2020 2020 2020  eption(.        
-00002630: 2020 2020 2253 656c 6563 7469 6f6e 7320      "Selections 
-00002640: 6172 6520 6e6f 7420 7965 7420 7375 7070  are not yet supp
-00002650: 6f72 7465 6420 666f 7220 6d75 6c74 692d  orted for multi-
-00002660: 7669 6577 2063 6861 7274 7320 2863 6861  view charts (cha
-00002670: 7274 2063 6f6d 706f 7369 7469 6f6e 7329  rt compositions)
-00002680: 2e20 220a 2020 2020 2020 2020 2020 2020  . ".            
-00002690: 2249 6620 796f 7520 776f 756c 6420 6c69  "If you would li
-000026a0: 6b65 2074 6f20 7573 6520 7365 6c65 6374  ke to use select
-000026b0: 696f 6e73 206f 6e20 6d75 6c74 692d 7669  ions on multi-vi
-000026c0: 6577 2063 6861 7274 732c 2070 6c65 6173  ew charts, pleas
-000026d0: 6520 7570 766f 7465 2022 0a20 2020 2020  e upvote ".     
-000026e0: 2020 2020 2020 2022 7468 6973 205b 4769         "this [Gi
-000026f0: 7468 7562 2069 7373 7565 5d28 6874 7470  thub issue](http
-00002700: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f73  s://github.com/s
-00002710: 7472 6561 6d6c 6974 2f73 7472 6561 6d6c  treamlit/streaml
-00002720: 6974 2f69 7373 7565 732f 3836 3433 292e  it/issues/8643).
-00002730: 220a 2020 2020 2020 2020 290a 0a0a 6465  ".        )...de
-00002740: 6620 5f65 7874 7261 6374 5f73 656c 6563  f _extract_selec
-00002750: 7469 6f6e 5f70 6172 616d 6574 6572 7328  tion_parameters(
-00002760: 7370 6563 3a20 5665 6761 4c69 7465 5370  spec: VegaLiteSp
-00002770: 6563 2920 2d3e 2073 6574 5b73 7472 5d3a  ec) -> set[str]:
-00002780: 0a20 2020 2022 2222 4578 7472 6163 7420  .    """Extract 
-00002790: 7468 6520 6e61 6d65 7320 6f66 2061 6c6c  the names of all
-000027a0: 2076 616c 6964 2073 656c 6563 7469 6f6e   valid selection
-000027b0: 2070 6172 616d 6574 6572 7320 6672 6f6d   parameters from
-000027c0: 2074 6865 2073 7065 632e 2222 220a 2020   the spec.""".  
-000027d0: 2020 6966 206e 6f74 2073 7065 6320 6f72    if not spec or
-000027e0: 2022 7061 7261 6d73 2220 6e6f 7420 696e   "params" not in
-000027f0: 2073 7065 633a 0a20 2020 2020 2020 2072   spec:.        r
-00002800: 6574 7572 6e20 7365 7428 290a 0a20 2020  eturn set()..   
-00002810: 2070 6172 616d 5f6e 616d 6573 203d 2073   param_names = s
-00002820: 6574 2829 0a0a 2020 2020 666f 7220 7061  et()..    for pa
-00002830: 7261 6d20 696e 2073 7065 635b 2270 6172  ram in spec["par
-00002840: 616d 7322 5d3a 0a20 2020 2020 2020 2023  ams"]:.        #
-00002850: 2043 6865 636b 2069 6620 6974 206c 6f6f   Check if it loo
-00002860: 6b73 206c 696b 6520 6120 7661 6c69 6420  ks like a valid 
-00002870: 7365 6c65 6374 696f 6e20 7061 7261 6d65  selection parame
-00002880: 7465 723a 0a20 2020 2020 2020 2023 2068  ter:.        # h
-00002890: 7474 7073 3a2f 2f76 6567 612e 6769 7468  ttps://vega.gith
-000028a0: 7562 2e69 6f2f 7665 6761 2d6c 6974 652f  ub.io/vega-lite/
-000028b0: 646f 6373 2f73 656c 6563 7469 6f6e 2e68  docs/selection.h
-000028c0: 746d 6c0a 2020 2020 2020 2020 6966 2070  tml.        if p
-000028d0: 6172 616d 2e67 6574 2822 6e61 6d65 2229  aram.get("name")
-000028e0: 2061 6e64 2070 6172 616d 2e67 6574 2822   and param.get("
-000028f0: 7365 6c65 6374 2229 3a0a 2020 2020 2020  select"):.      
-00002900: 2020 2020 2020 2320 5365 6c65 6374 696f        # Selectio
-00002910: 6e20 666f 756e 642c 206a 7573 7420 7265  n found, just re
-00002920: 7475 726e 2068 6572 6520 746f 206e 6f74  turn here to not
-00002930: 2073 686f 7720 7468 6520 6578 6365 7074   show the except
-00002940: 696f 6e2e 0a20 2020 2020 2020 2020 2020  ion..           
-00002950: 2070 6172 616d 5f6e 616d 6573 2e61 6464   param_names.add
-00002960: 2870 6172 616d 5b22 6e61 6d65 225d 290a  (param["name"]).
-00002970: 0a20 2020 2072 6574 7572 6e20 7061 7261  .    return para
-00002980: 6d5f 6e61 6d65 730a 0a0a 6465 6620 5f70  m_names...def _p
-00002990: 6172 7365 5f73 656c 6563 7469 6f6e 5f6d  arse_selection_m
-000029a0: 6f64 6528 0a20 2020 2073 7065 633a 2056  ode(.    spec: V
-000029b0: 6567 614c 6974 6553 7065 632c 0a20 2020  egaLiteSpec,.   
-000029c0: 2073 656c 6563 7469 6f6e 5f6d 6f64 653a   selection_mode:
-000029d0: 2073 7472 207c 2049 7465 7261 626c 655b   str | Iterable[
-000029e0: 7374 725d 207c 204e 6f6e 652c 0a29 202d  str] | None,.) -
-000029f0: 3e20 6c69 7374 5b73 7472 5d3a 0a20 2020  > list[str]:.   
-00002a00: 2022 2222 5061 7273 6520 616e 6420 6368   """Parse and ch
-00002a10: 6563 6b20 7468 6520 7573 6572 2070 726f  eck the user pro
-00002a20: 7669 6465 6420 7365 6c65 6374 696f 6e20  vided selection 
-00002a30: 6d6f 6465 732e 0a0a 2020 2020 5468 6973  modes...    This
-00002a40: 2077 696c 6c20 7261 6973 6520 616e 2065   will raise an e
-00002a50: 7863 6570 7469 6f6e 2069 6620 6e6f 2076  xception if no v
-00002a60: 616c 6964 2073 656c 6563 7469 6f6e 2070  alid selection p
-00002a70: 6172 616d 6574 6572 7320 6172 6520 666f  arameters are fo
-00002a80: 756e 6420 696e 2074 6865 2073 7065 630a  und in the spec.
-00002a90: 2020 2020 6f72 2069 6620 7468 6520 7573      or if the us
-00002aa0: 6572 2070 726f 7669 6465 6420 7365 6c65  er provided sele
-00002ab0: 6374 696f 6e20 6d6f 6465 7320 6172 6520  ction modes are 
-00002ac0: 6e6f 7420 6465 6669 6e65 6420 696e 2074  not defined in t
-00002ad0: 6865 2073 7065 632e 0a0a 2020 2020 5061  he spec...    Pa
-00002ae0: 7261 6d65 7465 7273 0a20 2020 202d 2d2d  rameters.    ---
-00002af0: 2d2d 2d2d 2d2d 2d0a 2020 2020 7370 6563  -------.    spec
-00002b00: 203a 2056 6567 614c 6974 6553 7065 630a   : VegaLiteSpec.
-00002b10: 2020 2020 2020 2020 5468 6520 5665 6761          The Vega
-00002b20: 2d4c 6974 6520 6368 6172 7420 7370 6563  -Lite chart spec
-00002b30: 6966 6963 6174 696f 6e2e 0a0a 2020 2020  ification...    
-00002b40: 7365 6c65 6374 696f 6e5f 6d6f 6465 203a  selection_mode :
-00002b50: 2073 7472 2c20 4974 6572 6162 6c65 5b73   str, Iterable[s
-00002b60: 7472 5d2c 206f 7220 4e6f 6e65 0a20 2020  tr], or None.   
-00002b70: 2020 2020 2054 6865 2075 7365 7220 7072       The user pr
-00002b80: 6f76 6964 6564 2073 656c 6563 7469 6f6e  ovided selection
-00002b90: 206d 6f64 6528 7329 2e0a 0a20 2020 2052   mode(s)...    R
-00002ba0: 6574 7572 6e73 0a20 2020 202d 2d2d 2d2d  eturns.    -----
-00002bb0: 2d2d 0a20 2020 206c 6973 745b 7374 725d  --.    list[str]
-00002bc0: 0a20 2020 2020 2020 2054 6865 2070 6172  .        The par
-00002bd0: 7365 6420 7365 6c65 6374 696f 6e20 6d6f  sed selection mo
-00002be0: 6465 2873 2920 7468 6174 2073 686f 756c  de(s) that shoul
-00002bf0: 6420 6265 2061 6374 6976 6174 6564 2e0a  d be activated..
-00002c00: 2020 2020 2222 220a 0a20 2020 2023 2045      """..    # E
-00002c10: 7874 7261 6374 2061 6c6c 2073 656c 6563  xtract all selec
-00002c20: 7469 6f6e 2070 6172 616d 6574 6572 7320  tion parameters 
-00002c30: 6672 6f6d 2074 6865 2073 7065 633a 0a20  from the spec:. 
-00002c40: 2020 2061 6c6c 5f73 656c 6563 7469 6f6e     all_selection
-00002c50: 5f70 6172 616d 7320 3d20 5f65 7874 7261  _params = _extra
-00002c60: 6374 5f73 656c 6563 7469 6f6e 5f70 6172  ct_selection_par
-00002c70: 616d 6574 6572 7328 7370 6563 290a 0a20  ameters(spec).. 
-00002c80: 2020 2069 6620 6e6f 7420 616c 6c5f 7365     if not all_se
-00002c90: 6c65 6374 696f 6e5f 7061 7261 6d73 3a0a  lection_params:.
-00002ca0: 2020 2020 2020 2020 7261 6973 6520 5374          raise St
-00002cb0: 7265 616d 6c69 7441 5049 4578 6365 7074  reamlitAPIExcept
-00002cc0: 696f 6e28 0a20 2020 2020 2020 2020 2020  ion(.           
-00002cd0: 2022 5365 6c65 6374 696f 6e73 2061 7265   "Selections are
-00002ce0: 2061 6374 6976 6174 6564 2c20 6275 7420   activated, but 
-00002cf0: 7468 6520 7072 6f76 6964 6564 2063 6861  the provided cha
-00002d00: 7274 2073 7065 6320 646f 6573 206e 6f74  rt spec does not
-00002d10: 2022 0a20 2020 2020 2020 2020 2020 2022   ".            "
-00002d20: 6861 7665 2061 6e79 2073 656c 6563 7469  have any selecti
-00002d30: 6f6e 7320 6465 6669 6e65 642e 2054 6f20  ons defined. To 
-00002d40: 6164 6420 7365 6c65 6374 696f 6e73 2074  add selections t
-00002d50: 6f20 6073 742e 616c 7461 6972 5f63 6861  o `st.altair_cha
-00002d60: 7274 602c 2063 6865 636b 206f 7574 2074  rt`, check out t
-00002d70: 6865 2064 6f63 756d 656e 7461 7469 6f6e  he documentation
-00002d80: 2022 0a20 2020 2020 2020 2020 2020 2022   ".            "
-00002d90: 5b68 6572 655d 2868 7474 7073 3a2f 2f61  [here](https://a
-00002da0: 6c74 6169 722d 7669 7a2e 6769 7468 7562  ltair-viz.github
-00002db0: 2e69 6f2f 7573 6572 5f67 7569 6465 2f69  .io/user_guide/i
-00002dc0: 6e74 6572 6163 7469 6f6e 732e 6874 6d6c  nteractions.html
-00002dd0: 2373 656c 6563 7469 6f6e 732d 6361 7074  #selections-capt
-00002de0: 7572 696e 672d 6368 6172 742d 696e 7465  uring-chart-inte
-00002df0: 7261 6374 696f 6e73 292e 2022 0a20 2020  ractions). ".   
-00002e00: 2020 2020 2020 2020 2022 466f 7220 6164           "For ad
-00002e10: 6469 6e67 2073 656c 6563 7469 6f6e 7320  ding selections 
-00002e20: 746f 2060 7374 2e76 6567 615f 6c69 7465  to `st.vega_lite
-00002e30: 5f63 6861 7274 602c 2074 616b 6520 6120  _chart`, take a 
-00002e40: 6c6f 6f6b 2022 0a20 2020 2020 2020 2020  look ".         
-00002e50: 2020 2022 6174 2074 6865 2073 7065 6369     "at the speci
-00002e60: 6669 6361 7469 6f6e 205b 6865 7265 5d28  fication [here](
-00002e70: 6874 7470 733a 2f2f 7665 6761 2e67 6974  https://vega.git
-00002e80: 6875 622e 696f 2f76 6567 612d 6c69 7465  hub.io/vega-lite
-00002e90: 2f64 6f63 732f 7365 6c65 6374 696f 6e2e  /docs/selection.
-00002ea0: 6874 6d6c 292e 220a 2020 2020 2020 2020  html).".        
-00002eb0: 290a 0a20 2020 2069 6620 7365 6c65 6374  )..    if select
-00002ec0: 696f 6e5f 6d6f 6465 2069 7320 4e6f 6e65  ion_mode is None
-00002ed0: 3a0a 2020 2020 2020 2020 2320 4163 7469  :.        # Acti
-00002ee0: 7661 7465 2061 6c6c 2073 656c 6563 7469  vate all selecti
-00002ef0: 6f6e 2070 6172 616d 6574 6572 733a 0a20  on parameters:. 
-00002f00: 2020 2020 2020 2072 6574 7572 6e20 736f         return so
-00002f10: 7274 6564 286c 6973 7428 616c 6c5f 7365  rted(list(all_se
-00002f20: 6c65 6374 696f 6e5f 7061 7261 6d73 2929  lection_params))
-00002f30: 0a0a 2020 2020 6966 2069 7369 6e73 7461  ..    if isinsta
-00002f40: 6e63 6528 7365 6c65 6374 696f 6e5f 6d6f  nce(selection_mo
-00002f50: 6465 2c20 7374 7229 3a0a 2020 2020 2020  de, str):.      
-00002f60: 2020 2320 436f 6e76 6572 7420 7369 6e67    # Convert sing
-00002f70: 6c65 2073 7472 696e 6720 746f 206c 6973  le string to lis
-00002f80: 743a 0a20 2020 2020 2020 2073 656c 6563  t:.        selec
-00002f90: 7469 6f6e 5f6d 6f64 6520 3d20 5b73 656c  tion_mode = [sel
-00002fa0: 6563 7469 6f6e 5f6d 6f64 655d 0a0a 2020  ection_mode]..  
-00002fb0: 2020 2320 4368 6563 6b20 7468 6174 2061    # Check that a
-00002fc0: 6c6c 2070 726f 7669 6465 6420 7365 6c65  ll provided sele
-00002fd0: 6374 696f 6e20 7061 7261 6d65 7465 7273  ction parameters
-00002fe0: 2061 7265 2064 6566 696e 6564 2069 6e20   are defined in 
-00002ff0: 7468 6520 7370 6563 3a0a 2020 2020 666f  the spec:.    fo
-00003000: 7220 7365 6c65 6374 696f 6e5f 6e61 6d65  r selection_name
-00003010: 2069 6e20 7365 6c65 6374 696f 6e5f 6d6f   in selection_mo
-00003020: 6465 3a0a 2020 2020 2020 2020 6966 2073  de:.        if s
-00003030: 656c 6563 7469 6f6e 5f6e 616d 6520 6e6f  election_name no
-00003040: 7420 696e 2061 6c6c 5f73 656c 6563 7469  t in all_selecti
-00003050: 6f6e 5f70 6172 616d 733a 0a20 2020 2020  on_params:.     
-00003060: 2020 2020 2020 2072 6169 7365 2053 7472         raise Str
-00003070: 6561 6d6c 6974 4150 4945 7863 6570 7469  eamlitAPIExcepti
-00003080: 6f6e 280a 2020 2020 2020 2020 2020 2020  on(.            
-00003090: 2020 2020 6622 5365 6c65 6374 696f 6e20      f"Selection 
-000030a0: 7061 7261 6d65 7465 7220 277b 7365 6c65  parameter '{sele
-000030b0: 6374 696f 6e5f 6e61 6d65 7d27 2069 7320  ction_name}' is 
-000030c0: 6e6f 7420 6465 6669 6e65 6420 696e 2074  not defined in t
-000030d0: 6865 2063 6861 7274 2073 7065 632e 2022  he chart spec. "
-000030e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000030f0: 2066 2241 7661 696c 6162 6c65 2073 656c   f"Available sel
-00003100: 6563 7469 6f6e 2070 6172 616d 6574 6572  ection parameter
-00003110: 7320 6172 653a 207b 616c 6c5f 7365 6c65  s are: {all_sele
-00003120: 6374 696f 6e5f 7061 7261 6d73 7d2e 220a  ction_params}.".
-00003130: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00003140: 2020 7265 7475 726e 2073 6f72 7465 6428    return sorted(
-00003150: 6c69 7374 2873 656c 6563 7469 6f6e 5f6d  list(selection_m
-00003160: 6f64 6529 290a 0a0a 6465 6620 5f72 6573  ode))...def _res
-00003170: 6574 5f63 6f75 6e74 6572 5f70 6174 7465  et_counter_patte
-00003180: 726e 2870 7265 6669 783a 2073 7472 2c20  rn(prefix: str, 
-00003190: 7665 6761 5f73 7065 633a 2073 7472 2920  vega_spec: str) 
-000031a0: 2d3e 2073 7472 3a0a 2020 2020 2222 2241  -> str:.    """A
-000031b0: 6c74 6169 7220 7573 6573 2061 2067 6c6f  ltair uses a glo
-000031c0: 6261 6c20 636f 756e 7465 7220 666f 7220  bal counter for 
-000031d0: 756e 6e61 6d65 6420 7061 7261 6d65 7465  unnamed paramete
-000031e0: 7273 2061 6e64 2076 6965 7773 2e0a 2020  rs and views..  
-000031f0: 2020 5765 206e 6565 6420 746f 2072 6573    We need to res
-00003200: 6574 2074 6865 7365 2063 6f75 6e74 6572  et these counter
-00003210: 7320 6f6e 2061 2073 7065 632d 6c65 7665  s on a spec-leve
-00003220: 6c20 746f 206d 616b 6520 7468 650a 2020  l to make the.  
-00003230: 2020 7370 6563 2073 7461 626c 6520 6163    spec stable ac
-00003240: 726f 7373 2072 6572 756e 7320 616e 6420  ross reruns and 
-00003250: 6176 6f69 6420 6368 616e 6765 7320 746f  avoid changes to
-00003260: 2074 6865 2065 6c65 6d65 6e74 2049 442e   the element ID.
-00003270: 0a20 2020 2022 2222 0a20 2020 2070 6174  .    """.    pat
-00003280: 7465 726e 203d 2072 652e 636f 6d70 696c  tern = re.compil
-00003290: 6528 7266 2722 7b70 7265 6669 787d 5c64  e(rf'"{prefix}\d
-000032a0: 2b22 2729 0a20 2020 2023 2047 6574 2061  +"').    # Get a
-000032b0: 6c6c 206d 6174 6368 6573 2077 6974 686f  ll matches witho
-000032c0: 7574 2064 7570 6c69 6361 7465 7320 696e  ut duplicates in
-000032d0: 206f 7264 6572 206f 6620 6170 7065 6172   order of appear
-000032e0: 616e 6365 2e0a 2020 2020 2320 5573 696e  ance..    # Usin
-000032f0: 6720 6120 7365 7420 6865 7265 2077 6f75  g a set here wou
-00003300: 6c64 206e 6f74 2067 7561 7261 6e74 6565  ld not guarantee
-00003310: 2074 6865 206f 7264 6572 206f 6620 6170   the order of ap
-00003320: 7065 6172 616e 6365 2c0a 2020 2020 2320  pearance,.    # 
-00003330: 7768 6963 6820 6d69 6768 7420 6c65 6164  which might lead
-00003340: 2074 6f20 6469 6666 6572 656e 7420 7265   to different re
-00003350: 706c 6163 656d 656e 7473 206f 6e20 6561  placements on ea
-00003360: 6368 2072 756e 2e0a 2020 2020 2320 5468  ch run..    # Th
-00003370: 6520 6f72 6465 7220 6f66 2074 6865 2073  e order of the s
-00003380: 7065 6320 6672 6f6d 2041 6c74 6169 7220  pec from Altair 
-00003390: 6973 2065 7870 6563 7465 6420 746f 2073  is expected to s
-000033a0: 7461 7920 7374 6162 6c65 0a20 2020 2023  tay stable.    #
-000033b0: 2077 6974 6869 6e20 7468 6520 7361 6d65   within the same
-000033c0: 2073 6573 7369 6f6e 202f 2041 6c74 6169   session / Altai
-000033d0: 7220 7665 7273 696f 6e2e 0a20 2020 2023  r version..    #
-000033e0: 2054 6865 206f 7264 6572 206d 6967 6874   The order might
-000033f0: 2063 6861 6e67 6520 7769 7468 2041 6c74   change with Alt
-00003400: 6169 7220 7570 6461 7465 732c 2062 7574  air updates, but
-00003410: 2074 6861 7427 7320 6e6f 7420 7265 616c   that's not real
-00003420: 6c79 0a20 2020 2023 2061 2063 6173 6520  ly.    # a case 
-00003430: 7468 6174 2069 7320 7265 6c65 7661 6e74  that is relevant
-00003440: 2066 6f72 2075 7320 7369 6e63 6520 7765   for us since we
-00003450: 206d 6169 6e6c 7920 6361 7265 2061 626f   mainly care abo
-00003460: 7574 2068 6176 696e 670a 2020 2020 2320  ut having.    # 
-00003470: 7468 6973 2073 7461 626c 6520 7769 7468  this stable with
-00003480: 696e 2061 2073 6573 7369 6f6e 2e0a 2020  in a session..  
-00003490: 2020 6966 206d 6174 6368 6573 203a 3d20    if matches := 
-000034a0: 6c69 7374 2864 6963 742e 6672 6f6d 6b65  list(dict.fromke
-000034b0: 7973 2870 6174 7465 726e 2e66 696e 6461  ys(pattern.finda
-000034c0: 6c6c 2876 6567 615f 7370 6563 2929 293a  ll(vega_spec))):
-000034d0: 0a20 2020 2020 2020 2023 2041 6464 2061  .        # Add a
-000034e0: 2070 7265 6669 7820 746f 2074 6865 2072   prefix to the r
-000034f0: 6570 6c61 6365 6d65 6e74 2074 6f20 6176  eplacement to av
-00003500: 6f69 640a 2020 2020 2020 2020 2320 7265  oid.        # re
-00003510: 706c 6163 696e 6720 696e 7374 616e 6365  placing instance
-00003520: 7320 7468 6174 2061 6c72 6561 6479 2068  s that already h
-00003530: 6176 6520 6265 656e 2072 6570 6c61 6365  ave been replace
-00003540: 6420 6265 666f 7265 2e0a 2020 2020 2020  d before..      
-00003550: 2020 2320 5468 6520 7072 6566 6978 2068    # The prefix h
-00003560: 6572 6520 6973 2061 7262 6974 7261 7269  ere is arbitrari
-00003570: 6c79 2063 686f 7365 6e20 7769 7468 2074  ly chosen with t
-00003580: 6865 206d 6169 6e20 676f 616c 0a20 2020  he main goal.   
-00003590: 2020 2020 2023 2074 6861 7420 6974 7320       # that its 
-000035a0: 6578 7472 656d 656c 7920 756e 6c69 6b65  extremely unlike
-000035b0: 6c79 2074 6f20 616c 7265 6164 7920 6265  ly to already be
-000035c0: 2070 6172 7420 6f66 2074 6865 2073 7065   part of the spe
-000035d0: 633a 0a20 2020 2020 2020 2072 6570 6c61  c:.        repla
-000035e0: 6365 6d65 6e74 5f70 7265 6669 7820 3d20  cement_prefix = 
-000035f0: 225f 5f72 6570 6c61 6365 5f70 7265 6669  "__replace_prefi
-00003600: 785f 6f39 6864 3130 316e 3232 6531 5f5f  x_o9hd101n22e1__
-00003610: 220a 0a20 2020 2020 2020 2023 2052 6570  "..        # Rep
-00003620: 6c61 6365 2061 6c6c 206d 6174 6368 6573  lace all matches
-00003630: 2077 6974 6820 6120 636f 756e 7465 7220   with a counter 
-00003640: 7374 6172 7469 6e67 2066 726f 6d20 310a  starting from 1.
-00003650: 2020 2020 2020 2020 2320 5765 2073 7461          # We sta
-00003660: 7274 2066 726f 6d20 3120 746f 2069 6d69  rt from 1 to imi
-00003670: 7461 7465 2074 6865 2061 6c74 6169 7220  tate the altair 
-00003680: 6265 6861 7669 6f72 2e0a 2020 2020 2020  behavior..      
-00003690: 2020 666f 7220 636f 756e 7465 722c 206d    for counter, m
-000036a0: 6174 6368 2069 6e20 656e 756d 6572 6174  atch in enumerat
-000036b0: 6528 6d61 7463 6865 732c 2073 7461 7274  e(matches, start
-000036c0: 3d31 293a 0a20 2020 2020 2020 2020 2020  =1):.           
-000036d0: 2076 6567 615f 7370 6563 203d 2076 6567   vega_spec = veg
-000036e0: 615f 7370 6563 2e72 6570 6c61 6365 280a  a_spec.replace(.
-000036f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003700: 6d61 7463 682c 2066 2722 7b72 6570 6c61  match, f'"{repla
-00003710: 6365 6d65 6e74 5f70 7265 6669 787d 7b70  cement_prefix}{p
-00003720: 7265 6669 787d 7b63 6f75 6e74 6572 7d22  refix}{counter}"
-00003730: 270a 2020 2020 2020 2020 2020 2020 290a  '.            ).
-00003740: 0a20 2020 2020 2020 2023 2052 656d 6f76  .        # Remov
-00003750: 6520 7468 6520 7072 6566 6978 2061 6761  e the prefix aga
-00003760: 696e 2066 726f 6d20 616c 6c20 7265 706c  in from all repl
-00003770: 6163 656d 656e 7473 3a0a 2020 2020 2020  acements:.      
-00003780: 2020 7665 6761 5f73 7065 6320 3d20 7665    vega_spec = ve
-00003790: 6761 5f73 7065 632e 7265 706c 6163 6528  ga_spec.replace(
-000037a0: 7265 706c 6163 656d 656e 745f 7072 6566  replacement_pref
-000037b0: 6978 2c20 2222 290a 2020 2020 7265 7475  ix, "").    retu
-000037c0: 726e 2076 6567 615f 7370 6563 0a0a 0a64  rn vega_spec...d
-000037d0: 6566 205f 7374 6162 696c 697a 655f 7665  ef _stabilize_ve
-000037e0: 6761 5f6a 736f 6e5f 7370 6563 2876 6567  ga_json_spec(veg
-000037f0: 615f 7370 6563 3a20 7374 7229 202d 3e20  a_spec: str) -> 
-00003800: 7374 723a 0a20 2020 2022 2222 4d61 6b65  str:.    """Make
-00003810: 7320 7468 6520 6368 6172 7420 7370 6563  s the chart spec
-00003820: 2073 7461 7920 7374 6162 6c65 2061 6372   stay stable acr
-00003830: 6f73 7320 7265 7275 6e73 2061 6e64 2073  oss reruns and s
-00003840: 6573 7369 6f6e 732e 0a0a 2020 2020 416c  essions...    Al
-00003850: 7461 6972 2061 7574 6f20 6372 6561 7465  tair auto create
-00003860: 7320 6e61 6d65 7320 666f 7220 756e 6e61  s names for unna
-00003870: 6d65 6420 7061 7261 6d65 7465 7273 2026  med parameters &
-00003880: 2076 6965 7773 2e20 4974 2075 7365 7320   views. It uses 
-00003890: 6120 676c 6f62 616c 2063 6f75 6e74 6572  a global counter
-000038a0: 0a20 2020 2066 6f72 2074 6865 206e 616d  .    for the nam
-000038b0: 696e 6720 7768 6963 6820 7769 6c6c 2072  ing which will r
-000038c0: 6573 756c 7420 696e 2061 2064 6966 6665  esult in a diffe
-000038d0: 7265 6e74 2073 7065 6320 6f6e 2065 7665  rent spec on eve
-000038e0: 7279 2072 6572 756e 2e0a 2020 2020 496e  ry rerun..    In
-000038f0: 2053 7472 6561 6d6c 6974 2c20 7765 206e   Streamlit, we n
-00003900: 6565 6420 7468 6520 7370 6563 2074 6f20  eed the spec to 
-00003910: 6265 2073 7461 626c 6520 6163 726f 7373  be stable across
-00003920: 2072 6572 756e 7320 616e 6420 7365 7373   reruns and sess
-00003930: 696f 6e73 2074 6f20 7072 6576 656e 7420  ions to prevent 
-00003940: 7468 6520 6368 6172 740a 2020 2020 6672  the chart.    fr
-00003950: 6f6d 2067 6574 7469 6e67 2061 206e 6577  om getting a new
-00003960: 2069 6465 6e74 6974 792e 2053 6f20 7765   identity. So we
-00003970: 206e 6565 6420 746f 2072 6570 6c61 6365   need to replace
-00003980: 2074 6865 206e 616d 6573 2077 6974 6820   the names with 
-00003990: 636f 756e 7465 7220 7769 7468 2061 2073  counter with a s
-000039a0: 7461 626c 6520 6e61 6d65 2e0a 2020 2020  table name..    
-000039b0: 4861 7669 6e67 2061 2073 7461 626c 6520  Having a stable 
-000039c0: 6368 6172 7420 7370 6563 2069 7320 616c  chart spec is al
-000039d0: 736f 2069 6d70 6f72 7461 6e74 2066 6f72  so important for
-000039e0: 2066 6561 7475 7265 7320 6c69 6b65 2066   features like f
-000039f0: 6f72 7761 7264 206d 6573 7361 6765 2063  orward message c
-00003a00: 6163 6865 2c0a 2020 2020 7768 6572 6520  ache,.    where 
-00003a10: 7765 2064 6f6e 2774 2077 616e 7420 746f  we don't want to
-00003a20: 2068 6176 6520 6368 616e 6769 6e67 206d   have changing m
-00003a30: 6573 7361 6765 7320 6f6e 2065 7665 7279  essages on every
-00003a40: 2072 6572 756e 2e0a 0a20 2020 2050 6172   rerun...    Par
-00003a50: 616d 6574 6572 2063 6f75 6e74 6572 3a0a  ameter counter:.
-00003a60: 2020 2020 6874 7470 733a 2f2f 6769 7468      https://gith
-00003a70: 7562 2e63 6f6d 2f76 6567 612f 616c 7461  ub.com/vega/alta
-00003a80: 6972 2f62 6c6f 622f 6633 3435 6364 3933  ir/blob/f345cd93
-00003a90: 3638 6165 3262 6263 3938 3632 3865 3932  68ae2bbc98628e92
-00003aa0: 3435 6339 3366 6139 6662 3538 3236 3231  45c93fa9fb582621
-00003ab0: 2f61 6c74 6169 722f 7665 6761 6c69 7465  /altair/vegalite
-00003ac0: 2f76 352f 6170 692e 7079 234c 3139 360a  /v5/api.py#L196.
-00003ad0: 0a20 2020 2056 6965 7720 636f 756e 7465  .    View counte
-00003ae0: 723a 0a20 2020 2068 7474 7073 3a2f 2f67  r:.    https://g
-00003af0: 6974 6875 622e 636f 6d2f 7665 6761 2f61  ithub.com/vega/a
-00003b00: 6c74 6169 722f 626c 6f62 2f66 3334 3563  ltair/blob/f345c
-00003b10: 6439 3336 3861 6532 6262 6339 3836 3238  d9368ae2bbc98628
-00003b20: 6539 3234 3563 3933 6661 3966 6235 3832  e9245c93fa9fb582
-00003b30: 3632 312f 616c 7461 6972 2f76 6567 616c  621/altair/vegal
-00003b40: 6974 652f 7635 2f61 7069 2e70 7923 4c32  ite/v5/api.py#L2
-00003b50: 3838 350a 0a20 2020 2054 6869 7320 6973  885..    This is
-00003b60: 2074 656d 706f 7261 7279 2073 6f6c 7574   temporary solut
-00003b70: 696f 6e20 7761 6974 696e 6720 666f 7220  ion waiting for 
-00003b80: 6120 6669 7820 666f 7220 7468 6973 2069  a fix for this i
-00003b90: 7373 7565 3a0a 2020 2020 6874 7470 733a  ssue:.    https:
-00003ba0: 2f2f 6769 7468 7562 2e63 6f6d 2f76 6567  //github.com/veg
-00003bb0: 612f 616c 7461 6972 2f69 7373 7565 732f  a/altair/issues/
-00003bc0: 3334 3136 0a0a 2020 2020 4f74 6865 7220  3416..    Other 
-00003bd0: 736f 6c75 7469 6f6e 7320 7765 2063 6f6e  solutions we con
-00003be0: 7369 6465 7265 643a 0a20 2020 2020 2d20  sidered:.     - 
-00003bf0: 776f 726b 696e 6720 6f6e 2074 6865 2064  working on the d
-00003c00: 6963 7420 6f62 6a65 6374 3a20 7468 6973  ict object: this
-00003c10: 2077 6f75 6c64 2072 6571 7569 7265 2074   would require t
-00003c20: 6f20 6974 6572 6174 6520 7468 726f 7567  o iterate throug
-00003c30: 6820 7468 6520 6f62 6a65 6374 2061 6e64  h the object and
-00003c40: 2064 6f20 7468 650a 2020 2020 2020 2073   do the.       s
-00003c50: 616d 6520 6b69 6e64 206f 6620 7265 706c  ame kind of repl
-00003c60: 6163 656d 656e 743b 2074 686f 7567 6820  acement; though 
-00003c70: 7765 2077 6f75 6c64 206e 6565 6420 746f  we would need to
-00003c80: 206b 6e6f 7720 7468 6520 7374 7275 6374   know the struct
-00003c90: 7572 6520 616e 6420 7369 6e63 6520 7765  ure and since we
-00003ca0: 206e 6565 640a 2020 2020 2020 2074 6865   need.       the
-00003cb0: 2073 7065 6320 696e 2053 7472 696e 672d   spec in String-
-00003cc0: 666f 726d 6174 2061 6e79 7761 7973 2c20  format anyways, 
-00003cd0: 7765 2064 6565 6d65 6420 7468 6174 2065  we deemed that e
-00003ce0: 7865 6375 7469 6e67 2074 6865 2072 6570  xecuting the rep
-00003cf0: 6c61 6365 6d65 6e74 206f 6e20 7468 650a  lacement on the.
-00003d00: 2020 2020 2020 2053 7472 696e 6720 6973         String is
-00003d10: 2074 6865 2062 6574 7465 7220 616c 7465   the better alte
-00003d20: 726e 6174 6976 650a 2020 2020 202d 2072  rnative.     - r
-00003d30: 6573 6574 7469 6e67 2074 6865 2063 6f75  esetting the cou
-00003d40: 6e74 6572 3a20 7468 6520 636f 756e 7465  nter: the counte
-00003d50: 7220 6973 2069 6e63 7265 6d65 6e74 6564  r is incremented
-00003d60: 2061 6c72 6561 6479 2077 6865 6e20 7468   already when th
-00003d70: 6520 6368 6172 7420 6f62 6a65 6374 2069  e chart object i
-00003d80: 7320 6372 6561 7465 640a 2020 2020 2020  s created.      
-00003d90: 2028 7365 6520 7468 6973 2047 6974 4875   (see this GitHu
-00003da0: 6220 6973 7375 6520 636f 6d6d 656e 7420  b issue comment 
-00003db0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00003dc0: 6f6d 2f76 6567 612f 616c 7461 6972 2f69  om/vega/altair/i
-00003dd0: 7373 7565 732f 3334 3136 2369 7373 7565  ssues/3416#issue
-00003de0: 636f 6d6d 656e 742d 3230 3938 3533 3034  comment-20985304
-00003df0: 3634 292c 0a20 2020 2020 2020 736f 2069  64),.       so i
-00003e00: 7420 776f 756c 6420 6265 2074 6f6f 206c  t would be too l
-00003e10: 6174 6520 6865 7265 2074 6f20 7265 7365  ate here to rese
-00003e20: 7420 7468 6520 636f 756e 7465 7220 7769  t the counter wi
-00003e30: 7468 2061 2074 6872 6561 642d 6c6f 636b  th a thread-lock
-00003e40: 2074 6f20 7072 6576 656e 7420 696e 7465   to prevent inte
-00003e50: 7266 6572 656e 6365 0a20 2020 2020 2020  rference.       
-00003e60: 6265 7477 6565 6e20 7365 7373 696f 6e73  between sessions
-00003e70: 0a20 2020 2022 2222 0a0a 2020 2020 2320  .    """..    # 
-00003e80: 5765 206f 6e6c 7920 7761 6e74 2074 6f20  We only want to 
-00003e90: 6170 706c 7920 7468 6573 6520 7265 706c  apply these repl
-00003ea0: 6163 656d 656e 7473 2069 6620 6974 2069  acements if it i
-00003eb0: 7320 7265 616c 6c79 206e 6563 6573 7361  s really necessa
-00003ec0: 7279 0a20 2020 2023 2073 696e 6365 2074  ry.    # since t
-00003ed0: 6865 7265 2069 7320 6120 7269 736b 2074  here is a risk t
-00003ee0: 6861 7420 7765 2072 6570 6c61 6365 206e  hat we replace n
-00003ef0: 616d 6573 2074 6861 7420 7768 6572 6520  ames that where 
-00003f00: 6368 6f73 656e 2062 7920 7468 6520 7573  chosen by the us
-00003f10: 6572 0a20 2020 2023 2061 6e64 2074 6865  er.    # and the
-00003f20: 7265 6279 2069 6e74 726f 6475 6365 2075  reby introduce u
-00003f30: 6e77 616e 7465 6420 7369 6465 2065 6666  nwanted side eff
-00003f40: 6563 7473 2e0a 0a20 2020 2023 2057 6520  ects...    # We 
-00003f50: 6f6e 6c79 206e 6565 6420 746f 2061 7070  only need to app
-00003f60: 6c79 2074 6865 2070 6172 616d 5f20 6669  ly the param_ fi
-00003f70: 7820 6966 2074 6865 7265 2061 7265 2061  x if there are a
-00003f80: 6374 7561 6c6c 7920 7061 7261 6d65 7465  ctually paramete
-00003f90: 7273 2064 6566 696e 6564 0a20 2020 2023  rs defined.    #
-00003fa0: 2073 6f6d 6577 6865 7265 2069 6e20 7468   somewhere in th
-00003fb0: 6520 7370 6563 2e20 5765 2063 616e 2063  e spec. We can c
-00003fc0: 6865 636b 2066 6f72 2074 6869 7320 6279  heck for this by
-00003fd0: 206c 6f6f 6b69 6e67 2066 6f72 2074 6865   looking for the
-00003fe0: 2027 2270 6172 616d 7322 2720 6b65 792e   '"params"' key.
-00003ff0: 0a20 2020 2023 2054 6869 7320 6973 6e27  .    # This isn'
-00004000: 7420 6120 7065 7266 6563 7420 6368 6563  t a perfect chec
-00004010: 6b2c 2062 7574 2067 6f6f 6420 656e 6f75  k, but good enou
-00004020: 6768 2074 6f20 7072 6576 656e 7420 756e  gh to prevent un
-00004030: 6e65 6365 7373 6172 7920 6578 6563 7574  necessary execut
-00004040: 696f 6e73 0a20 2020 2023 2066 6f72 2074  ions.    # for t
-00004050: 6865 206d 616a 6f72 6974 7920 6f66 2063  he majority of c
-00004060: 6861 7274 732e 0a20 2020 2069 6620 2722  harts..    if '"
-00004070: 7061 7261 6d73 2227 2069 6e20 7665 6761  params"' in vega
-00004080: 5f73 7065 633a 0a20 2020 2020 2020 2076  _spec:.        v
-00004090: 6567 615f 7370 6563 203d 205f 7265 7365  ega_spec = _rese
-000040a0: 745f 636f 756e 7465 725f 7061 7474 6572  t_counter_patter
-000040b0: 6e28 2270 6172 616d 5f22 2c20 7665 6761  n("param_", vega
-000040c0: 5f73 7065 6329 0a0a 2020 2020 2320 5369  _spec)..    # Si
-000040d0: 6d70 6c65 2063 6865 636b 2069 6620 7468  mple check if th
-000040e0: 6520 7370 6563 2063 6f6e 7461 696e 7320  e spec contains 
-000040f0: 6120 636f 6d70 6f73 6974 6520 6368 6172  a composite char
-00004100: 743a 0a20 2020 2023 2068 7474 7073 3a2f  t:.    # https:/
-00004110: 2f76 6567 612e 6769 7468 7562 2e69 6f2f  /vega.github.io/
-00004120: 7665 6761 2d6c 6974 652f 646f 6373 2f63  vega-lite/docs/c
-00004130: 6f6d 706f 7369 7469 6f6e 2e68 746d 6c0a  omposition.html.
-00004140: 2020 2020 2320 4f74 6865 7220 6368 6172      # Other char
-00004150: 7473 2077 696c 6c20 6e6f 7420 636f 6e74  ts will not cont
-00004160: 6169 6e20 7468 6520 6076 6965 775f 6020  ain the `view_` 
-00004170: 6e61 6d65 2c0a 2020 2020 2320 736f 2069  name,.    # so i
-00004180: 7473 2062 6574 7465 7220 746f 206e 6f74  ts better to not
-00004190: 2072 6570 6c61 6365 2074 6869 7320 7061   replace this pa
-000041a0: 7474 6572 6e2e 0a20 2020 2069 6620 7265  ttern..    if re
-000041b0: 2e73 6561 7263 6828 7227 2228 7663 6f6e  .search(r'"(vcon
-000041c0: 6361 747c 6863 6f6e 6361 747c 6661 6365  cat|hconcat|face
-000041d0: 747c 6c61 7965 727c 636f 6e63 6174 7c72  t|layer|concat|r
-000041e0: 6570 6561 7429 2227 2c20 7665 6761 5f73  epeat)"', vega_s
-000041f0: 7065 6329 3a0a 2020 2020 2020 2020 7665  pec):.        ve
-00004200: 6761 5f73 7065 6320 3d20 5f72 6573 6574  ga_spec = _reset
-00004210: 5f63 6f75 6e74 6572 5f70 6174 7465 726e  _counter_pattern
-00004220: 2822 7669 6577 5f22 2c20 7665 6761 5f73  ("view_", vega_s
-00004230: 7065 6329 0a20 2020 2072 6574 7572 6e20  pec).    return 
-00004240: 7665 6761 5f73 7065 630a 0a0a 636c 6173  vega_spec...clas
-00004250: 7320 5665 6761 4368 6172 7473 4d69 7869  s VegaChartsMixi
-00004260: 6e3a 0a20 2020 2022 2222 4d69 782d 696e  n:.    """Mix-in
-00004270: 2063 6c61 7373 2066 6f72 2061 6c6c 2076   class for all v
-00004280: 6567 612d 7265 6c61 7465 6420 6368 6172  ega-related char
-00004290: 7420 636f 6d6d 616e 6473 2e0a 0a20 2020  t commands...   
-000042a0: 2041 6c74 6169 7220 6973 2061 2070 7974   Altair is a pyt
-000042b0: 686f 6e20 7772 6170 7065 7220 6f6e 2074  hon wrapper on t
-000042c0: 6f70 206f 6620 7468 6520 7665 6761 2d6c  op of the vega-l
-000042d0: 6974 6520 7370 6563 2e20 416e 6420 6f75  ite spec. And ou
-000042e0: 720a 2020 2020 6275 696c 742d 696e 2063  r.    built-in c
-000042f0: 6861 7274 2063 6f6d 6d61 6e64 7320 6172  hart commands ar
-00004300: 6520 6a75 7374 2061 6e6f 7468 6572 206c  e just another l
-00004310: 6179 6572 206f 6e2d 746f 7020 6f66 2041  ayer on-top of A
-00004320: 6c74 6169 722e 0a20 2020 2041 6c6c 206f  ltair..    All o
-00004330: 6620 7468 6573 6520 6368 6172 7420 636f  f these chart co
-00004340: 6d6d 616e 6473 2077 696c 6c20 6265 2065  mmands will be e
-00004350: 7665 6e74 7561 6c6c 7920 636f 6e76 6572  ventually conver
-00004360: 7465 6420 746f 2061 2076 6567 612d 6c69  ted to a vega-li
-00004370: 7465 0a20 2020 2073 7065 6320 616e 6420  te.    spec and 
-00004380: 7265 6e64 6572 6564 2075 7369 6e67 2074  rendered using t
-00004390: 6865 2073 616d 6520 7665 6761 2d6c 6974  he same vega-lit
-000043a0: 6520 6368 6172 7420 636f 6d70 6f6e 656e  e chart componen
-000043b0: 742e 0a20 2020 2022 2222 0a0a 2020 2020  t..    """..    
-000043c0: 4067 6174 6865 725f 6d65 7472 6963 7328  @gather_metrics(
-000043d0: 226c 696e 655f 6368 6172 7422 290a 2020  "line_chart").  
-000043e0: 2020 6465 6620 6c69 6e65 5f63 6861 7274    def line_chart
-000043f0: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
-00004400: 2020 2020 2020 2020 6461 7461 3a20 4461          data: Da
-00004410: 7461 203d 204e 6f6e 652c 0a20 2020 2020  ta = None,.     
-00004420: 2020 202a 2c0a 2020 2020 2020 2020 783a     *,.        x:
-00004430: 2073 7472 207c 204e 6f6e 6520 3d20 4e6f   str | None = No
-00004440: 6e65 2c0a 2020 2020 2020 2020 793a 2073  ne,.        y: s
-00004450: 7472 207c 2053 6571 7565 6e63 655b 7374  tr | Sequence[st
-00004460: 725d 207c 204e 6f6e 6520 3d20 4e6f 6e65  r] | None = None
-00004470: 2c0a 2020 2020 2020 2020 636f 6c6f 723a  ,.        color:
-00004480: 2073 7472 207c 2043 6f6c 6f72 207c 206c   str | Color | l
-00004490: 6973 745b 436f 6c6f 725d 207c 204e 6f6e  ist[Color] | Non
-000044a0: 6520 3d20 4e6f 6e65 2c0a 2020 2020 2020  e = None,.      
-000044b0: 2020 7769 6474 683a 2069 6e74 203d 2030    width: int = 0
-000044c0: 2c0a 2020 2020 2020 2020 6865 6967 6874  ,.        height
-000044d0: 3a20 696e 7420 3d20 302c 0a20 2020 2020  : int = 0,.     
-000044e0: 2020 2075 7365 5f63 6f6e 7461 696e 6572     use_container
-000044f0: 5f77 6964 7468 3a20 626f 6f6c 203d 2054  _width: bool = T
-00004500: 7275 652c 0a20 2020 2029 202d 3e20 4465  rue,.    ) -> De
-00004510: 6c74 6147 656e 6572 6174 6f72 3a0a 2020  ltaGenerator:.  
-00004520: 2020 2020 2020 2222 2244 6973 706c 6179        """Display
-00004530: 2061 206c 696e 6520 6368 6172 742e 0a0a   a line chart...
-00004540: 2020 2020 2020 2020 5468 6973 2069 7320          This is 
-00004550: 7379 6e74 6178 2d73 7567 6172 2061 726f  syntax-sugar aro
-00004560: 756e 6420 6060 7374 2e61 6c74 6169 725f  und ``st.altair_
-00004570: 6368 6172 7460 602e 2054 6865 206d 6169  chart``. The mai
-00004580: 6e20 6469 6666 6572 656e 6365 0a20 2020  n difference.   
-00004590: 2020 2020 2069 7320 7468 6973 2063 6f6d       is this com
-000045a0: 6d61 6e64 2075 7365 7320 7468 6520 6461  mand uses the da
-000045b0: 7461 2773 206f 776e 2063 6f6c 756d 6e20  ta's own column 
-000045c0: 616e 6420 696e 6469 6365 7320 746f 2066  and indices to f
-000045d0: 6967 7572 6520 6f75 740a 2020 2020 2020  igure out.      
-000045e0: 2020 7468 6520 6368 6172 7427 7320 7370    the chart's sp
-000045f0: 6563 2e20 4173 2061 2072 6573 756c 7420  ec. As a result 
-00004600: 7468 6973 2069 7320 6561 7369 6572 2074  this is easier t
-00004610: 6f20 7573 6520 666f 7220 6d61 6e79 2022  o use for many "
-00004620: 6a75 7374 2070 6c6f 740a 2020 2020 2020  just plot.      
-00004630: 2020 7468 6973 2220 7363 656e 6172 696f    this" scenario
-00004640: 732c 2077 6869 6c65 2062 6569 6e67 206c  s, while being l
-00004650: 6573 7320 6375 7374 6f6d 697a 6162 6c65  ess customizable
-00004660: 2e0a 0a20 2020 2020 2020 2049 6620 6060  ...        If ``
-00004670: 7374 2e6c 696e 655f 6368 6172 7460 6020  st.line_chart`` 
-00004680: 646f 6573 206e 6f74 2067 7565 7373 2074  does not guess t
-00004690: 6865 2064 6174 6120 7370 6563 6966 6963  he data specific
-000046a0: 6174 696f 6e0a 2020 2020 2020 2020 636f  ation.        co
-000046b0: 7272 6563 746c 792c 2074 7279 2073 7065  rrectly, try spe
-000046c0: 6369 6679 696e 6720 796f 7572 2064 6573  cifying your des
-000046d0: 6972 6564 2063 6861 7274 2075 7369 6e67  ired chart using
-000046e0: 2060 6073 742e 616c 7461 6972 5f63 6861   ``st.altair_cha
-000046f0: 7274 6060 2e0a 0a20 2020 2020 2020 2050  rt``...        P
-00004700: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
-00004710: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
-00004720: 2020 2020 2064 6174 6120 3a20 7061 6e64       data : pand
-00004730: 6173 2e44 6174 6146 7261 6d65 2c20 7061  as.DataFrame, pa
-00004740: 6e64 6173 2e53 7479 6c65 722c 2070 7961  ndas.Styler, pya
-00004750: 7272 6f77 2e54 6162 6c65 2c20 6e75 6d70  rrow.Table, nump
-00004760: 792e 6e64 6172 7261 792c 2070 7973 7061  y.ndarray, pyspa
-00004770: 726b 2e73 716c 2e44 6174 6146 7261 6d65  rk.sql.DataFrame
-00004780: 2c20 736e 6f77 666c 616b 652e 736e 6f77  , snowflake.snow
-00004790: 7061 726b 2e64 6174 6166 7261 6d65 2e44  park.dataframe.D
-000047a0: 6174 6146 7261 6d65 2c20 736e 6f77 666c  ataFrame, snowfl
-000047b0: 616b 652e 736e 6f77 7061 726b 2e74 6162  ake.snowpark.tab
-000047c0: 6c65 2e54 6162 6c65 2c20 4974 6572 6162  le.Table, Iterab
-000047d0: 6c65 2c20 6469 6374 206f 7220 4e6f 6e65  le, dict or None
-000047e0: 0a20 2020 2020 2020 2020 2020 2044 6174  .            Dat
-000047f0: 6120 746f 2062 6520 706c 6f74 7465 642e  a to be plotted.
-00004800: 0a0a 2020 2020 2020 2020 7820 3a20 7374  ..        x : st
-00004810: 7220 6f72 204e 6f6e 650a 2020 2020 2020  r or None.      
-00004820: 2020 2020 2020 436f 6c75 6d6e 206e 616d        Column nam
-00004830: 6520 746f 2075 7365 2066 6f72 2074 6865  e to use for the
-00004840: 2078 2d61 7869 732e 2049 6620 4e6f 6e65   x-axis. If None
-00004850: 2c20 7573 6573 2074 6865 2064 6174 6120  , uses the data 
-00004860: 696e 6465 7820 666f 7220 7468 6520 782d  index for the x-
-00004870: 6178 6973 2e0a 0a20 2020 2020 2020 2079  axis...        y
-00004880: 203a 2073 7472 2c20 5365 7175 656e 6365   : str, Sequence
-00004890: 206f 6620 7374 722c 206f 7220 4e6f 6e65   of str, or None
-000048a0: 0a20 2020 2020 2020 2020 2020 2043 6f6c  .            Col
-000048b0: 756d 6e20 6e61 6d65 2873 2920 746f 2075  umn name(s) to u
-000048c0: 7365 2066 6f72 2074 6865 2079 2d61 7869  se for the y-axi
-000048d0: 732e 2049 6620 6120 5365 7175 656e 6365  s. If a Sequence
-000048e0: 206f 6620 7374 7269 6e67 732c 0a20 2020   of strings,.   
-000048f0: 2020 2020 2020 2020 2064 7261 7773 2073           draws s
-00004900: 6576 6572 616c 2073 6572 6965 7320 6f6e  everal series on
-00004910: 2074 6865 2073 616d 6520 6368 6172 7420   the same chart 
-00004920: 6279 206d 656c 7469 6e67 2079 6f75 7220  by melting your 
-00004930: 7769 6465 2d66 6f72 6d61 740a 2020 2020  wide-format.    
-00004940: 2020 2020 2020 2020 7461 626c 6520 696e          table in
-00004950: 746f 2061 206c 6f6e 672d 666f 726d 6174  to a long-format
-00004960: 2074 6162 6c65 2062 6568 696e 6420 7468   table behind th
-00004970: 6520 7363 656e 6573 2e20 4966 204e 6f6e  e scenes. If Non
-00004980: 652c 2064 7261 7773 0a20 2020 2020 2020  e, draws.       
-00004990: 2020 2020 2074 6865 2064 6174 6120 6f66       the data of
-000049a0: 2061 6c6c 2072 656d 6169 6e69 6e67 2063   all remaining c
-000049b0: 6f6c 756d 6e73 2061 7320 6461 7461 2073  olumns as data s
-000049c0: 6572 6965 732e 0a0a 2020 2020 2020 2020  eries...        
-000049d0: 636f 6c6f 7220 3a20 7374 722c 2074 7570  color : str, tup
-000049e0: 6c65 2c20 5365 7175 656e 6365 206f 6620  le, Sequence of 
-000049f0: 7374 722c 2053 6571 7565 6e63 6520 6f66  str, Sequence of
-00004a00: 2074 7570 6c65 2c20 6f72 204e 6f6e 650a   tuple, or None.
-00004a10: 2020 2020 2020 2020 2020 2020 5468 6520              The 
-00004a20: 636f 6c6f 7220 746f 2075 7365 2066 6f72  color to use for
-00004a30: 2064 6966 6665 7265 6e74 206c 696e 6573   different lines
-00004a40: 2069 6e20 7468 6973 2063 6861 7274 2e0a   in this chart..
-00004a50: 0a20 2020 2020 2020 2020 2020 2046 6f72  .            For
-00004a60: 2061 206c 696e 6520 6368 6172 7420 7769   a line chart wi
-00004a70: 7468 206a 7573 7420 6f6e 6520 6c69 6e65  th just one line
-00004a80: 2c20 7468 6973 2063 616e 2062 653a 0a0a  , this can be:..
-00004a90: 2020 2020 2020 2020 2020 2020 2a20 4e6f              * No
-00004aa0: 6e65 2c20 746f 2075 7365 2074 6865 2064  ne, to use the d
-00004ab0: 6566 6175 6c74 2063 6f6c 6f72 2e0a 2020  efault color..  
-00004ac0: 2020 2020 2020 2020 2020 2a20 4120 6865            * A he
-00004ad0: 7820 7374 7269 6e67 206c 696b 6520 2223  x string like "#
-00004ae0: 6666 6161 3030 2220 6f72 2022 2366 6661  ffaa00" or "#ffa
-00004af0: 6130 3038 3822 2e0a 2020 2020 2020 2020  a0088"..        
-00004b00: 2020 2020 2a20 416e 2052 4742 206f 7220      * An RGB or 
-00004b10: 5247 4241 2074 7570 6c65 2077 6974 6820  RGBA tuple with 
-00004b20: 7468 6520 7265 642c 2067 7265 656e 2c20  the red, green, 
-00004b30: 626c 7565 2c20 616e 6420 616c 7068 610a  blue, and alpha.
-00004b40: 2020 2020 2020 2020 2020 2020 2020 636f                co
-00004b50: 6d70 6f6e 656e 7473 2073 7065 6369 6669  mponents specifi
-00004b60: 6564 2061 7320 696e 7473 2066 726f 6d20  ed as ints from 
-00004b70: 3020 746f 2032 3535 206f 7220 666c 6f61  0 to 255 or floa
-00004b80: 7473 2066 726f 6d20 302e 3020 746f 0a20  ts from 0.0 to. 
-00004b90: 2020 2020 2020 2020 2020 2020 2031 2e30               1.0
-00004ba0: 2e0a 0a20 2020 2020 2020 2020 2020 2046  ...            F
-00004bb0: 6f72 2061 206c 696e 6520 6368 6172 7420  or a line chart 
-00004bc0: 7769 7468 206d 756c 7469 706c 6520 6c69  with multiple li
-00004bd0: 6e65 732c 2077 6865 7265 2074 6865 2064  nes, where the d
-00004be0: 6174 6166 7261 6d65 2069 7320 696e 0a20  ataframe is in. 
-00004bf0: 2020 2020 2020 2020 2020 206c 6f6e 6720             long 
-00004c00: 666f 726d 6174 2028 7468 6174 2069 732c  format (that is,
-00004c10: 2079 2069 7320 4e6f 6e65 206f 7220 6a75   y is None or ju
-00004c20: 7374 206f 6e65 2063 6f6c 756d 6e29 2c20  st one column), 
-00004c30: 7468 6973 2063 616e 2062 653a 0a0a 2020  this can be:..  
-00004c40: 2020 2020 2020 2020 2020 2a20 4e6f 6e65            * None
-00004c50: 2c20 746f 2075 7365 2074 6865 2064 6566  , to use the def
-00004c60: 6175 6c74 2063 6f6c 6f72 732e 0a20 2020  ault colors..   
-00004c70: 2020 2020 2020 2020 202a 2054 6865 206e           * The n
-00004c80: 616d 6520 6f66 2061 2063 6f6c 756d 6e20  ame of a column 
-00004c90: 696e 2074 6865 2064 6174 6173 6574 2e20  in the dataset. 
-00004ca0: 4461 7461 2070 6f69 6e74 7320 7769 6c6c  Data points will
-00004cb0: 2062 6520 6772 6f75 7065 640a 2020 2020   be grouped.    
-00004cc0: 2020 2020 2020 2020 2020 696e 746f 206c            into l
-00004cd0: 696e 6573 206f 6620 7468 6520 7361 6d65  ines of the same
-00004ce0: 2063 6f6c 6f72 2062 6173 6564 206f 6e20   color based on 
-00004cf0: 7468 6520 7661 6c75 6520 6f66 2074 6869  the value of thi
-00004d00: 7320 636f 6c75 6d6e 2e0a 2020 2020 2020  s column..      
-00004d10: 2020 2020 2020 2020 496e 2061 6464 6974          In addit
-00004d20: 696f 6e2c 2069 6620 7468 6520 7661 6c75  ion, if the valu
-00004d30: 6573 2069 6e20 7468 6973 2063 6f6c 756d  es in this colum
-00004d40: 6e20 6d61 7463 6820 6f6e 6520 6f66 2074  n match one of t
-00004d50: 6865 2063 6f6c 6f72 0a20 2020 2020 2020  he color.       
-00004d60: 2020 2020 2020 2066 6f72 6d61 7473 2061         formats a
-00004d70: 626f 7665 2028 6865 7820 7374 7269 6e67  bove (hex string
-00004d80: 206f 7220 636f 6c6f 7220 7475 706c 6529   or color tuple)
-00004d90: 2c20 7468 656e 2074 6861 7420 636f 6c6f  , then that colo
-00004da0: 7220 7769 6c6c 0a20 2020 2020 2020 2020  r will.         
-00004db0: 2020 2020 2062 6520 7573 6564 2e0a 0a20       be used... 
-00004dc0: 2020 2020 2020 2020 2020 2020 2046 6f72               For
-00004dd0: 2065 7861 6d70 6c65 3a20 6966 2074 6865   example: if the
-00004de0: 2064 6174 6173 6574 2068 6173 2031 3030   dataset has 100
-00004df0: 3020 726f 7773 2c20 6275 7420 7468 6973  0 rows, but this
-00004e00: 2063 6f6c 756d 6e20 6f6e 6c79 0a20 2020   column only.   
-00004e10: 2020 2020 2020 2020 2020 2063 6f6e 7461             conta
-00004e20: 696e 7320 7468 6520 7661 6c75 6573 2022  ins the values "
-00004e30: 6164 756c 7422 2c20 2263 6869 6c64 222c  adult", "child",
-00004e40: 2061 6e64 2022 6261 6279 222c 2074 6865   and "baby", the
-00004e50: 6e20 7468 6f73 6520 3130 3030 0a20 2020  n those 1000.   
-00004e60: 2020 2020 2020 2020 2020 2064 6174 6170             datap
-00004e70: 6f69 6e74 7320 7769 6c6c 2062 6520 6772  oints will be gr
-00004e80: 6f75 7065 6420 696e 746f 2074 6872 6565  ouped into three
-00004e90: 206c 696e 6573 2077 686f 7365 2063 6f6c   lines whose col
-00004ea0: 6f72 7320 7769 6c6c 2062 650a 2020 2020  ors will be.    
-00004eb0: 2020 2020 2020 2020 2020 6175 746f 6d61            automa
-00004ec0: 7469 6361 6c6c 7920 7365 6c65 6374 6564  tically selected
-00004ed0: 2066 726f 6d20 7468 6520 6465 6661 756c   from the defaul
-00004ee0: 7420 7061 6c65 7474 652e 0a0a 2020 2020  t palette...    
-00004ef0: 2020 2020 2020 2020 2020 4275 742c 2069            But, i
-00004f00: 6620 666f 7220 7468 6520 7361 6d65 2031  f for the same 1
-00004f10: 3030 302d 726f 7720 6461 7461 7365 742c  000-row dataset,
-00004f20: 2074 6869 7320 636f 6c75 6d6e 2063 6f6e   this column con
-00004f30: 7461 696e 6564 0a20 2020 2020 2020 2020  tained.         
-00004f40: 2020 2020 2074 6865 2076 616c 7565 7320       the values 
-00004f50: 2223 6666 6161 3030 222c 2022 2366 3066  "#ffaa00", "#f0f
-00004f60: 222c 2022 2330 3030 3066 6622 2c20 7468  ", "#0000ff", th
-00004f70: 656e 2074 6865 6e20 7468 6f73 6520 3130  en then those 10
-00004f80: 3030 0a20 2020 2020 2020 2020 2020 2020  00.             
-00004f90: 2064 6174 6170 6f69 6e74 7320 776f 756c   datapoints woul
-00004fa0: 6420 7374 696c 6c20 6265 2067 726f 7570  d still be group
-00004fb0: 6564 2069 6e74 6f20 7468 7265 6520 6c69  ed into three li
-00004fc0: 6e65 732c 2062 7574 2074 6865 6972 0a20  nes, but their. 
-00004fd0: 2020 2020 2020 2020 2020 2020 2063 6f6c               col
-00004fe0: 6f72 7320 776f 756c 6420 6265 2022 2366  ors would be "#f
-00004ff0: 6661 6130 3022 2c20 2223 6630 6622 2c20  faa00", "#f0f", 
-00005000: 2223 3030 3030 6666 2220 7468 6973 2074  "#0000ff" this t
-00005010: 696d 6520 6172 6f75 6e64 2e0a 0a20 2020  ime around...   
-00005020: 2020 2020 2020 2020 2046 6f72 2061 206c           For a l
-00005030: 696e 6520 6368 6172 7420 7769 7468 206d  ine chart with m
-00005040: 756c 7469 706c 6520 6c69 6e65 732c 2077  ultiple lines, w
-00005050: 6865 7265 2074 6865 2064 6174 6166 7261  here the datafra
-00005060: 6d65 2069 7320 696e 0a20 2020 2020 2020  me is in.       
-00005070: 2020 2020 2077 6964 6520 666f 726d 6174       wide format
-00005080: 2028 7468 6174 2069 732c 2079 2069 7320   (that is, y is 
-00005090: 6120 5365 7175 656e 6365 206f 6620 636f  a Sequence of co
-000050a0: 6c75 6d6e 7329 2c20 7468 6973 2063 616e  lumns), this can
-000050b0: 2062 653a 0a0a 2020 2020 2020 2020 2020   be:..          
-000050c0: 2020 2a20 4e6f 6e65 2c20 746f 2075 7365    * None, to use
-000050d0: 2074 6865 2064 6566 6175 6c74 2063 6f6c   the default col
-000050e0: 6f72 732e 0a20 2020 2020 2020 2020 2020  ors..           
-000050f0: 202a 2041 206c 6973 7420 6f66 2073 7472   * A list of str
-00005100: 696e 6720 636f 6c6f 7273 206f 7220 636f  ing colors or co
-00005110: 6c6f 7220 7475 706c 6573 2074 6f20 6265  lor tuples to be
-00005120: 2075 7365 6420 666f 7220 6561 6368 206f   used for each o
-00005130: 660a 2020 2020 2020 2020 2020 2020 2020  f.              
-00005140: 7468 6520 6c69 6e65 7320 696e 2074 6865  the lines in the
-00005150: 2063 6861 7274 2e20 5468 6973 206c 6973   chart. This lis
-00005160: 7420 7368 6f75 6c64 2068 6176 6520 7468  t should have th
-00005170: 6520 7361 6d65 206c 656e 6774 680a 2020  e same length.  
-00005180: 2020 2020 2020 2020 2020 2020 6173 2074              as t
-00005190: 6865 206e 756d 6265 7220 6f66 2079 2076  he number of y v
-000051a0: 616c 7565 7320 2865 2e67 2e20 6060 636f  alues (e.g. ``co
-000051b0: 6c6f 723d 5b22 2366 6430 222c 2022 2366  lor=["#fd0", "#f
-000051c0: 3066 222c 2022 2330 3466 225d 6060 0a20  0f", "#04f"]``. 
-000051d0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-000051e0: 2074 6872 6565 206c 696e 6573 292e 0a0a   three lines)...
-000051f0: 2020 2020 2020 2020 7769 6474 6820 3a20          width : 
-00005200: 696e 740a 2020 2020 2020 2020 2020 2020  int.            
-00005210: 5468 6520 6368 6172 7420 7769 6474 6820  The chart width 
-00005220: 696e 2070 6978 656c 732e 2049 6620 302c  in pixels. If 0,
-00005230: 2073 656c 6563 7473 2074 6865 2077 6964   selects the wid
-00005240: 7468 2061 7574 6f6d 6174 6963 616c 6c79  th automatically
-00005250: 2e0a 0a20 2020 2020 2020 2068 6569 6768  ...        heigh
-00005260: 7420 3a20 696e 740a 2020 2020 2020 2020  t : int.        
-00005270: 2020 2020 5468 6520 6368 6172 7420 6865      The chart he
-00005280: 6967 6874 2069 6e20 7069 7865 6c73 2e20  ight in pixels. 
-00005290: 4966 2030 2c20 7365 6c65 6374 7320 7468  If 0, selects th
-000052a0: 6520 6865 6967 6874 2061 7574 6f6d 6174  e height automat
-000052b0: 6963 616c 6c79 2e0a 0a20 2020 2020 2020  ically...       
-000052c0: 2075 7365 5f63 6f6e 7461 696e 6572 5f77   use_container_w
-000052d0: 6964 7468 203a 2062 6f6f 6c0a 2020 2020  idth : bool.    
-000052e0: 2020 2020 2020 2020 4966 2054 7275 652c          If True,
-000052f0: 2073 6574 2074 6865 2063 6861 7274 2077   set the chart w
-00005300: 6964 7468 2074 6f20 7468 6520 636f 6c75  idth to the colu
-00005310: 6d6e 2077 6964 7468 2e20 5468 6973 2074  mn width. This t
-00005320: 616b 6573 0a20 2020 2020 2020 2020 2020  akes.           
-00005330: 2070 7265 6365 6465 6e63 6520 6f76 6572   precedence over
-00005340: 2074 6865 2077 6964 7468 2061 7267 756d   the width argum
-00005350: 656e 742e 0a0a 2020 2020 2020 2020 4578  ent...        Ex
-00005360: 616d 706c 6573 0a20 2020 2020 2020 202d  amples.        -
-00005370: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
-00005380: 3e3e 3e20 696d 706f 7274 2073 7472 6561  >>> import strea
-00005390: 6d6c 6974 2061 7320 7374 0a20 2020 2020  mlit as st.     
-000053a0: 2020 203e 3e3e 2069 6d70 6f72 7420 7061     >>> import pa
-000053b0: 6e64 6173 2061 7320 7064 0a20 2020 2020  ndas as pd.     
-000053c0: 2020 203e 3e3e 2069 6d70 6f72 7420 6e75     >>> import nu
-000053d0: 6d70 7920 6173 206e 700a 2020 2020 2020  mpy as np.      
-000053e0: 2020 3e3e 3e0a 2020 2020 2020 2020 3e3e    >>>.        >>
-000053f0: 3e20 6368 6172 745f 6461 7461 203d 2070  > chart_data = p
-00005400: 642e 4461 7461 4672 616d 6528 6e70 2e72  d.DataFrame(np.r
-00005410: 616e 646f 6d2e 7261 6e64 6e28 3230 2c20  andom.randn(20, 
-00005420: 3329 2c20 636f 6c75 6d6e 733d 5b22 6122  3), columns=["a"
-00005430: 2c20 2262 222c 2022 6322 5d29 0a20 2020  , "b", "c"]).   
-00005440: 2020 2020 203e 3e3e 0a20 2020 2020 2020       >>>.       
-00005450: 203e 3e3e 2073 742e 6c69 6e65 5f63 6861   >>> st.line_cha
-00005460: 7274 2863 6861 7274 5f64 6174 6129 0a0a  rt(chart_data)..
-00005470: 2020 2020 2020 2020 2e2e 206f 7574 7075          .. outpu
-00005480: 743a 3a0a 2020 2020 2020 2020 2020 2068  t::.           h
-00005490: 7474 7073 3a2f 2f64 6f63 2d6c 696e 652d  ttps://doc-line-
-000054a0: 6368 6172 742e 7374 7265 616d 6c69 742e  chart.streamlit.
-000054b0: 6170 702f 0a20 2020 2020 2020 2020 2020  app/.           
-000054c0: 6865 6967 6874 3a20 3434 3070 780a 0a20  height: 440px.. 
-000054d0: 2020 2020 2020 2059 6f75 2063 616e 2061         You can a
-000054e0: 6c73 6f20 6368 6f6f 7365 2064 6966 6665  lso choose diffe
-000054f0: 7265 6e74 2063 6f6c 756d 6e73 2074 6f20  rent columns to 
-00005500: 7573 6520 666f 7220 7820 616e 6420 792c  use for x and y,
-00005510: 2061 7320 7765 6c6c 2061 7320 7365 740a   as well as set.
-00005520: 2020 2020 2020 2020 7468 6520 636f 6c6f          the colo
-00005530: 7220 6479 6e61 6d69 6361 6c6c 7920 6261  r dynamically ba
-00005540: 7365 6420 6f6e 2061 2033 7264 2063 6f6c  sed on a 3rd col
-00005550: 756d 6e20 2861 7373 756d 696e 6720 796f  umn (assuming yo
-00005560: 7572 2064 6174 6166 7261 6d65 2069 7320  ur dataframe is 
-00005570: 696e 0a20 2020 2020 2020 206c 6f6e 6720  in.        long 
-00005580: 666f 726d 6174 293a 0a0a 2020 2020 2020  format):..      
-00005590: 2020 3e3e 3e20 696d 706f 7274 2073 7472    >>> import str
-000055a0: 6561 6d6c 6974 2061 7320 7374 0a20 2020  eamlit as st.   
-000055b0: 2020 2020 203e 3e3e 2069 6d70 6f72 7420       >>> import 
-000055c0: 7061 6e64 6173 2061 7320 7064 0a20 2020  pandas as pd.   
-000055d0: 2020 2020 203e 3e3e 2069 6d70 6f72 7420       >>> import 
-000055e0: 6e75 6d70 7920 6173 206e 700a 2020 2020  numpy as np.    
-000055f0: 2020 2020 3e3e 3e0a 2020 2020 2020 2020      >>>.        
-00005600: 3e3e 3e20 6368 6172 745f 6461 7461 203d  >>> chart_data =
-00005610: 2070 642e 4461 7461 4672 616d 6528 0a20   pd.DataFrame(. 
-00005620: 2020 2020 2020 202e 2e2e 2020 2020 7b0a         ...    {.
-00005630: 2020 2020 2020 2020 2e2e 2e20 2020 2020          ...     
-00005640: 2020 2022 636f 6c31 223a 206e 702e 7261     "col1": np.ra
-00005650: 6e64 6f6d 2e72 616e 646e 2832 3029 2c0a  ndom.randn(20),.
-00005660: 2020 2020 2020 2020 2e2e 2e20 2020 2020          ...     
-00005670: 2020 2022 636f 6c32 223a 206e 702e 7261     "col2": np.ra
-00005680: 6e64 6f6d 2e72 616e 646e 2832 3029 2c0a  ndom.randn(20),.
-00005690: 2020 2020 2020 2020 2e2e 2e20 2020 2020          ...     
-000056a0: 2020 2022 636f 6c33 223a 206e 702e 7261     "col3": np.ra
-000056b0: 6e64 6f6d 2e63 686f 6963 6528 5b22 4122  ndom.choice(["A"
-000056c0: 2c20 2242 222c 2022 4322 5d2c 2032 3029  , "B", "C"], 20)
-000056d0: 2c0a 2020 2020 2020 2020 2e2e 2e20 2020  ,.        ...   
-000056e0: 207d 0a20 2020 2020 2020 202e 2e2e 2029   }.        ... )
-000056f0: 0a20 2020 2020 2020 203e 3e3e 0a20 2020  .        >>>.   
-00005700: 2020 2020 203e 3e3e 2073 742e 6c69 6e65       >>> st.line
-00005710: 5f63 6861 7274 2863 6861 7274 5f64 6174  _chart(chart_dat
-00005720: 612c 2078 3d22 636f 6c31 222c 2079 3d22  a, x="col1", y="
-00005730: 636f 6c32 222c 2063 6f6c 6f72 3d22 636f  col2", color="co
-00005740: 6c33 2229 0a0a 2020 2020 2020 2020 2e2e  l3")..        ..
-00005750: 206f 7574 7075 743a 3a0a 2020 2020 2020   output::.      
-00005760: 2020 2020 2068 7474 7073 3a2f 2f64 6f63       https://doc
-00005770: 2d6c 696e 652d 6368 6172 7431 2e73 7472  -line-chart1.str
-00005780: 6561 6d6c 6974 2e61 7070 2f0a 2020 2020  eamlit.app/.    
-00005790: 2020 2020 2020 2068 6569 6768 743a 2034         height: 4
-000057a0: 3430 7078 0a0a 2020 2020 2020 2020 4669  40px..        Fi
-000057b0: 6e61 6c6c 792c 2069 6620 796f 7572 2064  nally, if your d
-000057c0: 6174 6166 7261 6d65 2069 7320 696e 2077  ataframe is in w
-000057d0: 6964 6520 666f 726d 6174 2c20 796f 7520  ide format, you 
-000057e0: 6361 6e20 6772 6f75 7020 6d75 6c74 6970  can group multip
-000057f0: 6c65 0a20 2020 2020 2020 2063 6f6c 756d  le.        colum
-00005800: 6e73 2075 6e64 6572 2074 6865 2079 2061  ns under the y a
-00005810: 7267 756d 656e 7420 746f 2073 686f 7720  rgument to show 
-00005820: 6d75 6c74 6970 6c65 206c 696e 6573 2077  multiple lines w
-00005830: 6974 6820 6469 6666 6572 656e 740a 2020  ith different.  
-00005840: 2020 2020 2020 636f 6c6f 7273 3a0a 0a20        colors:.. 
-00005850: 2020 2020 2020 203e 3e3e 2069 6d70 6f72         >>> impor
-00005860: 7420 7374 7265 616d 6c69 7420 6173 2073  t streamlit as s
-00005870: 740a 2020 2020 2020 2020 3e3e 3e20 696d  t.        >>> im
-00005880: 706f 7274 2070 616e 6461 7320 6173 2070  port pandas as p
-00005890: 640a 2020 2020 2020 2020 3e3e 3e20 696d  d.        >>> im
-000058a0: 706f 7274 206e 756d 7079 2061 7320 6e70  port numpy as np
-000058b0: 0a20 2020 2020 2020 203e 3e3e 0a20 2020  .        >>>.   
-000058c0: 2020 2020 203e 3e3e 2063 6861 7274 5f64       >>> chart_d
-000058d0: 6174 6120 3d20 7064 2e44 6174 6146 7261  ata = pd.DataFra
-000058e0: 6d65 286e 702e 7261 6e64 6f6d 2e72 616e  me(np.random.ran
-000058f0: 646e 2832 302c 2033 292c 2063 6f6c 756d  dn(20, 3), colum
-00005900: 6e73 3d5b 2263 6f6c 3122 2c20 2263 6f6c  ns=["col1", "col
-00005910: 3222 2c20 2263 6f6c 3322 5d29 0a20 2020  2", "col3"]).   
-00005920: 2020 2020 203e 3e3e 0a20 2020 2020 2020       >>>.       
-00005930: 203e 3e3e 2073 742e 6c69 6e65 5f63 6861   >>> st.line_cha
-00005940: 7274 280a 2020 2020 2020 2020 2e2e 2e20  rt(.        ... 
-00005950: 2020 2063 6861 7274 5f64 6174 612c 2078     chart_data, x
-00005960: 3d22 636f 6c31 222c 2079 3d5b 2263 6f6c  ="col1", y=["col
-00005970: 3222 2c20 2263 6f6c 3322 5d2c 2063 6f6c  2", "col3"], col
-00005980: 6f72 3d5b 2223 4646 3030 3030 222c 2022  or=["#FF0000", "
-00005990: 2330 3030 3046 4622 5d20 2023 204f 7074  #0000FF"]  # Opt
-000059a0: 696f 6e61 6c0a 2020 2020 2020 2020 2e2e  ional.        ..
-000059b0: 2e20 290a 0a20 2020 2020 2020 202e 2e20  . )..        .. 
-000059c0: 6f75 7470 7574 3a3a 0a20 2020 2020 2020  output::.       
-000059d0: 2020 2020 6874 7470 733a 2f2f 646f 632d      https://doc-
-000059e0: 6c69 6e65 2d63 6861 7274 322e 7374 7265  line-chart2.stre
-000059f0: 616d 6c69 742e 6170 702f 0a20 2020 2020  amlit.app/.     
-00005a00: 2020 2020 2020 6865 6967 6874 3a20 3434        height: 44
-00005a10: 3070 780a 0a20 2020 2020 2020 2022 2222  0px..        """
-00005a20: 0a0a 2020 2020 2020 2020 6368 6172 742c  ..        chart,
-00005a30: 2061 6464 5f72 6f77 735f 6d65 7461 6461   add_rows_metada
-00005a40: 7461 203d 2067 656e 6572 6174 655f 6368  ta = generate_ch
-00005a50: 6172 7428 0a20 2020 2020 2020 2020 2020  art(.           
-00005a60: 2063 6861 7274 5f74 7970 653d 4368 6172   chart_type=Char
-00005a70: 7454 7970 652e 4c49 4e45 2c0a 2020 2020  tType.LINE,.    
-00005a80: 2020 2020 2020 2020 6461 7461 3d64 6174          data=dat
-00005a90: 612c 0a20 2020 2020 2020 2020 2020 2078  a,.            x
-00005aa0: 5f66 726f 6d5f 7573 6572 3d78 2c0a 2020  _from_user=x,.  
-00005ab0: 2020 2020 2020 2020 2020 795f 6672 6f6d            y_from
-00005ac0: 5f75 7365 723d 792c 0a20 2020 2020 2020  _user=y,.       
-00005ad0: 2020 2020 2063 6f6c 6f72 5f66 726f 6d5f       color_from_
-00005ae0: 7573 6572 3d63 6f6c 6f72 2c0a 2020 2020  user=color,.    
-00005af0: 2020 2020 2020 2020 7369 7a65 5f66 726f          size_fro
-00005b00: 6d5f 7573 6572 3d4e 6f6e 652c 0a20 2020  m_user=None,.   
-00005b10: 2020 2020 2020 2020 2077 6964 7468 3d77           width=w
-00005b20: 6964 7468 2c0a 2020 2020 2020 2020 2020  idth,.          
-00005b30: 2020 6865 6967 6874 3d68 6569 6768 742c    height=height,
-00005b40: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
-00005b50: 2020 2072 6574 7572 6e20 6361 7374 280a     return cast(.
-00005b60: 2020 2020 2020 2020 2020 2020 2244 656c              "Del
-00005b70: 7461 4765 6e65 7261 746f 7222 2c0a 2020  taGenerator",.  
-00005b80: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-00005b90: 616c 7461 6972 5f63 6861 7274 280a 2020  altair_chart(.  
-00005ba0: 2020 2020 2020 2020 2020 2020 2020 6368                ch
-00005bb0: 6172 742c 0a20 2020 2020 2020 2020 2020  art,.           
-00005bc0: 2020 2020 2075 7365 5f63 6f6e 7461 696e       use_contain
-00005bd0: 6572 5f77 6964 7468 3d75 7365 5f63 6f6e  er_width=use_con
-00005be0: 7461 696e 6572 5f77 6964 7468 2c0a 2020  tainer_width,.  
-00005bf0: 2020 2020 2020 2020 2020 2020 2020 7468                th
-00005c00: 656d 653d 2273 7472 6561 6d6c 6974 222c  eme="streamlit",
-00005c10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005c20: 2061 6464 5f72 6f77 735f 6d65 7461 6461   add_rows_metada
-00005c30: 7461 3d61 6464 5f72 6f77 735f 6d65 7461  ta=add_rows_meta
-00005c40: 6461 7461 2c0a 2020 2020 2020 2020 2020  data,.          
-00005c50: 2020 292c 0a20 2020 2020 2020 2029 0a0a    ),.        )..
-00005c60: 2020 2020 4067 6174 6865 725f 6d65 7472      @gather_metr
-00005c70: 6963 7328 2261 7265 615f 6368 6172 7422  ics("area_chart"
-00005c80: 290a 2020 2020 6465 6620 6172 6561 5f63  ).    def area_c
-00005c90: 6861 7274 280a 2020 2020 2020 2020 7365  hart(.        se
-00005ca0: 6c66 2c0a 2020 2020 2020 2020 6461 7461  lf,.        data
-00005cb0: 3a20 4461 7461 203d 204e 6f6e 652c 0a20  : Data = None,. 
-00005cc0: 2020 2020 2020 202a 2c0a 2020 2020 2020         *,.      
-00005cd0: 2020 783a 2073 7472 207c 204e 6f6e 6520    x: str | None 
-00005ce0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-00005cf0: 793a 2073 7472 207c 2053 6571 7565 6e63  y: str | Sequenc
-00005d00: 655b 7374 725d 207c 204e 6f6e 6520 3d20  e[str] | None = 
-00005d10: 4e6f 6e65 2c0a 2020 2020 2020 2020 636f  None,.        co
-00005d20: 6c6f 723a 2073 7472 207c 2043 6f6c 6f72  lor: str | Color
-00005d30: 207c 206c 6973 745b 436f 6c6f 725d 207c   | list[Color] |
-00005d40: 204e 6f6e 6520 3d20 4e6f 6e65 2c0a 2020   None = None,.  
-00005d50: 2020 2020 2020 7769 6474 683a 2069 6e74        width: int
-00005d60: 203d 2030 2c0a 2020 2020 2020 2020 6865   = 0,.        he
-00005d70: 6967 6874 3a20 696e 7420 3d20 302c 0a20  ight: int = 0,. 
-00005d80: 2020 2020 2020 2075 7365 5f63 6f6e 7461         use_conta
-00005d90: 696e 6572 5f77 6964 7468 3a20 626f 6f6c  iner_width: bool
-00005da0: 203d 2054 7275 652c 0a20 2020 2029 202d   = True,.    ) -
-00005db0: 3e20 4465 6c74 6147 656e 6572 6174 6f72  > DeltaGenerator
-00005dc0: 3a0a 2020 2020 2020 2020 2222 2244 6973  :.        """Dis
-00005dd0: 706c 6179 2061 6e20 6172 6561 2063 6861  play an area cha
-00005de0: 7274 2e0a 0a20 2020 2020 2020 2054 6869  rt...        Thi
-00005df0: 7320 6973 2073 796e 7461 782d 7375 6761  s is syntax-suga
-00005e00: 7220 6172 6f75 6e64 2060 6073 742e 616c  r around ``st.al
-00005e10: 7461 6972 5f63 6861 7274 6060 2e20 5468  tair_chart``. Th
-00005e20: 6520 6d61 696e 2064 6966 6665 7265 6e63  e main differenc
-00005e30: 650a 2020 2020 2020 2020 6973 2074 6869  e.        is thi
-00005e40: 7320 636f 6d6d 616e 6420 7573 6573 2074  s command uses t
-00005e50: 6865 2064 6174 6127 7320 6f77 6e20 636f  he data's own co
-00005e60: 6c75 6d6e 2061 6e64 2069 6e64 6963 6573  lumn and indices
-00005e70: 2074 6f20 6669 6775 7265 206f 7574 0a20   to figure out. 
-00005e80: 2020 2020 2020 2074 6865 2063 6861 7274         the chart
-00005e90: 2773 2073 7065 632e 2041 7320 6120 7265  's spec. As a re
-00005ea0: 7375 6c74 2074 6869 7320 6973 2065 6173  sult this is eas
-00005eb0: 6965 7220 746f 2075 7365 2066 6f72 206d  ier to use for m
-00005ec0: 616e 7920 226a 7573 7420 706c 6f74 0a20  any "just plot. 
-00005ed0: 2020 2020 2020 2074 6869 7322 2073 6365         this" sce
-00005ee0: 6e61 7269 6f73 2c20 7768 696c 6520 6265  narios, while be
-00005ef0: 696e 6720 6c65 7373 2063 7573 746f 6d69  ing less customi
-00005f00: 7a61 626c 652e 0a0a 2020 2020 2020 2020  zable...        
-00005f10: 4966 2060 6073 742e 6172 6561 5f63 6861  If ``st.area_cha
-00005f20: 7274 6060 2064 6f65 7320 6e6f 7420 6775  rt`` does not gu
-00005f30: 6573 7320 7468 6520 6461 7461 2073 7065  ess the data spe
-00005f40: 6369 6669 6361 7469 6f6e 0a20 2020 2020  cification.     
-00005f50: 2020 2063 6f72 7265 6374 6c79 2c20 7472     correctly, tr
-00005f60: 7920 7370 6563 6966 7969 6e67 2079 6f75  y specifying you
-00005f70: 7220 6465 7369 7265 6420 6368 6172 7420  r desired chart 
-00005f80: 7573 696e 6720 6060 7374 2e61 6c74 6169  using ``st.altai
-00005f90: 725f 6368 6172 7460 602e 0a0a 2020 2020  r_chart``...    
-00005fa0: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
-00005fb0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
-00005fc0: 2d0a 2020 2020 2020 2020 6461 7461 203a  -.        data :
-00005fd0: 2070 616e 6461 732e 4461 7461 4672 616d   pandas.DataFram
-00005fe0: 652c 2070 616e 6461 732e 5374 796c 6572  e, pandas.Styler
-00005ff0: 2c20 7079 6172 726f 772e 5461 626c 652c  , pyarrow.Table,
-00006000: 206e 756d 7079 2e6e 6461 7272 6179 2c20   numpy.ndarray, 
-00006010: 7079 7370 6172 6b2e 7371 6c2e 4461 7461  pyspark.sql.Data
-00006020: 4672 616d 652c 2073 6e6f 7766 6c61 6b65  Frame, snowflake
-00006030: 2e73 6e6f 7770 6172 6b2e 6461 7461 6672  .snowpark.datafr
-00006040: 616d 652e 4461 7461 4672 616d 652c 2073  ame.DataFrame, s
-00006050: 6e6f 7766 6c61 6b65 2e73 6e6f 7770 6172  nowflake.snowpar
-00006060: 6b2e 7461 626c 652e 5461 626c 652c 2049  k.table.Table, I
-00006070: 7465 7261 626c 652c 206f 7220 6469 6374  terable, or dict
-00006080: 0a20 2020 2020 2020 2020 2020 2044 6174  .            Dat
-00006090: 6120 746f 2062 6520 706c 6f74 7465 642e  a to be plotted.
-000060a0: 0a0a 2020 2020 2020 2020 7820 3a20 7374  ..        x : st
-000060b0: 7220 6f72 204e 6f6e 650a 2020 2020 2020  r or None.      
-000060c0: 2020 2020 2020 436f 6c75 6d6e 206e 616d        Column nam
-000060d0: 6520 746f 2075 7365 2066 6f72 2074 6865  e to use for the
-000060e0: 2078 2d61 7869 732e 2049 6620 4e6f 6e65   x-axis. If None
-000060f0: 2c20 7573 6573 2074 6865 2064 6174 6120  , uses the data 
-00006100: 696e 6465 7820 666f 7220 7468 6520 782d  index for the x-
-00006110: 6178 6973 2e0a 0a20 2020 2020 2020 2079  axis...        y
-00006120: 203a 2073 7472 2c20 5365 7175 656e 6365   : str, Sequence
-00006130: 206f 6620 7374 722c 206f 7220 4e6f 6e65   of str, or None
-00006140: 0a20 2020 2020 2020 2020 2020 2043 6f6c  .            Col
-00006150: 756d 6e20 6e61 6d65 2873 2920 746f 2075  umn name(s) to u
-00006160: 7365 2066 6f72 2074 6865 2079 2d61 7869  se for the y-axi
-00006170: 732e 2049 6620 6120 5365 7175 656e 6365  s. If a Sequence
-00006180: 206f 6620 7374 7269 6e67 732c 0a20 2020   of strings,.   
-00006190: 2020 2020 2020 2020 2064 7261 7773 2073           draws s
-000061a0: 6576 6572 616c 2073 6572 6965 7320 6f6e  everal series on
-000061b0: 2074 6865 2073 616d 6520 6368 6172 7420   the same chart 
-000061c0: 6279 206d 656c 7469 6e67 2079 6f75 7220  by melting your 
-000061d0: 7769 6465 2d66 6f72 6d61 740a 2020 2020  wide-format.    
-000061e0: 2020 2020 2020 2020 7461 626c 6520 696e          table in
-000061f0: 746f 2061 206c 6f6e 672d 666f 726d 6174  to a long-format
-00006200: 2074 6162 6c65 2062 6568 696e 6420 7468   table behind th
-00006210: 6520 7363 656e 6573 2e20 4966 204e 6f6e  e scenes. If Non
-00006220: 652c 2064 7261 7773 0a20 2020 2020 2020  e, draws.       
-00006230: 2020 2020 2074 6865 2064 6174 6120 6f66       the data of
-00006240: 2061 6c6c 2072 656d 6169 6e69 6e67 2063   all remaining c
-00006250: 6f6c 756d 6e73 2061 7320 6461 7461 2073  olumns as data s
-00006260: 6572 6965 732e 0a0a 2020 2020 2020 2020  eries...        
-00006270: 636f 6c6f 7220 3a20 7374 722c 2074 7570  color : str, tup
-00006280: 6c65 2c20 5365 7175 656e 6365 206f 6620  le, Sequence of 
-00006290: 7374 722c 2053 6571 7565 6e63 6520 6f66  str, Sequence of
-000062a0: 2074 7570 6c65 2c20 6f72 204e 6f6e 650a   tuple, or None.
-000062b0: 2020 2020 2020 2020 2020 2020 5468 6520              The 
-000062c0: 636f 6c6f 7220 746f 2075 7365 2066 6f72  color to use for
-000062d0: 2064 6966 6665 7265 6e74 2073 6572 6965   different serie
-000062e0: 7320 696e 2074 6869 7320 6368 6172 742e  s in this chart.
-000062f0: 0a0a 2020 2020 2020 2020 2020 2020 466f  ..            Fo
-00006300: 7220 616e 2061 7265 6120 6368 6172 7420  r an area chart 
-00006310: 7769 7468 206a 7573 7420 3120 7365 7269  with just 1 seri
-00006320: 6573 2c20 7468 6973 2063 616e 2062 653a  es, this can be:
-00006330: 0a0a 2020 2020 2020 2020 2020 2020 2a20  ..            * 
-00006340: 4e6f 6e65 2c20 746f 2075 7365 2074 6865  None, to use the
-00006350: 2064 6566 6175 6c74 2063 6f6c 6f72 2e0a   default color..
-00006360: 2020 2020 2020 2020 2020 2020 2a20 4120              * A 
-00006370: 6865 7820 7374 7269 6e67 206c 696b 6520  hex string like 
-00006380: 2223 6666 6161 3030 2220 6f72 2022 2366  "#ffaa00" or "#f
-00006390: 6661 6130 3038 3822 2e0a 2020 2020 2020  faa0088"..      
-000063a0: 2020 2020 2020 2a20 416e 2052 4742 206f        * An RGB o
-000063b0: 7220 5247 4241 2074 7570 6c65 2077 6974  r RGBA tuple wit
-000063c0: 6820 7468 6520 7265 642c 2067 7265 656e  h the red, green
-000063d0: 2c20 626c 7565 2c20 616e 6420 616c 7068  , blue, and alph
-000063e0: 610a 2020 2020 2020 2020 2020 2020 2020  a.              
-000063f0: 636f 6d70 6f6e 656e 7473 2073 7065 6369  components speci
-00006400: 6669 6564 2061 7320 696e 7473 2066 726f  fied as ints fro
-00006410: 6d20 3020 746f 2032 3535 206f 7220 666c  m 0 to 255 or fl
-00006420: 6f61 7473 2066 726f 6d20 302e 3020 746f  oats from 0.0 to
-00006430: 0a20 2020 2020 2020 2020 2020 2020 2031  .              1
-00006440: 2e30 2e0a 0a20 2020 2020 2020 2020 2020  .0...           
-00006450: 2046 6f72 2061 6e20 6172 6561 2063 6861   For an area cha
-00006460: 7274 2077 6974 6820 6d75 6c74 6970 6c65  rt with multiple
-00006470: 2073 6572 6965 732c 2077 6865 7265 2074   series, where t
-00006480: 6865 2064 6174 6166 7261 6d65 2069 7320  he dataframe is 
-00006490: 696e 0a20 2020 2020 2020 2020 2020 206c  in.            l
-000064a0: 6f6e 6720 666f 726d 6174 2028 7468 6174  ong format (that
-000064b0: 2069 732c 2079 2069 7320 4e6f 6e65 206f   is, y is None o
-000064c0: 7220 6a75 7374 206f 6e65 2063 6f6c 756d  r just one colum
-000064d0: 6e29 2c20 7468 6973 2063 616e 2062 653a  n), this can be:
-000064e0: 0a0a 2020 2020 2020 2020 2020 2020 2a20  ..            * 
-000064f0: 4e6f 6e65 2c20 746f 2075 7365 2074 6865  None, to use the
-00006500: 2064 6566 6175 6c74 2063 6f6c 6f72 732e   default colors.
-00006510: 0a20 2020 2020 2020 2020 2020 202a 2054  .            * T
-00006520: 6865 206e 616d 6520 6f66 2061 2063 6f6c  he name of a col
-00006530: 756d 6e20 696e 2074 6865 2064 6174 6173  umn in the datas
-00006540: 6574 2e20 4461 7461 2070 6f69 6e74 7320  et. Data points 
-00006550: 7769 6c6c 2062 6520 6772 6f75 7065 640a  will be grouped.
-00006560: 2020 2020 2020 2020 2020 2020 2020 696e                in
-00006570: 746f 2073 6572 6965 7320 6f66 2074 6865  to series of the
-00006580: 2073 616d 6520 636f 6c6f 7220 6261 7365   same color base
-00006590: 6420 6f6e 2074 6865 2076 616c 7565 206f  d on the value o
-000065a0: 6620 7468 6973 2063 6f6c 756d 6e2e 0a20  f this column.. 
-000065b0: 2020 2020 2020 2020 2020 2020 2049 6e20               In 
-000065c0: 6164 6469 7469 6f6e 2c20 6966 2074 6865  addition, if the
-000065d0: 2076 616c 7565 7320 696e 2074 6869 7320   values in this 
-000065e0: 636f 6c75 6d6e 206d 6174 6368 206f 6e65  column match one
-000065f0: 206f 6620 7468 6520 636f 6c6f 720a 2020   of the color.  
-00006600: 2020 2020 2020 2020 2020 2020 666f 726d              form
-00006610: 6174 7320 6162 6f76 6520 2868 6578 2073  ats above (hex s
-00006620: 7472 696e 6720 6f72 2063 6f6c 6f72 2074  tring or color t
-00006630: 7570 6c65 292c 2074 6865 6e20 7468 6174  uple), then that
-00006640: 2063 6f6c 6f72 2077 696c 6c0a 2020 2020   color will.    
-00006650: 2020 2020 2020 2020 2020 6265 2075 7365            be use
-00006660: 642e 0a0a 2020 2020 2020 2020 2020 2020  d...            
-00006670: 2020 466f 7220 6578 616d 706c 653a 2069    For example: i
-00006680: 6620 7468 6520 6461 7461 7365 7420 6861  f the dataset ha
-00006690: 7320 3130 3030 2072 6f77 732c 2062 7574  s 1000 rows, but
-000066a0: 2074 6869 7320 636f 6c75 6d6e 206f 6e6c   this column onl
-000066b0: 790a 2020 2020 2020 2020 2020 2020 2020  y.              
-000066c0: 636f 6e74 6169 6e73 2074 6865 2076 616c  contains the val
-000066d0: 7565 7320 2261 6475 6c74 222c 2022 6368  ues "adult", "ch
-000066e0: 696c 6422 2c20 616e 6420 2262 6162 7922  ild", and "baby"
-000066f0: 2c20 7468 656e 2074 686f 7365 2031 3030  , then those 100
-00006700: 300a 2020 2020 2020 2020 2020 2020 2020  0.              
-00006710: 6461 7461 706f 696e 7473 2077 696c 6c20  datapoints will 
-00006720: 6265 2067 726f 7570 6564 2069 6e74 6f20  be grouped into 
-00006730: 7468 7265 6520 7365 7269 6573 2077 686f  three series who
-00006740: 7365 2063 6f6c 6f72 7320 7769 6c6c 2062  se colors will b
-00006750: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-00006760: 6175 746f 6d61 7469 6361 6c6c 7920 7365  automatically se
-00006770: 6c65 6374 6564 2066 726f 6d20 7468 6520  lected from the 
-00006780: 6465 6661 756c 7420 7061 6c65 7474 652e  default palette.
-00006790: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000067a0: 4275 742c 2069 6620 666f 7220 7468 6520  But, if for the 
-000067b0: 7361 6d65 2031 3030 302d 726f 7720 6461  same 1000-row da
-000067c0: 7461 7365 742c 2074 6869 7320 636f 6c75  taset, this colu
-000067d0: 6d6e 2063 6f6e 7461 696e 6564 0a20 2020  mn contained.   
-000067e0: 2020 2020 2020 2020 2020 2074 6865 2076             the v
-000067f0: 616c 7565 7320 2223 6666 6161 3030 222c  alues "#ffaa00",
-00006800: 2022 2366 3066 222c 2022 2330 3030 3066   "#f0f", "#0000f
-00006810: 6622 2c20 7468 656e 2074 6865 6e20 7468  f", then then th
-00006820: 6f73 6520 3130 3030 0a20 2020 2020 2020  ose 1000.       
-00006830: 2020 2020 2020 2064 6174 6170 6f69 6e74         datapoint
-00006840: 7320 776f 756c 6420 7374 696c 6c20 6265  s would still be
-00006850: 2067 726f 7570 6564 2069 6e74 6f20 3320   grouped into 3 
-00006860: 7365 7269 6573 2c20 6275 7420 7468 6569  series, but thei
-00006870: 720a 2020 2020 2020 2020 2020 2020 2020  r.              
-00006880: 636f 6c6f 7273 2077 6f75 6c64 2062 6520  colors would be 
-00006890: 2223 6666 6161 3030 222c 2022 2366 3066  "#ffaa00", "#f0f
-000068a0: 222c 2022 2330 3030 3066 6622 2074 6869  ", "#0000ff" thi
-000068b0: 7320 7469 6d65 2061 726f 756e 642e 0a0a  s time around...
-000068c0: 2020 2020 2020 2020 2020 2020 466f 7220              For 
-000068d0: 616e 2061 7265 6120 6368 6172 7420 7769  an area chart wi
-000068e0: 7468 206d 756c 7469 706c 6520 7365 7269  th multiple seri
-000068f0: 6573 2c20 7768 6572 6520 7468 6520 6461  es, where the da
-00006900: 7461 6672 616d 6520 6973 2069 6e0a 2020  taframe is in.  
-00006910: 2020 2020 2020 2020 2020 7769 6465 2066            wide f
-00006920: 6f72 6d61 7420 2874 6861 7420 6973 2c20  ormat (that is, 
-00006930: 7920 6973 2061 2053 6571 7565 6e63 6520  y is a Sequence 
-00006940: 6f66 2063 6f6c 756d 6e73 292c 2074 6869  of columns), thi
-00006950: 7320 6361 6e20 6265 3a0a 0a20 2020 2020  s can be:..     
-00006960: 2020 2020 2020 202a 204e 6f6e 652c 2074         * None, t
-00006970: 6f20 7573 6520 7468 6520 6465 6661 756c  o use the defaul
-00006980: 7420 636f 6c6f 7273 2e0a 2020 2020 2020  t colors..      
-00006990: 2020 2020 2020 2a20 4120 6c69 7374 206f        * A list o
-000069a0: 6620 7374 7269 6e67 2063 6f6c 6f72 7320  f string colors 
-000069b0: 6f72 2063 6f6c 6f72 2074 7570 6c65 7320  or color tuples 
-000069c0: 746f 2062 6520 7573 6564 2066 6f72 2065  to be used for e
-000069d0: 6163 6820 6f66 0a20 2020 2020 2020 2020  ach of.         
-000069e0: 2020 2020 2074 6865 2073 6572 6965 7320       the series 
-000069f0: 696e 2074 6865 2063 6861 7274 2e20 5468  in the chart. Th
-00006a00: 6973 206c 6973 7420 7368 6f75 6c64 2068  is list should h
-00006a10: 6176 6520 7468 6520 7361 6d65 206c 656e  ave the same len
-00006a20: 6774 680a 2020 2020 2020 2020 2020 2020  gth.            
-00006a30: 2020 6173 2074 6865 206e 756d 6265 7220    as the number 
-00006a40: 6f66 2079 2076 616c 7565 7320 2865 2e67  of y values (e.g
-00006a50: 2e20 6060 636f 6c6f 723d 5b22 2366 6430  . ``color=["#fd0
-00006a60: 222c 2022 2366 3066 222c 2022 2330 3466  ", "#f0f", "#04f
-00006a70: 225d 6060 0a20 2020 2020 2020 2020 2020  "]``.           
-00006a80: 2020 2066 6f72 2074 6872 6565 206c 696e     for three lin
-00006a90: 6573 292e 0a0a 2020 2020 2020 2020 7769  es)...        wi
-00006aa0: 6474 6820 3a20 696e 740a 2020 2020 2020  dth : int.      
-00006ab0: 2020 2020 2020 5468 6520 6368 6172 7420        The chart 
-00006ac0: 7769 6474 6820 696e 2070 6978 656c 732e  width in pixels.
-00006ad0: 2049 6620 302c 2073 656c 6563 7473 2074   If 0, selects t
-00006ae0: 6865 2077 6964 7468 2061 7574 6f6d 6174  he width automat
-00006af0: 6963 616c 6c79 2e0a 0a20 2020 2020 2020  ically...       
-00006b00: 2068 6569 6768 7420 3a20 696e 740a 2020   height : int.  
-00006b10: 2020 2020 2020 2020 2020 5468 6520 6368            The ch
-00006b20: 6172 7420 6865 6967 6874 2069 6e20 7069  art height in pi
-00006b30: 7865 6c73 2e20 4966 2030 2c20 7365 6c65  xels. If 0, sele
-00006b40: 6374 7320 7468 6520 6865 6967 6874 2061  cts the height a
-00006b50: 7574 6f6d 6174 6963 616c 6c79 2e0a 0a20  utomatically... 
-00006b60: 2020 2020 2020 2075 7365 5f63 6f6e 7461         use_conta
-00006b70: 696e 6572 5f77 6964 7468 203a 2062 6f6f  iner_width : boo
-00006b80: 6c0a 2020 2020 2020 2020 2020 2020 4966  l.            If
-00006b90: 2054 7275 652c 2073 6574 2074 6865 2063   True, set the c
-00006ba0: 6861 7274 2077 6964 7468 2074 6f20 7468  hart width to th
-00006bb0: 6520 636f 6c75 6d6e 2077 6964 7468 2e20  e column width. 
-00006bc0: 5468 6973 2074 616b 6573 0a20 2020 2020  This takes.     
-00006bd0: 2020 2020 2020 2070 7265 6365 6465 6e63         precedenc
-00006be0: 6520 6f76 6572 2074 6865 2077 6964 7468  e over the width
-00006bf0: 2061 7267 756d 656e 742e 0a0a 2020 2020   argument...    
-00006c00: 2020 2020 4578 616d 706c 6573 0a20 2020      Examples.   
-00006c10: 2020 2020 202d 2d2d 2d2d 2d2d 2d0a 2020       --------.  
-00006c20: 2020 2020 2020 3e3e 3e20 696d 706f 7274        >>> import
-00006c30: 2073 7472 6561 6d6c 6974 2061 7320 7374   streamlit as st
-00006c40: 0a20 2020 2020 2020 203e 3e3e 2069 6d70  .        >>> imp
-00006c50: 6f72 7420 7061 6e64 6173 2061 7320 7064  ort pandas as pd
-00006c60: 0a20 2020 2020 2020 203e 3e3e 2069 6d70  .        >>> imp
-00006c70: 6f72 7420 6e75 6d70 7920 6173 206e 700a  ort numpy as np.
-00006c80: 2020 2020 2020 2020 3e3e 3e0a 2020 2020          >>>.    
-00006c90: 2020 2020 3e3e 3e20 6368 6172 745f 6461      >>> chart_da
-00006ca0: 7461 203d 2070 642e 4461 7461 4672 616d  ta = pd.DataFram
-00006cb0: 6528 6e70 2e72 616e 646f 6d2e 7261 6e64  e(np.random.rand
-00006cc0: 6e28 3230 2c20 3329 2c20 636f 6c75 6d6e  n(20, 3), column
-00006cd0: 733d 5b22 6122 2c20 2262 222c 2022 6322  s=["a", "b", "c"
-00006ce0: 5d29 0a20 2020 2020 2020 203e 3e3e 0a20  ]).        >>>. 
-00006cf0: 2020 2020 2020 203e 3e3e 2073 742e 6172         >>> st.ar
-00006d00: 6561 5f63 6861 7274 2863 6861 7274 5f64  ea_chart(chart_d
-00006d10: 6174 6129 0a0a 2020 2020 2020 2020 2e2e  ata)..        ..
-00006d20: 206f 7574 7075 743a 3a0a 2020 2020 2020   output::.      
-00006d30: 2020 2020 2068 7474 7073 3a2f 2f64 6f63       https://doc
-00006d40: 2d61 7265 612d 6368 6172 742e 7374 7265  -area-chart.stre
-00006d50: 616d 6c69 742e 6170 702f 0a20 2020 2020  amlit.app/.     
-00006d60: 2020 2020 2020 6865 6967 6874 3a20 3434        height: 44
-00006d70: 3070 780a 0a20 2020 2020 2020 2059 6f75  0px..        You
-00006d80: 2063 616e 2061 6c73 6f20 6368 6f6f 7365   can also choose
-00006d90: 2064 6966 6665 7265 6e74 2063 6f6c 756d   different colum
-00006da0: 6e73 2074 6f20 7573 6520 666f 7220 7820  ns to use for x 
-00006db0: 616e 6420 792c 2061 7320 7765 6c6c 2061  and y, as well a
-00006dc0: 7320 7365 740a 2020 2020 2020 2020 7468  s set.        th
-00006dd0: 6520 636f 6c6f 7220 6479 6e61 6d69 6361  e color dynamica
-00006de0: 6c6c 7920 6261 7365 6420 6f6e 2061 2033  lly based on a 3
-00006df0: 7264 2063 6f6c 756d 6e20 2861 7373 756d  rd column (assum
-00006e00: 696e 6720 796f 7572 2064 6174 6166 7261  ing your datafra
-00006e10: 6d65 2069 7320 696e 0a20 2020 2020 2020  me is in.       
-00006e20: 206c 6f6e 6720 666f 726d 6174 293a 0a0a   long format):..
-00006e30: 2020 2020 2020 2020 3e3e 3e20 696d 706f          >>> impo
-00006e40: 7274 2073 7472 6561 6d6c 6974 2061 7320  rt streamlit as 
-00006e50: 7374 0a20 2020 2020 2020 203e 3e3e 2069  st.        >>> i
-00006e60: 6d70 6f72 7420 7061 6e64 6173 2061 7320  mport pandas as 
-00006e70: 7064 0a20 2020 2020 2020 203e 3e3e 2069  pd.        >>> i
-00006e80: 6d70 6f72 7420 6e75 6d70 7920 6173 206e  mport numpy as n
-00006e90: 700a 2020 2020 2020 2020 3e3e 3e0a 2020  p.        >>>.  
-00006ea0: 2020 2020 2020 3e3e 3e20 6368 6172 745f        >>> chart_
-00006eb0: 6461 7461 203d 2070 642e 4461 7461 4672  data = pd.DataFr
-00006ec0: 616d 6528 0a20 2020 2020 2020 202e 2e2e  ame(.        ...
-00006ed0: 2020 2020 7b0a 2020 2020 2020 2020 2e2e      {.        ..
-00006ee0: 2e20 2020 2020 2020 2022 636f 6c31 223a  .        "col1":
-00006ef0: 206e 702e 7261 6e64 6f6d 2e72 616e 646e   np.random.randn
-00006f00: 2832 3029 2c0a 2020 2020 2020 2020 2e2e  (20),.        ..
-00006f10: 2e20 2020 2020 2020 2022 636f 6c32 223a  .        "col2":
-00006f20: 206e 702e 7261 6e64 6f6d 2e72 616e 646e   np.random.randn
-00006f30: 2832 3029 2c0a 2020 2020 2020 2020 2e2e  (20),.        ..
-00006f40: 2e20 2020 2020 2020 2022 636f 6c33 223a  .        "col3":
-00006f50: 206e 702e 7261 6e64 6f6d 2e63 686f 6963   np.random.choic
-00006f60: 6528 5b22 4122 2c20 2242 222c 2022 4322  e(["A", "B", "C"
-00006f70: 5d2c 2032 3029 2c0a 2020 2020 2020 2020  ], 20),.        
-00006f80: 2e2e 2e20 2020 207d 0a20 2020 2020 2020  ...    }.       
-00006f90: 202e 2e2e 2029 0a20 2020 2020 2020 203e   ... ).        >
-00006fa0: 3e3e 0a20 2020 2020 2020 203e 3e3e 2073  >>.        >>> s
-00006fb0: 742e 6172 6561 5f63 6861 7274 2863 6861  t.area_chart(cha
-00006fc0: 7274 5f64 6174 612c 2078 3d22 636f 6c31  rt_data, x="col1
-00006fd0: 222c 2079 3d22 636f 6c32 222c 2063 6f6c  ", y="col2", col
-00006fe0: 6f72 3d22 636f 6c33 2229 0a0a 2020 2020  or="col3")..    
-00006ff0: 2020 2020 2e2e 206f 7574 7075 743a 3a0a      .. output::.
-00007000: 2020 2020 2020 2020 2020 2068 7474 7073             https
-00007010: 3a2f 2f64 6f63 2d61 7265 612d 6368 6172  ://doc-area-char
-00007020: 7431 2e73 7472 6561 6d6c 6974 2e61 7070  t1.streamlit.app
-00007030: 2f0a 2020 2020 2020 2020 2020 2068 6569  /.           hei
-00007040: 6768 743a 2034 3430 7078 0a0a 2020 2020  ght: 440px..    
-00007050: 2020 2020 4669 6e61 6c6c 792c 2069 6620      Finally, if 
-00007060: 796f 7572 2064 6174 6166 7261 6d65 2069  your dataframe i
-00007070: 7320 696e 2077 6964 6520 666f 726d 6174  s in wide format
-00007080: 2c20 796f 7520 6361 6e20 6772 6f75 7020  , you can group 
-00007090: 6d75 6c74 6970 6c65 0a20 2020 2020 2020  multiple.       
-000070a0: 2063 6f6c 756d 6e73 2075 6e64 6572 2074   columns under t
-000070b0: 6865 2079 2061 7267 756d 656e 7420 746f  he y argument to
-000070c0: 2073 686f 7720 6d75 6c74 6970 6c65 2073   show multiple s
-000070d0: 6572 6965 7320 7769 7468 2064 6966 6665  eries with diffe
-000070e0: 7265 6e74 0a20 2020 2020 2020 2063 6f6c  rent.        col
-000070f0: 6f72 733a 0a0a 2020 2020 2020 2020 3e3e  ors:..        >>
-00007100: 3e20 696d 706f 7274 2073 7472 6561 6d6c  > import streaml
-00007110: 6974 2061 7320 7374 0a20 2020 2020 2020  it as st.       
-00007120: 203e 3e3e 2069 6d70 6f72 7420 7061 6e64   >>> import pand
-00007130: 6173 2061 7320 7064 0a20 2020 2020 2020  as as pd.       
-00007140: 203e 3e3e 2069 6d70 6f72 7420 6e75 6d70   >>> import nump
-00007150: 7920 6173 206e 700a 2020 2020 2020 2020  y as np.        
-00007160: 3e3e 3e0a 2020 2020 2020 2020 3e3e 3e20  >>>.        >>> 
-00007170: 6368 6172 745f 6461 7461 203d 2070 642e  chart_data = pd.
-00007180: 4461 7461 4672 616d 6528 6e70 2e72 616e  DataFrame(np.ran
-00007190: 646f 6d2e 7261 6e64 6e28 3230 2c20 3329  dom.randn(20, 3)
-000071a0: 2c20 636f 6c75 6d6e 733d 5b22 636f 6c31  , columns=["col1
-000071b0: 222c 2022 636f 6c32 222c 2022 636f 6c33  ", "col2", "col3
-000071c0: 225d 290a 2020 2020 2020 2020 3e3e 3e0a  "]).        >>>.
-000071d0: 2020 2020 2020 2020 3e3e 3e20 7374 2e61          >>> st.a
-000071e0: 7265 615f 6368 6172 7428 0a20 2020 2020  rea_chart(.     
-000071f0: 2020 202e 2e2e 2020 2020 6368 6172 745f     ...    chart_
-00007200: 6461 7461 2c20 783d 2263 6f6c 3122 2c20  data, x="col1", 
-00007210: 793d 5b22 636f 6c32 222c 2022 636f 6c33  y=["col2", "col3
-00007220: 225d 2c20 636f 6c6f 723d 5b22 2346 4630  "], color=["#FF0
-00007230: 3030 3022 2c20 2223 3030 3030 4646 225d  000", "#0000FF"]
-00007240: 2020 2320 4f70 7469 6f6e 616c 0a20 2020    # Optional.   
-00007250: 2020 2020 202e 2e2e 2029 0a0a 2020 2020       ... )..    
-00007260: 2020 2020 2e2e 206f 7574 7075 743a 3a0a      .. output::.
-00007270: 2020 2020 2020 2020 2020 2068 7474 7073             https
-00007280: 3a2f 2f64 6f63 2d61 7265 612d 6368 6172  ://doc-area-char
-00007290: 7432 2e73 7472 6561 6d6c 6974 2e61 7070  t2.streamlit.app
-000072a0: 2f0a 2020 2020 2020 2020 2020 2068 6569  /.           hei
-000072b0: 6768 743a 2034 3430 7078 0a0a 2020 2020  ght: 440px..    
-000072c0: 2020 2020 2222 220a 0a20 2020 2020 2020      """..       
-000072d0: 2063 6861 7274 2c20 6164 645f 726f 7773   chart, add_rows
-000072e0: 5f6d 6574 6164 6174 6120 3d20 6765 6e65  _metadata = gene
-000072f0: 7261 7465 5f63 6861 7274 280a 2020 2020  rate_chart(.    
-00007300: 2020 2020 2020 2020 6368 6172 745f 7479          chart_ty
-00007310: 7065 3d43 6861 7274 5479 7065 2e41 5245  pe=ChartType.ARE
-00007320: 412c 0a20 2020 2020 2020 2020 2020 2064  A,.            d
-00007330: 6174 613d 6461 7461 2c0a 2020 2020 2020  ata=data,.      
-00007340: 2020 2020 2020 785f 6672 6f6d 5f75 7365        x_from_use
-00007350: 723d 782c 0a20 2020 2020 2020 2020 2020  r=x,.           
-00007360: 2079 5f66 726f 6d5f 7573 6572 3d79 2c0a   y_from_user=y,.
-00007370: 2020 2020 2020 2020 2020 2020 636f 6c6f              colo
-00007380: 725f 6672 6f6d 5f75 7365 723d 636f 6c6f  r_from_user=colo
-00007390: 722c 0a20 2020 2020 2020 2020 2020 2073  r,.            s
-000073a0: 697a 655f 6672 6f6d 5f75 7365 723d 4e6f  ize_from_user=No
-000073b0: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
-000073c0: 7769 6474 683d 7769 6474 682c 0a20 2020  width=width,.   
-000073d0: 2020 2020 2020 2020 2068 6569 6768 743d           height=
-000073e0: 6865 6967 6874 2c0a 2020 2020 2020 2020  height,.        
-000073f0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-00007400: 2063 6173 7428 0a20 2020 2020 2020 2020   cast(.         
-00007410: 2020 2022 4465 6c74 6147 656e 6572 6174     "DeltaGenerat
-00007420: 6f72 222c 0a20 2020 2020 2020 2020 2020  or",.           
-00007430: 2073 656c 662e 5f61 6c74 6169 725f 6368   self._altair_ch
-00007440: 6172 7428 0a20 2020 2020 2020 2020 2020  art(.           
-00007450: 2020 2020 2063 6861 7274 2c0a 2020 2020       chart,.    
-00007460: 2020 2020 2020 2020 2020 2020 7573 655f              use_
-00007470: 636f 6e74 6169 6e65 725f 7769 6474 683d  container_width=
-00007480: 7573 655f 636f 6e74 6169 6e65 725f 7769  use_container_wi
-00007490: 6474 682c 0a20 2020 2020 2020 2020 2020  dth,.           
-000074a0: 2020 2020 2074 6865 6d65 3d22 7374 7265       theme="stre
-000074b0: 616d 6c69 7422 2c0a 2020 2020 2020 2020  amlit",.        
-000074c0: 2020 2020 2020 2020 6164 645f 726f 7773          add_rows
-000074d0: 5f6d 6574 6164 6174 613d 6164 645f 726f  _metadata=add_ro
-000074e0: 7773 5f6d 6574 6164 6174 612c 0a20 2020  ws_metadata,.   
-000074f0: 2020 2020 2020 2020 2029 2c0a 2020 2020           ),.    
-00007500: 2020 2020 290a 0a20 2020 2040 6761 7468      )..    @gath
-00007510: 6572 5f6d 6574 7269 6373 2822 6261 725f  er_metrics("bar_
-00007520: 6368 6172 7422 290a 2020 2020 6465 6620  chart").    def 
-00007530: 6261 725f 6368 6172 7428 0a20 2020 2020  bar_chart(.     
-00007540: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-00007550: 2064 6174 613a 2044 6174 6120 3d20 4e6f   data: Data = No
-00007560: 6e65 2c0a 2020 2020 2020 2020 2a2c 0a20  ne,.        *,. 
-00007570: 2020 2020 2020 2078 3a20 7374 7220 7c20         x: str | 
-00007580: 4e6f 6e65 203d 204e 6f6e 652c 0a20 2020  None = None,.   
-00007590: 2020 2020 2079 3a20 7374 7220 7c20 5365       y: str | Se
-000075a0: 7175 656e 6365 5b73 7472 5d20 7c20 4e6f  quence[str] | No
-000075b0: 6e65 203d 204e 6f6e 652c 0a20 2020 2020  ne = None,.     
-000075c0: 2020 2063 6f6c 6f72 3a20 7374 7220 7c20     color: str | 
-000075d0: 436f 6c6f 7220 7c20 6c69 7374 5b43 6f6c  Color | list[Col
-000075e0: 6f72 5d20 7c20 4e6f 6e65 203d 204e 6f6e  or] | None = Non
-000075f0: 652c 0a20 2020 2020 2020 2077 6964 7468  e,.        width
-00007600: 3a20 696e 7420 3d20 302c 0a20 2020 2020  : int = 0,.     
-00007610: 2020 2068 6569 6768 743a 2069 6e74 203d     height: int =
-00007620: 2030 2c0a 2020 2020 2020 2020 7573 655f   0,.        use_
-00007630: 636f 6e74 6169 6e65 725f 7769 6474 683a  container_width:
-00007640: 2062 6f6f 6c20 3d20 5472 7565 2c0a 2020   bool = True,.  
-00007650: 2020 2920 2d3e 2044 656c 7461 4765 6e65    ) -> DeltaGene
-00007660: 7261 746f 723a 0a20 2020 2020 2020 2022  rator:.        "
-00007670: 2222 4469 7370 6c61 7920 6120 6261 7220  ""Display a bar 
-00007680: 6368 6172 742e 0a0a 2020 2020 2020 2020  chart...        
-00007690: 5468 6973 2069 7320 7379 6e74 6178 2d73  This is syntax-s
-000076a0: 7567 6172 2061 726f 756e 6420 6060 7374  ugar around ``st
-000076b0: 2e61 6c74 6169 725f 6368 6172 7460 602e  .altair_chart``.
-000076c0: 2054 6865 206d 6169 6e20 6469 6666 6572   The main differ
-000076d0: 656e 6365 0a20 2020 2020 2020 2069 7320  ence.        is 
-000076e0: 7468 6973 2063 6f6d 6d61 6e64 2075 7365  this command use
-000076f0: 7320 7468 6520 6461 7461 2773 206f 776e  s the data's own
-00007700: 2063 6f6c 756d 6e20 616e 6420 696e 6469   column and indi
-00007710: 6365 7320 746f 2066 6967 7572 6520 6f75  ces to figure ou
-00007720: 740a 2020 2020 2020 2020 7468 6520 6368  t.        the ch
-00007730: 6172 7427 7320 7370 6563 2e20 4173 2061  art's spec. As a
-00007740: 2072 6573 756c 7420 7468 6973 2069 7320   result this is 
-00007750: 6561 7369 6572 2074 6f20 7573 6520 666f  easier to use fo
-00007760: 7220 6d61 6e79 2022 6a75 7374 2070 6c6f  r many "just plo
-00007770: 740a 2020 2020 2020 2020 7468 6973 2220  t.        this" 
-00007780: 7363 656e 6172 696f 732c 2077 6869 6c65  scenarios, while
-00007790: 2062 6569 6e67 206c 6573 7320 6375 7374   being less cust
-000077a0: 6f6d 697a 6162 6c65 2e0a 0a20 2020 2020  omizable...     
-000077b0: 2020 2049 6620 6060 7374 2e62 6172 5f63     If ``st.bar_c
-000077c0: 6861 7274 6060 2064 6f65 7320 6e6f 7420  hart`` does not 
-000077d0: 6775 6573 7320 7468 6520 6461 7461 2073  guess the data s
-000077e0: 7065 6369 6669 6361 7469 6f6e 0a20 2020  pecification.   
-000077f0: 2020 2020 2063 6f72 7265 6374 6c79 2c20       correctly, 
-00007800: 7472 7920 7370 6563 6966 7969 6e67 2079  try specifying y
-00007810: 6f75 7220 6465 7369 7265 6420 6368 6172  our desired char
-00007820: 7420 7573 696e 6720 6060 7374 2e61 6c74  t using ``st.alt
-00007830: 6169 725f 6368 6172 7460 602e 0a0a 2020  air_chart``...  
-00007840: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
-00007850: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-00007860: 2d2d 2d0a 2020 2020 2020 2020 6461 7461  ---.        data
-00007870: 203a 2070 616e 6461 732e 4461 7461 4672   : pandas.DataFr
-00007880: 616d 652c 2070 616e 6461 732e 5374 796c  ame, pandas.Styl
-00007890: 6572 2c20 7079 6172 726f 772e 5461 626c  er, pyarrow.Tabl
-000078a0: 652c 206e 756d 7079 2e6e 6461 7272 6179  e, numpy.ndarray
-000078b0: 2c20 7079 7370 6172 6b2e 7371 6c2e 4461  , pyspark.sql.Da
-000078c0: 7461 4672 616d 652c 2073 6e6f 7766 6c61  taFrame, snowfla
-000078d0: 6b65 2e73 6e6f 7770 6172 6b2e 6461 7461  ke.snowpark.data
-000078e0: 6672 616d 652e 4461 7461 4672 616d 652c  frame.DataFrame,
-000078f0: 2073 6e6f 7766 6c61 6b65 2e73 6e6f 7770   snowflake.snowp
-00007900: 6172 6b2e 7461 626c 652e 5461 626c 652c  ark.table.Table,
-00007910: 2049 7465 7261 626c 652c 206f 7220 6469   Iterable, or di
-00007920: 6374 0a20 2020 2020 2020 2020 2020 2044  ct.            D
-00007930: 6174 6120 746f 2062 6520 706c 6f74 7465  ata to be plotte
-00007940: 642e 0a0a 2020 2020 2020 2020 7820 3a20  d...        x : 
-00007950: 7374 7220 6f72 204e 6f6e 650a 2020 2020  str or None.    
-00007960: 2020 2020 2020 2020 436f 6c75 6d6e 206e          Column n
-00007970: 616d 6520 746f 2075 7365 2066 6f72 2074  ame to use for t
-00007980: 6865 2078 2d61 7869 732e 2049 6620 4e6f  he x-axis. If No
-00007990: 6e65 2c20 7573 6573 2074 6865 2064 6174  ne, uses the dat
-000079a0: 6120 696e 6465 7820 666f 7220 7468 6520  a index for the 
-000079b0: 782d 6178 6973 2e0a 0a20 2020 2020 2020  x-axis...       
-000079c0: 2079 203a 2073 7472 2c20 5365 7175 656e   y : str, Sequen
-000079d0: 6365 206f 6620 7374 722c 206f 7220 4e6f  ce of str, or No
-000079e0: 6e65 0a20 2020 2020 2020 2020 2020 2043  ne.            C
-000079f0: 6f6c 756d 6e20 6e61 6d65 2873 2920 746f  olumn name(s) to
-00007a00: 2075 7365 2066 6f72 2074 6865 2079 2d61   use for the y-a
-00007a10: 7869 732e 2049 6620 6120 5365 7175 656e  xis. If a Sequen
-00007a20: 6365 206f 6620 7374 7269 6e67 732c 0a20  ce of strings,. 
-00007a30: 2020 2020 2020 2020 2020 2064 7261 7773             draws
-00007a40: 2073 6576 6572 616c 2073 6572 6965 7320   several series 
-00007a50: 6f6e 2074 6865 2073 616d 6520 6368 6172  on the same char
-00007a60: 7420 6279 206d 656c 7469 6e67 2079 6f75  t by melting you
-00007a70: 7220 7769 6465 2d66 6f72 6d61 740a 2020  r wide-format.  
-00007a80: 2020 2020 2020 2020 2020 7461 626c 6520            table 
-00007a90: 696e 746f 2061 206c 6f6e 672d 666f 726d  into a long-form
-00007aa0: 6174 2074 6162 6c65 2062 6568 696e 6420  at table behind 
-00007ab0: 7468 6520 7363 656e 6573 2e20 4966 204e  the scenes. If N
-00007ac0: 6f6e 652c 2064 7261 7773 0a20 2020 2020  one, draws.     
-00007ad0: 2020 2020 2020 2074 6865 2064 6174 6120         the data 
-00007ae0: 6f66 2061 6c6c 2072 656d 6169 6e69 6e67  of all remaining
-00007af0: 2063 6f6c 756d 6e73 2061 7320 6461 7461   columns as data
-00007b00: 2073 6572 6965 732e 0a0a 2020 2020 2020   series...      
-00007b10: 2020 636f 6c6f 7220 3a20 7374 722c 2074    color : str, t
-00007b20: 7570 6c65 2c20 5365 7175 656e 6365 206f  uple, Sequence o
-00007b30: 6620 7374 722c 2053 6571 7565 6e63 6520  f str, Sequence 
-00007b40: 6f66 2074 7570 6c65 2c20 6f72 204e 6f6e  of tuple, or Non
-00007b50: 650a 2020 2020 2020 2020 2020 2020 5468  e.            Th
-00007b60: 6520 636f 6c6f 7220 746f 2075 7365 2066  e color to use f
-00007b70: 6f72 2064 6966 6665 7265 6e74 2073 6572  or different ser
-00007b80: 6965 7320 696e 2074 6869 7320 6368 6172  ies in this char
-00007b90: 742e 0a0a 2020 2020 2020 2020 2020 2020  t...            
-00007ba0: 466f 7220 6120 6261 7220 6368 6172 7420  For a bar chart 
-00007bb0: 7769 7468 206a 7573 7420 6f6e 6520 7365  with just one se
-00007bc0: 7269 6573 2c20 7468 6973 2063 616e 2062  ries, this can b
-00007bd0: 653a 0a0a 2020 2020 2020 2020 2020 2020  e:..            
-00007be0: 2a20 4e6f 6e65 2c20 746f 2075 7365 2074  * None, to use t
-00007bf0: 6865 2064 6566 6175 6c74 2063 6f6c 6f72  he default color
-00007c00: 2e0a 2020 2020 2020 2020 2020 2020 2a20  ..            * 
-00007c10: 4120 6865 7820 7374 7269 6e67 206c 696b  A hex string lik
-00007c20: 6520 2223 6666 6161 3030 2220 6f72 2022  e "#ffaa00" or "
-00007c30: 2366 6661 6130 3038 3822 2e0a 2020 2020  #ffaa0088"..    
-00007c40: 2020 2020 2020 2020 2a20 416e 2052 4742          * An RGB
-00007c50: 206f 7220 5247 4241 2074 7570 6c65 2077   or RGBA tuple w
-00007c60: 6974 6820 7468 6520 7265 642c 2067 7265  ith the red, gre
-00007c70: 656e 2c20 626c 7565 2c20 616e 6420 616c  en, blue, and al
-00007c80: 7068 610a 2020 2020 2020 2020 2020 2020  pha.            
-00007c90: 2020 636f 6d70 6f6e 656e 7473 2073 7065    components spe
-00007ca0: 6369 6669 6564 2061 7320 696e 7473 2066  cified as ints f
-00007cb0: 726f 6d20 3020 746f 2032 3535 206f 7220  rom 0 to 255 or 
-00007cc0: 666c 6f61 7473 2066 726f 6d20 302e 3020  floats from 0.0 
-00007cd0: 746f 0a20 2020 2020 2020 2020 2020 2020  to.             
-00007ce0: 2031 2e30 2e0a 0a20 2020 2020 2020 2020   1.0...         
-00007cf0: 2020 2046 6f72 2061 2062 6172 2063 6861     For a bar cha
-00007d00: 7274 2077 6974 6820 6d75 6c74 6970 6c65  rt with multiple
-00007d10: 2073 6572 6965 732c 2077 6865 7265 2074   series, where t
-00007d20: 6865 2064 6174 6166 7261 6d65 2069 7320  he dataframe is 
-00007d30: 696e 0a20 2020 2020 2020 2020 2020 206c  in.            l
-00007d40: 6f6e 6720 666f 726d 6174 2028 7468 6174  ong format (that
-00007d50: 2069 732c 2079 2069 7320 4e6f 6e65 206f   is, y is None o
-00007d60: 7220 6a75 7374 206f 6e65 2063 6f6c 756d  r just one colum
-00007d70: 6e29 2c20 7468 6973 2063 616e 2062 653a  n), this can be:
-00007d80: 0a0a 2020 2020 2020 2020 2020 2020 2a20  ..            * 
-00007d90: 4e6f 6e65 2c20 746f 2075 7365 2074 6865  None, to use the
-00007da0: 2064 6566 6175 6c74 2063 6f6c 6f72 732e   default colors.
-00007db0: 0a20 2020 2020 2020 2020 2020 202a 2054  .            * T
-00007dc0: 6865 206e 616d 6520 6f66 2061 2063 6f6c  he name of a col
-00007dd0: 756d 6e20 696e 2074 6865 2064 6174 6173  umn in the datas
-00007de0: 6574 2e20 4461 7461 2070 6f69 6e74 7320  et. Data points 
-00007df0: 7769 6c6c 2062 6520 6772 6f75 7065 640a  will be grouped.
-00007e00: 2020 2020 2020 2020 2020 2020 2020 696e                in
-00007e10: 746f 2073 6572 6965 7320 6f66 2074 6865  to series of the
-00007e20: 2073 616d 6520 636f 6c6f 7220 6261 7365   same color base
-00007e30: 6420 6f6e 2074 6865 2076 616c 7565 206f  d on the value o
-00007e40: 6620 7468 6973 2063 6f6c 756d 6e2e 0a20  f this column.. 
-00007e50: 2020 2020 2020 2020 2020 2020 2049 6e20               In 
-00007e60: 6164 6469 7469 6f6e 2c20 6966 2074 6865  addition, if the
-00007e70: 2076 616c 7565 7320 696e 2074 6869 7320   values in this 
-00007e80: 636f 6c75 6d6e 206d 6174 6368 206f 6e65  column match one
-00007e90: 206f 6620 7468 6520 636f 6c6f 720a 2020   of the color.  
-00007ea0: 2020 2020 2020 2020 2020 2020 666f 726d              form
-00007eb0: 6174 7320 6162 6f76 6520 2868 6578 2073  ats above (hex s
-00007ec0: 7472 696e 6720 6f72 2063 6f6c 6f72 2074  tring or color t
-00007ed0: 7570 6c65 292c 2074 6865 6e20 7468 6174  uple), then that
-00007ee0: 2063 6f6c 6f72 2077 696c 6c0a 2020 2020   color will.    
-00007ef0: 2020 2020 2020 2020 2020 6265 2075 7365            be use
-00007f00: 642e 0a0a 2020 2020 2020 2020 2020 2020  d...            
-00007f10: 2020 466f 7220 6578 616d 706c 653a 2069    For example: i
-00007f20: 6620 7468 6520 6461 7461 7365 7420 6861  f the dataset ha
-00007f30: 7320 3130 3030 2072 6f77 732c 2062 7574  s 1000 rows, but
-00007f40: 2074 6869 7320 636f 6c75 6d6e 206f 6e6c   this column onl
-00007f50: 790a 2020 2020 2020 2020 2020 2020 2020  y.              
-00007f60: 636f 6e74 6169 6e73 2074 6865 2076 616c  contains the val
-00007f70: 7565 7320 2261 6475 6c74 222c 2022 6368  ues "adult", "ch
-00007f80: 696c 6422 2c20 616e 6420 2262 6162 7922  ild", and "baby"
-00007f90: 2c20 7468 656e 2074 686f 7365 2031 3030  , then those 100
-00007fa0: 300a 2020 2020 2020 2020 2020 2020 2020  0.              
-00007fb0: 6461 7461 706f 696e 7473 2077 696c 6c20  datapoints will 
-00007fc0: 6265 2067 726f 7570 6564 2069 6e74 6f20  be grouped into 
-00007fd0: 7468 7265 6520 7365 7269 6573 2077 686f  three series who
-00007fe0: 7365 2063 6f6c 6f72 7320 7769 6c6c 2062  se colors will b
-00007ff0: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-00008000: 6175 746f 6d61 7469 6361 6c6c 7920 7365  automatically se
-00008010: 6c65 6374 6564 2066 726f 6d20 7468 6520  lected from the 
-00008020: 6465 6661 756c 7420 7061 6c65 7474 652e  default palette.
-00008030: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00008040: 4275 742c 2069 6620 666f 7220 7468 6520  But, if for the 
-00008050: 7361 6d65 2031 3030 302d 726f 7720 6461  same 1000-row da
-00008060: 7461 7365 742c 2074 6869 7320 636f 6c75  taset, this colu
-00008070: 6d6e 2063 6f6e 7461 696e 6564 0a20 2020  mn contained.   
-00008080: 2020 2020 2020 2020 2020 2074 6865 2076             the v
-00008090: 616c 7565 7320 2223 6666 6161 3030 222c  alues "#ffaa00",
-000080a0: 2022 2366 3066 222c 2022 2330 3030 3066   "#f0f", "#0000f
-000080b0: 6622 2c20 7468 656e 2074 6865 6e20 7468  f", then then th
-000080c0: 6f73 6520 3130 3030 0a20 2020 2020 2020  ose 1000.       
-000080d0: 2020 2020 2020 2064 6174 6170 6f69 6e74         datapoint
-000080e0: 7320 776f 756c 6420 7374 696c 6c20 6265  s would still be
-000080f0: 2067 726f 7570 6564 2069 6e74 6f20 3320   grouped into 3 
-00008100: 7365 7269 6573 2c20 6275 7420 7468 6569  series, but thei
-00008110: 720a 2020 2020 2020 2020 2020 2020 2020  r.              
-00008120: 636f 6c6f 7273 2077 6f75 6c64 2062 6520  colors would be 
-00008130: 2223 6666 6161 3030 222c 2022 2366 3066  "#ffaa00", "#f0f
-00008140: 222c 2022 2330 3030 3066 6622 2074 6869  ", "#0000ff" thi
-00008150: 7320 7469 6d65 2061 726f 756e 642e 0a0a  s time around...
-00008160: 2020 2020 2020 2020 2020 2020 466f 7220              For 
-00008170: 6120 6261 7220 6368 6172 7420 7769 7468  a bar chart with
-00008180: 206d 756c 7469 706c 6520 7365 7269 6573   multiple series
-00008190: 2c20 7768 6572 6520 7468 6520 6461 7461  , where the data
-000081a0: 6672 616d 6520 6973 2069 6e0a 2020 2020  frame is in.    
-000081b0: 2020 2020 2020 2020 7769 6465 2066 6f72          wide for
-000081c0: 6d61 7420 2874 6861 7420 6973 2c20 7920  mat (that is, y 
-000081d0: 6973 2061 2053 6571 7565 6e63 6520 6f66  is a Sequence of
-000081e0: 2063 6f6c 756d 6e73 292c 2074 6869 7320   columns), this 
-000081f0: 6361 6e20 6265 3a0a 0a20 2020 2020 2020  can be:..       
-00008200: 2020 2020 202a 204e 6f6e 652c 2074 6f20       * None, to 
-00008210: 7573 6520 7468 6520 6465 6661 756c 7420  use the default 
-00008220: 636f 6c6f 7273 2e0a 2020 2020 2020 2020  colors..        
-00008230: 2020 2020 2a20 4120 6c69 7374 206f 6620      * A list of 
-00008240: 7374 7269 6e67 2063 6f6c 6f72 7320 6f72  string colors or
-00008250: 2063 6f6c 6f72 2074 7570 6c65 7320 746f   color tuples to
-00008260: 2062 6520 7573 6564 2066 6f72 2065 6163   be used for eac
-00008270: 6820 6f66 0a20 2020 2020 2020 2020 2020  h of.           
-00008280: 2020 2074 6865 2073 6572 6965 7320 696e     the series in
-00008290: 2074 6865 2063 6861 7274 2e20 5468 6973   the chart. This
-000082a0: 206c 6973 7420 7368 6f75 6c64 2068 6176   list should hav
-000082b0: 6520 7468 6520 7361 6d65 206c 656e 6774  e the same lengt
-000082c0: 680a 2020 2020 2020 2020 2020 2020 2020  h.              
-000082d0: 6173 2074 6865 206e 756d 6265 7220 6f66  as the number of
-000082e0: 2079 2076 616c 7565 7320 2865 2e67 2e20   y values (e.g. 
-000082f0: 6060 636f 6c6f 723d 5b22 2366 6430 222c  ``color=["#fd0",
-00008300: 2022 2366 3066 222c 2022 2330 3466 225d   "#f0f", "#04f"]
-00008310: 6060 0a20 2020 2020 2020 2020 2020 2020  ``.             
-00008320: 2066 6f72 2074 6872 6565 206c 696e 6573   for three lines
-00008330: 292e 0a0a 2020 2020 2020 2020 7769 6474  )...        widt
-00008340: 6820 3a20 696e 740a 2020 2020 2020 2020  h : int.        
-00008350: 2020 2020 5468 6520 6368 6172 7420 7769      The chart wi
-00008360: 6474 6820 696e 2070 6978 656c 732e 2049  dth in pixels. I
-00008370: 6620 302c 2073 656c 6563 7473 2074 6865  f 0, selects the
-00008380: 2077 6964 7468 2061 7574 6f6d 6174 6963   width automatic
-00008390: 616c 6c79 2e0a 0a20 2020 2020 2020 2068  ally...        h
-000083a0: 6569 6768 7420 3a20 696e 740a 2020 2020  eight : int.    
-000083b0: 2020 2020 2020 2020 5468 6520 6368 6172          The char
-000083c0: 7420 6865 6967 6874 2069 6e20 7069 7865  t height in pixe
-000083d0: 6c73 2e20 4966 2030 2c20 7365 6c65 6374  ls. If 0, select
-000083e0: 7320 7468 6520 6865 6967 6874 2061 7574  s the height aut
-000083f0: 6f6d 6174 6963 616c 6c79 2e0a 0a20 2020  omatically...   
-00008400: 2020 2020 2075 7365 5f63 6f6e 7461 696e       use_contain
-00008410: 6572 5f77 6964 7468 203a 2062 6f6f 6c0a  er_width : bool.
-00008420: 2020 2020 2020 2020 2020 2020 4966 2054              If T
-00008430: 7275 652c 2073 6574 2074 6865 2063 6861  rue, set the cha
-00008440: 7274 2077 6964 7468 2074 6f20 7468 6520  rt width to the 
-00008450: 636f 6c75 6d6e 2077 6964 7468 2e20 5468  column width. Th
-00008460: 6973 2074 616b 6573 0a20 2020 2020 2020  is takes.       
-00008470: 2020 2020 2070 7265 6365 6465 6e63 6520       precedence 
-00008480: 6f76 6572 2074 6865 2077 6964 7468 2061  over the width a
-00008490: 7267 756d 656e 742e 0a0a 2020 2020 2020  rgument...      
-000084a0: 2020 4578 616d 706c 6573 0a20 2020 2020    Examples.     
-000084b0: 2020 202d 2d2d 2d2d 2d2d 2d0a 2020 2020     --------.    
-000084c0: 2020 2020 3e3e 3e20 696d 706f 7274 2073      >>> import s
-000084d0: 7472 6561 6d6c 6974 2061 7320 7374 0a20  treamlit as st. 
-000084e0: 2020 2020 2020 203e 3e3e 2069 6d70 6f72         >>> impor
-000084f0: 7420 7061 6e64 6173 2061 7320 7064 0a20  t pandas as pd. 
-00008500: 2020 2020 2020 203e 3e3e 2069 6d70 6f72         >>> impor
-00008510: 7420 6e75 6d70 7920 6173 206e 700a 2020  t numpy as np.  
-00008520: 2020 2020 2020 3e3e 3e0a 2020 2020 2020        >>>.      
-00008530: 2020 3e3e 3e20 6368 6172 745f 6461 7461    >>> chart_data
-00008540: 203d 2070 642e 4461 7461 4672 616d 6528   = pd.DataFrame(
-00008550: 6e70 2e72 616e 646f 6d2e 7261 6e64 6e28  np.random.randn(
-00008560: 3230 2c20 3329 2c20 636f 6c75 6d6e 733d  20, 3), columns=
-00008570: 5b22 6122 2c20 2262 222c 2022 6322 5d29  ["a", "b", "c"])
-00008580: 0a20 2020 2020 2020 203e 3e3e 0a20 2020  .        >>>.   
-00008590: 2020 2020 203e 3e3e 2073 742e 6261 725f       >>> st.bar_
-000085a0: 6368 6172 7428 6368 6172 745f 6461 7461  chart(chart_data
-000085b0: 290a 0a20 2020 2020 2020 202e 2e20 6f75  )..        .. ou
-000085c0: 7470 7574 3a3a 0a20 2020 2020 2020 2020  tput::.         
-000085d0: 2020 6874 7470 733a 2f2f 646f 632d 6261    https://doc-ba
-000085e0: 722d 6368 6172 742e 7374 7265 616d 6c69  r-chart.streamli
-000085f0: 742e 6170 702f 0a20 2020 2020 2020 2020  t.app/.         
-00008600: 2020 6865 6967 6874 3a20 3434 3070 780a    height: 440px.
-00008610: 0a20 2020 2020 2020 2059 6f75 2063 616e  .        You can
-00008620: 2061 6c73 6f20 6368 6f6f 7365 2064 6966   also choose dif
-00008630: 6665 7265 6e74 2063 6f6c 756d 6e73 2074  ferent columns t
-00008640: 6f20 7573 6520 666f 7220 7820 616e 6420  o use for x and 
-00008650: 792c 2061 7320 7765 6c6c 2061 7320 7365  y, as well as se
-00008660: 740a 2020 2020 2020 2020 7468 6520 636f  t.        the co
-00008670: 6c6f 7220 6479 6e61 6d69 6361 6c6c 7920  lor dynamically 
-00008680: 6261 7365 6420 6f6e 2061 2033 7264 2063  based on a 3rd c
-00008690: 6f6c 756d 6e20 2861 7373 756d 696e 6720  olumn (assuming 
-000086a0: 796f 7572 2064 6174 6166 7261 6d65 2069  your dataframe i
-000086b0: 7320 696e 0a20 2020 2020 2020 206c 6f6e  s in.        lon
-000086c0: 6720 666f 726d 6174 293a 0a0a 2020 2020  g format):..    
-000086d0: 2020 2020 3e3e 3e20 696d 706f 7274 2073      >>> import s
-000086e0: 7472 6561 6d6c 6974 2061 7320 7374 0a20  treamlit as st. 
-000086f0: 2020 2020 2020 203e 3e3e 2069 6d70 6f72         >>> impor
-00008700: 7420 7061 6e64 6173 2061 7320 7064 0a20  t pandas as pd. 
-00008710: 2020 2020 2020 203e 3e3e 2069 6d70 6f72         >>> impor
-00008720: 7420 6e75 6d70 7920 6173 206e 700a 2020  t numpy as np.  
-00008730: 2020 2020 2020 3e3e 3e0a 2020 2020 2020        >>>.      
-00008740: 2020 3e3e 3e20 6368 6172 745f 6461 7461    >>> chart_data
-00008750: 203d 2070 642e 4461 7461 4672 616d 6528   = pd.DataFrame(
-00008760: 0a20 2020 2020 2020 202e 2e2e 2020 2020  .        ...    
-00008770: 7b0a 2020 2020 2020 2020 2e2e 2e20 2020  {.        ...   
-00008780: 2020 2020 2022 636f 6c31 223a 206c 6973       "col1": lis
-00008790: 7428 7261 6e67 6528 3230 2929 202a 2033  t(range(20)) * 3
-000087a0: 2c0a 2020 2020 2020 2020 2e2e 2e20 2020  ,.        ...   
-000087b0: 2020 2020 2022 636f 6c32 223a 206e 702e       "col2": np.
-000087c0: 7261 6e64 6f6d 2e72 616e 646e 2836 3029  random.randn(60)
-000087d0: 2c0a 2020 2020 2020 2020 2e2e 2e20 2020  ,.        ...   
-000087e0: 2020 2020 2022 636f 6c33 223a 205b 2241       "col3": ["A
-000087f0: 225d 202a 2032 3020 2b20 5b22 4222 5d20  "] * 20 + ["B"] 
-00008800: 2a20 3230 202b 205b 2243 225d 202a 2032  * 20 + ["C"] * 2
-00008810: 302c 0a20 2020 2020 2020 202e 2e2e 2020  0,.        ...  
-00008820: 2020 7d0a 2020 2020 2020 2020 2e2e 2e20    }.        ... 
-00008830: 290a 2020 2020 2020 2020 3e3e 3e0a 2020  ).        >>>.  
-00008840: 2020 2020 2020 3e3e 3e20 7374 2e62 6172        >>> st.bar
-00008850: 5f63 6861 7274 2863 6861 7274 5f64 6174  _chart(chart_dat
-00008860: 612c 2078 3d22 636f 6c31 222c 2079 3d22  a, x="col1", y="
-00008870: 636f 6c32 222c 2063 6f6c 6f72 3d22 636f  col2", color="co
-00008880: 6c33 2229 0a0a 2020 2020 2020 2020 2e2e  l3")..        ..
-00008890: 206f 7574 7075 743a 3a0a 2020 2020 2020   output::.      
-000088a0: 2020 2020 2068 7474 7073 3a2f 2f64 6f63       https://doc
-000088b0: 2d62 6172 2d63 6861 7274 312e 7374 7265  -bar-chart1.stre
-000088c0: 616d 6c69 742e 6170 702f 0a20 2020 2020  amlit.app/.     
-000088d0: 2020 2020 2020 6865 6967 6874 3a20 3434        height: 44
-000088e0: 3070 780a 0a20 2020 2020 2020 2046 696e  0px..        Fin
-000088f0: 616c 6c79 2c20 6966 2079 6f75 7220 6461  ally, if your da
-00008900: 7461 6672 616d 6520 6973 2069 6e20 7769  taframe is in wi
-00008910: 6465 2066 6f72 6d61 742c 2079 6f75 2063  de format, you c
-00008920: 616e 2067 726f 7570 206d 756c 7469 706c  an group multipl
-00008930: 650a 2020 2020 2020 2020 636f 6c75 6d6e  e.        column
-00008940: 7320 756e 6465 7220 7468 6520 7920 6172  s under the y ar
-00008950: 6775 6d65 6e74 2074 6f20 7368 6f77 206d  gument to show m
-00008960: 756c 7469 706c 6520 7365 7269 6573 2077  ultiple series w
-00008970: 6974 6820 6469 6666 6572 656e 740a 2020  ith different.  
-00008980: 2020 2020 2020 636f 6c6f 7273 3a0a 0a20        colors:.. 
-00008990: 2020 2020 2020 203e 3e3e 2069 6d70 6f72         >>> impor
-000089a0: 7420 7374 7265 616d 6c69 7420 6173 2073  t streamlit as s
-000089b0: 740a 2020 2020 2020 2020 3e3e 3e20 696d  t.        >>> im
-000089c0: 706f 7274 2070 616e 6461 7320 6173 2070  port pandas as p
-000089d0: 640a 2020 2020 2020 2020 3e3e 3e20 696d  d.        >>> im
-000089e0: 706f 7274 206e 756d 7079 2061 7320 6e70  port numpy as np
-000089f0: 0a20 2020 2020 2020 203e 3e3e 0a20 2020  .        >>>.   
-00008a00: 2020 2020 203e 3e3e 2063 6861 7274 5f64       >>> chart_d
-00008a10: 6174 6120 3d20 7064 2e44 6174 6146 7261  ata = pd.DataFra
-00008a20: 6d65 280a 2020 2020 2020 2020 2e2e 2e20  me(.        ... 
-00008a30: 2020 207b 2263 6f6c 3122 3a20 6c69 7374     {"col1": list
-00008a40: 2872 616e 6765 2832 3029 292c 2022 636f  (range(20)), "co
-00008a50: 6c32 223a 206e 702e 7261 6e64 6f6d 2e72  l2": np.random.r
-00008a60: 616e 646e 2832 3029 2c20 2263 6f6c 3322  andn(20), "col3"
-00008a70: 3a20 6e70 2e72 616e 646f 6d2e 7261 6e64  : np.random.rand
-00008a80: 6e28 3230 297d 0a20 2020 2020 2020 202e  n(20)}.        .
-00008a90: 2e2e 2029 0a20 2020 2020 2020 203e 3e3e  .. ).        >>>
-00008aa0: 0a20 2020 2020 2020 203e 3e3e 2073 742e  .        >>> st.
-00008ab0: 6261 725f 6368 6172 7428 0a20 2020 2020  bar_chart(.     
-00008ac0: 2020 202e 2e2e 2020 2020 6368 6172 745f     ...    chart_
-00008ad0: 6461 7461 2c20 783d 2263 6f6c 3122 2c20  data, x="col1", 
-00008ae0: 793d 5b22 636f 6c32 222c 2022 636f 6c33  y=["col2", "col3
-00008af0: 225d 2c20 636f 6c6f 723d 5b22 2346 4630  "], color=["#FF0
-00008b00: 3030 3022 2c20 2223 3030 3030 4646 225d  000", "#0000FF"]
-00008b10: 2020 2320 4f70 7469 6f6e 616c 0a20 2020    # Optional.   
-00008b20: 2020 2020 202e 2e2e 2029 0a0a 2020 2020       ... )..    
-00008b30: 2020 2020 2e2e 206f 7574 7075 743a 3a0a      .. output::.
-00008b40: 2020 2020 2020 2020 2020 2068 7474 7073             https
-00008b50: 3a2f 2f64 6f63 2d62 6172 2d63 6861 7274  ://doc-bar-chart
-00008b60: 322e 7374 7265 616d 6c69 742e 6170 702f  2.streamlit.app/
-00008b70: 0a20 2020 2020 2020 2020 2020 6865 6967  .           heig
-00008b80: 6874 3a20 3434 3070 780a 0a20 2020 2020  ht: 440px..     
-00008b90: 2020 2022 2222 0a0a 2020 2020 2020 2020     """..        
-00008ba0: 6368 6172 742c 2061 6464 5f72 6f77 735f  chart, add_rows_
-00008bb0: 6d65 7461 6461 7461 203d 2067 656e 6572  metadata = gener
-00008bc0: 6174 655f 6368 6172 7428 0a20 2020 2020  ate_chart(.     
-00008bd0: 2020 2020 2020 2063 6861 7274 5f74 7970         chart_typ
-00008be0: 653d 4368 6172 7454 7970 652e 4241 522c  e=ChartType.BAR,
-00008bf0: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
-00008c00: 613d 6461 7461 2c0a 2020 2020 2020 2020  a=data,.        
-00008c10: 2020 2020 785f 6672 6f6d 5f75 7365 723d      x_from_user=
-00008c20: 782c 0a20 2020 2020 2020 2020 2020 2079  x,.            y
-00008c30: 5f66 726f 6d5f 7573 6572 3d79 2c0a 2020  _from_user=y,.  
-00008c40: 2020 2020 2020 2020 2020 636f 6c6f 725f            color_
-00008c50: 6672 6f6d 5f75 7365 723d 636f 6c6f 722c  from_user=color,
-00008c60: 0a20 2020 2020 2020 2020 2020 2073 697a  .            siz
-00008c70: 655f 6672 6f6d 5f75 7365 723d 4e6f 6e65  e_from_user=None
-00008c80: 2c0a 2020 2020 2020 2020 2020 2020 7769  ,.            wi
-00008c90: 6474 683d 7769 6474 682c 0a20 2020 2020  dth=width,.     
-00008ca0: 2020 2020 2020 2068 6569 6768 743d 6865         height=he
-00008cb0: 6967 6874 2c0a 2020 2020 2020 2020 290a  ight,.        ).
-00008cc0: 2020 2020 2020 2020 7265 7475 726e 2063          return c
-00008cd0: 6173 7428 0a20 2020 2020 2020 2020 2020  ast(.           
-00008ce0: 2022 4465 6c74 6147 656e 6572 6174 6f72   "DeltaGenerator
-00008cf0: 222c 0a20 2020 2020 2020 2020 2020 2073  ",.            s
-00008d00: 656c 662e 5f61 6c74 6169 725f 6368 6172  elf._altair_char
-00008d10: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
-00008d20: 2020 2063 6861 7274 2c0a 2020 2020 2020     chart,.      
-00008d30: 2020 2020 2020 2020 2020 7573 655f 636f            use_co
-00008d40: 6e74 6169 6e65 725f 7769 6474 683d 7573  ntainer_width=us
-00008d50: 655f 636f 6e74 6169 6e65 725f 7769 6474  e_container_widt
-00008d60: 682c 0a20 2020 2020 2020 2020 2020 2020  h,.             
-00008d70: 2020 2074 6865 6d65 3d22 7374 7265 616d     theme="stream
-00008d80: 6c69 7422 2c0a 2020 2020 2020 2020 2020  lit",.          
-00008d90: 2020 2020 2020 6164 645f 726f 7773 5f6d        add_rows_m
-00008da0: 6574 6164 6174 613d 6164 645f 726f 7773  etadata=add_rows
-00008db0: 5f6d 6574 6164 6174 612c 0a20 2020 2020  _metadata,.     
-00008dc0: 2020 2020 2020 2029 2c0a 2020 2020 2020         ),.      
-00008dd0: 2020 290a 0a20 2020 2040 6761 7468 6572    )..    @gather
-00008de0: 5f6d 6574 7269 6373 2822 7363 6174 7465  _metrics("scatte
-00008df0: 725f 6368 6172 7422 290a 2020 2020 6465  r_chart").    de
-00008e00: 6620 7363 6174 7465 725f 6368 6172 7428  f scatter_chart(
-00008e10: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
-00008e20: 2020 2020 2020 2064 6174 613a 2044 6174         data: Dat
-00008e30: 6120 3d20 4e6f 6e65 2c0a 2020 2020 2020  a = None,.      
-00008e40: 2020 2a2c 0a20 2020 2020 2020 2078 3a20    *,.        x: 
-00008e50: 7374 7220 7c20 4e6f 6e65 203d 204e 6f6e  str | None = Non
-00008e60: 652c 0a20 2020 2020 2020 2079 3a20 7374  e,.        y: st
-00008e70: 7220 7c20 5365 7175 656e 6365 5b73 7472  r | Sequence[str
-00008e80: 5d20 7c20 4e6f 6e65 203d 204e 6f6e 652c  ] | None = None,
-00008e90: 0a20 2020 2020 2020 2063 6f6c 6f72 3a20  .        color: 
-00008ea0: 7374 7220 7c20 436f 6c6f 7220 7c20 6c69  str | Color | li
-00008eb0: 7374 5b43 6f6c 6f72 5d20 7c20 4e6f 6e65  st[Color] | None
-00008ec0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-00008ed0: 2073 697a 653a 2073 7472 207c 2066 6c6f   size: str | flo
-00008ee0: 6174 207c 2069 6e74 207c 204e 6f6e 6520  at | int | None 
-00008ef0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-00008f00: 7769 6474 683a 2069 6e74 203d 2030 2c0a  width: int = 0,.
-00008f10: 2020 2020 2020 2020 6865 6967 6874 3a20          height: 
-00008f20: 696e 7420 3d20 302c 0a20 2020 2020 2020  int = 0,.       
-00008f30: 2075 7365 5f63 6f6e 7461 696e 6572 5f77   use_container_w
-00008f40: 6964 7468 3a20 626f 6f6c 203d 2054 7275  idth: bool = Tru
-00008f50: 652c 0a20 2020 2029 202d 3e20 4465 6c74  e,.    ) -> Delt
-00008f60: 6147 656e 6572 6174 6f72 3a0a 2020 2020  aGenerator:.    
-00008f70: 2020 2020 2222 2244 6973 706c 6179 2061      """Display a
-00008f80: 2073 6361 7474 6572 706c 6f74 2063 6861   scatterplot cha
-00008f90: 7274 2e0a 0a20 2020 2020 2020 2054 6869  rt...        Thi
-00008fa0: 7320 6973 2073 796e 7461 782d 7375 6761  s is syntax-suga
-00008fb0: 7220 6172 6f75 6e64 2060 6073 742e 616c  r around ``st.al
-00008fc0: 7461 6972 5f63 6861 7274 6060 2e20 5468  tair_chart``. Th
-00008fd0: 6520 6d61 696e 2064 6966 6665 7265 6e63  e main differenc
-00008fe0: 650a 2020 2020 2020 2020 6973 2074 6869  e.        is thi
-00008ff0: 7320 636f 6d6d 616e 6420 7573 6573 2074  s command uses t
-00009000: 6865 2064 6174 6127 7320 6f77 6e20 636f  he data's own co
-00009010: 6c75 6d6e 2061 6e64 2069 6e64 6963 6573  lumn and indices
-00009020: 2074 6f20 6669 6775 7265 206f 7574 0a20   to figure out. 
-00009030: 2020 2020 2020 2074 6865 2063 6861 7274         the chart
-00009040: 2773 2073 7065 632e 2041 7320 6120 7265  's spec. As a re
-00009050: 7375 6c74 2074 6869 7320 6973 2065 6173  sult this is eas
-00009060: 6965 7220 746f 2075 7365 2066 6f72 206d  ier to use for m
-00009070: 616e 7920 226a 7573 7420 706c 6f74 0a20  any "just plot. 
-00009080: 2020 2020 2020 2074 6869 7322 2073 6365         this" sce
-00009090: 6e61 7269 6f73 2c20 7768 696c 6520 6265  narios, while be
-000090a0: 696e 6720 6c65 7373 2063 7573 746f 6d69  ing less customi
-000090b0: 7a61 626c 652e 0a0a 2020 2020 2020 2020  zable...        
-000090c0: 4966 2060 6073 742e 7363 6174 7465 725f  If ``st.scatter_
-000090d0: 6368 6172 7460 6020 646f 6573 206e 6f74  chart`` does not
-000090e0: 2067 7565 7373 2074 6865 2064 6174 6120   guess the data 
-000090f0: 7370 6563 6966 6963 6174 696f 6e20 636f  specification co
-00009100: 7272 6563 746c 792c 0a20 2020 2020 2020  rrectly,.       
-00009110: 2074 7279 2073 7065 6369 6679 696e 6720   try specifying 
-00009120: 796f 7572 2064 6573 6972 6564 2063 6861  your desired cha
-00009130: 7274 2075 7369 6e67 2060 6073 742e 616c  rt using ``st.al
-00009140: 7461 6972 5f63 6861 7274 6060 2e0a 0a20  tair_chart``... 
-00009150: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
-00009160: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
-00009170: 2d2d 2d2d 0a20 2020 2020 2020 2064 6174  ----.        dat
-00009180: 6120 3a20 7061 6e64 6173 2e44 6174 6146  a : pandas.DataF
-00009190: 7261 6d65 2c20 7061 6e64 6173 2e53 7479  rame, pandas.Sty
-000091a0: 6c65 722c 2070 7961 7272 6f77 2e54 6162  ler, pyarrow.Tab
-000091b0: 6c65 2c20 6e75 6d70 792e 6e64 6172 7261  le, numpy.ndarra
-000091c0: 792c 2070 7973 7061 726b 2e73 716c 2e44  y, pyspark.sql.D
-000091d0: 6174 6146 7261 6d65 2c20 736e 6f77 666c  ataFrame, snowfl
-000091e0: 616b 652e 736e 6f77 7061 726b 2e64 6174  ake.snowpark.dat
-000091f0: 6166 7261 6d65 2e44 6174 6146 7261 6d65  aframe.DataFrame
-00009200: 2c20 736e 6f77 666c 616b 652e 736e 6f77  , snowflake.snow
-00009210: 7061 726b 2e74 6162 6c65 2e54 6162 6c65  park.table.Table
-00009220: 2c20 4974 6572 6162 6c65 2c20 6469 6374  , Iterable, dict
-00009230: 206f 7220 4e6f 6e65 0a20 2020 2020 2020   or None.       
-00009240: 2020 2020 2044 6174 6120 746f 2062 6520       Data to be 
-00009250: 706c 6f74 7465 642e 0a0a 2020 2020 2020  plotted...      
-00009260: 2020 7820 3a20 7374 7220 6f72 204e 6f6e    x : str or Non
-00009270: 650a 2020 2020 2020 2020 2020 2020 436f  e.            Co
-00009280: 6c75 6d6e 206e 616d 6520 746f 2075 7365  lumn name to use
-00009290: 2066 6f72 2074 6865 2078 2d61 7869 732e   for the x-axis.
-000092a0: 2049 6620 4e6f 6e65 2c20 7573 6573 2074   If None, uses t
-000092b0: 6865 2064 6174 6120 696e 6465 7820 666f  he data index fo
-000092c0: 7220 7468 6520 782d 6178 6973 2e0a 0a20  r the x-axis... 
-000092d0: 2020 2020 2020 2079 203a 2073 7472 2c20         y : str, 
-000092e0: 5365 7175 656e 6365 206f 6620 7374 722c  Sequence of str,
-000092f0: 206f 7220 4e6f 6e65 0a20 2020 2020 2020   or None.       
-00009300: 2020 2020 2043 6f6c 756d 6e20 6e61 6d65       Column name
-00009310: 2873 2920 746f 2075 7365 2066 6f72 2074  (s) to use for t
-00009320: 6865 2079 2d61 7869 732e 2049 6620 6120  he y-axis. If a 
-00009330: 5365 7175 656e 6365 206f 6620 7374 7269  Sequence of stri
-00009340: 6e67 732c 0a20 2020 2020 2020 2020 2020  ngs,.           
-00009350: 2064 7261 7773 2073 6576 6572 616c 2073   draws several s
-00009360: 6572 6965 7320 6f6e 2074 6865 2073 616d  eries on the sam
-00009370: 6520 6368 6172 7420 6279 206d 656c 7469  e chart by melti
-00009380: 6e67 2079 6f75 7220 7769 6465 2d66 6f72  ng your wide-for
-00009390: 6d61 740a 2020 2020 2020 2020 2020 2020  mat.            
-000093a0: 7461 626c 6520 696e 746f 2061 206c 6f6e  table into a lon
-000093b0: 672d 666f 726d 6174 2074 6162 6c65 2062  g-format table b
-000093c0: 6568 696e 6420 7468 6520 7363 656e 6573  ehind the scenes
-000093d0: 2e20 4966 204e 6f6e 652c 2064 7261 7773  . If None, draws
-000093e0: 0a20 2020 2020 2020 2020 2020 2074 6865  .            the
-000093f0: 2064 6174 6120 6f66 2061 6c6c 2072 656d   data of all rem
-00009400: 6169 6e69 6e67 2063 6f6c 756d 6e73 2061  aining columns a
-00009410: 7320 6461 7461 2073 6572 6965 732e 0a0a  s data series...
-00009420: 2020 2020 2020 2020 636f 6c6f 7220 3a20          color : 
-00009430: 7374 722c 2074 7570 6c65 2c20 5365 7175  str, tuple, Sequ
-00009440: 656e 6365 206f 6620 7374 722c 2053 6571  ence of str, Seq
-00009450: 7565 6e63 6520 6f66 2074 7570 6c65 2c20  uence of tuple, 
-00009460: 6f72 204e 6f6e 650a 2020 2020 2020 2020  or None.        
-00009470: 2020 2020 5468 6520 636f 6c6f 7220 6f66      The color of
-00009480: 2074 6865 2063 6972 636c 6573 2072 6570   the circles rep
-00009490: 7265 7365 6e74 696e 6720 6561 6368 2064  resenting each d
-000094a0: 6174 6170 6f69 6e74 2e0a 0a20 2020 2020  atapoint...     
-000094b0: 2020 2020 2020 2054 6869 7320 6361 6e20         This can 
-000094c0: 6265 3a0a 0a20 2020 2020 2020 2020 2020  be:..           
-000094d0: 202a 204e 6f6e 652c 2074 6f20 7573 6520   * None, to use 
-000094e0: 7468 6520 6465 6661 756c 7420 636f 6c6f  the default colo
-000094f0: 722e 0a20 2020 2020 2020 2020 2020 202a  r..            *
-00009500: 2041 2068 6578 2073 7472 696e 6720 6c69   A hex string li
-00009510: 6b65 2022 2366 6661 6130 3022 206f 7220  ke "#ffaa00" or 
-00009520: 2223 6666 6161 3030 3838 222e 0a20 2020  "#ffaa0088"..   
-00009530: 2020 2020 2020 2020 202a 2041 6e20 5247           * An RG
-00009540: 4220 6f72 2052 4742 4120 7475 706c 6520  B or RGBA tuple 
-00009550: 7769 7468 2074 6865 2072 6564 2c20 6772  with the red, gr
-00009560: 6565 6e2c 2062 6c75 652c 2061 6e64 2061  een, blue, and a
-00009570: 6c70 6861 0a20 2020 2020 2020 2020 2020  lpha.           
-00009580: 2020 2063 6f6d 706f 6e65 6e74 7320 7370     components sp
-00009590: 6563 6966 6965 6420 6173 2069 6e74 7320  ecified as ints 
-000095a0: 6672 6f6d 2030 2074 6f20 3235 3520 6f72  from 0 to 255 or
-000095b0: 2066 6c6f 6174 7320 6672 6f6d 2030 2e30   floats from 0.0
-000095c0: 2074 6f0a 2020 2020 2020 2020 2020 2020   to.            
-000095d0: 2020 312e 302e 0a20 2020 2020 2020 2020    1.0..         
-000095e0: 2020 202a 2054 6865 206e 616d 6520 6f66     * The name of
-000095f0: 2061 2063 6f6c 756d 6e20 696e 2074 6865   a column in the
-00009600: 2064 6174 6173 6574 2077 6865 7265 2074   dataset where t
-00009610: 6865 2063 6f6c 6f72 206f 6620 7468 6174  he color of that
-00009620: 0a20 2020 2020 2020 2020 2020 2020 2064  .              d
-00009630: 6174 6170 6f69 6e74 2077 696c 6c20 636f  atapoint will co
-00009640: 6d65 2066 726f 6d2e 0a0a 2020 2020 2020  me from...      
-00009650: 2020 2020 2020 2020 4966 2074 6865 2076          If the v
-00009660: 616c 7565 7320 696e 2074 6869 7320 636f  alues in this co
-00009670: 6c75 6d6e 2061 7265 2069 6e20 6f6e 6520  lumn are in one 
-00009680: 6f66 2074 6865 2063 6f6c 6f72 2066 6f72  of the color for
-00009690: 6d61 7473 0a20 2020 2020 2020 2020 2020  mats.           
-000096a0: 2020 2061 626f 7665 2028 6865 7820 7374     above (hex st
-000096b0: 7269 6e67 206f 7220 636f 6c6f 7220 7475  ring or color tu
-000096c0: 706c 6529 2c20 7468 656e 2074 6861 7420  ple), then that 
-000096d0: 636f 6c6f 7220 7769 6c6c 2062 6520 7573  color will be us
-000096e0: 6564 2e0a 0a20 2020 2020 2020 2020 2020  ed...           
-000096f0: 2020 204f 7468 6572 7769 7365 2c20 7468     Otherwise, th
-00009700: 6520 636f 6c6f 7220 7769 6c6c 2062 6520  e color will be 
-00009710: 6175 746f 6d61 7469 6361 6c6c 7920 7069  automatically pi
-00009720: 636b 6564 2066 726f 6d20 7468 650a 2020  cked from the.  
-00009730: 2020 2020 2020 2020 2020 2020 6465 6661              defa
-00009740: 756c 7420 7061 6c65 7474 652e 0a0a 2020  ult palette...  
-00009750: 2020 2020 2020 2020 2020 2020 466f 7220              For 
-00009760: 6578 616d 706c 653a 2069 6620 7468 6520  example: if the 
-00009770: 6461 7461 7365 7420 6861 7320 3130 3030  dataset has 1000
-00009780: 2072 6f77 732c 2062 7574 2074 6869 7320   rows, but this 
-00009790: 636f 6c75 6d6e 206f 6e6c 790a 2020 2020  column only.    
-000097a0: 2020 2020 2020 2020 2020 636f 6e74 6169            contai
-000097b0: 6e73 2074 6865 2076 616c 7565 7320 2261  ns the values "a
-000097c0: 6475 6c74 222c 2022 6368 696c 6422 2c20  dult", "child", 
-000097d0: 616e 6420 2262 6162 7922 2c20 7468 656e  and "baby", then
-000097e0: 2074 686f 7365 2031 3030 300a 2020 2020   those 1000.    
-000097f0: 2020 2020 2020 2020 2020 6461 7461 706f            datapo
-00009800: 696e 7473 2062 6520 7368 6f77 6e20 7573  ints be shown us
-00009810: 696e 6720 7468 7265 6520 636f 6c6f 7273  ing three colors
-00009820: 2066 726f 6d20 7468 6520 6465 6661 756c   from the defaul
-00009830: 7420 7061 6c65 7474 652e 0a0a 2020 2020  t palette...    
-00009840: 2020 2020 2020 2020 2020 4275 7420 6966            But if
-00009850: 2074 6869 7320 636f 6c75 6d6e 206f 6e6c   this column onl
-00009860: 7920 636f 6e74 6169 6e73 2066 6c6f 6174  y contains float
-00009870: 7320 6f72 2069 6e74 732c 2074 6865 6e20  s or ints, then 
-00009880: 7468 6f73 650a 2020 2020 2020 2020 2020  those.          
-00009890: 2020 2020 3130 3030 2064 6174 6170 6f69      1000 datapoi
-000098a0: 6e74 7320 7769 6c6c 2062 6520 7368 6f77  nts will be show
-000098b0: 6e20 7573 696e 6720 6120 636f 6c6f 7273  n using a colors
-000098c0: 2066 726f 6d20 6120 636f 6e74 696e 756f   from a continuo
-000098d0: 7573 0a20 2020 2020 2020 2020 2020 2020  us.             
-000098e0: 2063 6f6c 6f72 2067 7261 6469 656e 742e   color gradient.
-000098f0: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00009900: 4669 6e61 6c6c 792c 2069 6620 7468 6973  Finally, if this
-00009910: 2063 6f6c 756d 6e20 6f6e 6c79 2063 6f6e   column only con
-00009920: 7461 696e 7320 7468 6520 7661 6c75 6573  tains the values
-00009930: 2022 2366 6661 6130 3022 2c0a 2020 2020   "#ffaa00",.    
-00009940: 2020 2020 2020 2020 2020 2223 6630 6622            "#f0f"
-00009950: 2c20 2223 3030 3030 6666 222c 2074 6865  , "#0000ff", the
-00009960: 6e20 7468 656e 2065 6163 6820 6f66 2074  n then each of t
-00009970: 686f 7365 2031 3030 3020 6461 7461 706f  hose 1000 datapo
-00009980: 696e 7473 2077 696c 6c0a 2020 2020 2020  ints will.      
-00009990: 2020 2020 2020 2020 6265 2061 7373 6967          be assig
-000099a0: 6e65 6420 2223 6666 6161 3030 222c 2022  ned "#ffaa00", "
-000099b0: 2366 3066 222c 206f 7220 2223 3030 3030  #f0f", or "#0000
-000099c0: 6666 2220 6173 2061 7070 726f 7072 6961  ff" as appropria
-000099d0: 7465 2e0a 0a20 2020 2020 2020 2020 2020  te...           
-000099e0: 2049 6620 7468 6520 6461 7461 6672 616d   If the datafram
-000099f0: 6520 6973 2069 6e20 7769 6465 2066 6f72  e is in wide for
-00009a00: 6d61 7420 2874 6861 7420 6973 2c20 7920  mat (that is, y 
-00009a10: 6973 2061 2053 6571 7565 6e63 6520 6f66  is a Sequence of
-00009a20: 0a20 2020 2020 2020 2020 2020 2063 6f6c  .            col
-00009a30: 756d 6e73 292c 2074 6869 7320 6361 6e20  umns), this can 
-00009a40: 616c 736f 2062 653a 0a0a 2020 2020 2020  also be:..      
-00009a50: 2020 2020 2020 2a20 4120 6c69 7374 206f        * A list o
-00009a60: 6620 7374 7269 6e67 2063 6f6c 6f72 7320  f string colors 
-00009a70: 6f72 2063 6f6c 6f72 2074 7570 6c65 7320  or color tuples 
-00009a80: 746f 2062 6520 7573 6564 2066 6f72 2065  to be used for e
-00009a90: 6163 6820 6f66 0a20 2020 2020 2020 2020  ach of.         
-00009aa0: 2020 2020 2074 6865 2073 6572 6965 7320       the series 
-00009ab0: 696e 2074 6865 2063 6861 7274 2e20 5468  in the chart. Th
-00009ac0: 6973 206c 6973 7420 7368 6f75 6c64 2068  is list should h
-00009ad0: 6176 6520 7468 6520 7361 6d65 206c 656e  ave the same len
-00009ae0: 6774 680a 2020 2020 2020 2020 2020 2020  gth.            
-00009af0: 2020 6173 2074 6865 206e 756d 6265 7220    as the number 
-00009b00: 6f66 2079 2076 616c 7565 7320 2865 2e67  of y values (e.g
-00009b10: 2e20 6060 636f 6c6f 723d 5b22 2366 6430  . ``color=["#fd0
-00009b20: 222c 2022 2366 3066 222c 2022 2330 3466  ", "#f0f", "#04f
-00009b30: 225d 6060 0a20 2020 2020 2020 2020 2020  "]``.           
-00009b40: 2020 2066 6f72 2074 6872 6565 2073 6572     for three ser
-00009b50: 6965 7329 2e0a 0a20 2020 2020 2020 2073  ies)...        s
-00009b60: 697a 6520 3a20 7374 722c 2066 6c6f 6174  ize : str, float
-00009b70: 2c20 696e 742c 206f 7220 4e6f 6e65 0a20  , int, or None. 
-00009b80: 2020 2020 2020 2020 2020 2054 6865 2073             The s
-00009b90: 697a 6520 6f66 2074 6865 2063 6972 636c  ize of the circl
-00009ba0: 6573 2072 6570 7265 7365 6e74 696e 6720  es representing 
-00009bb0: 6561 6368 2070 6f69 6e74 2e0a 0a20 2020  each point...   
-00009bc0: 2020 2020 2020 2020 2054 6869 7320 6361           This ca
-00009bd0: 6e20 6265 3a0a 0a20 2020 2020 2020 2020  n be:..         
-00009be0: 2020 202a 2041 206e 756d 6265 7220 6c69     * A number li
-00009bf0: 6b65 2031 3030 2c20 746f 2073 7065 6369  ke 100, to speci
-00009c00: 6679 2061 2073 696e 676c 6520 7369 7a65  fy a single size
-00009c10: 2074 6f20 7573 6520 666f 7220 616c 6c0a   to use for all.
-00009c20: 2020 2020 2020 2020 2020 2020 2020 6461                da
-00009c30: 7461 706f 696e 7473 2e0a 2020 2020 2020  tapoints..      
-00009c40: 2020 2020 2020 2a20 5468 6520 6e61 6d65        * The name
-00009c50: 206f 6620 7468 6520 636f 6c75 6d6e 2074   of the column t
-00009c60: 6f20 7573 6520 666f 7220 7468 6520 7369  o use for the si
-00009c70: 7a65 2e20 5468 6973 2061 6c6c 6f77 7320  ze. This allows 
-00009c80: 6561 6368 0a20 2020 2020 2020 2020 2020  each.           
-00009c90: 2020 2064 6174 6170 6f69 6e74 2074 6f20     datapoint to 
-00009ca0: 6265 2072 6570 7265 7365 6e74 6564 2062  be represented b
-00009cb0: 7920 6120 6369 7263 6c65 206f 6620 6120  y a circle of a 
-00009cc0: 6469 6666 6572 656e 7420 7369 7a65 2e0a  different size..
-00009cd0: 0a20 2020 2020 2020 2077 6964 7468 203a  .        width :
-00009ce0: 2069 6e74 0a20 2020 2020 2020 2020 2020   int.           
-00009cf0: 2054 6865 2063 6861 7274 2077 6964 7468   The chart width
-00009d00: 2069 6e20 7069 7865 6c73 2e20 4966 2030   in pixels. If 0
-00009d10: 2c20 7365 6c65 6374 7320 7468 6520 7769  , selects the wi
-00009d20: 6474 6820 6175 746f 6d61 7469 6361 6c6c  dth automaticall
-00009d30: 792e 0a0a 2020 2020 2020 2020 6865 6967  y...        heig
-00009d40: 6874 203a 2069 6e74 0a20 2020 2020 2020  ht : int.       
-00009d50: 2020 2020 2054 6865 2063 6861 7274 2068       The chart h
-00009d60: 6569 6768 7420 696e 2070 6978 656c 732e  eight in pixels.
-00009d70: 2049 6620 302c 2073 656c 6563 7473 2074   If 0, selects t
-00009d80: 6865 2068 6569 6768 7420 6175 746f 6d61  he height automa
-00009d90: 7469 6361 6c6c 792e 0a0a 2020 2020 2020  tically...      
-00009da0: 2020 7573 655f 636f 6e74 6169 6e65 725f    use_container_
-00009db0: 7769 6474 6820 3a20 626f 6f6c 0a20 2020  width : bool.   
-00009dc0: 2020 2020 2020 2020 2049 6620 5472 7565           If True
-00009dd0: 2c20 7365 7420 7468 6520 6368 6172 7420  , set the chart 
-00009de0: 7769 6474 6820 746f 2074 6865 2063 6f6c  width to the col
-00009df0: 756d 6e20 7769 6474 682e 2054 6869 7320  umn width. This 
-00009e00: 7461 6b65 730a 2020 2020 2020 2020 2020  takes.          
-00009e10: 2020 7072 6563 6564 656e 6365 206f 7665    precedence ove
-00009e20: 7220 7468 6520 7769 6474 6820 6172 6775  r the width argu
-00009e30: 6d65 6e74 2e0a 0a20 2020 2020 2020 2045  ment...        E
-00009e40: 7861 6d70 6c65 730a 2020 2020 2020 2020  xamples.        
-00009e50: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
-00009e60: 203e 3e3e 2069 6d70 6f72 7420 7374 7265   >>> import stre
-00009e70: 616d 6c69 7420 6173 2073 740a 2020 2020  amlit as st.    
-00009e80: 2020 2020 3e3e 3e20 696d 706f 7274 2070      >>> import p
-00009e90: 616e 6461 7320 6173 2070 640a 2020 2020  andas as pd.    
-00009ea0: 2020 2020 3e3e 3e20 696d 706f 7274 206e      >>> import n
-00009eb0: 756d 7079 2061 7320 6e70 0a20 2020 2020  umpy as np.     
-00009ec0: 2020 203e 3e3e 0a20 2020 2020 2020 203e     >>>.        >
-00009ed0: 3e3e 2063 6861 7274 5f64 6174 6120 3d20  >> chart_data = 
-00009ee0: 7064 2e44 6174 6146 7261 6d65 286e 702e  pd.DataFrame(np.
-00009ef0: 7261 6e64 6f6d 2e72 616e 646e 2832 302c  random.randn(20,
-00009f00: 2033 292c 2063 6f6c 756d 6e73 3d5b 2261   3), columns=["a
-00009f10: 222c 2022 6222 2c20 2263 225d 290a 2020  ", "b", "c"]).  
-00009f20: 2020 2020 2020 3e3e 3e0a 2020 2020 2020        >>>.      
-00009f30: 2020 3e3e 3e20 7374 2e73 6361 7474 6572    >>> st.scatter
-00009f40: 5f63 6861 7274 2863 6861 7274 5f64 6174  _chart(chart_dat
-00009f50: 6129 0a0a 2020 2020 2020 2020 2e2e 206f  a)..        .. o
-00009f60: 7574 7075 743a 3a0a 2020 2020 2020 2020  utput::.        
-00009f70: 2020 2068 7474 7073 3a2f 2f64 6f63 2d73     https://doc-s
-00009f80: 6361 7474 6572 2d63 6861 7274 2e73 7472  catter-chart.str
-00009f90: 6561 6d6c 6974 2e61 7070 2f0a 2020 2020  eamlit.app/.    
-00009fa0: 2020 2020 2020 2068 6569 6768 743a 2034         height: 4
-00009fb0: 3430 7078 0a0a 2020 2020 2020 2020 596f  40px..        Yo
-00009fc0: 7520 6361 6e20 616c 736f 2063 686f 6f73  u can also choos
-00009fd0: 6520 6469 6666 6572 656e 7420 636f 6c75  e different colu
-00009fe0: 6d6e 7320 746f 2075 7365 2066 6f72 2078  mns to use for x
-00009ff0: 2061 6e64 2079 2c20 6173 2077 656c 6c20   and y, as well 
-0000a000: 6173 2073 6574 0a20 2020 2020 2020 2074  as set.        t
-0000a010: 6865 2063 6f6c 6f72 2064 796e 616d 6963  he color dynamic
-0000a020: 616c 6c79 2062 6173 6564 206f 6e20 6120  ally based on a 
-0000a030: 3372 6420 636f 6c75 6d6e 2028 6173 7375  3rd column (assu
-0000a040: 6d69 6e67 2079 6f75 7220 6461 7461 6672  ming your datafr
-0000a050: 616d 6520 6973 2069 6e0a 2020 2020 2020  ame is in.      
-0000a060: 2020 6c6f 6e67 2066 6f72 6d61 7429 3a0a    long format):.
-0000a070: 0a20 2020 2020 2020 203e 3e3e 2069 6d70  .        >>> imp
-0000a080: 6f72 7420 7374 7265 616d 6c69 7420 6173  ort streamlit as
-0000a090: 2073 740a 2020 2020 2020 2020 3e3e 3e20   st.        >>> 
-0000a0a0: 696d 706f 7274 2070 616e 6461 7320 6173  import pandas as
-0000a0b0: 2070 640a 2020 2020 2020 2020 3e3e 3e20   pd.        >>> 
-0000a0c0: 696d 706f 7274 206e 756d 7079 2061 7320  import numpy as 
-0000a0d0: 6e70 0a20 2020 2020 2020 203e 3e3e 0a20  np.        >>>. 
-0000a0e0: 2020 2020 2020 203e 3e3e 2063 6861 7274         >>> chart
-0000a0f0: 5f64 6174 6120 3d20 7064 2e44 6174 6146  _data = pd.DataF
-0000a100: 7261 6d65 286e 702e 7261 6e64 6f6d 2e72  rame(np.random.r
-0000a110: 616e 646e 2832 302c 2033 292c 2063 6f6c  andn(20, 3), col
-0000a120: 756d 6e73 3d5b 2263 6f6c 3122 2c20 2263  umns=["col1", "c
-0000a130: 6f6c 3222 2c20 2263 6f6c 3322 5d29 0a20  ol2", "col3"]). 
-0000a140: 2020 2020 2020 203e 3e3e 2063 6861 7274         >>> chart
-0000a150: 5f64 6174 615b 2763 6f6c 3427 5d20 3d20  _data['col4'] = 
-0000a160: 6e70 2e72 616e 646f 6d2e 6368 6f69 6365  np.random.choice
-0000a170: 285b 2741 272c 2742 272c 2743 275d 2c20  (['A','B','C'], 
-0000a180: 3230 290a 2020 2020 2020 2020 3e3e 3e0a  20).        >>>.
-0000a190: 2020 2020 2020 2020 3e3e 3e20 7374 2e73          >>> st.s
-0000a1a0: 6361 7474 6572 5f63 6861 7274 280a 2020  catter_chart(.  
-0000a1b0: 2020 2020 2020 2e2e 2e20 2020 2020 6368        ...     ch
-0000a1c0: 6172 745f 6461 7461 2c0a 2020 2020 2020  art_data,.      
-0000a1d0: 2020 2e2e 2e20 2020 2020 783d 2763 6f6c    ...     x='col
-0000a1e0: 3127 2c0a 2020 2020 2020 2020 2e2e 2e20  1',.        ... 
-0000a1f0: 2020 2020 793d 2763 6f6c 3227 2c0a 2020      y='col2',.  
-0000a200: 2020 2020 2020 2e2e 2e20 2020 2020 636f        ...     co
-0000a210: 6c6f 723d 2763 6f6c 3427 2c0a 2020 2020  lor='col4',.    
-0000a220: 2020 2020 2e2e 2e20 2020 2020 7369 7a65      ...     size
-0000a230: 3d27 636f 6c33 272c 0a20 2020 2020 2020  ='col3',.       
-0000a240: 202e 2e2e 2029 0a0a 2020 2020 2020 2020   ... )..        
-0000a250: 2e2e 206f 7574 7075 743a 3a0a 2020 2020  .. output::.    
-0000a260: 2020 2020 2020 2068 7474 7073 3a2f 2f64         https://d
-0000a270: 6f63 2d73 6361 7474 6572 2d63 6861 7274  oc-scatter-chart
-0000a280: 312e 7374 7265 616d 6c69 742e 6170 702f  1.streamlit.app/
-0000a290: 0a20 2020 2020 2020 2020 2020 6865 6967  .           heig
-0000a2a0: 6874 3a20 3434 3070 780a 0a20 2020 2020  ht: 440px..     
-0000a2b0: 2020 2046 696e 616c 6c79 2c20 6966 2079     Finally, if y
-0000a2c0: 6f75 7220 6461 7461 6672 616d 6520 6973  our dataframe is
-0000a2d0: 2069 6e20 7769 6465 2066 6f72 6d61 742c   in wide format,
-0000a2e0: 2079 6f75 2063 616e 2067 726f 7570 206d   you can group m
-0000a2f0: 756c 7469 706c 650a 2020 2020 2020 2020  ultiple.        
-0000a300: 636f 6c75 6d6e 7320 756e 6465 7220 7468  columns under th
-0000a310: 6520 7920 6172 6775 6d65 6e74 2074 6f20  e y argument to 
-0000a320: 7368 6f77 206d 756c 7469 706c 6520 7365  show multiple se
-0000a330: 7269 6573 2077 6974 6820 6469 6666 6572  ries with differ
-0000a340: 656e 740a 2020 2020 2020 2020 636f 6c6f  ent.        colo
-0000a350: 7273 3a0a 0a20 2020 2020 2020 203e 3e3e  rs:..        >>>
-0000a360: 2069 6d70 6f72 7420 7374 7265 616d 6c69   import streamli
-0000a370: 7420 6173 2073 740a 2020 2020 2020 2020  t as st.        
-0000a380: 3e3e 3e20 696d 706f 7274 2070 616e 6461  >>> import panda
-0000a390: 7320 6173 2070 640a 2020 2020 2020 2020  s as pd.        
-0000a3a0: 3e3e 3e20 696d 706f 7274 206e 756d 7079  >>> import numpy
-0000a3b0: 2061 7320 6e70 0a20 2020 2020 2020 203e   as np.        >
-0000a3c0: 3e3e 0a20 2020 2020 2020 203e 3e3e 2063  >>.        >>> c
-0000a3d0: 6861 7274 5f64 6174 6120 3d20 7064 2e44  hart_data = pd.D
-0000a3e0: 6174 6146 7261 6d65 286e 702e 7261 6e64  ataFrame(np.rand
-0000a3f0: 6f6d 2e72 616e 646e 2832 302c 2034 292c  om.randn(20, 4),
-0000a400: 2063 6f6c 756d 6e73 3d5b 2263 6f6c 3122   columns=["col1"
-0000a410: 2c20 2263 6f6c 3222 2c20 2263 6f6c 3322  , "col2", "col3"
-0000a420: 2c20 2263 6f6c 3422 5d29 0a20 2020 2020  , "col4"]).     
-0000a430: 2020 203e 3e3e 0a20 2020 2020 2020 203e     >>>.        >
-0000a440: 3e3e 2073 742e 7363 6174 7465 725f 6368  >> st.scatter_ch
-0000a450: 6172 7428 0a20 2020 2020 2020 202e 2e2e  art(.        ...
-0000a460: 2020 2020 2063 6861 7274 5f64 6174 612c       chart_data,
-0000a470: 0a20 2020 2020 2020 202e 2e2e 2020 2020  .        ...    
-0000a480: 2078 3d27 636f 6c31 272c 0a20 2020 2020   x='col1',.     
-0000a490: 2020 202e 2e2e 2020 2020 2079 3d5b 2763     ...     y=['c
-0000a4a0: 6f6c 3227 2c20 2763 6f6c 3327 5d2c 0a20  ol2', 'col3'],. 
-0000a4b0: 2020 2020 2020 202e 2e2e 2020 2020 2073         ...     s
-0000a4c0: 697a 653d 2763 6f6c 3427 2c0a 2020 2020  ize='col4',.    
-0000a4d0: 2020 2020 2e2e 2e20 2020 2020 636f 6c6f      ...     colo
-0000a4e0: 723d 5b27 2346 4630 3030 3027 2c20 2723  r=['#FF0000', '#
-0000a4f0: 3030 3030 4646 275d 2c20 2023 204f 7074  0000FF'],  # Opt
-0000a500: 696f 6e61 6c0a 2020 2020 2020 2020 2e2e  ional.        ..
-0000a510: 2e20 290a 0a20 2020 2020 2020 202e 2e20  . )..        .. 
-0000a520: 6f75 7470 7574 3a3a 0a20 2020 2020 2020  output::.       
-0000a530: 2020 2020 6874 7470 733a 2f2f 646f 632d      https://doc-
-0000a540: 7363 6174 7465 722d 6368 6172 7432 2e73  scatter-chart2.s
-0000a550: 7472 6561 6d6c 6974 2e61 7070 2f0a 2020  treamlit.app/.  
-0000a560: 2020 2020 2020 2020 2068 6569 6768 743a           height:
-0000a570: 2034 3430 7078 0a0a 2020 2020 2020 2020   440px..        
-0000a580: 2222 220a 0a20 2020 2020 2020 2063 6861  """..        cha
-0000a590: 7274 2c20 6164 645f 726f 7773 5f6d 6574  rt, add_rows_met
-0000a5a0: 6164 6174 6120 3d20 6765 6e65 7261 7465  adata = generate
-0000a5b0: 5f63 6861 7274 280a 2020 2020 2020 2020  _chart(.        
-0000a5c0: 2020 2020 6368 6172 745f 7479 7065 3d43      chart_type=C
-0000a5d0: 6861 7274 5479 7065 2e53 4341 5454 4552  hartType.SCATTER
-0000a5e0: 2c0a 2020 2020 2020 2020 2020 2020 6461  ,.            da
-0000a5f0: 7461 3d64 6174 612c 0a20 2020 2020 2020  ta=data,.       
-0000a600: 2020 2020 2078 5f66 726f 6d5f 7573 6572       x_from_user
-0000a610: 3d78 2c0a 2020 2020 2020 2020 2020 2020  =x,.            
-0000a620: 795f 6672 6f6d 5f75 7365 723d 792c 0a20  y_from_user=y,. 
-0000a630: 2020 2020 2020 2020 2020 2063 6f6c 6f72             color
-0000a640: 5f66 726f 6d5f 7573 6572 3d63 6f6c 6f72  _from_user=color
-0000a650: 2c0a 2020 2020 2020 2020 2020 2020 7369  ,.            si
-0000a660: 7a65 5f66 726f 6d5f 7573 6572 3d73 697a  ze_from_user=siz
-0000a670: 652c 0a20 2020 2020 2020 2020 2020 2077  e,.            w
-0000a680: 6964 7468 3d77 6964 7468 2c0a 2020 2020  idth=width,.    
-0000a690: 2020 2020 2020 2020 6865 6967 6874 3d68          height=h
-0000a6a0: 6569 6768 742c 0a20 2020 2020 2020 2029  eight,.        )
-0000a6b0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0000a6c0: 6361 7374 280a 2020 2020 2020 2020 2020  cast(.          
-0000a6d0: 2020 2244 656c 7461 4765 6e65 7261 746f    "DeltaGenerato
-0000a6e0: 7222 2c0a 2020 2020 2020 2020 2020 2020  r",.            
-0000a6f0: 7365 6c66 2e5f 616c 7461 6972 5f63 6861  self._altair_cha
-0000a700: 7274 280a 2020 2020 2020 2020 2020 2020  rt(.            
-0000a710: 2020 2020 6368 6172 742c 0a20 2020 2020      chart,.     
-0000a720: 2020 2020 2020 2020 2020 2075 7365 5f63             use_c
-0000a730: 6f6e 7461 696e 6572 5f77 6964 7468 3d75  ontainer_width=u
-0000a740: 7365 5f63 6f6e 7461 696e 6572 5f77 6964  se_container_wid
-0000a750: 7468 2c0a 2020 2020 2020 2020 2020 2020  th,.            
-0000a760: 2020 2020 7468 656d 653d 2273 7472 6561      theme="strea
-0000a770: 6d6c 6974 222c 0a20 2020 2020 2020 2020  mlit",.         
-0000a780: 2020 2020 2020 2061 6464 5f72 6f77 735f         add_rows_
-0000a790: 6d65 7461 6461 7461 3d61 6464 5f72 6f77  metadata=add_row
-0000a7a0: 735f 6d65 7461 6461 7461 2c0a 2020 2020  s_metadata,.    
-0000a7b0: 2020 2020 2020 2020 292c 0a20 2020 2020          ),.     
-0000a7c0: 2020 2029 0a0a 2020 2020 406f 7665 726c     )..    @overl
-0000a7d0: 6f61 640a 2020 2020 6465 6620 616c 7461  oad.    def alta
-0000a7e0: 6972 5f63 6861 7274 280a 2020 2020 2020  ir_chart(.      
-0000a7f0: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-0000a800: 616c 7461 6972 5f63 6861 7274 3a20 616c  altair_chart: al
-0000a810: 742e 4368 6172 742c 0a20 2020 2020 2020  t.Chart,.       
-0000a820: 202a 2c0a 2020 2020 2020 2020 7573 655f   *,.        use_
-0000a830: 636f 6e74 6169 6e65 725f 7769 6474 683a  container_width:
-0000a840: 2062 6f6f 6c20 3d20 4661 6c73 652c 0a20   bool = False,. 
-0000a850: 2020 2020 2020 2074 6865 6d65 3a20 4c69         theme: Li
-0000a860: 7465 7261 6c5b 2273 7472 6561 6d6c 6974  teral["streamlit
-0000a870: 225d 207c 204e 6f6e 6520 3d20 2273 7472  "] | None = "str
-0000a880: 6561 6d6c 6974 222c 0a20 2020 2020 2020  eamlit",.       
-0000a890: 206b 6579 3a20 4b65 7920 7c20 4e6f 6e65   key: Key | None
-0000a8a0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-0000a8b0: 206f 6e5f 7365 6c65 6374 3a20 4c69 7465   on_select: Lite
-0000a8c0: 7261 6c5b 2269 676e 6f72 6522 5d2c 2020  ral["ignore"],  
-0000a8d0: 2320 4e6f 2064 6566 6175 6c74 2076 616c  # No default val
-0000a8e0: 7565 2068 6572 6520 746f 206d 616b 6520  ue here to make 
-0000a8f0: 6974 2077 6f72 6b20 7769 7468 206d 7970  it work with myp
-0000a900: 790a 2020 2020 2020 2020 7365 6c65 6374  y.        select
-0000a910: 696f 6e5f 6d6f 6465 3a20 7374 7220 7c20  ion_mode: str | 
-0000a920: 4974 6572 6162 6c65 5b73 7472 5d20 7c20  Iterable[str] | 
-0000a930: 4e6f 6e65 203d 204e 6f6e 652c 0a20 2020  None = None,.   
-0000a940: 2029 202d 3e20 4465 6c74 6147 656e 6572   ) -> DeltaGener
-0000a950: 6174 6f72 3a0a 2020 2020 2020 2020 2e2e  ator:.        ..
-0000a960: 2e0a 0a20 2020 2040 6f76 6572 6c6f 6164  ...    @overload
-0000a970: 0a20 2020 2064 6566 2061 6c74 6169 725f  .    def altair_
-0000a980: 6368 6172 7428 0a20 2020 2020 2020 2073  chart(.        s
-0000a990: 656c 662c 0a20 2020 2020 2020 2061 6c74  elf,.        alt
-0000a9a0: 6169 725f 6368 6172 743a 2061 6c74 2e43  air_chart: alt.C
-0000a9b0: 6861 7274 2c0a 2020 2020 2020 2020 2a2c  hart,.        *,
-0000a9c0: 0a20 2020 2020 2020 2075 7365 5f63 6f6e  .        use_con
-0000a9d0: 7461 696e 6572 5f77 6964 7468 3a20 626f  tainer_width: bo
-0000a9e0: 6f6c 203d 2046 616c 7365 2c0a 2020 2020  ol = False,.    
-0000a9f0: 2020 2020 7468 656d 653a 204c 6974 6572      theme: Liter
-0000aa00: 616c 5b22 7374 7265 616d 6c69 7422 5d20  al["streamlit"] 
-0000aa10: 7c20 4e6f 6e65 203d 2022 7374 7265 616d  | None = "stream
-0000aa20: 6c69 7422 2c0a 2020 2020 2020 2020 6b65  lit",.        ke
-0000aa30: 793a 204b 6579 207c 204e 6f6e 6520 3d20  y: Key | None = 
-0000aa40: 4e6f 6e65 2c0a 2020 2020 2020 2020 6f6e  None,.        on
-0000aa50: 5f73 656c 6563 743a 204c 6974 6572 616c  _select: Literal
-0000aa60: 5b22 7265 7275 6e22 5d20 7c20 5769 6467  ["rerun"] | Widg
-0000aa70: 6574 4361 6c6c 6261 636b 203d 2022 7265  etCallback = "re
-0000aa80: 7275 6e22 2c0a 2020 2020 2020 2020 7365  run",.        se
-0000aa90: 6c65 6374 696f 6e5f 6d6f 6465 3a20 7374  lection_mode: st
-0000aaa0: 7220 7c20 4974 6572 6162 6c65 5b73 7472  r | Iterable[str
-0000aab0: 5d20 7c20 4e6f 6e65 203d 204e 6f6e 652c  ] | None = None,
-0000aac0: 0a20 2020 2029 202d 3e20 5665 6761 4c69  .    ) -> VegaLi
-0000aad0: 7465 5374 6174 653a 0a20 2020 2020 2020  teState:.       
-0000aae0: 202e 2e2e 0a0a 2020 2020 4067 6174 6865   .....    @gathe
-0000aaf0: 725f 6d65 7472 6963 7328 2261 6c74 6169  r_metrics("altai
-0000ab00: 725f 6368 6172 7422 290a 2020 2020 6465  r_chart").    de
-0000ab10: 6620 616c 7461 6972 5f63 6861 7274 280a  f altair_chart(.
-0000ab20: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
-0000ab30: 2020 2020 2020 616c 7461 6972 5f63 6861        altair_cha
-0000ab40: 7274 3a20 616c 742e 4368 6172 742c 0a20  rt: alt.Chart,. 
-0000ab50: 2020 2020 2020 202a 2c0a 2020 2020 2020         *,.      
-0000ab60: 2020 7573 655f 636f 6e74 6169 6e65 725f    use_container_
-0000ab70: 7769 6474 683a 2062 6f6f 6c20 3d20 4661  width: bool = Fa
-0000ab80: 6c73 652c 0a20 2020 2020 2020 2074 6865  lse,.        the
-0000ab90: 6d65 3a20 4c69 7465 7261 6c5b 2273 7472  me: Literal["str
-0000aba0: 6561 6d6c 6974 225d 207c 204e 6f6e 6520  eamlit"] | None 
-0000abb0: 3d20 2273 7472 6561 6d6c 6974 222c 0a20  = "streamlit",. 
-0000abc0: 2020 2020 2020 206b 6579 3a20 4b65 7920         key: Key 
-0000abd0: 7c20 4e6f 6e65 203d 204e 6f6e 652c 0a20  | None = None,. 
-0000abe0: 2020 2020 2020 206f 6e5f 7365 6c65 6374         on_select
-0000abf0: 3a20 4c69 7465 7261 6c5b 2272 6572 756e  : Literal["rerun
-0000ac00: 222c 2022 6967 6e6f 7265 225d 207c 2057  ", "ignore"] | W
-0000ac10: 6964 6765 7443 616c 6c62 6163 6b20 3d20  idgetCallback = 
-0000ac20: 2269 676e 6f72 6522 2c0a 2020 2020 2020  "ignore",.      
-0000ac30: 2020 7365 6c65 6374 696f 6e5f 6d6f 6465    selection_mode
-0000ac40: 3a20 7374 7220 7c20 4974 6572 6162 6c65  : str | Iterable
-0000ac50: 5b73 7472 5d20 7c20 4e6f 6e65 203d 204e  [str] | None = N
-0000ac60: 6f6e 652c 0a20 2020 2029 202d 3e20 4465  one,.    ) -> De
-0000ac70: 6c74 6147 656e 6572 6174 6f72 207c 2056  ltaGenerator | V
-0000ac80: 6567 614c 6974 6553 7461 7465 3a0a 2020  egaLiteState:.  
-0000ac90: 2020 2020 2020 2222 2244 6973 706c 6179        """Display
-0000aca0: 2061 2063 6861 7274 2075 7369 6e67 2074   a chart using t
-0000acb0: 6865 2041 6c74 6169 7220 6c69 6272 6172  he Altair librar
-0000acc0: 792e 0a0a 2020 2020 2020 2020 5061 7261  y...        Para
-0000acd0: 6d65 7465 7273 0a20 2020 2020 2020 202d  meters.        -
-0000ace0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
-0000acf0: 2020 616c 7461 6972 5f63 6861 7274 203a    altair_chart :
-0000ad00: 2061 6c74 6169 722e 4368 6172 740a 2020   altair.Chart.  
-0000ad10: 2020 2020 2020 2020 2020 5468 6520 416c            The Al
-0000ad20: 7461 6972 2063 6861 7274 206f 626a 6563  tair chart objec
-0000ad30: 7420 746f 2064 6973 706c 6179 2e0a 0a20  t to display... 
-0000ad40: 2020 2020 2020 2075 7365 5f63 6f6e 7461         use_conta
-0000ad50: 696e 6572 5f77 6964 7468 203a 2062 6f6f  iner_width : boo
-0000ad60: 6c0a 2020 2020 2020 2020 2020 2020 4966  l.            If
-0000ad70: 2054 7275 652c 2073 6574 2074 6865 2063   True, set the c
-0000ad80: 6861 7274 2077 6964 7468 2074 6f20 7468  hart width to th
-0000ad90: 6520 636f 6c75 6d6e 2077 6964 7468 2e20  e column width. 
-0000ada0: 5468 6973 2074 616b 6573 0a20 2020 2020  This takes.     
-0000adb0: 2020 2020 2020 2070 7265 6365 6465 6e63         precedenc
-0000adc0: 6520 6f76 6572 2041 6c74 6169 7227 7320  e over Altair's 
-0000add0: 6e61 7469 7665 2060 6077 6964 7468 6060  native ``width``
-0000ade0: 2076 616c 7565 2e0a 0a20 2020 2020 2020   value...       
-0000adf0: 2074 6865 6d65 203a 2022 7374 7265 616d   theme : "stream
-0000ae00: 6c69 7422 206f 7220 4e6f 6e65 0a20 2020  lit" or None.   
-0000ae10: 2020 2020 2020 2020 2054 6865 2074 6865           The the
-0000ae20: 6d65 206f 6620 7468 6520 6368 6172 742e  me of the chart.
-0000ae30: 2043 7572 7265 6e74 6c79 2c20 7765 206f   Currently, we o
-0000ae40: 6e6c 7920 7375 7070 6f72 7420 2273 7472  nly support "str
-0000ae50: 6561 6d6c 6974 2220 666f 7220 7468 6520  eamlit" for the 
-0000ae60: 5374 7265 616d 6c69 740a 2020 2020 2020  Streamlit.      
-0000ae70: 2020 2020 2020 6465 6669 6e65 6420 6465        defined de
-0000ae80: 7369 676e 206f 7220 4e6f 6e65 2074 6f20  sign or None to 
-0000ae90: 6661 6c6c 6261 636b 2074 6f20 7468 6520  fallback to the 
-0000aea0: 6465 6661 756c 7420 6265 6861 7669 6f72  default behavior
-0000aeb0: 206f 6620 7468 6520 6c69 6272 6172 792e   of the library.
-0000aec0: 0a0a 2020 2020 2020 2020 6b65 7920 3a20  ..        key : 
-0000aed0: 7374 720a 2020 2020 2020 2020 2020 2020  str.            
-0000aee0: 416e 206f 7074 696f 6e61 6c20 7374 7269  An optional stri
-0000aef0: 6e67 2074 6f20 7573 6520 6173 2074 6865  ng to use as the
-0000af00: 2075 6e69 7175 6520 6b65 7920 666f 7220   unique key for 
-0000af10: 7468 6973 2065 6c65 6d65 6e74 2077 6865  this element whe
-0000af20: 6e20 7573 6564 2069 6e20 636f 6d62 696e  n used in combin
-0000af30: 6174 696f 6e0a 2020 2020 2020 2020 2020  ation.          
-0000af40: 2020 7769 7468 2060 6060 6f6e 5f73 656c    with ```on_sel
-0000af50: 6563 7460 6060 2e20 4966 2074 6869 7320  ect```. If this 
-0000af60: 6973 206f 6d69 7474 6564 2c20 6120 6b65  is omitted, a ke
-0000af70: 7920 7769 6c6c 2062 6520 6765 6e65 7261  y will be genera
-0000af80: 7465 6420 666f 7220 7468 6520 7769 6467  ted for the widg
-0000af90: 6574 2062 6173 6564 0a20 2020 2020 2020  et based.       
-0000afa0: 2020 2020 206f 6e20 6974 7320 636f 6e74       on its cont
-0000afb0: 656e 742e 204d 756c 7469 706c 6520 7769  ent. Multiple wi
-0000afc0: 6467 6574 7320 6f66 2074 6865 2073 616d  dgets of the sam
-0000afd0: 6520 7479 7065 206d 6179 206e 6f74 2073  e type may not s
-0000afe0: 6861 7265 2074 6865 2073 616d 6520 6b65  hare the same ke
-0000aff0: 792e 0a0a 2020 2020 2020 2020 6f6e 5f73  y...        on_s
-0000b000: 656c 6563 7420 3a20 2269 676e 6f72 6522  elect : "ignore"
-0000b010: 206f 7220 2272 6572 756e 2220 6f72 2063   or "rerun" or c
-0000b020: 616c 6c61 626c 650a 2020 2020 2020 2020  allable.        
-0000b030: 2020 2020 436f 6e74 726f 6c73 2074 6865      Controls the
-0000b040: 2062 6568 6176 696f 7220 696e 2072 6573   behavior in res
-0000b050: 706f 6e73 6520 746f 2073 656c 6563 7469  ponse to selecti
-0000b060: 6f6e 2065 7665 6e74 7320 6f6e 2074 6865  on events on the
-0000b070: 2063 6861 7274 732e 2043 616e 2062 6520   charts. Can be 
-0000b080: 6f6e 6520 6f66 3a0a 2020 2020 2020 2020  one of:.        
-0000b090: 2020 2020 2d20 2269 676e 6f72 6522 2028      - "ignore" (
-0000b0a0: 6465 6661 756c 7429 3a20 5374 7265 616d  default): Stream
-0000b0b0: 6c69 7420 7769 6c6c 206e 6f74 2072 6561  lit will not rea
-0000b0c0: 6374 2074 6f20 616e 7920 7365 6c65 6374  ct to any select
-0000b0d0: 696f 6e20 6576 656e 7473 2069 6e20 7468  ion events in th
-0000b0e0: 6520 6368 6172 742e 0a20 2020 2020 2020  e chart..       
-0000b0f0: 2020 2020 202d 2022 7265 7275 6e3a 2053       - "rerun: S
-0000b100: 7472 6561 6d6c 6974 2077 696c 6c20 7265  treamlit will re
-0000b110: 7275 6e20 7468 6520 6170 7020 7768 656e  run the app when
-0000b120: 2074 6865 2075 7365 7220 7365 6c65 6374   the user select
-0000b130: 7320 6461 7461 2069 6e20 7468 6520 6368  s data in the ch
-0000b140: 6172 742e 2049 6e20 7468 6973 2063 6173  art. In this cas
-0000b150: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-0000b160: 2060 6060 7374 2e61 6c74 6169 725f 6368   ```st.altair_ch
-0000b170: 6172 7460 6060 2077 696c 6c20 7265 7475  art``` will retu
-0000b180: 726e 2074 6865 2073 656c 6563 7469 6f6e  rn the selection
-0000b190: 2064 6174 6120 6173 2061 2064 6963 7469   data as a dicti
-0000b1a0: 6f6e 6172 792e 0a20 2020 2020 2020 2020  onary..         
-0000b1b0: 2020 202d 2063 616c 6c61 626c 653a 2049     - callable: I
-0000b1c0: 6620 6120 6361 6c6c 6162 6c65 2069 7320  f a callable is 
-0000b1d0: 7072 6f76 6964 6564 2c20 5374 7265 616d  provided, Stream
-0000b1e0: 6c69 7420 7769 6c6c 2072 6572 756e 2061  lit will rerun a
-0000b1f0: 6e64 2065 7865 6375 7465 2074 6865 2063  nd execute the c
-0000b200: 616c 6c61 626c 6520 6173 2061 0a20 2020  allable as a.   
-0000b210: 2020 2020 2020 2020 2020 2063 616c 6c62             callb
-0000b220: 6163 6b20 6675 6e63 7469 6f6e 2062 6566  ack function bef
-0000b230: 6f72 6520 7468 6520 7265 7374 206f 6620  ore the rest of 
-0000b240: 7468 6520 6170 702e 2054 6865 2073 656c  the app. The sel
-0000b250: 6563 7469 6f6e 2064 6174 6120 6361 6e20  ection data can 
-0000b260: 6265 2072 6574 7269 6576 6564 2074 6872  be retrieved thr
-0000b270: 6f75 6768 0a20 2020 2020 2020 2020 2020  ough.           
-0000b280: 2020 2073 6573 7369 6f6e 2073 7461 7465     session state
-0000b290: 2062 7920 7365 7474 696e 6720 7468 6520   by setting the 
-0000b2a0: 6b65 7920 7061 7261 6d65 7465 722e 0a0a  key parameter...
-0000b2b0: 2020 2020 2020 2020 4578 616d 706c 650a          Example.
-0000b2c0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0a          -------.
-0000b2d0: 0a20 2020 2020 2020 203e 3e3e 2069 6d70  .        >>> imp
-0000b2e0: 6f72 7420 7374 7265 616d 6c69 7420 6173  ort streamlit as
-0000b2f0: 2073 740a 2020 2020 2020 2020 3e3e 3e20   st.        >>> 
-0000b300: 696d 706f 7274 2070 616e 6461 7320 6173  import pandas as
-0000b310: 2070 640a 2020 2020 2020 2020 3e3e 3e20   pd.        >>> 
-0000b320: 696d 706f 7274 206e 756d 7079 2061 7320  import numpy as 
-0000b330: 6e70 0a20 2020 2020 2020 203e 3e3e 2069  np.        >>> i
-0000b340: 6d70 6f72 7420 616c 7461 6972 2061 7320  mport altair as 
-0000b350: 616c 740a 2020 2020 2020 2020 3e3e 3e0a  alt.        >>>.
-0000b360: 2020 2020 2020 2020 3e3e 3e20 6368 6172          >>> char
-0000b370: 745f 6461 7461 203d 2070 642e 4461 7461  t_data = pd.Data
-0000b380: 4672 616d 6528 6e70 2e72 616e 646f 6d2e  Frame(np.random.
-0000b390: 7261 6e64 6e28 3230 2c20 3329 2c20 636f  randn(20, 3), co
-0000b3a0: 6c75 6d6e 733d 5b22 6122 2c20 2262 222c  lumns=["a", "b",
-0000b3b0: 2022 6322 5d29 0a20 2020 2020 2020 203e   "c"]).        >
-0000b3c0: 3e3e 0a20 2020 2020 2020 203e 3e3e 2063  >>.        >>> c
-0000b3d0: 203d 2028 0a20 2020 2020 2020 202e 2e2e   = (.        ...
-0000b3e0: 2020 2020 616c 742e 4368 6172 7428 6368      alt.Chart(ch
-0000b3f0: 6172 745f 6461 7461 290a 2020 2020 2020  art_data).      
-0000b400: 2020 2e2e 2e20 2020 202e 6d61 726b 5f63    ...    .mark_c
-0000b410: 6972 636c 6528 290a 2020 2020 2020 2020  ircle().        
-0000b420: 2e2e 2e20 2020 202e 656e 636f 6465 2878  ...    .encode(x
-0000b430: 3d22 6122 2c20 793d 2262 222c 2073 697a  ="a", y="b", siz
-0000b440: 653d 2263 222c 2063 6f6c 6f72 3d22 6322  e="c", color="c"
-0000b450: 2c20 746f 6f6c 7469 703d 5b22 6122 2c20  , tooltip=["a", 
-0000b460: 2262 222c 2022 6322 5d29 0a20 2020 2020  "b", "c"]).     
-0000b470: 2020 202e 2e2e 2029 0a20 2020 2020 2020     ... ).       
-0000b480: 203e 3e3e 0a20 2020 2020 2020 203e 3e3e   >>>.        >>>
-0000b490: 2073 742e 616c 7461 6972 5f63 6861 7274   st.altair_chart
-0000b4a0: 2863 2c20 7573 655f 636f 6e74 6169 6e65  (c, use_containe
-0000b4b0: 725f 7769 6474 683d 5472 7565 290a 0a20  r_width=True).. 
-0000b4c0: 2020 2020 2020 202e 2e20 6f75 7470 7574         .. output
-0000b4d0: 3a3a 0a20 2020 2020 2020 2020 2020 6874  ::.           ht
-0000b4e0: 7470 733a 2f2f 646f 632d 7665 6761 2d6c  tps://doc-vega-l
-0000b4f0: 6974 652d 6368 6172 742e 7374 7265 616d  ite-chart.stream
-0000b500: 6c69 742e 6170 702f 0a20 2020 2020 2020  lit.app/.       
-0000b510: 2020 2020 6865 6967 6874 3a20 3330 3070      height: 300p
-0000b520: 780a 0a20 2020 2020 2020 2045 7861 6d70  x..        Examp
-0000b530: 6c65 7320 6f66 2041 6c74 6169 7220 6368  les of Altair ch
-0000b540: 6172 7473 2063 616e 2062 6520 666f 756e  arts can be foun
-0000b550: 6420 6174 0a20 2020 2020 2020 2068 7474  d at.        htt
-0000b560: 7073 3a2f 2f61 6c74 6169 722d 7669 7a2e  ps://altair-viz.
-0000b570: 6769 7468 7562 2e69 6f2f 6761 6c6c 6572  github.io/galler
-0000b580: 792f 2e0a 0a20 2020 2020 2020 2022 2222  y/...        """
-0000b590: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0000b5a0: 7365 6c66 2e5f 616c 7461 6972 5f63 6861  self._altair_cha
-0000b5b0: 7274 280a 2020 2020 2020 2020 2020 2020  rt(.            
-0000b5c0: 616c 7461 6972 5f63 6861 7274 3d61 6c74  altair_chart=alt
-0000b5d0: 6169 725f 6368 6172 742c 0a20 2020 2020  air_chart,.     
-0000b5e0: 2020 2020 2020 2075 7365 5f63 6f6e 7461         use_conta
-0000b5f0: 696e 6572 5f77 6964 7468 3d75 7365 5f63  iner_width=use_c
-0000b600: 6f6e 7461 696e 6572 5f77 6964 7468 2c0a  ontainer_width,.
-0000b610: 2020 2020 2020 2020 2020 2020 7468 656d              them
-0000b620: 653d 7468 656d 652c 0a20 2020 2020 2020  e=theme,.       
-0000b630: 2020 2020 206b 6579 3d6b 6579 2c0a 2020       key=key,.  
-0000b640: 2020 2020 2020 2020 2020 6f6e 5f73 656c            on_sel
-0000b650: 6563 743d 6f6e 5f73 656c 6563 742c 0a20  ect=on_select,. 
-0000b660: 2020 2020 2020 2020 2020 2073 656c 6563             selec
-0000b670: 7469 6f6e 5f6d 6f64 653d 7365 6c65 6374  tion_mode=select
-0000b680: 696f 6e5f 6d6f 6465 2c0a 2020 2020 2020  ion_mode,.      
-0000b690: 2020 290a 0a20 2020 2040 6f76 6572 6c6f    )..    @overlo
-0000b6a0: 6164 0a20 2020 2064 6566 2076 6567 615f  ad.    def vega_
-0000b6b0: 6c69 7465 5f63 6861 7274 280a 2020 2020  lite_chart(.    
-0000b6c0: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
-0000b6d0: 2020 6461 7461 3a20 4461 7461 203d 204e    data: Data = N
-0000b6e0: 6f6e 652c 0a20 2020 2020 2020 2073 7065  one,.        spe
-0000b6f0: 633a 2056 6567 614c 6974 6553 7065 6320  c: VegaLiteSpec 
-0000b700: 7c20 4e6f 6e65 203d 204e 6f6e 652c 0a20  | None = None,. 
-0000b710: 2020 2020 2020 202a 2c0a 2020 2020 2020         *,.      
-0000b720: 2020 7573 655f 636f 6e74 6169 6e65 725f    use_container_
-0000b730: 7769 6474 683a 2062 6f6f 6c20 3d20 4661  width: bool = Fa
-0000b740: 6c73 652c 0a20 2020 2020 2020 2074 6865  lse,.        the
-0000b750: 6d65 3a20 4c69 7465 7261 6c5b 2273 7472  me: Literal["str
-0000b760: 6561 6d6c 6974 225d 207c 204e 6f6e 6520  eamlit"] | None 
-0000b770: 3d20 2273 7472 6561 6d6c 6974 222c 0a20  = "streamlit",. 
-0000b780: 2020 2020 2020 206b 6579 3a20 4b65 7920         key: Key 
-0000b790: 7c20 4e6f 6e65 203d 204e 6f6e 652c 0a20  | None = None,. 
-0000b7a0: 2020 2020 2020 206f 6e5f 7365 6c65 6374         on_select
-0000b7b0: 3a20 4c69 7465 7261 6c5b 2269 676e 6f72  : Literal["ignor
-0000b7c0: 6522 5d2c 2020 2320 4e6f 2064 6566 6175  e"],  # No defau
-0000b7d0: 6c74 2076 616c 7565 2068 6572 6520 746f  lt value here to
-0000b7e0: 206d 616b 6520 6974 2077 6f72 6b20 7769   make it work wi
-0000b7f0: 7468 206d 7970 790a 2020 2020 2020 2020  th mypy.        
-0000b800: 7365 6c65 6374 696f 6e5f 6d6f 6465 3a20  selection_mode: 
-0000b810: 7374 7220 7c20 4974 6572 6162 6c65 5b73  str | Iterable[s
-0000b820: 7472 5d20 7c20 4e6f 6e65 203d 204e 6f6e  tr] | None = Non
-0000b830: 652c 0a20 2020 2020 2020 202a 2a6b 7761  e,.        **kwa
-0000b840: 7267 733a 2041 6e79 2c0a 2020 2020 2920  rgs: Any,.    ) 
-0000b850: 2d3e 2044 656c 7461 4765 6e65 7261 746f  -> DeltaGenerato
-0000b860: 723a 0a20 2020 2020 2020 202e 2e2e 0a0a  r:.        .....
-0000b870: 2020 2020 406f 7665 726c 6f61 640a 2020      @overload.  
-0000b880: 2020 6465 6620 7665 6761 5f6c 6974 655f    def vega_lite_
-0000b890: 6368 6172 7428 0a20 2020 2020 2020 2073  chart(.        s
-0000b8a0: 656c 662c 0a20 2020 2020 2020 2064 6174  elf,.        dat
-0000b8b0: 613a 2044 6174 6120 3d20 4e6f 6e65 2c0a  a: Data = None,.
-0000b8c0: 2020 2020 2020 2020 7370 6563 3a20 5665          spec: Ve
-0000b8d0: 6761 4c69 7465 5370 6563 207c 204e 6f6e  gaLiteSpec | Non
-0000b8e0: 6520 3d20 4e6f 6e65 2c0a 2020 2020 2020  e = None,.      
-0000b8f0: 2020 2a2c 0a20 2020 2020 2020 2075 7365    *,.        use
-0000b900: 5f63 6f6e 7461 696e 6572 5f77 6964 7468  _container_width
-0000b910: 3a20 626f 6f6c 203d 2046 616c 7365 2c0a  : bool = False,.
-0000b920: 2020 2020 2020 2020 7468 656d 653a 204c          theme: L
-0000b930: 6974 6572 616c 5b22 7374 7265 616d 6c69  iteral["streamli
-0000b940: 7422 5d20 7c20 4e6f 6e65 203d 2022 7374  t"] | None = "st
-0000b950: 7265 616d 6c69 7422 2c0a 2020 2020 2020  reamlit",.      
-0000b960: 2020 6b65 793a 204b 6579 207c 204e 6f6e    key: Key | Non
-0000b970: 6520 3d20 4e6f 6e65 2c0a 2020 2020 2020  e = None,.      
-0000b980: 2020 6f6e 5f73 656c 6563 743a 204c 6974    on_select: Lit
-0000b990: 6572 616c 5b22 7265 7275 6e22 5d20 7c20  eral["rerun"] | 
-0000b9a0: 5769 6467 6574 4361 6c6c 6261 636b 203d  WidgetCallback =
-0000b9b0: 2022 7265 7275 6e22 2c0a 2020 2020 2020   "rerun",.      
-0000b9c0: 2020 7365 6c65 6374 696f 6e5f 6d6f 6465    selection_mode
-0000b9d0: 3a20 7374 7220 7c20 4974 6572 6162 6c65  : str | Iterable
-0000b9e0: 5b73 7472 5d20 7c20 4e6f 6e65 203d 204e  [str] | None = N
-0000b9f0: 6f6e 652c 0a20 2020 2020 2020 202a 2a6b  one,.        **k
-0000ba00: 7761 7267 733a 2041 6e79 2c0a 2020 2020  wargs: Any,.    
-0000ba10: 2920 2d3e 2056 6567 614c 6974 6553 7461  ) -> VegaLiteSta
-0000ba20: 7465 3a0a 2020 2020 2020 2020 2e2e 2e0a  te:.        ....
-0000ba30: 0a20 2020 2040 6761 7468 6572 5f6d 6574  .    @gather_met
-0000ba40: 7269 6373 2822 7665 6761 5f6c 6974 655f  rics("vega_lite_
-0000ba50: 6368 6172 7422 290a 2020 2020 6465 6620  chart").    def 
-0000ba60: 7665 6761 5f6c 6974 655f 6368 6172 7428  vega_lite_chart(
-0000ba70: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
-0000ba80: 2020 2020 2020 2064 6174 613a 2044 6174         data: Dat
-0000ba90: 6120 3d20 4e6f 6e65 2c0a 2020 2020 2020  a = None,.      
-0000baa0: 2020 7370 6563 3a20 5665 6761 4c69 7465    spec: VegaLite
-0000bab0: 5370 6563 207c 204e 6f6e 6520 3d20 4e6f  Spec | None = No
-0000bac0: 6e65 2c0a 2020 2020 2020 2020 2a2c 0a20  ne,.        *,. 
-0000bad0: 2020 2020 2020 2075 7365 5f63 6f6e 7461         use_conta
-0000bae0: 696e 6572 5f77 6964 7468 3a20 626f 6f6c  iner_width: bool
-0000baf0: 203d 2046 616c 7365 2c0a 2020 2020 2020   = False,.      
-0000bb00: 2020 7468 656d 653a 204c 6974 6572 616c    theme: Literal
-0000bb10: 5b22 7374 7265 616d 6c69 7422 5d20 7c20  ["streamlit"] | 
-0000bb20: 4e6f 6e65 203d 2022 7374 7265 616d 6c69  None = "streamli
-0000bb30: 7422 2c0a 2020 2020 2020 2020 6b65 793a  t",.        key:
-0000bb40: 204b 6579 207c 204e 6f6e 6520 3d20 4e6f   Key | None = No
-0000bb50: 6e65 2c0a 2020 2020 2020 2020 6f6e 5f73  ne,.        on_s
-0000bb60: 656c 6563 743a 204c 6974 6572 616c 5b22  elect: Literal["
-0000bb70: 7265 7275 6e22 2c20 2269 676e 6f72 6522  rerun", "ignore"
-0000bb80: 5d20 7c20 5769 6467 6574 4361 6c6c 6261  ] | WidgetCallba
-0000bb90: 636b 203d 2022 6967 6e6f 7265 222c 0a20  ck = "ignore",. 
-0000bba0: 2020 2020 2020 2073 656c 6563 7469 6f6e         selection
-0000bbb0: 5f6d 6f64 653a 2073 7472 207c 2049 7465  _mode: str | Ite
-0000bbc0: 7261 626c 655b 7374 725d 207c 204e 6f6e  rable[str] | Non
-0000bbd0: 6520 3d20 4e6f 6e65 2c0a 2020 2020 2020  e = None,.      
-0000bbe0: 2020 2a2a 6b77 6172 6773 3a20 416e 792c    **kwargs: Any,
-0000bbf0: 0a20 2020 2029 202d 3e20 4465 6c74 6147  .    ) -> DeltaG
-0000bc00: 656e 6572 6174 6f72 207c 2056 6567 614c  enerator | VegaL
-0000bc10: 6974 6553 7461 7465 3a0a 2020 2020 2020  iteState:.      
-0000bc20: 2020 2222 2244 6973 706c 6179 2061 2063    """Display a c
-0000bc30: 6861 7274 2075 7369 6e67 2074 6865 2056  hart using the V
-0000bc40: 6567 612d 4c69 7465 206c 6962 7261 7279  ega-Lite library
-0000bc50: 2e0a 0a20 2020 2020 2020 2050 6172 616d  ...        Param
-0000bc60: 6574 6572 730a 2020 2020 2020 2020 2d2d  eters.        --
-0000bc70: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
-0000bc80: 2064 6174 6120 3a20 7061 6e64 6173 2e44   data : pandas.D
-0000bc90: 6174 6146 7261 6d65 2c20 7061 6e64 6173  ataFrame, pandas
-0000bca0: 2e53 7479 6c65 722c 2070 7961 7272 6f77  .Styler, pyarrow
-0000bcb0: 2e54 6162 6c65 2c20 6e75 6d70 792e 6e64  .Table, numpy.nd
-0000bcc0: 6172 7261 792c 2049 7465 7261 626c 652c  array, Iterable,
-0000bcd0: 2064 6963 742c 206f 7220 4e6f 6e65 0a20   dict, or None. 
-0000bce0: 2020 2020 2020 2020 2020 2045 6974 6865             Eithe
-0000bcf0: 7220 7468 6520 6461 7461 2074 6f20 6265  r the data to be
-0000bd00: 2070 6c6f 7474 6564 206f 7220 6120 5665   plotted or a Ve
-0000bd10: 6761 2d4c 6974 6520 7370 6563 2063 6f6e  ga-Lite spec con
-0000bd20: 7461 696e 696e 6720 7468 650a 2020 2020  taining the.    
-0000bd30: 2020 2020 2020 2020 6461 7461 2028 7768          data (wh
-0000bd40: 6963 6820 6d6f 7265 2063 6c6f 7365 6c79  ich more closely
-0000bd50: 2066 6f6c 6c6f 7773 2074 6865 2056 6567   follows the Veg
-0000bd60: 612d 4c69 7465 2041 5049 292e 0a0a 2020  a-Lite API)...  
-0000bd70: 2020 2020 2020 7370 6563 203a 2064 6963        spec : dic
-0000bd80: 7420 6f72 204e 6f6e 650a 2020 2020 2020  t or None.      
-0000bd90: 2020 2020 2020 5468 6520 5665 6761 2d4c        The Vega-L
-0000bda0: 6974 6520 7370 6563 2066 6f72 2074 6865  ite spec for the
-0000bdb0: 2063 6861 7274 2e20 4966 2074 6865 2073   chart. If the s
-0000bdc0: 7065 6320 7761 7320 616c 7265 6164 7920  pec was already 
-0000bdd0: 7061 7373 6564 2069 6e0a 2020 2020 2020  passed in.      
-0000bde0: 2020 2020 2020 7468 6520 7072 6576 696f        the previo
-0000bdf0: 7573 2061 7267 756d 656e 742c 2074 6869  us argument, thi
-0000be00: 7320 6d75 7374 2062 6520 7365 7420 746f  s must be set to
-0000be10: 204e 6f6e 652e 2053 6565 0a20 2020 2020   None. See.     
-0000be20: 2020 2020 2020 2068 7474 7073 3a2f 2f76         https://v
-0000be30: 6567 612e 6769 7468 7562 2e69 6f2f 7665  ega.github.io/ve
-0000be40: 6761 2d6c 6974 652f 646f 6373 2f20 666f  ga-lite/docs/ fo
-0000be50: 7220 6d6f 7265 2069 6e66 6f2e 0a0a 2020  r more info...  
-0000be60: 2020 2020 2020 7573 655f 636f 6e74 6169        use_contai
-0000be70: 6e65 725f 7769 6474 6820 3a20 626f 6f6c  ner_width : bool
-0000be80: 0a20 2020 2020 2020 2020 2020 2049 6620  .            If 
-0000be90: 5472 7565 2c20 7365 7420 7468 6520 6368  True, set the ch
-0000bea0: 6172 7420 7769 6474 6820 746f 2074 6865  art width to the
-0000beb0: 2063 6f6c 756d 6e20 7769 6474 682e 2054   column width. T
-0000bec0: 6869 7320 7461 6b65 730a 2020 2020 2020  his takes.      
-0000bed0: 2020 2020 2020 7072 6563 6564 656e 6365        precedence
-0000bee0: 206f 7665 7220 5665 6761 2d4c 6974 6527   over Vega-Lite'
-0000bef0: 7320 6e61 7469 7665 2060 7769 6474 6860  s native `width`
-0000bf00: 2076 616c 7565 2e0a 0a20 2020 2020 2020   value...       
-0000bf10: 2074 6865 6d65 203a 2022 7374 7265 616d   theme : "stream
-0000bf20: 6c69 7422 206f 7220 4e6f 6e65 0a20 2020  lit" or None.   
-0000bf30: 2020 2020 2020 2020 2054 6865 2074 6865           The the
-0000bf40: 6d65 206f 6620 7468 6520 6368 6172 742e  me of the chart.
-0000bf50: 2043 7572 7265 6e74 6c79 2c20 7765 206f   Currently, we o
-0000bf60: 6e6c 7920 7375 7070 6f72 7420 2273 7472  nly support "str
-0000bf70: 6561 6d6c 6974 2220 666f 7220 7468 6520  eamlit" for the 
-0000bf80: 5374 7265 616d 6c69 740a 2020 2020 2020  Streamlit.      
-0000bf90: 2020 2020 2020 6465 6669 6e65 6420 6465        defined de
-0000bfa0: 7369 676e 206f 7220 4e6f 6e65 2074 6f20  sign or None to 
-0000bfb0: 6661 6c6c 6261 636b 2074 6f20 7468 6520  fallback to the 
-0000bfc0: 6465 6661 756c 7420 6265 6861 7669 6f72  default behavior
-0000bfd0: 206f 6620 7468 6520 6c69 6272 6172 792e   of the library.
-0000bfe0: 0a0a 2020 2020 2020 2020 6b65 7920 3a20  ..        key : 
-0000bff0: 7374 720a 2020 2020 2020 2020 2020 2020  str.            
-0000c000: 416e 206f 7074 696f 6e61 6c20 7374 7269  An optional stri
-0000c010: 6e67 2074 6f20 7573 6520 6173 2074 6865  ng to use as the
-0000c020: 2075 6e69 7175 6520 6b65 7920 666f 7220   unique key for 
-0000c030: 7468 6973 2065 6c65 6d65 6e74 2077 6865  this element whe
-0000c040: 6e20 7573 6564 2069 6e20 636f 6d62 696e  n used in combin
-0000c050: 6174 696f 6e0a 2020 2020 2020 2020 2020  ation.          
-0000c060: 2020 7769 7468 2060 6060 6f6e 5f73 656c    with ```on_sel
-0000c070: 6563 7460 6060 2e20 4966 2074 6869 7320  ect```. If this 
-0000c080: 6973 206f 6d69 7474 6564 2c20 6120 6b65  is omitted, a ke
-0000c090: 7920 7769 6c6c 2062 6520 6765 6e65 7261  y will be genera
-0000c0a0: 7465 6420 666f 7220 7468 6520 7769 6467  ted for the widg
-0000c0b0: 6574 2062 6173 6564 0a20 2020 2020 2020  et based.       
-0000c0c0: 2020 2020 206f 6e20 6974 7320 636f 6e74       on its cont
-0000c0d0: 656e 742e 204d 756c 7469 706c 6520 7769  ent. Multiple wi
-0000c0e0: 6467 6574 7320 6f66 2074 6865 2073 616d  dgets of the sam
-0000c0f0: 6520 7479 7065 206d 6179 206e 6f74 2073  e type may not s
-0000c100: 6861 7265 2074 6865 2073 616d 6520 6b65  hare the same ke
-0000c110: 792e 0a0a 2020 2020 2020 2020 6f6e 5f73  y...        on_s
-0000c120: 656c 6563 7420 3a20 2269 676e 6f72 6522  elect : "ignore"
-0000c130: 206f 7220 2272 6572 756e 2220 6f72 2063   or "rerun" or c
-0000c140: 616c 6c61 626c 650a 2020 2020 2020 2020  allable.        
-0000c150: 2020 2020 436f 6e74 726f 6c73 2074 6865      Controls the
-0000c160: 2062 6568 6176 696f 7220 696e 2072 6573   behavior in res
-0000c170: 706f 6e73 6520 746f 2073 656c 6563 7469  ponse to selecti
-0000c180: 6f6e 2065 7665 6e74 7320 6f6e 2074 6865  on events on the
-0000c190: 2063 6861 7274 732e 2043 616e 2062 6520   charts. Can be 
-0000c1a0: 6f6e 6520 6f66 3a0a 2020 2020 2020 2020  one of:.        
-0000c1b0: 2020 2020 2d20 2269 676e 6f72 6522 2028      - "ignore" (
-0000c1c0: 6465 6661 756c 7429 3a20 5374 7265 616d  default): Stream
-0000c1d0: 6c69 7420 7769 6c6c 206e 6f74 2072 6561  lit will not rea
-0000c1e0: 6374 2074 6f20 616e 7920 7365 6c65 6374  ct to any select
-0000c1f0: 696f 6e20 6576 656e 7473 2069 6e20 7468  ion events in th
-0000c200: 6520 6368 6172 742e 0a20 2020 2020 2020  e chart..       
-0000c210: 2020 2020 202d 2022 7265 7275 6e3a 2053       - "rerun: S
-0000c220: 7472 6561 6d6c 6974 2077 696c 6c20 7265  treamlit will re
-0000c230: 7275 6e20 7468 6520 6170 7020 7768 656e  run the app when
-0000c240: 2074 6865 2075 7365 7220 7365 6c65 6374   the user select
-0000c250: 7320 6461 7461 2069 6e20 7468 6520 6368  s data in the ch
-0000c260: 6172 742e 2049 6e20 7468 6973 2063 6173  art. In this cas
-0000c270: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-0000c280: 2060 6060 7374 2e76 6567 615f 6c69 7465   ```st.vega_lite
-0000c290: 5f63 6861 7274 6060 6020 7769 6c6c 2072  _chart``` will r
-0000c2a0: 6574 7572 6e20 7468 6520 7365 6c65 6374  eturn the select
-0000c2b0: 696f 6e20 6461 7461 2061 7320 6120 6469  ion data as a di
-0000c2c0: 6374 696f 6e61 7279 2e0a 2020 2020 2020  ctionary..      
-0000c2d0: 2020 2020 2020 2d20 6361 6c6c 6162 6c65        - callable
-0000c2e0: 3a20 4966 2061 2063 616c 6c61 626c 6520  : If a callable 
-0000c2f0: 6973 2070 726f 7669 6465 642c 2053 7472  is provided, Str
-0000c300: 6561 6d6c 6974 2077 696c 6c20 7265 7275  eamlit will reru
-0000c310: 6e20 616e 6420 6578 6563 7574 6520 7468  n and execute th
-0000c320: 6520 6361 6c6c 6162 6c65 2061 7320 610a  e callable as a.
-0000c330: 2020 2020 2020 2020 2020 2020 2020 6361                ca
-0000c340: 6c6c 6261 636b 2066 756e 6374 696f 6e20  llback function 
-0000c350: 6265 666f 7265 2074 6865 2072 6573 7420  before the rest 
-0000c360: 6f66 2074 6865 2061 7070 2e20 5468 6520  of the app. The 
-0000c370: 7365 6c65 6374 696f 6e20 6461 7461 2063  selection data c
-0000c380: 616e 2062 6520 7265 7472 6965 7665 6420  an be retrieved 
-0000c390: 7468 726f 7567 680a 2020 2020 2020 2020  through.        
-0000c3a0: 2020 2020 2020 7365 7373 696f 6e20 7374        session st
-0000c3b0: 6174 6520 6279 2073 6574 7469 6e67 2074  ate by setting t
-0000c3c0: 6865 206b 6579 2070 6172 616d 6574 6572  he key parameter
-0000c3d0: 2e0a 0a20 2020 2020 2020 202a 2a6b 7761  ...        **kwa
-0000c3e0: 7267 7320 3a20 616e 790a 2020 2020 2020  rgs : any.      
-0000c3f0: 2020 2020 2020 5361 6d65 2061 7320 7370        Same as sp
-0000c400: 6563 2c20 6275 7420 6173 206b 6579 776f  ec, but as keywo
-0000c410: 7264 732e 0a0a 2020 2020 2020 2020 4578  rds...        Ex
-0000c420: 616d 706c 650a 2020 2020 2020 2020 2d2d  ample.        --
-0000c430: 2d2d 2d2d 2d0a 2020 2020 2020 2020 3e3e  -----.        >>
-0000c440: 3e20 696d 706f 7274 2073 7472 6561 6d6c  > import streaml
-0000c450: 6974 2061 7320 7374 0a20 2020 2020 2020  it as st.       
-0000c460: 203e 3e3e 2069 6d70 6f72 7420 7061 6e64   >>> import pand
-0000c470: 6173 2061 7320 7064 0a20 2020 2020 2020  as as pd.       
-0000c480: 203e 3e3e 2069 6d70 6f72 7420 6e75 6d70   >>> import nump
-0000c490: 7920 6173 206e 700a 2020 2020 2020 2020  y as np.        
-0000c4a0: 3e3e 3e0a 2020 2020 2020 2020 3e3e 3e20  >>>.        >>> 
-0000c4b0: 6368 6172 745f 6461 7461 203d 2070 642e  chart_data = pd.
-0000c4c0: 4461 7461 4672 616d 6528 6e70 2e72 616e  DataFrame(np.ran
-0000c4d0: 646f 6d2e 7261 6e64 6e28 3230 302c 2033  dom.randn(200, 3
-0000c4e0: 292c 2063 6f6c 756d 6e73 3d5b 2261 222c  ), columns=["a",
-0000c4f0: 2022 6222 2c20 2263 225d 290a 2020 2020   "b", "c"]).    
-0000c500: 2020 2020 3e3e 3e0a 2020 2020 2020 2020      >>>.        
-0000c510: 3e3e 3e20 7374 2e76 6567 615f 6c69 7465  >>> st.vega_lite
-0000c520: 5f63 6861 7274 280a 2020 2020 2020 2020  _chart(.        
-0000c530: 2e2e 2e20 2020 2063 6861 7274 5f64 6174  ...    chart_dat
-0000c540: 612c 0a20 2020 2020 2020 202e 2e2e 2020  a,.        ...  
-0000c550: 2020 7b0a 2020 2020 2020 2020 2e2e 2e20    {.        ... 
-0000c560: 2020 2020 2020 2022 6d61 726b 223a 207b         "mark": {
-0000c570: 2274 7970 6522 3a20 2263 6972 636c 6522  "type": "circle"
-0000c580: 2c20 2274 6f6f 6c74 6970 223a 2054 7275  , "tooltip": Tru
-0000c590: 657d 2c0a 2020 2020 2020 2020 2e2e 2e20  e},.        ... 
-0000c5a0: 2020 2020 2020 2022 656e 636f 6469 6e67         "encoding
-0000c5b0: 223a 207b 0a20 2020 2020 2020 202e 2e2e  ": {.        ...
-0000c5c0: 2020 2020 2020 2020 2020 2020 2278 223a              "x":
-0000c5d0: 207b 2266 6965 6c64 223a 2022 6122 2c20   {"field": "a", 
-0000c5e0: 2274 7970 6522 3a20 2271 7561 6e74 6974  "type": "quantit
-0000c5f0: 6174 6976 6522 7d2c 0a20 2020 2020 2020  ative"},.       
-0000c600: 202e 2e2e 2020 2020 2020 2020 2020 2020   ...            
-0000c610: 2279 223a 207b 2266 6965 6c64 223a 2022  "y": {"field": "
-0000c620: 6222 2c20 2274 7970 6522 3a20 2271 7561  b", "type": "qua
-0000c630: 6e74 6974 6174 6976 6522 7d2c 0a20 2020  ntitative"},.   
-0000c640: 2020 2020 202e 2e2e 2020 2020 2020 2020       ...        
-0000c650: 2020 2020 2273 697a 6522 3a20 7b22 6669      "size": {"fi
-0000c660: 656c 6422 3a20 2263 222c 2022 7479 7065  eld": "c", "type
-0000c670: 223a 2022 7175 616e 7469 7461 7469 7665  ": "quantitative
-0000c680: 227d 2c0a 2020 2020 2020 2020 2e2e 2e20  "},.        ... 
-0000c690: 2020 2020 2020 2020 2020 2022 636f 6c6f             "colo
-0000c6a0: 7222 3a20 7b22 6669 656c 6422 3a20 2263  r": {"field": "c
-0000c6b0: 222c 2022 7479 7065 223a 2022 7175 616e  ", "type": "quan
-0000c6c0: 7469 7461 7469 7665 227d 2c0a 2020 2020  titative"},.    
-0000c6d0: 2020 2020 2e2e 2e20 2020 2020 2020 207d      ...        }
-0000c6e0: 2c0a 2020 2020 2020 2020 2e2e 2e20 2020  ,.        ...   
-0000c6f0: 207d 2c0a 2020 2020 2020 2020 2e2e 2e20   },.        ... 
-0000c700: 290a 0a20 2020 2020 2020 202e 2e20 6f75  )..        .. ou
-0000c710: 7470 7574 3a3a 0a20 2020 2020 2020 2020  tput::.         
-0000c720: 2020 6874 7470 733a 2f2f 646f 632d 7665    https://doc-ve
-0000c730: 6761 2d6c 6974 652d 6368 6172 742e 7374  ga-lite-chart.st
-0000c740: 7265 616d 6c69 742e 6170 702f 0a20 2020  reamlit.app/.   
-0000c750: 2020 2020 2020 2020 6865 6967 6874 3a20          height: 
-0000c760: 3330 3070 780a 0a20 2020 2020 2020 2045  300px..        E
-0000c770: 7861 6d70 6c65 7320 6f66 2056 6567 612d  xamples of Vega-
-0000c780: 4c69 7465 2075 7361 6765 2077 6974 686f  Lite usage witho
-0000c790: 7574 2053 7472 6561 6d6c 6974 2063 616e  ut Streamlit can
-0000c7a0: 2062 6520 666f 756e 6420 6174 0a20 2020   be found at.   
-0000c7b0: 2020 2020 2068 7474 7073 3a2f 2f76 6567       https://veg
-0000c7c0: 612e 6769 7468 7562 2e69 6f2f 7665 6761  a.github.io/vega
-0000c7d0: 2d6c 6974 652f 6578 616d 706c 6573 2f2e  -lite/examples/.
-0000c7e0: 204d 6f73 7420 6f66 2074 686f 7365 2063   Most of those c
-0000c7f0: 616e 2062 6520 6561 7369 6c79 0a20 2020  an be easily.   
-0000c800: 2020 2020 2074 7261 6e73 6c61 7465 6420       translated 
-0000c810: 746f 2074 6865 2073 796e 7461 7820 7368  to the syntax sh
-0000c820: 6f77 6e20 6162 6f76 652e 0a0a 2020 2020  own above...    
-0000c830: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-0000c840: 7265 7475 726e 2073 656c 662e 5f76 6567  return self._veg
-0000c850: 615f 6c69 7465 5f63 6861 7274 280a 2020  a_lite_chart(.  
-0000c860: 2020 2020 2020 2020 2020 6461 7461 3d64            data=d
-0000c870: 6174 612c 0a20 2020 2020 2020 2020 2020  ata,.           
-0000c880: 2073 7065 633d 7370 6563 2c0a 2020 2020   spec=spec,.    
-0000c890: 2020 2020 2020 2020 7573 655f 636f 6e74          use_cont
-0000c8a0: 6169 6e65 725f 7769 6474 683d 7573 655f  ainer_width=use_
-0000c8b0: 636f 6e74 6169 6e65 725f 7769 6474 682c  container_width,
-0000c8c0: 0a20 2020 2020 2020 2020 2020 2074 6865  .            the
-0000c8d0: 6d65 3d74 6865 6d65 2c0a 2020 2020 2020  me=theme,.      
-0000c8e0: 2020 2020 2020 6b65 793d 6b65 792c 0a20        key=key,. 
-0000c8f0: 2020 2020 2020 2020 2020 206f 6e5f 7365             on_se
-0000c900: 6c65 6374 3d6f 6e5f 7365 6c65 6374 2c0a  lect=on_select,.
-0000c910: 2020 2020 2020 2020 2020 2020 7365 6c65              sele
-0000c920: 6374 696f 6e5f 6d6f 6465 3d73 656c 6563  ction_mode=selec
-0000c930: 7469 6f6e 5f6d 6f64 652c 0a20 2020 2020  tion_mode,.     
-0000c940: 2020 2020 2020 202a 2a6b 7761 7267 732c         **kwargs,
-0000c950: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
-0000c960: 6465 6620 5f61 6c74 6169 725f 6368 6172  def _altair_char
-0000c970: 7428 0a20 2020 2020 2020 2073 656c 662c  t(.        self,
-0000c980: 0a20 2020 2020 2020 2061 6c74 6169 725f  .        altair_
-0000c990: 6368 6172 743a 2061 6c74 2e43 6861 7274  chart: alt.Chart
-0000c9a0: 2c0a 2020 2020 2020 2020 7573 655f 636f  ,.        use_co
-0000c9b0: 6e74 6169 6e65 725f 7769 6474 683a 2062  ntainer_width: b
-0000c9c0: 6f6f 6c20 3d20 4661 6c73 652c 0a20 2020  ool = False,.   
-0000c9d0: 2020 2020 2074 6865 6d65 3a20 4c69 7465       theme: Lite
-0000c9e0: 7261 6c5b 2273 7472 6561 6d6c 6974 225d  ral["streamlit"]
-0000c9f0: 207c 204e 6f6e 6520 3d20 2273 7472 6561   | None = "strea
-0000ca00: 6d6c 6974 222c 0a20 2020 2020 2020 206b  mlit",.        k
-0000ca10: 6579 3a20 4b65 7920 7c20 4e6f 6e65 203d  ey: Key | None =
-0000ca20: 204e 6f6e 652c 0a20 2020 2020 2020 206f   None,.        o
-0000ca30: 6e5f 7365 6c65 6374 3a20 4c69 7465 7261  n_select: Litera
-0000ca40: 6c5b 2272 6572 756e 222c 2022 6967 6e6f  l["rerun", "igno
-0000ca50: 7265 225d 207c 2057 6964 6765 7443 616c  re"] | WidgetCal
-0000ca60: 6c62 6163 6b20 3d20 2269 676e 6f72 6522  lback = "ignore"
-0000ca70: 2c0a 2020 2020 2020 2020 7365 6c65 6374  ,.        select
-0000ca80: 696f 6e5f 6d6f 6465 3a20 7374 7220 7c20  ion_mode: str | 
-0000ca90: 4974 6572 6162 6c65 5b73 7472 5d20 7c20  Iterable[str] | 
-0000caa0: 4e6f 6e65 203d 204e 6f6e 652c 0a20 2020  None = None,.   
-0000cab0: 2020 2020 2061 6464 5f72 6f77 735f 6d65       add_rows_me
-0000cac0: 7461 6461 7461 3a20 4164 6452 6f77 734d  tadata: AddRowsM
-0000cad0: 6574 6164 6174 6120 7c20 4e6f 6e65 203d  etadata | None =
-0000cae0: 204e 6f6e 652c 0a20 2020 2029 202d 3e20   None,.    ) -> 
-0000caf0: 4465 6c74 6147 656e 6572 6174 6f72 207c  DeltaGenerator |
-0000cb00: 2056 6567 614c 6974 6553 7461 7465 3a0a   VegaLiteState:.
-0000cb10: 2020 2020 2020 2020 2222 2249 6e74 6572          """Inter
-0000cb20: 6e61 6c20 6d65 7468 6f64 2074 6f20 656e  nal method to en
-0000cb30: 7175 6575 6520 6120 7665 6761 2d6c 6974  queue a vega-lit
-0000cb40: 6520 6368 6172 7420 656c 656d 656e 7420  e chart element 
-0000cb50: 6261 7365 6420 6f6e 2061 6e20 416c 7461  based on an Alta
-0000cb60: 6972 2063 6861 7274 2e0a 0a20 2020 2020  ir chart...     
-0000cb70: 2020 2053 6565 2074 6865 2060 616c 7461     See the `alta
-0000cb80: 6972 5f63 6861 7274 6020 6d65 7468 6f64  ir_chart` method
-0000cb90: 2064 6f63 7374 7269 6e67 2066 6f72 206d   docstring for m
-0000cba0: 6f72 6520 696e 666f 726d 6174 696f 6e2e  ore information.
-0000cbb0: 0a20 2020 2020 2020 2022 2222 0a0a 2020  .        """..  
-0000cbc0: 2020 2020 2020 6966 2074 7970 655f 7574        if type_ut
-0000cbd0: 696c 2e69 735f 616c 7461 6972 5f76 6572  il.is_altair_ver
-0000cbe0: 7369 6f6e 5f6c 6573 735f 7468 616e 2822  sion_less_than("
-0000cbf0: 352e 302e 3022 2920 616e 6420 6f6e 5f73  5.0.0") and on_s
-0000cc00: 656c 6563 7420 213d 2022 6967 6e6f 7265  elect != "ignore
-0000cc10: 223a 0a20 2020 2020 2020 2020 2020 2072  ":.            r
-0000cc20: 6169 7365 2053 7472 6561 6d6c 6974 4150  aise StreamlitAP
-0000cc30: 4945 7863 6570 7469 6f6e 280a 2020 2020  IException(.    
-0000cc40: 2020 2020 2020 2020 2020 2020 2253 7472              "Str
-0000cc50: 6561 6d6c 6974 2064 6f65 7320 6e6f 7420  eamlit does not 
-0000cc60: 7375 7070 6f72 7420 7365 6c65 6374 696f  support selectio
-0000cc70: 6e73 2077 6974 6820 416c 7461 6972 2034  ns with Altair 4
-0000cc80: 2e78 2e20 506c 6561 7365 2075 7067 7261  .x. Please upgra
-0000cc90: 6465 2074 6f20 5665 7273 696f 6e20 352e  de to Version 5.
-0000cca0: 2022 0a20 2020 2020 2020 2020 2020 2020   ".             
-0000ccb0: 2020 2022 4966 2079 6f75 2077 6f75 6c64     "If you would
-0000ccc0: 206c 696b 6520 746f 2075 7365 2041 6c74   like to use Alt
-0000ccd0: 6169 7220 342e 7820 7769 7468 2073 656c  air 4.x with sel
-0000cce0: 6563 7469 6f6e 732c 2070 6c65 6173 6520  ections, please 
-0000ccf0: 7570 766f 7465 2022 0a20 2020 2020 2020  upvote ".       
-0000cd00: 2020 2020 2020 2020 2022 7468 6973 205b           "this [
-0000cd10: 4769 7468 7562 2069 7373 7565 5d28 6874  Github issue](ht
-0000cd20: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-0000cd30: 2f73 7472 6561 6d6c 6974 2f73 7472 6561  /streamlit/strea
-0000cd40: 6d6c 6974 2f69 7373 7565 732f 3835 3136  mlit/issues/8516
-0000cd50: 292e 220a 2020 2020 2020 2020 2020 2020  ).".            
-0000cd60: 290a 0a20 2020 2020 2020 2076 6567 615f  )..        vega_
-0000cd70: 6c69 7465 5f73 7065 6320 3d20 5f63 6f6e  lite_spec = _con
-0000cd80: 7665 7274 5f61 6c74 6169 725f 746f 5f76  vert_altair_to_v
-0000cd90: 6567 615f 6c69 7465 5f73 7065 6328 616c  ega_lite_spec(al
-0000cda0: 7461 6972 5f63 6861 7274 290a 2020 2020  tair_chart).    
-0000cdb0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-0000cdc0: 5f76 6567 615f 6c69 7465 5f63 6861 7274  _vega_lite_chart
-0000cdd0: 280a 2020 2020 2020 2020 2020 2020 6461  (.            da
-0000cde0: 7461 3d4e 6f6e 652c 2020 2320 5468 6520  ta=None,  # The 
-0000cdf0: 6461 7461 2069 7320 616c 7265 6164 7920  data is already 
-0000ce00: 7061 7274 206f 6620 7468 6520 7370 6563  part of the spec
-0000ce10: 0a20 2020 2020 2020 2020 2020 2073 7065  .            spe
-0000ce20: 633d 7665 6761 5f6c 6974 655f 7370 6563  c=vega_lite_spec
-0000ce30: 2c0a 2020 2020 2020 2020 2020 2020 7573  ,.            us
-0000ce40: 655f 636f 6e74 6169 6e65 725f 7769 6474  e_container_widt
-0000ce50: 683d 7573 655f 636f 6e74 6169 6e65 725f  h=use_container_
-0000ce60: 7769 6474 682c 0a20 2020 2020 2020 2020  width,.         
-0000ce70: 2020 2074 6865 6d65 3d74 6865 6d65 2c0a     theme=theme,.
-0000ce80: 2020 2020 2020 2020 2020 2020 6b65 793d              key=
-0000ce90: 6b65 792c 0a20 2020 2020 2020 2020 2020  key,.           
-0000cea0: 206f 6e5f 7365 6c65 6374 3d6f 6e5f 7365   on_select=on_se
-0000ceb0: 6c65 6374 2c0a 2020 2020 2020 2020 2020  lect,.          
-0000cec0: 2020 7365 6c65 6374 696f 6e5f 6d6f 6465    selection_mode
-0000ced0: 3d73 656c 6563 7469 6f6e 5f6d 6f64 652c  =selection_mode,
-0000cee0: 0a20 2020 2020 2020 2020 2020 2061 6464  .            add
-0000cef0: 5f72 6f77 735f 6d65 7461 6461 7461 3d61  _rows_metadata=a
-0000cf00: 6464 5f72 6f77 735f 6d65 7461 6461 7461  dd_rows_metadata
-0000cf10: 2c0a 2020 2020 2020 2020 290a 0a20 2020  ,.        )..   
-0000cf20: 2064 6566 205f 7665 6761 5f6c 6974 655f   def _vega_lite_
-0000cf30: 6368 6172 7428 0a20 2020 2020 2020 2073  chart(.        s
-0000cf40: 656c 662c 0a20 2020 2020 2020 2064 6174  elf,.        dat
-0000cf50: 613a 2044 6174 6120 3d20 4e6f 6e65 2c0a  a: Data = None,.
-0000cf60: 2020 2020 2020 2020 7370 6563 3a20 5665          spec: Ve
-0000cf70: 6761 4c69 7465 5370 6563 207c 204e 6f6e  gaLiteSpec | Non
-0000cf80: 6520 3d20 4e6f 6e65 2c0a 2020 2020 2020  e = None,.      
-0000cf90: 2020 7573 655f 636f 6e74 6169 6e65 725f    use_container_
-0000cfa0: 7769 6474 683a 2062 6f6f 6c20 3d20 4661  width: bool = Fa
-0000cfb0: 6c73 652c 0a20 2020 2020 2020 2074 6865  lse,.        the
-0000cfc0: 6d65 3a20 4c69 7465 7261 6c5b 2273 7472  me: Literal["str
-0000cfd0: 6561 6d6c 6974 225d 207c 204e 6f6e 6520  eamlit"] | None 
-0000cfe0: 3d20 2273 7472 6561 6d6c 6974 222c 0a20  = "streamlit",. 
-0000cff0: 2020 2020 2020 206b 6579 3a20 4b65 7920         key: Key 
-0000d000: 7c20 4e6f 6e65 203d 204e 6f6e 652c 0a20  | None = None,. 
-0000d010: 2020 2020 2020 206f 6e5f 7365 6c65 6374         on_select
-0000d020: 3a20 4c69 7465 7261 6c5b 2272 6572 756e  : Literal["rerun
-0000d030: 222c 2022 6967 6e6f 7265 225d 207c 2057  ", "ignore"] | W
-0000d040: 6964 6765 7443 616c 6c62 6163 6b20 3d20  idgetCallback = 
-0000d050: 2269 676e 6f72 6522 2c0a 2020 2020 2020  "ignore",.      
-0000d060: 2020 7365 6c65 6374 696f 6e5f 6d6f 6465    selection_mode
-0000d070: 3a20 7374 7220 7c20 4974 6572 6162 6c65  : str | Iterable
-0000d080: 5b73 7472 5d20 7c20 4e6f 6e65 203d 204e  [str] | None = N
-0000d090: 6f6e 652c 0a20 2020 2020 2020 2061 6464  one,.        add
-0000d0a0: 5f72 6f77 735f 6d65 7461 6461 7461 3a20  _rows_metadata: 
-0000d0b0: 4164 6452 6f77 734d 6574 6164 6174 6120  AddRowsMetadata 
-0000d0c0: 7c20 4e6f 6e65 203d 204e 6f6e 652c 0a20  | None = None,. 
-0000d0d0: 2020 2020 2020 202a 2a6b 7761 7267 733a         **kwargs:
-0000d0e0: 2041 6e79 2c0a 2020 2020 2920 2d3e 2044   Any,.    ) -> D
-0000d0f0: 656c 7461 4765 6e65 7261 746f 7220 7c20  eltaGenerator | 
-0000d100: 5665 6761 4c69 7465 5374 6174 653a 0a20  VegaLiteState:. 
-0000d110: 2020 2020 2020 2022 2222 496e 7465 726e         """Intern
-0000d120: 616c 206d 6574 686f 6420 746f 2065 6e71  al method to enq
-0000d130: 7565 7565 2061 2076 6567 612d 6c69 7465  ueue a vega-lite
-0000d140: 2063 6861 7274 2065 6c65 6d65 6e74 2062   chart element b
-0000d150: 6173 6564 206f 6e20 6120 7665 6761 2d6c  ased on a vega-l
-0000d160: 6974 6520 7370 6563 2e0a 0a20 2020 2020  ite spec...     
-0000d170: 2020 2053 6565 2074 6865 2060 7665 6761     See the `vega
-0000d180: 5f6c 6974 655f 6368 6172 7460 206d 6574  _lite_chart` met
-0000d190: 686f 6420 646f 6373 7472 696e 6720 666f  hod docstring fo
-0000d1a0: 7220 6d6f 7265 2069 6e66 6f72 6d61 7469  r more informati
-0000d1b0: 6f6e 2e0a 2020 2020 2020 2020 2222 220a  on..        """.
-0000d1c0: 0a20 2020 2020 2020 2069 6620 7468 656d  .        if them
-0000d1d0: 6520 6e6f 7420 696e 205b 2273 7472 6561  e not in ["strea
-0000d1e0: 6d6c 6974 222c 204e 6f6e 655d 3a0a 2020  mlit", None]:.  
-0000d1f0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-0000d200: 5374 7265 616d 6c69 7441 5049 4578 6365  StreamlitAPIExce
-0000d210: 7074 696f 6e28 0a20 2020 2020 2020 2020  ption(.         
-0000d220: 2020 2020 2020 2066 2759 6f75 2073 6574         f'You set
-0000d230: 2074 6865 6d65 3d22 7b74 6865 6d65 7d22   theme="{theme}"
-0000d240: 2077 6869 6c65 2053 7472 6561 6d6c 6974   while Streamlit
-0000d250: 2063 6861 7274 7320 6f6e 6c79 2073 7570   charts only sup
-0000d260: 706f 7274 2074 6865 6d65 3de2 809d 7374  port theme=...st
-0000d270: 7265 616d 6c69 74e2 809d 206f 7220 7468  reamlit... or th
-0000d280: 656d 653d 4e6f 6e65 2074 6f20 6661 6c6c  eme=None to fall
-0000d290: 6261 636b 2074 6f20 7468 6520 6465 6661  back to the defa
-0000d2a0: 756c 7420 6c69 6272 6172 7920 7468 656d  ult library them
-0000d2b0: 652e 270a 2020 2020 2020 2020 2020 2020  e.'.            
-0000d2c0: 290a 0a20 2020 2020 2020 2069 6620 6f6e  )..        if on
-0000d2d0: 5f73 656c 6563 7420 6e6f 7420 696e 205b  _select not in [
-0000d2e0: 2269 676e 6f72 6522 2c20 2272 6572 756e  "ignore", "rerun
-0000d2f0: 225d 2061 6e64 206e 6f74 2063 616c 6c61  "] and not calla
-0000d300: 626c 6528 6f6e 5f73 656c 6563 7429 3a0a  ble(on_select):.
-0000d310: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-0000d320: 6520 5374 7265 616d 6c69 7441 5049 4578  e StreamlitAPIEx
-0000d330: 6365 7074 696f 6e28 0a20 2020 2020 2020  ception(.       
-0000d340: 2020 2020 2020 2020 2066 2259 6f75 2068           f"You h
-0000d350: 6176 6520 7061 7373 6564 207b 6f6e 5f73  ave passed {on_s
-0000d360: 656c 6563 747d 2074 6f20 606f 6e5f 7365  elect} to `on_se
-0000d370: 6c65 6374 602e 2042 7574 206f 6e6c 7920  lect`. But only 
-0000d380: 2769 676e 6f72 6527 2c20 2772 6572 756e  'ignore', 'rerun
-0000d390: 272c 206f 7220 6120 6361 6c6c 6162 6c65  ', or a callable
-0000d3a0: 2069 7320 7375 7070 6f72 7465 642e 220a   is supported.".
-0000d3b0: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
-0000d3c0: 2020 2020 2020 206b 6579 203d 2074 6f5f         key = to_
-0000d3d0: 6b65 7928 6b65 7929 0a20 2020 2020 2020  key(key).       
-0000d3e0: 2069 735f 7365 6c65 6374 696f 6e5f 6163   is_selection_ac
-0000d3f0: 7469 7661 7465 6420 3d20 6f6e 5f73 656c  tivated = on_sel
-0000d400: 6563 7420 213d 2022 6967 6e6f 7265 220a  ect != "ignore".
-0000d410: 0a20 2020 2020 2020 2069 6620 6973 5f73  .        if is_s
-0000d420: 656c 6563 7469 6f6e 5f61 6374 6976 6174  election_activat
-0000d430: 6564 3a0a 2020 2020 2020 2020 2020 2020  ed:.            
-0000d440: 2320 5275 6e20 736f 6d65 2063 6865 636b  # Run some check
-0000d450: 7320 7468 6174 2061 7265 206f 6e6c 7920  s that are only 
-0000d460: 7265 6c65 7661 6e74 2077 6865 6e20 7365  relevant when se
-0000d470: 6c65 6374 696f 6e73 2061 7265 2061 6374  lections are act
-0000d480: 6976 6174 6564 0a0a 2020 2020 2020 2020  ivated..        
-0000d490: 2020 2020 2320 496d 706f 7274 2068 6572      # Import her
-0000d4a0: 6520 746f 2061 766f 6964 2063 6972 6375  e to avoid circu
-0000d4b0: 6c61 7220 696d 706f 7274 730a 2020 2020  lar imports.    
-0000d4c0: 2020 2020 2020 2020 6672 6f6d 2073 7472          from str
-0000d4d0: 6561 6d6c 6974 2e65 6c65 6d65 6e74 732e  eamlit.elements.
-0000d4e0: 7574 696c 7320 696d 706f 7274 2028 0a20  utils import (. 
-0000d4f0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-0000d500: 6865 636b 5f63 6163 6865 5f72 6570 6c61  heck_cache_repla
-0000d510: 795f 7275 6c65 732c 0a20 2020 2020 2020  y_rules,.       
-0000d520: 2020 2020 2020 2020 2063 6865 636b 5f63           check_c
-0000d530: 616c 6c62 6163 6b5f 7275 6c65 732c 0a20  allback_rules,. 
-0000d540: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-0000d550: 6865 636b 5f73 6573 7369 6f6e 5f73 7461  heck_session_sta
-0000d560: 7465 5f72 756c 6573 2c0a 2020 2020 2020  te_rules,.      
-0000d570: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-0000d580: 2020 2020 2063 6865 636b 5f63 6163 6865       check_cache
-0000d590: 5f72 6570 6c61 795f 7275 6c65 7328 290a  _replay_rules().
-0000d5a0: 2020 2020 2020 2020 2020 2020 6966 2063              if c
-0000d5b0: 616c 6c61 626c 6528 6f6e 5f73 656c 6563  allable(on_selec
-0000d5c0: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
-0000d5d0: 2020 2020 6368 6563 6b5f 6361 6c6c 6261      check_callba
-0000d5e0: 636b 5f72 756c 6573 2873 656c 662e 6467  ck_rules(self.dg
-0000d5f0: 2c20 6f6e 5f73 656c 6563 7429 0a20 2020  , on_select).   
-0000d600: 2020 2020 2020 2020 2063 6865 636b 5f73           check_s
-0000d610: 6573 7369 6f6e 5f73 7461 7465 5f72 756c  ession_state_rul
-0000d620: 6573 2864 6566 6175 6c74 5f76 616c 7565  es(default_value
-0000d630: 3d4e 6f6e 652c 206b 6579 3d6b 6579 2c20  =None, key=key, 
-0000d640: 7772 6974 6573 5f61 6c6c 6f77 6564 3d46  writes_allowed=F
-0000d650: 616c 7365 290a 0a20 2020 2020 2020 2023  alse)..        #
-0000d660: 2053 7570 706f 7274 2070 6173 7369 6e67   Support passing
-0000d670: 2064 6174 6120 696e 7369 6465 2073 7065   data inside spe
-0000d680: 635b 2764 6174 6173 6574 7327 5d20 616e  c['datasets'] an
-0000d690: 6420 7370 6563 5b27 6461 7461 275d 2e0a  d spec['data']..
-0000d6a0: 2020 2020 2020 2020 2320 2854 6865 2064          # (The d
-0000d6b0: 6174 6120 6765 7473 2070 756c 6c65 6420  ata gets pulled 
-0000d6c0: 6f75 7420 6f66 2074 6865 2073 7065 6320  out of the spec 
-0000d6d0: 6469 6374 206c 6174 6572 206f 6e2e 290a  dict later on.).
-0000d6e0: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
-0000d6f0: 7461 6e63 6528 6461 7461 2c20 6469 6374  tance(data, dict
-0000d700: 2920 616e 6420 7370 6563 2069 7320 4e6f  ) and spec is No
-0000d710: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0000d720: 7370 6563 203d 2064 6174 610a 2020 2020  spec = data.    
-0000d730: 2020 2020 2020 2020 6461 7461 203d 204e          data = N
-0000d740: 6f6e 650a 0a20 2020 2020 2020 2069 6620  one..        if 
-0000d750: 7370 6563 2069 7320 4e6f 6e65 3a0a 2020  spec is None:.  
-0000d760: 2020 2020 2020 2020 2020 7370 6563 203d            spec =
-0000d770: 207b 7d0a 0a20 2020 2020 2020 2076 6567   {}..        veg
-0000d780: 615f 6c69 7465 5f70 726f 746f 203d 2041  a_lite_proto = A
-0000d790: 7272 6f77 5665 6761 4c69 7465 4368 6172  rrowVegaLiteChar
-0000d7a0: 7450 726f 746f 2829 0a0a 2020 2020 2020  tProto()..      
-0000d7b0: 2020 7370 6563 203d 205f 7072 6570 6172    spec = _prepar
-0000d7c0: 655f 7665 6761 5f6c 6974 655f 7370 6563  e_vega_lite_spec
-0000d7d0: 2873 7065 632c 2075 7365 5f63 6f6e 7461  (spec, use_conta
-0000d7e0: 696e 6572 5f77 6964 7468 2c20 2a2a 6b77  iner_width, **kw
-0000d7f0: 6172 6773 290a 2020 2020 2020 2020 5f6d  args).        _m
-0000d800: 6172 7368 616c 6c5f 6368 6172 745f 6461  arshall_chart_da
-0000d810: 7461 2876 6567 615f 6c69 7465 5f70 726f  ta(vega_lite_pro
-0000d820: 746f 2c20 7370 6563 2c20 6461 7461 290a  to, spec, data).
-0000d830: 0a20 2020 2020 2020 2023 2050 7265 7665  .        # Preve
-0000d840: 6e74 2074 6865 2073 7065 6320 6672 6f6d  nt the spec from
-0000d850: 2063 6861 6e67 696e 6720 6163 726f 7373   changing across
-0000d860: 2072 6572 756e 733a 0a20 2020 2020 2020   reruns:.       
-0000d870: 2076 6567 615f 6c69 7465 5f70 726f 746f   vega_lite_proto
-0000d880: 2e73 7065 6320 3d20 5f73 7461 6269 6c69  .spec = _stabili
-0000d890: 7a65 5f76 6567 615f 6a73 6f6e 5f73 7065  ze_vega_json_spe
-0000d8a0: 6328 6a73 6f6e 2e64 756d 7073 2873 7065  c(json.dumps(spe
-0000d8b0: 6329 290a 2020 2020 2020 2020 7665 6761  c)).        vega
-0000d8c0: 5f6c 6974 655f 7072 6f74 6f2e 7573 655f  _lite_proto.use_
-0000d8d0: 636f 6e74 6169 6e65 725f 7769 6474 6820  container_width 
-0000d8e0: 3d20 7573 655f 636f 6e74 6169 6e65 725f  = use_container_
-0000d8f0: 7769 6474 680a 2020 2020 2020 2020 7665  width.        ve
-0000d900: 6761 5f6c 6974 655f 7072 6f74 6f2e 7468  ga_lite_proto.th
-0000d910: 656d 6520 3d20 7468 656d 6520 6f72 2022  eme = theme or "
-0000d920: 220a 0a20 2020 2020 2020 2069 6620 6973  "..        if is
-0000d930: 5f73 656c 6563 7469 6f6e 5f61 6374 6976  _selection_activ
-0000d940: 6174 6564 3a0a 2020 2020 2020 2020 2020  ated:.          
-0000d950: 2020 2320 496d 706f 7274 2068 6572 6520    # Import here 
-0000d960: 746f 2061 766f 6964 2063 6972 6375 6c61  to avoid circula
-0000d970: 7220 696d 706f 7274 730a 2020 2020 2020  r imports.      
-0000d980: 2020 2020 2020 6672 6f6d 2073 7472 6561        from strea
-0000d990: 6d6c 6974 2e65 6c65 6d65 6e74 732e 666f  mlit.elements.fo
-0000d9a0: 726d 2069 6d70 6f72 7420 6375 7272 656e  rm import curren
-0000d9b0: 745f 666f 726d 5f69 640a 0a20 2020 2020  t_form_id..     
-0000d9c0: 2020 2020 2020 2023 204c 6f61 6420 7468         # Load th
-0000d9d0: 6520 7374 6162 696c 697a 6564 2073 7065  e stabilized spe
-0000d9e0: 6320 6167 6169 6e20 6173 2061 2064 6963  c again as a dic
-0000d9f0: 743a 0a20 2020 2020 2020 2020 2020 2066  t:.            f
-0000da00: 696e 616c 5f73 7065 6320 3d20 6a73 6f6e  inal_spec = json
-0000da10: 2e6c 6f61 6473 2876 6567 615f 6c69 7465  .loads(vega_lite
-0000da20: 5f70 726f 746f 2e73 7065 6329 0a20 2020  _proto.spec).   
-0000da30: 2020 2020 2020 2020 2023 2054 656d 706f           # Tempo
-0000da40: 7261 7279 206c 696d 6974 6174 696f 6e20  rary limitation 
-0000da50: 746f 2064 6973 616c 6c6f 7720 6d75 6c74  to disallow mult
-0000da60: 692d 7669 6577 2063 6861 7274 7320 2863  i-view charts (c
-0000da70: 6f6d 706f 7369 7469 6f6e 7329 2077 6974  ompositions) wit
-0000da80: 6820 7365 6c65 6374 696f 6e73 2e0a 2020  h selections..  
-0000da90: 2020 2020 2020 2020 2020 5f64 6973 616c            _disal
-0000daa0: 6c6f 775f 6d75 6c74 695f 7669 6577 5f63  low_multi_view_c
-0000dab0: 6861 7274 7328 6669 6e61 6c5f 7370 6563  harts(final_spec
-0000dac0: 290a 0a20 2020 2020 2020 2020 2020 2023  )..            #
-0000dad0: 2050 6172 7365 2061 6e64 2063 6865 636b   Parse and check
-0000dae0: 2074 6865 2073 7065 6369 6669 6564 2073   the specified s
-0000daf0: 656c 6563 7469 6f6e 206d 6f64 6573 0a20  election modes. 
-0000db00: 2020 2020 2020 2020 2020 2070 6172 7365             parse
-0000db10: 645f 7365 6c65 6374 696f 6e5f 6d6f 6465  d_selection_mode
-0000db20: 7320 3d20 5f70 6172 7365 5f73 656c 6563  s = _parse_selec
-0000db30: 7469 6f6e 5f6d 6f64 6528 6669 6e61 6c5f  tion_mode(final_
-0000db40: 7370 6563 2c20 7365 6c65 6374 696f 6e5f  spec, selection_
-0000db50: 6d6f 6465 290a 2020 2020 2020 2020 2020  mode).          
-0000db60: 2020 7665 6761 5f6c 6974 655f 7072 6f74    vega_lite_prot
-0000db70: 6f2e 7365 6c65 6374 696f 6e5f 6d6f 6465  o.selection_mode
-0000db80: 2e65 7874 656e 6428 7061 7273 6564 5f73  .extend(parsed_s
-0000db90: 656c 6563 7469 6f6e 5f6d 6f64 6573 290a  election_modes).
-0000dba0: 0a20 2020 2020 2020 2020 2020 2076 6567  .            veg
-0000dbb0: 615f 6c69 7465 5f70 726f 746f 2e66 6f72  a_lite_proto.for
-0000dbc0: 6d5f 6964 203d 2063 7572 7265 6e74 5f66  m_id = current_f
-0000dbd0: 6f72 6d5f 6964 2873 656c 662e 6467 290a  orm_id(self.dg).
-0000dbe0: 0a20 2020 2020 2020 2020 2020 2063 7478  .            ctx
-0000dbf0: 203d 2067 6574 5f73 6372 6970 745f 7275   = get_script_ru
-0000dc00: 6e5f 6374 7828 290a 2020 2020 2020 2020  n_ctx().        
-0000dc10: 2020 2020 7665 6761 5f6c 6974 655f 7072      vega_lite_pr
-0000dc20: 6f74 6f2e 6964 203d 2063 6f6d 7075 7465  oto.id = compute
-0000dc30: 5f77 6964 6765 745f 6964 280a 2020 2020  _widget_id(.    
-0000dc40: 2020 2020 2020 2020 2020 2020 2261 7272              "arr
-0000dc50: 6f77 5f76 6567 615f 6c69 7465 5f63 6861  ow_vega_lite_cha
-0000dc60: 7274 222c 0a20 2020 2020 2020 2020 2020  rt",.           
-0000dc70: 2020 2020 2075 7365 725f 6b65 793d 6b65       user_key=ke
-0000dc80: 792c 0a20 2020 2020 2020 2020 2020 2020  y,.             
-0000dc90: 2020 206b 6579 3d6b 6579 2c0a 2020 2020     key=key,.    
-0000dca0: 2020 2020 2020 2020 2020 2020 7665 6761              vega
-0000dcb0: 5f6c 6974 655f 7370 6563 3d76 6567 615f  _lite_spec=vega_
-0000dcc0: 6c69 7465 5f70 726f 746f 2e73 7065 632c  lite_proto.spec,
-0000dcd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000dce0: 2023 2054 6865 2064 6174 6120 6973 2065   # The data is e
-0000dcf0: 6974 6865 7220 696e 2076 6567 615f 6c69  ither in vega_li
-0000dd00: 7465 5f70 726f 746f 2e64 6174 612e 6461  te_proto.data.da
-0000dd10: 7461 0a20 2020 2020 2020 2020 2020 2020  ta.             
-0000dd20: 2020 2023 206f 7220 696e 2061 206e 616d     # or in a nam
-0000dd30: 6564 2064 6174 6173 6574 2069 6e20 7665  ed dataset in ve
-0000dd40: 6761 5f6c 6974 655f 7072 6f74 6f2e 6461  ga_lite_proto.da
-0000dd50: 7461 7365 7473 0a20 2020 2020 2020 2020  tasets.         
-0000dd60: 2020 2020 2020 2076 6567 615f 6c69 7465         vega_lite
-0000dd70: 5f64 6174 613d 7665 6761 5f6c 6974 655f  _data=vega_lite_
-0000dd80: 7072 6f74 6f2e 6461 7461 2e64 6174 612c  proto.data.data,
-0000dd90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000dda0: 2023 2049 7473 2065 6e6f 7567 6820 746f   # Its enough to
-0000ddb0: 206a 7573 7420 7573 6520 7468 6520 6e61   just use the na
-0000ddc0: 6d65 7320 6865 7265 2073 696e 6365 2074  mes here since t
-0000ddd0: 6865 7920 6172 6520 6578 7065 6374 6564  hey are expected
-0000dde0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ddf0: 2023 2074 6f20 636f 6e74 6169 6e20 6861   # to contain ha
-0000de00: 7368 6573 2062 6173 6564 206f 6e20 7468  shes based on th
-0000de10: 6520 6461 7461 7365 7420 6461 7461 2e0a  e dataset data..
-0000de20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000de30: 6e61 6d65 645f 6461 7461 7365 7473 3d5b  named_datasets=[
-0000de40: 6461 7461 7365 742e 6e61 6d65 2066 6f72  dataset.name for
-0000de50: 2064 6174 6173 6574 2069 6e20 7665 6761   dataset in vega
-0000de60: 5f6c 6974 655f 7072 6f74 6f2e 6461 7461  _lite_proto.data
-0000de70: 7365 7473 5d2c 0a20 2020 2020 2020 2020  sets],.         
-0000de80: 2020 2020 2020 2074 6865 6d65 3d74 6865         theme=the
-0000de90: 6d65 2c0a 2020 2020 2020 2020 2020 2020  me,.            
-0000dea0: 2020 2020 7573 655f 636f 6e74 6169 6e65      use_containe
-0000deb0: 725f 7769 6474 683d 7573 655f 636f 6e74  r_width=use_cont
-0000dec0: 6169 6e65 725f 7769 6474 682c 0a20 2020  ainer_width,.   
-0000ded0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000dee0: 6563 7469 6f6e 5f6d 6f64 653d 7061 7273  ection_mode=pars
-0000def0: 6564 5f73 656c 6563 7469 6f6e 5f6d 6f64  ed_selection_mod
-0000df00: 6573 2c0a 2020 2020 2020 2020 2020 2020  es,.            
-0000df10: 2020 2020 666f 726d 5f69 643d 7665 6761      form_id=vega
-0000df20: 5f6c 6974 655f 7072 6f74 6f2e 666f 726d  _lite_proto.form
-0000df30: 5f69 642c 0a20 2020 2020 2020 2020 2020  _id,.           
-0000df40: 2020 2020 2070 6167 653d 6374 782e 7061       page=ctx.pa
-0000df50: 6765 5f73 6372 6970 745f 6861 7368 2069  ge_script_hash i
-0000df60: 6620 6374 7820 656c 7365 204e 6f6e 652c  f ctx else None,
-0000df70: 0a20 2020 2020 2020 2020 2020 2029 0a0a  .            )..
-0000df80: 2020 2020 2020 2020 2020 2020 7365 7264              serd
-0000df90: 6520 3d20 5665 6761 4c69 7465 5374 6174  e = VegaLiteStat
-0000dfa0: 6553 6572 6465 2870 6172 7365 645f 7365  eSerde(parsed_se
-0000dfb0: 6c65 6374 696f 6e5f 6d6f 6465 7329 0a0a  lection_modes)..
-0000dfc0: 2020 2020 2020 2020 2020 2020 7769 6467              widg
-0000dfd0: 6574 5f73 7461 7465 203d 2072 6567 6973  et_state = regis
-0000dfe0: 7465 725f 7769 6467 6574 280a 2020 2020  ter_widget(.    
-0000dff0: 2020 2020 2020 2020 2020 2020 2276 6567              "veg
-0000e000: 615f 6c69 7465 5f63 6861 7274 222c 0a20  a_lite_chart",. 
-0000e010: 2020 2020 2020 2020 2020 2020 2020 2076                 v
-0000e020: 6567 615f 6c69 7465 5f70 726f 746f 2c0a  ega_lite_proto,.
-0000e030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e040: 7573 6572 5f6b 6579 3d6b 6579 2c0a 2020  user_key=key,.  
-0000e050: 2020 2020 2020 2020 2020 2020 2020 6f6e                on
-0000e060: 5f63 6861 6e67 655f 6861 6e64 6c65 723d  _change_handler=
-0000e070: 6f6e 5f73 656c 6563 7420 6966 2063 616c  on_select if cal
-0000e080: 6c61 626c 6528 6f6e 5f73 656c 6563 7429  lable(on_select)
-0000e090: 2065 6c73 6520 4e6f 6e65 2c0a 2020 2020   else None,.    
-0000e0a0: 2020 2020 2020 2020 2020 2020 6465 7365              dese
-0000e0b0: 7269 616c 697a 6572 3d73 6572 6465 2e64  rializer=serde.d
-0000e0c0: 6573 6572 6961 6c69 7a65 2c0a 2020 2020  eserialize,.    
-0000e0d0: 2020 2020 2020 2020 2020 2020 7365 7269              seri
-0000e0e0: 616c 697a 6572 3d73 6572 6465 2e73 6572  alizer=serde.ser
-0000e0f0: 6961 6c69 7a65 2c0a 2020 2020 2020 2020  ialize,.        
-0000e100: 2020 2020 2020 2020 6374 783d 6374 782c          ctx=ctx,
-0000e110: 0a20 2020 2020 2020 2020 2020 2029 0a0a  .            )..
-0000e120: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000e130: 2e64 672e 5f65 6e71 7565 7565 280a 2020  .dg._enqueue(.  
-0000e140: 2020 2020 2020 2020 2020 2020 2020 2261                "a
-0000e150: 7272 6f77 5f76 6567 615f 6c69 7465 5f63  rrow_vega_lite_c
-0000e160: 6861 7274 222c 0a20 2020 2020 2020 2020  hart",.         
-0000e170: 2020 2020 2020 2076 6567 615f 6c69 7465         vega_lite
-0000e180: 5f70 726f 746f 2c0a 2020 2020 2020 2020  _proto,.        
-0000e190: 2020 2020 2020 2020 6164 645f 726f 7773          add_rows
-0000e1a0: 5f6d 6574 6164 6174 613d 6164 645f 726f  _metadata=add_ro
-0000e1b0: 7773 5f6d 6574 6164 6174 612c 0a20 2020  ws_metadata,.   
-0000e1c0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-0000e1d0: 2020 2020 2020 2072 6574 7572 6e20 6361         return ca
-0000e1e0: 7374 2856 6567 614c 6974 6553 7461 7465  st(VegaLiteState
-0000e1f0: 2c20 7769 6467 6574 5f73 7461 7465 2e76  , widget_state.v
-0000e200: 616c 7565 290a 2020 2020 2020 2020 2320  alue).        # 
-0000e210: 4966 2069 7473 206e 6f74 2075 7365 6420  If its not used 
-0000e220: 7769 7468 2073 656c 6563 7469 6f6e 7320  with selections 
-0000e230: 6163 7469 7661 7465 642c 206a 7573 7420  activated, just 
-0000e240: 7265 7475 726e 0a20 2020 2020 2020 2023  return.        #
-0000e250: 2074 6865 2064 656c 7461 2067 656e 6572   the delta gener
-0000e260: 6174 6f72 2072 656c 6174 6564 2074 6f20  ator related to 
-0000e270: 7468 6973 2065 6c65 6d65 6e74 2e0a 2020  this element..  
-0000e280: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-0000e290: 662e 6467 2e5f 656e 7175 6575 6528 0a20  f.dg._enqueue(. 
-0000e2a0: 2020 2020 2020 2020 2020 2022 6172 726f             "arro
-0000e2b0: 775f 7665 6761 5f6c 6974 655f 6368 6172  w_vega_lite_char
-0000e2c0: 7422 2c0a 2020 2020 2020 2020 2020 2020  t",.            
-0000e2d0: 7665 6761 5f6c 6974 655f 7072 6f74 6f2c  vega_lite_proto,
-0000e2e0: 0a20 2020 2020 2020 2020 2020 2061 6464  .            add
-0000e2f0: 5f72 6f77 735f 6d65 7461 6461 7461 3d61  _rows_metadata=a
-0000e300: 6464 5f72 6f77 735f 6d65 7461 6461 7461  dd_rows_metadata
-0000e310: 2c0a 2020 2020 2020 2020 290a 0a20 2020  ,.        )..   
-0000e320: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
-0000e330: 6566 2064 6728 7365 6c66 2920 2d3e 2044  ef dg(self) -> D
-0000e340: 656c 7461 4765 6e65 7261 746f 723a 0a20  eltaGenerator:. 
-0000e350: 2020 2020 2020 2022 2222 4765 7420 6f75         """Get ou
-0000e360: 7220 4465 6c74 6147 656e 6572 6174 6f72  r DeltaGenerator
-0000e370: 2e22 2222 0a20 2020 2020 2020 2072 6574  .""".        ret
-0000e380: 7572 6e20 6361 7374 2822 4465 6c74 6147  urn cast("DeltaG
-0000e390: 656e 6572 6174 6f72 222c 2073 656c 6629  enerator", self)
-0000e3a0: 0a                                       .
+00000a00: 2020 2054 6865 2073 6368 656d 6120 666f     The schema fo
+00000a10: 7220 7468 6520 5665 6761 2d4c 6974 6520  r the Vega-Lite 
+00000a20: 6576 656e 7420 7374 6174 652e 0a0a 2020  event state...  
+00000a30: 2020 5468 6520 6576 656e 7420 7374 6174    The event stat
+00000a40: 6520 6973 2073 746f 7265 6420 696e 2061  e is stored in a
+00000a50: 2064 6963 7469 6f6e 6172 792d 6c69 6b65   dictionary-like
+00000a60: 206f 626a 6563 7420 7468 6174 2073 7570   object that sup
+00000a70: 6f72 7473 2062 6f74 680a 2020 2020 6b65  orts both.    ke
+00000a80: 7920 616e 6420 6174 7472 6962 7574 6520  y and attribute 
+00000a90: 6e6f 7461 7469 6f6e 2e20 4576 656e 7420  notation. Event 
+00000aa0: 7374 6174 6573 2063 616e 6e6f 7420 6265  states cannot be
+00000ab0: 2070 726f 6772 616d 6d61 7469 6361 6c6c   programmaticall
+00000ac0: 790a 2020 2020 6368 616e 6765 6420 6f72  y.    changed or
+00000ad0: 2073 6574 2074 6872 6f75 6768 2053 6573   set through Ses
+00000ae0: 7369 6f6e 2053 7461 7465 2e0a 0a20 2020  sion State...   
+00000af0: 204f 6e6c 7920 7365 6c65 6374 696f 6e20   Only selection 
+00000b00: 6576 656e 7473 2061 7265 2073 7570 706f  events are suppo
+00000b10: 7274 6564 2061 7420 7468 6973 2074 696d  rted at this tim
+00000b20: 652e 0a0a 2020 2020 4174 7472 6962 7574  e...    Attribut
+00000b30: 6573 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  es.    ---------
+00000b40: 2d0a 2020 2020 7365 6c65 6374 696f 6e20  -.    selection 
+00000b50: 3a20 4174 7472 6962 7574 6544 6963 7469  : AttributeDicti
+00000b60: 6f6e 6172 790a 2020 2020 2020 2020 5468  onary.        Th
+00000b70: 6520 7374 6174 6520 6f66 2074 6865 2060  e state of the `
+00000b80: 606f 6e5f 7365 6c65 6374 6060 2065 7665  `on_select`` eve
+00000b90: 6e74 2e20 5468 6520 6e61 6d65 206f 6620  nt. The name of 
+00000ba0: 6561 6368 2073 656c 6563 7469 6f6e 0a20  each selection. 
+00000bb0: 2020 2020 2020 2070 6172 616d 6574 6572         parameter
+00000bc0: 2062 6563 6f6d 6573 2061 6e20 6174 7472   becomes an attr
+00000bd0: 6962 7574 6520 696e 2074 6865 2060 6073  ibute in the ``s
+00000be0: 656c 6563 7469 6f6e 6060 2061 7474 7269  election`` attri
+00000bf0: 6275 7465 0a20 2020 2020 2020 2064 6963  bute.        dic
+00000c00: 7469 6f6e 6172 792e 2054 6865 2066 6f72  tionary. The for
+00000c10: 6d61 7420 6f66 2074 6865 2064 6174 6120  mat of the data 
+00000c20: 7769 7468 696e 2065 6163 6820 6174 7472  within each attr
+00000c30: 6962 7574 6520 6973 2064 6574 6572 6d69  ibute is determi
+00000c40: 6e65 640a 2020 2020 2020 2020 6279 2074  ned.        by t
+00000c50: 6865 2073 656c 6563 7469 6f6e 2070 6172  he selection par
+00000c60: 616d 6574 6572 2064 6566 696e 6974 696f  ameter definitio
+00000c70: 6e20 7769 7468 696e 2056 6567 612d 4c69  n within Vega-Li
+00000c80: 7465 2e0a 0a20 2020 2045 7861 6d70 6c65  te...    Example
+00000c90: 730a 2020 2020 2d2d 2d2d 2d2d 2d2d 0a20  s.    --------. 
+00000ca0: 2020 2054 6865 2066 6f6c 6c6f 7769 6e67     The following
+00000cb0: 2074 776f 2065 7861 6d70 6c65 7320 6861   two examples ha
+00000cc0: 7665 2065 7175 6976 616c 656e 7420 6465  ve equivalent de
+00000cd0: 6669 6e69 7469 6f6e 732e 2045 6163 6820  finitions. Each 
+00000ce0: 6f6e 6520 6861 7320 610a 2020 2020 706f  one has a.    po
+00000cf0: 696e 7420 616e 6420 696e 7465 7276 616c  int and interval
+00000d00: 2073 656c 6563 7469 6f6e 2070 6172 616d   selection param
+00000d10: 6574 6572 2069 6e63 6c75 6465 2069 6e20  eter include in 
+00000d20: 7468 6520 6368 6172 7420 6465 6669 6e69  the chart defini
+00000d30: 7469 6f6e 2e0a 2020 2020 5468 6520 706f  tion..    The po
+00000d40: 696e 7420 7365 6c65 6369 746f 6e20 7061  int seleciton pa
+00000d50: 7261 6d65 7465 7220 6973 206e 616d 6564  rameter is named
+00000d60: 2060 6022 706f 696e 745f 7365 6c65 6374   ``"point_select
+00000d70: 696f 6e22 6060 2e20 5468 6520 696e 7465  ion"``. The inte
+00000d80: 7276 616c 0a20 2020 206f 7220 626f 7820  rval.    or box 
+00000d90: 7365 6c65 6374 696f 6e20 7061 7261 6d65  selection parame
+00000da0: 7465 7220 6973 206e 616d 6564 2060 6022  ter is named ``"
+00000db0: 696e 7465 7276 616c 5f73 656c 6563 7469  interval_selecti
+00000dc0: 6f6e 2260 602e 0a0a 2020 2020 5468 6520  on"``...    The 
+00000dd0: 666f 6c6c 6f77 2065 7861 6d70 6c65 2075  follow example u
+00000de0: 7365 7320 6060 7374 2e61 6c74 6169 725f  ses ``st.altair_
+00000df0: 6368 6172 7460 603a 0a0a 2020 2020 3e3e  chart``:..    >>
+00000e00: 3e20 696d 706f 7274 2073 7472 6561 6d6c  > import streaml
+00000e10: 6974 2061 7320 7374 0a20 2020 203e 3e3e  it as st.    >>>
+00000e20: 2069 6d70 6f72 7420 7061 6e64 6173 2061   import pandas a
+00000e30: 7320 7064 0a20 2020 203e 3e3e 2069 6d70  s pd.    >>> imp
+00000e40: 6f72 7420 6e75 6d70 7920 6173 206e 700a  ort numpy as np.
+00000e50: 2020 2020 3e3e 3e20 696d 706f 7274 2061      >>> import a
+00000e60: 6c74 6169 7220 6173 2061 6c74 0a20 2020  ltair as alt.   
+00000e70: 203e 3e3e 0a20 2020 203e 3e3e 2069 6620   >>>.    >>> if 
+00000e80: 2264 6174 6122 206e 6f74 2069 6e20 7374  "data" not in st
+00000e90: 2e73 6573 7369 6f6e 5f73 7461 7465 3a0a  .session_state:.
+00000ea0: 2020 2020 3e3e 3e20 2020 2020 7374 2e73      >>>     st.s
+00000eb0: 6573 7369 6f6e 5f73 7461 7465 2e64 6174  ession_state.dat
+00000ec0: 6120 3d20 7064 2e44 6174 6146 7261 6d65  a = pd.DataFrame
+00000ed0: 280a 2020 2020 2e2e 2e20 2020 2020 2020  (.    ...       
+00000ee0: 2020 6e70 2e72 616e 646f 6d2e 7261 6e64    np.random.rand
+00000ef0: 6e28 3230 2c20 3329 2c20 636f 6c75 6d6e  n(20, 3), column
+00000f00: 733d 5b22 6122 2c20 2262 222c 2022 6322  s=["a", "b", "c"
+00000f10: 5d0a 2020 2020 2e2e 2e20 2020 2020 290a  ].    ...     ).
+00000f20: 2020 2020 3e3e 3e20 6466 203d 2073 742e      >>> df = st.
+00000f30: 7365 7373 696f 6e5f 7374 6174 652e 6461  session_state.da
+00000f40: 7461 0a20 2020 203e 3e3e 0a20 2020 203e  ta.    >>>.    >
+00000f50: 3e3e 2070 6f69 6e74 5f73 656c 6563 746f  >> point_selecto
+00000f60: 7220 3d20 616c 742e 7365 6c65 6374 696f  r = alt.selectio
+00000f70: 6e5f 706f 696e 7428 2270 6f69 6e74 5f73  n_point("point_s
+00000f80: 656c 6563 7469 6f6e 2229 0a20 2020 203e  election").    >
+00000f90: 3e3e 2069 6e74 6572 7661 6c5f 7365 6c65  >> interval_sele
+00000fa0: 6374 6f72 203d 2061 6c74 2e73 656c 6563  ctor = alt.selec
+00000fb0: 7469 6f6e 5f69 6e74 6572 7661 6c28 2269  tion_interval("i
+00000fc0: 6e74 6572 7661 6c5f 7365 6c65 6374 696f  nterval_selectio
+00000fd0: 6e22 290a 2020 2020 3e3e 3e20 6368 6172  n").    >>> char
+00000fe0: 7420 3d20 280a 2020 2020 2e2e 2e20 2020  t = (.    ...   
+00000ff0: 2020 616c 742e 4368 6172 7428 6466 290a    alt.Chart(df).
+00001000: 2020 2020 2e2e 2e20 2020 2020 2e6d 6172      ...     .mar
+00001010: 6b5f 6369 7263 6c65 2829 0a20 2020 202e  k_circle().    .
+00001020: 2e2e 2020 2020 202e 656e 636f 6465 280a  ..     .encode(.
+00001030: 2020 2020 2e2e 2e20 2020 2020 2020 2020      ...         
+00001040: 783d 2261 222c 0a20 2020 202e 2e2e 2020  x="a",.    ...  
+00001050: 2020 2020 2020 2079 3d22 6222 2c0a 2020         y="b",.  
+00001060: 2020 2e2e 2e20 2020 2020 2020 2020 7369    ...         si
+00001070: 7a65 3d22 6322 2c0a 2020 2020 2e2e 2e20  ze="c",.    ... 
+00001080: 2020 2020 2020 2020 636f 6c6f 723d 2263          color="c
+00001090: 222c 0a20 2020 202e 2e2e 2020 2020 2020  ",.    ...      
+000010a0: 2020 2074 6f6f 6c74 6970 3d5b 2261 222c     tooltip=["a",
+000010b0: 2022 6222 2c20 2263 225d 2c0a 2020 2020   "b", "c"],.    
+000010c0: 2e2e 2e20 2020 2020 2020 2020 6669 6c6c  ...         fill
+000010d0: 4f70 6163 6974 793d 616c 742e 636f 6e64  Opacity=alt.cond
+000010e0: 6974 696f 6e28 706f 696e 745f 7365 6c65  ition(point_sele
+000010f0: 6374 6f72 2c20 616c 742e 7661 6c75 6528  ctor, alt.value(
+00001100: 3129 2c20 616c 742e 7661 6c75 6528 302e  1), alt.value(0.
+00001110: 3329 292c 0a20 2020 202e 2e2e 2020 2020  3)),.    ...    
+00001120: 2029 0a20 2020 202e 2e2e 2020 2020 202e   ).    ...     .
+00001130: 6164 645f 7061 7261 6d73 2870 6f69 6e74  add_params(point
+00001140: 5f73 656c 6563 746f 722c 2069 6e74 6572  _selector, inter
+00001150: 7661 6c5f 7365 6c65 6374 6f72 290a 2020  val_selector).  
+00001160: 2020 2e2e 2e20 290a 2020 2020 3e3e 3e0a    ... ).    >>>.
+00001170: 2020 2020 3e3e 3e20 6576 656e 7420 3d20      >>> event = 
+00001180: 7374 2e61 6c74 6169 725f 6368 6172 7428  st.altair_chart(
+00001190: 6368 6172 742c 206b 6579 3d22 616c 745f  chart, key="alt_
+000011a0: 6368 6172 7422 2c20 6f6e 5f73 656c 6563  chart", on_selec
+000011b0: 743d 2272 6572 756e 2229 0a20 2020 203e  t="rerun").    >
+000011c0: 3e3e 0a20 2020 203e 3e3e 2065 7665 6e74  >>.    >>> event
+000011d0: 0a0a 2020 2020 5468 6520 666f 6c6c 6f77  ..    The follow
+000011e0: 696e 6720 6578 616d 706c 6520 7573 6573  ing example uses
+000011f0: 2060 6073 742e 7665 6761 5f6c 6974 655f   ``st.vega_lite_
+00001200: 6368 6172 7460 603a 0a0a 2020 2020 3e3e  chart``:..    >>
+00001210: 3e20 696d 706f 7274 2073 7472 6561 6d6c  > import streaml
+00001220: 6974 2061 7320 7374 0a20 2020 203e 3e3e  it as st.    >>>
+00001230: 2069 6d70 6f72 7420 7061 6e64 6173 2061   import pandas a
+00001240: 7320 7064 0a20 2020 203e 3e3e 2069 6d70  s pd.    >>> imp
+00001250: 6f72 7420 6e75 6d70 7920 6173 206e 700a  ort numpy as np.
+00001260: 2020 2020 3e3e 3e0a 2020 2020 3e3e 3e20      >>>.    >>> 
+00001270: 6966 2022 6461 7461 2220 6e6f 7420 696e  if "data" not in
+00001280: 2073 742e 7365 7373 696f 6e5f 7374 6174   st.session_stat
+00001290: 653a 0a20 2020 203e 3e3e 2020 2020 2073  e:.    >>>     s
+000012a0: 742e 7365 7373 696f 6e5f 7374 6174 652e  t.session_state.
+000012b0: 6461 7461 203d 2070 642e 4461 7461 4672  data = pd.DataFr
+000012c0: 616d 6528 0a20 2020 202e 2e2e 2020 2020  ame(.    ...    
+000012d0: 2020 2020 206e 702e 7261 6e64 6f6d 2e72       np.random.r
+000012e0: 616e 646e 2832 302c 2033 292c 2063 6f6c  andn(20, 3), col
+000012f0: 756d 6e73 3d5b 2261 222c 2022 6222 2c20  umns=["a", "b", 
+00001300: 2263 225d 0a20 2020 202e 2e2e 2020 2020  "c"].    ...    
+00001310: 2029 0a20 2020 203e 3e3e 0a20 2020 203e   ).    >>>.    >
+00001320: 3e3e 2073 7065 6320 3d20 7b0a 2020 2020  >> spec = {.    
+00001330: 2e2e 2e20 2020 2020 226d 6172 6b22 3a20  ...     "mark": 
+00001340: 7b22 7479 7065 223a 2022 6369 7263 6c65  {"type": "circle
+00001350: 222c 2022 746f 6f6c 7469 7022 3a20 5472  ", "tooltip": Tr
+00001360: 7565 7d2c 0a20 2020 202e 2e2e 2020 2020  ue},.    ...    
+00001370: 2022 7061 7261 6d73 223a 205b 0a20 2020   "params": [.   
+00001380: 202e 2e2e 2020 2020 2020 2020 207b 226e   ...         {"n
+00001390: 616d 6522 3a20 2269 6e74 6572 7661 6c5f  ame": "interval_
+000013a0: 7365 6c65 6374 696f 6e22 2c20 2273 656c  selection", "sel
+000013b0: 6563 7422 3a20 2269 6e74 6572 7661 6c22  ect": "interval"
+000013c0: 7d2c 0a20 2020 202e 2e2e 2020 2020 2020  },.    ...      
+000013d0: 2020 207b 226e 616d 6522 3a20 2270 6f69     {"name": "poi
+000013e0: 6e74 5f73 656c 6563 7469 6f6e 222c 2022  nt_selection", "
+000013f0: 7365 6c65 6374 223a 2022 706f 696e 7422  select": "point"
+00001400: 7d2c 0a20 2020 202e 2e2e 2020 2020 205d  },.    ...     ]
+00001410: 2c0a 2020 2020 2e2e 2e20 2020 2020 2265  ,.    ...     "e
+00001420: 6e63 6f64 696e 6722 3a20 7b0a 2020 2020  ncoding": {.    
+00001430: 2e2e 2e20 2020 2020 2020 2020 2278 223a  ...         "x":
+00001440: 207b 2266 6965 6c64 223a 2022 6122 2c20   {"field": "a", 
+00001450: 2274 7970 6522 3a20 2271 7561 6e74 6974  "type": "quantit
+00001460: 6174 6976 6522 7d2c 0a20 2020 202e 2e2e  ative"},.    ...
+00001470: 2020 2020 2020 2020 2022 7922 3a20 7b22           "y": {"
+00001480: 6669 656c 6422 3a20 2262 222c 2022 7479  field": "b", "ty
+00001490: 7065 223a 2022 7175 616e 7469 7461 7469  pe": "quantitati
+000014a0: 7665 227d 2c0a 2020 2020 2e2e 2e20 2020  ve"},.    ...   
+000014b0: 2020 2020 2020 2273 697a 6522 3a20 7b22        "size": {"
+000014c0: 6669 656c 6422 3a20 2263 222c 2022 7479  field": "c", "ty
+000014d0: 7065 223a 2022 7175 616e 7469 7461 7469  pe": "quantitati
+000014e0: 7665 227d 2c0a 2020 2020 2e2e 2e20 2020  ve"},.    ...   
+000014f0: 2020 2020 2020 2263 6f6c 6f72 223a 207b        "color": {
+00001500: 2266 6965 6c64 223a 2022 6322 2c20 2274  "field": "c", "t
+00001510: 7970 6522 3a20 2271 7561 6e74 6974 6174  ype": "quantitat
+00001520: 6976 6522 7d2c 0a20 2020 202e 2e2e 2020  ive"},.    ...  
+00001530: 2020 2020 2020 2022 6669 6c6c 4f70 6163         "fillOpac
+00001540: 6974 7922 3a20 7b0a 2020 2020 2e2e 2e20  ity": {.    ... 
+00001550: 2020 2020 2020 2020 2020 2020 2263 6f6e              "con
+00001560: 6469 7469 6f6e 223a 207b 2270 6172 616d  dition": {"param
+00001570: 223a 2022 706f 696e 745f 7365 6c65 6374  ": "point_select
+00001580: 696f 6e22 2c20 2276 616c 7565 223a 2031  ion", "value": 1
+00001590: 7d2c 0a20 2020 202e 2e2e 2020 2020 2020  },.    ...      
+000015a0: 2020 2020 2020 2022 7661 6c75 6522 3a20         "value": 
+000015b0: 302e 332c 0a20 2020 202e 2e2e 2020 2020  0.3,.    ...    
+000015c0: 2020 2020 207d 2c0a 2020 2020 2e2e 2e20       },.    ... 
+000015d0: 2020 2020 7d2c 0a20 2020 202e 2e2e 207d      },.    ... }
+000015e0: 0a20 2020 203e 3e3e 0a20 2020 203e 3e3e  .    >>>.    >>>
+000015f0: 2065 7665 6e74 203d 2073 742e 7665 6761   event = st.vega
+00001600: 5f6c 6974 655f 6368 6172 7428 7374 2e73  _lite_chart(st.s
+00001610: 6573 7369 6f6e 5f73 7461 7465 2e64 6174  ession_state.dat
+00001620: 612c 2073 7065 632c 206b 6579 3d22 7665  a, spec, key="ve
+00001630: 6761 5f63 6861 7274 222c 206f 6e5f 7365  ga_chart", on_se
+00001640: 6c65 6374 3d22 7265 7275 6e22 290a 2020  lect="rerun").  
+00001650: 2020 3e3e 3e0a 2020 2020 3e3e 3e20 6576    >>>.    >>> ev
+00001660: 656e 740a 0a20 2020 2054 7279 2073 656c  ent..    Try sel
+00001670: 6563 7469 6e67 2070 6f69 6e74 7320 696e  ecting points in
+00001680: 2074 6869 7320 696e 7465 7261 6374 6976   this interactiv
+00001690: 6520 6578 616d 706c 652e 2057 6865 6e20  e example. When 
+000016a0: 796f 7520 636c 6963 6b20 6120 706f 696e  you click a poin
+000016b0: 742c 0a20 2020 2074 6865 2073 656c 6563  t,.    the selec
+000016c0: 7469 6f6e 2077 696c 6c20 6170 7065 6172  tion will appear
+000016d0: 2075 6e64 6572 2074 6865 2061 7474 7269   under the attri
+000016e0: 6275 7465 2c20 6060 2270 6f69 6e74 5f73  bute, ``"point_s
+000016f0: 656c 6563 7469 6f6e 2260 602c 2077 6869  election"``, whi
+00001700: 6368 0a20 2020 2069 7320 7468 6520 6e61  ch.    is the na
+00001710: 6d65 2067 6976 656e 2074 6f20 7468 6520  me given to the 
+00001720: 706f 696e 7420 7365 6c65 6374 696f 6e20  point selection 
+00001730: 7061 7261 6d65 7465 722e 2053 696d 696c  parameter. Simil
+00001740: 6172 6c79 2c20 7768 656e 2079 6f75 0a20  arly, when you. 
+00001750: 2020 206d 616b 6520 616e 2069 6e74 6572     make an inter
+00001760: 7661 6c20 7365 6c65 6374 696f 6e2c 2069  val selection, i
+00001770: 7420 7769 6c6c 2061 7070 6561 7220 756e  t will appear un
+00001780: 6465 7220 7468 6520 6174 7472 6962 7574  der the attribut
+00001790: 650a 2020 2020 6060 2269 6e74 6572 7661  e.    ``"interva
+000017a0: 6c5f 7365 6c65 6374 696f 6e22 6060 2e20  l_selection"``. 
+000017b0: 596f 7520 6361 6e20 6769 7665 2079 6f75  You can give you
+000017c0: 7220 7365 6c65 6374 696f 6e20 7061 7261  r selection para
+000017d0: 6d65 7465 7273 206f 7468 6572 0a20 2020  meters other.   
+000017e0: 206e 616d 6573 2069 6620 6465 7369 7265   names if desire
+000017f0: 642e 0a0a 2020 2020 4966 2079 6f75 2068  d...    If you h
+00001800: 6f6c 6420 6060 5368 6966 7460 6020 7768  old ``Shift`` wh
+00001810: 696c 6520 7365 6c65 6374 696e 6720 706f  ile selecting po
+00001820: 696e 7473 2c20 6578 6973 7469 6e67 2070  ints, existing p
+00001830: 6f69 6e74 2073 656c 6563 7469 6f6e 730a  oint selections.
+00001840: 2020 2020 7769 6c6c 2062 6520 7072 6573      will be pres
+00001850: 6572 7665 642e 2049 6e74 6572 7661 6c20  erved. Interval 
+00001860: 7365 6c65 6374 696f 6e73 2061 7265 206e  selections are n
+00001870: 6f74 2070 7265 7365 7276 6564 2077 6865  ot preserved whe
+00001880: 6e20 6d61 6b69 6e67 0a20 2020 2061 6464  n making.    add
+00001890: 6974 696f 6e61 6c20 7365 6c65 6374 696f  itional selectio
+000018a0: 6e73 2e0a 0a20 2020 202e 2e20 6f75 7470  ns...    .. outp
+000018b0: 7574 3a3a 0a20 2020 2020 2020 2068 7474  ut::.        htt
+000018c0: 7073 3a2f 2f64 6f63 2d63 6861 7274 2d65  ps://doc-chart-e
+000018d0: 7665 6e74 732d 7665 6761 2d6c 6974 652d  vents-vega-lite-
+000018e0: 7374 6174 652e 7374 7265 616d 6c69 742e  state.streamlit.
+000018f0: 6170 700a 2020 2020 2020 2020 6865 6967  app.        heig
+00001900: 6874 3a20 3630 3070 780a 0a20 2020 2022  ht: 600px..    "
+00001910: 2222 0a0a 2020 2020 7365 6c65 6374 696f  ""..    selectio
+00001920: 6e3a 2041 7474 7269 6275 7465 4469 6374  n: AttributeDict
+00001930: 696f 6e61 7279 0a0a 0a40 6461 7461 636c  ionary...@datacl
+00001940: 6173 730a 636c 6173 7320 5665 6761 4c69  ass.class VegaLi
+00001950: 7465 5374 6174 6553 6572 6465 3a0a 2020  teStateSerde:.  
+00001960: 2020 2222 2256 6567 614c 6974 6553 7461    """VegaLiteSta
+00001970: 7465 5365 7264 6520 6973 2075 7365 6420  teSerde is used 
+00001980: 746f 2073 6572 6961 6c69 7a65 2061 6e64  to serialize and
+00001990: 2064 6573 6572 6961 6c69 7a65 2074 6865   deserialize the
+000019a0: 2056 6567 614c 6974 6520 4368 6172 7420   VegaLite Chart 
+000019b0: 7374 6174 652e 2222 220a 0a20 2020 2073  state."""..    s
+000019c0: 656c 6563 7469 6f6e 5f70 6172 616d 6574  election_paramet
+000019d0: 6572 733a 2053 6571 7565 6e63 655b 7374  ers: Sequence[st
+000019e0: 725d 0a0a 2020 2020 6465 6620 6465 7365  r]..    def dese
+000019f0: 7269 616c 697a 6528 7365 6c66 2c20 7569  rialize(self, ui
+00001a00: 5f76 616c 7565 3a20 7374 7220 7c20 4e6f  _value: str | No
+00001a10: 6e65 2c20 7769 6467 6574 5f69 643a 2073  ne, widget_id: s
+00001a20: 7472 203d 2022 2229 202d 3e20 5665 6761  tr = "") -> Vega
+00001a30: 4c69 7465 5374 6174 653a 0a20 2020 2020  LiteState:.     
+00001a40: 2020 2065 6d70 7479 5f73 656c 6563 7469     empty_selecti
+00001a50: 6f6e 5f73 7461 7465 3a20 5665 6761 4c69  on_state: VegaLi
+00001a60: 7465 5374 6174 6520 3d20 7b0a 2020 2020  teState = {.    
+00001a70: 2020 2020 2020 2020 2273 656c 6563 7469          "selecti
+00001a80: 6f6e 223a 2041 7474 7269 6275 7465 4469  on": AttributeDi
+00001a90: 6374 696f 6e61 7279 280a 2020 2020 2020  ctionary(.      
+00001aa0: 2020 2020 2020 2020 2020 2320 496e 6974            # Init
+00001ab0: 6961 6c69 7a65 2074 6865 2073 656c 6563  ialize the selec
+00001ac0: 7420 7374 6174 6520 7769 7468 2065 6d70  t state with emp
+00001ad0: 7479 2064 6963 7469 6f6e 6172 6965 7320  ty dictionaries 
+00001ae0: 666f 7220 6561 6368 2073 656c 6563 7469  for each selecti
+00001af0: 6f6e 2070 6172 616d 6574 6572 2e0a 2020  on parameter..  
+00001b00: 2020 2020 2020 2020 2020 2020 2020 7b70                {p
+00001b10: 6172 616d 3a20 7b7d 2066 6f72 2070 6172  aram: {} for par
+00001b20: 616d 2069 6e20 7365 6c66 2e73 656c 6563  am in self.selec
+00001b30: 7469 6f6e 5f70 6172 616d 6574 6572 737d  tion_parameters}
+00001b40: 0a20 2020 2020 2020 2020 2020 2029 2c0a  .            ),.
+00001b50: 2020 2020 2020 2020 7d0a 0a20 2020 2020          }..     
+00001b60: 2020 2073 656c 6563 7469 6f6e 5f73 7461     selection_sta
+00001b70: 7465 203d 2028 0a20 2020 2020 2020 2020  te = (.         
+00001b80: 2020 2065 6d70 7479 5f73 656c 6563 7469     empty_selecti
+00001b90: 6f6e 5f73 7461 7465 0a20 2020 2020 2020  on_state.       
+00001ba0: 2020 2020 2069 6620 7569 5f76 616c 7565       if ui_value
+00001bb0: 2069 7320 4e6f 6e65 0a20 2020 2020 2020   is None.       
+00001bc0: 2020 2020 2065 6c73 6520 6361 7374 2856       else cast(V
+00001bd0: 6567 614c 6974 6553 7461 7465 2c20 4174  egaLiteState, At
+00001be0: 7472 6962 7574 6544 6963 7469 6f6e 6172  tributeDictionar
+00001bf0: 7928 6a73 6f6e 2e6c 6f61 6473 2875 695f  y(json.loads(ui_
+00001c00: 7661 6c75 6529 2929 0a20 2020 2020 2020  value))).       
+00001c10: 2029 0a0a 2020 2020 2020 2020 6966 2022   )..        if "
+00001c20: 7365 6c65 6374 696f 6e22 206e 6f74 2069  selection" not i
+00001c30: 6e20 7365 6c65 6374 696f 6e5f 7374 6174  n selection_stat
+00001c40: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+00001c50: 656c 6563 7469 6f6e 5f73 7461 7465 203d  election_state =
+00001c60: 2065 6d70 7479 5f73 656c 6563 7469 6f6e   empty_selection
+00001c70: 5f73 7461 7465 0a0a 2020 2020 2020 2020  _state..        
+00001c80: 7265 7475 726e 2063 6173 7428 5665 6761  return cast(Vega
+00001c90: 4c69 7465 5374 6174 652c 2041 7474 7269  LiteState, Attri
+00001ca0: 6275 7465 4469 6374 696f 6e61 7279 2873  buteDictionary(s
+00001cb0: 656c 6563 7469 6f6e 5f73 7461 7465 2929  election_state))
+00001cc0: 0a0a 2020 2020 6465 6620 7365 7269 616c  ..    def serial
+00001cd0: 697a 6528 7365 6c66 2c20 7365 6c65 6374  ize(self, select
+00001ce0: 696f 6e5f 7374 6174 653a 2056 6567 614c  ion_state: VegaL
+00001cf0: 6974 6553 7461 7465 2920 2d3e 2073 7472  iteState) -> str
+00001d00: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+00001d10: 206a 736f 6e2e 6475 6d70 7328 7365 6c65   json.dumps(sele
+00001d20: 6374 696f 6e5f 7374 6174 652c 2064 6566  ction_state, def
+00001d30: 6175 6c74 3d73 7472 290a 0a0a 6465 6620  ault=str)...def 
+00001d40: 5f70 7265 7061 7265 5f76 6567 615f 6c69  _prepare_vega_li
+00001d50: 7465 5f73 7065 6328 0a20 2020 2073 7065  te_spec(.    spe
+00001d60: 633a 2056 6567 614c 6974 6553 7065 632c  c: VegaLiteSpec,
+00001d70: 0a20 2020 2075 7365 5f63 6f6e 7461 696e  .    use_contain
+00001d80: 6572 5f77 6964 7468 3a20 626f 6f6c 203d  er_width: bool =
+00001d90: 2046 616c 7365 2c0a 2020 2020 2a2a 6b77   False,.    **kw
+00001da0: 6172 6773 2c0a 2920 2d3e 2056 6567 614c  args,.) -> VegaL
+00001db0: 6974 6553 7065 633a 0a20 2020 2069 6620  iteSpec:.    if 
+00001dc0: 6c65 6e28 6b77 6172 6773 293a 0a20 2020  len(kwargs):.   
+00001dd0: 2020 2020 2023 2053 7570 706f 7274 2070       # Support p
+00001de0: 6173 7369 6e67 2069 6e20 6b77 6172 6773  assing in kwargs
+00001df0: 2e20 4578 616d 706c 653a 0a20 2020 2020  . Example:.     
+00001e00: 2020 2023 2020 206d 6172 7368 616c 6c28     #   marshall(
+00001e10: 7072 6f74 6f2c 207b 666f 6f3a 2027 6261  proto, {foo: 'ba
+00001e20: 7227 7d2c 2062 617a 3d27 626f 7a27 290a  r'}, baz='boz').
+00001e30: 2020 2020 2020 2020 2320 4d65 7267 6520          # Merge 
+00001e40: 7370 6563 2077 6974 6820 756e 666c 6174  spec with unflat
+00001e50: 7465 6e65 6420 6b77 6172 6773 2c20 7768  tened kwargs, wh
+00001e60: 6572 6520 6b77 6172 6773 2074 616b 6520  ere kwargs take 
+00001e70: 7072 6563 6564 656e 6365 2e0a 2020 2020  precedence..    
+00001e80: 2020 2020 2320 5468 6973 206f 6e6c 7920      # This only 
+00001e90: 776f 726b 7320 666f 7220 7374 7269 6e67  works for string
+00001ea0: 206b 6579 732c 2062 7574 206b 7761 7267   keys, but kwarg
+00001eb0: 206b 6579 7320 6172 6520 7374 7269 6e67   keys are string
+00001ec0: 7320 616e 7977 6179 732e 0a20 2020 2020  s anyways..     
+00001ed0: 2020 2073 7065 6320 3d20 6469 6374 2873     spec = dict(s
+00001ee0: 7065 632c 202a 2a64 6963 7474 6f6f 6c73  pec, **dicttools
+00001ef0: 2e75 6e66 6c61 7474 656e 286b 7761 7267  .unflatten(kwarg
+00001f00: 732c 205f 4348 414e 4e45 4c53 2929 0a20  s, _CHANNELS)). 
+00001f10: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00001f20: 2023 2043 6c6f 6e65 2074 6865 2073 7065   # Clone the spe
+00001f30: 6320 6469 6374 2c20 7369 6e63 6520 7765  c dict, since we
+00001f40: 206d 6179 2062 6520 6d75 7461 7469 6e67   may be mutating
+00001f50: 2069 742e 0a20 2020 2020 2020 2073 7065   it..        spe
+00001f60: 6320 3d20 6469 6374 2873 7065 6329 0a0a  c = dict(spec)..
+00001f70: 2020 2020 6966 206c 656e 2873 7065 6329      if len(spec)
+00001f80: 203d 3d20 303a 0a20 2020 2020 2020 2072   == 0:.        r
+00001f90: 6169 7365 2053 7472 6561 6d6c 6974 4150  aise StreamlitAP
+00001fa0: 4945 7863 6570 7469 6f6e 2822 5665 6761  IException("Vega
+00001fb0: 2d4c 6974 6520 6368 6172 7473 2072 6571  -Lite charts req
+00001fc0: 7569 7265 2061 206e 6f6e 2d65 6d70 7479  uire a non-empty
+00001fd0: 2073 7065 6320 6469 6374 2e22 290a 0a20   spec dict.").. 
+00001fe0: 2020 2069 6620 2261 7574 6f73 697a 6522     if "autosize"
+00001ff0: 206e 6f74 2069 6e20 7370 6563 3a0a 2020   not in spec:.  
+00002000: 2020 2020 2020 2320 7479 7065 2066 6974        # type fit
+00002010: 2064 6f65 7320 6e6f 7420 776f 726b 2066   does not work f
+00002020: 6f72 206d 616e 7920 6368 6172 7420 7479  or many chart ty
+00002030: 7065 732e 2054 6869 7320 6368 616e 6765  pes. This change
+00002040: 2066 6f63 7573 6573 0a20 2020 2020 2020   focuses.       
+00002050: 2023 206f 6e20 7663 6f6e 6361 7420 7769   # on vconcat wi
+00002060: 7468 2075 7365 5f63 6f6e 7461 696e 6572  th use_container
+00002070: 5f77 6964 7468 3d54 7275 6520 6173 2074  _width=True as t
+00002080: 6865 7265 2061 7265 2075 6e69 6e74 656e  here are uninten
+00002090: 6465 640a 2020 2020 2020 2020 2320 636f  ded.        # co
+000020a0: 6e73 6571 7565 6e63 6573 206f 6620 6368  nsequences of ch
+000020b0: 616e 6769 6e67 2074 6865 2064 6566 6175  anging the defau
+000020c0: 6c74 2061 7574 6f73 697a 6520 666f 7220  lt autosize for 
+000020d0: 616c 6c20 6368 6172 7473 2e0a 2020 2020  all charts..    
+000020e0: 2020 2020 2320 6669 742d 7820 6669 7473      # fit-x fits
+000020f0: 2074 6865 2077 6964 7468 2061 6e64 2068   the width and h
+00002100: 6569 6768 7420 6361 6e20 6265 2061 646a  eight can be adj
+00002110: 7573 7465 642e 0a20 2020 2020 2020 2069  usted..        i
+00002120: 6620 2276 636f 6e63 6174 2220 696e 2073  f "vconcat" in s
+00002130: 7065 6320 616e 6420 7573 655f 636f 6e74  pec and use_cont
+00002140: 6169 6e65 725f 7769 6474 683a 0a20 2020  ainer_width:.   
+00002150: 2020 2020 2020 2020 2073 7065 635b 2261           spec["a
+00002160: 7574 6f73 697a 6522 5d20 3d20 7b22 7479  utosize"] = {"ty
+00002170: 7065 223a 2022 6669 742d 7822 2c20 2263  pe": "fit-x", "c
+00002180: 6f6e 7461 696e 7322 3a20 2270 6164 6469  ontains": "paddi
+00002190: 6e67 227d 0a20 2020 2020 2020 2065 6c73  ng"}.        els
+000021a0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+000021b0: 7065 635b 2261 7574 6f73 697a 6522 5d20  pec["autosize"] 
+000021c0: 3d20 7b22 7479 7065 223a 2022 6669 7422  = {"type": "fit"
+000021d0: 2c20 2263 6f6e 7461 696e 7322 3a20 2270  , "contains": "p
+000021e0: 6164 6469 6e67 227d 0a0a 2020 2020 7265  adding"}..    re
+000021f0: 7475 726e 2073 7065 630a 0a0a 6465 6620  turn spec...def 
+00002200: 5f73 6572 6961 6c69 7a65 5f64 6174 6128  _serialize_data(
+00002210: 6461 7461 3a20 416e 7929 202d 3e20 6279  data: Any) -> by
+00002220: 7465 733a 0a20 2020 2022 2222 5365 7269  tes:.    """Seri
+00002230: 616c 697a 6520 7468 6520 616e 7920 7479  alize the any ty
+00002240: 7065 206f 6620 6461 7461 2073 7472 7563  pe of data struc
+00002250: 7475 7265 2074 6f20 4172 726f 7720 4950  ture to Arrow IP
+00002260: 4320 666f 726d 6174 2028 6279 7465 7329  C format (bytes)
+00002270: 2e22 2222 0a20 2020 2069 6d70 6f72 7420  .""".    import 
+00002280: 7079 6172 726f 7720 6173 2070 610a 0a20  pyarrow as pa.. 
+00002290: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
+000022a0: 2864 6174 612c 2070 612e 5461 626c 6529  (data, pa.Table)
+000022b0: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+000022c0: 2074 7970 655f 7574 696c 2e70 7961 7272   type_util.pyarr
+000022d0: 6f77 5f74 6162 6c65 5f74 6f5f 6279 7465  ow_table_to_byte
+000022e0: 7328 6461 7461 290a 0a20 2020 2064 6620  s(data)..    df 
+000022f0: 3d20 7479 7065 5f75 7469 6c2e 636f 6e76  = type_util.conv
+00002300: 6572 745f 616e 7974 6869 6e67 5f74 6f5f  ert_anything_to_
+00002310: 6466 2864 6174 6129 0a20 2020 2072 6574  df(data).    ret
+00002320: 7572 6e20 7479 7065 5f75 7469 6c2e 6461  urn type_util.da
+00002330: 7461 5f66 7261 6d65 5f74 6f5f 6279 7465  ta_frame_to_byte
+00002340: 7328 6466 290a 0a0a 6465 6620 5f6d 6172  s(df)...def _mar
+00002350: 7368 616c 6c5f 6368 6172 745f 6461 7461  shall_chart_data
+00002360: 280a 2020 2020 7072 6f74 6f3a 2041 7272  (.    proto: Arr
+00002370: 6f77 5665 6761 4c69 7465 4368 6172 7450  owVegaLiteChartP
+00002380: 726f 746f 2c0a 2020 2020 7370 6563 3a20  roto,.    spec: 
+00002390: 5665 6761 4c69 7465 5370 6563 2c0a 2020  VegaLiteSpec,.  
+000023a0: 2020 6461 7461 3a20 4461 7461 203d 204e    data: Data = N
+000023b0: 6f6e 652c 0a29 202d 3e20 4e6f 6e65 3a0a  one,.) -> None:.
+000023c0: 2020 2020 2222 2241 6464 7320 7468 6520      """Adds the 
+000023d0: 6461 7461 2074 6f20 7468 6520 7072 6f74  data to the prot
+000023e0: 6f20 616e 6420 7265 6d6f 7665 7320 6974  o and removes it
+000023f0: 2066 726f 6d20 7468 6520 7370 6563 2064   from the spec d
+00002400: 6963 742e 0a20 2020 2054 6865 7365 206f  ict..    These o
+00002410: 7065 7261 7469 6f6e 7320 7769 6c6c 2068  perations will h
+00002420: 6170 7065 6e20 696e 2d70 6c61 6365 2e22  appen in-place."
+00002430: 2222 0a0a 2020 2020 2320 5075 6c6c 2064  ""..    # Pull d
+00002440: 6174 6120 6f75 7420 6f66 2073 7065 6320  ata out of spec 
+00002450: 6469 6374 2077 6865 6e20 6974 2773 2069  dict when it's i
+00002460: 6e20 6120 2764 6174 6173 6574 7327 206b  n a 'datasets' k
+00002470: 6579 3a0a 2020 2020 2320 2020 6461 7461  ey:.    #   data
+00002480: 7365 7473 3a20 7b66 6f6f 3a20 6466 315f  sets: {foo: df1_
+00002490: 6279 7465 732c 2062 6172 3a20 6466 325f  bytes, bar: df2_
+000024a0: 6279 7465 737d 2c20 2e2e 2e7d 0a20 2020  bytes}, ...}.   
+000024b0: 2069 6620 2264 6174 6173 6574 7322 2069   if "datasets" i
+000024c0: 6e20 7370 6563 3a0a 2020 2020 2020 2020  n spec:.        
+000024d0: 666f 7220 6461 7461 7365 745f 6e61 6d65  for dataset_name
+000024e0: 2c20 6461 7461 7365 745f 6461 7461 2069  , dataset_data i
+000024f0: 6e20 7370 6563 5b22 6461 7461 7365 7473  n spec["datasets
+00002500: 225d 2e69 7465 6d73 2829 3a0a 2020 2020  "].items():.    
+00002510: 2020 2020 2020 2020 6461 7461 7365 7420          dataset 
+00002520: 3d20 7072 6f74 6f2e 6461 7461 7365 7473  = proto.datasets
+00002530: 2e61 6464 2829 0a20 2020 2020 2020 2020  .add().         
+00002540: 2020 2064 6174 6173 6574 2e6e 616d 6520     dataset.name 
+00002550: 3d20 7374 7228 6461 7461 7365 745f 6e61  = str(dataset_na
+00002560: 6d65 290a 2020 2020 2020 2020 2020 2020  me).            
+00002570: 6461 7461 7365 742e 6861 735f 6e61 6d65  dataset.has_name
+00002580: 203d 2054 7275 650a 2020 2020 2020 2020   = True.        
+00002590: 2020 2020 2320 5468 6520 4944 2074 7261      # The ID tra
+000025a0: 6e73 666f 726d 6572 2028 6964 5f74 7261  nsformer (id_tra
+000025b0: 6e73 666f 726d 2066 756e 6374 696f 6e20  nsform function 
+000025c0: 7265 6769 7374 6572 6564 2062 6566 6f72  registered befor
+000025d0: 6520 636f 6e76 6572 7369 6f6e 2074 6f20  e conversion to 
+000025e0: 6469 6374 290a 2020 2020 2020 2020 2020  dict).          
+000025f0: 2020 2320 616c 7265 6164 7920 7365 7269    # already seri
+00002600: 616c 697a 6573 2074 6865 2064 6174 6120  alizes the data 
+00002610: 696e 746f 2041 7272 6f77 2049 5043 2066  into Arrow IPC f
+00002620: 6f72 6d61 7420 2862 7974 6573 2920 7768  ormat (bytes) wh
+00002630: 656e 2074 6865 2041 6c74 6169 7220 6f62  en the Altair ob
+00002640: 6a65 6374 0a20 2020 2020 2020 2020 2020  ject.           
+00002650: 2023 2067 6574 7320 636f 6e76 6572 7465   # gets converte
+00002660: 6420 696e 746f 2074 6865 2076 6567 612d  d into the vega-
+00002670: 6c69 7465 2073 7065 6320 6469 6374 2e0a  lite spec dict..
+00002680: 2020 2020 2020 2020 2020 2020 2320 4966              # If
+00002690: 2069 7473 2061 6c72 6561 6479 2069 6e20   its already in 
+000026a0: 6279 7465 732c 2077 6520 646f 6e27 7420  bytes, we don't 
+000026b0: 6e65 6564 2074 6f20 7365 7269 616c 697a  need to serializ
+000026c0: 6520 6974 2068 6572 6520 6167 6169 6e2e  e it here again.
+000026d0: 0a20 2020 2020 2020 2020 2020 2023 2057  .            # W
+000026e0: 6520 6a75 7374 206e 6565 6420 746f 2070  e just need to p
+000026f0: 6173 7320 7468 6520 6461 7461 2069 6e66  ass the data inf
+00002700: 6f72 6d61 7469 6f6e 2069 6e74 6f20 7468  ormation into th
+00002710: 6520 636f 7272 6563 7420 7072 6f74 6f20  e correct proto 
+00002720: 6669 656c 6473 2e0a 0a20 2020 2020 2020  fields...       
+00002730: 2020 2020 2023 2054 4f44 4f28 6c75 6b61       # TODO(luka
+00002740: 736d 6173 7563 6829 3a20 4172 6520 7468  smasuch): Are th
+00002750: 6572 6520 616e 7920 6f74 6865 7220 6361  ere any other ca
+00002760: 7365 7320 7768 6572 6520 7765 206e 6565  ses where we nee
+00002770: 6420 746f 2073 6572 6961 6c69 7a65 2074  d to serialize t
+00002780: 6865 2064 6174 610a 2020 2020 2020 2020  he data.        
+00002790: 2020 2020 2320 2020 2020 2020 2020 2020      #           
+000027a0: 2020 2020 2020 2020 206f 7220 6361 6e20           or can 
+000027b0: 7765 2072 656d 6f76 6520 7468 6520 5f73  we remove the _s
+000027c0: 6572 6961 6c69 7a65 5f64 6174 6120 6865  erialize_data he
+000027d0: 7265 3f0a 2020 2020 2020 2020 2020 2020  re?.            
+000027e0: 6461 7461 7365 742e 6461 7461 2e64 6174  dataset.data.dat
+000027f0: 6120 3d20 280a 2020 2020 2020 2020 2020  a = (.          
+00002800: 2020 2020 2020 6461 7461 7365 745f 6461        dataset_da
+00002810: 7461 0a20 2020 2020 2020 2020 2020 2020  ta.             
+00002820: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
+00002830: 2864 6174 6173 6574 5f64 6174 612c 2062  (dataset_data, b
+00002840: 7974 6573 290a 2020 2020 2020 2020 2020  ytes).          
+00002850: 2020 2020 2020 656c 7365 205f 7365 7269        else _seri
+00002860: 616c 697a 655f 6461 7461 2864 6174 6173  alize_data(datas
+00002870: 6574 5f64 6174 6129 0a20 2020 2020 2020  et_data).       
+00002880: 2020 2020 2029 0a20 2020 2020 2020 2064       ).        d
+00002890: 656c 2073 7065 635b 2264 6174 6173 6574  el spec["dataset
+000028a0: 7322 5d0a 0a20 2020 2023 2050 756c 6c20  s"]..    # Pull 
+000028b0: 6461 7461 206f 7574 206f 6620 7370 6563  data out of spec
+000028c0: 2064 6963 7420 7768 656e 2069 7427 7320   dict when it's 
+000028d0: 696e 2061 2074 6f70 2d6c 6576 656c 2027  in a top-level '
+000028e0: 6461 7461 2720 6b65 793a 0a20 2020 2023  data' key:.    #
+000028f0: 2020 207b 6461 7461 3a20 6466 7d0a 2020     {data: df}.  
+00002900: 2020 2320 2020 7b64 6174 613a 207b 7661    #   {data: {va
+00002910: 6c75 6573 3a20 6466 2c20 2e2e 2e7d 7d0a  lues: df, ...}}.
+00002920: 2020 2020 2320 2020 7b64 6174 613a 207b      #   {data: {
+00002930: 7572 6c3a 2027 7572 6c27 7d7d 0a20 2020  url: 'url'}}.   
+00002940: 2023 2020 207b 6461 7461 3a20 7b6e 616d   #   {data: {nam
+00002950: 653a 2027 666f 6f27 7d7d 0a20 2020 2069  e: 'foo'}}.    i
+00002960: 6620 2264 6174 6122 2069 6e20 7370 6563  f "data" in spec
+00002970: 3a0a 2020 2020 2020 2020 6461 7461 5f73  :.        data_s
+00002980: 7065 6320 3d20 7370 6563 5b22 6461 7461  pec = spec["data
+00002990: 225d 0a0a 2020 2020 2020 2020 6966 2069  "]..        if i
+000029a0: 7369 6e73 7461 6e63 6528 6461 7461 5f73  sinstance(data_s
+000029b0: 7065 632c 2064 6963 7429 3a0a 2020 2020  pec, dict):.    
+000029c0: 2020 2020 2020 2020 6966 2022 7661 6c75          if "valu
+000029d0: 6573 2220 696e 2064 6174 615f 7370 6563  es" in data_spec
+000029e0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000029f0: 2020 6461 7461 203d 2064 6174 615f 7370    data = data_sp
+00002a00: 6563 5b22 7661 6c75 6573 225d 0a20 2020  ec["values"].   
+00002a10: 2020 2020 2020 2020 2020 2020 2064 656c               del
+00002a20: 2073 7065 635b 2264 6174 6122 5d0a 2020   spec["data"].  
+00002a30: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00002a40: 2020 2020 2020 2020 6461 7461 203d 2064          data = d
+00002a50: 6174 615f 7370 6563 0a20 2020 2020 2020  ata_spec.       
+00002a60: 2020 2020 2064 656c 2073 7065 635b 2264       del spec["d
+00002a70: 6174 6122 5d0a 0a20 2020 2069 6620 6461  ata"]..    if da
+00002a80: 7461 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ta is not None:.
+00002a90: 2020 2020 2020 2020 7072 6f74 6f2e 6461          proto.da
+00002aa0: 7461 2e64 6174 6120 3d20 5f73 6572 6961  ta.data = _seria
+00002ab0: 6c69 7a65 5f64 6174 6128 6461 7461 290a  lize_data(data).
+00002ac0: 0a0a 6465 6620 5f63 6f6e 7665 7274 5f61  ..def _convert_a
+00002ad0: 6c74 6169 725f 746f 5f76 6567 615f 6c69  ltair_to_vega_li
+00002ae0: 7465 5f73 7065 6328 616c 7461 6972 5f63  te_spec(altair_c
+00002af0: 6861 7274 3a20 616c 742e 4368 6172 7429  hart: alt.Chart)
+00002b00: 202d 3e20 5665 6761 4c69 7465 5370 6563   -> VegaLiteSpec
+00002b10: 3a0a 2020 2020 2222 2243 6f6e 7665 7274  :.    """Convert
+00002b20: 2061 6e20 416c 7461 6972 2063 6861 7274   an Altair chart
+00002b30: 206f 626a 6563 7420 746f 2061 2056 6567   object to a Veg
+00002b40: 612d 4c69 7465 2063 6861 7274 2073 7065  a-Lite chart spe
+00002b50: 632e 2222 220a 2020 2020 696d 706f 7274  c.""".    import
+00002b60: 2061 6c74 6169 7220 6173 2061 6c74 0a0a   altair as alt..
+00002b70: 2020 2020 2320 4e6f 726d 616c 6c79 2061      # Normally a
+00002b80: 6c74 6169 725f 6368 6172 742e 746f 5f64  ltair_chart.to_d
+00002b90: 6963 7428 2920 776f 756c 6420 7472 616e  ict() would tran
+00002ba0: 7366 6f72 6d20 7468 6520 6461 7461 6672  sform the datafr
+00002bb0: 616d 6520 7573 6564 2062 7920 7468 650a  ame used by the.
+00002bc0: 2020 2020 2320 6368 6172 7420 696e 746f      # chart into
+00002bd0: 2061 6e20 6172 7261 7920 6f66 2064 6963   an array of dic
+00002be0: 7469 6f6e 6172 6965 732e 2054 6f20 6176  tionaries. To av
+00002bf0: 6f69 6420 7468 6174 2c20 7765 2069 6e73  oid that, we ins
+00002c00: 7461 6c6c 2061 0a20 2020 2023 2074 7261  tall a.    # tra
+00002c10: 6e73 666f 726d 6572 2074 6861 7420 7265  nsformer that re
+00002c20: 706c 6163 6573 2064 6174 6173 6574 7320  places datasets 
+00002c30: 7769 7468 2061 2072 6566 6572 656e 6365  with a reference
+00002c40: 2062 7920 7468 6520 6f62 6a65 6374 2069   by the object i
+00002c50: 6420 6f66 0a20 2020 2023 2074 6865 2064  d of.    # the d
+00002c60: 6174 6166 7261 6d65 2e20 5765 2074 6865  ataframe. We the
+00002c70: 6e20 6669 6c6c 2069 6e20 7468 6520 6461  n fill in the da
+00002c80: 7461 7365 7420 6d61 6e75 616c 6c79 206c  taset manually l
+00002c90: 6174 6572 206f 6e2e 0a0a 2020 2020 6461  ater on...    da
+00002ca0: 7461 7365 7473 203d 207b 7d0a 0a20 2020  tasets = {}..   
+00002cb0: 2064 6566 2069 645f 7472 616e 7366 6f72   def id_transfor
+00002cc0: 6d28 6461 7461 2920 2d3e 2064 6963 745b  m(data) -> dict[
+00002cd0: 7374 722c 2073 7472 5d3a 0a20 2020 2020  str, str]:.     
+00002ce0: 2020 2022 2222 416c 7461 6972 2064 6174     """Altair dat
+00002cf0: 6120 7472 616e 7366 6f72 6d65 7220 7468  a transformer th
+00002d00: 6174 2073 6572 6961 6c69 7a65 7320 7468  at serializes th
+00002d10: 6520 6461 7461 2c0a 2020 2020 2020 2020  e data,.        
+00002d20: 6372 6561 7465 7320 6120 7374 6162 6c65  creates a stable
+00002d30: 206e 616d 6520 6261 7365 6420 6f6e 2074   name based on t
+00002d40: 6865 2068 6173 6820 6f66 2074 6865 2064  he hash of the d
+00002d50: 6174 612c 0a20 2020 2020 2020 2073 746f  ata,.        sto
+00002d60: 7265 7320 7468 6520 6279 7465 7320 696e  res the bytes in
+00002d70: 746f 2074 6865 2064 6174 6173 6574 7320  to the datasets 
+00002d80: 6d61 7070 696e 6720 616e 640a 2020 2020  mapping and.    
+00002d90: 2020 2020 7265 7475 726e 7320 7468 6973      returns this
+00002da0: 206e 616d 6520 746f 2068 6176 6520 6974   name to have it
+00002db0: 2062 6520 7573 6564 2069 6e20 416c 7461   be used in Alta
+00002dc0: 6972 2e0a 2020 2020 2020 2020 2222 220a  ir..        """.
+00002dd0: 2020 2020 2020 2020 2320 416c 7265 6164          # Alread
+00002de0: 7920 7365 7269 616c 697a 6520 7468 6520  y serialize the 
+00002df0: 6461 7461 2074 6f20 6265 2061 626c 6520  data to be able 
+00002e00: 746f 2063 7265 6174 6520 6120 7374 6162  to create a stab
+00002e10: 6c65 0a20 2020 2020 2020 2023 2064 6174  le.        # dat
+00002e20: 6173 6574 206e 616d 653a 0a20 2020 2020  aset name:.     
+00002e30: 2020 2064 6174 615f 6279 7465 7320 3d20     data_bytes = 
+00002e40: 5f73 6572 6961 6c69 7a65 5f64 6174 6128  _serialize_data(
+00002e50: 6461 7461 290a 2020 2020 2020 2020 2320  data).        # 
+00002e60: 5573 6520 7468 6520 6d64 3520 6861 7368  Use the md5 hash
+00002e70: 206f 6620 7468 6520 6461 7461 2061 7320   of the data as 
+00002e80: 7468 6520 6e61 6d65 3a0a 2020 2020 2020  the name:.      
+00002e90: 2020 6820 3d20 6861 7368 6c69 622e 6e65    h = hashlib.ne
+00002ea0: 7728 226d 6435 222c 202a 2a48 4153 484c  w("md5", **HASHL
+00002eb0: 4942 5f4b 5741 5247 5329 0a20 2020 2020  IB_KWARGS).     
+00002ec0: 2020 2068 2e75 7064 6174 6528 7374 7228     h.update(str(
+00002ed0: 6461 7461 5f62 7974 6573 292e 656e 636f  data_bytes).enco
+00002ee0: 6465 2822 7574 662d 3822 2929 0a20 2020  de("utf-8")).   
+00002ef0: 2020 2020 206e 616d 6520 3d20 682e 6865       name = h.he
+00002f00: 7864 6967 6573 7428 290a 0a20 2020 2020  xdigest()..     
+00002f10: 2020 2064 6174 6173 6574 735b 6e61 6d65     datasets[name
+00002f20: 5d20 3d20 6461 7461 5f62 7974 6573 0a20  ] = data_bytes. 
+00002f30: 2020 2020 2020 2072 6574 7572 6e20 7b22         return {"
+00002f40: 6e61 6d65 223a 206e 616d 657d 0a0a 2020  name": name}..  
+00002f50: 2020 616c 742e 6461 7461 5f74 7261 6e73    alt.data_trans
+00002f60: 666f 726d 6572 732e 7265 6769 7374 6572  formers.register
+00002f70: 2822 6964 222c 2069 645f 7472 616e 7366  ("id", id_transf
+00002f80: 6f72 6d29 2020 2320 7479 7065 3a20 6967  orm)  # type: ig
+00002f90: 6e6f 7265 5b61 7474 722d 6465 6669 6e65  nore[attr-define
+00002fa0: 642c 756e 7573 6564 2d69 676e 6f72 655d  d,unused-ignore]
+00002fb0: 0a0a 2020 2020 2320 5468 6520 6465 6661  ..    # The defa
+00002fc0: 756c 7420 616c 7461 6972 2074 6865 6d65  ult altair theme
+00002fd0: 2068 6173 2073 6f6d 6520 7769 6474 682f   has some width/
+00002fe0: 6865 6967 6874 2064 6566 6175 6c74 7320  height defaults 
+00002ff0: 6465 6669 6e65 640a 2020 2020 2320 7768  defined.    # wh
+00003000: 6963 6820 6172 6520 6e6f 7420 7573 6566  ich are not usef
+00003010: 756c 2066 6f72 2053 7472 6561 6d6c 6974  ul for Streamlit
+00003020: 2e20 5468 6572 6566 6f72 652c 2077 6520  . Therefore, we 
+00003030: 6368 616e 6765 2074 6865 2074 6865 6d65  change the theme
+00003040: 2074 6f0a 2020 2020 2320 226e 6f6e 6522   to.    # "none"
+00003050: 2074 6f20 6176 6f69 6420 7468 6f73 6520   to avoid those 
+00003060: 6465 6661 756c 7473 2e0a 2020 2020 7769  defaults..    wi
+00003070: 7468 2061 6c74 2e74 6865 6d65 732e 656e  th alt.themes.en
+00003080: 6162 6c65 2822 6e6f 6e65 2229 2069 6620  able("none") if 
+00003090: 616c 742e 7468 656d 6573 2e61 6374 6976  alt.themes.activ
+000030a0: 6520 3d3d 2022 6465 6661 756c 7422 2065  e == "default" e
+000030b0: 6c73 6520 6e75 6c6c 636f 6e74 6578 7428  lse nullcontext(
+000030c0: 293a 2020 2320 7479 7065 3a20 6967 6e6f  ):  # type: igno
+000030d0: 7265 5b61 7474 722d 6465 6669 6e65 642c  re[attr-defined,
+000030e0: 756e 7573 6564 2d69 676e 6f72 655d 0a20  unused-ignore]. 
+000030f0: 2020 2020 2020 2077 6974 6820 616c 742e         with alt.
+00003100: 6461 7461 5f74 7261 6e73 666f 726d 6572  data_transformer
+00003110: 732e 656e 6162 6c65 2822 6964 2229 3a20  s.enable("id"): 
+00003120: 2023 2074 7970 653a 2069 676e 6f72 655b   # type: ignore[
+00003130: 6174 7472 2d64 6566 696e 6564 2c75 6e75  attr-defined,unu
+00003140: 7365 642d 6967 6e6f 7265 5d0a 2020 2020  sed-ignore].    
+00003150: 2020 2020 2020 2020 6368 6172 745f 6469          chart_di
+00003160: 6374 203d 2061 6c74 6169 725f 6368 6172  ct = altair_char
+00003170: 742e 746f 5f64 6963 7428 290a 0a20 2020  t.to_dict()..   
+00003180: 2023 2050 7574 2064 6174 6173 6574 7320   # Put datasets 
+00003190: 6261 636b 2069 6e74 6f20 7468 6520 6368  back into the ch
+000031a0: 6172 7420 6469 6374 3a0a 2020 2020 6368  art dict:.    ch
+000031b0: 6172 745f 6469 6374 5b22 6461 7461 7365  art_dict["datase
+000031c0: 7473 225d 203d 2064 6174 6173 6574 730a  ts"] = datasets.
+000031d0: 2020 2020 7265 7475 726e 2063 6861 7274      return chart
+000031e0: 5f64 6963 740a 0a0a 6465 6620 5f64 6973  _dict...def _dis
+000031f0: 616c 6c6f 775f 6d75 6c74 695f 7669 6577  allow_multi_view
+00003200: 5f63 6861 7274 7328 7370 6563 3a20 5665  _charts(spec: Ve
+00003210: 6761 4c69 7465 5370 6563 2920 2d3e 204e  gaLiteSpec) -> N
+00003220: 6f6e 653a 0a20 2020 2022 2222 5261 6973  one:.    """Rais
+00003230: 6520 616e 2065 7863 6570 7469 6f6e 2069  e an exception i
+00003240: 6620 7468 6520 7370 6563 2063 6f6e 7461  f the spec conta
+00003250: 696e 7320 6120 6d75 6c74 692d 7669 6577  ins a multi-view
+00003260: 2063 6861 7274 2028 7669 6577 2063 6f6d   chart (view com
+00003270: 706f 7369 7469 6f6e 292e 0a0a 2020 2020  position)...    
+00003280: 5468 6973 2069 7320 696e 7465 6e64 6564  This is intended
+00003290: 2074 6f20 6265 2075 7365 6420 6173 2061   to be used as a
+000032a0: 2074 656d 706f 7261 7279 2073 6f6c 7574   temporary solut
+000032b0: 696f 6e20 746f 2070 7265 7665 6e74 2073  ion to prevent s
+000032c0: 656c 6563 7469 6f6e 7320 6f6e 0a20 2020  elections on.   
+000032d0: 206d 756c 7469 2d76 6965 7720 6368 6172   multi-view char
+000032e0: 7473 2e20 5468 6572 6520 6172 6520 746f  ts. There are to
+000032f0: 6f20 6d61 6e79 2065 6467 6520 6361 7365  o many edge case
+00003300: 7320 746f 2068 616e 646c 6520 7365 6c65  s to handle sele
+00003310: 6374 696f 6e73 206f 6e20 7468 6573 650a  ctions on these.
+00003320: 2020 2020 6368 6172 7473 2063 6f72 7265      charts corre
+00003330: 6374 6c79 2c20 736f 2077 6527 7265 2064  ctly, so we're d
+00003340: 6973 616c 6c6f 7769 6e67 2074 6865 6d20  isallowing them 
+00003350: 666f 7220 6e6f 772e 0a0a 2020 2020 4d6f  for now...    Mo
+00003360: 7265 2069 6e66 6f72 6d61 7469 6f6e 2061  re information a
+00003370: 626f 7574 2076 6965 7720 636f 6d70 6f73  bout view compos
+00003380: 6974 696f 6e73 3a20 6874 7470 733a 2f2f  itions: https://
+00003390: 7665 6761 2e67 6974 6875 622e 696f 2f76  vega.github.io/v
+000033a0: 6567 612d 6c69 7465 2f64 6f63 732f 636f  ega-lite/docs/co
+000033b0: 6d70 6f73 6974 696f 6e2e 6874 6d6c 0a20  mposition.html. 
+000033c0: 2020 2022 2222 0a0a 2020 2020 6966 2028     """..    if (
+000033d0: 0a20 2020 2020 2020 2061 6e79 286b 6579  .        any(key
+000033e0: 2069 6e20 7370 6563 2066 6f72 206b 6579   in spec for key
+000033f0: 2069 6e20 5b22 6c61 7965 7222 2c20 2268   in ["layer", "h
+00003400: 636f 6e63 6174 222c 2022 7663 6f6e 6361  concat", "vconca
+00003410: 7422 2c20 2263 6f6e 6361 7422 2c20 2273  t", "concat", "s
+00003420: 7065 6322 5d29 0a20 2020 2020 2020 206f  pec"]).        o
+00003430: 7220 2265 6e63 6f64 696e 6722 206e 6f74  r "encoding" not
+00003440: 2069 6e20 7370 6563 0a20 2020 2029 3a0a   in spec.    ):.
+00003450: 2020 2020 2020 2020 7261 6973 6520 5374          raise St
+00003460: 7265 616d 6c69 7441 5049 4578 6365 7074  reamlitAPIExcept
+00003470: 696f 6e28 0a20 2020 2020 2020 2020 2020  ion(.           
+00003480: 2022 5365 6c65 6374 696f 6e73 2061 7265   "Selections are
+00003490: 206e 6f74 2079 6574 2073 7570 706f 7274   not yet support
+000034a0: 6564 2066 6f72 206d 756c 7469 2d76 6965  ed for multi-vie
+000034b0: 7720 6368 6172 7473 2028 6368 6172 7420  w charts (chart 
+000034c0: 636f 6d70 6f73 6974 696f 6e73 292e 2022  compositions). "
+000034d0: 0a20 2020 2020 2020 2020 2020 2022 4966  .            "If
+000034e0: 2079 6f75 2077 6f75 6c64 206c 696b 6520   you would like 
+000034f0: 746f 2075 7365 2073 656c 6563 7469 6f6e  to use selection
+00003500: 7320 6f6e 206d 756c 7469 2d76 6965 7720  s on multi-view 
+00003510: 6368 6172 7473 2c20 706c 6561 7365 2075  charts, please u
+00003520: 7076 6f74 6520 220a 2020 2020 2020 2020  pvote ".        
+00003530: 2020 2020 2274 6869 7320 5b47 6974 6875      "this [Githu
+00003540: 6220 6973 7375 655d 2868 7474 7073 3a2f  b issue](https:/
+00003550: 2f67 6974 6875 622e 636f 6d2f 7374 7265  /github.com/stre
+00003560: 616d 6c69 742f 7374 7265 616d 6c69 742f  amlit/streamlit/
+00003570: 6973 7375 6573 2f38 3634 3329 2e22 0a20  issues/8643).". 
+00003580: 2020 2020 2020 2029 0a0a 0a64 6566 205f         )...def _
+00003590: 6578 7472 6163 745f 7365 6c65 6374 696f  extract_selectio
+000035a0: 6e5f 7061 7261 6d65 7465 7273 2873 7065  n_parameters(spe
+000035b0: 633a 2056 6567 614c 6974 6553 7065 6329  c: VegaLiteSpec)
+000035c0: 202d 3e20 7365 745b 7374 725d 3a0a 2020   -> set[str]:.  
+000035d0: 2020 2222 2245 7874 7261 6374 2074 6865    """Extract the
+000035e0: 206e 616d 6573 206f 6620 616c 6c20 7661   names of all va
+000035f0: 6c69 6420 7365 6c65 6374 696f 6e20 7061  lid selection pa
+00003600: 7261 6d65 7465 7273 2066 726f 6d20 7468  rameters from th
+00003610: 6520 7370 6563 2e22 2222 0a20 2020 2069  e spec.""".    i
+00003620: 6620 6e6f 7420 7370 6563 206f 7220 2270  f not spec or "p
+00003630: 6172 616d 7322 206e 6f74 2069 6e20 7370  arams" not in sp
+00003640: 6563 3a0a 2020 2020 2020 2020 7265 7475  ec:.        retu
+00003650: 726e 2073 6574 2829 0a0a 2020 2020 7061  rn set()..    pa
+00003660: 7261 6d5f 6e61 6d65 7320 3d20 7365 7428  ram_names = set(
+00003670: 290a 0a20 2020 2066 6f72 2070 6172 616d  )..    for param
+00003680: 2069 6e20 7370 6563 5b22 7061 7261 6d73   in spec["params
+00003690: 225d 3a0a 2020 2020 2020 2020 2320 4368  "]:.        # Ch
+000036a0: 6563 6b20 6966 2069 7420 6c6f 6f6b 7320  eck if it looks 
+000036b0: 6c69 6b65 2061 2076 616c 6964 2073 656c  like a valid sel
+000036c0: 6563 7469 6f6e 2070 6172 616d 6574 6572  ection parameter
+000036d0: 3a0a 2020 2020 2020 2020 2320 6874 7470  :.        # http
+000036e0: 733a 2f2f 7665 6761 2e67 6974 6875 622e  s://vega.github.
+000036f0: 696f 2f76 6567 612d 6c69 7465 2f64 6f63  io/vega-lite/doc
+00003700: 732f 7365 6c65 6374 696f 6e2e 6874 6d6c  s/selection.html
+00003710: 0a20 2020 2020 2020 2069 6620 7061 7261  .        if para
+00003720: 6d2e 6765 7428 226e 616d 6522 2920 616e  m.get("name") an
+00003730: 6420 7061 7261 6d2e 6765 7428 2273 656c  d param.get("sel
+00003740: 6563 7422 293a 0a20 2020 2020 2020 2020  ect"):.         
+00003750: 2020 2023 2053 656c 6563 7469 6f6e 2066     # Selection f
+00003760: 6f75 6e64 2c20 6a75 7374 2072 6574 7572  ound, just retur
+00003770: 6e20 6865 7265 2074 6f20 6e6f 7420 7368  n here to not sh
+00003780: 6f77 2074 6865 2065 7863 6570 7469 6f6e  ow the exception
+00003790: 2e0a 2020 2020 2020 2020 2020 2020 7061  ..            pa
+000037a0: 7261 6d5f 6e61 6d65 732e 6164 6428 7061  ram_names.add(pa
+000037b0: 7261 6d5b 226e 616d 6522 5d29 0a0a 2020  ram["name"])..  
+000037c0: 2020 7265 7475 726e 2070 6172 616d 5f6e    return param_n
+000037d0: 616d 6573 0a0a 0a64 6566 205f 7061 7273  ames...def _pars
+000037e0: 655f 7365 6c65 6374 696f 6e5f 6d6f 6465  e_selection_mode
+000037f0: 280a 2020 2020 7370 6563 3a20 5665 6761  (.    spec: Vega
+00003800: 4c69 7465 5370 6563 2c0a 2020 2020 7365  LiteSpec,.    se
+00003810: 6c65 6374 696f 6e5f 6d6f 6465 3a20 7374  lection_mode: st
+00003820: 7220 7c20 4974 6572 6162 6c65 5b73 7472  r | Iterable[str
+00003830: 5d20 7c20 4e6f 6e65 2c0a 2920 2d3e 206c  ] | None,.) -> l
+00003840: 6973 745b 7374 725d 3a0a 2020 2020 2222  ist[str]:.    ""
+00003850: 2250 6172 7365 2061 6e64 2063 6865 636b  "Parse and check
+00003860: 2074 6865 2075 7365 7220 7072 6f76 6964   the user provid
+00003870: 6564 2073 656c 6563 7469 6f6e 206d 6f64  ed selection mod
+00003880: 6573 2e0a 0a20 2020 2054 6869 7320 7769  es...    This wi
+00003890: 6c6c 2072 6169 7365 2061 6e20 6578 6365  ll raise an exce
+000038a0: 7074 696f 6e20 6966 206e 6f20 7661 6c69  ption if no vali
+000038b0: 6420 7365 6c65 6374 696f 6e20 7061 7261  d selection para
+000038c0: 6d65 7465 7273 2061 7265 2066 6f75 6e64  meters are found
+000038d0: 2069 6e20 7468 6520 7370 6563 0a20 2020   in the spec.   
+000038e0: 206f 7220 6966 2074 6865 2075 7365 7220   or if the user 
+000038f0: 7072 6f76 6964 6564 2073 656c 6563 7469  provided selecti
+00003900: 6f6e 206d 6f64 6573 2061 7265 206e 6f74  on modes are not
+00003910: 2064 6566 696e 6564 2069 6e20 7468 6520   defined in the 
+00003920: 7370 6563 2e0a 0a20 2020 2050 6172 616d  spec...    Param
+00003930: 6574 6572 730a 2020 2020 2d2d 2d2d 2d2d  eters.    ------
+00003940: 2d2d 2d2d 0a20 2020 2073 7065 6320 3a20  ----.    spec : 
+00003950: 5665 6761 4c69 7465 5370 6563 0a20 2020  VegaLiteSpec.   
+00003960: 2020 2020 2054 6865 2056 6567 612d 4c69       The Vega-Li
+00003970: 7465 2063 6861 7274 2073 7065 6369 6669  te chart specifi
+00003980: 6361 7469 6f6e 2e0a 0a20 2020 2073 656c  cation...    sel
+00003990: 6563 7469 6f6e 5f6d 6f64 6520 3a20 7374  ection_mode : st
+000039a0: 722c 2049 7465 7261 626c 655b 7374 725d  r, Iterable[str]
+000039b0: 2c20 6f72 204e 6f6e 650a 2020 2020 2020  , or None.      
+000039c0: 2020 5468 6520 7573 6572 2070 726f 7669    The user provi
+000039d0: 6465 6420 7365 6c65 6374 696f 6e20 6d6f  ded selection mo
+000039e0: 6465 2873 292e 0a0a 2020 2020 5265 7475  de(s)...    Retu
+000039f0: 726e 730a 2020 2020 2d2d 2d2d 2d2d 2d0a  rns.    -------.
+00003a00: 2020 2020 6c69 7374 5b73 7472 5d0a 2020      list[str].  
+00003a10: 2020 2020 2020 5468 6520 7061 7273 6564        The parsed
+00003a20: 2073 656c 6563 7469 6f6e 206d 6f64 6528   selection mode(
+00003a30: 7329 2074 6861 7420 7368 6f75 6c64 2062  s) that should b
+00003a40: 6520 6163 7469 7661 7465 642e 0a20 2020  e activated..   
+00003a50: 2022 2222 0a0a 2020 2020 2320 4578 7472   """..    # Extr
+00003a60: 6163 7420 616c 6c20 7365 6c65 6374 696f  act all selectio
+00003a70: 6e20 7061 7261 6d65 7465 7273 2066 726f  n parameters fro
+00003a80: 6d20 7468 6520 7370 6563 3a0a 2020 2020  m the spec:.    
+00003a90: 616c 6c5f 7365 6c65 6374 696f 6e5f 7061  all_selection_pa
+00003aa0: 7261 6d73 203d 205f 6578 7472 6163 745f  rams = _extract_
+00003ab0: 7365 6c65 6374 696f 6e5f 7061 7261 6d65  selection_parame
+00003ac0: 7465 7273 2873 7065 6329 0a0a 2020 2020  ters(spec)..    
+00003ad0: 6966 206e 6f74 2061 6c6c 5f73 656c 6563  if not all_selec
+00003ae0: 7469 6f6e 5f70 6172 616d 733a 0a20 2020  tion_params:.   
+00003af0: 2020 2020 2072 6169 7365 2053 7472 6561       raise Strea
+00003b00: 6d6c 6974 4150 4945 7863 6570 7469 6f6e  mlitAPIException
+00003b10: 280a 2020 2020 2020 2020 2020 2020 2253  (.            "S
+00003b20: 656c 6563 7469 6f6e 7320 6172 6520 6163  elections are ac
+00003b30: 7469 7661 7465 642c 2062 7574 2074 6865  tivated, but the
+00003b40: 2070 726f 7669 6465 6420 6368 6172 7420   provided chart 
+00003b50: 7370 6563 2064 6f65 7320 6e6f 7420 220a  spec does not ".
+00003b60: 2020 2020 2020 2020 2020 2020 2268 6176              "hav
+00003b70: 6520 616e 7920 7365 6c65 6374 696f 6e73  e any selections
+00003b80: 2064 6566 696e 6564 2e20 546f 2061 6464   defined. To add
+00003b90: 2073 656c 6563 7469 6f6e 7320 746f 2060   selections to `
+00003ba0: 7374 2e61 6c74 6169 725f 6368 6172 7460  st.altair_chart`
+00003bb0: 2c20 6368 6563 6b20 6f75 7420 7468 6520  , check out the 
+00003bc0: 646f 6375 6d65 6e74 6174 696f 6e20 220a  documentation ".
+00003bd0: 2020 2020 2020 2020 2020 2020 225b 6865              "[he
+00003be0: 7265 5d28 6874 7470 733a 2f2f 616c 7461  re](https://alta
+00003bf0: 6972 2d76 697a 2e67 6974 6875 622e 696f  ir-viz.github.io
+00003c00: 2f75 7365 725f 6775 6964 652f 696e 7465  /user_guide/inte
+00003c10: 7261 6374 696f 6e73 2e68 746d 6c23 7365  ractions.html#se
+00003c20: 6c65 6374 696f 6e73 2d63 6170 7475 7269  lections-capturi
+00003c30: 6e67 2d63 6861 7274 2d69 6e74 6572 6163  ng-chart-interac
+00003c40: 7469 6f6e 7329 2e20 220a 2020 2020 2020  tions). ".      
+00003c50: 2020 2020 2020 2246 6f72 2061 6464 696e        "For addin
+00003c60: 6720 7365 6c65 6374 696f 6e73 2074 6f20  g selections to 
+00003c70: 6073 742e 7665 6761 5f6c 6974 655f 6368  `st.vega_lite_ch
+00003c80: 6172 7460 2c20 7461 6b65 2061 206c 6f6f  art`, take a loo
+00003c90: 6b20 220a 2020 2020 2020 2020 2020 2020  k ".            
+00003ca0: 2261 7420 7468 6520 7370 6563 6966 6963  "at the specific
+00003cb0: 6174 696f 6e20 5b68 6572 655d 2868 7474  ation [here](htt
+00003cc0: 7073 3a2f 2f76 6567 612e 6769 7468 7562  ps://vega.github
+00003cd0: 2e69 6f2f 7665 6761 2d6c 6974 652f 646f  .io/vega-lite/do
+00003ce0: 6373 2f73 656c 6563 7469 6f6e 2e68 746d  cs/selection.htm
+00003cf0: 6c29 2e22 0a20 2020 2020 2020 2029 0a0a  l).".        )..
+00003d00: 2020 2020 6966 2073 656c 6563 7469 6f6e      if selection
+00003d10: 5f6d 6f64 6520 6973 204e 6f6e 653a 0a20  _mode is None:. 
+00003d20: 2020 2020 2020 2023 2041 6374 6976 6174         # Activat
+00003d30: 6520 616c 6c20 7365 6c65 6374 696f 6e20  e all selection 
+00003d40: 7061 7261 6d65 7465 7273 3a0a 2020 2020  parameters:.    
+00003d50: 2020 2020 7265 7475 726e 2073 6f72 7465      return sorte
+00003d60: 6428 6c69 7374 2861 6c6c 5f73 656c 6563  d(list(all_selec
+00003d70: 7469 6f6e 5f70 6172 616d 7329 290a 0a20  tion_params)).. 
+00003d80: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
+00003d90: 2873 656c 6563 7469 6f6e 5f6d 6f64 652c  (selection_mode,
+00003da0: 2073 7472 293a 0a20 2020 2020 2020 2023   str):.        #
+00003db0: 2043 6f6e 7665 7274 2073 696e 676c 6520   Convert single 
+00003dc0: 7374 7269 6e67 2074 6f20 6c69 7374 3a0a  string to list:.
+00003dd0: 2020 2020 2020 2020 7365 6c65 6374 696f          selectio
+00003de0: 6e5f 6d6f 6465 203d 205b 7365 6c65 6374  n_mode = [select
+00003df0: 696f 6e5f 6d6f 6465 5d0a 0a20 2020 2023  ion_mode]..    #
+00003e00: 2043 6865 636b 2074 6861 7420 616c 6c20   Check that all 
+00003e10: 7072 6f76 6964 6564 2073 656c 6563 7469  provided selecti
+00003e20: 6f6e 2070 6172 616d 6574 6572 7320 6172  on parameters ar
+00003e30: 6520 6465 6669 6e65 6420 696e 2074 6865  e defined in the
+00003e40: 2073 7065 633a 0a20 2020 2066 6f72 2073   spec:.    for s
+00003e50: 656c 6563 7469 6f6e 5f6e 616d 6520 696e  election_name in
+00003e60: 2073 656c 6563 7469 6f6e 5f6d 6f64 653a   selection_mode:
+00003e70: 0a20 2020 2020 2020 2069 6620 7365 6c65  .        if sele
+00003e80: 6374 696f 6e5f 6e61 6d65 206e 6f74 2069  ction_name not i
+00003e90: 6e20 616c 6c5f 7365 6c65 6374 696f 6e5f  n all_selection_
+00003ea0: 7061 7261 6d73 3a0a 2020 2020 2020 2020  params:.        
+00003eb0: 2020 2020 7261 6973 6520 5374 7265 616d      raise Stream
+00003ec0: 6c69 7441 5049 4578 6365 7074 696f 6e28  litAPIException(
+00003ed0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003ee0: 2066 2253 656c 6563 7469 6f6e 2070 6172   f"Selection par
+00003ef0: 616d 6574 6572 2027 7b73 656c 6563 7469  ameter '{selecti
+00003f00: 6f6e 5f6e 616d 657d 2720 6973 206e 6f74  on_name}' is not
+00003f10: 2064 6566 696e 6564 2069 6e20 7468 6520   defined in the 
+00003f20: 6368 6172 7420 7370 6563 2e20 220a 2020  chart spec. ".  
+00003f30: 2020 2020 2020 2020 2020 2020 2020 6622                f"
+00003f40: 4176 6169 6c61 626c 6520 7365 6c65 6374  Available select
+00003f50: 696f 6e20 7061 7261 6d65 7465 7273 2061  ion parameters a
+00003f60: 7265 3a20 7b61 6c6c 5f73 656c 6563 7469  re: {all_selecti
+00003f70: 6f6e 5f70 6172 616d 737d 2e22 0a20 2020  on_params}.".   
+00003f80: 2020 2020 2020 2020 2029 0a20 2020 2072           ).    r
+00003f90: 6574 7572 6e20 736f 7274 6564 286c 6973  eturn sorted(lis
+00003fa0: 7428 7365 6c65 6374 696f 6e5f 6d6f 6465  t(selection_mode
+00003fb0: 2929 0a0a 0a64 6566 205f 7265 7365 745f  ))...def _reset_
+00003fc0: 636f 756e 7465 725f 7061 7474 6572 6e28  counter_pattern(
+00003fd0: 7072 6566 6978 3a20 7374 722c 2076 6567  prefix: str, veg
+00003fe0: 615f 7370 6563 3a20 7374 7229 202d 3e20  a_spec: str) -> 
+00003ff0: 7374 723a 0a20 2020 2022 2222 416c 7461  str:.    """Alta
+00004000: 6972 2075 7365 7320 6120 676c 6f62 616c  ir uses a global
+00004010: 2063 6f75 6e74 6572 2066 6f72 2075 6e6e   counter for unn
+00004020: 616d 6564 2070 6172 616d 6574 6572 7320  amed parameters 
+00004030: 616e 6420 7669 6577 732e 0a20 2020 2057  and views..    W
+00004040: 6520 6e65 6564 2074 6f20 7265 7365 7420  e need to reset 
+00004050: 7468 6573 6520 636f 756e 7465 7273 206f  these counters o
+00004060: 6e20 6120 7370 6563 2d6c 6576 656c 2074  n a spec-level t
+00004070: 6f20 6d61 6b65 2074 6865 0a20 2020 2073  o make the.    s
+00004080: 7065 6320 7374 6162 6c65 2061 6372 6f73  pec stable acros
+00004090: 7320 7265 7275 6e73 2061 6e64 2061 766f  s reruns and avo
+000040a0: 6964 2063 6861 6e67 6573 2074 6f20 7468  id changes to th
+000040b0: 6520 656c 656d 656e 7420 4944 2e0a 2020  e element ID..  
+000040c0: 2020 2222 220a 2020 2020 7061 7474 6572    """.    patter
+000040d0: 6e20 3d20 7265 2e63 6f6d 7069 6c65 2872  n = re.compile(r
+000040e0: 6627 227b 7072 6566 6978 7d5c 642b 2227  f'"{prefix}\d+"'
+000040f0: 290a 2020 2020 2320 4765 7420 616c 6c20  ).    # Get all 
+00004100: 6d61 7463 6865 7320 7769 7468 6f75 7420  matches without 
+00004110: 6475 706c 6963 6174 6573 2069 6e20 6f72  duplicates in or
+00004120: 6465 7220 6f66 2061 7070 6561 7261 6e63  der of appearanc
+00004130: 652e 0a20 2020 2023 2055 7369 6e67 2061  e..    # Using a
+00004140: 2073 6574 2068 6572 6520 776f 756c 6420   set here would 
+00004150: 6e6f 7420 6775 6172 616e 7465 6520 7468  not guarantee th
+00004160: 6520 6f72 6465 7220 6f66 2061 7070 6561  e order of appea
+00004170: 7261 6e63 652c 0a20 2020 2023 2077 6869  rance,.    # whi
+00004180: 6368 206d 6967 6874 206c 6561 6420 746f  ch might lead to
+00004190: 2064 6966 6665 7265 6e74 2072 6570 6c61   different repla
+000041a0: 6365 6d65 6e74 7320 6f6e 2065 6163 6820  cements on each 
+000041b0: 7275 6e2e 0a20 2020 2023 2054 6865 206f  run..    # The o
+000041c0: 7264 6572 206f 6620 7468 6520 7370 6563  rder of the spec
+000041d0: 2066 726f 6d20 416c 7461 6972 2069 7320   from Altair is 
+000041e0: 6578 7065 6374 6564 2074 6f20 7374 6179  expected to stay
+000041f0: 2073 7461 626c 650a 2020 2020 2320 7769   stable.    # wi
+00004200: 7468 696e 2074 6865 2073 616d 6520 7365  thin the same se
+00004210: 7373 696f 6e20 2f20 416c 7461 6972 2076  ssion / Altair v
+00004220: 6572 7369 6f6e 2e0a 2020 2020 2320 5468  ersion..    # Th
+00004230: 6520 6f72 6465 7220 6d69 6768 7420 6368  e order might ch
+00004240: 616e 6765 2077 6974 6820 416c 7461 6972  ange with Altair
+00004250: 2075 7064 6174 6573 2c20 6275 7420 7468   updates, but th
+00004260: 6174 2773 206e 6f74 2072 6561 6c6c 790a  at's not really.
+00004270: 2020 2020 2320 6120 6361 7365 2074 6861      # a case tha
+00004280: 7420 6973 2072 656c 6576 616e 7420 666f  t is relevant fo
+00004290: 7220 7573 2073 696e 6365 2077 6520 6d61  r us since we ma
+000042a0: 696e 6c79 2063 6172 6520 6162 6f75 7420  inly care about 
+000042b0: 6861 7669 6e67 0a20 2020 2023 2074 6869  having.    # thi
+000042c0: 7320 7374 6162 6c65 2077 6974 6869 6e20  s stable within 
+000042d0: 6120 7365 7373 696f 6e2e 0a20 2020 2069  a session..    i
+000042e0: 6620 6d61 7463 6865 7320 3a3d 206c 6973  f matches := lis
+000042f0: 7428 6469 6374 2e66 726f 6d6b 6579 7328  t(dict.fromkeys(
+00004300: 7061 7474 6572 6e2e 6669 6e64 616c 6c28  pattern.findall(
+00004310: 7665 6761 5f73 7065 6329 2929 3a0a 2020  vega_spec))):.  
+00004320: 2020 2020 2020 2320 4164 6420 6120 7072        # Add a pr
+00004330: 6566 6978 2074 6f20 7468 6520 7265 706c  efix to the repl
+00004340: 6163 656d 656e 7420 746f 2061 766f 6964  acement to avoid
+00004350: 0a20 2020 2020 2020 2023 2072 6570 6c61  .        # repla
+00004360: 6369 6e67 2069 6e73 7461 6e63 6573 2074  cing instances t
+00004370: 6861 7420 616c 7265 6164 7920 6861 7665  hat already have
+00004380: 2062 6565 6e20 7265 706c 6163 6564 2062   been replaced b
+00004390: 6566 6f72 652e 0a20 2020 2020 2020 2023  efore..        #
+000043a0: 2054 6865 2070 7265 6669 7820 6865 7265   The prefix here
+000043b0: 2069 7320 6172 6269 7472 6172 696c 7920   is arbitrarily 
+000043c0: 6368 6f73 656e 2077 6974 6820 7468 6520  chosen with the 
+000043d0: 6d61 696e 2067 6f61 6c0a 2020 2020 2020  main goal.      
+000043e0: 2020 2320 7468 6174 2069 7473 2065 7874    # that its ext
+000043f0: 7265 6d65 6c79 2075 6e6c 696b 656c 7920  remely unlikely 
+00004400: 746f 2061 6c72 6561 6479 2062 6520 7061  to already be pa
+00004410: 7274 206f 6620 7468 6520 7370 6563 3a0a  rt of the spec:.
+00004420: 2020 2020 2020 2020 7265 706c 6163 656d          replacem
+00004430: 656e 745f 7072 6566 6978 203d 2022 5f5f  ent_prefix = "__
+00004440: 7265 706c 6163 655f 7072 6566 6978 5f6f  replace_prefix_o
+00004450: 3968 6431 3031 6e32 3265 315f 5f22 0a0a  9hd101n22e1__"..
+00004460: 2020 2020 2020 2020 2320 5265 706c 6163          # Replac
+00004470: 6520 616c 6c20 6d61 7463 6865 7320 7769  e all matches wi
+00004480: 7468 2061 2063 6f75 6e74 6572 2073 7461  th a counter sta
+00004490: 7274 696e 6720 6672 6f6d 2031 0a20 2020  rting from 1.   
+000044a0: 2020 2020 2023 2057 6520 7374 6172 7420       # We start 
+000044b0: 6672 6f6d 2031 2074 6f20 696d 6974 6174  from 1 to imitat
+000044c0: 6520 7468 6520 616c 7461 6972 2062 6568  e the altair beh
+000044d0: 6176 696f 722e 0a20 2020 2020 2020 2066  avior..        f
+000044e0: 6f72 2063 6f75 6e74 6572 2c20 6d61 7463  or counter, matc
+000044f0: 6820 696e 2065 6e75 6d65 7261 7465 286d  h in enumerate(m
+00004500: 6174 6368 6573 2c20 7374 6172 743d 3129  atches, start=1)
+00004510: 3a0a 2020 2020 2020 2020 2020 2020 7665  :.            ve
+00004520: 6761 5f73 7065 6320 3d20 7665 6761 5f73  ga_spec = vega_s
+00004530: 7065 632e 7265 706c 6163 6528 0a20 2020  pec.replace(.   
+00004540: 2020 2020 2020 2020 2020 2020 206d 6174               mat
+00004550: 6368 2c20 6627 227b 7265 706c 6163 656d  ch, f'"{replacem
+00004560: 656e 745f 7072 6566 6978 7d7b 7072 6566  ent_prefix}{pref
+00004570: 6978 7d7b 636f 756e 7465 727d 2227 0a20  ix}{counter}"'. 
+00004580: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
+00004590: 2020 2020 2020 2320 5265 6d6f 7665 2074        # Remove t
+000045a0: 6865 2070 7265 6669 7820 6167 6169 6e20  he prefix again 
+000045b0: 6672 6f6d 2061 6c6c 2072 6570 6c61 6365  from all replace
+000045c0: 6d65 6e74 733a 0a20 2020 2020 2020 2076  ments:.        v
+000045d0: 6567 615f 7370 6563 203d 2076 6567 615f  ega_spec = vega_
+000045e0: 7370 6563 2e72 6570 6c61 6365 2872 6570  spec.replace(rep
+000045f0: 6c61 6365 6d65 6e74 5f70 7265 6669 782c  lacement_prefix,
+00004600: 2022 2229 0a20 2020 2072 6574 7572 6e20   "").    return 
+00004610: 7665 6761 5f73 7065 630a 0a0a 6465 6620  vega_spec...def 
+00004620: 5f73 7461 6269 6c69 7a65 5f76 6567 615f  _stabilize_vega_
+00004630: 6a73 6f6e 5f73 7065 6328 7665 6761 5f73  json_spec(vega_s
+00004640: 7065 633a 2073 7472 2920 2d3e 2073 7472  pec: str) -> str
+00004650: 3a0a 2020 2020 2222 224d 616b 6573 2074  :.    """Makes t
+00004660: 6865 2063 6861 7274 2073 7065 6320 7374  he chart spec st
+00004670: 6179 2073 7461 626c 6520 6163 726f 7373  ay stable across
+00004680: 2072 6572 756e 7320 616e 6420 7365 7373   reruns and sess
+00004690: 696f 6e73 2e0a 0a20 2020 2041 6c74 6169  ions...    Altai
+000046a0: 7220 6175 746f 2063 7265 6174 6573 206e  r auto creates n
+000046b0: 616d 6573 2066 6f72 2075 6e6e 616d 6564  ames for unnamed
+000046c0: 2070 6172 616d 6574 6572 7320 2620 7669   parameters & vi
+000046d0: 6577 732e 2049 7420 7573 6573 2061 2067  ews. It uses a g
+000046e0: 6c6f 6261 6c20 636f 756e 7465 720a 2020  lobal counter.  
+000046f0: 2020 666f 7220 7468 6520 6e61 6d69 6e67    for the naming
+00004700: 2077 6869 6368 2077 696c 6c20 7265 7375   which will resu
+00004710: 6c74 2069 6e20 6120 6469 6666 6572 656e  lt in a differen
+00004720: 7420 7370 6563 206f 6e20 6576 6572 7920  t spec on every 
+00004730: 7265 7275 6e2e 0a20 2020 2049 6e20 5374  rerun..    In St
+00004740: 7265 616d 6c69 742c 2077 6520 6e65 6564  reamlit, we need
+00004750: 2074 6865 2073 7065 6320 746f 2062 6520   the spec to be 
+00004760: 7374 6162 6c65 2061 6372 6f73 7320 7265  stable across re
+00004770: 7275 6e73 2061 6e64 2073 6573 7369 6f6e  runs and session
+00004780: 7320 746f 2070 7265 7665 6e74 2074 6865  s to prevent the
+00004790: 2063 6861 7274 0a20 2020 2066 726f 6d20   chart.    from 
+000047a0: 6765 7474 696e 6720 6120 6e65 7720 6964  getting a new id
+000047b0: 656e 7469 7479 2e20 536f 2077 6520 6e65  entity. So we ne
+000047c0: 6564 2074 6f20 7265 706c 6163 6520 7468  ed to replace th
+000047d0: 6520 6e61 6d65 7320 7769 7468 2063 6f75  e names with cou
+000047e0: 6e74 6572 2077 6974 6820 6120 7374 6162  nter with a stab
+000047f0: 6c65 206e 616d 652e 0a20 2020 2048 6176  le name..    Hav
+00004800: 696e 6720 6120 7374 6162 6c65 2063 6861  ing a stable cha
+00004810: 7274 2073 7065 6320 6973 2061 6c73 6f20  rt spec is also 
+00004820: 696d 706f 7274 616e 7420 666f 7220 6665  important for fe
+00004830: 6174 7572 6573 206c 696b 6520 666f 7277  atures like forw
+00004840: 6172 6420 6d65 7373 6167 6520 6361 6368  ard message cach
+00004850: 652c 0a20 2020 2077 6865 7265 2077 6520  e,.    where we 
+00004860: 646f 6e27 7420 7761 6e74 2074 6f20 6861  don't want to ha
+00004870: 7665 2063 6861 6e67 696e 6720 6d65 7373  ve changing mess
+00004880: 6167 6573 206f 6e20 6576 6572 7920 7265  ages on every re
+00004890: 7275 6e2e 0a0a 2020 2020 5061 7261 6d65  run...    Parame
+000048a0: 7465 7220 636f 756e 7465 723a 0a20 2020  ter counter:.   
+000048b0: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
+000048c0: 636f 6d2f 7665 6761 2f61 6c74 6169 722f  com/vega/altair/
+000048d0: 626c 6f62 2f66 3334 3563 6439 3336 3861  blob/f345cd9368a
+000048e0: 6532 6262 6339 3836 3238 6539 3234 3563  e2bbc98628e9245c
+000048f0: 3933 6661 3966 6235 3832 3632 312f 616c  93fa9fb582621/al
+00004900: 7461 6972 2f76 6567 616c 6974 652f 7635  tair/vegalite/v5
+00004910: 2f61 7069 2e70 7923 4c31 3936 0a0a 2020  /api.py#L196..  
+00004920: 2020 5669 6577 2063 6f75 6e74 6572 3a0a    View counter:.
+00004930: 2020 2020 6874 7470 733a 2f2f 6769 7468      https://gith
+00004940: 7562 2e63 6f6d 2f76 6567 612f 616c 7461  ub.com/vega/alta
+00004950: 6972 2f62 6c6f 622f 6633 3435 6364 3933  ir/blob/f345cd93
+00004960: 3638 6165 3262 6263 3938 3632 3865 3932  68ae2bbc98628e92
+00004970: 3435 6339 3366 6139 6662 3538 3236 3231  45c93fa9fb582621
+00004980: 2f61 6c74 6169 722f 7665 6761 6c69 7465  /altair/vegalite
+00004990: 2f76 352f 6170 692e 7079 234c 3238 3835  /v5/api.py#L2885
+000049a0: 0a0a 2020 2020 5468 6973 2069 7320 7465  ..    This is te
+000049b0: 6d70 6f72 6172 7920 736f 6c75 7469 6f6e  mporary solution
+000049c0: 2077 6169 7469 6e67 2066 6f72 2061 2066   waiting for a f
+000049d0: 6978 2066 6f72 2074 6869 7320 6973 7375  ix for this issu
+000049e0: 653a 0a20 2020 2068 7474 7073 3a2f 2f67  e:.    https://g
+000049f0: 6974 6875 622e 636f 6d2f 7665 6761 2f61  ithub.com/vega/a
+00004a00: 6c74 6169 722f 6973 7375 6573 2f33 3431  ltair/issues/341
+00004a10: 360a 0a20 2020 204f 7468 6572 2073 6f6c  6..    Other sol
+00004a20: 7574 696f 6e73 2077 6520 636f 6e73 6964  utions we consid
+00004a30: 6572 6564 3a0a 2020 2020 202d 2077 6f72  ered:.     - wor
+00004a40: 6b69 6e67 206f 6e20 7468 6520 6469 6374  king on the dict
+00004a50: 206f 626a 6563 743a 2074 6869 7320 776f   object: this wo
+00004a60: 756c 6420 7265 7175 6972 6520 746f 2069  uld require to i
+00004a70: 7465 7261 7465 2074 6872 6f75 6768 2074  terate through t
+00004a80: 6865 206f 626a 6563 7420 616e 6420 646f  he object and do
+00004a90: 2074 6865 0a20 2020 2020 2020 7361 6d65   the.       same
+00004aa0: 206b 696e 6420 6f66 2072 6570 6c61 6365   kind of replace
+00004ab0: 6d65 6e74 3b20 7468 6f75 6768 2077 6520  ment; though we 
+00004ac0: 776f 756c 6420 6e65 6564 2074 6f20 6b6e  would need to kn
+00004ad0: 6f77 2074 6865 2073 7472 7563 7475 7265  ow the structure
+00004ae0: 2061 6e64 2073 696e 6365 2077 6520 6e65   and since we ne
+00004af0: 6564 0a20 2020 2020 2020 7468 6520 7370  ed.       the sp
+00004b00: 6563 2069 6e20 5374 7269 6e67 2d66 6f72  ec in String-for
+00004b10: 6d61 7420 616e 7977 6179 732c 2077 6520  mat anyways, we 
+00004b20: 6465 656d 6564 2074 6861 7420 6578 6563  deemed that exec
+00004b30: 7574 696e 6720 7468 6520 7265 706c 6163  uting the replac
+00004b40: 656d 656e 7420 6f6e 2074 6865 0a20 2020  ement on the.   
+00004b50: 2020 2020 5374 7269 6e67 2069 7320 7468      String is th
+00004b60: 6520 6265 7474 6572 2061 6c74 6572 6e61  e better alterna
+00004b70: 7469 7665 0a20 2020 2020 2d20 7265 7365  tive.     - rese
+00004b80: 7474 696e 6720 7468 6520 636f 756e 7465  tting the counte
+00004b90: 723a 2074 6865 2063 6f75 6e74 6572 2069  r: the counter i
+00004ba0: 7320 696e 6372 656d 656e 7465 6420 616c  s incremented al
+00004bb0: 7265 6164 7920 7768 656e 2074 6865 2063  ready when the c
+00004bc0: 6861 7274 206f 626a 6563 7420 6973 2063  hart object is c
+00004bd0: 7265 6174 6564 0a20 2020 2020 2020 2873  reated.       (s
+00004be0: 6565 2074 6869 7320 4769 7448 7562 2069  ee this GitHub i
+00004bf0: 7373 7565 2063 6f6d 6d65 6e74 2068 7474  ssue comment htt
+00004c00: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00004c10: 7665 6761 2f61 6c74 6169 722f 6973 7375  vega/altair/issu
+00004c20: 6573 2f33 3431 3623 6973 7375 6563 6f6d  es/3416#issuecom
+00004c30: 6d65 6e74 2d32 3039 3835 3330 3436 3429  ment-2098530464)
+00004c40: 2c0a 2020 2020 2020 2073 6f20 6974 2077  ,.       so it w
+00004c50: 6f75 6c64 2062 6520 746f 6f20 6c61 7465  ould be too late
+00004c60: 2068 6572 6520 746f 2072 6573 6574 2074   here to reset t
+00004c70: 6865 2063 6f75 6e74 6572 2077 6974 6820  he counter with 
+00004c80: 6120 7468 7265 6164 2d6c 6f63 6b20 746f  a thread-lock to
+00004c90: 2070 7265 7665 6e74 2069 6e74 6572 6665   prevent interfe
+00004ca0: 7265 6e63 650a 2020 2020 2020 2062 6574  rence.       bet
+00004cb0: 7765 656e 2073 6573 7369 6f6e 730a 2020  ween sessions.  
+00004cc0: 2020 2222 220a 0a20 2020 2023 2057 6520    """..    # We 
+00004cd0: 6f6e 6c79 2077 616e 7420 746f 2061 7070  only want to app
+00004ce0: 6c79 2074 6865 7365 2072 6570 6c61 6365  ly these replace
+00004cf0: 6d65 6e74 7320 6966 2069 7420 6973 2072  ments if it is r
+00004d00: 6561 6c6c 7920 6e65 6365 7373 6172 790a  eally necessary.
+00004d10: 2020 2020 2320 7369 6e63 6520 7468 6572      # since ther
+00004d20: 6520 6973 2061 2072 6973 6b20 7468 6174  e is a risk that
+00004d30: 2077 6520 7265 706c 6163 6520 6e61 6d65   we replace name
+00004d40: 7320 7468 6174 2077 6865 7265 2063 686f  s that where cho
+00004d50: 7365 6e20 6279 2074 6865 2075 7365 720a  sen by the user.
+00004d60: 2020 2020 2320 616e 6420 7468 6572 6562      # and thereb
+00004d70: 7920 696e 7472 6f64 7563 6520 756e 7761  y introduce unwa
+00004d80: 6e74 6564 2073 6964 6520 6566 6665 6374  nted side effect
+00004d90: 732e 0a0a 2020 2020 2320 5765 206f 6e6c  s...    # We onl
+00004da0: 7920 6e65 6564 2074 6f20 6170 706c 7920  y need to apply 
+00004db0: 7468 6520 7061 7261 6d5f 2066 6978 2069  the param_ fix i
+00004dc0: 6620 7468 6572 6520 6172 6520 6163 7475  f there are actu
+00004dd0: 616c 6c79 2070 6172 616d 6574 6572 7320  ally parameters 
+00004de0: 6465 6669 6e65 640a 2020 2020 2320 736f  defined.    # so
+00004df0: 6d65 7768 6572 6520 696e 2074 6865 2073  mewhere in the s
+00004e00: 7065 632e 2057 6520 6361 6e20 6368 6563  pec. We can chec
+00004e10: 6b20 666f 7220 7468 6973 2062 7920 6c6f  k for this by lo
+00004e20: 6f6b 696e 6720 666f 7220 7468 6520 2722  oking for the '"
+00004e30: 7061 7261 6d73 2227 206b 6579 2e0a 2020  params"' key..  
+00004e40: 2020 2320 5468 6973 2069 736e 2774 2061    # This isn't a
+00004e50: 2070 6572 6665 6374 2063 6865 636b 2c20   perfect check, 
+00004e60: 6275 7420 676f 6f64 2065 6e6f 7567 6820  but good enough 
+00004e70: 746f 2070 7265 7665 6e74 2075 6e6e 6563  to prevent unnec
+00004e80: 6573 7361 7279 2065 7865 6375 7469 6f6e  essary execution
+00004e90: 730a 2020 2020 2320 666f 7220 7468 6520  s.    # for the 
+00004ea0: 6d61 6a6f 7269 7479 206f 6620 6368 6172  majority of char
+00004eb0: 7473 2e0a 2020 2020 6966 2027 2270 6172  ts..    if '"par
+00004ec0: 616d 7322 2720 696e 2076 6567 615f 7370  ams"' in vega_sp
+00004ed0: 6563 3a0a 2020 2020 2020 2020 7665 6761  ec:.        vega
+00004ee0: 5f73 7065 6320 3d20 5f72 6573 6574 5f63  _spec = _reset_c
+00004ef0: 6f75 6e74 6572 5f70 6174 7465 726e 2822  ounter_pattern("
+00004f00: 7061 7261 6d5f 222c 2076 6567 615f 7370  param_", vega_sp
+00004f10: 6563 290a 0a20 2020 2023 2053 696d 706c  ec)..    # Simpl
+00004f20: 6520 6368 6563 6b20 6966 2074 6865 2073  e check if the s
+00004f30: 7065 6320 636f 6e74 6169 6e73 2061 2063  pec contains a c
+00004f40: 6f6d 706f 7369 7465 2063 6861 7274 3a0a  omposite chart:.
+00004f50: 2020 2020 2320 6874 7470 733a 2f2f 7665      # https://ve
+00004f60: 6761 2e67 6974 6875 622e 696f 2f76 6567  ga.github.io/veg
+00004f70: 612d 6c69 7465 2f64 6f63 732f 636f 6d70  a-lite/docs/comp
+00004f80: 6f73 6974 696f 6e2e 6874 6d6c 0a20 2020  osition.html.   
+00004f90: 2023 204f 7468 6572 2063 6861 7274 7320   # Other charts 
+00004fa0: 7769 6c6c 206e 6f74 2063 6f6e 7461 696e  will not contain
+00004fb0: 2074 6865 2060 7669 6577 5f60 206e 616d   the `view_` nam
+00004fc0: 652c 0a20 2020 2023 2073 6f20 6974 7320  e,.    # so its 
+00004fd0: 6265 7474 6572 2074 6f20 6e6f 7420 7265  better to not re
+00004fe0: 706c 6163 6520 7468 6973 2070 6174 7465  place this patte
+00004ff0: 726e 2e0a 2020 2020 6966 2072 652e 7365  rn..    if re.se
+00005000: 6172 6368 2872 2722 2876 636f 6e63 6174  arch(r'"(vconcat
+00005010: 7c68 636f 6e63 6174 7c66 6163 6574 7c6c  |hconcat|facet|l
+00005020: 6179 6572 7c63 6f6e 6361 747c 7265 7065  ayer|concat|repe
+00005030: 6174 2922 272c 2076 6567 615f 7370 6563  at)"', vega_spec
+00005040: 293a 0a20 2020 2020 2020 2076 6567 615f  ):.        vega_
+00005050: 7370 6563 203d 205f 7265 7365 745f 636f  spec = _reset_co
+00005060: 756e 7465 725f 7061 7474 6572 6e28 2276  unter_pattern("v
+00005070: 6965 775f 222c 2076 6567 615f 7370 6563  iew_", vega_spec
+00005080: 290a 2020 2020 7265 7475 726e 2076 6567  ).    return veg
+00005090: 615f 7370 6563 0a0a 0a63 6c61 7373 2056  a_spec...class V
+000050a0: 6567 6143 6861 7274 734d 6978 696e 3a0a  egaChartsMixin:.
+000050b0: 2020 2020 2222 224d 6978 2d69 6e20 636c      """Mix-in cl
+000050c0: 6173 7320 666f 7220 616c 6c20 7665 6761  ass for all vega
+000050d0: 2d72 656c 6174 6564 2063 6861 7274 2063  -related chart c
+000050e0: 6f6d 6d61 6e64 732e 0a0a 2020 2020 416c  ommands...    Al
+000050f0: 7461 6972 2069 7320 6120 7079 7468 6f6e  tair is a python
+00005100: 2077 7261 7070 6572 206f 6e20 746f 7020   wrapper on top 
+00005110: 6f66 2074 6865 2076 6567 612d 6c69 7465  of the vega-lite
+00005120: 2073 7065 632e 2041 6e64 206f 7572 0a20   spec. And our. 
+00005130: 2020 2062 7569 6c74 2d69 6e20 6368 6172     built-in char
+00005140: 7420 636f 6d6d 616e 6473 2061 7265 206a  t commands are j
+00005150: 7573 7420 616e 6f74 6865 7220 6c61 7965  ust another laye
+00005160: 7220 6f6e 2d74 6f70 206f 6620 416c 7461  r on-top of Alta
+00005170: 6972 2e0a 2020 2020 416c 6c20 6f66 2074  ir..    All of t
+00005180: 6865 7365 2063 6861 7274 2063 6f6d 6d61  hese chart comma
+00005190: 6e64 7320 7769 6c6c 2062 6520 6576 656e  nds will be even
+000051a0: 7475 616c 6c79 2063 6f6e 7665 7274 6564  tually converted
+000051b0: 2074 6f20 6120 7665 6761 2d6c 6974 650a   to a vega-lite.
+000051c0: 2020 2020 7370 6563 2061 6e64 2072 656e      spec and ren
+000051d0: 6465 7265 6420 7573 696e 6720 7468 6520  dered using the 
+000051e0: 7361 6d65 2076 6567 612d 6c69 7465 2063  same vega-lite c
+000051f0: 6861 7274 2063 6f6d 706f 6e65 6e74 2e0a  hart component..
+00005200: 2020 2020 2222 220a 0a20 2020 2040 6761      """..    @ga
+00005210: 7468 6572 5f6d 6574 7269 6373 2822 6c69  ther_metrics("li
+00005220: 6e65 5f63 6861 7274 2229 0a20 2020 2064  ne_chart").    d
+00005230: 6566 206c 696e 655f 6368 6172 7428 0a20  ef line_chart(. 
+00005240: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+00005250: 2020 2020 2064 6174 613a 2044 6174 6120       data: Data 
+00005260: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+00005270: 2a2c 0a20 2020 2020 2020 2078 3a20 7374  *,.        x: st
+00005280: 7220 7c20 4e6f 6e65 203d 204e 6f6e 652c  r | None = None,
+00005290: 0a20 2020 2020 2020 2079 3a20 7374 7220  .        y: str 
+000052a0: 7c20 5365 7175 656e 6365 5b73 7472 5d20  | Sequence[str] 
+000052b0: 7c20 4e6f 6e65 203d 204e 6f6e 652c 0a20  | None = None,. 
+000052c0: 2020 2020 2020 2063 6f6c 6f72 3a20 7374         color: st
+000052d0: 7220 7c20 436f 6c6f 7220 7c20 6c69 7374  r | Color | list
+000052e0: 5b43 6f6c 6f72 5d20 7c20 4e6f 6e65 203d  [Color] | None =
+000052f0: 204e 6f6e 652c 0a20 2020 2020 2020 2077   None,.        w
+00005300: 6964 7468 3a20 696e 7420 7c20 4e6f 6e65  idth: int | None
+00005310: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+00005320: 2068 6569 6768 743a 2069 6e74 207c 204e   height: int | N
+00005330: 6f6e 6520 3d20 4e6f 6e65 2c0a 2020 2020  one = None,.    
+00005340: 2020 2020 7573 655f 636f 6e74 6169 6e65      use_containe
+00005350: 725f 7769 6474 683a 2062 6f6f 6c20 3d20  r_width: bool = 
+00005360: 5472 7565 2c0a 2020 2020 2920 2d3e 2044  True,.    ) -> D
+00005370: 656c 7461 4765 6e65 7261 746f 723a 0a20  eltaGenerator:. 
+00005380: 2020 2020 2020 2022 2222 4469 7370 6c61         """Displa
+00005390: 7920 6120 6c69 6e65 2063 6861 7274 2e0a  y a line chart..
+000053a0: 0a20 2020 2020 2020 2054 6869 7320 6973  .        This is
+000053b0: 2073 796e 7461 782d 7375 6761 7220 6172   syntax-sugar ar
+000053c0: 6f75 6e64 2060 6073 742e 616c 7461 6972  ound ``st.altair
+000053d0: 5f63 6861 7274 6060 2e20 5468 6520 6d61  _chart``. The ma
+000053e0: 696e 2064 6966 6665 7265 6e63 650a 2020  in difference.  
+000053f0: 2020 2020 2020 6973 2074 6869 7320 636f        is this co
+00005400: 6d6d 616e 6420 7573 6573 2074 6865 2064  mmand uses the d
+00005410: 6174 6127 7320 6f77 6e20 636f 6c75 6d6e  ata's own column
+00005420: 2061 6e64 2069 6e64 6963 6573 2074 6f20   and indices to 
+00005430: 6669 6775 7265 206f 7574 0a20 2020 2020  figure out.     
+00005440: 2020 2074 6865 2063 6861 7274 2773 2041     the chart's A
+00005450: 6c74 6169 7220 7370 6563 2e20 4173 2061  ltair spec. As a
+00005460: 2072 6573 756c 7420 7468 6973 2069 7320   result this is 
+00005470: 6561 7369 6572 2074 6f20 7573 6520 666f  easier to use fo
+00005480: 7220 6d61 6e79 0a20 2020 2020 2020 2022  r many.        "
+00005490: 6a75 7374 2070 6c6f 7420 7468 6973 2220  just plot this" 
+000054a0: 7363 656e 6172 696f 732c 2077 6869 6c65  scenarios, while
+000054b0: 2062 6569 6e67 206c 6573 7320 6375 7374   being less cust
+000054c0: 6f6d 697a 6162 6c65 2e0a 0a20 2020 2020  omizable...     
+000054d0: 2020 2049 6620 6060 7374 2e6c 696e 655f     If ``st.line_
+000054e0: 6368 6172 7460 6020 646f 6573 206e 6f74  chart`` does not
+000054f0: 2067 7565 7373 2074 6865 2064 6174 6120   guess the data 
+00005500: 7370 6563 6966 6963 6174 696f 6e0a 2020  specification.  
+00005510: 2020 2020 2020 636f 7272 6563 746c 792c        correctly,
+00005520: 2074 7279 2073 7065 6369 6679 696e 6720   try specifying 
+00005530: 796f 7572 2064 6573 6972 6564 2063 6861  your desired cha
+00005540: 7274 2075 7369 6e67 2060 6073 742e 616c  rt using ``st.al
+00005550: 7461 6972 5f63 6861 7274 6060 2e0a 0a20  tair_chart``... 
+00005560: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
+00005570: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
+00005580: 2d2d 2d2d 0a20 2020 2020 2020 2064 6174  ----.        dat
+00005590: 6120 3a20 7061 6e64 6173 2e44 6174 6146  a : pandas.DataF
+000055a0: 7261 6d65 2c20 7061 6e64 6173 2e53 7479  rame, pandas.Sty
+000055b0: 6c65 722c 2070 7961 7272 6f77 2e54 6162  ler, pyarrow.Tab
+000055c0: 6c65 2c20 6e75 6d70 792e 6e64 6172 7261  le, numpy.ndarra
+000055d0: 792c 2070 7973 7061 726b 2e73 716c 2e44  y, pyspark.sql.D
+000055e0: 6174 6146 7261 6d65 2c20 736e 6f77 666c  ataFrame, snowfl
+000055f0: 616b 652e 736e 6f77 7061 726b 2e64 6174  ake.snowpark.dat
+00005600: 6166 7261 6d65 2e44 6174 6146 7261 6d65  aframe.DataFrame
+00005610: 2c20 736e 6f77 666c 616b 652e 736e 6f77  , snowflake.snow
+00005620: 7061 726b 2e74 6162 6c65 2e54 6162 6c65  park.table.Table
+00005630: 2c20 4974 6572 6162 6c65 2c20 6469 6374  , Iterable, dict
+00005640: 206f 7220 4e6f 6e65 0a20 2020 2020 2020   or None.       
+00005650: 2020 2020 2044 6174 6120 746f 2062 6520       Data to be 
+00005660: 706c 6f74 7465 642e 0a0a 2020 2020 2020  plotted...      
+00005670: 2020 7820 3a20 7374 7220 6f72 204e 6f6e    x : str or Non
+00005680: 650a 2020 2020 2020 2020 2020 2020 436f  e.            Co
+00005690: 6c75 6d6e 206e 616d 6520 746f 2075 7365  lumn name to use
+000056a0: 2066 6f72 2074 6865 2078 2d61 7869 732e   for the x-axis.
+000056b0: 2049 6620 4e6f 6e65 2c20 7573 6573 2074   If None, uses t
+000056c0: 6865 2064 6174 6120 696e 6465 7820 666f  he data index fo
+000056d0: 7220 7468 6520 782d 6178 6973 2e0a 0a20  r the x-axis... 
+000056e0: 2020 2020 2020 2079 203a 2073 7472 2c20         y : str, 
+000056f0: 5365 7175 656e 6365 206f 6620 7374 722c  Sequence of str,
+00005700: 206f 7220 4e6f 6e65 0a20 2020 2020 2020   or None.       
+00005710: 2020 2020 2043 6f6c 756d 6e20 6e61 6d65       Column name
+00005720: 2873 2920 746f 2075 7365 2066 6f72 2074  (s) to use for t
+00005730: 6865 2079 2d61 7869 732e 2049 6620 6120  he y-axis. If a 
+00005740: 5365 7175 656e 6365 206f 6620 7374 7269  Sequence of stri
+00005750: 6e67 732c 0a20 2020 2020 2020 2020 2020  ngs,.           
+00005760: 2064 7261 7773 2073 6576 6572 616c 2073   draws several s
+00005770: 6572 6965 7320 6f6e 2074 6865 2073 616d  eries on the sam
+00005780: 6520 6368 6172 7420 6279 206d 656c 7469  e chart by melti
+00005790: 6e67 2079 6f75 7220 7769 6465 2d66 6f72  ng your wide-for
+000057a0: 6d61 740a 2020 2020 2020 2020 2020 2020  mat.            
+000057b0: 7461 626c 6520 696e 746f 2061 206c 6f6e  table into a lon
+000057c0: 672d 666f 726d 6174 2074 6162 6c65 2062  g-format table b
+000057d0: 6568 696e 6420 7468 6520 7363 656e 6573  ehind the scenes
+000057e0: 2e20 4966 204e 6f6e 652c 2064 7261 7773  . If None, draws
+000057f0: 0a20 2020 2020 2020 2020 2020 2074 6865  .            the
+00005800: 2064 6174 6120 6f66 2061 6c6c 2072 656d   data of all rem
+00005810: 6169 6e69 6e67 2063 6f6c 756d 6e73 2061  aining columns a
+00005820: 7320 6461 7461 2073 6572 6965 732e 0a0a  s data series...
+00005830: 2020 2020 2020 2020 636f 6c6f 7220 3a20          color : 
+00005840: 7374 722c 2074 7570 6c65 2c20 5365 7175  str, tuple, Sequ
+00005850: 656e 6365 206f 6620 7374 722c 2053 6571  ence of str, Seq
+00005860: 7565 6e63 6520 6f66 2074 7570 6c65 2c20  uence of tuple, 
+00005870: 6f72 204e 6f6e 650a 2020 2020 2020 2020  or None.        
+00005880: 2020 2020 5468 6520 636f 6c6f 7220 746f      The color to
+00005890: 2075 7365 2066 6f72 2064 6966 6665 7265   use for differe
+000058a0: 6e74 206c 696e 6573 2069 6e20 7468 6973  nt lines in this
+000058b0: 2063 6861 7274 2e0a 0a20 2020 2020 2020   chart...       
+000058c0: 2020 2020 2046 6f72 2061 206c 696e 6520       For a line 
+000058d0: 6368 6172 7420 7769 7468 206a 7573 7420  chart with just 
+000058e0: 6f6e 6520 6c69 6e65 2c20 7468 6973 2063  one line, this c
+000058f0: 616e 2062 653a 0a0a 2020 2020 2020 2020  an be:..        
+00005900: 2020 2020 2a20 4e6f 6e65 2c20 746f 2075      * None, to u
+00005910: 7365 2074 6865 2064 6566 6175 6c74 2063  se the default c
+00005920: 6f6c 6f72 2e0a 2020 2020 2020 2020 2020  olor..          
+00005930: 2020 2a20 4120 6865 7820 7374 7269 6e67    * A hex string
+00005940: 206c 696b 6520 2223 6666 6161 3030 2220   like "#ffaa00" 
+00005950: 6f72 2022 2366 6661 6130 3038 3822 2e0a  or "#ffaa0088"..
+00005960: 2020 2020 2020 2020 2020 2020 2a20 416e              * An
+00005970: 2052 4742 206f 7220 5247 4241 2074 7570   RGB or RGBA tup
+00005980: 6c65 2077 6974 6820 7468 6520 7265 642c  le with the red,
+00005990: 2067 7265 656e 2c20 626c 7565 2c20 616e   green, blue, an
+000059a0: 6420 616c 7068 610a 2020 2020 2020 2020  d alpha.        
+000059b0: 2020 2020 2020 636f 6d70 6f6e 656e 7473        components
+000059c0: 2073 7065 6369 6669 6564 2061 7320 696e   specified as in
+000059d0: 7473 2066 726f 6d20 3020 746f 2032 3535  ts from 0 to 255
+000059e0: 206f 7220 666c 6f61 7473 2066 726f 6d20   or floats from 
+000059f0: 302e 3020 746f 0a20 2020 2020 2020 2020  0.0 to.         
+00005a00: 2020 2020 2031 2e30 2e0a 0a20 2020 2020       1.0...     
+00005a10: 2020 2020 2020 2046 6f72 2061 206c 696e         For a lin
+00005a20: 6520 6368 6172 7420 7769 7468 206d 756c  e chart with mul
+00005a30: 7469 706c 6520 6c69 6e65 732c 2077 6865  tiple lines, whe
+00005a40: 7265 2074 6865 2064 6174 6166 7261 6d65  re the dataframe
+00005a50: 2069 7320 696e 0a20 2020 2020 2020 2020   is in.         
+00005a60: 2020 206c 6f6e 6720 666f 726d 6174 2028     long format (
+00005a70: 7468 6174 2069 732c 2079 2069 7320 4e6f  that is, y is No
+00005a80: 6e65 206f 7220 6a75 7374 206f 6e65 2063  ne or just one c
+00005a90: 6f6c 756d 6e29 2c20 7468 6973 2063 616e  olumn), this can
+00005aa0: 2062 653a 0a0a 2020 2020 2020 2020 2020   be:..          
+00005ab0: 2020 2a20 4e6f 6e65 2c20 746f 2075 7365    * None, to use
+00005ac0: 2074 6865 2064 6566 6175 6c74 2063 6f6c   the default col
+00005ad0: 6f72 732e 0a20 2020 2020 2020 2020 2020  ors..           
+00005ae0: 202a 2054 6865 206e 616d 6520 6f66 2061   * The name of a
+00005af0: 2063 6f6c 756d 6e20 696e 2074 6865 2064   column in the d
+00005b00: 6174 6173 6574 2e20 4461 7461 2070 6f69  ataset. Data poi
+00005b10: 6e74 7320 7769 6c6c 2062 6520 6772 6f75  nts will be grou
+00005b20: 7065 640a 2020 2020 2020 2020 2020 2020  ped.            
+00005b30: 2020 696e 746f 206c 696e 6573 206f 6620    into lines of 
+00005b40: 7468 6520 7361 6d65 2063 6f6c 6f72 2062  the same color b
+00005b50: 6173 6564 206f 6e20 7468 6520 7661 6c75  ased on the valu
+00005b60: 6520 6f66 2074 6869 7320 636f 6c75 6d6e  e of this column
+00005b70: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00005b80: 496e 2061 6464 6974 696f 6e2c 2069 6620  In addition, if 
+00005b90: 7468 6520 7661 6c75 6573 2069 6e20 7468  the values in th
+00005ba0: 6973 2063 6f6c 756d 6e20 6d61 7463 6820  is column match 
+00005bb0: 6f6e 6520 6f66 2074 6865 2063 6f6c 6f72  one of the color
+00005bc0: 0a20 2020 2020 2020 2020 2020 2020 2066  .              f
+00005bd0: 6f72 6d61 7473 2061 626f 7665 2028 6865  ormats above (he
+00005be0: 7820 7374 7269 6e67 206f 7220 636f 6c6f  x string or colo
+00005bf0: 7220 7475 706c 6529 2c20 7468 656e 2074  r tuple), then t
+00005c00: 6861 7420 636f 6c6f 7220 7769 6c6c 0a20  hat color will. 
+00005c10: 2020 2020 2020 2020 2020 2020 2062 6520               be 
+00005c20: 7573 6564 2e0a 0a20 2020 2020 2020 2020  used...         
+00005c30: 2020 2020 2046 6f72 2065 7861 6d70 6c65       For example
+00005c40: 3a20 6966 2074 6865 2064 6174 6173 6574  : if the dataset
+00005c50: 2068 6173 2031 3030 3020 726f 7773 2c20   has 1000 rows, 
+00005c60: 6275 7420 7468 6973 2063 6f6c 756d 6e20  but this column 
+00005c70: 6f6e 6c79 0a20 2020 2020 2020 2020 2020  only.           
+00005c80: 2020 2063 6f6e 7461 696e 7320 7468 6520     contains the 
+00005c90: 7661 6c75 6573 2022 6164 756c 7422 2c20  values "adult", 
+00005ca0: 2263 6869 6c64 222c 2061 6e64 2022 6261  "child", and "ba
+00005cb0: 6279 222c 2074 6865 6e20 7468 6f73 6520  by", then those 
+00005cc0: 3130 3030 0a20 2020 2020 2020 2020 2020  1000.           
+00005cd0: 2020 2064 6174 6170 6f69 6e74 7320 7769     datapoints wi
+00005ce0: 6c6c 2062 6520 6772 6f75 7065 6420 696e  ll be grouped in
+00005cf0: 746f 2074 6872 6565 206c 696e 6573 2077  to three lines w
+00005d00: 686f 7365 2063 6f6c 6f72 7320 7769 6c6c  hose colors will
+00005d10: 2062 650a 2020 2020 2020 2020 2020 2020   be.            
+00005d20: 2020 6175 746f 6d61 7469 6361 6c6c 7920    automatically 
+00005d30: 7365 6c65 6374 6564 2066 726f 6d20 7468  selected from th
+00005d40: 6520 6465 6661 756c 7420 7061 6c65 7474  e default palett
+00005d50: 652e 0a0a 2020 2020 2020 2020 2020 2020  e...            
+00005d60: 2020 4275 742c 2069 6620 666f 7220 7468    But, if for th
+00005d70: 6520 7361 6d65 2031 3030 302d 726f 7720  e same 1000-row 
+00005d80: 6461 7461 7365 742c 2074 6869 7320 636f  dataset, this co
+00005d90: 6c75 6d6e 2063 6f6e 7461 696e 6564 0a20  lumn contained. 
+00005da0: 2020 2020 2020 2020 2020 2020 2074 6865               the
+00005db0: 2076 616c 7565 7320 2223 6666 6161 3030   values "#ffaa00
+00005dc0: 222c 2022 2366 3066 222c 2022 2330 3030  ", "#f0f", "#000
+00005dd0: 3066 6622 2c20 7468 656e 2074 6865 6e20  0ff", then then 
+00005de0: 7468 6f73 6520 3130 3030 0a20 2020 2020  those 1000.     
+00005df0: 2020 2020 2020 2020 2064 6174 6170 6f69           datapoi
+00005e00: 6e74 7320 776f 756c 6420 7374 696c 6c20  nts would still 
+00005e10: 6265 2067 726f 7570 6564 2069 6e74 6f20  be grouped into 
+00005e20: 7468 7265 6520 6c69 6e65 732c 2062 7574  three lines, but
+00005e30: 2074 6865 6972 0a20 2020 2020 2020 2020   their.         
+00005e40: 2020 2020 2063 6f6c 6f72 7320 776f 756c       colors woul
+00005e50: 6420 6265 2022 2366 6661 6130 3022 2c20  d be "#ffaa00", 
+00005e60: 2223 6630 6622 2c20 2223 3030 3030 6666  "#f0f", "#0000ff
+00005e70: 2220 7468 6973 2074 696d 6520 6172 6f75  " this time arou
+00005e80: 6e64 2e0a 0a20 2020 2020 2020 2020 2020  nd...           
+00005e90: 2046 6f72 2061 206c 696e 6520 6368 6172   For a line char
+00005ea0: 7420 7769 7468 206d 756c 7469 706c 6520  t with multiple 
+00005eb0: 6c69 6e65 732c 2077 6865 7265 2074 6865  lines, where the
+00005ec0: 2064 6174 6166 7261 6d65 2069 7320 696e   dataframe is in
+00005ed0: 0a20 2020 2020 2020 2020 2020 2077 6964  .            wid
+00005ee0: 6520 666f 726d 6174 2028 7468 6174 2069  e format (that i
+00005ef0: 732c 2079 2069 7320 6120 5365 7175 656e  s, y is a Sequen
+00005f00: 6365 206f 6620 636f 6c75 6d6e 7329 2c20  ce of columns), 
+00005f10: 7468 6973 2063 616e 2062 653a 0a0a 2020  this can be:..  
+00005f20: 2020 2020 2020 2020 2020 2a20 4e6f 6e65            * None
+00005f30: 2c20 746f 2075 7365 2074 6865 2064 6566  , to use the def
+00005f40: 6175 6c74 2063 6f6c 6f72 732e 0a20 2020  ault colors..   
+00005f50: 2020 2020 2020 2020 202a 2041 206c 6973           * A lis
+00005f60: 7420 6f66 2073 7472 696e 6720 636f 6c6f  t of string colo
+00005f70: 7273 206f 7220 636f 6c6f 7220 7475 706c  rs or color tupl
+00005f80: 6573 2074 6f20 6265 2075 7365 6420 666f  es to be used fo
+00005f90: 7220 6561 6368 206f 660a 2020 2020 2020  r each of.      
+00005fa0: 2020 2020 2020 2020 7468 6520 6c69 6e65          the line
+00005fb0: 7320 696e 2074 6865 2063 6861 7274 2e20  s in the chart. 
+00005fc0: 5468 6973 206c 6973 7420 7368 6f75 6c64  This list should
+00005fd0: 2068 6176 6520 7468 6520 7361 6d65 206c   have the same l
+00005fe0: 656e 6774 680a 2020 2020 2020 2020 2020  ength.          
+00005ff0: 2020 2020 6173 2074 6865 206e 756d 6265      as the numbe
+00006000: 7220 6f66 2079 2076 616c 7565 7320 2865  r of y values (e
+00006010: 2e67 2e20 6060 636f 6c6f 723d 5b22 2366  .g. ``color=["#f
+00006020: 6430 222c 2022 2366 3066 222c 2022 2330  d0", "#f0f", "#0
+00006030: 3466 225d 6060 0a20 2020 2020 2020 2020  4f"]``.         
+00006040: 2020 2020 2066 6f72 2074 6872 6565 206c       for three l
+00006050: 696e 6573 292e 0a0a 2020 2020 2020 2020  ines)...        
+00006060: 7769 6474 6820 3a20 696e 7420 6f72 204e  width : int or N
+00006070: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
+00006080: 4465 7369 7265 6420 7769 6474 6820 6f66  Desired width of
+00006090: 2074 6865 2063 6861 7274 2065 7870 7265   the chart expre
+000060a0: 7373 6564 2069 6e20 7069 7865 6c73 2e20  ssed in pixels. 
+000060b0: 4966 2060 6077 6964 7468 6060 2069 730a  If ``width`` is.
+000060c0: 2020 2020 2020 2020 2020 2020 6060 4e6f              ``No
+000060d0: 6e65 6060 2028 6465 6661 756c 7429 2c20  ne`` (default), 
+000060e0: 5374 7265 616d 6c69 7420 7365 7473 2074  Streamlit sets t
+000060f0: 6865 2077 6964 7468 206f 6620 7468 6520  he width of the 
+00006100: 6368 6172 7420 746f 2066 6974 0a20 2020  chart to fit.   
+00006110: 2020 2020 2020 2020 2069 7473 2063 6f6e           its con
+00006120: 7465 6e74 7320 6163 636f 7264 696e 6720  tents according 
+00006130: 746f 2074 6865 2070 6c6f 7474 696e 6720  to the plotting 
+00006140: 6c69 6272 6172 792c 2075 7020 746f 2074  library, up to t
+00006150: 6865 2077 6964 7468 206f 660a 2020 2020  he width of.    
+00006160: 2020 2020 2020 2020 7468 6520 7061 7265          the pare
+00006170: 6e74 2063 6f6e 7461 696e 6572 2e20 4966  nt container. If
+00006180: 2060 6077 6964 7468 6060 2069 7320 6772   ``width`` is gr
+00006190: 6561 7465 7220 7468 616e 2074 6865 2077  eater than the w
+000061a0: 6964 7468 206f 6620 7468 650a 2020 2020  idth of the.    
+000061b0: 2020 2020 2020 2020 7061 7265 6e74 2063          parent c
+000061c0: 6f6e 7461 696e 6572 2c20 5374 7265 616d  ontainer, Stream
+000061d0: 6c69 7420 7365 7473 2074 6865 2063 6861  lit sets the cha
+000061e0: 7274 2077 6964 7468 2074 6f20 6d61 7463  rt width to matc
+000061f0: 6820 7468 6520 7769 6474 680a 2020 2020  h the width.    
+00006200: 2020 2020 2020 2020 6f66 2074 6865 2070          of the p
+00006210: 6172 656e 7420 636f 6e74 6169 6e65 722e  arent container.
+00006220: 0a0a 2020 2020 2020 2020 6865 6967 6874  ..        height
+00006230: 203a 2069 6e74 206f 7220 4e6f 6e65 0a20   : int or None. 
+00006240: 2020 2020 2020 2020 2020 2044 6573 6972             Desir
+00006250: 6564 2068 6569 6768 7420 6f66 2074 6865  ed height of the
+00006260: 2063 6861 7274 2065 7870 7265 7373 6564   chart expressed
+00006270: 2069 6e20 7069 7865 6c73 2e20 4966 2060   in pixels. If `
+00006280: 6068 6569 6768 7460 6020 6973 0a20 2020  `height`` is.   
+00006290: 2020 2020 2020 2020 2060 604e 6f6e 6560           ``None`
+000062a0: 6020 2864 6566 6175 6c74 292c 2053 7472  ` (default), Str
+000062b0: 6561 6d6c 6974 2073 6574 7320 7468 6520  eamlit sets the 
+000062c0: 6865 6967 6874 206f 6620 7468 6520 6368  height of the ch
+000062d0: 6172 7420 746f 2066 6974 0a20 2020 2020  art to fit.     
+000062e0: 2020 2020 2020 2069 7473 2063 6f6e 7465         its conte
+000062f0: 6e74 7320 6163 636f 7264 696e 6720 746f  nts according to
+00006300: 2074 6865 2070 6c6f 7474 696e 6720 6c69   the plotting li
+00006310: 6272 6172 792e 0a0a 2020 2020 2020 2020  brary...        
+00006320: 7573 655f 636f 6e74 6169 6e65 725f 7769  use_container_wi
+00006330: 6474 6820 3a20 626f 6f6c 0a20 2020 2020  dth : bool.     
+00006340: 2020 2020 2020 2057 6865 7468 6572 2074         Whether t
+00006350: 6f20 6f76 6572 7269 6465 2060 6077 6964  o override ``wid
+00006360: 7468 6060 2077 6974 6820 7468 6520 7769  th`` with the wi
+00006370: 6474 6820 6f66 2074 6865 2070 6172 656e  dth of the paren
+00006380: 740a 2020 2020 2020 2020 2020 2020 636f  t.            co
+00006390: 6e74 6169 6e65 722e 2049 6620 6060 7573  ntainer. If ``us
+000063a0: 655f 636f 6e74 6169 6e65 725f 7769 6474  e_container_widt
+000063b0: 6860 6020 6973 2060 6046 616c 7365 6060  h`` is ``False``
+000063c0: 2028 6465 6661 756c 7429 2c0a 2020 2020   (default),.    
+000063d0: 2020 2020 2020 2020 5374 7265 616d 6c69          Streamli
+000063e0: 7420 7365 7473 2074 6865 2063 6861 7274  t sets the chart
+000063f0: 2773 2077 6964 7468 2061 6363 6f72 6469  's width accordi
+00006400: 6e67 2074 6f20 6060 7769 6474 6860 602e  ng to ``width``.
+00006410: 2049 660a 2020 2020 2020 2020 2020 2020   If.            
+00006420: 6060 7573 655f 636f 6e74 6169 6e65 725f  ``use_container_
+00006430: 7769 6474 6860 6020 6973 2060 6054 7275  width`` is ``Tru
+00006440: 6560 602c 2053 7472 6561 6d6c 6974 2073  e``, Streamlit s
+00006450: 6574 7320 7468 6520 7769 6474 6820 6f66  ets the width of
+00006460: 0a20 2020 2020 2020 2020 2020 2074 6865  .            the
+00006470: 2063 6861 7274 2074 6f20 6d61 7463 6820   chart to match 
+00006480: 7468 6520 7769 6474 6820 6f66 2074 6865  the width of the
+00006490: 2070 6172 656e 7420 636f 6e74 6169 6e65   parent containe
+000064a0: 722e 0a0a 2020 2020 2020 2020 4578 616d  r...        Exam
+000064b0: 706c 6573 0a20 2020 2020 2020 202d 2d2d  ples.        ---
+000064c0: 2d2d 2d2d 2d0a 2020 2020 2020 2020 3e3e  -----.        >>
+000064d0: 3e20 696d 706f 7274 2073 7472 6561 6d6c  > import streaml
+000064e0: 6974 2061 7320 7374 0a20 2020 2020 2020  it as st.       
+000064f0: 203e 3e3e 2069 6d70 6f72 7420 7061 6e64   >>> import pand
+00006500: 6173 2061 7320 7064 0a20 2020 2020 2020  as as pd.       
+00006510: 203e 3e3e 2069 6d70 6f72 7420 6e75 6d70   >>> import nump
+00006520: 7920 6173 206e 700a 2020 2020 2020 2020  y as np.        
+00006530: 3e3e 3e0a 2020 2020 2020 2020 3e3e 3e20  >>>.        >>> 
+00006540: 6368 6172 745f 6461 7461 203d 2070 642e  chart_data = pd.
+00006550: 4461 7461 4672 616d 6528 6e70 2e72 616e  DataFrame(np.ran
+00006560: 646f 6d2e 7261 6e64 6e28 3230 2c20 3329  dom.randn(20, 3)
+00006570: 2c20 636f 6c75 6d6e 733d 5b22 6122 2c20  , columns=["a", 
+00006580: 2262 222c 2022 6322 5d29 0a20 2020 2020  "b", "c"]).     
+00006590: 2020 203e 3e3e 0a20 2020 2020 2020 203e     >>>.        >
+000065a0: 3e3e 2073 742e 6c69 6e65 5f63 6861 7274  >> st.line_chart
+000065b0: 2863 6861 7274 5f64 6174 6129 0a0a 2020  (chart_data)..  
+000065c0: 2020 2020 2020 2e2e 206f 7574 7075 743a        .. output:
+000065d0: 3a0a 2020 2020 2020 2020 2020 2068 7474  :.           htt
+000065e0: 7073 3a2f 2f64 6f63 2d6c 696e 652d 6368  ps://doc-line-ch
+000065f0: 6172 742e 7374 7265 616d 6c69 742e 6170  art.streamlit.ap
+00006600: 702f 0a20 2020 2020 2020 2020 2020 6865  p/.           he
+00006610: 6967 6874 3a20 3434 3070 780a 0a20 2020  ight: 440px..   
+00006620: 2020 2020 2059 6f75 2063 616e 2061 6c73       You can als
+00006630: 6f20 6368 6f6f 7365 2064 6966 6665 7265  o choose differe
+00006640: 6e74 2063 6f6c 756d 6e73 2074 6f20 7573  nt columns to us
+00006650: 6520 666f 7220 7820 616e 6420 792c 2061  e for x and y, a
+00006660: 7320 7765 6c6c 2061 7320 7365 740a 2020  s well as set.  
+00006670: 2020 2020 2020 7468 6520 636f 6c6f 7220        the color 
+00006680: 6479 6e61 6d69 6361 6c6c 7920 6261 7365  dynamically base
+00006690: 6420 6f6e 2061 2033 7264 2063 6f6c 756d  d on a 3rd colum
+000066a0: 6e20 2861 7373 756d 696e 6720 796f 7572  n (assuming your
+000066b0: 2064 6174 6166 7261 6d65 2069 7320 696e   dataframe is in
+000066c0: 0a20 2020 2020 2020 206c 6f6e 6720 666f  .        long fo
+000066d0: 726d 6174 293a 0a0a 2020 2020 2020 2020  rmat):..        
+000066e0: 3e3e 3e20 696d 706f 7274 2073 7472 6561  >>> import strea
+000066f0: 6d6c 6974 2061 7320 7374 0a20 2020 2020  mlit as st.     
+00006700: 2020 203e 3e3e 2069 6d70 6f72 7420 7061     >>> import pa
+00006710: 6e64 6173 2061 7320 7064 0a20 2020 2020  ndas as pd.     
+00006720: 2020 203e 3e3e 2069 6d70 6f72 7420 6e75     >>> import nu
+00006730: 6d70 7920 6173 206e 700a 2020 2020 2020  mpy as np.      
+00006740: 2020 3e3e 3e0a 2020 2020 2020 2020 3e3e    >>>.        >>
+00006750: 3e20 6368 6172 745f 6461 7461 203d 2070  > chart_data = p
+00006760: 642e 4461 7461 4672 616d 6528 0a20 2020  d.DataFrame(.   
+00006770: 2020 2020 202e 2e2e 2020 2020 7b0a 2020       ...    {.  
+00006780: 2020 2020 2020 2e2e 2e20 2020 2020 2020        ...       
+00006790: 2022 636f 6c31 223a 206e 702e 7261 6e64   "col1": np.rand
+000067a0: 6f6d 2e72 616e 646e 2832 3029 2c0a 2020  om.randn(20),.  
+000067b0: 2020 2020 2020 2e2e 2e20 2020 2020 2020        ...       
+000067c0: 2022 636f 6c32 223a 206e 702e 7261 6e64   "col2": np.rand
+000067d0: 6f6d 2e72 616e 646e 2832 3029 2c0a 2020  om.randn(20),.  
+000067e0: 2020 2020 2020 2e2e 2e20 2020 2020 2020        ...       
+000067f0: 2022 636f 6c33 223a 206e 702e 7261 6e64   "col3": np.rand
+00006800: 6f6d 2e63 686f 6963 6528 5b22 4122 2c20  om.choice(["A", 
+00006810: 2242 222c 2022 4322 5d2c 2032 3029 2c0a  "B", "C"], 20),.
+00006820: 2020 2020 2020 2020 2e2e 2e20 2020 207d          ...    }
+00006830: 0a20 2020 2020 2020 202e 2e2e 2029 0a20  .        ... ). 
+00006840: 2020 2020 2020 203e 3e3e 0a20 2020 2020         >>>.     
+00006850: 2020 203e 3e3e 2073 742e 6c69 6e65 5f63     >>> st.line_c
+00006860: 6861 7274 2863 6861 7274 5f64 6174 612c  hart(chart_data,
+00006870: 2078 3d22 636f 6c31 222c 2079 3d22 636f   x="col1", y="co
+00006880: 6c32 222c 2063 6f6c 6f72 3d22 636f 6c33  l2", color="col3
+00006890: 2229 0a0a 2020 2020 2020 2020 2e2e 206f  ")..        .. o
+000068a0: 7574 7075 743a 3a0a 2020 2020 2020 2020  utput::.        
+000068b0: 2020 2068 7474 7073 3a2f 2f64 6f63 2d6c     https://doc-l
+000068c0: 696e 652d 6368 6172 7431 2e73 7472 6561  ine-chart1.strea
+000068d0: 6d6c 6974 2e61 7070 2f0a 2020 2020 2020  mlit.app/.      
+000068e0: 2020 2020 2068 6569 6768 743a 2034 3430       height: 440
+000068f0: 7078 0a0a 2020 2020 2020 2020 4669 6e61  px..        Fina
+00006900: 6c6c 792c 2069 6620 796f 7572 2064 6174  lly, if your dat
+00006910: 6166 7261 6d65 2069 7320 696e 2077 6964  aframe is in wid
+00006920: 6520 666f 726d 6174 2c20 796f 7520 6361  e format, you ca
+00006930: 6e20 6772 6f75 7020 6d75 6c74 6970 6c65  n group multiple
+00006940: 0a20 2020 2020 2020 2063 6f6c 756d 6e73  .        columns
+00006950: 2075 6e64 6572 2074 6865 2079 2061 7267   under the y arg
+00006960: 756d 656e 7420 746f 2073 686f 7720 6d75  ument to show mu
+00006970: 6c74 6970 6c65 206c 696e 6573 2077 6974  ltiple lines wit
+00006980: 6820 6469 6666 6572 656e 740a 2020 2020  h different.    
+00006990: 2020 2020 636f 6c6f 7273 3a0a 0a20 2020      colors:..   
+000069a0: 2020 2020 203e 3e3e 2069 6d70 6f72 7420       >>> import 
+000069b0: 7374 7265 616d 6c69 7420 6173 2073 740a  streamlit as st.
+000069c0: 2020 2020 2020 2020 3e3e 3e20 696d 706f          >>> impo
+000069d0: 7274 2070 616e 6461 7320 6173 2070 640a  rt pandas as pd.
+000069e0: 2020 2020 2020 2020 3e3e 3e20 696d 706f          >>> impo
+000069f0: 7274 206e 756d 7079 2061 7320 6e70 0a20  rt numpy as np. 
+00006a00: 2020 2020 2020 203e 3e3e 0a20 2020 2020         >>>.     
+00006a10: 2020 203e 3e3e 2063 6861 7274 5f64 6174     >>> chart_dat
+00006a20: 6120 3d20 7064 2e44 6174 6146 7261 6d65  a = pd.DataFrame
+00006a30: 286e 702e 7261 6e64 6f6d 2e72 616e 646e  (np.random.randn
+00006a40: 2832 302c 2033 292c 2063 6f6c 756d 6e73  (20, 3), columns
+00006a50: 3d5b 2263 6f6c 3122 2c20 2263 6f6c 3222  =["col1", "col2"
+00006a60: 2c20 2263 6f6c 3322 5d29 0a20 2020 2020  , "col3"]).     
+00006a70: 2020 203e 3e3e 0a20 2020 2020 2020 203e     >>>.        >
+00006a80: 3e3e 2073 742e 6c69 6e65 5f63 6861 7274  >> st.line_chart
+00006a90: 280a 2020 2020 2020 2020 2e2e 2e20 2020  (.        ...   
+00006aa0: 2063 6861 7274 5f64 6174 612c 2078 3d22   chart_data, x="
+00006ab0: 636f 6c31 222c 2079 3d5b 2263 6f6c 3222  col1", y=["col2"
+00006ac0: 2c20 2263 6f6c 3322 5d2c 2063 6f6c 6f72  , "col3"], color
+00006ad0: 3d5b 2223 4646 3030 3030 222c 2022 2330  =["#FF0000", "#0
+00006ae0: 3030 3046 4622 5d20 2023 204f 7074 696f  000FF"]  # Optio
+00006af0: 6e61 6c0a 2020 2020 2020 2020 2e2e 2e20  nal.        ... 
+00006b00: 290a 0a20 2020 2020 2020 202e 2e20 6f75  )..        .. ou
+00006b10: 7470 7574 3a3a 0a20 2020 2020 2020 2020  tput::.         
+00006b20: 2020 6874 7470 733a 2f2f 646f 632d 6c69    https://doc-li
+00006b30: 6e65 2d63 6861 7274 322e 7374 7265 616d  ne-chart2.stream
+00006b40: 6c69 742e 6170 702f 0a20 2020 2020 2020  lit.app/.       
+00006b50: 2020 2020 6865 6967 6874 3a20 3434 3070      height: 440p
+00006b60: 780a 0a20 2020 2020 2020 2022 2222 0a0a  x..        """..
+00006b70: 2020 2020 2020 2020 6368 6172 742c 2061          chart, a
+00006b80: 6464 5f72 6f77 735f 6d65 7461 6461 7461  dd_rows_metadata
+00006b90: 203d 2067 656e 6572 6174 655f 6368 6172   = generate_char
+00006ba0: 7428 0a20 2020 2020 2020 2020 2020 2063  t(.            c
+00006bb0: 6861 7274 5f74 7970 653d 4368 6172 7454  hart_type=ChartT
+00006bc0: 7970 652e 4c49 4e45 2c0a 2020 2020 2020  ype.LINE,.      
+00006bd0: 2020 2020 2020 6461 7461 3d64 6174 612c        data=data,
+00006be0: 0a20 2020 2020 2020 2020 2020 2078 5f66  .            x_f
+00006bf0: 726f 6d5f 7573 6572 3d78 2c0a 2020 2020  rom_user=x,.    
+00006c00: 2020 2020 2020 2020 795f 6672 6f6d 5f75          y_from_u
+00006c10: 7365 723d 792c 0a20 2020 2020 2020 2020  ser=y,.         
+00006c20: 2020 2063 6f6c 6f72 5f66 726f 6d5f 7573     color_from_us
+00006c30: 6572 3d63 6f6c 6f72 2c0a 2020 2020 2020  er=color,.      
+00006c40: 2020 2020 2020 7369 7a65 5f66 726f 6d5f        size_from_
+00006c50: 7573 6572 3d4e 6f6e 652c 0a20 2020 2020  user=None,.     
+00006c60: 2020 2020 2020 2077 6964 7468 3d77 6964         width=wid
+00006c70: 7468 2c0a 2020 2020 2020 2020 2020 2020  th,.            
+00006c80: 6865 6967 6874 3d68 6569 6768 742c 0a20  height=height,. 
+00006c90: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00006ca0: 2072 6574 7572 6e20 6361 7374 280a 2020   return cast(.  
+00006cb0: 2020 2020 2020 2020 2020 2244 656c 7461            "Delta
+00006cc0: 4765 6e65 7261 746f 7222 2c0a 2020 2020  Generator",.    
+00006cd0: 2020 2020 2020 2020 7365 6c66 2e5f 616c          self._al
+00006ce0: 7461 6972 5f63 6861 7274 280a 2020 2020  tair_chart(.    
+00006cf0: 2020 2020 2020 2020 2020 2020 6368 6172              char
+00006d00: 742c 0a20 2020 2020 2020 2020 2020 2020  t,.             
+00006d10: 2020 2075 7365 5f63 6f6e 7461 696e 6572     use_container
+00006d20: 5f77 6964 7468 3d75 7365 5f63 6f6e 7461  _width=use_conta
+00006d30: 696e 6572 5f77 6964 7468 2c0a 2020 2020  iner_width,.    
+00006d40: 2020 2020 2020 2020 2020 2020 7468 656d              them
+00006d50: 653d 2273 7472 6561 6d6c 6974 222c 0a20  e="streamlit",. 
+00006d60: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00006d70: 6464 5f72 6f77 735f 6d65 7461 6461 7461  dd_rows_metadata
+00006d80: 3d61 6464 5f72 6f77 735f 6d65 7461 6461  =add_rows_metada
+00006d90: 7461 2c0a 2020 2020 2020 2020 2020 2020  ta,.            
+00006da0: 292c 0a20 2020 2020 2020 2029 0a0a 2020  ),.        )..  
+00006db0: 2020 4067 6174 6865 725f 6d65 7472 6963    @gather_metric
+00006dc0: 7328 2261 7265 615f 6368 6172 7422 290a  s("area_chart").
+00006dd0: 2020 2020 6465 6620 6172 6561 5f63 6861      def area_cha
+00006de0: 7274 280a 2020 2020 2020 2020 7365 6c66  rt(.        self
+00006df0: 2c0a 2020 2020 2020 2020 6461 7461 3a20  ,.        data: 
+00006e00: 4461 7461 203d 204e 6f6e 652c 0a20 2020  Data = None,.   
+00006e10: 2020 2020 202a 2c0a 2020 2020 2020 2020       *,.        
+00006e20: 783a 2073 7472 207c 204e 6f6e 6520 3d20  x: str | None = 
+00006e30: 4e6f 6e65 2c0a 2020 2020 2020 2020 793a  None,.        y:
+00006e40: 2073 7472 207c 2053 6571 7565 6e63 655b   str | Sequence[
+00006e50: 7374 725d 207c 204e 6f6e 6520 3d20 4e6f  str] | None = No
+00006e60: 6e65 2c0a 2020 2020 2020 2020 636f 6c6f  ne,.        colo
+00006e70: 723a 2073 7472 207c 2043 6f6c 6f72 207c  r: str | Color |
+00006e80: 206c 6973 745b 436f 6c6f 725d 207c 204e   list[Color] | N
+00006e90: 6f6e 6520 3d20 4e6f 6e65 2c0a 2020 2020  one = None,.    
+00006ea0: 2020 2020 7769 6474 683a 2069 6e74 207c      width: int |
+00006eb0: 204e 6f6e 6520 3d20 4e6f 6e65 2c0a 2020   None = None,.  
+00006ec0: 2020 2020 2020 6865 6967 6874 3a20 696e        height: in
+00006ed0: 7420 7c20 4e6f 6e65 203d 204e 6f6e 652c  t | None = None,
+00006ee0: 0a20 2020 2020 2020 2075 7365 5f63 6f6e  .        use_con
+00006ef0: 7461 696e 6572 5f77 6964 7468 3a20 626f  tainer_width: bo
+00006f00: 6f6c 203d 2054 7275 652c 0a20 2020 2029  ol = True,.    )
+00006f10: 202d 3e20 4465 6c74 6147 656e 6572 6174   -> DeltaGenerat
+00006f20: 6f72 3a0a 2020 2020 2020 2020 2222 2244  or:.        """D
+00006f30: 6973 706c 6179 2061 6e20 6172 6561 2063  isplay an area c
+00006f40: 6861 7274 2e0a 0a20 2020 2020 2020 2054  hart...        T
+00006f50: 6869 7320 6973 2073 796e 7461 782d 7375  his is syntax-su
+00006f60: 6761 7220 6172 6f75 6e64 2060 6073 742e  gar around ``st.
+00006f70: 616c 7461 6972 5f63 6861 7274 6060 2e20  altair_chart``. 
+00006f80: 5468 6520 6d61 696e 2064 6966 6665 7265  The main differe
+00006f90: 6e63 650a 2020 2020 2020 2020 6973 2074  nce.        is t
+00006fa0: 6869 7320 636f 6d6d 616e 6420 7573 6573  his command uses
+00006fb0: 2074 6865 2064 6174 6127 7320 6f77 6e20   the data's own 
+00006fc0: 636f 6c75 6d6e 2061 6e64 2069 6e64 6963  column and indic
+00006fd0: 6573 2074 6f20 6669 6775 7265 206f 7574  es to figure out
+00006fe0: 0a20 2020 2020 2020 2074 6865 2063 6861  .        the cha
+00006ff0: 7274 2773 2041 6c74 6169 7220 7370 6563  rt's Altair spec
+00007000: 2e20 4173 2061 2072 6573 756c 7420 7468  . As a result th
+00007010: 6973 2069 7320 6561 7369 6572 2074 6f20  is is easier to 
+00007020: 7573 6520 666f 7220 6d61 6e79 0a20 2020  use for many.   
+00007030: 2020 2020 2022 6a75 7374 2070 6c6f 7420       "just plot 
+00007040: 7468 6973 2220 7363 656e 6172 696f 732c  this" scenarios,
+00007050: 2077 6869 6c65 2062 6569 6e67 206c 6573   while being les
+00007060: 7320 6375 7374 6f6d 697a 6162 6c65 2e0a  s customizable..
+00007070: 0a20 2020 2020 2020 2049 6620 6060 7374  .        If ``st
+00007080: 2e61 7265 615f 6368 6172 7460 6020 646f  .area_chart`` do
+00007090: 6573 206e 6f74 2067 7565 7373 2074 6865  es not guess the
+000070a0: 2064 6174 6120 7370 6563 6966 6963 6174   data specificat
+000070b0: 696f 6e0a 2020 2020 2020 2020 636f 7272  ion.        corr
+000070c0: 6563 746c 792c 2074 7279 2073 7065 6369  ectly, try speci
+000070d0: 6679 696e 6720 796f 7572 2064 6573 6972  fying your desir
+000070e0: 6564 2063 6861 7274 2075 7369 6e67 2060  ed chart using `
+000070f0: 6073 742e 616c 7461 6972 5f63 6861 7274  `st.altair_chart
+00007100: 6060 2e0a 0a20 2020 2020 2020 2050 6172  ``...        Par
+00007110: 616d 6574 6572 730a 2020 2020 2020 2020  ameters.        
+00007120: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
+00007130: 2020 2064 6174 6120 3a20 7061 6e64 6173     data : pandas
+00007140: 2e44 6174 6146 7261 6d65 2c20 7061 6e64  .DataFrame, pand
+00007150: 6173 2e53 7479 6c65 722c 2070 7961 7272  as.Styler, pyarr
+00007160: 6f77 2e54 6162 6c65 2c20 6e75 6d70 792e  ow.Table, numpy.
+00007170: 6e64 6172 7261 792c 2070 7973 7061 726b  ndarray, pyspark
+00007180: 2e73 716c 2e44 6174 6146 7261 6d65 2c20  .sql.DataFrame, 
+00007190: 736e 6f77 666c 616b 652e 736e 6f77 7061  snowflake.snowpa
+000071a0: 726b 2e64 6174 6166 7261 6d65 2e44 6174  rk.dataframe.Dat
+000071b0: 6146 7261 6d65 2c20 736e 6f77 666c 616b  aFrame, snowflak
+000071c0: 652e 736e 6f77 7061 726b 2e74 6162 6c65  e.snowpark.table
+000071d0: 2e54 6162 6c65 2c20 4974 6572 6162 6c65  .Table, Iterable
+000071e0: 2c20 6f72 2064 6963 740a 2020 2020 2020  , or dict.      
+000071f0: 2020 2020 2020 4461 7461 2074 6f20 6265        Data to be
+00007200: 2070 6c6f 7474 6564 2e0a 0a20 2020 2020   plotted...     
+00007210: 2020 2078 203a 2073 7472 206f 7220 4e6f     x : str or No
+00007220: 6e65 0a20 2020 2020 2020 2020 2020 2043  ne.            C
+00007230: 6f6c 756d 6e20 6e61 6d65 2074 6f20 7573  olumn name to us
+00007240: 6520 666f 7220 7468 6520 782d 6178 6973  e for the x-axis
+00007250: 2e20 4966 204e 6f6e 652c 2075 7365 7320  . If None, uses 
+00007260: 7468 6520 6461 7461 2069 6e64 6578 2066  the data index f
+00007270: 6f72 2074 6865 2078 2d61 7869 732e 0a0a  or the x-axis...
+00007280: 2020 2020 2020 2020 7920 3a20 7374 722c          y : str,
+00007290: 2053 6571 7565 6e63 6520 6f66 2073 7472   Sequence of str
+000072a0: 2c20 6f72 204e 6f6e 650a 2020 2020 2020  , or None.      
+000072b0: 2020 2020 2020 436f 6c75 6d6e 206e 616d        Column nam
+000072c0: 6528 7329 2074 6f20 7573 6520 666f 7220  e(s) to use for 
+000072d0: 7468 6520 792d 6178 6973 2e20 4966 2061  the y-axis. If a
+000072e0: 2053 6571 7565 6e63 6520 6f66 2073 7472   Sequence of str
+000072f0: 696e 6773 2c0a 2020 2020 2020 2020 2020  ings,.          
+00007300: 2020 6472 6177 7320 7365 7665 7261 6c20    draws several 
+00007310: 7365 7269 6573 206f 6e20 7468 6520 7361  series on the sa
+00007320: 6d65 2063 6861 7274 2062 7920 6d65 6c74  me chart by melt
+00007330: 696e 6720 796f 7572 2077 6964 652d 666f  ing your wide-fo
+00007340: 726d 6174 0a20 2020 2020 2020 2020 2020  rmat.           
+00007350: 2074 6162 6c65 2069 6e74 6f20 6120 6c6f   table into a lo
+00007360: 6e67 2d66 6f72 6d61 7420 7461 626c 6520  ng-format table 
+00007370: 6265 6869 6e64 2074 6865 2073 6365 6e65  behind the scene
+00007380: 732e 2049 6620 4e6f 6e65 2c20 6472 6177  s. If None, draw
+00007390: 730a 2020 2020 2020 2020 2020 2020 7468  s.            th
+000073a0: 6520 6461 7461 206f 6620 616c 6c20 7265  e data of all re
+000073b0: 6d61 696e 696e 6720 636f 6c75 6d6e 7320  maining columns 
+000073c0: 6173 2064 6174 6120 7365 7269 6573 2e0a  as data series..
+000073d0: 0a20 2020 2020 2020 2063 6f6c 6f72 203a  .        color :
+000073e0: 2073 7472 2c20 7475 706c 652c 2053 6571   str, tuple, Seq
+000073f0: 7565 6e63 6520 6f66 2073 7472 2c20 5365  uence of str, Se
+00007400: 7175 656e 6365 206f 6620 7475 706c 652c  quence of tuple,
+00007410: 206f 7220 4e6f 6e65 0a20 2020 2020 2020   or None.       
+00007420: 2020 2020 2054 6865 2063 6f6c 6f72 2074       The color t
+00007430: 6f20 7573 6520 666f 7220 6469 6666 6572  o use for differ
+00007440: 656e 7420 7365 7269 6573 2069 6e20 7468  ent series in th
+00007450: 6973 2063 6861 7274 2e0a 0a20 2020 2020  is chart...     
+00007460: 2020 2020 2020 2046 6f72 2061 6e20 6172         For an ar
+00007470: 6561 2063 6861 7274 2077 6974 6820 6a75  ea chart with ju
+00007480: 7374 2031 2073 6572 6965 732c 2074 6869  st 1 series, thi
+00007490: 7320 6361 6e20 6265 3a0a 0a20 2020 2020  s can be:..     
+000074a0: 2020 2020 2020 202a 204e 6f6e 652c 2074         * None, t
+000074b0: 6f20 7573 6520 7468 6520 6465 6661 756c  o use the defaul
+000074c0: 7420 636f 6c6f 722e 0a20 2020 2020 2020  t color..       
+000074d0: 2020 2020 202a 2041 2068 6578 2073 7472       * A hex str
+000074e0: 696e 6720 6c69 6b65 2022 2366 6661 6130  ing like "#ffaa0
+000074f0: 3022 206f 7220 2223 6666 6161 3030 3838  0" or "#ffaa0088
+00007500: 222e 0a20 2020 2020 2020 2020 2020 202a  "..            *
+00007510: 2041 6e20 5247 4220 6f72 2052 4742 4120   An RGB or RGBA 
+00007520: 7475 706c 6520 7769 7468 2074 6865 2072  tuple with the r
+00007530: 6564 2c20 6772 6565 6e2c 2062 6c75 652c  ed, green, blue,
+00007540: 2061 6e64 2061 6c70 6861 0a20 2020 2020   and alpha.     
+00007550: 2020 2020 2020 2020 2063 6f6d 706f 6e65           compone
+00007560: 6e74 7320 7370 6563 6966 6965 6420 6173  nts specified as
+00007570: 2069 6e74 7320 6672 6f6d 2030 2074 6f20   ints from 0 to 
+00007580: 3235 3520 6f72 2066 6c6f 6174 7320 6672  255 or floats fr
+00007590: 6f6d 2030 2e30 2074 6f0a 2020 2020 2020  om 0.0 to.      
+000075a0: 2020 2020 2020 2020 312e 302e 0a0a 2020          1.0...  
+000075b0: 2020 2020 2020 2020 2020 466f 7220 616e            For an
+000075c0: 2061 7265 6120 6368 6172 7420 7769 7468   area chart with
+000075d0: 206d 756c 7469 706c 6520 7365 7269 6573   multiple series
+000075e0: 2c20 7768 6572 6520 7468 6520 6461 7461  , where the data
+000075f0: 6672 616d 6520 6973 2069 6e0a 2020 2020  frame is in.    
+00007600: 2020 2020 2020 2020 6c6f 6e67 2066 6f72          long for
+00007610: 6d61 7420 2874 6861 7420 6973 2c20 7920  mat (that is, y 
+00007620: 6973 204e 6f6e 6520 6f72 206a 7573 7420  is None or just 
+00007630: 6f6e 6520 636f 6c75 6d6e 292c 2074 6869  one column), thi
+00007640: 7320 6361 6e20 6265 3a0a 0a20 2020 2020  s can be:..     
+00007650: 2020 2020 2020 202a 204e 6f6e 652c 2074         * None, t
+00007660: 6f20 7573 6520 7468 6520 6465 6661 756c  o use the defaul
+00007670: 7420 636f 6c6f 7273 2e0a 2020 2020 2020  t colors..      
+00007680: 2020 2020 2020 2a20 5468 6520 6e61 6d65        * The name
+00007690: 206f 6620 6120 636f 6c75 6d6e 2069 6e20   of a column in 
+000076a0: 7468 6520 6461 7461 7365 742e 2044 6174  the dataset. Dat
+000076b0: 6120 706f 696e 7473 2077 696c 6c20 6265  a points will be
+000076c0: 2067 726f 7570 6564 0a20 2020 2020 2020   grouped.       
+000076d0: 2020 2020 2020 2069 6e74 6f20 7365 7269         into seri
+000076e0: 6573 206f 6620 7468 6520 7361 6d65 2063  es of the same c
+000076f0: 6f6c 6f72 2062 6173 6564 206f 6e20 7468  olor based on th
+00007700: 6520 7661 6c75 6520 6f66 2074 6869 7320  e value of this 
+00007710: 636f 6c75 6d6e 2e0a 2020 2020 2020 2020  column..        
+00007720: 2020 2020 2020 496e 2061 6464 6974 696f        In additio
+00007730: 6e2c 2069 6620 7468 6520 7661 6c75 6573  n, if the values
+00007740: 2069 6e20 7468 6973 2063 6f6c 756d 6e20   in this column 
+00007750: 6d61 7463 6820 6f6e 6520 6f66 2074 6865  match one of the
+00007760: 2063 6f6c 6f72 0a20 2020 2020 2020 2020   color.         
+00007770: 2020 2020 2066 6f72 6d61 7473 2061 626f       formats abo
+00007780: 7665 2028 6865 7820 7374 7269 6e67 206f  ve (hex string o
+00007790: 7220 636f 6c6f 7220 7475 706c 6529 2c20  r color tuple), 
+000077a0: 7468 656e 2074 6861 7420 636f 6c6f 7220  then that color 
+000077b0: 7769 6c6c 0a20 2020 2020 2020 2020 2020  will.           
+000077c0: 2020 2062 6520 7573 6564 2e0a 0a20 2020     be used...   
+000077d0: 2020 2020 2020 2020 2020 2046 6f72 2065             For e
+000077e0: 7861 6d70 6c65 3a20 6966 2074 6865 2064  xample: if the d
+000077f0: 6174 6173 6574 2068 6173 2031 3030 3020  ataset has 1000 
+00007800: 726f 7773 2c20 6275 7420 7468 6973 2063  rows, but this c
+00007810: 6f6c 756d 6e20 6f6e 6c79 0a20 2020 2020  olumn only.     
+00007820: 2020 2020 2020 2020 2063 6f6e 7461 696e           contain
+00007830: 7320 7468 6520 7661 6c75 6573 2022 6164  s the values "ad
+00007840: 756c 7422 2c20 2263 6869 6c64 222c 2061  ult", "child", a
+00007850: 6e64 2022 6261 6279 222c 2074 6865 6e20  nd "baby", then 
+00007860: 7468 6f73 6520 3130 3030 0a20 2020 2020  those 1000.     
+00007870: 2020 2020 2020 2020 2064 6174 6170 6f69           datapoi
+00007880: 6e74 7320 7769 6c6c 2062 6520 6772 6f75  nts will be grou
+00007890: 7065 6420 696e 746f 2074 6872 6565 2073  ped into three s
+000078a0: 6572 6965 7320 7768 6f73 6520 636f 6c6f  eries whose colo
+000078b0: 7273 2077 696c 6c20 6265 0a20 2020 2020  rs will be.     
+000078c0: 2020 2020 2020 2020 2061 7574 6f6d 6174           automat
+000078d0: 6963 616c 6c79 2073 656c 6563 7465 6420  ically selected 
+000078e0: 6672 6f6d 2074 6865 2064 6566 6175 6c74  from the default
+000078f0: 2070 616c 6574 7465 2e0a 0a20 2020 2020   palette...     
+00007900: 2020 2020 2020 2020 2042 7574 2c20 6966           But, if
+00007910: 2066 6f72 2074 6865 2073 616d 6520 3130   for the same 10
+00007920: 3030 2d72 6f77 2064 6174 6173 6574 2c20  00-row dataset, 
+00007930: 7468 6973 2063 6f6c 756d 6e20 636f 6e74  this column cont
+00007940: 6169 6e65 640a 2020 2020 2020 2020 2020  ained.          
+00007950: 2020 2020 7468 6520 7661 6c75 6573 2022      the values "
+00007960: 2366 6661 6130 3022 2c20 2223 6630 6622  #ffaa00", "#f0f"
+00007970: 2c20 2223 3030 3030 6666 222c 2074 6865  , "#0000ff", the
+00007980: 6e20 7468 656e 2074 686f 7365 2031 3030  n then those 100
+00007990: 300a 2020 2020 2020 2020 2020 2020 2020  0.              
+000079a0: 6461 7461 706f 696e 7473 2077 6f75 6c64  datapoints would
+000079b0: 2073 7469 6c6c 2062 6520 6772 6f75 7065   still be groupe
+000079c0: 6420 696e 746f 2033 2073 6572 6965 732c  d into 3 series,
+000079d0: 2062 7574 2074 6865 6972 0a20 2020 2020   but their.     
+000079e0: 2020 2020 2020 2020 2063 6f6c 6f72 7320           colors 
+000079f0: 776f 756c 6420 6265 2022 2366 6661 6130  would be "#ffaa0
+00007a00: 3022 2c20 2223 6630 6622 2c20 2223 3030  0", "#f0f", "#00
+00007a10: 3030 6666 2220 7468 6973 2074 696d 6520  00ff" this time 
+00007a20: 6172 6f75 6e64 2e0a 0a20 2020 2020 2020  around...       
+00007a30: 2020 2020 2046 6f72 2061 6e20 6172 6561       For an area
+00007a40: 2063 6861 7274 2077 6974 6820 6d75 6c74   chart with mult
+00007a50: 6970 6c65 2073 6572 6965 732c 2077 6865  iple series, whe
+00007a60: 7265 2074 6865 2064 6174 6166 7261 6d65  re the dataframe
+00007a70: 2069 7320 696e 0a20 2020 2020 2020 2020   is in.         
+00007a80: 2020 2077 6964 6520 666f 726d 6174 2028     wide format (
+00007a90: 7468 6174 2069 732c 2079 2069 7320 6120  that is, y is a 
+00007aa0: 5365 7175 656e 6365 206f 6620 636f 6c75  Sequence of colu
+00007ab0: 6d6e 7329 2c20 7468 6973 2063 616e 2062  mns), this can b
+00007ac0: 653a 0a0a 2020 2020 2020 2020 2020 2020  e:..            
+00007ad0: 2a20 4e6f 6e65 2c20 746f 2075 7365 2074  * None, to use t
+00007ae0: 6865 2064 6566 6175 6c74 2063 6f6c 6f72  he default color
+00007af0: 732e 0a20 2020 2020 2020 2020 2020 202a  s..            *
+00007b00: 2041 206c 6973 7420 6f66 2073 7472 696e   A list of strin
+00007b10: 6720 636f 6c6f 7273 206f 7220 636f 6c6f  g colors or colo
+00007b20: 7220 7475 706c 6573 2074 6f20 6265 2075  r tuples to be u
+00007b30: 7365 6420 666f 7220 6561 6368 206f 660a  sed for each of.
+00007b40: 2020 2020 2020 2020 2020 2020 2020 7468                th
+00007b50: 6520 7365 7269 6573 2069 6e20 7468 6520  e series in the 
+00007b60: 6368 6172 742e 2054 6869 7320 6c69 7374  chart. This list
+00007b70: 2073 686f 756c 6420 6861 7665 2074 6865   should have the
+00007b80: 2073 616d 6520 6c65 6e67 7468 0a20 2020   same length.   
+00007b90: 2020 2020 2020 2020 2020 2061 7320 7468             as th
+00007ba0: 6520 6e75 6d62 6572 206f 6620 7920 7661  e number of y va
+00007bb0: 6c75 6573 2028 652e 672e 2060 6063 6f6c  lues (e.g. ``col
+00007bc0: 6f72 3d5b 2223 6664 3022 2c20 2223 6630  or=["#fd0", "#f0
+00007bd0: 6622 2c20 2223 3034 6622 5d60 600a 2020  f", "#04f"]``.  
+00007be0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00007bf0: 7468 7265 6520 6c69 6e65 7329 2e0a 0a20  three lines)... 
+00007c00: 2020 2020 2020 2077 6964 7468 203a 2069         width : i
+00007c10: 6e74 206f 7220 4e6f 6e65 0a20 2020 2020  nt or None.     
+00007c20: 2020 2020 2020 2044 6573 6972 6564 2077         Desired w
+00007c30: 6964 7468 206f 6620 7468 6520 6368 6172  idth of the char
+00007c40: 7420 6578 7072 6573 7365 6420 696e 2070  t expressed in p
+00007c50: 6978 656c 732e 2049 6620 6060 7769 6474  ixels. If ``widt
+00007c60: 6860 6020 6973 0a20 2020 2020 2020 2020  h`` is.         
+00007c70: 2020 2060 604e 6f6e 6560 6020 2864 6566     ``None`` (def
+00007c80: 6175 6c74 292c 2053 7472 6561 6d6c 6974  ault), Streamlit
+00007c90: 2073 6574 7320 7468 6520 7769 6474 6820   sets the width 
+00007ca0: 6f66 2074 6865 2063 6861 7274 2074 6f20  of the chart to 
+00007cb0: 6669 740a 2020 2020 2020 2020 2020 2020  fit.            
+00007cc0: 6974 7320 636f 6e74 656e 7473 2061 6363  its contents acc
+00007cd0: 6f72 6469 6e67 2074 6f20 7468 6520 706c  ording to the pl
+00007ce0: 6f74 7469 6e67 206c 6962 7261 7279 2c20  otting library, 
+00007cf0: 7570 2074 6f20 7468 6520 7769 6474 6820  up to the width 
+00007d00: 6f66 0a20 2020 2020 2020 2020 2020 2074  of.            t
+00007d10: 6865 2070 6172 656e 7420 636f 6e74 6169  he parent contai
+00007d20: 6e65 722e 2049 6620 6060 7769 6474 6860  ner. If ``width`
+00007d30: 6020 6973 2067 7265 6174 6572 2074 6861  ` is greater tha
+00007d40: 6e20 7468 6520 7769 6474 6820 6f66 2074  n the width of t
+00007d50: 6865 0a20 2020 2020 2020 2020 2020 2070  he.            p
+00007d60: 6172 656e 7420 636f 6e74 6169 6e65 722c  arent container,
+00007d70: 2053 7472 6561 6d6c 6974 2073 6574 7320   Streamlit sets 
+00007d80: 7468 6520 6368 6172 7420 7769 6474 6820  the chart width 
+00007d90: 746f 206d 6174 6368 2074 6865 2077 6964  to match the wid
+00007da0: 7468 0a20 2020 2020 2020 2020 2020 206f  th.            o
+00007db0: 6620 7468 6520 7061 7265 6e74 2063 6f6e  f the parent con
+00007dc0: 7461 696e 6572 2e0a 0a20 2020 2020 2020  tainer...       
+00007dd0: 2068 6569 6768 7420 3a20 696e 7420 6f72   height : int or
+00007de0: 204e 6f6e 650a 2020 2020 2020 2020 2020   None.          
+00007df0: 2020 4465 7369 7265 6420 6865 6967 6874    Desired height
+00007e00: 206f 6620 7468 6520 6368 6172 7420 6578   of the chart ex
+00007e10: 7072 6573 7365 6420 696e 2070 6978 656c  pressed in pixel
+00007e20: 732e 2049 6620 6060 6865 6967 6874 6060  s. If ``height``
+00007e30: 2069 730a 2020 2020 2020 2020 2020 2020   is.            
+00007e40: 6060 4e6f 6e65 6060 2028 6465 6661 756c  ``None`` (defaul
+00007e50: 7429 2c20 5374 7265 616d 6c69 7420 7365  t), Streamlit se
+00007e60: 7473 2074 6865 2068 6569 6768 7420 6f66  ts the height of
+00007e70: 2074 6865 2063 6861 7274 2074 6f20 6669   the chart to fi
+00007e80: 740a 2020 2020 2020 2020 2020 2020 6974  t.            it
+00007e90: 7320 636f 6e74 656e 7473 2061 6363 6f72  s contents accor
+00007ea0: 6469 6e67 2074 6f20 7468 6520 706c 6f74  ding to the plot
+00007eb0: 7469 6e67 206c 6962 7261 7279 2e0a 0a20  ting library... 
+00007ec0: 2020 2020 2020 2075 7365 5f63 6f6e 7461         use_conta
+00007ed0: 696e 6572 5f77 6964 7468 203a 2062 6f6f  iner_width : boo
+00007ee0: 6c0a 2020 2020 2020 2020 2020 2020 5768  l.            Wh
+00007ef0: 6574 6865 7220 746f 206f 7665 7272 6964  ether to overrid
+00007f00: 6520 6060 7769 6474 6860 6020 7769 7468  e ``width`` with
+00007f10: 2074 6865 2077 6964 7468 206f 6620 7468   the width of th
+00007f20: 6520 7061 7265 6e74 0a20 2020 2020 2020  e parent.       
+00007f30: 2020 2020 2063 6f6e 7461 696e 6572 2e20       container. 
+00007f40: 4966 2060 6075 7365 5f63 6f6e 7461 696e  If ``use_contain
+00007f50: 6572 5f77 6964 7468 6060 2069 7320 6060  er_width`` is ``
+00007f60: 4661 6c73 6560 6020 2864 6566 6175 6c74  False`` (default
+00007f70: 292c 0a20 2020 2020 2020 2020 2020 2053  ),.            S
+00007f80: 7472 6561 6d6c 6974 2073 6574 7320 7468  treamlit sets th
+00007f90: 6520 6368 6172 7427 7320 7769 6474 6820  e chart's width 
+00007fa0: 6163 636f 7264 696e 6720 746f 2060 6077  according to ``w
+00007fb0: 6964 7468 6060 2e20 4966 0a20 2020 2020  idth``. If.     
+00007fc0: 2020 2020 2020 2060 6075 7365 5f63 6f6e         ``use_con
+00007fd0: 7461 696e 6572 5f77 6964 7468 6060 2069  tainer_width`` i
+00007fe0: 7320 6060 5472 7565 6060 2c20 5374 7265  s ``True``, Stre
+00007ff0: 616d 6c69 7420 7365 7473 2074 6865 2077  amlit sets the w
+00008000: 6964 7468 206f 660a 2020 2020 2020 2020  idth of.        
+00008010: 2020 2020 7468 6520 6368 6172 7420 746f      the chart to
+00008020: 206d 6174 6368 2074 6865 2077 6964 7468   match the width
+00008030: 206f 6620 7468 6520 7061 7265 6e74 2063   of the parent c
+00008040: 6f6e 7461 696e 6572 2e0a 0a20 2020 2020  ontainer...     
+00008050: 2020 2045 7861 6d70 6c65 730a 2020 2020     Examples.    
+00008060: 2020 2020 2d2d 2d2d 2d2d 2d2d 0a20 2020      --------.   
+00008070: 2020 2020 203e 3e3e 2069 6d70 6f72 7420       >>> import 
+00008080: 7374 7265 616d 6c69 7420 6173 2073 740a  streamlit as st.
+00008090: 2020 2020 2020 2020 3e3e 3e20 696d 706f          >>> impo
+000080a0: 7274 2070 616e 6461 7320 6173 2070 640a  rt pandas as pd.
+000080b0: 2020 2020 2020 2020 3e3e 3e20 696d 706f          >>> impo
+000080c0: 7274 206e 756d 7079 2061 7320 6e70 0a20  rt numpy as np. 
+000080d0: 2020 2020 2020 203e 3e3e 0a20 2020 2020         >>>.     
+000080e0: 2020 203e 3e3e 2063 6861 7274 5f64 6174     >>> chart_dat
+000080f0: 6120 3d20 7064 2e44 6174 6146 7261 6d65  a = pd.DataFrame
+00008100: 286e 702e 7261 6e64 6f6d 2e72 616e 646e  (np.random.randn
+00008110: 2832 302c 2033 292c 2063 6f6c 756d 6e73  (20, 3), columns
+00008120: 3d5b 2261 222c 2022 6222 2c20 2263 225d  =["a", "b", "c"]
+00008130: 290a 2020 2020 2020 2020 3e3e 3e0a 2020  ).        >>>.  
+00008140: 2020 2020 2020 3e3e 3e20 7374 2e61 7265        >>> st.are
+00008150: 615f 6368 6172 7428 6368 6172 745f 6461  a_chart(chart_da
+00008160: 7461 290a 0a20 2020 2020 2020 202e 2e20  ta)..        .. 
+00008170: 6f75 7470 7574 3a3a 0a20 2020 2020 2020  output::.       
+00008180: 2020 2020 6874 7470 733a 2f2f 646f 632d      https://doc-
+00008190: 6172 6561 2d63 6861 7274 2e73 7472 6561  area-chart.strea
+000081a0: 6d6c 6974 2e61 7070 2f0a 2020 2020 2020  mlit.app/.      
+000081b0: 2020 2020 2068 6569 6768 743a 2034 3430       height: 440
+000081c0: 7078 0a0a 2020 2020 2020 2020 596f 7520  px..        You 
+000081d0: 6361 6e20 616c 736f 2063 686f 6f73 6520  can also choose 
+000081e0: 6469 6666 6572 656e 7420 636f 6c75 6d6e  different column
+000081f0: 7320 746f 2075 7365 2066 6f72 2078 2061  s to use for x a
+00008200: 6e64 2079 2c20 6173 2077 656c 6c20 6173  nd y, as well as
+00008210: 2073 6574 0a20 2020 2020 2020 2074 6865   set.        the
+00008220: 2063 6f6c 6f72 2064 796e 616d 6963 616c   color dynamical
+00008230: 6c79 2062 6173 6564 206f 6e20 6120 3372  ly based on a 3r
+00008240: 6420 636f 6c75 6d6e 2028 6173 7375 6d69  d column (assumi
+00008250: 6e67 2079 6f75 7220 6461 7461 6672 616d  ng your datafram
+00008260: 6520 6973 2069 6e0a 2020 2020 2020 2020  e is in.        
+00008270: 6c6f 6e67 2066 6f72 6d61 7429 3a0a 0a20  long format):.. 
+00008280: 2020 2020 2020 203e 3e3e 2069 6d70 6f72         >>> impor
+00008290: 7420 7374 7265 616d 6c69 7420 6173 2073  t streamlit as s
+000082a0: 740a 2020 2020 2020 2020 3e3e 3e20 696d  t.        >>> im
+000082b0: 706f 7274 2070 616e 6461 7320 6173 2070  port pandas as p
+000082c0: 640a 2020 2020 2020 2020 3e3e 3e20 696d  d.        >>> im
+000082d0: 706f 7274 206e 756d 7079 2061 7320 6e70  port numpy as np
+000082e0: 0a20 2020 2020 2020 203e 3e3e 0a20 2020  .        >>>.   
+000082f0: 2020 2020 203e 3e3e 2063 6861 7274 5f64       >>> chart_d
+00008300: 6174 6120 3d20 7064 2e44 6174 6146 7261  ata = pd.DataFra
+00008310: 6d65 280a 2020 2020 2020 2020 2e2e 2e20  me(.        ... 
+00008320: 2020 207b 0a20 2020 2020 2020 202e 2e2e     {.        ...
+00008330: 2020 2020 2020 2020 2263 6f6c 3122 3a20          "col1": 
+00008340: 6e70 2e72 616e 646f 6d2e 7261 6e64 6e28  np.random.randn(
+00008350: 3230 292c 0a20 2020 2020 2020 202e 2e2e  20),.        ...
+00008360: 2020 2020 2020 2020 2263 6f6c 3222 3a20          "col2": 
+00008370: 6e70 2e72 616e 646f 6d2e 7261 6e64 6e28  np.random.randn(
+00008380: 3230 292c 0a20 2020 2020 2020 202e 2e2e  20),.        ...
+00008390: 2020 2020 2020 2020 2263 6f6c 3322 3a20          "col3": 
+000083a0: 6e70 2e72 616e 646f 6d2e 6368 6f69 6365  np.random.choice
+000083b0: 285b 2241 222c 2022 4222 2c20 2243 225d  (["A", "B", "C"]
+000083c0: 2c20 3230 292c 0a20 2020 2020 2020 202e  , 20),.        .
+000083d0: 2e2e 2020 2020 7d0a 2020 2020 2020 2020  ..    }.        
+000083e0: 2e2e 2e20 290a 2020 2020 2020 2020 3e3e  ... ).        >>
+000083f0: 3e0a 2020 2020 2020 2020 3e3e 3e20 7374  >.        >>> st
+00008400: 2e61 7265 615f 6368 6172 7428 6368 6172  .area_chart(char
+00008410: 745f 6461 7461 2c20 783d 2263 6f6c 3122  t_data, x="col1"
+00008420: 2c20 793d 2263 6f6c 3222 2c20 636f 6c6f  , y="col2", colo
+00008430: 723d 2263 6f6c 3322 290a 0a20 2020 2020  r="col3")..     
+00008440: 2020 202e 2e20 6f75 7470 7574 3a3a 0a20     .. output::. 
+00008450: 2020 2020 2020 2020 2020 6874 7470 733a            https:
+00008460: 2f2f 646f 632d 6172 6561 2d63 6861 7274  //doc-area-chart
+00008470: 312e 7374 7265 616d 6c69 742e 6170 702f  1.streamlit.app/
+00008480: 0a20 2020 2020 2020 2020 2020 6865 6967  .           heig
+00008490: 6874 3a20 3434 3070 780a 0a20 2020 2020  ht: 440px..     
+000084a0: 2020 2046 696e 616c 6c79 2c20 6966 2079     Finally, if y
+000084b0: 6f75 7220 6461 7461 6672 616d 6520 6973  our dataframe is
+000084c0: 2069 6e20 7769 6465 2066 6f72 6d61 742c   in wide format,
+000084d0: 2079 6f75 2063 616e 2067 726f 7570 206d   you can group m
+000084e0: 756c 7469 706c 650a 2020 2020 2020 2020  ultiple.        
+000084f0: 636f 6c75 6d6e 7320 756e 6465 7220 7468  columns under th
+00008500: 6520 7920 6172 6775 6d65 6e74 2074 6f20  e y argument to 
+00008510: 7368 6f77 206d 756c 7469 706c 6520 7365  show multiple se
+00008520: 7269 6573 2077 6974 6820 6469 6666 6572  ries with differ
+00008530: 656e 740a 2020 2020 2020 2020 636f 6c6f  ent.        colo
+00008540: 7273 3a0a 0a20 2020 2020 2020 203e 3e3e  rs:..        >>>
+00008550: 2069 6d70 6f72 7420 7374 7265 616d 6c69   import streamli
+00008560: 7420 6173 2073 740a 2020 2020 2020 2020  t as st.        
+00008570: 3e3e 3e20 696d 706f 7274 2070 616e 6461  >>> import panda
+00008580: 7320 6173 2070 640a 2020 2020 2020 2020  s as pd.        
+00008590: 3e3e 3e20 696d 706f 7274 206e 756d 7079  >>> import numpy
+000085a0: 2061 7320 6e70 0a20 2020 2020 2020 203e   as np.        >
+000085b0: 3e3e 0a20 2020 2020 2020 203e 3e3e 2063  >>.        >>> c
+000085c0: 6861 7274 5f64 6174 6120 3d20 7064 2e44  hart_data = pd.D
+000085d0: 6174 6146 7261 6d65 286e 702e 7261 6e64  ataFrame(np.rand
+000085e0: 6f6d 2e72 616e 646e 2832 302c 2033 292c  om.randn(20, 3),
+000085f0: 2063 6f6c 756d 6e73 3d5b 2263 6f6c 3122   columns=["col1"
+00008600: 2c20 2263 6f6c 3222 2c20 2263 6f6c 3322  , "col2", "col3"
+00008610: 5d29 0a20 2020 2020 2020 203e 3e3e 0a20  ]).        >>>. 
+00008620: 2020 2020 2020 203e 3e3e 2073 742e 6172         >>> st.ar
+00008630: 6561 5f63 6861 7274 280a 2020 2020 2020  ea_chart(.      
+00008640: 2020 2e2e 2e20 2020 2063 6861 7274 5f64    ...    chart_d
+00008650: 6174 612c 2078 3d22 636f 6c31 222c 2079  ata, x="col1", y
+00008660: 3d5b 2263 6f6c 3222 2c20 2263 6f6c 3322  =["col2", "col3"
+00008670: 5d2c 2063 6f6c 6f72 3d5b 2223 4646 3030  ], color=["#FF00
+00008680: 3030 222c 2022 2330 3030 3046 4622 5d20  00", "#0000FF"] 
+00008690: 2023 204f 7074 696f 6e61 6c0a 2020 2020   # Optional.    
+000086a0: 2020 2020 2e2e 2e20 290a 0a20 2020 2020      ... )..     
+000086b0: 2020 202e 2e20 6f75 7470 7574 3a3a 0a20     .. output::. 
+000086c0: 2020 2020 2020 2020 2020 6874 7470 733a            https:
+000086d0: 2f2f 646f 632d 6172 6561 2d63 6861 7274  //doc-area-chart
+000086e0: 322e 7374 7265 616d 6c69 742e 6170 702f  2.streamlit.app/
+000086f0: 0a20 2020 2020 2020 2020 2020 6865 6967  .           heig
+00008700: 6874 3a20 3434 3070 780a 0a20 2020 2020  ht: 440px..     
+00008710: 2020 2022 2222 0a0a 2020 2020 2020 2020     """..        
+00008720: 6368 6172 742c 2061 6464 5f72 6f77 735f  chart, add_rows_
+00008730: 6d65 7461 6461 7461 203d 2067 656e 6572  metadata = gener
+00008740: 6174 655f 6368 6172 7428 0a20 2020 2020  ate_chart(.     
+00008750: 2020 2020 2020 2063 6861 7274 5f74 7970         chart_typ
+00008760: 653d 4368 6172 7454 7970 652e 4152 4541  e=ChartType.AREA
+00008770: 2c0a 2020 2020 2020 2020 2020 2020 6461  ,.            da
+00008780: 7461 3d64 6174 612c 0a20 2020 2020 2020  ta=data,.       
+00008790: 2020 2020 2078 5f66 726f 6d5f 7573 6572       x_from_user
+000087a0: 3d78 2c0a 2020 2020 2020 2020 2020 2020  =x,.            
+000087b0: 795f 6672 6f6d 5f75 7365 723d 792c 0a20  y_from_user=y,. 
+000087c0: 2020 2020 2020 2020 2020 2063 6f6c 6f72             color
+000087d0: 5f66 726f 6d5f 7573 6572 3d63 6f6c 6f72  _from_user=color
+000087e0: 2c0a 2020 2020 2020 2020 2020 2020 7369  ,.            si
+000087f0: 7a65 5f66 726f 6d5f 7573 6572 3d4e 6f6e  ze_from_user=Non
+00008800: 652c 0a20 2020 2020 2020 2020 2020 2077  e,.            w
+00008810: 6964 7468 3d77 6964 7468 2c0a 2020 2020  idth=width,.    
+00008820: 2020 2020 2020 2020 6865 6967 6874 3d68          height=h
+00008830: 6569 6768 742c 0a20 2020 2020 2020 2029  eight,.        )
+00008840: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00008850: 6361 7374 280a 2020 2020 2020 2020 2020  cast(.          
+00008860: 2020 2244 656c 7461 4765 6e65 7261 746f    "DeltaGenerato
+00008870: 7222 2c0a 2020 2020 2020 2020 2020 2020  r",.            
+00008880: 7365 6c66 2e5f 616c 7461 6972 5f63 6861  self._altair_cha
+00008890: 7274 280a 2020 2020 2020 2020 2020 2020  rt(.            
+000088a0: 2020 2020 6368 6172 742c 0a20 2020 2020      chart,.     
+000088b0: 2020 2020 2020 2020 2020 2075 7365 5f63             use_c
+000088c0: 6f6e 7461 696e 6572 5f77 6964 7468 3d75  ontainer_width=u
+000088d0: 7365 5f63 6f6e 7461 696e 6572 5f77 6964  se_container_wid
+000088e0: 7468 2c0a 2020 2020 2020 2020 2020 2020  th,.            
+000088f0: 2020 2020 7468 656d 653d 2273 7472 6561      theme="strea
+00008900: 6d6c 6974 222c 0a20 2020 2020 2020 2020  mlit",.         
+00008910: 2020 2020 2020 2061 6464 5f72 6f77 735f         add_rows_
+00008920: 6d65 7461 6461 7461 3d61 6464 5f72 6f77  metadata=add_row
+00008930: 735f 6d65 7461 6461 7461 2c0a 2020 2020  s_metadata,.    
+00008940: 2020 2020 2020 2020 292c 0a20 2020 2020          ),.     
+00008950: 2020 2029 0a0a 2020 2020 4067 6174 6865     )..    @gathe
+00008960: 725f 6d65 7472 6963 7328 2262 6172 5f63  r_metrics("bar_c
+00008970: 6861 7274 2229 0a20 2020 2064 6566 2062  hart").    def b
+00008980: 6172 5f63 6861 7274 280a 2020 2020 2020  ar_chart(.      
+00008990: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
+000089a0: 6461 7461 3a20 4461 7461 203d 204e 6f6e  data: Data = Non
+000089b0: 652c 0a20 2020 2020 2020 202a 2c0a 2020  e,.        *,.  
+000089c0: 2020 2020 2020 783a 2073 7472 207c 204e        x: str | N
+000089d0: 6f6e 6520 3d20 4e6f 6e65 2c0a 2020 2020  one = None,.    
+000089e0: 2020 2020 793a 2073 7472 207c 2053 6571      y: str | Seq
+000089f0: 7565 6e63 655b 7374 725d 207c 204e 6f6e  uence[str] | Non
+00008a00: 6520 3d20 4e6f 6e65 2c0a 2020 2020 2020  e = None,.      
+00008a10: 2020 636f 6c6f 723a 2073 7472 207c 2043    color: str | C
+00008a20: 6f6c 6f72 207c 206c 6973 745b 436f 6c6f  olor | list[Colo
+00008a30: 725d 207c 204e 6f6e 6520 3d20 4e6f 6e65  r] | None = None
+00008a40: 2c0a 2020 2020 2020 2020 7769 6474 683a  ,.        width:
+00008a50: 2069 6e74 207c 204e 6f6e 6520 3d20 4e6f   int | None = No
+00008a60: 6e65 2c0a 2020 2020 2020 2020 6865 6967  ne,.        heig
+00008a70: 6874 3a20 696e 7420 7c20 4e6f 6e65 203d  ht: int | None =
+00008a80: 204e 6f6e 652c 0a20 2020 2020 2020 2075   None,.        u
+00008a90: 7365 5f63 6f6e 7461 696e 6572 5f77 6964  se_container_wid
+00008aa0: 7468 3a20 626f 6f6c 203d 2054 7275 652c  th: bool = True,
+00008ab0: 0a20 2020 2029 202d 3e20 4465 6c74 6147  .    ) -> DeltaG
+00008ac0: 656e 6572 6174 6f72 3a0a 2020 2020 2020  enerator:.      
+00008ad0: 2020 2222 2244 6973 706c 6179 2061 2062    """Display a b
+00008ae0: 6172 2063 6861 7274 2e0a 0a20 2020 2020  ar chart...     
+00008af0: 2020 2054 6869 7320 6973 2073 796e 7461     This is synta
+00008b00: 782d 7375 6761 7220 6172 6f75 6e64 2060  x-sugar around `
+00008b10: 6073 742e 616c 7461 6972 5f63 6861 7274  `st.altair_chart
+00008b20: 6060 2e20 5468 6520 6d61 696e 2064 6966  ``. The main dif
+00008b30: 6665 7265 6e63 650a 2020 2020 2020 2020  ference.        
+00008b40: 6973 2074 6869 7320 636f 6d6d 616e 6420  is this command 
+00008b50: 7573 6573 2074 6865 2064 6174 6127 7320  uses the data's 
+00008b60: 6f77 6e20 636f 6c75 6d6e 2061 6e64 2069  own column and i
+00008b70: 6e64 6963 6573 2074 6f20 6669 6775 7265  ndices to figure
+00008b80: 206f 7574 0a20 2020 2020 2020 2074 6865   out.        the
+00008b90: 2063 6861 7274 2773 2041 6c74 6169 7220   chart's Altair 
+00008ba0: 7370 6563 2e20 4173 2061 2072 6573 756c  spec. As a resul
+00008bb0: 7420 7468 6973 2069 7320 6561 7369 6572  t this is easier
+00008bc0: 2074 6f20 7573 6520 666f 7220 6d61 6e79   to use for many
+00008bd0: 0a20 2020 2020 2020 2022 6a75 7374 2070  .        "just p
+00008be0: 6c6f 7420 7468 6973 2220 7363 656e 6172  lot this" scenar
+00008bf0: 696f 732c 2077 6869 6c65 2062 6569 6e67  ios, while being
+00008c00: 206c 6573 7320 6375 7374 6f6d 697a 6162   less customizab
+00008c10: 6c65 2e0a 0a20 2020 2020 2020 2049 6620  le...        If 
+00008c20: 6060 7374 2e62 6172 5f63 6861 7274 6060  ``st.bar_chart``
+00008c30: 2064 6f65 7320 6e6f 7420 6775 6573 7320   does not guess 
+00008c40: 7468 6520 6461 7461 2073 7065 6369 6669  the data specifi
+00008c50: 6361 7469 6f6e 0a20 2020 2020 2020 2063  cation.        c
+00008c60: 6f72 7265 6374 6c79 2c20 7472 7920 7370  orrectly, try sp
+00008c70: 6563 6966 7969 6e67 2079 6f75 7220 6465  ecifying your de
+00008c80: 7369 7265 6420 6368 6172 7420 7573 696e  sired chart usin
+00008c90: 6720 6060 7374 2e61 6c74 6169 725f 6368  g ``st.altair_ch
+00008ca0: 6172 7460 602e 0a0a 2020 2020 2020 2020  art``...        
+00008cb0: 5061 7261 6d65 7465 7273 0a20 2020 2020  Parameters.     
+00008cc0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
+00008cd0: 2020 2020 2020 6461 7461 203a 2070 616e        data : pan
+00008ce0: 6461 732e 4461 7461 4672 616d 652c 2070  das.DataFrame, p
+00008cf0: 616e 6461 732e 5374 796c 6572 2c20 7079  andas.Styler, py
+00008d00: 6172 726f 772e 5461 626c 652c 206e 756d  arrow.Table, num
+00008d10: 7079 2e6e 6461 7272 6179 2c20 7079 7370  py.ndarray, pysp
+00008d20: 6172 6b2e 7371 6c2e 4461 7461 4672 616d  ark.sql.DataFram
+00008d30: 652c 2073 6e6f 7766 6c61 6b65 2e73 6e6f  e, snowflake.sno
+00008d40: 7770 6172 6b2e 6461 7461 6672 616d 652e  wpark.dataframe.
+00008d50: 4461 7461 4672 616d 652c 2073 6e6f 7766  DataFrame, snowf
+00008d60: 6c61 6b65 2e73 6e6f 7770 6172 6b2e 7461  lake.snowpark.ta
+00008d70: 626c 652e 5461 626c 652c 2049 7465 7261  ble.Table, Itera
+00008d80: 626c 652c 206f 7220 6469 6374 0a20 2020  ble, or dict.   
+00008d90: 2020 2020 2020 2020 2044 6174 6120 746f           Data to
+00008da0: 2062 6520 706c 6f74 7465 642e 0a0a 2020   be plotted...  
+00008db0: 2020 2020 2020 7820 3a20 7374 7220 6f72        x : str or
+00008dc0: 204e 6f6e 650a 2020 2020 2020 2020 2020   None.          
+00008dd0: 2020 436f 6c75 6d6e 206e 616d 6520 746f    Column name to
+00008de0: 2075 7365 2066 6f72 2074 6865 2078 2d61   use for the x-a
+00008df0: 7869 732e 2049 6620 4e6f 6e65 2c20 7573  xis. If None, us
+00008e00: 6573 2074 6865 2064 6174 6120 696e 6465  es the data inde
+00008e10: 7820 666f 7220 7468 6520 782d 6178 6973  x for the x-axis
+00008e20: 2e0a 0a20 2020 2020 2020 2079 203a 2073  ...        y : s
+00008e30: 7472 2c20 5365 7175 656e 6365 206f 6620  tr, Sequence of 
+00008e40: 7374 722c 206f 7220 4e6f 6e65 0a20 2020  str, or None.   
+00008e50: 2020 2020 2020 2020 2043 6f6c 756d 6e20           Column 
+00008e60: 6e61 6d65 2873 2920 746f 2075 7365 2066  name(s) to use f
+00008e70: 6f72 2074 6865 2079 2d61 7869 732e 2049  or the y-axis. I
+00008e80: 6620 6120 5365 7175 656e 6365 206f 6620  f a Sequence of 
+00008e90: 7374 7269 6e67 732c 0a20 2020 2020 2020  strings,.       
+00008ea0: 2020 2020 2064 7261 7773 2073 6576 6572       draws sever
+00008eb0: 616c 2073 6572 6965 7320 6f6e 2074 6865  al series on the
+00008ec0: 2073 616d 6520 6368 6172 7420 6279 206d   same chart by m
+00008ed0: 656c 7469 6e67 2079 6f75 7220 7769 6465  elting your wide
+00008ee0: 2d66 6f72 6d61 740a 2020 2020 2020 2020  -format.        
+00008ef0: 2020 2020 7461 626c 6520 696e 746f 2061      table into a
+00008f00: 206c 6f6e 672d 666f 726d 6174 2074 6162   long-format tab
+00008f10: 6c65 2062 6568 696e 6420 7468 6520 7363  le behind the sc
+00008f20: 656e 6573 2e20 4966 204e 6f6e 652c 2064  enes. If None, d
+00008f30: 7261 7773 0a20 2020 2020 2020 2020 2020  raws.           
+00008f40: 2074 6865 2064 6174 6120 6f66 2061 6c6c   the data of all
+00008f50: 2072 656d 6169 6e69 6e67 2063 6f6c 756d   remaining colum
+00008f60: 6e73 2061 7320 6461 7461 2073 6572 6965  ns as data serie
+00008f70: 732e 0a0a 2020 2020 2020 2020 636f 6c6f  s...        colo
+00008f80: 7220 3a20 7374 722c 2074 7570 6c65 2c20  r : str, tuple, 
+00008f90: 5365 7175 656e 6365 206f 6620 7374 722c  Sequence of str,
+00008fa0: 2053 6571 7565 6e63 6520 6f66 2074 7570   Sequence of tup
+00008fb0: 6c65 2c20 6f72 204e 6f6e 650a 2020 2020  le, or None.    
+00008fc0: 2020 2020 2020 2020 5468 6520 636f 6c6f          The colo
+00008fd0: 7220 746f 2075 7365 2066 6f72 2064 6966  r to use for dif
+00008fe0: 6665 7265 6e74 2073 6572 6965 7320 696e  ferent series in
+00008ff0: 2074 6869 7320 6368 6172 742e 0a0a 2020   this chart...  
+00009000: 2020 2020 2020 2020 2020 466f 7220 6120            For a 
+00009010: 6261 7220 6368 6172 7420 7769 7468 206a  bar chart with j
+00009020: 7573 7420 6f6e 6520 7365 7269 6573 2c20  ust one series, 
+00009030: 7468 6973 2063 616e 2062 653a 0a0a 2020  this can be:..  
+00009040: 2020 2020 2020 2020 2020 2a20 4e6f 6e65            * None
+00009050: 2c20 746f 2075 7365 2074 6865 2064 6566  , to use the def
+00009060: 6175 6c74 2063 6f6c 6f72 2e0a 2020 2020  ault color..    
+00009070: 2020 2020 2020 2020 2a20 4120 6865 7820          * A hex 
+00009080: 7374 7269 6e67 206c 696b 6520 2223 6666  string like "#ff
+00009090: 6161 3030 2220 6f72 2022 2366 6661 6130  aa00" or "#ffaa0
+000090a0: 3038 3822 2e0a 2020 2020 2020 2020 2020  088"..          
+000090b0: 2020 2a20 416e 2052 4742 206f 7220 5247    * An RGB or RG
+000090c0: 4241 2074 7570 6c65 2077 6974 6820 7468  BA tuple with th
+000090d0: 6520 7265 642c 2067 7265 656e 2c20 626c  e red, green, bl
+000090e0: 7565 2c20 616e 6420 616c 7068 610a 2020  ue, and alpha.  
+000090f0: 2020 2020 2020 2020 2020 2020 636f 6d70              comp
+00009100: 6f6e 656e 7473 2073 7065 6369 6669 6564  onents specified
+00009110: 2061 7320 696e 7473 2066 726f 6d20 3020   as ints from 0 
+00009120: 746f 2032 3535 206f 7220 666c 6f61 7473  to 255 or floats
+00009130: 2066 726f 6d20 302e 3020 746f 0a20 2020   from 0.0 to.   
+00009140: 2020 2020 2020 2020 2020 2031 2e30 2e0a             1.0..
+00009150: 0a20 2020 2020 2020 2020 2020 2046 6f72  .            For
+00009160: 2061 2062 6172 2063 6861 7274 2077 6974   a bar chart wit
+00009170: 6820 6d75 6c74 6970 6c65 2073 6572 6965  h multiple serie
+00009180: 732c 2077 6865 7265 2074 6865 2064 6174  s, where the dat
+00009190: 6166 7261 6d65 2069 7320 696e 0a20 2020  aframe is in.   
+000091a0: 2020 2020 2020 2020 206c 6f6e 6720 666f           long fo
+000091b0: 726d 6174 2028 7468 6174 2069 732c 2079  rmat (that is, y
+000091c0: 2069 7320 4e6f 6e65 206f 7220 6a75 7374   is None or just
+000091d0: 206f 6e65 2063 6f6c 756d 6e29 2c20 7468   one column), th
+000091e0: 6973 2063 616e 2062 653a 0a0a 2020 2020  is can be:..    
+000091f0: 2020 2020 2020 2020 2a20 4e6f 6e65 2c20          * None, 
+00009200: 746f 2075 7365 2074 6865 2064 6566 6175  to use the defau
+00009210: 6c74 2063 6f6c 6f72 732e 0a20 2020 2020  lt colors..     
+00009220: 2020 2020 2020 202a 2054 6865 206e 616d         * The nam
+00009230: 6520 6f66 2061 2063 6f6c 756d 6e20 696e  e of a column in
+00009240: 2074 6865 2064 6174 6173 6574 2e20 4461   the dataset. Da
+00009250: 7461 2070 6f69 6e74 7320 7769 6c6c 2062  ta points will b
+00009260: 6520 6772 6f75 7065 640a 2020 2020 2020  e grouped.      
+00009270: 2020 2020 2020 2020 696e 746f 2073 6572          into ser
+00009280: 6965 7320 6f66 2074 6865 2073 616d 6520  ies of the same 
+00009290: 636f 6c6f 7220 6261 7365 6420 6f6e 2074  color based on t
+000092a0: 6865 2076 616c 7565 206f 6620 7468 6973  he value of this
+000092b0: 2063 6f6c 756d 6e2e 0a20 2020 2020 2020   column..       
+000092c0: 2020 2020 2020 2049 6e20 6164 6469 7469         In additi
+000092d0: 6f6e 2c20 6966 2074 6865 2076 616c 7565  on, if the value
+000092e0: 7320 696e 2074 6869 7320 636f 6c75 6d6e  s in this column
+000092f0: 206d 6174 6368 206f 6e65 206f 6620 7468   match one of th
+00009300: 6520 636f 6c6f 720a 2020 2020 2020 2020  e color.        
+00009310: 2020 2020 2020 666f 726d 6174 7320 6162        formats ab
+00009320: 6f76 6520 2868 6578 2073 7472 696e 6720  ove (hex string 
+00009330: 6f72 2063 6f6c 6f72 2074 7570 6c65 292c  or color tuple),
+00009340: 2074 6865 6e20 7468 6174 2063 6f6c 6f72   then that color
+00009350: 2077 696c 6c0a 2020 2020 2020 2020 2020   will.          
+00009360: 2020 2020 6265 2075 7365 642e 0a0a 2020      be used...  
+00009370: 2020 2020 2020 2020 2020 2020 466f 7220              For 
+00009380: 6578 616d 706c 653a 2069 6620 7468 6520  example: if the 
+00009390: 6461 7461 7365 7420 6861 7320 3130 3030  dataset has 1000
+000093a0: 2072 6f77 732c 2062 7574 2074 6869 7320   rows, but this 
+000093b0: 636f 6c75 6d6e 206f 6e6c 790a 2020 2020  column only.    
+000093c0: 2020 2020 2020 2020 2020 636f 6e74 6169            contai
+000093d0: 6e73 2074 6865 2076 616c 7565 7320 2261  ns the values "a
+000093e0: 6475 6c74 222c 2022 6368 696c 6422 2c20  dult", "child", 
+000093f0: 616e 6420 2262 6162 7922 2c20 7468 656e  and "baby", then
+00009400: 2074 686f 7365 2031 3030 300a 2020 2020   those 1000.    
+00009410: 2020 2020 2020 2020 2020 6461 7461 706f            datapo
+00009420: 696e 7473 2077 696c 6c20 6265 2067 726f  ints will be gro
+00009430: 7570 6564 2069 6e74 6f20 7468 7265 6520  uped into three 
+00009440: 7365 7269 6573 2077 686f 7365 2063 6f6c  series whose col
+00009450: 6f72 7320 7769 6c6c 2062 650a 2020 2020  ors will be.    
+00009460: 2020 2020 2020 2020 2020 6175 746f 6d61            automa
+00009470: 7469 6361 6c6c 7920 7365 6c65 6374 6564  tically selected
+00009480: 2066 726f 6d20 7468 6520 6465 6661 756c   from the defaul
+00009490: 7420 7061 6c65 7474 652e 0a0a 2020 2020  t palette...    
+000094a0: 2020 2020 2020 2020 2020 4275 742c 2069            But, i
+000094b0: 6620 666f 7220 7468 6520 7361 6d65 2031  f for the same 1
+000094c0: 3030 302d 726f 7720 6461 7461 7365 742c  000-row dataset,
+000094d0: 2074 6869 7320 636f 6c75 6d6e 2063 6f6e   this column con
+000094e0: 7461 696e 6564 0a20 2020 2020 2020 2020  tained.         
+000094f0: 2020 2020 2074 6865 2076 616c 7565 7320       the values 
+00009500: 2223 6666 6161 3030 222c 2022 2366 3066  "#ffaa00", "#f0f
+00009510: 222c 2022 2330 3030 3066 6622 2c20 7468  ", "#0000ff", th
+00009520: 656e 2074 6865 6e20 7468 6f73 6520 3130  en then those 10
+00009530: 3030 0a20 2020 2020 2020 2020 2020 2020  00.             
+00009540: 2064 6174 6170 6f69 6e74 7320 776f 756c   datapoints woul
+00009550: 6420 7374 696c 6c20 6265 2067 726f 7570  d still be group
+00009560: 6564 2069 6e74 6f20 3320 7365 7269 6573  ed into 3 series
+00009570: 2c20 6275 7420 7468 6569 720a 2020 2020  , but their.    
+00009580: 2020 2020 2020 2020 2020 636f 6c6f 7273            colors
+00009590: 2077 6f75 6c64 2062 6520 2223 6666 6161   would be "#ffaa
+000095a0: 3030 222c 2022 2366 3066 222c 2022 2330  00", "#f0f", "#0
+000095b0: 3030 3066 6622 2074 6869 7320 7469 6d65  000ff" this time
+000095c0: 2061 726f 756e 642e 0a0a 2020 2020 2020   around...      
+000095d0: 2020 2020 2020 466f 7220 6120 6261 7220        For a bar 
+000095e0: 6368 6172 7420 7769 7468 206d 756c 7469  chart with multi
+000095f0: 706c 6520 7365 7269 6573 2c20 7768 6572  ple series, wher
+00009600: 6520 7468 6520 6461 7461 6672 616d 6520  e the dataframe 
+00009610: 6973 2069 6e0a 2020 2020 2020 2020 2020  is in.          
+00009620: 2020 7769 6465 2066 6f72 6d61 7420 2874    wide format (t
+00009630: 6861 7420 6973 2c20 7920 6973 2061 2053  hat is, y is a S
+00009640: 6571 7565 6e63 6520 6f66 2063 6f6c 756d  equence of colum
+00009650: 6e73 292c 2074 6869 7320 6361 6e20 6265  ns), this can be
+00009660: 3a0a 0a20 2020 2020 2020 2020 2020 202a  :..            *
+00009670: 204e 6f6e 652c 2074 6f20 7573 6520 7468   None, to use th
+00009680: 6520 6465 6661 756c 7420 636f 6c6f 7273  e default colors
+00009690: 2e0a 2020 2020 2020 2020 2020 2020 2a20  ..            * 
+000096a0: 4120 6c69 7374 206f 6620 7374 7269 6e67  A list of string
+000096b0: 2063 6f6c 6f72 7320 6f72 2063 6f6c 6f72   colors or color
+000096c0: 2074 7570 6c65 7320 746f 2062 6520 7573   tuples to be us
+000096d0: 6564 2066 6f72 2065 6163 6820 6f66 0a20  ed for each of. 
+000096e0: 2020 2020 2020 2020 2020 2020 2074 6865               the
+000096f0: 2073 6572 6965 7320 696e 2074 6865 2063   series in the c
+00009700: 6861 7274 2e20 5468 6973 206c 6973 7420  hart. This list 
+00009710: 7368 6f75 6c64 2068 6176 6520 7468 6520  should have the 
+00009720: 7361 6d65 206c 656e 6774 680a 2020 2020  same length.    
+00009730: 2020 2020 2020 2020 2020 6173 2074 6865            as the
+00009740: 206e 756d 6265 7220 6f66 2079 2076 616c   number of y val
+00009750: 7565 7320 2865 2e67 2e20 6060 636f 6c6f  ues (e.g. ``colo
+00009760: 723d 5b22 2366 6430 222c 2022 2366 3066  r=["#fd0", "#f0f
+00009770: 222c 2022 2330 3466 225d 6060 0a20 2020  ", "#04f"]``.   
+00009780: 2020 2020 2020 2020 2020 2066 6f72 2074             for t
+00009790: 6872 6565 206c 696e 6573 292e 0a0a 2020  hree lines)...  
+000097a0: 2020 2020 2020 7769 6474 6820 3a20 696e        width : in
+000097b0: 7420 6f72 204e 6f6e 650a 2020 2020 2020  t or None.      
+000097c0: 2020 2020 2020 4465 7369 7265 6420 7769        Desired wi
+000097d0: 6474 6820 6f66 2074 6865 2063 6861 7274  dth of the chart
+000097e0: 2065 7870 7265 7373 6564 2069 6e20 7069   expressed in pi
+000097f0: 7865 6c73 2e20 4966 2060 6077 6964 7468  xels. If ``width
+00009800: 6060 2069 730a 2020 2020 2020 2020 2020  `` is.          
+00009810: 2020 6060 4e6f 6e65 6060 2028 6465 6661    ``None`` (defa
+00009820: 756c 7429 2c20 5374 7265 616d 6c69 7420  ult), Streamlit 
+00009830: 7365 7473 2074 6865 2077 6964 7468 206f  sets the width o
+00009840: 6620 7468 6520 6368 6172 7420 746f 2066  f the chart to f
+00009850: 6974 0a20 2020 2020 2020 2020 2020 2069  it.            i
+00009860: 7473 2063 6f6e 7465 6e74 7320 6163 636f  ts contents acco
+00009870: 7264 696e 6720 746f 2074 6865 2070 6c6f  rding to the plo
+00009880: 7474 696e 6720 6c69 6272 6172 792c 2075  tting library, u
+00009890: 7020 746f 2074 6865 2077 6964 7468 206f  p to the width o
+000098a0: 660a 2020 2020 2020 2020 2020 2020 7468  f.            th
+000098b0: 6520 7061 7265 6e74 2063 6f6e 7461 696e  e parent contain
+000098c0: 6572 2e20 4966 2060 6077 6964 7468 6060  er. If ``width``
+000098d0: 2069 7320 6772 6561 7465 7220 7468 616e   is greater than
+000098e0: 2074 6865 2077 6964 7468 206f 6620 7468   the width of th
+000098f0: 650a 2020 2020 2020 2020 2020 2020 7061  e.            pa
+00009900: 7265 6e74 2063 6f6e 7461 696e 6572 2c20  rent container, 
+00009910: 5374 7265 616d 6c69 7420 7365 7473 2074  Streamlit sets t
+00009920: 6865 2063 6861 7274 2077 6964 7468 2074  he chart width t
+00009930: 6f20 6d61 7463 6820 7468 6520 7769 6474  o match the widt
+00009940: 680a 2020 2020 2020 2020 2020 2020 6f66  h.            of
+00009950: 2074 6865 2070 6172 656e 7420 636f 6e74   the parent cont
+00009960: 6169 6e65 722e 0a0a 2020 2020 2020 2020  ainer...        
+00009970: 6865 6967 6874 203a 2069 6e74 206f 7220  height : int or 
+00009980: 4e6f 6e65 0a20 2020 2020 2020 2020 2020  None.           
+00009990: 2044 6573 6972 6564 2068 6569 6768 7420   Desired height 
+000099a0: 6f66 2074 6865 2063 6861 7274 2065 7870  of the chart exp
+000099b0: 7265 7373 6564 2069 6e20 7069 7865 6c73  ressed in pixels
+000099c0: 2e20 4966 2060 6068 6569 6768 7460 6020  . If ``height`` 
+000099d0: 6973 0a20 2020 2020 2020 2020 2020 2060  is.            `
+000099e0: 604e 6f6e 6560 6020 2864 6566 6175 6c74  `None`` (default
+000099f0: 292c 2053 7472 6561 6d6c 6974 2073 6574  ), Streamlit set
+00009a00: 7320 7468 6520 6865 6967 6874 206f 6620  s the height of 
+00009a10: 7468 6520 6368 6172 7420 746f 2066 6974  the chart to fit
+00009a20: 0a20 2020 2020 2020 2020 2020 2069 7473  .            its
+00009a30: 2063 6f6e 7465 6e74 7320 6163 636f 7264   contents accord
+00009a40: 696e 6720 746f 2074 6865 2070 6c6f 7474  ing to the plott
+00009a50: 696e 6720 6c69 6272 6172 792e 0a0a 2020  ing library...  
+00009a60: 2020 2020 2020 7573 655f 636f 6e74 6169        use_contai
+00009a70: 6e65 725f 7769 6474 6820 3a20 626f 6f6c  ner_width : bool
+00009a80: 0a20 2020 2020 2020 2020 2020 2057 6865  .            Whe
+00009a90: 7468 6572 2074 6f20 6f76 6572 7269 6465  ther to override
+00009aa0: 2060 6077 6964 7468 6060 2077 6974 6820   ``width`` with 
+00009ab0: 7468 6520 7769 6474 6820 6f66 2074 6865  the width of the
+00009ac0: 2070 6172 656e 740a 2020 2020 2020 2020   parent.        
+00009ad0: 2020 2020 636f 6e74 6169 6e65 722e 2049      container. I
+00009ae0: 6620 6060 7573 655f 636f 6e74 6169 6e65  f ``use_containe
+00009af0: 725f 7769 6474 6860 6020 6973 2060 6046  r_width`` is ``F
+00009b00: 616c 7365 6060 2028 6465 6661 756c 7429  alse`` (default)
+00009b10: 2c0a 2020 2020 2020 2020 2020 2020 5374  ,.            St
+00009b20: 7265 616d 6c69 7420 7365 7473 2074 6865  reamlit sets the
+00009b30: 2063 6861 7274 2773 2077 6964 7468 2061   chart's width a
+00009b40: 6363 6f72 6469 6e67 2074 6f20 6060 7769  ccording to ``wi
+00009b50: 6474 6860 602e 2049 660a 2020 2020 2020  dth``. If.      
+00009b60: 2020 2020 2020 6060 7573 655f 636f 6e74        ``use_cont
+00009b70: 6169 6e65 725f 7769 6474 6860 6020 6973  ainer_width`` is
+00009b80: 2060 6054 7275 6560 602c 2053 7472 6561   ``True``, Strea
+00009b90: 6d6c 6974 2073 6574 7320 7468 6520 7769  mlit sets the wi
+00009ba0: 6474 6820 6f66 0a20 2020 2020 2020 2020  dth of.         
+00009bb0: 2020 2074 6865 2063 6861 7274 2074 6f20     the chart to 
+00009bc0: 6d61 7463 6820 7468 6520 7769 6474 6820  match the width 
+00009bd0: 6f66 2074 6865 2070 6172 656e 7420 636f  of the parent co
+00009be0: 6e74 6169 6e65 722e 0a0a 2020 2020 2020  ntainer...      
+00009bf0: 2020 4578 616d 706c 6573 0a20 2020 2020    Examples.     
+00009c00: 2020 202d 2d2d 2d2d 2d2d 2d0a 2020 2020     --------.    
+00009c10: 2020 2020 3e3e 3e20 696d 706f 7274 2073      >>> import s
+00009c20: 7472 6561 6d6c 6974 2061 7320 7374 0a20  treamlit as st. 
+00009c30: 2020 2020 2020 203e 3e3e 2069 6d70 6f72         >>> impor
+00009c40: 7420 7061 6e64 6173 2061 7320 7064 0a20  t pandas as pd. 
+00009c50: 2020 2020 2020 203e 3e3e 2069 6d70 6f72         >>> impor
+00009c60: 7420 6e75 6d70 7920 6173 206e 700a 2020  t numpy as np.  
+00009c70: 2020 2020 2020 3e3e 3e0a 2020 2020 2020        >>>.      
+00009c80: 2020 3e3e 3e20 6368 6172 745f 6461 7461    >>> chart_data
+00009c90: 203d 2070 642e 4461 7461 4672 616d 6528   = pd.DataFrame(
+00009ca0: 6e70 2e72 616e 646f 6d2e 7261 6e64 6e28  np.random.randn(
+00009cb0: 3230 2c20 3329 2c20 636f 6c75 6d6e 733d  20, 3), columns=
+00009cc0: 5b22 6122 2c20 2262 222c 2022 6322 5d29  ["a", "b", "c"])
+00009cd0: 0a20 2020 2020 2020 203e 3e3e 0a20 2020  .        >>>.   
+00009ce0: 2020 2020 203e 3e3e 2073 742e 6261 725f       >>> st.bar_
+00009cf0: 6368 6172 7428 6368 6172 745f 6461 7461  chart(chart_data
+00009d00: 290a 0a20 2020 2020 2020 202e 2e20 6f75  )..        .. ou
+00009d10: 7470 7574 3a3a 0a20 2020 2020 2020 2020  tput::.         
+00009d20: 2020 6874 7470 733a 2f2f 646f 632d 6261    https://doc-ba
+00009d30: 722d 6368 6172 742e 7374 7265 616d 6c69  r-chart.streamli
+00009d40: 742e 6170 702f 0a20 2020 2020 2020 2020  t.app/.         
+00009d50: 2020 6865 6967 6874 3a20 3434 3070 780a    height: 440px.
+00009d60: 0a20 2020 2020 2020 2059 6f75 2063 616e  .        You can
+00009d70: 2061 6c73 6f20 6368 6f6f 7365 2064 6966   also choose dif
+00009d80: 6665 7265 6e74 2063 6f6c 756d 6e73 2074  ferent columns t
+00009d90: 6f20 7573 6520 666f 7220 7820 616e 6420  o use for x and 
+00009da0: 792c 2061 7320 7765 6c6c 2061 7320 7365  y, as well as se
+00009db0: 740a 2020 2020 2020 2020 7468 6520 636f  t.        the co
+00009dc0: 6c6f 7220 6479 6e61 6d69 6361 6c6c 7920  lor dynamically 
+00009dd0: 6261 7365 6420 6f6e 2061 2033 7264 2063  based on a 3rd c
+00009de0: 6f6c 756d 6e20 2861 7373 756d 696e 6720  olumn (assuming 
+00009df0: 796f 7572 2064 6174 6166 7261 6d65 2069  your dataframe i
+00009e00: 7320 696e 0a20 2020 2020 2020 206c 6f6e  s in.        lon
+00009e10: 6720 666f 726d 6174 293a 0a0a 2020 2020  g format):..    
+00009e20: 2020 2020 3e3e 3e20 696d 706f 7274 2073      >>> import s
+00009e30: 7472 6561 6d6c 6974 2061 7320 7374 0a20  treamlit as st. 
+00009e40: 2020 2020 2020 203e 3e3e 2069 6d70 6f72         >>> impor
+00009e50: 7420 7061 6e64 6173 2061 7320 7064 0a20  t pandas as pd. 
+00009e60: 2020 2020 2020 203e 3e3e 2069 6d70 6f72         >>> impor
+00009e70: 7420 6e75 6d70 7920 6173 206e 700a 2020  t numpy as np.  
+00009e80: 2020 2020 2020 3e3e 3e0a 2020 2020 2020        >>>.      
+00009e90: 2020 3e3e 3e20 6368 6172 745f 6461 7461    >>> chart_data
+00009ea0: 203d 2070 642e 4461 7461 4672 616d 6528   = pd.DataFrame(
+00009eb0: 0a20 2020 2020 2020 202e 2e2e 2020 2020  .        ...    
+00009ec0: 7b0a 2020 2020 2020 2020 2e2e 2e20 2020  {.        ...   
+00009ed0: 2020 2020 2022 636f 6c31 223a 206c 6973       "col1": lis
+00009ee0: 7428 7261 6e67 6528 3230 2929 202a 2033  t(range(20)) * 3
+00009ef0: 2c0a 2020 2020 2020 2020 2e2e 2e20 2020  ,.        ...   
+00009f00: 2020 2020 2022 636f 6c32 223a 206e 702e       "col2": np.
+00009f10: 7261 6e64 6f6d 2e72 616e 646e 2836 3029  random.randn(60)
+00009f20: 2c0a 2020 2020 2020 2020 2e2e 2e20 2020  ,.        ...   
+00009f30: 2020 2020 2022 636f 6c33 223a 205b 2241       "col3": ["A
+00009f40: 225d 202a 2032 3020 2b20 5b22 4222 5d20  "] * 20 + ["B"] 
+00009f50: 2a20 3230 202b 205b 2243 225d 202a 2032  * 20 + ["C"] * 2
+00009f60: 302c 0a20 2020 2020 2020 202e 2e2e 2020  0,.        ...  
+00009f70: 2020 7d0a 2020 2020 2020 2020 2e2e 2e20    }.        ... 
+00009f80: 290a 2020 2020 2020 2020 3e3e 3e0a 2020  ).        >>>.  
+00009f90: 2020 2020 2020 3e3e 3e20 7374 2e62 6172        >>> st.bar
+00009fa0: 5f63 6861 7274 2863 6861 7274 5f64 6174  _chart(chart_dat
+00009fb0: 612c 2078 3d22 636f 6c31 222c 2079 3d22  a, x="col1", y="
+00009fc0: 636f 6c32 222c 2063 6f6c 6f72 3d22 636f  col2", color="co
+00009fd0: 6c33 2229 0a0a 2020 2020 2020 2020 2e2e  l3")..        ..
+00009fe0: 206f 7574 7075 743a 3a0a 2020 2020 2020   output::.      
+00009ff0: 2020 2020 2068 7474 7073 3a2f 2f64 6f63       https://doc
+0000a000: 2d62 6172 2d63 6861 7274 312e 7374 7265  -bar-chart1.stre
+0000a010: 616d 6c69 742e 6170 702f 0a20 2020 2020  amlit.app/.     
+0000a020: 2020 2020 2020 6865 6967 6874 3a20 3434        height: 44
+0000a030: 3070 780a 0a20 2020 2020 2020 2046 696e  0px..        Fin
+0000a040: 616c 6c79 2c20 6966 2079 6f75 7220 6461  ally, if your da
+0000a050: 7461 6672 616d 6520 6973 2069 6e20 7769  taframe is in wi
+0000a060: 6465 2066 6f72 6d61 742c 2079 6f75 2063  de format, you c
+0000a070: 616e 2067 726f 7570 206d 756c 7469 706c  an group multipl
+0000a080: 650a 2020 2020 2020 2020 636f 6c75 6d6e  e.        column
+0000a090: 7320 756e 6465 7220 7468 6520 7920 6172  s under the y ar
+0000a0a0: 6775 6d65 6e74 2074 6f20 7368 6f77 206d  gument to show m
+0000a0b0: 756c 7469 706c 6520 7365 7269 6573 2077  ultiple series w
+0000a0c0: 6974 6820 6469 6666 6572 656e 740a 2020  ith different.  
+0000a0d0: 2020 2020 2020 636f 6c6f 7273 3a0a 0a20        colors:.. 
+0000a0e0: 2020 2020 2020 203e 3e3e 2069 6d70 6f72         >>> impor
+0000a0f0: 7420 7374 7265 616d 6c69 7420 6173 2073  t streamlit as s
+0000a100: 740a 2020 2020 2020 2020 3e3e 3e20 696d  t.        >>> im
+0000a110: 706f 7274 2070 616e 6461 7320 6173 2070  port pandas as p
+0000a120: 640a 2020 2020 2020 2020 3e3e 3e20 696d  d.        >>> im
+0000a130: 706f 7274 206e 756d 7079 2061 7320 6e70  port numpy as np
+0000a140: 0a20 2020 2020 2020 203e 3e3e 0a20 2020  .        >>>.   
+0000a150: 2020 2020 203e 3e3e 2063 6861 7274 5f64       >>> chart_d
+0000a160: 6174 6120 3d20 7064 2e44 6174 6146 7261  ata = pd.DataFra
+0000a170: 6d65 280a 2020 2020 2020 2020 2e2e 2e20  me(.        ... 
+0000a180: 2020 207b 2263 6f6c 3122 3a20 6c69 7374     {"col1": list
+0000a190: 2872 616e 6765 2832 3029 292c 2022 636f  (range(20)), "co
+0000a1a0: 6c32 223a 206e 702e 7261 6e64 6f6d 2e72  l2": np.random.r
+0000a1b0: 616e 646e 2832 3029 2c20 2263 6f6c 3322  andn(20), "col3"
+0000a1c0: 3a20 6e70 2e72 616e 646f 6d2e 7261 6e64  : np.random.rand
+0000a1d0: 6e28 3230 297d 0a20 2020 2020 2020 202e  n(20)}.        .
+0000a1e0: 2e2e 2029 0a20 2020 2020 2020 203e 3e3e  .. ).        >>>
+0000a1f0: 0a20 2020 2020 2020 203e 3e3e 2073 742e  .        >>> st.
+0000a200: 6261 725f 6368 6172 7428 0a20 2020 2020  bar_chart(.     
+0000a210: 2020 202e 2e2e 2020 2020 6368 6172 745f     ...    chart_
+0000a220: 6461 7461 2c20 783d 2263 6f6c 3122 2c20  data, x="col1", 
+0000a230: 793d 5b22 636f 6c32 222c 2022 636f 6c33  y=["col2", "col3
+0000a240: 225d 2c20 636f 6c6f 723d 5b22 2346 4630  "], color=["#FF0
+0000a250: 3030 3022 2c20 2223 3030 3030 4646 225d  000", "#0000FF"]
+0000a260: 2020 2320 4f70 7469 6f6e 616c 0a20 2020    # Optional.   
+0000a270: 2020 2020 202e 2e2e 2029 0a0a 2020 2020       ... )..    
+0000a280: 2020 2020 2e2e 206f 7574 7075 743a 3a0a      .. output::.
+0000a290: 2020 2020 2020 2020 2020 2068 7474 7073             https
+0000a2a0: 3a2f 2f64 6f63 2d62 6172 2d63 6861 7274  ://doc-bar-chart
+0000a2b0: 322e 7374 7265 616d 6c69 742e 6170 702f  2.streamlit.app/
+0000a2c0: 0a20 2020 2020 2020 2020 2020 6865 6967  .           heig
+0000a2d0: 6874 3a20 3434 3070 780a 0a20 2020 2020  ht: 440px..     
+0000a2e0: 2020 2022 2222 0a0a 2020 2020 2020 2020     """..        
+0000a2f0: 6368 6172 742c 2061 6464 5f72 6f77 735f  chart, add_rows_
+0000a300: 6d65 7461 6461 7461 203d 2067 656e 6572  metadata = gener
+0000a310: 6174 655f 6368 6172 7428 0a20 2020 2020  ate_chart(.     
+0000a320: 2020 2020 2020 2063 6861 7274 5f74 7970         chart_typ
+0000a330: 653d 4368 6172 7454 7970 652e 4241 522c  e=ChartType.BAR,
+0000a340: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
+0000a350: 613d 6461 7461 2c0a 2020 2020 2020 2020  a=data,.        
+0000a360: 2020 2020 785f 6672 6f6d 5f75 7365 723d      x_from_user=
+0000a370: 782c 0a20 2020 2020 2020 2020 2020 2079  x,.            y
+0000a380: 5f66 726f 6d5f 7573 6572 3d79 2c0a 2020  _from_user=y,.  
+0000a390: 2020 2020 2020 2020 2020 636f 6c6f 725f            color_
+0000a3a0: 6672 6f6d 5f75 7365 723d 636f 6c6f 722c  from_user=color,
+0000a3b0: 0a20 2020 2020 2020 2020 2020 2073 697a  .            siz
+0000a3c0: 655f 6672 6f6d 5f75 7365 723d 4e6f 6e65  e_from_user=None
+0000a3d0: 2c0a 2020 2020 2020 2020 2020 2020 7769  ,.            wi
+0000a3e0: 6474 683d 7769 6474 682c 0a20 2020 2020  dth=width,.     
+0000a3f0: 2020 2020 2020 2068 6569 6768 743d 6865         height=he
+0000a400: 6967 6874 2c0a 2020 2020 2020 2020 290a  ight,.        ).
+0000a410: 2020 2020 2020 2020 7265 7475 726e 2063          return c
+0000a420: 6173 7428 0a20 2020 2020 2020 2020 2020  ast(.           
+0000a430: 2022 4465 6c74 6147 656e 6572 6174 6f72   "DeltaGenerator
+0000a440: 222c 0a20 2020 2020 2020 2020 2020 2073  ",.            s
+0000a450: 656c 662e 5f61 6c74 6169 725f 6368 6172  elf._altair_char
+0000a460: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
+0000a470: 2020 2063 6861 7274 2c0a 2020 2020 2020     chart,.      
+0000a480: 2020 2020 2020 2020 2020 7573 655f 636f            use_co
+0000a490: 6e74 6169 6e65 725f 7769 6474 683d 7573  ntainer_width=us
+0000a4a0: 655f 636f 6e74 6169 6e65 725f 7769 6474  e_container_widt
+0000a4b0: 682c 0a20 2020 2020 2020 2020 2020 2020  h,.             
+0000a4c0: 2020 2074 6865 6d65 3d22 7374 7265 616d     theme="stream
+0000a4d0: 6c69 7422 2c0a 2020 2020 2020 2020 2020  lit",.          
+0000a4e0: 2020 2020 2020 6164 645f 726f 7773 5f6d        add_rows_m
+0000a4f0: 6574 6164 6174 613d 6164 645f 726f 7773  etadata=add_rows
+0000a500: 5f6d 6574 6164 6174 612c 0a20 2020 2020  _metadata,.     
+0000a510: 2020 2020 2020 2029 2c0a 2020 2020 2020         ),.      
+0000a520: 2020 290a 0a20 2020 2040 6761 7468 6572    )..    @gather
+0000a530: 5f6d 6574 7269 6373 2822 7363 6174 7465  _metrics("scatte
+0000a540: 725f 6368 6172 7422 290a 2020 2020 6465  r_chart").    de
+0000a550: 6620 7363 6174 7465 725f 6368 6172 7428  f scatter_chart(
+0000a560: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
+0000a570: 2020 2020 2020 2064 6174 613a 2044 6174         data: Dat
+0000a580: 6120 3d20 4e6f 6e65 2c0a 2020 2020 2020  a = None,.      
+0000a590: 2020 2a2c 0a20 2020 2020 2020 2078 3a20    *,.        x: 
+0000a5a0: 7374 7220 7c20 4e6f 6e65 203d 204e 6f6e  str | None = Non
+0000a5b0: 652c 0a20 2020 2020 2020 2079 3a20 7374  e,.        y: st
+0000a5c0: 7220 7c20 5365 7175 656e 6365 5b73 7472  r | Sequence[str
+0000a5d0: 5d20 7c20 4e6f 6e65 203d 204e 6f6e 652c  ] | None = None,
+0000a5e0: 0a20 2020 2020 2020 2063 6f6c 6f72 3a20  .        color: 
+0000a5f0: 7374 7220 7c20 436f 6c6f 7220 7c20 6c69  str | Color | li
+0000a600: 7374 5b43 6f6c 6f72 5d20 7c20 4e6f 6e65  st[Color] | None
+0000a610: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+0000a620: 2073 697a 653a 2073 7472 207c 2066 6c6f   size: str | flo
+0000a630: 6174 207c 2069 6e74 207c 204e 6f6e 6520  at | int | None 
+0000a640: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+0000a650: 7769 6474 683a 2069 6e74 207c 204e 6f6e  width: int | Non
+0000a660: 6520 3d20 4e6f 6e65 2c0a 2020 2020 2020  e = None,.      
+0000a670: 2020 6865 6967 6874 3a20 696e 7420 7c20    height: int | 
+0000a680: 4e6f 6e65 203d 204e 6f6e 652c 0a20 2020  None = None,.   
+0000a690: 2020 2020 2075 7365 5f63 6f6e 7461 696e       use_contain
+0000a6a0: 6572 5f77 6964 7468 3a20 626f 6f6c 203d  er_width: bool =
+0000a6b0: 2054 7275 652c 0a20 2020 2029 202d 3e20   True,.    ) -> 
+0000a6c0: 4465 6c74 6147 656e 6572 6174 6f72 3a0a  DeltaGenerator:.
+0000a6d0: 2020 2020 2020 2020 2222 2244 6973 706c          """Displ
+0000a6e0: 6179 2061 2073 6361 7474 6572 706c 6f74  ay a scatterplot
+0000a6f0: 2063 6861 7274 2e0a 0a20 2020 2020 2020   chart...       
+0000a700: 2054 6869 7320 6973 2073 796e 7461 782d   This is syntax-
+0000a710: 7375 6761 7220 6172 6f75 6e64 2060 6073  sugar around ``s
+0000a720: 742e 616c 7461 6972 5f63 6861 7274 6060  t.altair_chart``
+0000a730: 2e20 5468 6520 6d61 696e 2064 6966 6665  . The main diffe
+0000a740: 7265 6e63 650a 2020 2020 2020 2020 6973  rence.        is
+0000a750: 2074 6869 7320 636f 6d6d 616e 6420 7573   this command us
+0000a760: 6573 2074 6865 2064 6174 6127 7320 6f77  es the data's ow
+0000a770: 6e20 636f 6c75 6d6e 2061 6e64 2069 6e64  n column and ind
+0000a780: 6963 6573 2074 6f20 6669 6775 7265 206f  ices to figure o
+0000a790: 7574 0a20 2020 2020 2020 2074 6865 2063  ut.        the c
+0000a7a0: 6861 7274 2773 2041 6c74 6169 7220 7370  hart's Altair sp
+0000a7b0: 6563 2e20 4173 2061 2072 6573 756c 7420  ec. As a result 
+0000a7c0: 7468 6973 2069 7320 6561 7369 6572 2074  this is easier t
+0000a7d0: 6f20 7573 6520 666f 7220 6d61 6e79 0a20  o use for many. 
+0000a7e0: 2020 2020 2020 2022 6a75 7374 2070 6c6f         "just plo
+0000a7f0: 7420 7468 6973 2220 7363 656e 6172 696f  t this" scenario
+0000a800: 732c 2077 6869 6c65 2062 6569 6e67 206c  s, while being l
+0000a810: 6573 7320 6375 7374 6f6d 697a 6162 6c65  ess customizable
+0000a820: 2e0a 0a20 2020 2020 2020 2049 6620 6060  ...        If ``
+0000a830: 7374 2e73 6361 7474 6572 5f63 6861 7274  st.scatter_chart
+0000a840: 6060 2064 6f65 7320 6e6f 7420 6775 6573  `` does not gues
+0000a850: 7320 7468 6520 6461 7461 2073 7065 6369  s the data speci
+0000a860: 6669 6361 7469 6f6e 2063 6f72 7265 6374  fication correct
+0000a870: 6c79 2c0a 2020 2020 2020 2020 7472 7920  ly,.        try 
+0000a880: 7370 6563 6966 7969 6e67 2079 6f75 7220  specifying your 
+0000a890: 6465 7369 7265 6420 6368 6172 7420 7573  desired chart us
+0000a8a0: 696e 6720 6060 7374 2e61 6c74 6169 725f  ing ``st.altair_
+0000a8b0: 6368 6172 7460 602e 0a0a 2020 2020 2020  chart``...      
+0000a8c0: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
+0000a8d0: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a       ----------.
+0000a8e0: 2020 2020 2020 2020 6461 7461 203a 2070          data : p
+0000a8f0: 616e 6461 732e 4461 7461 4672 616d 652c  andas.DataFrame,
+0000a900: 2070 616e 6461 732e 5374 796c 6572 2c20   pandas.Styler, 
+0000a910: 7079 6172 726f 772e 5461 626c 652c 206e  pyarrow.Table, n
+0000a920: 756d 7079 2e6e 6461 7272 6179 2c20 7079  umpy.ndarray, py
+0000a930: 7370 6172 6b2e 7371 6c2e 4461 7461 4672  spark.sql.DataFr
+0000a940: 616d 652c 2073 6e6f 7766 6c61 6b65 2e73  ame, snowflake.s
+0000a950: 6e6f 7770 6172 6b2e 6461 7461 6672 616d  nowpark.datafram
+0000a960: 652e 4461 7461 4672 616d 652c 2073 6e6f  e.DataFrame, sno
+0000a970: 7766 6c61 6b65 2e73 6e6f 7770 6172 6b2e  wflake.snowpark.
+0000a980: 7461 626c 652e 5461 626c 652c 2049 7465  table.Table, Ite
+0000a990: 7261 626c 652c 2064 6963 7420 6f72 204e  rable, dict or N
+0000a9a0: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
+0000a9b0: 4461 7461 2074 6f20 6265 2070 6c6f 7474  Data to be plott
+0000a9c0: 6564 2e0a 0a20 2020 2020 2020 2078 203a  ed...        x :
+0000a9d0: 2073 7472 206f 7220 4e6f 6e65 0a20 2020   str or None.   
+0000a9e0: 2020 2020 2020 2020 2043 6f6c 756d 6e20           Column 
+0000a9f0: 6e61 6d65 2074 6f20 7573 6520 666f 7220  name to use for 
+0000aa00: 7468 6520 782d 6178 6973 2e20 4966 204e  the x-axis. If N
+0000aa10: 6f6e 652c 2075 7365 7320 7468 6520 6461  one, uses the da
+0000aa20: 7461 2069 6e64 6578 2066 6f72 2074 6865  ta index for the
+0000aa30: 2078 2d61 7869 732e 0a0a 2020 2020 2020   x-axis...      
+0000aa40: 2020 7920 3a20 7374 722c 2053 6571 7565    y : str, Seque
+0000aa50: 6e63 6520 6f66 2073 7472 2c20 6f72 204e  nce of str, or N
+0000aa60: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
+0000aa70: 436f 6c75 6d6e 206e 616d 6528 7329 2074  Column name(s) t
+0000aa80: 6f20 7573 6520 666f 7220 7468 6520 792d  o use for the y-
+0000aa90: 6178 6973 2e20 4966 2061 2053 6571 7565  axis. If a Seque
+0000aaa0: 6e63 6520 6f66 2073 7472 696e 6773 2c0a  nce of strings,.
+0000aab0: 2020 2020 2020 2020 2020 2020 6472 6177              draw
+0000aac0: 7320 7365 7665 7261 6c20 7365 7269 6573  s several series
+0000aad0: 206f 6e20 7468 6520 7361 6d65 2063 6861   on the same cha
+0000aae0: 7274 2062 7920 6d65 6c74 696e 6720 796f  rt by melting yo
+0000aaf0: 7572 2077 6964 652d 666f 726d 6174 0a20  ur wide-format. 
+0000ab00: 2020 2020 2020 2020 2020 2074 6162 6c65             table
+0000ab10: 2069 6e74 6f20 6120 6c6f 6e67 2d66 6f72   into a long-for
+0000ab20: 6d61 7420 7461 626c 6520 6265 6869 6e64  mat table behind
+0000ab30: 2074 6865 2073 6365 6e65 732e 2049 6620   the scenes. If 
+0000ab40: 4e6f 6e65 2c20 6472 6177 730a 2020 2020  None, draws.    
+0000ab50: 2020 2020 2020 2020 7468 6520 6461 7461          the data
+0000ab60: 206f 6620 616c 6c20 7265 6d61 696e 696e   of all remainin
+0000ab70: 6720 636f 6c75 6d6e 7320 6173 2064 6174  g columns as dat
+0000ab80: 6120 7365 7269 6573 2e0a 0a20 2020 2020  a series...     
+0000ab90: 2020 2063 6f6c 6f72 203a 2073 7472 2c20     color : str, 
+0000aba0: 7475 706c 652c 2053 6571 7565 6e63 6520  tuple, Sequence 
+0000abb0: 6f66 2073 7472 2c20 5365 7175 656e 6365  of str, Sequence
+0000abc0: 206f 6620 7475 706c 652c 206f 7220 4e6f   of tuple, or No
+0000abd0: 6e65 0a20 2020 2020 2020 2020 2020 2054  ne.            T
+0000abe0: 6865 2063 6f6c 6f72 206f 6620 7468 6520  he color of the 
+0000abf0: 6369 7263 6c65 7320 7265 7072 6573 656e  circles represen
+0000ac00: 7469 6e67 2065 6163 6820 6461 7461 706f  ting each datapo
+0000ac10: 696e 742e 0a0a 2020 2020 2020 2020 2020  int...          
+0000ac20: 2020 5468 6973 2063 616e 2062 653a 0a0a    This can be:..
+0000ac30: 2020 2020 2020 2020 2020 2020 2a20 4e6f              * No
+0000ac40: 6e65 2c20 746f 2075 7365 2074 6865 2064  ne, to use the d
+0000ac50: 6566 6175 6c74 2063 6f6c 6f72 2e0a 2020  efault color..  
+0000ac60: 2020 2020 2020 2020 2020 2a20 4120 6865            * A he
+0000ac70: 7820 7374 7269 6e67 206c 696b 6520 2223  x string like "#
+0000ac80: 6666 6161 3030 2220 6f72 2022 2366 6661  ffaa00" or "#ffa
+0000ac90: 6130 3038 3822 2e0a 2020 2020 2020 2020  a0088"..        
+0000aca0: 2020 2020 2a20 416e 2052 4742 206f 7220      * An RGB or 
+0000acb0: 5247 4241 2074 7570 6c65 2077 6974 6820  RGBA tuple with 
+0000acc0: 7468 6520 7265 642c 2067 7265 656e 2c20  the red, green, 
+0000acd0: 626c 7565 2c20 616e 6420 616c 7068 610a  blue, and alpha.
+0000ace0: 2020 2020 2020 2020 2020 2020 2020 636f                co
+0000acf0: 6d70 6f6e 656e 7473 2073 7065 6369 6669  mponents specifi
+0000ad00: 6564 2061 7320 696e 7473 2066 726f 6d20  ed as ints from 
+0000ad10: 3020 746f 2032 3535 206f 7220 666c 6f61  0 to 255 or floa
+0000ad20: 7473 2066 726f 6d20 302e 3020 746f 0a20  ts from 0.0 to. 
+0000ad30: 2020 2020 2020 2020 2020 2020 2031 2e30               1.0
+0000ad40: 2e0a 2020 2020 2020 2020 2020 2020 2a20  ..            * 
+0000ad50: 5468 6520 6e61 6d65 206f 6620 6120 636f  The name of a co
+0000ad60: 6c75 6d6e 2069 6e20 7468 6520 6461 7461  lumn in the data
+0000ad70: 7365 7420 7768 6572 6520 7468 6520 636f  set where the co
+0000ad80: 6c6f 7220 6f66 2074 6861 740a 2020 2020  lor of that.    
+0000ad90: 2020 2020 2020 2020 2020 6461 7461 706f            datapo
+0000ada0: 696e 7420 7769 6c6c 2063 6f6d 6520 6672  int will come fr
+0000adb0: 6f6d 2e0a 0a20 2020 2020 2020 2020 2020  om...           
+0000adc0: 2020 2049 6620 7468 6520 7661 6c75 6573     If the values
+0000add0: 2069 6e20 7468 6973 2063 6f6c 756d 6e20   in this column 
+0000ade0: 6172 6520 696e 206f 6e65 206f 6620 7468  are in one of th
+0000adf0: 6520 636f 6c6f 7220 666f 726d 6174 730a  e color formats.
+0000ae00: 2020 2020 2020 2020 2020 2020 2020 6162                ab
+0000ae10: 6f76 6520 2868 6578 2073 7472 696e 6720  ove (hex string 
+0000ae20: 6f72 2063 6f6c 6f72 2074 7570 6c65 292c  or color tuple),
+0000ae30: 2074 6865 6e20 7468 6174 2063 6f6c 6f72   then that color
+0000ae40: 2077 696c 6c20 6265 2075 7365 642e 0a0a   will be used...
+0000ae50: 2020 2020 2020 2020 2020 2020 2020 4f74                Ot
+0000ae60: 6865 7277 6973 652c 2074 6865 2063 6f6c  herwise, the col
+0000ae70: 6f72 2077 696c 6c20 6265 2061 7574 6f6d  or will be autom
+0000ae80: 6174 6963 616c 6c79 2070 6963 6b65 6420  atically picked 
+0000ae90: 6672 6f6d 2074 6865 0a20 2020 2020 2020  from the.       
+0000aea0: 2020 2020 2020 2064 6566 6175 6c74 2070         default p
+0000aeb0: 616c 6574 7465 2e0a 0a20 2020 2020 2020  alette...       
+0000aec0: 2020 2020 2020 2046 6f72 2065 7861 6d70         For examp
+0000aed0: 6c65 3a20 6966 2074 6865 2064 6174 6173  le: if the datas
+0000aee0: 6574 2068 6173 2031 3030 3020 726f 7773  et has 1000 rows
+0000aef0: 2c20 6275 7420 7468 6973 2063 6f6c 756d  , but this colum
+0000af00: 6e20 6f6e 6c79 0a20 2020 2020 2020 2020  n only.         
+0000af10: 2020 2020 2063 6f6e 7461 696e 7320 7468       contains th
+0000af20: 6520 7661 6c75 6573 2022 6164 756c 7422  e values "adult"
+0000af30: 2c20 2263 6869 6c64 222c 2061 6e64 2022  , "child", and "
+0000af40: 6261 6279 222c 2074 6865 6e20 7468 6f73  baby", then thos
+0000af50: 6520 3130 3030 0a20 2020 2020 2020 2020  e 1000.         
+0000af60: 2020 2020 2064 6174 6170 6f69 6e74 7320       datapoints 
+0000af70: 6265 2073 686f 776e 2075 7369 6e67 2074  be shown using t
+0000af80: 6872 6565 2063 6f6c 6f72 7320 6672 6f6d  hree colors from
+0000af90: 2074 6865 2064 6566 6175 6c74 2070 616c   the default pal
+0000afa0: 6574 7465 2e0a 0a20 2020 2020 2020 2020  ette...         
+0000afb0: 2020 2020 2042 7574 2069 6620 7468 6973       But if this
+0000afc0: 2063 6f6c 756d 6e20 6f6e 6c79 2063 6f6e   column only con
+0000afd0: 7461 696e 7320 666c 6f61 7473 206f 7220  tains floats or 
+0000afe0: 696e 7473 2c20 7468 656e 2074 686f 7365  ints, then those
+0000aff0: 0a20 2020 2020 2020 2020 2020 2020 2031  .              1
+0000b000: 3030 3020 6461 7461 706f 696e 7473 2077  000 datapoints w
+0000b010: 696c 6c20 6265 2073 686f 776e 2075 7369  ill be shown usi
+0000b020: 6e67 2061 2063 6f6c 6f72 7320 6672 6f6d  ng a colors from
+0000b030: 2061 2063 6f6e 7469 6e75 6f75 730a 2020   a continuous.  
+0000b040: 2020 2020 2020 2020 2020 2020 636f 6c6f              colo
+0000b050: 7220 6772 6164 6965 6e74 2e0a 0a20 2020  r gradient...   
+0000b060: 2020 2020 2020 2020 2020 2046 696e 616c             Final
+0000b070: 6c79 2c20 6966 2074 6869 7320 636f 6c75  ly, if this colu
+0000b080: 6d6e 206f 6e6c 7920 636f 6e74 6169 6e73  mn only contains
+0000b090: 2074 6865 2076 616c 7565 7320 2223 6666   the values "#ff
+0000b0a0: 6161 3030 222c 0a20 2020 2020 2020 2020  aa00",.         
+0000b0b0: 2020 2020 2022 2366 3066 222c 2022 2330       "#f0f", "#0
+0000b0c0: 3030 3066 6622 2c20 7468 656e 2074 6865  000ff", then the
+0000b0d0: 6e20 6561 6368 206f 6620 7468 6f73 6520  n each of those 
+0000b0e0: 3130 3030 2064 6174 6170 6f69 6e74 7320  1000 datapoints 
+0000b0f0: 7769 6c6c 0a20 2020 2020 2020 2020 2020  will.           
+0000b100: 2020 2062 6520 6173 7369 676e 6564 2022     be assigned "
+0000b110: 2366 6661 6130 3022 2c20 2223 6630 6622  #ffaa00", "#f0f"
+0000b120: 2c20 6f72 2022 2330 3030 3066 6622 2061  , or "#0000ff" a
+0000b130: 7320 6170 7072 6f70 7269 6174 652e 0a0a  s appropriate...
+0000b140: 2020 2020 2020 2020 2020 2020 4966 2074              If t
+0000b150: 6865 2064 6174 6166 7261 6d65 2069 7320  he dataframe is 
+0000b160: 696e 2077 6964 6520 666f 726d 6174 2028  in wide format (
+0000b170: 7468 6174 2069 732c 2079 2069 7320 6120  that is, y is a 
+0000b180: 5365 7175 656e 6365 206f 660a 2020 2020  Sequence of.    
+0000b190: 2020 2020 2020 2020 636f 6c75 6d6e 7329          columns)
+0000b1a0: 2c20 7468 6973 2063 616e 2061 6c73 6f20  , this can also 
+0000b1b0: 6265 3a0a 0a20 2020 2020 2020 2020 2020  be:..           
+0000b1c0: 202a 2041 206c 6973 7420 6f66 2073 7472   * A list of str
+0000b1d0: 696e 6720 636f 6c6f 7273 206f 7220 636f  ing colors or co
+0000b1e0: 6c6f 7220 7475 706c 6573 2074 6f20 6265  lor tuples to be
+0000b1f0: 2075 7365 6420 666f 7220 6561 6368 206f   used for each o
+0000b200: 660a 2020 2020 2020 2020 2020 2020 2020  f.              
+0000b210: 7468 6520 7365 7269 6573 2069 6e20 7468  the series in th
+0000b220: 6520 6368 6172 742e 2054 6869 7320 6c69  e chart. This li
+0000b230: 7374 2073 686f 756c 6420 6861 7665 2074  st should have t
+0000b240: 6865 2073 616d 6520 6c65 6e67 7468 0a20  he same length. 
+0000b250: 2020 2020 2020 2020 2020 2020 2061 7320               as 
+0000b260: 7468 6520 6e75 6d62 6572 206f 6620 7920  the number of y 
+0000b270: 7661 6c75 6573 2028 652e 672e 2060 6063  values (e.g. ``c
+0000b280: 6f6c 6f72 3d5b 2223 6664 3022 2c20 2223  olor=["#fd0", "#
+0000b290: 6630 6622 2c20 2223 3034 6622 5d60 600a  f0f", "#04f"]``.
+0000b2a0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+0000b2b0: 7220 7468 7265 6520 7365 7269 6573 292e  r three series).
+0000b2c0: 0a0a 2020 2020 2020 2020 7369 7a65 203a  ..        size :
+0000b2d0: 2073 7472 2c20 666c 6f61 742c 2069 6e74   str, float, int
+0000b2e0: 2c20 6f72 204e 6f6e 650a 2020 2020 2020  , or None.      
+0000b2f0: 2020 2020 2020 5468 6520 7369 7a65 206f        The size o
+0000b300: 6620 7468 6520 6369 7263 6c65 7320 7265  f the circles re
+0000b310: 7072 6573 656e 7469 6e67 2065 6163 6820  presenting each 
+0000b320: 706f 696e 742e 0a0a 2020 2020 2020 2020  point...        
+0000b330: 2020 2020 5468 6973 2063 616e 2062 653a      This can be:
+0000b340: 0a0a 2020 2020 2020 2020 2020 2020 2a20  ..            * 
+0000b350: 4120 6e75 6d62 6572 206c 696b 6520 3130  A number like 10
+0000b360: 302c 2074 6f20 7370 6563 6966 7920 6120  0, to specify a 
+0000b370: 7369 6e67 6c65 2073 697a 6520 746f 2075  single size to u
+0000b380: 7365 2066 6f72 2061 6c6c 0a20 2020 2020  se for all.     
+0000b390: 2020 2020 2020 2020 2064 6174 6170 6f69           datapoi
+0000b3a0: 6e74 732e 0a20 2020 2020 2020 2020 2020  nts..           
+0000b3b0: 202a 2054 6865 206e 616d 6520 6f66 2074   * The name of t
+0000b3c0: 6865 2063 6f6c 756d 6e20 746f 2075 7365  he column to use
+0000b3d0: 2066 6f72 2074 6865 2073 697a 652e 2054   for the size. T
+0000b3e0: 6869 7320 616c 6c6f 7773 2065 6163 680a  his allows each.
+0000b3f0: 2020 2020 2020 2020 2020 2020 2020 6461                da
+0000b400: 7461 706f 696e 7420 746f 2062 6520 7265  tapoint to be re
+0000b410: 7072 6573 656e 7465 6420 6279 2061 2063  presented by a c
+0000b420: 6972 636c 6520 6f66 2061 2064 6966 6665  ircle of a diffe
+0000b430: 7265 6e74 2073 697a 652e 0a0a 2020 2020  rent size...    
+0000b440: 2020 2020 7769 6474 6820 3a20 696e 7420      width : int 
+0000b450: 6f72 204e 6f6e 650a 2020 2020 2020 2020  or None.        
+0000b460: 2020 2020 4465 7369 7265 6420 7769 6474      Desired widt
+0000b470: 6820 6f66 2074 6865 2063 6861 7274 2065  h of the chart e
+0000b480: 7870 7265 7373 6564 2069 6e20 7069 7865  xpressed in pixe
+0000b490: 6c73 2e20 4966 2060 6077 6964 7468 6060  ls. If ``width``
+0000b4a0: 2069 730a 2020 2020 2020 2020 2020 2020   is.            
+0000b4b0: 6060 4e6f 6e65 6060 2028 6465 6661 756c  ``None`` (defaul
+0000b4c0: 7429 2c20 5374 7265 616d 6c69 7420 7365  t), Streamlit se
+0000b4d0: 7473 2074 6865 2077 6964 7468 206f 6620  ts the width of 
+0000b4e0: 7468 6520 6368 6172 7420 746f 2066 6974  the chart to fit
+0000b4f0: 0a20 2020 2020 2020 2020 2020 2069 7473  .            its
+0000b500: 2063 6f6e 7465 6e74 7320 6163 636f 7264   contents accord
+0000b510: 696e 6720 746f 2074 6865 2070 6c6f 7474  ing to the plott
+0000b520: 696e 6720 6c69 6272 6172 792c 2075 7020  ing library, up 
+0000b530: 746f 2074 6865 2077 6964 7468 206f 660a  to the width of.
+0000b540: 2020 2020 2020 2020 2020 2020 7468 6520              the 
+0000b550: 7061 7265 6e74 2063 6f6e 7461 696e 6572  parent container
+0000b560: 2e20 4966 2060 6077 6964 7468 6060 2069  . If ``width`` i
+0000b570: 7320 6772 6561 7465 7220 7468 616e 2074  s greater than t
+0000b580: 6865 2077 6964 7468 206f 6620 7468 650a  he width of the.
+0000b590: 2020 2020 2020 2020 2020 2020 7061 7265              pare
+0000b5a0: 6e74 2063 6f6e 7461 696e 6572 2c20 5374  nt container, St
+0000b5b0: 7265 616d 6c69 7420 7365 7473 2074 6865  reamlit sets the
+0000b5c0: 2063 6861 7274 2077 6964 7468 2074 6f20   chart width to 
+0000b5d0: 6d61 7463 6820 7468 6520 7769 6474 680a  match the width.
+0000b5e0: 2020 2020 2020 2020 2020 2020 6f66 2074              of t
+0000b5f0: 6865 2070 6172 656e 7420 636f 6e74 6169  he parent contai
+0000b600: 6e65 722e 0a0a 2020 2020 2020 2020 6865  ner...        he
+0000b610: 6967 6874 203a 2069 6e74 206f 7220 4e6f  ight : int or No
+0000b620: 6e65 0a20 2020 2020 2020 2020 2020 2044  ne.            D
+0000b630: 6573 6972 6564 2068 6569 6768 7420 6f66  esired height of
+0000b640: 2074 6865 2063 6861 7274 2065 7870 7265   the chart expre
+0000b650: 7373 6564 2069 6e20 7069 7865 6c73 2e20  ssed in pixels. 
+0000b660: 4966 2060 6068 6569 6768 7460 6020 6973  If ``height`` is
+0000b670: 0a20 2020 2020 2020 2020 2020 2060 604e  .            ``N
+0000b680: 6f6e 6560 6020 2864 6566 6175 6c74 292c  one`` (default),
+0000b690: 2053 7472 6561 6d6c 6974 2073 6574 7320   Streamlit sets 
+0000b6a0: 7468 6520 6865 6967 6874 206f 6620 7468  the height of th
+0000b6b0: 6520 6368 6172 7420 746f 2066 6974 0a20  e chart to fit. 
+0000b6c0: 2020 2020 2020 2020 2020 2069 7473 2063             its c
+0000b6d0: 6f6e 7465 6e74 7320 6163 636f 7264 696e  ontents accordin
+0000b6e0: 6720 746f 2074 6865 2070 6c6f 7474 696e  g to the plottin
+0000b6f0: 6720 6c69 6272 6172 792e 0a0a 2020 2020  g library...    
+0000b700: 2020 2020 7573 655f 636f 6e74 6169 6e65      use_containe
+0000b710: 725f 7769 6474 6820 3a20 626f 6f6c 0a20  r_width : bool. 
+0000b720: 2020 2020 2020 2020 2020 2057 6865 7468             Wheth
+0000b730: 6572 2074 6f20 6f76 6572 7269 6465 2060  er to override `
+0000b740: 6077 6964 7468 6060 2077 6974 6820 7468  `width`` with th
+0000b750: 6520 7769 6474 6820 6f66 2074 6865 2070  e width of the p
+0000b760: 6172 656e 740a 2020 2020 2020 2020 2020  arent.          
+0000b770: 2020 636f 6e74 6169 6e65 722e 2049 6620    container. If 
+0000b780: 6060 7573 655f 636f 6e74 6169 6e65 725f  ``use_container_
+0000b790: 7769 6474 6860 6020 6973 2060 6046 616c  width`` is ``Fal
+0000b7a0: 7365 6060 2028 6465 6661 756c 7429 2c0a  se`` (default),.
+0000b7b0: 2020 2020 2020 2020 2020 2020 5374 7265              Stre
+0000b7c0: 616d 6c69 7420 7365 7473 2074 6865 2063  amlit sets the c
+0000b7d0: 6861 7274 2773 2077 6964 7468 2061 6363  hart's width acc
+0000b7e0: 6f72 6469 6e67 2074 6f20 6060 7769 6474  ording to ``widt
+0000b7f0: 6860 602e 2049 660a 2020 2020 2020 2020  h``. If.        
+0000b800: 2020 2020 6060 7573 655f 636f 6e74 6169      ``use_contai
+0000b810: 6e65 725f 7769 6474 6860 6020 6973 2060  ner_width`` is `
+0000b820: 6054 7275 6560 602c 2053 7472 6561 6d6c  `True``, Streaml
+0000b830: 6974 2073 6574 7320 7468 6520 7769 6474  it sets the widt
+0000b840: 6820 6f66 0a20 2020 2020 2020 2020 2020  h of.           
+0000b850: 2074 6865 2063 6861 7274 2074 6f20 6d61   the chart to ma
+0000b860: 7463 6820 7468 6520 7769 6474 6820 6f66  tch the width of
+0000b870: 2074 6865 2070 6172 656e 7420 636f 6e74   the parent cont
+0000b880: 6169 6e65 722e 0a0a 2020 2020 2020 2020  ainer...        
+0000b890: 4578 616d 706c 6573 0a20 2020 2020 2020  Examples.       
+0000b8a0: 202d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020   --------.      
+0000b8b0: 2020 3e3e 3e20 696d 706f 7274 2073 7472    >>> import str
+0000b8c0: 6561 6d6c 6974 2061 7320 7374 0a20 2020  eamlit as st.   
+0000b8d0: 2020 2020 203e 3e3e 2069 6d70 6f72 7420       >>> import 
+0000b8e0: 7061 6e64 6173 2061 7320 7064 0a20 2020  pandas as pd.   
+0000b8f0: 2020 2020 203e 3e3e 2069 6d70 6f72 7420       >>> import 
+0000b900: 6e75 6d70 7920 6173 206e 700a 2020 2020  numpy as np.    
+0000b910: 2020 2020 3e3e 3e0a 2020 2020 2020 2020      >>>.        
+0000b920: 3e3e 3e20 6368 6172 745f 6461 7461 203d  >>> chart_data =
+0000b930: 2070 642e 4461 7461 4672 616d 6528 6e70   pd.DataFrame(np
+0000b940: 2e72 616e 646f 6d2e 7261 6e64 6e28 3230  .random.randn(20
+0000b950: 2c20 3329 2c20 636f 6c75 6d6e 733d 5b22  , 3), columns=["
+0000b960: 6122 2c20 2262 222c 2022 6322 5d29 0a20  a", "b", "c"]). 
+0000b970: 2020 2020 2020 203e 3e3e 0a20 2020 2020         >>>.     
+0000b980: 2020 203e 3e3e 2073 742e 7363 6174 7465     >>> st.scatte
+0000b990: 725f 6368 6172 7428 6368 6172 745f 6461  r_chart(chart_da
+0000b9a0: 7461 290a 0a20 2020 2020 2020 202e 2e20  ta)..        .. 
+0000b9b0: 6f75 7470 7574 3a3a 0a20 2020 2020 2020  output::.       
+0000b9c0: 2020 2020 6874 7470 733a 2f2f 646f 632d      https://doc-
+0000b9d0: 7363 6174 7465 722d 6368 6172 742e 7374  scatter-chart.st
+0000b9e0: 7265 616d 6c69 742e 6170 702f 0a20 2020  reamlit.app/.   
+0000b9f0: 2020 2020 2020 2020 6865 6967 6874 3a20          height: 
+0000ba00: 3434 3070 780a 0a20 2020 2020 2020 2059  440px..        Y
+0000ba10: 6f75 2063 616e 2061 6c73 6f20 6368 6f6f  ou can also choo
+0000ba20: 7365 2064 6966 6665 7265 6e74 2063 6f6c  se different col
+0000ba30: 756d 6e73 2074 6f20 7573 6520 666f 7220  umns to use for 
+0000ba40: 7820 616e 6420 792c 2061 7320 7765 6c6c  x and y, as well
+0000ba50: 2061 7320 7365 740a 2020 2020 2020 2020   as set.        
+0000ba60: 7468 6520 636f 6c6f 7220 6479 6e61 6d69  the color dynami
+0000ba70: 6361 6c6c 7920 6261 7365 6420 6f6e 2061  cally based on a
+0000ba80: 2033 7264 2063 6f6c 756d 6e20 2861 7373   3rd column (ass
+0000ba90: 756d 696e 6720 796f 7572 2064 6174 6166  uming your dataf
+0000baa0: 7261 6d65 2069 7320 696e 0a20 2020 2020  rame is in.     
+0000bab0: 2020 206c 6f6e 6720 666f 726d 6174 293a     long format):
+0000bac0: 0a0a 2020 2020 2020 2020 3e3e 3e20 696d  ..        >>> im
+0000bad0: 706f 7274 2073 7472 6561 6d6c 6974 2061  port streamlit a
+0000bae0: 7320 7374 0a20 2020 2020 2020 203e 3e3e  s st.        >>>
+0000baf0: 2069 6d70 6f72 7420 7061 6e64 6173 2061   import pandas a
+0000bb00: 7320 7064 0a20 2020 2020 2020 203e 3e3e  s pd.        >>>
+0000bb10: 2069 6d70 6f72 7420 6e75 6d70 7920 6173   import numpy as
+0000bb20: 206e 700a 2020 2020 2020 2020 3e3e 3e0a   np.        >>>.
+0000bb30: 2020 2020 2020 2020 3e3e 3e20 6368 6172          >>> char
+0000bb40: 745f 6461 7461 203d 2070 642e 4461 7461  t_data = pd.Data
+0000bb50: 4672 616d 6528 6e70 2e72 616e 646f 6d2e  Frame(np.random.
+0000bb60: 7261 6e64 6e28 3230 2c20 3329 2c20 636f  randn(20, 3), co
+0000bb70: 6c75 6d6e 733d 5b22 636f 6c31 222c 2022  lumns=["col1", "
+0000bb80: 636f 6c32 222c 2022 636f 6c33 225d 290a  col2", "col3"]).
+0000bb90: 2020 2020 2020 2020 3e3e 3e20 6368 6172          >>> char
+0000bba0: 745f 6461 7461 5b27 636f 6c34 275d 203d  t_data['col4'] =
+0000bbb0: 206e 702e 7261 6e64 6f6d 2e63 686f 6963   np.random.choic
+0000bbc0: 6528 5b27 4127 2c27 4227 2c27 4327 5d2c  e(['A','B','C'],
+0000bbd0: 2032 3029 0a20 2020 2020 2020 203e 3e3e   20).        >>>
+0000bbe0: 0a20 2020 2020 2020 203e 3e3e 2073 742e  .        >>> st.
+0000bbf0: 7363 6174 7465 725f 6368 6172 7428 0a20  scatter_chart(. 
+0000bc00: 2020 2020 2020 202e 2e2e 2020 2020 2063         ...     c
+0000bc10: 6861 7274 5f64 6174 612c 0a20 2020 2020  hart_data,.     
+0000bc20: 2020 202e 2e2e 2020 2020 2078 3d27 636f     ...     x='co
+0000bc30: 6c31 272c 0a20 2020 2020 2020 202e 2e2e  l1',.        ...
+0000bc40: 2020 2020 2079 3d27 636f 6c32 272c 0a20       y='col2',. 
+0000bc50: 2020 2020 2020 202e 2e2e 2020 2020 2063         ...     c
+0000bc60: 6f6c 6f72 3d27 636f 6c34 272c 0a20 2020  olor='col4',.   
+0000bc70: 2020 2020 202e 2e2e 2020 2020 2073 697a       ...     siz
+0000bc80: 653d 2763 6f6c 3327 2c0a 2020 2020 2020  e='col3',.      
+0000bc90: 2020 2e2e 2e20 290a 0a20 2020 2020 2020    ... )..       
+0000bca0: 202e 2e20 6f75 7470 7574 3a3a 0a20 2020   .. output::.   
+0000bcb0: 2020 2020 2020 2020 6874 7470 733a 2f2f          https://
+0000bcc0: 646f 632d 7363 6174 7465 722d 6368 6172  doc-scatter-char
+0000bcd0: 7431 2e73 7472 6561 6d6c 6974 2e61 7070  t1.streamlit.app
+0000bce0: 2f0a 2020 2020 2020 2020 2020 2068 6569  /.           hei
+0000bcf0: 6768 743a 2034 3430 7078 0a0a 2020 2020  ght: 440px..    
+0000bd00: 2020 2020 4669 6e61 6c6c 792c 2069 6620      Finally, if 
+0000bd10: 796f 7572 2064 6174 6166 7261 6d65 2069  your dataframe i
+0000bd20: 7320 696e 2077 6964 6520 666f 726d 6174  s in wide format
+0000bd30: 2c20 796f 7520 6361 6e20 6772 6f75 7020  , you can group 
+0000bd40: 6d75 6c74 6970 6c65 0a20 2020 2020 2020  multiple.       
+0000bd50: 2063 6f6c 756d 6e73 2075 6e64 6572 2074   columns under t
+0000bd60: 6865 2079 2061 7267 756d 656e 7420 746f  he y argument to
+0000bd70: 2073 686f 7720 6d75 6c74 6970 6c65 2073   show multiple s
+0000bd80: 6572 6965 7320 7769 7468 2064 6966 6665  eries with diffe
+0000bd90: 7265 6e74 0a20 2020 2020 2020 2063 6f6c  rent.        col
+0000bda0: 6f72 733a 0a0a 2020 2020 2020 2020 3e3e  ors:..        >>
+0000bdb0: 3e20 696d 706f 7274 2073 7472 6561 6d6c  > import streaml
+0000bdc0: 6974 2061 7320 7374 0a20 2020 2020 2020  it as st.       
+0000bdd0: 203e 3e3e 2069 6d70 6f72 7420 7061 6e64   >>> import pand
+0000bde0: 6173 2061 7320 7064 0a20 2020 2020 2020  as as pd.       
+0000bdf0: 203e 3e3e 2069 6d70 6f72 7420 6e75 6d70   >>> import nump
+0000be00: 7920 6173 206e 700a 2020 2020 2020 2020  y as np.        
+0000be10: 3e3e 3e0a 2020 2020 2020 2020 3e3e 3e20  >>>.        >>> 
+0000be20: 6368 6172 745f 6461 7461 203d 2070 642e  chart_data = pd.
+0000be30: 4461 7461 4672 616d 6528 6e70 2e72 616e  DataFrame(np.ran
+0000be40: 646f 6d2e 7261 6e64 6e28 3230 2c20 3429  dom.randn(20, 4)
+0000be50: 2c20 636f 6c75 6d6e 733d 5b22 636f 6c31  , columns=["col1
+0000be60: 222c 2022 636f 6c32 222c 2022 636f 6c33  ", "col2", "col3
+0000be70: 222c 2022 636f 6c34 225d 290a 2020 2020  ", "col4"]).    
+0000be80: 2020 2020 3e3e 3e0a 2020 2020 2020 2020      >>>.        
+0000be90: 3e3e 3e20 7374 2e73 6361 7474 6572 5f63  >>> st.scatter_c
+0000bea0: 6861 7274 280a 2020 2020 2020 2020 2e2e  hart(.        ..
+0000beb0: 2e20 2020 2020 6368 6172 745f 6461 7461  .     chart_data
+0000bec0: 2c0a 2020 2020 2020 2020 2e2e 2e20 2020  ,.        ...   
+0000bed0: 2020 783d 2763 6f6c 3127 2c0a 2020 2020    x='col1',.    
+0000bee0: 2020 2020 2e2e 2e20 2020 2020 793d 5b27      ...     y=['
+0000bef0: 636f 6c32 272c 2027 636f 6c33 275d 2c0a  col2', 'col3'],.
+0000bf00: 2020 2020 2020 2020 2e2e 2e20 2020 2020          ...     
+0000bf10: 7369 7a65 3d27 636f 6c34 272c 0a20 2020  size='col4',.   
+0000bf20: 2020 2020 202e 2e2e 2020 2020 2063 6f6c       ...     col
+0000bf30: 6f72 3d5b 2723 4646 3030 3030 272c 2027  or=['#FF0000', '
+0000bf40: 2330 3030 3046 4627 5d2c 2020 2320 4f70  #0000FF'],  # Op
+0000bf50: 7469 6f6e 616c 0a20 2020 2020 2020 202e  tional.        .
+0000bf60: 2e2e 2029 0a0a 2020 2020 2020 2020 2e2e  .. )..        ..
+0000bf70: 206f 7574 7075 743a 3a0a 2020 2020 2020   output::.      
+0000bf80: 2020 2020 2068 7474 7073 3a2f 2f64 6f63       https://doc
+0000bf90: 2d73 6361 7474 6572 2d63 6861 7274 322e  -scatter-chart2.
+0000bfa0: 7374 7265 616d 6c69 742e 6170 702f 0a20  streamlit.app/. 
+0000bfb0: 2020 2020 2020 2020 2020 6865 6967 6874            height
+0000bfc0: 3a20 3434 3070 780a 0a20 2020 2020 2020  : 440px..       
+0000bfd0: 2022 2222 0a0a 2020 2020 2020 2020 6368   """..        ch
+0000bfe0: 6172 742c 2061 6464 5f72 6f77 735f 6d65  art, add_rows_me
+0000bff0: 7461 6461 7461 203d 2067 656e 6572 6174  tadata = generat
+0000c000: 655f 6368 6172 7428 0a20 2020 2020 2020  e_chart(.       
+0000c010: 2020 2020 2063 6861 7274 5f74 7970 653d       chart_type=
+0000c020: 4368 6172 7454 7970 652e 5343 4154 5445  ChartType.SCATTE
+0000c030: 522c 0a20 2020 2020 2020 2020 2020 2064  R,.            d
+0000c040: 6174 613d 6461 7461 2c0a 2020 2020 2020  ata=data,.      
+0000c050: 2020 2020 2020 785f 6672 6f6d 5f75 7365        x_from_use
+0000c060: 723d 782c 0a20 2020 2020 2020 2020 2020  r=x,.           
+0000c070: 2079 5f66 726f 6d5f 7573 6572 3d79 2c0a   y_from_user=y,.
+0000c080: 2020 2020 2020 2020 2020 2020 636f 6c6f              colo
+0000c090: 725f 6672 6f6d 5f75 7365 723d 636f 6c6f  r_from_user=colo
+0000c0a0: 722c 0a20 2020 2020 2020 2020 2020 2073  r,.            s
+0000c0b0: 697a 655f 6672 6f6d 5f75 7365 723d 7369  ize_from_user=si
+0000c0c0: 7a65 2c0a 2020 2020 2020 2020 2020 2020  ze,.            
+0000c0d0: 7769 6474 683d 7769 6474 682c 0a20 2020  width=width,.   
+0000c0e0: 2020 2020 2020 2020 2068 6569 6768 743d           height=
+0000c0f0: 6865 6967 6874 2c0a 2020 2020 2020 2020  height,.        
+0000c100: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+0000c110: 2063 6173 7428 0a20 2020 2020 2020 2020   cast(.         
+0000c120: 2020 2022 4465 6c74 6147 656e 6572 6174     "DeltaGenerat
+0000c130: 6f72 222c 0a20 2020 2020 2020 2020 2020  or",.           
+0000c140: 2073 656c 662e 5f61 6c74 6169 725f 6368   self._altair_ch
+0000c150: 6172 7428 0a20 2020 2020 2020 2020 2020  art(.           
+0000c160: 2020 2020 2063 6861 7274 2c0a 2020 2020       chart,.    
+0000c170: 2020 2020 2020 2020 2020 2020 7573 655f              use_
+0000c180: 636f 6e74 6169 6e65 725f 7769 6474 683d  container_width=
+0000c190: 7573 655f 636f 6e74 6169 6e65 725f 7769  use_container_wi
+0000c1a0: 6474 682c 0a20 2020 2020 2020 2020 2020  dth,.           
+0000c1b0: 2020 2020 2074 6865 6d65 3d22 7374 7265       theme="stre
+0000c1c0: 616d 6c69 7422 2c0a 2020 2020 2020 2020  amlit",.        
+0000c1d0: 2020 2020 2020 2020 6164 645f 726f 7773          add_rows
+0000c1e0: 5f6d 6574 6164 6174 613d 6164 645f 726f  _metadata=add_ro
+0000c1f0: 7773 5f6d 6574 6164 6174 612c 0a20 2020  ws_metadata,.   
+0000c200: 2020 2020 2020 2020 2029 2c0a 2020 2020           ),.    
+0000c210: 2020 2020 290a 0a20 2020 2040 6f76 6572      )..    @over
+0000c220: 6c6f 6164 0a20 2020 2064 6566 2061 6c74  load.    def alt
+0000c230: 6169 725f 6368 6172 7428 0a20 2020 2020  air_chart(.     
+0000c240: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
+0000c250: 2061 6c74 6169 725f 6368 6172 743a 2061   altair_chart: a
+0000c260: 6c74 2e43 6861 7274 2c0a 2020 2020 2020  lt.Chart,.      
+0000c270: 2020 2a2c 0a20 2020 2020 2020 2075 7365    *,.        use
+0000c280: 5f63 6f6e 7461 696e 6572 5f77 6964 7468  _container_width
+0000c290: 3a20 626f 6f6c 203d 2046 616c 7365 2c0a  : bool = False,.
+0000c2a0: 2020 2020 2020 2020 7468 656d 653a 204c          theme: L
+0000c2b0: 6974 6572 616c 5b22 7374 7265 616d 6c69  iteral["streamli
+0000c2c0: 7422 5d20 7c20 4e6f 6e65 203d 2022 7374  t"] | None = "st
+0000c2d0: 7265 616d 6c69 7422 2c0a 2020 2020 2020  reamlit",.      
+0000c2e0: 2020 6b65 793a 204b 6579 207c 204e 6f6e    key: Key | Non
+0000c2f0: 6520 3d20 4e6f 6e65 2c0a 2020 2020 2020  e = None,.      
+0000c300: 2020 6f6e 5f73 656c 6563 743a 204c 6974    on_select: Lit
+0000c310: 6572 616c 5b22 6967 6e6f 7265 225d 2c20  eral["ignore"], 
+0000c320: 2023 204e 6f20 6465 6661 756c 7420 7661   # No default va
+0000c330: 6c75 6520 6865 7265 2074 6f20 6d61 6b65  lue here to make
+0000c340: 2069 7420 776f 726b 2077 6974 6820 6d79   it work with my
+0000c350: 7079 0a20 2020 2020 2020 2073 656c 6563  py.        selec
+0000c360: 7469 6f6e 5f6d 6f64 653a 2073 7472 207c  tion_mode: str |
+0000c370: 2049 7465 7261 626c 655b 7374 725d 207c   Iterable[str] |
+0000c380: 204e 6f6e 6520 3d20 4e6f 6e65 2c0a 2020   None = None,.  
+0000c390: 2020 2920 2d3e 2044 656c 7461 4765 6e65    ) -> DeltaGene
+0000c3a0: 7261 746f 723a 0a20 2020 2020 2020 202e  rator:.        .
+0000c3b0: 2e2e 0a0a 2020 2020 406f 7665 726c 6f61  ....    @overloa
+0000c3c0: 640a 2020 2020 6465 6620 616c 7461 6972  d.    def altair
+0000c3d0: 5f63 6861 7274 280a 2020 2020 2020 2020  _chart(.        
+0000c3e0: 7365 6c66 2c0a 2020 2020 2020 2020 616c  self,.        al
+0000c3f0: 7461 6972 5f63 6861 7274 3a20 616c 742e  tair_chart: alt.
+0000c400: 4368 6172 742c 0a20 2020 2020 2020 202a  Chart,.        *
+0000c410: 2c0a 2020 2020 2020 2020 7573 655f 636f  ,.        use_co
+0000c420: 6e74 6169 6e65 725f 7769 6474 683a 2062  ntainer_width: b
+0000c430: 6f6f 6c20 3d20 4661 6c73 652c 0a20 2020  ool = False,.   
+0000c440: 2020 2020 2074 6865 6d65 3a20 4c69 7465       theme: Lite
+0000c450: 7261 6c5b 2273 7472 6561 6d6c 6974 225d  ral["streamlit"]
+0000c460: 207c 204e 6f6e 6520 3d20 2273 7472 6561   | None = "strea
+0000c470: 6d6c 6974 222c 0a20 2020 2020 2020 206b  mlit",.        k
+0000c480: 6579 3a20 4b65 7920 7c20 4e6f 6e65 203d  ey: Key | None =
+0000c490: 204e 6f6e 652c 0a20 2020 2020 2020 206f   None,.        o
+0000c4a0: 6e5f 7365 6c65 6374 3a20 4c69 7465 7261  n_select: Litera
+0000c4b0: 6c5b 2272 6572 756e 225d 207c 2057 6964  l["rerun"] | Wid
+0000c4c0: 6765 7443 616c 6c62 6163 6b20 3d20 2272  getCallback = "r
+0000c4d0: 6572 756e 222c 0a20 2020 2020 2020 2073  erun",.        s
+0000c4e0: 656c 6563 7469 6f6e 5f6d 6f64 653a 2073  election_mode: s
+0000c4f0: 7472 207c 2049 7465 7261 626c 655b 7374  tr | Iterable[st
+0000c500: 725d 207c 204e 6f6e 6520 3d20 4e6f 6e65  r] | None = None
+0000c510: 2c0a 2020 2020 2920 2d3e 2056 6567 614c  ,.    ) -> VegaL
+0000c520: 6974 6553 7461 7465 3a0a 2020 2020 2020  iteState:.      
+0000c530: 2020 2e2e 2e0a 0a20 2020 2040 6761 7468    .....    @gath
+0000c540: 6572 5f6d 6574 7269 6373 2822 616c 7461  er_metrics("alta
+0000c550: 6972 5f63 6861 7274 2229 0a20 2020 2064  ir_chart").    d
+0000c560: 6566 2061 6c74 6169 725f 6368 6172 7428  ef altair_chart(
+0000c570: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
+0000c580: 2020 2020 2020 2061 6c74 6169 725f 6368         altair_ch
+0000c590: 6172 743a 2061 6c74 2e43 6861 7274 2c0a  art: alt.Chart,.
+0000c5a0: 2020 2020 2020 2020 2a2c 0a20 2020 2020          *,.     
+0000c5b0: 2020 2075 7365 5f63 6f6e 7461 696e 6572     use_container
+0000c5c0: 5f77 6964 7468 3a20 626f 6f6c 203d 2046  _width: bool = F
+0000c5d0: 616c 7365 2c0a 2020 2020 2020 2020 7468  alse,.        th
+0000c5e0: 656d 653a 204c 6974 6572 616c 5b22 7374  eme: Literal["st
+0000c5f0: 7265 616d 6c69 7422 5d20 7c20 4e6f 6e65  reamlit"] | None
+0000c600: 203d 2022 7374 7265 616d 6c69 7422 2c0a   = "streamlit",.
+0000c610: 2020 2020 2020 2020 6b65 793a 204b 6579          key: Key
+0000c620: 207c 204e 6f6e 6520 3d20 4e6f 6e65 2c0a   | None = None,.
+0000c630: 2020 2020 2020 2020 6f6e 5f73 656c 6563          on_selec
+0000c640: 743a 204c 6974 6572 616c 5b22 7265 7275  t: Literal["reru
+0000c650: 6e22 2c20 2269 676e 6f72 6522 5d20 7c20  n", "ignore"] | 
+0000c660: 5769 6467 6574 4361 6c6c 6261 636b 203d  WidgetCallback =
+0000c670: 2022 6967 6e6f 7265 222c 0a20 2020 2020   "ignore",.     
+0000c680: 2020 2073 656c 6563 7469 6f6e 5f6d 6f64     selection_mod
+0000c690: 653a 2073 7472 207c 2049 7465 7261 626c  e: str | Iterabl
+0000c6a0: 655b 7374 725d 207c 204e 6f6e 6520 3d20  e[str] | None = 
+0000c6b0: 4e6f 6e65 2c0a 2020 2020 2920 2d3e 2044  None,.    ) -> D
+0000c6c0: 656c 7461 4765 6e65 7261 746f 7220 7c20  eltaGenerator | 
+0000c6d0: 5665 6761 4c69 7465 5374 6174 653a 0a20  VegaLiteState:. 
+0000c6e0: 2020 2020 2020 2022 2222 4469 7370 6c61         """Displa
+0000c6f0: 7920 6120 6368 6172 7420 7573 696e 6720  y a chart using 
+0000c700: 7468 6520 5665 6761 2d41 6c74 6169 7220  the Vega-Altair 
+0000c710: 6c69 6272 6172 792e 0a0a 2020 2020 2020  library...      
+0000c720: 2020 6056 6567 612d 416c 7461 6972 203c    `Vega-Altair <
+0000c730: 6874 7470 733a 2f2f 616c 7461 6972 2d76  https://altair-v
+0000c740: 697a 2e67 6974 6875 622e 696f 2f3e 605f  iz.github.io/>`_
+0000c750: 2069 7320 6120 6465 636c 6172 6174 6976   is a declarativ
+0000c760: 650a 2020 2020 2020 2020 7374 6174 6973  e.        statis
+0000c770: 7469 6361 6c20 7669 7375 616c 697a 6174  tical visualizat
+0000c780: 696f 6e20 6c69 6272 6172 7920 666f 7220  ion library for 
+0000c790: 5079 7468 6f6e 2c20 6261 7365 6420 6f6e  Python, based on
+0000c7a0: 2056 6567 6120 616e 640a 2020 2020 2020   Vega and.      
+0000c7b0: 2020 5665 6761 2d4c 6974 652e 0a0a 2020    Vega-Lite...  
+0000c7c0: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
+0000c7d0: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+0000c7e0: 2d2d 2d0a 2020 2020 2020 2020 616c 7461  ---.        alta
+0000c7f0: 6972 5f63 6861 7274 203a 2061 6c74 6169  ir_chart : altai
+0000c800: 722e 4368 6172 740a 2020 2020 2020 2020  r.Chart.        
+0000c810: 2020 2020 5468 6520 416c 7461 6972 2063      The Altair c
+0000c820: 6861 7274 206f 626a 6563 7420 746f 2064  hart object to d
+0000c830: 6973 706c 6179 2e20 5365 650a 2020 2020  isplay. See.    
+0000c840: 2020 2020 2020 2020 6874 7470 733a 2f2f          https://
+0000c850: 616c 7461 6972 2d76 697a 2e67 6974 6875  altair-viz.githu
+0000c860: 622e 696f 2f67 616c 6c65 7279 2f20 666f  b.io/gallery/ fo
+0000c870: 7220 6578 616d 706c 6573 206f 6620 6772  r examples of gr
+0000c880: 6170 680a 2020 2020 2020 2020 2020 2020  aph.            
+0000c890: 6465 7363 7269 7074 696f 6e73 2e0a 0a20  descriptions... 
+0000c8a0: 2020 2020 2020 2075 7365 5f63 6f6e 7461         use_conta
+0000c8b0: 696e 6572 5f77 6964 7468 203a 2062 6f6f  iner_width : boo
+0000c8c0: 6c0a 2020 2020 2020 2020 2020 2020 5768  l.            Wh
+0000c8d0: 6574 6865 7220 746f 206f 7665 7272 6964  ether to overrid
+0000c8e0: 6520 7468 6520 6669 6775 7265 2773 206e  e the figure's n
+0000c8f0: 6174 6976 6520 7769 6474 6820 7769 7468  ative width with
+0000c900: 2074 6865 2077 6964 7468 206f 660a 2020   the width of.  
+0000c910: 2020 2020 2020 2020 2020 7468 6520 7061            the pa
+0000c920: 7265 6e74 2063 6f6e 7461 696e 6572 2e20  rent container. 
+0000c930: 4966 2060 6075 7365 5f63 6f6e 7461 696e  If ``use_contain
+0000c940: 6572 5f77 6964 7468 6060 2069 7320 6060  er_width`` is ``
+0000c950: 4661 6c73 6560 600a 2020 2020 2020 2020  False``.        
+0000c960: 2020 2020 2864 6566 6175 6c74 292c 2053      (default), S
+0000c970: 7472 6561 6d6c 6974 2073 6574 7320 7468  treamlit sets th
+0000c980: 6520 7769 6474 6820 6f66 2074 6865 2063  e width of the c
+0000c990: 6861 7274 2074 6f20 6669 7420 6974 7320  hart to fit its 
+0000c9a0: 636f 6e74 656e 7473 0a20 2020 2020 2020  contents.       
+0000c9b0: 2020 2020 2061 6363 6f72 6469 6e67 2074       according t
+0000c9c0: 6f20 7468 6520 706c 6f74 7469 6e67 206c  o the plotting l
+0000c9d0: 6962 7261 7279 2c20 7570 2074 6f20 7468  ibrary, up to th
+0000c9e0: 6520 7769 6474 6820 6f66 2074 6865 2070  e width of the p
+0000c9f0: 6172 656e 740a 2020 2020 2020 2020 2020  arent.          
+0000ca00: 2020 636f 6e74 6169 6e65 722e 2049 6620    container. If 
+0000ca10: 6060 7573 655f 636f 6e74 6169 6e65 725f  ``use_container_
+0000ca20: 7769 6474 6860 6020 6973 2060 6054 7275  width`` is ``Tru
+0000ca30: 6560 602c 2053 7472 6561 6d6c 6974 2073  e``, Streamlit s
+0000ca40: 6574 730a 2020 2020 2020 2020 2020 2020  ets.            
+0000ca50: 7468 6520 7769 6474 6820 6f66 2074 6865  the width of the
+0000ca60: 2066 6967 7572 6520 746f 206d 6174 6368   figure to match
+0000ca70: 2074 6865 2077 6964 7468 206f 6620 7468   the width of th
+0000ca80: 6520 7061 7265 6e74 2063 6f6e 7461 696e  e parent contain
+0000ca90: 6572 2e0a 0a20 2020 2020 2020 2074 6865  er...        the
+0000caa0: 6d65 203a 2022 7374 7265 616d 6c69 7422  me : "streamlit"
+0000cab0: 206f 7220 4e6f 6e65 0a20 2020 2020 2020   or None.       
+0000cac0: 2020 2020 2054 6865 2074 6865 6d65 206f       The theme o
+0000cad0: 6620 7468 6520 6368 6172 742e 2049 6620  f the chart. If 
+0000cae0: 6060 7468 656d 6560 6020 6973 2060 6022  ``theme`` is ``"
+0000caf0: 7374 7265 616d 6c69 7422 6060 2028 6465  streamlit"`` (de
+0000cb00: 6661 756c 7429 2c0a 2020 2020 2020 2020  fault),.        
+0000cb10: 2020 2020 5374 7265 616d 6c69 7420 7573      Streamlit us
+0000cb20: 6573 2069 7473 206f 776e 2064 6573 6967  es its own desig
+0000cb30: 6e20 6465 6661 756c 742e 2049 6620 6060  n default. If ``
+0000cb40: 7468 656d 6560 6020 6973 2060 604e 6f6e  theme`` is ``Non
+0000cb50: 6560 602c 0a20 2020 2020 2020 2020 2020  e``,.           
+0000cb60: 2053 7472 6561 6d6c 6974 2066 616c 6c73   Streamlit falls
+0000cb70: 2062 6163 6b20 746f 2074 6865 2064 6566   back to the def
+0000cb80: 6175 6c74 2062 6568 6176 696f 7220 6f66  ault behavior of
+0000cb90: 2074 6865 206c 6962 7261 7279 2e0a 0a20   the library... 
+0000cba0: 2020 2020 2020 206b 6579 203a 2073 7472         key : str
+0000cbb0: 0a20 2020 2020 2020 2020 2020 2041 6e20  .            An 
+0000cbc0: 6f70 7469 6f6e 616c 2073 7472 696e 6720  optional string 
+0000cbd0: 746f 2075 7365 2066 6f72 2067 6976 696e  to use for givin
+0000cbe0: 6720 7468 6973 2065 6c65 6d65 6e74 2061  g this element a
+0000cbf0: 2073 7461 626c 650a 2020 2020 2020 2020   stable.        
+0000cc00: 2020 2020 6964 656e 7469 7479 2e20 4966      identity. If
+0000cc10: 2060 606b 6579 6060 2069 7320 6060 4e6f   ``key`` is ``No
+0000cc20: 6e65 6060 2028 6465 6661 756c 7429 2c20  ne`` (default), 
+0000cc30: 7468 6973 2065 6c65 6d65 6e74 2773 2069  this element's i
+0000cc40: 6465 6e74 6974 790a 2020 2020 2020 2020  dentity.        
+0000cc50: 2020 2020 7769 6c6c 2062 6520 6465 7465      will be dete
+0000cc60: 726d 696e 6564 2062 6173 6564 206f 6e20  rmined based on 
+0000cc70: 7468 6520 7661 6c75 6573 206f 6620 7468  the values of th
+0000cc80: 6520 6f74 6865 7220 7061 7261 6d65 7465  e other paramete
+0000cc90: 7273 2e0a 0a20 2020 2020 2020 2020 2020  rs...           
+0000cca0: 2041 6464 6974 696f 6e61 6c6c 792c 2069   Additionally, i
+0000ccb0: 6620 7365 6c65 6374 696f 6e73 2061 7265  f selections are
+0000ccc0: 2061 6374 6976 6174 6564 2061 6e64 2060   activated and `
+0000ccd0: 606b 6579 6060 2069 7320 7072 6f76 6964  `key`` is provid
+0000cce0: 6564 2c0a 2020 2020 2020 2020 2020 2020  ed,.            
+0000ccf0: 5374 7265 616d 6c69 7420 7769 6c6c 2072  Streamlit will r
+0000cd00: 6567 6973 7465 7220 7468 6520 6b65 7920  egister the key 
+0000cd10: 696e 2053 6573 7369 6f6e 2053 7461 7465  in Session State
+0000cd20: 2074 6f20 7374 6f72 6520 7468 650a 2020   to store the.  
+0000cd30: 2020 2020 2020 2020 2020 7365 6c65 6374            select
+0000cd40: 696f 6e20 7374 6174 652e 2054 6865 2073  ion state. The s
+0000cd50: 656c 6563 7469 6f6e 2073 7461 7465 2069  election state i
+0000cd60: 7320 7265 6164 2d6f 6e6c 792e 0a0a 2020  s read-only...  
+0000cd70: 2020 2020 2020 6f6e 5f73 656c 6563 7420        on_select 
+0000cd80: 3a20 2269 676e 6f72 6522 2c20 2272 6572  : "ignore", "rer
+0000cd90: 756e 222c 206f 7220 6361 6c6c 6162 6c65  un", or callable
+0000cda0: 0a20 2020 2020 2020 2020 2020 2048 6f77  .            How
+0000cdb0: 2074 6865 2066 6967 7572 6520 7368 6f75   the figure shou
+0000cdc0: 6c64 2072 6573 706f 6e64 2074 6f20 7573  ld respond to us
+0000cdd0: 6572 2073 656c 6563 7469 6f6e 2065 7665  er selection eve
+0000cde0: 6e74 732e 2054 6869 730a 2020 2020 2020  nts. This.      
+0000cdf0: 2020 2020 2020 636f 6e74 726f 6c73 2077        controls w
+0000ce00: 6865 7468 6572 206f 7220 6e6f 7420 7468  hether or not th
+0000ce10: 6520 6669 6775 7265 2062 6568 6176 6573  e figure behaves
+0000ce20: 206c 696b 6520 616e 2069 6e70 7574 2077   like an input w
+0000ce30: 6964 6765 742e 0a20 2020 2020 2020 2020  idget..         
+0000ce40: 2020 2060 606f 6e5f 7365 6c65 6374 6060     ``on_select``
+0000ce50: 2063 616e 2062 6520 6f6e 6520 6f66 2074   can be one of t
+0000ce60: 6865 2066 6f6c 6c6f 7769 6e67 3a0a 0a20  he following:.. 
+0000ce70: 2020 2020 2020 2020 2020 202d 2060 6022             - ``"
+0000ce80: 6967 6e6f 7265 2260 6020 2864 6566 6175  ignore"`` (defau
+0000ce90: 6c74 293a 2053 7472 6561 6d6c 6974 2077  lt): Streamlit w
+0000cea0: 696c 6c20 6e6f 7420 7265 6163 7420 746f  ill not react to
+0000ceb0: 2061 6e79 2073 656c 6563 7469 6f6e 0a20   any selection. 
+0000cec0: 2020 2020 2020 2020 2020 2020 2065 7665               eve
+0000ced0: 6e74 7320 696e 2074 6865 2063 6861 7274  nts in the chart
+0000cee0: 2e20 5468 6520 6669 6775 7265 2077 696c  . The figure wil
+0000cef0: 6c20 6e6f 7420 6265 6861 7665 206c 696b  l not behave lik
+0000cf00: 6520 616e 2069 6e70 7574 0a20 2020 2020  e an input.     
+0000cf10: 2020 2020 2020 2020 2077 6964 6765 742e           widget.
+0000cf20: 0a0a 2020 2020 2020 2020 2020 2020 2d20  ..            - 
+0000cf30: 6060 2272 6572 756e 2260 603a 2053 7472  ``"rerun"``: Str
+0000cf40: 6561 6d6c 6974 2077 696c 6c20 7265 7275  eamlit will reru
+0000cf50: 6e20 7468 6520 6170 7020 7768 656e 2074  n the app when t
+0000cf60: 6865 2075 7365 7220 7365 6c65 6374 730a  he user selects.
+0000cf70: 2020 2020 2020 2020 2020 2020 2020 6461                da
+0000cf80: 7461 2069 6e20 7468 6520 6368 6172 742e  ta in the chart.
+0000cf90: 2049 6e20 7468 6973 2063 6173 652c 2060   In this case, `
+0000cfa0: 6073 742e 616c 7461 6972 5f63 6861 7274  `st.altair_chart
+0000cfb0: 6060 2077 696c 6c20 7265 7475 726e 0a20  `` will return. 
+0000cfc0: 2020 2020 2020 2020 2020 2020 2074 6865               the
+0000cfd0: 2073 656c 6563 7469 6f6e 2064 6174 6120   selection data 
+0000cfe0: 6173 2061 2064 6963 7469 6f6e 6172 792e  as a dictionary.
+0000cff0: 0a0a 2020 2020 2020 2020 2020 2020 2d20  ..            - 
+0000d000: 4120 6060 6361 6c6c 6162 6c65 6060 3a20  A ``callable``: 
+0000d010: 5374 7265 616d 6c69 7420 7769 6c6c 2072  Streamlit will r
+0000d020: 6572 756e 2074 6865 2061 7070 2061 6e64  erun the app and
+0000d030: 2065 7865 6375 7465 2074 6865 0a20 2020   execute the.   
+0000d040: 2020 2020 2020 2020 2020 2060 6063 616c             ``cal
+0000d050: 6c61 626c 6560 6020 6173 2061 2063 616c  lable`` as a cal
+0000d060: 6c62 6163 6b20 6675 6e63 7469 6f6e 2062  lback function b
+0000d070: 6566 6f72 6520 7468 6520 7265 7374 206f  efore the rest o
+0000d080: 6620 7468 6520 6170 702e 0a20 2020 2020  f the app..     
+0000d090: 2020 2020 2020 2020 2049 6e20 7468 6973           In this
+0000d0a0: 2063 6173 652c 2060 6073 742e 616c 7461   case, ``st.alta
+0000d0b0: 6972 5f63 6861 7274 6060 2077 696c 6c20  ir_chart`` will 
+0000d0c0: 7265 7475 726e 2074 6865 2073 656c 6563  return the selec
+0000d0d0: 7469 6f6e 2064 6174 610a 2020 2020 2020  tion data.      
+0000d0e0: 2020 2020 2020 2020 6173 2061 2064 6963          as a dic
+0000d0f0: 7469 6f6e 6172 792e 0a0a 2020 2020 2020  tionary...      
+0000d100: 2020 2020 2020 546f 2075 7365 2073 656c        To use sel
+0000d110: 6563 7469 6f6e 2065 7665 6e74 732c 2074  ection events, t
+0000d120: 6865 206f 626a 6563 7420 7061 7373 6564  he object passed
+0000d130: 2074 6f20 6060 616c 7461 6972 5f63 6861   to ``altair_cha
+0000d140: 7274 6060 206d 7573 740a 2020 2020 2020  rt`` must.      
+0000d150: 2020 2020 2020 696e 636c 7564 6520 7365        include se
+0000d160: 6c65 6374 696f 6e20 7061 7261 6d74 6572  lection paramter
+0000d170: 732e 2054 6f20 6c65 6172 6e20 6162 6f75  s. To learn abou
+0000d180: 7420 6465 6669 6e69 6e67 2069 6e74 6572  t defining inter
+0000d190: 6163 7469 6f6e 730a 2020 2020 2020 2020  actions.        
+0000d1a0: 2020 2020 696e 2041 6c74 6169 7220 616e      in Altair an
+0000d1b0: 6420 686f 7720 746f 2064 6563 6c61 7265  d how to declare
+0000d1c0: 2073 656c 6563 7469 6f6e 2d74 7970 6520   selection-type 
+0000d1d0: 7061 7261 6d65 7465 7273 2c20 7365 650a  parameters, see.
+0000d1e0: 2020 2020 2020 2020 2020 2020 6049 6e74              `Int
+0000d1f0: 6572 6163 7469 7665 2043 6861 7274 7320  eractive Charts 
+0000d200: 5c0a 2020 2020 2020 2020 2020 2020 3c68  \.            <h
+0000d210: 7474 7073 3a2f 2f61 6c74 6169 722d 7669  ttps://altair-vi
+0000d220: 7a2e 6769 7468 7562 2e69 6f2f 7573 6572  z.github.io/user
+0000d230: 5f67 7569 6465 2f69 6e74 6572 6163 7469  _guide/interacti
+0000d240: 6f6e 732e 6874 6d6c 3e60 5f0a 2020 2020  ons.html>`_.    
+0000d250: 2020 2020 2020 2020 696e 2041 6c74 6169          in Altai
+0000d260: 7227 7320 646f 6375 6d65 6e74 6174 696f  r's documentatio
+0000d270: 6e2e 0a0a 2020 2020 2020 2020 7365 6c65  n...        sele
+0000d280: 6374 696f 6e5f 6d6f 6465 203a 2073 7472  ction_mode : str
+0000d290: 206f 7220 4974 6572 6162 6c65 206f 6620   or Iterable of 
+0000d2a0: 7374 720a 2020 2020 2020 2020 2020 2020  str.            
+0000d2b0: 5468 6520 7365 6c65 6374 696f 6e20 7061  The selection pa
+0000d2c0: 7261 6d65 7465 7273 2053 7472 6561 6d6c  rameters Streaml
+0000d2d0: 6974 2073 686f 756c 6420 7573 652e 2049  it should use. I
+0000d2e0: 660a 2020 2020 2020 2020 2020 2020 6060  f.            ``
+0000d2f0: 7365 6c65 6374 696f 6e5f 6d6f 6465 6060  selection_mode``
+0000d300: 2069 7320 6060 4e6f 6e65 6060 2028 6465   is ``None`` (de
+0000d310: 6661 756c 7429 2c20 5374 7265 616d 6c69  fault), Streamli
+0000d320: 7420 7769 6c6c 2075 7365 2061 6c6c 0a20  t will use all. 
+0000d330: 2020 2020 2020 2020 2020 2073 656c 6563             selec
+0000d340: 7469 6f6e 2070 6172 616d 6574 6572 7320  tion parameters 
+0000d350: 6465 6669 6e65 6420 696e 2074 6865 2063  defined in the c
+0000d360: 6861 7274 2773 2041 6c74 6169 7220 7370  hart's Altair sp
+0000d370: 6563 2e0a 0a20 2020 2020 2020 2020 2020  ec...           
+0000d380: 2057 6865 6e20 5374 7265 616d 6c69 7420   When Streamlit 
+0000d390: 7573 6573 2061 2073 656c 6563 7469 6f6e  uses a selection
+0000d3a0: 2070 6172 616d 6574 6572 2c20 7365 6c65   parameter, sele
+0000d3b0: 6374 696f 6e73 2066 726f 6d20 7468 6174  ctions from that
+0000d3c0: 0a20 2020 2020 2020 2020 2020 2070 6172  .            par
+0000d3d0: 616d 6574 6572 2077 696c 6c20 7472 6967  ameter will trig
+0000d3e0: 6765 7220 6120 7265 7275 6e20 616e 6420  ger a rerun and 
+0000d3f0: 6265 2069 6e63 6c75 6465 6420 696e 2074  be included in t
+0000d400: 6865 2073 656c 6563 7469 6f6e 0a20 2020  he selection.   
+0000d410: 2020 2020 2020 2020 2073 7461 7465 2e20           state. 
+0000d420: 5768 656e 2053 7472 6561 6d6c 6974 2064  When Streamlit d
+0000d430: 6f65 7320 6e6f 7420 7573 6520 6120 7365  oes not use a se
+0000d440: 6c65 6374 696f 6e20 7061 7261 6d65 7465  lection paramete
+0000d450: 722c 0a20 2020 2020 2020 2020 2020 2073  r,.            s
+0000d460: 656c 6563 7469 6f6e 7320 6672 6f6d 2074  elections from t
+0000d470: 6861 7420 7061 7261 6d65 7465 7220 7769  hat parameter wi
+0000d480: 6c6c 206e 6f74 2074 7269 6767 6572 2061  ll not trigger a
+0000d490: 2072 6572 756e 2061 6e64 206e 6f74 2062   rerun and not b
+0000d4a0: 650a 2020 2020 2020 2020 2020 2020 696e  e.            in
+0000d4b0: 636c 7564 6564 2069 6e20 7468 6520 7365  cluded in the se
+0000d4c0: 6c65 6374 696f 6e20 7374 6174 652e 0a0a  lection state...
+0000d4d0: 2020 2020 2020 2020 2020 2020 5365 6c65              Sele
+0000d4e0: 6374 696f 6e20 7061 7261 6d65 7465 7273  ction parameters
+0000d4f0: 2061 7265 2069 6465 6e74 6966 6965 6420   are identified 
+0000d500: 6279 2074 6865 6972 2060 606e 616d 6560  by their ``name`
+0000d510: 6020 7072 6f70 6572 7479 2e0a 0a20 2020  ` property...   
+0000d520: 2020 2020 2052 6574 7572 6e73 0a20 2020       Returns.   
+0000d530: 2020 2020 202d 2d2d 2d2d 2d2d 0a20 2020       -------.   
+0000d540: 2020 2020 2065 6c65 6d65 6e74 206f 7220       element or 
+0000d550: 6469 6374 0a20 2020 2020 2020 2020 2020  dict.           
+0000d560: 2049 6620 6060 6f6e 5f73 656c 6563 7460   If ``on_select`
+0000d570: 6020 6973 2060 6022 6967 6e6f 7265 2260  ` is ``"ignore"`
+0000d580: 6020 2864 6566 6175 6c74 292c 2074 6869  ` (default), thi
+0000d590: 7320 6d65 7468 6f64 2072 6574 7572 6e73  s method returns
+0000d5a0: 2061 6e0a 2020 2020 2020 2020 2020 2020   an.            
+0000d5b0: 696e 7465 726e 616c 2070 6c61 6365 686f  internal placeho
+0000d5c0: 6c64 6572 2066 6f72 2074 6865 2063 6861  lder for the cha
+0000d5d0: 7274 2065 6c65 6d65 6e74 2074 6861 7420  rt element that 
+0000d5e0: 6361 6e20 6265 2075 7365 6420 7769 7468  can be used with
+0000d5f0: 0a20 2020 2020 2020 2020 2020 2074 6865  .            the
+0000d600: 2060 602e 6164 645f 726f 7773 2829 6060   ``.add_rows()``
+0000d610: 206d 6574 686f 642e 204f 7468 6572 7769   method. Otherwi
+0000d620: 7365 2c20 7468 6973 206d 6574 686f 6420  se, this method 
+0000d630: 7265 7475 726e 7320 610a 2020 2020 2020  returns a.      
+0000d640: 2020 2020 2020 6469 6374 696f 6e61 7279        dictionary
+0000d650: 2d6c 696b 6520 6f62 6a65 6374 2074 6861  -like object tha
+0000d660: 7420 7375 7070 6f72 7473 2062 6f74 6820  t supports both 
+0000d670: 6b65 7920 616e 6420 6174 7472 6962 7574  key and attribut
+0000d680: 650a 2020 2020 2020 2020 2020 2020 6e6f  e.            no
+0000d690: 7461 7469 6f6e 2e20 5468 6520 6174 7472  tation. The attr
+0000d6a0: 6962 7574 6573 2061 7265 2064 6573 6372  ibutes are descr
+0000d6b0: 6962 6564 2062 7920 7468 6520 6060 5665  ibed by the ``Ve
+0000d6c0: 6761 4c69 7465 5374 6174 6560 600a 2020  gaLiteState``.  
+0000d6d0: 2020 2020 2020 2020 2020 6469 6374 696f            dictio
+0000d6e0: 6e61 7279 2073 6368 656d 612e 0a0a 2020  nary schema...  
+0000d6f0: 2020 2020 2020 4578 616d 706c 650a 2020        Example.  
+0000d700: 2020 2020 2020 2d2d 2d2d 2d2d 2d0a 0a20        -------.. 
+0000d710: 2020 2020 2020 203e 3e3e 2069 6d70 6f72         >>> impor
+0000d720: 7420 7374 7265 616d 6c69 7420 6173 2073  t streamlit as s
+0000d730: 740a 2020 2020 2020 2020 3e3e 3e20 696d  t.        >>> im
+0000d740: 706f 7274 2070 616e 6461 7320 6173 2070  port pandas as p
+0000d750: 640a 2020 2020 2020 2020 3e3e 3e20 696d  d.        >>> im
+0000d760: 706f 7274 206e 756d 7079 2061 7320 6e70  port numpy as np
+0000d770: 0a20 2020 2020 2020 203e 3e3e 2069 6d70  .        >>> imp
+0000d780: 6f72 7420 616c 7461 6972 2061 7320 616c  ort altair as al
+0000d790: 740a 2020 2020 2020 2020 3e3e 3e0a 2020  t.        >>>.  
+0000d7a0: 2020 2020 2020 3e3e 3e20 6368 6172 745f        >>> chart_
+0000d7b0: 6461 7461 203d 2070 642e 4461 7461 4672  data = pd.DataFr
+0000d7c0: 616d 6528 6e70 2e72 616e 646f 6d2e 7261  ame(np.random.ra
+0000d7d0: 6e64 6e28 3230 2c20 3329 2c20 636f 6c75  ndn(20, 3), colu
+0000d7e0: 6d6e 733d 5b22 6122 2c20 2262 222c 2022  mns=["a", "b", "
+0000d7f0: 6322 5d29 0a20 2020 2020 2020 203e 3e3e  c"]).        >>>
+0000d800: 0a20 2020 2020 2020 203e 3e3e 2063 203d  .        >>> c =
+0000d810: 2028 0a20 2020 2020 2020 202e 2e2e 2020   (.        ...  
+0000d820: 2020 616c 742e 4368 6172 7428 6368 6172    alt.Chart(char
+0000d830: 745f 6461 7461 290a 2020 2020 2020 2020  t_data).        
+0000d840: 2e2e 2e20 2020 202e 6d61 726b 5f63 6972  ...    .mark_cir
+0000d850: 636c 6528 290a 2020 2020 2020 2020 2e2e  cle().        ..
+0000d860: 2e20 2020 202e 656e 636f 6465 2878 3d22  .    .encode(x="
+0000d870: 6122 2c20 793d 2262 222c 2073 697a 653d  a", y="b", size=
+0000d880: 2263 222c 2063 6f6c 6f72 3d22 6322 2c20  "c", color="c", 
+0000d890: 746f 6f6c 7469 703d 5b22 6122 2c20 2262  tooltip=["a", "b
+0000d8a0: 222c 2022 6322 5d29 0a20 2020 2020 2020  ", "c"]).       
+0000d8b0: 202e 2e2e 2029 0a20 2020 2020 2020 203e   ... ).        >
+0000d8c0: 3e3e 0a20 2020 2020 2020 203e 3e3e 2073  >>.        >>> s
+0000d8d0: 742e 616c 7461 6972 5f63 6861 7274 2863  t.altair_chart(c
+0000d8e0: 2c20 7573 655f 636f 6e74 6169 6e65 725f  , use_container_
+0000d8f0: 7769 6474 683d 5472 7565 290a 0a20 2020  width=True)..   
+0000d900: 2020 2020 202e 2e20 6f75 7470 7574 3a3a       .. output::
+0000d910: 0a20 2020 2020 2020 2020 2020 6874 7470  .           http
+0000d920: 733a 2f2f 646f 632d 7665 6761 2d6c 6974  s://doc-vega-lit
+0000d930: 652d 6368 6172 742e 7374 7265 616d 6c69  e-chart.streamli
+0000d940: 742e 6170 702f 0a20 2020 2020 2020 2020  t.app/.         
+0000d950: 2020 6865 6967 6874 3a20 3435 3070 780a    height: 450px.
+0000d960: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000d970: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+0000d980: 2e5f 616c 7461 6972 5f63 6861 7274 280a  ._altair_chart(.
+0000d990: 2020 2020 2020 2020 2020 2020 616c 7461              alta
+0000d9a0: 6972 5f63 6861 7274 3d61 6c74 6169 725f  ir_chart=altair_
+0000d9b0: 6368 6172 742c 0a20 2020 2020 2020 2020  chart,.         
+0000d9c0: 2020 2075 7365 5f63 6f6e 7461 696e 6572     use_container
+0000d9d0: 5f77 6964 7468 3d75 7365 5f63 6f6e 7461  _width=use_conta
+0000d9e0: 696e 6572 5f77 6964 7468 2c0a 2020 2020  iner_width,.    
+0000d9f0: 2020 2020 2020 2020 7468 656d 653d 7468          theme=th
+0000da00: 656d 652c 0a20 2020 2020 2020 2020 2020  eme,.           
+0000da10: 206b 6579 3d6b 6579 2c0a 2020 2020 2020   key=key,.      
+0000da20: 2020 2020 2020 6f6e 5f73 656c 6563 743d        on_select=
+0000da30: 6f6e 5f73 656c 6563 742c 0a20 2020 2020  on_select,.     
+0000da40: 2020 2020 2020 2073 656c 6563 7469 6f6e         selection
+0000da50: 5f6d 6f64 653d 7365 6c65 6374 696f 6e5f  _mode=selection_
+0000da60: 6d6f 6465 2c0a 2020 2020 2020 2020 290a  mode,.        ).
+0000da70: 0a20 2020 2040 6f76 6572 6c6f 6164 0a20  .    @overload. 
+0000da80: 2020 2064 6566 2076 6567 615f 6c69 7465     def vega_lite
+0000da90: 5f63 6861 7274 280a 2020 2020 2020 2020  _chart(.        
+0000daa0: 7365 6c66 2c0a 2020 2020 2020 2020 6461  self,.        da
+0000dab0: 7461 3a20 4461 7461 203d 204e 6f6e 652c  ta: Data = None,
+0000dac0: 0a20 2020 2020 2020 2073 7065 633a 2056  .        spec: V
+0000dad0: 6567 614c 6974 6553 7065 6320 7c20 4e6f  egaLiteSpec | No
+0000dae0: 6e65 203d 204e 6f6e 652c 0a20 2020 2020  ne = None,.     
+0000daf0: 2020 202a 2c0a 2020 2020 2020 2020 7573     *,.        us
+0000db00: 655f 636f 6e74 6169 6e65 725f 7769 6474  e_container_widt
+0000db10: 683a 2062 6f6f 6c20 3d20 4661 6c73 652c  h: bool = False,
+0000db20: 0a20 2020 2020 2020 2074 6865 6d65 3a20  .        theme: 
+0000db30: 4c69 7465 7261 6c5b 2273 7472 6561 6d6c  Literal["streaml
+0000db40: 6974 225d 207c 204e 6f6e 6520 3d20 2273  it"] | None = "s
+0000db50: 7472 6561 6d6c 6974 222c 0a20 2020 2020  treamlit",.     
+0000db60: 2020 206b 6579 3a20 4b65 7920 7c20 4e6f     key: Key | No
+0000db70: 6e65 203d 204e 6f6e 652c 0a20 2020 2020  ne = None,.     
+0000db80: 2020 206f 6e5f 7365 6c65 6374 3a20 4c69     on_select: Li
+0000db90: 7465 7261 6c5b 2269 676e 6f72 6522 5d2c  teral["ignore"],
+0000dba0: 2020 2320 4e6f 2064 6566 6175 6c74 2076    # No default v
+0000dbb0: 616c 7565 2068 6572 6520 746f 206d 616b  alue here to mak
+0000dbc0: 6520 6974 2077 6f72 6b20 7769 7468 206d  e it work with m
+0000dbd0: 7970 790a 2020 2020 2020 2020 7365 6c65  ypy.        sele
+0000dbe0: 6374 696f 6e5f 6d6f 6465 3a20 7374 7220  ction_mode: str 
+0000dbf0: 7c20 4974 6572 6162 6c65 5b73 7472 5d20  | Iterable[str] 
+0000dc00: 7c20 4e6f 6e65 203d 204e 6f6e 652c 0a20  | None = None,. 
+0000dc10: 2020 2020 2020 202a 2a6b 7761 7267 733a         **kwargs:
+0000dc20: 2041 6e79 2c0a 2020 2020 2920 2d3e 2044   Any,.    ) -> D
+0000dc30: 656c 7461 4765 6e65 7261 746f 723a 0a20  eltaGenerator:. 
+0000dc40: 2020 2020 2020 202e 2e2e 0a0a 2020 2020         .....    
+0000dc50: 406f 7665 726c 6f61 640a 2020 2020 6465  @overload.    de
+0000dc60: 6620 7665 6761 5f6c 6974 655f 6368 6172  f vega_lite_char
+0000dc70: 7428 0a20 2020 2020 2020 2073 656c 662c  t(.        self,
+0000dc80: 0a20 2020 2020 2020 2064 6174 613a 2044  .        data: D
+0000dc90: 6174 6120 3d20 4e6f 6e65 2c0a 2020 2020  ata = None,.    
+0000dca0: 2020 2020 7370 6563 3a20 5665 6761 4c69      spec: VegaLi
+0000dcb0: 7465 5370 6563 207c 204e 6f6e 6520 3d20  teSpec | None = 
+0000dcc0: 4e6f 6e65 2c0a 2020 2020 2020 2020 2a2c  None,.        *,
+0000dcd0: 0a20 2020 2020 2020 2075 7365 5f63 6f6e  .        use_con
+0000dce0: 7461 696e 6572 5f77 6964 7468 3a20 626f  tainer_width: bo
+0000dcf0: 6f6c 203d 2046 616c 7365 2c0a 2020 2020  ol = False,.    
+0000dd00: 2020 2020 7468 656d 653a 204c 6974 6572      theme: Liter
+0000dd10: 616c 5b22 7374 7265 616d 6c69 7422 5d20  al["streamlit"] 
+0000dd20: 7c20 4e6f 6e65 203d 2022 7374 7265 616d  | None = "stream
+0000dd30: 6c69 7422 2c0a 2020 2020 2020 2020 6b65  lit",.        ke
+0000dd40: 793a 204b 6579 207c 204e 6f6e 6520 3d20  y: Key | None = 
+0000dd50: 4e6f 6e65 2c0a 2020 2020 2020 2020 6f6e  None,.        on
+0000dd60: 5f73 656c 6563 743a 204c 6974 6572 616c  _select: Literal
+0000dd70: 5b22 7265 7275 6e22 5d20 7c20 5769 6467  ["rerun"] | Widg
+0000dd80: 6574 4361 6c6c 6261 636b 203d 2022 7265  etCallback = "re
+0000dd90: 7275 6e22 2c0a 2020 2020 2020 2020 7365  run",.        se
+0000dda0: 6c65 6374 696f 6e5f 6d6f 6465 3a20 7374  lection_mode: st
+0000ddb0: 7220 7c20 4974 6572 6162 6c65 5b73 7472  r | Iterable[str
+0000ddc0: 5d20 7c20 4e6f 6e65 203d 204e 6f6e 652c  ] | None = None,
+0000ddd0: 0a20 2020 2020 2020 202a 2a6b 7761 7267  .        **kwarg
+0000dde0: 733a 2041 6e79 2c0a 2020 2020 2920 2d3e  s: Any,.    ) ->
+0000ddf0: 2056 6567 614c 6974 6553 7461 7465 3a0a   VegaLiteState:.
+0000de00: 2020 2020 2020 2020 2e2e 2e0a 0a20 2020          .....   
+0000de10: 2040 6761 7468 6572 5f6d 6574 7269 6373   @gather_metrics
+0000de20: 2822 7665 6761 5f6c 6974 655f 6368 6172  ("vega_lite_char
+0000de30: 7422 290a 2020 2020 6465 6620 7665 6761  t").    def vega
+0000de40: 5f6c 6974 655f 6368 6172 7428 0a20 2020  _lite_chart(.   
+0000de50: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+0000de60: 2020 2064 6174 613a 2044 6174 6120 3d20     data: Data = 
+0000de70: 4e6f 6e65 2c0a 2020 2020 2020 2020 7370  None,.        sp
+0000de80: 6563 3a20 5665 6761 4c69 7465 5370 6563  ec: VegaLiteSpec
+0000de90: 207c 204e 6f6e 6520 3d20 4e6f 6e65 2c0a   | None = None,.
+0000dea0: 2020 2020 2020 2020 2a2c 0a20 2020 2020          *,.     
+0000deb0: 2020 2075 7365 5f63 6f6e 7461 696e 6572     use_container
+0000dec0: 5f77 6964 7468 3a20 626f 6f6c 203d 2046  _width: bool = F
+0000ded0: 616c 7365 2c0a 2020 2020 2020 2020 7468  alse,.        th
+0000dee0: 656d 653a 204c 6974 6572 616c 5b22 7374  eme: Literal["st
+0000def0: 7265 616d 6c69 7422 5d20 7c20 4e6f 6e65  reamlit"] | None
+0000df00: 203d 2022 7374 7265 616d 6c69 7422 2c0a   = "streamlit",.
+0000df10: 2020 2020 2020 2020 6b65 793a 204b 6579          key: Key
+0000df20: 207c 204e 6f6e 6520 3d20 4e6f 6e65 2c0a   | None = None,.
+0000df30: 2020 2020 2020 2020 6f6e 5f73 656c 6563          on_selec
+0000df40: 743a 204c 6974 6572 616c 5b22 7265 7275  t: Literal["reru
+0000df50: 6e22 2c20 2269 676e 6f72 6522 5d20 7c20  n", "ignore"] | 
+0000df60: 5769 6467 6574 4361 6c6c 6261 636b 203d  WidgetCallback =
+0000df70: 2022 6967 6e6f 7265 222c 0a20 2020 2020   "ignore",.     
+0000df80: 2020 2073 656c 6563 7469 6f6e 5f6d 6f64     selection_mod
+0000df90: 653a 2073 7472 207c 2049 7465 7261 626c  e: str | Iterabl
+0000dfa0: 655b 7374 725d 207c 204e 6f6e 6520 3d20  e[str] | None = 
+0000dfb0: 4e6f 6e65 2c0a 2020 2020 2020 2020 2a2a  None,.        **
+0000dfc0: 6b77 6172 6773 3a20 416e 792c 0a20 2020  kwargs: Any,.   
+0000dfd0: 2029 202d 3e20 4465 6c74 6147 656e 6572   ) -> DeltaGener
+0000dfe0: 6174 6f72 207c 2056 6567 614c 6974 6553  ator | VegaLiteS
+0000dff0: 7461 7465 3a0a 2020 2020 2020 2020 2222  tate:.        ""
+0000e000: 2244 6973 706c 6179 2061 2063 6861 7274  "Display a chart
+0000e010: 2075 7369 6e67 2074 6865 2056 6567 612d   using the Vega-
+0000e020: 4c69 7465 206c 6962 7261 7279 2e0a 0a20  Lite library... 
+0000e030: 2020 2020 2020 2060 5665 6761 2d4c 6974         `Vega-Lit
+0000e040: 6520 3c68 7474 7073 3a2f 2f76 6567 612e  e <https://vega.
+0000e050: 6769 7468 7562 2e69 6f2f 7665 6761 2d6c  github.io/vega-l
+0000e060: 6974 652f 3e60 5f20 6973 2061 2068 6967  ite/>`_ is a hig
+0000e070: 682d 6c65 7665 6c0a 2020 2020 2020 2020  h-level.        
+0000e080: 6772 616d 6d61 7220 666f 7220 6465 6669  grammar for defi
+0000e090: 6e69 6e67 2069 6e74 6572 6163 7469 7665  ning interactive
+0000e0a0: 2067 7261 7068 6963 732e 0a0a 2020 2020   graphics...    
+0000e0b0: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
+0000e0c0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
+0000e0d0: 2d0a 2020 2020 2020 2020 6461 7461 203a  -.        data :
+0000e0e0: 2070 616e 6461 732e 4461 7461 4672 616d   pandas.DataFram
+0000e0f0: 652c 2070 616e 6461 732e 5374 796c 6572  e, pandas.Styler
+0000e100: 2c20 7079 6172 726f 772e 5461 626c 652c  , pyarrow.Table,
+0000e110: 206e 756d 7079 2e6e 6461 7272 6179 2c20   numpy.ndarray, 
+0000e120: 4974 6572 6162 6c65 2c20 6469 6374 2c20  Iterable, dict, 
+0000e130: 6f72 204e 6f6e 650a 2020 2020 2020 2020  or None.        
+0000e140: 2020 2020 4569 7468 6572 2074 6865 2064      Either the d
+0000e150: 6174 6120 746f 2062 6520 706c 6f74 7465  ata to be plotte
+0000e160: 6420 6f72 2061 2056 6567 612d 4c69 7465  d or a Vega-Lite
+0000e170: 2073 7065 6320 636f 6e74 6169 6e69 6e67   spec containing
+0000e180: 2074 6865 0a20 2020 2020 2020 2020 2020   the.           
+0000e190: 2064 6174 6120 2877 6869 6368 206d 6f72   data (which mor
+0000e1a0: 6520 636c 6f73 656c 7920 666f 6c6c 6f77  e closely follow
+0000e1b0: 7320 7468 6520 5665 6761 2d4c 6974 6520  s the Vega-Lite 
+0000e1c0: 4150 4929 2e0a 0a20 2020 2020 2020 2073  API)...        s
+0000e1d0: 7065 6320 3a20 6469 6374 206f 7220 4e6f  pec : dict or No
+0000e1e0: 6e65 0a20 2020 2020 2020 2020 2020 2054  ne.            T
+0000e1f0: 6865 2056 6567 612d 4c69 7465 2073 7065  he Vega-Lite spe
+0000e200: 6320 666f 7220 7468 6520 6368 6172 742e  c for the chart.
+0000e210: 2049 6620 6060 7370 6563 6060 2069 7320   If ``spec`` is 
+0000e220: 6060 4e6f 6e65 6060 2028 6465 6661 756c  ``None`` (defaul
+0000e230: 7429 2c0a 2020 2020 2020 2020 2020 2020  t),.            
+0000e240: 5374 7265 616d 6c69 7420 7573 6573 2074  Streamlit uses t
+0000e250: 6865 2073 7065 6320 7061 7373 6564 2069  he spec passed i
+0000e260: 6e20 6060 6461 7461 6060 2e20 596f 7520  n ``data``. You 
+0000e270: 6361 6e6e 6f74 2070 6173 7320 6120 7370  cannot pass a sp
+0000e280: 6563 0a20 2020 2020 2020 2020 2020 2074  ec.            t
+0000e290: 6f20 626f 7468 2060 6064 6174 6160 6020  o both ``data`` 
+0000e2a0: 616e 6420 6060 7370 6563 6060 2e20 5365  and ``spec``. Se
+0000e2b0: 650a 2020 2020 2020 2020 2020 2020 6874  e.            ht
+0000e2c0: 7470 733a 2f2f 7665 6761 2e67 6974 6875  tps://vega.githu
+0000e2d0: 622e 696f 2f76 6567 612d 6c69 7465 2f64  b.io/vega-lite/d
+0000e2e0: 6f63 732f 2066 6f72 206d 6f72 6520 696e  ocs/ for more in
+0000e2f0: 666f 2e0a 0a20 2020 2020 2020 2075 7365  fo...        use
+0000e300: 5f63 6f6e 7461 696e 6572 5f77 6964 7468  _container_width
+0000e310: 203a 2062 6f6f 6c0a 2020 2020 2020 2020   : bool.        
+0000e320: 2020 2020 5768 6574 6865 7220 746f 206f      Whether to o
+0000e330: 7665 7272 6964 6520 7468 6520 6669 6775  verride the figu
+0000e340: 7265 2773 206e 6174 6976 6520 7769 6474  re's native widt
+0000e350: 6820 7769 7468 2074 6865 2077 6964 7468  h with the width
+0000e360: 206f 660a 2020 2020 2020 2020 2020 2020   of.            
+0000e370: 7468 6520 7061 7265 6e74 2063 6f6e 7461  the parent conta
+0000e380: 696e 6572 2e20 4966 2060 6075 7365 5f63  iner. If ``use_c
+0000e390: 6f6e 7461 696e 6572 5f77 6964 7468 6060  ontainer_width``
+0000e3a0: 2069 7320 6060 4661 6c73 6560 600a 2020   is ``False``.  
+0000e3b0: 2020 2020 2020 2020 2020 2864 6566 6175            (defau
+0000e3c0: 6c74 292c 2053 7472 6561 6d6c 6974 2073  lt), Streamlit s
+0000e3d0: 6574 7320 7468 6520 7769 6474 6820 6f66  ets the width of
+0000e3e0: 2074 6865 2063 6861 7274 2074 6f20 6669   the chart to fi
+0000e3f0: 7420 6974 7320 636f 6e74 656e 7473 0a20  t its contents. 
+0000e400: 2020 2020 2020 2020 2020 2061 6363 6f72             accor
+0000e410: 6469 6e67 2074 6f20 7468 6520 706c 6f74  ding to the plot
+0000e420: 7469 6e67 206c 6962 7261 7279 2c20 7570  ting library, up
+0000e430: 2074 6f20 7468 6520 7769 6474 6820 6f66   to the width of
+0000e440: 2074 6865 2070 6172 656e 740a 2020 2020   the parent.    
+0000e450: 2020 2020 2020 2020 636f 6e74 6169 6e65          containe
+0000e460: 722e 2049 6620 6060 7573 655f 636f 6e74  r. If ``use_cont
+0000e470: 6169 6e65 725f 7769 6474 6860 6020 6973  ainer_width`` is
+0000e480: 2060 6054 7275 6560 602c 2053 7472 6561   ``True``, Strea
+0000e490: 6d6c 6974 2073 6574 730a 2020 2020 2020  mlit sets.      
+0000e4a0: 2020 2020 2020 7468 6520 7769 6474 6820        the width 
+0000e4b0: 6f66 2074 6865 2066 6967 7572 6520 746f  of the figure to
+0000e4c0: 206d 6174 6368 2074 6865 2077 6964 7468   match the width
+0000e4d0: 206f 6620 7468 6520 7061 7265 6e74 2063   of the parent c
+0000e4e0: 6f6e 7461 696e 6572 2e0a 0a20 2020 2020  ontainer...     
+0000e4f0: 2020 2074 6865 6d65 203a 2022 7374 7265     theme : "stre
+0000e500: 616d 6c69 7422 206f 7220 4e6f 6e65 0a20  amlit" or None. 
+0000e510: 2020 2020 2020 2020 2020 2054 6865 2074             The t
+0000e520: 6865 6d65 206f 6620 7468 6520 6368 6172  heme of the char
+0000e530: 742e 2049 6620 6060 7468 656d 6560 6020  t. If ``theme`` 
+0000e540: 6973 2060 6022 7374 7265 616d 6c69 7422  is ``"streamlit"
+0000e550: 6060 2028 6465 6661 756c 7429 2c0a 2020  `` (default),.  
+0000e560: 2020 2020 2020 2020 2020 5374 7265 616d            Stream
+0000e570: 6c69 7420 7573 6573 2069 7473 206f 776e  lit uses its own
+0000e580: 2064 6573 6967 6e20 6465 6661 756c 742e   design default.
+0000e590: 2049 6620 6060 7468 656d 6560 6020 6973   If ``theme`` is
+0000e5a0: 2060 604e 6f6e 6560 602c 0a20 2020 2020   ``None``,.     
+0000e5b0: 2020 2020 2020 2053 7472 6561 6d6c 6974         Streamlit
+0000e5c0: 2066 616c 6c73 2062 6163 6b20 746f 2074   falls back to t
+0000e5d0: 6865 2064 6566 6175 6c74 2062 6568 6176  he default behav
+0000e5e0: 696f 7220 6f66 2074 6865 206c 6962 7261  ior of the libra
+0000e5f0: 7279 2e0a 0a20 2020 2020 2020 206b 6579  ry...        key
+0000e600: 203a 2073 7472 0a20 2020 2020 2020 2020   : str.         
+0000e610: 2020 2041 6e20 6f70 7469 6f6e 616c 2073     An optional s
+0000e620: 7472 696e 6720 746f 2075 7365 2066 6f72  tring to use for
+0000e630: 2067 6976 696e 6720 7468 6973 2065 6c65   giving this ele
+0000e640: 6d65 6e74 2061 2073 7461 626c 650a 2020  ment a stable.  
+0000e650: 2020 2020 2020 2020 2020 6964 656e 7469            identi
+0000e660: 7479 2e20 4966 2060 606b 6579 6060 2069  ty. If ``key`` i
+0000e670: 7320 6060 4e6f 6e65 6060 2028 6465 6661  s ``None`` (defa
+0000e680: 756c 7429 2c20 7468 6973 2065 6c65 6d65  ult), this eleme
+0000e690: 6e74 2773 2069 6465 6e74 6974 790a 2020  nt's identity.  
+0000e6a0: 2020 2020 2020 2020 2020 7769 6c6c 2062            will b
+0000e6b0: 6520 6465 7465 726d 696e 6564 2062 6173  e determined bas
+0000e6c0: 6564 206f 6e20 7468 6520 7661 6c75 6573  ed on the values
+0000e6d0: 206f 6620 7468 6520 6f74 6865 7220 7061   of the other pa
+0000e6e0: 7261 6d65 7465 7273 2e0a 0a20 2020 2020  rameters...     
+0000e6f0: 2020 2020 2020 2041 6464 6974 696f 6e61         Additiona
+0000e700: 6c6c 792c 2069 6620 7365 6c65 6374 696f  lly, if selectio
+0000e710: 6e73 2061 7265 2061 6374 6976 6174 6564  ns are activated
+0000e720: 2061 6e64 2060 606b 6579 6060 2069 7320   and ``key`` is 
+0000e730: 7072 6f76 6964 6564 2c0a 2020 2020 2020  provided,.      
+0000e740: 2020 2020 2020 5374 7265 616d 6c69 7420        Streamlit 
+0000e750: 7769 6c6c 2072 6567 6973 7465 7220 7468  will register th
+0000e760: 6520 6b65 7920 696e 2053 6573 7369 6f6e  e key in Session
+0000e770: 2053 7461 7465 2074 6f20 7374 6f72 6520   State to store 
+0000e780: 7468 650a 2020 2020 2020 2020 2020 2020  the.            
+0000e790: 7365 6c65 6374 696f 6e20 7374 6174 652e  selection state.
+0000e7a0: 2054 6865 2073 656c 6563 7469 6f6e 2073   The selection s
+0000e7b0: 7461 7465 2069 7320 7265 6164 2d6f 6e6c  tate is read-onl
+0000e7c0: 792e 0a0a 2020 2020 2020 2020 6f6e 5f73  y...        on_s
+0000e7d0: 656c 6563 7420 3a20 2269 676e 6f72 6522  elect : "ignore"
+0000e7e0: 2c20 2272 6572 756e 222c 206f 7220 6361  , "rerun", or ca
+0000e7f0: 6c6c 6162 6c65 0a20 2020 2020 2020 2020  llable.         
+0000e800: 2020 2048 6f77 2074 6865 2066 6967 7572     How the figur
+0000e810: 6520 7368 6f75 6c64 2072 6573 706f 6e64  e should respond
+0000e820: 2074 6f20 7573 6572 2073 656c 6563 7469   to user selecti
+0000e830: 6f6e 2065 7665 6e74 732e 2054 6869 730a  on events. This.
+0000e840: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
+0000e850: 726f 6c73 2077 6865 7468 6572 206f 7220  rols whether or 
+0000e860: 6e6f 7420 7468 6520 6669 6775 7265 2062  not the figure b
+0000e870: 6568 6176 6573 206c 696b 6520 616e 2069  ehaves like an i
+0000e880: 6e70 7574 2077 6964 6765 742e 0a20 2020  nput widget..   
+0000e890: 2020 2020 2020 2020 2060 606f 6e5f 7365           ``on_se
+0000e8a0: 6c65 6374 6060 2063 616e 2062 6520 6f6e  lect`` can be on
+0000e8b0: 6520 6f66 2074 6865 2066 6f6c 6c6f 7769  e of the followi
+0000e8c0: 6e67 3a0a 0a20 2020 2020 2020 2020 2020  ng:..           
+0000e8d0: 202d 2060 6022 6967 6e6f 7265 2260 6020   - ``"ignore"`` 
+0000e8e0: 2864 6566 6175 6c74 293a 2053 7472 6561  (default): Strea
+0000e8f0: 6d6c 6974 2077 696c 6c20 6e6f 7420 7265  mlit will not re
+0000e900: 6163 7420 746f 2061 6e79 2073 656c 6563  act to any selec
+0000e910: 7469 6f6e 0a20 2020 2020 2020 2020 2020  tion.           
+0000e920: 2020 2065 7665 6e74 7320 696e 2074 6865     events in the
+0000e930: 2063 6861 7274 2e20 5468 6520 6669 6775   chart. The figu
+0000e940: 7265 2077 696c 6c20 6e6f 7420 6265 6861  re will not beha
+0000e950: 7665 206c 696b 6520 616e 2069 6e70 7574  ve like an input
+0000e960: 0a20 2020 2020 2020 2020 2020 2020 2077  .              w
+0000e970: 6964 6765 742e 0a0a 2020 2020 2020 2020  idget...        
+0000e980: 2020 2020 2d20 6060 2272 6572 756e 2260      - ``"rerun"`
+0000e990: 603a 2053 7472 6561 6d6c 6974 2077 696c  `: Streamlit wil
+0000e9a0: 6c20 7265 7275 6e20 7468 6520 6170 7020  l rerun the app 
+0000e9b0: 7768 656e 2074 6865 2075 7365 7220 7365  when the user se
+0000e9c0: 6c65 6374 730a 2020 2020 2020 2020 2020  lects.          
+0000e9d0: 2020 2020 6461 7461 2069 6e20 7468 6520      data in the 
+0000e9e0: 6368 6172 742e 2049 6e20 7468 6973 2063  chart. In this c
+0000e9f0: 6173 652c 2060 6073 742e 7665 6761 5f6c  ase, ``st.vega_l
+0000ea00: 6974 655f 6368 6172 7460 6020 7769 6c6c  ite_chart`` will
+0000ea10: 0a20 2020 2020 2020 2020 2020 2020 2072  .              r
+0000ea20: 6574 7572 6e20 7468 6520 7365 6c65 6374  eturn the select
+0000ea30: 696f 6e20 6461 7461 2061 7320 6120 6469  ion data as a di
+0000ea40: 6374 696f 6e61 7279 2e0a 0a20 2020 2020  ctionary...     
+0000ea50: 2020 2020 2020 202d 2041 2060 6063 616c         - A ``cal
+0000ea60: 6c61 626c 6560 603a 2053 7472 6561 6d6c  lable``: Streaml
+0000ea70: 6974 2077 696c 6c20 7265 7275 6e20 7468  it will rerun th
+0000ea80: 6520 6170 7020 616e 6420 6578 6563 7574  e app and execut
+0000ea90: 6520 7468 650a 2020 2020 2020 2020 2020  e the.          
+0000eaa0: 2020 2020 6060 6361 6c6c 6162 6c65 6060      ``callable``
+0000eab0: 2061 7320 6120 6361 6c6c 6261 636b 2066   as a callback f
+0000eac0: 756e 6374 696f 6e20 6265 666f 7265 2074  unction before t
+0000ead0: 6865 2072 6573 7420 6f66 2074 6865 2061  he rest of the a
+0000eae0: 7070 2e0a 2020 2020 2020 2020 2020 2020  pp..            
+0000eaf0: 2020 496e 2074 6869 7320 6361 7365 2c20    In this case, 
+0000eb00: 6060 7374 2e76 6567 615f 6c69 7465 5f63  ``st.vega_lite_c
+0000eb10: 6861 7274 6060 2077 696c 6c20 7265 7475  hart`` will retu
+0000eb20: 726e 2074 6865 2073 656c 6563 7469 6f6e  rn the selection
+0000eb30: 2064 6174 610a 2020 2020 2020 2020 2020   data.          
+0000eb40: 2020 2020 6173 2061 2064 6963 7469 6f6e      as a diction
+0000eb50: 6172 792e 0a0a 2020 2020 2020 2020 2020  ary...          
+0000eb60: 2020 546f 2075 7365 2073 656c 6563 7469    To use selecti
+0000eb70: 6f6e 2065 7665 6e74 732c 2074 6865 2056  on events, the V
+0000eb80: 6567 612d 4c69 7465 2073 7065 6320 6465  ega-Lite spec de
+0000eb90: 6669 6e65 6420 696e 2060 6064 6174 6160  fined in ``data`
+0000eba0: 6020 6f72 0a20 2020 2020 2020 2020 2020  ` or.           
+0000ebb0: 2060 6073 7065 6360 6020 6d75 7374 2069   ``spec`` must i
+0000ebc0: 6e63 6c75 6465 2073 656c 6563 7469 6f6e  nclude selection
+0000ebd0: 2070 6172 616d 6574 6572 7320 6672 6f6d   parameters from
+0000ebe0: 2074 6865 2074 6865 2063 6861 7274 696e   the the chartin
+0000ebf0: 670a 2020 2020 2020 2020 2020 2020 6c69  g.            li
+0000ec00: 6272 6172 792e 2054 6f20 6c65 6172 6e20  brary. To learn 
+0000ec10: 6162 6f75 7420 6465 6669 6e69 6e67 2069  about defining i
+0000ec20: 6e74 6572 6163 7469 6f6e 7320 696e 2056  nteractions in V
+0000ec30: 6567 612d 4c69 7465 2c20 7365 650a 2020  ega-Lite, see.  
+0000ec40: 2020 2020 2020 2020 2020 6044 796e 616d            `Dynam
+0000ec50: 6963 2042 6568 6176 696f 7273 2077 6974  ic Behaviors wit
+0000ec60: 6820 5061 7261 6d65 7465 7273 205c 0a20  h Parameters \. 
+0000ec70: 2020 2020 2020 2020 2020 203c 6874 7470             <http
+0000ec80: 733a 2f2f 7665 6761 2e67 6974 6875 622e  s://vega.github.
+0000ec90: 696f 2f76 6567 612d 6c69 7465 2f64 6f63  io/vega-lite/doc
+0000eca0: 732f 7061 7261 6d65 7465 722e 6874 6d6c  s/parameter.html
+0000ecb0: 3e60 5f0a 2020 2020 2020 2020 2020 2020  >`_.            
+0000ecc0: 696e 2056 6567 612d 4c69 7465 2773 2064  in Vega-Lite's d
+0000ecd0: 6f63 756d 656e 7461 7469 6f6e 2e0a 0a20  ocumentation... 
+0000ece0: 2020 2020 2020 2073 656c 6563 7469 6f6e         selection
+0000ecf0: 5f6d 6f64 6520 3a20 7374 7220 6f72 2049  _mode : str or I
+0000ed00: 7465 7261 626c 6520 6f66 2073 7472 0a20  terable of str. 
+0000ed10: 2020 2020 2020 2020 2020 2054 6865 2073             The s
+0000ed20: 656c 6563 7469 6f6e 2070 6172 616d 6574  election paramet
+0000ed30: 6572 7320 5374 7265 616d 6c69 7420 7368  ers Streamlit sh
+0000ed40: 6f75 6c64 2075 7365 2e20 4966 0a20 2020  ould use. If.   
+0000ed50: 2020 2020 2020 2020 2060 6073 656c 6563           ``selec
+0000ed60: 7469 6f6e 5f6d 6f64 6560 6020 6973 2060  tion_mode`` is `
+0000ed70: 604e 6f6e 6560 6020 2864 6566 6175 6c74  `None`` (default
+0000ed80: 292c 2053 7472 6561 6d6c 6974 2077 696c  ), Streamlit wil
+0000ed90: 6c20 7573 6520 616c 6c0a 2020 2020 2020  l use all.      
+0000eda0: 2020 2020 2020 7365 6c65 6374 696f 6e20        selection 
+0000edb0: 7061 7261 6d65 7465 7273 2064 6566 696e  parameters defin
+0000edc0: 6564 2069 6e20 7468 6520 6368 6172 7427  ed in the chart'
+0000edd0: 7320 5665 6761 2d4c 6974 6520 7370 6563  s Vega-Lite spec
+0000ede0: 2e0a 0a20 2020 2020 2020 2020 2020 2057  ...            W
+0000edf0: 6865 6e20 5374 7265 616d 6c69 7420 7573  hen Streamlit us
+0000ee00: 6573 2061 2073 656c 6563 7469 6f6e 2070  es a selection p
+0000ee10: 6172 616d 6574 6572 2c20 7365 6c65 6374  arameter, select
+0000ee20: 696f 6e73 2066 726f 6d20 7468 6174 0a20  ions from that. 
+0000ee30: 2020 2020 2020 2020 2020 2070 6172 616d             param
+0000ee40: 6574 6572 2077 696c 6c20 7472 6967 6765  eter will trigge
+0000ee50: 7220 6120 7265 7275 6e20 616e 6420 6265  r a rerun and be
+0000ee60: 2069 6e63 6c75 6465 6420 696e 2074 6865   included in the
+0000ee70: 2073 656c 6563 7469 6f6e 0a20 2020 2020   selection.     
+0000ee80: 2020 2020 2020 2073 7461 7465 2e20 5768         state. Wh
+0000ee90: 656e 2053 7472 6561 6d6c 6974 2064 6f65  en Streamlit doe
+0000eea0: 7320 6e6f 7420 7573 6520 6120 7365 6c65  s not use a sele
+0000eeb0: 6374 696f 6e20 7061 7261 6d65 7465 722c  ction parameter,
+0000eec0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000eed0: 6563 7469 6f6e 7320 6672 6f6d 2074 6861  ections from tha
+0000eee0: 7420 7061 7261 6d65 7465 7220 7769 6c6c  t parameter will
+0000eef0: 206e 6f74 2074 7269 6767 6572 2061 2072   not trigger a r
+0000ef00: 6572 756e 2061 6e64 206e 6f74 2062 650a  erun and not be.
+0000ef10: 2020 2020 2020 2020 2020 2020 696e 636c              incl
+0000ef20: 7564 6564 2069 6e20 7468 6520 7365 6c65  uded in the sele
+0000ef30: 6374 696f 6e20 7374 6174 652e 0a0a 2020  ction state...  
+0000ef40: 2020 2020 2020 2020 2020 5365 6c65 6374            Select
+0000ef50: 696f 6e20 7061 7261 6d65 7465 7273 2061  ion parameters a
+0000ef60: 7265 2069 6465 6e74 6966 6965 6420 6279  re identified by
+0000ef70: 2074 6865 6972 2060 606e 616d 6560 6020   their ``name`` 
+0000ef80: 7072 6f70 6572 7479 2e0a 0a20 2020 2020  property...     
+0000ef90: 2020 202a 2a6b 7761 7267 7320 3a20 616e     **kwargs : an
+0000efa0: 790a 2020 2020 2020 2020 2020 2020 5468  y.            Th
+0000efb0: 6520 5665 6761 2d4c 6974 6520 7370 6563  e Vega-Lite spec
+0000efc0: 2066 6f72 2074 6865 2063 6861 7274 2061   for the chart a
+0000efd0: 7320 6b65 7977 6f72 6473 2e20 5468 6973  s keywords. This
+0000efe0: 2069 7320 616e 2061 6c74 6572 6e61 7469   is an alternati
+0000eff0: 7665 0a20 2020 2020 2020 2020 2020 2074  ve.            t
+0000f000: 6f20 6060 7370 6563 6060 2e0a 0a20 2020  o ``spec``...   
+0000f010: 2020 2020 2052 6574 7572 6e73 0a20 2020       Returns.   
+0000f020: 2020 2020 202d 2d2d 2d2d 2d2d 0a20 2020       -------.   
+0000f030: 2020 2020 2065 6c65 6d65 6e74 206f 7220       element or 
+0000f040: 6469 6374 0a20 2020 2020 2020 2020 2020  dict.           
+0000f050: 2049 6620 6060 6f6e 5f73 656c 6563 7460   If ``on_select`
+0000f060: 6020 6973 2060 6022 6967 6e6f 7265 2260  ` is ``"ignore"`
+0000f070: 6020 2864 6566 6175 6c74 292c 2074 6869  ` (default), thi
+0000f080: 7320 6d65 7468 6f64 2072 6574 7572 6e73  s method returns
+0000f090: 2061 6e0a 2020 2020 2020 2020 2020 2020   an.            
+0000f0a0: 696e 7465 726e 616c 2070 6c61 6365 686f  internal placeho
+0000f0b0: 6c64 6572 2066 6f72 2074 6865 2063 6861  lder for the cha
+0000f0c0: 7274 2065 6c65 6d65 6e74 2074 6861 7420  rt element that 
+0000f0d0: 6361 6e20 6265 2075 7365 6420 7769 7468  can be used with
+0000f0e0: 0a20 2020 2020 2020 2020 2020 2074 6865  .            the
+0000f0f0: 2060 602e 6164 645f 726f 7773 2829 6060   ``.add_rows()``
+0000f100: 206d 6574 686f 642e 204f 7468 6572 7769   method. Otherwi
+0000f110: 7365 2c20 7468 6973 206d 6574 686f 6420  se, this method 
+0000f120: 7265 7475 726e 7320 610a 2020 2020 2020  returns a.      
+0000f130: 2020 2020 2020 6469 6374 696f 6e61 7279        dictionary
+0000f140: 2d6c 696b 6520 6f62 6a65 6374 2074 6861  -like object tha
+0000f150: 7420 7375 7070 6f72 7473 2062 6f74 6820  t supports both 
+0000f160: 6b65 7920 616e 6420 6174 7472 6962 7574  key and attribut
+0000f170: 650a 2020 2020 2020 2020 2020 2020 6e6f  e.            no
+0000f180: 7461 7469 6f6e 2e20 5468 6520 6174 7472  tation. The attr
+0000f190: 6962 7574 6573 2061 7265 2064 6573 6372  ibutes are descr
+0000f1a0: 6962 6564 2062 7920 7468 6520 6060 5665  ibed by the ``Ve
+0000f1b0: 6761 4c69 7465 5374 6174 6560 600a 2020  gaLiteState``.  
+0000f1c0: 2020 2020 2020 2020 2020 6469 6374 696f            dictio
+0000f1d0: 6e61 7279 2073 6368 656d 612e 0a0a 2020  nary schema...  
+0000f1e0: 2020 2020 2020 4578 616d 706c 650a 2020        Example.  
+0000f1f0: 2020 2020 2020 2d2d 2d2d 2d2d 2d0a 2020        -------.  
+0000f200: 2020 2020 2020 3e3e 3e20 696d 706f 7274        >>> import
+0000f210: 2073 7472 6561 6d6c 6974 2061 7320 7374   streamlit as st
+0000f220: 0a20 2020 2020 2020 203e 3e3e 2069 6d70  .        >>> imp
+0000f230: 6f72 7420 7061 6e64 6173 2061 7320 7064  ort pandas as pd
+0000f240: 0a20 2020 2020 2020 203e 3e3e 2069 6d70  .        >>> imp
+0000f250: 6f72 7420 6e75 6d70 7920 6173 206e 700a  ort numpy as np.
+0000f260: 2020 2020 2020 2020 3e3e 3e0a 2020 2020          >>>.    
+0000f270: 2020 2020 3e3e 3e20 6368 6172 745f 6461      >>> chart_da
+0000f280: 7461 203d 2070 642e 4461 7461 4672 616d  ta = pd.DataFram
+0000f290: 6528 6e70 2e72 616e 646f 6d2e 7261 6e64  e(np.random.rand
+0000f2a0: 6e28 3230 302c 2033 292c 2063 6f6c 756d  n(200, 3), colum
+0000f2b0: 6e73 3d5b 2261 222c 2022 6222 2c20 2263  ns=["a", "b", "c
+0000f2c0: 225d 290a 2020 2020 2020 2020 3e3e 3e0a  "]).        >>>.
+0000f2d0: 2020 2020 2020 2020 3e3e 3e20 7374 2e76          >>> st.v
+0000f2e0: 6567 615f 6c69 7465 5f63 6861 7274 280a  ega_lite_chart(.
+0000f2f0: 2020 2020 2020 2020 2e2e 2e20 2020 2063          ...    c
+0000f300: 6861 7274 5f64 6174 612c 0a20 2020 2020  hart_data,.     
+0000f310: 2020 202e 2e2e 2020 2020 7b0a 2020 2020     ...    {.    
+0000f320: 2020 2020 2e2e 2e20 2020 2020 2020 2022      ...        "
+0000f330: 6d61 726b 223a 207b 2274 7970 6522 3a20  mark": {"type": 
+0000f340: 2263 6972 636c 6522 2c20 2274 6f6f 6c74  "circle", "toolt
+0000f350: 6970 223a 2054 7275 657d 2c0a 2020 2020  ip": True},.    
+0000f360: 2020 2020 2e2e 2e20 2020 2020 2020 2022      ...        "
+0000f370: 656e 636f 6469 6e67 223a 207b 0a20 2020  encoding": {.   
+0000f380: 2020 2020 202e 2e2e 2020 2020 2020 2020       ...        
+0000f390: 2020 2020 2278 223a 207b 2266 6965 6c64      "x": {"field
+0000f3a0: 223a 2022 6122 2c20 2274 7970 6522 3a20  ": "a", "type": 
+0000f3b0: 2271 7561 6e74 6974 6174 6976 6522 7d2c  "quantitative"},
+0000f3c0: 0a20 2020 2020 2020 202e 2e2e 2020 2020  .        ...    
+0000f3d0: 2020 2020 2020 2020 2279 223a 207b 2266          "y": {"f
+0000f3e0: 6965 6c64 223a 2022 6222 2c20 2274 7970  ield": "b", "typ
+0000f3f0: 6522 3a20 2271 7561 6e74 6974 6174 6976  e": "quantitativ
+0000f400: 6522 7d2c 0a20 2020 2020 2020 202e 2e2e  e"},.        ...
+0000f410: 2020 2020 2020 2020 2020 2020 2273 697a              "siz
+0000f420: 6522 3a20 7b22 6669 656c 6422 3a20 2263  e": {"field": "c
+0000f430: 222c 2022 7479 7065 223a 2022 7175 616e  ", "type": "quan
+0000f440: 7469 7461 7469 7665 227d 2c0a 2020 2020  titative"},.    
+0000f450: 2020 2020 2e2e 2e20 2020 2020 2020 2020      ...         
+0000f460: 2020 2022 636f 6c6f 7222 3a20 7b22 6669     "color": {"fi
+0000f470: 656c 6422 3a20 2263 222c 2022 7479 7065  eld": "c", "type
+0000f480: 223a 2022 7175 616e 7469 7461 7469 7665  ": "quantitative
+0000f490: 227d 2c0a 2020 2020 2020 2020 2e2e 2e20  "},.        ... 
+0000f4a0: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
+0000f4b0: 2020 2e2e 2e20 2020 207d 2c0a 2020 2020    ...    },.    
+0000f4c0: 2020 2020 2e2e 2e20 290a 0a20 2020 2020      ... )..     
+0000f4d0: 2020 202e 2e20 6f75 7470 7574 3a3a 0a20     .. output::. 
+0000f4e0: 2020 2020 2020 2020 2020 6874 7470 733a            https:
+0000f4f0: 2f2f 646f 632d 7665 6761 2d6c 6974 652d  //doc-vega-lite-
+0000f500: 6368 6172 742e 7374 7265 616d 6c69 742e  chart.streamlit.
+0000f510: 6170 702f 0a20 2020 2020 2020 2020 2020  app/.           
+0000f520: 6865 6967 6874 3a20 3435 3070 780a 0a20  height: 450px.. 
+0000f530: 2020 2020 2020 2045 7861 6d70 6c65 7320         Examples 
+0000f540: 6f66 2056 6567 612d 4c69 7465 2075 7361  of Vega-Lite usa
+0000f550: 6765 2077 6974 686f 7574 2053 7472 6561  ge without Strea
+0000f560: 6d6c 6974 2063 616e 2062 6520 666f 756e  mlit can be foun
+0000f570: 6420 6174 0a20 2020 2020 2020 2068 7474  d at.        htt
+0000f580: 7073 3a2f 2f76 6567 612e 6769 7468 7562  ps://vega.github
+0000f590: 2e69 6f2f 7665 6761 2d6c 6974 652f 6578  .io/vega-lite/ex
+0000f5a0: 616d 706c 6573 2f2e 204d 6f73 7420 6f66  amples/. Most of
+0000f5b0: 2074 686f 7365 2063 616e 2062 6520 6561   those can be ea
+0000f5c0: 7369 6c79 0a20 2020 2020 2020 2074 7261  sily.        tra
+0000f5d0: 6e73 6c61 7465 6420 746f 2074 6865 2073  nslated to the s
+0000f5e0: 796e 7461 7820 7368 6f77 6e20 6162 6f76  yntax shown abov
+0000f5f0: 652e 0a0a 2020 2020 2020 2020 2222 220a  e...        """.
+0000f600: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+0000f610: 656c 662e 5f76 6567 615f 6c69 7465 5f63  elf._vega_lite_c
+0000f620: 6861 7274 280a 2020 2020 2020 2020 2020  hart(.          
+0000f630: 2020 6461 7461 3d64 6174 612c 0a20 2020    data=data,.   
+0000f640: 2020 2020 2020 2020 2073 7065 633d 7370           spec=sp
+0000f650: 6563 2c0a 2020 2020 2020 2020 2020 2020  ec,.            
+0000f660: 7573 655f 636f 6e74 6169 6e65 725f 7769  use_container_wi
+0000f670: 6474 683d 7573 655f 636f 6e74 6169 6e65  dth=use_containe
+0000f680: 725f 7769 6474 682c 0a20 2020 2020 2020  r_width,.       
+0000f690: 2020 2020 2074 6865 6d65 3d74 6865 6d65       theme=theme
+0000f6a0: 2c0a 2020 2020 2020 2020 2020 2020 6b65  ,.            ke
+0000f6b0: 793d 6b65 792c 0a20 2020 2020 2020 2020  y=key,.         
+0000f6c0: 2020 206f 6e5f 7365 6c65 6374 3d6f 6e5f     on_select=on_
+0000f6d0: 7365 6c65 6374 2c0a 2020 2020 2020 2020  select,.        
+0000f6e0: 2020 2020 7365 6c65 6374 696f 6e5f 6d6f      selection_mo
+0000f6f0: 6465 3d73 656c 6563 7469 6f6e 5f6d 6f64  de=selection_mod
+0000f700: 652c 0a20 2020 2020 2020 2020 2020 202a  e,.            *
+0000f710: 2a6b 7761 7267 732c 0a20 2020 2020 2020  *kwargs,.       
+0000f720: 2029 0a0a 2020 2020 6465 6620 5f61 6c74   )..    def _alt
+0000f730: 6169 725f 6368 6172 7428 0a20 2020 2020  air_chart(.     
+0000f740: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
+0000f750: 2061 6c74 6169 725f 6368 6172 743a 2061   altair_chart: a
+0000f760: 6c74 2e43 6861 7274 2c0a 2020 2020 2020  lt.Chart,.      
+0000f770: 2020 7573 655f 636f 6e74 6169 6e65 725f    use_container_
+0000f780: 7769 6474 683a 2062 6f6f 6c20 3d20 4661  width: bool = Fa
+0000f790: 6c73 652c 0a20 2020 2020 2020 2074 6865  lse,.        the
+0000f7a0: 6d65 3a20 4c69 7465 7261 6c5b 2273 7472  me: Literal["str
+0000f7b0: 6561 6d6c 6974 225d 207c 204e 6f6e 6520  eamlit"] | None 
+0000f7c0: 3d20 2273 7472 6561 6d6c 6974 222c 0a20  = "streamlit",. 
+0000f7d0: 2020 2020 2020 206b 6579 3a20 4b65 7920         key: Key 
+0000f7e0: 7c20 4e6f 6e65 203d 204e 6f6e 652c 0a20  | None = None,. 
+0000f7f0: 2020 2020 2020 206f 6e5f 7365 6c65 6374         on_select
+0000f800: 3a20 4c69 7465 7261 6c5b 2272 6572 756e  : Literal["rerun
+0000f810: 222c 2022 6967 6e6f 7265 225d 207c 2057  ", "ignore"] | W
+0000f820: 6964 6765 7443 616c 6c62 6163 6b20 3d20  idgetCallback = 
+0000f830: 2269 676e 6f72 6522 2c0a 2020 2020 2020  "ignore",.      
+0000f840: 2020 7365 6c65 6374 696f 6e5f 6d6f 6465    selection_mode
+0000f850: 3a20 7374 7220 7c20 4974 6572 6162 6c65  : str | Iterable
+0000f860: 5b73 7472 5d20 7c20 4e6f 6e65 203d 204e  [str] | None = N
+0000f870: 6f6e 652c 0a20 2020 2020 2020 2061 6464  one,.        add
+0000f880: 5f72 6f77 735f 6d65 7461 6461 7461 3a20  _rows_metadata: 
+0000f890: 4164 6452 6f77 734d 6574 6164 6174 6120  AddRowsMetadata 
+0000f8a0: 7c20 4e6f 6e65 203d 204e 6f6e 652c 0a20  | None = None,. 
+0000f8b0: 2020 2029 202d 3e20 4465 6c74 6147 656e     ) -> DeltaGen
+0000f8c0: 6572 6174 6f72 207c 2056 6567 614c 6974  erator | VegaLit
+0000f8d0: 6553 7461 7465 3a0a 2020 2020 2020 2020  eState:.        
+0000f8e0: 2222 2249 6e74 6572 6e61 6c20 6d65 7468  """Internal meth
+0000f8f0: 6f64 2074 6f20 656e 7175 6575 6520 6120  od to enqueue a 
+0000f900: 7665 6761 2d6c 6974 6520 6368 6172 7420  vega-lite chart 
+0000f910: 656c 656d 656e 7420 6261 7365 6420 6f6e  element based on
+0000f920: 2061 6e20 416c 7461 6972 2063 6861 7274   an Altair chart
+0000f930: 2e0a 0a20 2020 2020 2020 2053 6565 2074  ...        See t
+0000f940: 6865 2060 616c 7461 6972 5f63 6861 7274  he `altair_chart
+0000f950: 6020 6d65 7468 6f64 2064 6f63 7374 7269  ` method docstri
+0000f960: 6e67 2066 6f72 206d 6f72 6520 696e 666f  ng for more info
+0000f970: 726d 6174 696f 6e2e 0a20 2020 2020 2020  rmation..       
+0000f980: 2022 2222 0a0a 2020 2020 2020 2020 6966   """..        if
+0000f990: 2074 7970 655f 7574 696c 2e69 735f 616c   type_util.is_al
+0000f9a0: 7461 6972 5f76 6572 7369 6f6e 5f6c 6573  tair_version_les
+0000f9b0: 735f 7468 616e 2822 352e 302e 3022 2920  s_than("5.0.0") 
+0000f9c0: 616e 6420 6f6e 5f73 656c 6563 7420 213d  and on_select !=
+0000f9d0: 2022 6967 6e6f 7265 223a 0a20 2020 2020   "ignore":.     
+0000f9e0: 2020 2020 2020 2072 6169 7365 2053 7472         raise Str
+0000f9f0: 6561 6d6c 6974 4150 4945 7863 6570 7469  eamlitAPIExcepti
+0000fa00: 6f6e 280a 2020 2020 2020 2020 2020 2020  on(.            
+0000fa10: 2020 2020 2253 7472 6561 6d6c 6974 2064      "Streamlit d
+0000fa20: 6f65 7320 6e6f 7420 7375 7070 6f72 7420  oes not support 
+0000fa30: 7365 6c65 6374 696f 6e73 2077 6974 6820  selections with 
+0000fa40: 416c 7461 6972 2034 2e78 2e20 506c 6561  Altair 4.x. Plea
+0000fa50: 7365 2075 7067 7261 6465 2074 6f20 5665  se upgrade to Ve
+0000fa60: 7273 696f 6e20 352e 2022 0a20 2020 2020  rsion 5. ".     
+0000fa70: 2020 2020 2020 2020 2020 2022 4966 2079             "If y
+0000fa80: 6f75 2077 6f75 6c64 206c 696b 6520 746f  ou would like to
+0000fa90: 2075 7365 2041 6c74 6169 7220 342e 7820   use Altair 4.x 
+0000faa0: 7769 7468 2073 656c 6563 7469 6f6e 732c  with selections,
+0000fab0: 2070 6c65 6173 6520 7570 766f 7465 2022   please upvote "
+0000fac0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000fad0: 2022 7468 6973 205b 4769 7468 7562 2069   "this [Github i
+0000fae0: 7373 7565 5d28 6874 7470 733a 2f2f 6769  ssue](https://gi
+0000faf0: 7468 7562 2e63 6f6d 2f73 7472 6561 6d6c  thub.com/streaml
+0000fb00: 6974 2f73 7472 6561 6d6c 6974 2f69 7373  it/streamlit/iss
+0000fb10: 7565 732f 3835 3136 292e 220a 2020 2020  ues/8516).".    
+0000fb20: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+0000fb30: 2020 2076 6567 615f 6c69 7465 5f73 7065     vega_lite_spe
+0000fb40: 6320 3d20 5f63 6f6e 7665 7274 5f61 6c74  c = _convert_alt
+0000fb50: 6169 725f 746f 5f76 6567 615f 6c69 7465  air_to_vega_lite
+0000fb60: 5f73 7065 6328 616c 7461 6972 5f63 6861  _spec(altair_cha
+0000fb70: 7274 290a 2020 2020 2020 2020 7265 7475  rt).        retu
+0000fb80: 726e 2073 656c 662e 5f76 6567 615f 6c69  rn self._vega_li
+0000fb90: 7465 5f63 6861 7274 280a 2020 2020 2020  te_chart(.      
+0000fba0: 2020 2020 2020 6461 7461 3d4e 6f6e 652c        data=None,
+0000fbb0: 2020 2320 5468 6520 6461 7461 2069 7320    # The data is 
+0000fbc0: 616c 7265 6164 7920 7061 7274 206f 6620  already part of 
+0000fbd0: 7468 6520 7370 6563 0a20 2020 2020 2020  the spec.       
+0000fbe0: 2020 2020 2073 7065 633d 7665 6761 5f6c       spec=vega_l
+0000fbf0: 6974 655f 7370 6563 2c0a 2020 2020 2020  ite_spec,.      
+0000fc00: 2020 2020 2020 7573 655f 636f 6e74 6169        use_contai
+0000fc10: 6e65 725f 7769 6474 683d 7573 655f 636f  ner_width=use_co
+0000fc20: 6e74 6169 6e65 725f 7769 6474 682c 0a20  ntainer_width,. 
+0000fc30: 2020 2020 2020 2020 2020 2074 6865 6d65             theme
+0000fc40: 3d74 6865 6d65 2c0a 2020 2020 2020 2020  =theme,.        
+0000fc50: 2020 2020 6b65 793d 6b65 792c 0a20 2020      key=key,.   
+0000fc60: 2020 2020 2020 2020 206f 6e5f 7365 6c65           on_sele
+0000fc70: 6374 3d6f 6e5f 7365 6c65 6374 2c0a 2020  ct=on_select,.  
+0000fc80: 2020 2020 2020 2020 2020 7365 6c65 6374            select
+0000fc90: 696f 6e5f 6d6f 6465 3d73 656c 6563 7469  ion_mode=selecti
+0000fca0: 6f6e 5f6d 6f64 652c 0a20 2020 2020 2020  on_mode,.       
+0000fcb0: 2020 2020 2061 6464 5f72 6f77 735f 6d65       add_rows_me
+0000fcc0: 7461 6461 7461 3d61 6464 5f72 6f77 735f  tadata=add_rows_
+0000fcd0: 6d65 7461 6461 7461 2c0a 2020 2020 2020  metadata,.      
+0000fce0: 2020 290a 0a20 2020 2064 6566 205f 7665    )..    def _ve
+0000fcf0: 6761 5f6c 6974 655f 6368 6172 7428 0a20  ga_lite_chart(. 
+0000fd00: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+0000fd10: 2020 2020 2064 6174 613a 2044 6174 6120       data: Data 
+0000fd20: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+0000fd30: 7370 6563 3a20 5665 6761 4c69 7465 5370  spec: VegaLiteSp
+0000fd40: 6563 207c 204e 6f6e 6520 3d20 4e6f 6e65  ec | None = None
+0000fd50: 2c0a 2020 2020 2020 2020 7573 655f 636f  ,.        use_co
+0000fd60: 6e74 6169 6e65 725f 7769 6474 683a 2062  ntainer_width: b
+0000fd70: 6f6f 6c20 3d20 4661 6c73 652c 0a20 2020  ool = False,.   
+0000fd80: 2020 2020 2074 6865 6d65 3a20 4c69 7465       theme: Lite
+0000fd90: 7261 6c5b 2273 7472 6561 6d6c 6974 225d  ral["streamlit"]
+0000fda0: 207c 204e 6f6e 6520 3d20 2273 7472 6561   | None = "strea
+0000fdb0: 6d6c 6974 222c 0a20 2020 2020 2020 206b  mlit",.        k
+0000fdc0: 6579 3a20 4b65 7920 7c20 4e6f 6e65 203d  ey: Key | None =
+0000fdd0: 204e 6f6e 652c 0a20 2020 2020 2020 206f   None,.        o
+0000fde0: 6e5f 7365 6c65 6374 3a20 4c69 7465 7261  n_select: Litera
+0000fdf0: 6c5b 2272 6572 756e 222c 2022 6967 6e6f  l["rerun", "igno
+0000fe00: 7265 225d 207c 2057 6964 6765 7443 616c  re"] | WidgetCal
+0000fe10: 6c62 6163 6b20 3d20 2269 676e 6f72 6522  lback = "ignore"
+0000fe20: 2c0a 2020 2020 2020 2020 7365 6c65 6374  ,.        select
+0000fe30: 696f 6e5f 6d6f 6465 3a20 7374 7220 7c20  ion_mode: str | 
+0000fe40: 4974 6572 6162 6c65 5b73 7472 5d20 7c20  Iterable[str] | 
+0000fe50: 4e6f 6e65 203d 204e 6f6e 652c 0a20 2020  None = None,.   
+0000fe60: 2020 2020 2061 6464 5f72 6f77 735f 6d65       add_rows_me
+0000fe70: 7461 6461 7461 3a20 4164 6452 6f77 734d  tadata: AddRowsM
+0000fe80: 6574 6164 6174 6120 7c20 4e6f 6e65 203d  etadata | None =
+0000fe90: 204e 6f6e 652c 0a20 2020 2020 2020 202a   None,.        *
+0000fea0: 2a6b 7761 7267 733a 2041 6e79 2c0a 2020  *kwargs: Any,.  
+0000feb0: 2020 2920 2d3e 2044 656c 7461 4765 6e65    ) -> DeltaGene
+0000fec0: 7261 746f 7220 7c20 5665 6761 4c69 7465  rator | VegaLite
+0000fed0: 5374 6174 653a 0a20 2020 2020 2020 2022  State:.        "
+0000fee0: 2222 496e 7465 726e 616c 206d 6574 686f  ""Internal metho
+0000fef0: 6420 746f 2065 6e71 7565 7565 2061 2076  d to enqueue a v
+0000ff00: 6567 612d 6c69 7465 2063 6861 7274 2065  ega-lite chart e
+0000ff10: 6c65 6d65 6e74 2062 6173 6564 206f 6e20  lement based on 
+0000ff20: 6120 7665 6761 2d6c 6974 6520 7370 6563  a vega-lite spec
+0000ff30: 2e0a 0a20 2020 2020 2020 2053 6565 2074  ...        See t
+0000ff40: 6865 2060 7665 6761 5f6c 6974 655f 6368  he `vega_lite_ch
+0000ff50: 6172 7460 206d 6574 686f 6420 646f 6373  art` method docs
+0000ff60: 7472 696e 6720 666f 7220 6d6f 7265 2069  tring for more i
+0000ff70: 6e66 6f72 6d61 7469 6f6e 2e0a 2020 2020  nformation..    
+0000ff80: 2020 2020 2222 220a 0a20 2020 2020 2020      """..       
+0000ff90: 2069 6620 7468 656d 6520 6e6f 7420 696e   if theme not in
+0000ffa0: 205b 2273 7472 6561 6d6c 6974 222c 204e   ["streamlit", N
+0000ffb0: 6f6e 655d 3a0a 2020 2020 2020 2020 2020  one]:.          
+0000ffc0: 2020 7261 6973 6520 5374 7265 616d 6c69    raise Streamli
+0000ffd0: 7441 5049 4578 6365 7074 696f 6e28 0a20  tAPIException(. 
+0000ffe0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0000fff0: 2759 6f75 2073 6574 2074 6865 6d65 3d22  'You set theme="
+00010000: 7b74 6865 6d65 7d22 2077 6869 6c65 2053  {theme}" while S
+00010010: 7472 6561 6d6c 6974 2063 6861 7274 7320  treamlit charts 
+00010020: 6f6e 6c79 2073 7570 706f 7274 2074 6865  only support the
+00010030: 6d65 3de2 809d 7374 7265 616d 6c69 74e2  me=...streamlit.
+00010040: 809d 206f 7220 7468 656d 653d 4e6f 6e65  .. or theme=None
+00010050: 2074 6f20 6661 6c6c 6261 636b 2074 6f20   to fallback to 
+00010060: 7468 6520 6465 6661 756c 7420 6c69 6272  the default libr
+00010070: 6172 7920 7468 656d 652e 270a 2020 2020  ary theme.'.    
+00010080: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+00010090: 2020 2069 6620 6f6e 5f73 656c 6563 7420     if on_select 
+000100a0: 6e6f 7420 696e 205b 2269 676e 6f72 6522  not in ["ignore"
+000100b0: 2c20 2272 6572 756e 225d 2061 6e64 206e  , "rerun"] and n
+000100c0: 6f74 2063 616c 6c61 626c 6528 6f6e 5f73  ot callable(on_s
+000100d0: 656c 6563 7429 3a0a 2020 2020 2020 2020  elect):.        
+000100e0: 2020 2020 7261 6973 6520 5374 7265 616d      raise Stream
+000100f0: 6c69 7441 5049 4578 6365 7074 696f 6e28  litAPIException(
+00010100: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010110: 2066 2259 6f75 2068 6176 6520 7061 7373   f"You have pass
+00010120: 6564 207b 6f6e 5f73 656c 6563 747d 2074  ed {on_select} t
+00010130: 6f20 606f 6e5f 7365 6c65 6374 602e 2042  o `on_select`. B
+00010140: 7574 206f 6e6c 7920 2769 676e 6f72 6527  ut only 'ignore'
+00010150: 2c20 2772 6572 756e 272c 206f 7220 6120  , 'rerun', or a 
+00010160: 6361 6c6c 6162 6c65 2069 7320 7375 7070  callable is supp
+00010170: 6f72 7465 642e 220a 2020 2020 2020 2020  orted.".        
+00010180: 2020 2020 290a 0a20 2020 2020 2020 206b      )..        k
+00010190: 6579 203d 2074 6f5f 6b65 7928 6b65 7929  ey = to_key(key)
+000101a0: 0a20 2020 2020 2020 2069 735f 7365 6c65  .        is_sele
+000101b0: 6374 696f 6e5f 6163 7469 7661 7465 6420  ction_activated 
+000101c0: 3d20 6f6e 5f73 656c 6563 7420 213d 2022  = on_select != "
+000101d0: 6967 6e6f 7265 220a 0a20 2020 2020 2020  ignore"..       
+000101e0: 2069 6620 6973 5f73 656c 6563 7469 6f6e   if is_selection
+000101f0: 5f61 6374 6976 6174 6564 3a0a 2020 2020  _activated:.    
+00010200: 2020 2020 2020 2020 2320 5275 6e20 736f          # Run so
+00010210: 6d65 2063 6865 636b 7320 7468 6174 2061  me checks that a
+00010220: 7265 206f 6e6c 7920 7265 6c65 7661 6e74  re only relevant
+00010230: 2077 6865 6e20 7365 6c65 6374 696f 6e73   when selections
+00010240: 2061 7265 2061 6374 6976 6174 6564 0a0a   are activated..
+00010250: 2020 2020 2020 2020 2020 2020 2320 496d              # Im
+00010260: 706f 7274 2068 6572 6520 746f 2061 766f  port here to avo
+00010270: 6964 2063 6972 6375 6c61 7220 696d 706f  id circular impo
+00010280: 7274 730a 2020 2020 2020 2020 2020 2020  rts.            
+00010290: 6672 6f6d 2073 7472 6561 6d6c 6974 2e65  from streamlit.e
+000102a0: 6c65 6d65 6e74 732e 7574 696c 7320 696d  lements.utils im
+000102b0: 706f 7274 2028 0a20 2020 2020 2020 2020  port (.         
+000102c0: 2020 2020 2020 2063 6865 636b 5f63 6163         check_cac
+000102d0: 6865 5f72 6570 6c61 795f 7275 6c65 732c  he_replay_rules,
+000102e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000102f0: 2063 6865 636b 5f63 616c 6c62 6163 6b5f   check_callback_
+00010300: 7275 6c65 732c 0a20 2020 2020 2020 2020  rules,.         
+00010310: 2020 2020 2020 2063 6865 636b 5f73 6573         check_ses
+00010320: 7369 6f6e 5f73 7461 7465 5f72 756c 6573  sion_state_rules
+00010330: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
+00010340: 0a20 2020 2020 2020 2020 2020 2063 6865  .            che
+00010350: 636b 5f63 6163 6865 5f72 6570 6c61 795f  ck_cache_replay_
+00010360: 7275 6c65 7328 290a 2020 2020 2020 2020  rules().        
+00010370: 2020 2020 6966 2063 616c 6c61 626c 6528      if callable(
+00010380: 6f6e 5f73 656c 6563 7429 3a0a 2020 2020  on_select):.    
+00010390: 2020 2020 2020 2020 2020 2020 6368 6563              chec
+000103a0: 6b5f 6361 6c6c 6261 636b 5f72 756c 6573  k_callback_rules
+000103b0: 2873 656c 662e 6467 2c20 6f6e 5f73 656c  (self.dg, on_sel
+000103c0: 6563 7429 0a20 2020 2020 2020 2020 2020  ect).           
+000103d0: 2063 6865 636b 5f73 6573 7369 6f6e 5f73   check_session_s
+000103e0: 7461 7465 5f72 756c 6573 2864 6566 6175  tate_rules(defau
+000103f0: 6c74 5f76 616c 7565 3d4e 6f6e 652c 206b  lt_value=None, k
+00010400: 6579 3d6b 6579 2c20 7772 6974 6573 5f61  ey=key, writes_a
+00010410: 6c6c 6f77 6564 3d46 616c 7365 290a 0a20  llowed=False).. 
+00010420: 2020 2020 2020 2023 2053 7570 706f 7274         # Support
+00010430: 2070 6173 7369 6e67 2064 6174 6120 696e   passing data in
+00010440: 7369 6465 2073 7065 635b 2764 6174 6173  side spec['datas
+00010450: 6574 7327 5d20 616e 6420 7370 6563 5b27  ets'] and spec['
+00010460: 6461 7461 275d 2e0a 2020 2020 2020 2020  data']..        
+00010470: 2320 2854 6865 2064 6174 6120 6765 7473  # (The data gets
+00010480: 2070 756c 6c65 6420 6f75 7420 6f66 2074   pulled out of t
+00010490: 6865 2073 7065 6320 6469 6374 206c 6174  he spec dict lat
+000104a0: 6572 206f 6e2e 290a 2020 2020 2020 2020  er on.).        
+000104b0: 6966 2069 7369 6e73 7461 6e63 6528 6461  if isinstance(da
+000104c0: 7461 2c20 6469 6374 2920 616e 6420 7370  ta, dict) and sp
+000104d0: 6563 2069 7320 4e6f 6e65 3a0a 2020 2020  ec is None:.    
+000104e0: 2020 2020 2020 2020 7370 6563 203d 2064          spec = d
+000104f0: 6174 610a 2020 2020 2020 2020 2020 2020  ata.            
+00010500: 6461 7461 203d 204e 6f6e 650a 0a20 2020  data = None..   
+00010510: 2020 2020 2069 6620 7370 6563 2069 7320       if spec is 
+00010520: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00010530: 2020 7370 6563 203d 207b 7d0a 0a20 2020    spec = {}..   
+00010540: 2020 2020 2076 6567 615f 6c69 7465 5f70       vega_lite_p
+00010550: 726f 746f 203d 2041 7272 6f77 5665 6761  roto = ArrowVega
+00010560: 4c69 7465 4368 6172 7450 726f 746f 2829  LiteChartProto()
+00010570: 0a0a 2020 2020 2020 2020 7370 6563 203d  ..        spec =
+00010580: 205f 7072 6570 6172 655f 7665 6761 5f6c   _prepare_vega_l
+00010590: 6974 655f 7370 6563 2873 7065 632c 2075  ite_spec(spec, u
+000105a0: 7365 5f63 6f6e 7461 696e 6572 5f77 6964  se_container_wid
+000105b0: 7468 2c20 2a2a 6b77 6172 6773 290a 2020  th, **kwargs).  
+000105c0: 2020 2020 2020 5f6d 6172 7368 616c 6c5f        _marshall_
+000105d0: 6368 6172 745f 6461 7461 2876 6567 615f  chart_data(vega_
+000105e0: 6c69 7465 5f70 726f 746f 2c20 7370 6563  lite_proto, spec
+000105f0: 2c20 6461 7461 290a 0a20 2020 2020 2020  , data)..       
+00010600: 2023 2050 7265 7665 6e74 2074 6865 2073   # Prevent the s
+00010610: 7065 6320 6672 6f6d 2063 6861 6e67 696e  pec from changin
+00010620: 6720 6163 726f 7373 2072 6572 756e 733a  g across reruns:
+00010630: 0a20 2020 2020 2020 2076 6567 615f 6c69  .        vega_li
+00010640: 7465 5f70 726f 746f 2e73 7065 6320 3d20  te_proto.spec = 
+00010650: 5f73 7461 6269 6c69 7a65 5f76 6567 615f  _stabilize_vega_
+00010660: 6a73 6f6e 5f73 7065 6328 6a73 6f6e 2e64  json_spec(json.d
+00010670: 756d 7073 2873 7065 6329 290a 2020 2020  umps(spec)).    
+00010680: 2020 2020 7665 6761 5f6c 6974 655f 7072      vega_lite_pr
+00010690: 6f74 6f2e 7573 655f 636f 6e74 6169 6e65  oto.use_containe
+000106a0: 725f 7769 6474 6820 3d20 7573 655f 636f  r_width = use_co
+000106b0: 6e74 6169 6e65 725f 7769 6474 680a 2020  ntainer_width.  
+000106c0: 2020 2020 2020 7665 6761 5f6c 6974 655f        vega_lite_
+000106d0: 7072 6f74 6f2e 7468 656d 6520 3d20 7468  proto.theme = th
+000106e0: 656d 6520 6f72 2022 220a 0a20 2020 2020  eme or ""..     
+000106f0: 2020 2069 6620 6973 5f73 656c 6563 7469     if is_selecti
+00010700: 6f6e 5f61 6374 6976 6174 6564 3a0a 2020  on_activated:.  
+00010710: 2020 2020 2020 2020 2020 2320 496d 706f            # Impo
+00010720: 7274 2068 6572 6520 746f 2061 766f 6964  rt here to avoid
+00010730: 2063 6972 6375 6c61 7220 696d 706f 7274   circular import
+00010740: 730a 2020 2020 2020 2020 2020 2020 6672  s.            fr
+00010750: 6f6d 2073 7472 6561 6d6c 6974 2e65 6c65  om streamlit.ele
+00010760: 6d65 6e74 732e 666f 726d 2069 6d70 6f72  ments.form impor
+00010770: 7420 6375 7272 656e 745f 666f 726d 5f69  t current_form_i
+00010780: 640a 0a20 2020 2020 2020 2020 2020 2023  d..            #
+00010790: 204c 6f61 6420 7468 6520 7374 6162 696c   Load the stabil
+000107a0: 697a 6564 2073 7065 6320 6167 6169 6e20  ized spec again 
+000107b0: 6173 2061 2064 6963 743a 0a20 2020 2020  as a dict:.     
+000107c0: 2020 2020 2020 2066 696e 616c 5f73 7065         final_spe
+000107d0: 6320 3d20 6a73 6f6e 2e6c 6f61 6473 2876  c = json.loads(v
+000107e0: 6567 615f 6c69 7465 5f70 726f 746f 2e73  ega_lite_proto.s
+000107f0: 7065 6329 0a20 2020 2020 2020 2020 2020  pec).           
+00010800: 2023 2054 656d 706f 7261 7279 206c 696d   # Temporary lim
+00010810: 6974 6174 696f 6e20 746f 2064 6973 616c  itation to disal
+00010820: 6c6f 7720 6d75 6c74 692d 7669 6577 2063  low multi-view c
+00010830: 6861 7274 7320 2863 6f6d 706f 7369 7469  harts (compositi
+00010840: 6f6e 7329 2077 6974 6820 7365 6c65 6374  ons) with select
+00010850: 696f 6e73 2e0a 2020 2020 2020 2020 2020  ions..          
+00010860: 2020 5f64 6973 616c 6c6f 775f 6d75 6c74    _disallow_mult
+00010870: 695f 7669 6577 5f63 6861 7274 7328 6669  i_view_charts(fi
+00010880: 6e61 6c5f 7370 6563 290a 0a20 2020 2020  nal_spec)..     
+00010890: 2020 2020 2020 2023 2050 6172 7365 2061         # Parse a
+000108a0: 6e64 2063 6865 636b 2074 6865 2073 7065  nd check the spe
+000108b0: 6369 6669 6564 2073 656c 6563 7469 6f6e  cified selection
+000108c0: 206d 6f64 6573 0a20 2020 2020 2020 2020   modes.         
+000108d0: 2020 2070 6172 7365 645f 7365 6c65 6374     parsed_select
+000108e0: 696f 6e5f 6d6f 6465 7320 3d20 5f70 6172  ion_modes = _par
+000108f0: 7365 5f73 656c 6563 7469 6f6e 5f6d 6f64  se_selection_mod
+00010900: 6528 6669 6e61 6c5f 7370 6563 2c20 7365  e(final_spec, se
+00010910: 6c65 6374 696f 6e5f 6d6f 6465 290a 2020  lection_mode).  
+00010920: 2020 2020 2020 2020 2020 7665 6761 5f6c            vega_l
+00010930: 6974 655f 7072 6f74 6f2e 7365 6c65 6374  ite_proto.select
+00010940: 696f 6e5f 6d6f 6465 2e65 7874 656e 6428  ion_mode.extend(
+00010950: 7061 7273 6564 5f73 656c 6563 7469 6f6e  parsed_selection
+00010960: 5f6d 6f64 6573 290a 0a20 2020 2020 2020  _modes)..       
+00010970: 2020 2020 2076 6567 615f 6c69 7465 5f70       vega_lite_p
+00010980: 726f 746f 2e66 6f72 6d5f 6964 203d 2063  roto.form_id = c
+00010990: 7572 7265 6e74 5f66 6f72 6d5f 6964 2873  urrent_form_id(s
+000109a0: 656c 662e 6467 290a 0a20 2020 2020 2020  elf.dg)..       
+000109b0: 2020 2020 2063 7478 203d 2067 6574 5f73       ctx = get_s
+000109c0: 6372 6970 745f 7275 6e5f 6374 7828 290a  cript_run_ctx().
+000109d0: 2020 2020 2020 2020 2020 2020 7665 6761              vega
+000109e0: 5f6c 6974 655f 7072 6f74 6f2e 6964 203d  _lite_proto.id =
+000109f0: 2063 6f6d 7075 7465 5f77 6964 6765 745f   compute_widget_
+00010a00: 6964 280a 2020 2020 2020 2020 2020 2020  id(.            
+00010a10: 2020 2020 2261 7272 6f77 5f76 6567 615f      "arrow_vega_
+00010a20: 6c69 7465 5f63 6861 7274 222c 0a20 2020  lite_chart",.   
+00010a30: 2020 2020 2020 2020 2020 2020 2075 7365               use
+00010a40: 725f 6b65 793d 6b65 792c 0a20 2020 2020  r_key=key,.     
+00010a50: 2020 2020 2020 2020 2020 206b 6579 3d6b             key=k
+00010a60: 6579 2c0a 2020 2020 2020 2020 2020 2020  ey,.            
+00010a70: 2020 2020 7665 6761 5f6c 6974 655f 7370      vega_lite_sp
+00010a80: 6563 3d76 6567 615f 6c69 7465 5f70 726f  ec=vega_lite_pro
+00010a90: 746f 2e73 7065 632c 0a20 2020 2020 2020  to.spec,.       
+00010aa0: 2020 2020 2020 2020 2023 2054 6865 2064           # The d
+00010ab0: 6174 6120 6973 2065 6974 6865 7220 696e  ata is either in
+00010ac0: 2076 6567 615f 6c69 7465 5f70 726f 746f   vega_lite_proto
+00010ad0: 2e64 6174 612e 6461 7461 0a20 2020 2020  .data.data.     
+00010ae0: 2020 2020 2020 2020 2020 2023 206f 7220             # or 
+00010af0: 696e 2061 206e 616d 6564 2064 6174 6173  in a named datas
+00010b00: 6574 2069 6e20 7665 6761 5f6c 6974 655f  et in vega_lite_
+00010b10: 7072 6f74 6f2e 6461 7461 7365 7473 0a20  proto.datasets. 
+00010b20: 2020 2020 2020 2020 2020 2020 2020 2076                 v
+00010b30: 6567 615f 6c69 7465 5f64 6174 613d 7665  ega_lite_data=ve
+00010b40: 6761 5f6c 6974 655f 7072 6f74 6f2e 6461  ga_lite_proto.da
+00010b50: 7461 2e64 6174 612c 0a20 2020 2020 2020  ta.data,.       
+00010b60: 2020 2020 2020 2020 2023 2049 7473 2065           # Its e
+00010b70: 6e6f 7567 6820 746f 206a 7573 7420 7573  nough to just us
+00010b80: 6520 7468 6520 6e61 6d65 7320 6865 7265  e the names here
+00010b90: 2073 696e 6365 2074 6865 7920 6172 6520   since they are 
+00010ba0: 6578 7065 6374 6564 0a20 2020 2020 2020  expected.       
+00010bb0: 2020 2020 2020 2020 2023 2074 6f20 636f           # to co
+00010bc0: 6e74 6169 6e20 6861 7368 6573 2062 6173  ntain hashes bas
+00010bd0: 6564 206f 6e20 7468 6520 6461 7461 7365  ed on the datase
+00010be0: 7420 6461 7461 2e0a 2020 2020 2020 2020  t data..        
+00010bf0: 2020 2020 2020 2020 6e61 6d65 645f 6461          named_da
+00010c00: 7461 7365 7473 3d5b 6461 7461 7365 742e  tasets=[dataset.
+00010c10: 6e61 6d65 2066 6f72 2064 6174 6173 6574  name for dataset
+00010c20: 2069 6e20 7665 6761 5f6c 6974 655f 7072   in vega_lite_pr
+00010c30: 6f74 6f2e 6461 7461 7365 7473 5d2c 0a20  oto.datasets],. 
+00010c40: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00010c50: 6865 6d65 3d74 6865 6d65 2c0a 2020 2020  heme=theme,.    
+00010c60: 2020 2020 2020 2020 2020 2020 7573 655f              use_
+00010c70: 636f 6e74 6169 6e65 725f 7769 6474 683d  container_width=
+00010c80: 7573 655f 636f 6e74 6169 6e65 725f 7769  use_container_wi
+00010c90: 6474 682c 0a20 2020 2020 2020 2020 2020  dth,.           
+00010ca0: 2020 2020 2073 656c 6563 7469 6f6e 5f6d       selection_m
+00010cb0: 6f64 653d 7061 7273 6564 5f73 656c 6563  ode=parsed_selec
+00010cc0: 7469 6f6e 5f6d 6f64 6573 2c0a 2020 2020  tion_modes,.    
+00010cd0: 2020 2020 2020 2020 2020 2020 666f 726d              form
+00010ce0: 5f69 643d 7665 6761 5f6c 6974 655f 7072  _id=vega_lite_pr
+00010cf0: 6f74 6f2e 666f 726d 5f69 642c 0a20 2020  oto.form_id,.   
+00010d00: 2020 2020 2020 2020 2020 2020 2070 6167               pag
+00010d10: 653d 6374 782e 7061 6765 5f73 6372 6970  e=ctx.page_scrip
+00010d20: 745f 6861 7368 2069 6620 6374 7820 656c  t_hash if ctx el
+00010d30: 7365 204e 6f6e 652c 0a20 2020 2020 2020  se None,.       
+00010d40: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
+00010d50: 2020 2020 7365 7264 6520 3d20 5665 6761      serde = Vega
+00010d60: 4c69 7465 5374 6174 6553 6572 6465 2870  LiteStateSerde(p
+00010d70: 6172 7365 645f 7365 6c65 6374 696f 6e5f  arsed_selection_
+00010d80: 6d6f 6465 7329 0a0a 2020 2020 2020 2020  modes)..        
+00010d90: 2020 2020 7769 6467 6574 5f73 7461 7465      widget_state
+00010da0: 203d 2072 6567 6973 7465 725f 7769 6467   = register_widg
+00010db0: 6574 280a 2020 2020 2020 2020 2020 2020  et(.            
+00010dc0: 2020 2020 2276 6567 615f 6c69 7465 5f63      "vega_lite_c
+00010dd0: 6861 7274 222c 0a20 2020 2020 2020 2020  hart",.         
+00010de0: 2020 2020 2020 2076 6567 615f 6c69 7465         vega_lite
+00010df0: 5f70 726f 746f 2c0a 2020 2020 2020 2020  _proto,.        
+00010e00: 2020 2020 2020 2020 7573 6572 5f6b 6579          user_key
+00010e10: 3d6b 6579 2c0a 2020 2020 2020 2020 2020  =key,.          
+00010e20: 2020 2020 2020 6f6e 5f63 6861 6e67 655f        on_change_
+00010e30: 6861 6e64 6c65 723d 6f6e 5f73 656c 6563  handler=on_selec
+00010e40: 7420 6966 2063 616c 6c61 626c 6528 6f6e  t if callable(on
+00010e50: 5f73 656c 6563 7429 2065 6c73 6520 4e6f  _select) else No
+00010e60: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
+00010e70: 2020 2020 6465 7365 7269 616c 697a 6572      deserializer
+00010e80: 3d73 6572 6465 2e64 6573 6572 6961 6c69  =serde.deseriali
+00010e90: 7a65 2c0a 2020 2020 2020 2020 2020 2020  ze,.            
+00010ea0: 2020 2020 7365 7269 616c 697a 6572 3d73      serializer=s
+00010eb0: 6572 6465 2e73 6572 6961 6c69 7a65 2c0a  erde.serialize,.
+00010ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010ed0: 6374 783d 6374 782c 0a20 2020 2020 2020  ctx=ctx,.       
+00010ee0: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
+00010ef0: 2020 2020 7365 6c66 2e64 672e 5f65 6e71      self.dg._enq
+00010f00: 7565 7565 280a 2020 2020 2020 2020 2020  ueue(.          
+00010f10: 2020 2020 2020 2261 7272 6f77 5f76 6567        "arrow_veg
+00010f20: 615f 6c69 7465 5f63 6861 7274 222c 0a20  a_lite_chart",. 
+00010f30: 2020 2020 2020 2020 2020 2020 2020 2076                 v
+00010f40: 6567 615f 6c69 7465 5f70 726f 746f 2c0a  ega_lite_proto,.
+00010f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010f60: 6164 645f 726f 7773 5f6d 6574 6164 6174  add_rows_metadat
+00010f70: 613d 6164 645f 726f 7773 5f6d 6574 6164  a=add_rows_metad
+00010f80: 6174 612c 0a20 2020 2020 2020 2020 2020  ata,.           
+00010f90: 2029 0a20 2020 2020 2020 2020 2020 2072   ).            r
+00010fa0: 6574 7572 6e20 6361 7374 2856 6567 614c  eturn cast(VegaL
+00010fb0: 6974 6553 7461 7465 2c20 7769 6467 6574  iteState, widget
+00010fc0: 5f73 7461 7465 2e76 616c 7565 290a 2020  _state.value).  
+00010fd0: 2020 2020 2020 2320 4966 2069 7473 206e        # If its n
+00010fe0: 6f74 2075 7365 6420 7769 7468 2073 656c  ot used with sel
+00010ff0: 6563 7469 6f6e 7320 6163 7469 7661 7465  ections activate
+00011000: 642c 206a 7573 7420 7265 7475 726e 0a20  d, just return. 
+00011010: 2020 2020 2020 2023 2074 6865 2064 656c         # the del
+00011020: 7461 2067 656e 6572 6174 6f72 2072 656c  ta generator rel
+00011030: 6174 6564 2074 6f20 7468 6973 2065 6c65  ated to this ele
+00011040: 6d65 6e74 2e0a 2020 2020 2020 2020 7265  ment..        re
+00011050: 7475 726e 2073 656c 662e 6467 2e5f 656e  turn self.dg._en
+00011060: 7175 6575 6528 0a20 2020 2020 2020 2020  queue(.         
+00011070: 2020 2022 6172 726f 775f 7665 6761 5f6c     "arrow_vega_l
+00011080: 6974 655f 6368 6172 7422 2c0a 2020 2020  ite_chart",.    
+00011090: 2020 2020 2020 2020 7665 6761 5f6c 6974          vega_lit
+000110a0: 655f 7072 6f74 6f2c 0a20 2020 2020 2020  e_proto,.       
+000110b0: 2020 2020 2061 6464 5f72 6f77 735f 6d65       add_rows_me
+000110c0: 7461 6461 7461 3d61 6464 5f72 6f77 735f  tadata=add_rows_
+000110d0: 6d65 7461 6461 7461 2c0a 2020 2020 2020  metadata,.      
+000110e0: 2020 290a 0a20 2020 2040 7072 6f70 6572    )..    @proper
+000110f0: 7479 0a20 2020 2064 6566 2064 6728 7365  ty.    def dg(se
+00011100: 6c66 2920 2d3e 2044 656c 7461 4765 6e65  lf) -> DeltaGene
+00011110: 7261 746f 723a 0a20 2020 2020 2020 2022  rator:.        "
+00011120: 2222 4765 7420 6f75 7220 4465 6c74 6147  ""Get our DeltaG
+00011130: 656e 6572 6174 6f72 2e22 2222 0a20 2020  enerator.""".   
+00011140: 2020 2020 2072 6574 7572 6e20 6361 7374       return cast
+00011150: 2822 4465 6c74 6147 656e 6572 6174 6f72  ("DeltaGenerator
+00011160: 222c 2073 656c 6629 0a                   ", self).
```

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/widgets/__init__.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/elements/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/widgets/button.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/elements/widgets/button.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/widgets/camera_input.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/elements/widgets/camera_input.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/widgets/chat.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/elements/widgets/chat.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/widgets/checkbox.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/elements/widgets/checkbox.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/widgets/color_picker.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/elements/widgets/color_picker.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/widgets/data_editor.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/elements/widgets/data_editor.py`

 * *Files 2% similar despite different names*

```diff
@@ -616,28 +616,37 @@
                   complex, list, tuple, bytes, bytearray, memoryview, dict, set, frozenset,
                   fractions.Fraction, pandas.Interval, and pandas.Period.
                 - To prevent overflow in JavaScript, columns containing datetime.timedelta
                   and pandas.Timedelta values will default to uneditable but this can be
                   changed through column configuration.
 
         width : int or None
-            Desired width of the data editor expressed in pixels. If None, the width will
-            be automatically determined.
+            Desired width of the data editor expressed in pixels. If ``width``
+            is ``None`` (default), Streamlit sets the data editor width to fit
+            its contents up to the width of the parent container. If ``width``
+            is greater than the width of the parent container, Streamlit sets
+            the data editor width to match the width of the parent container.
 
         height : int or None
-            Desired height of the data editor expressed in pixels. If None, the height will
-            be automatically determined.
+            Desired height of the data editor expressed in pixels. If ``height``
+            is ``None`` (default), Streamlit sets the height to show at most
+            ten rows. Vertical scrolling within the data editor element is
+            enabled when the height does not accomodate all rows.
 
         use_container_width : bool
-            If True, set the data editor width to the width of the parent container.
-            This takes precedence over the width argument. Defaults to False.
+            Whether to override ``width`` with the width of the parent
+            container. If ``use_container_width`` is ``False`` (default),
+            Streamlit sets the data editor's width according to ``width``. If
+            ``use_container_width`` is ``True``, Streamlit sets the width of
+            the data editor to match the width of the parent container.
 
         hide_index : bool or None
-            Whether to hide the index column(s). If None (default), the visibility of
-            index columns is automatically determined based on the data.
+            Whether to hide the index column(s). If ``hide_index`` is ``None``
+            (default), the visibility of index columns is automatically
+            determined based on the data.
 
         column_order : Iterable of str or None
             Specifies the display order of columns. This also affects which columns are
             visible. For example, ``column_order=("col2", "col1")`` will display 'col2'
             first, followed by 'col1', and will hide all other non-index columns. If
             None (default), the order is inherited from the original data structure.
```

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/widgets/file_uploader.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/elements/widgets/file_uploader.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/widgets/multiselect.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/elements/widgets/multiselect.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/widgets/number_input.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/elements/widgets/number_input.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/widgets/radio.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/elements/widgets/radio.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/widgets/select_slider.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/elements/widgets/select_slider.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/widgets/selectbox.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/elements/widgets/selectbox.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/widgets/slider.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/elements/widgets/slider.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/widgets/text_widgets.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/elements/widgets/text_widgets.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/widgets/time_widgets.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/elements/widgets/time_widgets.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/write.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/elements/write.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/emojis.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/emojis.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/env_util.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/env_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/error_util.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/error_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/errors.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/errors.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/external/__init__.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/external/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/external/langchain/__init__.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/external/langchain/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/external/langchain/streamlit_callback_handler.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/external/langchain/streamlit_callback_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/file_util.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/file_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/folder_black_list.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/folder_black_list.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/git_util.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/git_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/hello/Hello.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/hello/Hello.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/hello/__init__.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/hello/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/hello/pages/0_Animation_Demo.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/hello/pages/0_Animation_Demo.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/hello/pages/1_Plotting_Demo.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/hello/pages/1_Plotting_Demo.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/hello/pages/2_Mapping_Demo.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/hello/pages/2_Mapping_Demo.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/hello/pages/3_DataFrame_Demo.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/hello/pages/3_DataFrame_Demo.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/hello/utils.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/hello/utils.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/js_number.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/js_number.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/logger.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/logger.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/material_icon_names.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/material_icon_names.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/platform.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/platform.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Alert_pb2.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Alert_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Alert_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/AppPage_pb2.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/AppPage_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/AppPage_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/AppPage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/ArrowNamedDataSet_pb2.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/ArrowNamedDataSet_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/ArrowNamedDataSet_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/ArrowNamedDataSet_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/ArrowVegaLiteChart_pb2.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/ArrowVegaLiteChart_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/ArrowVegaLiteChart_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/ArrowVegaLiteChart_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Arrow_pb2.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Arrow_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Arrow_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Arrow_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Audio_pb2.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Audio_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Audio_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Audio_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/AutoRerun_pb2.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/AutoRerun_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/AutoRerun_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/AutoRerun_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/BackMsg_pb2.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/BackMsg_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/BackMsg_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/BackMsg_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Balloons_pb2.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Balloons_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Balloons_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Balloons_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Block_pb2.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Block_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Block_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Block_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/BokehChart_pb2.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/BokehChart_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/BokehChart_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/BokehChart_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Button_pb2.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Button_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Button_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Button_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/CameraInput_pb2.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/CameraInput_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/CameraInput_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/CameraInput_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/ChatInput_pb2.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/ChatInput_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/ChatInput_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/ChatInput_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Checkbox_pb2.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Checkbox_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Checkbox_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Checkbox_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/ClientState_pb2.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/ClientState_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/ClientState_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/ClientState_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Code_pb2.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Code_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Code_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Code_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/ColorPicker_pb2.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/ColorPicker_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/ColorPicker_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/ColorPicker_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Common_pb2.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Common_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Common_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Components_pb2.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Components_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Components_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Components_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/DataFrame_pb2.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/DataFrame_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/DataFrame_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/DataFrame_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/DateInput_pb2.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/DateInput_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/DateInput_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/DateInput_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/DeckGlJsonChart_pb2.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/DeckGlJsonChart_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/DeckGlJsonChart_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/DeckGlJsonChart_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Delta_pb2.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Delta_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Delta_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Delta_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/DocString_pb2.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/DocString_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/DocString_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/DocString_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/DownloadButton_pb2.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/DownloadButton_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/DownloadButton_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/DownloadButton_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Element_pb2.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Element_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Element_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Element_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Empty_pb2.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Empty_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Empty_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Empty_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Exception_pb2.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Exception_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Exception_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Exception_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Favicon_pb2.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Favicon_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Favicon_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Favicon_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/FileUploader_pb2.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/FileUploader_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/FileUploader_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/FileUploader_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/ForwardMsg_pb2.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/ForwardMsg_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/ForwardMsg_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/ForwardMsg_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/GitInfo_pb2.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/GitInfo_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/GitInfo_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/GitInfo_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/GraphVizChart_pb2.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/GraphVizChart_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/GraphVizChart_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/GraphVizChart_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Heading_pb2.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Heading_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Heading_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Heading_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Html_pb2.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Html_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Html_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Html_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/IFrame_pb2.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/IFrame_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/IFrame_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/IFrame_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Image_pb2.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Image_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Image_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Image_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Json_pb2.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Json_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Json_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Json_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/LabelVisibilityMessage_pb2.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/LabelVisibilityMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/LabelVisibilityMessage_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/LabelVisibilityMessage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/LinkButton_pb2.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/LinkButton_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/LinkButton_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/LinkButton_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Logo_pb2.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Logo_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Logo_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Logo_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Markdown_pb2.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Markdown_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Markdown_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Markdown_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Metric_pb2.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Metric_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Metric_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Metric_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/MultiSelect_pb2.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/MultiSelect_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/MultiSelect_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/MultiSelect_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/NamedDataSet_pb2.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/NamedDataSet_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/NamedDataSet_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/NamedDataSet_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/NewSession_pb2.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/NewSession_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/NewSession_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/NewSession_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/NumberInput_pb2.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/NumberInput_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/NumberInput_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/NumberInput_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/PageConfig_pb2.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/PageConfig_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/PageConfig_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/PageConfig_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/PageInfo_pb2.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/PageInfo_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/PageInfo_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/PageInfo_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/PageLink_pb2.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/PageLink_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/PageLink_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/PageLink_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/PageNotFound_pb2.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/PageNotFound_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/PageNotFound_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/PageNotFound_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/PageProfile_pb2.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/PageProfile_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/PageProfile_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/PageProfile_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/PagesChanged_pb2.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/PagesChanged_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/PagesChanged_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/PagesChanged_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/ParentMessage_pb2.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/ParentMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/ParentMessage_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/ParentMessage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/PlotlyChart_pb2.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/PlotlyChart_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/PlotlyChart_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/PlotlyChart_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Progress_pb2.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Progress_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Progress_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Progress_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Radio_pb2.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Radio_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Radio_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Radio_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/RootContainer_pb2.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/RootContainer_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/RootContainer_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/RootContainer_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Selectbox_pb2.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Selectbox_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Selectbox_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Selectbox_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/SessionEvent_pb2.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/SessionEvent_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/SessionEvent_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/SessionEvent_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/SessionStatus_pb2.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/SessionStatus_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/SessionStatus_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/SessionStatus_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Skeleton_pb2.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Skeleton_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Skeleton_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Skeleton_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Slider_pb2.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Slider_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Slider_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Slider_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Snow_pb2.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Snow_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Snow_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Snow_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Spinner_pb2.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Spinner_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Spinner_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Spinner_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/TextArea_pb2.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/TextArea_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/TextArea_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/TextArea_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/TextInput_pb2.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/TextInput_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/TextInput_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/TextInput_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Text_pb2.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Text_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Text_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Text_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/TimeInput_pb2.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/TimeInput_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/TimeInput_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/TimeInput_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Toast_pb2.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Toast_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Toast_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Toast_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/VegaLiteChart_pb2.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/VegaLiteChart_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/VegaLiteChart_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/VegaLiteChart_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Video_pb2.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Video_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Video_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/Video_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/WidgetStates_pb2.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/WidgetStates_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/WidgetStates_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/WidgetStates_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/__init__.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/openmetrics_data_model_pb2.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/openmetrics_data_model_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/openmetrics_data_model_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240523/streamlit/proto/openmetrics_data_model_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/__init__.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/app_session.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/app_session.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,15 +140,16 @@
         # due to the source code changing we need to pass in the previous client state.
         self._client_state = ClientState()
 
         self._local_sources_watcher: LocalSourcesWatcher | None = None
         self._stop_config_listener: Callable[[], bool] | None = None
         self._stop_pages_listener: Callable[[], None] | None = None
 
-        self.register_file_watchers()
+        if config.get_option("server.fileWatcherType") != "none":
+            self.register_file_watchers()
 
         self._run_on_save = config.get_option("server.runOnSave")
 
         self._scriptrunner: ScriptRunner | None = None
 
         # This needs to be lazily imported to avoid a dependency cycle.
         from streamlit.runtime.state import SessionState
```

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/caching/__init__.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/caching/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/caching/cache_data_api.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/caching/cache_data_api.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/caching/cache_errors.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/caching/cache_errors.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/caching/cache_resource_api.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/caching/cache_resource_api.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/caching/cache_type.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/caching/cache_type.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/caching/cache_utils.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/caching/cache_utils.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/caching/cached_message_replay.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/caching/cached_message_replay.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/caching/hashing.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/caching/hashing.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/caching/storage/__init__.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/caching/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/caching/storage/cache_storage_protocol.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/caching/storage/cache_storage_protocol.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/caching/storage/dummy_cache_storage.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/caching/storage/dummy_cache_storage.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/caching/storage/in_memory_cache_storage_wrapper.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/caching/storage/in_memory_cache_storage_wrapper.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/caching/storage/local_disk_cache_storage.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/caching/storage/local_disk_cache_storage.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/connection_factory.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/connection_factory.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/credentials.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/credentials.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/forward_msg_cache.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/forward_msg_cache.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/forward_msg_queue.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/forward_msg_queue.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/fragment.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/fragment.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/legacy_caching/__init__.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/legacy_caching/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/legacy_caching/caching.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/legacy_caching/caching.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/legacy_caching/hashing.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/legacy_caching/hashing.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/media_file_manager.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/media_file_manager.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/media_file_storage.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/media_file_storage.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/memory_media_file_storage.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/memory_media_file_storage.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/memory_session_storage.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/memory_session_storage.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/memory_uploaded_file_manager.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/memory_uploaded_file_manager.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/metrics_util.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/metrics_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/runtime.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/runtime.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/runtime_util.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/runtime_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/script_data.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/script_data.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/scriptrunner/__init__.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/scriptrunner/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/scriptrunner/magic.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/scriptrunner/magic.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/scriptrunner/magic_funcs.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/scriptrunner/magic_funcs.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/scriptrunner/script_cache.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/scriptrunner/script_cache.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/scriptrunner/script_requests.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/scriptrunner/script_requests.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/scriptrunner/script_run_context.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/scriptrunner/script_run_context.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/scriptrunner/script_runner.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/scriptrunner/script_runner.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/secrets.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/secrets.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/session_manager.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/session_manager.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/state/__init__.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/state/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/state/common.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/state/common.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/state/query_params.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/state/query_params.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/state/query_params_proxy.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/state/query_params_proxy.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/state/safe_session_state.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/state/safe_session_state.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/state/session_state.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/state/session_state.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/state/session_state_proxy.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/state/session_state_proxy.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/state/widgets.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/state/widgets.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/stats.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/stats.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/uploaded_file_manager.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/uploaded_file_manager.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/websocket_session_manager.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/runtime/websocket_session_manager.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/source_util.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/source_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/asset-manifest.json` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/favicon.png` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/favicon.png`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/index.html` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/index.html`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/css/3466.8b8f33d6.chunk.css` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/css/3466.8b8f33d6.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/css/5441.e3b876c5.chunk.css` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/css/5441.e3b876c5.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/css/8148.49dfd2ce.chunk.css` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/css/8148.49dfd2ce.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/css/main.3aaaea00.css` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/css/main.3aaaea00.css`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/1074.73973756.chunk.js` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/1074.73973756.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/1168.14f7c6ff.chunk.js` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/1168.14f7c6ff.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/1307.0f0cca93.chunk.js` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/1307.0f0cca93.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/1451.3b0a3e31.chunk.js` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/1451.3b0a3e31.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/1479.6709db03.chunk.js` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/1479.6709db03.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/178.7bea8c5d.chunk.js` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/178.7bea8c5d.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/1792.8bd6ce2a.chunk.js` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/1792.8bd6ce2a.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/2178.90362aae.chunk.js` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/2178.90362aae.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/2187.9469f035.chunk.js` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/2187.9469f035.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/2469.09ea79bb.chunk.js` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/2469.09ea79bb.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/2634.1249dc7a.chunk.js` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/2634.1249dc7a.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/2736.4336e2b9.chunk.js` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/2736.4336e2b9.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/3053.7e70ec3b.chunk.js` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/3053.7e70ec3b.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/329.464ed8ec.chunk.js` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/329.464ed8ec.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/329.464ed8ec.chunk.js.LICENSE.txt` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/329.464ed8ec.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/3301.1d1b10bb.chunk.js` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/3301.1d1b10bb.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/3466.05d62820.chunk.js` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/3466.05d62820.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/3466.05d62820.chunk.js.LICENSE.txt` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/3466.05d62820.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/3513.7dedbda2.chunk.js` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/3513.7dedbda2.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/4113.99983645.chunk.js` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/4113.99983645.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/4132.49bf3f2c.chunk.js` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/4132.49bf3f2c.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/4177.69f9f18d.chunk.js` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/4177.69f9f18d.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/4319.bf1c86bf.chunk.js` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/4319.bf1c86bf.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/4477.1bd49702.chunk.js` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/4477.1bd49702.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/4500.b6f348d1.chunk.js` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/4500.b6f348d1.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/4666.c4b22a63.chunk.js` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/4666.c4b22a63.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/474.7eb0c6cd.chunk.js` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/474.7eb0c6cd.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/5106.44f0ff51.chunk.js` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/5106.44f0ff51.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/5117.04bfe5d3.chunk.js` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/5117.04bfe5d3.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/5249.f2f4070d.chunk.js` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/5249.f2f4070d.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/5345.73d26e5d.chunk.js` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/5345.73d26e5d.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/5379.6571574f.chunk.js` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/5379.6571574f.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/5441.1b94928f.chunk.js` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/5441.1b94928f.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/5791.9a42fb4b.chunk.js` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/5791.9a42fb4b.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/6013.4ba2d616.chunk.js` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/6013.4ba2d616.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/6405.ac5a6f23.chunk.js` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/6405.ac5a6f23.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/6718.802da17e.chunk.js` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/6718.802da17e.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/6853.93dd1c4c.chunk.js` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/6853.93dd1c4c.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/6950.70fe55c2.chunk.js` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/6950.70fe55c2.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/7142.83028745.chunk.js` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/7142.83028745.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/7175.be4076bc.chunk.js` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/7175.be4076bc.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/7323.b74cc85b.chunk.js` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/7323.b74cc85b.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/7323.b74cc85b.chunk.js.LICENSE.txt` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/7323.b74cc85b.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/7483.64f23be7.chunk.js` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/7483.64f23be7.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/7602.e8abc06b.chunk.js` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/7602.e8abc06b.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/7805.acc6316a.chunk.js` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/7805.acc6316a.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/8005.43974a35.chunk.js` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/8005.43974a35.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/8148.a17a918e.chunk.js` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/8148.a17a918e.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/8427.bd0a7cf3.chunk.js` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/8427.bd0a7cf3.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/8477.de889fe5.chunk.js` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/8477.de889fe5.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/8492.0d93bd08.chunk.js` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/8492.0d93bd08.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/8536.f8de3d9a.chunk.js` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/8536.f8de3d9a.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/8570.6de19120.chunk.js` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/8570.6de19120.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/8691.9ccf7f89.chunk.js` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/8691.9ccf7f89.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/9330.2b4c99e0.chunk.js` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/9330.2b4c99e0.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/9336.3e046ad7.chunk.js` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/9336.3e046ad7.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/937.a1248039.chunk.js` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/937.a1248039.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/9656.8c935274.chunk.js` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/9656.8c935274.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/9865.fd93213d.chunk.js` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/9865.fd93213d.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/main.7e42f54d.js` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/main.7e42f54d.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/main.7e42f54d.js.LICENSE.txt` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/js/main.7e42f54d.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_AMS-Regular.73ea273a72f4aca30ca5.woff2` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_AMS-Regular.73ea273a72f4aca30ca5.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_AMS-Regular.853be92419a6c3766b9a.ttf` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_AMS-Regular.853be92419a6c3766b9a.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_AMS-Regular.d562e886c52f12660a41.woff` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_AMS-Regular.d562e886c52f12660a41.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Caligraphic-Bold.7489a2fbfb9bfe704420.ttf` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Caligraphic-Bold.7489a2fbfb9bfe704420.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Caligraphic-Bold.a1abf90dfd72792a577a.woff2` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Caligraphic-Bold.a1abf90dfd72792a577a.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Caligraphic-Bold.d757c535a2e5902f1325.woff` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Caligraphic-Bold.d757c535a2e5902f1325.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Caligraphic-Regular.7e873d3833eb108a0758.ttf` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Caligraphic-Regular.7e873d3833eb108a0758.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Caligraphic-Regular.d6484fce1ef428d5bd94.woff2` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Caligraphic-Regular.d6484fce1ef428d5bd94.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Caligraphic-Regular.db074fa22cf224af93d7.woff` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Caligraphic-Regular.db074fa22cf224af93d7.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Fraktur-Bold.354501bac435c3264834.woff` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Fraktur-Bold.354501bac435c3264834.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Fraktur-Bold.4c761b3711973ab04edf.ttf` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Fraktur-Bold.4c761b3711973ab04edf.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Fraktur-Bold.931d67ea207ab37ee693.woff2` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Fraktur-Bold.931d67ea207ab37ee693.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Fraktur-Regular.172d3529b26f8cedef6b.woff2` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Fraktur-Regular.172d3529b26f8cedef6b.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Fraktur-Regular.6fdf0ac577be0ba82a4c.woff` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Fraktur-Regular.6fdf0ac577be0ba82a4c.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Fraktur-Regular.ed305b5434865e06ffde.ttf` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Fraktur-Regular.ed305b5434865e06ffde.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Main-Bold.0c3b8929d377c0e9b2f3.woff` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Main-Bold.0c3b8929d377c0e9b2f3.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Main-Bold.39890742bc957b368704.woff2` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Main-Bold.39890742bc957b368704.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Main-Bold.8169508bf58f8bd92ad8.ttf` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Main-Bold.8169508bf58f8bd92ad8.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Main-BoldItalic.20f389c4120be058d80a.woff2` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Main-BoldItalic.20f389c4120be058d80a.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Main-BoldItalic.428978dc7837d46de091.woff` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Main-BoldItalic.428978dc7837d46de091.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Main-BoldItalic.828abcb200061cffbaae.ttf` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Main-BoldItalic.828abcb200061cffbaae.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Main-Italic.fa675e5e4bec9eb250b6.ttf` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Main-Italic.fa675e5e4bec9eb250b6.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Main-Italic.fd947498bc16392e76c2.woff` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Main-Italic.fd947498bc16392e76c2.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Main-Italic.fe2176f79edaa716e621.woff2` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Main-Italic.fe2176f79edaa716e621.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Main-Regular.4f35fbcc9ee8614c2bcc.woff` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Main-Regular.4f35fbcc9ee8614c2bcc.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Main-Regular.9eba1d77abcf2aa6e94e.ttf` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Main-Regular.9eba1d77abcf2aa6e94e.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Main-Regular.f650f111a3b890d116f1.woff2` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Main-Regular.f650f111a3b890d116f1.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Math-BoldItalic.3f07ed67f06c720120ce.woff` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Math-BoldItalic.3f07ed67f06c720120ce.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Math-BoldItalic.bf2d440b3a42ea78a998.ttf` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Math-BoldItalic.bf2d440b3a42ea78a998.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Math-BoldItalic.dcbcbd93bac0470b462d.woff2` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Math-BoldItalic.dcbcbd93bac0470b462d.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Math-Italic.6d3d25f4820d0da8f01f.woff2` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Math-Italic.6d3d25f4820d0da8f01f.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Math-Italic.8a5f936332e8028c7278.ttf` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Math-Italic.8a5f936332e8028c7278.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Math-Italic.96759856b4e70f3a8338.woff` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Math-Italic.96759856b4e70f3a8338.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_SansSerif-Bold.5b49f4993ae22d7975b4.ttf` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_SansSerif-Bold.5b49f4993ae22d7975b4.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_SansSerif-Bold.95591a929f0d32aa282a.woff2` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_SansSerif-Bold.95591a929f0d32aa282a.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_SansSerif-Bold.b9cd458ac6d5889ff9c3.woff` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_SansSerif-Bold.b9cd458ac6d5889ff9c3.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_SansSerif-Italic.7d393d382f3e7fb1c637.woff2` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_SansSerif-Italic.7d393d382f3e7fb1c637.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_SansSerif-Italic.8d593cfaa96238d5e2f8.woff` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_SansSerif-Italic.8d593cfaa96238d5e2f8.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_SansSerif-Italic.b257a18c016f37ee4543.ttf` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_SansSerif-Italic.b257a18c016f37ee4543.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_SansSerif-Regular.02271ec5cb9f5b4588ac.woff` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_SansSerif-Regular.02271ec5cb9f5b4588ac.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_SansSerif-Regular.2f7bc363fc5424ebda59.ttf` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_SansSerif-Regular.2f7bc363fc5424ebda59.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_SansSerif-Regular.cd5e231e0cc53b2cb2c0.woff2` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_SansSerif-Regular.cd5e231e0cc53b2cb2c0.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Script-Regular.073b3402d036714b4370.woff` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Script-Regular.073b3402d036714b4370.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Script-Regular.c81d1b2a4b75d3eded60.woff2` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Script-Regular.c81d1b2a4b75d3eded60.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Script-Regular.fc9ba5249878cd8f8d88.ttf` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Script-Regular.fc9ba5249878cd8f8d88.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Size1-Regular.0108e89c9003e8c14ea3.woff` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Size1-Regular.0108e89c9003e8c14ea3.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Size1-Regular.6de7d4b539221a49e9e2.ttf` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Size1-Regular.6de7d4b539221a49e9e2.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Size1-Regular.6eec866c69313624be60.woff2` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Size1-Regular.6eec866c69313624be60.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Size2-Regular.2960900c4f271311eb36.woff2` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Size2-Regular.2960900c4f271311eb36.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Size2-Regular.3a99e70aee4076660d38.woff` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Size2-Regular.3a99e70aee4076660d38.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Size2-Regular.57f5c1837853986ea1db.ttf` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Size2-Regular.57f5c1837853986ea1db.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Size3-Regular.7947224e8a9914fa332b.woff` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Size3-Regular.7947224e8a9914fa332b.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Size3-Regular.8d6b6822586eea3d3b20.ttf` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Size3-Regular.8d6b6822586eea3d3b20.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Size3-Regular.e1951519f6f0596f7356.woff2` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Size3-Regular.e1951519f6f0596f7356.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Size4-Regular.4ad7c7e8bb8d10a34bb7.ttf` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Size4-Regular.4ad7c7e8bb8d10a34bb7.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Size4-Regular.aeffd8025cba3647f1a6.woff` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Size4-Regular.aeffd8025cba3647f1a6.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Size4-Regular.e418bf257af1052628d8.woff2` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Size4-Regular.e418bf257af1052628d8.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Typewriter-Regular.4c6b94fd1d07f8beff7c.woff` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Typewriter-Regular.4c6b94fd1d07f8beff7c.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Typewriter-Regular.c295e7f71970f03c0549.woff2` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Typewriter-Regular.c295e7f71970f03c0549.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Typewriter-Regular.c5c02d763c89380dcb4e.ttf` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/KaTeX_Typewriter-Regular.c5c02d763c89380dcb4e.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/MaterialSymbols-Outlined.909d2dce4aba724ad02f.woff2` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/MaterialSymbols-Outlined.909d2dce4aba724ad02f.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/SourceCodePro-Bold.17a68a0751a813474a0e.woff2` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/SourceCodePro-Bold.17a68a0751a813474a0e.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/SourceCodePro-BoldItalic.d45b7a3df103d441d78b.woff2` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/SourceCodePro-BoldItalic.d45b7a3df103d441d78b.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/SourceCodePro-Italic.ec122a420df4175e74f2.woff2` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/SourceCodePro-Italic.ec122a420df4175e74f2.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/SourceCodePro-Regular.84b900b88d09398d86b0.woff2` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/SourceCodePro-Regular.84b900b88d09398d86b0.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/SourceCodePro-SemiBold.17291d1c493cb25eb2c3.woff2` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/SourceCodePro-SemiBold.17291d1c493cb25eb2c3.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/SourceCodePro-SemiBoldItalic.f879ae27307c3926522b.woff2` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/SourceCodePro-SemiBoldItalic.f879ae27307c3926522b.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/SourceSansPro-Bold.118dea98980e20a81ced.woff2` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/SourceSansPro-Bold.118dea98980e20a81ced.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/SourceSansPro-BoldItalic.1d664be59d2eb5fef029.woff2` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/SourceSansPro-BoldItalic.1d664be59d2eb5fef029.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/SourceSansPro-Italic.8a9bfea74d43927d6eec.woff2` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/SourceSansPro-Italic.8a9bfea74d43927d6eec.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/SourceSansPro-Regular.0d69e5ff5e92ac64a0c9.woff2` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/SourceSansPro-Regular.0d69e5ff5e92ac64a0c9.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/SourceSansPro-SemiBold.abed79cd0df1827e18cf.woff2` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/SourceSansPro-SemiBold.abed79cd0df1827e18cf.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/SourceSansPro-SemiBoldItalic.befb0a2824eabc5ce36b.woff2` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/SourceSansPro-SemiBoldItalic.befb0a2824eabc5ce36b.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/SourceSerifPro-Bold.d7975b56594770699ae0.woff2` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/SourceSerifPro-Bold.d7975b56594770699ae0.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/SourceSerifPro-BoldItalic.913697a7178b128caa4c.woff2` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/SourceSerifPro-BoldItalic.913697a7178b128caa4c.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/SourceSerifPro-Italic.d3529cb5797663ac5d88.woff2` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/SourceSerifPro-Italic.d3529cb5797663ac5d88.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/SourceSerifPro-Regular.e6c37aa3926474cc93e1.woff2` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/SourceSerifPro-Regular.e6c37aa3926474cc93e1.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/SourceSerifPro-SemiBold.5c1d378dd5990ef334ca.woff2` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/SourceSerifPro-SemiBold.5c1d378dd5990ef334ca.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/SourceSerifPro-SemiBoldItalic.249e948b885d0c7d30a8.woff2` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/SourceSerifPro-SemiBoldItalic.249e948b885d0c7d30a8.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/fireworks.0906f02ea43f1018a6d2.gif` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/fireworks.0906f02ea43f1018a6d2.gif`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/flake-0.beded754e8024c73d9d2.png` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/flake-0.beded754e8024c73d9d2.png`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/flake-1.8077dc154e0bf900aa73.png` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/flake-1.8077dc154e0bf900aa73.png`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/flake-2.e3f07d06933dd0e84c24.png` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/flake-2.e3f07d06933dd0e84c24.png`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/logo.83ae4f2fb87e38be7cbb8a5d2beb64d2.svg` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/logo.83ae4f2fb87e38be7cbb8a5d2beb64d2.svg`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/rocket.b75b17d2b0a063c6cea230d1a9d77f1e.svg` & `streamlit_nightly-1.35.1.dev20240523/streamlit/static/static/media/rocket.b75b17d2b0a063c6cea230d1a9d77f1e.svg`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/string_util.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/string_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/temporary_directory.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/temporary_directory.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/testing/__init__.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/testing/v1/__init__.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/testing/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/testing/v1/app_test.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/testing/v1/app_test.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/testing/v1/element_tree.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/testing/v1/element_tree.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/testing/v1/local_script_runner.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/testing/v1/local_script_runner.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/testing/v1/util.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/testing/v1/util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/time_util.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/time_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/type_util.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/type_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/url_util.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/url_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/user_info.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/user_info.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/util.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/vendor/ipython/modified_sys_path.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/vendor/ipython/modified_sys_path.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/vendor/pympler/asizeof.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/vendor/pympler/asizeof.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/version.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/version.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/watcher/__init__.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/watcher/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/watcher/event_based_path_watcher.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/watcher/event_based_path_watcher.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/watcher/local_sources_watcher.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/watcher/local_sources_watcher.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/watcher/path_watcher.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/watcher/path_watcher.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/watcher/polling_path_watcher.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/watcher/polling_path_watcher.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/watcher/util.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/watcher/util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/web/__init__.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/web/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/web/bootstrap.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/web/bootstrap.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/web/cache_storage_manager_config.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/web/cache_storage_manager_config.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/web/cli.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/web/cli.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/web/server/__init__.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/web/server/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/web/server/app_static_file_handler.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/web/server/app_static_file_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/web/server/browser_websocket_handler.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/web/server/browser_websocket_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -171,23 +171,27 @@
             self._runtime.handle_backmsg_deserialization_exception(self._session_id, ex)
             return
 
         # "debug_disconnect_websocket" and "debug_shutdown_runtime" are special
         # developmentMode-only messages used in e2e tests to test reconnect handling and
         # disabling widgets.
         if msg.WhichOneof("type") == "debug_disconnect_websocket":
-            if config.get_option("global.developmentMode"):
+            if config.get_option("global.developmentMode") or config.get_option(
+                "global.e2eTest"
+            ):
                 self.close()
             else:
                 _LOGGER.warning(
-                    "Client tried to disconnect websocket when not in development mode."
+                    "Client tried to disconnect websocket when not in development mode or e2e testing."
                 )
         elif msg.WhichOneof("type") == "debug_shutdown_runtime":
-            if config.get_option("global.developmentMode"):
+            if config.get_option("global.developmentMode") or config.get_option(
+                "global.e2eTest"
+            ):
                 self._runtime.stop()
             else:
                 _LOGGER.warning(
-                    "Client tried to shut down runtime when not in development mode."
+                    "Client tried to shut down runtime when not in development mode or e2e testing."
                 )
         else:
             # AppSession handles all other BackMsg types.
             self._runtime.handle_backmsg(self._session_id, msg)
```

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/web/server/component_request_handler.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/web/server/component_request_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/web/server/media_file_handler.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/web/server/media_file_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/web/server/routes.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/web/server/routes.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/web/server/server.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/web/server/server.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/web/server/server_util.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/web/server/server_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/web/server/stats_request_handler.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/web/server/stats_request_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/web/server/upload_file_request_handler.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/web/server/upload_file_request_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit/web/server/websocket_headers.py` & `streamlit_nightly-1.35.1.dev20240523/streamlit/web/server/websocket_headers.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit_nightly.egg-info/PKG-INFO` & `streamlit_nightly-1.35.1.dev20240523/streamlit_nightly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-nightly
-Version: 1.34.1.dev20240522
+Version: 1.35.1.dev20240523
 Summary: A faster way to build and share data apps
 Home-page: https://streamlit.io
 Author: Snowflake Inc
 Author-email: hello@streamlit.io
 License: Apache License 2.0
 Project-URL: Source Code, https://github.com/streamlit/streamlit
 Project-URL: Bug Tracker, https://github.com/streamlit/streamlit/issues
```

### Comparing `streamlit_nightly-1.34.1.dev20240522/streamlit_nightly.egg-info/SOURCES.txt` & `streamlit_nightly-1.35.1.dev20240523/streamlit_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240522/tests/testutil.py` & `streamlit_nightly-1.35.1.dev20240523/tests/testutil.py`

 * *Files identical despite different names*

