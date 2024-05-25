# Comparing `tmp/flet_core-0.9.0.dev1630.tar.gz` & `tmp/flet_core-0.9.0.dev1631.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flet_core-0.9.0.dev1630.tar", max compression
+gzip compressed data, was "flet_core-0.9.0.dev1631.tar", max compression
```

## Comparing `flet_core-0.9.0.dev1630.tar` & `flet_core-0.9.0.dev1631.tar`

### file list

```diff
@@ -1,133 +1,133 @@
--rw-r--r--   0        0        0      189 2023-08-02 21:47:06.464837 flet_core-0.9.0.dev1630/README.md
--rw-r--r--   0        0        0      723 2023-08-02 21:47:43.434245 flet_core-0.9.0.dev1630/pyproject.toml
--rw-r--r--   0        0        0     6623 2023-08-02 21:47:06.464837 flet_core-0.9.0.dev1630/src/flet_core/__init__.py
--rw-r--r--   0        0        0     6774 2023-08-02 21:47:06.464837 flet_core-0.9.0.dev1630/src/flet_core/alert_dialog.py
--rw-r--r--   0        0        0      407 2023-08-02 21:47:06.464837 flet_core-0.9.0.dev1630/src/flet_core/alignment.py
--rw-r--r--   0        0        0     7226 2023-08-02 21:47:06.464837 flet_core-0.9.0.dev1630/src/flet_core/animated_switcher.py
--rw-r--r--   0        0        0     2806 2023-08-02 21:47:06.464837 flet_core-0.9.0.dev1630/src/flet_core/animation.py
--rw-r--r--   0        0        0     5403 2023-08-02 21:47:06.464837 flet_core-0.9.0.dev1630/src/flet_core/app_bar.py
--rw-r--r--   0        0        0     7892 2023-08-02 21:47:06.464837 flet_core-0.9.0.dev1630/src/flet_core/audio.py
--rw-r--r--   0        0        0     5446 2023-08-02 21:47:06.464837 flet_core-0.9.0.dev1630/src/flet_core/banner.py
--rw-r--r--   0        0        0      326 2023-08-02 21:47:06.464837 flet_core-0.9.0.dev1630/src/flet_core/blur.py
--rw-r--r--   0        0        0     1079 2023-08-02 21:47:06.464837 flet_core-0.9.0.dev1630/src/flet_core/border.py
--rw-r--r--   0        0        0      958 2023-08-02 21:47:06.464837 flet_core-0.9.0.dev1630/src/flet_core/border_radius.py
--rw-r--r--   0        0        0     4320 2023-08-02 21:47:06.464837 flet_core-0.9.0.dev1630/src/flet_core/bottom_sheet.py
--rw-r--r--   0        0        0     2202 2023-08-02 21:47:06.464837 flet_core-0.9.0.dev1630/src/flet_core/buttons.py
--rw-r--r--   0        0        0      514 2023-08-02 21:47:06.464837 flet_core-0.9.0.dev1630/src/flet_core/canvas/__init__.py
--rw-r--r--   0        0        0     2903 2023-08-02 21:47:06.464837 flet_core-0.9.0.dev1630/src/flet_core/canvas/arc.py
--rw-r--r--   0        0        0     4629 2023-08-02 21:47:06.464837 flet_core-0.9.0.dev1630/src/flet_core/canvas/canvas.py
--rw-r--r--   0        0        0     1639 2023-08-02 21:47:06.464837 flet_core-0.9.0.dev1630/src/flet_core/canvas/circle.py
--rw-r--r--   0        0        0     1361 2023-08-02 21:47:06.464837 flet_core-0.9.0.dev1630/src/flet_core/canvas/color.py
--rw-r--r--   0        0        0      837 2023-08-02 21:47:06.464837 flet_core-0.9.0.dev1630/src/flet_core/canvas/fill.py
--rw-r--r--   0        0        0     1862 2023-08-02 21:47:06.464837 flet_core-0.9.0.dev1630/src/flet_core/canvas/line.py
--rw-r--r--   0        0        0     1907 2023-08-02 21:47:06.464837 flet_core-0.9.0.dev1630/src/flet_core/canvas/oval.py
--rw-r--r--   0        0        0     3486 2023-08-02 21:47:06.464837 flet_core-0.9.0.dev1630/src/flet_core/canvas/path.py
--rw-r--r--   0        0        0     1772 2023-08-02 21:47:06.464837 flet_core-0.9.0.dev1630/src/flet_core/canvas/points.py
--rw-r--r--   0        0        0     2361 2023-08-02 21:47:06.468837 flet_core-0.9.0.dev1630/src/flet_core/canvas/rect.py
--rw-r--r--   0        0        0     1963 2023-08-02 21:47:06.468837 flet_core-0.9.0.dev1630/src/flet_core/canvas/shadow.py
--rw-r--r--   0        0        0      347 2023-08-02 21:47:06.468837 flet_core-0.9.0.dev1630/src/flet_core/canvas/shape.py
--rw-r--r--   0        0        0     4172 2023-08-02 21:47:06.468837 flet_core-0.9.0.dev1630/src/flet_core/canvas/text.py
--rw-r--r--   0        0        0     5695 2023-08-02 21:47:06.468837 flet_core-0.9.0.dev1630/src/flet_core/card.py
--rw-r--r--   0        0        0     9855 2023-08-02 21:47:06.468837 flet_core-0.9.0.dev1630/src/flet_core/charts/bar_chart.py
--rw-r--r--   0        0        0     2061 2023-08-02 21:47:06.468837 flet_core-0.9.0.dev1630/src/flet_core/charts/bar_chart_group.py
--rw-r--r--   0        0        0     6837 2023-08-02 21:47:06.468837 flet_core-0.9.0.dev1630/src/flet_core/charts/bar_chart_rod.py
--rw-r--r--   0        0        0     1949 2023-08-02 21:47:06.468837 flet_core-0.9.0.dev1630/src/flet_core/charts/bar_chart_rod_stack_item.py
--rw-r--r--   0        0        0     2924 2023-08-02 21:47:06.468837 flet_core-0.9.0.dev1630/src/flet_core/charts/chart_axis.py
--rw-r--r--   0        0        0     1293 2023-08-02 21:47:06.468837 flet_core-0.9.0.dev1630/src/flet_core/charts/chart_axis_label.py
--rw-r--r--   0        0        0      338 2023-08-02 21:47:06.468837 flet_core-0.9.0.dev1630/src/flet_core/charts/chart_grid_lines.py
--rw-r--r--   0        0        0      286 2023-08-02 21:47:06.468837 flet_core-0.9.0.dev1630/src/flet_core/charts/chart_point_line.py
--rw-r--r--   0        0        0     1006 2023-08-02 21:47:06.468837 flet_core-0.9.0.dev1630/src/flet_core/charts/chart_point_shape.py
--rw-r--r--   0        0        0    11228 2023-08-02 21:47:06.468837 flet_core-0.9.0.dev1630/src/flet_core/charts/line_chart.py
--rw-r--r--   0        0        0     8258 2023-08-02 21:47:06.468837 flet_core-0.9.0.dev1630/src/flet_core/charts/line_chart_data.py
--rw-r--r--   0        0        0     5496 2023-08-02 21:47:06.468837 flet_core-0.9.0.dev1630/src/flet_core/charts/line_chart_data_point.py
--rw-r--r--   0        0        0     5888 2023-08-02 21:47:06.468837 flet_core-0.9.0.dev1630/src/flet_core/charts/pie_chart.py
--rw-r--r--   0        0        0     3824 2023-08-02 21:47:06.468837 flet_core-0.9.0.dev1630/src/flet_core/charts/pie_chart_section.py
--rw-r--r--   0        0        0     7156 2023-08-02 21:47:06.468837 flet_core-0.9.0.dev1630/src/flet_core/checkbox.py
--rw-r--r--   0        0        0     6795 2023-08-02 21:47:06.468837 flet_core-0.9.0.dev1630/src/flet_core/circle_avatar.py
--rw-r--r--   0        0        0     3085 2023-08-02 21:47:06.468837 flet_core-0.9.0.dev1630/src/flet_core/client_storage.py
--rw-r--r--   0        0        0     1148 2023-08-02 21:47:06.468837 flet_core-0.9.0.dev1630/src/flet_core/clipboard.py
--rw-r--r--   0        0        0    10708 2023-08-02 21:47:06.468837 flet_core-0.9.0.dev1630/src/flet_core/colors.py
--rw-r--r--   0        0        0     6924 2023-08-02 21:47:06.468837 flet_core-0.9.0.dev1630/src/flet_core/column.py
--rw-r--r--   0        0        0     1140 2023-08-02 21:47:06.468837 flet_core-0.9.0.dev1630/src/flet_core/connection.py
--rw-r--r--   0        0        0     7099 2023-08-02 21:47:06.468837 flet_core-0.9.0.dev1630/src/flet_core/constrained_control.py
--rw-r--r--   0        0        0    14684 2023-08-02 21:47:06.468837 flet_core-0.9.0.dev1630/src/flet_core/container.py
--rw-r--r--   0        0        0    14139 2023-08-02 21:47:06.468837 flet_core-0.9.0.dev1630/src/flet_core/control.py
--rw-r--r--   0        0        0      260 2023-08-02 21:47:06.468837 flet_core-0.9.0.dev1630/src/flet_core/control_event.py
--rw-r--r--   0        0        0    20707 2023-08-02 21:47:06.468837 flet_core-0.9.0.dev1630/src/flet_core/datatable.py
--rw-r--r--   0        0        0     2263 2023-08-02 21:47:06.468837 flet_core-0.9.0.dev1630/src/flet_core/divider.py
--rw-r--r--   0        0        0     6270 2023-08-02 21:47:06.468837 flet_core-0.9.0.dev1630/src/flet_core/drag_target.py
--rw-r--r--   0        0        0     6063 2023-08-02 21:47:06.468837 flet_core-0.9.0.dev1630/src/flet_core/draggable.py
--rw-r--r--   0        0        0     9177 2023-08-02 21:47:06.468837 flet_core-0.9.0.dev1630/src/flet_core/dropdown.py
--rw-r--r--   0        0        0     8848 2023-08-02 21:47:06.468837 flet_core-0.9.0.dev1630/src/flet_core/elevated_button.py
--rw-r--r--   0        0        0     1978 2023-08-02 21:47:06.468837 flet_core-0.9.0.dev1630/src/flet_core/embed_json_encoder.py
--rw-r--r--   0        0        0      166 2023-08-02 21:47:06.468837 flet_core-0.9.0.dev1630/src/flet_core/event.py
--rw-r--r--   0        0        0     1839 2023-08-02 21:47:06.468837 flet_core-0.9.0.dev1630/src/flet_core/event_handler.py
--rw-r--r--   0        0        0     9777 2023-08-02 21:47:06.468837 flet_core-0.9.0.dev1630/src/flet_core/file_picker.py
--rw-r--r--   0        0        0     2694 2023-08-02 21:47:06.468837 flet_core-0.9.0.dev1630/src/flet_core/filled_button.py
--rw-r--r--   0        0        0     2828 2023-08-02 21:47:06.468837 flet_core-0.9.0.dev1630/src/flet_core/filled_tonal_button.py
--rw-r--r--   0        0        0     3613 2023-08-02 21:47:06.468837 flet_core-0.9.0.dev1630/src/flet_core/flet_app.py
--rw-r--r--   0        0        0     7111 2023-08-02 21:47:06.468837 flet_core-0.9.0.dev1630/src/flet_core/floating_action_button.py
--rw-r--r--   0        0        0    13981 2023-08-02 21:47:06.468837 flet_core-0.9.0.dev1630/src/flet_core/form_field_control.py
--rw-r--r--   0        0        0    28044 2023-08-02 21:47:06.468837 flet_core-0.9.0.dev1630/src/flet_core/gesture_detector.py
--rw-r--r--   0        0        0     1531 2023-08-02 21:47:06.468837 flet_core-0.9.0.dev1630/src/flet_core/gradients.py
--rw-r--r--   0        0        0     6804 2023-08-02 21:47:06.468837 flet_core-0.9.0.dev1630/src/flet_core/grid_view.py
--rw-r--r--   0        0        0     2100 2023-08-02 21:47:06.468837 flet_core-0.9.0.dev1630/src/flet_core/haptic_feedback.py
--rw-r--r--   0        0        0     3430 2023-08-02 21:47:06.468837 flet_core-0.9.0.dev1630/src/flet_core/icon.py
--rw-r--r--   0        0        0     8438 2023-08-02 21:47:06.468837 flet_core-0.9.0.dev1630/src/flet_core/icon_button.py
--rw-r--r--   0        0        0   362652 2023-08-02 21:47:06.468837 flet_core-0.9.0.dev1630/src/flet_core/icons.py
--rw-r--r--   0        0        0     7171 2023-08-02 21:47:06.472836 flet_core-0.9.0.dev1630/src/flet_core/image.py
--rw-r--r--   0        0        0      367 2023-08-02 21:47:06.472836 flet_core-0.9.0.dev1630/src/flet_core/inline_span.py
--rw-r--r--   0        0        0     8737 2023-08-02 21:47:06.472836 flet_core-0.9.0.dev1630/src/flet_core/list_tile.py
--rw-r--r--   0        0        0     6401 2023-08-02 21:47:06.472836 flet_core-0.9.0.dev1630/src/flet_core/list_view.py
--rw-r--r--   0        0        0     9071 2023-08-02 21:47:06.472836 flet_core-0.9.0.dev1630/src/flet_core/local_connection.py
--rw-r--r--   0        0        0      223 2023-08-02 21:47:06.472836 flet_core-0.9.0.dev1630/src/flet_core/locks.py
--rw-r--r--   0        0        0      583 2023-08-02 21:47:06.472836 flet_core-0.9.0.dev1630/src/flet_core/margin.py
--rw-r--r--   0        0        0     6129 2023-08-02 21:47:06.472836 flet_core-0.9.0.dev1630/src/flet_core/markdown.py
--rw-r--r--   0        0        0     5180 2023-08-02 21:47:06.472836 flet_core-0.9.0.dev1630/src/flet_core/matplotlib_chart.py
--rw-r--r--   0        0        0     8334 2023-08-02 21:47:06.472836 flet_core-0.9.0.dev1630/src/flet_core/navigation_bar.py
--rw-r--r--   0        0        0    11998 2023-08-02 21:47:06.472836 flet_core-0.9.0.dev1630/src/flet_core/navigation_rail.py
--rw-r--r--   0        0        0     7489 2023-08-02 21:47:06.472836 flet_core-0.9.0.dev1630/src/flet_core/outlined_button.py
--rw-r--r--   0        0        0      587 2023-08-02 21:47:06.472836 flet_core-0.9.0.dev1630/src/flet_core/padding.py
--rw-r--r--   0        0        0    58165 2023-08-02 21:47:06.472836 flet_core-0.9.0.dev1630/src/flet_core/page.py
--rw-r--r--   0        0        0     2746 2023-08-02 21:47:06.472836 flet_core-0.9.0.dev1630/src/flet_core/painting.py
--rw-r--r--   0        0        0     4410 2023-08-02 21:47:06.472836 flet_core-0.9.0.dev1630/src/flet_core/plotly_chart.py
--rw-r--r--   0        0        0     6811 2023-08-02 21:47:06.472836 flet_core-0.9.0.dev1630/src/flet_core/popup_menu_button.py
--rw-r--r--   0        0        0     4293 2023-08-02 21:47:06.472836 flet_core-0.9.0.dev1630/src/flet_core/progress_bar.py
--rw-r--r--   0        0        0     4491 2023-08-02 21:47:06.472836 flet_core-0.9.0.dev1630/src/flet_core/progress_ring.py
--rw-r--r--   0        0        0     4148 2023-08-02 21:47:06.472836 flet_core-0.9.0.dev1630/src/flet_core/protocol.py
--rw-r--r--   0        0        0     3419 2023-08-02 21:47:06.472836 flet_core-0.9.0.dev1630/src/flet_core/querystring.py
--rw-r--r--   0        0        0     5765 2023-08-02 21:47:06.472836 flet_core-0.9.0.dev1630/src/flet_core/radio.py
--rw-r--r--   0        0        0     2389 2023-08-02 21:47:06.472836 flet_core-0.9.0.dev1630/src/flet_core/radio_group.py
--rw-r--r--   0        0        0      291 2023-08-02 21:47:06.472836 flet_core-0.9.0.dev1630/src/flet_core/ref.py
--rw-r--r--   0        0        0     6344 2023-08-02 21:47:06.472836 flet_core-0.9.0.dev1630/src/flet_core/responsive_row.py
--rw-r--r--   0        0        0     6908 2023-08-02 21:47:06.472836 flet_core-0.9.0.dev1630/src/flet_core/row.py
--rw-r--r--   0        0        0     4805 2023-08-02 21:47:06.472836 flet_core-0.9.0.dev1630/src/flet_core/safe_area.py
--rw-r--r--   0        0        0     4486 2023-08-02 21:47:06.472836 flet_core-0.9.0.dev1630/src/flet_core/scrollable_control.py
--rw-r--r--   0        0        0     1637 2023-08-02 21:47:06.472836 flet_core-0.9.0.dev1630/src/flet_core/semantics.py
--rw-r--r--   0        0        0      576 2023-08-02 21:47:06.472836 flet_core-0.9.0.dev1630/src/flet_core/session_storage.py
--rw-r--r--   0        0        0     5318 2023-08-02 21:47:06.472836 flet_core-0.9.0.dev1630/src/flet_core/shader_mask.py
--rw-r--r--   0        0        0      572 2023-08-02 21:47:06.472836 flet_core-0.9.0.dev1630/src/flet_core/shadow.py
--rw-r--r--   0        0        0     2919 2023-08-02 21:47:06.472836 flet_core-0.9.0.dev1630/src/flet_core/shake_detector.py
--rw-r--r--   0        0        0     7382 2023-08-02 21:47:06.472836 flet_core-0.9.0.dev1630/src/flet_core/slider.py
--rw-r--r--   0        0        0     6842 2023-08-02 21:47:06.472836 flet_core-0.9.0.dev1630/src/flet_core/snack_bar.py
--rw-r--r--   0        0        0     4889 2023-08-02 21:47:06.472836 flet_core-0.9.0.dev1630/src/flet_core/stack.py
--rw-r--r--   0        0        0     8104 2023-08-02 21:47:06.472836 flet_core-0.9.0.dev1630/src/flet_core/switch.py
--rw-r--r--   0        0        0    10820 2023-08-02 21:47:06.472836 flet_core-0.9.0.dev1630/src/flet_core/tabs.py
--rw-r--r--   0        0        0      632 2023-08-02 21:47:06.472836 flet_core-0.9.0.dev1630/src/flet_core/template_route.py
--rw-r--r--   0        0        0    10568 2023-08-02 21:47:06.472836 flet_core-0.9.0.dev1630/src/flet_core/text.py
--rw-r--r--   0        0        0     7462 2023-08-02 21:47:06.472836 flet_core-0.9.0.dev1630/src/flet_core/text_button.py
--rw-r--r--   0        0        0     3092 2023-08-02 21:47:06.472836 flet_core-0.9.0.dev1630/src/flet_core/text_span.py
--rw-r--r--   0        0        0     1260 2023-08-02 21:47:06.472836 flet_core-0.9.0.dev1630/src/flet_core/text_style.py
--rw-r--r--   0        0        0    17045 2023-08-02 21:47:06.472836 flet_core-0.9.0.dev1630/src/flet_core/textfield.py
--rw-r--r--   0        0        0     6172 2023-08-02 21:47:06.472836 flet_core-0.9.0.dev1630/src/flet_core/theme.py
--rw-r--r--   0        0        0     8362 2023-08-02 21:47:06.472836 flet_core-0.9.0.dev1630/src/flet_core/tooltip.py
--rw-r--r--   0        0        0      544 2023-08-02 21:47:06.472836 flet_core-0.9.0.dev1630/src/flet_core/transform.py
--rw-r--r--   0        0        0     2753 2023-08-02 21:47:06.472836 flet_core-0.9.0.dev1630/src/flet_core/transparent_pointer.py
--rw-r--r--   0        0        0     5550 2023-08-02 21:47:06.472836 flet_core-0.9.0.dev1630/src/flet_core/types.py
--rw-r--r--   0        0        0      684 2023-08-02 21:47:06.472836 flet_core-0.9.0.dev1630/src/flet_core/user_control.py
--rw-r--r--   0        0        0     4263 2023-08-02 21:47:06.472836 flet_core-0.9.0.dev1630/src/flet_core/utils.py
--rw-r--r--   0        0        0      103 2023-08-02 21:47:42.686258 flet_core-0.9.0.dev1630/src/flet_core/version.py
--rw-r--r--   0        0        0     2337 2023-08-02 21:47:06.472836 flet_core-0.9.0.dev1630/src/flet_core/vertical_divider.py
--rw-r--r--   0        0        0     6265 2023-08-02 21:47:06.472836 flet_core-0.9.0.dev1630/src/flet_core/view.py
--rw-r--r--   0        0        0     4049 2023-08-02 21:47:06.472836 flet_core-0.9.0.dev1630/src/flet_core/window_drag_area.py
--rw-r--r--   0        0        0     1052 1970-01-01 00:00:00.000000 flet_core-0.9.0.dev1630/PKG-INFO
+-rw-r--r--   0        0        0      189 2023-08-04 18:58:41.299380 flet_core-0.9.0.dev1631/README.md
+-rw-r--r--   0        0        0      723 2023-08-04 18:59:18.405202 flet_core-0.9.0.dev1631/pyproject.toml
+-rw-r--r--   0        0        0     6623 2023-08-04 18:58:41.299380 flet_core-0.9.0.dev1631/src/flet_core/__init__.py
+-rw-r--r--   0        0        0     6774 2023-08-04 18:58:41.299380 flet_core-0.9.0.dev1631/src/flet_core/alert_dialog.py
+-rw-r--r--   0        0        0      407 2023-08-04 18:58:41.299380 flet_core-0.9.0.dev1631/src/flet_core/alignment.py
+-rw-r--r--   0        0        0     7226 2023-08-04 18:58:41.299380 flet_core-0.9.0.dev1631/src/flet_core/animated_switcher.py
+-rw-r--r--   0        0        0     2806 2023-08-04 18:58:41.299380 flet_core-0.9.0.dev1631/src/flet_core/animation.py
+-rw-r--r--   0        0        0     5403 2023-08-04 18:58:41.299380 flet_core-0.9.0.dev1631/src/flet_core/app_bar.py
+-rw-r--r--   0        0        0     7892 2023-08-04 18:58:41.299380 flet_core-0.9.0.dev1631/src/flet_core/audio.py
+-rw-r--r--   0        0        0     5446 2023-08-04 18:58:41.299380 flet_core-0.9.0.dev1631/src/flet_core/banner.py
+-rw-r--r--   0        0        0      326 2023-08-04 18:58:41.299380 flet_core-0.9.0.dev1631/src/flet_core/blur.py
+-rw-r--r--   0        0        0     1079 2023-08-04 18:58:41.299380 flet_core-0.9.0.dev1631/src/flet_core/border.py
+-rw-r--r--   0        0        0      958 2023-08-04 18:58:41.299380 flet_core-0.9.0.dev1631/src/flet_core/border_radius.py
+-rw-r--r--   0        0        0     4320 2023-08-04 18:58:41.299380 flet_core-0.9.0.dev1631/src/flet_core/bottom_sheet.py
+-rw-r--r--   0        0        0     2202 2023-08-04 18:58:41.299380 flet_core-0.9.0.dev1631/src/flet_core/buttons.py
+-rw-r--r--   0        0        0      514 2023-08-04 18:58:41.299380 flet_core-0.9.0.dev1631/src/flet_core/canvas/__init__.py
+-rw-r--r--   0        0        0     2903 2023-08-04 18:58:41.299380 flet_core-0.9.0.dev1631/src/flet_core/canvas/arc.py
+-rw-r--r--   0        0        0     4629 2023-08-04 18:58:41.303380 flet_core-0.9.0.dev1631/src/flet_core/canvas/canvas.py
+-rw-r--r--   0        0        0     1639 2023-08-04 18:58:41.303380 flet_core-0.9.0.dev1631/src/flet_core/canvas/circle.py
+-rw-r--r--   0        0        0     1361 2023-08-04 18:58:41.303380 flet_core-0.9.0.dev1631/src/flet_core/canvas/color.py
+-rw-r--r--   0        0        0      837 2023-08-04 18:58:41.303380 flet_core-0.9.0.dev1631/src/flet_core/canvas/fill.py
+-rw-r--r--   0        0        0     1862 2023-08-04 18:58:41.303380 flet_core-0.9.0.dev1631/src/flet_core/canvas/line.py
+-rw-r--r--   0        0        0     1907 2023-08-04 18:58:41.303380 flet_core-0.9.0.dev1631/src/flet_core/canvas/oval.py
+-rw-r--r--   0        0        0     3486 2023-08-04 18:58:41.303380 flet_core-0.9.0.dev1631/src/flet_core/canvas/path.py
+-rw-r--r--   0        0        0     1772 2023-08-04 18:58:41.303380 flet_core-0.9.0.dev1631/src/flet_core/canvas/points.py
+-rw-r--r--   0        0        0     2361 2023-08-04 18:58:41.303380 flet_core-0.9.0.dev1631/src/flet_core/canvas/rect.py
+-rw-r--r--   0        0        0     1963 2023-08-04 18:58:41.303380 flet_core-0.9.0.dev1631/src/flet_core/canvas/shadow.py
+-rw-r--r--   0        0        0      347 2023-08-04 18:58:41.303380 flet_core-0.9.0.dev1631/src/flet_core/canvas/shape.py
+-rw-r--r--   0        0        0     4172 2023-08-04 18:58:41.303380 flet_core-0.9.0.dev1631/src/flet_core/canvas/text.py
+-rw-r--r--   0        0        0     5695 2023-08-04 18:58:41.303380 flet_core-0.9.0.dev1631/src/flet_core/card.py
+-rw-r--r--   0        0        0     9855 2023-08-04 18:58:41.303380 flet_core-0.9.0.dev1631/src/flet_core/charts/bar_chart.py
+-rw-r--r--   0        0        0     2061 2023-08-04 18:58:41.303380 flet_core-0.9.0.dev1631/src/flet_core/charts/bar_chart_group.py
+-rw-r--r--   0        0        0     6837 2023-08-04 18:58:41.303380 flet_core-0.9.0.dev1631/src/flet_core/charts/bar_chart_rod.py
+-rw-r--r--   0        0        0     1949 2023-08-04 18:58:41.303380 flet_core-0.9.0.dev1631/src/flet_core/charts/bar_chart_rod_stack_item.py
+-rw-r--r--   0        0        0     2924 2023-08-04 18:58:41.303380 flet_core-0.9.0.dev1631/src/flet_core/charts/chart_axis.py
+-rw-r--r--   0        0        0     1293 2023-08-04 18:58:41.303380 flet_core-0.9.0.dev1631/src/flet_core/charts/chart_axis_label.py
+-rw-r--r--   0        0        0      338 2023-08-04 18:58:41.303380 flet_core-0.9.0.dev1631/src/flet_core/charts/chart_grid_lines.py
+-rw-r--r--   0        0        0      286 2023-08-04 18:58:41.303380 flet_core-0.9.0.dev1631/src/flet_core/charts/chart_point_line.py
+-rw-r--r--   0        0        0     1006 2023-08-04 18:58:41.303380 flet_core-0.9.0.dev1631/src/flet_core/charts/chart_point_shape.py
+-rw-r--r--   0        0        0    11228 2023-08-04 18:58:41.303380 flet_core-0.9.0.dev1631/src/flet_core/charts/line_chart.py
+-rw-r--r--   0        0        0     8258 2023-08-04 18:58:41.303380 flet_core-0.9.0.dev1631/src/flet_core/charts/line_chart_data.py
+-rw-r--r--   0        0        0     5496 2023-08-04 18:58:41.303380 flet_core-0.9.0.dev1631/src/flet_core/charts/line_chart_data_point.py
+-rw-r--r--   0        0        0     5888 2023-08-04 18:58:41.303380 flet_core-0.9.0.dev1631/src/flet_core/charts/pie_chart.py
+-rw-r--r--   0        0        0     3824 2023-08-04 18:58:41.303380 flet_core-0.9.0.dev1631/src/flet_core/charts/pie_chart_section.py
+-rw-r--r--   0        0        0     7156 2023-08-04 18:58:41.303380 flet_core-0.9.0.dev1631/src/flet_core/checkbox.py
+-rw-r--r--   0        0        0     6795 2023-08-04 18:58:41.303380 flet_core-0.9.0.dev1631/src/flet_core/circle_avatar.py
+-rw-r--r--   0        0        0     3085 2023-08-04 18:58:41.303380 flet_core-0.9.0.dev1631/src/flet_core/client_storage.py
+-rw-r--r--   0        0        0     1148 2023-08-04 18:58:41.303380 flet_core-0.9.0.dev1631/src/flet_core/clipboard.py
+-rw-r--r--   0        0        0    10708 2023-08-04 18:58:41.303380 flet_core-0.9.0.dev1631/src/flet_core/colors.py
+-rw-r--r--   0        0        0     6924 2023-08-04 18:58:41.303380 flet_core-0.9.0.dev1631/src/flet_core/column.py
+-rw-r--r--   0        0        0     1140 2023-08-04 18:58:41.303380 flet_core-0.9.0.dev1631/src/flet_core/connection.py
+-rw-r--r--   0        0        0     7099 2023-08-04 18:58:41.303380 flet_core-0.9.0.dev1631/src/flet_core/constrained_control.py
+-rw-r--r--   0        0        0    14684 2023-08-04 18:58:41.303380 flet_core-0.9.0.dev1631/src/flet_core/container.py
+-rw-r--r--   0        0        0    14139 2023-08-04 18:58:41.303380 flet_core-0.9.0.dev1631/src/flet_core/control.py
+-rw-r--r--   0        0        0      260 2023-08-04 18:58:41.303380 flet_core-0.9.0.dev1631/src/flet_core/control_event.py
+-rw-r--r--   0        0        0    20707 2023-08-04 18:58:41.303380 flet_core-0.9.0.dev1631/src/flet_core/datatable.py
+-rw-r--r--   0        0        0     2263 2023-08-04 18:58:41.303380 flet_core-0.9.0.dev1631/src/flet_core/divider.py
+-rw-r--r--   0        0        0     6270 2023-08-04 18:58:41.303380 flet_core-0.9.0.dev1631/src/flet_core/drag_target.py
+-rw-r--r--   0        0        0     6063 2023-08-04 18:58:41.303380 flet_core-0.9.0.dev1631/src/flet_core/draggable.py
+-rw-r--r--   0        0        0     9177 2023-08-04 18:58:41.303380 flet_core-0.9.0.dev1631/src/flet_core/dropdown.py
+-rw-r--r--   0        0        0     8848 2023-08-04 18:58:41.303380 flet_core-0.9.0.dev1631/src/flet_core/elevated_button.py
+-rw-r--r--   0        0        0     1978 2023-08-04 18:58:41.303380 flet_core-0.9.0.dev1631/src/flet_core/embed_json_encoder.py
+-rw-r--r--   0        0        0      166 2023-08-04 18:58:41.303380 flet_core-0.9.0.dev1631/src/flet_core/event.py
+-rw-r--r--   0        0        0     1839 2023-08-04 18:58:41.303380 flet_core-0.9.0.dev1631/src/flet_core/event_handler.py
+-rw-r--r--   0        0        0     9777 2023-08-04 18:58:41.303380 flet_core-0.9.0.dev1631/src/flet_core/file_picker.py
+-rw-r--r--   0        0        0     2694 2023-08-04 18:58:41.303380 flet_core-0.9.0.dev1631/src/flet_core/filled_button.py
+-rw-r--r--   0        0        0     2828 2023-08-04 18:58:41.303380 flet_core-0.9.0.dev1631/src/flet_core/filled_tonal_button.py
+-rw-r--r--   0        0        0     3613 2023-08-04 18:58:41.303380 flet_core-0.9.0.dev1631/src/flet_core/flet_app.py
+-rw-r--r--   0        0        0     7111 2023-08-04 18:58:41.303380 flet_core-0.9.0.dev1631/src/flet_core/floating_action_button.py
+-rw-r--r--   0        0        0    13981 2023-08-04 18:58:41.303380 flet_core-0.9.0.dev1631/src/flet_core/form_field_control.py
+-rw-r--r--   0        0        0    28044 2023-08-04 18:58:41.303380 flet_core-0.9.0.dev1631/src/flet_core/gesture_detector.py
+-rw-r--r--   0        0        0     1531 2023-08-04 18:58:41.303380 flet_core-0.9.0.dev1631/src/flet_core/gradients.py
+-rw-r--r--   0        0        0     6804 2023-08-04 18:58:41.303380 flet_core-0.9.0.dev1631/src/flet_core/grid_view.py
+-rw-r--r--   0        0        0     2100 2023-08-04 18:58:41.303380 flet_core-0.9.0.dev1631/src/flet_core/haptic_feedback.py
+-rw-r--r--   0        0        0     3430 2023-08-04 18:58:41.303380 flet_core-0.9.0.dev1631/src/flet_core/icon.py
+-rw-r--r--   0        0        0     8438 2023-08-04 18:58:41.303380 flet_core-0.9.0.dev1631/src/flet_core/icon_button.py
+-rw-r--r--   0        0        0   362652 2023-08-04 18:58:41.307380 flet_core-0.9.0.dev1631/src/flet_core/icons.py
+-rw-r--r--   0        0        0     7171 2023-08-04 18:58:41.307380 flet_core-0.9.0.dev1631/src/flet_core/image.py
+-rw-r--r--   0        0        0      367 2023-08-04 18:58:41.307380 flet_core-0.9.0.dev1631/src/flet_core/inline_span.py
+-rw-r--r--   0        0        0     8737 2023-08-04 18:58:41.307380 flet_core-0.9.0.dev1631/src/flet_core/list_tile.py
+-rw-r--r--   0        0        0     6401 2023-08-04 18:58:41.307380 flet_core-0.9.0.dev1631/src/flet_core/list_view.py
+-rw-r--r--   0        0        0     9071 2023-08-04 18:58:41.307380 flet_core-0.9.0.dev1631/src/flet_core/local_connection.py
+-rw-r--r--   0        0        0      223 2023-08-04 18:58:41.307380 flet_core-0.9.0.dev1631/src/flet_core/locks.py
+-rw-r--r--   0        0        0      583 2023-08-04 18:58:41.307380 flet_core-0.9.0.dev1631/src/flet_core/margin.py
+-rw-r--r--   0        0        0     6129 2023-08-04 18:58:41.307380 flet_core-0.9.0.dev1631/src/flet_core/markdown.py
+-rw-r--r--   0        0        0     5180 2023-08-04 18:58:41.307380 flet_core-0.9.0.dev1631/src/flet_core/matplotlib_chart.py
+-rw-r--r--   0        0        0     8334 2023-08-04 18:58:41.307380 flet_core-0.9.0.dev1631/src/flet_core/navigation_bar.py
+-rw-r--r--   0        0        0    11998 2023-08-04 18:58:41.307380 flet_core-0.9.0.dev1631/src/flet_core/navigation_rail.py
+-rw-r--r--   0        0        0     7489 2023-08-04 18:58:41.307380 flet_core-0.9.0.dev1631/src/flet_core/outlined_button.py
+-rw-r--r--   0        0        0      587 2023-08-04 18:58:41.307380 flet_core-0.9.0.dev1631/src/flet_core/padding.py
+-rw-r--r--   0        0        0    58165 2023-08-04 18:58:41.307380 flet_core-0.9.0.dev1631/src/flet_core/page.py
+-rw-r--r--   0        0        0     2746 2023-08-04 18:58:41.307380 flet_core-0.9.0.dev1631/src/flet_core/painting.py
+-rw-r--r--   0        0        0     4410 2023-08-04 18:58:41.307380 flet_core-0.9.0.dev1631/src/flet_core/plotly_chart.py
+-rw-r--r--   0        0        0     6811 2023-08-04 18:58:41.307380 flet_core-0.9.0.dev1631/src/flet_core/popup_menu_button.py
+-rw-r--r--   0        0        0     4293 2023-08-04 18:58:41.307380 flet_core-0.9.0.dev1631/src/flet_core/progress_bar.py
+-rw-r--r--   0        0        0     4491 2023-08-04 18:58:41.307380 flet_core-0.9.0.dev1631/src/flet_core/progress_ring.py
+-rw-r--r--   0        0        0     4148 2023-08-04 18:58:41.307380 flet_core-0.9.0.dev1631/src/flet_core/protocol.py
+-rw-r--r--   0        0        0     3419 2023-08-04 18:58:41.307380 flet_core-0.9.0.dev1631/src/flet_core/querystring.py
+-rw-r--r--   0        0        0     5765 2023-08-04 18:58:41.307380 flet_core-0.9.0.dev1631/src/flet_core/radio.py
+-rw-r--r--   0        0        0     2389 2023-08-04 18:58:41.307380 flet_core-0.9.0.dev1631/src/flet_core/radio_group.py
+-rw-r--r--   0        0        0      291 2023-08-04 18:58:41.307380 flet_core-0.9.0.dev1631/src/flet_core/ref.py
+-rw-r--r--   0        0        0     6344 2023-08-04 18:58:41.307380 flet_core-0.9.0.dev1631/src/flet_core/responsive_row.py
+-rw-r--r--   0        0        0     6908 2023-08-04 18:58:41.307380 flet_core-0.9.0.dev1631/src/flet_core/row.py
+-rw-r--r--   0        0        0     4805 2023-08-04 18:58:41.307380 flet_core-0.9.0.dev1631/src/flet_core/safe_area.py
+-rw-r--r--   0        0        0     4486 2023-08-04 18:58:41.307380 flet_core-0.9.0.dev1631/src/flet_core/scrollable_control.py
+-rw-r--r--   0        0        0     1637 2023-08-04 18:58:41.307380 flet_core-0.9.0.dev1631/src/flet_core/semantics.py
+-rw-r--r--   0        0        0      576 2023-08-04 18:58:41.307380 flet_core-0.9.0.dev1631/src/flet_core/session_storage.py
+-rw-r--r--   0        0        0     5318 2023-08-04 18:58:41.307380 flet_core-0.9.0.dev1631/src/flet_core/shader_mask.py
+-rw-r--r--   0        0        0      572 2023-08-04 18:58:41.307380 flet_core-0.9.0.dev1631/src/flet_core/shadow.py
+-rw-r--r--   0        0        0     2919 2023-08-04 18:58:41.307380 flet_core-0.9.0.dev1631/src/flet_core/shake_detector.py
+-rw-r--r--   0        0        0     7382 2023-08-04 18:58:41.307380 flet_core-0.9.0.dev1631/src/flet_core/slider.py
+-rw-r--r--   0        0        0     6842 2023-08-04 18:58:41.307380 flet_core-0.9.0.dev1631/src/flet_core/snack_bar.py
+-rw-r--r--   0        0        0     4889 2023-08-04 18:58:41.307380 flet_core-0.9.0.dev1631/src/flet_core/stack.py
+-rw-r--r--   0        0        0     8104 2023-08-04 18:58:41.307380 flet_core-0.9.0.dev1631/src/flet_core/switch.py
+-rw-r--r--   0        0        0    10820 2023-08-04 18:58:41.307380 flet_core-0.9.0.dev1631/src/flet_core/tabs.py
+-rw-r--r--   0        0        0      632 2023-08-04 18:58:41.307380 flet_core-0.9.0.dev1631/src/flet_core/template_route.py
+-rw-r--r--   0        0        0    10568 2023-08-04 18:58:41.307380 flet_core-0.9.0.dev1631/src/flet_core/text.py
+-rw-r--r--   0        0        0     7462 2023-08-04 18:58:41.307380 flet_core-0.9.0.dev1631/src/flet_core/text_button.py
+-rw-r--r--   0        0        0     3092 2023-08-04 18:58:41.307380 flet_core-0.9.0.dev1631/src/flet_core/text_span.py
+-rw-r--r--   0        0        0     1260 2023-08-04 18:58:41.307380 flet_core-0.9.0.dev1631/src/flet_core/text_style.py
+-rw-r--r--   0        0        0    17045 2023-08-04 18:58:41.307380 flet_core-0.9.0.dev1631/src/flet_core/textfield.py
+-rw-r--r--   0        0        0     6172 2023-08-04 18:58:41.307380 flet_core-0.9.0.dev1631/src/flet_core/theme.py
+-rw-r--r--   0        0        0     8362 2023-08-04 18:58:41.307380 flet_core-0.9.0.dev1631/src/flet_core/tooltip.py
+-rw-r--r--   0        0        0      544 2023-08-04 18:58:41.307380 flet_core-0.9.0.dev1631/src/flet_core/transform.py
+-rw-r--r--   0        0        0     2753 2023-08-04 18:58:41.307380 flet_core-0.9.0.dev1631/src/flet_core/transparent_pointer.py
+-rw-r--r--   0        0        0     5550 2023-08-04 18:58:41.307380 flet_core-0.9.0.dev1631/src/flet_core/types.py
+-rw-r--r--   0        0        0      684 2023-08-04 18:58:41.307380 flet_core-0.9.0.dev1631/src/flet_core/user_control.py
+-rw-r--r--   0        0        0     4263 2023-08-04 18:58:41.307380 flet_core-0.9.0.dev1631/src/flet_core/utils.py
+-rw-r--r--   0        0        0      103 2023-08-04 18:59:17.141427 flet_core-0.9.0.dev1631/src/flet_core/version.py
+-rw-r--r--   0        0        0     2337 2023-08-04 18:58:41.307380 flet_core-0.9.0.dev1631/src/flet_core/vertical_divider.py
+-rw-r--r--   0        0        0     6265 2023-08-04 18:58:41.307380 flet_core-0.9.0.dev1631/src/flet_core/view.py
+-rw-r--r--   0        0        0     4049 2023-08-04 18:58:41.307380 flet_core-0.9.0.dev1631/src/flet_core/window_drag_area.py
+-rw-r--r--   0        0        0     1052 1970-01-01 00:00:00.000000 flet_core-0.9.0.dev1631/PKG-INFO
```

### Comparing `flet_core-0.9.0.dev1630/pyproject.toml` & `flet_core-0.9.0.dev1631/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flet-core"
-version = "0.9.0.dev1630"
+version = "0.9.0.dev1631"
 description = "Flet core library"
 authors = ["Appveyor Systems Inc. <hello@flet.dev>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 packages = [
     { include = "flet_core", from = "src" },
```

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/__init__.py` & `flet_core-0.9.0.dev1631/src/flet_core/__init__.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/alert_dialog.py` & `flet_core-0.9.0.dev1631/src/flet_core/alert_dialog.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/animated_switcher.py` & `flet_core-0.9.0.dev1631/src/flet_core/animated_switcher.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/animation.py` & `flet_core-0.9.0.dev1631/src/flet_core/animation.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/app_bar.py` & `flet_core-0.9.0.dev1631/src/flet_core/app_bar.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/audio.py` & `flet_core-0.9.0.dev1631/src/flet_core/audio.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/banner.py` & `flet_core-0.9.0.dev1631/src/flet_core/banner.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/border.py` & `flet_core-0.9.0.dev1631/src/flet_core/border.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/border_radius.py` & `flet_core-0.9.0.dev1631/src/flet_core/border_radius.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/bottom_sheet.py` & `flet_core-0.9.0.dev1631/src/flet_core/bottom_sheet.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/buttons.py` & `flet_core-0.9.0.dev1631/src/flet_core/buttons.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/canvas/__init__.py` & `flet_core-0.9.0.dev1631/src/flet_core/canvas/__init__.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/canvas/arc.py` & `flet_core-0.9.0.dev1631/src/flet_core/canvas/arc.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/canvas/canvas.py` & `flet_core-0.9.0.dev1631/src/flet_core/canvas/canvas.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/canvas/circle.py` & `flet_core-0.9.0.dev1631/src/flet_core/canvas/circle.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/canvas/color.py` & `flet_core-0.9.0.dev1631/src/flet_core/canvas/color.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/canvas/fill.py` & `flet_core-0.9.0.dev1631/src/flet_core/canvas/fill.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/canvas/line.py` & `flet_core-0.9.0.dev1631/src/flet_core/canvas/line.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/canvas/oval.py` & `flet_core-0.9.0.dev1631/src/flet_core/canvas/oval.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/canvas/path.py` & `flet_core-0.9.0.dev1631/src/flet_core/canvas/path.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/canvas/points.py` & `flet_core-0.9.0.dev1631/src/flet_core/canvas/points.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/canvas/rect.py` & `flet_core-0.9.0.dev1631/src/flet_core/canvas/rect.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/canvas/shadow.py` & `flet_core-0.9.0.dev1631/src/flet_core/canvas/shadow.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/canvas/text.py` & `flet_core-0.9.0.dev1631/src/flet_core/canvas/text.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/card.py` & `flet_core-0.9.0.dev1631/src/flet_core/card.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/charts/bar_chart.py` & `flet_core-0.9.0.dev1631/src/flet_core/charts/bar_chart.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/charts/bar_chart_group.py` & `flet_core-0.9.0.dev1631/src/flet_core/charts/bar_chart_group.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/charts/bar_chart_rod.py` & `flet_core-0.9.0.dev1631/src/flet_core/charts/bar_chart_rod.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/charts/bar_chart_rod_stack_item.py` & `flet_core-0.9.0.dev1631/src/flet_core/charts/bar_chart_rod_stack_item.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/charts/chart_axis.py` & `flet_core-0.9.0.dev1631/src/flet_core/charts/chart_axis.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/charts/chart_axis_label.py` & `flet_core-0.9.0.dev1631/src/flet_core/charts/chart_axis_label.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/charts/chart_point_shape.py` & `flet_core-0.9.0.dev1631/src/flet_core/charts/chart_point_shape.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/charts/line_chart.py` & `flet_core-0.9.0.dev1631/src/flet_core/charts/line_chart.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/charts/line_chart_data.py` & `flet_core-0.9.0.dev1631/src/flet_core/charts/line_chart_data.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/charts/line_chart_data_point.py` & `flet_core-0.9.0.dev1631/src/flet_core/charts/line_chart_data_point.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/charts/pie_chart.py` & `flet_core-0.9.0.dev1631/src/flet_core/charts/pie_chart.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/charts/pie_chart_section.py` & `flet_core-0.9.0.dev1631/src/flet_core/charts/pie_chart_section.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/checkbox.py` & `flet_core-0.9.0.dev1631/src/flet_core/checkbox.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/circle_avatar.py` & `flet_core-0.9.0.dev1631/src/flet_core/circle_avatar.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/client_storage.py` & `flet_core-0.9.0.dev1631/src/flet_core/client_storage.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/clipboard.py` & `flet_core-0.9.0.dev1631/src/flet_core/clipboard.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/colors.py` & `flet_core-0.9.0.dev1631/src/flet_core/colors.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/column.py` & `flet_core-0.9.0.dev1631/src/flet_core/column.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/connection.py` & `flet_core-0.9.0.dev1631/src/flet_core/connection.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/constrained_control.py` & `flet_core-0.9.0.dev1631/src/flet_core/constrained_control.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/container.py` & `flet_core-0.9.0.dev1631/src/flet_core/container.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/control.py` & `flet_core-0.9.0.dev1631/src/flet_core/control.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/datatable.py` & `flet_core-0.9.0.dev1631/src/flet_core/datatable.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/divider.py` & `flet_core-0.9.0.dev1631/src/flet_core/divider.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/drag_target.py` & `flet_core-0.9.0.dev1631/src/flet_core/drag_target.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/draggable.py` & `flet_core-0.9.0.dev1631/src/flet_core/draggable.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/dropdown.py` & `flet_core-0.9.0.dev1631/src/flet_core/dropdown.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/elevated_button.py` & `flet_core-0.9.0.dev1631/src/flet_core/elevated_button.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/embed_json_encoder.py` & `flet_core-0.9.0.dev1631/src/flet_core/embed_json_encoder.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/event_handler.py` & `flet_core-0.9.0.dev1631/src/flet_core/event_handler.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/file_picker.py` & `flet_core-0.9.0.dev1631/src/flet_core/file_picker.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/filled_button.py` & `flet_core-0.9.0.dev1631/src/flet_core/filled_button.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/filled_tonal_button.py` & `flet_core-0.9.0.dev1631/src/flet_core/filled_tonal_button.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/flet_app.py` & `flet_core-0.9.0.dev1631/src/flet_core/flet_app.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/floating_action_button.py` & `flet_core-0.9.0.dev1631/src/flet_core/floating_action_button.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/form_field_control.py` & `flet_core-0.9.0.dev1631/src/flet_core/form_field_control.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/gesture_detector.py` & `flet_core-0.9.0.dev1631/src/flet_core/gesture_detector.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/gradients.py` & `flet_core-0.9.0.dev1631/src/flet_core/gradients.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/grid_view.py` & `flet_core-0.9.0.dev1631/src/flet_core/grid_view.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/haptic_feedback.py` & `flet_core-0.9.0.dev1631/src/flet_core/haptic_feedback.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/icon.py` & `flet_core-0.9.0.dev1631/src/flet_core/icon.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/icon_button.py` & `flet_core-0.9.0.dev1631/src/flet_core/icon_button.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/icons.py` & `flet_core-0.9.0.dev1631/src/flet_core/icons.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/image.py` & `flet_core-0.9.0.dev1631/src/flet_core/image.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/list_tile.py` & `flet_core-0.9.0.dev1631/src/flet_core/list_tile.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/list_view.py` & `flet_core-0.9.0.dev1631/src/flet_core/list_view.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/local_connection.py` & `flet_core-0.9.0.dev1631/src/flet_core/local_connection.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/margin.py` & `flet_core-0.9.0.dev1631/src/flet_core/margin.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/markdown.py` & `flet_core-0.9.0.dev1631/src/flet_core/markdown.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/matplotlib_chart.py` & `flet_core-0.9.0.dev1631/src/flet_core/matplotlib_chart.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/navigation_bar.py` & `flet_core-0.9.0.dev1631/src/flet_core/navigation_bar.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/navigation_rail.py` & `flet_core-0.9.0.dev1631/src/flet_core/navigation_rail.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/outlined_button.py` & `flet_core-0.9.0.dev1631/src/flet_core/outlined_button.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/padding.py` & `flet_core-0.9.0.dev1631/src/flet_core/padding.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/page.py` & `flet_core-0.9.0.dev1631/src/flet_core/page.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/painting.py` & `flet_core-0.9.0.dev1631/src/flet_core/painting.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/plotly_chart.py` & `flet_core-0.9.0.dev1631/src/flet_core/plotly_chart.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/popup_menu_button.py` & `flet_core-0.9.0.dev1631/src/flet_core/popup_menu_button.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/progress_bar.py` & `flet_core-0.9.0.dev1631/src/flet_core/progress_bar.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/progress_ring.py` & `flet_core-0.9.0.dev1631/src/flet_core/progress_ring.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/protocol.py` & `flet_core-0.9.0.dev1631/src/flet_core/protocol.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/querystring.py` & `flet_core-0.9.0.dev1631/src/flet_core/querystring.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/radio.py` & `flet_core-0.9.0.dev1631/src/flet_core/radio.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/radio_group.py` & `flet_core-0.9.0.dev1631/src/flet_core/radio_group.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/responsive_row.py` & `flet_core-0.9.0.dev1631/src/flet_core/responsive_row.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/row.py` & `flet_core-0.9.0.dev1631/src/flet_core/row.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/safe_area.py` & `flet_core-0.9.0.dev1631/src/flet_core/safe_area.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/scrollable_control.py` & `flet_core-0.9.0.dev1631/src/flet_core/scrollable_control.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/semantics.py` & `flet_core-0.9.0.dev1631/src/flet_core/semantics.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/session_storage.py` & `flet_core-0.9.0.dev1631/src/flet_core/session_storage.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/shader_mask.py` & `flet_core-0.9.0.dev1631/src/flet_core/shader_mask.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/shadow.py` & `flet_core-0.9.0.dev1631/src/flet_core/shadow.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/shake_detector.py` & `flet_core-0.9.0.dev1631/src/flet_core/shake_detector.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/slider.py` & `flet_core-0.9.0.dev1631/src/flet_core/slider.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/snack_bar.py` & `flet_core-0.9.0.dev1631/src/flet_core/snack_bar.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/stack.py` & `flet_core-0.9.0.dev1631/src/flet_core/stack.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/switch.py` & `flet_core-0.9.0.dev1631/src/flet_core/switch.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/tabs.py` & `flet_core-0.9.0.dev1631/src/flet_core/tabs.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/template_route.py` & `flet_core-0.9.0.dev1631/src/flet_core/template_route.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/text.py` & `flet_core-0.9.0.dev1631/src/flet_core/text.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/text_button.py` & `flet_core-0.9.0.dev1631/src/flet_core/text_button.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/text_span.py` & `flet_core-0.9.0.dev1631/src/flet_core/text_span.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/text_style.py` & `flet_core-0.9.0.dev1631/src/flet_core/text_style.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/textfield.py` & `flet_core-0.9.0.dev1631/src/flet_core/textfield.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/theme.py` & `flet_core-0.9.0.dev1631/src/flet_core/theme.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/tooltip.py` & `flet_core-0.9.0.dev1631/src/flet_core/tooltip.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/transform.py` & `flet_core-0.9.0.dev1631/src/flet_core/transform.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/transparent_pointer.py` & `flet_core-0.9.0.dev1631/src/flet_core/transparent_pointer.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/types.py` & `flet_core-0.9.0.dev1631/src/flet_core/types.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/user_control.py` & `flet_core-0.9.0.dev1631/src/flet_core/user_control.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/utils.py` & `flet_core-0.9.0.dev1631/src/flet_core/utils.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/vertical_divider.py` & `flet_core-0.9.0.dev1631/src/flet_core/vertical_divider.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/view.py` & `flet_core-0.9.0.dev1631/src/flet_core/view.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/src/flet_core/window_drag_area.py` & `flet_core-0.9.0.dev1631/src/flet_core/window_drag_area.py`

 * *Files identical despite different names*

### Comparing `flet_core-0.9.0.dev1630/PKG-INFO` & `flet_core-0.9.0.dev1631/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flet-core
-Version: 0.9.0.dev1630
+Version: 0.9.0.dev1631
 Summary: Flet core library
 License: Apache-2.0
 Author: Appveyor Systems Inc.
 Author-email: hello@flet.dev
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

