# Comparing `tmp/ourskyai_astro_api-1.3.3668.tar.gz` & `tmp/ourskyai_astro_api-1.3.3671.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ourskyai_astro_api-1.3.3668.tar", max compression
+gzip compressed data, was "ourskyai_astro_api-1.3.3671.tar", max compression
```

## Comparing `ourskyai_astro_api-1.3.3668.tar` & `ourskyai_astro_api-1.3.3671.tar`

### file list

```diff
@@ -1,78 +1,78 @@
--rw-r--r--   0        0        0    11541 2024-05-24 20:17:11.128959 ourskyai_astro_api-1.3.3668/README.md
--rw-r--r--   0        0        0     6292 2024-05-24 20:17:15.261006 ourskyai_astro_api-1.3.3668/ourskyai_astro_api/__init__.py
--rw-r--r--   0        0        0      106 2024-05-24 20:17:15.289006 ourskyai_astro_api-1.3.3668/ourskyai_astro_api/api/__init__.py
--rw-r--r--   0        0        0   260295 2024-05-24 20:17:15.381007 ourskyai_astro_api-1.3.3668/ourskyai_astro_api/api/default_api.py
--rw-r--r--   0        0        0    30352 2024-05-24 20:17:15.437008 ourskyai_astro_api-1.3.3668/ourskyai_astro_api/api_client.py
--rw-r--r--   0        0        0      852 2024-05-24 20:17:15.533009 ourskyai_astro_api-1.3.3668/ourskyai_astro_api/api_response.py
--rw-r--r--   0        0        0    14687 2024-05-24 20:17:15.589010 ourskyai_astro_api-1.3.3668/ourskyai_astro_api/configuration.py
--rw-r--r--   0        0        0     5433 2024-05-24 20:17:15.645010 ourskyai_astro_api-1.3.3668/ourskyai_astro_api/exceptions.py
--rw-r--r--   0        0        0     5651 2024-05-24 20:17:15.705011 ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/__init__.py
--rw-r--r--   0        0        0      819 2024-05-24 20:17:15.761011 ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/asset_file_type.py
--rw-r--r--   0        0        0      931 2024-05-24 20:17:15.869013 ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/asset_type.py
--rw-r--r--   0        0        0      809 2024-05-24 20:17:15.929013 ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/calibration_master_type.py
--rw-r--r--   0        0        0     2092 2024-05-24 20:17:15.969014 ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/daily_weather_city.py
--rw-r--r--   0        0        0     4308 2024-05-24 20:17:16.021014 ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/daily_weather_forecast_item.py
--rw-r--r--   0        0        0     2527 2024-05-24 20:17:16.069015 ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/daily_weather_forecast_item_temp.py
--rw-r--r--   0        0        0     2551 2024-05-24 20:17:16.109015 ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/daily_weather_forecast_item_weather_inner.py
--rw-r--r--   0        0        0     2947 2024-05-24 20:17:16.161016 ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/daily_weather_forecast_list_response.py
--rw-r--r--   0        0        0     1904 2024-05-24 20:17:16.209016 ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/empty_success.py
--rw-r--r--   0        0        0     1186 2024-05-24 20:17:16.265017 ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/filter_type.py
--rw-r--r--   0        0        0     1930 2024-05-24 20:17:16.309018 ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/fits_header.py
--rw-r--r--   0        0        0     2155 2024-05-24 20:17:16.365018 ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/location.py
--rw-r--r--   0        0        0      747 2024-05-24 20:17:16.417019 ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/mount_type.py
--rw-r--r--   0        0        0      887 2024-05-24 20:17:16.521020 ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/node_state.py
--rw-r--r--   0        0        0      827 2024-05-24 20:17:16.589021 ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/optical_tube_type.py
--rw-r--r--   0        0        0      751 2024-05-24 20:17:16.673022 ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/shutter_type.py
--rw-r--r--   0        0        0     1892 2024-05-24 20:17:16.733023 ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/successful_create.py
--rw-r--r--   0        0        0      768 2024-05-24 20:17:16.785023 ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/tracking_type.py
--rw-r--r--   0        0        0     3258 2024-05-24 20:17:16.829023 ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_astro_project.py
--rw-r--r--   0        0        0     3969 2024-05-24 20:17:16.881024 ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_astro_project_asset.py
--rw-r--r--   0        0        0     2569 2024-05-24 20:17:16.917024 ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_astro_project_asset_metadata.py
--rw-r--r--   0        0        0     2399 2024-05-24 20:17:16.969025 ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_astro_project_asset_metadata_color_combination.py
--rw-r--r--   0        0        0     2381 2024-05-24 20:17:17.013026 ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_astro_target.py
--rw-r--r--   0        0        0     3640 2024-05-24 20:17:17.105027 ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_calibration_master.py
--rw-r--r--   0        0        0     4908 2024-05-24 20:17:17.153027 ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_camera.py
--rw-r--r--   0        0        0     2421 2024-05-24 20:17:17.201028 ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_create_astro_project_image_set_request.py
--rw-r--r--   0        0        0     2668 2024-05-24 20:17:17.245028 ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_create_astro_project_request.py
--rw-r--r--   0        0        0     2121 2024-05-24 20:17:17.325029 ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_create_astro_project_response.py
--rw-r--r--   0        0        0     3777 2024-05-24 20:17:17.425030 ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_create_calibration_master_request.py
--rw-r--r--   0        0        0     2147 2024-05-24 20:17:17.481031 ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_create_calibration_master_response.py
--rw-r--r--   0        0        0     7059 2024-05-24 20:17:17.529031 ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_create_camera_request.py
--rw-r--r--   0        0        0     2044 2024-05-24 20:17:17.605032 ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_create_image_set_image_request.py
--rw-r--r--   0        0        0     2115 2024-05-24 20:17:17.685033 ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_create_image_set_image_response.py
--rw-r--r--   0        0        0     2683 2024-05-24 20:17:17.749034 ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_create_image_set_request.py
--rw-r--r--   0        0        0     2296 2024-05-24 20:17:17.801035 ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_create_mount_request.py
--rw-r--r--   0        0        0     3146 2024-05-24 20:17:17.857035 ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_create_node_request.py
--rw-r--r--   0        0        0     2447 2024-05-24 20:17:17.905036 ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_create_optical_tube_request.py
--rw-r--r--   0        0        0     2441 2024-05-24 20:17:17.949036 ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_elevation_mask_point.py
--rw-r--r--   0        0        0     3289 2024-05-24 20:17:17.997037 ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_gain_curve.py
--rw-r--r--   0        0        0     2051 2024-05-24 20:17:18.049037 ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_gain_curve_point.py
--rw-r--r--   0        0        0     2096 2024-05-24 20:17:18.097038 ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_get_astro_platform_credit_balance_response.py
--rw-r--r--   0        0        0     2364 2024-05-24 20:17:18.153038 ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_get_nodes.py
--rw-r--r--   0        0        0     7066 2024-05-24 20:17:18.213039 ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_get_or_create_camera_request.py
--rw-r--r--   0        0        0     2324 2024-05-24 20:17:18.281040 ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_get_or_create_mount_request.py
--rw-r--r--   0        0        0     2513 2024-05-24 20:17:18.353041 ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_get_or_create_optical_tube_request.py
--rw-r--r--   0        0        0     3436 2024-05-24 20:17:18.405041 ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_image_set.py
--rw-r--r--   0        0        0     5797 2024-05-24 20:17:18.457042 ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_image_set_image.py
--rw-r--r--   0        0        0      795 2024-05-24 20:17:18.513043 ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_job_kind.py
--rw-r--r--   0        0        0     2632 2024-05-24 20:17:18.569043 ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_job_log.py
--rw-r--r--   0        0        0      803 2024-05-24 20:17:18.601044 ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_job_status.py
--rw-r--r--   0        0        0     1914 2024-05-24 20:17:18.649044 ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_mount.py
--rw-r--r--   0        0        0     4458 2024-05-24 20:17:18.705045 ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_node.py
--rw-r--r--   0        0        0     2564 2024-05-24 20:17:18.765045 ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_node_with_location.py
--rw-r--r--   0        0        0     2239 2024-05-24 20:17:18.817046 ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_optical_tube.py
--rw-r--r--   0        0        0     3057 2024-05-24 20:17:18.869047 ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_platform_credit.py
--rw-r--r--   0        0        0      870 2024-05-24 20:17:18.937047 ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_platform_credit_source.py
--rw-r--r--   0        0        0      800 2024-05-24 20:17:18.985048 ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_platform_credit_type.py
--rw-r--r--   0        0        0      776 2024-05-24 20:17:19.045048 ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_platform_credit_unit.py
--rw-r--r--   0        0        0     2045 2024-05-24 20:17:19.093049 ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_put_stack_astro_project_request.py
--rw-r--r--   0        0        0     2051 2024-05-24 20:17:19.153050 ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_read_noise_point.py
--rw-r--r--   0        0        0     2050 2024-05-24 20:17:19.217050 ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_setup_action.py
--rw-r--r--   0        0        0     2940 2024-05-24 20:17:19.265051 ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_slew_timing.py
--rw-r--r--   0        0        0     2240 2024-05-24 20:17:19.297051 ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_slew_timing_interval.py
--rw-r--r--   0        0        0     4605 2024-05-24 20:17:19.357052 ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_update_node_request.py
--rw-r--r--   0        0        0     2522 2024-05-24 20:17:19.413053 ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_video_mode_framerate_property.py
--rw-r--r--   0        0        0        0 2024-05-24 20:17:19.441053 ourskyai_astro_api-1.3.3668/ourskyai_astro_api/py.typed
--rw-r--r--   0        0        0    12935 2024-05-24 20:17:19.505054 ourskyai_astro_api-1.3.3668/ourskyai_astro_api/rest.py
--rw-r--r--   0        0        0      739 2024-05-24 20:17:19.669056 ourskyai_astro_api-1.3.3668/pyproject.toml
--rw-r--r--   0        0        0    12509 1970-01-01 00:00:00.000000 ourskyai_astro_api-1.3.3668/PKG-INFO
+-rw-r--r--   0        0        0    11541 2024-05-24 22:50:26.094619 ourskyai_astro_api-1.3.3671/README.md
+-rw-r--r--   0        0        0     6292 2024-05-24 22:50:29.834662 ourskyai_astro_api-1.3.3671/ourskyai_astro_api/__init__.py
+-rw-r--r--   0        0        0      106 2024-05-24 22:50:29.866663 ourskyai_astro_api-1.3.3671/ourskyai_astro_api/api/__init__.py
+-rw-r--r--   0        0        0   260295 2024-05-24 22:50:29.930663 ourskyai_astro_api-1.3.3671/ourskyai_astro_api/api/default_api.py
+-rw-r--r--   0        0        0    30352 2024-05-24 22:50:29.982664 ourskyai_astro_api-1.3.3671/ourskyai_astro_api/api_client.py
+-rw-r--r--   0        0        0      852 2024-05-24 22:50:30.074665 ourskyai_astro_api-1.3.3671/ourskyai_astro_api/api_response.py
+-rw-r--r--   0        0        0    14687 2024-05-24 22:50:30.122666 ourskyai_astro_api-1.3.3671/ourskyai_astro_api/configuration.py
+-rw-r--r--   0        0        0     5433 2024-05-24 22:50:30.178666 ourskyai_astro_api-1.3.3671/ourskyai_astro_api/exceptions.py
+-rw-r--r--   0        0        0     5651 2024-05-24 22:50:30.278667 ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/__init__.py
+-rw-r--r--   0        0        0      819 2024-05-24 22:50:30.358668 ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/asset_file_type.py
+-rw-r--r--   0        0        0      931 2024-05-24 22:50:30.426669 ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/asset_type.py
+-rw-r--r--   0        0        0      809 2024-05-24 22:50:30.478670 ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/calibration_master_type.py
+-rw-r--r--   0        0        0     2092 2024-05-24 22:50:30.530670 ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/daily_weather_city.py
+-rw-r--r--   0        0        0     4308 2024-05-24 22:50:30.606671 ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/daily_weather_forecast_item.py
+-rw-r--r--   0        0        0     2527 2024-05-24 22:50:30.650672 ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/daily_weather_forecast_item_temp.py
+-rw-r--r--   0        0        0     2551 2024-05-24 22:50:30.718672 ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/daily_weather_forecast_item_weather_inner.py
+-rw-r--r--   0        0        0     2947 2024-05-24 22:50:30.762673 ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/daily_weather_forecast_list_response.py
+-rw-r--r--   0        0        0     1904 2024-05-24 22:50:30.802673 ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/empty_success.py
+-rw-r--r--   0        0        0     1186 2024-05-24 22:50:30.858674 ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/filter_type.py
+-rw-r--r--   0        0        0     1930 2024-05-24 22:50:30.910674 ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/fits_header.py
+-rw-r--r--   0        0        0     2155 2024-05-24 22:50:30.966675 ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/location.py
+-rw-r--r--   0        0        0      747 2024-05-24 22:50:31.014676 ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/mount_type.py
+-rw-r--r--   0        0        0      887 2024-05-24 22:50:31.062676 ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/node_state.py
+-rw-r--r--   0        0        0      827 2024-05-24 22:50:31.122677 ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/optical_tube_type.py
+-rw-r--r--   0        0        0      751 2024-05-24 22:50:31.182678 ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/shutter_type.py
+-rw-r--r--   0        0        0     1892 2024-05-24 22:50:31.226678 ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/successful_create.py
+-rw-r--r--   0        0        0      768 2024-05-24 22:50:31.270678 ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/tracking_type.py
+-rw-r--r--   0        0        0     3258 2024-05-24 22:50:31.338679 ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_astro_project.py
+-rw-r--r--   0        0        0     3969 2024-05-24 22:50:31.386680 ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_astro_project_asset.py
+-rw-r--r--   0        0        0     2569 2024-05-24 22:50:31.438680 ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_astro_project_asset_metadata.py
+-rw-r--r--   0        0        0     2399 2024-05-24 22:50:31.514681 ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_astro_project_asset_metadata_color_combination.py
+-rw-r--r--   0        0        0     2381 2024-05-24 22:50:31.562682 ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_astro_target.py
+-rw-r--r--   0        0        0     3640 2024-05-24 22:50:31.598682 ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_calibration_master.py
+-rw-r--r--   0        0        0     4908 2024-05-24 22:50:31.646683 ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_camera.py
+-rw-r--r--   0        0        0     2421 2024-05-24 22:50:31.686683 ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_create_astro_project_image_set_request.py
+-rw-r--r--   0        0        0     2668 2024-05-24 22:50:31.734684 ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_create_astro_project_request.py
+-rw-r--r--   0        0        0     2121 2024-05-24 22:50:31.782684 ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_create_astro_project_response.py
+-rw-r--r--   0        0        0     3777 2024-05-24 22:50:31.854685 ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_create_calibration_master_request.py
+-rw-r--r--   0        0        0     2147 2024-05-24 22:50:31.902686 ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_create_calibration_master_response.py
+-rw-r--r--   0        0        0     7059 2024-05-24 22:50:31.958686 ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_create_camera_request.py
+-rw-r--r--   0        0        0     2044 2024-05-24 22:50:32.014687 ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_create_image_set_image_request.py
+-rw-r--r--   0        0        0     2115 2024-05-24 22:50:32.054687 ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_create_image_set_image_response.py
+-rw-r--r--   0        0        0     2683 2024-05-24 22:50:32.114688 ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_create_image_set_request.py
+-rw-r--r--   0        0        0     2296 2024-05-24 22:50:32.170689 ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_create_mount_request.py
+-rw-r--r--   0        0        0     3146 2024-05-24 22:50:32.214689 ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_create_node_request.py
+-rw-r--r--   0        0        0     2447 2024-05-24 22:50:32.258690 ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_create_optical_tube_request.py
+-rw-r--r--   0        0        0     2441 2024-05-24 22:50:32.334690 ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_elevation_mask_point.py
+-rw-r--r--   0        0        0     3289 2024-05-24 22:50:32.378691 ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_gain_curve.py
+-rw-r--r--   0        0        0     2051 2024-05-24 22:50:32.454692 ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_gain_curve_point.py
+-rw-r--r--   0        0        0     2096 2024-05-24 22:50:32.502692 ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_get_astro_platform_credit_balance_response.py
+-rw-r--r--   0        0        0     2364 2024-05-24 22:50:32.546693 ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_get_nodes.py
+-rw-r--r--   0        0        0     7066 2024-05-24 22:50:32.598693 ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_get_or_create_camera_request.py
+-rw-r--r--   0        0        0     2324 2024-05-24 22:50:32.642694 ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_get_or_create_mount_request.py
+-rw-r--r--   0        0        0     2513 2024-05-24 22:50:32.694695 ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_get_or_create_optical_tube_request.py
+-rw-r--r--   0        0        0     3436 2024-05-24 22:50:32.738695 ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_image_set.py
+-rw-r--r--   0        0        0     5797 2024-05-24 22:50:32.782696 ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_image_set_image.py
+-rw-r--r--   0        0        0      795 2024-05-24 22:50:32.838696 ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_job_kind.py
+-rw-r--r--   0        0        0     2632 2024-05-24 22:50:32.882697 ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_job_log.py
+-rw-r--r--   0        0        0      803 2024-05-24 22:50:32.926697 ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_job_status.py
+-rw-r--r--   0        0        0     1914 2024-05-24 22:50:32.974698 ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_mount.py
+-rw-r--r--   0        0        0     4458 2024-05-24 22:50:33.026698 ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_node.py
+-rw-r--r--   0        0        0     2564 2024-05-24 22:50:33.102699 ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_node_with_location.py
+-rw-r--r--   0        0        0     2239 2024-05-24 22:50:33.138700 ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_optical_tube.py
+-rw-r--r--   0        0        0     3057 2024-05-24 22:50:33.198700 ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_platform_credit.py
+-rw-r--r--   0        0        0      870 2024-05-24 22:50:33.250701 ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_platform_credit_source.py
+-rw-r--r--   0        0        0      800 2024-05-24 22:50:33.306702 ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_platform_credit_type.py
+-rw-r--r--   0        0        0      776 2024-05-24 22:50:33.366702 ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_platform_credit_unit.py
+-rw-r--r--   0        0        0     2045 2024-05-24 22:50:33.430703 ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_put_stack_astro_project_request.py
+-rw-r--r--   0        0        0     2051 2024-05-24 22:50:33.462703 ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_read_noise_point.py
+-rw-r--r--   0        0        0     2050 2024-05-24 22:50:33.510704 ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_setup_action.py
+-rw-r--r--   0        0        0     2940 2024-05-24 22:50:33.566704 ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_slew_timing.py
+-rw-r--r--   0        0        0     2240 2024-05-24 22:50:33.614705 ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_slew_timing_interval.py
+-rw-r--r--   0        0        0     4605 2024-05-24 22:50:33.678706 ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_update_node_request.py
+-rw-r--r--   0        0        0     2522 2024-05-24 22:50:33.730706 ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_video_mode_framerate_property.py
+-rw-r--r--   0        0        0        0 2024-05-24 22:50:33.758707 ourskyai_astro_api-1.3.3671/ourskyai_astro_api/py.typed
+-rw-r--r--   0        0        0    12935 2024-05-24 22:50:33.810707 ourskyai_astro_api-1.3.3671/ourskyai_astro_api/rest.py
+-rw-r--r--   0        0        0      739 2024-05-24 22:50:33.870708 ourskyai_astro_api-1.3.3671/pyproject.toml
+-rw-r--r--   0        0        0    12509 1970-01-01 00:00:00.000000 ourskyai_astro_api-1.3.3671/PKG-INFO
```

### Comparing `ourskyai_astro_api-1.3.3668/README.md` & `ourskyai_astro_api-1.3.3671/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # ourskyai-astro-api
 No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 1.3.3668
-- Package version: 1.3.3668
+- API version: 1.3.3671
+- Package version: 1.3.3671
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 3.7+
 
 ## Installation & Usage
```

### Comparing `ourskyai_astro_api-1.3.3668/ourskyai_astro_api/__init__.py` & `ourskyai_astro_api-1.3.3671/ourskyai_astro_api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 # flake8: noqa
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-__version__ = "1.3.3668"
+__version__ = "1.3.3671"
 
 # import apis into sdk package
 from ourskyai_astro_api.api.default_api import DefaultApi
 
 # import ApiClient
 from ourskyai_astro_api.api_response import ApiResponse
 from ourskyai_astro_api.api_client import ApiClient
```

### Comparing `ourskyai_astro_api-1.3.3668/ourskyai_astro_api/api/default_api.py` & `ourskyai_astro_api-1.3.3671/ourskyai_astro_api/api/default_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import re  # noqa: F401
```

### Comparing `ourskyai_astro_api-1.3.3668/ourskyai_astro_api/api_client.py` & `ourskyai_astro_api-1.3.3671/ourskyai_astro_api/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import atexit
@@ -72,15 +72,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.3.3668/python'
+        self.user_agent = 'OpenAPI-Generator/1.3.3671/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `ourskyai_astro_api-1.3.3668/ourskyai_astro_api/api_response.py` & `ourskyai_astro_api-1.3.3671/ourskyai_astro_api/api_response.py`

 * *Files identical despite different names*

### Comparing `ourskyai_astro_api-1.3.3668/ourskyai_astro_api/configuration.py` & `ourskyai_astro_api-1.3.3671/ourskyai_astro_api/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import copy
@@ -371,16 +371,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 1.3.3668\n"\
-               "SDK Package Version: 1.3.3668".\
+               "Version of the API: 1.3.3671\n"\
+               "SDK Package Version: 1.3.3671".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `ourskyai_astro_api-1.3.3668/ourskyai_astro_api/exceptions.py` & `ourskyai_astro_api-1.3.3671/ourskyai_astro_api/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 class OpenApiException(Exception):
```

### Comparing `ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/__init__.py` & `ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 # import models into model package
```

### Comparing `ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/asset_file_type.py` & `ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/asset_file_type.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/asset_type.py` & `ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/asset_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/calibration_master_type.py` & `ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/calibration_master_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/daily_weather_city.py` & `ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/daily_weather_city.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/daily_weather_forecast_item.py` & `ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/daily_weather_forecast_item.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/daily_weather_forecast_item_temp.py` & `ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/daily_weather_forecast_item_temp.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/daily_weather_forecast_item_weather_inner.py` & `ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/daily_weather_forecast_item_weather_inner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/daily_weather_forecast_list_response.py` & `ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/daily_weather_forecast_list_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/empty_success.py` & `ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/empty_success.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/filter_type.py` & `ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/filter_type.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/fits_header.py` & `ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/fits_header.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/location.py` & `ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/location.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/mount_type.py` & `ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/mount_type.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/node_state.py` & `ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/node_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/optical_tube_type.py` & `ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/optical_tube_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/shutter_type.py` & `ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_job_status.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
@@ -17,24 +17,26 @@
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class ShutterType(str, Enum):
+class V1JobStatus(str, Enum):
     """
-    ShutterType
+    V1JobStatus
     """
 
     """
     allowed enum values
     """
-    ROLLING = 'ROLLING'
-    GLOBAL = 'GLOBAL'
+    PENDING = 'PENDING'
+    RUNNING = 'RUNNING'
+    SUCCEEDED = 'SUCCEEDED'
+    FAILED = 'FAILED'
 
     @classmethod
-    def from_json(cls, json_str: str) -> ShutterType:
-        """Create an instance of ShutterType from a JSON string"""
-        return ShutterType(json.loads(json_str))
+    def from_json(cls, json_str: str) -> V1JobStatus:
+        """Create an instance of V1JobStatus from a JSON string"""
+        return V1JobStatus(json.loads(json_str))
```

### Comparing `ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/successful_create.py` & `ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/successful_create.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/tracking_type.py` & `ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/tracking_type.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_astro_project.py` & `ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_astro_project.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_astro_project_asset.py` & `ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_astro_project_asset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_astro_project_asset_metadata.py` & `ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_astro_project_asset_metadata.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_astro_project_asset_metadata_color_combination.py` & `ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_astro_project_asset_metadata_color_combination.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_astro_target.py` & `ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_astro_target.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_calibration_master.py` & `ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_calibration_master.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_camera.py` & `ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_camera.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_create_astro_project_image_set_request.py` & `ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_create_astro_project_image_set_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_create_astro_project_request.py` & `ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_create_astro_project_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_create_astro_project_response.py` & `ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_create_astro_project_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_create_calibration_master_request.py` & `ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_create_calibration_master_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_create_calibration_master_response.py` & `ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_create_calibration_master_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_create_camera_request.py` & `ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_create_camera_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_create_image_set_image_request.py` & `ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_create_image_set_image_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_create_image_set_image_response.py` & `ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_create_image_set_image_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_create_image_set_request.py` & `ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_create_image_set_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_create_mount_request.py` & `ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_create_mount_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_create_node_request.py` & `ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_create_node_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_create_optical_tube_request.py` & `ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_create_optical_tube_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_elevation_mask_point.py` & `ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_elevation_mask_point.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_gain_curve.py` & `ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_gain_curve.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_gain_curve_point.py` & `ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_gain_curve_point.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_get_astro_platform_credit_balance_response.py` & `ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_get_astro_platform_credit_balance_response.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_get_nodes.py` & `ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_get_nodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_get_or_create_camera_request.py` & `ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_get_or_create_camera_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_get_or_create_mount_request.py` & `ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_get_or_create_mount_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_get_or_create_optical_tube_request.py` & `ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_get_or_create_optical_tube_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_image_set.py` & `ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_image_set.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_image_set_image.py` & `ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_image_set_image.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_job_kind.py` & `ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_job_kind.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_job_log.py` & `ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_job_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_mount.py` & `ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_mount.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_node.py` & `ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_node.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_node_with_location.py` & `ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_node_with_location.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_optical_tube.py` & `ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_optical_tube.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_platform_credit.py` & `ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_platform_credit.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_platform_credit_source.py` & `ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_platform_credit_source.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_platform_credit_type.py` & `ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_platform_credit_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_platform_credit_unit.py` & `ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_platform_credit_unit.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_put_stack_astro_project_request.py` & `ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_put_stack_astro_project_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_read_noise_point.py` & `ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_read_noise_point.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_setup_action.py` & `ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_setup_action.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_slew_timing.py` & `ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_slew_timing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_slew_timing_interval.py` & `ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_slew_timing_interval.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_update_node_request.py` & `ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_update_node_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3668/ourskyai_astro_api/models/v1_video_mode_framerate_property.py` & `ourskyai_astro_api-1.3.3671/ourskyai_astro_api/models/v1_video_mode_framerate_property.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3668/ourskyai_astro_api/rest.py` & `ourskyai_astro_api-1.3.3671/ourskyai_astro_api/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import io
```

### Comparing `ourskyai_astro_api-1.3.3668/pyproject.toml` & `ourskyai_astro_api-1.3.3671/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ourskyai_astro_api"
-version = "1.3.3668"
+version = "1.3.3671"
 description = "OurSky Astro"
 authors = ["OpenAPI Generator Community <team@openapitools.org>"]
 license = "NoLicense"
 readme = "README.md"
 repository = "https://github.com/GIT_USER_ID/GIT_REPO_ID"
 keywords = ["OpenAPI", "OpenAPI-Generator", "OurSky Astro"]
 include = ["ourskyai_astro_api/py.typed"]
```

### Comparing `ourskyai_astro_api-1.3.3668/PKG-INFO` & `ourskyai_astro_api-1.3.3671/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ourskyai_astro_api
-Version: 1.3.3668
+Version: 1.3.3671
 Summary: OurSky Astro
 Home-page: https://github.com/GIT_USER_ID/GIT_REPO_ID
 License: NoLicense
 Keywords: OpenAPI,OpenAPI-Generator,OurSky Astro
 Author: OpenAPI Generator Community
 Author-email: team@openapitools.org
 Requires-Python: >=3.7,<4.0
@@ -24,16 +24,16 @@
 Description-Content-Type: text/markdown
 
 # ourskyai-astro-api
 No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 1.3.3668
-- Package version: 1.3.3668
+- API version: 1.3.3671
+- Package version: 1.3.3671
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 3.7+
 
 ## Installation & Usage
```

