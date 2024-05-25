# Comparing `tmp/pyside_app_core-0.2.0.tar.gz` & `tmp/pyside_app_core-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyside_app_core-0.2.0.tar", last modified: Thu Apr 25 15:28:07 2024, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `pyside_app_core-0.2.0.tar` & `pyside_app_core-0.3.0.tar`

### file list

```diff
@@ -1,93 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:28:07.094338 pyside_app_core-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    42650 2024-04-25 15:28:07.094338 pyside_app_core-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 15:28:07.094338 pyside_app_core-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:28:07.078338 pyside_app_core-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:28:07.082338 pyside_app_core-0.2.0/src/pyside_app_core/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:28:07.082338 pyside_app_core-0.2.0/src/pyside_app_core/errors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/errors/basic_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/errors/encode_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/errors/excepthook.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/errors/serial_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:28:07.082338 pyside_app_core-0.2.0/src/pyside_app_core/frameless/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/frameless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/frameless/about_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/frameless/base_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     6945 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/frameless/base_window.py
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/frameless/error_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/frameless/main_toolbar_window.py
--rw-r--r--   0 runner    (1001) docker     (127)    11904 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/frameless/window_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/frameless/window_shade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:28:07.086338 pyside_app_core-0.2.0/src/pyside_app_core/log/
--rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/log/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:28:07.086338 pyside_app_core-0.2.0/src/pyside_app_core/qt/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/qt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/qt/application_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:28:07.086338 pyside_app_core-0.2.0/src/pyside_app_core/qt/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/qt/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/qt/util/style_sheet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:28:07.086338 pyside_app_core-0.2.0/src/pyside_app_core/qt/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/qt/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/qt/widgets/base_app.py
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/qt/widgets/dynamic_stacked_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/qt/widgets/menu_ctx.py
--rw-r--r--   0 runner    (1001) docker     (127)     6343 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/qt/widgets/multi_combo_box.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/qt/widgets/object_name_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/qt/widgets/settings_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/qt/widgets/tool_bar_ctx.py
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/qt/widgets/tool_button.py
--rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/qt/widgets/tool_stack.py
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/qt/widgets/window_settings_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:28:07.078338 pyside_app_core-0.2.0/src/pyside_app_core/resources/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:28:07.086338 pyside_app_core-0.2.0/src/pyside_app_core/resources/icons/
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/resources/icons/console.svg
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/resources/icons/down-arrow.svg
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/resources/icons/grab-corner.svg
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/resources/icons/reload.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/resources/icons/save.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:28:07.086338 pyside_app_core-0.2.0/src/pyside_app_core/resources/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/resources/templates/resources.qrc.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)     5903 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/resources/templates/style.qss.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:28:07.090338 pyside_app_core-0.2.0/src/pyside_app_core/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/services/debug_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/services/platform_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:28:07.090338 pyside_app_core-0.2.0/src/pyside_app_core/services/serial_service/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/services/serial_service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6555 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/services/serial_service/serial_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:28:07.090338 pyside_app_core-0.2.0/src/pyside_app_core/services/serial_service/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/services/serial_service/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/services/serial_service/utils/abstract_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/services/serial_service/utils/conversion_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/services/serial_service/utils/float_map.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:28:07.090338 pyside_app_core-0.2.0/src/pyside_app_core/style/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/style/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/style/pixel_val.py
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/style/s_color.py
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/style/theme.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:28:07.090338 pyside_app_core-0.2.0/src/pyside_app_core/theme_generator/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/theme_generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/theme_generator/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/theme_generator/generate_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/theme_generator/standard_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/theme_generator/style_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:28:07.090338 pyside_app_core-0.2.0/src/pyside_app_core/types/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/types/numeric.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:28:07.090338 pyside_app_core-0.2.0/src/pyside_app_core/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-25 15:27:59.000000 pyside_app_core-0.2.0/src/pyside_app_core/utils/compare.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:28:07.090338 pyside_app_core-0.2.0/src/pyside_app_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    42650 2024-04-25 15:28:07.000000 pyside_app_core-0.2.0/src/pyside_app_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-04-25 15:28:07.000000 pyside_app_core-0.2.0/src/pyside_app_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 15:28:07.000000 pyside_app_core-0.2.0/src/pyside_app_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-25 15:28:07.000000 pyside_app_core-0.2.0/src/pyside_app_core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-25 15:28:07.000000 pyside_app_core-0.2.0/src/pyside_app_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-25 15:28:07.000000 pyside_app_core-0.2.0/src/pyside_app_core.egg-info/top_level.txt
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 pyside_app_core-0.3.0/.github/release-drafter.yml
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 pyside_app_core-0.3.0/.github/workflows/ci.yaml
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 pyside_app_core-0.3.0/.github/workflows/draft-release.yml
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 pyside_app_core-0.3.0/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 pyside_app_core-0.3.0/examples/toolbar_app/README.md
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 pyside_app_core-0.3.0/examples/toolbar_app/__init__.py
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 pyside_app_core-0.3.0/examples/toolbar_app/__main__.py
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 pyside_app_core-0.3.0/examples/toolbar_app/app.py
+-rw-r--r--   0        0        0     2305 2020-02-02 00:00:00.000000 pyside_app_core-0.3.0/examples/toolbar_app/main_window.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pyside_app_core-0.3.0/src/pyside_app_core/__init__.py
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 pyside_app_core-0.3.0/src/pyside_app_core/constants.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyside_app_core-0.3.0/src/pyside_app_core/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyside_app_core-0.3.0/src/pyside_app_core/errors/__init__.py
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 pyside_app_core-0.3.0/src/pyside_app_core/errors/basic_errors.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 pyside_app_core-0.3.0/src/pyside_app_core/errors/encode_errors.py
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 pyside_app_core-0.3.0/src/pyside_app_core/errors/excepthook.py
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 pyside_app_core-0.3.0/src/pyside_app_core/errors/serial_errors.py
+-rw-r--r--   0        0        0     2755 2020-02-02 00:00:00.000000 pyside_app_core-0.3.0/src/pyside_app_core/log/__init__.py
+-rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 pyside_app_core-0.3.0/src/pyside_app_core/qt/__init__.py
+-rw-r--r--   0        0        0     2815 2020-02-02 00:00:00.000000 pyside_app_core-0.3.0/src/pyside_app_core/qt/application_service.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 pyside_app_core-0.3.0/src/pyside_app_core/qt/standard/__init__.py
+-rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 pyside_app_core-0.3.0/src/pyside_app_core/qt/standard/about_dialog.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 pyside_app_core-0.3.0/src/pyside_app_core/qt/standard/base_window.py
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 pyside_app_core-0.3.0/src/pyside_app_core/qt/standard/error_dialog.py
+-rw-r--r--   0        0        0     2931 2020-02-02 00:00:00.000000 pyside_app_core-0.3.0/src/pyside_app_core/qt/standard/main_window.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyside_app_core-0.3.0/src/pyside_app_core/qt/widgets/__init__.py
+-rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 pyside_app_core-0.3.0/src/pyside_app_core/qt/widgets/base_app.py
+-rw-r--r--   0        0        0     4879 2020-02-02 00:00:00.000000 pyside_app_core-0.3.0/src/pyside_app_core/qt/widgets/connection_manager.py
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 pyside_app_core-0.3.0/src/pyside_app_core/qt/widgets/core_icon.py
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 pyside_app_core-0.3.0/src/pyside_app_core/qt/widgets/dynamic_stacked_widget.py
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 pyside_app_core-0.3.0/src/pyside_app_core/qt/widgets/menu_ctx.py
+-rw-r--r--   0        0        0     7301 2020-02-02 00:00:00.000000 pyside_app_core-0.3.0/src/pyside_app_core/qt/widgets/multi_combo_box.py
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 pyside_app_core-0.3.0/src/pyside_app_core/qt/widgets/object_name_mixin.py
+-rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 pyside_app_core-0.3.0/src/pyside_app_core/qt/widgets/settings_mixin.py
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 pyside_app_core-0.3.0/src/pyside_app_core/qt/widgets/tool_bar_ctx.py
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 pyside_app_core-0.3.0/src/pyside_app_core/qt/widgets/tool_button.py
+-rw-r--r--   0        0        0     3447 2020-02-02 00:00:00.000000 pyside_app_core-0.3.0/src/pyside_app_core/qt/widgets/tool_stack.py
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 pyside_app_core-0.3.0/src/pyside_app_core/qt/widgets/window_settings_mixin.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 pyside_app_core-0.3.0/src/pyside_app_core/resource_generator/__init__.py
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 pyside_app_core-0.3.0/src/pyside_app_core/resource_generator/__main__.py
+-rw-r--r--   0        0        0     2706 2020-02-02 00:00:00.000000 pyside_app_core-0.3.0/src/pyside_app_core/resource_generator/generate_resources.py
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 pyside_app_core-0.3.0/src/pyside_app_core/resource_generator/resource_types.py
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 pyside_app_core-0.3.0/src/pyside_app_core/resources/core/iconoir/LICENSE.txt
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 pyside_app_core-0.3.0/src/pyside_app_core/resources/core/iconoir/ev-plug-charging.svg
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 pyside_app_core-0.3.0/src/pyside_app_core/resources/core/iconoir/ev-plug-xmark.svg
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 pyside_app_core-0.3.0/src/pyside_app_core/resources/core/iconoir/ev-plug.svg
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 pyside_app_core-0.3.0/src/pyside_app_core/resources/core/iconoir/floppy-disk.svg
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 pyside_app_core-0.3.0/src/pyside_app_core/resources/core/iconoir/iconoir.link
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 pyside_app_core-0.3.0/src/pyside_app_core/resources/core/iconoir/refresh-circle.svg
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 pyside_app_core-0.3.0/src/pyside_app_core/resources/core/notices/about.md.jinja2
+-rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 pyside_app_core-0.3.0/src/pyside_app_core/resources/core/notices/licenses/iconoir.md
+-rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 pyside_app_core-0.3.0/src/pyside_app_core/resources/core/notices/licenses/jinja2.md
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 pyside_app_core-0.3.0/src/pyside_app_core/resources/core/notices/licenses/python.md
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 pyside_app_core-0.3.0/src/pyside_app_core/resources/core/notices/licenses/qt.md
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 pyside_app_core-0.3.0/src/pyside_app_core/resources/templates/resources.qrc.jinja2
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyside_app_core-0.3.0/src/pyside_app_core/services/__init__.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 pyside_app_core-0.3.0/src/pyside_app_core/services/debug_service.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 pyside_app_core-0.3.0/src/pyside_app_core/services/platform_service.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 pyside_app_core-0.3.0/src/pyside_app_core/services/serial_service/__init__.py
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 pyside_app_core-0.3.0/src/pyside_app_core/services/serial_service/conversion_utils.py
+-rw-r--r--   0        0        0     3676 2020-02-02 00:00:00.000000 pyside_app_core-0.3.0/src/pyside_app_core/services/serial_service/float_map.py
+-rw-r--r--   0        0        0     5731 2020-02-02 00:00:00.000000 pyside_app_core-0.3.0/src/pyside_app_core/services/serial_service/service.py
+-rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 pyside_app_core-0.3.0/src/pyside_app_core/services/serial_service/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyside_app_core-0.3.0/src/pyside_app_core/types/__init__.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 pyside_app_core-0.3.0/src/pyside_app_core/types/numeric.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyside_app_core-0.3.0/src/pyside_app_core/utils/__init__.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 pyside_app_core-0.3.0/src/pyside_app_core/utils/compare.py
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 pyside_app_core-0.3.0/src/pyside_app_core/utils/files.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 pyside_app_core-0.3.0/src/pyside_app_core/utils/strings.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 pyside_app_core-0.3.0/src/pyside_app_core/utils/time_ms.py
+-rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 pyside_app_core-0.3.0/tests/unit/test_conversion_utils.py
+-rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 pyside_app_core-0.3.0/tests/unit/test_float_map.py
+-rw-r--r--   0        0        0     2682 2020-02-02 00:00:00.000000 pyside_app_core-0.3.0/tests/unit/test_serial_service.py
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 pyside_app_core-0.3.0/tests/unit/test_utils_compare.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 pyside_app_core-0.3.0/tests/unit/test_utils_format.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 pyside_app_core-0.3.0/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 pyside_app_core-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 pyside_app_core-0.3.0/README.md
+-rw-r--r--   0        0        0     3655 2020-02-02 00:00:00.000000 pyside_app_core-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 pyside_app_core-0.3.0/PKG-INFO
```

### Comparing `pyside_app_core-0.2.0/LICENSE` & `pyside_app_core-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyside_app_core-0.2.0/src/pyside_app_core/constants.py` & `pyside_app_core-0.3.0/src/pyside_app_core/constants.py`

 * *Files identical despite different names*

### Comparing `pyside_app_core-0.2.0/src/pyside_app_core/errors/excepthook.py` & `pyside_app_core-0.3.0/src/pyside_app_core/errors/excepthook.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,41 +1,39 @@
 import sys
 import traceback
 from types import TracebackType
-from typing import Protocol, Type
+from typing import Protocol
 
 from PySide6.QtWidgets import QDialog
 
 from pyside_app_core import log
 
 
 class ErrorDialogInterface(Protocol):
-    def __init__(self, message: str, details: str | None = None):
-        ...
+    def __init__(self, etype: type[BaseException], message: str, details: str | None = None): ...
 
-    def exec(self) -> None:
-        ...
+    def exec(self) -> int: ...
 
 
-_error_dialog_class: Type[ErrorDialogInterface] | None = None
+_error_dialog_class: type[ErrorDialogInterface] | None = None
 
 
-def install_excepthook(error_dialog: Type[QDialog] | None = None) -> None:
-    global _error_dialog_class
+def install_excepthook(error_dialog: type[QDialog] | None) -> None:
+    global _error_dialog_class  # noqa
     _error_dialog_class = error_dialog
     sys.excepthook = __custom_excepthook
 
 
 def __custom_excepthook(
-    etype: Type[BaseException], evalue: BaseException, tb: TracebackType | None
-):
+    etype: type[BaseException],
+    evalue: BaseException,
+    tb: TracebackType | None,
+) -> None:
     formatted_exception_string = "".join(traceback.format_exception(etype, evalue, tb))
 
-    if hasattr(evalue, "internal"):
-        if evalue.internal:
-            log.exception(formatted_exception_string)
-            return
+    log.exception(formatted_exception_string)
+
+    if hasattr(evalue, "internal") and evalue.internal:
+        return
 
     if _error_dialog_class:
-        _error_dialog_class(
-            f"<{etype.__name__}>\n{evalue}", formatted_exception_string
-        ).exec()
+        _error_dialog_class(etype, str(evalue), formatted_exception_string).exec()
```

### Comparing `pyside_app_core-0.2.0/src/pyside_app_core/errors/serial_errors.py` & `pyside_app_core-0.3.0/src/pyside_app_core/errors/serial_errors.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,21 +4,22 @@
 
 
 class SerialError(CoreError):
     def __init__(
         self,
         port: QtSerialPort.QSerialPort | None,
         error: QtSerialPort.QSerialPort.SerialPortError,
-        internal=False,
+        *,
+        internal: bool = False,
     ):
         if port:
             msg = f"Serial error{f' {error} ' if error else ' '}on port: {port.portName()}"
         else:
-            msg = f"Serial port not configured"
-        super(SerialError, self).__init__(msg, internal=internal)
+            msg = "Serial port not configured"
+        super().__init__(msg, internal=internal)
 
 
 class SerialUnknownError(SerialError):
     """something went wrong"""
 
 
 class SerialConnectionError(SerialError):
```

### Comparing `pyside_app_core-0.2.0/src/pyside_app_core/frameless/main_toolbar_window.py` & `pyside_app_core-0.3.0/src/pyside_app_core/qt/standard/main_window.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,75 +1,76 @@
-from PySide6.QtCore import QPoint, QRect, Qt
-from PySide6.QtGui import QAction
+from PySide6.QtCore import Qt, QUrl
+from PySide6.QtGui import QAction, QDesktopServices
 from PySide6.QtWidgets import QMainWindow, QWidget
 
-from pyside_app_core.frameless.about_dialog import AboutDialog
-from pyside_app_core.frameless.base_window import FramelessBaseMixin
+from pyside_app_core.qt.application_service import AppMetadata
+from pyside_app_core.qt.standard.about_dialog import AboutDialog
+from pyside_app_core.qt.standard.base_window import BaseMixin
 from pyside_app_core.qt.widgets.menu_ctx import MenuBarContext
 from pyside_app_core.qt.widgets.tool_bar_ctx import ToolBarContext
 from pyside_app_core.qt.widgets.window_settings_mixin import WindowSettingsMixin
 from pyside_app_core.services import platform_service
 
 
-class FramelessMainToolbarWindow(WindowSettingsMixin, FramelessBaseMixin, QMainWindow):
-    def __init__(self):
-        super(FramelessMainToolbarWindow, self).__init__(parent=None)
+class MainWindow(WindowSettingsMixin, BaseMixin, QMainWindow):
+    def __init__(self) -> None:
+        super().__init__(parent=None)
 
         self._about_dialog = AboutDialog()
 
         self._central = QWidget(parent=self)
-        self._central.setStyleSheet("""background-color: none;""")
         self.setCentralWidget(self._central)
 
         # must call in order to show grab handle
         self.statusBar().show()
 
-        self._menu_bar = MenuBarContext(
-            self,
-            border_width=(
-                0 if platform_service.is_macos else self._theme.win_divider_width
-            ),
-            border_color=self._theme.win_divider_color,
-        )
-
+        self._menu_bar = MenuBarContext(self)
         self._menu_bar.setNativeMenuBar(platform_service.is_macos)
-        self.setMenuWidget(self._menu_bar)
+        self.setMenuBar(self._menu_bar)
 
-        with self._menu_bar.add_menu(self.tr("File")) as file_menu:
-            with file_menu.add_action(self.tr("Quit")) as exit_action:
-                exit_action.setMenuRole(QAction.MenuRole.QuitRole)
-                exit_action.triggered.connect(self.close)
+        with (
+            self._menu_bar.menu("File") as file_menu,
+            file_menu.action("Quit") as exit_action,
+        ):
+            exit_action.setMenuRole(QAction.MenuRole.QuitRole)
+            exit_action.triggered.connect(self.close)
+
+        self._build_menus()
+
+        with self._menu_bar.menu("Window") as window_menu:
+            with window_menu.action("Minimize") as min_action:
+                min_action.setShortcut("Ctrl+M")
+                min_action.triggered.connect(self.showMinimized)
+            with window_menu.action("Zoom") as zoom_action:
+                zoom_action.triggered.connect(self.showMaximized)
 
-        with self._menu_bar.add_menu(self.tr("Help")) as help_menu:
-            with help_menu.add_action(self.tr("About")) as about_action:
+        with self._menu_bar.menu("Help") as help_menu:
+            with help_menu.action("About") as about_action:
                 about_action.setMenuRole(QAction.MenuRole.AboutRole)
+                about_action.triggered.connect(self._about_dialog.exec)
 
-                def _show_about():
-                    self._about_dialog.exec()
+            if AppMetadata.help_url:
+                with help_menu.action("Get Help") as help_action:
+                    help_action.triggered.connect(lambda: QDesktopServices.openUrl(QUrl(AppMetadata.help_url)))
+
+            if AppMetadata.bug_report_url:
+                with help_menu.action("Report Bug") as help_action:
+                    help_action.triggered.connect(lambda: QDesktopServices.openUrl(QUrl(AppMetadata.bug_report_url)))
 
-                about_action.triggered.connect(_show_about)
+    @property
+    def menu_bar(self) -> MenuBarContext:
+        return self._menu_bar
 
-        self._tool_bar = ToolBarContext(area="top", parent=self, movable=False)
-        self._tool_bar.setToolButtonStyle(Qt.ToolButtonStyle.ToolButtonIconOnly)
+    def _build_menus(self) -> None:
+        pass
 
-        if platform_service.is_macos:
-            spacer = QWidget(self)
-            spacer.setFixedWidth(self._window_actions.container_width + 5)
-            spacer.setFixedHeight(28)
-            self._tool_bar.addWidget(spacer)
-
-        self._menu_bar.set_offset(
-            5 if platform_service.is_macos else self._window_actions.container_height
-        )
-        self._menu_bar.set_shift(8)
 
-    @property
-    def menu_bar(self):
-        return self._menu_bar
+class MainToolbarWindow(MainWindow):
+    def __init__(self) -> None:
+        super().__init__()
 
-    @property
-    def tool_bar(self):
-        return self._tool_bar
+        self._tool_bar = ToolBarContext(area="top", parent=self, movable=False)
+        self._tool_bar.setToolButtonStyle(Qt.ToolButtonStyle.ToolButtonIconOnly)
 
     @property
-    def window_bar_geo(self) -> QRect:
-        return QRect(QPoint(0, 0), self.tool_bar.geometry().bottomRight())
+    def tool_bar(self) -> ToolBarContext:
+        return self._tool_bar
```

### Comparing `pyside_app_core-0.2.0/src/pyside_app_core/qt/widgets/dynamic_stacked_widget.py` & `pyside_app_core-0.3.0/src/pyside_app_core/qt/widgets/dynamic_stacked_widget.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,14 @@
 from PySide6 import QtWidgets
 from PySide6.QtWidgets import QSizePolicy
 
 from pyside_app_core.qt.widgets.object_name_mixin import ObjectNameMixin
 
 
 class DynamicStackedWidget(ObjectNameMixin, QtWidgets.QStackedWidget):
-    def __init__(self, parent: QtWidgets.QWidget):
-        super(DynamicStackedWidget, self).__init__(parent=parent)
+    def __init__(self, parent: QtWidgets.QWidget) -> None:
+        super().__init__(parent=parent)
 
         self.setSizePolicy(QSizePolicy.Policy.Maximum, QSizePolicy.Policy.Maximum)
         self.setMinimumHeight(10)
         self.setMaximumHeight(100000)
         self.setContentsMargins(0, 0, 0, 0)
-
-        self.setStyleSheet(
-            f"""
-        #{self.obj_name} QStackedWidget{{
-            background: red;
-        }}
-        """
-        )
```

### Comparing `pyside_app_core-0.2.0/src/pyside_app_core/qt/widgets/multi_combo_box.py` & `pyside_app_core-0.3.0/src/pyside_app_core/qt/widgets/multi_combo_box.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,180 +1,217 @@
 """
 Adapted from:
 https://gis.stackexchange.com/questions/350148/qcombobox-multiple-selection-pyqt5
 """
 
-from typing import Generator, Generic, Tuple, TypeVar
+from collections.abc import Generator
+from typing import Generic, TypeVar, cast
 
-from PySide6.QtCore import QEvent, Qt, Signal
-from PySide6.QtGui import QFontMetrics, QStandardItem
-from PySide6.QtWidgets import QComboBox, QStyledItemDelegate, QWidget
+from PySide6.QtCore import (
+    QEvent,
+    QModelIndex,
+    QObject,
+    QPersistentModelIndex,
+    QSize,
+    Qt,
+    QTimerEvent,
+    Signal,
+)
+from PySide6.QtGui import (
+    QFontMetrics,
+    QMouseEvent,
+    QResizeEvent,
+    QStandardItem,
+    QStandardItemModel,
+)
+from PySide6.QtWidgets import (
+    QComboBox,
+    QStyledItemDelegate,
+    QStyleOptionViewItem,
+    QWidget,
+)
 
 from pyside_app_core.qt.widgets.object_name_mixin import ObjectNameMixin
 from pyside_app_core.qt.widgets.settings_mixin import SettingsMixin
 
 DT = TypeVar("DT")
 
 
-class MultiComboBox(ObjectNameMixin, SettingsMixin, Generic[DT], QComboBox):
-    # Subclass Delegate to increase item height
+class MultiComboBox(ObjectNameMixin, SettingsMixin, QComboBox, Generic[DT]):
+    """a combo box of checkable items.
+    The selected options will be listed as text in the combo box line.
+    The first option is a show/hide all option.
+    """
+
     class Delegate(QStyledItemDelegate):
-        def sizeHint(self, option, index):
+        def sizeHint(  # noqa:N802
+            self,
+            option: QStyleOptionViewItem,
+            index: QModelIndex | QPersistentModelIndex,
+        ) -> QSize:
             size = super().sizeHint(option, index)
             size.setHeight(20)
             return size
 
-    selectionChanged = Signal(list)
+    selectionChanged = Signal(list)  # noqa:N815
 
-    def __init__(self, parent: QWidget, *args, **kwargs):
-        super(MultiComboBox, self).__init__(parent=parent, *args, **kwargs)
+    def __init__(
+        self,
+        placeholder_text: str,
+        all_text: str = "Show/Hide All",
+        parent: QWidget | None = None,
+        *args: object,
+        **kwargs: object,
+    ) -> None:
+        super().__init__(*args, parent=parent, **kwargs)
 
         # Make the combo editable to set a custom text, but readonly
         self.setEditable(True)
         self.lineEdit().setReadOnly(True)
-        self.lineEdit().setPlaceholderText("Command Filter")
+        self.lineEdit().setPlaceholderText(placeholder_text)
 
         # Use custom delegate
         self.setItemDelegate(MultiComboBox.Delegate())
 
         # Hide and show popup when clicking the line edit
         self.lineEdit().installEventFilter(self)
         self.closeOnLineEditClick = False
 
         # Prevent popup from closing when clicking on an item
         self.view().viewport().installEventFilter(self)
 
-        self.addItem("Show/Hide All", isChecked=True)
+        self.addItem(all_text, is_checked=True)
 
         self.model().itemChanged.connect(self._update_selection)
         self.model().dataChanged.connect(self._update_text)
         self.model().dataChanged.connect(self._emit_current_data)
 
-    def _emit_current_data(self):
+    def model(self) -> QStandardItemModel:
+        return cast(QStandardItemModel, super().model())
+
+    def _emit_current_data(self) -> None:
         self.selectionChanged.emit(self.currentData())
 
-    def _update_selection(self, item: QStandardItem):
+    def _update_selection(self, item: QStandardItem) -> None:
         if item.index().row() == 0:
+            # update on the show/hide all case
             state = item.checkState()
             self.model().layoutAboutToBeChanged.emit()
             for item in self.modelItems():
                 item.setCheckState(state)
             self.model().layoutChanged.emit()
 
-    def resizeEvent(self, event):
+    def resizeEvent(self, event: QResizeEvent) -> None:  # noqa: N802
         # Recompute text to elide as needed
         self._update_text()
         super().resizeEvent(event)
 
-    def eventFilter(self, object, event):
-        if object == self.lineEdit():
+    def eventFilter(self, watched: QObject, event: QEvent) -> bool:  # noqa: N802
+        if watched == self.lineEdit():
             if event.type() == QEvent.Type.MouseButtonRelease:
                 if self.closeOnLineEditClick:
                     self.hidePopup()
                 else:
                     self.showPopup()
                 return True
             return False
 
-        if object == self.view().viewport():
-            if event.type() == QEvent.Type.MouseButtonRelease:
-                index = self.view().indexAt(event.pos())
-                item = self.model().item(index.row())
+        if watched == self.view().viewport() and (
+            isinstance(event, QMouseEvent) and event.type() == QEvent.Type.MouseButtonRelease
+        ):
+            index = self.view().indexAt(event.pos())
+            item = self.model().item(index.row())
 
-                if item.checkState() == Qt.CheckState.Checked:
-                    item.setCheckState(Qt.CheckState.Unchecked)
-                else:
-                    item.setCheckState(Qt.CheckState.Checked)
-                return True
+            if item.checkState() == Qt.CheckState.Checked:
+                item.setCheckState(Qt.CheckState.Unchecked)
+            else:
+                item.setCheckState(Qt.CheckState.Checked)
+            return True
         return False
 
-    def showPopup(self):
+    def showPopup(self) -> None:  # noqa: N802
         super().showPopup()
         # When the popup is displayed, a click on the lineedit should close it
         self.closeOnLineEditClick = True
 
-    def hidePopup(self):
+    def hidePopup(self) -> None:  # noqa: N802
         super().hidePopup()
         # Used to prevent immediate reopening when clicking on the lineEdit
         self.startTimer(100)
         # Refresh the display text when closing
         self._update_text()
 
-    def timerEvent(self, event):
+    def timerEvent(self, event: QTimerEvent) -> None:  # noqa: N802
         # After timeout, kill timer, and re-enable click on line edit
         self.killTimer(event.timerId())
         self.closeOnLineEditClick = False
 
-    def _update_text(self):
-        texts = []
-        for item in self.modelItems():
-            if item.checkState() == Qt.CheckState.Checked:
-                texts.append(item.text())
+    def _update_text(self) -> None:
+        texts = [i.text() for i in self.modelItems() if i.checkState() == Qt.CheckState.Checked]
         text = ", ".join(texts)
 
         # Compute elided text (with "...")
         metrics = QFontMetrics(self.lineEdit().font())
-        text = metrics.elidedText(
-            text, Qt.TextElideMode.ElideRight, self.lineEdit().width()
-        )
+        text = metrics.elidedText(text, Qt.TextElideMode.ElideRight, self.lineEdit().width())
         self.lineEdit().setText(text)
 
-    def addItem(self, text, userData: DT | None = None, isChecked=False, **kwargs):
+    def addItem(  # type:ignore[override] # noqa
+        self,
+        text: str,
+        user_data: DT | None = None,
+        *,
+        is_checked: bool = False,
+    ) -> None:
         item = QStandardItem()
         item.setText(text)
-        if userData is None:
+        if user_data is None:
             item.setData(text, Qt.ItemDataRole.UserRole)
         else:
-            item.setData(userData, Qt.ItemDataRole.UserRole)
+            item.setData(user_data, Qt.ItemDataRole.UserRole)
 
         item.setFlags(Qt.ItemFlag.ItemIsEnabled | Qt.ItemFlag.ItemIsUserCheckable)
-        item.setCheckState(
-            Qt.CheckState.Checked if isChecked else Qt.CheckState.Unchecked
-        )
+        item.setCheckState(Qt.CheckState.Checked if is_checked else Qt.CheckState.Unchecked)
 
         self.model().appendRow(item)
 
-    def addItems(
-        self, texts: list[str], dataList: list[DT] | None = None, allChecked=False
-    ):
+    def addItems(  # type:ignore[override] # noqa
+        self,
+        texts: list[str],
+        data_list: list[DT] | None = None,
+        *,
+        all_checked: bool = False,
+    ) -> None:
         for i, text in enumerate(texts):
             try:
-                data = (dataList or [])[i]
+                data = (data_list or [])[i]
             except (TypeError, IndexError):
                 data = None
-            self.addItem(text, data, isChecked=allChecked)
-
-    def currentData(self, role: Qt.ItemDataRole = Qt.ItemDataRole.UserRole) -> list[DT]:
-        res = []
-        for item in self.modelItems():
-            if item.checkState() == Qt.CheckState.Checked:
-                res.append(item.data(role))
-        return res
+            self.addItem(text, data, is_checked=all_checked)
 
-    def currentOptions(self) -> list[Tuple[str, DT]]:
-        res = []
-        for item in self.modelItems():
-            if item.checkState() == Qt.CheckState.Checked:
-                res.append((item.text(), item.data(Qt.ItemDataRole.UserRole)))
-        return res
+    def currentData(  # type: ignore[override] # noqa
+        self,
+        role: Qt.ItemDataRole = Qt.ItemDataRole.UserRole,
+    ) -> list[DT]:
+        return [i.data(role) for i in self.modelItems() if i.checkState() == Qt.CheckState.Checked]
+
+    def currentOptions(self) -> list[tuple[str, DT]]:  # noqa: N802
+        return [
+            (i.text(), i.data(Qt.ItemDataRole.UserRole))
+            for i in self.modelItems()
+            if i.checkState() == Qt.CheckState.Checked
+        ]
 
-    def modelItems(self) -> Generator[QStandardItem, None, None]:
+    def modelItems(self) -> Generator[QStandardItem, None, None]:  # noqa: N802
         for i in range(1, self.model().rowCount()):
             yield self.model().item(i)
 
     def _restore_state(self) -> None:
-        options = self._settings.value(f"{self.obj_name}_options")
+        options = cast(list[str], self._settings.value(f"{self.obj_name}_options"))
         if not options:
             return
 
         for item in self.modelItems():
-            state = (
-                Qt.CheckState.Checked
-                if item.text() in options
-                else Qt.CheckState.Unchecked
-            )
+            state = Qt.CheckState.Checked if item.text() in options else Qt.CheckState.Unchecked
             item.setCheckState(state)
 
     def _store_state(self) -> None:
-        self._settings.setValue(
-            f"{self.obj_name}_options", [n for n, _ in self.currentOptions()]
-        )
+        self._settings.setValue(f"{self.obj_name}_options", [n for n, _ in self.currentOptions()])
```

### Comparing `pyside_app_core-0.2.0/src/pyside_app_core/qt/widgets/object_name_mixin.py` & `pyside_app_core-0.3.0/src/pyside_app_core/qt/widgets/object_name_mixin.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from typing import cast
 
 from PySide6.QtCore import Qt
 from PySide6.QtWidgets import QWidget
 
 
 class ObjectNameMixin:
-    def __init__(self, *args, **kwargs):
-        super(ObjectNameMixin, self).__init__(*args, **kwargs)
+    def __init__(self, *args: object, **kwargs: object) -> None:
+        super().__init__(*args, **kwargs)
 
         if isinstance(self, QWidget):
             self.setAttribute(Qt.WidgetAttribute.WA_StyledBackground)
 
         obj_name = self.__class__.__name__
         if hasattr(self, "OBJECT_NAME"):
             obj_name = self.OBJECT_NAME.replace(" ", "_")
 
         cast(QWidget, self).setObjectName(obj_name)
 
     @property
-    def obj_name(self):
+    def obj_name(self) -> str:
         return cast(QWidget, self).objectName()
```

### Comparing `pyside_app_core-0.2.0/src/pyside_app_core/qt/widgets/settings_mixin.py` & `pyside_app_core-0.3.0/src/pyside_app_core/qt/widgets/settings_mixin.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,36 @@
-import os
 from typing import cast
 
 from PySide6.QtCore import QCoreApplication, QObject, QSettings
 from PySide6.QtGui import QShowEvent
 from PySide6.QtWidgets import QWidget
 
-from pyside_app_core.qt import application_service
+from pyside_app_core.qt.application_service import AppMetadata
 
 
 class SettingsMixin:
-    def __init__(self, parent: QObject, *args, **kwargs):
-        super(SettingsMixin, self).__init__(*args, **kwargs)
+    def __init__(self, parent: QObject | None = None, *args: object, **kwargs: object):
+        super().__init__(*args, **kwargs)
 
         self._settings = QSettings(
-            application_service.get_app_id(),
-            application_service.get_app_name(),
+            AppMetadata.id,
+            AppMetadata.name,
             parent,
         )
 
         self._restored = False
 
-        QCoreApplication.instance().aboutToQuit.connect(self._store_state)
+        cast(QCoreApplication, QCoreApplication.instance()).aboutToQuit.connect(self._store_state)
 
-    def showEvent(self, event: QShowEvent):
+    def showEvent(self, event: QShowEvent) -> None:  # noqa: N802
         if not self._restored:
             self._restore_state()
             self._restored = True
 
         if isinstance(self, QWidget):
             cast(QWidget, super()).showEvent(event)
 
-    def _restore_state(self):
+    def _restore_state(self) -> None:
         pass
 
-    def _store_state(self):
+    def _store_state(self) -> None:
         pass
```

### Comparing `pyside_app_core-0.2.0/src/pyside_app_core/qt/widgets/tool_bar_ctx.py` & `pyside_app_core-0.3.0/src/pyside_app_core/qt/widgets/tool_bar_ctx.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,79 +1,56 @@
 import contextlib
-from typing import ContextManager, List, Literal
+from collections.abc import Iterator
+from typing import Literal
 
 from PySide6.QtCore import QSize, Qt
 from PySide6.QtGui import QAction, QIcon
 from PySide6.QtWidgets import QMainWindow, QToolBar, QToolButton
 
 from pyside_app_core.qt.widgets.object_name_mixin import ObjectNameMixin
-from pyside_app_core.qt import application_service
 
 ToolBarArea = Literal["top", "bottom", "left", "right"]
 
 _TOOL_BAR_AREA_MAP = {
     "top": Qt.ToolBarArea.TopToolBarArea,
     "bottom": Qt.ToolBarArea.BottomToolBarArea,
     "right": Qt.ToolBarArea.RightToolBarArea,
     "left": Qt.ToolBarArea.LeftToolBarArea,
 }
 
 
 class ToolBarContext(ObjectNameMixin, QToolBar):
-    def __init__(self, area: ToolBarArea, parent: QMainWindow, movable=False):
+    def __init__(self, area: ToolBarArea, parent: QMainWindow, *, movable: bool = False) -> None:
         self._area = area
-        self._theme = application_service.get_app_theme()
-        self._actions: List[QAction] = []
+        self._actions: list[QAction] = []
 
         if area == "left":
             self._border_side = "right"
         elif area == "right":
             self._border_side = "left"
         elif area == "top":
             self._border_side = "bottom"
         else:
             self._border_side = "top"
 
         self.OBJECT_NAME = f"ToolBar_{area}"
-        super(ToolBarContext, self).__init__(self.OBJECT_NAME, parent=parent)
+        super().__init__(self.OBJECT_NAME, parent=parent)
 
         self.setContentsMargins(0, 0, 0, 0)
         self.setGeometry(10, 10, self.width(), self.height())
         self.setMovable(movable)
         self.setIconSize(QSize(28, 28))
 
         parent.addToolBar(_TOOL_BAR_AREA_MAP[self._area], self)
 
-        self._setup_style()
-
     @contextlib.contextmanager
-    def add_action(
-        self, name: str, icon: QIcon | None = None
-    ) -> ContextManager[QAction]:
+    def add_action(self, name: str, icon: QIcon | None = None) -> Iterator[QAction]:
         action = QAction(text=name, parent=self)
         action.setObjectName(f"ToolBarAction_{name}")
         if icon:
             action.setIcon(icon)
 
         self._actions.append(action)
         if len(self._actions) == 1:
-            _ = [c for c in self.children() if isinstance(c, QToolButton)][0]
+            _ = next(c for c in self.children() if isinstance(c, QToolButton))
         yield action
         self.addAction(action)
-
-    def _setup_style(self):
-        self.setStyleSheet(
-            f"""
-QToolBar#{self.obj_name} {{
-    border-{self._border_side}: {self._theme.win_divider_width} solid {self._theme.win_divider_color};
-}}
-QToolBar#{self.obj_name} > QToolButton {{
-    margin-left: 0px;
-    margin-top: 10px;
-    margin-bottom: 10px;
-    spacing: 0;
-}}
-QToolButton:first {{
-    background-color: red;
-}}
-"""
-        )
```

### Comparing `pyside_app_core-0.2.0/src/pyside_app_core/qt/widgets/tool_button.py` & `pyside_app_core-0.3.0/src/pyside_app_core/qt/widgets/tool_button.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from typing import Tuple
-
 from PySide6.QtCore import QSize
 from PySide6.QtGui import QIcon
 from PySide6.QtWidgets import QPushButton, QWidget
 
 from pyside_app_core.qt.widgets.object_name_mixin import ObjectNameMixin
 
 
 class ToolButton(ObjectNameMixin, QPushButton):
     def __init__(self, icon: QIcon, tooltip: str, parent: QWidget):
-        super(ToolButton, self).__init__(icon=icon, parent=parent)
+        super().__init__(icon=icon, parent=parent)
 
         self.setMinimumSize(24, 24)
 
         self.setToolTip(tooltip)
         self.setContentsMargins(0, 0, 0, 0)
 
-    def setFixedSize(self, size: QSize | Tuple[int, int]) -> None:
+    def setFixedSize(  # type: ignore[override] # noqa
+        self, size: QSize | tuple[int, int]
+    ) -> None:
         if isinstance(size, tuple):
             size = QSize(size[0], size[1])
         super().setFixedSize(size + QSize(10, 10))
         self.setIconSize(size)
```

### Comparing `pyside_app_core-0.2.0/src/pyside_app_core/qt/widgets/tool_stack.py` & `pyside_app_core-0.3.0/src/pyside_app_core/qt/widgets/tool_stack.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,41 +4,28 @@
 from PySide6.QtGui import QAction, QIcon
 from PySide6.QtWidgets import QButtonGroup, QHBoxLayout, QMenu, QVBoxLayout, QWidget
 
 from pyside_app_core.qt.widgets.dynamic_stacked_widget import DynamicStackedWidget
 from pyside_app_core.qt.widgets.object_name_mixin import ObjectNameMixin
 from pyside_app_core.qt.widgets.settings_mixin import SettingsMixin
 from pyside_app_core.qt.widgets.tool_button import ToolButton
-from pyside_app_core.style.theme import QssTheme
 
 ToolStackSide = Literal["right", "left"]
 
 
 class ToolStack(SettingsMixin, ObjectNameMixin, QWidget):
     def __init__(
         self,
         side: ToolStackSide,
         parent: QWidget,
-        theme: QssTheme,
         menu: QMenu | None = None,
     ):
-        super(ToolStack, self).__init__(parent=parent)
+        super().__init__(parent=parent)
 
-        opposite_side = "left" if side == "right" else "right"
-
-        self.setStyleSheet(
-            f"""
-            #{self.obj_name}_CONTAINER {{
-                border-{opposite_side}: {theme.win_divider_width} solid {theme.win_divider_color};
-            }}
-            #{self.obj_name}_BUTTON_CONTAINER {{
-                border-{opposite_side}: {theme.win_divider_width} solid {theme.win_divider_color};
-            }}
-            """
-        )
+        # opposite_side = "left" if side == "right" else "right"
 
         self._menu = menu
 
         container_layout = QHBoxLayout()
         container_layout.setContentsMargins(0, 0, 0, 0)
         container_layout.setSpacing(0)
         self.setLayout(container_layout)
@@ -60,15 +47,15 @@
             container_layout.addWidget(self._stack)
             container_layout.addWidget(_button_container)
         else:
             self._button_layout.setContentsMargins(10, 10, 10, 3)
             container_layout.addWidget(_button_container)
             container_layout.addWidget(self._stack)
 
-    def add_widget(self, icon: QIcon, widget: QWidget, tooltip: str):
+    def add_widget(self, icon: QIcon, widget: QWidget, tooltip: str) -> None:
         container = QWidget(self)
         container.setObjectName(f"{self.obj_name}_CONTAINER")
         container_layout = QVBoxLayout()
         container.setLayout(container_layout)
         container_layout.addWidget(widget)
         container_layout.addStretch()
 
@@ -92,21 +79,21 @@
 
         if self._menu:
             action = QAction(text=tooltip, parent=self._menu)
             action.triggered.connect(lambda: self._on_menu_click(index))
             self._menu.addAction(action)
 
     @Slot(int, bool)
-    def _on_click(self, index: int, checked: bool):
+    def _on_click(self, index: int, checked: bool) -> None:  # noqa: FBT001
         for i, button in enumerate(self._button_group.buttons()):
             self._stack.setCurrentIndex(index)
 
             if index == i:
                 self._stack.setVisible(checked)
                 button.setChecked(checked)
 
             else:
                 button.setChecked(False)
 
     @Slot(int, bool)
-    def _on_menu_click(self, index: int):
+    def _on_menu_click(self, index: int) -> None:
         self._on_click(index, True)
```

### Comparing `pyside_app_core-0.2.0/src/pyside_app_core/qt/widgets/window_settings_mixin.py` & `pyside_app_core-0.3.0/src/pyside_app_core/qt/widgets/window_settings_mixin.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,26 @@
 from typing import cast
 
-from PySide6.QtCore import QObject
+from PySide6.QtCore import QByteArray, QObject
 from PySide6.QtWidgets import QMainWindow, QWidget
 
 from pyside_app_core.qt.widgets.object_name_mixin import ObjectNameMixin
 from pyside_app_core.qt.widgets.settings_mixin import SettingsMixin
 
 
 class WindowSettingsMixin(ObjectNameMixin, SettingsMixin):
-    def __init__(self, parent: QObject, *args, **kwargs):
-        super(WindowSettingsMixin, self).__init__(parent=parent, *args, **kwargs)
+    def __init__(self, parent: QObject | None = None, *args: object, **kwargs: object) -> None:
+        super().__init__(*args, parent=parent, **kwargs)
 
     def _store_state(self) -> None:
-        self._settings.setValue(
-            f"{self.obj_name}_geometry", cast(QWidget, self).saveGeometry()
-        )
+        self._settings.setValue(f"{self.obj_name}_geometry", cast(QWidget, self).saveGeometry())
 
         if isinstance(self, QMainWindow):
-            cast(SettingsMixin, self)._settings.setValue(
+            cast(SettingsMixin, self)._settings.setValue(  # noqa: SLF001
                 f"{cast(ObjectNameMixin, self).obj_name}_window_state", self.saveState()
             )
 
     def _restore_state(self) -> None:
-        cast(QWidget, self).restoreGeometry(
-            self._settings.value(f"{self.obj_name}_geometry")
-        )
+        cast(QWidget, self).restoreGeometry(cast(QByteArray, self._settings.value(f"{self.obj_name}_geometry")))
 
-        # if isinstance(self, QMainWindow):
-        #     self.restoreState(self._settings.value(f"{self.obj_name}_window_state"))
+        if isinstance(self, QMainWindow):
+            self.restoreState(cast(QByteArray, self._settings.value(f"{self.obj_name}_window_state")))
```

### Comparing `pyside_app_core-0.2.0/src/pyside_app_core/services/serial_service/serial_service.py` & `pyside_app_core-0.3.0/src/pyside_app_core/services/serial_service/service.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,58 +1,62 @@
-import logging
-from typing import List, Protocol
+from typing import cast
 
-from PySide6.QtCore import QIODevice, QObject, Qt, QTimer, Signal
+from PySide6.QtCore import QIODevice, QObject, QTimer, Signal
 from PySide6.QtSerialPort import QSerialPort, QSerialPortInfo
 
 from pyside_app_core import log
 from pyside_app_core.errors.serial_errors import (
     SerialConnectionError,
     SerialDisconnectedError,
     SerialError,
     SerialReadError,
     SerialUnknownError,
     SerialWriteError,
 )
-from pyside_app_core.services.serial_service.utils.abstract_decoder import (
-    CommandInterface,
+from pyside_app_core.services.serial_service.types import (
+    Encodable,
+    PortFilter,
+    SerialReader,
     TranscoderInterface,
 )
+from pyside_app_core.utils.time_ms import SECONDS
 
-log.set_level(lvl=logging.DEBUG)
 
-
-class CanRegister(Protocol):
-    def bind_serial_service(self, serial_service: "SerialService"):
-        ...
+def _noop(ports: list[QSerialPortInfo]) -> list[QSerialPortInfo]:
+    log.debug(f"Filtering ports: {ports}")
+    return ports
 
 
 class SerialService(QObject):
     ports = Signal(list)
     com_connect = Signal(QSerialPort)
     com_disconnect = Signal()
     data = Signal(object)
     error = Signal(Exception)
 
-    def __init__(self, transcoder: TranscoderInterface, parent: QObject):
-        super(SerialService, self).__init__(parent=parent)
+    def __init__(self, transcoder: type[TranscoderInterface], parent: QObject):
+        super().__init__(parent=parent)
+
+        self._port_filter: PortFilter = _noop
 
-        self._transcoder = transcoder
+        self._transcoder: type[TranscoderInterface] = transcoder
         self._com: QSerialPort | None = None
         self._buffer = bytearray()
 
-    def _new_com(
-        self, port_info: QSerialPortInfo
-    ) -> tuple[QSerialPort, QSerialPort.SerialPortError | None]:
+    def _new_com(self, port_info: QSerialPortInfo) -> tuple[QSerialPort, QSerialPort.SerialPortError | None]:
         com = QSerialPort(port_info, parent=self)
         com.setBaudRate(QSerialPort.BaudRate.Baud115200)
         open_ok = com.open(QIODevice.OpenModeFlag.ReadWrite)
 
         return com, None if open_ok else com.error()
 
+    def set_port_filter(self, func: PortFilter) -> None:
+        log.debug(f"updating port filter: {func}")
+        self._port_filter = func
+
     def open_connection(self, port_info: QSerialPortInfo) -> bool:
         self.close_connection()
 
         self._com, error = self._new_com(port_info)
         if error:
             self._on_error(error)
             return False
@@ -60,143 +64,110 @@
         self._com.readyRead.connect(self._on_data)
         self._com.errorOccurred.connect(self._on_error)
 
         self.com_connect.emit(self._com)
 
         return True
 
-    def register_reader(self, reader: QObject) -> None:
-        if hasattr(reader, "handle_serial_connect"):
-            self.com_connect[QSerialPort].connect(
-                reader.handle_serial_connect,
-                type=Qt.ConnectionType.UniqueConnection,
-            )
-        if hasattr(reader, "handle_serial_disconnect"):
-            self.com_disconnect.connect(
-                reader.handle_serial_disconnect,
-                type=Qt.ConnectionType.UniqueConnection,
-            )
-        if hasattr(reader, "handle_serial_ports"):
-            self.ports[list].connect(
-                reader.handle_serial_ports,
-                type=Qt.ConnectionType.UniqueConnection,
-            )
-        if hasattr(reader, "handle_serial_data"):
-            self.data[bytearray].connect(
-                reader.handle_serial_data,
-                type=Qt.ConnectionType.UniqueConnection,
-            )
-        if hasattr(reader, "handle_serial_error"):
-            self.error[Exception].connect(
-                reader.handle_serial_error,
-                type=Qt.ConnectionType.UniqueConnection,
-            )
-
-    def link(self, *can_register: CanRegister):
-        for item in can_register:
-            item.bind_serial_service(self)
+    def register_reader(self, reader: SerialReader) -> None:
+        log.debug(f"Registering reader {reader}")
+        self.com_connect.connect(reader.handle_serial_connect)
+        self.com_disconnect.connect(reader.handle_serial_disconnect)
+        self.ports.connect(reader.handle_serial_ports)
+        self.data.connect(reader.handle_serial_data)
+        self.error.connect(reader.handle_serial_error)
 
     def scan_for_ports(self) -> None:
+        log.debug("Scanning for ports...")
         ports = QSerialPortInfo.availablePorts()
 
         self._debug_ports(ports)
-        log.debug("sending ports...")
 
-        self.ports.emit([p for p in ports if self._port_filter(p)])
+        filtered_ports = self._port_filter(ports)
+        log.debug(f"Sending ports: {filtered_ports}")
+
+        self.ports.emit(filtered_ports)
 
-    def send_command(self, command: CommandInterface) -> None:
-        log.debug(f"sending cmd: {command}")
+    def send_data(self, data: Encodable) -> None:
+        log.debug(f"sending data: {data}")
 
         if not self._com:
             log.debug("com port not connected")
             return
 
-        self._com.write(command.encode())
+        self._com.write(self._transcoder.encode(data))
 
     def close_connection(self) -> None:
         if not self._com:
             return
 
         self.com_disconnect.emit()
 
         try:
             self._com.errorOccurred.disconnect()
             self._com.readyRead.disconnect()
-        except Exception as e:
+        except Exception as e:  # noqa: BLE001
             log.exception(e)
-            pass
 
         if self._com and self._com.isOpen():
             self._com.flush()
             self._com.close()
 
         self._com.deleteLater()
         self._com = None
 
-    def deleteLater(self) -> None:
+    def deleteLater(self) -> None:  # noqa: N802
         self.close_connection()
         super().deleteLater()
 
-    def _on_data(self, *args, **kwargs) -> None:
+    def _on_data(self, *_: object, **__: object) -> None:
         if not self._com:
             return
 
-        read: bytes = self._com.readAll()
-        data = bytearray(read)
-        self._buffer.extend(data)
-
-        if b"\x00" in self._buffer:
-            chunks: list[bytearray]
-            remainder: bytearray
-            *chunks, remainder = self._buffer.split(b"\x00")
-
-            for chunk in chunks:
-                try:
-                    command = self._transcoder.decode_data(chunk)
-                except Exception as e:
-                    log.exception(e)
-                    command = self._transcoder.format_error(e)
+        self._buffer.extend(cast(bytearray, self._com.readAll()))
 
-                self.data.emit(command)
+        chunks, remainder = self._transcoder.process_buffer(self._buffer)
+
+        for chunk in chunks:
+            try:
+                result = self._transcoder.decode(chunk)
+                log.debug(f"received data: {result}")
+                self.data.emit(result)
+            except Exception as e:  # noqa: BLE001
+                log.exception(e)
+                self.error.emit(e)
 
             self._buffer.clear()
-            self._buffer.extend(remainder)
+            if remainder is not None:
+                self._buffer.extend(remainder)
 
     def _on_error(self, error: QSerialPort.SerialPortError | None) -> None:
         exception: SerialError
 
         if error is None or error == QSerialPort.SerialPortError.NoError:
             return
-        elif error == QSerialPort.SerialPortError.OpenError:
+        if error == QSerialPort.SerialPortError.OpenError:
             exception = SerialConnectionError(self._com, error)
         elif error == QSerialPort.SerialPortError.ReadError:
             exception = SerialReadError(self._com, error)
         elif error == QSerialPort.SerialPortError.WriteError:
             exception = SerialWriteError(self._com, error)
         elif error == QSerialPort.SerialPortError.ResourceError:
             exception = SerialDisconnectedError(self._com, error, internal=True)
         else:
             exception = SerialUnknownError(self._com, error)
 
         self.close_connection()
 
-        QTimer.singleShot(3000, self.scan_for_ports)
+        QTimer.singleShot(3 * SECONDS, self.scan_for_ports)
 
         self.error.emit(exception)
         raise exception
 
-    def _port_filter(self, p: QSerialPort) -> bool:
-        filters: list[bool] = [
-            # p.portName().startswith("cu."),
-            # "bluetooth" not in p.portName().lower()
-        ]
-
-        return all(filters)
-
-    def _debug_ports(self, ports: List[QSerialPortInfo]) -> None:
+    def _debug_ports(self, ports: list[QSerialPortInfo]) -> None:
         for p in ports:
             log.debug("-----------------------------")
             log.debug(f"name:         {p.portName()}")
             log.debug(f"manufacturer: {p.manufacturer()}")
             log.debug(f"productId:    {p.productIdentifier()}")
             log.debug(f"serialNumber: {p.serialNumber()}")
             log.debug(f"vendorId:     {p.vendorIdentifier()}")
```

### Comparing `pyside_app_core-0.2.0/src/pyside_app_core/services/serial_service/utils/conversion_utils.py` & `pyside_app_core-0.3.0/src/pyside_app_core/services/serial_service/conversion_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,52 +1,43 @@
 import struct
-from typing import List
 
 from pyside_app_core.constants import (
     DATA_ENCODING_ENDIAN,
-    LIST_DATA_LEN_MAX,
     DATA_STRUCT_ENDIAN,
-    LIST_DATA_LEN_BYTES,
     FLOAT_PRECISION,
+    LIST_DATA_LEN_BYTES,
+    LIST_DATA_LEN_MAX,
 )
 from pyside_app_core.errors.encode_errors import EncodingListError
 from pyside_app_core.types.numeric import FloatPrecision
 
 
-def int_to_bytes(val: int, num_bytes: int, signed: bool) -> bytes:
+def int_to_bytes(val: int, *, num_bytes: int, signed: bool) -> bytes:
     return val.to_bytes(length=num_bytes, byteorder=DATA_ENCODING_ENDIAN, signed=signed)
 
 
-def int_from_bytes(val: bytes, signed: bool) -> int:
+def int_from_bytes(val: bytes, *, signed: bool) -> int:
     return int.from_bytes(bytes=val, byteorder=DATA_ENCODING_ENDIAN, signed=signed)
 
 
-def encode_float_list(
-    floats: List[float], precision: FloatPrecision = FLOAT_PRECISION
-) -> bytearray:
+def encode_float_list(floats: list[float], precision: FloatPrecision = FLOAT_PRECISION) -> bytearray:
     data_len = len(floats)
     if data_len > LIST_DATA_LEN_MAX:
         raise EncodingListError(data_len)
 
     precision_format = "f" if precision == "single" else "d"
 
     encoded = bytearray()
-    encoded.extend(int_to_bytes(data_len, LIST_DATA_LEN_BYTES, False))
-    encoded.extend(
-        struct.pack(f"{DATA_STRUCT_ENDIAN}{data_len}{precision_format}", *floats)
-    )
+    encoded.extend(int_to_bytes(data_len, num_bytes=LIST_DATA_LEN_BYTES, signed=False))
+    encoded.extend(struct.pack(f"{DATA_STRUCT_ENDIAN}{data_len}{precision_format}", *floats))
 
     return encoded
 
 
-def decode_float_list(
-    raw_data: bytes, precision: FloatPrecision = FLOAT_PRECISION
-) -> List[float]:
+def decode_float_list(raw_data: bytes, precision: FloatPrecision = FLOAT_PRECISION) -> list[float]:
     len_bytes = raw_data[:LIST_DATA_LEN_BYTES]
     data_bytes = raw_data[LIST_DATA_LEN_BYTES:]
 
     precision_format = "f" if precision == "single" else "d"
 
-    data_len = int_from_bytes(len_bytes, False)
-    return list(
-        struct.unpack(f"{DATA_STRUCT_ENDIAN}{data_len}{precision_format}", data_bytes)
-    )
+    data_len = int_from_bytes(len_bytes, signed=False)
+    return list(struct.unpack(f"{DATA_STRUCT_ENDIAN}{data_len}{precision_format}", data_bytes))
```

### Comparing `pyside_app_core-0.2.0/src/pyside_app_core/services/serial_service/utils/float_map.py` & `pyside_app_core-0.3.0/src/pyside_app_core/services/serial_service/float_map.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,58 +1,61 @@
 import struct
+from collections.abc import Iterator, Mapping
 from decimal import Decimal
-from typing import Any, Iterator, Mapping, Self, TypeVar
+from typing import Any, TypeVar
 
-from pyside_app_core.utils import compare
 from pyside_app_core.constants import (
     DATA_STRUCT_ENDIAN,
     FLOAT_PRECISION,
     STRUCT_FLOAT_FMT,
 )
-from pyside_app_core.services.serial_service.utils import conversion_utils
+from pyside_app_core.services.serial_service import conversion_utils
+from pyside_app_core.utils import compare
 
 K = TypeVar("K", bound=int)
 
+_TWO_BYTE_LEN = 65535
+
 
 class FloatMap(Mapping[K, float]):
     _count_fmt = "H"  # unsigned short, 2 bytes
     _key_fmt = "H"  # unsigned short, 2 bytes
 
     def __init__(self, data: Mapping[K, float]):
         self._data = data
 
         if not data:
             raise ValueError(f"can't create an empty {self.__class__.__name__}")
 
-        if len(data) > 65535:
+        if len(data) > _TWO_BYTE_LEN:
             raise ValueError("data has too many values, must fit in 2 bytes")
 
-        for k in data.keys():
-            if k > 65535:
+        for k in data:
+            if k > _TWO_BYTE_LEN:
                 raise ValueError(f'key: "{k}" does not fit in 2 bytes')
 
             if k < 0:
                 raise ValueError(f'key: "{k}" is not a positive number')
 
     def __getitem__(self, k: K) -> float:
         return self._data[k]
 
     def __len__(self) -> int:
         return len(self._data)
 
     def __iter__(self) -> Iterator[K]:
         return iter(self._data)
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return self._data.__repr__()
 
-    def __str__(self):
+    def __str__(self) -> str:
         return self._data.__str__()
 
-    def __eq__(self, other: Self) -> bool:  # type: ignore[override]
+    def __eq__(self, other: "FloatMap[K]") -> bool:  # type: ignore[override]
         val_eq: list[bool] = []
         for k, v in self.items():
             other_v = other.get(k)
             if other_v:
                 val_eq.append(compare.float_approx(v, other_v))
 
         return all(
@@ -97,25 +100,23 @@
         for key, value in self._data.items():
             flattened_data.extend([key, value])
 
         raw = struct.pack(self.pack_format(count), count, *flattened_data)
         return bytearray(raw)
 
     @classmethod
-    def unpack(cls, raw_data: bytes) -> Self:
+    def unpack(cls, raw_data: bytes) -> "FloatMap[K]":
         count_bytes = 2
         raw_pair_count = raw_data[:count_bytes]
         raw_key_val = raw_data[count_bytes:]
 
         pair_count = conversion_utils.int_from_bytes(raw_pair_count, signed=False)
         fmt_chars = [cls._key_fmt, STRUCT_FLOAT_FMT] * pair_count
 
-        flat_pairs = struct.unpack(
-            f"{DATA_STRUCT_ENDIAN}{''.join(fmt_chars)}", raw_key_val
-        )
+        flat_pairs = struct.unpack(f"{DATA_STRUCT_ENDIAN}{''.join(fmt_chars)}", raw_key_val)
 
         data = {}
         iterable = iter(flat_pairs)
 
         for key in iterable:
             val = next(iterable)
             if FLOAT_PRECISION == "single":
```

### Comparing `pyside_app_core-0.2.0/src/pyside_app_core/theme_generator/generate_resources.py` & `pyside_app_core-0.3.0/src/pyside_app_core/resource_generator/generate_resources.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,85 +1,105 @@
 import subprocess
 import tempfile
 from pathlib import Path
-from typing import List, Literal, Type
+from typing import Literal
 
-from jinja2 import ChoiceLoader, Environment, FileSystemLoader, PackageLoader
+from jinja2 import Environment, PackageLoader
 
-from pyside_app_core.theme_generator.standard_resources import STANDARD_RESOURCES
-from pyside_app_core.theme_generator.style_types import QtResourceGroup
-from pyside_app_core.style.theme import DEFAULT_THEME, QssTheme
+from pyside_app_core.resource_generator.resource_types import (
+    QtResourceFile,
+    QtResourceGroup,
+)
 
+_std_resource_root = Path(__file__).parent.parent / "resources" / "core"
 
-def _compose_template_environment(*extra_template_files: Path) -> Environment:
-    loaders = [PackageLoader("pyside_app_core.resources")]
 
-    if extra_template_files:
-        dirs = list(set([str(p.parent) for p in extra_template_files]))
-        loaders.append(FileSystemLoader(dirs))
-
-    return Environment(loader=ChoiceLoader(loaders), autoescape=False)
-
-
-def _compile_qss_template(theme: QssTheme, qss_extra: List[Path] | None = None) -> str:
-    qss_extra = qss_extra or []
-    env = _compose_template_environment(*qss_extra)
-    qss_template = env.get_template("style.qss.jinja2")
-    return qss_template.render(theme=theme, qss_extra=[q.name for q in qss_extra])
-
-
-def _compile_qrc_template(resources: List[QtResourceGroup]) -> str:
-    env = _compose_template_environment()
+def _compile_qrc_template(resources: list[QtResourceGroup]) -> str:
+    env = Environment(loader=PackageLoader("pyside_app_core.resources"), autoescape=True)
     qrc_template = env.get_template("resources.qrc.jinja2")
     return qrc_template.render(qresources=resources)
 
 
 def _write_file(target: Path, data: str) -> Path:
     with open(target, "w") as f:
         f.write(data)
 
     return target
 
 
 ResourceFormat = Literal["python", "binary"]
 
 
+def _build_resource_groups(root_paths: list[Path]) -> list[QtResourceGroup]:
+    groups: list[QtResourceGroup] = []
+    root_prefixes: list[str] = []
+
+    for root_path in root_paths:
+        if not root_path.is_dir():
+            continue
+
+        prefix = root_path.name
+        if prefix in root_prefixes:
+            raise ValueError(f"Root path {root_path} has duplicate prefix {prefix}")
+
+        root_prefixes.append(prefix)
+
+        files: list[QtResourceFile] = []
+
+        for item in root_path.glob("**/*"):
+            if item.is_dir():
+                continue
+            files.append(
+                QtResourceFile(
+                    str(item),
+                    item.relative_to(root_path).as_posix(),
+                )
+            )
+
+        groups.append(
+            QtResourceGroup(
+                prefix,
+                None,
+                files,
+            )
+        )
+
+    return groups
+
+
 def compile_qrc_to_resources(
     target_dir: Path,
-    qss_theme: QssTheme | Type[QssTheme],
     rcc_format: ResourceFormat = "binary",
-    qss_template_extra: List[Path] | None = None,
-    resources_extra: List[QtResourceGroup] | None = None,
+    additional_resource_roots: list[Path] | None = None,
+    *,
+    debug: bool = False,
 ) -> Path:
-    if not isinstance(qss_theme, QssTheme):
-        qss_theme = qss_theme()
-
     with tempfile.TemporaryDirectory() as tempdir:
-        tempdir = Path(tempdir)
-
-        _write_file(
-            tempdir / "style.qss",
-            _compile_qss_template(qss_theme or DEFAULT_THEME, qss_template_extra),
-        )
+        temp_path = Path(tempdir)
 
-        resources = STANDARD_RESOURCES
-        if resources_extra:
-            resources.extend(resources_extra)
-
-        qrc_file = _write_file(
-            tempdir / "resources.qrc", _compile_qrc_template(resources)
+        resources = _build_resource_groups(
+            [
+                _std_resource_root,
+                *(additional_resource_roots or []),
+            ]
         )
 
-        file_name = "resources.py"
+        qrc_file = _write_file(temp_path / "resources.qrc", _compile_qrc_template(resources))
 
         rcc_args = []
+
         if rcc_format == "binary":
             file_name = "resources.rcc"
             rcc_args.append("--binary")
+        else:
+            file_name = "resources.py"
 
         file_target = target_dir / file_name
 
-        subprocess.check_call(
-            ["pyside6-rcc", *rcc_args, "-o", str(file_target), str(qrc_file)]
-        )
+        subprocess.check_call(["pyside6-rcc", *rcc_args, "-o", str(file_target), str(qrc_file)])
+
+        if debug:
+            print("-" * 80)
+            print(qrc_file.read_text())
+            print("-" * 80)
 
     return file_target
```

