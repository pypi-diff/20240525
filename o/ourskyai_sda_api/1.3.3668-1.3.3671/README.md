# Comparing `tmp/ourskyai_sda_api-1.3.3668.tar.gz` & `tmp/ourskyai_sda_api-1.3.3671.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ourskyai_sda_api-1.3.3668.tar", max compression
+gzip compressed data, was "ourskyai_sda_api-1.3.3671.tar", max compression
```

## Comparing `ourskyai_sda_api-1.3.3668.tar` & `ourskyai_sda_api-1.3.3671.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0    10151 2024-05-24 20:17:11.100959 ourskyai_sda_api-1.3.3668/README.md
--rw-r--r--   0        0        0     5222 2024-05-24 20:17:14.184994 ourskyai_sda_api-1.3.3668/ourskyai_sda_api/__init__.py
--rw-r--r--   0        0        0      104 2024-05-24 20:17:14.216994 ourskyai_sda_api-1.3.3668/ourskyai_sda_api/api/__init__.py
--rw-r--r--   0        0        0   220784 2024-05-24 20:17:14.320995 ourskyai_sda_api-1.3.3668/ourskyai_sda_api/api/default_api.py
--rw-r--r--   0        0        0    30830 2024-05-24 20:17:14.396996 ourskyai_sda_api-1.3.3668/ourskyai_sda_api/api_client.py
--rw-r--r--   0        0        0      852 2024-05-24 20:17:14.440997 ourskyai_sda_api-1.3.3668/ourskyai_sda_api/api_response.py
--rw-r--r--   0        0        0    15175 2024-05-24 20:17:14.488997 ourskyai_sda_api-1.3.3668/ourskyai_sda_api/configuration.py
--rw-r--r--   0        0        0     5923 2024-05-24 20:17:14.524998 ourskyai_sda_api-1.3.3668/ourskyai_sda_api/exceptions.py
--rw-r--r--   0        0        0     4601 2024-05-24 20:17:14.568998 ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/__init__.py
--rw-r--r--   0        0        0     4311 2024-05-24 20:17:14.616999 ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/astrometric_offsets.py
--rw-r--r--   0        0        0     2394 2024-05-24 20:17:14.737000 ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/empty_success.py
--rw-r--r--   0        0        0     1676 2024-05-24 20:17:14.781000 ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/filter_type.py
--rw-r--r--   0        0        0     2420 2024-05-24 20:17:14.817001 ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/fits_header.py
--rw-r--r--   0        0        0     2645 2024-05-24 20:17:14.861001 ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/location.py
--rw-r--r--   0        0        0     1237 2024-05-24 20:17:14.917002 ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/mount_type.py
--rw-r--r--   0        0        0     2756 2024-05-24 20:17:14.961002 ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/observation_bounding_box.py
--rw-r--r--   0        0        0     3713 2024-05-24 20:17:15.029003 ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/observation_quality.py
--rw-r--r--   0        0        0     6381 2024-05-24 20:17:15.117004 ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/observation_result.py
--rw-r--r--   0        0        0     1320 2024-05-24 20:17:15.153005 ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/observation_state.py
--rw-r--r--   0        0        0     1529 2024-05-24 20:17:15.253006 ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/orbit_type.py
--rw-r--r--   0        0        0     1361 2024-05-24 20:17:15.309006 ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/satellite_target_tracking_status.py
--rw-r--r--   0        0        0     1241 2024-05-24 20:17:15.349007 ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/shutter_type.py
--rw-r--r--   0        0        0     2382 2024-05-24 20:17:15.401008 ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/successful_create.py
--rw-r--r--   0        0        0     1258 2024-05-24 20:17:15.445008 ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/tracking_type.py
--rw-r--r--   0        0        0     2534 2024-05-24 20:17:15.513009 ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/v1_create_image_set_image_request.py
--rw-r--r--   0        0        0     2605 2024-05-24 20:17:15.577009 ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/v1_create_image_set_image_response.py
--rw-r--r--   0        0        0     3169 2024-05-24 20:17:15.629010 ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/v1_create_image_set_request.py
--rw-r--r--   0        0        0     2609 2024-05-24 20:17:15.681011 ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/v1_create_organization_target_request.py
--rw-r--r--   0        0        0     2761 2024-05-24 20:17:15.733011 ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/v1_create_satellite_target_request.py
--rw-r--r--   0        0        0     3373 2024-05-24 20:17:15.785012 ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/v1_create_search_instruction_request.py
--rw-r--r--   0        0        0     3353 2024-05-24 20:17:15.821012 ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/v1_create_survey_instruction_request.py
--rw-r--r--   0        0        0     3017 2024-05-24 20:17:15.909013 ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/v1_get_satellite_targets_response.py
--rw-r--r--   0        0        0     4457 2024-05-24 20:17:15.965014 ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/v1_ground_station_participant.py
--rw-r--r--   0        0        0     3922 2024-05-24 20:17:16.009014 ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/v1_image_set.py
--rw-r--r--   0        0        0     6285 2024-05-24 20:17:16.057015 ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/v1_image_set_image.py
--rw-r--r--   0        0        0     4676 2024-05-24 20:17:16.093015 ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/v1_observation_feature.py
--rw-r--r--   0        0        0     3748 2024-05-24 20:17:16.153016 ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/v1_observation_sequence_result.py
--rw-r--r--   0        0        0     4306 2024-05-24 20:17:16.197016 ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/v1_observation_sequence_result_image_sets_inner.py
--rw-r--r--   0        0        0     4637 2024-05-24 20:17:16.245017 ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/v1_observation_status.py
--rw-r--r--   0        0        0     3192 2024-05-24 20:17:16.337018 ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/v1_organization_target.py
--rw-r--r--   0        0        0     3644 2024-05-24 20:17:16.425019 ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/v1_satellite_potential.py
--rw-r--r--   0        0        0     3528 2024-05-24 20:17:16.469020 ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/v1_satellite_target.py
--rw-r--r--   0        0        0     3733 2024-05-24 20:17:16.517020 ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/v1_search_instruction.py
--rw-r--r--   0        0        0     3407 2024-05-24 20:17:16.585021 ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/v1_search_instruction_step.py
--rw-r--r--   0        0        0     3634 2024-05-24 20:17:16.641021 ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/v1_survey_instruction.py
--rw-r--r--   0        0        0     2799 2024-05-24 20:17:16.689022 ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/v1_survey_instruction_step.py
--rw-r--r--   0        0        0     3716 2024-05-24 20:17:16.741022 ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/v1_target_correlation.py
--rw-r--r--   0        0        0     3185 2024-05-24 20:17:16.793023 ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/v1_tdm.py
--rw-r--r--   0        0        0     2575 2024-05-24 20:17:16.845024 ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/v1_update_email_configuration_request.py
--rw-r--r--   0        0        0     2913 2024-05-24 20:17:16.901024 ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/v1_update_satellite_target_request.py
--rw-r--r--   0        0        0     3146 2024-05-24 20:17:16.977025 ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/v1_update_webhook_configuration_request.py
--rw-r--r--   0        0        0     2963 2024-05-24 20:17:17.025026 ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/v1_webhook_configuration.py
--rw-r--r--   0        0        0     1386 2024-05-24 20:17:17.073026 ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/weather_condition.py
--rw-r--r--   0        0        0     1350 2024-05-24 20:17:17.117027 ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/webhook_auth_type.py
--rw-r--r--   0        0        0     1734 2024-05-24 20:17:17.169027 ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/webhook_event.py
--rw-r--r--   0        0        0        0 2024-05-24 20:17:17.201028 ourskyai_sda_api-1.3.3668/ourskyai_sda_api/py.typed
--rw-r--r--   0        0        0    13423 2024-05-24 20:17:17.269029 ourskyai_sda_api-1.3.3668/ourskyai_sda_api/rest.py
--rw-r--r--   0        0        0      731 2024-05-24 20:17:17.317029 ourskyai_sda_api-1.3.3668/pyproject.toml
--rw-r--r--   0        0        0    11113 1970-01-01 00:00:00.000000 ourskyai_sda_api-1.3.3668/PKG-INFO
+-rw-r--r--   0        0        0    10151 2024-05-24 22:50:26.018619 ourskyai_sda_api-1.3.3671/README.md
+-rw-r--r--   0        0        0     5222 2024-05-24 22:50:28.950652 ourskyai_sda_api-1.3.3671/ourskyai_sda_api/__init__.py
+-rw-r--r--   0        0        0      104 2024-05-24 22:50:28.982653 ourskyai_sda_api-1.3.3671/ourskyai_sda_api/api/__init__.py
+-rw-r--r--   0        0        0   220784 2024-05-24 22:50:29.074653 ourskyai_sda_api-1.3.3671/ourskyai_sda_api/api/default_api.py
+-rw-r--r--   0        0        0    30830 2024-05-24 22:50:29.122654 ourskyai_sda_api-1.3.3671/ourskyai_sda_api/api_client.py
+-rw-r--r--   0        0        0      852 2024-05-24 22:50:29.178655 ourskyai_sda_api-1.3.3671/ourskyai_sda_api/api_response.py
+-rw-r--r--   0        0        0    15175 2024-05-24 22:50:29.242656 ourskyai_sda_api-1.3.3671/ourskyai_sda_api/configuration.py
+-rw-r--r--   0        0        0     5923 2024-05-24 22:50:29.294656 ourskyai_sda_api-1.3.3671/ourskyai_sda_api/exceptions.py
+-rw-r--r--   0        0        0     4601 2024-05-24 22:50:29.374657 ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/__init__.py
+-rw-r--r--   0        0        0     4311 2024-05-24 22:50:29.418658 ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/astrometric_offsets.py
+-rw-r--r--   0        0        0     2394 2024-05-24 22:50:29.478658 ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/empty_success.py
+-rw-r--r--   0        0        0     1676 2024-05-24 22:50:29.554659 ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/filter_type.py
+-rw-r--r--   0        0        0     2420 2024-05-24 22:50:29.614660 ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/fits_header.py
+-rw-r--r--   0        0        0     2645 2024-05-24 22:50:29.662660 ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/location.py
+-rw-r--r--   0        0        0     1237 2024-05-24 22:50:29.698661 ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/mount_type.py
+-rw-r--r--   0        0        0     2756 2024-05-24 22:50:29.734661 ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/observation_bounding_box.py
+-rw-r--r--   0        0        0     3713 2024-05-24 22:50:29.770661 ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/observation_quality.py
+-rw-r--r--   0        0        0     6381 2024-05-24 22:50:29.826662 ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/observation_result.py
+-rw-r--r--   0        0        0     1320 2024-05-24 22:50:29.882663 ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/observation_state.py
+-rw-r--r--   0        0        0     1529 2024-05-24 22:50:29.930663 ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/orbit_type.py
+-rw-r--r--   0        0        0     1361 2024-05-24 22:50:29.974664 ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/satellite_target_tracking_status.py
+-rw-r--r--   0        0        0     1241 2024-05-24 22:50:30.038665 ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/shutter_type.py
+-rw-r--r--   0        0        0     2382 2024-05-24 22:50:30.086665 ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/successful_create.py
+-rw-r--r--   0        0        0     1258 2024-05-24 22:50:30.130666 ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/tracking_type.py
+-rw-r--r--   0        0        0     2534 2024-05-24 22:50:30.182666 ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/v1_create_image_set_image_request.py
+-rw-r--r--   0        0        0     2605 2024-05-24 22:50:30.246667 ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/v1_create_image_set_image_response.py
+-rw-r--r--   0        0        0     3169 2024-05-24 22:50:30.302667 ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/v1_create_image_set_request.py
+-rw-r--r--   0        0        0     2609 2024-05-24 22:50:30.362668 ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/v1_create_organization_target_request.py
+-rw-r--r--   0        0        0     2761 2024-05-24 22:50:30.410669 ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/v1_create_satellite_target_request.py
+-rw-r--r--   0        0        0     3373 2024-05-24 22:50:30.450669 ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/v1_create_search_instruction_request.py
+-rw-r--r--   0        0        0     3353 2024-05-24 22:50:30.514670 ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/v1_create_survey_instruction_request.py
+-rw-r--r--   0        0        0     3017 2024-05-24 22:50:30.578671 ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/v1_get_satellite_targets_response.py
+-rw-r--r--   0        0        0     4457 2024-05-24 22:50:30.638671 ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/v1_ground_station_participant.py
+-rw-r--r--   0        0        0     3922 2024-05-24 22:50:30.690672 ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/v1_image_set.py
+-rw-r--r--   0        0        0     6285 2024-05-24 22:50:30.734672 ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/v1_image_set_image.py
+-rw-r--r--   0        0        0     4676 2024-05-24 22:50:30.794673 ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/v1_observation_feature.py
+-rw-r--r--   0        0        0     3748 2024-05-24 22:50:30.850674 ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/v1_observation_sequence_result.py
+-rw-r--r--   0        0        0     4306 2024-05-24 22:50:30.906674 ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/v1_observation_sequence_result_image_sets_inner.py
+-rw-r--r--   0        0        0     4637 2024-05-24 22:50:30.958675 ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/v1_observation_status.py
+-rw-r--r--   0        0        0     3192 2024-05-24 22:50:31.018676 ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/v1_organization_target.py
+-rw-r--r--   0        0        0     3644 2024-05-24 22:50:31.098677 ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/v1_satellite_potential.py
+-rw-r--r--   0        0        0     3528 2024-05-24 22:50:31.142677 ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/v1_satellite_target.py
+-rw-r--r--   0        0        0     3733 2024-05-24 22:50:31.190678 ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/v1_search_instruction.py
+-rw-r--r--   0        0        0     3407 2024-05-24 22:50:31.234678 ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/v1_search_instruction_step.py
+-rw-r--r--   0        0        0     3634 2024-05-24 22:50:31.306679 ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/v1_survey_instruction.py
+-rw-r--r--   0        0        0     2799 2024-05-24 22:50:31.350679 ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/v1_survey_instruction_step.py
+-rw-r--r--   0        0        0     3716 2024-05-24 22:50:31.406680 ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/v1_target_correlation.py
+-rw-r--r--   0        0        0     3185 2024-05-24 22:50:31.474681 ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/v1_tdm.py
+-rw-r--r--   0        0        0     2575 2024-05-24 22:50:31.530681 ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/v1_update_email_configuration_request.py
+-rw-r--r--   0        0        0     2913 2024-05-24 22:50:31.574682 ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/v1_update_satellite_target_request.py
+-rw-r--r--   0        0        0     3146 2024-05-24 22:50:31.618682 ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/v1_update_webhook_configuration_request.py
+-rw-r--r--   0        0        0     2963 2024-05-24 22:50:31.658683 ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/v1_webhook_configuration.py
+-rw-r--r--   0        0        0     1386 2024-05-24 22:50:31.702683 ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/weather_condition.py
+-rw-r--r--   0        0        0     1350 2024-05-24 22:50:31.746684 ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/webhook_auth_type.py
+-rw-r--r--   0        0        0     1734 2024-05-24 22:50:31.826685 ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/webhook_event.py
+-rw-r--r--   0        0        0        0 2024-05-24 22:50:31.854685 ourskyai_sda_api-1.3.3671/ourskyai_sda_api/py.typed
+-rw-r--r--   0        0        0    13423 2024-05-24 22:50:31.926686 ourskyai_sda_api-1.3.3671/ourskyai_sda_api/rest.py
+-rw-r--r--   0        0        0      731 2024-05-24 22:50:31.982687 ourskyai_sda_api-1.3.3671/pyproject.toml
+-rw-r--r--   0        0        0    11113 1970-01-01 00:00:00.000000 ourskyai_sda_api-1.3.3671/PKG-INFO
```

### Comparing `ourskyai_sda_api-1.3.3668/README.md` & `ourskyai_sda_api-1.3.3671/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 The basic flow for a new organization is as follows:
 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe.
 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above.
 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
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

### Comparing `ourskyai_sda_api-1.3.3668/ourskyai_sda_api/__init__.py` & `ourskyai_sda_api-1.3.3671/ourskyai_sda_api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 # flake8: noqa
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-__version__ = "1.3.3668"
+__version__ = "1.3.3671"
 
 # import apis into sdk package
 from ourskyai_sda_api.api.default_api import DefaultApi
 
 # import ApiClient
 from ourskyai_sda_api.api_response import ApiResponse
 from ourskyai_sda_api.api_client import ApiClient
```

### Comparing `ourskyai_sda_api-1.3.3668/ourskyai_sda_api/api/default_api.py` & `ourskyai_sda_api-1.3.3671/ourskyai_sda_api/api/default_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import re  # noqa: F401
```

### Comparing `ourskyai_sda_api-1.3.3668/ourskyai_sda_api/api_client.py` & `ourskyai_sda_api-1.3.3671/ourskyai_sda_api/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
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

### Comparing `ourskyai_sda_api-1.3.3668/ourskyai_sda_api/api_response.py` & `ourskyai_sda_api-1.3.3671/ourskyai_sda_api/api_response.py`

 * *Files identical despite different names*

### Comparing `ourskyai_sda_api-1.3.3668/ourskyai_sda_api/configuration.py` & `ourskyai_sda_api-1.3.3671/ourskyai_sda_api/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
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

### Comparing `ourskyai_sda_api-1.3.3668/ourskyai_sda_api/exceptions.py` & `ourskyai_sda_api-1.3.3671/ourskyai_sda_api/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 class OpenApiException(Exception):
```

### Comparing `ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/__init__.py` & `ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 # import models into model package
```

### Comparing `ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/astrometric_offsets.py` & `ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/astrometric_offsets.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/empty_success.py` & `ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/empty_success.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/filter_type.py` & `ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/filter_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/fits_header.py` & `ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/fits_header.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/location.py` & `ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/location.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/mount_type.py` & `ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/mount_type.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/observation_bounding_box.py` & `ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/observation_bounding_box.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/observation_quality.py` & `ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/observation_quality.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/observation_result.py` & `ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/observation_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/observation_state.py` & `ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/observation_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/orbit_type.py` & `ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/orbit_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/satellite_target_tracking_status.py` & `ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/satellite_target_tracking_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/shutter_type.py` & `ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/shutter_type.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/successful_create.py` & `ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/successful_create.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/tracking_type.py` & `ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/tracking_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/v1_create_image_set_image_request.py` & `ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/v1_create_image_set_image_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/v1_create_image_set_image_response.py` & `ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/v1_create_image_set_image_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/v1_create_image_set_request.py` & `ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/v1_create_image_set_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/v1_create_organization_target_request.py` & `ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/v1_create_organization_target_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/v1_create_satellite_target_request.py` & `ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/v1_create_satellite_target_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/v1_create_search_instruction_request.py` & `ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/v1_create_search_instruction_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/v1_create_survey_instruction_request.py` & `ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/v1_create_survey_instruction_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/v1_get_satellite_targets_response.py` & `ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/v1_get_satellite_targets_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/v1_ground_station_participant.py` & `ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/v1_ground_station_participant.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/v1_image_set.py` & `ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/v1_image_set.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/v1_image_set_image.py` & `ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/v1_image_set_image.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/v1_observation_feature.py` & `ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/v1_observation_feature.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/v1_observation_sequence_result.py` & `ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/v1_observation_sequence_result.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/v1_observation_sequence_result_image_sets_inner.py` & `ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/v1_observation_sequence_result_image_sets_inner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/v1_observation_status.py` & `ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/v1_observation_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/v1_organization_target.py` & `ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/v1_organization_target.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/v1_satellite_potential.py` & `ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/v1_satellite_potential.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/v1_satellite_target.py` & `ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/v1_satellite_target.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/v1_search_instruction.py` & `ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/v1_search_instruction.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/v1_search_instruction_step.py` & `ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/v1_search_instruction_step.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/v1_survey_instruction.py` & `ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/v1_survey_instruction.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/v1_survey_instruction_step.py` & `ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/v1_survey_instruction_step.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/v1_target_correlation.py` & `ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/v1_target_correlation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/v1_tdm.py` & `ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/v1_tdm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/v1_update_email_configuration_request.py` & `ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/v1_update_email_configuration_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/v1_update_satellite_target_request.py` & `ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/v1_update_satellite_target_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/v1_update_webhook_configuration_request.py` & `ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/v1_update_webhook_configuration_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/v1_webhook_configuration.py` & `ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/v1_webhook_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/weather_condition.py` & `ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/weather_condition.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/webhook_auth_type.py` & `ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/webhook_auth_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_sda_api-1.3.3668/ourskyai_sda_api/models/webhook_event.py` & `ourskyai_sda_api-1.3.3671/ourskyai_sda_api/models/webhook_event.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_sda_api-1.3.3668/ourskyai_sda_api/rest.py` & `ourskyai_sda_api-1.3.3671/ourskyai_sda_api/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3668
+    The version of the OpenAPI document: 1.3.3671
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import io
```

### Comparing `ourskyai_sda_api-1.3.3668/pyproject.toml` & `ourskyai_sda_api-1.3.3671/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ourskyai_sda_api"
-version = "1.3.3668"
+version = "1.3.3671"
 description = "OurSky SDA"
 authors = ["OpenAPI Generator Community <team@openapitools.org>"]
 license = "NoLicense"
 readme = "README.md"
 repository = "https://github.com/GIT_USER_ID/GIT_REPO_ID"
 keywords = ["OpenAPI", "OpenAPI-Generator", "OurSky SDA"]
 include = ["ourskyai_sda_api/py.typed"]
```

### Comparing `ourskyai_sda_api-1.3.3668/PKG-INFO` & `ourskyai_sda_api-1.3.3671/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ourskyai_sda_api
-Version: 1.3.3668
+Version: 1.3.3671
 Summary: OurSky SDA
 Home-page: https://github.com/GIT_USER_ID/GIT_REPO_ID
 License: NoLicense
 Keywords: OpenAPI,OpenAPI-Generator,OurSky SDA
 Author: OpenAPI Generator Community
 Author-email: team@openapitools.org
 Requires-Python: >=3.7,<4.0
@@ -27,16 +27,16 @@
 The basic flow for a new organization is as follows:
 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe.
 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above.
 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
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

