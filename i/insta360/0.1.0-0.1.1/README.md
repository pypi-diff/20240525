# Comparing `tmp/insta360-0.1.0.tar.gz` & `tmp/insta360-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "insta360-0.1.0.tar", max compression
+gzip compressed data, was "insta360-0.1.1.tar", max compression
```

## Comparing `insta360-0.1.0.tar` & `insta360-0.1.1.tar`

### file list

```diff
@@ -1,127 +1,127 @@
--rw-r--r--   0        0        0    35149 2024-03-25 14:56:57.716565 insta360-0.1.0/LICENSE
--rw-r--r--   0        0        0     8554 2024-05-21 17:23:51.694053 insta360-0.1.0/README.md
--rw-r--r--   0        0        0     8903 2024-05-21 17:23:51.698053 insta360-0.1.0/insta360/osc.py
--rw-r--r--   0        0        0     1943 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/active_sensor_device_pb2.py
--rw-r--r--   0        0        0     1291 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/authorization_operation_type_pb2.py
--rw-r--r--   0        0        0     1882 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/authorization_result_pb2.py
--rw-r--r--   0        0        0     1301 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/battery_low_pb2.py
--rw-r--r--   0        0        0     1849 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/battery_pb2.py
--rw-r--r--   0        0        0     1319 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/battery_update_pb2.py
--rw-r--r--   0        0        0     1396 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/bluetooth_pb2.py
--rw-r--r--   0        0        0     1883 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/bt_central_notification_pb2.py
--rw-r--r--   0        0        0     2228 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/bt_central_pb2.py
--rw-r--r--   0        0        0     1831 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/button_press_params_pb2.py
--rw-r--r--   0        0        0     4820 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/button_press_pb2.py
--rw-r--r--   0        0        0     1174 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/calibrate_gyro_pb2.py
--rw-r--r--   0        0        0     1841 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/camera_posture_pb2.py
--rw-r--r--   0        0        0     1555 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/camera_submode_pb2.py
--rw-r--r--   0        0        0     1835 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/camera_wifi_connection_result_pb2.py
--rw-r--r--   0        0        0     1280 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/cancel_capture_pb2.py
--rw-r--r--   0        0        0     1425 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/cancel_request_authorization_pb2.py
--rw-r--r--   0        0        0     1316 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/capture_auto_split_pb2.py
--rw-r--r--   0        0        0     2569 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/capture_state_pb2.py
--rw-r--r--   0        0        0     2053 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/capture_stopped_pb2.py
--rw-r--r--   0        0        0     2714 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/chargebox_pb2.py
--rw-r--r--   0        0        0     1780 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/charging_command_type_pb2.py
--rw-r--r--   0        0        0     1760 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/check_authorization_pb2.py
--rw-r--r--   0        0        0     1300 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/close_camera_oled_pb2.py
--rw-r--r--   0        0        0     1642 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/current_capture_status_pb2.py
--rw-r--r--   0        0        0     1713 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/darkeis_status_pb2.py
--rw-r--r--   0        0        0     1266 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/delete_file_operation_pb2.py
--rw-r--r--   0        0        0     1345 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/delete_files_pb2.py
--rw-r--r--   0        0        0     1197 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/detect_face_pb2.py
--rw-r--r--   0        0        0     2861 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/download_info_pb2.py
--rw-r--r--   0        0        0     1563 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/error_pb2.py
--rw-r--r--   0        0        0     1625 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/exposure_pb2.py
--rw-r--r--   0        0        0     1546 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/exposure_update_pb2.py
--rw-r--r--   0        0        0    19622 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/extra_info_pb2.py
--rw-r--r--   0        0        0     1246 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/file_type_pb2.py
--rw-r--r--   0        0        0     1387 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/fileinfo_list_pb2.py
--rw-r--r--   0        0        0     1207 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/flicker_pb2.py
--rw-r--r--   0        0        0     2618 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/fw_upgrade_state_pb2.py
--rw-r--r--   0        0        0     1905 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/get_button_press_params_pb2.py
--rw-r--r--   0        0        0     2158 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/get_current_button_status_pb2.py
--rw-r--r--   0        0        0     2009 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/get_current_capture_status_pb2.py
--rw-r--r--   0        0        0     2269 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/get_file_extra_pb2.py
--rw-r--r--   0        0        0     1399 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/get_file_finish_pb2.py
--rw-r--r--   0        0        0     1521 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/get_file_list_pb2.py
--rw-r--r--   0        0        0     1423 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/get_file_pb2.py
--rw-r--r--   0        0        0     1355 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/get_flowstate_enable_pb2.py
--rw-r--r--   0        0        0     1293 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/get_gyro_pb2.py
--rw-r--r--   0        0        0     1189 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/get_mini_thumbnail_pb2.py
--rw-r--r--   0        0        0     1982 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/get_multi_photography_options_pb2.py
--rw-r--r--   0        0        0     1523 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/get_options_pb2.py
--rw-r--r--   0        0        0     1821 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/get_photography_options_pb2.py
--rw-r--r--   0        0        0     1173 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/get_sfr_result_pb2.py
--rw-r--r--   0        0        0     1170 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/get_sfr_status_pb2.py
--rw-r--r--   0        0        0     1486 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/get_sync_capture_mode_pb2.py
--rw-r--r--   0        0        0     1541 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/get_timelapse_options_pb2.py
--rw-r--r--   0        0        0     1540 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/get_whiteblance_status_pb2.py
--rw-r--r--   0        0        0     1525 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/get_wifi_connection_info_pb2.py
--rw-r--r--   0        0        0     1177 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/heat_shell_pb2.py
--rw-r--r--   0        0        0     1520 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/key_pressed_pb2.py
--rw-r--r--   0        0        0     1761 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/live_stream_params_update_pb2.py
--rw-r--r--   0        0        0     2204 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/media_pb2.py
--rw-r--r--   0        0        0    10568 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/message_code_pb2.py
--rw-r--r--   0        0        0     2933 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/multi_photography_options_pb2.py
--rw-r--r--   0        0        0     1634 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/offset_state_pb2.py
--rw-r--r--   0        0        0     1282 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/open_camera_oled_pb2.py
--rw-r--r--   0        0        0     1420 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/open_iperf_service_pb2.py
--rw-r--r--   0        0        0    20380 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/options_pb2.py
--rw-r--r--   0        0        0     2658 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/photo_pb2.py
--rw-r--r--   0        0        0    15011 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/photography_options_pb2.py
--rw-r--r--   0        0        0     1382 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/request_authorization_pb2.py
--rw-r--r--   0        0        0     1435 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/sd_card_speed_pb2.py
--rw-r--r--   0        0        0     2538 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/sensor_pb2.py
--rw-r--r--   0        0        0     1835 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/set_access_camera_file_state_pb2.py
--rw-r--r--   0        0        0     1261 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/set_appid_pb2.py
--rw-r--r--   0        0        0     1894 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/set_button_press_params_pb2.py
--rw-r--r--   0        0        0     1364 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/set_charging_data_pb2.py
--rw-r--r--   0        0        0     1361 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/set_file_extra_pb2.py
--rw-r--r--   0        0        0     1355 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/set_flowstate_enable_pb2.py
--rw-r--r--   0        0        0     1773 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/set_key_time_point_pb2.py
--rw-r--r--   0        0        0     1974 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/set_multi_photography_options_pb2.py
--rw-r--r--   0        0        0     1523 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/set_options_pb2.py
--rw-r--r--   0        0        0     1814 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/set_photography_options_pb2.py
--rw-r--r--   0        0        0     1658 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/set_standby_mode_pb2.py
--rw-r--r--   0        0        0     1488 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/set_sync_capture_mode_pb2.py
--rw-r--r--   0        0        0     1551 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/set_timelapse_options_pb2.py
--rw-r--r--   0        0        0     1526 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/set_wifi_connection_info_pb2.py
--rw-r--r--   0        0        0     1666 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/set_wifi_seize_pb2.py
--rw-r--r--   0        0        0     1515 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/shutdown_pb2.py
--rw-r--r--   0        0        0     1288 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/start_bullettime_pb2.py
--rw-r--r--   0        0        0     1387 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/start_capture_pb2.py
--rw-r--r--   0        0        0     1223 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/start_hdr_pb2.py
--rw-r--r--   0        0        0     2069 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/start_live_stream_pb2.py
--rw-r--r--   0        0        0     1558 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/start_timelapse_pb2.py
--rw-r--r--   0        0        0     1279 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/start_timeshift_pb2.py
--rw-r--r--   0        0        0     1544 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/stop_bullettime_pb2.py
--rw-r--r--   0        0        0     1639 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/stop_capture_pb2.py
--rw-r--r--   0        0        0     1481 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/stop_hdr_pb2.py
--rw-r--r--   0        0        0     1282 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/stop_live_stream_pb2.py
--rw-r--r--   0        0        0     1660 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/stop_timelapse_pb2.py
--rw-r--r--   0        0        0     1533 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/stop_timeshift_pb2.py
--rw-r--r--   0        0        0     1893 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/storage_pb2.py
--rw-r--r--   0        0        0     1364 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/storage_update_pb2.py
--rw-r--r--   0        0        0     1600 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/support_take_photo_on_rec_pb2.py
--rw-r--r--   0        0        0     1637 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/sync_capture_mode_pb2.py
--rw-r--r--   0        0        0     1219 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/sync_capture_mode_update_pb2.py
--rw-r--r--   0        0        0     2406 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/take_picture_pb2.py
--rw-r--r--   0        0        0     1642 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/take_picture_state_update_pb2.py
--rw-r--r--   0        0        0     1523 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/temperature_pb2.py
--rw-r--r--   0        0        0     2180 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/timelapse_pb2.py
--rw-r--r--   0        0        0     1261 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/timelapse_status_update_pb2.py
--rw-r--r--   0        0        0     2097 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/track_pb2.py
--rw-r--r--   0        0        0     1265 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/upload_gps_pb2.py
--rw-r--r--   0        0        0    11289 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/video_pb2.py
--rw-r--r--   0        0        0     1311 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/wifi_connection_info_pb2.py
--rw-r--r--   0        0        0     1388 2024-05-10 09:52:01.809418 insta360-0.1.0/insta360/pb2/window_crop_info_pb2.py
--rw-r--r--   0        0        0    40788 2024-05-21 17:23:51.698053 insta360-0.1.0/insta360/rtmp.py
--rwxr-xr-x   0        0        0     1201 2024-05-10 09:52:01.813417 insta360-0.1.0/insta360/utils/extract-proto-and-compile
--rwxr-xr-x   0        0        0     2905 2024-05-10 09:52:01.813417 insta360-0.1.0/insta360/utils/from_binary.py
--rw-r--r--   0        0        0        0 2024-05-10 09:52:01.813417 insta360-0.1.0/insta360/utils/sample_generator.py
--rw-r--r--   0        0        0     1866 2024-05-10 09:52:01.813417 insta360-0.1.0/insta360/utils/utilities.py
--rw-r--r--   0        0        0    10246 2024-05-10 09:52:01.813417 insta360-0.1.0/insta360/utils/utils/common.py
--rw-r--r--   0        0        0     9109 2024-05-10 09:52:01.813417 insta360-0.1.0/insta360/utils/utils/descpb_to_proto.py
--rw-r--r--   0        0        0      656 2024-05-10 09:52:01.813417 insta360-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     9268 1970-01-01 00:00:00.000000 insta360-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-04 03:41:45.631531 insta360-0.1.1/LICENSE
+-rw-r--r--   0        0        0     8482 2024-05-25 04:48:30.044633 insta360-0.1.1/README.md
+-rw-r--r--   0        0        0     8903 2024-05-16 15:02:41.226638 insta360-0.1.1/insta360/osc.py
+-rw-r--r--   0        0        0     1943 2024-05-01 10:50:12.681873 insta360-0.1.1/insta360/pb2/active_sensor_device_pb2.py
+-rw-r--r--   0        0        0     1291 2024-05-01 10:50:20.662189 insta360-0.1.1/insta360/pb2/authorization_operation_type_pb2.py
+-rw-r--r--   0        0        0     1882 2024-05-01 10:50:29.021668 insta360-0.1.1/insta360/pb2/authorization_result_pb2.py
+-rw-r--r--   0        0        0     1301 2024-05-01 10:50:48.412615 insta360-0.1.1/insta360/pb2/battery_low_pb2.py
+-rw-r--r--   0        0        0     1849 2024-05-01 10:50:56.658868 insta360-0.1.1/insta360/pb2/battery_pb2.py
+-rw-r--r--   0        0        0     1319 2024-05-01 10:51:06.651229 insta360-0.1.1/insta360/pb2/battery_update_pb2.py
+-rw-r--r--   0        0        0     1396 2024-05-01 10:51:11.451195 insta360-0.1.1/insta360/pb2/bluetooth_pb2.py
+-rw-r--r--   0        0        0     1883 2024-05-01 10:51:24.697612 insta360-0.1.1/insta360/pb2/bt_central_notification_pb2.py
+-rw-r--r--   0        0        0     2228 2024-05-01 10:51:31.074396 insta360-0.1.1/insta360/pb2/bt_central_pb2.py
+-rw-r--r--   0        0        0     1831 2024-05-01 10:51:40.861665 insta360-0.1.1/insta360/pb2/button_press_params_pb2.py
+-rw-r--r--   0        0        0     4820 2024-05-01 10:51:46.272134 insta360-0.1.1/insta360/pb2/button_press_pb2.py
+-rw-r--r--   0        0        0     1174 2024-05-01 10:51:50.121425 insta360-0.1.1/insta360/pb2/calibrate_gyro_pb2.py
+-rw-r--r--   0        0        0     1841 2024-05-01 10:51:54.287953 insta360-0.1.1/insta360/pb2/camera_posture_pb2.py
+-rw-r--r--   0        0        0     1555 2024-05-01 10:52:07.223882 insta360-0.1.1/insta360/pb2/camera_submode_pb2.py
+-rw-r--r--   0        0        0     1835 2024-05-01 10:52:18.299970 insta360-0.1.1/insta360/pb2/camera_wifi_connection_result_pb2.py
+-rw-r--r--   0        0        0     1280 2024-05-01 10:52:23.968146 insta360-0.1.1/insta360/pb2/cancel_capture_pb2.py
+-rw-r--r--   0        0        0     1425 2024-05-01 10:52:34.212111 insta360-0.1.1/insta360/pb2/cancel_request_authorization_pb2.py
+-rw-r--r--   0        0        0     1316 2024-05-01 10:53:06.874531 insta360-0.1.1/insta360/pb2/capture_auto_split_pb2.py
+-rw-r--r--   0        0        0     2569 2024-05-01 10:53:10.537207 insta360-0.1.1/insta360/pb2/capture_state_pb2.py
+-rw-r--r--   0        0        0     2053 2024-05-01 10:53:16.076323 insta360-0.1.1/insta360/pb2/capture_stopped_pb2.py
+-rw-r--r--   0        0        0     2714 2024-05-01 10:40:12.307158 insta360-0.1.1/insta360/pb2/chargebox_pb2.py
+-rw-r--r--   0        0        0     1780 2024-05-01 10:53:26.951801 insta360-0.1.1/insta360/pb2/charging_command_type_pb2.py
+-rw-r--r--   0        0        0     1760 2024-05-01 10:53:33.450395 insta360-0.1.1/insta360/pb2/check_authorization_pb2.py
+-rw-r--r--   0        0        0     1300 2024-05-01 10:53:36.349880 insta360-0.1.1/insta360/pb2/close_camera_oled_pb2.py
+-rw-r--r--   0        0        0     1642 2024-05-01 10:35:12.928867 insta360-0.1.1/insta360/pb2/current_capture_status_pb2.py
+-rw-r--r--   0        0        0     1713 2024-05-01 10:53:43.286030 insta360-0.1.1/insta360/pb2/darkeis_status_pb2.py
+-rw-r--r--   0        0        0     1266 2024-05-01 10:53:46.176908 insta360-0.1.1/insta360/pb2/delete_file_operation_pb2.py
+-rw-r--r--   0        0        0     1345 2024-05-01 10:53:49.663118 insta360-0.1.1/insta360/pb2/delete_files_pb2.py
+-rw-r--r--   0        0        0     1197 2024-05-01 10:53:53.286506 insta360-0.1.1/insta360/pb2/detect_face_pb2.py
+-rw-r--r--   0        0        0     2861 2024-05-01 10:53:56.326069 insta360-0.1.1/insta360/pb2/download_info_pb2.py
+-rw-r--r--   0        0        0     1563 2024-05-01 10:53:59.213902 insta360-0.1.1/insta360/pb2/error_pb2.py
+-rw-r--r--   0        0        0     1625 2024-05-01 10:54:02.136759 insta360-0.1.1/insta360/pb2/exposure_pb2.py
+-rw-r--r--   0        0        0     1546 2024-05-01 10:54:10.425974 insta360-0.1.1/insta360/pb2/exposure_update_pb2.py
+-rw-r--r--   0        0        0    19622 2024-05-01 10:38:25.693362 insta360-0.1.1/insta360/pb2/extra_info_pb2.py
+-rw-r--r--   0        0        0     1246 2024-05-01 10:54:19.589726 insta360-0.1.1/insta360/pb2/file_type_pb2.py
+-rw-r--r--   0        0        0     1387 2024-05-01 10:54:24.100896 insta360-0.1.1/insta360/pb2/fileinfo_list_pb2.py
+-rw-r--r--   0        0        0     1207 2024-05-01 10:54:27.788730 insta360-0.1.1/insta360/pb2/flicker_pb2.py
+-rw-r--r--   0        0        0     2618 2024-05-01 10:54:30.337360 insta360-0.1.1/insta360/pb2/fw_upgrade_state_pb2.py
+-rw-r--r--   0        0        0     1905 2024-05-01 10:54:41.142304 insta360-0.1.1/insta360/pb2/get_button_press_params_pb2.py
+-rw-r--r--   0        0        0     2158 2024-05-01 10:54:48.016043 insta360-0.1.1/insta360/pb2/get_current_button_status_pb2.py
+-rw-r--r--   0        0        0     2009 2024-05-01 10:35:29.990254 insta360-0.1.1/insta360/pb2/get_current_capture_status_pb2.py
+-rw-r--r--   0        0        0     2269 2024-05-01 10:54:59.833141 insta360-0.1.1/insta360/pb2/get_file_extra_pb2.py
+-rw-r--r--   0        0        0     1399 2024-05-01 10:55:10.377566 insta360-0.1.1/insta360/pb2/get_file_finish_pb2.py
+-rw-r--r--   0        0        0     1521 2024-05-01 10:35:40.840306 insta360-0.1.1/insta360/pb2/get_file_list_pb2.py
+-rw-r--r--   0        0        0     1423 2024-05-01 10:55:21.292648 insta360-0.1.1/insta360/pb2/get_file_pb2.py
+-rw-r--r--   0        0        0     1355 2024-05-01 10:55:28.756126 insta360-0.1.1/insta360/pb2/get_flowstate_enable_pb2.py
+-rw-r--r--   0        0        0     1293 2024-05-01 10:55:31.527965 insta360-0.1.1/insta360/pb2/get_gyro_pb2.py
+-rw-r--r--   0        0        0     1189 2024-05-01 10:55:34.139465 insta360-0.1.1/insta360/pb2/get_mini_thumbnail_pb2.py
+-rw-r--r--   0        0        0     1982 2024-05-01 10:55:47.589405 insta360-0.1.1/insta360/pb2/get_multi_photography_options_pb2.py
+-rw-r--r--   0        0        0     1523 2024-05-01 10:35:56.890582 insta360-0.1.1/insta360/pb2/get_options_pb2.py
+-rw-r--r--   0        0        0     1821 2024-05-01 10:36:28.690470 insta360-0.1.1/insta360/pb2/get_photography_options_pb2.py
+-rw-r--r--   0        0        0     1173 2024-05-01 10:55:57.284321 insta360-0.1.1/insta360/pb2/get_sfr_result_pb2.py
+-rw-r--r--   0        0        0     1170 2024-05-01 10:56:00.214851 insta360-0.1.1/insta360/pb2/get_sfr_status_pb2.py
+-rw-r--r--   0        0        0     1486 2024-05-01 10:56:05.328923 insta360-0.1.1/insta360/pb2/get_sync_capture_mode_pb2.py
+-rw-r--r--   0        0        0     1541 2024-05-01 10:56:11.254301 insta360-0.1.1/insta360/pb2/get_timelapse_options_pb2.py
+-rw-r--r--   0        0        0     1540 2024-05-01 10:56:14.189618 insta360-0.1.1/insta360/pb2/get_whiteblance_status_pb2.py
+-rw-r--r--   0        0        0     1525 2024-05-01 10:56:21.091509 insta360-0.1.1/insta360/pb2/get_wifi_connection_info_pb2.py
+-rw-r--r--   0        0        0     1177 2024-05-01 10:56:25.324176 insta360-0.1.1/insta360/pb2/heat_shell_pb2.py
+-rw-r--r--   0        0        0     1520 2024-05-01 10:56:28.703111 insta360-0.1.1/insta360/pb2/key_pressed_pb2.py
+-rw-r--r--   0        0        0     1761 2024-05-01 10:56:36.781540 insta360-0.1.1/insta360/pb2/live_stream_params_update_pb2.py
+-rw-r--r--   0        0        0     2204 2024-05-01 10:56:44.591866 insta360-0.1.1/insta360/pb2/media_pb2.py
+-rw-r--r--   0        0        0    10568 2024-05-01 10:56:47.229315 insta360-0.1.1/insta360/pb2/message_code_pb2.py
+-rw-r--r--   0        0        0     2933 2024-05-01 10:56:56.395851 insta360-0.1.1/insta360/pb2/multi_photography_options_pb2.py
+-rw-r--r--   0        0        0     1634 2024-05-01 10:57:02.018278 insta360-0.1.1/insta360/pb2/offset_state_pb2.py
+-rw-r--r--   0        0        0     1282 2024-05-01 10:57:04.653166 insta360-0.1.1/insta360/pb2/open_camera_oled_pb2.py
+-rw-r--r--   0        0        0     1420 2024-05-01 10:57:06.702051 insta360-0.1.1/insta360/pb2/open_iperf_service_pb2.py
+-rw-r--r--   0        0        0    20380 2024-05-01 10:36:12.664976 insta360-0.1.1/insta360/pb2/options_pb2.py
+-rw-r--r--   0        0        0     2658 2024-05-01 10:57:11.378423 insta360-0.1.1/insta360/pb2/photo_pb2.py
+-rw-r--r--   0        0        0    15011 2024-05-01 10:37:27.346713 insta360-0.1.1/insta360/pb2/photography_options_pb2.py
+-rw-r--r--   0        0        0     1382 2024-05-01 10:57:19.454492 insta360-0.1.1/insta360/pb2/request_authorization_pb2.py
+-rw-r--r--   0        0        0     1435 2024-05-01 10:57:22.381055 insta360-0.1.1/insta360/pb2/sd_card_speed_pb2.py
+-rw-r--r--   0        0        0     2538 2024-05-01 10:57:25.379604 insta360-0.1.1/insta360/pb2/sensor_pb2.py
+-rw-r--r--   0        0        0     1835 2024-05-01 10:58:46.219095 insta360-0.1.1/insta360/pb2/set_access_camera_file_state_pb2.py
+-rw-r--r--   0        0        0     1261 2024-05-01 10:58:49.306111 insta360-0.1.1/insta360/pb2/set_appid_pb2.py
+-rw-r--r--   0        0        0     1894 2024-05-01 10:59:01.982856 insta360-0.1.1/insta360/pb2/set_button_press_params_pb2.py
+-rw-r--r--   0        0        0     1364 2024-05-01 10:59:05.895492 insta360-0.1.1/insta360/pb2/set_charging_data_pb2.py
+-rw-r--r--   0        0        0     1361 2024-05-01 10:59:12.870230 insta360-0.1.1/insta360/pb2/set_file_extra_pb2.py
+-rw-r--r--   0        0        0     1355 2024-05-01 10:59:15.955263 insta360-0.1.1/insta360/pb2/set_flowstate_enable_pb2.py
+-rw-r--r--   0        0        0     1773 2024-05-01 10:59:31.620109 insta360-0.1.1/insta360/pb2/set_key_time_point_pb2.py
+-rw-r--r--   0        0        0     1974 2024-05-01 10:59:42.193248 insta360-0.1.1/insta360/pb2/set_multi_photography_options_pb2.py
+-rw-r--r--   0        0        0     1523 2024-05-01 10:37:05.071548 insta360-0.1.1/insta360/pb2/set_options_pb2.py
+-rw-r--r--   0        0        0     1814 2024-05-01 10:37:18.716658 insta360-0.1.1/insta360/pb2/set_photography_options_pb2.py
+-rw-r--r--   0        0        0     1658 2024-05-01 10:59:52.258481 insta360-0.1.1/insta360/pb2/set_standby_mode_pb2.py
+-rw-r--r--   0        0        0     1488 2024-05-01 10:59:59.444033 insta360-0.1.1/insta360/pb2/set_sync_capture_mode_pb2.py
+-rw-r--r--   0        0        0     1551 2024-05-01 11:00:08.583501 insta360-0.1.1/insta360/pb2/set_timelapse_options_pb2.py
+-rw-r--r--   0        0        0     1526 2024-05-01 11:00:15.710818 insta360-0.1.1/insta360/pb2/set_wifi_connection_info_pb2.py
+-rw-r--r--   0        0        0     1666 2024-05-01 11:00:21.319696 insta360-0.1.1/insta360/pb2/set_wifi_seize_pb2.py
+-rw-r--r--   0        0        0     1515 2024-05-01 11:00:23.544335 insta360-0.1.1/insta360/pb2/shutdown_pb2.py
+-rw-r--r--   0        0        0     1288 2024-05-01 11:00:25.880369 insta360-0.1.1/insta360/pb2/start_bullettime_pb2.py
+-rw-r--r--   0        0        0     1387 2024-05-01 10:37:46.770429 insta360-0.1.1/insta360/pb2/start_capture_pb2.py
+-rw-r--r--   0        0        0     1223 2024-05-01 11:00:31.256703 insta360-0.1.1/insta360/pb2/start_hdr_pb2.py
+-rw-r--r--   0        0        0     2069 2024-05-01 10:37:59.241339 insta360-0.1.1/insta360/pb2/start_live_stream_pb2.py
+-rw-r--r--   0        0        0     1558 2024-05-01 11:00:42.022507 insta360-0.1.1/insta360/pb2/start_timelapse_pb2.py
+-rw-r--r--   0        0        0     1279 2024-05-01 11:00:46.209544 insta360-0.1.1/insta360/pb2/start_timeshift_pb2.py
+-rw-r--r--   0        0        0     1544 2024-05-01 11:00:53.784248 insta360-0.1.1/insta360/pb2/stop_bullettime_pb2.py
+-rw-r--r--   0        0        0     1639 2024-05-01 10:38:17.616363 insta360-0.1.1/insta360/pb2/stop_capture_pb2.py
+-rw-r--r--   0        0        0     1481 2024-05-01 11:01:03.671890 insta360-0.1.1/insta360/pb2/stop_hdr_pb2.py
+-rw-r--r--   0        0        0     1282 2024-05-01 11:01:07.691655 insta360-0.1.1/insta360/pb2/stop_live_stream_pb2.py
+-rw-r--r--   0        0        0     1660 2024-05-01 11:01:14.683543 insta360-0.1.1/insta360/pb2/stop_timelapse_pb2.py
+-rw-r--r--   0        0        0     1533 2024-05-01 11:01:21.349310 insta360-0.1.1/insta360/pb2/stop_timeshift_pb2.py
+-rw-r--r--   0        0        0     1893 2024-05-01 11:01:24.870213 insta360-0.1.1/insta360/pb2/storage_pb2.py
+-rw-r--r--   0        0        0     1364 2024-05-01 10:38:54.268715 insta360-0.1.1/insta360/pb2/storage_update_pb2.py
+-rw-r--r--   0        0        0     1600 2024-05-01 11:01:31.020593 insta360-0.1.1/insta360/pb2/support_take_photo_on_rec_pb2.py
+-rw-r--r--   0        0        0     1637 2024-05-01 11:01:33.836310 insta360-0.1.1/insta360/pb2/sync_capture_mode_pb2.py
+-rw-r--r--   0        0        0     1219 2024-05-01 11:01:36.395495 insta360-0.1.1/insta360/pb2/sync_capture_mode_update_pb2.py
+-rw-r--r--   0        0        0     2406 2024-05-01 10:39:07.401562 insta360-0.1.1/insta360/pb2/take_picture_pb2.py
+-rw-r--r--   0        0        0     1642 2024-05-01 11:01:40.486974 insta360-0.1.1/insta360/pb2/take_picture_state_update_pb2.py
+-rw-r--r--   0        0        0     1523 2024-05-01 11:01:43.025082 insta360-0.1.1/insta360/pb2/temperature_pb2.py
+-rw-r--r--   0        0        0     2180 2024-05-01 11:01:45.397424 insta360-0.1.1/insta360/pb2/timelapse_pb2.py
+-rw-r--r--   0        0        0     1261 2024-05-01 11:01:47.999757 insta360-0.1.1/insta360/pb2/timelapse_status_update_pb2.py
+-rw-r--r--   0        0        0     2097 2024-05-01 11:01:52.964411 insta360-0.1.1/insta360/pb2/track_pb2.py
+-rw-r--r--   0        0        0     1265 2024-05-01 11:01:56.219978 insta360-0.1.1/insta360/pb2/upload_gps_pb2.py
+-rw-r--r--   0        0        0    11289 2024-05-01 11:01:58.423712 insta360-0.1.1/insta360/pb2/video_pb2.py
+-rw-r--r--   0        0        0     1311 2024-05-01 11:02:00.633715 insta360-0.1.1/insta360/pb2/wifi_connection_info_pb2.py
+-rw-r--r--   0        0        0     1388 2024-05-01 11:02:03.085155 insta360-0.1.1/insta360/pb2/window_crop_info_pb2.py
+-rw-r--r--   0        0        0    40788 2024-05-20 14:05:19.901838 insta360-0.1.1/insta360/rtmp.py
+-rwxr-xr-x   0        0        0     1201 2024-04-04 03:41:45.644511 insta360-0.1.1/insta360/utils/extract-proto-and-compile
+-rwxr-xr-x   0        0        0     2905 2024-04-04 03:41:45.644595 insta360-0.1.1/insta360/utils/from_binary.py
+-rw-r--r--   0        0        0        0 2024-05-01 08:07:40.055776 insta360-0.1.1/insta360/utils/sample_generator.py
+-rw-r--r--   0        0        0     1866 2024-05-01 10:19:08.047071 insta360-0.1.1/insta360/utils/utilities.py
+-rw-r--r--   0        0        0    10246 2024-04-04 03:41:45.644729 insta360-0.1.1/insta360/utils/utils/common.py
+-rw-r--r--   0        0        0     9109 2024-04-04 03:41:45.644828 insta360-0.1.1/insta360/utils/utils/descpb_to_proto.py
+-rw-r--r--   0        0        0      656 2024-05-25 04:53:54.323322 insta360-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     9247 1970-01-01 00:00:00.000000 insta360-0.1.1/PKG-INFO
```

### Comparing `insta360-0.1.0/LICENSE` & `insta360-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/README.md` & `insta360-0.1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -60,27 +60,28 @@
 | get_options      |     ❌      | ❌  | ❌  |
 | reset            |     ❌      | ❌  | ❌  |
 | switch_wifi      |     ❌      | ❌  | ❌  |
 | upload_file      |     ❌      | ❌  | ❌  |
 
 # Installation
 
-Currently, the package is not available on PyPi. To install the package, clone the repository and run the following command:
+To install the package, run the following command:
 
-1. Make sure [poetry](https://python-poetry.org/docs/#installation) is installed.
-2. Run: `poetry config virtualenvs.in-project true`
-3. Ensure you are using supported python version (3.8 and above): `poetry env use 3.8`
-4. Run: `poetry install`
+```bash
+pip install insta360
+```
 
 # Usage
 
 First make sure you are [connected](#connecting-to-the-wifi) to the camera's WiFi network.
 
 The package provides two modules, `rtmp` and `osc`, for interacting with Insta360 cameras using RTMP and OSC protocols, respectively. OSC being an open standard, could be considered as more reliable and stable compared to RTMP. However, RTMP provides some functionalities that are not available in OSC. Depending on your use case, you can choose to use either of the modules.
 
+Below are some examples of how to use the `rtmp` and `osc` modules. For more detailed information, refer to the [documentation](https://insta360.whitebox.aero).
+
 Here is an example of how to use the `rtmp` module:
 
 ```python
 import time
 from insta360.rtmp import Client
 
 # Create an RTMP client
@@ -165,15 +166,15 @@
 # Start recording
 python3 insta360_cmd -c capture
 
 # Know all the options
 python3 insta360_cmd -h
 ```
 
-![insta360_cmd screenshot](assets/insta360_cmd.jpg "insta360_cmd screenshot")
+![insta360_cmd screenshot](https://gitlab.com/whitebox-aero/insta360/-/raw/main/assets/insta360_cmd.jpg "insta360_cmd screenshot")
 
 ## Docs
 
 Documentation is auto-generated generated with [MkDocs](https://www.mkdocs.org/). While contributing, make sure to follow [google docstring conventions](https://mkdocstrings.github.io/griffe/docstrings/#google-style) when documenting the code.
 
 To generate the docs, first install the required packages:
```

### Comparing `insta360-0.1.0/insta360/osc.py` & `insta360-0.1.1/insta360/osc.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/active_sensor_device_pb2.py` & `insta360-0.1.1/insta360/pb2/active_sensor_device_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/authorization_operation_type_pb2.py` & `insta360-0.1.1/insta360/pb2/authorization_operation_type_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/authorization_result_pb2.py` & `insta360-0.1.1/insta360/pb2/authorization_result_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/battery_low_pb2.py` & `insta360-0.1.1/insta360/pb2/battery_low_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/battery_pb2.py` & `insta360-0.1.1/insta360/pb2/battery_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/battery_update_pb2.py` & `insta360-0.1.1/insta360/pb2/battery_update_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/bluetooth_pb2.py` & `insta360-0.1.1/insta360/pb2/bluetooth_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/bt_central_notification_pb2.py` & `insta360-0.1.1/insta360/pb2/bt_central_notification_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/bt_central_pb2.py` & `insta360-0.1.1/insta360/pb2/bt_central_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/button_press_params_pb2.py` & `insta360-0.1.1/insta360/pb2/button_press_params_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/button_press_pb2.py` & `insta360-0.1.1/insta360/pb2/button_press_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/calibrate_gyro_pb2.py` & `insta360-0.1.1/insta360/pb2/calibrate_gyro_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/camera_posture_pb2.py` & `insta360-0.1.1/insta360/pb2/camera_posture_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/camera_submode_pb2.py` & `insta360-0.1.1/insta360/pb2/camera_submode_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/camera_wifi_connection_result_pb2.py` & `insta360-0.1.1/insta360/pb2/camera_wifi_connection_result_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/cancel_capture_pb2.py` & `insta360-0.1.1/insta360/pb2/cancel_capture_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/cancel_request_authorization_pb2.py` & `insta360-0.1.1/insta360/pb2/cancel_request_authorization_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/capture_auto_split_pb2.py` & `insta360-0.1.1/insta360/pb2/capture_auto_split_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/capture_state_pb2.py` & `insta360-0.1.1/insta360/pb2/capture_state_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/capture_stopped_pb2.py` & `insta360-0.1.1/insta360/pb2/capture_stopped_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/chargebox_pb2.py` & `insta360-0.1.1/insta360/pb2/chargebox_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/charging_command_type_pb2.py` & `insta360-0.1.1/insta360/pb2/charging_command_type_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/check_authorization_pb2.py` & `insta360-0.1.1/insta360/pb2/check_authorization_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/close_camera_oled_pb2.py` & `insta360-0.1.1/insta360/pb2/close_camera_oled_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/current_capture_status_pb2.py` & `insta360-0.1.1/insta360/pb2/current_capture_status_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/darkeis_status_pb2.py` & `insta360-0.1.1/insta360/pb2/darkeis_status_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/delete_file_operation_pb2.py` & `insta360-0.1.1/insta360/pb2/delete_file_operation_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/delete_files_pb2.py` & `insta360-0.1.1/insta360/pb2/delete_files_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/detect_face_pb2.py` & `insta360-0.1.1/insta360/pb2/detect_face_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/download_info_pb2.py` & `insta360-0.1.1/insta360/pb2/download_info_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/error_pb2.py` & `insta360-0.1.1/insta360/pb2/error_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/exposure_pb2.py` & `insta360-0.1.1/insta360/pb2/exposure_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/exposure_update_pb2.py` & `insta360-0.1.1/insta360/pb2/exposure_update_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/extra_info_pb2.py` & `insta360-0.1.1/insta360/pb2/extra_info_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/file_type_pb2.py` & `insta360-0.1.1/insta360/pb2/file_type_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/fileinfo_list_pb2.py` & `insta360-0.1.1/insta360/pb2/fileinfo_list_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/flicker_pb2.py` & `insta360-0.1.1/insta360/pb2/flicker_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/fw_upgrade_state_pb2.py` & `insta360-0.1.1/insta360/pb2/fw_upgrade_state_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/get_button_press_params_pb2.py` & `insta360-0.1.1/insta360/pb2/get_button_press_params_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/get_current_button_status_pb2.py` & `insta360-0.1.1/insta360/pb2/get_current_button_status_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/get_current_capture_status_pb2.py` & `insta360-0.1.1/insta360/pb2/get_current_capture_status_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/get_file_extra_pb2.py` & `insta360-0.1.1/insta360/pb2/get_file_extra_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/get_file_finish_pb2.py` & `insta360-0.1.1/insta360/pb2/get_file_finish_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/get_file_list_pb2.py` & `insta360-0.1.1/insta360/pb2/get_file_list_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/get_file_pb2.py` & `insta360-0.1.1/insta360/pb2/get_file_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/get_flowstate_enable_pb2.py` & `insta360-0.1.1/insta360/pb2/get_flowstate_enable_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/get_gyro_pb2.py` & `insta360-0.1.1/insta360/pb2/get_gyro_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/get_mini_thumbnail_pb2.py` & `insta360-0.1.1/insta360/pb2/get_mini_thumbnail_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/get_multi_photography_options_pb2.py` & `insta360-0.1.1/insta360/pb2/get_multi_photography_options_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/get_options_pb2.py` & `insta360-0.1.1/insta360/pb2/get_options_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/get_photography_options_pb2.py` & `insta360-0.1.1/insta360/pb2/get_photography_options_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/get_sfr_result_pb2.py` & `insta360-0.1.1/insta360/pb2/get_sfr_result_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/get_sfr_status_pb2.py` & `insta360-0.1.1/insta360/pb2/get_sfr_status_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/get_sync_capture_mode_pb2.py` & `insta360-0.1.1/insta360/pb2/get_sync_capture_mode_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/get_timelapse_options_pb2.py` & `insta360-0.1.1/insta360/pb2/get_timelapse_options_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/get_whiteblance_status_pb2.py` & `insta360-0.1.1/insta360/pb2/get_whiteblance_status_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/get_wifi_connection_info_pb2.py` & `insta360-0.1.1/insta360/pb2/get_wifi_connection_info_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/heat_shell_pb2.py` & `insta360-0.1.1/insta360/pb2/heat_shell_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/key_pressed_pb2.py` & `insta360-0.1.1/insta360/pb2/key_pressed_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/live_stream_params_update_pb2.py` & `insta360-0.1.1/insta360/pb2/live_stream_params_update_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/media_pb2.py` & `insta360-0.1.1/insta360/pb2/media_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/message_code_pb2.py` & `insta360-0.1.1/insta360/pb2/message_code_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/multi_photography_options_pb2.py` & `insta360-0.1.1/insta360/pb2/multi_photography_options_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/offset_state_pb2.py` & `insta360-0.1.1/insta360/pb2/offset_state_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/open_camera_oled_pb2.py` & `insta360-0.1.1/insta360/pb2/open_camera_oled_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/open_iperf_service_pb2.py` & `insta360-0.1.1/insta360/pb2/open_iperf_service_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/options_pb2.py` & `insta360-0.1.1/insta360/pb2/options_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/photo_pb2.py` & `insta360-0.1.1/insta360/pb2/photo_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/photography_options_pb2.py` & `insta360-0.1.1/insta360/pb2/photography_options_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/request_authorization_pb2.py` & `insta360-0.1.1/insta360/pb2/request_authorization_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/sd_card_speed_pb2.py` & `insta360-0.1.1/insta360/pb2/sd_card_speed_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/sensor_pb2.py` & `insta360-0.1.1/insta360/pb2/sensor_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/set_access_camera_file_state_pb2.py` & `insta360-0.1.1/insta360/pb2/set_access_camera_file_state_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/set_appid_pb2.py` & `insta360-0.1.1/insta360/pb2/set_appid_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/set_button_press_params_pb2.py` & `insta360-0.1.1/insta360/pb2/set_button_press_params_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/set_charging_data_pb2.py` & `insta360-0.1.1/insta360/pb2/set_charging_data_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/set_file_extra_pb2.py` & `insta360-0.1.1/insta360/pb2/set_file_extra_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/set_flowstate_enable_pb2.py` & `insta360-0.1.1/insta360/pb2/set_flowstate_enable_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/set_key_time_point_pb2.py` & `insta360-0.1.1/insta360/pb2/set_key_time_point_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/set_multi_photography_options_pb2.py` & `insta360-0.1.1/insta360/pb2/set_multi_photography_options_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/set_options_pb2.py` & `insta360-0.1.1/insta360/pb2/set_options_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/set_photography_options_pb2.py` & `insta360-0.1.1/insta360/pb2/set_photography_options_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/set_standby_mode_pb2.py` & `insta360-0.1.1/insta360/pb2/set_standby_mode_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/set_sync_capture_mode_pb2.py` & `insta360-0.1.1/insta360/pb2/set_sync_capture_mode_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/set_timelapse_options_pb2.py` & `insta360-0.1.1/insta360/pb2/set_timelapse_options_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/set_wifi_connection_info_pb2.py` & `insta360-0.1.1/insta360/pb2/set_wifi_connection_info_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/set_wifi_seize_pb2.py` & `insta360-0.1.1/insta360/pb2/set_wifi_seize_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/shutdown_pb2.py` & `insta360-0.1.1/insta360/pb2/shutdown_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/start_bullettime_pb2.py` & `insta360-0.1.1/insta360/pb2/start_bullettime_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/start_capture_pb2.py` & `insta360-0.1.1/insta360/pb2/start_capture_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/start_hdr_pb2.py` & `insta360-0.1.1/insta360/pb2/start_hdr_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/start_live_stream_pb2.py` & `insta360-0.1.1/insta360/pb2/start_live_stream_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/start_timelapse_pb2.py` & `insta360-0.1.1/insta360/pb2/start_timelapse_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/start_timeshift_pb2.py` & `insta360-0.1.1/insta360/pb2/start_timeshift_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/stop_bullettime_pb2.py` & `insta360-0.1.1/insta360/pb2/stop_bullettime_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/stop_capture_pb2.py` & `insta360-0.1.1/insta360/pb2/stop_capture_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/stop_hdr_pb2.py` & `insta360-0.1.1/insta360/pb2/stop_hdr_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/stop_live_stream_pb2.py` & `insta360-0.1.1/insta360/pb2/stop_live_stream_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/stop_timelapse_pb2.py` & `insta360-0.1.1/insta360/pb2/stop_timelapse_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/stop_timeshift_pb2.py` & `insta360-0.1.1/insta360/pb2/stop_timeshift_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/storage_pb2.py` & `insta360-0.1.1/insta360/pb2/storage_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/storage_update_pb2.py` & `insta360-0.1.1/insta360/pb2/storage_update_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/support_take_photo_on_rec_pb2.py` & `insta360-0.1.1/insta360/pb2/support_take_photo_on_rec_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/sync_capture_mode_pb2.py` & `insta360-0.1.1/insta360/pb2/sync_capture_mode_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/sync_capture_mode_update_pb2.py` & `insta360-0.1.1/insta360/pb2/sync_capture_mode_update_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/take_picture_pb2.py` & `insta360-0.1.1/insta360/pb2/take_picture_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/take_picture_state_update_pb2.py` & `insta360-0.1.1/insta360/pb2/take_picture_state_update_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/temperature_pb2.py` & `insta360-0.1.1/insta360/pb2/temperature_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/timelapse_pb2.py` & `insta360-0.1.1/insta360/pb2/timelapse_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/timelapse_status_update_pb2.py` & `insta360-0.1.1/insta360/pb2/timelapse_status_update_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/track_pb2.py` & `insta360-0.1.1/insta360/pb2/track_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/upload_gps_pb2.py` & `insta360-0.1.1/insta360/pb2/upload_gps_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/video_pb2.py` & `insta360-0.1.1/insta360/pb2/video_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/wifi_connection_info_pb2.py` & `insta360-0.1.1/insta360/pb2/wifi_connection_info_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/pb2/window_crop_info_pb2.py` & `insta360-0.1.1/insta360/pb2/window_crop_info_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/rtmp.py` & `insta360-0.1.1/insta360/rtmp.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/utils/extract-proto-and-compile` & `insta360-0.1.1/insta360/utils/extract-proto-and-compile`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/utils/from_binary.py` & `insta360-0.1.1/insta360/utils/from_binary.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/utils/utilities.py` & `insta360-0.1.1/insta360/utils/utilities.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/utils/utils/common.py` & `insta360-0.1.1/insta360/utils/utils/common.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/insta360/utils/utils/descpb_to_proto.py` & `insta360-0.1.1/insta360/utils/utils/descpb_to_proto.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.0/pyproject.toml` & `insta360-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "insta360"
-version = "0.1.0"
+version = "0.1.1"
 description = "APIs to interact with insta360 cameras."
 authors = ["avilabss <contact@avilabs.net>", "Niccolo Rigacci <niccolo@rigacci.org>", "WhiteBox <contact@whitebox.aero>"]
 license = "GNU General Public License v3.0 or later"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8.0"
```

### Comparing `insta360-0.1.0/PKG-INFO` & `insta360-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: insta360
-Version: 0.1.0
+Version: 0.1.1
 Summary: APIs to interact with insta360 cameras.
 License: GPL-3.0-or-later
 Author: avilabss
 Author-email: contact@avilabs.net
 Requires-Python: >=3.8.0,<4.0.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: protobuf (>=5.26.1,<6.0.0)
 Requires-Dist: pydantic (>=2.7.1,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # insta360-api
 
@@ -79,27 +80,28 @@
 | get_options      |     ❌      | ❌  | ❌  |
 | reset            |     ❌      | ❌  | ❌  |
 | switch_wifi      |     ❌      | ❌  | ❌  |
 | upload_file      |     ❌      | ❌  | ❌  |
 
 # Installation
 
-Currently, the package is not available on PyPi. To install the package, clone the repository and run the following command:
+To install the package, run the following command:
 
-1. Make sure [poetry](https://python-poetry.org/docs/#installation) is installed.
-2. Run: `poetry config virtualenvs.in-project true`
-3. Ensure you are using supported python version (3.8 and above): `poetry env use 3.8`
-4. Run: `poetry install`
+```bash
+pip install insta360
+```
 
 # Usage
 
 First make sure you are [connected](#connecting-to-the-wifi) to the camera's WiFi network.
 
 The package provides two modules, `rtmp` and `osc`, for interacting with Insta360 cameras using RTMP and OSC protocols, respectively. OSC being an open standard, could be considered as more reliable and stable compared to RTMP. However, RTMP provides some functionalities that are not available in OSC. Depending on your use case, you can choose to use either of the modules.
 
+Below are some examples of how to use the `rtmp` and `osc` modules. For more detailed information, refer to the [documentation](https://insta360.whitebox.aero).
+
 Here is an example of how to use the `rtmp` module:
 
 ```python
 import time
 from insta360.rtmp import Client
 
 # Create an RTMP client
@@ -184,15 +186,15 @@
 # Start recording
 python3 insta360_cmd -c capture
 
 # Know all the options
 python3 insta360_cmd -h
 ```
 
-![insta360_cmd screenshot](assets/insta360_cmd.jpg "insta360_cmd screenshot")
+![insta360_cmd screenshot](https://gitlab.com/whitebox-aero/insta360/-/raw/main/assets/insta360_cmd.jpg "insta360_cmd screenshot")
 
 ## Docs
 
 Documentation is auto-generated generated with [MkDocs](https://www.mkdocs.org/). While contributing, make sure to follow [google docstring conventions](https://mkdocstrings.github.io/griffe/docstrings/#google-style) when documenting the code.
 
 To generate the docs, first install the required packages:
```

