# Comparing `tmp/mct-quantizers-nightly-1.5.0.20240523.post1117.tar.gz` & `tmp/mct-quantizers-nightly-1.5.0.20240524.post1127.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mct-quantizers-nightly-1.5.0.20240523.post1117.tar", last modified: Thu May 23 00:11:21 2024, max compression
+gzip compressed data, was "mct-quantizers-nightly-1.5.0.20240524.post1127.tar", last modified: Fri May 24 00:11:28 2024, max compression
```

## Comparing `mct-quantizers-nightly-1.5.0.20240523.post1117.tar` & `mct-quantizers-nightly-1.5.0.20240524.post1127.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:11:21.220130 mct-quantizers-nightly-1.5.0.20240523.post1117/
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-05-23 00:10:52.000000 mct-quantizers-nightly-1.5.0.20240523.post1117/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-05-23 00:11:21.220130 mct-quantizers-nightly-1.5.0.20240523.post1117/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-05-23 00:10:52.000000 mct-quantizers-nightly-1.5.0.20240523.post1117/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:11:21.208129 mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-05-23 00:10:52.000000 mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:11:21.212129 mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/common/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-23 00:10:52.000000 mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-05-23 00:10:52.000000 mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/common/base_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-05-23 00:10:52.000000 mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-23 00:10:52.000000 mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/common/get_all_subclasses.py
--rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-05-23 00:10:52.000000 mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/common/get_quantizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-05-23 00:10:52.000000 mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/common/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-23 00:10:52.000000 mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/common/quant_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-05-23 00:10:52.000000 mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/common/quant_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:11:21.212129 mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-23 00:10:52.000000 mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6815 2024-05-23 00:10:52.000000 mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/keras/activation_quantization_holder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4430 2024-05-23 00:10:52.000000 mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/keras/load_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-05-23 00:10:52.000000 mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/keras/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    21750 2024-05-23 00:10:52.000000 mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/keras/quantize_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-05-23 00:10:52.000000 mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/keras/quantizer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:11:21.212129 mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/keras/quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-05-23 00:10:52.000000 mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/keras/quantizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:11:21.212129 mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/keras/quantizers/activation_inferable_quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-23 00:10:52.000000 mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/keras/quantizers/activation_inferable_quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8576 2024-05-23 00:10:52.000000 mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-05-23 00:10:52.000000 mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-05-23 00:10:52.000000 mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5421 2024-05-23 00:10:52.000000 mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-05-23 00:10:52.000000 mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/keras/quantizers/base_keras_inferable_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:11:21.212129 mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/keras/quantizers/weights_inferable_quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-23 00:10:52.000000 mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/keras/quantizers/weights_inferable_quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4632 2024-05-23 00:10:52.000000 mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10743 2024-05-23 00:10:52.000000 mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3835 2024-05-23 00:10:52.000000 mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5027 2024-05-23 00:10:52.000000 mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9491 2024-05-23 00:10:52.000000 mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-05-23 00:10:52.000000 mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/keras/validation_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4809 2024-05-23 00:10:52.000000 mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:11:21.216129 mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-23 00:10:52.000000 mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-05-23 00:10:52.000000 mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/pytorch/activation_quantization_holder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-05-23 00:10:52.000000 mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/pytorch/load_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4680 2024-05-23 00:10:52.000000 mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/pytorch/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-05-23 00:10:52.000000 mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/pytorch/onnxruntime_session_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     3273 2024-05-23 00:10:52.000000 mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/pytorch/onnxruntime_validations.py
--rw-r--r--   0 runner    (1001) docker     (127)    14180 2024-05-23 00:10:52.000000 mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/pytorch/quantize_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     6816 2024-05-23 00:10:52.000000 mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/pytorch/quantizer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:11:21.216129 mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/pytorch/quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-23 00:10:52.000000 mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/pytorch/quantizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:11:21.216129 mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-23 00:10:52.000000 mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4401 2024-05-23 00:10:52.000000 mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7265 2024-05-23 00:10:52.000000 mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10019 2024-05-23 00:10:52.000000 mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11047 2024-05-23 00:10:52.000000 mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-23 00:10:52.000000 mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/base_activation_quantizer_autograd_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-05-23 00:10:52.000000 mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/pytorch/quantizers/base_lut_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-05-23 00:10:52.000000 mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/pytorch/quantizers/base_pytorch_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-05-23 00:10:52.000000 mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/pytorch/quantizers/base_quantizer_autograd_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-05-23 00:10:52.000000 mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/pytorch/quantizers/base_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-05-23 00:10:52.000000 mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/pytorch/quantizers/base_uniform_inferable_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:11:21.220130 mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-23 00:10:52.000000 mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-23 00:10:52.000000 mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/base_weight_quantizer_autograd_function.py
--rw-r--r--   0 runner    (1001) docker     (127)    10532 2024-05-23 00:10:52.000000 mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    12857 2024-05-23 00:10:52.000000 mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8359 2024-05-23 00:10:52.000000 mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    13106 2024-05-23 00:10:52.000000 mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    15290 2024-05-23 00:10:52.000000 mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:11:21.220130 mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-05-23 00:11:20.000000 mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4170 2024-05-23 00:11:21.000000 mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 00:11:20.000000 mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-23 00:11:20.000000 mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-23 00:11:20.000000 mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers_nightly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-23 00:11:21.220130 mct-quantizers-nightly-1.5.0.20240523.post1117/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-05-23 00:11:17.000000 mct-quantizers-nightly-1.5.0.20240523.post1117/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 00:11:28.752155 mct-quantizers-nightly-1.5.0.20240524.post1127/
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-05-24 00:11:15.000000 mct-quantizers-nightly-1.5.0.20240524.post1127/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-05-24 00:11:28.752155 mct-quantizers-nightly-1.5.0.20240524.post1127/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-05-24 00:11:15.000000 mct-quantizers-nightly-1.5.0.20240524.post1127/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 00:11:28.744155 mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-05-24 00:11:15.000000 mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 00:11:28.744155 mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-24 00:11:15.000000 mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-05-24 00:11:15.000000 mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/common/base_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-05-24 00:11:15.000000 mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-24 00:11:15.000000 mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/common/get_all_subclasses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-05-24 00:11:15.000000 mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/common/get_quantizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-05-24 00:11:15.000000 mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/common/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-24 00:11:15.000000 mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/common/quant_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-05-24 00:11:15.000000 mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/common/quant_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 00:11:28.748155 mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-24 00:11:15.000000 mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6815 2024-05-24 00:11:15.000000 mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/keras/activation_quantization_holder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4430 2024-05-24 00:11:15.000000 mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/keras/load_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-05-24 00:11:15.000000 mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/keras/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21750 2024-05-24 00:11:15.000000 mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/keras/quantize_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-05-24 00:11:15.000000 mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/keras/quantizer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 00:11:28.748155 mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/keras/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-05-24 00:11:15.000000 mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/keras/quantizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 00:11:28.748155 mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/keras/quantizers/activation_inferable_quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-24 00:11:15.000000 mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/keras/quantizers/activation_inferable_quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8576 2024-05-24 00:11:15.000000 mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-05-24 00:11:15.000000 mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-05-24 00:11:15.000000 mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5421 2024-05-24 00:11:15.000000 mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-05-24 00:11:15.000000 mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/keras/quantizers/base_keras_inferable_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 00:11:28.748155 mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/keras/quantizers/weights_inferable_quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-24 00:11:15.000000 mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/keras/quantizers/weights_inferable_quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4632 2024-05-24 00:11:15.000000 mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10743 2024-05-24 00:11:15.000000 mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3835 2024-05-24 00:11:15.000000 mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5027 2024-05-24 00:11:15.000000 mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9491 2024-05-24 00:11:15.000000 mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-05-24 00:11:15.000000 mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/keras/validation_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4809 2024-05-24 00:11:15.000000 mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 00:11:28.748155 mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-24 00:11:15.000000 mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-05-24 00:11:15.000000 mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/pytorch/activation_quantization_holder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-05-24 00:11:15.000000 mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/pytorch/load_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4680 2024-05-24 00:11:15.000000 mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/pytorch/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-05-24 00:11:15.000000 mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/pytorch/onnxruntime_session_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3273 2024-05-24 00:11:15.000000 mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/pytorch/onnxruntime_validations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14180 2024-05-24 00:11:15.000000 mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/pytorch/quantize_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6816 2024-05-24 00:11:15.000000 mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/pytorch/quantizer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 00:11:28.752155 mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/pytorch/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-24 00:11:15.000000 mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/pytorch/quantizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 00:11:28.752155 mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-24 00:11:15.000000 mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4401 2024-05-24 00:11:15.000000 mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7265 2024-05-24 00:11:15.000000 mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10019 2024-05-24 00:11:15.000000 mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11047 2024-05-24 00:11:15.000000 mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-24 00:11:15.000000 mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/base_activation_quantizer_autograd_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-05-24 00:11:15.000000 mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/pytorch/quantizers/base_lut_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-05-24 00:11:15.000000 mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/pytorch/quantizers/base_pytorch_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-05-24 00:11:15.000000 mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/pytorch/quantizers/base_quantizer_autograd_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-05-24 00:11:15.000000 mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/pytorch/quantizers/base_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-05-24 00:11:15.000000 mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/pytorch/quantizers/base_uniform_inferable_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 00:11:28.752155 mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-24 00:11:15.000000 mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-24 00:11:15.000000 mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/base_weight_quantizer_autograd_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10532 2024-05-24 00:11:15.000000 mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12857 2024-05-24 00:11:15.000000 mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8359 2024-05-24 00:11:15.000000 mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13106 2024-05-24 00:11:15.000000 mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15290 2024-05-24 00:11:15.000000 mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 00:11:28.752155 mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-05-24 00:11:28.000000 mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4170 2024-05-24 00:11:28.000000 mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 00:11:28.000000 mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-24 00:11:28.000000 mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-24 00:11:28.000000 mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers_nightly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-24 00:11:28.752155 mct-quantizers-nightly-1.5.0.20240524.post1127/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-05-24 00:11:27.000000 mct-quantizers-nightly-1.5.0.20240524.post1127/setup.py
```

### Comparing `mct-quantizers-nightly-1.5.0.20240523.post1117/LICENSE.md` & `mct-quantizers-nightly-1.5.0.20240524.post1127/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.5.0.20240523.post1117/PKG-INFO` & `mct-quantizers-nightly-1.5.0.20240524.post1127/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mct-quantizers-nightly
-Version: 1.5.0.20240523.post1117
+Version: 1.5.0.20240524.post1127
 Summary: Infrastructure for support neural networks compression
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: # Model Compression Toolkit (MCT) Quantizers
         
         The MCT Quantizers library is an open-source library developed by researchers and engineers working at Sony Semiconductor Israel.
```

### Comparing `mct-quantizers-nightly-1.5.0.20240523.post1117/README.md` & `mct-quantizers-nightly-1.5.0.20240524.post1127/README.md`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/__init__.py` & `mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/common/__init__.py` & `mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/common/base_inferable_quantizer.py` & `mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/common/base_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/common/constants.py` & `mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/common/constants.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/common/get_all_subclasses.py` & `mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/common/get_all_subclasses.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/common/get_quantizers.py` & `mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/common/get_quantizers.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/common/metadata.py` & `mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/common/metadata.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/common/quant_info.py` & `mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/common/quant_info.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/common/quant_utils.py` & `mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/common/quant_utils.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/keras/__init__.py` & `mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/keras/activation_quantization_holder.py` & `mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/keras/activation_quantization_holder.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/keras/load_model.py` & `mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/keras/load_model.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/keras/metadata.py` & `mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/keras/metadata.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/keras/quantize_wrapper.py` & `mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/keras/quantize_wrapper.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/keras/quantizer_utils.py` & `mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/keras/quantizer_utils.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/keras/quantizers/__init__.py` & `mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/keras/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/keras/quantizers/activation_inferable_quantizers/__init__.py` & `mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/keras/quantizers/activation_inferable_quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py` & `mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py` & `mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py` & `mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py` & `mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/keras/quantizers/base_keras_inferable_quantizer.py` & `mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/keras/quantizers/base_keras_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/keras/quantizers/weights_inferable_quantizers/__init__.py` & `mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/keras/quantizers/weights_inferable_quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py` & `mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py` & `mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py` & `mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py` & `mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py` & `mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/keras/validation_functions.py` & `mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/keras/validation_functions.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/logger.py` & `mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/logger.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/pytorch/__init__.py` & `mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/pytorch/activation_quantization_holder.py` & `mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/pytorch/activation_quantization_holder.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/pytorch/load_model.py` & `mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/pytorch/load_model.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/pytorch/metadata.py` & `mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/pytorch/metadata.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/pytorch/onnxruntime_session_options.py` & `mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/pytorch/onnxruntime_session_options.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/pytorch/onnxruntime_validations.py` & `mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/pytorch/onnxruntime_validations.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/pytorch/quantize_wrapper.py` & `mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/pytorch/quantize_wrapper.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/pytorch/quantizer_utils.py` & `mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/pytorch/quantizer_utils.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/pytorch/quantizers/__init__.py` & `mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/pytorch/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/__init__.py` & `mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py` & `mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py` & `mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py` & `mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py` & `mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/base_activation_quantizer_autograd_function.py` & `mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/base_activation_quantizer_autograd_function.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/pytorch/quantizers/base_lut_symmetric_inferable_quantizer.py` & `mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/pytorch/quantizers/base_lut_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/pytorch/quantizers/base_pytorch_inferable_quantizer.py` & `mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/pytorch/quantizers/base_pytorch_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/pytorch/quantizers/base_quantizer_autograd_function.py` & `mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/pytorch/quantizers/base_quantizer_autograd_function.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/pytorch/quantizers/base_symmetric_inferable_quantizer.py` & `mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/pytorch/quantizers/base_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/pytorch/quantizers/base_uniform_inferable_quantizer.py` & `mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/pytorch/quantizers/base_uniform_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/__init__.py` & `mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/base_weight_quantizer_autograd_function.py` & `mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/base_weight_quantizer_autograd_function.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py` & `mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py` & `mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py` & `mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py` & `mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py` & `mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers_nightly.egg-info/PKG-INFO` & `mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mct-quantizers-nightly
-Version: 1.5.0.20240523.post1117
+Version: 1.5.0.20240524.post1127
 Summary: Infrastructure for support neural networks compression
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: # Model Compression Toolkit (MCT) Quantizers
         
         The MCT Quantizers library is an open-source library developed by researchers and engineers working at Sony Semiconductor Israel.
```

### Comparing `mct-quantizers-nightly-1.5.0.20240523.post1117/mct_quantizers_nightly.egg-info/SOURCES.txt` & `mct-quantizers-nightly-1.5.0.20240524.post1127/mct_quantizers_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.5.0.20240523.post1117/setup.py` & `mct-quantizers-nightly-1.5.0.20240524.post1127/setup.py`

 * *Files identical despite different names*

