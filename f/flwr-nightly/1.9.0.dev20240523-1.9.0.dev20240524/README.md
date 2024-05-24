# Comparing `tmp/flwr_nightly-1.9.0.dev20240523.tar.gz` & `tmp/flwr_nightly-1.9.0.dev20240524.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flwr_nightly-1.9.0.dev20240523.tar", max compression
+gzip compressed data, was "flwr_nightly-1.9.0.dev20240524.tar", max compression
```

## Comparing `flwr_nightly-1.9.0.dev20240523.tar` & `flwr_nightly-1.9.0.dev20240524.tar`

### file list

```diff
@@ -1,231 +1,231 @@
--rw-r--r--   0        0        0    11358 2024-05-23 23:05:25.340638 flwr_nightly-1.9.0.dev20240523/LICENSE
--rw-r--r--   0        0        0    13010 2024-05-23 23:05:25.340638 flwr_nightly-1.9.0.dev20240523/README.md
--rw-r--r--   0        0        0     5836 2024-05-23 23:05:38.880659 flwr_nightly-1.9.0.dev20240523/pyproject.toml
--rw-r--r--   0        0        0      937 2024-05-23 23:05:25.768638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/__init__.py
--rw-r--r--   0        0        0      720 2024-05-23 23:05:25.768638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/cli/__init__.py
--rw-r--r--   0        0        0     1141 2024-05-23 23:05:25.768638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/cli/app.py
--rw-r--r--   0        0        0     5064 2024-05-23 23:05:25.768638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/cli/build.py
--rw-r--r--   0        0        0     4277 2024-05-23 23:05:25.768638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/cli/config_utils.py
--rw-r--r--   0        0        0     2215 2024-05-23 23:05:25.768638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/cli/example.py
--rw-r--r--   0        0        0      789 2024-05-23 23:05:25.768638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/cli/new/__init__.py
--rw-r--r--   0        0        0     6223 2024-05-23 23:05:25.768638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/cli/new/new.py
--rw-r--r--   0        0        0      725 2024-05-23 23:05:25.768638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/cli/new/templates/__init__.py
--rw-r--r--   0        0        0     3078 2024-05-23 23:05:25.768638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/cli/new/templates/app/.gitignore.tpl
--rw-r--r--   0        0        0      668 2024-05-23 23:05:25.768638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/cli/new/templates/app/README.md.tpl
--rw-r--r--   0        0        0      729 2024-05-23 23:05:25.768638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/cli/new/templates/app/__init__.py
--rw-r--r--   0        0        0      736 2024-05-23 23:05:25.768638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/cli/new/templates/app/code/__init__.py
--rw-r--r--   0        0        0       21 2024-05-23 23:05:25.768638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/cli/new/templates/app/code/__init__.py.tpl
--rw-r--r--   0        0        0     1450 2024-05-23 23:05:25.768638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/cli/new/templates/app/code/client.hf.py.tpl
--rw-r--r--   0        0        0     1434 2024-05-23 23:05:25.768638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/cli/new/templates/app/code/client.jax.py.tpl
--rw-r--r--   0        0        0     2113 2024-05-23 23:05:25.768638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/cli/new/templates/app/code/client.mlx.py.tpl
--rw-r--r--   0        0        0      521 2024-05-23 23:05:25.768638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/cli/new/templates/app/code/client.numpy.py.tpl
--rw-r--r--   0        0        0     1172 2024-05-23 23:05:25.768638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/cli/new/templates/app/code/client.pytorch.py.tpl
--rw-r--r--   0        0        0     2801 2024-05-23 23:05:25.768638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/cli/new/templates/app/code/client.sklearn.py.tpl
--rw-r--r--   0        0        0     1280 2024-05-23 23:05:25.768638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/cli/new/templates/app/code/client.tensorflow.py.tpl
--rw-r--r--   0        0        0      338 2024-05-23 23:05:25.768638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/cli/new/templates/app/code/server.hf.py.tpl
--rw-r--r--   0        0        0      246 2024-05-23 23:05:25.768638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/cli/new/templates/app/code/server.jax.py.tpl
--rw-r--r--   0        0        0      272 2024-05-23 23:05:25.768638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/cli/new/templates/app/code/server.mlx.py.tpl
--rw-r--r--   0        0        0      248 2024-05-23 23:05:25.768638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/cli/new/templates/app/code/server.numpy.py.tpl
--rw-r--r--   0        0        0      593 2024-05-23 23:05:25.768638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/cli/new/templates/app/code/server.pytorch.py.tpl
--rw-r--r--   0        0        0      341 2024-05-23 23:05:25.768638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/cli/new/templates/app/code/server.sklearn.py.tpl
--rw-r--r--   0        0        0      579 2024-05-23 23:05:25.768638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/cli/new/templates/app/code/server.tensorflow.py.tpl
--rw-r--r--   0        0        0     2857 2024-05-23 23:05:25.768638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/cli/new/templates/app/code/task.hf.py.tpl
--rw-r--r--   0        0        0     1519 2024-05-23 23:05:25.768638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/cli/new/templates/app/code/task.jax.py.tpl
--rw-r--r--   0        0        0     2598 2024-05-23 23:05:25.768638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/cli/new/templates/app/code/task.mlx.py.tpl
--rw-r--r--   0        0        0     3684 2024-05-23 23:05:25.768638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/cli/new/templates/app/code/task.pytorch.py.tpl
--rw-r--r--   0        0        0     1044 2024-05-23 23:05:25.768638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/cli/new/templates/app/code/task.tensorflow.py.tpl
--rw-r--r--   0        0        0      759 2024-05-23 23:05:25.768638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/cli/new/templates/app/pyproject.hf.toml.tpl
--rw-r--r--   0        0        0      568 2024-05-23 23:05:25.768638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/cli/new/templates/app/pyproject.jax.toml.tpl
--rw-r--r--   0        0        0      668 2024-05-23 23:05:25.768638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/cli/new/templates/app/pyproject.mlx.toml.tpl
--rw-r--r--   0        0        0      606 2024-05-23 23:05:25.768638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/cli/new/templates/app/pyproject.numpy.toml.tpl
--rw-r--r--   0        0        0      675 2024-05-23 23:05:25.768638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/cli/new/templates/app/pyproject.pytorch.toml.tpl
--rw-r--r--   0        0        0      655 2024-05-23 23:05:25.768638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/cli/new/templates/app/pyproject.sklearn.toml.tpl
--rw-r--r--   0        0        0      654 2024-05-23 23:05:25.768638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/cli/new/templates/app/pyproject.tensorflow.toml.tpl
--rw-r--r--   0        0        0      789 2024-05-23 23:05:25.768638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/cli/run/__init__.py
--rw-r--r--   0        0        0     2687 2024-05-23 23:05:25.768638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/cli/run/run.py
--rw-r--r--   0        0        0     4119 2024-05-23 23:05:25.768638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/cli/utils.py
--rw-r--r--   0        0        0     1268 2024-05-23 23:05:25.768638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/client/__init__.py
--rw-r--r--   0        0        0    22313 2024-05-23 23:05:25.768638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/client/app.py
--rw-r--r--   0        0        0     8183 2024-05-23 23:05:25.768638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/client/client.py
--rw-r--r--   0        0        0     8636 2024-05-23 23:05:25.768638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/client/client_app.py
--rw-r--r--   0        0        0     7435 2024-05-23 23:05:25.768638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/client/dpfedavg_numpy_client.py
--rw-r--r--   0        0        0      735 2024-05-23 23:05:25.768638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/client/grpc_client/__init__.py
--rw-r--r--   0        0        0     8993 2024-05-23 23:05:25.768638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/client/grpc_client/connection.py
--rw-r--r--   0        0        0      752 2024-05-23 23:05:25.768638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/client/grpc_rere_client/__init__.py
--rw-r--r--   0        0        0     4903 2024-05-23 23:05:25.768638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/client/grpc_rere_client/client_interceptor.py
--rw-r--r--   0        0        0     9597 2024-05-23 23:05:25.768638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/client/grpc_rere_client/connection.py
--rw-r--r--   0        0        0     2404 2024-05-23 23:05:25.768638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/client/heartbeat.py
--rw-r--r--   0        0        0      719 2024-05-23 23:05:25.768638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/client/message_handler/__init__.py
--rw-r--r--   0        0        0     6553 2024-05-23 23:05:25.768638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/client/message_handler/message_handler.py
--rw-r--r--   0        0        0     1824 2024-05-23 23:05:25.768638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/client/message_handler/task_handler.py
--rw-r--r--   0        0        0     1143 2024-05-23 23:05:25.768638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/client/mod/__init__.py
--rw-r--r--   0        0        0     5415 2024-05-23 23:05:25.768638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/client/mod/centraldp_mods.py
--rw-r--r--   0        0        0     2624 2024-05-23 23:05:25.768638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/client/mod/comms_mods.py
--rw-r--r--   0        0        0     4982 2024-05-23 23:05:25.772638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/client/mod/localdp_mod.py
--rw-r--r--   0        0        0      849 2024-05-23 23:05:25.772638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/client/mod/secure_aggregation/__init__.py
--rw-r--r--   0        0        0     1095 2024-05-23 23:05:25.772638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/client/mod/secure_aggregation/secagg_mod.py
--rw-r--r--   0        0        0    19699 2024-05-23 23:05:25.772638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/client/mod/secure_aggregation/secaggplus_mod.py
--rw-r--r--   0        0        0     1226 2024-05-23 23:05:25.772638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/client/mod/utils.py
--rw-r--r--   0        0        0     1778 2024-05-23 23:05:25.772638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/client/node_state.py
--rw-r--r--   0        0        0     2195 2024-05-23 23:05:25.772638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/client/node_state_tests.py
--rw-r--r--   0        0        0    10283 2024-05-23 23:05:25.772638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/client/numpy_client.py
--rw-r--r--   0        0        0      735 2024-05-23 23:05:25.772638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/client/rest_client/__init__.py
--rw-r--r--   0        0        0    11520 2024-05-23 23:05:25.772638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/client/rest_client/connection.py
--rw-r--r--   0        0        0      865 2024-05-23 23:05:25.772638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/client/supernode/__init__.py
--rw-r--r--   0        0        0     9052 2024-05-23 23:05:25.772638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/client/supernode/app.py
--rw-r--r--   0        0        0     1006 2024-05-23 23:05:25.772638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/client/typing.py
--rw-r--r--   0        0        0     3721 2024-05-23 23:05:25.772638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/common/__init__.py
--rw-r--r--   0        0        0     1882 2024-05-23 23:05:25.772638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/common/address.py
--rw-r--r--   0        0        0     2424 2024-05-23 23:05:25.772638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/common/constant.py
--rw-r--r--   0        0        0     1313 2024-05-23 23:05:25.772638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/common/context.py
--rw-r--r--   0        0        0      891 2024-05-23 23:05:25.772638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/common/date.py
--rw-r--r--   0        0        0     6113 2024-05-23 23:05:25.772638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/common/differential_privacy.py
--rw-r--r--   0        0        0     1074 2024-05-23 23:05:25.772638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/common/differential_privacy_constants.py
--rw-r--r--   0        0        0     2004 2024-05-23 23:05:25.772638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/common/dp.py
--rw-r--r--   0        0        0     2812 2024-05-23 23:05:25.772638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/common/exit_handlers.py
--rw-r--r--   0        0        0     2460 2024-05-23 23:05:25.772638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/common/grpc.py
--rw-r--r--   0        0        0     7107 2024-05-23 23:05:25.772638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/common/logger.py
--rw-r--r--   0        0        0    13896 2024-05-23 23:05:25.772638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/common/message.py
--rw-r--r--   0        0        0     4961 2024-05-23 23:05:25.772638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/common/object_ref.py
--rw-r--r--   0        0        0     2095 2024-05-23 23:05:25.772638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/common/parameter.py
--rw-r--r--   0        0        0     1385 2024-05-23 23:05:25.772638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/common/pyproject.py
--rw-r--r--   0        0        0     1054 2024-05-23 23:05:25.772638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/common/record/__init__.py
--rw-r--r--   0        0        0     4652 2024-05-23 23:05:25.772638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/common/record/configsrecord.py
--rw-r--r--   0        0        0     1393 2024-05-23 23:05:25.772638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/common/record/conversion_utils.py
--rw-r--r--   0        0        0     3923 2024-05-23 23:05:25.772638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/common/record/metricsrecord.py
--rw-r--r--   0        0        0     4838 2024-05-23 23:05:25.772638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/common/record/parametersrecord.py
--rw-r--r--   0        0        0     5056 2024-05-23 23:05:25.772638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/common/record/recordset.py
--rw-r--r--   0        0        0     3879 2024-05-23 23:05:25.772638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/common/record/typeddict.py
--rw-r--r--   0        0        0    13798 2024-05-23 23:05:25.772638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/common/recordset_compat.py
--rw-r--r--   0        0        0    11707 2024-05-23 23:05:25.772638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/common/retry_invoker.py
--rw-r--r--   0        0        0      731 2024-05-23 23:05:25.772638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/common/secure_aggregation/__init__.py
--rw-r--r--   0        0        0      738 2024-05-23 23:05:25.772638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/common/secure_aggregation/crypto/__init__.py
--rw-r--r--   0        0        0     2792 2024-05-23 23:05:25.772638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/common/secure_aggregation/crypto/shamir.py
--rw-r--r--   0        0        0     4707 2024-05-23 23:05:25.772638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/common/secure_aggregation/crypto/symmetric_encryption.py
--rw-r--r--   0        0        0     3026 2024-05-23 23:05:25.772638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/common/secure_aggregation/ndarrays_arithmetic.py
--rw-r--r--   0        0        0     2310 2024-05-23 23:05:25.772638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/common/secure_aggregation/quantization.py
--rw-r--r--   0        0        0     2183 2024-05-23 23:05:25.772638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/common/secure_aggregation/secaggplus_constants.py
--rw-r--r--   0        0        0     3221 2024-05-23 23:05:25.772638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/common/secure_aggregation/secaggplus_utils.py
--rw-r--r--   0        0        0    22250 2024-05-23 23:05:25.772638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/common/serde.py
--rw-r--r--   0        0        0     7865 2024-05-23 23:05:25.772638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/common/telemetry.py
--rw-r--r--   0        0        0     4382 2024-05-23 23:05:25.772638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/common/typing.py
--rw-r--r--   0        0        0      666 2024-05-23 23:05:25.772638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/common/version.py
--rw-r--r--   0        0        0      683 2024-05-23 23:05:25.772638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/proto/__init__.py
--rw-r--r--   0        0        0     3207 2024-05-23 23:05:25.772638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/proto/driver_pb2.py
--rw-r--r--   0        0        0     5016 2024-05-23 23:05:25.772638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/proto/driver_pb2.pyi
--rw-r--r--   0        0        0     7304 2024-05-23 23:05:25.772638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/proto/driver_pb2_grpc.py
--rw-r--r--   0        0        0     2022 2024-05-23 23:05:25.776638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/proto/driver_pb2_grpc.pyi
--rw-r--r--   0        0        0     1084 2024-05-23 23:05:25.776638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/proto/error_pb2.py
--rw-r--r--   0        0        0      734 2024-05-23 23:05:25.776638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/proto/error_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-23 23:05:25.776638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/proto/error_pb2_grpc.py
--rw-r--r--   0        0        0       76 2024-05-23 23:05:25.776638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/proto/error_pb2_grpc.pyi
--rw-r--r--   0        0        0     5018 2024-05-23 23:05:25.776638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/proto/fleet_pb2.py
--rw-r--r--   0        0        0     9161 2024-05-23 23:05:25.776638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/proto/fleet_pb2.pyi
--rw-r--r--   0        0        0    10605 2024-05-23 23:05:25.776638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/proto/fleet_pb2_grpc.py
--rw-r--r--   0        0        0     2811 2024-05-23 23:05:25.776638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/proto/fleet_pb2_grpc.pyi
--rw-r--r--   0        0        0     1081 2024-05-23 23:05:25.776638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/proto/node_pb2.py
--rw-r--r--   0        0        0      751 2024-05-23 23:05:25.776638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/proto/node_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-23 23:05:25.776638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/proto/node_pb2_grpc.py
--rw-r--r--   0        0        0       76 2024-05-23 23:05:25.776638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/proto/node_pb2_grpc.pyi
--rw-r--r--   0        0        0     6009 2024-05-23 23:05:25.776638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/proto/recordset_pb2.py
--rw-r--r--   0        0        0    14161 2024-05-23 23:05:25.776638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/proto/recordset_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-23 23:05:25.776638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/proto/recordset_pb2_grpc.py
--rw-r--r--   0        0        0       76 2024-05-23 23:05:25.776638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/proto/recordset_pb2_grpc.pyi
--rw-r--r--   0        0        0     2472 2024-05-23 23:05:25.776638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/proto/task_pb2.py
--rw-r--r--   0        0        0     4320 2024-05-23 23:05:25.776638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/proto/task_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-23 23:05:25.776638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/proto/task_pb2_grpc.py
--rw-r--r--   0        0        0       76 2024-05-23 23:05:25.776638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/proto/task_pb2_grpc.pyi
--rw-r--r--   0        0        0     9781 2024-05-23 23:05:25.776638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/proto/transport_pb2.py
--rw-r--r--   0        0        0    21497 2024-05-23 23:05:25.776638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/proto/transport_pb2.pyi
--rw-r--r--   0        0        0     2598 2024-05-23 23:05:25.776638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/proto/transport_pb2_grpc.py
--rw-r--r--   0        0        0      766 2024-05-23 23:05:25.776638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/proto/transport_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2024-05-23 23:05:25.776638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/py.typed
--rw-r--r--   0        0        0     1716 2024-05-23 23:05:25.776638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/__init__.py
--rw-r--r--   0        0        0    28913 2024-05-23 23:05:25.776638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/app.py
--rw-r--r--   0        0        0     6127 2024-05-23 23:05:25.776638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/client_manager.py
--rw-r--r--   0        0        0     2399 2024-05-23 23:05:25.776638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/client_proxy.py
--rw-r--r--   0        0        0      892 2024-05-23 23:05:25.776638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/compat/__init__.py
--rw-r--r--   0        0        0     3421 2024-05-23 23:05:25.776638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/compat/app.py
--rw-r--r--   0        0        0     3468 2024-05-23 23:05:25.776638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/compat/app_utils.py
--rw-r--r--   0        0        0     5444 2024-05-23 23:05:25.776638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/compat/driver_client_proxy.py
--rw-r--r--   0        0        0     1766 2024-05-23 23:05:25.776638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/compat/legacy_context.py
--rw-r--r--   0        0        0     1061 2024-05-23 23:05:25.776638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/criterion.py
--rw-r--r--   0        0        0      886 2024-05-23 23:05:25.776638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/driver/__init__.py
--rw-r--r--   0        0        0     5090 2024-05-23 23:05:25.776638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/driver/driver.py
--rw-r--r--   0        0        0    11832 2024-05-23 23:05:25.776638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/driver/grpc_driver.py
--rw-r--r--   0        0        0     6490 2024-05-23 23:05:25.776638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/driver/inmemory_driver.py
--rw-r--r--   0        0        0     5063 2024-05-23 23:05:25.776638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/history.py
--rw-r--r--   0        0        0     5972 2024-05-23 23:05:25.776638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/run_serverapp.py
--rw-r--r--   0        0        0    17821 2024-05-23 23:05:25.776638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/server.py
--rw-r--r--   0        0        0     4402 2024-05-23 23:05:25.776638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/server_app.py
--rw-r--r--   0        0        0     1349 2024-05-23 23:05:25.776638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/server_config.py
--rw-r--r--   0        0        0     2836 2024-05-23 23:05:25.776638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/strategy/__init__.py
--rw-r--r--   0        0        0    13468 2024-05-23 23:05:25.776638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/strategy/aggregate.py
--rw-r--r--   0        0        0     6532 2024-05-23 23:05:25.776638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/strategy/bulyan.py
--rw-r--r--   0        0        0    17406 2024-05-23 23:05:25.776638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/strategy/dp_adaptive_clipping.py
--rw-r--r--   0        0        0    12853 2024-05-23 23:05:25.776638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/strategy/dp_fixed_clipping.py
--rw-r--r--   0        0        0     4877 2024-05-23 23:05:25.776638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/strategy/dpfedavg_adaptive.py
--rw-r--r--   0        0        0     7219 2024-05-23 23:05:25.776638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/strategy/dpfedavg_fixed.py
--rw-r--r--   0        0        0     5900 2024-05-23 23:05:25.776638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/strategy/fault_tolerant_fedavg.py
--rw-r--r--   0        0        0     6505 2024-05-23 23:05:25.776638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/strategy/fedadagrad.py
--rw-r--r--   0        0        0     6763 2024-05-23 23:05:25.776638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/strategy/fedadam.py
--rw-r--r--   0        0        0    11799 2024-05-23 23:05:25.776638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/strategy/fedavg.py
--rw-r--r--   0        0        0     9784 2024-05-23 23:05:25.776638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/strategy/fedavg_android.py
--rw-r--r--   0        0        0     8132 2024-05-23 23:05:25.776638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/strategy/fedavgm.py
--rw-r--r--   0        0        0     2704 2024-05-23 23:05:25.776638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/strategy/fedmedian.py
--rw-r--r--   0        0        0     5242 2024-05-23 23:05:25.776638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/strategy/fedopt.py
--rw-r--r--   0        0        0     6862 2024-05-23 23:05:25.776638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/strategy/fedprox.py
--rw-r--r--   0        0        0     5890 2024-05-23 23:05:25.776638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/strategy/fedtrimmedavg.py
--rw-r--r--   0        0        0     6080 2024-05-23 23:05:25.776638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/strategy/fedxgb_bagging.py
--rw-r--r--   0        0        0     5607 2024-05-23 23:05:25.776638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/strategy/fedxgb_cyclic.py
--rw-r--r--   0        0        0     4047 2024-05-23 23:05:25.776638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/strategy/fedxgb_nn_avg.py
--rw-r--r--   0        0        0     6801 2024-05-23 23:05:25.776638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/strategy/fedyogi.py
--rw-r--r--   0        0        0     6285 2024-05-23 23:05:25.780638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/strategy/krum.py
--rw-r--r--   0        0        0    10150 2024-05-23 23:05:25.780638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/strategy/qfedavg.py
--rw-r--r--   0        0        0     7543 2024-05-23 23:05:25.780638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/strategy/strategy.py
--rw-r--r--   0        0        0      707 2024-05-23 23:05:25.780638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/superlink/__init__.py
--rw-r--r--   0        0        0      712 2024-05-23 23:05:25.780638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/superlink/driver/__init__.py
--rw-r--r--   0        0        0     1932 2024-05-23 23:05:25.780638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/superlink/driver/driver_grpc.py
--rw-r--r--   0        0        0     4791 2024-05-23 23:05:25.780638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/superlink/driver/driver_servicer.py
--rw-r--r--   0        0        0      711 2024-05-23 23:05:25.780638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/superlink/fleet/__init__.py
--rw-r--r--   0        0        0      735 2024-05-23 23:05:25.780638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/superlink/fleet/grpc_bidi/__init__.py
--rw-r--r--   0        0        0     5993 2024-05-23 23:05:25.780638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/superlink/fleet/grpc_bidi/flower_service_servicer.py
--rw-r--r--   0        0        0     6458 2024-05-23 23:05:25.780638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_bridge.py
--rw-r--r--   0        0        0     4887 2024-05-23 23:05:25.780638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_client_proxy.py
--rw-r--r--   0        0        0    11932 2024-05-23 23:05:25.780638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_server.py
--rw-r--r--   0        0        0      758 2024-05-23 23:05:25.780638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/superlink/fleet/grpc_rere/__init__.py
--rw-r--r--   0        0        0     3387 2024-05-23 23:05:25.780638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/superlink/fleet/grpc_rere/fleet_servicer.py
--rw-r--r--   0        0        0     7691 2024-05-23 23:05:25.780638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/superlink/fleet/grpc_rere/server_interceptor.py
--rw-r--r--   0        0        0      731 2024-05-23 23:05:25.780638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/superlink/fleet/message_handler/__init__.py
--rw-r--r--   0        0        0     3622 2024-05-23 23:05:25.780638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/superlink/fleet/message_handler/message_handler.py
--rw-r--r--   0        0        0      735 2024-05-23 23:05:25.780638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/superlink/fleet/rest_rere/__init__.py
--rw-r--r--   0        0        0     7621 2024-05-23 23:05:25.780638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/superlink/fleet/rest_rere/rest_api.py
--rw-r--r--   0        0        0      783 2024-05-23 23:05:25.780638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/superlink/fleet/vce/__init__.py
--rw-r--r--   0        0        0     1466 2024-05-23 23:05:25.780638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/superlink/fleet/vce/backend/__init__.py
--rw-r--r--   0        0        0     2260 2024-05-23 23:05:25.780638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/superlink/fleet/vce/backend/backend.py
--rw-r--r--   0        0        0     6722 2024-05-23 23:05:25.780638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/superlink/fleet/vce/backend/raybackend.py
--rw-r--r--   0        0        0    12456 2024-05-23 23:05:25.780638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/superlink/fleet/vce/vce_api.py
--rw-r--r--   0        0        0     1003 2024-05-23 23:05:25.780638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/superlink/state/__init__.py
--rw-r--r--   0        0        0    12750 2024-05-23 23:05:25.780638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/superlink/state/in_memory_state.py
--rw-r--r--   0        0        0    28528 2024-05-23 23:05:25.780638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/superlink/state/sqlite_state.py
--rw-r--r--   0        0        0     7989 2024-05-23 23:05:25.780638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/superlink/state/state.py
--rw-r--r--   0        0        0     1654 2024-05-23 23:05:25.780638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/superlink/state/state_factory.py
--rw-r--r--   0        0        0     2207 2024-05-23 23:05:25.780638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/superlink/state/utils.py
--rw-r--r--   0        0        0      913 2024-05-23 23:05:25.780638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/typing.py
--rw-r--r--   0        0        0      908 2024-05-23 23:05:25.780638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/utils/__init__.py
--rw-r--r--   0        0        0     5485 2024-05-23 23:05:25.780638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/utils/tensorboard.py
--rw-r--r--   0        0        0     5301 2024-05-23 23:05:25.780638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/utils/validator.py
--rw-r--r--   0        0        0      902 2024-05-23 23:05:25.780638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/workflow/__init__.py
--rw-r--r--   0        0        0     1082 2024-05-23 23:05:25.780638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/workflow/constant.py
--rw-r--r--   0        0        0    14003 2024-05-23 23:05:25.780638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/workflow/default_workflows.py
--rw-r--r--   0        0        0      880 2024-05-23 23:05:25.780638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/workflow/secure_aggregation/__init__.py
--rw-r--r--   0        0        0     5838 2024-05-23 23:05:25.780638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/workflow/secure_aggregation/secagg_workflow.py
--rw-r--r--   0        0        0    29038 2024-05-23 23:05:25.780638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/workflow/secure_aggregation/secaggplus_workflow.py
--rw-r--r--   0        0        0     1348 2024-05-23 23:05:25.780638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/simulation/__init__.py
--rw-r--r--   0        0        0    14380 2024-05-23 23:05:25.780638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/simulation/app.py
--rw-r--r--   0        0        0      734 2024-05-23 23:05:25.780638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/simulation/ray_transport/__init__.py
--rw-r--r--   0        0        0    19367 2024-05-23 23:05:25.780638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/simulation/ray_transport/ray_actor.py
--rw-r--r--   0        0        0     6738 2024-05-23 23:05:25.780638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/simulation/ray_transport/ray_client_proxy.py
--rw-r--r--   0        0        0     2392 2024-05-23 23:05:25.780638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/simulation/ray_transport/utils.py
--rw-r--r--   0        0        0    15098 2024-05-23 23:05:25.780638 flwr_nightly-1.9.0.dev20240523/src/py/flwr/simulation/run_simulation.py
--rw-r--r--   0        0        0    15434 1970-01-01 00:00:00.000000 flwr_nightly-1.9.0.dev20240523/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-05-24 23:05:22.683554 flwr_nightly-1.9.0.dev20240524/LICENSE
+-rw-r--r--   0        0        0    13010 2024-05-24 23:05:22.683554 flwr_nightly-1.9.0.dev20240524/README.md
+-rw-r--r--   0        0        0     5813 2024-05-24 23:05:41.599603 flwr_nightly-1.9.0.dev20240524/pyproject.toml
+-rw-r--r--   0        0        0      937 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/__init__.py
+-rw-r--r--   0        0        0      720 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/__init__.py
+-rw-r--r--   0        0        0     1141 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/app.py
+-rw-r--r--   0        0        0     5064 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/build.py
+-rw-r--r--   0        0        0     4277 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/config_utils.py
+-rw-r--r--   0        0        0     2215 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/example.py
+-rw-r--r--   0        0        0      789 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/__init__.py
+-rw-r--r--   0        0        0     6223 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/new.py
+-rw-r--r--   0        0        0      725 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/__init__.py
+-rw-r--r--   0        0        0     3078 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/.gitignore.tpl
+-rw-r--r--   0        0        0      668 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/README.md.tpl
+-rw-r--r--   0        0        0      729 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/__init__.py
+-rw-r--r--   0        0        0      736 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/code/__init__.py
+-rw-r--r--   0        0        0       21 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/code/__init__.py.tpl
+-rw-r--r--   0        0        0     1450 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/code/client.hf.py.tpl
+-rw-r--r--   0        0        0     1434 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/code/client.jax.py.tpl
+-rw-r--r--   0        0        0     2113 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/code/client.mlx.py.tpl
+-rw-r--r--   0        0        0      521 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/code/client.numpy.py.tpl
+-rw-r--r--   0        0        0     1172 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/code/client.pytorch.py.tpl
+-rw-r--r--   0        0        0     2801 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/code/client.sklearn.py.tpl
+-rw-r--r--   0        0        0     1280 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/code/client.tensorflow.py.tpl
+-rw-r--r--   0        0        0      338 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/code/server.hf.py.tpl
+-rw-r--r--   0        0        0      246 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/code/server.jax.py.tpl
+-rw-r--r--   0        0        0      272 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/code/server.mlx.py.tpl
+-rw-r--r--   0        0        0      248 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/code/server.numpy.py.tpl
+-rw-r--r--   0        0        0      593 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/code/server.pytorch.py.tpl
+-rw-r--r--   0        0        0      341 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/code/server.sklearn.py.tpl
+-rw-r--r--   0        0        0      579 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/code/server.tensorflow.py.tpl
+-rw-r--r--   0        0        0     2857 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/code/task.hf.py.tpl
+-rw-r--r--   0        0        0     1519 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/code/task.jax.py.tpl
+-rw-r--r--   0        0        0     2598 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/code/task.mlx.py.tpl
+-rw-r--r--   0        0        0     3684 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/code/task.pytorch.py.tpl
+-rw-r--r--   0        0        0     1044 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/code/task.tensorflow.py.tpl
+-rw-r--r--   0        0        0      759 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/pyproject.hf.toml.tpl
+-rw-r--r--   0        0        0      568 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/pyproject.jax.toml.tpl
+-rw-r--r--   0        0        0      668 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/pyproject.mlx.toml.tpl
+-rw-r--r--   0        0        0      606 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/pyproject.numpy.toml.tpl
+-rw-r--r--   0        0        0      675 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/pyproject.pytorch.toml.tpl
+-rw-r--r--   0        0        0      655 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/pyproject.sklearn.toml.tpl
+-rw-r--r--   0        0        0      654 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/pyproject.tensorflow.toml.tpl
+-rw-r--r--   0        0        0      789 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/run/__init__.py
+-rw-r--r--   0        0        0     2687 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/run/run.py
+-rw-r--r--   0        0        0     4119 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/utils.py
+-rw-r--r--   0        0        0     1268 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/__init__.py
+-rw-r--r--   0        0        0    22313 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/app.py
+-rw-r--r--   0        0        0     8183 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/client.py
+-rw-r--r--   0        0        0     8636 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/client_app.py
+-rw-r--r--   0        0        0     7435 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/dpfedavg_numpy_client.py
+-rw-r--r--   0        0        0      735 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/grpc_client/__init__.py
+-rw-r--r--   0        0        0     8993 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/grpc_client/connection.py
+-rw-r--r--   0        0        0      752 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/grpc_rere_client/__init__.py
+-rw-r--r--   0        0        0     4903 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/grpc_rere_client/client_interceptor.py
+-rw-r--r--   0        0        0     9597 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/grpc_rere_client/connection.py
+-rw-r--r--   0        0        0     2404 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/heartbeat.py
+-rw-r--r--   0        0        0      719 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/message_handler/__init__.py
+-rw-r--r--   0        0        0     6553 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/message_handler/message_handler.py
+-rw-r--r--   0        0        0     1824 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/message_handler/task_handler.py
+-rw-r--r--   0        0        0     1143 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/mod/__init__.py
+-rw-r--r--   0        0        0     5415 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/mod/centraldp_mods.py
+-rw-r--r--   0        0        0     2624 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/mod/comms_mods.py
+-rw-r--r--   0        0        0     4982 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/mod/localdp_mod.py
+-rw-r--r--   0        0        0      849 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/mod/secure_aggregation/__init__.py
+-rw-r--r--   0        0        0     1095 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/mod/secure_aggregation/secagg_mod.py
+-rw-r--r--   0        0        0    19699 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/mod/secure_aggregation/secaggplus_mod.py
+-rw-r--r--   0        0        0     1226 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/mod/utils.py
+-rw-r--r--   0        0        0     1778 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/node_state.py
+-rw-r--r--   0        0        0     2195 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/node_state_tests.py
+-rw-r--r--   0        0        0    10283 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/numpy_client.py
+-rw-r--r--   0        0        0      735 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/rest_client/__init__.py
+-rw-r--r--   0        0        0    11520 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/rest_client/connection.py
+-rw-r--r--   0        0        0      865 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/supernode/__init__.py
+-rw-r--r--   0        0        0     9915 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/supernode/app.py
+-rw-r--r--   0        0        0     1006 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/typing.py
+-rw-r--r--   0        0        0     3721 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/__init__.py
+-rw-r--r--   0        0        0     1882 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/address.py
+-rw-r--r--   0        0        0     2424 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/constant.py
+-rw-r--r--   0        0        0     1313 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/context.py
+-rw-r--r--   0        0        0      891 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/date.py
+-rw-r--r--   0        0        0     6113 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/differential_privacy.py
+-rw-r--r--   0        0        0     1074 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/differential_privacy_constants.py
+-rw-r--r--   0        0        0     2004 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/dp.py
+-rw-r--r--   0        0        0     2812 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/exit_handlers.py
+-rw-r--r--   0        0        0     2460 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/grpc.py
+-rw-r--r--   0        0        0     7107 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/logger.py
+-rw-r--r--   0        0        0    13896 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/message.py
+-rw-r--r--   0        0        0     4961 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/object_ref.py
+-rw-r--r--   0        0        0     2095 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/parameter.py
+-rw-r--r--   0        0        0     1385 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/pyproject.py
+-rw-r--r--   0        0        0     1054 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/record/__init__.py
+-rw-r--r--   0        0        0     4652 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/record/configsrecord.py
+-rw-r--r--   0        0        0     1393 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/record/conversion_utils.py
+-rw-r--r--   0        0        0     3923 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/record/metricsrecord.py
+-rw-r--r--   0        0        0     4838 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/record/parametersrecord.py
+-rw-r--r--   0        0        0     5056 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/record/recordset.py
+-rw-r--r--   0        0        0     3879 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/record/typeddict.py
+-rw-r--r--   0        0        0    14009 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/recordset_compat.py
+-rw-r--r--   0        0        0    11707 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/retry_invoker.py
+-rw-r--r--   0        0        0      731 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/secure_aggregation/__init__.py
+-rw-r--r--   0        0        0      738 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/secure_aggregation/crypto/__init__.py
+-rw-r--r--   0        0        0     2792 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/secure_aggregation/crypto/shamir.py
+-rw-r--r--   0        0        0     4173 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/secure_aggregation/crypto/symmetric_encryption.py
+-rw-r--r--   0        0        0     3026 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/secure_aggregation/ndarrays_arithmetic.py
+-rw-r--r--   0        0        0     2310 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/secure_aggregation/quantization.py
+-rw-r--r--   0        0        0     2183 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/secure_aggregation/secaggplus_constants.py
+-rw-r--r--   0        0        0     3221 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/secure_aggregation/secaggplus_utils.py
+-rw-r--r--   0        0        0    22250 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/serde.py
+-rw-r--r--   0        0        0     7865 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/telemetry.py
+-rw-r--r--   0        0        0     4382 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/typing.py
+-rw-r--r--   0        0        0      666 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/version.py
+-rw-r--r--   0        0        0      683 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/__init__.py
+-rw-r--r--   0        0        0     3207 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/driver_pb2.py
+-rw-r--r--   0        0        0     5016 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/driver_pb2.pyi
+-rw-r--r--   0        0        0     7304 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/driver_pb2_grpc.py
+-rw-r--r--   0        0        0     2022 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/driver_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1084 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/error_pb2.py
+-rw-r--r--   0        0        0      734 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/error_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/error_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/error_pb2_grpc.pyi
+-rw-r--r--   0        0        0     5018 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/fleet_pb2.py
+-rw-r--r--   0        0        0     9161 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/fleet_pb2.pyi
+-rw-r--r--   0        0        0    10605 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/fleet_pb2_grpc.py
+-rw-r--r--   0        0        0     2811 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/fleet_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1081 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/node_pb2.py
+-rw-r--r--   0        0        0      751 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/node_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/node_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/node_pb2_grpc.pyi
+-rw-r--r--   0        0        0     6009 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/recordset_pb2.py
+-rw-r--r--   0        0        0    14161 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/recordset_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/recordset_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/recordset_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2472 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/task_pb2.py
+-rw-r--r--   0        0        0     4320 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/task_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/task_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/task_pb2_grpc.pyi
+-rw-r--r--   0        0        0     9781 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/transport_pb2.py
+-rw-r--r--   0        0        0    21497 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/transport_pb2.pyi
+-rw-r--r--   0        0        0     2598 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/transport_pb2_grpc.py
+-rw-r--r--   0        0        0      766 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/transport_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/py.typed
+-rw-r--r--   0        0        0     1716 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/__init__.py
+-rw-r--r--   0        0        0    29973 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/app.py
+-rw-r--r--   0        0        0     6127 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/client_manager.py
+-rw-r--r--   0        0        0     2399 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/client_proxy.py
+-rw-r--r--   0        0        0      892 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/compat/__init__.py
+-rw-r--r--   0        0        0     3421 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/compat/app.py
+-rw-r--r--   0        0        0     3468 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/compat/app_utils.py
+-rw-r--r--   0        0        0     5444 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/compat/driver_client_proxy.py
+-rw-r--r--   0        0        0     1766 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/compat/legacy_context.py
+-rw-r--r--   0        0        0     1061 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/criterion.py
+-rw-r--r--   0        0        0      886 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/driver/__init__.py
+-rw-r--r--   0        0        0     5090 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/driver/driver.py
+-rw-r--r--   0        0        0    11832 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/driver/grpc_driver.py
+-rw-r--r--   0        0        0     6490 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/driver/inmemory_driver.py
+-rw-r--r--   0        0        0     5063 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/history.py
+-rw-r--r--   0        0        0     5972 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/run_serverapp.py
+-rw-r--r--   0        0        0    17821 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/server.py
+-rw-r--r--   0        0        0     4402 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/server_app.py
+-rw-r--r--   0        0        0     1349 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/server_config.py
+-rw-r--r--   0        0        0     2836 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/__init__.py
+-rw-r--r--   0        0        0    13468 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/aggregate.py
+-rw-r--r--   0        0        0     6532 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/bulyan.py
+-rw-r--r--   0        0        0    17406 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/dp_adaptive_clipping.py
+-rw-r--r--   0        0        0    12853 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/dp_fixed_clipping.py
+-rw-r--r--   0        0        0     4877 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/dpfedavg_adaptive.py
+-rw-r--r--   0        0        0     7219 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/dpfedavg_fixed.py
+-rw-r--r--   0        0        0     5900 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/fault_tolerant_fedavg.py
+-rw-r--r--   0        0        0     6505 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/fedadagrad.py
+-rw-r--r--   0        0        0     6763 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/fedadam.py
+-rw-r--r--   0        0        0    11799 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/fedavg.py
+-rw-r--r--   0        0        0     9784 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/fedavg_android.py
+-rw-r--r--   0        0        0     8132 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/fedavgm.py
+-rw-r--r--   0        0        0     2704 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/fedmedian.py
+-rw-r--r--   0        0        0     5242 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/fedopt.py
+-rw-r--r--   0        0        0     6862 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/fedprox.py
+-rw-r--r--   0        0        0     5890 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/fedtrimmedavg.py
+-rw-r--r--   0        0        0     6080 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/fedxgb_bagging.py
+-rw-r--r--   0        0        0     5607 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/fedxgb_cyclic.py
+-rw-r--r--   0        0        0     4047 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/fedxgb_nn_avg.py
+-rw-r--r--   0        0        0     6801 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/fedyogi.py
+-rw-r--r--   0        0        0     6285 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/krum.py
+-rw-r--r--   0        0        0    10150 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/qfedavg.py
+-rw-r--r--   0        0        0     7543 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/strategy.py
+-rw-r--r--   0        0        0      707 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/__init__.py
+-rw-r--r--   0        0        0      712 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/driver/__init__.py
+-rw-r--r--   0        0        0     1932 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/driver/driver_grpc.py
+-rw-r--r--   0        0        0     4791 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/driver/driver_servicer.py
+-rw-r--r--   0        0        0      711 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/fleet/__init__.py
+-rw-r--r--   0        0        0      735 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/fleet/grpc_bidi/__init__.py
+-rw-r--r--   0        0        0     5993 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/fleet/grpc_bidi/flower_service_servicer.py
+-rw-r--r--   0        0        0     6458 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_bridge.py
+-rw-r--r--   0        0        0     4887 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_client_proxy.py
+-rw-r--r--   0        0        0    11932 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_server.py
+-rw-r--r--   0        0        0      758 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/fleet/grpc_rere/__init__.py
+-rw-r--r--   0        0        0     3387 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/fleet/grpc_rere/fleet_servicer.py
+-rw-r--r--   0        0        0     7691 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/fleet/grpc_rere/server_interceptor.py
+-rw-r--r--   0        0        0      731 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/fleet/message_handler/__init__.py
+-rw-r--r--   0        0        0     3622 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/fleet/message_handler/message_handler.py
+-rw-r--r--   0        0        0      735 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/fleet/rest_rere/__init__.py
+-rw-r--r--   0        0        0     7621 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/fleet/rest_rere/rest_api.py
+-rw-r--r--   0        0        0      783 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/fleet/vce/__init__.py
+-rw-r--r--   0        0        0     1466 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/fleet/vce/backend/__init__.py
+-rw-r--r--   0        0        0     2260 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/fleet/vce/backend/backend.py
+-rw-r--r--   0        0        0     6722 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/fleet/vce/backend/raybackend.py
+-rw-r--r--   0        0        0    12456 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/fleet/vce/vce_api.py
+-rw-r--r--   0        0        0     1003 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/state/__init__.py
+-rw-r--r--   0        0        0    12750 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/state/in_memory_state.py
+-rw-r--r--   0        0        0    28528 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/state/sqlite_state.py
+-rw-r--r--   0        0        0     7989 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/state/state.py
+-rw-r--r--   0        0        0     1654 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/state/state_factory.py
+-rw-r--r--   0        0        0     2207 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/state/utils.py
+-rw-r--r--   0        0        0      913 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/typing.py
+-rw-r--r--   0        0        0      908 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/utils/__init__.py
+-rw-r--r--   0        0        0     5485 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/utils/tensorboard.py
+-rw-r--r--   0        0        0     5301 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/utils/validator.py
+-rw-r--r--   0        0        0      902 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/workflow/__init__.py
+-rw-r--r--   0        0        0     1082 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/workflow/constant.py
+-rw-r--r--   0        0        0    14003 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/workflow/default_workflows.py
+-rw-r--r--   0        0        0      880 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/workflow/secure_aggregation/__init__.py
+-rw-r--r--   0        0        0     5838 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/workflow/secure_aggregation/secagg_workflow.py
+-rw-r--r--   0        0        0    29038 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/workflow/secure_aggregation/secaggplus_workflow.py
+-rw-r--r--   0        0        0     1348 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/simulation/__init__.py
+-rw-r--r--   0        0        0    14380 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/simulation/app.py
+-rw-r--r--   0        0        0      734 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/simulation/ray_transport/__init__.py
+-rw-r--r--   0        0        0    19367 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/simulation/ray_transport/ray_actor.py
+-rw-r--r--   0        0        0     6738 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/simulation/ray_transport/ray_client_proxy.py
+-rw-r--r--   0        0        0     2392 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/simulation/ray_transport/utils.py
+-rw-r--r--   0        0        0    15098 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/simulation/run_simulation.py
+-rw-r--r--   0        0        0    15398 1970-01-01 00:00:00.000000 flwr_nightly-1.9.0.dev20240524/PKG-INFO
```

### Comparing `flwr_nightly-1.9.0.dev20240523/LICENSE` & `flwr_nightly-1.9.0.dev20240524/LICENSE`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/README.md` & `flwr_nightly-1.9.0.dev20240524/README.md`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/pyproject.toml` & `flwr_nightly-1.9.0.dev20240524/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.4.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "flwr-nightly"
-version = "1.9.0.dev20240523"
+version = "1.9.0.dev20240524"
 description = "Flower: A Friendly Federated Learning Framework"
 license = "Apache-2.0"
 authors = ["The Flower Authors <hello@flower.ai>"]
 readme = "README.md"
 homepage = "https://flower.ai"
 repository = "https://github.com/adap/flower"
 documentation = "https://flower.ai"
@@ -69,17 +69,16 @@
 protobuf = "^4.25.2"
 cryptography = "^42.0.4"
 pycryptodome = "^3.18.0"
 iterators = "^0.0.2"
 typer = { version = "^0.9.0", extras=["all"] }
 tomli = "^2.0.1"
 pathspec = "^0.12.1"
-setuptools = "!=70.0.0"
 # Optional dependencies (Simulation Engine)
-ray = { version = "==2.6.3", optional = true, python = ">=3.8,<3.12" }
+ray = { version = "==2.10.0", optional = true, python = ">=3.8,<3.12" }
 # Optional dependencies (REST transport layer)
 requests = { version = "^2.31.0", optional = true }
 starlette = { version = "^0.31.0", optional = true }
 uvicorn = { version = "^0.23.0", extras = ["standard"], optional = true }
 
 [tool.poetry.extras]
 simulation = ["ray", "pydantic"]
```

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/__init__.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/cli/__init__.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/cli/app.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/cli/build.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/build.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/cli/config_utils.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/config_utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/cli/example.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/example.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/cli/new/__init__.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/cli/new/new.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/new.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/cli/new/templates/__init__.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/cli/new/templates/app/.gitignore.tpl` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/.gitignore.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/cli/new/templates/app/README.md.tpl` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/README.md.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/cli/new/templates/app/__init__.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/cli/new/templates/app/code/__init__.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/code/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/cli/new/templates/app/code/client.hf.py.tpl` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/code/client.hf.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/cli/new/templates/app/code/client.jax.py.tpl` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/code/client.jax.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/cli/new/templates/app/code/client.mlx.py.tpl` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/code/client.mlx.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/cli/new/templates/app/code/client.numpy.py.tpl` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/code/client.numpy.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/cli/new/templates/app/code/client.pytorch.py.tpl` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/code/client.pytorch.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/cli/new/templates/app/code/client.sklearn.py.tpl` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/code/client.sklearn.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/cli/new/templates/app/code/client.tensorflow.py.tpl` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/code/client.tensorflow.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/cli/new/templates/app/code/server.pytorch.py.tpl` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/code/server.pytorch.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/cli/new/templates/app/code/server.tensorflow.py.tpl` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/code/server.tensorflow.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/cli/new/templates/app/code/task.hf.py.tpl` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/code/task.hf.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/cli/new/templates/app/code/task.jax.py.tpl` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/code/task.jax.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/cli/new/templates/app/code/task.mlx.py.tpl` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/code/task.mlx.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/cli/new/templates/app/code/task.pytorch.py.tpl` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/code/task.pytorch.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/cli/new/templates/app/code/task.tensorflow.py.tpl` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/code/task.tensorflow.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/cli/new/templates/app/pyproject.hf.toml.tpl` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/pyproject.hf.toml.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/cli/new/templates/app/pyproject.jax.toml.tpl` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/pyproject.jax.toml.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/cli/new/templates/app/pyproject.mlx.toml.tpl` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/pyproject.mlx.toml.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/cli/new/templates/app/pyproject.numpy.toml.tpl` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/pyproject.numpy.toml.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/cli/new/templates/app/pyproject.pytorch.toml.tpl` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/pyproject.pytorch.toml.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/cli/new/templates/app/pyproject.sklearn.toml.tpl` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/pyproject.sklearn.toml.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/cli/new/templates/app/pyproject.tensorflow.toml.tpl` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/pyproject.tensorflow.toml.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/cli/run/__init__.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/run/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/cli/run/run.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/run/run.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/cli/utils.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/client/__init__.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/client/app.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/client/client.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/client.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/client/client_app.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/client_app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/client/dpfedavg_numpy_client.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/dpfedavg_numpy_client.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/client/grpc_client/__init__.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/grpc_client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/client/grpc_client/connection.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/grpc_client/connection.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/client/grpc_rere_client/__init__.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/grpc_rere_client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/client/grpc_rere_client/client_interceptor.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/grpc_rere_client/client_interceptor.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/client/grpc_rere_client/connection.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/grpc_rere_client/connection.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/client/heartbeat.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/heartbeat.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/client/message_handler/__init__.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/message_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/client/message_handler/message_handler.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/message_handler/message_handler.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/client/message_handler/task_handler.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/message_handler/task_handler.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/client/mod/__init__.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/mod/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/client/mod/centraldp_mods.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/mod/centraldp_mods.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/client/mod/comms_mods.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/mod/comms_mods.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/client/mod/localdp_mod.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/mod/localdp_mod.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/client/mod/secure_aggregation/__init__.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/mod/secure_aggregation/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/client/mod/secure_aggregation/secagg_mod.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/mod/secure_aggregation/secagg_mod.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/client/mod/secure_aggregation/secaggplus_mod.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/mod/secure_aggregation/secaggplus_mod.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/client/mod/utils.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/mod/utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/client/node_state.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/node_state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/client/node_state_tests.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/node_state_tests.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/client/numpy_client.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/numpy_client.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/client/rest_client/__init__.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/rest_client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/client/rest_client/connection.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/rest_client/connection.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/client/supernode/__init__.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/supernode/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/client/supernode/app.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/supernode/app.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,28 +16,26 @@
 
 import argparse
 import sys
 from logging import DEBUG, INFO, WARN
 from pathlib import Path
 from typing import Callable, Optional, Tuple
 
+from cryptography.exceptions import UnsupportedAlgorithm
 from cryptography.hazmat.primitives.asymmetric import ec
 from cryptography.hazmat.primitives.serialization import (
     load_ssh_private_key,
     load_ssh_public_key,
 )
 
 from flwr.client.client_app import ClientApp, LoadClientAppError
 from flwr.common import EventType, event
 from flwr.common.exit_handlers import register_exit_handlers
 from flwr.common.logger import log
 from flwr.common.object_ref import load_app, validate
-from flwr.common.secure_aggregation.crypto.symmetric_encryption import (
-    ssh_types_to_elliptic_curve,
-)
 
 from ..app import _start_client_internal
 
 
 def run_supernode() -> None:
     """Run Flower SuperNode."""
     log(INFO, "Starting Flower SuperNode")
@@ -238,44 +236,64 @@
         "--dir",
         default="",
         help="Add specified directory to the PYTHONPATH and load Flower "
         "app from there."
         " Default: current working directory.",
     )
     parser.add_argument(
-        "--authentication-keys",
-        nargs=2,
-        metavar=("CLIENT_PRIVATE_KEY", "CLIENT_PUBLIC_KEY"),
+        "--auth-supernode-private-key",
+        type=str,
+        help="The SuperNode's private key (as a path str) to enable authentication.",
+    )
+    parser.add_argument(
+        "--auth-supernode-public-key",
         type=str,
-        help="Provide two file paths: (1) the client's private "
-        "key file, and (2) the client's public key file.",
+        help="The SuperNode's public key (as a path str) to enable authentication.",
     )
 
 
 def _try_setup_client_authentication(
     args: argparse.Namespace,
 ) -> Optional[Tuple[ec.EllipticCurvePrivateKey, ec.EllipticCurvePublicKey]]:
-    if not args.authentication_keys:
+    if not args.auth_supernode_private_key and not args.auth_supernode_public_key:
         return None
 
-    ssh_private_key = load_ssh_private_key(
-        Path(args.authentication_keys[0]).read_bytes(),
-        None,
-    )
-    ssh_public_key = load_ssh_public_key(Path(args.authentication_keys[1]).read_bytes())
+    if not args.auth_supernode_private_key or not args.auth_supernode_public_key:
+        sys.exit(
+            "Authentication requires file paths to both "
+            "'--auth-supernode-private-key' and '--auth-supernode-public-key'"
+            "to be provided (providing only one of them is not sufficient)."
+        )
+
+    try:
+        ssh_private_key = load_ssh_private_key(
+            Path(args.auth_supernode_private_key).read_bytes(),
+            None,
+        )
+        if not isinstance(ssh_private_key, ec.EllipticCurvePrivateKey):
+            raise ValueError()
+    except (ValueError, UnsupportedAlgorithm):
+        sys.exit(
+            "Error: Unable to parse the private key file in "
+            "'--auth-supernode-private-key'. Authentication requires elliptic "
+            "curve private and public key pair. Please ensure that the file "
+            "path points to a valid private key file and try again."
+        )
 
     try:
-        client_private_key, client_public_key = ssh_types_to_elliptic_curve(
-            ssh_private_key, ssh_public_key
+        ssh_public_key = load_ssh_public_key(
+            Path(args.auth_supernode_public_key).read_bytes()
         )
-    except TypeError:
+        if not isinstance(ssh_public_key, ec.EllipticCurvePublicKey):
+            raise ValueError()
+    except (ValueError, UnsupportedAlgorithm):
         sys.exit(
-            "The file paths provided could not be read as a private and public "
-            "key pair. Client authentication requires an elliptic curve public and "
-            "private key pair. Please provide the file paths containing elliptic "
-            "curve private and public keys to '--authentication-keys'."
+            "Error: Unable to parse the public key file in "
+            "'--auth-supernode-public-key'. Authentication requires elliptic "
+            "curve private and public key pair. Please ensure that the file "
+            "path points to a valid public key file and try again."
         )
 
     return (
-        client_private_key,
-        client_public_key,
+        ssh_private_key,
+        ssh_public_key,
     )
```

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/client/typing.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/typing.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/common/__init__.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/common/address.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/address.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/common/constant.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/constant.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/common/context.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/context.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/common/date.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/date.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/common/differential_privacy.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/differential_privacy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/common/differential_privacy_constants.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/differential_privacy_constants.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/common/dp.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/dp.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/common/exit_handlers.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/exit_handlers.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/common/grpc.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/common/logger.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/logger.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/common/message.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/message.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/common/object_ref.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/object_ref.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/common/parameter.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/parameter.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/common/pyproject.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/pyproject.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/common/record/__init__.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/record/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/common/record/configsrecord.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/record/configsrecord.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/common/record/conversion_utils.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/record/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/common/record/metricsrecord.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/record/metricsrecord.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/common/record/parametersrecord.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/record/parametersrecord.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/common/record/recordset.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/record/recordset.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/common/record/typeddict.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/record/typeddict.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/common/recordset_compat.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/recordset_compat.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,16 @@
     GetPropertiesRes,
     MetricsRecordValues,
     Parameters,
     Scalar,
     Status,
 )
 
+EMPTY_TENSOR_KEY = "_empty"
+
 
 def parametersrecord_to_parameters(
     record: ParametersRecord, keep_input: bool
 ) -> Parameters:
     """Convert ParameterRecord to legacy Parameters.
 
     Warnings
@@ -55,15 +57,16 @@
     keep_input : bool
         A boolean indicating whether entries in the record should be deleted from the
         input dictionary immediately after adding them to the record.
     """
     parameters = Parameters(tensors=[], tensor_type="")
 
     for key in list(record.keys()):
-        parameters.tensors.append(record[key].data)
+        if key != EMPTY_TENSOR_KEY:
+            parameters.tensors.append(record[key].data)
 
         if not parameters.tensor_type:
             # Setting from first array in record. Recall the warning in the docstrings
             # of this function.
             parameters.tensor_type = record[key].stype
 
         if not keep_input:
@@ -99,14 +102,18 @@
             tensor = parameters.tensors[idx]
         else:
             tensor = parameters.tensors.pop(0)
         ordered_dict[str(idx)] = Array(
             data=tensor, dtype="", stype=tensor_type, shape=[]
         )
 
+    if num_arrays == 0:
+        ordered_dict[EMPTY_TENSOR_KEY] = Array(
+            data=b"", dtype="", stype=tensor_type, shape=[]
+        )
     return ParametersRecord(ordered_dict, keep_input=keep_input)
 
 
 def _check_mapping_from_recordscalartype_to_scalar(
     record_data: Mapping[str, Union[ConfigsRecordValues, MetricsRecordValues]]
 ) -> Dict[str, Scalar]:
     """Check mapping `common.*RecordValues` into `common.Scalar` is possible."""
```

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/common/retry_invoker.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/retry_invoker.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/common/secure_aggregation/__init__.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/secure_aggregation/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/common/secure_aggregation/crypto/__init__.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/secure_aggregation/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/common/secure_aggregation/crypto/shamir.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/secure_aggregation/crypto/shamir.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/common/secure_aggregation/crypto/symmetric_encryption.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/secure_aggregation/crypto/symmetric_encryption.py`

 * *Files 18% similar despite different names*

```diff
@@ -113,22 +113,7 @@
     computed_hmac = hmac.HMAC(key, hashes.SHA256())
     computed_hmac.update(message)
     try:
         computed_hmac.verify(hmac_value)
         return True
     except InvalidSignature:
         return False
-
-
-def ssh_types_to_elliptic_curve(
-    private_key: serialization.SSHPrivateKeyTypes,
-    public_key: serialization.SSHPublicKeyTypes,
-) -> Tuple[ec.EllipticCurvePrivateKey, ec.EllipticCurvePublicKey]:
-    """Cast SSH key types to elliptic curve."""
-    if isinstance(private_key, ec.EllipticCurvePrivateKey) and isinstance(
-        public_key, ec.EllipticCurvePublicKey
-    ):
-        return (private_key, public_key)
-
-    raise TypeError(
-        "The provided key is not an EllipticCurvePrivateKey or EllipticCurvePublicKey"
-    )
```

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/common/secure_aggregation/ndarrays_arithmetic.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/secure_aggregation/ndarrays_arithmetic.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/common/secure_aggregation/quantization.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/secure_aggregation/quantization.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/common/secure_aggregation/secaggplus_constants.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/secure_aggregation/secaggplus_constants.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/common/secure_aggregation/secaggplus_utils.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/secure_aggregation/secaggplus_utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/common/serde.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/serde.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/common/telemetry.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/telemetry.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/common/typing.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/typing.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/common/version.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/version.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/proto/__init__.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/proto/driver_pb2.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/driver_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/proto/driver_pb2.pyi` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/driver_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/proto/driver_pb2_grpc.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/driver_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/proto/driver_pb2_grpc.pyi` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/driver_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/proto/error_pb2.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/error_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/proto/error_pb2.pyi` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/error_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/proto/fleet_pb2.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/fleet_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/proto/fleet_pb2.pyi` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/fleet_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/proto/fleet_pb2_grpc.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/fleet_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/proto/fleet_pb2_grpc.pyi` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/fleet_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/proto/node_pb2.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/node_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/proto/node_pb2.pyi` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/node_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/proto/recordset_pb2.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/recordset_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/proto/recordset_pb2.pyi` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/recordset_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/proto/task_pb2.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/task_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/proto/task_pb2.pyi` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/task_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/proto/transport_pb2.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/transport_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/proto/transport_pb2.pyi` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/transport_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/proto/transport_pb2_grpc.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/transport_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/proto/transport_pb2_grpc.pyi` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/transport_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/__init__.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/app.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 import threading
 from logging import ERROR, INFO, WARN
 from os.path import isfile
 from pathlib import Path
 from typing import List, Optional, Sequence, Set, Tuple
 
 import grpc
+from cryptography.exceptions import UnsupportedAlgorithm
 from cryptography.hazmat.primitives.asymmetric import ec
 from cryptography.hazmat.primitives.serialization import (
     load_ssh_private_key,
     load_ssh_public_key,
 )
 
 from flwr.common import GRPC_MAX_MESSAGE_LENGTH, EventType, event
@@ -41,15 +42,14 @@
     TRANSPORT_TYPE_VCE,
 )
 from flwr.common.exit_handlers import register_exit_handlers
 from flwr.common.logger import log, warn_deprecated_feature
 from flwr.common.secure_aggregation.crypto.symmetric_encryption import (
     private_key_to_bytes,
     public_key_to_bytes,
-    ssh_types_to_elliptic_curve,
 )
 from flwr.proto.fleet_pb2_grpc import (  # pylint: disable=E0611
     add_FleetServicer_to_server,
 )
 
 from .client_manager import ClientManager
 from .history import History
@@ -431,71 +431,96 @@
         driver_server.wait_for_termination(timeout=1)
 
 
 def _try_setup_client_authentication(
     args: argparse.Namespace,
     certificates: Optional[Tuple[bytes, bytes, bytes]],
 ) -> Optional[Tuple[Set[bytes], ec.EllipticCurvePrivateKey, ec.EllipticCurvePublicKey]]:
-    if not args.require_client_authentication:
+    if (
+        not args.auth_list_public_keys
+        and not args.auth_superlink_private_key
+        and not args.auth_superlink_public_key
+    ):
         return None
 
+    if (
+        not args.auth_list_public_keys
+        or not args.auth_superlink_private_key
+        or not args.auth_superlink_public_key
+    ):
+        sys.exit(
+            "Authentication requires providing file paths for "
+            "'--auth-list-public-keys', '--auth-superlink-private-key' and "
+            "'--auth-superlink-public-key'. Provide all three to enable authentication."
+        )
+
     if certificates is None:
         sys.exit(
-            "Client authentication only works over secure connections. "
-            "Please provide certificate paths using '--certificates' when "
-            "enabling '--require-client-authentication'."
+            "Authentication requires secure connections. "
+            "Please provide certificate paths using '--certificates' and "
+            "try again."
         )
 
-    client_keys_file_path = Path(args.require_client_authentication[0])
+    client_keys_file_path = Path(args.auth_list_public_keys)
     if not client_keys_file_path.exists():
         sys.exit(
-            "The provided path to the client public keys CSV file does not exist: "
+            "The provided path to the known public keys CSV file does not exist: "
             f"{client_keys_file_path}. "
-            "Please provide the CSV file path containing known client public keys "
-            "to '--require-client-authentication'."
+            "Please provide the CSV file path containing known public keys "
+            "to '--auth-list-public-keys'."
         )
 
     client_public_keys: Set[bytes] = set()
-    ssh_private_key = load_ssh_private_key(
-        Path(args.require_client_authentication[1]).read_bytes(),
-        None,
-    )
-    ssh_public_key = load_ssh_public_key(
-        Path(args.require_client_authentication[2]).read_bytes()
-    )
 
     try:
-        server_private_key, server_public_key = ssh_types_to_elliptic_curve(
-            ssh_private_key, ssh_public_key
+        ssh_private_key = load_ssh_private_key(
+            Path(args.auth_superlink_private_key).read_bytes(),
+            None,
+        )
+        if not isinstance(ssh_private_key, ec.EllipticCurvePrivateKey):
+            raise ValueError()
+    except (ValueError, UnsupportedAlgorithm):
+        sys.exit(
+            "Error: Unable to parse the private key file in "
+            "'--auth-superlink-private-key'. Authentication requires elliptic "
+            "curve private and public key pair. Please ensure that the file "
+            "path points to a valid private key file and try again."
+        )
+
+    try:
+        ssh_public_key = load_ssh_public_key(
+            Path(args.auth_superlink_public_key).read_bytes()
         )
-    except TypeError:
+        if not isinstance(ssh_public_key, ec.EllipticCurvePublicKey):
+            raise ValueError()
+    except (ValueError, UnsupportedAlgorithm):
         sys.exit(
-            "The file paths provided could not be read as a private and public "
-            "key pair. Client authentication requires an elliptic curve public and "
-            "private key pair. Please provide the file paths containing elliptic "
-            "curve private and public keys to '--require-client-authentication'."
+            "Error: Unable to parse the public key file in "
+            "'--auth-superlink-public-key'. Authentication requires elliptic "
+            "curve private and public key pair. Please ensure that the file "
+            "path points to a valid public key file and try again."
         )
 
     with open(client_keys_file_path, newline="", encoding="utf-8") as csvfile:
         reader = csv.reader(csvfile)
         for row in reader:
             for element in row:
                 public_key = load_ssh_public_key(element.encode())
                 if isinstance(public_key, ec.EllipticCurvePublicKey):
                     client_public_keys.add(public_key_to_bytes(public_key))
                 else:
                     sys.exit(
-                        "Error: Unable to parse the public keys in the .csv "
-                        "file. Please ensure that the .csv file contains valid "
-                        "SSH public keys and try again."
+                        "Error: Unable to parse the public keys in the CSV "
+                        "file. Please ensure that the CSV file path points to a valid "
+                        "known SSH public keys files and try again."
                     )
         return (
             client_public_keys,
-            server_private_key,
-            server_public_key,
+            ssh_private_key,
+            ssh_public_key,
         )
 
 
 def _try_obtain_certificates(
     args: argparse.Namespace,
 ) -> Optional[Tuple[bytes, bytes, bytes]]:
     # Obtain certificates
@@ -710,21 +735,28 @@
         "file that will be opened. Note that passing ':memory:' "
         "will open a connection to a database that is in RAM, "
         "instead of on disk. If nothing is provided, "
         "Flower will just create a state in memory.",
         default=DATABASE,
     )
     parser.add_argument(
-        "--require-client-authentication",
-        nargs=3,
-        metavar=("CLIENT_KEYS", "SERVER_PRIVATE_KEY", "SERVER_PUBLIC_KEY"),
+        "--auth-list-public-keys",
+        type=str,
+        help="A CSV file (as a path str) containing a list of known public "
+        "keys to enable authentication.",
+    )
+    parser.add_argument(
+        "--auth-superlink-private-key",
+        type=str,
+        help="The SuperLink's private key (as a path str) to enable authentication.",
+    )
+    parser.add_argument(
+        "--auth-superlink-public-key",
         type=str,
-        help="Provide three file paths: (1) a .csv file containing a list of "
-        "known client public keys for authentication, (2) the server's private "
-        "key file, and (3) the server's public key file.",
+        help="The SuperLink's public key (as a path str) to enable authentication.",
     )
 
 
 def _add_args_driver_api(parser: argparse.ArgumentParser) -> None:
     parser.add_argument(
         "--driver-api-address",
         help="Driver API (gRPC) server address (IPv4, IPv6, or a domain name)",
```

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/client_manager.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/client_manager.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/client_proxy.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/compat/__init__.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/compat/app.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/compat/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/compat/app_utils.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/compat/app_utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/compat/driver_client_proxy.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/compat/driver_client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/compat/legacy_context.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/compat/legacy_context.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/criterion.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/criterion.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/driver/__init__.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/driver/driver.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/driver/driver.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/driver/grpc_driver.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/driver/grpc_driver.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/driver/inmemory_driver.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/driver/inmemory_driver.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/history.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/history.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/run_serverapp.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/run_serverapp.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/server.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/server.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/server_app.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/server_app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/server_config.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/server_config.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/strategy/__init__.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/strategy/aggregate.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/aggregate.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/strategy/bulyan.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/bulyan.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/strategy/dp_adaptive_clipping.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/dp_adaptive_clipping.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/strategy/dp_fixed_clipping.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/dp_fixed_clipping.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/strategy/dpfedavg_adaptive.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/dpfedavg_adaptive.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/strategy/dpfedavg_fixed.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/dpfedavg_fixed.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/strategy/fault_tolerant_fedavg.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/fault_tolerant_fedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/strategy/fedadagrad.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/fedadagrad.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/strategy/fedadam.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/fedadam.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/strategy/fedavg.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/fedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/strategy/fedavg_android.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/fedavg_android.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/strategy/fedavgm.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/fedavgm.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/strategy/fedmedian.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/fedmedian.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/strategy/fedopt.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/fedopt.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/strategy/fedprox.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/fedprox.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/strategy/fedtrimmedavg.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/fedtrimmedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/strategy/fedxgb_bagging.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/fedxgb_bagging.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/strategy/fedxgb_cyclic.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/fedxgb_cyclic.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/strategy/fedxgb_nn_avg.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/fedxgb_nn_avg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/strategy/fedyogi.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/fedyogi.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/strategy/krum.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/krum.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/strategy/qfedavg.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/qfedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/strategy/strategy.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/strategy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/superlink/__init__.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/superlink/driver/__init__.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/superlink/driver/driver_grpc.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/driver/driver_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/superlink/driver/driver_servicer.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/driver/driver_servicer.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/superlink/fleet/__init__.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/fleet/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/superlink/fleet/grpc_bidi/__init__.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/fleet/grpc_bidi/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/superlink/fleet/grpc_bidi/flower_service_servicer.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/fleet/grpc_bidi/flower_service_servicer.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_bridge.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_bridge.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_client_proxy.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_server.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_server.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/superlink/fleet/grpc_rere/__init__.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/fleet/grpc_rere/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/superlink/fleet/grpc_rere/fleet_servicer.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/fleet/grpc_rere/fleet_servicer.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/superlink/fleet/grpc_rere/server_interceptor.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/fleet/grpc_rere/server_interceptor.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/superlink/fleet/message_handler/__init__.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/fleet/message_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/superlink/fleet/message_handler/message_handler.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/fleet/message_handler/message_handler.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/superlink/fleet/rest_rere/__init__.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/fleet/rest_rere/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/superlink/fleet/rest_rere/rest_api.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/fleet/rest_rere/rest_api.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/superlink/fleet/vce/__init__.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/fleet/vce/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/superlink/fleet/vce/backend/__init__.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/fleet/vce/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/superlink/fleet/vce/backend/backend.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/fleet/vce/backend/backend.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/superlink/fleet/vce/backend/raybackend.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/fleet/vce/backend/raybackend.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/superlink/fleet/vce/vce_api.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/fleet/vce/vce_api.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/superlink/state/__init__.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/state/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/superlink/state/in_memory_state.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/state/in_memory_state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/superlink/state/sqlite_state.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/state/sqlite_state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/superlink/state/state.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/state/state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/superlink/state/state_factory.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/state/state_factory.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/superlink/state/utils.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/state/utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/typing.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/typing.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/utils/__init__.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/utils/tensorboard.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/utils/tensorboard.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/utils/validator.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/utils/validator.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/workflow/__init__.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/workflow/constant.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/workflow/constant.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/workflow/default_workflows.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/workflow/default_workflows.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/workflow/secure_aggregation/__init__.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/workflow/secure_aggregation/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/workflow/secure_aggregation/secagg_workflow.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/workflow/secure_aggregation/secagg_workflow.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/server/workflow/secure_aggregation/secaggplus_workflow.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/workflow/secure_aggregation/secaggplus_workflow.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/simulation/__init__.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/simulation/app.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/simulation/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/simulation/ray_transport/__init__.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/simulation/ray_transport/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/simulation/ray_transport/ray_actor.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/simulation/ray_transport/ray_actor.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/simulation/ray_transport/ray_client_proxy.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/simulation/ray_transport/ray_client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/simulation/ray_transport/utils.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/simulation/ray_transport/utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/src/py/flwr/simulation/run_simulation.py` & `flwr_nightly-1.9.0.dev20240524/src/py/flwr/simulation/run_simulation.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240523/PKG-INFO` & `flwr_nightly-1.9.0.dev20240524/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flwr-nightly
-Version: 1.9.0.dev20240523
+Version: 1.9.0.dev20240524
 Summary: Flower: A Friendly Federated Learning Framework
 Home-page: https://flower.ai
 License: Apache-2.0
 Keywords: flower,fl,federated learning,federated analytics,federated evaluation,machine learning
 Author: The Flower Authors
 Author-email: hello@flower.ai
 Requires-Python: >=3.8,<4.0
@@ -35,17 +35,16 @@
 Requires-Dist: cryptography (>=42.0.4,<43.0.0)
 Requires-Dist: grpcio (>=1.60.0,<2.0.0)
 Requires-Dist: iterators (>=0.0.2,<0.0.3)
 Requires-Dist: numpy (>=1.21.0,<2.0.0)
 Requires-Dist: pathspec (>=0.12.1,<0.13.0)
 Requires-Dist: protobuf (>=4.25.2,<5.0.0)
 Requires-Dist: pycryptodome (>=3.18.0,<4.0.0)
-Requires-Dist: ray (==2.6.3) ; (python_version >= "3.8" and python_version < "3.12") and (extra == "simulation")
+Requires-Dist: ray (==2.10.0) ; (python_version >= "3.8" and python_version < "3.12") and (extra == "simulation")
 Requires-Dist: requests (>=2.31.0,<3.0.0) ; extra == "rest"
-Requires-Dist: setuptools (!=70.0.0)
 Requires-Dist: starlette (>=0.31.0,<0.32.0) ; extra == "rest"
 Requires-Dist: tomli (>=2.0.1,<3.0.0)
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
 Requires-Dist: uvicorn[standard] (>=0.23.0,<0.24.0) ; extra == "rest"
 Project-URL: Documentation, https://flower.ai
 Project-URL: Repository, https://github.com/adap/flower
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flwr-nightly Version: 1.9.0.dev20240523 Summary:
+Metadata-Version: 2.1 Name: flwr-nightly Version: 1.9.0.dev20240524 Summary:
 Flower: A Friendly Federated Learning Framework Home-page: https://flower.ai
 License: Apache-2.0 Keywords: flower,fl,federated learning,federated
 analytics,federated evaluation,machine learning Author: The Flower Authors
 Author-email: hello@flower.ai Requires-Python: >=3.8,<4.0 Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Operating System
@@ -18,23 +18,23 @@
 Engineering :: Mathematics Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries Classifier: Topic ::
 Software Development :: Libraries :: Python Modules Classifier: Typing :: Typed
 Provides-Extra: rest Provides-Extra: simulation Requires-Dist: cryptography
 (>=42.0.4,<43.0.0) Requires-Dist: grpcio (>=1.60.0,<2.0.0) Requires-Dist:
 iterators (>=0.0.2,<0.0.3) Requires-Dist: numpy (>=1.21.0,<2.0.0) Requires-
 Dist: pathspec (>=0.12.1,<0.13.0) Requires-Dist: protobuf (>=4.25.2,<5.0.0)
-Requires-Dist: pycryptodome (>=3.18.0,<4.0.0) Requires-Dist: ray (==2.6.3) ;
+Requires-Dist: pycryptodome (>=3.18.0,<4.0.0) Requires-Dist: ray (==2.10.0) ;
 (python_version >= "3.8" and python_version < "3.12") and (extra ==
 "simulation") Requires-Dist: requests (>=2.31.0,<3.0.0) ; extra == "rest"
-Requires-Dist: setuptools (!=70.0.0) Requires-Dist: starlette
-(>=0.31.0,<0.32.0) ; extra == "rest" Requires-Dist: tomli (>=2.0.1,<3.0.0)
-Requires-Dist: typer[all] (>=0.9.0,<0.10.0) Requires-Dist: uvicorn[standard]
-(>=0.23.0,<0.24.0) ; extra == "rest" Project-URL: Documentation, https://
-flower.ai Project-URL: Repository, https://github.com/adap/flower Description-
-Content-Type: text/markdown # Flower: A Friendly Federated Learning Framework
+Requires-Dist: starlette (>=0.31.0,<0.32.0) ; extra == "rest" Requires-Dist:
+tomli (>=2.0.1,<3.0.0) Requires-Dist: typer[all] (>=0.9.0,<0.10.0) Requires-
+Dist: uvicorn[standard] (>=0.23.0,<0.24.0) ; extra == "rest" Project-URL:
+Documentation, https://flower.ai Project-URL: Repository, https://github.com/
+adap/flower Description-Content-Type: text/markdown # Flower: A Friendly
+Federated Learning Framework
                                _[_F_l_o_w_e_r_ _W_e_b_s_i_t_e_]
                   _W_e_b_s_i_t_e | _B_l_o_g | _D_o_c_s | _C_o_n_f_e_r_e_n_c_e | _S_l_a_c_k
 
 [![GitHub license](https://img.shields.io/github/license/adap/flower)](https://
 github.com/adap/flower/blob/main/LICENSE) [![PRs Welcome](https://
 img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/adap/
 flower/blob/main/CONTRIBUTING.md) ![Build](https://github.com/adap/flower/
```

