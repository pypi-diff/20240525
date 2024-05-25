# Comparing `tmp/inference-0.9.9-py3-none-any.whl.zip` & `tmp/inference-0.9.9rc23-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,224 +1,224 @@
-Zip file size: 282101 bytes, number of entries: 222
--rw-r--r--  2.0 unx      209 b- defN 24-Feb-07 17:23 inference/__init__.py
--rw-r--r--  2.0 unx     1728 b- defN 24-Feb-07 17:23 inference/core/__init__.py
--rw-r--r--  2.0 unx      183 b- defN 24-Feb-07 17:23 inference/core/constants.py
--rw-r--r--  2.0 unx    12459 b- defN 24-Feb-07 17:23 inference/core/env.py
--rw-r--r--  2.0 unx     3611 b- defN 24-Feb-07 17:23 inference/core/exceptions.py
--rw-r--r--  2.0 unx      371 b- defN 24-Feb-07 17:23 inference/core/logger.py
--rw-r--r--  2.0 unx     6486 b- defN 24-Feb-07 17:23 inference/core/nms.py
--rw-r--r--  2.0 unx    12130 b- defN 24-Feb-07 17:23 inference/core/roboflow_api.py
--rw-r--r--  2.0 unx     2216 b- defN 24-Feb-07 17:23 inference/core/usage.py
--rw-r--r--  2.0 unx       74 b- defN 24-Feb-07 17:23 inference/core/version.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-07 17:23 inference/core/active_learning/__init__.py
--rw-r--r--  2.0 unx     2933 b- defN 24-Feb-07 17:23 inference/core/active_learning/accounting.py
--rw-r--r--  2.0 unx      986 b- defN 24-Feb-07 17:23 inference/core/active_learning/batching.py
--rw-r--r--  2.0 unx     8948 b- defN 24-Feb-07 17:23 inference/core/active_learning/cache_operations.py
--rw-r--r--  2.0 unx     6493 b- defN 24-Feb-07 17:23 inference/core/active_learning/configuration.py
--rw-r--r--  2.0 unx     7126 b- defN 24-Feb-07 17:23 inference/core/active_learning/core.py
--rw-r--r--  2.0 unx     4541 b- defN 24-Feb-07 17:23 inference/core/active_learning/entities.py
--rw-r--r--  2.0 unx     8845 b- defN 24-Feb-07 17:23 inference/core/active_learning/middlewares.py
--rw-r--r--  2.0 unx     4036 b- defN 24-Feb-07 17:23 inference/core/active_learning/post_processing.py
--rw-r--r--  2.0 unx      458 b- defN 24-Feb-07 17:23 inference/core/active_learning/utils.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-07 17:23 inference/core/active_learning/samplers/__init__.py
--rw-r--r--  2.0 unx     7302 b- defN 24-Feb-07 17:23 inference/core/active_learning/samplers/close_to_threshold.py
--rw-r--r--  2.0 unx     1725 b- defN 24-Feb-07 17:23 inference/core/active_learning/samplers/contains_classes.py
--rw-r--r--  2.0 unx     3488 b- defN 24-Feb-07 17:23 inference/core/active_learning/samplers/number_of_detections.py
--rw-r--r--  2.0 unx     1018 b- defN 24-Feb-07 17:23 inference/core/active_learning/samplers/random.py
--rw-r--r--  2.0 unx      813 b- defN 24-Feb-07 17:23 inference/core/cache/__init__.py
--rw-r--r--  2.0 unx     3443 b- defN 24-Feb-07 17:23 inference/core/cache/base.py
--rw-r--r--  2.0 unx     5884 b- defN 24-Feb-07 17:23 inference/core/cache/memory.py
--rw-r--r--  2.0 unx     2858 b- defN 24-Feb-07 17:23 inference/core/cache/model_artifacts.py
--rw-r--r--  2.0 unx     6401 b- defN 24-Feb-07 17:23 inference/core/cache/redis.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-07 17:23 inference/core/devices/__init__.py
--rw-r--r--  2.0 unx     3803 b- defN 24-Feb-07 17:23 inference/core/devices/utils.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-07 17:23 inference/core/entities/__init__.py
--rw-r--r--  2.0 unx      428 b- defN 24-Feb-07 17:23 inference/core/entities/common.py
--rw-r--r--  2.0 unx       81 b- defN 24-Feb-07 17:23 inference/core/entities/types.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-07 17:23 inference/core/entities/requests/__init__.py
--rw-r--r--  2.0 unx     3142 b- defN 24-Feb-07 17:23 inference/core/entities/requests/clip.py
--rw-r--r--  2.0 unx     1890 b- defN 24-Feb-07 17:23 inference/core/entities/requests/cogvlm.py
--rw-r--r--  2.0 unx     1002 b- defN 24-Feb-07 17:23 inference/core/entities/requests/doctr.py
--rw-r--r--  2.0 unx     1918 b- defN 24-Feb-07 17:23 inference/core/entities/requests/gaze.py
--rw-r--r--  2.0 unx      544 b- defN 24-Feb-07 17:23 inference/core/entities/requests/groundingdino.py
--rw-r--r--  2.0 unx     9765 b- defN 24-Feb-07 17:23 inference/core/entities/requests/inference.py
--rw-r--r--  2.0 unx     6929 b- defN 24-Feb-07 17:23 inference/core/entities/requests/sam.py
--rw-r--r--  2.0 unx      968 b- defN 24-Feb-07 17:23 inference/core/entities/requests/server_state.py
--rw-r--r--  2.0 unx      853 b- defN 24-Feb-07 17:23 inference/core/entities/requests/workflows.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-07 17:23 inference/core/entities/responses/__init__.py
--rw-r--r--  2.0 unx     1531 b- defN 24-Feb-07 17:23 inference/core/entities/responses/clip.py
--rw-r--r--  2.0 unx      322 b- defN 24-Feb-07 17:23 inference/core/entities/responses/cogvlm.py
--rw-r--r--  2.0 unx      727 b- defN 24-Feb-07 17:23 inference/core/entities/responses/doctr.py
--rw-r--r--  2.0 unx     1303 b- defN 24-Feb-07 17:23 inference/core/entities/responses/gaze.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-07 17:23 inference/core/entities/responses/groundingdino.py
--rw-r--r--  2.0 unx    12378 b- defN 24-Feb-07 17:23 inference/core/entities/responses/inference.py
--rw-r--r--  2.0 unx      300 b- defN 24-Feb-07 17:23 inference/core/entities/responses/notebooks.py
--rw-r--r--  2.0 unx     2207 b- defN 24-Feb-07 17:23 inference/core/entities/responses/sam.py
--rw-r--r--  2.0 unx     2305 b- defN 24-Feb-07 17:23 inference/core/entities/responses/server_state.py
--rw-r--r--  2.0 unx      249 b- defN 24-Feb-07 17:23 inference/core/entities/responses/workflows.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-07 17:23 inference/core/interfaces/__init__.py
--rw-r--r--  2.0 unx      261 b- defN 24-Feb-07 17:23 inference/core/interfaces/base.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-07 17:23 inference/core/interfaces/camera/__init__.py
--rw-r--r--  2.0 unx     5517 b- defN 24-Feb-07 17:23 inference/core/interfaces/camera/camera.py
--rw-r--r--  2.0 unx     1621 b- defN 24-Feb-07 17:23 inference/core/interfaces/camera/entities.py
--rw-r--r--  2.0 unx      202 b- defN 24-Feb-07 17:23 inference/core/interfaces/camera/exceptions.py
--rw-r--r--  2.0 unx     4000 b- defN 24-Feb-07 17:23 inference/core/interfaces/camera/utils.py
--rw-r--r--  2.0 unx    41415 b- defN 24-Feb-07 17:23 inference/core/interfaces/camera/video_source.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-07 17:23 inference/core/interfaces/http/__init__.py
--rw-r--r--  2.0 unx    61261 b- defN 24-Feb-07 17:23 inference/core/interfaces/http/http_api.py
--rw-r--r--  2.0 unx     2384 b- defN 24-Feb-07 17:23 inference/core/interfaces/http/orjson_utils.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-07 17:23 inference/core/interfaces/stream/__init__.py
--rw-r--r--  2.0 unx     3784 b- defN 24-Feb-07 17:23 inference/core/interfaces/stream/entities.py
--rw-r--r--  2.0 unx    21169 b- defN 24-Feb-07 17:23 inference/core/interfaces/stream/inference_pipeline.py
--rw-r--r--  2.0 unx    13697 b- defN 24-Feb-07 17:23 inference/core/interfaces/stream/sinks.py
--rw-r--r--  2.0 unx    12281 b- defN 24-Feb-07 17:23 inference/core/interfaces/stream/stream.py
--rw-r--r--  2.0 unx    10930 b- defN 24-Feb-07 17:23 inference/core/interfaces/stream/watchdog.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-07 17:23 inference/core/interfaces/udp/__init__.py
--rw-r--r--  2.0 unx    11027 b- defN 24-Feb-07 17:23 inference/core/interfaces/udp/udp_stream.py
--rw-r--r--  2.0 unx        1 b- defN 24-Feb-07 17:23 inference/core/managers/__init__.py
--rw-r--r--  2.0 unx     5907 b- defN 24-Feb-07 17:23 inference/core/managers/active_learning.py
--rw-r--r--  2.0 unx    11690 b- defN 24-Feb-07 17:23 inference/core/managers/base.py
--rw-r--r--  2.0 unx      242 b- defN 24-Feb-07 17:23 inference/core/managers/entities.py
--rw-r--r--  2.0 unx     3703 b- defN 24-Feb-07 17:23 inference/core/managers/metrics.py
--rw-r--r--  2.0 unx     5306 b- defN 24-Feb-07 17:23 inference/core/managers/pingback.py
--rw-r--r--  2.0 unx      675 b- defN 24-Feb-07 17:23 inference/core/managers/stub_loader.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-07 17:23 inference/core/managers/decorators/__init__.py
--rw-r--r--  2.0 unx     6222 b- defN 24-Feb-07 17:23 inference/core/managers/decorators/base.py
--rw-r--r--  2.0 unx     4286 b- defN 24-Feb-07 17:23 inference/core/managers/decorators/fixed_size_cache.py
--rw-r--r--  2.0 unx      487 b- defN 24-Feb-07 17:23 inference/core/managers/decorators/locked_load.py
--rw-r--r--  2.0 unx     1990 b- defN 24-Feb-07 17:23 inference/core/managers/decorators/logger.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-07 17:23 inference/core/models/__init__.py
--rw-r--r--  2.0 unx     5316 b- defN 24-Feb-07 17:23 inference/core/models/base.py
--rw-r--r--  2.0 unx    16272 b- defN 24-Feb-07 17:23 inference/core/models/classification_base.py
--rw-r--r--  2.0 unx    13358 b- defN 24-Feb-07 17:23 inference/core/models/instance_segmentation_base.py
--rw-r--r--  2.0 unx     7645 b- defN 24-Feb-07 17:23 inference/core/models/keypoints_detection_base.py
--rw-r--r--  2.0 unx    12638 b- defN 24-Feb-07 17:23 inference/core/models/object_detection_base.py
--rw-r--r--  2.0 unx    32993 b- defN 24-Feb-07 17:23 inference/core/models/roboflow.py
--rw-r--r--  2.0 unx     4805 b- defN 24-Feb-07 17:23 inference/core/models/stubs.py
--rw-r--r--  2.0 unx      103 b- defN 24-Feb-07 17:23 inference/core/models/types.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-07 17:23 inference/core/models/utils/__init__.py
--rw-r--r--  2.0 unx      619 b- defN 24-Feb-07 17:23 inference/core/models/utils/batching.py
--rw-r--r--  2.0 unx     1492 b- defN 24-Feb-07 17:23 inference/core/models/utils/keypoints.py
--rw-r--r--  2.0 unx      173 b- defN 24-Feb-07 17:23 inference/core/models/utils/validate.py
--rw-r--r--  2.0 unx        1 b- defN 24-Feb-07 17:23 inference/core/registries/__init__.py
--rw-r--r--  2.0 unx     1395 b- defN 24-Feb-07 17:23 inference/core/registries/base.py
--rw-r--r--  2.0 unx     8545 b- defN 24-Feb-07 17:23 inference/core/registries/roboflow.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-07 17:23 inference/core/utils/__init__.py
--rw-r--r--  2.0 unx     2104 b- defN 24-Feb-07 17:23 inference/core/utils/environment.py
--rw-r--r--  2.0 unx     1908 b- defN 24-Feb-07 17:23 inference/core/utils/file_system.py
--rw-r--r--  2.0 unx    14257 b- defN 24-Feb-07 17:23 inference/core/utils/image_utils.py
--rw-r--r--  2.0 unx      679 b- defN 24-Feb-07 17:23 inference/core/utils/notebooks.py
--rw-r--r--  2.0 unx      660 b- defN 24-Feb-07 17:23 inference/core/utils/onnx.py
--rw-r--r--  2.0 unx    21533 b- defN 24-Feb-07 17:23 inference/core/utils/postprocess.py
--rw-r--r--  2.0 unx     8381 b- defN 24-Feb-07 17:23 inference/core/utils/preprocess.py
--rw-r--r--  2.0 unx      712 b- defN 24-Feb-07 17:23 inference/core/utils/requests.py
--rw-r--r--  2.0 unx      419 b- defN 24-Feb-07 17:23 inference/core/utils/roboflow.py
--rw-r--r--  2.0 unx      430 b- defN 24-Feb-07 17:23 inference/core/utils/s3.py
--rw-r--r--  2.0 unx      244 b- defN 24-Feb-07 17:23 inference/core/utils/url_utils.py
--rw-r--r--  2.0 unx     4444 b- defN 24-Feb-07 17:23 inference/core/utils/visualisation.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-07 17:23 inference/enterprise/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-07 17:23 inference/enterprise/device_manager/__init__.py
--rw-r--r--  2.0 unx     2902 b- defN 24-Feb-07 17:23 inference/enterprise/device_manager/command_handler.py
--rw-r--r--  2.0 unx     9478 b- defN 24-Feb-07 17:23 inference/enterprise/device_manager/container_service.py
--rw-r--r--  2.0 unx     1825 b- defN 24-Feb-07 17:23 inference/enterprise/device_manager/device_manager.py
--rw-r--r--  2.0 unx     1514 b- defN 24-Feb-07 17:23 inference/enterprise/device_manager/helpers.py
--rw-r--r--  2.0 unx     5353 b- defN 24-Feb-07 17:23 inference/enterprise/device_manager/metrics_service.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-07 17:23 inference/enterprise/parallel/__init__.py
--rw-r--r--  2.0 unx       53 b- defN 24-Feb-07 17:23 inference/enterprise/parallel/celeryconfig.py
--rw-r--r--  2.0 unx     5502 b- defN 24-Feb-07 17:23 inference/enterprise/parallel/dispatch_manager.py
--rw-r--r--  2.0 unx      719 b- defN 24-Feb-07 17:23 inference/enterprise/parallel/entrypoint.py
--rw-r--r--  2.0 unx     7761 b- defN 24-Feb-07 17:23 inference/enterprise/parallel/infer.py
--rw-r--r--  2.0 unx     1157 b- defN 24-Feb-07 17:23 inference/enterprise/parallel/parallel_http_api.py
--rw-r--r--  2.0 unx      786 b- defN 24-Feb-07 17:23 inference/enterprise/parallel/parallel_http_config.py
--rw-r--r--  2.0 unx     4949 b- defN 24-Feb-07 17:23 inference/enterprise/parallel/tasks.py
--rw-r--r--  2.0 unx     1784 b- defN 24-Feb-07 17:23 inference/enterprise/parallel/utils.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-07 17:23 inference/enterprise/stream_management/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-07 17:23 inference/enterprise/stream_management/api/__init__.py
--rw-r--r--  2.0 unx     6192 b- defN 24-Feb-07 17:23 inference/enterprise/stream_management/api/app.py
--rw-r--r--  2.0 unx     3843 b- defN 24-Feb-07 17:23 inference/enterprise/stream_management/api/entities.py
--rw-r--r--  2.0 unx      512 b- defN 24-Feb-07 17:23 inference/enterprise/stream_management/api/errors.py
--rw-r--r--  2.0 unx     9550 b- defN 24-Feb-07 17:23 inference/enterprise/stream_management/api/stream_manager_client.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-07 17:23 inference/enterprise/stream_management/manager/__init__.py
--rw-r--r--  2.0 unx     9885 b- defN 24-Feb-07 17:23 inference/enterprise/stream_management/manager/app.py
--rw-r--r--  2.0 unx     2490 b- defN 24-Feb-07 17:23 inference/enterprise/stream_management/manager/communication.py
--rw-r--r--  2.0 unx      710 b- defN 24-Feb-07 17:23 inference/enterprise/stream_management/manager/entities.py
--rw-r--r--  2.0 unx      325 b- defN 24-Feb-07 17:23 inference/enterprise/stream_management/manager/errors.py
--rw-r--r--  2.0 unx    11131 b- defN 24-Feb-07 17:23 inference/enterprise/stream_management/manager/inference_pipeline_manager.py
--rw-r--r--  2.0 unx     1619 b- defN 24-Feb-07 17:23 inference/enterprise/stream_management/manager/serialisation.py
--rw-r--r--  2.0 unx      679 b- defN 24-Feb-07 17:23 inference/enterprise/stream_management/manager/tcp_server.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-07 17:23 inference/enterprise/workflows/__init__.py
--rw-r--r--  2.0 unx       93 b- defN 24-Feb-07 17:23 inference/enterprise/workflows/constants.py
--rw-r--r--  2.0 unx     1008 b- defN 24-Feb-07 17:23 inference/enterprise/workflows/errors.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-07 17:23 inference/enterprise/workflows/complier/__init__.py
--rw-r--r--  2.0 unx     3197 b- defN 24-Feb-07 17:23 inference/enterprise/workflows/complier/core.py
--rw-r--r--  2.0 unx       97 b- defN 24-Feb-07 17:23 inference/enterprise/workflows/complier/entities.py
--rw-r--r--  2.0 unx    10391 b- defN 24-Feb-07 17:23 inference/enterprise/workflows/complier/execution_engine.py
--rw-r--r--  2.0 unx     6055 b- defN 24-Feb-07 17:23 inference/enterprise/workflows/complier/flow_coordinator.py
--rw-r--r--  2.0 unx    17013 b- defN 24-Feb-07 17:23 inference/enterprise/workflows/complier/graph_parser.py
--rw-r--r--  2.0 unx     6321 b- defN 24-Feb-07 17:23 inference/enterprise/workflows/complier/runtime_input_validator.py
--rw-r--r--  2.0 unx     3240 b- defN 24-Feb-07 17:23 inference/enterprise/workflows/complier/utils.py
--rw-r--r--  2.0 unx     2945 b- defN 24-Feb-07 17:23 inference/enterprise/workflows/complier/validator.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-07 17:23 inference/enterprise/workflows/complier/steps_executors/__init__.py
--rw-r--r--  2.0 unx    31521 b- defN 24-Feb-07 17:23 inference/enterprise/workflows/complier/steps_executors/auxiliary.py
--rw-r--r--  2.0 unx      340 b- defN 24-Feb-07 17:23 inference/enterprise/workflows/complier/steps_executors/constants.py
--rw-r--r--  2.0 unx    25024 b- defN 24-Feb-07 17:23 inference/enterprise/workflows/complier/steps_executors/models.py
--rw-r--r--  2.0 unx      105 b- defN 24-Feb-07 17:23 inference/enterprise/workflows/complier/steps_executors/types.py
--rw-r--r--  2.0 unx     2600 b- defN 24-Feb-07 17:23 inference/enterprise/workflows/complier/steps_executors/utils.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-07 17:23 inference/enterprise/workflows/entities/__init__.py
--rw-r--r--  2.0 unx      124 b- defN 24-Feb-07 17:23 inference/enterprise/workflows/entities/base.py
--rw-r--r--  2.0 unx      570 b- defN 24-Feb-07 17:23 inference/enterprise/workflows/entities/inputs.py
--rw-r--r--  2.0 unx      472 b- defN 24-Feb-07 17:23 inference/enterprise/workflows/entities/outputs.py
--rw-r--r--  2.0 unx    39791 b- defN 24-Feb-07 17:23 inference/enterprise/workflows/entities/steps.py
--rw-r--r--  2.0 unx     7979 b- defN 24-Feb-07 17:23 inference/enterprise/workflows/entities/validators.py
--rw-r--r--  2.0 unx     1514 b- defN 24-Feb-07 17:23 inference/enterprise/workflows/entities/workflows_specification.py
--rw-r--r--  2.0 unx      889 b- defN 24-Feb-07 17:23 inference/models/__init__.py
--rw-r--r--  2.0 unx     1139 b- defN 24-Feb-07 17:23 inference/models/aliases.py
--rw-r--r--  2.0 unx     5784 b- defN 24-Feb-07 17:23 inference/models/utils.py
--rw-r--r--  2.0 unx       50 b- defN 24-Feb-07 17:23 inference/models/clip/__init__.py
--rw-r--r--  2.0 unx    14580 b- defN 24-Feb-07 17:23 inference/models/clip/clip_model.py
--rw-r--r--  2.0 unx       50 b- defN 24-Feb-07 17:23 inference/models/cogvlm/__init__.py
--rw-r--r--  2.0 unx     3566 b- defN 24-Feb-07 17:23 inference/models/cogvlm/cogvlm.py
--rw-r--r--  2.0 unx       53 b- defN 24-Feb-07 17:23 inference/models/doctr/__init__.py
--rw-r--r--  2.0 unx     5300 b- defN 24-Feb-07 17:23 inference/models/doctr/doctr_model.py
--rw-r--r--  2.0 unx       44 b- defN 24-Feb-07 17:23 inference/models/gaze/__init__.py
--rw-r--r--  2.0 unx    13268 b- defN 24-Feb-07 17:23 inference/models/gaze/gaze.py
--rw-r--r--  2.0 unx     2883 b- defN 24-Feb-07 17:23 inference/models/gaze/l2cs.py
--rw-r--r--  2.0 unx       73 b- defN 24-Feb-07 17:23 inference/models/grounding_dino/__init__.py
--rw-r--r--  2.0 unx     5106 b- defN 24-Feb-07 17:23 inference/models/grounding_dino/grounding_dino.py
--rw-r--r--  2.0 unx       66 b- defN 24-Feb-07 17:23 inference/models/sam/__init__.py
--rw-r--r--  2.0 unx    14060 b- defN 24-Feb-07 17:23 inference/models/sam/segment_anything.py
--rw-r--r--  2.0 unx       70 b- defN 24-Feb-07 17:23 inference/models/vit/__init__.py
--rw-r--r--  2.0 unx     1544 b- defN 24-Feb-07 17:23 inference/models/vit/vit_classification.py
--rw-r--r--  2.0 unx       72 b- defN 24-Feb-07 17:23 inference/models/yolact/__init__.py
--rw-r--r--  2.0 unx    13175 b- defN 24-Feb-07 17:23 inference/models/yolact/yolact_instance_segmentation.py
--rw-r--r--  2.0 unx       85 b- defN 24-Feb-07 17:23 inference/models/yolonas/__init__.py
--rw-r--r--  2.0 unx     1193 b- defN 24-Feb-07 17:23 inference/models/yolonas/yolonas_object_detection.py
--rw-r--r--  2.0 unx      183 b- defN 24-Feb-07 17:23 inference/models/yolov5/__init__.py
--rw-r--r--  2.0 unx     1236 b- defN 24-Feb-07 17:23 inference/models/yolov5/yolov5_instance_segmentation.py
--rw-r--r--  2.0 unx     1195 b- defN 24-Feb-07 17:23 inference/models/yolov5/yolov5_object_detection.py
--rw-r--r--  2.0 unx      101 b- defN 24-Feb-07 17:23 inference/models/yolov7/__init__.py
--rw-r--r--  2.0 unx     1101 b- defN 24-Feb-07 17:23 inference/models/yolov7/yolov7_instance_segmentation.py
--rw-r--r--  2.0 unx      350 b- defN 24-Feb-07 17:23 inference/models/yolov8/__init__.py
--rw-r--r--  2.0 unx      415 b- defN 24-Feb-07 17:23 inference/models/yolov8/yolov8_classification.py
--rw-r--r--  2.0 unx     1803 b- defN 24-Feb-07 17:23 inference/models/yolov8/yolov8_instance_segmentation.py
--rw-r--r--  2.0 unx     2275 b- defN 24-Feb-07 17:23 inference/models/yolov8/yolov8_keypoints_detection.py
--rw-r--r--  2.0 unx     1629 b- defN 24-Feb-07 17:23 inference/models/yolov8/yolov8_object_detection.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-07 17:23 inference_cli/__init__.py
--rw-r--r--  2.0 unx     2428 b- defN 24-Feb-07 17:23 inference_cli/cloud.py
--rw-r--r--  2.0 unx     2725 b- defN 24-Feb-07 17:23 inference_cli/main.py
--rw-r--r--  2.0 unx     2098 b- defN 24-Feb-07 17:23 inference_cli/server.py
--rw-r--r--  2.0 unx      305 b- defN 24-Feb-07 17:23 inference_cli/lib/__init__.py
--rw-r--r--  2.0 unx     7205 b- defN 24-Feb-07 17:23 inference_cli/lib/cloud_adapter.py
--rw-r--r--  2.0 unx     8071 b- defN 24-Feb-07 17:23 inference_cli/lib/container_adapter.py
--rw-r--r--  2.0 unx      111 b- defN 24-Feb-07 17:23 inference_cli/lib/env.py
--rw-r--r--  2.0 unx       58 b- defN 24-Feb-07 17:23 inference_cli/lib/exceptions.py
--rw-r--r--  2.0 unx    13645 b- defN 24-Feb-07 17:23 inference_cli/lib/infer_adapter.py
--rw-r--r--  2.0 unx      223 b- defN 24-Feb-07 17:23 inference_cli/lib/logger.py
--rw-r--r--  2.0 unx      954 b- defN 24-Feb-07 17:23 inference_cli/lib/utils.py
--rw-r--r--  2.0 unx      421 b- defN 24-Feb-07 17:24 inference-0.9.9.dist-info/LICENSE
--rw-r--r--  2.0 unx    10237 b- defN 24-Feb-07 17:24 inference-0.9.9.dist-info/LICENSE.core
--rw-r--r--  2.0 unx    18151 b- defN 24-Feb-07 17:24 inference-0.9.9.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Feb-07 17:24 inference-0.9.9.dist-info/WHEEL
--rw-r--r--  2.0 unx       53 b- defN 24-Feb-07 17:24 inference-0.9.9.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       24 b- defN 24-Feb-07 17:24 inference-0.9.9.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    21780 b- defN 24-Feb-07 17:24 inference-0.9.9.dist-info/RECORD
-222 files, 993632 bytes uncompressed, 246563 bytes compressed:  75.2%
+Zip file size: 281908 bytes, number of entries: 222
+-rw-r--r--  2.0 unx      209 b- defN 24-Feb-07 12:15 inference/__init__.py
+-rw-r--r--  2.0 unx     1728 b- defN 24-Feb-07 12:15 inference/core/__init__.py
+-rw-r--r--  2.0 unx      183 b- defN 24-Feb-07 12:15 inference/core/constants.py
+-rw-r--r--  2.0 unx    12459 b- defN 24-Feb-07 12:15 inference/core/env.py
+-rw-r--r--  2.0 unx     3611 b- defN 24-Feb-07 12:15 inference/core/exceptions.py
+-rw-r--r--  2.0 unx      371 b- defN 24-Feb-07 12:15 inference/core/logger.py
+-rw-r--r--  2.0 unx     6486 b- defN 24-Feb-07 12:15 inference/core/nms.py
+-rw-r--r--  2.0 unx    12130 b- defN 24-Feb-07 12:15 inference/core/roboflow_api.py
+-rw-r--r--  2.0 unx     2216 b- defN 24-Feb-07 12:15 inference/core/usage.py
+-rw-r--r--  2.0 unx       78 b- defN 24-Feb-07 12:15 inference/core/version.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Feb-07 12:15 inference/core/active_learning/__init__.py
+-rw-r--r--  2.0 unx     2933 b- defN 24-Feb-07 12:15 inference/core/active_learning/accounting.py
+-rw-r--r--  2.0 unx      986 b- defN 24-Feb-07 12:15 inference/core/active_learning/batching.py
+-rw-r--r--  2.0 unx     8948 b- defN 24-Feb-07 12:15 inference/core/active_learning/cache_operations.py
+-rw-r--r--  2.0 unx     6493 b- defN 24-Feb-07 12:15 inference/core/active_learning/configuration.py
+-rw-r--r--  2.0 unx     7126 b- defN 24-Feb-07 12:15 inference/core/active_learning/core.py
+-rw-r--r--  2.0 unx     4541 b- defN 24-Feb-07 12:15 inference/core/active_learning/entities.py
+-rw-r--r--  2.0 unx     8845 b- defN 24-Feb-07 12:15 inference/core/active_learning/middlewares.py
+-rw-r--r--  2.0 unx     4036 b- defN 24-Feb-07 12:15 inference/core/active_learning/post_processing.py
+-rw-r--r--  2.0 unx      458 b- defN 24-Feb-07 12:15 inference/core/active_learning/utils.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Feb-07 12:15 inference/core/active_learning/samplers/__init__.py
+-rw-r--r--  2.0 unx     7302 b- defN 24-Feb-07 12:15 inference/core/active_learning/samplers/close_to_threshold.py
+-rw-r--r--  2.0 unx     1725 b- defN 24-Feb-07 12:15 inference/core/active_learning/samplers/contains_classes.py
+-rw-r--r--  2.0 unx     3488 b- defN 24-Feb-07 12:15 inference/core/active_learning/samplers/number_of_detections.py
+-rw-r--r--  2.0 unx     1018 b- defN 24-Feb-07 12:15 inference/core/active_learning/samplers/random.py
+-rw-r--r--  2.0 unx      813 b- defN 24-Feb-07 12:15 inference/core/cache/__init__.py
+-rw-r--r--  2.0 unx     3443 b- defN 24-Feb-07 12:15 inference/core/cache/base.py
+-rw-r--r--  2.0 unx     5884 b- defN 24-Feb-07 12:15 inference/core/cache/memory.py
+-rw-r--r--  2.0 unx     2858 b- defN 24-Feb-07 12:15 inference/core/cache/model_artifacts.py
+-rw-r--r--  2.0 unx     6401 b- defN 24-Feb-07 12:15 inference/core/cache/redis.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Feb-07 12:15 inference/core/devices/__init__.py
+-rw-r--r--  2.0 unx     3803 b- defN 24-Feb-07 12:15 inference/core/devices/utils.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Feb-07 12:15 inference/core/entities/__init__.py
+-rw-r--r--  2.0 unx      428 b- defN 24-Feb-07 12:15 inference/core/entities/common.py
+-rw-r--r--  2.0 unx       81 b- defN 24-Feb-07 12:15 inference/core/entities/types.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Feb-07 12:15 inference/core/entities/requests/__init__.py
+-rw-r--r--  2.0 unx     3142 b- defN 24-Feb-07 12:15 inference/core/entities/requests/clip.py
+-rw-r--r--  2.0 unx     1890 b- defN 24-Feb-07 12:15 inference/core/entities/requests/cogvlm.py
+-rw-r--r--  2.0 unx     1002 b- defN 24-Feb-07 12:15 inference/core/entities/requests/doctr.py
+-rw-r--r--  2.0 unx     1918 b- defN 24-Feb-07 12:15 inference/core/entities/requests/gaze.py
+-rw-r--r--  2.0 unx      544 b- defN 24-Feb-07 12:15 inference/core/entities/requests/groundingdino.py
+-rw-r--r--  2.0 unx     9765 b- defN 24-Feb-07 12:15 inference/core/entities/requests/inference.py
+-rw-r--r--  2.0 unx     6929 b- defN 24-Feb-07 12:15 inference/core/entities/requests/sam.py
+-rw-r--r--  2.0 unx      968 b- defN 24-Feb-07 12:15 inference/core/entities/requests/server_state.py
+-rw-r--r--  2.0 unx      853 b- defN 24-Feb-07 12:15 inference/core/entities/requests/workflows.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Feb-07 12:15 inference/core/entities/responses/__init__.py
+-rw-r--r--  2.0 unx     1531 b- defN 24-Feb-07 12:15 inference/core/entities/responses/clip.py
+-rw-r--r--  2.0 unx      322 b- defN 24-Feb-07 12:15 inference/core/entities/responses/cogvlm.py
+-rw-r--r--  2.0 unx      727 b- defN 24-Feb-07 12:15 inference/core/entities/responses/doctr.py
+-rw-r--r--  2.0 unx     1303 b- defN 24-Feb-07 12:15 inference/core/entities/responses/gaze.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Feb-07 12:15 inference/core/entities/responses/groundingdino.py
+-rw-r--r--  2.0 unx    12378 b- defN 24-Feb-07 12:15 inference/core/entities/responses/inference.py
+-rw-r--r--  2.0 unx      300 b- defN 24-Feb-07 12:15 inference/core/entities/responses/notebooks.py
+-rw-r--r--  2.0 unx     2207 b- defN 24-Feb-07 12:15 inference/core/entities/responses/sam.py
+-rw-r--r--  2.0 unx     2305 b- defN 24-Feb-07 12:15 inference/core/entities/responses/server_state.py
+-rw-r--r--  2.0 unx      249 b- defN 24-Feb-07 12:15 inference/core/entities/responses/workflows.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Feb-07 12:15 inference/core/interfaces/__init__.py
+-rw-r--r--  2.0 unx      261 b- defN 24-Feb-07 12:15 inference/core/interfaces/base.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Feb-07 12:15 inference/core/interfaces/camera/__init__.py
+-rw-r--r--  2.0 unx     5517 b- defN 24-Feb-07 12:15 inference/core/interfaces/camera/camera.py
+-rw-r--r--  2.0 unx     1621 b- defN 24-Feb-07 12:15 inference/core/interfaces/camera/entities.py
+-rw-r--r--  2.0 unx      202 b- defN 24-Feb-07 12:15 inference/core/interfaces/camera/exceptions.py
+-rw-r--r--  2.0 unx     4000 b- defN 24-Feb-07 12:15 inference/core/interfaces/camera/utils.py
+-rw-r--r--  2.0 unx    41415 b- defN 24-Feb-07 12:15 inference/core/interfaces/camera/video_source.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Feb-07 12:15 inference/core/interfaces/http/__init__.py
+-rw-r--r--  2.0 unx    61261 b- defN 24-Feb-07 12:15 inference/core/interfaces/http/http_api.py
+-rw-r--r--  2.0 unx     2384 b- defN 24-Feb-07 12:15 inference/core/interfaces/http/orjson_utils.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Feb-07 12:15 inference/core/interfaces/stream/__init__.py
+-rw-r--r--  2.0 unx     3784 b- defN 24-Feb-07 12:15 inference/core/interfaces/stream/entities.py
+-rw-r--r--  2.0 unx    21169 b- defN 24-Feb-07 12:15 inference/core/interfaces/stream/inference_pipeline.py
+-rw-r--r--  2.0 unx    13697 b- defN 24-Feb-07 12:15 inference/core/interfaces/stream/sinks.py
+-rw-r--r--  2.0 unx    12281 b- defN 24-Feb-07 12:15 inference/core/interfaces/stream/stream.py
+-rw-r--r--  2.0 unx    10930 b- defN 24-Feb-07 12:15 inference/core/interfaces/stream/watchdog.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Feb-07 12:15 inference/core/interfaces/udp/__init__.py
+-rw-r--r--  2.0 unx    11027 b- defN 24-Feb-07 12:15 inference/core/interfaces/udp/udp_stream.py
+-rw-r--r--  2.0 unx        1 b- defN 24-Feb-07 12:15 inference/core/managers/__init__.py
+-rw-r--r--  2.0 unx     5907 b- defN 24-Feb-07 12:15 inference/core/managers/active_learning.py
+-rw-r--r--  2.0 unx    11690 b- defN 24-Feb-07 12:15 inference/core/managers/base.py
+-rw-r--r--  2.0 unx      242 b- defN 24-Feb-07 12:15 inference/core/managers/entities.py
+-rw-r--r--  2.0 unx     3703 b- defN 24-Feb-07 12:15 inference/core/managers/metrics.py
+-rw-r--r--  2.0 unx     5306 b- defN 24-Feb-07 12:15 inference/core/managers/pingback.py
+-rw-r--r--  2.0 unx      675 b- defN 24-Feb-07 12:15 inference/core/managers/stub_loader.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Feb-07 12:15 inference/core/managers/decorators/__init__.py
+-rw-r--r--  2.0 unx     6222 b- defN 24-Feb-07 12:15 inference/core/managers/decorators/base.py
+-rw-r--r--  2.0 unx     4286 b- defN 24-Feb-07 12:15 inference/core/managers/decorators/fixed_size_cache.py
+-rw-r--r--  2.0 unx      487 b- defN 24-Feb-07 12:15 inference/core/managers/decorators/locked_load.py
+-rw-r--r--  2.0 unx     1990 b- defN 24-Feb-07 12:15 inference/core/managers/decorators/logger.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Feb-07 12:15 inference/core/models/__init__.py
+-rw-r--r--  2.0 unx     5316 b- defN 24-Feb-07 12:15 inference/core/models/base.py
+-rw-r--r--  2.0 unx    16272 b- defN 24-Feb-07 12:15 inference/core/models/classification_base.py
+-rw-r--r--  2.0 unx    13358 b- defN 24-Feb-07 12:15 inference/core/models/instance_segmentation_base.py
+-rw-r--r--  2.0 unx     7645 b- defN 24-Feb-07 12:15 inference/core/models/keypoints_detection_base.py
+-rw-r--r--  2.0 unx    12638 b- defN 24-Feb-07 12:15 inference/core/models/object_detection_base.py
+-rw-r--r--  2.0 unx    32993 b- defN 24-Feb-07 12:15 inference/core/models/roboflow.py
+-rw-r--r--  2.0 unx     4805 b- defN 24-Feb-07 12:15 inference/core/models/stubs.py
+-rw-r--r--  2.0 unx      103 b- defN 24-Feb-07 12:15 inference/core/models/types.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Feb-07 12:15 inference/core/models/utils/__init__.py
+-rw-r--r--  2.0 unx      619 b- defN 24-Feb-07 12:15 inference/core/models/utils/batching.py
+-rw-r--r--  2.0 unx     1492 b- defN 24-Feb-07 12:15 inference/core/models/utils/keypoints.py
+-rw-r--r--  2.0 unx      173 b- defN 24-Feb-07 12:15 inference/core/models/utils/validate.py
+-rw-r--r--  2.0 unx        1 b- defN 24-Feb-07 12:15 inference/core/registries/__init__.py
+-rw-r--r--  2.0 unx     1395 b- defN 24-Feb-07 12:15 inference/core/registries/base.py
+-rw-r--r--  2.0 unx     8545 b- defN 24-Feb-07 12:15 inference/core/registries/roboflow.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Feb-07 12:15 inference/core/utils/__init__.py
+-rw-r--r--  2.0 unx     2104 b- defN 24-Feb-07 12:15 inference/core/utils/environment.py
+-rw-r--r--  2.0 unx     1908 b- defN 24-Feb-07 12:15 inference/core/utils/file_system.py
+-rw-r--r--  2.0 unx    14257 b- defN 24-Feb-07 12:15 inference/core/utils/image_utils.py
+-rw-r--r--  2.0 unx      679 b- defN 24-Feb-07 12:15 inference/core/utils/notebooks.py
+-rw-r--r--  2.0 unx      660 b- defN 24-Feb-07 12:15 inference/core/utils/onnx.py
+-rw-r--r--  2.0 unx    21533 b- defN 24-Feb-07 12:15 inference/core/utils/postprocess.py
+-rw-r--r--  2.0 unx     8381 b- defN 24-Feb-07 12:15 inference/core/utils/preprocess.py
+-rw-r--r--  2.0 unx      712 b- defN 24-Feb-07 12:15 inference/core/utils/requests.py
+-rw-r--r--  2.0 unx      419 b- defN 24-Feb-07 12:15 inference/core/utils/roboflow.py
+-rw-r--r--  2.0 unx      430 b- defN 24-Feb-07 12:15 inference/core/utils/s3.py
+-rw-r--r--  2.0 unx      244 b- defN 24-Feb-07 12:15 inference/core/utils/url_utils.py
+-rw-r--r--  2.0 unx     4444 b- defN 24-Feb-07 12:15 inference/core/utils/visualisation.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Feb-07 12:15 inference/enterprise/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Feb-07 12:15 inference/enterprise/device_manager/__init__.py
+-rw-r--r--  2.0 unx     2902 b- defN 24-Feb-07 12:15 inference/enterprise/device_manager/command_handler.py
+-rw-r--r--  2.0 unx     9478 b- defN 24-Feb-07 12:15 inference/enterprise/device_manager/container_service.py
+-rw-r--r--  2.0 unx     1825 b- defN 24-Feb-07 12:15 inference/enterprise/device_manager/device_manager.py
+-rw-r--r--  2.0 unx     1514 b- defN 24-Feb-07 12:15 inference/enterprise/device_manager/helpers.py
+-rw-r--r--  2.0 unx     5353 b- defN 24-Feb-07 12:15 inference/enterprise/device_manager/metrics_service.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Feb-07 12:15 inference/enterprise/parallel/__init__.py
+-rw-r--r--  2.0 unx       53 b- defN 24-Feb-07 12:15 inference/enterprise/parallel/celeryconfig.py
+-rw-r--r--  2.0 unx     5502 b- defN 24-Feb-07 12:15 inference/enterprise/parallel/dispatch_manager.py
+-rw-r--r--  2.0 unx      719 b- defN 24-Feb-07 12:15 inference/enterprise/parallel/entrypoint.py
+-rw-r--r--  2.0 unx     7761 b- defN 24-Feb-07 12:15 inference/enterprise/parallel/infer.py
+-rw-r--r--  2.0 unx     1157 b- defN 24-Feb-07 12:15 inference/enterprise/parallel/parallel_http_api.py
+-rw-r--r--  2.0 unx      786 b- defN 24-Feb-07 12:15 inference/enterprise/parallel/parallel_http_config.py
+-rw-r--r--  2.0 unx     4949 b- defN 24-Feb-07 12:15 inference/enterprise/parallel/tasks.py
+-rw-r--r--  2.0 unx     1784 b- defN 24-Feb-07 12:15 inference/enterprise/parallel/utils.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Feb-07 12:15 inference/enterprise/stream_management/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Feb-07 12:15 inference/enterprise/stream_management/api/__init__.py
+-rw-r--r--  2.0 unx     6192 b- defN 24-Feb-07 12:15 inference/enterprise/stream_management/api/app.py
+-rw-r--r--  2.0 unx     3843 b- defN 24-Feb-07 12:15 inference/enterprise/stream_management/api/entities.py
+-rw-r--r--  2.0 unx      512 b- defN 24-Feb-07 12:15 inference/enterprise/stream_management/api/errors.py
+-rw-r--r--  2.0 unx     9550 b- defN 24-Feb-07 12:15 inference/enterprise/stream_management/api/stream_manager_client.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Feb-07 12:15 inference/enterprise/stream_management/manager/__init__.py
+-rw-r--r--  2.0 unx     9885 b- defN 24-Feb-07 12:15 inference/enterprise/stream_management/manager/app.py
+-rw-r--r--  2.0 unx     2490 b- defN 24-Feb-07 12:15 inference/enterprise/stream_management/manager/communication.py
+-rw-r--r--  2.0 unx      710 b- defN 24-Feb-07 12:15 inference/enterprise/stream_management/manager/entities.py
+-rw-r--r--  2.0 unx      325 b- defN 24-Feb-07 12:15 inference/enterprise/stream_management/manager/errors.py
+-rw-r--r--  2.0 unx    11131 b- defN 24-Feb-07 12:15 inference/enterprise/stream_management/manager/inference_pipeline_manager.py
+-rw-r--r--  2.0 unx     1619 b- defN 24-Feb-07 12:15 inference/enterprise/stream_management/manager/serialisation.py
+-rw-r--r--  2.0 unx      679 b- defN 24-Feb-07 12:15 inference/enterprise/stream_management/manager/tcp_server.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Feb-07 12:15 inference/enterprise/workflows/__init__.py
+-rw-r--r--  2.0 unx       93 b- defN 24-Feb-07 12:15 inference/enterprise/workflows/constants.py
+-rw-r--r--  2.0 unx     1008 b- defN 24-Feb-07 12:15 inference/enterprise/workflows/errors.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Feb-07 12:15 inference/enterprise/workflows/complier/__init__.py
+-rw-r--r--  2.0 unx     3197 b- defN 24-Feb-07 12:15 inference/enterprise/workflows/complier/core.py
+-rw-r--r--  2.0 unx       97 b- defN 24-Feb-07 12:15 inference/enterprise/workflows/complier/entities.py
+-rw-r--r--  2.0 unx    10391 b- defN 24-Feb-07 12:15 inference/enterprise/workflows/complier/execution_engine.py
+-rw-r--r--  2.0 unx     6055 b- defN 24-Feb-07 12:15 inference/enterprise/workflows/complier/flow_coordinator.py
+-rw-r--r--  2.0 unx    17013 b- defN 24-Feb-07 12:15 inference/enterprise/workflows/complier/graph_parser.py
+-rw-r--r--  2.0 unx     6321 b- defN 24-Feb-07 12:15 inference/enterprise/workflows/complier/runtime_input_validator.py
+-rw-r--r--  2.0 unx     3240 b- defN 24-Feb-07 12:15 inference/enterprise/workflows/complier/utils.py
+-rw-r--r--  2.0 unx     2945 b- defN 24-Feb-07 12:15 inference/enterprise/workflows/complier/validator.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Feb-07 12:15 inference/enterprise/workflows/complier/steps_executors/__init__.py
+-rw-r--r--  2.0 unx    31521 b- defN 24-Feb-07 12:15 inference/enterprise/workflows/complier/steps_executors/auxiliary.py
+-rw-r--r--  2.0 unx      340 b- defN 24-Feb-07 12:15 inference/enterprise/workflows/complier/steps_executors/constants.py
+-rw-r--r--  2.0 unx    25024 b- defN 24-Feb-07 12:15 inference/enterprise/workflows/complier/steps_executors/models.py
+-rw-r--r--  2.0 unx      105 b- defN 24-Feb-07 12:15 inference/enterprise/workflows/complier/steps_executors/types.py
+-rw-r--r--  2.0 unx     2600 b- defN 24-Feb-07 12:15 inference/enterprise/workflows/complier/steps_executors/utils.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Feb-07 12:15 inference/enterprise/workflows/entities/__init__.py
+-rw-r--r--  2.0 unx      124 b- defN 24-Feb-07 12:15 inference/enterprise/workflows/entities/base.py
+-rw-r--r--  2.0 unx      570 b- defN 24-Feb-07 12:15 inference/enterprise/workflows/entities/inputs.py
+-rw-r--r--  2.0 unx      472 b- defN 24-Feb-07 12:15 inference/enterprise/workflows/entities/outputs.py
+-rw-r--r--  2.0 unx    39791 b- defN 24-Feb-07 12:15 inference/enterprise/workflows/entities/steps.py
+-rw-r--r--  2.0 unx     7979 b- defN 24-Feb-07 12:15 inference/enterprise/workflows/entities/validators.py
+-rw-r--r--  2.0 unx     1514 b- defN 24-Feb-07 12:15 inference/enterprise/workflows/entities/workflows_specification.py
+-rw-r--r--  2.0 unx      889 b- defN 24-Feb-07 12:15 inference/models/__init__.py
+-rw-r--r--  2.0 unx     1139 b- defN 24-Feb-07 12:15 inference/models/aliases.py
+-rw-r--r--  2.0 unx     5784 b- defN 24-Feb-07 12:15 inference/models/utils.py
+-rw-r--r--  2.0 unx       50 b- defN 24-Feb-07 12:15 inference/models/clip/__init__.py
+-rw-r--r--  2.0 unx    14580 b- defN 24-Feb-07 12:15 inference/models/clip/clip_model.py
+-rw-r--r--  2.0 unx       50 b- defN 24-Feb-07 12:15 inference/models/cogvlm/__init__.py
+-rw-r--r--  2.0 unx     3566 b- defN 24-Feb-07 12:15 inference/models/cogvlm/cogvlm.py
+-rw-r--r--  2.0 unx       53 b- defN 24-Feb-07 12:15 inference/models/doctr/__init__.py
+-rw-r--r--  2.0 unx     5300 b- defN 24-Feb-07 12:15 inference/models/doctr/doctr_model.py
+-rw-r--r--  2.0 unx       44 b- defN 24-Feb-07 12:15 inference/models/gaze/__init__.py
+-rw-r--r--  2.0 unx    13268 b- defN 24-Feb-07 12:15 inference/models/gaze/gaze.py
+-rw-r--r--  2.0 unx     2883 b- defN 24-Feb-07 12:15 inference/models/gaze/l2cs.py
+-rw-r--r--  2.0 unx       73 b- defN 24-Feb-07 12:15 inference/models/grounding_dino/__init__.py
+-rw-r--r--  2.0 unx     5106 b- defN 24-Feb-07 12:15 inference/models/grounding_dino/grounding_dino.py
+-rw-r--r--  2.0 unx       66 b- defN 24-Feb-07 12:15 inference/models/sam/__init__.py
+-rw-r--r--  2.0 unx    14060 b- defN 24-Feb-07 12:15 inference/models/sam/segment_anything.py
+-rw-r--r--  2.0 unx       70 b- defN 24-Feb-07 12:15 inference/models/vit/__init__.py
+-rw-r--r--  2.0 unx     1544 b- defN 24-Feb-07 12:15 inference/models/vit/vit_classification.py
+-rw-r--r--  2.0 unx       72 b- defN 24-Feb-07 12:15 inference/models/yolact/__init__.py
+-rw-r--r--  2.0 unx    13175 b- defN 24-Feb-07 12:15 inference/models/yolact/yolact_instance_segmentation.py
+-rw-r--r--  2.0 unx       85 b- defN 24-Feb-07 12:15 inference/models/yolonas/__init__.py
+-rw-r--r--  2.0 unx     1193 b- defN 24-Feb-07 12:15 inference/models/yolonas/yolonas_object_detection.py
+-rw-r--r--  2.0 unx      183 b- defN 24-Feb-07 12:15 inference/models/yolov5/__init__.py
+-rw-r--r--  2.0 unx     1236 b- defN 24-Feb-07 12:15 inference/models/yolov5/yolov5_instance_segmentation.py
+-rw-r--r--  2.0 unx     1195 b- defN 24-Feb-07 12:15 inference/models/yolov5/yolov5_object_detection.py
+-rw-r--r--  2.0 unx      101 b- defN 24-Feb-07 12:15 inference/models/yolov7/__init__.py
+-rw-r--r--  2.0 unx     1101 b- defN 24-Feb-07 12:15 inference/models/yolov7/yolov7_instance_segmentation.py
+-rw-r--r--  2.0 unx      350 b- defN 24-Feb-07 12:15 inference/models/yolov8/__init__.py
+-rw-r--r--  2.0 unx      415 b- defN 24-Feb-07 12:15 inference/models/yolov8/yolov8_classification.py
+-rw-r--r--  2.0 unx     1803 b- defN 24-Feb-07 12:15 inference/models/yolov8/yolov8_instance_segmentation.py
+-rw-r--r--  2.0 unx     2275 b- defN 24-Feb-07 12:15 inference/models/yolov8/yolov8_keypoints_detection.py
+-rw-r--r--  2.0 unx     1629 b- defN 24-Feb-07 12:15 inference/models/yolov8/yolov8_object_detection.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Feb-07 12:15 inference_cli/__init__.py
+-rw-r--r--  2.0 unx     2428 b- defN 24-Feb-07 12:15 inference_cli/cloud.py
+-rw-r--r--  2.0 unx     2725 b- defN 24-Feb-07 12:15 inference_cli/main.py
+-rw-r--r--  2.0 unx     2098 b- defN 24-Feb-07 12:15 inference_cli/server.py
+-rw-r--r--  2.0 unx      305 b- defN 24-Feb-07 12:15 inference_cli/lib/__init__.py
+-rw-r--r--  2.0 unx     7205 b- defN 24-Feb-07 12:15 inference_cli/lib/cloud_adapter.py
+-rw-r--r--  2.0 unx     8071 b- defN 24-Feb-07 12:15 inference_cli/lib/container_adapter.py
+-rw-r--r--  2.0 unx      111 b- defN 24-Feb-07 12:15 inference_cli/lib/env.py
+-rw-r--r--  2.0 unx       58 b- defN 24-Feb-07 12:15 inference_cli/lib/exceptions.py
+-rw-r--r--  2.0 unx    13645 b- defN 24-Feb-07 12:15 inference_cli/lib/infer_adapter.py
+-rw-r--r--  2.0 unx      223 b- defN 24-Feb-07 12:15 inference_cli/lib/logger.py
+-rw-r--r--  2.0 unx      954 b- defN 24-Feb-07 12:15 inference_cli/lib/utils.py
+-rw-r--r--  2.0 unx      421 b- defN 24-Feb-07 12:16 inference-0.9.9rc23.dist-info/LICENSE
+-rw-r--r--  2.0 unx    10237 b- defN 24-Feb-07 12:16 inference-0.9.9rc23.dist-info/LICENSE.core
+-rw-r--r--  2.0 unx    17292 b- defN 24-Feb-07 12:16 inference-0.9.9rc23.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Feb-07 12:16 inference-0.9.9rc23.dist-info/WHEEL
+-rw-r--r--  2.0 unx       53 b- defN 24-Feb-07 12:16 inference-0.9.9rc23.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       24 b- defN 24-Feb-07 12:16 inference-0.9.9rc23.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    21808 b- defN 24-Feb-07 12:16 inference-0.9.9rc23.dist-info/RECORD
+222 files, 992805 bytes uncompressed, 246314 bytes compressed:  75.2%
```

## zipnote {}

```diff
@@ -639,29 +639,29 @@
 
 Filename: inference_cli/lib/logger.py
 Comment: 
 
 Filename: inference_cli/lib/utils.py
 Comment: 
 
-Filename: inference-0.9.9.dist-info/LICENSE
+Filename: inference-0.9.9rc23.dist-info/LICENSE
 Comment: 
 
-Filename: inference-0.9.9.dist-info/LICENSE.core
+Filename: inference-0.9.9rc23.dist-info/LICENSE.core
 Comment: 
 
-Filename: inference-0.9.9.dist-info/METADATA
+Filename: inference-0.9.9rc23.dist-info/METADATA
 Comment: 
 
-Filename: inference-0.9.9.dist-info/WHEEL
+Filename: inference-0.9.9rc23.dist-info/WHEEL
 Comment: 
 
-Filename: inference-0.9.9.dist-info/entry_points.txt
+Filename: inference-0.9.9rc23.dist-info/entry_points.txt
 Comment: 
 
-Filename: inference-0.9.9.dist-info/top_level.txt
+Filename: inference-0.9.9rc23.dist-info/top_level.txt
 Comment: 
 
-Filename: inference-0.9.9.dist-info/RECORD
+Filename: inference-0.9.9rc23.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## inference/core/version.py

```diff
@@ -1,5 +1,5 @@
-__version__ = "0.9.9"
+__version__ = "0.9.9rc23"
 
 
 if __name__ == "__main__":
     print(__version__)
```

## Comparing `inference-0.9.9.dist-info/LICENSE.core` & `inference-0.9.9rc23.dist-info/LICENSE.core`

 * *Files identical despite different names*

## Comparing `inference-0.9.9.dist-info/METADATA` & `inference-0.9.9rc23.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,46 +1,21 @@
 Metadata-Version: 2.1
 Name: inference
-Version: 0.9.9
+Version: 0.9.9rc23
 Summary: With no prior knowledge of machine learning or device-specific deployment, you can deploy a computer vision model to a range of devices and environments using Roboflow Inference.
 Home-page: https://github.com/roboflow/inference
 Author: Roboflow
 Author-email: help@roboflow.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: LICENSE.core
-Requires-Dist: APScheduler <=3.10.1
-Requires-Dist: cython <=3.0.0
-Requires-Dist: python-dotenv <=2.0.0
-Requires-Dist: fastapi <1.0,>=0.100
-Requires-Dist: numpy <=1.25.2
-Requires-Dist: opencv-python <=4.8.0.76
-Requires-Dist: piexif <=1.1.3
-Requires-Dist: pillow <11.0
-Requires-Dist: prometheus-fastapi-instrumentator <=6.0.0
-Requires-Dist: redis <6.0.0
-Requires-Dist: requests >=2.26.0
-Requires-Dist: rich <=13.5.2
-Requires-Dist: shapely <=2.0.1
-Requires-Dist: supervision <1.0.0,>0.16.0
-Requires-Dist: pybase64 <2.0.0
-Requires-Dist: scikit-image >=0.19.0
-Requires-Dist: requests-toolbelt >=1.0.0
-Requires-Dist: wheel >=0.38.1
-Requires-Dist: setuptools >=65.5.1
-Requires-Dist: pytest-asyncio <=0.21.1
-Requires-Dist: networkx >=3.1
-Requires-Dist: pydantic >=2.0
-Requires-Dist: onnxruntime <=1.15.1
-Requires-Dist: GPUtil ==1.4.0
-Requires-Dist: inference-cli ==0.9.9
 Provides-Extra: clip
 Requires-Dist: rf-clip ==1.0 ; extra == 'clip'
 Provides-Extra: gaze
 Requires-Dist: mediapipe <0.11,>=0.9 ; extra == 'gaze'
 Provides-Extra: hosted
 Requires-Dist: boto3 <=1.28.23 ; extra == 'hosted'
 Requires-Dist: pymemcache <=4.0.0 ; extra == 'hosted'
```

## Comparing `inference-0.9.9.dist-info/RECORD` & `inference-0.9.9rc23.dist-info/RECORD`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 inference/core/constants.py,sha256=vArFjw8mR6utyw8JRz5P9HB1RRXeqO2QlFtGvdoKO6o,183
 inference/core/env.py,sha256=1g4TmZzsW2DxlzMGJPUWvGTeXpfda2LkdJJymDYAU1I,12459
 inference/core/exceptions.py,sha256=OsoiZhGJAvexbMs2g50w9Eqiapoirhu_7REWP68R7vI,3611
 inference/core/logger.py,sha256=ATNT62Gf4vNB1nSsNYDjp71Vl7NUQzXcvmT-8tZWvGg,371
 inference/core/nms.py,sha256=Nmo43rr3m2kuK5puPXtD79-P5vIj1lAkg_sPu7cLPig,6486
 inference/core/roboflow_api.py,sha256=pjPgS5uMohePeD2hNhhe-OtDeLlgfN7ocON1842sXVg,12130
 inference/core/usage.py,sha256=9Km5cGfzkIAmVlzcAQY-RXByi1QZ7_G49uKv6KqrLOA,2216
-inference/core/version.py,sha256=bqUGdqbZS37wg-igCRU6VQhbPjYgtBWzt4SXBpuuDjw,74
+inference/core/version.py,sha256=aeCX65wj2wOyKA6nK9QbNhIR-u4qs7jnQQgNh083cPg,78
 inference/core/active_learning/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 inference/core/active_learning/accounting.py,sha256=i6vqs41UQbsyt4wyts1TcdyMEOWk4BBIhxSMK5Lk80w,2933
 inference/core/active_learning/batching.py,sha256=DaMrZU68V3xVfrrLfYgQEYTpqCtsjvToadb2a_CTQ8Q,986
 inference/core/active_learning/cache_operations.py,sha256=AP-fqzVQd_6y_XLrlDIG-uW6wbOlD2tRIWXNPLjldR8,8948
 inference/core/active_learning/configuration.py,sha256=Hmc6MlK0mUMsAQ_EyoYEVp5COKqRu54e3Gj-9qHIgTo,6493
 inference/core/active_learning/core.py,sha256=UJHenmGraJtxHGZPluNV4Vvsw7ZfBlkNaoUYhDSqCMQ,7126
 inference/core/active_learning/entities.py,sha256=DRPsVscTwbnHUfe7ZNyNbWWiE4idMZgtWpFRF36JBjc,4541
@@ -209,14 +209,14 @@
 inference_cli/lib/cloud_adapter.py,sha256=uMI9iF6HcBZb6e0HUzL99uXPxkyynnlPVyiHJKBk3zI,7205
 inference_cli/lib/container_adapter.py,sha256=sGCdNO1CsmSH6WdrmPtmyhvgIzhn6kKuKohumcMC3cA,8071
 inference_cli/lib/env.py,sha256=Q0unXcIInG-es1xrcYwSecBMfC6v3iBUXsWf4Ph5duM,111
 inference_cli/lib/exceptions.py,sha256=QG9LbV_WNlrdX22FVQWVgDeiKwIH2oZuA95Cetibg_A,58
 inference_cli/lib/infer_adapter.py,sha256=DY9mATO_y0gYiLcQjB0jfH6cZbWTJp1OG_vzggjY2fk,13645
 inference_cli/lib/logger.py,sha256=-iEOIxVEysU8qDPOluh_k6We4RGP8k7LYTjPFusMiCc,223
 inference_cli/lib/utils.py,sha256=ru_bGs_xgqsW7fknu_jkzQEbr6jb7V_PCAylaej4yeA,954
-inference-0.9.9.dist-info/LICENSE,sha256=6_siNlKng4EAb5WZXZuD9cKF38PWick7dL42U_h1KIE,421
-inference-0.9.9.dist-info/LICENSE.core,sha256=Ioa7wFnewa3uNb527FeTbJztwGh5UsYJ9aNnfqyfDLs,10237
-inference-0.9.9.dist-info/METADATA,sha256=JOdCFsxb_nvfRVA2uQFek93ndORtNpVz5dKwLbJ9VXM,18151
-inference-0.9.9.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-inference-0.9.9.dist-info/entry_points.txt,sha256=Dm0LrFRve6WvcWk8HRaftIFO8t6vYYmK4AOPHKxE0Ow,53
-inference-0.9.9.dist-info/top_level.txt,sha256=D3WONB8QzL2SAlaDLnKfMY695oOJ30WxYQ4oFngpvIw,24
-inference-0.9.9.dist-info/RECORD,,
+inference-0.9.9rc23.dist-info/LICENSE,sha256=6_siNlKng4EAb5WZXZuD9cKF38PWick7dL42U_h1KIE,421
+inference-0.9.9rc23.dist-info/LICENSE.core,sha256=Ioa7wFnewa3uNb527FeTbJztwGh5UsYJ9aNnfqyfDLs,10237
+inference-0.9.9rc23.dist-info/METADATA,sha256=758LzJ3OCYX8FCjE2IBHUTXDY1iwPW61GwhxyoWhbuU,17292
+inference-0.9.9rc23.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+inference-0.9.9rc23.dist-info/entry_points.txt,sha256=Dm0LrFRve6WvcWk8HRaftIFO8t6vYYmK4AOPHKxE0Ow,53
+inference-0.9.9rc23.dist-info/top_level.txt,sha256=D3WONB8QzL2SAlaDLnKfMY695oOJ30WxYQ4oFngpvIw,24
+inference-0.9.9rc23.dist-info/RECORD,,
```

