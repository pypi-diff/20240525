# Comparing `tmp/inference_gpu-0.9.9-py3-none-any.whl.zip` & `tmp/inference_gpu-0.9.9rc23-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,224 +1,296 @@
-Zip file size: 282153 bytes, number of entries: 222
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
--rw-r--r--  2.0 unx      421 b- defN 24-Feb-07 17:24 inference_gpu-0.9.9.dist-info/LICENSE
--rw-r--r--  2.0 unx    10237 b- defN 24-Feb-07 17:24 inference_gpu-0.9.9.dist-info/LICENSE.core
--rw-r--r--  2.0 unx    18129 b- defN 24-Feb-07 17:24 inference_gpu-0.9.9.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Feb-07 17:24 inference_gpu-0.9.9.dist-info/WHEEL
--rw-r--r--  2.0 unx       53 b- defN 24-Feb-07 17:24 inference_gpu-0.9.9.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       24 b- defN 24-Feb-07 17:24 inference_gpu-0.9.9.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    21808 b- defN 24-Feb-07 17:24 inference_gpu-0.9.9.dist-info/RECORD
-222 files, 993638 bytes uncompressed, 246559 bytes compressed:  75.2%
+Zip file size: 357002 bytes, number of entries: 294
+-rw-r--r--  2.0 unx        0 b- defN 23-Oct-06 15:29 cli/inference_cli/__init__.py
+-rw-r--r--  2.0 unx     1198 b- defN 23-Oct-06 15:29 cli/inference_cli/main.py
+-rw-r--r--  2.0 unx     1022 b- defN 23-Oct-06 15:29 cli/inference_cli/server.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Dec-01 20:12 development/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Dec-01 20:12 development/stream_interface/__init__.py
+-rw-r--r--  2.0 unx     3594 b- defN 23-Dec-01 20:12 development/stream_interface/camera_demo.py
+-rw-r--r--  2.0 unx     1444 b- defN 23-Dec-01 20:12 development/stream_interface/camera_test.py
+-rw-r--r--  2.0 unx     2475 b- defN 23-Dec-01 20:12 development/stream_interface/create_dummy_streams.py
+-rw-r--r--  2.0 unx     4827 b- defN 23-Dec-01 20:12 development/stream_interface/inference_pipeline_demo.py
+-rw-r--r--  2.0 unx      790 b- defN 23-Dec-01 20:12 development/stream_interface/multiplexer.py
+-rw-r--r--  2.0 unx     4433 b- defN 23-Dec-01 20:12 development/stream_interface/multiplexer_demo.py
+-rw-r--r--  2.0 unx     2934 b- defN 23-Dec-01 20:12 development/stream_interface/old_camera_demo.py
+-rw-r--r--  2.0 unx     2314 b- defN 23-Dec-01 20:12 development/stream_interface/old_inference_pipeline_demo.py
+-rw-r--r--  2.0 unx      579 b- defN 23-Dec-14 20:38 development/stream_interface/udp_receiver.py
+-rw-r--r--  2.0 unx      209 b- defN 23-Dec-29 18:16 inference/__init__.py
+-rw-r--r--  2.0 unx     1728 b- defN 23-Dec-01 20:12 inference/core/__init__.py
+-rw-r--r--  2.0 unx      183 b- defN 23-Dec-14 20:38 inference/core/constants.py
+-rw-r--r--  2.0 unx    34827 b- defN 23-Oct-12 18:46 inference/core/data_models.py
+-rw-r--r--  2.0 unx    12459 b- defN 24-Feb-07 14:49 inference/core/env.py
+-rw-r--r--  2.0 unx     3611 b- defN 24-Feb-01 14:55 inference/core/exceptions.py
+-rw-r--r--  2.0 unx      371 b- defN 24-Jan-08 15:24 inference/core/logger.py
+-rw-r--r--  2.0 unx     6486 b- defN 24-Jan-08 15:24 inference/core/nms.py
+-rw-r--r--  2.0 unx    12130 b- defN 24-Feb-07 14:49 inference/core/roboflow_api.py
+-rw-r--r--  2.0 unx     2216 b- defN 23-Oct-20 14:44 inference/core/usage.py
+-rw-r--r--  2.0 unx       78 b- defN 24-Feb-07 14:49 inference/core/version.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Dec-01 20:12 inference/core/active_learning/__init__.py
+-rw-r--r--  2.0 unx     2933 b- defN 24-Jan-08 15:24 inference/core/active_learning/accounting.py
+-rw-r--r--  2.0 unx      986 b- defN 23-Dec-01 20:12 inference/core/active_learning/batching.py
+-rw-r--r--  2.0 unx     8948 b- defN 23-Dec-29 15:15 inference/core/active_learning/cache_operations.py
+-rw-r--r--  2.0 unx     6493 b- defN 23-Dec-29 15:15 inference/core/active_learning/configuration.py
+-rw-r--r--  2.0 unx     7126 b- defN 23-Dec-29 15:15 inference/core/active_learning/core.py
+-rw-r--r--  2.0 unx     4541 b- defN 23-Dec-01 20:12 inference/core/active_learning/entities.py
+-rw-r--r--  2.0 unx     8845 b- defN 23-Dec-29 15:15 inference/core/active_learning/middlewares.py
+-rw-r--r--  2.0 unx     4036 b- defN 24-Feb-02 15:37 inference/core/active_learning/post_processing.py
+-rw-r--r--  2.0 unx      458 b- defN 23-Dec-01 20:12 inference/core/active_learning/utils.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Dec-01 20:12 inference/core/active_learning/samplers/__init__.py
+-rw-r--r--  2.0 unx     7302 b- defN 23-Dec-29 15:15 inference/core/active_learning/samplers/close_to_threshold.py
+-rw-r--r--  2.0 unx     1725 b- defN 23-Dec-01 20:12 inference/core/active_learning/samplers/contains_classes.py
+-rw-r--r--  2.0 unx     3488 b- defN 23-Dec-01 20:12 inference/core/active_learning/samplers/number_of_detections.py
+-rw-r--r--  2.0 unx     1018 b- defN 23-Dec-01 20:12 inference/core/active_learning/samplers/random.py
+-rw-r--r--  2.0 unx      813 b- defN 24-Jan-08 15:24 inference/core/cache/__init__.py
+-rw-r--r--  2.0 unx     3443 b- defN 24-Jan-08 15:24 inference/core/cache/base.py
+-rw-r--r--  2.0 unx     5884 b- defN 23-Dec-06 20:33 inference/core/cache/memory.py
+-rw-r--r--  2.0 unx     2858 b- defN 23-Dec-01 20:12 inference/core/cache/model_artifacts.py
+-rw-r--r--  2.0 unx     6401 b- defN 24-Feb-07 14:49 inference/core/cache/redis.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-15 19:04 inference/core/devices/__init__.py
+-rw-r--r--  2.0 unx     3803 b- defN 23-Oct-20 14:44 inference/core/devices/utils.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Dec-01 20:12 inference/core/entities/__init__.py
+-rw-r--r--  2.0 unx      428 b- defN 23-Dec-01 20:12 inference/core/entities/common.py
+-rw-r--r--  2.0 unx       81 b- defN 23-Dec-01 20:12 inference/core/entities/types.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Dec-01 20:12 inference/core/entities/requests/__init__.py
+-rw-r--r--  2.0 unx     3142 b- defN 24-Feb-07 14:49 inference/core/entities/requests/clip.py
+-rw-r--r--  2.0 unx     1890 b- defN 24-Feb-07 14:49 inference/core/entities/requests/cogvlm.py
+-rw-r--r--  2.0 unx     1002 b- defN 24-Feb-07 14:49 inference/core/entities/requests/doctr.py
+-rw-r--r--  2.0 unx     1918 b- defN 24-Feb-07 14:49 inference/core/entities/requests/gaze.py
+-rw-r--r--  2.0 unx      544 b- defN 24-Feb-07 14:49 inference/core/entities/requests/groundingdino.py
+-rw-r--r--  2.0 unx     9765 b- defN 24-Feb-07 14:49 inference/core/entities/requests/inference.py
+-rw-r--r--  2.0 unx     6929 b- defN 24-Feb-07 14:49 inference/core/entities/requests/sam.py
+-rw-r--r--  2.0 unx      968 b- defN 24-Feb-07 14:49 inference/core/entities/requests/server_state.py
+-rw-r--r--  2.0 unx      853 b- defN 24-Feb-02 15:37 inference/core/entities/requests/workflows.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Dec-01 20:12 inference/core/entities/responses/__init__.py
+-rw-r--r--  2.0 unx     1531 b- defN 24-Feb-07 14:49 inference/core/entities/responses/clip.py
+-rw-r--r--  2.0 unx      322 b- defN 24-Feb-07 14:49 inference/core/entities/responses/cogvlm.py
+-rw-r--r--  2.0 unx      727 b- defN 24-Jan-17 15:40 inference/core/entities/responses/doctr.py
+-rw-r--r--  2.0 unx     1303 b- defN 24-Feb-07 14:49 inference/core/entities/responses/gaze.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Dec-29 15:15 inference/core/entities/responses/groundingdino.py
+-rw-r--r--  2.0 unx    12378 b- defN 24-Feb-07 14:49 inference/core/entities/responses/inference.py
+-rw-r--r--  2.0 unx      300 b- defN 23-Dec-29 18:16 inference/core/entities/responses/notebooks.py
+-rw-r--r--  2.0 unx     2207 b- defN 24-Feb-07 14:49 inference/core/entities/responses/sam.py
+-rw-r--r--  2.0 unx     2305 b- defN 24-Feb-07 14:49 inference/core/entities/responses/server_state.py
+-rw-r--r--  2.0 unx      249 b- defN 24-Feb-02 15:37 inference/core/entities/responses/workflows.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-15 19:04 inference/core/interfaces/__init__.py
+-rw-r--r--  2.0 unx      261 b- defN 23-Aug-15 19:04 inference/core/interfaces/base.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-15 19:04 inference/core/interfaces/camera/__init__.py
+-rw-r--r--  2.0 unx     5517 b- defN 23-Dec-01 20:12 inference/core/interfaces/camera/camera.py
+-rw-r--r--  2.0 unx     1621 b- defN 24-Jan-08 15:24 inference/core/interfaces/camera/entities.py
+-rw-r--r--  2.0 unx      202 b- defN 23-Dec-01 20:12 inference/core/interfaces/camera/exceptions.py
+-rw-r--r--  2.0 unx     4000 b- defN 24-Feb-02 15:37 inference/core/interfaces/camera/utils.py
+-rw-r--r--  2.0 unx    41415 b- defN 24-Feb-02 15:37 inference/core/interfaces/camera/video_source.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-15 19:04 inference/core/interfaces/http/__init__.py
+-rw-r--r--  2.0 unx    61261 b- defN 24-Feb-02 15:37 inference/core/interfaces/http/http_api.py
+-rw-r--r--  2.0 unx     2384 b- defN 24-Feb-02 15:37 inference/core/interfaces/http/orjson_utils.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Oct-20 14:44 inference/core/interfaces/stream/__init__.py
+-rw-r--r--  2.0 unx     3784 b- defN 23-Dec-01 20:12 inference/core/interfaces/stream/entities.py
+-rw-r--r--  2.0 unx    21169 b- defN 24-Feb-02 15:37 inference/core/interfaces/stream/inference_pipeline.py
+-rw-r--r--  2.0 unx    13697 b- defN 24-Feb-02 15:37 inference/core/interfaces/stream/sinks.py
+-rw-r--r--  2.0 unx    12281 b- defN 23-Dec-29 15:15 inference/core/interfaces/stream/stream.py
+-rw-r--r--  2.0 unx    10930 b- defN 23-Dec-01 20:12 inference/core/interfaces/stream/watchdog.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-16 12:32 inference/core/interfaces/udp/__init__.py
+-rw-r--r--  2.0 unx    11027 b- defN 23-Dec-29 15:15 inference/core/interfaces/udp/udp_stream.py
+-rw-r--r--  2.0 unx        1 b- defN 23-Aug-15 19:04 inference/core/managers/__init__.py
+-rw-r--r--  2.0 unx     5907 b- defN 24-Jan-08 15:24 inference/core/managers/active_learning.py
+-rw-r--r--  2.0 unx    11690 b- defN 24-Jan-17 15:40 inference/core/managers/base.py
+-rw-r--r--  2.0 unx      242 b- defN 23-Oct-20 14:44 inference/core/managers/entities.py
+-rw-r--r--  2.0 unx     3703 b- defN 24-Feb-07 14:49 inference/core/managers/metrics.py
+-rw-r--r--  2.0 unx     5306 b- defN 24-Feb-07 14:49 inference/core/managers/pingback.py
+-rw-r--r--  2.0 unx      675 b- defN 23-Dec-01 20:12 inference/core/managers/stub_loader.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-15 19:04 inference/core/managers/decorators/__init__.py
+-rw-r--r--  2.0 unx     6222 b- defN 23-Dec-01 20:12 inference/core/managers/decorators/base.py
+-rw-r--r--  2.0 unx     4286 b- defN 23-Dec-29 15:15 inference/core/managers/decorators/fixed_size_cache.py
+-rw-r--r--  2.0 unx      487 b- defN 23-Dec-01 20:12 inference/core/managers/decorators/locked_load.py
+-rw-r--r--  2.0 unx     1990 b- defN 23-Dec-01 20:12 inference/core/managers/decorators/logger.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-15 19:04 inference/core/models/__init__.py
+-rw-r--r--  2.0 unx     5316 b- defN 23-Dec-14 20:38 inference/core/models/base.py
+-rw-r--r--  2.0 unx    16272 b- defN 23-Dec-14 20:38 inference/core/models/classification_base.py
+-rw-r--r--  2.0 unx    13358 b- defN 24-Jan-23 15:04 inference/core/models/instance_segmentation_base.py
+-rw-r--r--  2.0 unx     7645 b- defN 24-Feb-01 14:55 inference/core/models/keypoints_detection_base.py
+-rw-r--r--  2.0 unx     4786 b- defN 23-Aug-31 21:11 inference/core/models/mixins.py
+-rw-r--r--  2.0 unx    12638 b- defN 24-Feb-07 14:49 inference/core/models/object_detection_base.py
+-rw-r--r--  2.0 unx    32993 b- defN 24-Feb-07 14:49 inference/core/models/roboflow.py
+-rw-r--r--  2.0 unx     4805 b- defN 23-Dec-14 20:38 inference/core/models/stubs.py
+-rw-r--r--  2.0 unx      103 b- defN 23-Oct-20 14:44 inference/core/models/types.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Dec-19 16:15 inference/core/models/utils/__init__.py
+-rw-r--r--  2.0 unx      619 b- defN 23-Dec-29 15:15 inference/core/models/utils/batching.py
+-rw-r--r--  2.0 unx     1492 b- defN 24-Feb-01 14:55 inference/core/models/utils/keypoints.py
+-rw-r--r--  2.0 unx      173 b- defN 23-Dec-14 20:38 inference/core/models/utils/validate.py
+-rw-r--r--  2.0 unx        1 b- defN 23-Aug-15 19:04 inference/core/registries/__init__.py
+-rw-r--r--  2.0 unx     1395 b- defN 23-Dec-01 20:12 inference/core/registries/base.py
+-rw-r--r--  2.0 unx     8545 b- defN 24-Jan-08 15:24 inference/core/registries/roboflow.py
+-rw-r--r--  2.0 unx        1 b- defN 23-Aug-15 19:04 inference/core/registries/decorators/__init__.py
+-rw-r--r--  2.0 unx     1347 b- defN 23-Aug-15 19:04 inference/core/registries/decorators/base.py
+-rw-r--r--  2.0 unx     2462 b- defN 23-Aug-15 19:04 inference/core/registries/decorators/fixed_device_id.py
+-rw-r--r--  2.0 unx     2250 b- defN 23-Aug-15 19:04 inference/core/registries/decorators/trt_device_id.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-15 19:04 inference/core/utils/__init__.py
+-rw-r--r--  2.0 unx     2104 b- defN 23-Dec-01 20:12 inference/core/utils/environment.py
+-rw-r--r--  2.0 unx     1908 b- defN 23-Dec-01 20:12 inference/core/utils/file_system.py
+-rw-r--r--  2.0 unx    14257 b- defN 24-Jan-17 15:40 inference/core/utils/image_utils.py
+-rw-r--r--  2.0 unx      679 b- defN 23-Dec-29 18:16 inference/core/utils/notebooks.py
+-rw-r--r--  2.0 unx      660 b- defN 23-Dec-01 20:12 inference/core/utils/onnx.py
+-rw-r--r--  2.0 unx    21533 b- defN 23-Dec-01 20:12 inference/core/utils/postprocess.py
+-rw-r--r--  2.0 unx     8381 b- defN 23-Dec-01 20:12 inference/core/utils/preprocess.py
+-rw-r--r--  2.0 unx      712 b- defN 23-Dec-01 20:12 inference/core/utils/requests.py
+-rw-r--r--  2.0 unx      419 b- defN 23-Dec-01 20:12 inference/core/utils/roboflow.py
+-rw-r--r--  2.0 unx      430 b- defN 23-Dec-01 20:12 inference/core/utils/s3.py
+-rw-r--r--  2.0 unx      244 b- defN 23-Dec-01 20:12 inference/core/utils/url_utils.py
+-rw-r--r--  2.0 unx      142 b- defN 23-Dec-14 20:30 inference/core/utils/validate.py
+-rw-r--r--  2.0 unx     4444 b- defN 23-Dec-01 20:12 inference/core/utils/visualisation.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Jan-08 15:24 inference/enterprise/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Oct-20 14:44 inference/enterprise/device_manager/__init__.py
+-rw-r--r--  2.0 unx     2902 b- defN 23-Dec-01 20:12 inference/enterprise/device_manager/command_handler.py
+-rw-r--r--  2.0 unx     9478 b- defN 23-Oct-20 14:44 inference/enterprise/device_manager/container_service.py
+-rw-r--r--  2.0 unx     1825 b- defN 23-Oct-20 14:44 inference/enterprise/device_manager/device_manager.py
+-rw-r--r--  2.0 unx     1514 b- defN 23-Oct-20 14:44 inference/enterprise/device_manager/helpers.py
+-rw-r--r--  2.0 unx     5353 b- defN 23-Dec-01 20:12 inference/enterprise/device_manager/metrics_service.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Jan-08 15:24 inference/enterprise/parallel/__init__.py
+-rw-r--r--  2.0 unx       53 b- defN 23-Dec-01 20:12 inference/enterprise/parallel/celeryconfig.py
+-rw-r--r--  2.0 unx     5502 b- defN 24-Feb-07 14:49 inference/enterprise/parallel/dispatch_manager.py
+-rw-r--r--  2.0 unx      719 b- defN 23-Dec-14 20:38 inference/enterprise/parallel/entrypoint.py
+-rw-r--r--  2.0 unx     7761 b- defN 23-Dec-14 20:38 inference/enterprise/parallel/infer.py
+-rw-r--r--  2.0 unx     1157 b- defN 23-Dec-06 20:33 inference/enterprise/parallel/parallel_http_api.py
+-rw-r--r--  2.0 unx      786 b- defN 23-Dec-06 20:33 inference/enterprise/parallel/parallel_http_config.py
+-rw-r--r--  2.0 unx     4949 b- defN 23-Dec-14 20:38 inference/enterprise/parallel/tasks.py
+-rw-r--r--  2.0 unx     1784 b- defN 23-Dec-06 20:33 inference/enterprise/parallel/utils.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Dec-19 16:15 inference/enterprise/stream_management/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Dec-19 16:15 inference/enterprise/stream_management/api/__init__.py
+-rw-r--r--  2.0 unx     6192 b- defN 23-Dec-19 16:15 inference/enterprise/stream_management/api/app.py
+-rw-r--r--  2.0 unx     3843 b- defN 23-Dec-29 18:16 inference/enterprise/stream_management/api/entities.py
+-rw-r--r--  2.0 unx      512 b- defN 23-Dec-19 16:15 inference/enterprise/stream_management/api/errors.py
+-rw-r--r--  2.0 unx     9550 b- defN 23-Dec-19 16:15 inference/enterprise/stream_management/api/stream_manager_client.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Dec-19 16:15 inference/enterprise/stream_management/manager/__init__.py
+-rw-r--r--  2.0 unx     9885 b- defN 23-Dec-19 16:15 inference/enterprise/stream_management/manager/app.py
+-rw-r--r--  2.0 unx     2490 b- defN 23-Dec-19 16:15 inference/enterprise/stream_management/manager/communication.py
+-rw-r--r--  2.0 unx      710 b- defN 23-Dec-19 16:15 inference/enterprise/stream_management/manager/entities.py
+-rw-r--r--  2.0 unx      325 b- defN 23-Dec-19 16:15 inference/enterprise/stream_management/manager/errors.py
+-rw-r--r--  2.0 unx    11131 b- defN 23-Dec-29 18:16 inference/enterprise/stream_management/manager/inference_pipeline_manager.py
+-rw-r--r--  2.0 unx     1619 b- defN 23-Dec-19 16:15 inference/enterprise/stream_management/manager/serialisation.py
+-rw-r--r--  2.0 unx      679 b- defN 23-Dec-19 16:15 inference/enterprise/stream_management/manager/tcp_server.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Feb-02 15:37 inference/enterprise/workflows/__init__.py
+-rw-r--r--  2.0 unx       93 b- defN 24-Feb-02 15:37 inference/enterprise/workflows/constants.py
+-rw-r--r--  2.0 unx     1008 b- defN 24-Feb-02 15:37 inference/enterprise/workflows/errors.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Feb-02 15:37 inference/enterprise/workflows/complier/__init__.py
+-rw-r--r--  2.0 unx     3197 b- defN 24-Feb-02 15:37 inference/enterprise/workflows/complier/core.py
+-rw-r--r--  2.0 unx       97 b- defN 24-Feb-02 15:37 inference/enterprise/workflows/complier/entities.py
+-rw-r--r--  2.0 unx    10391 b- defN 24-Feb-02 15:37 inference/enterprise/workflows/complier/execution_engine.py
+-rw-r--r--  2.0 unx     6055 b- defN 24-Feb-02 15:37 inference/enterprise/workflows/complier/flow_coordinator.py
+-rw-r--r--  2.0 unx    17013 b- defN 24-Feb-02 15:37 inference/enterprise/workflows/complier/graph_parser.py
+-rw-r--r--  2.0 unx     6321 b- defN 24-Feb-02 15:37 inference/enterprise/workflows/complier/runtime_input_validator.py
+-rw-r--r--  2.0 unx     3240 b- defN 24-Feb-02 15:37 inference/enterprise/workflows/complier/utils.py
+-rw-r--r--  2.0 unx     2945 b- defN 24-Feb-02 15:37 inference/enterprise/workflows/complier/validator.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Feb-02 15:37 inference/enterprise/workflows/complier/steps_executors/__init__.py
+-rw-r--r--  2.0 unx    31521 b- defN 24-Feb-02 15:37 inference/enterprise/workflows/complier/steps_executors/auxiliary.py
+-rw-r--r--  2.0 unx      340 b- defN 24-Feb-02 15:37 inference/enterprise/workflows/complier/steps_executors/constants.py
+-rw-r--r--  2.0 unx    25024 b- defN 24-Feb-07 14:49 inference/enterprise/workflows/complier/steps_executors/models.py
+-rw-r--r--  2.0 unx      105 b- defN 24-Feb-02 15:37 inference/enterprise/workflows/complier/steps_executors/types.py
+-rw-r--r--  2.0 unx     2600 b- defN 24-Feb-02 15:37 inference/enterprise/workflows/complier/steps_executors/utils.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Feb-02 15:37 inference/enterprise/workflows/entities/__init__.py
+-rw-r--r--  2.0 unx      124 b- defN 24-Feb-02 15:37 inference/enterprise/workflows/entities/base.py
+-rw-r--r--  2.0 unx      570 b- defN 24-Feb-02 15:37 inference/enterprise/workflows/entities/inputs.py
+-rw-r--r--  2.0 unx      472 b- defN 24-Feb-02 15:37 inference/enterprise/workflows/entities/outputs.py
+-rw-r--r--  2.0 unx    39791 b- defN 24-Feb-07 14:49 inference/enterprise/workflows/entities/steps.py
+-rw-r--r--  2.0 unx     7979 b- defN 24-Feb-07 14:49 inference/enterprise/workflows/entities/validators.py
+-rw-r--r--  2.0 unx     1514 b- defN 24-Feb-02 15:37 inference/enterprise/workflows/entities/workflows_specification.py
+-rw-r--r--  2.0 unx      889 b- defN 24-Feb-07 14:49 inference/models/__init__.py
+-rw-r--r--  2.0 unx     1139 b- defN 24-Feb-07 14:49 inference/models/aliases.py
+-rw-r--r--  2.0 unx     5784 b- defN 24-Feb-07 14:49 inference/models/utils.py
+-rw-r--r--  2.0 unx       50 b- defN 23-Aug-31 21:11 inference/models/clip/__init__.py
+-rw-r--r--  2.0 unx     9748 b- defN 23-Aug-15 19:04 inference/models/clip/clip.py
+-rw-r--r--  2.0 unx    14580 b- defN 23-Dec-29 15:15 inference/models/clip/clip_model.py
+-rw-r--r--  2.0 unx       50 b- defN 23-Dec-14 20:38 inference/models/cogvlm/__init__.py
+-rw-r--r--  2.0 unx     3566 b- defN 23-Dec-29 15:15 inference/models/cogvlm/cogvlm.py
+-rw-r--r--  2.0 unx       53 b- defN 23-Dec-01 20:12 inference/models/doctr/__init__.py
+-rw-r--r--  2.0 unx     5300 b- defN 23-Dec-29 15:15 inference/models/doctr/doctr_model.py
+-rw-r--r--  2.0 unx       44 b- defN 23-Aug-31 21:11 inference/models/gaze/__init__.py
+-rw-r--r--  2.0 unx    13268 b- defN 23-Dec-29 15:15 inference/models/gaze/gaze.py
+-rw-r--r--  2.0 unx     2883 b- defN 23-Aug-31 21:11 inference/models/gaze/l2cs.py
+-rw-r--r--  2.0 unx       73 b- defN 23-Dec-29 15:15 inference/models/grounding_dino/__init__.py
+-rw-r--r--  2.0 unx     5106 b- defN 23-Dec-29 15:15 inference/models/grounding_dino/grounding_dino.py
+-rw-r--r--  2.0 unx       66 b- defN 23-Aug-31 21:11 inference/models/sam/__init__.py
+-rw-r--r--  2.0 unx    14060 b- defN 24-Feb-02 15:37 inference/models/sam/segment_anything.py
+-rw-r--r--  2.0 unx       70 b- defN 23-Aug-31 21:11 inference/models/vit/__init__.py
+-rw-r--r--  2.0 unx     1544 b- defN 23-Oct-20 14:44 inference/models/vit/vit_classification.py
+-rw-r--r--  2.0 unx       72 b- defN 23-Aug-31 21:11 inference/models/yolact/__init__.py
+-rw-r--r--  2.0 unx    13175 b- defN 23-Dec-01 20:12 inference/models/yolact/yolact_instance_segmentation.py
+-rw-r--r--  2.0 unx       85 b- defN 24-Feb-07 14:49 inference/models/yolonas/__init__.py
+-rw-r--r--  2.0 unx     1193 b- defN 24-Feb-07 14:49 inference/models/yolonas/yolonas_object_detection.py
+-rw-r--r--  2.0 unx      183 b- defN 23-Aug-31 21:11 inference/models/yolov5/__init__.py
+-rw-r--r--  2.0 unx     1236 b- defN 23-Oct-20 14:44 inference/models/yolov5/yolov5_instance_segmentation.py
+-rw-r--r--  2.0 unx     1195 b- defN 23-Oct-20 14:44 inference/models/yolov5/yolov5_object_detection.py
+-rw-r--r--  2.0 unx      101 b- defN 23-Aug-31 21:11 inference/models/yolov7/__init__.py
+-rw-r--r--  2.0 unx     1101 b- defN 23-Oct-20 14:44 inference/models/yolov7/yolov7_instance_segmentation.py
+-rw-r--r--  2.0 unx      350 b- defN 23-Dec-29 15:15 inference/models/yolov8/__init__.py
+-rw-r--r--  2.0 unx      415 b- defN 23-Oct-20 14:44 inference/models/yolov8/yolov8_classification.py
+-rw-r--r--  2.0 unx     1803 b- defN 23-Oct-20 14:44 inference/models/yolov8/yolov8_instance_segmentation.py
+-rw-r--r--  2.0 unx     2275 b- defN 23-Dec-14 20:38 inference/models/yolov8/yolov8_keypoints_detection.py
+-rw-r--r--  2.0 unx     1629 b- defN 23-Oct-20 14:44 inference/models/yolov8/yolov8_object_detection.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Oct-20 14:44 inference_cli/__init__.py
+-rw-r--r--  2.0 unx     2428 b- defN 24-Feb-01 14:55 inference_cli/cloud.py
+-rw-r--r--  2.0 unx     2725 b- defN 24-Feb-01 14:55 inference_cli/main.py
+-rw-r--r--  2.0 unx     2098 b- defN 23-Dec-29 18:16 inference_cli/server.py
+-rw-r--r--  2.0 unx       78 b- defN 24-Feb-07 14:52 inference_cli/version.py
+-rw-r--r--  2.0 unx      305 b- defN 24-Feb-01 14:55 inference_cli/lib/__init__.py
+-rw-r--r--  2.0 unx     7205 b- defN 24-Feb-01 14:55 inference_cli/lib/cloud_adapter.py
+-rw-r--r--  2.0 unx     8071 b- defN 24-Jan-17 15:40 inference_cli/lib/container_adapter.py
+-rw-r--r--  2.0 unx      111 b- defN 24-Feb-01 14:55 inference_cli/lib/env.py
+-rw-r--r--  2.0 unx       58 b- defN 24-Jan-08 15:24 inference_cli/lib/exceptions.py
+-rw-r--r--  2.0 unx    13645 b- defN 24-Feb-02 15:37 inference_cli/lib/infer_adapter.py
+-rw-r--r--  2.0 unx      223 b- defN 23-Dec-19 16:15 inference_cli/lib/logger.py
+-rw-r--r--  2.0 unx      954 b- defN 24-Feb-01 14:55 inference_cli/lib/utils.py
+-rw-r--r--  2.0 unx      280 b- defN 23-Oct-06 15:29 inference_client/__init__.py
+-rw-r--r--  2.0 unx       74 b- defN 23-Oct-06 15:29 inference_client/version.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Oct-06 15:29 inference_client/http/__init__.py
+-rw-r--r--  2.0 unx    14400 b- defN 23-Oct-06 15:29 inference_client/http/client.py
+-rw-r--r--  2.0 unx     6835 b- defN 23-Oct-06 15:29 inference_client/http/entities.py
+-rw-r--r--  2.0 unx     1371 b- defN 23-Oct-06 15:29 inference_client/http/errors.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Oct-06 15:29 inference_client/http/utils/__init__.py
+-rw-r--r--  2.0 unx     1325 b- defN 23-Oct-06 15:29 inference_client/http/utils/encoding.py
+-rw-r--r--  2.0 unx      325 b- defN 23-Oct-06 15:29 inference_client/http/utils/iterables.py
+-rw-r--r--  2.0 unx     4188 b- defN 23-Oct-06 15:29 inference_client/http/utils/loaders.py
+-rw-r--r--  2.0 unx     4878 b- defN 23-Oct-06 15:29 inference_client/http/utils/post_processing.py
+-rw-r--r--  2.0 unx     1764 b- defN 23-Oct-06 15:29 inference_client/http/utils/pre_processing.py
+-rw-r--r--  2.0 unx      271 b- defN 23-Oct-20 14:44 inference_sdk/__init__.py
+-rw-r--r--  2.0 unx       78 b- defN 24-Feb-07 14:52 inference_sdk/version.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Oct-20 14:44 inference_sdk/http/__init__.py
+-rw-r--r--  2.0 unx    42988 b- defN 24-Feb-07 14:49 inference_sdk/http/client.py
+-rw-r--r--  2.0 unx     7706 b- defN 24-Feb-02 15:37 inference_sdk/http/entities.py
+-rw-r--r--  2.0 unx     1481 b- defN 24-Feb-02 15:37 inference_sdk/http/errors.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Oct-20 14:44 inference_sdk/http/utils/__init__.py
+-rw-r--r--  2.0 unx     1128 b- defN 24-Feb-07 14:49 inference_sdk/http/utils/aliases.py
+-rw-r--r--  2.0 unx     1315 b- defN 24-Feb-02 15:37 inference_sdk/http/utils/encoding.py
+-rw-r--r--  2.0 unx     5615 b- defN 24-Feb-02 15:37 inference_sdk/http/utils/executors.py
+-rw-r--r--  2.0 unx      683 b- defN 24-Feb-02 15:37 inference_sdk/http/utils/iterables.py
+-rw-r--r--  2.0 unx     8287 b- defN 24-Feb-02 15:37 inference_sdk/http/utils/loaders.py
+-rw-r--r--  2.0 unx     7864 b- defN 24-Feb-02 15:37 inference_sdk/http/utils/post_processing.py
+-rw-r--r--  2.0 unx     1764 b- defN 23-Oct-20 14:44 inference_sdk/http/utils/pre_processing.py
+-rw-r--r--  2.0 unx     2844 b- defN 24-Feb-02 15:37 inference_sdk/http/utils/request_building.py
+-rw-r--r--  2.0 unx     1343 b- defN 24-Feb-02 15:37 inference_sdk/http/utils/requests.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Oct-06 15:29 tests/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Oct-06 15:29 tests/inference/__init__.py
+-rw-r--r--  2.0 unx     2487 b- defN 23-Oct-06 15:29 tests/inference/clip_test.py
+-rw-r--r--  2.0 unx     3226 b- defN 23-Oct-06 15:29 tests/inference/gaze_test.py
+-rw-r--r--  2.0 unx     1981 b- defN 23-Oct-06 15:29 tests/inference/populate_expected_responses.py
+-rw-r--r--  2.0 unx     1244 b- defN 23-Oct-06 15:29 tests/inference/populate_expected_responses_clip.py
+-rw-r--r--  2.0 unx     1241 b- defN 23-Oct-06 15:29 tests/inference/populate_expected_responses_sam.py
+-rw-r--r--  2.0 unx    18954 b- defN 23-Oct-06 15:29 tests/inference/regression_test.py
+-rw-r--r--  2.0 unx     2503 b- defN 23-Oct-06 15:29 tests/inference/sam_test.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Oct-06 15:29 tests/inference_client/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Oct-06 15:29 tests/inference_client/unit_tests/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Oct-06 15:29 tests/inference_client/unit_tests/http/__init__.py
+-rw-r--r--  2.0 unx    30817 b- defN 23-Oct-06 15:29 tests/inference_client/unit_tests/http/test_client.py
+-rw-r--r--  2.0 unx     3409 b- defN 23-Oct-06 15:29 tests/inference_client/unit_tests/http/test_entities.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Oct-06 15:29 tests/inference_client/unit_tests/http/utils/__init__.py
+-rw-r--r--  2.0 unx     1248 b- defN 23-Oct-06 15:29 tests/inference_client/unit_tests/http/utils/conftest.py
+-rw-r--r--  2.0 unx     3376 b- defN 23-Oct-06 15:29 tests/inference_client/unit_tests/http/utils/test_encoding.py
+-rw-r--r--  2.0 unx     1409 b- defN 23-Oct-06 15:29 tests/inference_client/unit_tests/http/utils/test_iterables.py
+-rw-r--r--  2.0 unx    10964 b- defN 23-Oct-06 15:29 tests/inference_client/unit_tests/http/utils/test_loaders.py
+-rw-r--r--  2.0 unx    10200 b- defN 23-Oct-06 15:29 tests/inference_client/unit_tests/http/utils/test_postprocessing.py
+-rw-r--r--  2.0 unx     1982 b- defN 23-Oct-06 15:29 tests/inference_client/unit_tests/http/utils/test_preprocessing.py
+-rw-r--r--  2.0 unx      421 b- defN 24-Feb-07 14:54 inference_gpu-0.9.9rc23.dist-info/LICENSE
+-rw-r--r--  2.0 unx    10237 b- defN 24-Feb-07 14:54 inference_gpu-0.9.9rc23.dist-info/LICENSE.core
+-rw-r--r--  2.0 unx    17296 b- defN 24-Feb-07 14:54 inference_gpu-0.9.9rc23.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Feb-07 14:54 inference_gpu-0.9.9rc23.dist-info/WHEEL
+-rw-r--r--  2.0 unx       53 b- defN 24-Feb-07 14:54 inference_gpu-0.9.9rc23.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       24 b- defN 24-Feb-07 14:54 inference_gpu-0.9.9rc23.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    28764 b- defN 24-Feb-07 14:54 inference_gpu-0.9.9rc23.dist-info/RECORD
+294 files, 1294864 bytes uncompressed, 310136 bytes compressed:  76.0%
```

## zipnote {}

```diff
@@ -1,16 +1,61 @@
+Filename: cli/inference_cli/__init__.py
+Comment: 
+
+Filename: cli/inference_cli/main.py
+Comment: 
+
+Filename: cli/inference_cli/server.py
+Comment: 
+
+Filename: development/__init__.py
+Comment: 
+
+Filename: development/stream_interface/__init__.py
+Comment: 
+
+Filename: development/stream_interface/camera_demo.py
+Comment: 
+
+Filename: development/stream_interface/camera_test.py
+Comment: 
+
+Filename: development/stream_interface/create_dummy_streams.py
+Comment: 
+
+Filename: development/stream_interface/inference_pipeline_demo.py
+Comment: 
+
+Filename: development/stream_interface/multiplexer.py
+Comment: 
+
+Filename: development/stream_interface/multiplexer_demo.py
+Comment: 
+
+Filename: development/stream_interface/old_camera_demo.py
+Comment: 
+
+Filename: development/stream_interface/old_inference_pipeline_demo.py
+Comment: 
+
+Filename: development/stream_interface/udp_receiver.py
+Comment: 
+
 Filename: inference/__init__.py
 Comment: 
 
 Filename: inference/core/__init__.py
 Comment: 
 
 Filename: inference/core/constants.py
 Comment: 
 
+Filename: inference/core/data_models.py
+Comment: 
+
 Filename: inference/core/env.py
 Comment: 
 
 Filename: inference/core/exceptions.py
 Comment: 
 
 Filename: inference/core/logger.py
@@ -270,14 +315,17 @@
 
 Filename: inference/core/models/instance_segmentation_base.py
 Comment: 
 
 Filename: inference/core/models/keypoints_detection_base.py
 Comment: 
 
+Filename: inference/core/models/mixins.py
+Comment: 
+
 Filename: inference/core/models/object_detection_base.py
 Comment: 
 
 Filename: inference/core/models/roboflow.py
 Comment: 
 
 Filename: inference/core/models/stubs.py
@@ -303,14 +351,26 @@
 
 Filename: inference/core/registries/base.py
 Comment: 
 
 Filename: inference/core/registries/roboflow.py
 Comment: 
 
+Filename: inference/core/registries/decorators/__init__.py
+Comment: 
+
+Filename: inference/core/registries/decorators/base.py
+Comment: 
+
+Filename: inference/core/registries/decorators/fixed_device_id.py
+Comment: 
+
+Filename: inference/core/registries/decorators/trt_device_id.py
+Comment: 
+
 Filename: inference/core/utils/__init__.py
 Comment: 
 
 Filename: inference/core/utils/environment.py
 Comment: 
 
 Filename: inference/core/utils/file_system.py
@@ -339,14 +399,17 @@
 
 Filename: inference/core/utils/s3.py
 Comment: 
 
 Filename: inference/core/utils/url_utils.py
 Comment: 
 
+Filename: inference/core/utils/validate.py
+Comment: 
+
 Filename: inference/core/utils/visualisation.py
 Comment: 
 
 Filename: inference/enterprise/__init__.py
 Comment: 
 
 Filename: inference/enterprise/device_manager/__init__.py
@@ -519,14 +582,17 @@
 
 Filename: inference/models/utils.py
 Comment: 
 
 Filename: inference/models/clip/__init__.py
 Comment: 
 
+Filename: inference/models/clip/clip.py
+Comment: 
+
 Filename: inference/models/clip/clip_model.py
 Comment: 
 
 Filename: inference/models/cogvlm/__init__.py
 Comment: 
 
 Filename: inference/models/cogvlm/cogvlm.py
@@ -615,14 +681,17 @@
 
 Filename: inference_cli/main.py
 Comment: 
 
 Filename: inference_cli/server.py
 Comment: 
 
+Filename: inference_cli/version.py
+Comment: 
+
 Filename: inference_cli/lib/__init__.py
 Comment: 
 
 Filename: inference_cli/lib/cloud_adapter.py
 Comment: 
 
 Filename: inference_cli/lib/container_adapter.py
@@ -639,29 +708,176 @@
 
 Filename: inference_cli/lib/logger.py
 Comment: 
 
 Filename: inference_cli/lib/utils.py
 Comment: 
 
-Filename: inference_gpu-0.9.9.dist-info/LICENSE
+Filename: inference_client/__init__.py
+Comment: 
+
+Filename: inference_client/version.py
+Comment: 
+
+Filename: inference_client/http/__init__.py
+Comment: 
+
+Filename: inference_client/http/client.py
+Comment: 
+
+Filename: inference_client/http/entities.py
+Comment: 
+
+Filename: inference_client/http/errors.py
+Comment: 
+
+Filename: inference_client/http/utils/__init__.py
+Comment: 
+
+Filename: inference_client/http/utils/encoding.py
+Comment: 
+
+Filename: inference_client/http/utils/iterables.py
+Comment: 
+
+Filename: inference_client/http/utils/loaders.py
+Comment: 
+
+Filename: inference_client/http/utils/post_processing.py
+Comment: 
+
+Filename: inference_client/http/utils/pre_processing.py
+Comment: 
+
+Filename: inference_sdk/__init__.py
+Comment: 
+
+Filename: inference_sdk/version.py
+Comment: 
+
+Filename: inference_sdk/http/__init__.py
+Comment: 
+
+Filename: inference_sdk/http/client.py
+Comment: 
+
+Filename: inference_sdk/http/entities.py
+Comment: 
+
+Filename: inference_sdk/http/errors.py
+Comment: 
+
+Filename: inference_sdk/http/utils/__init__.py
+Comment: 
+
+Filename: inference_sdk/http/utils/aliases.py
+Comment: 
+
+Filename: inference_sdk/http/utils/encoding.py
+Comment: 
+
+Filename: inference_sdk/http/utils/executors.py
+Comment: 
+
+Filename: inference_sdk/http/utils/iterables.py
+Comment: 
+
+Filename: inference_sdk/http/utils/loaders.py
+Comment: 
+
+Filename: inference_sdk/http/utils/post_processing.py
+Comment: 
+
+Filename: inference_sdk/http/utils/pre_processing.py
+Comment: 
+
+Filename: inference_sdk/http/utils/request_building.py
+Comment: 
+
+Filename: inference_sdk/http/utils/requests.py
+Comment: 
+
+Filename: tests/__init__.py
+Comment: 
+
+Filename: tests/inference/__init__.py
+Comment: 
+
+Filename: tests/inference/clip_test.py
+Comment: 
+
+Filename: tests/inference/gaze_test.py
+Comment: 
+
+Filename: tests/inference/populate_expected_responses.py
+Comment: 
+
+Filename: tests/inference/populate_expected_responses_clip.py
+Comment: 
+
+Filename: tests/inference/populate_expected_responses_sam.py
+Comment: 
+
+Filename: tests/inference/regression_test.py
+Comment: 
+
+Filename: tests/inference/sam_test.py
+Comment: 
+
+Filename: tests/inference_client/__init__.py
+Comment: 
+
+Filename: tests/inference_client/unit_tests/__init__.py
+Comment: 
+
+Filename: tests/inference_client/unit_tests/http/__init__.py
+Comment: 
+
+Filename: tests/inference_client/unit_tests/http/test_client.py
+Comment: 
+
+Filename: tests/inference_client/unit_tests/http/test_entities.py
+Comment: 
+
+Filename: tests/inference_client/unit_tests/http/utils/__init__.py
+Comment: 
+
+Filename: tests/inference_client/unit_tests/http/utils/conftest.py
+Comment: 
+
+Filename: tests/inference_client/unit_tests/http/utils/test_encoding.py
+Comment: 
+
+Filename: tests/inference_client/unit_tests/http/utils/test_iterables.py
+Comment: 
+
+Filename: tests/inference_client/unit_tests/http/utils/test_loaders.py
+Comment: 
+
+Filename: tests/inference_client/unit_tests/http/utils/test_postprocessing.py
+Comment: 
+
+Filename: tests/inference_client/unit_tests/http/utils/test_preprocessing.py
+Comment: 
+
+Filename: inference_gpu-0.9.9rc23.dist-info/LICENSE
 Comment: 
 
-Filename: inference_gpu-0.9.9.dist-info/LICENSE.core
+Filename: inference_gpu-0.9.9rc23.dist-info/LICENSE.core
 Comment: 
 
-Filename: inference_gpu-0.9.9.dist-info/METADATA
+Filename: inference_gpu-0.9.9rc23.dist-info/METADATA
 Comment: 
 
-Filename: inference_gpu-0.9.9.dist-info/WHEEL
+Filename: inference_gpu-0.9.9rc23.dist-info/WHEEL
 Comment: 
 
-Filename: inference_gpu-0.9.9.dist-info/entry_points.txt
+Filename: inference_gpu-0.9.9rc23.dist-info/entry_points.txt
 Comment: 
 
-Filename: inference_gpu-0.9.9.dist-info/top_level.txt
+Filename: inference_gpu-0.9.9rc23.dist-info/top_level.txt
 Comment: 
 
-Filename: inference_gpu-0.9.9.dist-info/RECORD
+Filename: inference_gpu-0.9.9rc23.dist-info/RECORD
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

## Comparing `inference_gpu-0.9.9.dist-info/LICENSE.core` & `inference_gpu-0.9.9rc23.dist-info/LICENSE.core`

 * *Files identical despite different names*

## Comparing `inference_gpu-0.9.9.dist-info/METADATA` & `inference_gpu-0.9.9rc23.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,45 +1,21 @@
 Metadata-Version: 2.1
 Name: inference-gpu
-Version: 0.9.9
+Version: 0.9.9rc23
 Summary: With no prior knowledge of machine learning or device-specific deployment, you can deploy a computer vision model to a range of devices and environments using Roboflow Inference.
 Home-page: https://github.com/roboflow/inference
 Author: Roboflow
 Author-email: help@roboflow.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
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
-Requires-Dist: onnxruntime-gpu <=1.15.1
-Requires-Dist: inference-cli ==0.9.9
 Provides-Extra: clip
 Requires-Dist: rf-clip ==1.0 ; extra == 'clip'
 Provides-Extra: gaze
 Requires-Dist: mediapipe <0.11,>=0.9 ; extra == 'gaze'
 Provides-Extra: hosted
 Requires-Dist: boto3 <=1.28.23 ; extra == 'hosted'
 Requires-Dist: pymemcache <=4.0.0 ; extra == 'hosted'
```

## Comparing `inference_gpu-0.9.9.dist-info/RECORD` & `inference_gpu-0.9.9rc23.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,32 @@
+cli/inference_cli/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+cli/inference_cli/main.py,sha256=UnwKBEXjIrRLiB0lH0qw_75CX0wOzex4iOeJVUqPOr8,1198
+cli/inference_cli/server.py,sha256=PAkIYL9eNF_vJz5Vfw5T8FD5s7vduJLhbMTmke0HZq4,1022
+development/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+development/stream_interface/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+development/stream_interface/camera_demo.py,sha256=vDsv2uJmUPKB9gMC3UcblfdZw-XCwSE6kHnnacHG6Do,3594
+development/stream_interface/camera_test.py,sha256=HB7fCRv0JS4SmbiCr8TlA0lkwWfPLVILDEkQCBwaQ2k,1444
+development/stream_interface/create_dummy_streams.py,sha256=1l1C37YwtT_pI6FSK3M7r1pcJkbOH16dDCLiZ39aZWE,2475
+development/stream_interface/inference_pipeline_demo.py,sha256=C_KU08t1olMWOn_s6lvEXVQocUx1XmSMK1Je0D5Mbfg,4827
+development/stream_interface/multiplexer.py,sha256=76ulJfgFRE5EpIR2I3ix9qxvvQjQErYX2OVLsXPXsw0,790
+development/stream_interface/multiplexer_demo.py,sha256=P4h0cwcuc1o30_kFE_uP4pzTS9teYM77nLBnPBrPbWU,4433
+development/stream_interface/old_camera_demo.py,sha256=FVK2Le4AW2nCoRqyWx1wWPNGLRVQStDnjTK5iRBMKkY,2934
+development/stream_interface/old_inference_pipeline_demo.py,sha256=-lDPMqgv9MDZP08qe-QmtRSjcWpv7uuoD1TbNmdYwoI,2314
+development/stream_interface/udp_receiver.py,sha256=qU1LLH85-pxOvOb5OsKUszYJYgSPNEjhKLTJ2se_8p0,579
 inference/__init__.py,sha256=ViPGYL_0ke_-bFnF_rXnV0SOQu6zB20pI8-zq-KxWnY,209
 inference/core/__init__.py,sha256=2ECiVgXKnx-57HSeLsclTfsxyuhcjm-J1dvu6458zJ0,1728
 inference/core/constants.py,sha256=vArFjw8mR6utyw8JRz5P9HB1RRXeqO2QlFtGvdoKO6o,183
+inference/core/data_models.py,sha256=gCAn9ilBoTTELixO7K4q7uz2hKHoaqS06IHJb_OBYEc,34827
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
@@ -86,37 +101,43 @@
 inference/core/managers/decorators/locked_load.py,sha256=9M1CISfb-Yu1mgCTe6OhdKNOZCrf6P64oOpFlmoJglE,487
 inference/core/managers/decorators/logger.py,sha256=ZXrM76tKBE6xG6EXLmwSzODnFUiFGi4PNboSzJRscjk,1990
 inference/core/models/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 inference/core/models/base.py,sha256=vY54BFs_iCaZOI5IPL3WMgOU6tNHWnx_0V_ywtPFPIs,5316
 inference/core/models/classification_base.py,sha256=p3B9xLCVJvo-w3uG-ag4EqoDc6rctQd9lImRS3ms290,16272
 inference/core/models/instance_segmentation_base.py,sha256=G5ydVj8fzK3AFdBxA9xduYHRJWfGeZ_oW113eLLss9w,13358
 inference/core/models/keypoints_detection_base.py,sha256=6zg77SwFXM9rj98PkPFX3NDlmLXKiv-4CFgyG8qQtqU,7645
+inference/core/models/mixins.py,sha256=US_AboVezubaI7EOH63usIsrdSxuIYvCiRXRC76rSe8,4786
 inference/core/models/object_detection_base.py,sha256=KLzMYlHa_xq9NwmySSaW1UVSOQsBAr5uYqjRmJthGuo,12638
 inference/core/models/roboflow.py,sha256=WshvKGIb_fynyJI_75EgUWP4zrbaZUpC8MaOmlpRAJM,32993
 inference/core/models/stubs.py,sha256=8o01f2gGassRRaHeKPUvECOGIlR2Zm2pOsGhiPD07Xk,4805
 inference/core/models/types.py,sha256=QPpQYSoWrulQIkShHQ32j2-XrpV0d0nJPZPOn5OLnZA,103
 inference/core/models/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 inference/core/models/utils/batching.py,sha256=ewfZ7vvQi4vyqXxswWH8h0qMQ3zO8PwR6HA9u_E1Xnk,619
 inference/core/models/utils/keypoints.py,sha256=YnXqKgYyKXt55jRFySRgMw7I4wmvbXk1pVv3ltXeDpI,1492
 inference/core/models/utils/validate.py,sha256=ATHGFqIU1Xx6NHhGvWA_r-RY8LbnQzXRe0we_7EYf-U,173
 inference/core/registries/__init__.py,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
 inference/core/registries/base.py,sha256=GFQojRoKhGiuU85NcDv3lOyBkSFfhcAx9vpixDS9Muw,1395
 inference/core/registries/roboflow.py,sha256=M_d-AW44ngnOFohL_mn_KOeyb1UnRyKlPUdUhS_l5Yo,8545
+inference/core/registries/decorators/__init__.py,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+inference/core/registries/decorators/base.py,sha256=QIQAT7U7Z0Cc1lQgSIPGQ8LURK__5iGJtVPQTxMUQpA,1347
+inference/core/registries/decorators/fixed_device_id.py,sha256=E4y-1zQRGJ79iduK5voT4fllNQ--F4Ev-YH6oilU6DQ,2462
+inference/core/registries/decorators/trt_device_id.py,sha256=yAacOP-j1D8Um_-QrQ7WGj2UfYcOZ8f_JzG_MbkT_nw,2250
 inference/core/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 inference/core/utils/environment.py,sha256=Prz_makJKdmrxY5NVLUtAJhTOSM4MfYLOxsIAB_vg5M,2104
 inference/core/utils/file_system.py,sha256=-qbmmePmwsAMu8e2GJYmHhycCQnn7rZi0oAcX0X9AnI,1908
 inference/core/utils/image_utils.py,sha256=GGCb3oD0ghUi9lTEpYXty1X60yhqGiTl9UNtdA80leU,14257
 inference/core/utils/notebooks.py,sha256=6Du8O87n0tNpmrUBwJzAE5aHDHWjoSRlwUTFC-gE884,679
 inference/core/utils/onnx.py,sha256=HiS-X5df0kWbDvT9vT5Oz4z35qj2vJRI3AnqZsLwj1c,660
 inference/core/utils/postprocess.py,sha256=Uaw0QZPS4_5ae8OApMOzw0gwSpeDL3GZ0gPA34US5nc,21533
 inference/core/utils/preprocess.py,sha256=vwfPpH-brzDjMuBuGb2P0rDDxsbbcDy2gnNymmAwGbs,8381
 inference/core/utils/requests.py,sha256=8v31vZJOQDjjG1Y-3SBFwhTwklFeOGCO4cmO243r0zg,712
 inference/core/utils/roboflow.py,sha256=ThonpeB5xCV24c67ZsnD4W-OeSQCMEn7FKKyxrE_wy8,419
 inference/core/utils/s3.py,sha256=cGQhyRQ6VEOqgjN3Pv8nVsfg6NsRYHZfl77SnIZWmmo,430
 inference/core/utils/url_utils.py,sha256=j8KqS6whemrCXfNUGH8Xo_ramyhkhvl4hTKVJUgaa_w,244
+inference/core/utils/validate.py,sha256=rZuu5ordt1s8kDGUK41c_iPgpSqYNHYLWttieppCTr8,142
 inference/core/utils/visualisation.py,sha256=-M5mgxl_XkSly4bA-cpr8hU4TfB1VmDzeLeuRhvzTlQ,4444
 inference/enterprise/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 inference/enterprise/device_manager/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 inference/enterprise/device_manager/command_handler.py,sha256=iDwObWUPy419QtWLwcvSU_ryb9wvFflZ2gS2m1E481A,2902
 inference/enterprise/device_manager/container_service.py,sha256=YdG-GDG1aHoy7hGh3xs7AvD3kZVn_i7VHlugEyBukLQ,9478
 inference/enterprise/device_manager/device_manager.py,sha256=WK1L_fzUmr1BL1XOThUx844l5tT0wteWUB-BukTm2yU,1825
 inference/enterprise/device_manager/helpers.py,sha256=Ig2y2TRc1u-yTuayRI5kRR8G6JNNiXQhQ86MIGpjYJE,1514
@@ -169,14 +190,15 @@
 inference/enterprise/workflows/entities/steps.py,sha256=FMOsvMCXIiDrHfuJcGU0bwrHRiflYyxRPYVOGThfrgA,39791
 inference/enterprise/workflows/entities/validators.py,sha256=zsolS9Vs-L1egAwXc7kxYfSrTZpxsUKQPreoCOynXEs,7979
 inference/enterprise/workflows/entities/workflows_specification.py,sha256=u0WFl-pTV0OXGEATKZBaXeiZBqXpy5PvWL9FEX8CJuM,1514
 inference/models/__init__.py,sha256=6kFaxN5ZU1eLhTalMVqqpFZzgAcAuBTEoNd4JWrggBI,889
 inference/models/aliases.py,sha256=yW-YZ0BpXvHmSZWLccet-Z8vsonKmiGnrsXmVpJRGBE,1139
 inference/models/utils.py,sha256=rn4YE2wJfQuq-27uDQO8Q88ap58DKKg071Gaf623M_s,5784
 inference/models/clip/__init__.py,sha256=iAq2TD2DhrWFG1NJ3kh9RatvBfieF6hj2z7UxPYhWxc,50
+inference/models/clip/clip.py,sha256=9wEU4oLXx_CKsOFuRNVdy6GjH-Ljo6vujkOOMyOiv2w,9748
 inference/models/clip/clip_model.py,sha256=yTjnaqKoMZN-0wXbyqt2SW5BD4KMveFvw3zY-nNoHfM,14580
 inference/models/cogvlm/__init__.py,sha256=Lr9qDmCPM_4fnvelMUI4X2M1Y-1pIz3vTUtWM8nzZL4,50
 inference/models/cogvlm/cogvlm.py,sha256=HabuDk7xHsasTM9odwzMmncXJsO4vdJJMHA14FOT2Bo,3566
 inference/models/doctr/__init__.py,sha256=gTF3hsbWM6um5myaYeFsmP7xmUp0TS4X8XpLmwoertw,53
 inference/models/doctr/doctr_model.py,sha256=4FYk30Fnscb7XtZbv2OT0avunvm9sNdprTmg93GrOHQ,5300
 inference/models/gaze/__init__.py,sha256=hHlwYHncEJVJ2jQ9SBBhpVNz2ra_w5shHPwE0BEDKuI,44
 inference/models/gaze/gaze.py,sha256=v04hNQWZZr29FCRRdoqhbUC2G34yhOiBd9q50va1T0c,13268
@@ -201,22 +223,72 @@
 inference/models/yolov8/yolov8_instance_segmentation.py,sha256=J-HK1V4YmJ6T-Z7MoYK-N0UwYoJAxu4b2kV1MXzt4qc,1803
 inference/models/yolov8/yolov8_keypoints_detection.py,sha256=z6c1P9Tm2mdbrW-43Iobsv7_5ue0T1WqgnKQ7GY5bTs,2275
 inference/models/yolov8/yolov8_object_detection.py,sha256=YX6YyQ6K3wtrq3Qd4RVmAgE6SNbrOE4EbYJUo7EXcCg,1629
 inference_cli/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 inference_cli/cloud.py,sha256=OLzYCWGRcqIiz3IhmR-NVYnT9KUp1cLdpGhl-73dLCQ,2428
 inference_cli/main.py,sha256=H5Uk29LfiIySGjge_HaG1Y0EjDtmUr7T2022Gln6Me4,2725
 inference_cli/server.py,sha256=pZuRH8uxo6XwB6v1BMhulCSHi-m-TuFhTxn5mFz_OLQ,2098
+inference_cli/version.py,sha256=aeCX65wj2wOyKA6nK9QbNhIR-u4qs7jnQQgNh083cPg,78
 inference_cli/lib/__init__.py,sha256=W2y_yrjAQ8TIoqApzagbY-aZyEWySSO1NJUfzhww3cY,305
 inference_cli/lib/cloud_adapter.py,sha256=uMI9iF6HcBZb6e0HUzL99uXPxkyynnlPVyiHJKBk3zI,7205
 inference_cli/lib/container_adapter.py,sha256=sGCdNO1CsmSH6WdrmPtmyhvgIzhn6kKuKohumcMC3cA,8071
 inference_cli/lib/env.py,sha256=Q0unXcIInG-es1xrcYwSecBMfC6v3iBUXsWf4Ph5duM,111
 inference_cli/lib/exceptions.py,sha256=QG9LbV_WNlrdX22FVQWVgDeiKwIH2oZuA95Cetibg_A,58
 inference_cli/lib/infer_adapter.py,sha256=DY9mATO_y0gYiLcQjB0jfH6cZbWTJp1OG_vzggjY2fk,13645
 inference_cli/lib/logger.py,sha256=-iEOIxVEysU8qDPOluh_k6We4RGP8k7LYTjPFusMiCc,223
 inference_cli/lib/utils.py,sha256=ru_bGs_xgqsW7fknu_jkzQEbr6jb7V_PCAylaej4yeA,954
-inference_gpu-0.9.9.dist-info/LICENSE,sha256=6_siNlKng4EAb5WZXZuD9cKF38PWick7dL42U_h1KIE,421
-inference_gpu-0.9.9.dist-info/LICENSE.core,sha256=Ioa7wFnewa3uNb527FeTbJztwGh5UsYJ9aNnfqyfDLs,10237
-inference_gpu-0.9.9.dist-info/METADATA,sha256=hnCiDOK_CR1iGgC9bN-HKplE20gfY80ytCW3dvNmIOM,18129
-inference_gpu-0.9.9.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-inference_gpu-0.9.9.dist-info/entry_points.txt,sha256=Dm0LrFRve6WvcWk8HRaftIFO8t6vYYmK4AOPHKxE0Ow,53
-inference_gpu-0.9.9.dist-info/top_level.txt,sha256=D3WONB8QzL2SAlaDLnKfMY695oOJ30WxYQ4oFngpvIw,24
-inference_gpu-0.9.9.dist-info/RECORD,,
+inference_client/__init__.py,sha256=8KZS3S70OamXNWyoa88sDGjXzFEKLGr2-Zc4YXSlZdw,280
+inference_client/version.py,sha256=njDohAc4RF3ligA9q1eoCYxnZIJa2KHRRVhcDRvx228,74
+inference_client/http/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+inference_client/http/client.py,sha256=bRcwiinPuRIzT5EdFaJfyZp6wDmV-lIW84dQ6SRVHOE,14400
+inference_client/http/entities.py,sha256=J7cUyp4K8onxIgsq2nhjyam9VYE6yVxViRqF4htTCIM,6835
+inference_client/http/errors.py,sha256=pwbb_WUJ8qdx6YmD6Nm2JlD6MPX96WisdV0CByVW20Y,1371
+inference_client/http/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+inference_client/http/utils/encoding.py,sha256=wyD3kJwwB2Hxb2T15Z5yjbqk2b_vtfSbbmq6hyuJoQI,1325
+inference_client/http/utils/iterables.py,sha256=gIh7L-AGCDysJst1IXHS4QF2mkntZK2-F8f_Oi0f-JM,325
+inference_client/http/utils/loaders.py,sha256=L9Lc8qvQWwJrzaAASdLuYCSdqd7DN-Lasn1dtk58nHo,4188
+inference_client/http/utils/post_processing.py,sha256=vFgz5eMBJZ7Ok_yoC8SnZBAwk1uiXDxeLu3r6o7nWGI,4878
+inference_client/http/utils/pre_processing.py,sha256=wjv0DMBxedO9b5c4N1o_1pjvNZymGhScT0QrEExcuVA,1764
+inference_sdk/__init__.py,sha256=Mvg5MwdGi8mPK-WQCHlaAPIRQkAIeMpRUw5PEAiOrC0,271
+inference_sdk/version.py,sha256=aeCX65wj2wOyKA6nK9QbNhIR-u4qs7jnQQgNh083cPg,78
+inference_sdk/http/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+inference_sdk/http/client.py,sha256=-ofzhRoQHQ9oZhVdr9VXuUcwGOM_9F44CtMw5HgESFY,42988
+inference_sdk/http/entities.py,sha256=7AUzCuGt_NW3zm_zryO62f8yS1Lh2ev5221FbA3Llns,7706
+inference_sdk/http/errors.py,sha256=Jp51BbjZILi_xioUkbccoAXlrwcoL_8KKgkzXZNFhwY,1481
+inference_sdk/http/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+inference_sdk/http/utils/aliases.py,sha256=MYmFYP4ivSsNn0pbSYsggje4Ap3T62VI7o9rvBQyDpc,1128
+inference_sdk/http/utils/encoding.py,sha256=mrcjB8RZct3cXcK5RmUxL3pZfRrxbqIG_5I6TFVV08o,1315
+inference_sdk/http/utils/executors.py,sha256=0khWUIO23qLC15hQDa6WmUDj1dlJUDn1yjLK8W9Pu-k,5615
+inference_sdk/http/utils/iterables.py,sha256=vIChVZaiUQrXe-ha7ewaZWryYR5qQxCYzW5W7Rp0DqQ,683
+inference_sdk/http/utils/loaders.py,sha256=la9QRY7LLm1scIIvD7fuV3YwQq8PgeKkfYWcCXrd3QA,8287
+inference_sdk/http/utils/post_processing.py,sha256=IJ34gvmE3dQ0PT9oTWlzWCCHWlv09cV5aHRZjpdhdFc,7864
+inference_sdk/http/utils/pre_processing.py,sha256=wjv0DMBxedO9b5c4N1o_1pjvNZymGhScT0QrEExcuVA,1764
+inference_sdk/http/utils/request_building.py,sha256=KfIqFsrLlNO1uCROsqLFEuGom-C35nSG8JpQdUTOUNs,2844
+inference_sdk/http/utils/requests.py,sha256=vK1y_9X_6JxgP9vpiAyLc6GzqBmmud6cA0JF7z1hPcw,1343
+tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+tests/inference/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+tests/inference/clip_test.py,sha256=WtNdSuea7mUKJmNPQ3-Taf29vursLrq8FX37scFCaAs,2487
+tests/inference/gaze_test.py,sha256=PeVZ9YsQO5Vz36wyfr7Bg7SccQzdmRPGMWrrDT-pYjM,3226
+tests/inference/populate_expected_responses.py,sha256=Qqwz8sgt3yR-D_TWPVucEAmeW4-yPCI2Rgeea3xSpzQ,1981
+tests/inference/populate_expected_responses_clip.py,sha256=V2FYaKKcisjHX-yYiMPM5j74hdnVNibDTPU5sD_B9kg,1244
+tests/inference/populate_expected_responses_sam.py,sha256=Cppl5QUi2u_JVGnEKv-fVnxWmT5LDPwKpZkuIgl55Ks,1241
+tests/inference/regression_test.py,sha256=V-zluX1HGItTZM9QBilOV2XaEPsBdse7QhmKD0cJomw,18954
+tests/inference/sam_test.py,sha256=dYBpGE4rsZHtv-i7AWgm1qk68MM_xOwEzSh430OTP94,2503
+tests/inference_client/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+tests/inference_client/unit_tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+tests/inference_client/unit_tests/http/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+tests/inference_client/unit_tests/http/test_client.py,sha256=-jYsHRwTAIGpJhfrRE3hOvPEnYQedYrbQF79Cp2-_K4,30817
+tests/inference_client/unit_tests/http/test_entities.py,sha256=uOcvAMY2y5lwyEhgYe0unsby04uze6mErzdo41W0J3o,3409
+tests/inference_client/unit_tests/http/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+tests/inference_client/unit_tests/http/utils/conftest.py,sha256=WtQ6Iz-S9paqa6I9N-I2UFuQj_eLfcVR57IZXXjdURU,1248
+tests/inference_client/unit_tests/http/utils/test_encoding.py,sha256=ojKCZ4MywJhJk3eifJtQLA-jE107mFFhxw5JuthQxTo,3376
+tests/inference_client/unit_tests/http/utils/test_iterables.py,sha256=5YtK7HhRaFWFs4cx90g9zHQJ-PGWe5vwllVsUTEL1hI,1409
+tests/inference_client/unit_tests/http/utils/test_loaders.py,sha256=IS88DLAHYo8nOVzGAdnap82kGbVkW1-5GHIqPdSb56Q,10964
+tests/inference_client/unit_tests/http/utils/test_postprocessing.py,sha256=ASNRWE1ajJP33Vk4kCIZapBUEO0o3BLCMKg9SmR4KAM,10200
+tests/inference_client/unit_tests/http/utils/test_preprocessing.py,sha256=xRRDzGDoZiG04eHw3vLqpHd8wM20f7yCdCykpBLT41c,1982
+inference_gpu-0.9.9rc23.dist-info/LICENSE,sha256=6_siNlKng4EAb5WZXZuD9cKF38PWick7dL42U_h1KIE,421
+inference_gpu-0.9.9rc23.dist-info/LICENSE.core,sha256=Ioa7wFnewa3uNb527FeTbJztwGh5UsYJ9aNnfqyfDLs,10237
+inference_gpu-0.9.9rc23.dist-info/METADATA,sha256=OykO4m2NlILTIvAowZLFuMifoZBn0uNxwwwlusZ-9no,17296
+inference_gpu-0.9.9rc23.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+inference_gpu-0.9.9rc23.dist-info/entry_points.txt,sha256=Dm0LrFRve6WvcWk8HRaftIFO8t6vYYmK4AOPHKxE0Ow,53
+inference_gpu-0.9.9rc23.dist-info/top_level.txt,sha256=D3WONB8QzL2SAlaDLnKfMY695oOJ30WxYQ4oFngpvIw,24
+inference_gpu-0.9.9rc23.dist-info/RECORD,,
```

