# Comparing `tmp/quite6-1.0.3.tar.gz` & `tmp/quite6-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quite6-1.0.3.tar", last modified: Fri May 17 03:40:26 2024, max compression
+gzip compressed data, was "quite6-1.0.4.tar", last modified: Sat May 25 14:32:00 2024, max compression
```

## Comparing `quite6-1.0.3.tar` & `quite6-1.0.4.tar`

### file list

```diff
@@ -1,89 +1,90 @@
-drwxr-xr-x   0 wangcong   (502) staff       (20)        0 2024-05-17 03:40:26.445895 quite6-1.0.3/
--rw-r--r--   0 wangcong   (502) staff       (20)     1074 2024-05-14 10:15:26.000000 quite6-1.0.3/LICENSE
--rw-r--r--   0 wangcong   (502) staff       (20)      104 2024-05-14 10:15:26.000000 quite6-1.0.3/MANIFEST.in
--rw-r--r--   0 wangcong   (502) staff       (20)     3749 2024-05-17 03:40:26.445516 quite6-1.0.3/PKG-INFO
--rw-r--r--   0 wangcong   (502) staff       (20)     2936 2024-05-14 10:15:26.000000 quite6-1.0.3/README.rst
--rw-r--r--   0 wangcong   (502) staff       (20)        6 2024-05-17 03:39:17.000000 quite6-1.0.3/RELEASE-VERSION
-drwxr-xr-x   0 wangcong   (502) staff       (20)        0 2024-05-17 03:40:26.351504 quite6-1.0.3/quite6/
--rw-r--r--   0 wangcong   (502) staff       (20)      272 2024-05-14 11:46:55.000000 quite6-1.0.3/quite6/__init__.py
-drwxr-xr-x   0 wangcong   (502) staff       (20)        0 2024-05-17 03:40:26.359221 quite6-1.0.3/quite6/controller/
--rw-r--r--   0 wangcong   (502) staff       (20)      211 2024-05-13 08:52:57.000000 quite6-1.0.3/quite6/controller/__init__.py
--rw-r--r--   0 wangcong   (502) staff       (20)      606 2024-05-14 14:24:17.000000 quite6-1.0.3/quite6/controller/dialog_ui_controller.py
--rw-r--r--   0 wangcong   (502) staff       (20)     2634 2024-05-14 14:24:17.000000 quite6-1.0.3/quite6/controller/file_dialog_controller.py
--rw-r--r--   0 wangcong   (502) staff       (20)     1616 2024-05-14 14:24:17.000000 quite6-1.0.3/quite6/controller/widget_controller.py
--rw-r--r--   0 wangcong   (502) staff       (20)     3514 2024-05-14 03:41:05.000000 quite6-1.0.3/quite6/controller/widget_ui_controller.py
-drwxr-xr-x   0 wangcong   (502) staff       (20)        0 2024-05-17 03:40:26.362341 quite6-1.0.3/quite6/core/
--rw-r--r--   0 wangcong   (502) staff       (20)      203 2024-05-14 10:47:48.000000 quite6-1.0.3/quite6/core/__init__.py
--rw-r--r--   0 wangcong   (502) staff       (20)     1326 2024-05-14 10:43:54.000000 quite6-1.0.3/quite6/core/event_loop.py
--rw-r--r--   0 wangcong   (502) staff       (20)      281 2024-05-14 10:43:54.000000 quite6-1.0.3/quite6/core/timer.py
--rw-r--r--   0 wangcong   (502) staff       (20)     3712 2024-05-14 15:04:01.000000 quite6-1.0.3/quite6/deferred_function.py
-drwxr-xr-x   0 wangcong   (502) staff       (20)        0 2024-05-17 03:40:26.365455 quite6-1.0.3/quite6/gui/
--rw-r--r--   0 wangcong   (502) staff       (20)     1118 2024-05-14 11:49:59.000000 quite6-1.0.3/quite6/gui/__init__.py
-drwxr-xr-x   0 wangcong   (502) staff       (20)        0 2024-05-17 03:40:26.378787 quite6-1.0.3/quite6/gui/interfaces/
--rw-r--r--   0 wangcong   (502) staff       (20)      554 2024-05-13 08:52:57.000000 quite6-1.0.3/quite6/gui/interfaces/__init__.py
-drwxr-xr-x   0 wangcong   (502) staff       (20)        0 2024-05-17 03:40:26.384586 quite6-1.0.3/quite6/gui/interfaces/ability_interfaces/
--rw-r--r--   0 wangcong   (502) staff       (20)      120 2024-05-13 08:52:57.000000 quite6-1.0.3/quite6/gui/interfaces/ability_interfaces/__init__.py
--rw-r--r--   0 wangcong   (502) staff       (20)      188 2024-05-13 08:52:57.000000 quite6-1.0.3/quite6/gui/interfaces/ability_interfaces/class_exec_interface.py
--rw-r--r--   0 wangcong   (502) staff       (20)     1092 2024-05-14 10:57:04.000000 quite6-1.0.3/quite6/gui/interfaces/ability_interfaces/container_ability_interface.py
--rw-r--r--   0 wangcong   (502) staff       (20)      539 2024-05-14 03:20:46.000000 quite6-1.0.3/quite6/gui/interfaces/base_interface.py
--rw-r--r--   0 wangcong   (502) staff       (20)      303 2024-05-13 08:52:57.000000 quite6-1.0.3/quite6/gui/interfaces/changed_signal_interface.py
--rw-r--r--   0 wangcong   (502) staff       (20)      470 2024-05-14 08:19:12.000000 quite6-1.0.3/quite6/gui/interfaces/closed_signal_interface.py
--rw-r--r--   0 wangcong   (502) staff       (20)      307 2024-05-14 10:57:04.000000 quite6-1.0.3/quite6/gui/interfaces/excited_signal_interface.py
--rw-r--r--   0 wangcong   (502) staff       (20)      199 2024-05-14 10:57:04.000000 quite6-1.0.3/quite6/gui/interfaces/focus_in_signal_interface.py
--rw-r--r--   0 wangcong   (502) staff       (20)      201 2024-05-14 10:57:04.000000 quite6-1.0.3/quite6/gui/interfaces/focus_out_signal_interface.py
--rw-r--r--   0 wangcong   (502) staff       (20)      322 2024-05-14 10:57:04.000000 quite6-1.0.3/quite6/gui/interfaces/row_changed_signal_interface.py
--rw-r--r--   0 wangcong   (502) staff       (20)      298 2024-05-13 08:52:57.000000 quite6-1.0.3/quite6/gui/interfaces/showed_signal_interface.py
-drwxr-xr-x   0 wangcong   (502) staff       (20)        0 2024-05-17 03:40:26.387281 quite6-1.0.3/quite6/gui/layouts/
--rw-r--r--   0 wangcong   (502) staff       (20)       40 2024-05-13 08:52:57.000000 quite6-1.0.3/quite6/gui/layouts/__init__.py
--rw-r--r--   0 wangcong   (502) staff       (20)     2712 2024-05-14 14:37:29.000000 quite6-1.0.3/quite6/gui/layouts/square_layout.py
-drwxr-xr-x   0 wangcong   (502) staff       (20)        0 2024-05-17 03:40:26.396098 quite6-1.0.3/quite6/gui/paint/
--rw-r--r--   0 wangcong   (502) staff       (20)      129 2024-05-13 08:52:57.000000 quite6-1.0.3/quite6/gui/paint/__init__.py
--rw-r--r--   0 wangcong   (502) staff       (20)     5084 2024-05-17 03:34:53.000000 quite6-1.0.3/quite6/gui/paint/painter.py
--rw-r--r--   0 wangcong   (502) staff       (20)      502 2024-05-14 11:03:11.000000 quite6-1.0.3/quite6/gui/paint/pen.py
--rw-r--r--   0 wangcong   (502) staff       (20)      904 2024-05-14 11:03:11.000000 quite6-1.0.3/quite6/gui/paint/point.py
--rw-r--r--   0 wangcong   (502) staff       (20)      280 2024-05-14 11:03:11.000000 quite6-1.0.3/quite6/gui/paint/scaling.py
--rw-r--r--   0 wangcong   (502) staff       (20)     1471 2024-05-14 11:03:11.000000 quite6-1.0.3/quite6/gui/paint/size.py
--rw-r--r--   0 wangcong   (502) staff       (20)      398 2024-05-14 10:17:44.000000 quite6-1.0.3/quite6/gui/qt_gui.py
--rw-r--r--   0 wangcong   (502) staff       (20)      311 2024-05-14 10:15:26.000000 quite6-1.0.3/quite6/gui/ui_extension.py
-drwxr-xr-x   0 wangcong   (502) staff       (20)        0 2024-05-17 03:40:26.435876 quite6-1.0.3/quite6/gui/widgets/
--rw-r--r--   0 wangcong   (502) staff       (20)      798 2024-05-14 11:10:25.000000 quite6-1.0.3/quite6/gui/widgets/__init__.py
--rw-r--r--   0 wangcong   (502) staff       (20)      383 2024-05-14 11:32:31.000000 quite6-1.0.3/quite6/gui/widgets/action.py
--rw-r--r--   0 wangcong   (502) staff       (20)     2454 2024-05-14 11:32:31.000000 quite6-1.0.3/quite6/gui/widgets/combo_box.py
--rw-r--r--   0 wangcong   (502) staff       (20)      926 2024-05-14 11:32:31.000000 quite6-1.0.3/quite6/gui/widgets/date_edit.py
--rw-r--r--   0 wangcong   (502) staff       (20)      683 2024-05-14 11:32:31.000000 quite6-1.0.3/quite6/gui/widgets/date_time_edit.py
--rw-r--r--   0 wangcong   (502) staff       (20)      780 2024-05-14 11:51:50.000000 quite6-1.0.3/quite6/gui/widgets/dialog.py
--rw-r--r--   0 wangcong   (502) staff       (20)      195 2024-05-14 11:32:31.000000 quite6-1.0.3/quite6/gui/widgets/dock_widget.py
--rw-r--r--   0 wangcong   (502) staff       (20)      721 2024-05-14 11:32:31.000000 quite6-1.0.3/quite6/gui/widgets/double_spin_box.py
--rw-r--r--   0 wangcong   (502) staff       (20)      189 2024-05-14 11:32:31.000000 quite6-1.0.3/quite6/gui/widgets/group_box.py
--rw-r--r--   0 wangcong   (502) staff       (20)     1627 2024-05-14 11:32:31.000000 quite6-1.0.3/quite6/gui/widgets/input_dialog.py
--rw-r--r--   0 wangcong   (502) staff       (20)      736 2024-05-14 14:37:29.000000 quite6-1.0.3/quite6/gui/widgets/label.py
--rw-r--r--   0 wangcong   (502) staff       (20)      183 2024-05-14 11:32:31.000000 quite6-1.0.3/quite6/gui/widgets/layout.py
--rw-r--r--   0 wangcong   (502) staff       (20)     1004 2024-05-14 11:32:31.000000 quite6-1.0.3/quite6/gui/widgets/line_edit.py
--rw-r--r--   0 wangcong   (502) staff       (20)     2347 2024-05-14 11:32:31.000000 quite6-1.0.3/quite6/gui/widgets/list_widget.py
--rw-r--r--   0 wangcong   (502) staff       (20)      697 2024-05-14 11:32:31.000000 quite6-1.0.3/quite6/gui/widgets/main_window.py
--rw-r--r--   0 wangcong   (502) staff       (20)     2904 2024-05-14 11:32:31.000000 quite6-1.0.3/quite6/gui/widgets/plot_widget.py
--rw-r--r--   0 wangcong   (502) staff       (20)      676 2024-05-14 11:32:31.000000 quite6-1.0.3/quite6/gui/widgets/push_button.py
--rw-r--r--   0 wangcong   (502) staff       (20)      680 2024-05-14 11:32:31.000000 quite6-1.0.3/quite6/gui/widgets/radio_button.py
--rw-r--r--   0 wangcong   (502) staff       (20)      582 2024-05-14 11:32:31.000000 quite6-1.0.3/quite6/gui/widgets/shortcut.py
--rw-r--r--   0 wangcong   (502) staff       (20)      693 2024-05-14 11:54:28.000000 quite6-1.0.3/quite6/gui/widgets/spin_box.py
--rw-r--r--   0 wangcong   (502) staff       (20)     6529 2024-05-14 11:32:31.000000 quite6-1.0.3/quite6/gui/widgets/table_view.py
--rw-r--r--   0 wangcong   (502) staff       (20)     9397 2024-05-14 14:37:29.000000 quite6-1.0.3/quite6/gui/widgets/table_widget.py
--rw-r--r--   0 wangcong   (502) staff       (20)      720 2024-05-14 11:37:12.000000 quite6-1.0.3/quite6/gui/widgets/text_edit.py
--rw-r--r--   0 wangcong   (502) staff       (20)      926 2024-05-14 11:37:12.000000 quite6-1.0.3/quite6/gui/widgets/time_edit.py
--rw-r--r--   0 wangcong   (502) staff       (20)     1326 2024-05-14 14:37:29.000000 quite6-1.0.3/quite6/gui/widgets/widget.py
-drwxr-xr-x   0 wangcong   (502) staff       (20)        0 2024-05-17 03:40:26.442957 quite6-1.0.3/quite6/tools/
--rw-r--r--   0 wangcong   (502) staff       (20)      110 2024-05-14 11:51:08.000000 quite6-1.0.3/quite6/tools/__init__.py
--rw-r--r--   0 wangcong   (502) staff       (20)     1207 2024-05-15 06:35:06.000000 quite6-1.0.3/quite6/tools/load_qrc.py
--rw-r--r--   0 wangcong   (502) staff       (20)     2461 2024-05-14 15:28:56.000000 quite6-1.0.3/quite6/tools/load_ui.py
--rw-r--r--   0 wangcong   (502) staff       (20)      315 2024-05-14 14:37:29.000000 quite6-1.0.3/quite6/tools/process.py
-drwxr-xr-x   0 wangcong   (502) staff       (20)        0 2024-05-17 03:40:26.444390 quite6-1.0.3/quite6.egg-info/
--rw-r--r--   0 wangcong   (502) staff       (20)     3749 2024-05-17 03:40:26.000000 quite6-1.0.3/quite6.egg-info/PKG-INFO
--rw-r--r--   0 wangcong   (502) staff       (20)     2394 2024-05-17 03:40:26.000000 quite6-1.0.3/quite6.egg-info/SOURCES.txt
--rw-r--r--   0 wangcong   (502) staff       (20)        1 2024-05-17 03:40:26.000000 quite6-1.0.3/quite6.egg-info/dependency_links.txt
--rw-r--r--   0 wangcong   (502) staff       (20)       41 2024-05-17 03:40:26.000000 quite6-1.0.3/quite6.egg-info/requires.txt
--rw-r--r--   0 wangcong   (502) staff       (20)        7 2024-05-17 03:40:26.000000 quite6-1.0.3/quite6.egg-info/top_level.txt
--rw-r--r--   0 wangcong   (502) staff       (20)     2557 2024-05-14 10:15:26.000000 quite6-1.0.3/readme.md
--rw-r--r--   0 wangcong   (502) staff       (20)       40 2024-05-16 14:15:45.000000 quite6-1.0.3/requirements.txt
--rw-r--r--   0 wangcong   (502) staff       (20)      154 2024-05-17 03:40:26.447990 quite6-1.0.3/setup.cfg
--rw-r--r--   0 wangcong   (502) staff       (20)     1633 2024-05-14 10:15:26.000000 quite6-1.0.3/setup.py
--rw-r--r--   0 wangcong   (502) staff       (20)     2173 2024-05-14 10:15:26.000000 quite6-1.0.3/version.py
+drwxr-xr-x   0 wangcong   (502) staff       (20)        0 2024-05-25 14:32:00.205851 quite6-1.0.4/
+-rw-r--r--   0 wangcong   (502) staff       (20)     1074 2024-05-14 10:15:26.000000 quite6-1.0.4/LICENSE
+-rw-r--r--   0 wangcong   (502) staff       (20)      104 2024-05-14 10:15:26.000000 quite6-1.0.4/MANIFEST.in
+-rw-r--r--   0 wangcong   (502) staff       (20)     3749 2024-05-25 14:32:00.205266 quite6-1.0.4/PKG-INFO
+-rw-r--r--   0 wangcong   (502) staff       (20)     2936 2024-05-14 10:15:26.000000 quite6-1.0.4/README.rst
+-rw-r--r--   0 wangcong   (502) staff       (20)        6 2024-05-25 14:31:52.000000 quite6-1.0.4/RELEASE-VERSION
+drwxr-xr-x   0 wangcong   (502) staff       (20)        0 2024-05-25 14:32:00.107096 quite6-1.0.4/quite6/
+-rw-r--r--   0 wangcong   (502) staff       (20)      272 2024-05-14 11:46:55.000000 quite6-1.0.4/quite6/__init__.py
+drwxr-xr-x   0 wangcong   (502) staff       (20)        0 2024-05-25 14:32:00.120574 quite6-1.0.4/quite6/controller/
+-rw-r--r--   0 wangcong   (502) staff       (20)      211 2024-05-13 08:52:57.000000 quite6-1.0.4/quite6/controller/__init__.py
+-rw-r--r--   0 wangcong   (502) staff       (20)      606 2024-05-14 14:24:17.000000 quite6-1.0.4/quite6/controller/dialog_ui_controller.py
+-rw-r--r--   0 wangcong   (502) staff       (20)     2634 2024-05-14 14:24:17.000000 quite6-1.0.4/quite6/controller/file_dialog_controller.py
+-rw-r--r--   0 wangcong   (502) staff       (20)     1616 2024-05-14 14:24:17.000000 quite6-1.0.4/quite6/controller/widget_controller.py
+-rw-r--r--   0 wangcong   (502) staff       (20)     3514 2024-05-14 03:41:05.000000 quite6-1.0.4/quite6/controller/widget_ui_controller.py
+drwxr-xr-x   0 wangcong   (502) staff       (20)        0 2024-05-25 14:32:00.125558 quite6-1.0.4/quite6/core/
+-rw-r--r--   0 wangcong   (502) staff       (20)      203 2024-05-14 10:47:48.000000 quite6-1.0.4/quite6/core/__init__.py
+-rw-r--r--   0 wangcong   (502) staff       (20)     1326 2024-05-14 10:43:54.000000 quite6-1.0.4/quite6/core/event_loop.py
+-rw-r--r--   0 wangcong   (502) staff       (20)      281 2024-05-14 10:43:54.000000 quite6-1.0.4/quite6/core/timer.py
+-rw-r--r--   0 wangcong   (502) staff       (20)     3712 2024-05-14 15:04:01.000000 quite6-1.0.4/quite6/deferred_function.py
+drwxr-xr-x   0 wangcong   (502) staff       (20)        0 2024-05-25 14:32:00.129339 quite6-1.0.4/quite6/gui/
+-rw-r--r--   0 wangcong   (502) staff       (20)     1129 2024-05-25 13:12:30.000000 quite6-1.0.4/quite6/gui/__init__.py
+drwxr-xr-x   0 wangcong   (502) staff       (20)        0 2024-05-25 14:32:00.139604 quite6-1.0.4/quite6/gui/interfaces/
+-rw-r--r--   0 wangcong   (502) staff       (20)      554 2024-05-13 08:52:57.000000 quite6-1.0.4/quite6/gui/interfaces/__init__.py
+drwxr-xr-x   0 wangcong   (502) staff       (20)        0 2024-05-25 14:32:00.142570 quite6-1.0.4/quite6/gui/interfaces/ability_interfaces/
+-rw-r--r--   0 wangcong   (502) staff       (20)      120 2024-05-13 08:52:57.000000 quite6-1.0.4/quite6/gui/interfaces/ability_interfaces/__init__.py
+-rw-r--r--   0 wangcong   (502) staff       (20)      188 2024-05-13 08:52:57.000000 quite6-1.0.4/quite6/gui/interfaces/ability_interfaces/class_exec_interface.py
+-rw-r--r--   0 wangcong   (502) staff       (20)     1092 2024-05-14 10:57:04.000000 quite6-1.0.4/quite6/gui/interfaces/ability_interfaces/container_ability_interface.py
+-rw-r--r--   0 wangcong   (502) staff       (20)      539 2024-05-14 03:20:46.000000 quite6-1.0.4/quite6/gui/interfaces/base_interface.py
+-rw-r--r--   0 wangcong   (502) staff       (20)      303 2024-05-13 08:52:57.000000 quite6-1.0.4/quite6/gui/interfaces/changed_signal_interface.py
+-rw-r--r--   0 wangcong   (502) staff       (20)      470 2024-05-14 08:19:12.000000 quite6-1.0.4/quite6/gui/interfaces/closed_signal_interface.py
+-rw-r--r--   0 wangcong   (502) staff       (20)      307 2024-05-14 10:57:04.000000 quite6-1.0.4/quite6/gui/interfaces/excited_signal_interface.py
+-rw-r--r--   0 wangcong   (502) staff       (20)      199 2024-05-14 10:57:04.000000 quite6-1.0.4/quite6/gui/interfaces/focus_in_signal_interface.py
+-rw-r--r--   0 wangcong   (502) staff       (20)      201 2024-05-14 10:57:04.000000 quite6-1.0.4/quite6/gui/interfaces/focus_out_signal_interface.py
+-rw-r--r--   0 wangcong   (502) staff       (20)      322 2024-05-14 10:57:04.000000 quite6-1.0.4/quite6/gui/interfaces/row_changed_signal_interface.py
+-rw-r--r--   0 wangcong   (502) staff       (20)      298 2024-05-13 08:52:57.000000 quite6-1.0.4/quite6/gui/interfaces/showed_signal_interface.py
+drwxr-xr-x   0 wangcong   (502) staff       (20)        0 2024-05-25 14:32:00.147502 quite6-1.0.4/quite6/gui/layouts/
+-rw-r--r--   0 wangcong   (502) staff       (20)       40 2024-05-13 08:52:57.000000 quite6-1.0.4/quite6/gui/layouts/__init__.py
+-rw-r--r--   0 wangcong   (502) staff       (20)     2712 2024-05-14 14:37:29.000000 quite6-1.0.4/quite6/gui/layouts/square_layout.py
+drwxr-xr-x   0 wangcong   (502) staff       (20)        0 2024-05-25 14:32:00.155799 quite6-1.0.4/quite6/gui/paint/
+-rw-r--r--   0 wangcong   (502) staff       (20)      129 2024-05-13 08:52:57.000000 quite6-1.0.4/quite6/gui/paint/__init__.py
+-rw-r--r--   0 wangcong   (502) staff       (20)     5084 2024-05-17 03:34:53.000000 quite6-1.0.4/quite6/gui/paint/painter.py
+-rw-r--r--   0 wangcong   (502) staff       (20)      502 2024-05-14 11:03:11.000000 quite6-1.0.4/quite6/gui/paint/pen.py
+-rw-r--r--   0 wangcong   (502) staff       (20)      904 2024-05-14 11:03:11.000000 quite6-1.0.4/quite6/gui/paint/point.py
+-rw-r--r--   0 wangcong   (502) staff       (20)      280 2024-05-14 11:03:11.000000 quite6-1.0.4/quite6/gui/paint/scaling.py
+-rw-r--r--   0 wangcong   (502) staff       (20)     1471 2024-05-14 11:03:11.000000 quite6-1.0.4/quite6/gui/paint/size.py
+-rw-r--r--   0 wangcong   (502) staff       (20)      398 2024-05-14 10:17:44.000000 quite6-1.0.4/quite6/gui/qt_gui.py
+-rw-r--r--   0 wangcong   (502) staff       (20)      311 2024-05-14 10:15:26.000000 quite6-1.0.4/quite6/gui/ui_extension.py
+drwxr-xr-x   0 wangcong   (502) staff       (20)        0 2024-05-25 14:32:00.197497 quite6-1.0.4/quite6/gui/widgets/
+-rw-r--r--   0 wangcong   (502) staff       (20)      832 2024-05-25 13:12:30.000000 quite6-1.0.4/quite6/gui/widgets/__init__.py
+-rw-r--r--   0 wangcong   (502) staff       (20)      383 2024-05-14 11:32:31.000000 quite6-1.0.4/quite6/gui/widgets/action.py
+-rw-r--r--   0 wangcong   (502) staff       (20)     2454 2024-05-14 11:32:31.000000 quite6-1.0.4/quite6/gui/widgets/combo_box.py
+-rw-r--r--   0 wangcong   (502) staff       (20)      926 2024-05-14 11:32:31.000000 quite6-1.0.4/quite6/gui/widgets/date_edit.py
+-rw-r--r--   0 wangcong   (502) staff       (20)      683 2024-05-14 11:32:31.000000 quite6-1.0.4/quite6/gui/widgets/date_time_edit.py
+-rw-r--r--   0 wangcong   (502) staff       (20)      780 2024-05-14 11:51:50.000000 quite6-1.0.4/quite6/gui/widgets/dialog.py
+-rw-r--r--   0 wangcong   (502) staff       (20)      195 2024-05-14 11:32:31.000000 quite6-1.0.4/quite6/gui/widgets/dock_widget.py
+-rw-r--r--   0 wangcong   (502) staff       (20)      721 2024-05-14 11:32:31.000000 quite6-1.0.4/quite6/gui/widgets/double_spin_box.py
+-rw-r--r--   0 wangcong   (502) staff       (20)      189 2024-05-14 11:32:31.000000 quite6-1.0.4/quite6/gui/widgets/group_box.py
+-rw-r--r--   0 wangcong   (502) staff       (20)     1627 2024-05-14 11:32:31.000000 quite6-1.0.4/quite6/gui/widgets/input_dialog.py
+-rw-r--r--   0 wangcong   (502) staff       (20)      736 2024-05-14 14:37:29.000000 quite6-1.0.4/quite6/gui/widgets/label.py
+-rw-r--r--   0 wangcong   (502) staff       (20)      183 2024-05-14 11:32:31.000000 quite6-1.0.4/quite6/gui/widgets/layout.py
+-rw-r--r--   0 wangcong   (502) staff       (20)     1004 2024-05-14 11:32:31.000000 quite6-1.0.4/quite6/gui/widgets/line_edit.py
+-rw-r--r--   0 wangcong   (502) staff       (20)     2347 2024-05-14 11:32:31.000000 quite6-1.0.4/quite6/gui/widgets/list_widget.py
+-rw-r--r--   0 wangcong   (502) staff       (20)      697 2024-05-14 11:32:31.000000 quite6-1.0.4/quite6/gui/widgets/main_window.py
+-rw-r--r--   0 wangcong   (502) staff       (20)     2904 2024-05-14 11:32:31.000000 quite6-1.0.4/quite6/gui/widgets/plot_widget.py
+-rw-r--r--   0 wangcong   (502) staff       (20)      676 2024-05-14 11:32:31.000000 quite6-1.0.4/quite6/gui/widgets/push_button.py
+-rw-r--r--   0 wangcong   (502) staff       (20)      680 2024-05-14 11:32:31.000000 quite6-1.0.4/quite6/gui/widgets/radio_button.py
+-rw-r--r--   0 wangcong   (502) staff       (20)      582 2024-05-14 11:32:31.000000 quite6-1.0.4/quite6/gui/widgets/shortcut.py
+-rw-r--r--   0 wangcong   (502) staff       (20)      693 2024-05-14 11:54:28.000000 quite6-1.0.4/quite6/gui/widgets/spin_box.py
+-rw-r--r--   0 wangcong   (502) staff       (20)     1658 2024-05-25 14:20:09.000000 quite6-1.0.4/quite6/gui/widgets/tab_widget.py
+-rw-r--r--   0 wangcong   (502) staff       (20)     6529 2024-05-14 11:32:31.000000 quite6-1.0.4/quite6/gui/widgets/table_view.py
+-rw-r--r--   0 wangcong   (502) staff       (20)     9397 2024-05-14 14:37:29.000000 quite6-1.0.4/quite6/gui/widgets/table_widget.py
+-rw-r--r--   0 wangcong   (502) staff       (20)      720 2024-05-14 11:37:12.000000 quite6-1.0.4/quite6/gui/widgets/text_edit.py
+-rw-r--r--   0 wangcong   (502) staff       (20)      926 2024-05-14 11:37:12.000000 quite6-1.0.4/quite6/gui/widgets/time_edit.py
+-rw-r--r--   0 wangcong   (502) staff       (20)     1326 2024-05-14 14:37:29.000000 quite6-1.0.4/quite6/gui/widgets/widget.py
+drwxr-xr-x   0 wangcong   (502) staff       (20)        0 2024-05-25 14:32:00.202538 quite6-1.0.4/quite6/tools/
+-rw-r--r--   0 wangcong   (502) staff       (20)      110 2024-05-14 11:51:08.000000 quite6-1.0.4/quite6/tools/__init__.py
+-rw-r--r--   0 wangcong   (502) staff       (20)     1207 2024-05-15 06:35:06.000000 quite6-1.0.4/quite6/tools/load_qrc.py
+-rw-r--r--   0 wangcong   (502) staff       (20)     2461 2024-05-14 15:28:56.000000 quite6-1.0.4/quite6/tools/load_ui.py
+-rw-r--r--   0 wangcong   (502) staff       (20)      315 2024-05-14 14:37:29.000000 quite6-1.0.4/quite6/tools/process.py
+drwxr-xr-x   0 wangcong   (502) staff       (20)        0 2024-05-25 14:32:00.203993 quite6-1.0.4/quite6.egg-info/
+-rw-r--r--   0 wangcong   (502) staff       (20)     3749 2024-05-25 14:31:59.000000 quite6-1.0.4/quite6.egg-info/PKG-INFO
+-rw-r--r--   0 wangcong   (502) staff       (20)     2427 2024-05-25 14:32:00.000000 quite6-1.0.4/quite6.egg-info/SOURCES.txt
+-rw-r--r--   0 wangcong   (502) staff       (20)        1 2024-05-25 14:31:59.000000 quite6-1.0.4/quite6.egg-info/dependency_links.txt
+-rw-r--r--   0 wangcong   (502) staff       (20)       41 2024-05-25 14:31:59.000000 quite6-1.0.4/quite6.egg-info/requires.txt
+-rw-r--r--   0 wangcong   (502) staff       (20)        7 2024-05-25 14:31:59.000000 quite6-1.0.4/quite6.egg-info/top_level.txt
+-rw-r--r--   0 wangcong   (502) staff       (20)     2557 2024-05-14 10:15:26.000000 quite6-1.0.4/readme.md
+-rw-r--r--   0 wangcong   (502) staff       (20)       40 2024-05-16 14:15:45.000000 quite6-1.0.4/requirements.txt
+-rw-r--r--   0 wangcong   (502) staff       (20)      154 2024-05-25 14:32:00.207638 quite6-1.0.4/setup.cfg
+-rw-r--r--   0 wangcong   (502) staff       (20)     1633 2024-05-14 10:15:26.000000 quite6-1.0.4/setup.py
+-rw-r--r--   0 wangcong   (502) staff       (20)     2173 2024-05-14 10:15:26.000000 quite6-1.0.4/version.py
```

### Comparing `quite6-1.0.3/LICENSE` & `quite6-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `quite6-1.0.3/PKG-INFO` & `quite6-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quite6
-Version: 1.0.3
+Version: 1.0.4
 Summary: QT UI Extension
 Home-page: https://github.com/KD-Group/quite6
 Author: SF-Zhou
 Author-email: sfzhou.scut@gmail.com
 License: MIT
 Keywords: qt ui
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `quite6-1.0.3/README.rst` & `quite6-1.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `quite6-1.0.3/quite6/controller/dialog_ui_controller.py` & `quite6-1.0.4/quite6/controller/dialog_ui_controller.py`

 * *Files identical despite different names*

### Comparing `quite6-1.0.3/quite6/controller/file_dialog_controller.py` & `quite6-1.0.4/quite6/controller/file_dialog_controller.py`

 * *Files identical despite different names*

### Comparing `quite6-1.0.3/quite6/controller/widget_controller.py` & `quite6-1.0.4/quite6/controller/widget_controller.py`

 * *Files identical despite different names*

### Comparing `quite6-1.0.3/quite6/controller/widget_ui_controller.py` & `quite6-1.0.4/quite6/controller/widget_ui_controller.py`

 * *Files identical despite different names*

### Comparing `quite6-1.0.3/quite6/core/event_loop.py` & `quite6-1.0.4/quite6/core/event_loop.py`

 * *Files identical despite different names*

### Comparing `quite6-1.0.3/quite6/deferred_function.py` & `quite6-1.0.4/quite6/deferred_function.py`

 * *Files identical despite different names*

### Comparing `quite6-1.0.3/quite6/gui/__init__.py` & `quite6-1.0.4/quite6/gui/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,10 +18,10 @@
 from .widgets import Widget, Dialog
 from .widgets import MainWindow, GroupBox, DockWidget
 from .widgets import Label, LineEdit, DateEdit, TextEdit, TimeEdit
 from .widgets import ListWidget, ComboBox
 from .widgets import SpinBox, DoubleSpinBox
 from .widgets import InputDialog
 from .widgets import Action, Shortcut, PushButton, RatioButton
-from .widgets import TableWidget, TableView
+from .widgets import TabWidget, TableWidget, TableView
 from .widgets import PlotWidget
 from .widgets import Layout
```

### Comparing `quite6-1.0.3/quite6/gui/interfaces/__init__.py` & `quite6-1.0.4/quite6/gui/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `quite6-1.0.3/quite6/gui/interfaces/ability_interfaces/container_ability_interface.py` & `quite6-1.0.4/quite6/gui/interfaces/ability_interfaces/container_ability_interface.py`

 * *Files identical despite different names*

### Comparing `quite6-1.0.3/quite6/gui/interfaces/base_interface.py` & `quite6-1.0.4/quite6/gui/interfaces/base_interface.py`

 * *Files identical despite different names*

### Comparing `quite6-1.0.3/quite6/gui/layouts/square_layout.py` & `quite6-1.0.4/quite6/gui/layouts/square_layout.py`

 * *Files identical despite different names*

### Comparing `quite6-1.0.3/quite6/gui/paint/painter.py` & `quite6-1.0.4/quite6/gui/paint/painter.py`

 * *Files identical despite different names*

### Comparing `quite6-1.0.3/quite6/gui/paint/point.py` & `quite6-1.0.4/quite6/gui/paint/point.py`

 * *Files identical despite different names*

### Comparing `quite6-1.0.3/quite6/gui/paint/size.py` & `quite6-1.0.4/quite6/gui/paint/size.py`

 * *Files identical despite different names*

### Comparing `quite6-1.0.3/quite6/gui/widgets/__init__.py` & `quite6-1.0.4/quite6/gui/widgets/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from .line_edit import LineEdit
 from .list_widget import ListWidget
 from .main_window import MainWindow
 from .plot_widget import PlotWidget
 from .push_button import PushButton
 from .shortcut import Shortcut
 from .spin_box import SpinBox
+from .tab_widget import TabWidget
 from .table_widget import TableWidget
 from .widget import Widget
 from .radio_button import RatioButton
 from .text_edit import TextEdit
 from .time_edit import TimeEdit
 from .table_view import TableView
 from .date_time_edit import DateTimeEdit
```

### Comparing `quite6-1.0.3/quite6/gui/widgets/combo_box.py` & `quite6-1.0.4/quite6/gui/widgets/combo_box.py`

 * *Files identical despite different names*

### Comparing `quite6-1.0.3/quite6/gui/widgets/date_edit.py` & `quite6-1.0.4/quite6/gui/widgets/date_edit.py`

 * *Files identical despite different names*

### Comparing `quite6-1.0.3/quite6/gui/widgets/date_time_edit.py` & `quite6-1.0.4/quite6/gui/widgets/date_time_edit.py`

 * *Files identical despite different names*

### Comparing `quite6-1.0.3/quite6/gui/widgets/dialog.py` & `quite6-1.0.4/quite6/gui/widgets/dialog.py`

 * *Files identical despite different names*

### Comparing `quite6-1.0.3/quite6/gui/widgets/double_spin_box.py` & `quite6-1.0.4/quite6/gui/widgets/double_spin_box.py`

 * *Files identical despite different names*

### Comparing `quite6-1.0.3/quite6/gui/widgets/input_dialog.py` & `quite6-1.0.4/quite6/gui/widgets/input_dialog.py`

 * *Files identical despite different names*

### Comparing `quite6-1.0.3/quite6/gui/widgets/label.py` & `quite6-1.0.4/quite6/gui/widgets/label.py`

 * *Files identical despite different names*

### Comparing `quite6-1.0.3/quite6/gui/widgets/line_edit.py` & `quite6-1.0.4/quite6/gui/widgets/line_edit.py`

 * *Files identical despite different names*

### Comparing `quite6-1.0.3/quite6/gui/widgets/list_widget.py` & `quite6-1.0.4/quite6/gui/widgets/list_widget.py`

 * *Files identical despite different names*

### Comparing `quite6-1.0.3/quite6/gui/widgets/main_window.py` & `quite6-1.0.4/quite6/gui/widgets/main_window.py`

 * *Files identical despite different names*

### Comparing `quite6-1.0.3/quite6/gui/widgets/plot_widget.py` & `quite6-1.0.4/quite6/gui/widgets/plot_widget.py`

 * *Files identical despite different names*

### Comparing `quite6-1.0.3/quite6/gui/widgets/push_button.py` & `quite6-1.0.4/quite6/gui/widgets/push_button.py`

 * *Files identical despite different names*

### Comparing `quite6-1.0.3/quite6/gui/widgets/radio_button.py` & `quite6-1.0.4/quite6/gui/widgets/radio_button.py`

 * *Files identical despite different names*

### Comparing `quite6-1.0.3/quite6/gui/widgets/shortcut.py` & `quite6-1.0.4/quite6/gui/widgets/shortcut.py`

 * *Files identical despite different names*

### Comparing `quite6-1.0.3/quite6/gui/widgets/spin_box.py` & `quite6-1.0.4/quite6/gui/widgets/spin_box.py`

 * *Files identical despite different names*

### Comparing `quite6-1.0.3/quite6/gui/widgets/table_view.py` & `quite6-1.0.4/quite6/gui/widgets/table_view.py`

 * *Files identical despite different names*

### Comparing `quite6-1.0.3/quite6/gui/widgets/table_widget.py` & `quite6-1.0.4/quite6/gui/widgets/table_widget.py`

 * *Files identical despite different names*

### Comparing `quite6-1.0.3/quite6/gui/widgets/text_edit.py` & `quite6-1.0.4/quite6/gui/widgets/text_edit.py`

 * *Files identical despite different names*

### Comparing `quite6-1.0.3/quite6/gui/widgets/time_edit.py` & `quite6-1.0.4/quite6/gui/widgets/time_edit.py`

 * *Files identical despite different names*

### Comparing `quite6-1.0.3/quite6/gui/widgets/widget.py` & `quite6-1.0.4/quite6/gui/widgets/widget.py`

 * *Files identical despite different names*

### Comparing `quite6-1.0.3/quite6/tools/load_qrc.py` & `quite6-1.0.4/quite6/tools/load_qrc.py`

 * *Files identical despite different names*

### Comparing `quite6-1.0.3/quite6/tools/load_ui.py` & `quite6-1.0.4/quite6/tools/load_ui.py`

 * *Files identical despite different names*

### Comparing `quite6-1.0.3/quite6.egg-info/PKG-INFO` & `quite6-1.0.4/quite6.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quite6
-Version: 1.0.3
+Version: 1.0.4
 Summary: QT UI Extension
 Home-page: https://github.com/KD-Group/quite6
 Author: SF-Zhou
 Author-email: sfzhou.scut@gmail.com
 License: MIT
 Keywords: qt ui
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `quite6-1.0.3/quite6.egg-info/SOURCES.txt` & `quite6-1.0.4/quite6.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -61,14 +61,15 @@
 quite6/gui/widgets/list_widget.py
 quite6/gui/widgets/main_window.py
 quite6/gui/widgets/plot_widget.py
 quite6/gui/widgets/push_button.py
 quite6/gui/widgets/radio_button.py
 quite6/gui/widgets/shortcut.py
 quite6/gui/widgets/spin_box.py
+quite6/gui/widgets/tab_widget.py
 quite6/gui/widgets/table_view.py
 quite6/gui/widgets/table_widget.py
 quite6/gui/widgets/text_edit.py
 quite6/gui/widgets/time_edit.py
 quite6/gui/widgets/widget.py
 quite6/tools/__init__.py
 quite6/tools/load_qrc.py
```

### Comparing `quite6-1.0.3/readme.md` & `quite6-1.0.4/readme.md`

 * *Files identical despite different names*

### Comparing `quite6-1.0.3/setup.py` & `quite6-1.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `quite6-1.0.3/version.py` & `quite6-1.0.4/version.py`

 * *Files identical despite different names*

