# Comparing `tmp/ourskyai_platform_api-1.3.3668.tar.gz` & `tmp/ourskyai_platform_api-1.3.3671.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ourskyai_platform_api-1.3.3668.tar", max compression
+gzip compressed data, was "ourskyai_platform_api-1.3.3671.tar", max compression
```

## Comparing `ourskyai_platform_api-1.3.3668.tar` & `ourskyai_platform_api-1.3.3671.tar`

### file list

```diff
@@ -1,78 +1,78 @@
--rw-r--r--   0        0        0     9968 2024-05-24 20:17:11.116959 ourskyai_platform_api-1.3.3668/README.md
--rw-r--r--   0        0        0     6552 2024-05-24 20:17:15.165005 ourskyai_platform_api-1.3.3668/ourskyai_platform_api/__init__.py
--rw-r--r--   0        0        0      109 2024-05-24 20:17:15.197005 ourskyai_platform_api-1.3.3668/ourskyai_platform_api/api/__init__.py
--rw-r--r--   0        0        0   206365 2024-05-24 20:17:15.285006 ourskyai_platform_api-1.3.3668/ourskyai_platform_api/api/default_api.py
--rw-r--r--   0        0        0    30373 2024-05-24 20:17:15.357007 ourskyai_platform_api-1.3.3668/ourskyai_platform_api/api_client.py
--rw-r--r--   0        0        0      852 2024-05-24 20:17:15.417008 ourskyai_platform_api-1.3.3668/ourskyai_platform_api/api_response.py
--rw-r--r--   0        0        0    14693 2024-05-24 20:17:15.473008 ourskyai_platform_api-1.3.3668/ourskyai_platform_api/configuration.py
--rw-r--r--   0        0        0     5436 2024-05-24 20:17:15.525009 ourskyai_platform_api-1.3.3668/ourskyai_platform_api/exceptions.py
--rw-r--r--   0        0        0     5881 2024-05-24 20:17:15.577009 ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/__init__.py
--rw-r--r--   0        0        0      745 2024-05-24 20:17:15.621010 ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/camera_mode.py
--rw-r--r--   0        0        0     1907 2024-05-24 20:17:15.677011 ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/empty_success.py
--rw-r--r--   0        0        0     1189 2024-05-24 20:17:15.721011 ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/filter_type.py
--rw-r--r--   0        0        0     1933 2024-05-24 20:17:15.761011 ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/fits_header.py
--rw-r--r--   0        0        0     2158 2024-05-24 20:17:15.817012 ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/location.py
--rw-r--r--   0        0        0      777 2024-05-24 20:17:15.857013 ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/metric_type.py
--rw-r--r--   0        0        0      750 2024-05-24 20:17:15.917013 ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/mount_type.py
--rw-r--r--   0        0        0      890 2024-05-24 20:17:15.961014 ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/node_state.py
--rw-r--r--   0        0        0      830 2024-05-24 20:17:16.013014 ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/optical_tube_type.py
--rw-r--r--   0        0        0     2407 2024-05-24 20:17:16.053015 ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/plate_solve_parameters.py
--rw-r--r--   0        0        0      754 2024-05-24 20:17:16.113016 ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/shutter_type.py
--rw-r--r--   0        0        0     1895 2024-05-24 20:17:16.149016 ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/successful_create.py
--rw-r--r--   0        0        0      771 2024-05-24 20:17:16.205016 ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/tracking_type.py
--rw-r--r--   0        0        0     2622 2024-05-24 20:17:16.293017 ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_auto_focus_instruction.py
--rw-r--r--   0        0        0     2366 2024-05-24 20:17:16.345018 ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_auto_focus_instruction_coordinates_inner.py
--rw-r--r--   0        0        0     4920 2024-05-24 20:17:16.393019 ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_camera.py
--rw-r--r--   0        0        0     2115 2024-05-24 20:17:16.513020 ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_client_token.py
--rw-r--r--   0        0        0     2047 2024-05-24 20:17:16.557021 ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_complete_observation_request.py
--rw-r--r--   0        0        0     2047 2024-05-24 20:17:16.593021 ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_create_image_set_image_request.py
--rw-r--r--   0        0        0     2118 2024-05-24 20:17:16.689022 ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_create_image_set_image_response.py
--rw-r--r--   0        0        0     2692 2024-05-24 20:17:16.753023 ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_create_image_set_request.py
--rw-r--r--   0        0        0     2302 2024-05-24 20:17:16.821023 ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_create_mount_request.py
--rw-r--r--   0        0        0     2071 2024-05-24 20:17:16.861024 ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_create_node_controller_artifact_request.py
--rw-r--r--   0        0        0     2710 2024-05-24 20:17:16.913025 ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_create_node_diagnostic.py
--rw-r--r--   0        0        0     2715 2024-05-24 20:17:16.961025 ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_create_node_diagnostics_request.py
--rw-r--r--   0        0        0     3152 2024-05-24 20:17:17.005025 ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_create_node_request.py
--rw-r--r--   0        0        0     2453 2024-05-24 20:17:17.057026 ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_create_optical_tube_request.py
--rw-r--r--   0        0        0     2124 2024-05-24 20:17:17.113027 ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_diagnostic_instruction.py
--rw-r--r--   0        0        0     2444 2024-05-24 20:17:17.165027 ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_elevation_mask_point.py
--rw-r--r--   0        0        0      719 2024-05-24 20:17:17.221028 ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_file_type.py
--rw-r--r--   0        0        0     3298 2024-05-24 20:17:17.293029 ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_gain_curve.py
--rw-r--r--   0        0        0     2054 2024-05-24 20:17:17.341029 ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_gain_curve_point.py
--rw-r--r--   0        0        0     2570 2024-05-24 20:17:17.401030 ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_get_instruction_request.py
--rw-r--r--   0        0        0     2370 2024-05-24 20:17:17.457031 ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_get_nodes.py
--rw-r--r--   0        0        0     7081 2024-05-24 20:17:17.505031 ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_get_or_create_camera_request.py
--rw-r--r--   0        0        0     2330 2024-05-24 20:17:17.609032 ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_get_or_create_mount_request.py
--rw-r--r--   0        0        0     2519 2024-05-24 20:17:17.697033 ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_get_or_create_optical_tube_request.py
--rw-r--r--   0        0        0     2675 2024-05-24 20:17:17.741034 ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_get_plate_solve_catalog_diff_request.py
--rw-r--r--   0        0        0     3985 2024-05-24 20:17:17.785034 ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_ground_station_participant.py
--rw-r--r--   0        0        0     3445 2024-05-24 20:17:17.833035 ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_image_set.py
--rw-r--r--   0        0        0     5803 2024-05-24 20:17:17.921036 ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_image_set_image.py
--rw-r--r--   0        0        0     3763 2024-05-24 20:17:18.013037 ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_instruction.py
--rw-r--r--   0        0        0     2400 2024-05-24 20:17:18.053037 ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_metric.py
--rw-r--r--   0        0        0     1917 2024-05-24 20:17:18.089038 ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_mount.py
--rw-r--r--   0        0        0     4470 2024-05-24 20:17:18.141038 ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_node.py
--rw-r--r--   0        0        0      850 2024-05-24 20:17:18.201039 ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_node_component_type.py
--rw-r--r--   0        0        0     1963 2024-05-24 20:17:18.249040 ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_node_controller_artifact.py
--rw-r--r--   0        0        0     1669 2024-05-24 20:17:18.293040 ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_node_diagnostic_type.py
--rw-r--r--   0        0        0     2573 2024-05-24 20:17:18.329040 ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_node_with_location.py
--rw-r--r--   0        0        0     5537 2024-05-24 20:17:18.389041 ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_observation_instruction.py
--rw-r--r--   0        0        0     2242 2024-05-24 20:17:18.445042 ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_optical_tube.py
--rw-r--r--   0        0        0     2135 2024-05-24 20:17:18.509042 ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_plate_solve_catalog_file.py
--rw-r--r--   0        0        0     2648 2024-05-24 20:17:18.549043 ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_plate_solve_catalog_file_download.py
--rw-r--r--   0        0        0     2054 2024-05-24 20:17:18.597043 ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_read_noise_point.py
--rw-r--r--   0        0        0     2401 2024-05-24 20:17:18.665044 ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_release.py
--rw-r--r--   0        0        0     2053 2024-05-24 20:17:18.725045 ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_setup_action.py
--rw-r--r--   0        0        0     2946 2024-05-24 20:17:18.777045 ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_slew_timing.py
--rw-r--r--   0        0        0     2243 2024-05-24 20:17:18.873046 ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_slew_timing_interval.py
--rw-r--r--   0        0        0     3601 2024-05-24 20:17:18.933047 ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_update_node_components_request.py
--rw-r--r--   0        0        0     6269 2024-05-24 20:17:18.989048 ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_update_node_components_request_camera.py
--rw-r--r--   0        0        0     2402 2024-05-24 20:17:19.041048 ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_update_node_components_request_mount.py
--rw-r--r--   0        0        0     2591 2024-05-24 20:17:19.101049 ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_update_node_components_request_optical_tube.py
--rw-r--r--   0        0        0     4620 2024-05-24 20:17:19.177050 ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_update_node_request.py
--rw-r--r--   0        0        0     2525 2024-05-24 20:17:19.229050 ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_video_mode_framerate_property.py
--rw-r--r--   0        0        0     2224 2024-05-24 20:17:19.281051 ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v2_complete_observation_request.py
--rw-r--r--   0        0        0        0 2024-05-24 20:17:19.309051 ourskyai_platform_api-1.3.3668/ourskyai_platform_api/py.typed
--rw-r--r--   0        0        0    12941 2024-05-24 20:17:19.353052 ourskyai_platform_api-1.3.3668/ourskyai_platform_api/rest.py
--rw-r--r--   0        0        0      751 2024-05-24 20:17:19.409052 ourskyai_platform_api-1.3.3668/pyproject.toml
--rw-r--r--   0        0        0    10945 1970-01-01 00:00:00.000000 ourskyai_platform_api-1.3.3668/PKG-INFO
+-rw-r--r--   0        0        0     9968 2024-05-24 22:50:26.058619 ourskyai_platform_api-1.3.3671/README.md
+-rw-r--r--   0        0        0     6552 2024-05-24 22:50:29.966664 ourskyai_platform_api-1.3.3671/ourskyai_platform_api/__init__.py
+-rw-r--r--   0        0        0      109 2024-05-24 22:50:29.998664 ourskyai_platform_api-1.3.3671/ourskyai_platform_api/api/__init__.py
+-rw-r--r--   0        0        0   206365 2024-05-24 22:50:30.090665 ourskyai_platform_api-1.3.3671/ourskyai_platform_api/api/default_api.py
+-rw-r--r--   0        0        0    30373 2024-05-24 22:50:30.134666 ourskyai_platform_api-1.3.3671/ourskyai_platform_api/api_client.py
+-rw-r--r--   0        0        0      852 2024-05-24 22:50:30.174666 ourskyai_platform_api-1.3.3671/ourskyai_platform_api/api_response.py
+-rw-r--r--   0        0        0    14693 2024-05-24 22:50:30.206667 ourskyai_platform_api-1.3.3671/ourskyai_platform_api/configuration.py
+-rw-r--r--   0        0        0     5436 2024-05-24 22:50:30.266667 ourskyai_platform_api-1.3.3671/ourskyai_platform_api/exceptions.py
+-rw-r--r--   0        0        0     5881 2024-05-24 22:50:30.318668 ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/__init__.py
+-rw-r--r--   0        0        0      745 2024-05-24 22:50:30.366668 ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/camera_mode.py
+-rw-r--r--   0        0        0     1907 2024-05-24 22:50:30.438669 ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/empty_success.py
+-rw-r--r--   0        0        0     1189 2024-05-24 22:50:30.518670 ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/filter_type.py
+-rw-r--r--   0        0        0     1933 2024-05-24 22:50:30.582671 ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/fits_header.py
+-rw-r--r--   0        0        0     2158 2024-05-24 22:50:30.626671 ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/location.py
+-rw-r--r--   0        0        0      777 2024-05-24 22:50:30.674672 ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/metric_type.py
+-rw-r--r--   0        0        0      750 2024-05-24 22:50:30.734672 ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/mount_type.py
+-rw-r--r--   0        0        0      890 2024-05-24 22:50:30.802673 ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/node_state.py
+-rw-r--r--   0        0        0      830 2024-05-24 22:50:30.870674 ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/optical_tube_type.py
+-rw-r--r--   0        0        0     2407 2024-05-24 22:50:30.914674 ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/plate_solve_parameters.py
+-rw-r--r--   0        0        0      754 2024-05-24 22:50:30.998675 ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/shutter_type.py
+-rw-r--r--   0        0        0     1895 2024-05-24 22:50:31.074676 ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/successful_create.py
+-rw-r--r--   0        0        0      771 2024-05-24 22:50:31.126677 ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/tracking_type.py
+-rw-r--r--   0        0        0     2622 2024-05-24 22:50:31.182678 ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_auto_focus_instruction.py
+-rw-r--r--   0        0        0     2366 2024-05-24 22:50:31.230678 ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_auto_focus_instruction_coordinates_inner.py
+-rw-r--r--   0        0        0     4920 2024-05-24 22:50:31.290679 ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_camera.py
+-rw-r--r--   0        0        0     2115 2024-05-24 22:50:31.398680 ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_client_token.py
+-rw-r--r--   0        0        0     2047 2024-05-24 22:50:31.446680 ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_complete_observation_request.py
+-rw-r--r--   0        0        0     2047 2024-05-24 22:50:31.514681 ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_create_image_set_image_request.py
+-rw-r--r--   0        0        0     2118 2024-05-24 22:50:31.566682 ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_create_image_set_image_response.py
+-rw-r--r--   0        0        0     2692 2024-05-24 22:50:31.618682 ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_create_image_set_request.py
+-rw-r--r--   0        0        0     2302 2024-05-24 22:50:31.666683 ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_create_mount_request.py
+-rw-r--r--   0        0        0     2071 2024-05-24 22:50:31.698683 ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_create_node_controller_artifact_request.py
+-rw-r--r--   0        0        0     2710 2024-05-24 22:50:31.754684 ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_create_node_diagnostic.py
+-rw-r--r--   0        0        0     2715 2024-05-24 22:50:31.818685 ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_create_node_diagnostics_request.py
+-rw-r--r--   0        0        0     3152 2024-05-24 22:50:31.862685 ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_create_node_request.py
+-rw-r--r--   0        0        0     2453 2024-05-24 22:50:31.922686 ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_create_optical_tube_request.py
+-rw-r--r--   0        0        0     2124 2024-05-24 22:50:31.966686 ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_diagnostic_instruction.py
+-rw-r--r--   0        0        0     2444 2024-05-24 22:50:32.062687 ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_elevation_mask_point.py
+-rw-r--r--   0        0        0      719 2024-05-24 22:50:32.134688 ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_file_type.py
+-rw-r--r--   0        0        0     3298 2024-05-24 22:50:32.182689 ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_gain_curve.py
+-rw-r--r--   0        0        0     2054 2024-05-24 22:50:32.230689 ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_gain_curve_point.py
+-rw-r--r--   0        0        0     2570 2024-05-24 22:50:32.294690 ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_get_instruction_request.py
+-rw-r--r--   0        0        0     2370 2024-05-24 22:50:32.346691 ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_get_nodes.py
+-rw-r--r--   0        0        0     7081 2024-05-24 22:50:32.406691 ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_get_or_create_camera_request.py
+-rw-r--r--   0        0        0     2330 2024-05-24 22:50:32.454692 ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_get_or_create_mount_request.py
+-rw-r--r--   0        0        0     2519 2024-05-24 22:50:32.510692 ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_get_or_create_optical_tube_request.py
+-rw-r--r--   0        0        0     2675 2024-05-24 22:50:32.554693 ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_get_plate_solve_catalog_diff_request.py
+-rw-r--r--   0        0        0     3985 2024-05-24 22:50:32.606694 ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_ground_station_participant.py
+-rw-r--r--   0        0        0     3445 2024-05-24 22:50:32.658694 ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_image_set.py
+-rw-r--r--   0        0        0     5803 2024-05-24 22:50:32.702695 ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_image_set_image.py
+-rw-r--r--   0        0        0     3763 2024-05-24 22:50:32.738695 ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_instruction.py
+-rw-r--r--   0        0        0     2400 2024-05-24 22:50:32.810696 ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_metric.py
+-rw-r--r--   0        0        0     1917 2024-05-24 22:50:32.854696 ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_mount.py
+-rw-r--r--   0        0        0     4470 2024-05-24 22:50:32.914697 ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_node.py
+-rw-r--r--   0        0        0      850 2024-05-24 22:50:32.994698 ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_node_component_type.py
+-rw-r--r--   0        0        0     1963 2024-05-24 22:50:33.042698 ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_node_controller_artifact.py
+-rw-r--r--   0        0        0     1669 2024-05-24 22:50:33.102699 ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_node_diagnostic_type.py
+-rw-r--r--   0        0        0     2573 2024-05-24 22:50:33.174700 ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_node_with_location.py
+-rw-r--r--   0        0        0     5537 2024-05-24 22:50:33.222700 ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_observation_instruction.py
+-rw-r--r--   0        0        0     2242 2024-05-24 22:50:33.266701 ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_optical_tube.py
+-rw-r--r--   0        0        0     2135 2024-05-24 22:50:33.314702 ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_plate_solve_catalog_file.py
+-rw-r--r--   0        0        0     2648 2024-05-24 22:50:33.406703 ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_plate_solve_catalog_file_download.py
+-rw-r--r--   0        0        0     2054 2024-05-24 22:50:33.462703 ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_read_noise_point.py
+-rw-r--r--   0        0        0     2401 2024-05-24 22:50:33.510704 ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_release.py
+-rw-r--r--   0        0        0     2053 2024-05-24 22:50:33.574705 ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_setup_action.py
+-rw-r--r--   0        0        0     2946 2024-05-24 22:50:33.622705 ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_slew_timing.py
+-rw-r--r--   0        0        0     2243 2024-05-24 22:50:33.662706 ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_slew_timing_interval.py
+-rw-r--r--   0        0        0     3601 2024-05-24 22:50:33.698706 ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_update_node_components_request.py
+-rw-r--r--   0        0        0     6269 2024-05-24 22:50:33.762707 ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_update_node_components_request_camera.py
+-rw-r--r--   0        0        0     2402 2024-05-24 22:50:33.818707 ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_update_node_components_request_mount.py
+-rw-r--r--   0        0        0     2591 2024-05-24 22:50:33.862708 ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_update_node_components_request_optical_tube.py
+-rw-r--r--   0        0        0     4620 2024-05-24 22:50:33.922708 ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_update_node_request.py
+-rw-r--r--   0        0        0     2525 2024-05-24 22:50:33.978709 ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_video_mode_framerate_property.py
+-rw-r--r--   0        0        0     2224 2024-05-24 22:50:34.018710 ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v2_complete_observation_request.py
+-rw-r--r--   0        0        0        0 2024-05-24 22:50:34.050710 ourskyai_platform_api-1.3.3671/ourskyai_platform_api/py.typed
+-rw-r--r--   0        0        0    12941 2024-05-24 22:50:34.114711 ourskyai_platform_api-1.3.3671/ourskyai_platform_api/rest.py
+-rw-r--r--   0        0        0      751 2024-05-24 22:50:34.174711 ourskyai_platform_api-1.3.3671/pyproject.toml
+-rw-r--r--   0        0        0    10945 1970-01-01 00:00:00.000000 ourskyai_platform_api-1.3.3671/PKG-INFO
```

### Comparing `ourskyai_platform_api-1.3.3668/README.md` & `ourskyai_platform_api-1.3.3671/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # ourskyai-platform-api
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

### Comparing `ourskyai_platform_api-1.3.3668/ourskyai_platform_api/__init__.py` & `ourskyai_platform_api-1.3.3671/ourskyai_platform_api/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 # flake8: noqa
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-__version__ = "1.3.3668"
+__version__ = "1.3.3671"
 
 # import apis into sdk package
 from ourskyai_platform_api.api.default_api import DefaultApi
 
 # import ApiClient
 from ourskyai_platform_api.api_response import ApiResponse
 from ourskyai_platform_api.api_client import ApiClient
```

### Comparing `ourskyai_platform_api-1.3.3668/ourskyai_platform_api/api/default_api.py` & `ourskyai_platform_api-1.3.3671/ourskyai_platform_api/api/default_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import re  # noqa: F401
```

### Comparing `ourskyai_platform_api-1.3.3668/ourskyai_platform_api/api_client.py` & `ourskyai_platform_api-1.3.3671/ourskyai_platform_api/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
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

### Comparing `ourskyai_platform_api-1.3.3668/ourskyai_platform_api/api_response.py` & `ourskyai_platform_api-1.3.3671/ourskyai_platform_api/api_response.py`

 * *Files identical despite different names*

### Comparing `ourskyai_platform_api-1.3.3668/ourskyai_platform_api/configuration.py` & `ourskyai_platform_api-1.3.3671/ourskyai_platform_api/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
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

### Comparing `ourskyai_platform_api-1.3.3668/ourskyai_platform_api/exceptions.py` & `ourskyai_platform_api-1.3.3671/ourskyai_platform_api/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 class OpenApiException(Exception):
```

### Comparing `ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/__init__.py` & `ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 # import models into model package
```

### Comparing `ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/camera_mode.py` & `ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/camera_mode.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/empty_success.py` & `ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/empty_success.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/filter_type.py` & `ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/filter_type.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/fits_header.py` & `ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/fits_header.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/location.py` & `ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/location.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/metric_type.py` & `ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/metric_type.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/mount_type.py` & `ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/mount_type.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/node_state.py` & `ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/node_state.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/optical_tube_type.py` & `ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/optical_tube_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/plate_solve_parameters.py` & `ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/plate_solve_parameters.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/shutter_type.py` & `ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/shutter_type.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/successful_create.py` & `ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/successful_create.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/tracking_type.py` & `ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/tracking_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_auto_focus_instruction.py` & `ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_auto_focus_instruction.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_auto_focus_instruction_coordinates_inner.py` & `ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_auto_focus_instruction_coordinates_inner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_camera.py` & `ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_camera.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_client_token.py` & `ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_client_token.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_complete_observation_request.py` & `ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_complete_observation_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_create_image_set_image_request.py` & `ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_create_image_set_image_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_create_image_set_image_response.py` & `ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_create_image_set_image_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_create_image_set_request.py` & `ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_create_image_set_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_create_mount_request.py` & `ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_create_mount_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_create_node_controller_artifact_request.py` & `ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_create_node_controller_artifact_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_create_node_diagnostic.py` & `ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_create_node_diagnostic.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_create_node_diagnostics_request.py` & `ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_create_node_diagnostics_request.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_create_node_request.py` & `ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_create_node_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_create_optical_tube_request.py` & `ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_create_optical_tube_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_diagnostic_instruction.py` & `ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_diagnostic_instruction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_elevation_mask_point.py` & `ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_elevation_mask_point.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_file_type.py` & `ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_file_type.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_gain_curve.py` & `ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_gain_curve.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_gain_curve_point.py` & `ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_gain_curve_point.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_get_instruction_request.py` & `ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_get_instruction_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_get_nodes.py` & `ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_get_nodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_get_or_create_camera_request.py` & `ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_get_or_create_camera_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_get_or_create_mount_request.py` & `ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_get_or_create_mount_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_get_or_create_optical_tube_request.py` & `ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_get_or_create_optical_tube_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_get_plate_solve_catalog_diff_request.py` & `ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_get_plate_solve_catalog_diff_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_ground_station_participant.py` & `ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_ground_station_participant.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_image_set.py` & `ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_image_set.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_image_set_image.py` & `ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_image_set_image.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_instruction.py` & `ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_instruction.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_metric.py` & `ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_metric.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_mount.py` & `ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_mount.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_node.py` & `ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_node.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_node_controller_artifact.py` & `ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_node_controller_artifact.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_node_diagnostic_type.py` & `ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_node_diagnostic_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_node_with_location.py` & `ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_node_with_location.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_observation_instruction.py` & `ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_observation_instruction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_optical_tube.py` & `ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_optical_tube.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_plate_solve_catalog_file.py` & `ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_plate_solve_catalog_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_plate_solve_catalog_file_download.py` & `ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_plate_solve_catalog_file_download.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_read_noise_point.py` & `ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_read_noise_point.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_release.py` & `ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_release.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_setup_action.py` & `ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_setup_action.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_slew_timing.py` & `ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_slew_timing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_slew_timing_interval.py` & `ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_slew_timing_interval.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_update_node_components_request.py` & `ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_update_node_components_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_update_node_components_request_camera.py` & `ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_update_node_components_request_camera.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_update_node_components_request_mount.py` & `ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_update_node_components_request_mount.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_update_node_components_request_optical_tube.py` & `ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_update_node_components_request_optical_tube.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_update_node_request.py` & `ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_update_node_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v1_video_mode_framerate_property.py` & `ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v1_video_mode_framerate_property.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3668/ourskyai_platform_api/models/v2_complete_observation_request.py` & `ourskyai_platform_api-1.3.3671/ourskyai_platform_api/models/v2_complete_observation_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3668/ourskyai_platform_api/rest.py` & `ourskyai_platform_api-1.3.3671/ourskyai_platform_api/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import io
```

### Comparing `ourskyai_platform_api-1.3.3668/pyproject.toml` & `ourskyai_platform_api-1.3.3671/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ourskyai_platform_api"
-version = "1.3.3668"
+version = "1.3.3671"
 description = "OurSky Platform"
 authors = ["OpenAPI Generator Community <team@openapitools.org>"]
 license = "NoLicense"
 readme = "README.md"
 repository = "https://github.com/GIT_USER_ID/GIT_REPO_ID"
 keywords = ["OpenAPI", "OpenAPI-Generator", "OurSky Platform"]
 include = ["ourskyai_platform_api/py.typed"]
```

### Comparing `ourskyai_platform_api-1.3.3668/PKG-INFO` & `ourskyai_platform_api-1.3.3671/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ourskyai_platform_api
-Version: 1.3.3668
+Version: 1.3.3671
 Summary: OurSky Platform
 Home-page: https://github.com/GIT_USER_ID/GIT_REPO_ID
 License: NoLicense
 Keywords: OpenAPI,OpenAPI-Generator,OurSky Platform
 Author: OpenAPI Generator Community
 Author-email: team@openapitools.org
 Requires-Python: >=3.7,<4.0
@@ -24,16 +24,16 @@
 Description-Content-Type: text/markdown
 
 # ourskyai-platform-api
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

